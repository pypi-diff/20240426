# Comparing `tmp/pipelinepy-1.0.1.tar.gz` & `tmp/pipelinepy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipelinepy-1.0.1.tar", max compression
+gzip compressed data, was "pipelinepy-1.0.2.tar", max compression
```

## Comparing `pipelinepy-1.0.1.tar` & `pipelinepy-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3523 2024-04-26 15:57:54.796963 pipelinepy-1.0.1/README.md
--rw-r--r--   0        0        0     1734 2024-04-25 11:28:25.562793 pipelinepy-1.0.1/pipelinepy/ImsTokenProvider.py
--rw-r--r--   0        0        0      108 2024-04-26 15:41:46.463623 pipelinepy-1.0.1/pipelinepy/__init__.py
--rw-r--r--   0        0        0      466 2024-04-26 15:59:13.010177 pipelinepy-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4317 1970-01-01 00:00:00.000000 pipelinepy-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3259 2024-04-26 16:13:40.243689 pipelinepy-1.0.2/README.md
+-rw-r--r--   0        0        0     1734 2024-04-26 16:03:08.953663 pipelinepy-1.0.2/pipelinepy/ImsTokenProvider.py
+-rw-r--r--   0        0        0      108 2024-04-26 16:03:08.950496 pipelinepy-1.0.2/pipelinepy/__init__.py
+-rw-r--r--   0        0        0      466 2024-04-26 16:15:33.136587 pipelinepy-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4053 1970-01-01 00:00:00.000000 pipelinepy-1.0.2/PKG-INFO
```

### Comparing `pipelinepy-1.0.1/pipelinepy/ImsTokenProvider.py` & `pipelinepy-1.0.2/pipelinepy/ImsTokenProvider.py`

 * *Files identical despite different names*

### Comparing `pipelinepy-1.0.1/PKG-INFO` & `pipelinepy-1.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipelinepy
-Version: 1.0.1
+Version: 1.0.2
 Summary: An IMS authorization code flow used with the Kafka client for Python (kafka-python-ng).
 Home-page: https://github.com/cristianpetrache/test-me
 Author: Petrut Petrache
 Author-email: cpetrache@adobe.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -15,19 +15,20 @@
 Requires-Dist: kafka-python-ng (>=2.2.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/cristianpetrache/test-me
 Description-Content-Type: text/markdown
 
 # pipelinepy
 
-This is a Python client callback for the Pipeline Kafka. It is designed to provide a simple and straightforward interface for interacting with IMS Kafka.
+This is a Python client callback for the Adobe Pipeline Kafka. It is designed to provide a 
+simple and straightforward interface for authenticating IMS users into Kafka.
 
 ## Installation
 
-To install the pipelinepy, you can use pip (artifactory-uw2 credentials are needed):
+To install the pipelinepy, you can use pip:
 
 ```bash
 pip install pipelinepy
 ```
 
 ## Usage
 
@@ -47,45 +48,45 @@
         threading.Thread.__init__(self)
         self.stop_event = threading.Event()
 
     def stop(self):
         self.stop_event.set()
 
     def run(self):
-        producer = KafkaProducer(bootstrap_servers=['kafka-a1-az1-va7-corp.int.pipeline.adobedc.net:443','kafka-a1-az2-va7-corp.int.pipeline.adobedc.net:443','kafka-a1-az3-va7-corp.int.pipeline.adobedc.net:443'],
+        producer = KafkaProducer(bootstrap_servers=['broker1:9092','broker2:9092','broker3:9092'],
                                  sasl_mechanism='OAUTHBEARER',
                                  security_protocol='SASL_SSL',
                                  sasl_oauth_token_provider=ImsTokenProvider())
 
         while not self.stop_event.is_set():
-            producer.send('xdm_acp_dcs_stg_gw23', b"Hello, world!")
-            producer.send('xdm_acp_dcs_stg_gw23', b"Salutare, lume!")
-            producer.send('xdm_acp_dcs_stg_gw23', b"\xc2\xa1Hola, mundo!")
+            producer.send('some_existing_topic', b"Hello, world!")
+            producer.send('some_existing_topic', b"Salutare, lume!")
+            producer.send('some_existing_topic', b"\xc2\xa1Hola, mundo!")
             time.sleep(1)
 
         producer.close()
 
 
 class Consumer(threading.Thread):
     def __init__(self):
         threading.Thread.__init__(self)
         self.stop_event = threading.Event()
 
     def stop(self):
         self.stop_event.set()
 
     def run(self):
-        consumer = KafkaConsumer(bootstrap_servers=['kafka-a1-az1-va7-corp.int.pipeline.adobedc.net:443','kafka-a1-az2-va7-corp.int.pipeline.adobedc.net:443','kafka-a1-az3-va7-corp.int.pipeline.adobedc.net:443'],
+        consumer = KafkaConsumer(bootstrap_servers=['broker1:9092','broker2:9092','broker3:9092'],
                                  auto_offset_reset='earliest',
-                                 group_id='petrut-test-cg',
+                                 group_id='test-cg',
                                  consumer_timeout_ms=1000,
                                  sasl_mechanism='OAUTHBEARER',
                                  security_protocol='SASL_SSL',
                                  sasl_oauth_token_provider=ImsTokenProvider())
-        consumer.subscribe(['xdm_acp_dcs_stg_gw23'])
+        consumer.subscribe(['some_existing_topic'])
 
         while not self.stop_event.is_set():
             for message in consumer:
                 print(message)
                 if self.stop_event.is_set():
                     break
```

