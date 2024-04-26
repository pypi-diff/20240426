# Comparing `tmp/ping-multi-ext-1.0.9.tar.gz` & `tmp/ping_multi_ext-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ping-multi-ext-1.0.9.tar", last modified: Wed Apr  3 06:42:21 2024, max compression
+gzip compressed data, was "ping_multi_ext-1.1.0.tar", last modified: Fri Apr 26 06:05:50 2024, max compression
```

## Comparing `ping-multi-ext-1.0.9.tar` & `ping_multi_ext-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 famzah    (1000) famzah    (1000)        0 2024-04-03 06:42:21.571717 ping-multi-ext-1.0.9/
--rw-rw-r--   0 famzah    (1000) famzah    (1000)     1070 2021-06-01 07:49:05.000000 ping-multi-ext-1.0.9/LICENSE
--rw-r--r--   0 famzah    (1000) famzah    (1000)     4796 2024-04-03 06:42:21.571717 ping-multi-ext-1.0.9/PKG-INFO
--rw-rw-r--   0 famzah    (1000) famzah    (1000)     3535 2023-03-09 20:51:20.000000 ping-multi-ext-1.0.9/README.rst
-drwxrwxr-x   0 famzah    (1000) famzah    (1000)        0 2024-04-03 06:42:21.571717 ping-multi-ext-1.0.9/ping_multi_ext/
--rw-rw-r--   0 famzah    (1000) famzah    (1000)       18 2024-04-03 06:23:28.000000 ping-multi-ext-1.0.9/ping_multi_ext/__init__.py
--rw-rw-r--   0 famzah    (1000) famzah    (1000)     1816 2024-04-02 19:00:13.000000 ping-multi-ext-1.0.9/ping_multi_ext/cmd_multi.py
--rw-rw-r--   0 famzah    (1000) famzah    (1000)      745 2024-04-02 18:50:02.000000 ping-multi-ext-1.0.9/ping_multi_ext/cmd_raw.py
--rw-rw-r--   0 famzah    (1000) famzah    (1000)    23408 2024-04-02 19:06:57.000000 ping-multi-ext-1.0.9/ping_multi_ext/core.py
--rw-rw-r--   0 famzah    (1000) famzah    (1000)     1439 2024-04-02 19:00:40.000000 ping-multi-ext-1.0.9/ping_multi_ext/lib.py
--rw-rw-r--   0 famzah    (1000) famzah    (1000)     8939 2021-06-15 07:20:19.000000 ping-multi-ext-1.0.9/ping_multi_ext/proc.py
-drwxrwxr-x   0 famzah    (1000) famzah    (1000)        0 2024-04-03 06:42:21.571717 ping-multi-ext-1.0.9/ping_multi_ext.egg-info/
--rw-r--r--   0 famzah    (1000) famzah    (1000)     4796 2024-04-03 06:42:21.000000 ping-multi-ext-1.0.9/ping_multi_ext.egg-info/PKG-INFO
--rw-rw-r--   0 famzah    (1000) famzah    (1000)      416 2024-04-03 06:42:21.000000 ping-multi-ext-1.0.9/ping_multi_ext.egg-info/SOURCES.txt
--rw-rw-r--   0 famzah    (1000) famzah    (1000)        1 2024-04-03 06:42:21.000000 ping-multi-ext-1.0.9/ping_multi_ext.egg-info/dependency_links.txt
--rw-rw-r--   0 famzah    (1000) famzah    (1000)      106 2024-04-03 06:42:21.000000 ping-multi-ext-1.0.9/ping_multi_ext.egg-info/entry_points.txt
--rw-rw-r--   0 famzah    (1000) famzah    (1000)       19 2024-04-03 06:42:21.000000 ping-multi-ext-1.0.9/ping_multi_ext.egg-info/requires.txt
--rw-rw-r--   0 famzah    (1000) famzah    (1000)       15 2024-04-03 06:42:21.000000 ping-multi-ext-1.0.9/ping_multi_ext.egg-info/top_level.txt
--rw-rw-r--   0 famzah    (1000) famzah    (1000)       74 2024-04-03 06:42:21.571717 ping-multi-ext-1.0.9/setup.cfg
--rw-rw-r--   0 famzah    (1000) famzah    (1000)     3430 2021-06-15 07:53:46.000000 ping-multi-ext-1.0.9/setup.py
+drwxrwxr-x   0 famzah    (1000) famzah    (1000)        0 2024-04-26 06:05:50.317210 ping_multi_ext-1.1.0/
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)     1070 2021-06-01 07:49:05.000000 ping_multi_ext-1.1.0/LICENSE
+-rw-r--r--   0 famzah    (1000) famzah    (1000)     5350 2024-04-26 06:05:50.317210 ping_multi_ext-1.1.0/PKG-INFO
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)     4089 2024-04-07 20:53:38.000000 ping_multi_ext-1.1.0/README.rst
+drwxrwxr-x   0 famzah    (1000) famzah    (1000)        0 2024-04-26 06:05:50.317210 ping_multi_ext-1.1.0/ping_multi_ext/
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)       18 2024-04-26 06:03:39.000000 ping_multi_ext-1.1.0/ping_multi_ext/__init__.py
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)     2894 2024-04-21 06:15:35.000000 ping_multi_ext-1.1.0/ping_multi_ext/cmd_multi.py
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)      745 2024-04-02 18:50:02.000000 ping_multi_ext-1.1.0/ping_multi_ext/cmd_raw.py
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)    23408 2024-04-02 19:06:57.000000 ping_multi_ext-1.1.0/ping_multi_ext/core.py
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)     2358 2024-04-15 07:27:05.000000 ping_multi_ext-1.1.0/ping_multi_ext/lib.py
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)     8939 2021-06-15 07:20:19.000000 ping_multi_ext-1.1.0/ping_multi_ext/proc.py
+drwxrwxr-x   0 famzah    (1000) famzah    (1000)        0 2024-04-26 06:05:50.317210 ping_multi_ext-1.1.0/ping_multi_ext.egg-info/
+-rw-r--r--   0 famzah    (1000) famzah    (1000)     5350 2024-04-26 06:05:50.000000 ping_multi_ext-1.1.0/ping_multi_ext.egg-info/PKG-INFO
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)      416 2024-04-26 06:05:50.000000 ping_multi_ext-1.1.0/ping_multi_ext.egg-info/SOURCES.txt
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)        1 2024-04-26 06:05:50.000000 ping_multi_ext-1.1.0/ping_multi_ext.egg-info/dependency_links.txt
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)      106 2024-04-26 06:05:50.000000 ping_multi_ext-1.1.0/ping_multi_ext.egg-info/entry_points.txt
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)       19 2024-04-26 06:05:50.000000 ping_multi_ext-1.1.0/ping_multi_ext.egg-info/requires.txt
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)       15 2024-04-26 06:05:50.000000 ping_multi_ext-1.1.0/ping_multi_ext.egg-info/top_level.txt
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)       74 2024-04-26 06:05:50.317210 ping_multi_ext-1.1.0/setup.cfg
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)     3430 2021-06-15 07:53:46.000000 ping_multi_ext-1.1.0/setup.py
```

### Comparing `ping-multi-ext-1.0.9/LICENSE` & `ping_multi_ext-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ping-multi-ext-1.0.9/PKG-INFO` & `ping_multi_ext-1.1.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: ping-multi-ext
-Version: 1.0.9
-Summary: Interactively ping one or many hosts from one or multiple locations (locally or via SSH)
-Home-page: https://github.com/famzah/ping-multi-ext
-Author: Ivan Zahariev (famzah)
-Project-URL: Bug Reports, https://github.com/famzah/ping-multi-ext/issues
-Project-URL: Source, https://github.com/famzah/ping-multi-ext
-Keywords: ping,multi,console,ssh,terminal,interactive
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Internet
-Classifier: Topic :: System :: Networking :: Monitoring
-Classifier: Topic :: Terminals
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6, <4
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: blessings
-Requires-Dist: curtsies
-
 ping-multi-ext
 **************
 
 This tool lets you interactively ping:
 
 * **One** host from **multiple** locations (via SSH)
 * **Multiple** hosts from **one** location (local machine, or remote via SSH)
