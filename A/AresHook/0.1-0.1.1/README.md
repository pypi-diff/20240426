# Comparing `tmp/AresHook-0.1.tar.gz` & `tmp/AresHook-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AresHook-0.1.tar", last modified: Tue Apr 23 03:38:00 2024, max compression
+gzip compressed data, was "AresHook-0.1.1.tar", last modified: Fri Apr 26 10:22:40 2024, max compression
```

## Comparing `AresHook-0.1.tar` & `AresHook-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,19 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 03:38:00.795336 AresHook-0.1/
--rw-rw-r--   0 mark      (1000) mark      (1000)       45 2024-04-23 03:37:51.000000 AresHook-0.1/.gitignore
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 03:38:00.795336 AresHook-0.1/AresHook.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      582 2024-04-23 03:38:00.000000 AresHook-0.1/AresHook.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      399 2024-04-23 03:38:00.000000 AresHook-0.1/AresHook.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-23 03:38:00.000000 AresHook-0.1/AresHook.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-23 03:38:00.000000 AresHook-0.1/AresHook.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-23 03:38:00.000000 AresHook-0.1/AresHook.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)      582 2024-04-23 03:38:00.795336 AresHook-0.1/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      257 2024-04-19 09:23:58.000000 AresHook-0.1/README.md
--rw-rw-r--   0 mark      (1000) mark      (1000)      200 2024-04-19 09:23:58.000000 AresHook-0.1/README.zh.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 03:38:00.795336 AresHook-0.1/ares/
--rw-rw-r--   0 mark      (1000) mark      (1000)      299 2024-04-22 01:16:12.000000 AresHook-0.1/ares/__init__.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 03:38:00.795336 AresHook-0.1/ares/_dobby/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2024-04-19 09:23:00.000000 AresHook-0.1/ares/_dobby/__init__.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 03:38:00.795336 AresHook-0.1/ares/_frida/
--rw-rw-r--   0 mark      (1000) mark      (1000)       70 2024-04-22 01:16:12.000000 AresHook-0.1/ares/_frida/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      941 2024-04-22 01:16:12.000000 AresHook-0.1/ares/_frida/_frida_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3331 2024-04-22 09:26:14.000000 AresHook-0.1/ares/_frida/_frida_hooker.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 03:38:00.795336 AresHook-0.1/ares/_sl_rom_hook/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2024-04-19 09:22:27.000000 AresHook-0.1/ares/_sl_rom_hook/__init__.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 03:38:00.795336 AresHook-0.1/ares/_xposed/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2024-04-19 09:22:47.000000 AresHook-0.1/ares/_xposed/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       57 2024-04-18 07:31:20.000000 AresHook-0.1/requirements.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-23 03:38:00.795336 AresHook-0.1/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      753 2024-04-23 02:39:30.000000 AresHook-0.1/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 10:22:40.697093 AresHook-0.1.1/
+-rw-rw-r--   0 mark      (1000) mark      (1000)       64 2024-04-23 06:07:42.000000 AresHook-0.1.1/.gitignore
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 10:22:40.697093 AresHook-0.1.1/AresHook.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      608 2024-04-26 10:22:40.000000 AresHook-0.1.1/AresHook.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      287 2024-04-26 10:22:40.000000 AresHook-0.1.1/AresHook.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 10:22:40.000000 AresHook-0.1.1/AresHook.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       27 2024-04-26 10:22:40.000000 AresHook-0.1.1/AresHook.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 10:22:40.000000 AresHook-0.1.1/AresHook.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)      608 2024-04-26 10:22:40.697093 AresHook-0.1.1/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      257 2024-04-19 09:23:58.000000 AresHook-0.1.1/README.md
+-rw-rw-r--   0 mark      (1000) mark      (1000)      200 2024-04-19 09:23:58.000000 AresHook-0.1.1/README.zh.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 10:22:40.697093 AresHook-0.1.1/ares/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      299 2024-04-22 01:16:12.000000 AresHook-0.1.1/ares/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1112 2024-04-26 10:22:24.000000 AresHook-0.1.1/ares/_exceptions.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3018 2024-04-26 10:18:17.000000 AresHook-0.1.1/ares/_frida.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      159 2024-04-26 10:16:53.000000 AresHook-0.1.1/ares/_modules.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)       77 2024-04-26 09:57:14.000000 AresHook-0.1.1/requirements.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 10:22:40.697093 AresHook-0.1.1/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      774 2024-04-26 10:22:24.000000 AresHook-0.1.1/setup.py
```

### Comparing `AresHook-0.1/ares/_frida/_frida_exception.py` & `AresHook-0.1.1/ares/_exceptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-class FridaServerNotRunning(Exception):
+class AresException(Exception):
+    def __init__(self, message: str):
+        super().__init__(message)
+
+
+class FridaServerNotRunningException(AresException):
     def __init__(self, device_serial: str):
         super().__init__(
             f"Frida server is not running on device with serial {device_serial}"
         )
 
 
