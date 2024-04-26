# Comparing `tmp/mozrunner-8.3.0.tar.gz` & `tmp/mozrunner-8.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozrunner-8.3.0.tar", last modified: Fri Aug  4 07:23:54 2023, max compression
+gzip compressed data, was "mozrunner-8.3.1.tar", last modified: Fri Apr 26 08:17:01 2024, max compression
```

## Comparing `mozrunner-8.3.0.tar` & `mozrunner-8.3.1.tar`

### file list

```diff
@@ -1,32 +1,40 @@
-drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-08-04 07:23:54.403684 mozrunner-8.3.0/
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      829 2023-08-04 07:23:54.403684 mozrunner-8.3.0/PKG-INFO
-drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-08-04 07:23:54.403684 mozrunner-8.3.0/mozrunner/
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      350 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/__init__.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     4610 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/application.py
-drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-08-04 07:23:54.403684 mozrunner-8.3.0/mozrunner/base/
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      353 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/base/__init__.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     4389 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/base/browser.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     6556 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/base/device.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     8839 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/base/runner.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     5644 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/cli.py
-drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-08-04 07:23:54.403684 mozrunner-8.3.0/mozrunner/devices/
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      487 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/devices/__init__.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    36892 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/devices/android_device.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     9067 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/devices/base.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     7373 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/devices/emulator.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1593 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/devices/emulator_battery.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      555 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/devices/emulator_geo.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     3478 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/devices/emulator_screen.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      535 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/errors.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     5191 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/runners.py
--rwxrwxr-x   0 jgraham   (1000) jgraham   (1000)    10403 2023-07-06 08:37:51.000000 mozrunner-8.3.0/mozrunner/utils.py
-drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-08-04 07:23:54.403684 mozrunner-8.3.0/mozrunner.egg-info/
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      829 2023-08-04 07:23:54.000000 mozrunner-8.3.0/mozrunner.egg-info/PKG-INFO
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      708 2023-08-04 07:23:54.000000 mozrunner-8.3.0/mozrunner.egg-info/SOURCES.txt
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2023-08-04 07:23:54.000000 mozrunner-8.3.0/mozrunner.egg-info/dependency_links.txt
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       44 2023-08-04 07:23:54.000000 mozrunner-8.3.0/mozrunner.egg-info/entry_points.txt
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2023-08-01 11:17:05.000000 mozrunner-8.3.0/mozrunner.egg-info/not-zip-safe
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      136 2023-08-04 07:23:54.000000 mozrunner-8.3.0/mozrunner.egg-info/requires.txt
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       10 2023-08-04 07:23:54.000000 mozrunner-8.3.0/mozrunner.egg-info/top_level.txt
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       67 2023-08-04 07:23:54.407684 mozrunner-8.3.0/setup.cfg
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1658 2023-08-03 14:51:45.000000 mozrunner-8.3.0/setup.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2024-04-26 08:17:01.621954 mozrunner-8.3.1/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      829 2024-04-26 08:17:01.621954 mozrunner-8.3.1/PKG-INFO
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2024-04-26 08:17:01.616954 mozrunner-8.3.1/mozrunner/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      350 2024-02-27 12:31:33.000000 mozrunner-8.3.1/mozrunner/__init__.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     4571 2024-02-27 12:31:33.000000 mozrunner-8.3.1/mozrunner/application.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2024-04-26 08:17:01.618954 mozrunner-8.3.1/mozrunner/base/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      353 2024-02-27 12:31:33.000000 mozrunner-8.3.1/mozrunner/base/__init__.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     4389 2024-02-27 12:31:33.000000 mozrunner-8.3.1/mozrunner/base/browser.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     6556 2024-02-27 12:31:33.000000 mozrunner-8.3.1/mozrunner/base/device.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     8839 2024-02-27 12:31:33.000000 mozrunner-8.3.1/mozrunner/base/runner.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     5644 2024-02-27 12:31:33.000000 mozrunner-8.3.1/mozrunner/cli.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2024-04-26 08:17:01.620954 mozrunner-8.3.1/mozrunner/devices/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      487 2024-02-27 12:31:33.000000 mozrunner-8.3.1/mozrunner/devices/__init__.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    37543 2024-03-14 12:27:46.000000 mozrunner-8.3.1/mozrunner/devices/android_device.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     9388 2024-04-15 11:43:40.000000 mozrunner-8.3.1/mozrunner/devices/base.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     7373 2024-02-27 12:31:33.000000 mozrunner-8.3.1/mozrunner/devices/emulator.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1593 2024-02-27 12:31:33.000000 mozrunner-8.3.1/mozrunner/devices/emulator_battery.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      555 2024-02-27 12:31:33.000000 mozrunner-8.3.1/mozrunner/devices/emulator_geo.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     3478 2024-02-27 12:31:33.000000 mozrunner-8.3.1/mozrunner/devices/emulator_screen.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      535 2024-02-27 12:31:33.000000 mozrunner-8.3.1/mozrunner/errors.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     5191 2024-02-27 12:31:33.000000 mozrunner-8.3.1/mozrunner/runners.py
+-rwxrwxr-x   0 jgraham   (1000) jgraham   (1000)    10402 2024-02-27 12:31:33.000000 mozrunner-8.3.1/mozrunner/utils.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2024-04-26 08:17:01.617954 mozrunner-8.3.1/mozrunner.egg-info/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      829 2024-04-26 08:17:01.000000 mozrunner-8.3.1/mozrunner.egg-info/PKG-INFO
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      855 2024-04-26 08:17:01.000000 mozrunner-8.3.1/mozrunner.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2024-04-26 08:17:01.000000 mozrunner-8.3.1/mozrunner.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       44 2024-04-26 08:17:01.000000 mozrunner-8.3.1/mozrunner.egg-info/entry_points.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2024-04-26 08:17:01.000000 mozrunner-8.3.1/mozrunner.egg-info/not-zip-safe
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      136 2024-04-26 08:17:01.000000 mozrunner-8.3.1/mozrunner.egg-info/requires.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       10 2024-04-26 08:17:01.000000 mozrunner-8.3.1/mozrunner.egg-info/top_level.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       67 2024-04-26 08:17:01.622954 mozrunner-8.3.1/setup.cfg
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1658 2024-04-26 08:14:51.000000 mozrunner-8.3.1/setup.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2024-04-26 08:17:01.621954 mozrunner-8.3.1/tests/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1046 2024-02-27 12:31:33.000000 mozrunner-8.3.1/tests/test_crash.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      963 2024-02-27 12:31:33.000000 mozrunner-8.3.1/tests/test_interactive.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1422 2024-02-27 12:31:33.000000 mozrunner-8.3.1/tests/test_start.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      470 2024-02-27 12:31:33.000000 mozrunner-8.3.1/tests/test_states.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1148 2024-02-27 12:31:33.000000 mozrunner-8.3.1/tests/test_stop.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1601 2024-02-27 12:31:33.000000 mozrunner-8.3.1/tests/test_threads.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      863 2024-02-27 12:31:33.000000 mozrunner-8.3.1/tests/test_wait.py
```

### Comparing `mozrunner-8.3.0/PKG-INFO` & `mozrunner-8.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozrunner
-Version: 8.3.0
+Version: 8.3.1
 Summary: Reliable start/stop/configuration of Mozilla Applications (Firefox, Thunderbird, etc.)
 Home-page: https://wiki.mozilla.org/Auto-tools/Projects/Mozbase
 Author: Mozilla Automation and Tools team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
 Keywords: mozilla
 Classifier: Environment :: Console
