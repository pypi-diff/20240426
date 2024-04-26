# Comparing `tmp/mozprofile-2.6.1.tar.gz` & `tmp/mozprofile-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mozprofile-2.6.1.tar", last modified: Thu Sep  7 19:04:43 2023, max compression
+gzip compressed data, was "mozprofile-3.0.0.tar", last modified: Fri Apr 26 08:16:25 2024, max compression
```

## Comparing `mozprofile-2.6.1.tar` & `mozprofile-3.0.0.tar`

### file list

```diff
@@ -1,21 +1,33 @@
-drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-09-07 19:04:43.000000 mozprofile-2.6.1/
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      823 2023-09-07 19:04:43.000000 mozprofile-2.6.1/PKG-INFO
-drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-09-07 19:04:43.000000 mozprofile-2.6.1/mozprofile/
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      729 2023-03-10 23:28:57.000000 mozprofile-2.6.1/mozprofile/__init__.py
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)    13425 2023-03-10 23:28:57.000000 mozprofile-2.6.1/mozprofile/addons.py
--rwxrwxr-x   0 gbrown    (1000) gbrown    (1000)     5779 2023-09-07 15:26:46.000000 mozprofile-2.6.1/mozprofile/cli.py
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     2340 2023-09-07 15:26:46.000000 mozprofile-2.6.1/mozprofile/diff.py
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)    10411 2023-03-22 17:09:12.000000 mozprofile-2.6.1/mozprofile/permissions.py
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     8785 2023-09-07 15:26:46.000000 mozprofile-2.6.1/mozprofile/prefs.py
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)    19761 2023-09-07 15:26:46.000000 mozprofile-2.6.1/mozprofile/profile.py
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     1181 2023-09-07 15:26:46.000000 mozprofile-2.6.1/mozprofile/view.py
-drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-09-07 19:04:43.000000 mozprofile-2.6.1/mozprofile.egg-info/
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      823 2023-09-07 19:04:43.000000 mozprofile-2.6.1/mozprofile.egg-info/PKG-INFO
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      425 2023-09-07 19:04:43.000000 mozprofile-2.6.1/mozprofile.egg-info/SOURCES.txt
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2023-09-07 19:04:43.000000 mozprofile-2.6.1/mozprofile.egg-info/dependency_links.txt
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      187 2023-09-07 19:04:43.000000 mozprofile-2.6.1/mozprofile.egg-info/entry_points.txt
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2023-09-07 19:04:43.000000 mozprofile-2.6.1/mozprofile.egg-info/not-zip-safe
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       72 2023-09-07 19:04:43.000000 mozprofile-2.6.1/mozprofile.egg-info/requires.txt
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       11 2023-09-07 19:04:43.000000 mozprofile-2.6.1/mozprofile.egg-info/top_level.txt
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       67 2023-09-07 19:04:43.000000 mozprofile-2.6.1/setup.cfg
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     1629 2023-09-07 18:38:33.000000 mozprofile-2.6.1/setup.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2024-04-26 08:16:25.535667 mozprofile-3.0.0/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      804 2024-04-26 08:16:25.535667 mozprofile-3.0.0/PKG-INFO
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2024-04-26 08:16:25.534667 mozprofile-3.0.0/mozprofile/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      729 2024-02-27 12:31:33.000000 mozprofile-3.0.0/mozprofile/__init__.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    13425 2024-02-27 12:31:33.000000 mozprofile-3.0.0/mozprofile/addons.py
+-rwxrwxr-x   0 jgraham   (1000) jgraham   (1000)     5779 2024-02-27 12:31:33.000000 mozprofile-3.0.0/mozprofile/cli.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     2340 2024-02-27 12:31:33.000000 mozprofile-3.0.0/mozprofile/diff.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    10411 2024-02-27 12:31:33.000000 mozprofile-3.0.0/mozprofile/permissions.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     8785 2024-02-27 12:31:33.000000 mozprofile-3.0.0/mozprofile/prefs.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    19761 2024-04-24 14:12:44.000000 mozprofile-3.0.0/mozprofile/profile.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1181 2024-02-27 12:31:33.000000 mozprofile-3.0.0/mozprofile/view.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2024-04-26 08:16:25.534667 mozprofile-3.0.0/mozprofile.egg-info/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      804 2024-04-26 08:16:25.000000 mozprofile-3.0.0/mozprofile.egg-info/PKG-INFO
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      701 2024-04-26 08:16:25.000000 mozprofile-3.0.0/mozprofile.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2024-04-26 08:16:25.000000 mozprofile-3.0.0/mozprofile.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      126 2024-04-26 08:16:25.000000 mozprofile-3.0.0/mozprofile.egg-info/entry_points.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2024-04-26 08:15:24.000000 mozprofile-3.0.0/mozprofile.egg-info/not-zip-safe
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       72 2024-04-26 08:16:25.000000 mozprofile-3.0.0/mozprofile.egg-info/requires.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       11 2024-04-26 08:16:25.000000 mozprofile-3.0.0/mozprofile.egg-info/top_level.txt
+-rw-r--r--   0 jgraham   (1000) jgraham   (1000)       67 2024-04-26 08:16:25.535667 mozprofile-3.0.0/setup.cfg
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1629 2024-04-26 08:14:51.000000 mozprofile-3.0.0/setup.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2024-04-26 08:16:25.535667 mozprofile-3.0.0/tests/
+-rwxrwxr-x   0 jgraham   (1000) jgraham   (1000)     5101 2024-02-27 12:31:33.000000 mozprofile-3.0.0/tests/test_addonid.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    11227 2024-02-27 12:31:33.000000 mozprofile-3.0.0/tests/test_addons.py
+-rwxrwxr-x   0 jgraham   (1000) jgraham   (1000)     1190 2024-02-27 12:31:33.000000 mozprofile-3.0.0/tests/test_bug758250.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1836 2024-02-27 12:31:33.000000 mozprofile-3.0.0/tests/test_chrome_profile.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     2070 2024-02-27 12:31:33.000000 mozprofile-3.0.0/tests/test_clone_cleanup.py
+-rwxrwxr-x   0 jgraham   (1000) jgraham   (1000)     1090 2024-02-27 12:31:33.000000 mozprofile-3.0.0/tests/test_nonce.py
+-rwxrwxr-x   0 jgraham   (1000) jgraham   (1000)     1967 2024-02-27 12:31:33.000000 mozprofile-3.0.0/tests/test_permissions.py
+-rwxrwxr-x   0 jgraham   (1000) jgraham   (1000)    13241 2024-02-27 12:31:33.000000 mozprofile-3.0.0/tests/test_preferences.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     2961 2024-02-27 12:31:33.000000 mozprofile-3.0.0/tests/test_profile.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     2170 2024-02-27 12:31:33.000000 mozprofile-3.0.0/tests/test_profile_view.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     3464 2024-02-27 12:31:33.000000 mozprofile-3.0.0/tests/test_server_locations.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mozprofile-2.6.1/PKG-INFO` & `mozprofile-3.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: mozprofile
-Version: 2.6.1
+Version: 3.0.0
 Summary: Library to create and modify Mozilla application profiles
 Home-page: https://wiki.mozilla.org/Auto-tools/Projects/Mozbase
 Author: Mozilla Automation and Tools team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
 Keywords: mozilla
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: manifest
 
 see https://firefox-source-docs.mozilla.org/mozbase/index.html
