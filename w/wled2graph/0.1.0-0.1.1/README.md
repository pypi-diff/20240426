# Comparing `tmp/wled2graph-0.1.0.tar.gz` & `tmp/wled2graph-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wled2graph-0.1.0.tar", max compression
+gzip compressed data, was "wled2graph-0.1.1.tar", max compression
```

## Comparing `wled2graph-0.1.0.tar` & `wled2graph-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1093 2024-02-12 03:01:36.201017 wled2graph-0.1.0/license.md
--rw-r--r--   0        0        0      426 2024-04-26 02:06:38.044716 wled2graph-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2748 2024-04-26 01:46:09.063120 wled2graph-0.1.0/readme.md
--rw-r--r--   0        0        0        0 2024-04-26 01:57:53.110281 wled2graph-0.1.0/wled2graph/__init__.py
--rw-r--r--   0        0        0     2545 2024-04-26 01:13:38.085503 wled2graph-0.1.0/wled2graph/args.py
--rw-r--r--   0        0        0     9212 2024-04-26 02:18:46.697627 wled2graph-0.1.0/wled2graph/graphs.py
--rw-r--r--   0        0        0      723 2024-04-26 02:16:47.871264 wled2graph-0.1.0/wled2graph/main.py
--rw-r--r--   0        0        0      837 2024-04-26 01:13:38.126910 wled2graph-0.1.0/wled2graph/template.py
--rw-r--r--   0        0        0     1614 2024-02-15 01:56:58.599653 wled2graph-0.1.0/wled2graph/utils.py
--rw-r--r--   0        0        0     2263 2024-04-26 01:13:38.137907 wled2graph-0.1.0/wled2graph/wled.py
--rw-r--r--   0        0        0   382558 2024-04-26 01:46:09.080448 wled2graph-0.1.0/wled2graph/wled2graph.png
--rw-r--r--   0        0        0     3304 1970-01-01 00:00:00.000000 wled2graph-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-02-12 03:01:36.201017 wled2graph-0.1.1/license.md
+-rw-r--r--   0        0        0      552 2024-04-26 03:12:53.232104 wled2graph-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3754 2024-04-26 03:07:51.253606 wled2graph-0.1.1/readme.md
+-rw-r--r--   0        0        0        0 2024-04-26 03:07:51.254552 wled2graph-0.1.1/wled2graph/__init__.py
+-rw-r--r--   0        0        0     2545 2024-04-26 03:07:51.256631 wled2graph-0.1.1/wled2graph/args.py
+-rw-r--r--   0        0        0     9212 2024-04-26 03:07:51.258332 wled2graph-0.1.1/wled2graph/graphs.py
+-rw-r--r--   0        0        0      723 2024-04-26 03:07:51.260240 wled2graph-0.1.1/wled2graph/main.py
+-rw-r--r--   0        0        0      837 2024-04-26 03:07:51.261282 wled2graph-0.1.1/wled2graph/template.py
+-rw-r--r--   0        0        0     1614 2024-04-26 03:07:51.262269 wled2graph-0.1.1/wled2graph/utils.py
+-rw-r--r--   0        0        0     2263 2024-04-26 03:07:51.264226 wled2graph-0.1.1/wled2graph/wled.py
+-rw-r--r--   0        0        0     4407 1970-01-01 00:00:00.000000 wled2graph-0.1.1/PKG-INFO
```

### Comparing `wled2graph-0.1.0/license.md` & `wled2graph-0.1.1/license.md`

 * *Files identical despite different names*

### Comparing `wled2graph-0.1.0/readme.md` & `wled2graph-0.1.1/readme.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,23 +8,52 @@
 
 - **Real-time FPS, BSSID, RSSI and Ping Visualization**: Continuously polls WLED endpoints and updates the graph with current FPS values.
 - **IP address hyperlink to WLED UI**: Just click through direct to the WLED UI for the selected WLED endpoint.
 - **Configurable Polling Frequency**: Allows customization of the polling interval to suit network and performance needs.
 - **Scalable**: Can monitor multiple WLED endpoints simultaneously.
 - **Customizable Data Points Rollover**: Supports setting a maximum number of data points to display on the graph, after which old data points are rolled off.
 