-class FridaDeviceNotFound(Exception):
+class FridaDeviceNotFoundException(AresException):
     def __init__(self, device_serial: str):
         super().__init__(f"Device with serial {device_serial} not found")
 
 
-class FridaProcessNotAttached(Exception):
+class FridaProcessNotAttachedException(AresException):
     def __init__(self):
         super().__init__("No session attached. Please call attach() method first.")
 
 
-class FridaTargetNotRunning(Exception):
+class FridaTargetNotRunningException(AresException):
     def __init__(self, target: [str, int]):
         if isinstance(target, int):
             super().__init__(f"Target with PID {target} is not running")
         else:
             super().__init__(f"Target {target} is not running")
 
 
-class FridaPackageNotInstalled(Exception):
+class FridaPackageNotInstalledException(AresException):
     def __init__(self, package_name: str):
         super().__init__(f"Package {package_name} is not installed")
```

### Comparing `AresHook-0.1/ares/_frida/_frida_hooker.py` & `AresHook-0.1.1/ares/_frida.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from functools import wraps
 
 import frida
-from frida.core import Device
+from frida.core import Device, Script, Session
 
-from ares._frida._frida_exception import *
+from ._exceptions import FridaPackageNotInstalled, FridaProcessNotAttached, \
+    FridaServerNotRunning, FridaTargetNotRunning
 
 
 class FridaHooker:
-    _device: frida.core.Device
-    _session: frida.core.Session
+    _device: Device
+    _session: Session
     _attached_pid: int
-    _running_script: list[frida.core.Script]
+    _running_script: list[Script]
 
     @staticmethod
     def __check_session(func):
         @wraps(func)
         def inner(self, *args, **kwargs):
             if self._session is None:
                 raise FridaProcessNotAttached()
@@ -51,23 +52,14 @@
 
     def __get_pid(self, target: [str | int]) -> int:
         if isinstance(target, int):
             return target
         return self._device.get_process(target).pid
 
     def attach(self, target: [str | int]) -> "FridaHooker":
-        """
-        :param target: The target to attach to.
-        Can be either a string
-            representing the process name or an integer
-            representing the process ID.
-        :return: An instance of FridaHooker
-        that is attached to the specified target.
-
-        """
         if not self.__is_package_running(target):
             raise FridaTargetNotRunning(target)
         target = self.__get_pid(target)
         if self._session is None:
             self._session = self._device.attach(target)
             self._attached_pid = target
         else:
@@ -89,10 +81,10 @@
     def resume(self) -> "FridaHooker":
         if self._attached_pid is not None:
             self._device.resume(self._attached_pid)
         return self
 
     @__check_session
     def run_script(self, script: str) -> "FridaHooker":
-        # TODO: record script, check if script is running(use hash to identify script)
+
         self._running_script.append(self._session.create_script(script))
         return self
```

### Comparing `AresHook-0.1/setup.py` & `AresHook-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='AresHook',
-    version='0.1',  # 初始版本号，如果使用自动版本管理，这个值可以是任意值
+    version='0.1.1',  # 初始版本号，如果使用自动版本管理，这个值可以是任意值
     author='369',
     author_email='luck.yangbo@gmail.com',
     description='A simple hook library.',
     long_description=long_description,
     packages=find_packages(),  # 自动查找并包含所有包
     install_requires=[
         'frida',
         'frida-tools',
+        'pydantic'
     ],
     setup_requires=['setuptools_scm'],
     use_scm_version=True,
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