```

### Comparing `mozrunner-8.3.0/mozrunner/application.py` & `mozrunner-8.3.1/mozrunner/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 import os
 import posixpath
 from abc import ABCMeta, abstractmethod
-from distutils.spawn import find_executable
+from shutil import which
 
 import six
 from mozdevice import ADBDeviceFactory
 from mozprofile import (
     ChromeProfile,
     ChromiumProfile,
     FirefoxProfile,
@@ -47,15 +47,15 @@
     _bindir = None
     remote_test_root = ""
     remote_process = None
 
     @property
     def bindir(self):
         if self._bindir is None:
-            paths = [find_executable("emulator")]
+            paths = [which("emulator")]
             paths = [p for p in paths if p is not None if os.path.isfile(p)]
             if not paths:
                 self._bindir = ""
             else:
                 self._bindir = os.path.dirname(paths[0])
         return self._bindir
 
@@ -84,15 +84,15 @@
 
     def which(self, binary):
         paths = os.environ.get("PATH", {}).split(os.pathsep)
         if self.bindir is not None and os.path.abspath(self.bindir) not in paths:
             paths.insert(0, os.path.abspath(self.bindir))
             os.environ["PATH"] = os.pathsep.join(paths)
 
-        return find_executable(binary)
+        return which(binary)
 
     @abstractmethod
     def stop_application(self):
         """Run (device manager) command to stop application."""
         pass
```

### Comparing `mozrunner-8.3.0/mozrunner/base/browser.py` & `mozrunner-8.3.1/mozrunner/base/browser.py`

 * *Files identical despite different names*

### Comparing `mozrunner-8.3.0/mozrunner/base/device.py` & `mozrunner-8.3.1/mozrunner/base/device.py`

 * *Files identical despite different names*

### Comparing `mozrunner-8.3.0/mozrunner/base/runner.py` & `mozrunner-8.3.1/mozrunner/base/runner.py`

 * *Files identical despite different names*

### Comparing `mozrunner-8.3.0/mozrunner/cli.py` & `mozrunner-8.3.1/mozrunner/cli.py`

 * *Files identical despite different names*

### Comparing `mozrunner-8.3.0/mozrunner/devices/android_device.py` & `mozrunner-8.3.1/mozrunner/devices/android_device.py`

 * *Files 12% similar despite different names*

```diff
@@ -172,15 +172,14 @@
         ],
         True,
     ),
 }
 
 
 def _get_device(substs, device_serial=None):
