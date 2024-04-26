# Comparing `tmp/klein_queue-2.4.5.tar.gz` & `tmp/klein_queue-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klein_queue-2.4.5.tar", last modified: Mon Apr 22 08:43:15 2024, max compression
+gzip compressed data, was "klein_queue-2.4.6.tar", last modified: Fri Apr 26 16:37:14 2024, max compression
```

## Comparing `klein_queue-2.4.5.tar` & `klein_queue-2.4.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:43:15.140802 klein_queue-2.4.5/
--rw-rw-rw-   0 root         (0) root         (0)     9136 2024-04-22 08:43:06.000000 klein_queue-2.4.5/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-22 08:43:06.000000 klein_queue-2.4.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4358 2024-04-22 08:43:15.140802 klein_queue-2.4.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3933 2024-04-22 08:43:06.000000 klein_queue-2.4.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 08:43:15.140802 klein_queue-2.4.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1637 2024-04-22 08:43:06.000000 klein_queue-2.4.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:43:15.136219 klein_queue-2.4.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:43:15.137136 klein_queue-2.4.5/src/klein_queue/
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-22 08:43:06.000000 klein_queue-2.4.5/src/klein_queue/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2024-04-22 08:43:06.000000 klein_queue-2.4.5/src/klein_queue/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:43:15.138969 klein_queue-2.4.5/src/klein_queue/rabbitmq/
--rw-rw-rw-   0 root         (0) root         (0)      267 2024-04-22 08:43:06.000000 klein_queue-2.4.5/src/klein_queue/rabbitmq/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2406 2024-04-22 08:43:06.000000 klein_queue-2.4.5/src/klein_queue/rabbitmq/api.py
--rw-rw-rw-   0 root         (0) root         (0)    11730 2024-04-22 08:43:06.000000 klein_queue-2.4.5/src/klein_queue/rabbitmq/connect.py
--rw-rw-rw-   0 root         (0) root         (0)    12614 2024-04-22 08:43:06.000000 klein_queue-2.4.5/src/klein_queue/rabbitmq/consumer.py
--rw-rw-rw-   0 root         (0) root         (0)     4596 2024-04-22 08:43:06.000000 klein_queue-2.4.5/src/klein_queue/rabbitmq/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7847 2024-04-22 08:43:06.000000 klein_queue-2.4.5/src/klein_queue/rabbitmq/publisher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:43:15.138969 klein_queue-2.4.5/src/klein_queue.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4358 2024-04-22 08:43:15.000000 klein_queue-2.4.5/src/klein_queue.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      558 2024-04-22 08:43:15.000000 klein_queue-2.4.5/src/klein_queue.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 08:43:15.000000 klein_queue-2.4.5/src/klein_queue.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-22 08:43:15.000000 klein_queue-2.4.5/src/klein_queue.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-22 08:43:15.000000 klein_queue-2.4.5/src/klein_queue.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 08:43:15.000000 klein_queue-2.4.5/src/klein_queue.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-04-22 08:43:06.000000 klein_queue-2.4.5/src/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:37:14.146484 klein_queue-2.4.6/
+-rw-rw-rw-   0 root         (0) root         (0)     9136 2024-04-26 16:37:04.000000 klein_queue-2.4.6/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-26 16:37:04.000000 klein_queue-2.4.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4351 2024-04-26 16:37:14.146484 klein_queue-2.4.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3933 2024-04-26 16:37:04.000000 klein_queue-2.4.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 16:37:14.146484 klein_queue-2.4.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1630 2024-04-26 16:37:04.000000 klein_queue-2.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:37:14.141901 klein_queue-2.4.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:37:14.143734 klein_queue-2.4.6/src/klein_queue/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-26 16:37:04.000000 klein_queue-2.4.6/src/klein_queue/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-04-26 16:37:04.000000 klein_queue-2.4.6/src/klein_queue/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:37:14.145568 klein_queue-2.4.6/src/klein_queue/rabbitmq/
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-04-26 16:37:04.000000 klein_queue-2.4.6/src/klein_queue/rabbitmq/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2406 2024-04-26 16:37:04.000000 klein_queue-2.4.6/src/klein_queue/rabbitmq/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    11730 2024-04-26 16:37:04.000000 klein_queue-2.4.6/src/klein_queue/rabbitmq/connect.py
+-rw-rw-rw-   0 root         (0) root         (0)    12614 2024-04-26 16:37:04.000000 klein_queue-2.4.6/src/klein_queue/rabbitmq/consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4596 2024-04-26 16:37:04.000000 klein_queue-2.4.6/src/klein_queue/rabbitmq/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7847 2024-04-26 16:37:04.000000 klein_queue-2.4.6/src/klein_queue/rabbitmq/publisher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:37:14.146484 klein_queue-2.4.6/src/klein_queue.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4351 2024-04-26 16:37:14.000000 klein_queue-2.4.6/src/klein_queue.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      558 2024-04-26 16:37:14.000000 klein_queue-2.4.6/src/klein_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 16:37:14.000000 klein_queue-2.4.6/src/klein_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2024-04-26 16:37:14.000000 klein_queue-2.4.6/src/klein_queue.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-26 16:37:14.000000 klein_queue-2.4.6/src/klein_queue.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 16:37:14.000000 klein_queue-2.4.6/src/klein_queue.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-04-26 16:37:04.000000 klein_queue-2.4.6/src/version.py
```

### Comparing `klein_queue-2.4.5/LICENSE.txt` & `klein_queue-2.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.5/PKG-INFO` & `klein_queue-2.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: klein_queue
-Version: 2.4.5
+Version: 2.4.6
 Summary: RabbitMQ integration
 Home-page: http://github.com/mdcatapult/py-queue
 Author: Medicines Discovery Catapult
 Author-email: SoftwareEngineering@md.catapult.org.uk
 License: Apache V2
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: klein_config<4.0.0,>=3.0.0
+Requires-Dist: klein_config>=3.0.0
 Requires-Dist: pika<2.0.0,>=1.1.0
 Requires-Dist: requests<3.0.0,>=2.23.0
 
 # Klein Queue
 
 Module to abstract queues. Currently implements RabbitMQ.
