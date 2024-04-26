# Comparing `tmp/machineroom-0.47.0.tar.gz` & `tmp/machineroom-0.47.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machineroom-0.47.0.tar", last modified: Fri Apr 26 06:23:51 2024, max compression
+gzip compressed data, was "machineroom-0.47.1.tar", last modified: Fri Apr 26 07:28:15 2024, max compression
```

## Comparing `machineroom-0.47.0.tar` & `machineroom-0.47.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 06:23:51.572775 machineroom-0.47.0/
--rw-r--r--   0 root         (0) staff       (20)     2365 2024-04-24 18:48:26.000000 machineroom-0.47.0/.gitignore
--rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.47.0/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     4856 2024-04-26 06:23:51.572607 machineroom-0.47.0/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3754 2024-04-26 03:38:34.000000 machineroom-0.47.0/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 06:23:51.560359 machineroom-0.47.0/cmdbin/
--rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.47.0/cmdbin/connect
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 06:23:51.566742 machineroom-0.47.0/machineroom/
--rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-26 06:23:51.000000 machineroom-0.47.0/machineroom/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    10230 2024-04-26 03:55:10.000000 machineroom-0.47.0/machineroom/const.py
--rw-r--r--   0 root         (0) staff       (20)      286 2024-04-26 04:12:22.000000 machineroom-0.47.0/machineroom/errs.py
--rw-r--r--   0 root         (0) staff       (20)     1831 2024-04-26 06:19:21.000000 machineroom-0.47.0/machineroom/infra.py
--rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.47.0/machineroom/schema.json
--rw-r--r--   0 root         (0) staff       (20)    14636 2024-04-26 02:51:44.000000 machineroom-0.47.0/machineroom/sql.py
--rw-r--r--   0 root         (0) staff       (20)    29286 2024-04-26 04:14:57.000000 machineroom-0.47.0/machineroom/taskbase.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 06:23:51.571168 machineroom-0.47.0/machineroom/tunnels/
--rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.47.0/machineroom/tunnels/__init__.py
--rwxr-xr-x   0 root         (0) staff       (20)     8068 2024-04-26 03:02:40.000000 machineroom-0.47.0/machineroom/tunnels/conn.py
--rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.47.0/machineroom/tunnels/fork.py
--rw-r--r--   0 root         (0) staff       (20)    17272 2024-04-26 06:23:36.000000 machineroom-0.47.0/machineroom/util.py
--rw-r--r--   0 root         (0) staff       (20)     6352 2024-04-26 03:58:26.000000 machineroom-0.47.0/machineroom/worker.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 06:23:51.572025 machineroom-0.47.0/machineroom.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     4856 2024-04-26 06:23:51.000000 machineroom-0.47.0/machineroom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      534 2024-04-26 06:23:51.000000 machineroom-0.47.0/machineroom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-26 06:23:51.000000 machineroom-0.47.0/machineroom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       28 2024-04-26 06:23:51.000000 machineroom-0.47.0/machineroom.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       12 2024-04-26 06:23:51.000000 machineroom-0.47.0/machineroom.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       79 2024-04-26 06:23:51.573320 machineroom-0.47.0/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.47.0/setup.py
--rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-15 07:27:18.000000 machineroom-0.47.0/update
--rw-r--r--   0 root         (0) staff       (20)        7 2024-04-26 06:23:43.000000 machineroom-0.47.0/version
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 07:28:15.218748 machineroom-0.47.1/
+-rw-r--r--   0 root         (0) staff       (20)     2370 2024-04-26 06:25:54.000000 machineroom-0.47.1/.gitignore
+-rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.47.1/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     4856 2024-04-26 07:28:15.218544 machineroom-0.47.1/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3754 2024-04-26 03:38:34.000000 machineroom-0.47.1/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 07:28:15.205391 machineroom-0.47.1/cmdbin/
+-rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.47.1/cmdbin/connect
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 07:28:15.212544 machineroom-0.47.1/machineroom/
+-rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-26 07:28:14.000000 machineroom-0.47.1/machineroom/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    10297 2024-04-26 07:21:15.000000 machineroom-0.47.1/machineroom/const.py
+-rw-r--r--   0 root         (0) staff       (20)      286 2024-04-26 04:12:22.000000 machineroom-0.47.1/machineroom/errs.py
+-rw-r--r--   0 root         (0) staff       (20)     1830 2024-04-26 06:41:52.000000 machineroom-0.47.1/machineroom/infra.py
+-rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.47.1/machineroom/schema.json
+-rw-r--r--   0 root         (0) staff       (20)    14128 2024-04-26 07:27:26.000000 machineroom-0.47.1/machineroom/sql.py
+-rw-r--r--   0 root         (0) staff       (20)    29559 2024-04-26 07:16:26.000000 machineroom-0.47.1/machineroom/taskbase.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 07:28:15.216944 machineroom-0.47.1/machineroom/tunnels/
+-rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.47.1/machineroom/tunnels/__init__.py
+-rwxr-xr-x   0 root         (0) staff       (20)     8068 2024-04-26 03:02:40.000000 machineroom-0.47.1/machineroom/tunnels/conn.py
+-rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.47.1/machineroom/tunnels/fork.py
+-rw-r--r--   0 root         (0) staff       (20)    17521 2024-04-26 07:21:15.000000 machineroom-0.47.1/machineroom/util.py
+-rw-r--r--   0 root         (0) staff       (20)     7702 2024-04-26 07:27:26.000000 machineroom-0.47.1/machineroom/worker.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 07:28:15.217844 machineroom-0.47.1/machineroom.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     4856 2024-04-26 07:28:15.000000 machineroom-0.47.1/machineroom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      534 2024-04-26 07:28:15.000000 machineroom-0.47.1/machineroom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-26 07:28:15.000000 machineroom-0.47.1/machineroom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       28 2024-04-26 07:28:15.000000 machineroom-0.47.1/machineroom.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       12 2024-04-26 07:28:15.000000 machineroom-0.47.1/machineroom.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-04-26 07:28:15.219425 machineroom-0.47.1/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.47.1/setup.py
+-rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-26 07:28:07.000000 machineroom-0.47.1/update
+-rw-r--r--   0 root         (0) staff       (20)        7 2024-04-26 07:28:08.000000 machineroom-0.47.1/version
```

### Comparing `machineroom-0.47.0/.gitignore` & `machineroom-0.47.1/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -185,14 +185,15 @@
 
 # Environments
 .env
 .venv
 env/
 venv/
 ENV/
