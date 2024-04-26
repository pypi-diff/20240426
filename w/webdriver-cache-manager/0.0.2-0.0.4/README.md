# Comparing `tmp/webdriver_cache_manager-0.0.2.tar.gz` & `tmp/webdriver_cache_manager-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webdriver_cache_manager-0.0.2.tar", last modified: Thu Dec  7 20:01:40 2023, max compression
+gzip compressed data, was "webdriver_cache_manager-0.0.4.tar", last modified: Fri Apr 26 17:04:45 2024, max compression
```

## Comparing `webdriver_cache_manager-0.0.2.tar` & `webdriver_cache_manager-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 20:01:40.472680 webdriver_cache_manager-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-07 20:01:32.000000 webdriver_cache_manager-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2023-12-07 20:01:40.472680 webdriver_cache_manager-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2023-12-07 20:01:32.000000 webdriver_cache_manager-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      639 2023-12-07 20:01:32.000000 webdriver_cache_manager-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 20:01:40.472680 webdriver_cache_manager-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 20:01:40.472680 webdriver_cache_manager-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 20:01:40.472680 webdriver_cache_manager-0.0.2/src/webdriver_cache_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-07 20:01:32.000000 webdriver_cache_manager-0.0.2/src/webdriver_cache_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2023-12-07 20:01:32.000000 webdriver_cache_manager-0.0.2/src/webdriver_cache_manager/webdriver_cache_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 20:01:40.472680 webdriver_cache_manager-0.0.2/src/webdriver_cache_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2023-12-07 20:01:40.000000 webdriver_cache_manager-0.0.2/src/webdriver_cache_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-12-07 20:01:40.000000 webdriver_cache_manager-0.0.2/src/webdriver_cache_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 20:01:40.000000 webdriver_cache_manager-0.0.2/src/webdriver_cache_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-07 20:01:40.000000 webdriver_cache_manager-0.0.2/src/webdriver_cache_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:04:45.655012 webdriver_cache_manager-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 17:04:41.000000 webdriver_cache_manager-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-26 17:04:45.655012 webdriver_cache_manager-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-26 17:04:41.000000 webdriver_cache_manager-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-26 17:04:41.000000 webdriver_cache_manager-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 17:04:45.655012 webdriver_cache_manager-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:04:45.651012 webdriver_cache_manager-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:04:45.655012 webdriver_cache_manager-0.0.4/src/webdriver_cache_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:04:41.000000 webdriver_cache_manager-0.0.4/src/webdriver_cache_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-26 17:04:41.000000 webdriver_cache_manager-0.0.4/src/webdriver_cache_manager/webdriver_cache_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:04:45.655012 webdriver_cache_manager-0.0.4/src/webdriver_cache_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-26 17:04:45.000000 webdriver_cache_manager-0.0.4/src/webdriver_cache_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-26 17:04:45.000000 webdriver_cache_manager-0.0.4/src/webdriver_cache_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 17:04:45.000000 webdriver_cache_manager-0.0.4/src/webdriver_cache_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 17:04:45.000000 webdriver_cache_manager-0.0.4/src/webdriver_cache_manager.egg-info/top_level.txt
```

### Comparing `webdriver_cache_manager-0.0.2/LICENSE` & `webdriver_cache_manager-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `webdriver_cache_manager-0.0.2/PKG-INFO` & `webdriver_cache_manager-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdriver_cache_manager
-Version: 0.0.2
+Version: 0.0.4
 Summary: Optimize WebDriver usage in Selenium with Python. Manage processes, terminate efficiently, and handle PIDs using CSV. Simplify automation!
 Author-email: Muhammad Nawaz <MNawaz6935@gmail.com>
 Project-URL: Homepage, https://github.com/mnawaz6935/webdriver_cache_manager
 Project-URL: Issues, https://github.com/mnawaz6935/webdriver_cache_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # webdriver_cache_manager
 
 `webdriver_cache_manager` simplifies managing ChromeDriver instances in Selenium using Python. Track active processes, terminate unused instances, and handle associated PIDs with ease.
 
+[![Upload Python Package](https://github.com/mnawaz6935/webdriver_cache_manager/actions/workflows/python-publish.yml/badge.svg?branch=main)](https://github.com/mnawaz6935/webdriver_cache_manager/actions/workflows/python-publish.yml)
 ## Installation
 
 Install via pip:
 
 ```bash
 pip install webdriver_cache_manager
 ```
```

