# Comparing `tmp/eva4-controller-py-0.1.3.tar.gz` & `tmp/eva4-controller-py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eva4-controller-py-0.1.3.tar", last modified: Mon Feb 19 22:18:55 2024, max compression
+gzip compressed data, was "eva4-controller-py-0.1.4.tar", last modified: Thu Apr 25 22:40:00 2024, max compression
```

## Comparing `eva4-controller-py-0.1.3.tar` & `eva4-controller-py-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-02-19 22:18:55.672215 eva4-controller-py-0.1.3/
--rw-r--r--   0 divisor   (1000) root         (0)    10644 2023-11-19 23:00:18.000000 eva4-controller-py-0.1.3/LICENSE
--rw-r--r--   0 divisor   (1000) root         (0)      521 2024-02-19 22:18:55.672215 eva4-controller-py-0.1.3/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)       46 2022-04-01 21:38:20.000000 eva4-controller-py-0.1.3/README.md
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-02-19 22:18:55.672215 eva4-controller-py-0.1.3/bin/
--rwxr-xr-x   0 divisor   (1000) root         (0)       75 2022-04-01 21:42:50.000000 eva4-controller-py-0.1.3/bin/eva4-svc-controller-py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-02-19 22:18:55.672215 eva4-controller-py-0.1.3/eva4_controller_py/
--rw-r--r--   0 divisor   (1000) root         (0)     5826 2024-02-19 22:18:39.000000 eva4-controller-py-0.1.3/eva4_controller_py/__init__.py
--rw-r--r--   0 divisor   (1000) root         (0)    20095 2024-02-19 22:18:39.000000 eva4-controller-py-0.1.3/eva4_controller_py/macro_api.py
--rw-r--r--   0 divisor   (1000) root         (0)     1307 2024-02-19 22:18:39.000000 eva4-controller-py-0.1.3/eva4_controller_py/macro_builtins.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-02-19 22:18:55.672215 eva4-controller-py-0.1.3/eva4_controller_py.egg-info/
--rw-r--r--   0 divisor   (1000) root         (0)      521 2024-02-19 22:18:55.000000 eva4-controller-py-0.1.3/eva4_controller_py.egg-info/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      362 2024-02-19 22:18:55.000000 eva4-controller-py-0.1.3/eva4_controller_py.egg-info/SOURCES.txt
--rw-r--r--   0 divisor   (1000) root         (0)        1 2024-02-19 22:18:55.000000 eva4-controller-py-0.1.3/eva4_controller_py.egg-info/dependency_links.txt
--rw-r--r--   0 divisor   (1000) root         (0)       45 2024-02-19 22:18:55.000000 eva4-controller-py-0.1.3/eva4_controller_py.egg-info/requires.txt
--rw-r--r--   0 divisor   (1000) root         (0)       19 2024-02-19 22:18:55.000000 eva4-controller-py-0.1.3/eva4_controller_py.egg-info/top_level.txt
--rw-r--r--   0 divisor   (1000) root         (0)       38 2024-02-19 22:18:55.672215 eva4-controller-py-0.1.3/setup.cfg
--rw-r--r--   0 divisor   (1000) root         (0)      820 2024-02-19 22:18:39.000000 eva4-controller-py-0.1.3/setup.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-04-25 22:40:00.065114 eva4-controller-py-0.1.4/
+-rw-r--r--   0 divisor   (1000) root         (0)    10644 2023-11-19 23:00:18.000000 eva4-controller-py-0.1.4/LICENSE
+-rw-r--r--   0 divisor   (1000) root         (0)      521 2024-04-25 22:40:00.065114 eva4-controller-py-0.1.4/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)       46 2022-04-01 21:38:20.000000 eva4-controller-py-0.1.4/README.md
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-04-25 22:40:00.065114 eva4-controller-py-0.1.4/bin/
+-rwxr-xr-x   0 divisor   (1000) root         (0)       75 2022-04-01 21:42:50.000000 eva4-controller-py-0.1.4/bin/eva4-svc-controller-py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-04-25 22:40:00.065114 eva4-controller-py-0.1.4/eva4_controller_py/
+-rw-r--r--   0 divisor   (1000) root         (0)     5826 2024-04-25 22:31:25.000000 eva4-controller-py-0.1.4/eva4_controller_py/__init__.py
+-rw-r--r--   0 divisor   (1000) root         (0)    21104 2024-04-25 22:36:53.000000 eva4-controller-py-0.1.4/eva4_controller_py/macro_api.py
+-rw-r--r--   0 divisor   (1000) root         (0)     1307 2024-04-25 22:31:25.000000 eva4-controller-py-0.1.4/eva4_controller_py/macro_builtins.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-04-25 22:40:00.065114 eva4-controller-py-0.1.4/eva4_controller_py.egg-info/
+-rw-r--r--   0 divisor   (1000) root         (0)      521 2024-04-25 22:40:00.000000 eva4-controller-py-0.1.4/eva4_controller_py.egg-info/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      362 2024-04-25 22:40:00.000000 eva4-controller-py-0.1.4/eva4_controller_py.egg-info/SOURCES.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        1 2024-04-25 22:40:00.000000 eva4-controller-py-0.1.4/eva4_controller_py.egg-info/dependency_links.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       45 2024-04-25 22:40:00.000000 eva4-controller-py-0.1.4/eva4_controller_py.egg-info/requires.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       19 2024-04-25 22:40:00.000000 eva4-controller-py-0.1.4/eva4_controller_py.egg-info/top_level.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       38 2024-04-25 22:40:00.065114 eva4-controller-py-0.1.4/setup.cfg
+-rw-r--r--   0 divisor   (1000) root         (0)      820 2024-04-25 22:31:25.000000 eva4-controller-py-0.1.4/setup.py
```

### Comparing `eva4-controller-py-0.1.3/LICENSE` & `eva4-controller-py-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eva4-controller-py-0.1.3/PKG-INFO` & `eva4-controller-py-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eva4-controller-py
-Version: 0.1.3
+Version: 0.1.4
 Summary: EVA ICS v4 Python macros controller service
 Home-page: https://github.com/eva-ics/eva4
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eva4-controller-py-0.1.3/eva4_controller_py/__init__.py` & `eva4-controller-py-0.1.4/eva4_controller_py/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 
 from evaics.sdk import Service, Controller, Action, no_rpc_method, ServiceInfo
 from evaics.sdk import OID
 
 from timeouter import Timer
 
 from types import SimpleNamespace