-
```

### Comparing `mozprofile-2.6.1/mozprofile/__init__.py` & `mozprofile-3.0.0/mozprofile/__init__.py`

 * *Files identical despite different names*

### Comparing `mozprofile-2.6.1/mozprofile/addons.py` & `mozprofile-3.0.0/mozprofile/addons.py`

 * *Files identical despite different names*

### Comparing `mozprofile-2.6.1/mozprofile/cli.py` & `mozprofile-3.0.0/mozprofile/cli.py`

 * *Files identical despite different names*

### Comparing `mozprofile-2.6.1/mozprofile/diff.py` & `mozprofile-3.0.0/mozprofile/diff.py`

 * *Files identical despite different names*

### Comparing `mozprofile-2.6.1/mozprofile/permissions.py` & `mozprofile-3.0.0/mozprofile/permissions.py`

 * *Files identical despite different names*

### Comparing `mozprofile-2.6.1/mozprofile/prefs.py` & `mozprofile-3.0.0/mozprofile/prefs.py`

 * *Files identical despite different names*

### Comparing `mozprofile-2.6.1/mozprofile/profile.py` & `mozprofile-3.0.0/mozprofile/profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -192,38 +192,38 @@
         self,
         profile=None,
         addons=None,
         preferences=None,
         locations=None,
         proxy=None,
         restore=True,