+
+## Installation from PyPi
+
+```bash
+pip install wled2graph
+```
+
+WLED2Graph is executed from the command line and requires a list of IP addresses corresponding to the WLED endpoints you wish to monitor.
+
+```bash
+wled2graph -w <WLED_IPs> [-t <time_period>] [-r <rollover>]
+```
+
+-w, --wleds: A comma-separated list of IP addresses for the WLED endpoints.  
+-t, --time-period: (Optional) The time period in seconds for polling the WLEDs. Default is 5 seconds.  
+-r, --rollover: (Optional) The number of data points to keep in the graph before rolling over. Default is 20000.  
+
+### Example
+To start monitoring two WLED endpoints with a polling interval of 10 seconds:
+
+```bash
+wled2graph -w 192.168.1.100,192.168.1.101 -t 10
+```
+
+To start monitoring five WLED endpoints with a polling interval of 1 seconds and a data point rollover of 30:
+
+```bash
+wled2graph -w "192.168.1.216, 192.168.1.217, 192.168.1.220, 192.168.1.229, 192.168.1.230" -t 1 -r 30
+```
+
+# How to develop on wled2graph
 ## Prerequisites
 
 Before you begin, ensure you have met the following requirements:
 
 - Python 3.9 or higher
 - [Poetry](https://python-poetry.org/docs/#installation), a tool for dependency management in Python projects.
 
-## Installation
-
 1. Clone the repository to your local machine:
 
     ```bash
     git clone https://github.com/bigredfrog/wled2graph.git
     cd wled2graph
     ```
 
@@ -32,15 +61,15 @@
 
     ```bash
     poetry install
     ```
 
     This will create a virtual environment and install the necessary Python libraries.
 
-## Usage
+## Development Usage
 
 WLED2Graph is executed from the command line and requires a list of IP addresses corresponding to the WLED endpoints you wish to monitor.
 
 ```bash
 poetry run python main.py -w <WLED_IPs> [-t <time_period>] [-r <rollover>]
 ```
```

### Comparing `wled2graph-0.1.0/wled2graph/args.py` & `wled2graph-0.1.1/wled2graph/args.py`

 * *Files identical despite different names*

### Comparing `wled2graph-0.1.0/wled2graph/graphs.py` & `wled2graph-0.1.1/wled2graph/graphs.py`

 * *Files identical despite different names*

### Comparing `wled2graph-0.1.0/wled2graph/main.py` & `wled2graph-0.1.1/wled2graph/main.py`

 * *Files identical despite different names*

### Comparing `wled2graph-0.1.0/wled2graph/template.py` & `wled2graph-0.1.1/wled2graph/template.py`

 * *Files identical despite different names*

### Comparing `wled2graph-0.1.0/wled2graph/utils.py` & `wled2graph-0.1.1/wled2graph/utils.py`

 * *Files identical despite different names*

### Comparing `wled2graph-0.1.0/wled2graph/wled.py` & `wled2graph-0.1.1/wled2graph/wled.py`

 * *Files identical despite different names*

### Comparing `wled2graph-0.1.0/PKG-INFO` & `wled2graph-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: wled2graph
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: wled2graph supports a table and graphs of FPS and other data from multiple WLED endpoints in real-time via a browser interface
 License: MIT
 Author: bigredfrog
 Author-email: big.red.frog@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -27,23 +27,52 @@
 
 - **Real-time FPS, BSSID, RSSI and Ping Visualization**: Continuously polls WLED endpoints and updates the graph with current FPS values.
 - **IP address hyperlink to WLED UI**: Just click through direct to the WLED UI for the selected WLED endpoint.
 - **Configurable Polling Frequency**: Allows customization of the polling interval to suit network and performance needs.
 - **Scalable**: Can monitor multiple WLED endpoints simultaneously.
 - **Customizable Data Points Rollover**: Supports setting a maximum number of data points to display on the graph, after which old data points are rolled off.
 
+
+## Installation from PyPi
+
+```bash
+pip install wled2graph
+```
+
+WLED2Graph is executed from the command line and requires a list of IP addresses corresponding to the WLED endpoints you wish to monitor.
+
+```bash
+wled2graph -w <WLED_IPs> [-t <time_period>] [-r <rollover>]
+```
+
+-w, --wleds: A comma-separated list of IP addresses for the WLED endpoints.  
+-t, --time-period: (Optional) The time period in seconds for polling the WLEDs. Default is 5 seconds.  
+-r, --rollover: (Optional) The number of data points to keep in the graph before rolling over. Default is 20000.  
+
+### Example
+To start monitoring two WLED endpoints with a polling interval of 10 seconds:
+
+```bash
+wled2graph -w 192.168.1.100,192.168.1.101 -t 10
+```
+
+To start monitoring five WLED endpoints with a polling interval of 1 seconds and a data point rollover of 30:
+
+```bash
+wled2graph -w "192.168.1.216, 192.168.1.217, 192.168.1.220, 192.168.1.229, 192.168.1.230" -t 1 -r 30
+```
+
+# How to develop on wled2graph
 ## Prerequisites
 
 Before you begin, ensure you have met the following requirements:
 
 - Python 3.9 or higher
 - [Poetry](https://python-poetry.org/docs/#installation), a tool for dependency management in Python projects.
 
-## Installation
-
 1. Clone the repository to your local machine:
 
     ```bash
     git clone https://github.com/bigredfrog/wled2graph.git
     cd wled2graph
     ```
 
@@ -51,15 +80,15 @@
 
     ```bash
     poetry install
     ```
 
     This will create a virtual environment and install the necessary Python libraries.
 
-## Usage
+## Development Usage
 
 WLED2Graph is executed from the command line and requires a list of IP addresses corresponding to the WLED endpoints you wish to monitor.
 
 ```bash
 poetry run python main.py -w <WLED_IPs> [-t <time_period>] [-r <rollover>]
 ```
```

