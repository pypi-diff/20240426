# Comparing `tmp/pyssh_util-1.0.0.tar.gz` & `tmp/pyssh_util-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyssh_util-1.0.0.tar", last modified: Fri Mar 15 14:39:12 2024, max compression
+gzip compressed data, was "pyssh_util-1.0.2.tar", last modified: Fri Apr 26 05:37:16 2024, max compression
```

## Comparing `pyssh_util-1.0.0.tar` & `pyssh_util-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:39:12.101728 pyssh_util-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-15 14:39:02.000000 pyssh_util-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-15 14:39:12.101728 pyssh_util-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-15 14:39:02.000000 pyssh_util-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:39:12.101728 pyssh_util-1.0.0/pyssh_util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:39:02.000000 pyssh_util-1.0.0/pyssh_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-03-15 14:39:02.000000 pyssh_util-1.0.0/pyssh_util/ssh_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:39:12.101728 pyssh_util-1.0.0/pyssh_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-15 14:39:12.000000 pyssh_util-1.0.0/pyssh_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-15 14:39:12.000000 pyssh_util-1.0.0/pyssh_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 14:39:12.000000 pyssh_util-1.0.0/pyssh_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-15 14:39:12.000000 pyssh_util-1.0.0/pyssh_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-15 14:39:12.000000 pyssh_util-1.0.0/pyssh_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 14:39:12.000000 pyssh_util-1.0.0/pyssh_util.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 14:39:12.101728 pyssh_util-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-15 14:39:02.000000 pyssh_util-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:37:16.684308 pyssh_util-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-26 05:37:08.000000 pyssh_util-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-26 05:37:16.684308 pyssh_util-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-26 05:37:08.000000 pyssh_util-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:37:16.684308 pyssh_util-1.0.2/pyssh_util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 05:37:08.000000 pyssh_util-1.0.2/pyssh_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-26 05:37:08.000000 pyssh_util-1.0.2/pyssh_util/ssh_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:37:16.684308 pyssh_util-1.0.2/pyssh_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-26 05:37:16.000000 pyssh_util-1.0.2/pyssh_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-26 05:37:16.000000 pyssh_util-1.0.2/pyssh_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 05:37:16.000000 pyssh_util-1.0.2/pyssh_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 05:37:16.000000 pyssh_util-1.0.2/pyssh_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 05:37:16.000000 pyssh_util-1.0.2/pyssh_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 05:37:16.000000 pyssh_util-1.0.2/pyssh_util.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 05:37:16.684308 pyssh_util-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-26 05:37:08.000000 pyssh_util-1.0.2/setup.py
```

### Comparing `pyssh_util-1.0.0/LICENSE` & `pyssh_util-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyssh_util-1.0.0/PKG-INFO` & `pyssh_util-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyssh_util
-Version: 1.0.0
+Version: 1.0.2
 Summary: ssh助手
 Home-page: https://github.com/buyfakett
 Author: buyfakett
 Author-email: buyfakett@vip.qq.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pyssh_util-1.0.0/README.md` & `pyssh_util-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyssh_util-1.0.0/pyssh_util/ssh_util.py` & `pyssh_util-1.0.2/pyssh_util/ssh_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.username = username
         self.password = password
         self.client = paramiko.SSHClient()
         self.client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
         self.connect()
 
     def connect(self):
-        self.client.connect(self.host, port=self.port, username=self.username, password=self.password)
+        self.client.connect(self.host, port=self.port, username=self.username, password=self.password, allow_agent=False, look_for_keys=False, gss_auth=False)
 
     def execute_command(self, command):
         logging.info(f"即将执行命令: {command}")
         stdin, stdout, stderr = self.client.exec_command(command)
         output = stdout.read().decode('utf-8')
         error = stderr.read().decode('utf-8')
         exit_code = stdout.channel.recv_exit_status()
```

### Comparing `pyssh_util-1.0.0/pyssh_util.egg-info/PKG-INFO` & `pyssh_util-1.0.2/pyssh_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyssh_util
-Version: 1.0.0
+Version: 1.0.2
 Summary: ssh助手
 Home-page: https://github.com/buyfakett
 Author: buyfakett
 Author-email: buyfakett@vip.qq.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pyssh_util-1.0.0/setup.py` & `pyssh_util-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with io.open("requirements.txt", 'r') as f:
     install_requires = f.read().split(os.sep)
 
 
 setup(
     name='pyssh_util',
-    version='1.0.0',
+    version='v1.0.2',
     description='ssh助手',
     author='buyfakett',
     author_email='buyfakett@vip.qq.com',
     license='MIT',
     url="https://github.com/buyfakett",
     packages=find_packages(),  # packages=["pytest"],
     long_description=long_description,
```