-        whitelistpaths=None,
+        allowlistpaths=None,
         **kwargs
     ):
         """
         :param profile: Path to the profile
         :param addons: String of one or list of addons to install
         :param preferences: Dictionary or class of preferences
         :param locations: ServerLocations object
         :param proxy: Setup a proxy
         :param restore: Flag for removing all custom settings during cleanup
-        :param whitelistpaths: List of paths to pass to Firefox to allow read
+        :param allowlistpaths: List of paths to pass to Firefox to allow read
             access to from the content process sandbox.
         """
         super(Profile, self).__init__(
             profile=profile,
             addons=addons,
             preferences=preferences,
             restore=restore,
             **kwargs
         )
 
         self._locations = locations
         self._proxy = proxy
-        self._whitelistpaths = whitelistpaths
+        self._allowlistpaths = allowlistpaths
 
         # Initialize all class members
         self._reset()
 
     def _reset(self):
         """Internal: Initialize all class members to their default value"""
 
@@ -245,38 +245,38 @@
             self.set_preferences(self.__class__.preferences)
         # Set additional preferences
         self.set_preferences(self._preferences)
 
         self.permissions = Permissions(self._locations)
         prefs_js, user_js = self.permissions.network_prefs(self._proxy)
 
-        if self._whitelistpaths:
+        if self._allowlistpaths:
             # On macOS we don't want to support a generalized read whitelist,
             # and the macOS sandbox policy language doesn't have support for
             # lists, so we handle these specially.
             if platform.system() == "Darwin":
-                assert len(self._whitelistpaths) <= 2
-                if len(self._whitelistpaths) == 2:
+                assert len(self._allowlistpaths) <= 2
+                if len(self._allowlistpaths) == 2:
                     prefs_js.append(
                         (
                             "security.sandbox.content.mac.testing_read_path2",
-                            self._whitelistpaths[1],
+                            self._allowlistpaths[1],
                         )
                     )
                 prefs_js.append(
                     (
                         "security.sandbox.content.mac.testing_read_path1",
-                        self._whitelistpaths[0],
+                        self._allowlistpaths[0],
                     )
                 )
             else:
                 prefs_js.append(
                     (
                         "security.sandbox.content.read_path_whitelist",
-                        ",".join(self._whitelistpaths),
+                        ",".join(self._allowlistpaths),
                     )
                 )
         self.set_preferences(prefs_js, "prefs.js")
         self.set_preferences(user_js)
 
         # handle add-on installation
         self.addons = AddonManager(self.profile, restore=self.restore)
```

### Comparing `mozprofile-2.6.1/mozprofile/view.py` & `mozprofile-3.0.0/mozprofile/view.py`

 * *Files identical despite different names*

### Comparing `mozprofile-2.6.1/mozprofile.egg-info/PKG-INFO` & `mozprofile-3.0.0/mozprofile.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: mozprofile
-Version: 2.6.1
+Version: 3.0.0
 Summary: Library to create and modify Mozilla application profiles
 Home-page: https://wiki.mozilla.org/Auto-tools/Projects/Mozbase
 Author: Mozilla Automation and Tools team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
 Keywords: mozilla
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: manifest
 
 see https://firefox-source-docs.mozilla.org/mozbase/index.html
-
```

### Comparing `mozprofile-2.6.1/setup.py` & `mozprofile-3.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
 from setuptools import setup
 
 PACKAGE_NAME = "mozprofile"
-PACKAGE_VERSION = "2.6.1"
+PACKAGE_VERSION = "3.0.0"
 
 deps = [
     "mozfile>=1.2",
     "mozlog>=6.0",
     "six>=1.13.0,<2",
 ]
```