@@ -98,26 +68,38 @@
 
   ping-multi google.com github.com github.com@root@my-server.com
 
 Ping multiple hosts specified in a file; you can also add more single hosts directly as additional command-line arguments: ::
 
   ping-multi -f sample.list
   
+IPv4 CIDR masks are supported: ::
+
+  ping-multi 192.168.0.0/30
+
 The usage help explains the additional command-line options: ::
 
   $ ping-multi -h
   
-  usage: ping-multi [-h] [--version] [-W,--wait SECS] [-i,--interval SECS] [-f,--file FILE] [--hosts-max-width HOSTS_MAX_WIDTH] [host [host ...]]
+  usage: ping-multi [-h] [--version] [--hosts-max-width HOSTS_MAX_WIDTH] [-s {Last,Loss%,Avg,Min,Max,StDev,RX_cnt,TX_cnt,XX_cnt}] [-f FILE]
+                    [-W SECS] [-i SECS] [-L COUNT_LIMIT] [-C]
+                    [host ...]
   
   Ping all hosts from FILE and HOSTs.
   
   positional arguments:
     host                  host to ping; you can specify this option many times
   
-  optional arguments:
+  options:
     -h, --help            show this help message and exit
     --version             show program's version number and exit
-    -W,--wait SECS        timeout in seconds to wait for a ping reply; default=1
-    -i,--interval SECS    time in seconds between sending each request; default=1
-    -f,--file FILE        read list of hosts from file
     --hosts-max-width HOSTS_MAX_WIDTH
                           maximum width of the hosts column; default=0
