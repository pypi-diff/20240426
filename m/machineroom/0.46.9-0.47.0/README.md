# Comparing `tmp/machineroom-0.46.9.tar.gz` & `tmp/machineroom-0.47.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machineroom-0.46.9.tar", last modified: Fri Apr 26 06:17:04 2024, max compression
+gzip compressed data, was "machineroom-0.47.0.tar", last modified: Fri Apr 26 06:23:51 2024, max compression
```

## Comparing `machineroom-0.46.9.tar` & `machineroom-0.47.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 06:17:04.960313 machineroom-0.46.9/
--rw-r--r--   0 root         (0) staff       (20)     2365 2024-04-24 18:48:26.000000 machineroom-0.46.9/.gitignore
--rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.46.9/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     4856 2024-04-26 06:17:04.960146 machineroom-0.46.9/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3754 2024-04-26 03:38:34.000000 machineroom-0.46.9/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 06:17:04.946563 machineroom-0.46.9/cmdbin/
--rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.46.9/cmdbin/connect
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 06:17:04.954306 machineroom-0.46.9/machineroom/
--rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-26 06:17:04.000000 machineroom-0.46.9/machineroom/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    10230 2024-04-26 03:55:10.000000 machineroom-0.46.9/machineroom/const.py
--rw-r--r--   0 root         (0) staff       (20)      286 2024-04-26 04:12:22.000000 machineroom-0.46.9/machineroom/errs.py
--rw-r--r--   0 root         (0) staff       (20)     1832 2024-04-26 03:58:26.000000 machineroom-0.46.9/machineroom/infra.py
--rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.46.9/machineroom/schema.json
--rw-r--r--   0 root         (0) staff       (20)    14636 2024-04-26 02:51:44.000000 machineroom-0.46.9/machineroom/sql.py
--rw-r--r--   0 root         (0) staff       (20)    29286 2024-04-26 04:14:57.000000 machineroom-0.46.9/machineroom/taskbase.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 06:17:04.958716 machineroom-0.46.9/machineroom/tunnels/
--rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.46.9/machineroom/tunnels/__init__.py
--rwxr-xr-x   0 root         (0) staff       (20)     8068 2024-04-26 03:02:40.000000 machineroom-0.46.9/machineroom/tunnels/conn.py
--rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.46.9/machineroom/tunnels/fork.py
--rw-r--r--   0 root         (0) staff       (20)    17145 2024-04-26 04:04:43.000000 machineroom-0.46.9/machineroom/util.py
--rw-r--r--   0 root         (0) staff       (20)     6352 2024-04-26 03:58:26.000000 machineroom-0.46.9/machineroom/worker.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 06:17:04.959552 machineroom-0.46.9/machineroom.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     4856 2024-04-26 06:17:04.000000 machineroom-0.46.9/machineroom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      534 2024-04-26 06:17:04.000000 machineroom-0.46.9/machineroom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-26 06:17:04.000000 machineroom-0.46.9/machineroom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       28 2024-04-26 06:17:04.000000 machineroom-0.46.9/machineroom.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       12 2024-04-26 06:17:04.000000 machineroom-0.46.9/machineroom.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       79 2024-04-26 06:17:04.960851 machineroom-0.46.9/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.46.9/setup.py
--rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-15 07:27:18.000000 machineroom-0.46.9/update
--rw-r--r--   0 root         (0) staff       (20)        7 2024-04-26 06:16:56.000000 machineroom-0.46.9/version
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 06:23:51.572775 machineroom-0.47.0/
+-rw-r--r--   0 root         (0) staff       (20)     2365 2024-04-24 18:48:26.000000 machineroom-0.47.0/.gitignore
+-rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.47.0/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     4856 2024-04-26 06:23:51.572607 machineroom-0.47.0/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3754 2024-04-26 03:38:34.000000 machineroom-0.47.0/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 06:23:51.560359 machineroom-0.47.0/cmdbin/
+-rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.47.0/cmdbin/connect
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 06:23:51.566742 machineroom-0.47.0/machineroom/
+-rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-26 06:23:51.000000 machineroom-0.47.0/machineroom/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    10230 2024-04-26 03:55:10.000000 machineroom-0.47.0/machineroom/const.py
+-rw-r--r--   0 root         (0) staff       (20)      286 2024-04-26 04:12:22.000000 machineroom-0.47.0/machineroom/errs.py
+-rw-r--r--   0 root         (0) staff       (20)     1831 2024-04-26 06:19:21.000000 machineroom-0.47.0/machineroom/infra.py
+-rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.47.0/machineroom/schema.json
+-rw-r--r--   0 root         (0) staff       (20)    14636 2024-04-26 02:51:44.000000 machineroom-0.47.0/machineroom/sql.py
+-rw-r--r--   0 root         (0) staff       (20)    29286 2024-04-26 04:14:57.000000 machineroom-0.47.0/machineroom/taskbase.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 06:23:51.571168 machineroom-0.47.0/machineroom/tunnels/
+-rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.47.0/machineroom/tunnels/__init__.py
+-rwxr-xr-x   0 root         (0) staff       (20)     8068 2024-04-26 03:02:40.000000 machineroom-0.47.0/machineroom/tunnels/conn.py
+-rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.47.0/machineroom/tunnels/fork.py
+-rw-r--r--   0 root         (0) staff       (20)    17272 2024-04-26 06:23:36.000000 machineroom-0.47.0/machineroom/util.py
+-rw-r--r--   0 root         (0) staff       (20)     6352 2024-04-26 03:58:26.000000 machineroom-0.47.0/machineroom/worker.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 06:23:51.572025 machineroom-0.47.0/machineroom.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     4856 2024-04-26 06:23:51.000000 machineroom-0.47.0/machineroom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      534 2024-04-26 06:23:51.000000 machineroom-0.47.0/machineroom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-26 06:23:51.000000 machineroom-0.47.0/machineroom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       28 2024-04-26 06:23:51.000000 machineroom-0.47.0/machineroom.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       12 2024-04-26 06:23:51.000000 machineroom-0.47.0/machineroom.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-04-26 06:23:51.573320 machineroom-0.47.0/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.47.0/setup.py
+-rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-15 07:27:18.000000 machineroom-0.47.0/update
+-rw-r--r--   0 root         (0) staff       (20)        7 2024-04-26 06:23:43.000000 machineroom-0.47.0/version
```

### Comparing `machineroom-0.46.9/.gitignore` & `machineroom-0.47.0/.gitignore`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.9/LICENSE` & `machineroom-0.47.0/LICENSE`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.9/PKG-INFO` & `machineroom-0.47.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.46.9
+Version: 0.47.0
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.46.9/README.md` & `machineroom-0.47.0/README.md`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.9/cmdbin/connect` & `machineroom-0.47.0/cmdbin/connect`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.9/machineroom/__init__.py` & `machineroom-0.47.0/machineroom/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 logger5 = logging.getLogger("invoke")
 logger2.setLevel(logging.ERROR)
 logger1.setLevel(logging.ERROR)
 logger3.setLevel(logging.ERROR)
 logger4.setLevel(logging.ERROR)
 logger5.setLevel(logging.ERROR)
 
