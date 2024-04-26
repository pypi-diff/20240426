# Comparing `tmp/etcetra-0.1.8.tar.gz` & `tmp/etcetra-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etcetra-0.1.8.tar", last modified: Fri Jun 24 04:33:38 2022, max compression
+gzip compressed data, was "etcetra-0.1.9.tar", last modified: Mon Aug  1 12:10:40 2022, max compression
```

## Comparing `etcetra-0.1.8.tar` & `etcetra-0.1.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 04:33:38.274180 etcetra-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    10947 2022-06-24 04:33:12.000000 etcetra-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7896 2022-06-24 04:33:38.274180 etcetra-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6833 2022-06-24 04:33:12.000000 etcetra-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2224 2022-06-24 04:33:38.274180 etcetra-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-24 04:33:12.000000 etcetra-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 04:33:38.266180 etcetra-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 04:33:38.266180 etcetra-0.1.8/src/etcetra/
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    62492 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 04:33:38.274180 etcetra-0.1.8/src/etcetra/grpc_api/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/annotations_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/annotations_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3219 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2090 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/code_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/code_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     8167 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/error_details_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/error_details_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5389 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/etcdserver_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/etcdserver_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    21714 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/gogo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/gogo_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2940 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/http_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/http_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1685 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/httpbody_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/httpbody_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2367 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/kv_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/kv_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4497 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/membership_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/membership_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     6179 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/raft_internal_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/raft_internal_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    75958 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/rpc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    68049 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/rpc_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/snap_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/snap_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1619 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     7878 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/v3election_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     8932 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/v3election_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3769 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/v3lock_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     4368 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/grpc_api/v3lock_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     4697 2022-06-24 04:33:12.000000 etcetra-0.1.8/src/etcetra/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 04:33:38.270180 etcetra-0.1.8/src/etcetra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7896 2022-06-24 04:33:37.000000 etcetra-0.1.8/src/etcetra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-06-24 04:33:38.000000 etcetra-0.1.8/src/etcetra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 04:33:37.000000 etcetra-0.1.8/src/etcetra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 04:33:34.000000 etcetra-0.1.8/src/etcetra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-06-24 04:33:37.000000 etcetra-0.1.8/src/etcetra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-24 04:33:38.000000 etcetra-0.1.8/src/etcetra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 12:10:40.218338 etcetra-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    10947 2022-08-01 12:10:26.000000 etcetra-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     7896 2022-08-01 12:10:40.218338 etcetra-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6833 2022-08-01 12:10:26.000000 etcetra-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2224 2022-08-01 12:10:40.222338 etcetra-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-01 12:10:26.000000 etcetra-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 12:10:40.214338 etcetra-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 12:10:40.214338 etcetra-0.1.9/src/etcetra/
+-rw-r--r--   0 runner    (1001) docker     (121)      203 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    62492 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 12:10:40.218338 etcetra-0.1.9/src/etcetra/grpc_api/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/annotations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/annotations_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3219 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2090 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/code_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/code_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8167 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/error_details_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/error_details_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5389 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/etcdserver_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/etcdserver_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21714 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/gogo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/gogo_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2940 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/http_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/http_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1685 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/httpbody_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/httpbody_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2367 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/kv_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/kv_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4497 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/membership_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/membership_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6179 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/raft_internal_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/raft_internal_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    75958 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/rpc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68049 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/rpc_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/snap_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/snap_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1619 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7878 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/v3election_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8932 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/v3election_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3769 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/v3lock_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4368 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/grpc_api/v3lock_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     4697 2022-08-01 12:10:26.000000 etcetra-0.1.9/src/etcetra/types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 12:10:40.214338 etcetra-0.1.9/src/etcetra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7896 2022-08-01 12:10:40.000000 etcetra-0.1.9/src/etcetra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-08-01 12:10:40.000000 etcetra-0.1.9/src/etcetra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-01 12:10:40.000000 etcetra-0.1.9/src/etcetra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-01 12:10:39.000000 etcetra-0.1.9/src/etcetra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      287 2022-08-01 12:10:40.000000 etcetra-0.1.9/src/etcetra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-01 12:10:40.000000 etcetra-0.1.9/src/etcetra.egg-info/top_level.txt
```

### Comparing `etcetra-0.1.8/LICENSE` & `etcetra-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/PKG-INFO` & `etcetra-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etcetra
-Version: 0.1.8
+Version: 0.1.9
 Summary: Etcd client built with pure asyncio gRPC library
 Home-page: https://github.com/lablup/etcetra
 Author: Lablup Inc.
 Author-email: kyujin.cho@lablup.com
 License: Apache License 2.0
 Project-URL: Documentation, https://github.com/lablup/etcetra/blob/main/docs/references.md
 Project-URL: Source, https://github.com/lablup/etcetra
