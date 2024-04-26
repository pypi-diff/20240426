# Comparing `tmp/ugot_broadcast_message-0.0.1.tar.gz` & `tmp/ugot_broadcast_message-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ugot_broadcast_message-0.0.1.tar", last modified: Tue Apr 16 08:52:26 2024, max compression
+gzip compressed data, was "ugot_broadcast_message-0.0.2.tar", last modified: Fri Apr 26 07:10:05 2024, max compression
```

## Comparing `ugot_broadcast_message-0.0.1.tar` & `ugot_broadcast_message-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 08:52:26.082640 ugot_broadcast_message-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-04-16 08:49:42.000000 ugot_broadcast_message-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1051 2024-04-16 08:52:26.082640 ugot_broadcast_message-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       37 2024-04-16 08:46:39.000000 ugot_broadcast_message-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-16 08:52:26.083640 ugot_broadcast_message-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1205 2024-04-16 08:52:07.000000 ugot_broadcast_message-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:52:26.081639 ugot_broadcast_message-0.0.1/uGot_Broadcast_message.egg-info/
--rw-rw-rw-   0        0        0     1051 2024-04-16 08:52:26.000000 ugot_broadcast_message-0.0.1/uGot_Broadcast_message.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2024-04-16 08:52:26.000000 ugot_broadcast_message-0.0.1/uGot_Broadcast_message.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 08:52:26.000000 ugot_broadcast_message-0.0.1/uGot_Broadcast_message.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-16 08:52:26.000000 ugot_broadcast_message-0.0.1/uGot_Broadcast_message.egg-info/requires.txt
--rw-rw-rw-   0        0        0       50 2024-04-16 08:52:26.000000 ugot_broadcast_message-0.0.1/uGot_Broadcast_message.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7158 2024-04-16 08:20:07.000000 ugot_broadcast_message-0.0.1/ugot_broadcast_message.py
--rw-rw-rw-   0        0        0     1800 2024-03-29 03:15:43.000000 ugot_broadcast_message-0.0.1/ugot_broadcast_message_pb2.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:10:05.254380 ugot_broadcast_message-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-16 08:49:42.000000 ugot_broadcast_message-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1141 2024-04-26 07:10:05.253380 ugot_broadcast_message-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2024-04-16 08:46:39.000000 ugot_broadcast_message-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 07:10:05.255381 ugot_broadcast_message-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1457 2024-04-26 07:07:55.000000 ugot_broadcast_message-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:10:05.252408 ugot_broadcast_message-0.0.2/uGot_Broadcast_message.egg-info/
+-rw-rw-rw-   0        0        0     1141 2024-04-26 07:10:05.000000 ugot_broadcast_message-0.0.2/uGot_Broadcast_message.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2024-04-26 07:10:05.000000 ugot_broadcast_message-0.0.2/uGot_Broadcast_message.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 07:10:05.000000 ugot_broadcast_message-0.0.2/uGot_Broadcast_message.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-26 07:10:05.000000 ugot_broadcast_message-0.0.2/uGot_Broadcast_message.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      177 2024-04-26 07:10:05.000000 ugot_broadcast_message-0.0.2/uGot_Broadcast_message.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7409 2024-04-26 06:57:41.000000 ugot_broadcast_message-0.0.2/ugot_broadcast_message.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:10:05.250389 ugot_broadcast_message-0.0.2/ugot_broadcast_message_pb2/
+-rw-rw-rw-   0        0        0      833 2024-04-26 06:55:35.000000 ugot_broadcast_message-0.0.2/ugot_broadcast_message_pb2/__init__.py
+-rw-rw-rw-   0        0        0     8708 2024-04-26 06:03:22.000000 ugot_broadcast_message-0.0.2/ugot_broadcast_message_pb2/ugot_broadcast_message_pb2_gen1.py
+-rw-rw-rw-   0        0        0     1800 2024-03-29 03:15:43.000000 ugot_broadcast_message-0.0.2/ugot_broadcast_message_pb2/ugot_broadcast_message_pb2_gen2.py
```

### Comparing `ugot_broadcast_message-0.0.1/LICENSE` & `ugot_broadcast_message-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ugot_broadcast_message-0.0.1/PKG-INFO` & `ugot_broadcast_message-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: uGot_Broadcast_message
-Version: 0.0.1
+Version: 0.0.2
 Summary: =A broadcast communication Python Library for uGot
 Home-page: https://github.com/naOKiGor/Python_ugot_broadcast_message
 Author: naOKiGor
 Author-email: evenaoki@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: protobuf>=5.26.1
+Requires-Dist: protobuf
+Requires-Dist: psutil
 
 uGot_Broadcast_message Python library