-__version__ = '0.46.9'
+__version__ = '0.47.0'
```

### Comparing `machineroom-0.46.9/machineroom/const.py` & `machineroom-0.47.0/machineroom/const.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.9/machineroom/infra.py` & `machineroom-0.47.0/machineroom/infra.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 execute_path = os.path.dirname(__file__)
 
 
 class Infra1(tb.DeploymentBotFoundation):
     def __init__(self, x):
         super().__init__(x)
 
-
     def run_conn(self, callback_x=None):
         k = self.start_server_from
         if self.srv.serv_count < k:
             print("cannot start from out of range server number")
             return
         if self.run_tunnel_detection():
             self.srv.use_next_node()
```

### Comparing `machineroom-0.46.9/machineroom/schema.json` & `machineroom-0.47.0/machineroom/schema.json`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.9/machineroom/sql.py` & `machineroom-0.47.0/machineroom/sql.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.9/machineroom/taskbase.py` & `machineroom-0.47.0/machineroom/taskbase.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.9/machineroom/tunnels/conn.py` & `machineroom-0.47.0/machineroom/tunnels/conn.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.9/machineroom/util.py` & `machineroom-0.47.0/machineroom/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,30 +38,37 @@
         if len(sys.argv) >= 3:
             opt2 = sys.argv[2]
             if len(sys.argv) >= 4:
                 opt3 = sys.argv[3]
 
     cmd = opt1
     f, c = function_command_alias("ls", CMD_LIST)
-    if f: cmd = c
+    if f is True:
+        cmd = c
     f, c = function_command_alias("scandocker", CMD_SCAN_DOCKER)
-    if f: cmd = c
+    if f is True:
+        cmd = c
     f, c = function_command_alias("import", CMD_IMPORT)
-    if f: cmd = c
+    if f is True:
+        cmd = c
     f, c = function_command_alias("v", CMD_VERSION)
-    if f: cmd = c
+    if f is True:
+        cmd = c
     f, c = function_command_alias("retire", CMD_RETIRE)
-    if f: cmd = c
+    if f is True:
+        cmd = c
     f, c = function_command_alias("off-cert", CMD_OFF_CERT)
-    if f: cmd = c
+    if f is True:
+        cmd = c
     f, c = function_command_alias("add-cert", CMD_ADD_CERT)
-    if f: cmd = c
-
+    if f is True:
+        cmd = c
     f, c = function_command_alias("generatewatchprofile", CMD_GENERATE_PROFILE)
-    if f: cmd = c
+    if f is True:
+        cmd = c
 
     return cmd, opt2, opt3
 
 
 def err_exit(msg):
     if isinstance(msg, str):
         print(msg)
```

### Comparing `machineroom-0.46.9/machineroom/worker.py` & `machineroom-0.47.0/machineroom/worker.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.9/machineroom.egg-info/PKG-INFO` & `machineroom-0.47.0/machineroom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.46.9
+Version: 0.47.0
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.46.9/machineroom.egg-info/SOURCES.txt` & `machineroom-0.47.0/machineroom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.9/setup.py` & `machineroom-0.47.0/setup.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.9/update` & `machineroom-0.47.0/update`

 * *Files identical despite different names*

