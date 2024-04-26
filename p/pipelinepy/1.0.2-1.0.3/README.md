# Comparing `tmp/pipelinepy-1.0.2.tar.gz` & `tmp/pipelinepy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipelinepy-1.0.2.tar", max compression
+gzip compressed data, was "pipelinepy-1.0.3.tar", max compression
```

## Comparing `pipelinepy-1.0.2.tar` & `pipelinepy-1.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3259 2024-04-26 16:13:40.243689 pipelinepy-1.0.2/README.md
--rw-r--r--   0        0        0     1734 2024-04-26 16:03:08.953663 pipelinepy-1.0.2/pipelinepy/ImsTokenProvider.py
--rw-r--r--   0        0        0      108 2024-04-26 16:03:08.950496 pipelinepy-1.0.2/pipelinepy/__init__.py
--rw-r--r--   0        0        0      466 2024-04-26 16:15:33.136587 pipelinepy-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4053 1970-01-01 00:00:00.000000 pipelinepy-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3262 2024-04-26 16:19:30.715659 pipelinepy-1.0.3/README.md
+-rw-r--r--   0        0        0     1734 2024-04-26 16:03:08.953663 pipelinepy-1.0.3/pipelinepy/ImsTokenProvider.py
+-rw-r--r--   0        0        0      108 2024-04-26 16:03:08.950496 pipelinepy-1.0.3/pipelinepy/__init__.py
+-rw-r--r--   0        0        0      472 2024-04-26 16:16:29.136681 pipelinepy-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 pipelinepy-1.0.3/PKG-INFO
```

### Comparing `pipelinepy-1.0.2/README.md` & `pipelinepy-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,21 @@
 
 ```bash
 pip install pipelinepy
 ```
 
 ## Usage
 
-To use the pipelinepy, you need to import it in your Python script, along with the kafka client implementation. 
+To use the pipelinepy, you need to import the specified requirements. 
 You can then create a Kafka producer and consumer, and use them to send and receive messages to/ from a Kafka topic.
 
+```bash
+pip install -r requirements.txt
+```
+
 ```python
 #!/usr/bin/env python
 import threading, time
 
 from kafka import KafkaConsumer, KafkaProducer
 from pipelinepy import ImsTokenProvider
```

### Comparing `pipelinepy-1.0.2/pipelinepy/ImsTokenProvider.py` & `pipelinepy-1.0.3/pipelinepy/ImsTokenProvider.py`

 * *Files identical despite different names*

### Comparing `pipelinepy-1.0.2/PKG-INFO` & `pipelinepy-1.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pipelinepy
-Version: 1.0.2
-Summary: An IMS authorization code flow used with the Kafka client for Python (kafka-python-ng).
+Version: 1.0.3
+Summary: An Adobe IMS authorization code flow used with the Kafka client for Python (kafka-python-ng).
 Home-page: https://github.com/cristianpetrache/test-me
 Author: Petrut Petrache
 Author-email: cpetrache@adobe.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -28,17 +28,21 @@
 
 ```bash
 pip install pipelinepy
 ```
 
 ## Usage
 
-To use the pipelinepy, you need to import it in your Python script, along with the kafka client implementation. 
+To use the pipelinepy, you need to import the specified requirements. 
 You can then create a Kafka producer and consumer, and use them to send and receive messages to/ from a Kafka topic.
 
+```bash
+pip install -r requirements.txt
+```
+
 ```python
 #!/usr/bin/env python
 import threading, time
 
 from kafka import KafkaConsumer, KafkaProducer
 from pipelinepy import ImsTokenProvider
```

