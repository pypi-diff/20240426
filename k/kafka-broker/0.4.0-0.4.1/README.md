# Comparing `tmp/kafka-broker-0.4.0.tar.gz` & `tmp/kafka-broker-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka-broker-0.4.0.tar", last modified: Mon Apr  8 12:54:17 2024, max compression
+gzip compressed data, was "kafka-broker-0.4.1.tar", last modified: Fri Apr 26 08:34:41 2024, max compression
```

## Comparing `kafka-broker-0.4.0.tar` & `kafka-broker-0.4.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 12:54:17.590570 kafka-broker-0.4.0/
--rw-rw-rw-   0        0        0     1090 2023-11-07 12:59:41.000000 kafka-broker-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     4264 2024-04-08 12:54:17.585570 kafka-broker-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     3507 2023-11-17 10:11:05.000000 kafka-broker-0.4.0/README.md
--rw-rw-rw-   0        0        0      851 2024-04-08 12:53:55.000000 kafka-broker-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 12:54:17.591568 kafka-broker-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      365 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 12:54:17.474334 kafka-broker-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 12:54:17.518929 kafka-broker-0.4.0/src/kafka_broker/
--rw-rw-rw-   0        0        0      385 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/__init__.py
--rw-rw-rw-   0        0        0      281 2023-11-20 13:43:40.000000 kafka-broker-0.4.0/src/kafka_broker/base_config.ini
--rw-rw-rw-   0        0        0     6006 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/broker_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-08 12:54:17.558371 kafka-broker-0.4.0/src/kafka_broker/classes/
--rw-rw-rw-   0        0        0        0 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/classes/__init__.py
--rw-rw-rw-   0        0        0     2003 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/classes/cache.py
--rw-rw-rw-   0        0        0     2190 2023-11-17 10:11:05.000000 kafka-broker-0.4.0/src/kafka_broker/classes/consumer_storage.py
--rw-rw-rw-   0        0        0     2888 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/classes/event_object.py
--rw-rw-rw-   0        0        0     3206 2024-04-08 12:47:05.000000 kafka-broker-0.4.0/src/kafka_broker/classes/event_router.py
--rw-rw-rw-   0        0        0     1167 2023-11-17 10:11:05.000000 kafka-broker-0.4.0/src/kafka_broker/config.py
--rw-rw-rw-   0        0        0     3234 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/consumer.py
--rw-rw-rw-   0        0        0      184 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-08 12:54:17.566903 kafka-broker-0.4.0/src/kafka_broker/exceptions/
--rw-rw-rw-   0        0        0        0 2023-11-20 10:24:31.000000 kafka-broker-0.4.0/src/kafka_broker/exceptions/__init__.py
--rw-rw-rw-   0        0        0      462 2024-04-08 12:44:45.000000 kafka-broker-0.4.0/src/kafka_broker/exceptions/base.py
--rw-rw-rw-   0        0        0      605 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/exceptions/cache.py
--rw-rw-rw-   0        0        0     1368 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/producer.py
--rw-rw-rw-   0        0        0        0 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-08 12:54:17.573456 kafka-broker-0.4.0/src/kafka_broker/schemas/
--rw-rw-rw-   0        0        0        0 2024-04-08 11:56:29.000000 kafka-broker-0.4.0/src/kafka_broker/schemas/__init__.py
--rw-rw-rw-   0        0        0      345 2024-04-08 12:41:26.000000 kafka-broker-0.4.0/src/kafka_broker/schemas/log.py
-drwxrwxrwx   0        0        0        0 2024-04-08 12:54:17.580003 kafka-broker-0.4.0/src/kafka_broker.egg-info/
--rw-rw-rw-   0        0        0     4264 2024-04-08 12:54:17.000000 kafka-broker-0.4.0/src/kafka_broker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      881 2024-04-08 12:54:17.000000 kafka-broker-0.4.0/src/kafka_broker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 12:54:17.000000 kafka-broker-0.4.0/src/kafka_broker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-08 12:54:17.000000 kafka-broker-0.4.0/src/kafka_broker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-08 12:54:17.000000 kafka-broker-0.4.0/src/kafka_broker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 12:54:17.576469 kafka-broker-0.4.0/tests/
--rw-rw-rw-   0        0        0      356 2023-11-17 10:11:05.000000 kafka-broker-0.4.0/tests/test_event_object.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:34:41.607711 kafka-broker-0.4.1/
+-rw-rw-rw-   0        0        0     1090 2023-11-07 12:59:41.000000 kafka-broker-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     4159 2024-04-26 08:34:41.606718 kafka-broker-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3507 2023-11-17 10:11:05.000000 kafka-broker-0.4.1/README.md
+-rw-rw-rw-   0        0        0      851 2024-04-26 08:32:57.000000 kafka-broker-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 08:34:41.608714 kafka-broker-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      365 2024-04-08 10:30:04.000000 kafka-broker-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:34:41.558555 kafka-broker-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 08:34:41.580094 kafka-broker-0.4.1/src/kafka_broker/
+-rw-rw-rw-   0        0        0      385 2024-04-08 10:30:04.000000 kafka-broker-0.4.1/src/kafka_broker/__init__.py
+-rw-rw-rw-   0        0        0      281 2023-11-20 13:43:40.000000 kafka-broker-0.4.1/src/kafka_broker/base_config.ini
+-rw-rw-rw-   0        0        0     6006 2024-04-08 10:30:04.000000 kafka-broker-0.4.1/src/kafka_broker/broker_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:34:41.596970 kafka-broker-0.4.1/src/kafka_broker/classes/
+-rw-rw-rw-   0        0        0        0 2024-04-08 10:30:04.000000 kafka-broker-0.4.1/src/kafka_broker/classes/__init__.py
+-rw-rw-rw-   0        0        0     2003 2024-04-08 10:30:04.000000 kafka-broker-0.4.1/src/kafka_broker/classes/cache.py
+-rw-rw-rw-   0        0        0     2190 2023-11-17 10:11:05.000000 kafka-broker-0.4.1/src/kafka_broker/classes/consumer_storage.py
+-rw-rw-rw-   0        0        0     2888 2024-04-08 10:30:04.000000 kafka-broker-0.4.1/src/kafka_broker/classes/event_object.py
+-rw-rw-rw-   0        0        0     3172 2024-04-26 08:28:50.000000 kafka-broker-0.4.1/src/kafka_broker/classes/event_router.py
+-rw-rw-rw-   0        0        0     1167 2023-11-17 10:11:05.000000 kafka-broker-0.4.1/src/kafka_broker/config.py
+-rw-rw-rw-   0        0        0     3234 2024-04-08 10:30:04.000000 kafka-broker-0.4.1/src/kafka_broker/consumer.py
+-rw-rw-rw-   0        0        0      184 2024-04-08 10:30:04.000000 kafka-broker-0.4.1/src/kafka_broker/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:34:41.600996 kafka-broker-0.4.1/src/kafka_broker/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-11-20 10:24:31.000000 kafka-broker-0.4.1/src/kafka_broker/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      462 2024-04-08 12:44:45.000000 kafka-broker-0.4.1/src/kafka_broker/exceptions/base.py
+-rw-rw-rw-   0        0        0      605 2024-04-08 10:30:04.000000 kafka-broker-0.4.1/src/kafka_broker/exceptions/cache.py
+-rw-rw-rw-   0        0        0     1368 2024-04-08 10:30:04.000000 kafka-broker-0.4.1/src/kafka_broker/producer.py
+-rw-rw-rw-   0        0        0        0 2024-04-08 10:30:04.000000 kafka-broker-0.4.1/src/kafka_broker/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-26 08:34:41.603162 kafka-broker-0.4.1/src/kafka_broker/schemas/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:56:29.000000 kafka-broker-0.4.1/src/kafka_broker/schemas/__init__.py
+-rw-rw-rw-   0        0        0      345 2024-04-08 12:41:26.000000 kafka-broker-0.4.1/src/kafka_broker/schemas/log.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:34:41.587323 kafka-broker-0.4.1/src/kafka_broker.egg-info/
+-rw-rw-rw-   0        0        0     4159 2024-04-26 08:34:41.000000 kafka-broker-0.4.1/src/kafka_broker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      881 2024-04-26 08:34:41.000000 kafka-broker-0.4.1/src/kafka_broker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 08:34:41.000000 kafka-broker-0.4.1/src/kafka_broker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-26 08:34:41.000000 kafka-broker-0.4.1/src/kafka_broker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-26 08:34:41.000000 kafka-broker-0.4.1/src/kafka_broker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 08:34:41.604188 kafka-broker-0.4.1/tests/
+-rw-rw-rw-   0        0        0      356 2023-11-17 10:11:05.000000 kafka-broker-0.4.1/tests/test_event_object.py
```

### Comparing `kafka-broker-0.4.0/LICENSE` & `kafka-broker-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.0/PKG-INFO` & `kafka-broker-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: kafka-broker
-Version: 0.4.0
+Version: 0.4.1
 Summary: A python package implementation for the confluent kafka package. Managing producing and consuming.
 Author-email: Tijmen Simons <tijmen.simons@student.hu.nl>, Ivar Stek <ivar.stek@student.hu.nl>
 Project-URL: Homepage, https://github.com/TijmenSimons/kafka-broker
 Project-URL: Bug Tracker, https://github.com/TijmenSimons/kafka-broker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: confluent_kafka>=2.3.0