```

### Comparing `klein_queue-2.4.5/README.md` & `klein_queue-2.4.6/README.md`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.5/setup.py` & `klein_queue-2.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,13 +36,13 @@
       url='http://github.com/mdcatapult/py-queue',
       author='Medicines Discovery Catapult',
       author_email='SoftwareEngineering@md.catapult.org.uk',
       license='Apache V2',
       packages=find_packages('src'),
       package_dir={'': 'src'},
       install_requires=[
-          'klein_config>=3.0.0,<4.0.0',
+          'klein_config>=3.0.0',
           'pika>=1.1.0,<2.0.0',
           'requests>=2.23.0,<3.0.0'
       ],
       zip_safe=True,
       include_package_data=True)
```

### Comparing `klein_queue-2.4.5/src/klein_queue/errors.py` & `klein_queue-2.4.6/src/klein_queue/errors.py`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.5/src/klein_queue/rabbitmq/api.py` & `klein_queue-2.4.6/src/klein_queue/rabbitmq/api.py`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.5/src/klein_queue/rabbitmq/connect.py` & `klein_queue-2.4.6/src/klein_queue/rabbitmq/connect.py`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.5/src/klein_queue/rabbitmq/consumer.py` & `klein_queue-2.4.6/src/klein_queue/rabbitmq/consumer.py`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.5/src/klein_queue/rabbitmq/exceptions.py` & `klein_queue-2.4.6/src/klein_queue/rabbitmq/exceptions.py`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.5/src/klein_queue/rabbitmq/publisher.py` & `klein_queue-2.4.6/src/klein_queue/rabbitmq/publisher.py`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.5/src/klein_queue.egg-info/PKG-INFO` & `klein_queue-2.4.6/src/klein_queue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: klein-queue
-Version: 2.4.5
+Name: klein_queue
+Version: 2.4.6
 Summary: RabbitMQ integration
 Home-page: http://github.com/mdcatapult/py-queue
 Author: Medicines Discovery Catapult
 Author-email: SoftwareEngineering@md.catapult.org.uk
 License: Apache V2
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: klein_config<4.0.0,>=3.0.0
+Requires-Dist: klein_config>=3.0.0
 Requires-Dist: pika<2.0.0,>=1.1.0
 Requires-Dist: requests<3.0.0,>=2.23.0
 
 # Klein Queue
 
 Module to abstract queues. Currently implements RabbitMQ.
```

### Comparing `klein_queue-2.4.5/src/klein_queue.egg-info/SOURCES.txt` & `klein_queue-2.4.6/src/klein_queue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