+enp/
 env.bak/
 venv.bak/
 
 # Spyder project settings
 .spyderproject
 .spyproject
```

### Comparing `machineroom-0.47.0/LICENSE` & `machineroom-0.47.1/LICENSE`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.0/PKG-INFO` & `machineroom-0.47.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.47.0
+Version: 0.47.1
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.47.0/README.md` & `machineroom-0.47.1/README.md`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.0/cmdbin/connect` & `machineroom-0.47.1/cmdbin/connect`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.0/machineroom/__init__.py` & `machineroom-0.47.1/machineroom/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 logger5 = logging.getLogger("invoke")
 logger2.setLevel(logging.ERROR)
 logger1.setLevel(logging.ERROR)
 logger3.setLevel(logging.ERROR)
 logger4.setLevel(logging.ERROR)
 logger5.setLevel(logging.ERROR)
 
-__version__ = '0.47.0'
+__version__ = '0.47.1'
```

### Comparing `machineroom-0.47.0/machineroom/const.py` & `machineroom-0.47.1/machineroom/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 CMD_IMPORT = ["import", "update_file", "update_conf", "updateconfig", "updateconfiguration", "updateconfigurations"]
 CMD_VERSION = ["v", "ver", "versions", "version"]
 CMD_RETIRE = ["retire", "retires", "retired"]
 CMD_OFF_CERT = ["off-cert", "takeoff", "stripcert", "takeout", "removecert", "certremove"]
 CMD_ADD_CERT = ["add-cert", "addingcert", "makecert", "cert-on", "on-cert", "customcert", "certificatessh",
                 "sshcertifcate"]
 CMD_GENERATE_PROFILE = ["generateprofile", "gen-profile", "watch-profile","watch_file","watchscan"]