-Requires-Dist: pymemcache>=4.0.0
-Requires-Dist: pydantic>=2.5.3
 
 # Kafka Broker
 
 A python package implementation for the confluent kafka package. Managing producing and consuming.
 
 Has built-in implementation for FastAPI.
```

### Comparing `kafka-broker-0.4.0/README.md` & `kafka-broker-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.0/pyproject.toml` & `kafka-broker-0.4.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kafka-broker"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="Tijmen Simons", email="tijmen.simons@student.hu.nl" },
   { name="Ivar Stek", email="ivar.stek@student.hu.nl" },
 ]
 description = "A python package implementation for the confluent kafka package. Managing producing and consuming."
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `kafka-broker-0.4.0/src/kafka_broker/broker_manager.py` & `kafka-broker-0.4.1/src/kafka_broker/broker_manager.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.0/src/kafka_broker/classes/cache.py` & `kafka-broker-0.4.1/src/kafka_broker/classes/cache.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.0/src/kafka_broker/classes/consumer_storage.py` & `kafka-broker-0.4.1/src/kafka_broker/classes/consumer_storage.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.0/src/kafka_broker/classes/event_object.py` & `kafka-broker-0.4.1/src/kafka_broker/classes/event_object.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.0/src/kafka_broker/classes/event_router.py` & `kafka-broker-0.4.1/src/kafka_broker/classes/event_router.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import Self
 from pydantic import ValidationError
 
-from src.kafka_broker.exceptions.base import CustomException
-from src.kafka_broker.schemas.log import Log
+from exceptions.base import CustomException
+from schemas.log import Log
 
 from ..enums import EventStatus
 from ..broker_manager import broker_manager
 from .event_object import EventObject
 
 logging_module = "LoggingModule"
 log_event = "log.create"
```

