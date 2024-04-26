# Comparing `tmp/rtorrent_rpc-0.5.2.tar.gz` & `tmp/rtorrent_rpc-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.5.2.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.6.0.tar", max compression
```

## Comparing `rtorrent_rpc-0.5.2.tar` & `rtorrent_rpc-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1084 2024-04-25 13:49:14.410746 rtorrent_rpc-0.5.2/LICENSE
--rw-r--r--   0        0        0     2456 2024-04-25 13:49:14.414746 rtorrent_rpc-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1406 2024-04-25 13:49:14.414746 rtorrent_rpc-0.5.2/readme.md
--rw-r--r--   0        0        0    29423 2024-04-25 13:49:14.414746 rtorrent_rpc-0.5.2/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     2327 2024-04-25 13:49:14.414746 rtorrent_rpc-0.5.2/rtorrent_rpc/_jsonrpc/__init__.py
--rw-r--r--   0        0        0     3050 2024-04-25 13:49:14.414746 rtorrent_rpc-0.5.2/rtorrent_rpc/_jsonrpc/transport.py
--rw-r--r--   0        0        0     1235 2024-04-25 13:49:14.414746 rtorrent_rpc-0.5.2/rtorrent_rpc/_scgi.py
--rw-r--r--   0        0        0      803 2024-04-25 13:49:14.414746 rtorrent_rpc-0.5.2/rtorrent_rpc/_transport.py
--rw-r--r--   0        0        0     2943 2024-04-25 13:49:14.414746 rtorrent_rpc-0.5.2/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0        0 2024-04-25 13:49:14.414746 rtorrent_rpc-0.5.2/rtorrent_rpc/py.typed
--rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 rtorrent_rpc-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-26 15:42:43.509531 rtorrent_rpc-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2456 2024-04-26 15:42:43.513531 rtorrent_rpc-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1436 2024-04-26 15:42:43.513531 rtorrent_rpc-0.6.0/readme.md
+-rw-r--r--   0        0        0    29423 2024-04-26 15:42:43.513531 rtorrent_rpc-0.6.0/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2327 2024-04-26 15:42:43.513531 rtorrent_rpc-0.6.0/rtorrent_rpc/_jsonrpc/__init__.py
+-rw-r--r--   0        0        0     3050 2024-04-26 15:42:43.513531 rtorrent_rpc-0.6.0/rtorrent_rpc/_jsonrpc/transport.py
+-rw-r--r--   0        0        0     1235 2024-04-26 15:42:43.513531 rtorrent_rpc-0.6.0/rtorrent_rpc/_scgi.py
+-rw-r--r--   0        0        0      803 2024-04-26 15:42:43.513531 rtorrent_rpc-0.6.0/rtorrent_rpc/_transport.py
+-rw-r--r--   0        0        0     3694 2024-04-26 15:42:43.513531 rtorrent_rpc-0.6.0/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:42:43.513531 rtorrent_rpc-0.6.0/rtorrent_rpc/py.typed
+-rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 rtorrent_rpc-0.6.0/PKG-INFO
```

### Comparing `rtorrent_rpc-0.5.2/LICENSE` & `rtorrent_rpc-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.5.2/pyproject.toml` & `rtorrent_rpc-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.5.2"
+version = "0.6.0"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
```

### Comparing `rtorrent_rpc-0.5.2/readme.md` & `rtorrent_rpc-0.6.0/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,23 +23,23 @@
 ```python
 from rtorrent_rpc import RTorrent
 
 client = RTorrent(address='scgi://127.0.0.1:5000')
 unix_client = RTorrent(address='scgi:///home/ubuntu/.local/share/rtorrent.sock')
 ```
 
-## Known problem:
+## Known Problem
 
 rTorrent's [xmlrpc do not support all utf8 characters](https://github.com/rakshasa/rtorrent/issues/1250), for example, emoji.
 
 If torrent name of file name contains any emoji,
-you can't retrieve correct torrent name of file name through xmlrpc.
+you can't retrieve correct torrent name or file name through xmlrpc.
 
 Please consider use a rtorrent distro with json-rpc support,
-for example: [jesec/rtorrent](https://github.com/jesec/rtorrent)
+for example: [jesec/rtorrent](https://github.com/jesec/rtorrent), which support utf8 correctly.
 
 If your rtorrent distro support jsonrpc,
 you can use send json-rpc request with `RTorrent(...).jsonrpc.call(...)`.
 
 ## License
 
 `rtorrent-rpc` is licensed under the MIT license.
```

### Comparing `rtorrent_rpc-0.5.2/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.6.0/rtorrent_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.5.2/rtorrent_rpc/_jsonrpc/__init__.py` & `rtorrent_rpc-0.6.0/rtorrent_rpc/_jsonrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.5.2/rtorrent_rpc/_jsonrpc/transport.py` & `rtorrent_rpc-0.6.0/rtorrent_rpc/_jsonrpc/transport.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.5.2/rtorrent_rpc/_scgi.py` & `rtorrent_rpc-0.6.0/rtorrent_rpc/_scgi.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.5.2/rtorrent_rpc/_transport.py` & `rtorrent_rpc-0.6.0/rtorrent_rpc/_transport.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.5.2/PKG-INFO` & `rtorrent_rpc-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.5.2
+Version: 0.6.0
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.8,<4.0
@@ -49,23 +49,23 @@
 ```python
 from rtorrent_rpc import RTorrent
 
 client = RTorrent(address='scgi://127.0.0.1:5000')
 unix_client = RTorrent(address='scgi:///home/ubuntu/.local/share/rtorrent.sock')
 ```
 
-## Known problem:
+## Known Problem
 
 rTorrent's [xmlrpc do not support all utf8 characters](https://github.com/rakshasa/rtorrent/issues/1250), for example, emoji.
 
 If torrent name of file name contains any emoji,
-you can't retrieve correct torrent name of file name through xmlrpc.
+you can't retrieve correct torrent name or file name through xmlrpc.
 
 Please consider use a rtorrent distro with json-rpc support,
-for example: [jesec/rtorrent](https://github.com/jesec/rtorrent)
+for example: [jesec/rtorrent](https://github.com/jesec/rtorrent), which support utf8 correctly.
 
 If your rtorrent distro support jsonrpc,
 you can use send json-rpc request with `RTorrent(...).jsonrpc.call(...)`.
 
 ## License
 
 `rtorrent-rpc` is licensed under the MIT license.
```