-
+CMD_SET_BASH_START = ["sethome","startpath","loginstart","loginat"]
 DETECT_PROCESS = 'ps aux | grep -sie "{COMMAND_NAME}" | grep -v "grep -sie"'
 HEALTH_CHK_DB = """docker run --rm -it --mount type=bind,source={PWD},destination=/data sstc/sqlite3 find . -maxdepth 1 -iname "*.db" -print0 -exec sqlite3 '{}' 'PRAGMA integrity_check;' ';'"""
 HEALTH_CHK_DB2 = """
 sudo apt update && sudo apt install sqlite3 -y
 sqlite3 --version
 sqlite3 {DB_FILE_PATH} "PRAGMA integrity_check;"
 """
```

### Comparing `machineroom-0.47.0/machineroom/infra.py` & `machineroom-0.47.1/machineroom/infra.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         k = self.start_server_from
         if self.srv.serv_count < k:
             print("cannot start from out of range server number")
             return
         if self.run_tunnel_detection():
             self.srv.use_next_node()
             k += 1
-
         while k < self.srv.serv_count:
             self.stage_0()
             c = self._est_connection()
             try:
                 self.stage_1(c)
                 if callable(callback_x):
                     callback_x(c)
```

### Comparing `machineroom-0.47.0/machineroom/schema.json` & `machineroom-0.47.1/machineroom/schema.json`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.0/machineroom/sql.py` & `machineroom-0.47.1/machineroom/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,39 +314,25 @@
 
     def _update_server_meta(self, server_id: str, res_file: dict):
         update_dic = {
             "res": json.dumps(res_file)
         }
         return self.update_param(server_id, update_dic)
 
-    def _insert_server(self, host: str, id: str, password: str, user: str, port: int,
-                       file: dict) -> bool:
-        p = {
-            "host": host,
-            "id": id,
-            "user": user,
-            "pass": password,
-            "port": port,
-            "next_action": "{}",
-            "description": "",
-            "res": json.dumps(file)
-        }
-        return self.insert_new(p)
-
     def get_res_kv(self, k: str):
         try:
             da = self.get_member_res(self._tblembr, self.server_id)
             if k in da:
                 return da[k]
             else:
                 return ""
         except TypeError:
             return ""
         except Exception:
-            return ''
+            return ""
 
     def total_count(self, tbl: str) -> int:
         cursor = self.conn.cursor()
         cursor.execute(f"SELECT COUNT(*) as count FROM {tbl}")
         (count,) = cursor.fetchone()
         cursor.close()
         if count > 0:
@@ -370,16 +356,14 @@
 
     def delete_res_kv(self, k: str):
         da = self.get_member_res(self._tblembr, self.server_id)
         if k in da:
             da.pop(k)
         self._update_server_meta(self.server_id, da)
 
-    def get_home_path(self) -> str:
-        return self.get_res_kv("home_path")
 
     def get_tunnel_profile(self):
         return self.get_res_kv("tunnel_profile")
 
     def _update_what_installed(self, program_key: str):
         da = self.get_member_res(self._tblembr, self.server_id)
         da.update({program_key: True})
@@ -394,15 +378,15 @@
 
     def entrance_L1(self, auth_data: dict):
         if self.has_this_server() is False:
             default_data = {
                 "id": self.server_id,
                 "next_action": "{}",
                 "description": "",
-                "res": json.dumps({})
+                "res": "{}",
             }
             default_data.update(auth_data)
             return self.insert_new(default_data)
         else:
             auth_data.pop("id")
             return self.update_param(self.server_id, auth_data)
```

