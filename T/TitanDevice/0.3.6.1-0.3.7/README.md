# Comparing `tmp/TitanDevice-0.3.6.1.tar.gz` & `tmp/TitanDevice-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.3.6.1.tar", last modified: Thu Apr 25 07:19:07 2024, max compression
+gzip compressed data, was "TitanDevice-0.3.7.tar", last modified: Fri Apr 26 10:24:36 2024, max compression
```

## Comparing `TitanDevice-0.3.6.1.tar` & `TitanDevice-0.3.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-25 07:19:07.549224 TitanDevice-0.3.6.1/
--rw-r--r--   0 mark      (1000) mark      (1000)      598 2024-04-25 07:19:07.549224 TitanDevice-0.3.6.1/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.3.6.1/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-25 07:19:07.549224 TitanDevice-0.3.6.1/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      598 2024-04-25 07:19:07.000000 TitanDevice-0.3.6.1/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-25 07:19:07.000000 TitanDevice-0.3.6.1/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-25 07:19:07.000000 TitanDevice-0.3.6.1/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-25 07:19:07.000000 TitanDevice-0.3.6.1/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-25 07:19:07.000000 TitanDevice-0.3.6.1/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-25 07:19:07.549224 TitanDevice-0.3.6.1/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      798 2024-04-25 07:18:59.000000 TitanDevice-0.3.6.1/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-25 07:19:07.549224 TitanDevice-0.3.6.1/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)     4205 2024-04-25 06:42:55.000000 TitanDevice-0.3.6.1/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1242 2024-04-25 02:18:35.000000 TitanDevice-0.3.6.1/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     7027 2024-04-25 07:18:59.000000 TitanDevice-0.3.6.1/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      559 2024-04-25 06:30:48.000000 TitanDevice-0.3.6.1/titan/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 10:24:36.043886 TitanDevice-0.3.7/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-26 10:24:36.043886 TitanDevice-0.3.7/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.3.7/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 10:24:36.039886 TitanDevice-0.3.7/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-26 10:24:36.000000 TitanDevice-0.3.7/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-26 10:24:36.000000 TitanDevice-0.3.7/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 10:24:36.000000 TitanDevice-0.3.7/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-26 10:24:36.000000 TitanDevice-0.3.7/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-26 10:24:36.000000 TitanDevice-0.3.7/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 10:24:36.043886 TitanDevice-0.3.7/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-26 10:24:31.000000 TitanDevice-0.3.7/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 10:24:36.039886 TitanDevice-0.3.7/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4205 2024-04-25 06:42:55.000000 TitanDevice-0.3.7/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1415 2024-04-26 10:24:31.000000 TitanDevice-0.3.7/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     7027 2024-04-25 07:52:49.000000 TitanDevice-0.3.7/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      559 2024-04-25 06:30:48.000000 TitanDevice-0.3.7/titan/_device_models.py
```

### Comparing `TitanDevice-0.3.6.1/PKG-INFO` & `TitanDevice-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.3.6.1
+Version: 0.3.7
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.3.6.1/TitanDevice.egg-info/PKG-INFO` & `TitanDevice-0.3.7/TitanDevice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.3.6.1
+Version: 0.3.7
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.3.6.1/setup.py` & `TitanDevice-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.3.6.1",
+    version="0.3.7",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.3.6.1/titan/__init__.py` & `TitanDevice-0.3.7/titan/__init__.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.3.6.1/titan/_device_exception.py` & `TitanDevice-0.3.7/titan/_device_exception.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,41 @@
-class DeviceNoFoundException(Exception):
+class TitanException(Exception):
+    def __init__(self, message: str):
+        super().__init__(message)
+
+
+class DeviceNoFoundException(TitanException):
     def __init__(self, device_serial):
         super().__init__(f"Device with serial {device_serial} not found")
 
 
-class DeviceMustBeRootedException(Exception):
+class DeviceMustBeRootedException(TitanException):
     def __init__(self, device_serial):
         super().__init__(
             f'Device [{device_serial}] must be rooted to perform this operation'
         )
 
 
-class FridaServerNotInstalled(Exception):
+class FridaServerNotInstalledException(TitanException):
     def __init__(self, device_serial, frida_server_path):
         super().__init__(
             f'Frida server is not installed in {frida_server_path} on device with serial {device_serial}'
         )
 
 
-class FridaServerNotRunning(Exception):
+class FridaServerNotRunningException(TitanException):
     def __init__(self, device_serial, frida_server_name):
         super().__init__(
             f'Frida server [{frida_server_name}] is not running on device with serial {device_serial}'
         )
 
 
-class PackageNotInstalled(Exception):
+class PackageNotInstalledException(TitanException):
     def __init__(self, device_serial, package_name):
         super().__init__(f'Package {package_name} is not installed in {device_serial}')
 
 
-class InstallPackageMustUninstallFirst(Exception):
+class InstallPackageMustUninstallFirstException(TitanException):
     def __init__(self, device_serial, package_name):
         super().__init__(
             f'Package {package_name} is already installed in {device_serial}'
         )
```

### Comparing `TitanDevice-0.3.6.1/titan/_device_manager.py` & `TitanDevice-0.3.7/titan/_device_manager.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.3.6.1/titan/_device_models.py` & `TitanDevice-0.3.7/titan/_device_models.py`

 * *Files identical despite different names*

