# Comparing `tmp/airflow-yeedu-operator-1.0.7.tar.gz` & `tmp/airflow-yeedu-operator-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-yeedu-operator-1.0.7.tar", last modified: Tue Apr 23 13:16:30 2024, max compression
+gzip compressed data, was "airflow-yeedu-operator-1.0.8.tar", last modified: Fri Apr 26 09:24:20 2024, max compression
```

## Comparing `airflow-yeedu-operator-1.0.7.tar` & `airflow-yeedu-operator-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-23 13:16:30.449856 airflow-yeedu-operator-1.0.7/
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)    11357 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.7/LICENSE
--rw-r--r--   0 rk0601    (1001) rk0601    (1001)     3072 2024-04-23 13:16:30.449856 airflow-yeedu-operator-1.0.7/PKG-INFO
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)     2647 2024-04-19 08:12:22.000000 airflow-yeedu-operator-1.0.7/README.md
-drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-23 13:16:30.449856 airflow-yeedu-operator-1.0.7/airflow_yeedu_operator.egg-info/
--rw-r--r--   0 rk0601    (1001) rk0601    (1001)     3072 2024-04-23 13:16:30.000000 airflow-yeedu-operator-1.0.7/airflow_yeedu_operator.egg-info/PKG-INFO
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      371 2024-04-23 13:16:30.000000 airflow-yeedu-operator-1.0.7/airflow_yeedu_operator.egg-info/SOURCES.txt
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)        1 2024-04-23 13:16:30.000000 airflow-yeedu-operator-1.0.7/airflow_yeedu_operator.egg-info/dependency_links.txt
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)       37 2024-04-23 13:16:30.000000 airflow-yeedu-operator-1.0.7/airflow_yeedu_operator.egg-info/requires.txt
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)        6 2024-04-23 13:16:30.000000 airflow-yeedu-operator-1.0.7/airflow_yeedu_operator.egg-info/top_level.txt
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)       38 2024-04-23 13:16:30.449856 airflow-yeedu-operator-1.0.7/setup.cfg
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      777 2024-04-23 13:11:58.000000 airflow-yeedu-operator-1.0.7/setup.py
-drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-23 13:16:30.449856 airflow-yeedu-operator-1.0.7/yeedu/
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      787 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.7/yeedu/__init__.py
-drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-23 13:16:30.449856 airflow-yeedu-operator-1.0.7/yeedu/hooks/
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      787 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.7/yeedu/hooks/__init__.py
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)     9653 2024-04-23 13:09:12.000000 airflow-yeedu-operator-1.0.7/yeedu/hooks/yeedu.py
-drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-23 13:16:30.449856 airflow-yeedu-operator-1.0.7/yeedu/operators/
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      787 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.7/yeedu/operators/__init__.py
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)    29437 2024-04-22 12:56:30.000000 airflow-yeedu-operator-1.0.7/yeedu/operators/yeedu.py
+drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-26 09:24:20.963348 airflow-yeedu-operator-1.0.8/
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)    11357 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.8/LICENSE
+-rw-r--r--   0 rk0601    (1001) rk0601    (1001)     5955 2024-04-26 09:24:20.963348 airflow-yeedu-operator-1.0.8/PKG-INFO
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)     5530 2024-04-26 09:22:42.000000 airflow-yeedu-operator-1.0.8/README.md
+drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-26 09:24:20.963348 airflow-yeedu-operator-1.0.8/airflow_yeedu_operator.egg-info/
+-rw-r--r--   0 rk0601    (1001) rk0601    (1001)     5955 2024-04-26 09:24:20.000000 airflow-yeedu-operator-1.0.8/airflow_yeedu_operator.egg-info/PKG-INFO
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      371 2024-04-26 09:24:20.000000 airflow-yeedu-operator-1.0.8/airflow_yeedu_operator.egg-info/SOURCES.txt
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)        1 2024-04-26 09:24:20.000000 airflow-yeedu-operator-1.0.8/airflow_yeedu_operator.egg-info/dependency_links.txt
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)       37 2024-04-26 09:24:20.000000 airflow-yeedu-operator-1.0.8/airflow_yeedu_operator.egg-info/requires.txt
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)        6 2024-04-26 09:24:20.000000 airflow-yeedu-operator-1.0.8/airflow_yeedu_operator.egg-info/top_level.txt
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)       38 2024-04-26 09:24:20.963348 airflow-yeedu-operator-1.0.8/setup.cfg
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      777 2024-04-25 08:51:52.000000 airflow-yeedu-operator-1.0.8/setup.py
+drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-26 09:24:20.963348 airflow-yeedu-operator-1.0.8/yeedu/
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      787 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.8/yeedu/__init__.py
+drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-26 09:24:20.963348 airflow-yeedu-operator-1.0.8/yeedu/hooks/
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      787 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.8/yeedu/hooks/__init__.py
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)     9902 2024-04-26 09:23:05.000000 airflow-yeedu-operator-1.0.8/yeedu/hooks/yeedu.py
+drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-26 09:24:20.963348 airflow-yeedu-operator-1.0.8/yeedu/operators/
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      787 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.8/yeedu/operators/__init__.py
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)    29457 2024-04-26 09:23:31.000000 airflow-yeedu-operator-1.0.8/yeedu/operators/yeedu.py
```

### Comparing `airflow-yeedu-operator-1.0.7/LICENSE` & `airflow-yeedu-operator-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-yeedu-operator-1.0.7/setup.py` & `airflow-yeedu-operator-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def read(*parts):
     return codecs.open(os.path.join(here, *parts), 'r').read()
 
 
 setup(
     name='airflow-yeedu-operator',
-    version='1.0.7',
+    version='1.0.8',
     description='Submission and monitoring of jobs using the Yeedu API in Apache Airflow. ',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     author='Yeedu',
     author_email='yeedu@modak.com',
     packages=find_packages(),
     install_requires=[
```

### Comparing `airflow-yeedu-operator-1.0.7/yeedu/__init__.py` & `airflow-yeedu-operator-1.0.8/yeedu/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-yeedu-operator-1.0.7/yeedu/hooks/__init__.py` & `airflow-yeedu-operator-1.0.8/yeedu/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-yeedu-operator-1.0.7/yeedu/hooks/yeedu.py` & `airflow-yeedu-operator-1.0.8/yeedu/hooks/yeedu.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from typing import Optional, Dict
 import json
 import os
 from requests.exceptions import RequestException
 
 
 
+session = requests.Session()
 
 YEEDU_SCHEDULER_USER = os.getenv("YEEDU_SCHEDULER_USER")
 YEEDU_SCHEDULER_PASSWORD = os.getenv("YEEDU_SCHEDULER_PASSWORD")
 
 headers: dict = {
             'accept': 'application/json',
             'Content-Type': 'application/json'
@@ -80,15 +81,19 @@
         :param method: The HTTP method (GET, POST, etc.).
         :param url: The URL of the API endpoint.
         :param data: The JSON data for the request.
         :param params: Optional dictionary of query parameters.
         :return: The API response.
         """
 
-        response = requests.request(method, url, headers=headers, json=data, params=params)
+        if method =='POST':
+            response = session.post(url, headers=headers, json=data, params=params)
+        else:
+            response = session.get(url, headers=headers, json=data, params=params)
+        #response = requests.request(method, url, headers=headers, json=data, params=params)
         return response  # Exit loop on successful response
             
 
     def yeedu_login(self):
         try:
             login_url = self.base_url+'login'
             data = {
@@ -228,15 +233,15 @@
                     api_status_code: int = response.status_code
                     self.log.info("Current API Status Code: %s",api_status_code)
                     if api_status_code == 200:
                         # If API status is a success, reset the failure attempts counter
                         attempts_failure = 0
                         job_status: str = response.json().get('job_status')
                         self.log.info("Current Job Status: %s ", job_status)
-                        if job_status in ['DONE', 'ERROR', 'TERMINATED', 'KILLED']:
+                        if job_status in ['DONE', 'ERROR', 'TERMINATED', 'KILLED','STOPPED']:
                             break
                 except RequestException as e:
                     attempts_failure += 1
                     delay = 20
                     self.log.info(f"GET Job Status API request failed (attempt {attempts_failure}/{max_attempts}) due to {e}")
                     self.log.info(f"Sleeping for {delay*attempts_failure} seconds before retrying...")
                     time.sleep(delay*attempts_failure)
```

### Comparing `airflow-yeedu-operator-1.0.7/yeedu/operators/__init__.py` & `airflow-yeedu-operator-1.0.8/yeedu/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-yeedu-operator-1.0.7/yeedu/operators/yeedu.py` & `airflow-yeedu-operator-1.0.8/yeedu/operators/yeedu.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,24 +175,24 @@
             logger.info("Job Submited (Job Id: %s)", job_id)
             job_status: str = self.hook.wait_for_completion(job_id)
 
             logger.info("Final Job Status: %s", job_status)
 
             if job_status in ['DONE']:
                 log_type: str = 'stdout'
-            elif job_status in ['ERROR', 'TERMINATED', 'KILLED']:
+            elif job_status in ['ERROR', 'TERMINATED', 'KILLED','STOPPED']:
                 log_type: str = 'stdout'
             else:
                 logger.error("Job completion status is unknown.")
                 return
 
             job_log: str = self.hook.get_job_logs(job_id, log_type)
             logger.info("Logs for Job ID %s (Log Type: %s): %s", job_id, log_type, job_log)
 
-            if job_status in ['ERROR', 'TERMINATED', 'KILLED']:
+            if job_status in ['ERROR', 'TERMINATED', 'KILLED','STOPPED']:
                 logger.error(job_log)
                 raise AirflowException(job_log)
                        
         except Exception as e:
             raise AirflowException(e)
```