### Comparing `machineroom-0.47.0/machineroom/taskbase.py` & `machineroom-0.47.1/machineroom/taskbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -672,24 +672,26 @@
     def _est_connection(self) -> Connection:
         if self.srv.has_this_server() is False:
             return Connection(host=self.srv.current_host, port=22, user=self.srv.current_user, connect_kwargs={
                 "password": self.srv.current_pass,
                 # "key_filename": ['/Users/..../.ssh/id_rsa']
             }, config=self._config())
         elif self.srv.is_cert_installed() is False:
-            return Connection(host=self.srv.current_host, port=22, user=self.srv.current_user, connect_kwargs={
-                "password": self.srv.current_pass,
-                # "key_filename": ['/Users/..../.ssh/id_rsa']
-            }, config=self._config())
+            return Connection(host=self.srv.current_host, port=self.srv.current_srv_port, user=self.srv.current_user,
+                              connect_kwargs={
+                                  "password": self.srv.current_pass,
+                                  # "key_filename": ['/Users/..../.ssh/id_rsa']
+                              }, config=self._config())
         else:
             print("cert is installed.")
-            return Connection(host=self.srv.current_host, port=22, user=self.srv.current_user, connect_kwargs={
-                # "password": self.srv.current_pass,
-                "key_filename": [Config.PUB_KEY]
-            }, config=self._config())
+            return Connection(host=self.srv.current_host, port=self.srv.current_srv_port, user=self.srv.current_user,
+                              connect_kwargs={
+                                  # "password": self.srv.current_pass,
+                                  "key_filename": [Config.PUB_KEY]
+                              }, config=self._config())
 
     def connection_err(self, item: Exception, on_err_exit: bool):
         print("======================== exit.")
         print(self.srv.current_id, self.srv.current_host)
         if "Connection reset by peer" in str(item) or "Errno 54" in str(item):
             print("Maybe Offline")
         else:
@@ -710,14 +712,16 @@
             return False
         else:
             self.connection_err(e, fail_exit)
             return True
 
     def stage_0(self):
         ...
+    def maybe_upgrade_docker(self):
+        ...
 
     def stage_1(self, c: Connection):
         for key in Config.STAGE1:
             self._stage_loop(c, key)
 
     def load_system_paths(self, c: Connection):
         r = c.run("which bash", warn=True, pty=True)
@@ -730,14 +734,15 @@
             if docker_version_checker(r):
                 self.srv.local().docker_ce_install()
             else:
                 r = c.run("which docker-compose", warn=True, pty=True)
                 if str(r.stdout.strip()) != "":
                     Config.DOCKER_COMPOSE = str(r.stdout.strip())
                     self.srv.local().docker_compose_install()
+                self.maybe_upgrade_docker()
 
         r = c.run("which daed", warn=True, pty=True)
         if str(r.stdout.strip()) != "":
             self.srv.local().dae_install()
 
     def _stage_loop(self, c: Connection, task: str):
         if task == "cert":
@@ -748,24 +753,14 @@
                 else:
                     self.srv.cert_install()
 
         if task == "env":
             c.config.load_shell_env()
             self.load_system_paths(c)
 
-        if task == "docker":
-            if self.srv.local().is_docker_ce_installed() is False:
-                if detect_program(c, "docker") is False:
-                    install_docker_ce(c)
-                    self.srv.local().docker_ce_install()
-                else:
-                    print("DOCKER is installed")
-            else:
-                install_docker_ce(c)
-
         if task == "python":
             if self.srv.local().is_python_installed() is False:
                 if detect_program(c, "python3") is False:
                     print("python3 needs to install")
                     install_python(c)
                     self.srv.local().python3_install()
 
@@ -805,7 +800,18 @@
     def install_xclash(self, install_times: int) -> bool:
         # if check_docker_ps_specific(c, "dreamacro/clash") is False:...
 
         return False
 
     def install_xclash_update(self) -> bool:
         return False
+
+
+"""if self.srv.local().is_docker_ce_installed() is False:
+                if detect_program(c, "docker") is False:
+                    install_docker_ce(c)
+                    self.srv.local().docker_ce_install()
+                else:
+                    print("DOCKER is installed")
+            else:
+                install_docker_ce(c)
+"""
```

### Comparing `machineroom-0.47.0/machineroom/tunnels/conn.py` & `machineroom-0.47.1/machineroom/tunnels/conn.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.0/machineroom/util.py` & `machineroom-0.47.1/machineroom/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 from invoke import StreamWatcher
 from machineroom.sql import ServerRoom
 
 from .const import *
 from .errs import *
 
 