-
     adb_path = _find_sdk_exe(substs, "adb", False)
     if not adb_path:
         adb_path = "adb"
     device = ADBDeviceFactory(
         adb=adb_path, verbose=verbose_logging, device=device_serial
     )
     return device
@@ -257,15 +256,15 @@
                 m = re.search('.*"(host-utils-.*)"', line)
                 if m:
                     manifest_version = m.group(1)
                     break
 
     # Compare, prompt, update
     if existing_version and manifest_version:
-        hu_version_regex = "host-utils-([\d\.]*)"
+        hu_version_regex = r"host-utils-([\d\.]*)"
         manifest_version = float(re.search(hu_version_regex, manifest_version).group(1))
         existing_version = float(re.search(hu_version_regex, existing_version).group(1))
         if existing_version < manifest_version:
             _log_info("Your host utilities are out of date!")
             _log_info(
                 "You have %s installed, but %s is available"
                 % (existing_version, manifest_version)
@@ -302,19 +301,29 @@
     If 'debugger' is specified, also check that lldb-server is installed;
     if it is not found, set it up.
     If 'network' is specified, also check that the device has basic
     network connectivity.
     Returns True if the emulator was started or another device was
     already connected.
     """
-    if "MOZ_DISABLE_ADB_INSTALL" in os.environ:
+    if "MOZ_DISABLE_ADB_INSTALL" in os.environ or install == InstallIntent.NO:
         install = InstallIntent.NO
         _log_info(
-            "Found MOZ_DISABLE_ADB_INSTALL in environment, skipping android app"
-            "installation"
+            "Found MOZ_DISABLE_ADB_INSTALL in environment and/or the"
+            " --noinstall flag, skipping android app installation"
+        )
+    else:
+        _log_info(
+            "*********************************************************************\n"
+            "Neither the MOZ_DISABLE_ADB_INSTALL environment variable nor the\n"
+            "--noinstall flag was found. The code will now uninstall the current\n"
+            "app then re-install the android app from a different source. If you\n"
+            "don't want this set your local env so that\n"
+            "MOZ_DISABLE_ADB_INSTALL=True or pass the --noinstall flag\n"
+            "*********************************************************************"
         )
     device_verified = False
     emulator = AndroidEmulator("*", substs=build_obj.substs, verbose=verbose)
     adb_path = _find_sdk_exe(build_obj.substs, "adb", False)
     if not adb_path:
         adb_path = "adb"
     adbhost = ADBHost(adb=adb_path, verbose=verbose, timeout=SHORT_TIMEOUT)
```

### Comparing `mozrunner-8.3.0/mozrunner/devices/base.py` & `mozrunner-8.3.1/mozrunner/devices/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,19 +110,22 @@
         config = ProfileConfigParser()
         config.read(local_profiles_ini.name)
         for section in config.sections():
             if "Profile" in section:
                 config.set(section, "IsRelative", 0)
                 config.set(section, "Path", self.app_ctx.remote_profile)
 
-        new_profiles_ini = tempfile.NamedTemporaryFile()
-        config.write(open(new_profiles_ini.name, "w"))
-
-        self.backup_file(self.app_ctx.remote_profiles_ini)
-        self.device.push(new_profiles_ini.name, self.app_ctx.remote_profiles_ini)
+        # delete=False to allow opening the same file from ADB on Windows.
+        # The file will still be deleted at the end of the `with` block.
+        # See the "Opening the temporary file again" paragraph in:
+        # https://docs.python.org/3/library/tempfile.html#tempfile.NamedTemporaryFile
+        with tempfile.NamedTemporaryFile(mode="w", delete=False) as new_profiles_ini:
+            config.write(new_profiles_ini)
+            self.backup_file(self.app_ctx.remote_profiles_ini)
+            self.device.push(new_profiles_ini.name, self.app_ctx.remote_profiles_ini)
 
         # Ideally all applications would read the profile the same way, but in practice
         # this isn't true. Perform application specific profile-related setup if necessary.
         if hasattr(self.app_ctx, "setup_profile"):
             for remote_path in self.app_ctx.remote_backup_files:
                 self.backup_file(remote_path)
             self.app_ctx.setup_profile(profile)
@@ -238,19 +241,19 @@
 
     def optionxform(self, optionstr):
         return optionstr
 
     def write(self, fp):
         if self._defaults:
             fp.write("[%s]\n" % ConfigParser.DEFAULTSECT)
-            for (key, value) in self._defaults.items():
+            for key, value in self._defaults.items():
                 fp.write("%s=%s\n" % (key, str(value).replace("\n", "\n\t")))
             fp.write("\n")
         for section in self._sections:
             fp.write("[%s]\n" % section)
-            for (key, value) in self._sections[section].items():
+            for key, value in self._sections[section].items():
                 if key == "__name__":
                     continue
                 if (value is not None) or (self._optcre == self.OPTCRE):
                     key = "=".join((key, str(value).replace("\n", "\n\t")))
                 fp.write("%s\n" % (key))
             fp.write("\n")
```

### Comparing `mozrunner-8.3.0/mozrunner/devices/emulator.py` & `mozrunner-8.3.1/mozrunner/devices/emulator.py`

 * *Files identical despite different names*

### Comparing `mozrunner-8.3.0/mozrunner/devices/emulator_battery.py` & `mozrunner-8.3.1/mozrunner/devices/emulator_battery.py`

 * *Files identical despite different names*

### Comparing `mozrunner-8.3.0/mozrunner/devices/emulator_geo.py` & `mozrunner-8.3.1/mozrunner/devices/emulator_geo.py`

 * *Files identical despite different names*

### Comparing `mozrunner-8.3.0/mozrunner/devices/emulator_screen.py` & `mozrunner-8.3.1/mozrunner/devices/emulator_screen.py`

 * *Files identical despite different names*

### Comparing `mozrunner-8.3.0/mozrunner/errors.py` & `mozrunner-8.3.1/mozrunner/errors.py`

 * *Files identical despite different names*

### Comparing `mozrunner-8.3.0/mozrunner/runners.py` & `mozrunner-8.3.1/mozrunner/runners.py`

 * *Files identical despite different names*

### Comparing `mozrunner-8.3.0/mozrunner/utils.py` & `mozrunner-8.3.1/mozrunner/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
                 key = key.strip()
                 value = value.strip()
                 ret[key] = value
         if dist.has_metadata("requires.txt"):
             ret["Dependencies"] = "\n" + dist.get_metadata("requires.txt")
         return ret
 
-
 except ImportError:
     # package resources not avaialable
     def get_metadata_from_egg(module):
         return {}
 
 
 def findInPath(fileName, path=os.environ["PATH"]):
```

### Comparing `mozrunner-8.3.0/mozrunner.egg-info/PKG-INFO` & `mozrunner-8.3.1/mozrunner.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozrunner
-Version: 8.3.0
+Version: 8.3.1
 Summary: Reliable start/stop/configuration of Mozilla Applications (Firefox, Thunderbird, etc.)
 Home-page: https://wiki.mozilla.org/Auto-tools/Projects/Mozbase
 Author: Mozilla Automation and Tools team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
 Keywords: mozilla
 Classifier: Environment :: Console
```

### Comparing `mozrunner-8.3.0/mozrunner.egg-info/SOURCES.txt` & `mozrunner-8.3.1/mozrunner.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,8 +19,15 @@
 mozrunner/base/runner.py
 mozrunner/devices/__init__.py
 mozrunner/devices/android_device.py
 mozrunner/devices/base.py
 mozrunner/devices/emulator.py
 mozrunner/devices/emulator_battery.py
 mozrunner/devices/emulator_geo.py
-mozrunner/devices/emulator_screen.py
+mozrunner/devices/emulator_screen.py
+tests/test_crash.py
+tests/test_interactive.py
+tests/test_start.py
+tests/test_states.py
+tests/test_stop.py
+tests/test_threads.py
+tests/test_wait.py
```

### Comparing `mozrunner-8.3.0/setup.py` & `mozrunner-8.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
 from setuptools import find_packages, setup
 
 PACKAGE_NAME = "mozrunner"
-PACKAGE_VERSION = "8.3.0"
+PACKAGE_VERSION = "8.3.1"
 
 desc = """Reliable start/stop/configuration of Mozilla Applications (Firefox, Thunderbird, etc.)"""
 
 deps = [
     "mozdevice>=4.0.0,<5",
     "mozfile>=1.2",
     "mozinfo>=0.7,<2",
     "mozlog>=6.0",
     "mozprocess>=1.3.0,<2",
-    "mozprofile~=2.3",
+    "mozprofile~=3.0",
     "six>=1.13.0,<2",
 ]
 
 EXTRAS_REQUIRE = {"crash": ["mozcrash >= 2.0"]}
 
 setup(
     name=PACKAGE_NAME,
```

