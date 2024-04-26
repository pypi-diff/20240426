# Comparing `tmp/llm_monitoring_sascha-0.0.7.tar.gz` & `tmp/llm_monitoring_sascha-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_monitoring_sascha-0.0.7.tar", last modified: Fri Apr 26 08:55:01 2024, max compression
+gzip compressed data, was "llm_monitoring_sascha-0.0.8.tar", last modified: Fri Apr 26 11:02:51 2024, max compression
```

## Comparing `llm_monitoring_sascha-0.0.7.tar` & `llm_monitoring_sascha-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:55:01.109447 llm_monitoring_sascha-0.0.7/
--rw-r--r--   0 sascha     (501) staff       (20)        8 2024-04-26 07:51:08.000000 llm_monitoring_sascha-0.0.7/LICENSE
--rw-r--r--   0 sascha     (501) staff       (20)      561 2024-04-26 08:55:01.109072 llm_monitoring_sascha-0.0.7/PKG-INFO
--rw-r--r--   0 sascha     (501) staff       (20)       10 2023-12-21 09:09:33.000000 llm_monitoring_sascha-0.0.7/README.md
-drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:55:01.108516 llm_monitoring_sascha-0.0.7/llm_monitoring_sascha.egg-info/
--rw-r--r--   0 sascha     (501) staff       (20)      561 2024-04-26 08:55:01.000000 llm_monitoring_sascha-0.0.7/llm_monitoring_sascha.egg-info/PKG-INFO
--rw-r--r--   0 sascha     (501) staff       (20)      320 2024-04-26 08:55:01.000000 llm_monitoring_sascha-0.0.7/llm_monitoring_sascha.egg-info/SOURCES.txt
--rw-r--r--   0 sascha     (501) staff       (20)        1 2024-04-26 08:55:01.000000 llm_monitoring_sascha-0.0.7/llm_monitoring_sascha.egg-info/dependency_links.txt
--rw-r--r--   0 sascha     (501) staff       (20)       20 2024-04-26 08:55:01.000000 llm_monitoring_sascha-0.0.7/llm_monitoring_sascha.egg-info/requires.txt
--rw-r--r--   0 sascha     (501) staff       (20)       11 2024-04-26 08:55:01.000000 llm_monitoring_sascha-0.0.7/llm_monitoring_sascha.egg-info/top_level.txt
-drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:55:01.108183 llm_monitoring_sascha-0.0.7/monitoring/
--rw-r--r--   0 sascha     (501) staff       (20)     2113 2024-04-25 14:07:28.000000 llm_monitoring_sascha-0.0.7/monitoring/__init__.py
--rw-r--r--   0 sascha     (501) staff       (20)     4629 2024-04-26 07:28:16.000000 llm_monitoring_sascha-0.0.7/monitoring/client.py
--rw-r--r--   0 sascha     (501) staff       (20)      186 2024-04-26 08:54:10.000000 llm_monitoring_sascha-0.0.7/monitoring/setup.py
--rw-r--r--   0 sascha     (501) staff       (20)      644 2024-04-26 08:54:56.000000 llm_monitoring_sascha-0.0.7/pyproject.toml
--rw-r--r--   0 sascha     (501) staff       (20)       38 2024-04-26 08:55:01.109549 llm_monitoring_sascha-0.0.7/setup.cfg
+drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 11:02:51.970075 llm_monitoring_sascha-0.0.8/
+-rw-r--r--   0 sascha     (501) staff       (20)        8 2024-04-26 07:51:08.000000 llm_monitoring_sascha-0.0.8/LICENSE
+-rw-r--r--   0 sascha     (501) staff       (20)      561 2024-04-26 11:02:51.969828 llm_monitoring_sascha-0.0.8/PKG-INFO
+-rw-r--r--   0 sascha     (501) staff       (20)       10 2023-12-21 09:09:33.000000 llm_monitoring_sascha-0.0.8/README.md
+drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 11:02:51.969541 llm_monitoring_sascha-0.0.8/llm_monitoring_sascha.egg-info/
+-rw-r--r--   0 sascha     (501) staff       (20)      561 2024-04-26 11:02:51.000000 llm_monitoring_sascha-0.0.8/llm_monitoring_sascha.egg-info/PKG-INFO
+-rw-r--r--   0 sascha     (501) staff       (20)      300 2024-04-26 11:02:51.000000 llm_monitoring_sascha-0.0.8/llm_monitoring_sascha.egg-info/SOURCES.txt
+-rw-r--r--   0 sascha     (501) staff       (20)        1 2024-04-26 11:02:51.000000 llm_monitoring_sascha-0.0.8/llm_monitoring_sascha.egg-info/dependency_links.txt
+-rw-r--r--   0 sascha     (501) staff       (20)       20 2024-04-26 11:02:51.000000 llm_monitoring_sascha-0.0.8/llm_monitoring_sascha.egg-info/requires.txt
+-rw-r--r--   0 sascha     (501) staff       (20)       11 2024-04-26 11:02:51.000000 llm_monitoring_sascha-0.0.8/llm_monitoring_sascha.egg-info/top_level.txt
+drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 11:02:51.969009 llm_monitoring_sascha-0.0.8/monitoring/
+-rw-r--r--   0 sascha     (501) staff       (20)     2113 2024-04-25 14:07:28.000000 llm_monitoring_sascha-0.0.8/monitoring/__init__.py
+-rw-r--r--   0 sascha     (501) staff       (20)     5416 2024-04-26 11:02:24.000000 llm_monitoring_sascha-0.0.8/monitoring/client.py
+-rw-r--r--   0 sascha     (501) staff       (20)      644 2024-04-26 11:02:36.000000 llm_monitoring_sascha-0.0.8/pyproject.toml
+-rw-r--r--   0 sascha     (501) staff       (20)       38 2024-04-26 11:02:51.970143 llm_monitoring_sascha-0.0.8/setup.cfg
```

### Comparing `llm_monitoring_sascha-0.0.7/PKG-INFO` & `llm_monitoring_sascha-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_monitoring_sascha
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small example package
 Author-email: Sascha Heyer <mail@saschaheyer.de>, Sascha Heyer <sascha@doit.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llm_monitoring_sascha-0.0.7/llm_monitoring_sascha.egg-info/PKG-INFO` & `llm_monitoring_sascha-0.0.8/llm_monitoring_sascha.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_monitoring_sascha
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small example package
 Author-email: Sascha Heyer <mail@saschaheyer.de>, Sascha Heyer <sascha@doit.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llm_monitoring_sascha-0.0.7/monitoring/__init__.py` & `llm_monitoring_sascha-0.0.8/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_monitoring_sascha-0.0.7/monitoring/client.py` & `llm_monitoring_sascha-0.0.8/monitoring/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import functools
 from enum import Enum
 from google.cloud import pubsub_v1
 import json
 import time
 from concurrent import futures
 