-def function_command_alias(actual: str, command_alias: list):
-    if actual in command_alias:
+def function_command_alias(input: str, actual: str, command_alias: list):
+    if input in command_alias:
         return True, actual
     return False, None
 
 
 def check_for_bad_ids(id_name: str):
-    all_bad = CMD_SCAN_DOCKER + CMD_IMPORT + CMD_SCAN_PORT + CMD_LIST + CMD_VERSION + CMD_RETIRE + CMD_OFF_CERT + CMD_ADD_CERT + CMD_GENERATE_PROFILE
+    all_bad = CMD_SCAN_DOCKER + CMD_IMPORT + CMD_SCAN_PORT + CMD_LIST + CMD_VERSION + CMD_RETIRE + CMD_OFF_CERT + CMD_ADD_CERT + CMD_GENERATE_PROFILE +CMD_SET_BASH_START
     if id_name in all_bad:
         raise BadIDs()
 
 
 def use_args() -> Tuple[str, str, str]:
     opt1 = ""
     opt2 = ""
@@ -37,36 +37,39 @@
         opt1 = sys.argv[1]
         if len(sys.argv) >= 3:
             opt2 = sys.argv[2]
             if len(sys.argv) >= 4:
                 opt3 = sys.argv[3]
 
     cmd = opt1
-    f, c = function_command_alias("ls", CMD_LIST)
+    f, c = function_command_alias(opt1, "ls", CMD_LIST)
     if f is True:
         cmd = c
-    f, c = function_command_alias("scandocker", CMD_SCAN_DOCKER)
+    f, c = function_command_alias(opt1, "docker-scan", CMD_SCAN_DOCKER)
     if f is True:
         cmd = c
-    f, c = function_command_alias("import", CMD_IMPORT)
+    f, c = function_command_alias(opt1, "import", CMD_IMPORT)
     if f is True:
         cmd = c
-    f, c = function_command_alias("v", CMD_VERSION)
+    f, c = function_command_alias(opt1, "v", CMD_VERSION)
     if f is True:
         cmd = c
-    f, c = function_command_alias("retire", CMD_RETIRE)
+    f, c = function_command_alias(opt1, "retire", CMD_RETIRE)
     if f is True:
         cmd = c
-    f, c = function_command_alias("off-cert", CMD_OFF_CERT)
+    f, c = function_command_alias(opt1, "off-cert", CMD_OFF_CERT)
     if f is True:
         cmd = c
-    f, c = function_command_alias("add-cert", CMD_ADD_CERT)
+    f, c = function_command_alias(opt1, "add-cert", CMD_ADD_CERT)
     if f is True:
         cmd = c
-    f, c = function_command_alias("generatewatchprofile", CMD_GENERATE_PROFILE)
+    f, c = function_command_alias(opt1, "watch-profile", CMD_GENERATE_PROFILE)
+    if f is True:
+        cmd = c
+    f, c = function_command_alias(opt1, "set-home", CMD_SET_BASH_START)
     if f is True:
         cmd = c
 
     return cmd, opt2, opt3
 
 
 def err_exit(msg):
@@ -422,14 +425,15 @@
 
 class Servers:
     _meta_file: str
     current_id: str
     current_host: str
     current_user: str
     current_pass: str
+    current_srv_port:int
     _srv_index: int
     _meta_file: int
     _tunnel_type: TunnelType
     profile_name: str
     _on_detect: bool
     _local_db: ServerRoom
 
@@ -490,28 +494,29 @@
             self.profile_name = line[0].replace("#", "")
             raise FoundVPNTunnel()
 
         self.current_id = ID
         self.current_host = IP
         self.current_user = configuration.get("user")
         self.current_pass = configuration.get("pass")