```

### Comparing `etcetra-0.1.8/README.md` & `etcetra-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/setup.cfg` & `etcetra-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 	= src
 packages = find_namespace:
 python_requires = >=3.9
 setup_requires = 
 	setuptools>=51.1.1
 	wheel>=0.36.2
 install_requires = 
-	grpcio~=1.47.0
-	grpcio-tools~=1.47.0
+	grpcio~=1.48.0
+	grpcio-tools~=1.48.0
 	async-timeout~=4.0.0
 zip_safe = false
 include_package_data = true
 
 [options.extras_require]
 build = 
 	wheel>=0.36.2
```

### Comparing `etcetra-0.1.8/src/etcetra/client.py` & `etcetra-0.1.9/src/etcetra/client.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/annotations_pb2.py` & `etcetra-0.1.9/src/etcetra/grpc_api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/auth_pb2.py` & `etcetra-0.1.9/src/etcetra/grpc_api/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/code_pb2.py` & `etcetra-0.1.9/src/etcetra/grpc_api/code_pb2.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/error_details_pb2.py` & `etcetra-0.1.9/src/etcetra/grpc_api/error_details_pb2.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/etcdserver_pb2.py` & `etcetra-0.1.9/src/etcetra/grpc_api/etcdserver_pb2.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/gogo_pb2.py` & `etcetra-0.1.9/src/etcetra/grpc_api/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/http_pb2.py` & `etcetra-0.1.9/src/etcetra/grpc_api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/httpbody_pb2.py` & `etcetra-0.1.9/src/etcetra/grpc_api/httpbody_pb2.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/kv_pb2.py` & `etcetra-0.1.9/src/etcetra/grpc_api/kv_pb2.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/membership_pb2.py` & `etcetra-0.1.9/src/etcetra/grpc_api/membership_pb2.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/raft_internal_pb2.py` & `etcetra-0.1.9/src/etcetra/grpc_api/raft_internal_pb2.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/rpc_pb2.py` & `etcetra-0.1.9/src/etcetra/grpc_api/rpc_pb2.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/rpc_pb2_grpc.py` & `etcetra-0.1.9/src/etcetra/grpc_api/rpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/snap_pb2.py` & `etcetra-0.1.9/src/etcetra/grpc_api/snap_pb2.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/status_pb2.py` & `etcetra-0.1.9/src/etcetra/grpc_api/status_pb2.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/v3election_pb2.py` & `etcetra-0.1.9/src/etcetra/grpc_api/v3election_pb2.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/v3election_pb2_grpc.py` & `etcetra-0.1.9/src/etcetra/grpc_api/v3election_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/v3lock_pb2.py` & `etcetra-0.1.9/src/etcetra/grpc_api/v3lock_pb2.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/grpc_api/v3lock_pb2_grpc.py` & `etcetra-0.1.9/src/etcetra/grpc_api/v3lock_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra/types.py` & `etcetra-0.1.9/src/etcetra/types.py`

 * *Files identical despite different names*

### Comparing `etcetra-0.1.8/src/etcetra.egg-info/PKG-INFO` & `etcetra-0.1.9/src/etcetra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etcetra
-Version: 0.1.8
+Version: 0.1.9
 Summary: Etcd client built with pure asyncio gRPC library
 Home-page: https://github.com/lablup/etcetra
 Author: Lablup Inc.
 Author-email: kyujin.cho@lablup.com
 License: Apache License 2.0
 Project-URL: Documentation, https://github.com/lablup/etcetra/blob/main/docs/references.md
 Project-URL: Source, https://github.com/lablup/etcetra
```

### Comparing `etcetra-0.1.8/src/etcetra.egg-info/SOURCES.txt` & `etcetra-0.1.9/src/etcetra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