+import logging
+logger = logging.getLogger(__name__)
+
 #TODO we should be able to detect the provider automatically and for now we could focus on Google
 class CloudProvider(Enum):
     Google = 1
     OpenAI = 2
     # Other cloud providers...
     
 class Identifier(Enum):
@@ -23,14 +26,21 @@
         self.topic_name = f"projects/{self.project}/topics/{topic_name}"
         self.monitored_attributes = {}
         # Other initialization logic
         self.publisher = pubsub_v1.PublisherClient()
         #self.topic_name = 
         self.publish_futures = []
 
+    def measure_response_time(self, func, *args, **kwargs):
+        import time
+        start_time = time.time()  # Start timing
+        response = func(*args, **kwargs)  # Execute the function and capture the response
+        end_time = time.time()  # End timing
+        response_time_ms = (end_time - start_time) * 1000  # Calculate response time in ms
+        return response_time_ms, response
 
     def get_attribute(self, attribute_name):
         return self.monitored_attributes.get(attribute_name, None)
     
     def publish_message(self):
         message = b"Hello, Pub/Sub!"
         future = self.publisher.publish(self.topic_name, data=message)
@@ -48,18 +58,22 @@
             #print("response")
             #print(response)
             print("kwargs")
             print(kwargs)
             #attrs = {attr: getattr(client, attr) for attr in dir(client)
             #         if not callable(getattr(client, attr)) and not attr.startswith("_")}
             #print("Attributes of the model before execution:", attrs)
-            
+           
+            #response_time, response = self.measure_response_time(func(*args, **kwargs))
+            response_time, response = self.measure_response_time(func, *args, **kwargs)
+
             response = func(*args, **kwargs)
             print("RESPONSE")
-            print(response)
+            #print(response)
+            print(response_time)
             
             
             #new_attrs = {attr: getattr(client, attr) for attr in dir(client)
             #             if not callable(getattr(client, attr)) and not attr.startswith("_")}
             #print("Attributes of the model after execution:", new_attrs)
            
             # Here, you can add the actual monitoring logic
@@ -88,14 +102,15 @@
                 generation = response.candidates[0].content.parts[0].text 
                 input_token_count = response._raw_response.usage_metadata.prompt_token_count
                 output_token_count = response._raw_response.usage_metadata.candidates_token_count
                 total_token_count = response._raw_response.usage_metadata.total_token_count
             
             message = json.dumps({
                 "model_name": model_name.split('/')[-1],
+                "response_time": response_time,
                 "temperature": temperature,
                 "top_p": top_p,
                 "prompt": prompt,
                 "generation": generation,
                 "input_token_count": input_token_count,
                 "output_token_count": output_token_count,
                 "total_token_count": total_token_count
@@ -109,14 +124,15 @@
             start_time = time.time()
             future = self.publisher.publish(self.topic_name, data=message)
             future.result()  # Block until the message has been confirmed as published
             end_time = time.time()
             duration = (end_time - start_time) * 1000
     
             print(f"Time taken to publish the message: {duration} ms")
+            logger.error(f"Time taken to publish the message: {duration} ms")
            
             return response
         
         return wrapper
```

### Comparing `llm_monitoring_sascha-0.0.7/pyproject.toml` & `llm_monitoring_sascha-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llm_monitoring_sascha"
 dependencies = [
   'google-cloud-pubsub'
 ]
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Sascha Heyer", email="mail@saschaheyer.de" },
   { name="Sascha Heyer", email="sascha@doit.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 classifiers = [
```