+    -s {Last,Loss%,Avg,Min,Max,StDev,RX_cnt,TX_cnt,XX_cnt}, --stat {Last,Loss%,Avg,Min,Max,StDev,RX_cnt,TX_cnt,XX_cnt}
+                          statistic to display initially; default=Last
+    -f FILE, --file FILE  read list of hosts from file
+    -W SECS, --wait SECS  timeout in seconds to wait for a ping reply; default=1
+    -i SECS, --interval SECS
+                          time in seconds between sending each request; default=1
+    -L COUNT_LIMIT, --count-limit COUNT_LIMIT
+                          limit the number of hosts; avoids unintended bulk actions; default=600
+    -C, --cidr-debug      debug IPv4 CIDR expansion
```

### Comparing `ping-multi-ext-1.0.9/ping_multi_ext/cmd_raw.py` & `ping_multi_ext-1.1.0/ping_multi_ext/cmd_raw.py`

 * *Files identical despite different names*

### Comparing `ping-multi-ext-1.0.9/ping_multi_ext/core.py` & `ping_multi_ext-1.1.0/ping_multi_ext/core.py`

 * *Files identical despite different names*

### Comparing `ping-multi-ext-1.0.9/ping_multi_ext/proc.py` & `ping_multi_ext-1.1.0/ping_multi_ext/proc.py`

 * *Files identical despite different names*

### Comparing `ping-multi-ext-1.0.9/ping_multi_ext.egg-info/PKG-INFO` & `ping_multi_ext-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ping-multi-ext
-Version: 1.0.9
+Version: 1.1.0
 Summary: Interactively ping one or many hosts from one or multiple locations (locally or via SSH)
 Home-page: https://github.com/famzah/ping-multi-ext
 Author: Ivan Zahariev (famzah)
 Project-URL: Bug Reports, https://github.com/famzah/ping-multi-ext/issues
 Project-URL: Source, https://github.com/famzah/ping-multi-ext
 Keywords: ping,multi,console,ssh,terminal,interactive
 Classifier: Development Status :: 5 - Production/Stable
@@ -98,26 +98,38 @@
 
   ping-multi google.com github.com github.com@root@my-server.com
 
 Ping multiple hosts specified in a file; you can also add more single hosts directly as additional command-line arguments: ::
 
   ping-multi -f sample.list
   
+IPv4 CIDR masks are supported: ::
+
+  ping-multi 192.168.0.0/30
+
 The usage help explains the additional command-line options: ::
 
   $ ping-multi -h
   
-  usage: ping-multi [-h] [--version] [-W,--wait SECS] [-i,--interval SECS] [-f,--file FILE] [--hosts-max-width HOSTS_MAX_WIDTH] [host [host ...]]
+  usage: ping-multi [-h] [--version] [--hosts-max-width HOSTS_MAX_WIDTH] [-s {Last,Loss%,Avg,Min,Max,StDev,RX_cnt,TX_cnt,XX_cnt}] [-f FILE]
+                    [-W SECS] [-i SECS] [-L COUNT_LIMIT] [-C]
+                    [host ...]
   
   Ping all hosts from FILE and HOSTs.
   
   positional arguments:
     host                  host to ping; you can specify this option many times
   
-  optional arguments:
+  options:
     -h, --help            show this help message and exit
     --version             show program's version number and exit
-    -W,--wait SECS        timeout in seconds to wait for a ping reply; default=1
-    -i,--interval SECS    time in seconds between sending each request; default=1
-    -f,--file FILE        read list of hosts from file
     --hosts-max-width HOSTS_MAX_WIDTH
                           maximum width of the hosts column; default=0
+    -s {Last,Loss%,Avg,Min,Max,StDev,RX_cnt,TX_cnt,XX_cnt}, --stat {Last,Loss%,Avg,Min,Max,StDev,RX_cnt,TX_cnt,XX_cnt}
+                          statistic to display initially; default=Last
+    -f FILE, --file FILE  read list of hosts from file
+    -W SECS, --wait SECS  timeout in seconds to wait for a ping reply; default=1
+    -i SECS, --interval SECS
+                          time in seconds between sending each request; default=1
+    -L COUNT_LIMIT, --count-limit COUNT_LIMIT
+                          limit the number of hosts; avoids unintended bulk actions; default=600
+    -C, --cidr-debug      debug IPv4 CIDR expansion
```

### Comparing `ping-multi-ext-1.0.9/setup.py` & `ping_multi_ext-1.1.0/setup.py`

 * *Files identical despite different names*