### Comparing `kafka-broker-0.4.0/src/kafka_broker/config.py` & `kafka-broker-0.4.1/src/kafka_broker/config.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.0/src/kafka_broker/consumer.py` & `kafka-broker-0.4.1/src/kafka_broker/consumer.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.0/src/kafka_broker/exceptions/cache.py` & `kafka-broker-0.4.1/src/kafka_broker/exceptions/cache.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.0/src/kafka_broker/producer.py` & `kafka-broker-0.4.1/src/kafka_broker/producer.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.0/src/kafka_broker.egg-info/PKG-INFO` & `kafka-broker-0.4.1/src/kafka_broker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: kafka-broker
-Version: 0.4.0
+Version: 0.4.1
 Summary: A python package implementation for the confluent kafka package. Managing producing and consuming.
 Author-email: Tijmen Simons <tijmen.simons@student.hu.nl>, Ivar Stek <ivar.stek@student.hu.nl>
 Project-URL: Homepage, https://github.com/TijmenSimons/kafka-broker
 Project-URL: Bug Tracker, https://github.com/TijmenSimons/kafka-broker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: confluent_kafka>=2.3.0
-Requires-Dist: pymemcache>=4.0.0
-Requires-Dist: pydantic>=2.5.3
 
 # Kafka Broker
 
 A python package implementation for the confluent kafka package. Managing producing and consuming.
 
 Has built-in implementation for FastAPI.
```

### Comparing `kafka-broker-0.4.0/src/kafka_broker.egg-info/SOURCES.txt` & `kafka-broker-0.4.1/src/kafka_broker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