### Comparing `webdriver_cache_manager-0.0.2/pyproject.toml` & `webdriver_cache_manager-0.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "webdriver_cache_manager"
-version = "0.0.2"
+version = "0.0.4"
 authors = [
   { name="Muhammad Nawaz", email="MNawaz6935@gmail.com" },
 ]
 description = "Optimize WebDriver usage in Selenium with Python. Manage processes, terminate efficiently, and handle PIDs using CSV. Simplify automation!"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `webdriver_cache_manager-0.0.2/src/webdriver_cache_manager/webdriver_cache_manager.py` & `webdriver_cache_manager-0.0.4/src/webdriver_cache_manager/webdriver_cache_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,62 @@
 import csv
 import logging
+import os
 import subprocess
 import traceback
-
 import psutil
 
+CSV_FILE_PATH = os.path.join(os.path.join( os.path.expanduser("~"), ".wcm"), "pids.csv")
 
-def save_pids_to_csv(chrome_driver_pid, chrome_pid):
-    with open('pids.csv', 'a+', newline='') as csvfile:
-        fieldnames = ['Process', 'PID']
+def save_pids_to_csv(file_path, chrome_driver_pid, chrome_pid):
+    with open(CSV_FILE_PATH, 'a+', newline='') as csvfile:
+        fieldnames = ['File Path', 'ChromeDriver PID', 'Chrome PID']
         writer = csv.DictWriter(csvfile, fieldnames=fieldnames)
-        writer.writeheader()
-        writer.writerow({'Process': 'ChromeDriver', 'PID': chrome_driver_pid})
-        writer.writerow({'Process': 'Chrome', 'PID': chrome_pid})
+        writer.writerow({'File Path': file_path, 'ChromeDriver PID': chrome_driver_pid, 'Chrome PID': chrome_pid})
 
 
-def read_pids_from_csv():
+def read_pids_from_csv(file_path):
     chrome_driver_pid = []
     chrome_pid = []
     try:
-        with open('pids.csv', newline='') as csvfile:
+        with open(CSV_FILE_PATH, newline='') as csvfile:
             reader = csv.DictReader(csvfile)
             for row in reader:
-                if row['Process'] == 'ChromeDriver':
-                    chrome_driver_pid.append(int(row['PID']))
-                elif row['Process'] == 'Chrome':
-                    chrome_pid.append(int(row['PID']))
+                if row['File Path'] == file_path:
+                    chrome_driver_pid.append(int(row['ChromeDriver PID']))
+                    chrome_pid.append(int(row['Chrome PID']))
     except FileNotFoundError:
         pass
     try:
-        with open('pids.csv', 'w', newline=''):
+        with open(CSV_FILE_PATH, 'w', newline=''):
             pass
     except:
         logging.error('Unable to clear process_ids file.')
     return chrome_driver_pid, chrome_pid
 
 
 def kill_process_by_pid(pid):
     try:
         subprocess.run(['taskkill', '/pid', str(pid), '/f'], check=True)
         logging.info(f"Process with PID {pid} killed successfully.")
     except subprocess.CalledProcessError as e:
         logging.info(f"Failed to kill process with PID {pid}. Error: {e}")
 
 
-def ManageChromeDriverCache(driver):
+def KillChromeAndDriverCache(file_path):
+    chrome_driver_pids, chrome_pids = read_pids_from_csv(file_path)
+    if chrome_driver_pids:
+        for pid in chrome_driver_pids:
+            kill_process_by_pid(pid)
+    if chrome_pids:
+        for pid in chrome_pids:
+            kill_process_by_pid(pid)
+
+
+def ManageChromeDriverCache(driver, file_path):
     try:
         # Get the ChromeDriver process ID
         chrome_driver_pid = driver.service.process.pid
         logging.info(f"ChromeDriver Process ID: {chrome_driver_pid}")
 
         # Find the PID of the Chrome process opened by the WebDriver
         chrome_pid = None
@@ -62,17 +70,10 @@
                     pass
 
         if chrome_pid:
             logging.info(f"Chrome Process ID:{chrome_pid}")
         else:
             logging.info("Chrome process not found for this WebDriver instance.")
 
-        chrome_driver_pids, chrome_pids = read_pids_from_csv()
-        save_pids_to_csv(chrome_driver_pid, chrome_pid)
-        if chrome_driver_pids:
-            for chrome_driver_pid in chrome_driver_pids:
-                kill_process_by_pid(chrome_driver_pid)
-        if chrome_pids:
-            for chrome_pid in chrome_pids:
-                kill_process_by_pid(chrome_pid)
+        save_pids_to_csv(file_path, chrome_driver_pid, chrome_pid)
     except Exception as e:
         logging.error(traceback.format_exc())
```

### Comparing `webdriver_cache_manager-0.0.2/src/webdriver_cache_manager.egg-info/PKG-INFO` & `webdriver_cache_manager-0.0.4/src/webdriver_cache_manager.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: webdriver-cache-manager
-Version: 0.0.2
+Name: webdriver_cache_manager
+Version: 0.0.4
 Summary: Optimize WebDriver usage in Selenium with Python. Manage processes, terminate efficiently, and handle PIDs using CSV. Simplify automation!
 Author-email: Muhammad Nawaz <MNawaz6935@gmail.com>
 Project-URL: Homepage, https://github.com/mnawaz6935/webdriver_cache_manager
 Project-URL: Issues, https://github.com/mnawaz6935/webdriver_cache_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # webdriver_cache_manager
 
 `webdriver_cache_manager` simplifies managing ChromeDriver instances in Selenium using Python. Track active processes, terminate unused instances, and handle associated PIDs with ease.
 
+[![Upload Python Package](https://github.com/mnawaz6935/webdriver_cache_manager/actions/workflows/python-publish.yml/badge.svg?branch=main)](https://github.com/mnawaz6935/webdriver_cache_manager/actions/workflows/python-publish.yml)
 ## Installation
 
 Install via pip:
 
 ```bash
 pip install webdriver_cache_manager
 ```
```

