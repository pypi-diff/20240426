# Comparing `tmp/rlsdk_python-0.2.2.tar.gz` & `tmp/rlsdk_python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlsdk_python-0.2.2.tar", max compression
+gzip compressed data, was "rlsdk_python-0.3.0.tar", max compression
```

## Comparing `rlsdk_python-0.2.2.tar` & `rlsdk_python-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      318 2024-04-23 15:41:21.873182 rlsdk_python-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1640 2024-04-21 20:56:20.206780 rlsdk_python-0.2.2/README.md
--rw-r--r--   0        0        0      107 2024-04-16 11:12:58.877877 rlsdk_python-0.2.2/rlsdk_python/__init__.py
--rw-r--r--   0        0        0     1812 2024-04-18 23:00:20.787805 rlsdk_python-0.2.2/rlsdk_python/event_handling.py
--rw-r--r--   0        0        0     1814 2024-04-18 21:23:06.061748 rlsdk_python-0.2.2/rlsdk_python/events.py
--rw-r--r--   0        0        0     4038 2024-04-17 01:30:35.234518 rlsdk_python-0.2.2/rlsdk_python/frida_script.py
--rw-r--r--   0        0        0    42303 2024-04-23 15:40:30.849073 rlsdk_python-0.2.2/rlsdk_python/game_objects.py
--rw-r--r--   0        0        0    17791 2024-04-23 15:00:21.419337 rlsdk_python-0.2.2/rlsdk_python/sdk.py
--rw-r--r--   0        0        0     1982 1970-01-01 00:00:00.000000 rlsdk_python-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      357 2024-04-26 19:59:33.045916 rlsdk_python-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1640 2024-04-21 20:56:20.206780 rlsdk_python-0.3.0/README.md
+-rw-r--r--   0        0        0      107 2024-04-16 11:12:58.877877 rlsdk_python-0.3.0/rlsdk_python/__init__.py
+-rw-r--r--   0        0        0     1812 2024-04-18 23:00:20.787805 rlsdk_python-0.3.0/rlsdk_python/event_handling.py
+-rw-r--r--   0        0        0     1814 2024-04-18 21:23:06.061748 rlsdk_python-0.3.0/rlsdk_python/events.py
+-rw-r--r--   0        0        0     4065 2024-04-26 18:56:51.985326 rlsdk_python-0.3.0/rlsdk_python/frida_script.py
+-rw-r--r--   0        0        0    30557 2024-04-26 15:34:23.035361 rlsdk_python-0.3.0/rlsdk_python/game_objects.py
+-rw-r--r--   0        0        0    21779 2024-04-26 19:56:52.007905 rlsdk_python-0.3.0/rlsdk_python/sdk.py
+-rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 rlsdk_python-0.3.0/PKG-INFO
```

### Comparing `rlsdk_python-0.2.2/README.md` & `rlsdk_python-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `rlsdk_python-0.2.2/rlsdk_python/event_handling.py` & `rlsdk_python-0.3.0/rlsdk_python/event_handling.py`

 * *Files identical despite different names*

### Comparing `rlsdk_python-0.2.2/rlsdk_python/events.py` & `rlsdk_python-0.3.0/rlsdk_python/events.py`

 * *Files identical despite different names*

### Comparing `rlsdk_python-0.2.2/rlsdk_python/frida_script.py` & `rlsdk_python-0.3.0/rlsdk_python/frida_script.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 frida_script = """
-console.log("Frida script started");
+
+
+function log(message) {
+    send({type: "log", message: message});
+}
+
+log("Frida script started");
 
 const hooked_functions = new Map();
 const hooked_functions_args_map = new Map();
 const discovered_functions = new Map();
 let scan_active = false;
 
-
 // Receive message
 
 recv('process_event_address', function onMessage(payload) {
-    console.log("Received ProcessEvent Address: 0x" + payload.address.toString(16));
+    log("Received ProcessEvent Address: 0x" + payload.address.toString(16));
 
 
     Interceptor.attach(ptr(payload.address), {
         onEnter: function(args) {
            
             // Le deuxième argument est le pointeur vers UFunction
             const uFunction = args[1];
@@ -65,15 +70,15 @@
                             for (let i = 0; i < bytes.length; i++) {
                                 let byte = bytes[i];
                                 let hex = byte.toString(16);
                                 hexString += (hex.length === 1 ? '0' : '') + hex;
                             }
                             casted_args[name] = hexString;
                         } else {
-                            console.error('Buffer is null');
+                            error('Buffer is null');
                         }
                     } else {
                         casted_args[name] = args[index];
                     }
                     
                 });
 
@@ -91,15 +96,15 @@
     });
 });
 
 
 recv('scan_functions', function onMessage(payload) {
     const duration = payload.duration;
     
-    console.log("Start scanning functions for " + duration + " seconds");
+    log("Start scanning functions for " + duration + " seconds");
 
     scan_active = true;
     // empty discovered functions
     discovered_functions.clear();
 
     setTimeout(function() {
         scan_active = false;
@@ -114,19 +119,16 @@
 
 
 recv('hook_function', function onMessage(payload) {
 
     hooked_functions.set(payload.address.toString(16), payload.name);
     hooked_functions_args_map.set(payload.address.toString(16), payload.args_map);
 
-    console.log("Received Hook Function: 0x" + payload.address.toString(16) + " " + payload.name);
+    log("Start hook function: 0x" + payload.address.toString(16) + " " + payload.name);
 
     recv('hook_function', onMessage);
 });
 
-
-
-
 """
```

### Comparing `rlsdk_python-0.2.2/PKG-INFO` & `rlsdk_python-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: rlsdk_python
-Version: 0.2.2
+Version: 0.3.0
 Summary: 
 Author: MarlburroW
 Author-email: nik0o@hotmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Pymem (>=1.13.1,<2.0.0)
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: frida (>=16.2.1,<17.0.0)
+Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # RLSDK Python
 
 This is reverse engineered python SDK package aiming to read data from RocketLeague.exe.
 
 ## How does it works
```