```

### Comparing `ugot_broadcast_message-0.0.1/setup.py` & `ugot_broadcast_message-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 from setuptools import setup
 
 setup(
     name='uGot_Broadcast_message',
-    version='0.0.1',
+    version='0.0.2',
     description='=A broadcast communication Python Library for uGot',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="MIT",
-    py_modules=['ugot_broadcast_message', 'ugot_broadcast_message_pb2'],
+    py_modules=[
+        'ugot_broadcast_message',
+        'ugot_broadcast_message_pb2/__init__',
+        'ugot_broadcast_message_pb2/ugot_broadcast_message_pb2_gen1',
+        'ugot_broadcast_message_pb2/ugot_broadcast_message_pb2_gen2'],
     author='naOKiGor',
     author_email='evenaoki@gmail.com',
     url='https://github.com/naOKiGor/Python_ugot_broadcast_message',
-    install_requires=['protobuf>=5.26.1'],
+    install_requires=['protobuf', 'psutil'],
+    python_requires=">=3.5",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
```

### Comparing `ugot_broadcast_message-0.0.1/uGot_Broadcast_message.egg-info/PKG-INFO` & `ugot_broadcast_message-0.0.2/uGot_Broadcast_message.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: uGot_Broadcast_message
-Version: 0.0.1
+Version: 0.0.2
 Summary: =A broadcast communication Python Library for uGot
 Home-page: https://github.com/naOKiGor/Python_ugot_broadcast_message
 Author: naOKiGor
 Author-email: evenaoki@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: protobuf>=5.26.1
+Requires-Dist: protobuf
+Requires-Dist: psutil
 
 uGot_Broadcast_message Python library
```

### Comparing `ugot_broadcast_message-0.0.1/ugot_broadcast_message.py` & `ugot_broadcast_message-0.0.2/ugot_broadcast_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import socket
 from io import BytesIO
 from typing import Optional
 import time
 import threading
+import psutil
+import re
 
 from ugot_broadcast_message_pb2 import broadcast_message_header, broadcast_message_payload
 
 DEFAULT_CHANNEL_ID = 0
 DEFAULT_BIND_HOST = '0.0.0.0'
 DEFAULT_BROADCAST_ADDRESS = '255.255.255.255'
 
@@ -56,15 +58,15 @@
         self.recv_sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         self.recv_sock.bind((DEFAULT_BIND_HOST if self.bind_host is None else self.bind_host, self.get_port()))
 
         def receive_loop():
             while self.enable:
                 try:
                     valid, message_content = self.__receive_message_impl__()
-                    if self.callback is not None:
+                    if valid and self.callback is not None:
                         self.callback(message_content)
                 except:
                     pass
 
         threading.Thread(target=receive_loop, daemon=True).start()
 
     def __release_udp__(self):
@@ -130,14 +132,17 @@
 
     def send_broadcast_message(self, message_value: str):
         self.__send_broadcast_message_impl__(message_value)
 
     def send_message_to(self, message_value: str, address: Optional[str]):
         self.__send_broadcast_message_impl__(message_value, address)
 
+    def __is_valid_ip_addr__(self, addr: str):
+        return re.match(r'(\d|[1-9]\d|1\d{2}|2[0-4]\d|25[0-5])(\.(\d|[1-9]\d|1\d{2}|2[0-4]\d|25[0-5])){3}', addr) is not None
+
     def __send_broadcast_message_impl__(self, message_value: str, address: Optional[str] = None):
         """Send communication message
         :param message_value: message content
         :param address: target address. Default: None, broadcast to 255.255.255.255
         """
         if not self.enable:
             return
@@ -160,16 +165,15 @@
         message.write(header_bytes)
         message.write(bytes([self.__crc_sum__(header_bytes)]))
         message.write(payload_bytes)
         message.write(bytes([self.__crc_sum__(payload_bytes)]))
         message_bytes = message.getvalue()
 
         if self.bind_host is None:
-            interfaces = socket.getaddrinfo(host=socket.gethostname(), port=None, family=socket.AF_INET)
-            broadcast_interfaces = set([ip[-1][0] for ip in interfaces])
+            broadcast_interfaces = set([item.address for value in psutil.net_if_addrs().values() for item in value if self.__is_valid_ip_addr__(item.address)])
         else:
             broadcast_interfaces = [self.bind_host]
 
         # Remove loopback interface
         if '127.0.0.1' in broadcast_interfaces:
             broadcast_interfaces.remove('127.0.0.1')
 
@@ -187,18 +191,20 @@
                 sock.sendto(message_bytes, broadcast_address)
                 sock.close()
             except:
                 pass
 
 
 if __name__ == '__main__':
+    from ugot_broadcast_message import ugot_broadcast_channel
+
     channel = ugot_broadcast_channel()
 
     # Optional set communication channel, default is 0
-    # channel.set_channel(0)
+    channel.set_channel(0)
 
     # Enable broadcast function, default is off
     channel.set_enable(True)
 
     # Set message received callback #1: use lambda
     channel.set_message_received_callback(lambda message_content: print(message_content))
```

### Comparing `ugot_broadcast_message-0.0.1/ugot_broadcast_message_pb2.py` & `ugot_broadcast_message-0.0.2/ugot_broadcast_message_pb2/ugot_broadcast_message_pb2_gen2.py`

 * *Files identical despite different names*

