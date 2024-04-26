# Comparing `tmp/wled2graph-0.1.1.tar.gz` & `tmp/wled2graph-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wled2graph-0.1.1.tar", max compression
+gzip compressed data, was "wled2graph-0.1.2.tar", max compression
```

## Comparing `wled2graph-0.1.1.tar` & `wled2graph-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1093 2024-02-12 03:01:36.201017 wled2graph-0.1.1/license.md
--rw-r--r--   0        0        0      552 2024-04-26 03:12:53.232104 wled2graph-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3754 2024-04-26 03:07:51.253606 wled2graph-0.1.1/readme.md
--rw-r--r--   0        0        0        0 2024-04-26 03:07:51.254552 wled2graph-0.1.1/wled2graph/__init__.py
--rw-r--r--   0        0        0     2545 2024-04-26 03:07:51.256631 wled2graph-0.1.1/wled2graph/args.py
--rw-r--r--   0        0        0     9212 2024-04-26 03:07:51.258332 wled2graph-0.1.1/wled2graph/graphs.py
--rw-r--r--   0        0        0      723 2024-04-26 03:07:51.260240 wled2graph-0.1.1/wled2graph/main.py
--rw-r--r--   0        0        0      837 2024-04-26 03:07:51.261282 wled2graph-0.1.1/wled2graph/template.py
--rw-r--r--   0        0        0     1614 2024-04-26 03:07:51.262269 wled2graph-0.1.1/wled2graph/utils.py
--rw-r--r--   0        0        0     2263 2024-04-26 03:07:51.264226 wled2graph-0.1.1/wled2graph/wled.py
--rw-r--r--   0        0        0     4407 1970-01-01 00:00:00.000000 wled2graph-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-02-12 03:01:36.201017 wled2graph-0.1.2/license.md
+-rw-r--r--   0        0        0      552 2024-04-26 03:29:33.733117 wled2graph-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3828 2024-04-26 03:29:06.416913 wled2graph-0.1.2/readme.md
+-rw-r--r--   0        0        0        0 2024-04-26 03:07:51.254552 wled2graph-0.1.2/wled2graph/__init__.py
+-rw-r--r--   0        0        0     2545 2024-04-26 03:07:51.256631 wled2graph-0.1.2/wled2graph/args.py
+-rw-r--r--   0        0        0     9212 2024-04-26 03:07:51.258332 wled2graph-0.1.2/wled2graph/graphs.py
+-rw-r--r--   0        0        0      723 2024-04-26 03:07:51.260240 wled2graph-0.1.2/wled2graph/main.py
+-rw-r--r--   0        0        0      837 2024-04-26 03:07:51.261282 wled2graph-0.1.2/wled2graph/template.py
+-rw-r--r--   0        0        0     1614 2024-04-26 03:07:51.262269 wled2graph-0.1.2/wled2graph/utils.py
+-rw-r--r--   0        0        0     2263 2024-04-26 03:07:51.264226 wled2graph-0.1.2/wled2graph/wled.py
+-rw-r--r--   0        0        0     4481 1970-01-01 00:00:00.000000 wled2graph-0.1.2/PKG-INFO
```

### Comparing `wled2graph-0.1.1/license.md` & `wled2graph-0.1.2/license.md`

 * *Files identical despite different names*

### Comparing `wled2graph-0.1.1/pyproject.toml` & `wled2graph-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wled2graph"
-version = "0.1.1"
+version = "0.1.2"
 description = "wled2graph supports a table and graphs of FPS and other data from multiple WLED endpoints in real-time via a browser interface"
 authors = ["bigredfrog <big.red.frog@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `wled2graph-0.1.1/readme.md` & `wled2graph-0.1.2/readme.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# WLED2Graph
+# wled2graph
 
-WLED2Graph is a Python program designed to visualize Frames Per Second (FPS) data and other from WLED endpoints on a network in real-time using a Bokeh graph server. It sets up a polling loop, defaulting to every 5 seconds, to fetch the current JSON state from each specified WLED endpoint
+wled2graph is a Python program designed to visualize Frames Per Second (FPS) data and other from WLED endpoints on a network in real-time using a Bokeh graph server. It sets up a polling loop, defaulting to every 5 seconds, to fetch the current JSON state from each specified WLED endpoint
 
-![WLED2Graph](wled2graph.png)
+![wled2graph screenshot](https://raw.githubusercontent.com/bigredfrog/wled2graph/master/wled2graph.png)
 
 ## Features
 
 - **Real-time FPS, BSSID, RSSI and Ping Visualization**: Continuously polls WLED endpoints and updates the graph with current FPS values.
 - **IP address hyperlink to WLED UI**: Just click through direct to the WLED UI for the selected WLED endpoint.
 - **Configurable Polling Frequency**: Allows customization of the polling interval to suit network and performance needs.
 - **Scalable**: Can monitor multiple WLED endpoints simultaneously.
```

### Comparing `wled2graph-0.1.1/wled2graph/args.py` & `wled2graph-0.1.2/wled2graph/args.py`

 * *Files identical despite different names*

### Comparing `wled2graph-0.1.1/wled2graph/graphs.py` & `wled2graph-0.1.2/wled2graph/graphs.py`

 * *Files identical despite different names*

### Comparing `wled2graph-0.1.1/wled2graph/main.py` & `wled2graph-0.1.2/wled2graph/main.py`

 * *Files identical despite different names*

### Comparing `wled2graph-0.1.1/wled2graph/template.py` & `wled2graph-0.1.2/wled2graph/template.py`

 * *Files identical despite different names*

### Comparing `wled2graph-0.1.1/wled2graph/utils.py` & `wled2graph-0.1.2/wled2graph/utils.py`

 * *Files identical despite different names*

### Comparing `wled2graph-0.1.1/wled2graph/wled.py` & `wled2graph-0.1.2/wled2graph/wled.py`

 * *Files identical despite different names*

### Comparing `wled2graph-0.1.1/PKG-INFO` & `wled2graph-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wled2graph
-Version: 0.1.1
+Version: 0.1.2
 Summary: wled2graph supports a table and graphs of FPS and other data from multiple WLED endpoints in real-time via a browser interface
 License: MIT
 Author: bigredfrog
 Author-email: big.red.frog@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,19 +13,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: bokeh (>=3.3.4,<4.0.0)
 Requires-Dist: icmplib (>=3.0.4,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
-# WLED2Graph
+# wled2graph
 
-WLED2Graph is a Python program designed to visualize Frames Per Second (FPS) data and other from WLED endpoints on a network in real-time using a Bokeh graph server. It sets up a polling loop, defaulting to every 5 seconds, to fetch the current JSON state from each specified WLED endpoint
+wled2graph is a Python program designed to visualize Frames Per Second (FPS) data and other from WLED endpoints on a network in real-time using a Bokeh graph server. It sets up a polling loop, defaulting to every 5 seconds, to fetch the current JSON state from each specified WLED endpoint
 
-![WLED2Graph](wled2graph.png)
+![wled2graph screenshot](https://raw.githubusercontent.com/bigredfrog/wled2graph/master/wled2graph.png)
 
 ## Features
 
 - **Real-time FPS, BSSID, RSSI and Ping Visualization**: Continuously polls WLED endpoints and updates the graph with current FPS values.
 - **IP address hyperlink to WLED UI**: Just click through direct to the WLED UI for the selected WLED endpoint.
 - **Configurable Polling Frequency**: Allows customization of the polling interval to suit network and performance needs.
 - **Scalable**: Can monitor multiple WLED endpoints simultaneously.
```