+        self.current_srv_port = configuration.get("port")
+        self._local_db.set_server_id(ID)
         if self._on_detect is False:
             print(f"## ☎️ Now enter network ID#{n}: {ID} {IP}")
         if self.has_tunnel():
             self._local_db.entrance_L2(self.profile_name, configuration)
         else:
             self._local_db.entrance_L1(configuration)
 
     def has_tunnel(self) -> bool:
         return self._tunnel_type != TunnelType.NO_TUNNEL
 
     def use_next_node(self, x: int = 1):
         self._srv_index = self._srv_index + x
         check_for_bad_ids(self.current_id)
-        self._local_db.set_server_id(self.current_id)
         self.read_serv_at(self._srv_index)
 
 
 def reader_split_recognition(line: str) -> list:
     if "----" in line:
         line = line.split("----")
     elif "---" in line:
```

### Comparing `machineroom-0.47.0/machineroom/worker.py` & `machineroom-0.47.1/machineroom/worker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import random
 
 from machineroom import taskbase as tb, __version__, ServerRoom, use_args, FieldConstruct, err_exit
 from machineroom.infra import Infra1
 from machineroom.tunnels.conn import *
 from fabric import Connection
+from tabulate import tabulate
 
 try:
     import SQLiteAsJSON
 except:
     os.system('python3.11 -m pip install SQLiteAsJSON')
     import SQLiteAsJSON
 
@@ -23,95 +24,119 @@
     def action_retire(self):
         self.run_offline(self._retire_on_each_server)
 
     def action_off_cert(self):
         self.run_offline(self._action_off_cert)
 
     def _retire_on_each_server(self):
-        self.db.update_res_kv("retired", True)
+        self.srv.local().update_res_kv("retired", True)
 
     def _action_off_cert(self):
-        self.db.delete_res_kv("identity_cert_installed")
+        self.srv.local().delete_res_kv("identity_cert_installed")
 
     def action_scan_ports(self):
         self.run_conn(self._from_c_ports)
 
     def _from_c_ports(self, c: Connection):
         m = tb.list_all_open_ports(c)
-        self.db.update_res_kv("ports", m)
+        self.srv.local().update_res_kv("ports", m)
         any_one = random.choice(m)
 
-
-
     def action_add_custom_cert(self, name, pubkey_path):
         def certification(c: Connection):
             if tb.detect_cert_signature(c, name) is False:
                 tb.copy_id(c, pubkey_path)
-                self.db.update_res_kv(f"custom_cert_{name}", True)
+                self.srv.local().update_res_kv(f"custom_cert_{name}", True)
 
         self.run_conn(certification)
 
     def action_remove_custom_cert(self, name):
         def certification(c: Connection):
             if tb.detect_cert_signature(c, name) is False:
-                self.db.delete_res_kv(f"custom_cert_{name}")
+                self.srv.local().delete_res_kv(f"custom_cert_{name}")
 
         self.run_conn(certification)
 
 
 def internal_work():
     """
     This is the cmd console use functions
     alpha stage now.
-    """
-    (a, b, c) = use_args()
-    local = ServerRoom()
-    if a == "ls":
-        print("Here is my machine room...")
-        gh = local.show_all_serv()
-        for (id, host, res) in gh:
-            local.set_server_id(id)
+
+
             y = FieldConstruct()
             y.add_icon(f"{id}  -> {host}     ")
             tun = local.get_tunnel_profile()
             if tun != "":
                 y.add_icon(f"TUNNEL PROFILE: {tun}")
             y.add_icon("EXPIRED" if local.is_what_installed_full("retire", id) else "")
             y.add_icon("CERT" if local.is_what_installed_full("identity_cert_installed", id) else "")
             y.add_icon("DOCKER" if local.is_what_installed_full("docker_compose_installed", id) else "")
             y.add_icon("DAED" if local.is_what_installed_full("daed_installed", id) else "")
             y.add_icon("YACHT" if local.is_what_installed_full("yacht_installed", id) else "")
             y.add_icon("PY" if local.is_what_installed_full("python3_installed", id) else "")