```

### Comparing `eva4-controller-py-0.1.3/eva4_controller_py/macro_api.py` & `eva4-controller-py-0.1.4/eva4_controller_py/macro_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 from evaics.exceptions import ResourceAlreadyExists
 from evaics.exceptions import ResourceNotFound
 from evaics.exceptions import ResourceBusy
 from evaics.exceptions import AccessDenied
 from evaics.exceptions import InvalidParameter
 from evaics.exceptions import MethodNotImplemented
 
-from evaics.sdk import LocalProxy, rpc_e2e, pack, unpack
+from evaics.sdk import LocalProxy, rpc_e2e, pack, unpack, OID
+from evaics.sdk import RAW_STATE_TOPIC
 
 from evaics.tools import dict_from_str
 
 _shared = {}
 _shared_lock = threading.RLock()
 
 eva_dir = None
@@ -43,15 +44,15 @@
     return payload
 
 
 def get_service():
     """
     Get the service object for the direct access
 
-    e.g. service.bus: direct access to BUS/RT
+    e.g. service.bus: direct access to BUS/RT,
     service.rpc: direct access to BUS/RT RPC
 
     Returns:
         the service object
     """
     return service
 
@@ -93,14 +94,51 @@
         raise rpc_e2e(e)
     if result:
         return unpack(result)
     else:
         return True
 
 
+def bus_publish(topic, payload, qos=0):
+    """
+    Publishes a message to a bus topic
+
+    Args:
+        topic: topic name
+        payload: message payload
+        qos: QoS level (default: 0)
+    """
+    try:
+        service.bus.send(
+            topic,
+            busrt.client.Frame(pack(payload),
+                               tp=busrt.client.OP_PUBLISH,
+                               qos=qos)).wait_completed()
+    except busrt.rpc.RpcException as e:
+        raise rpc_e2e(e)
+
+
+def update_state(oid, state):
+    """
+    Updates item state
+
+    Args:
+        oid: item OID
+        state: new state (may contain status/value fields)
+
+    Optional:
+        force: force update even if the state is not changed
+    """
+    if 'status' not in state:
+        state['status'] = 1
+    oid = OID(oid) if isinstance(oid, str) else oid
+    topic = f'{RAW_STATE_TOPIC}{oid.to_path()}'
+    bus_publish(topic, state)
+
+
 def report_accounting_event(u=None,
                             src=None,
                             svc=None,
                             subj=None,
                             oid=None,
                             data=None,
                             note=None,
@@ -767,17 +805,15 @@
         mask: path and mask (e.g. /opt/data/\*.jpg)
         recursive: if True, perform a recursive search
 
     Returns:
         dict with fields 'name' 'file', 'size' and 'time' { 'c': created,
         'm': modified }
     """
-    fls = [
-        x for x in glob.glob(mask, recursive=recursive) if os.path.isfile(x)
-    ]
+    fls = [x for x in glob.glob(mask, recursive=recursive) if os.path.isfile(x)]
     l = []
     for x in fls:
         l.append({
             'name': os.path.basename(x),
             'file': os.path.abspath(x),
             'size': os.path.getsize(x),
             'time': {
@@ -868,14 +904,15 @@
     '_sleep': time.sleep,
     'lock': lock,
     'unlock': unlock,
     'is_expired': is_expired,
     'is_busy': is_busy,
     'set': _set,
     'state': state,
+    'update_state': update_state,
     'sha256sum': sha256sum,
     'status': status,
     'value': value,
     'reset': reset,
     'clear': clear,
     'toggle': toggle,
     'increment': increment,
@@ -894,9 +931,10 @@
     'ping': ping,
     'time': time.time,
     'mail': mail,
     'instant': time.perf_counter,
     'date': date,
     'ls': ls,
     'rpc_call': rpc_call,
+    'bus_publish': bus_publish,
     'report_accounting_event': report_accounting_event
 }
```

### Comparing `eva4-controller-py-0.1.3/eva4_controller_py/macro_builtins.py` & `eva4-controller-py-0.1.4/eva4_controller_py/macro_builtins.py`

 * *Files identical despite different names*

### Comparing `eva4-controller-py-0.1.3/eva4_controller_py.egg-info/PKG-INFO` & `eva4-controller-py-0.1.4/eva4_controller_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eva4-controller-py
-Version: 0.1.3
+Version: 0.1.4
 Summary: EVA ICS v4 Python macros controller service
 Home-page: https://github.com/eva-ics/eva4
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eva4-controller-py-0.1.3/setup.py` & `eva4-controller-py-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
```