-            print(y.output())
-    elif a == "scandocker":
+
+    """
+    (a, b, c) = use_args()
+    local = ServerRoom()
+    if a == "ls":
+        gh = local.show_all_serv()
+        table_content = []
+        for (id, host, res) in gh:
+            local.set_server_id(id)
+            content = []
+            content.append(id)
+            content.append(host)
+            tun = local.get_tunnel_profile()
+            if tun != "":
+                content.append(f"TUNNEL PROFILE: {tun}")
+
+            content.append("EXPIRED" if local.is_what_installed_full("retire", id) else "")
+            content.append("CERT" if local.is_what_installed_full("identity_cert_installed", id) else "")
+            content.append("DOCKER" if local.is_what_installed_full("docker_compose_installed", id) else "")
+            content.append("DAED" if local.is_what_installed_full("daed_installed", id) else "")
+            content.append("YACHT" if local.is_what_installed_full("yacht_installed", id) else "")
+            content.append("PY" if local.is_what_installed_full("python3_installed", id) else "")
+
+            table_content.append(content)
+
+        print(tabulate(table_content))
+    elif a == "docker-scan":
         print("This to scan out the running docker containers in the status of that server")
     elif a == "scanports":
         print("This to scan out the running docker containers in the status of that server")
     elif a == "import":
         if b == "":
             err_exit("need to have one more arg")
         file = os.path.join(Config.DATAPATH_BASE, b)
         if os.path.exists(file) is False:
             err_exit("Wrong path cannot open this file" + file)
         job = ServerDoorJob(b)
         job.action_import()
     elif a == "v":
         print(f"version. {__version__}")
 
-    elif a == "generatewatchprofile":
+    elif a == "watch-profile":
         if b == "":
             err_exit("need to have one more arg")
         file = os.path.join(Config.DATAPATH_BASE, b)
         if os.path.exists(file) is False:
             err_exit("Wrong path cannot open this file" + file)
         job = ServerDoorJob(b)
-
         job.action_scan_ports()
 
-
+    elif a == "set-home":
+        if b == "":
+            err_exit("need to have one more arg for the server ID")
+        if c == "":
+            err_exit("need to have one more arg for the the remote start path, for example /home")
+        local.set_server_id(b)
+        if local.has_this_server() is False:
+            err_exit(f"there is no such server for ---> {b}")
+            local.update_res_kv("home_path", c)
 
     elif a == "retire":
         if b == "":
             err_exit("need to have one more arg")
         file = os.path.join(Config.DATAPATH_BASE, b)
         if os.path.exists(file) is False:
             err_exit("Wrong path cannot open this file" + file)
@@ -152,16 +177,16 @@
     elif a != None:
         local.set_server_id(a)
         if local.has_this_server() is False:
             err_exit(f"there is no such server for ---> {a}")
         cert = "/Users/hesdx/.ssh/id_rsa" if local.is_cert_installed() else ""
         (h, u, p) = local.get_info()
         port_sentence = "" if p == 22 else f"-p {p} "
-        home_path = local.get_home_path()
-        home_path = f'"cd {home_path}; bash"' if home_path != "" else ''
+        home_path = local.get_res_kv("home_path")
+        home_path = f'"cd {home_path}; bash"' if home_path != "" else ""
         if local.get_tunnel_profile() != "":
             print("TUNNEL PROFILE: {local.get_tunnel_profile()}")
             use_macos_vpn_on(local.get_tunnel_profile())
         os.system(f'ssh {port_sentence}-i {cert} -t {u}@{h} {home_path}')
     else:
         err_exit("cannot serv no args")
```

### Comparing `machineroom-0.47.0/machineroom.egg-info/PKG-INFO` & `machineroom-0.47.1/machineroom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.47.0
+Version: 0.47.1
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.47.0/machineroom.egg-info/SOURCES.txt` & `machineroom-0.47.1/machineroom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.0/setup.py` & `machineroom-0.47.1/setup.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.0/update` & `machineroom-0.47.1/update`

 * *Files identical despite different names*

