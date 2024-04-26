# Comparing `tmp/crunpyroll-2.3.5.tar.gz` & `tmp/crunpyroll-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunpyroll-2.3.5.tar", last modified: Sun Feb 18 14:10:55 2024, max compression
+gzip compressed data, was "crunpyroll-2.4.tar", last modified: Fri Apr 26 11:27:52 2024, max compression
```

## Comparing `crunpyroll-2.3.5.tar` & `crunpyroll-2.4.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 14:10:55.082695 crunpyroll-2.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-02-18 14:10:55.082695 crunpyroll-2.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 14:10:55.078695 crunpyroll-2.3.5/crunpyroll/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 14:10:55.078695 crunpyroll-2.3.5/crunpyroll/enums/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/enums/api_host.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/enums/content_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/enums/image_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 14:10:55.082695 crunpyroll-2.3.5/crunpyroll/methods/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/methods/get_episodes.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/methods/get_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/methods/get_license.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/methods/get_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/methods/get_old_streams.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/methods/get_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/methods/get_seasons.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/methods/get_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/methods/get_streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/methods/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 14:10:55.082695 crunpyroll-2.3.5/crunpyroll/types/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/types/cms.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/types/content.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/types/drm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/types/episodes.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/types/hardsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/types/images.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/types/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/types/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/types/movies.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/types/obj.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/types/old_streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/types/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/types/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/types/seasons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/types/series.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/types/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/types/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/crunpyroll/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 14:10:55.082695 crunpyroll-2.3.5/crunpyroll.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-02-18 14:10:55.000000 crunpyroll-2.3.5/crunpyroll.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-02-18 14:10:55.000000 crunpyroll-2.3.5/crunpyroll.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-18 14:10:55.000000 crunpyroll-2.3.5/crunpyroll.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-18 14:10:55.000000 crunpyroll-2.3.5/crunpyroll.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-18 14:10:55.000000 crunpyroll-2.3.5/crunpyroll.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-18 14:10:55.086695 crunpyroll-2.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-18 14:10:43.000000 crunpyroll-2.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:27:52.247069 crunpyroll-2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-26 11:27:48.000000 crunpyroll-2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-26 11:27:52.247069 crunpyroll-2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-26 11:27:48.000000 crunpyroll-2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:27:52.239069 crunpyroll-2.4/crunpyroll/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:27:52.243069 crunpyroll-2.4/crunpyroll/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/enums/api_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/enums/content_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/enums/image_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:27:52.243069 crunpyroll-2.4/crunpyroll/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/methods/delete_active_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/methods/get_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/methods/get_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/methods/get_license.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/methods/get_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/methods/get_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/methods/get_old_streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/methods/get_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/methods/get_seasons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/methods/get_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/methods/get_streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/methods/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:27:52.247069 crunpyroll-2.4/crunpyroll/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/cms.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/drm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/episodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/hardsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/movies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/old_streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/seasons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/types/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-26 11:27:48.000000 crunpyroll-2.4/crunpyroll/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:27:52.247069 crunpyroll-2.4/crunpyroll.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-26 11:27:52.000000 crunpyroll-2.4/crunpyroll.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-26 11:27:52.000000 crunpyroll-2.4/crunpyroll.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:27:52.000000 crunpyroll-2.4/crunpyroll.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 11:27:52.000000 crunpyroll-2.4/crunpyroll.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 11:27:52.000000 crunpyroll-2.4/crunpyroll.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 11:27:52.247069 crunpyroll-2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-26 11:27:48.000000 crunpyroll-2.4/setup.py
```

### Comparing `crunpyroll-2.3.5/LICENSE` & `crunpyroll-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/PKG-INFO` & `crunpyroll-2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crunpyroll
-Version: 2.3.5
+Version: 2.4
 Summary: Async API wrapper for Crunchyroll
 Home-page: https://github.com/stefanodvx/crunpyroll
 Author: stefanodvx
 Author-email: pp.stefanodvx@gmail.com
 Project-URL: Tracker, https://github.com/stefanodvx/crunpyroll/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -99,14 +99,19 @@
     challenge=challenge,
     token=streams.token
 )
 cdm.parse_license(session_id, license)
 for key in cdm.get_keys(session_id, "CONTENT"):
     print(f"{key.kid.hex}:{key.key.hex()}")
 cdm.close(session_id)
+# Deleting active streams will prevent Crunchyroll HTTP 420 (too_many_queued_streams) error.
+await client.delete_active_stream(
+    streams.media_id,
+    token=streams.token
+)
 ```
 Output:
 ```bash
 056ec1ca849e350181753cacc9bd404b:2307a188ecd8de3859b71b30791f171d
 ```
 > [!TIP]
 > Decryption keys are universally applicable to both video and audio streams, maintaining consistency across all available formats.
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: crunpyroll Version: 2.3.5 Summary: Async API
-wrapper for Crunchyroll Home-page: https://github.com/stefanodvx/crunpyroll
-Author: stefanodvx Author-email: pp.stefanodvx@gmail.com Project-URL: Tracker,
-https://github.com/stefanodvx/crunpyroll/issues Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-httpx Requires-Dist: xmltodict
+Metadata-Version: 2.1 Name: crunpyroll Version: 2.4 Summary: Async API wrapper
+for Crunchyroll Home-page: https://github.com/stefanodvx/crunpyroll Author:
+stefanodvx Author-email: pp.stefanodvx@gmail.com Project-URL: Tracker, https://
+github.com/stefanodvx/crunpyroll/issues Requires-Python: >=3.7 Description-
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: httpx
+Requires-Dist: xmltodict
                                  _[_C_r_u_n_p_y_r_o_l_l_]
 --- #### Features ð¥ - Fully async ([httpx](https://www.python-httpx.org/)) -
 Python 3.7+ support - Clean and modern code - Updated to latest Crunchyroll API
 --- #### Installation âï¸ ```bash # Using Git pip install -U git+https://
 github.com/stefanodvx/crunpyroll # Using PyPi (Recommended) pip install -
 U crunpyroll ``` --- #### Documentation ð The documentation page undergoes
 automatic updates with each push. To access the latest documentation page,
@@ -39,16 +39,18 @@
 client.get_streams("GRVDQ1G4R") # Get manifest of the format you prefer
 manifest = await client.get_manifest(streams.hardsubs[0].url) # print(manifest)
 # Get Widevine PSSH from manifest pssh = PSSH
 (manifest.content_protection.widevine.pssh) session_id = cdm.open() challenge =
 cdm.get_license_challenge(session_id, pssh) license = await client.get_license
 ( streams.media_id, challenge=challenge, token=streams.token )
 cdm.parse_license(session_id, license) for key in cdm.get_keys(session_id,
-"CONTENT"): print(f"{key.kid.hex}:{key.key.hex()}") cdm.close(session_id) ```
-Output: ```bash 056ec1ca849e350181753cacc9bd404b:
-2307a188ecd8de3859b71b30791f171d ``` > [!TIP] > Decryption keys are universally
-applicable to both video and audio streams, maintaining consistency across all
-available formats. --- #### TODO List ð - [ ] Add support for token login -
-[ ] Add support for visitor view (authless) - [ ] Add support for Music - [ ]
-Add missing documentation - [ ] Add missing API methods - [ ] Add support for
-PlayReady DRM --- > Stay informed about the latest developments by joining our
-[Telegram Channel](https://t.me/crunpyroll).
+"CONTENT"): print(f"{key.kid.hex}:{key.key.hex()}") cdm.close(session_id) #
+Deleting active streams will prevent Crunchyroll HTTP 420
+(too_many_queued_streams) error. await client.delete_active_stream
+( streams.media_id, token=streams.token ) ``` Output: ```bash
+056ec1ca849e350181753cacc9bd404b:2307a188ecd8de3859b71b30791f171d ``` > [!TIP]
+> Decryption keys are universally applicable to both video and audio streams,
+maintaining consistency across all available formats. --- #### TODO List ð -
+[ ] Add support for token login - [ ] Add support for visitor view (authless) -
+[ ] Add support for Music - [ ] Add missing documentation - [ ] Add missing API
+methods - [ ] Add support for PlayReady DRM --- > Stay informed about the
+latest developments by joining our [Telegram Channel](https://t.me/crunpyroll).
```

### Comparing `crunpyroll-2.3.5/README.md` & `crunpyroll-2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,19 @@
     challenge=challenge,
     token=streams.token
 )
 cdm.parse_license(session_id, license)
 for key in cdm.get_keys(session_id, "CONTENT"):
     print(f"{key.kid.hex}:{key.key.hex()}")
 cdm.close(session_id)
+# Deleting active streams will prevent Crunchyroll HTTP 420 (too_many_queued_streams) error.
+await client.delete_active_stream(
+    streams.media_id,
+    token=streams.token
+)
 ```
 Output:
 ```bash
 056ec1ca849e350181753cacc9bd404b:2307a188ecd8de3859b71b30791f171d
 ```
 > [!TIP]
 > Decryption keys are universally applicable to both video and audio streams, maintaining consistency across all available formats.
```

#### html2text {}

```diff
@@ -33,16 +33,18 @@
 client.get_streams("GRVDQ1G4R") # Get manifest of the format you prefer
 manifest = await client.get_manifest(streams.hardsubs[0].url) # print(manifest)
 # Get Widevine PSSH from manifest pssh = PSSH
 (manifest.content_protection.widevine.pssh) session_id = cdm.open() challenge =
 cdm.get_license_challenge(session_id, pssh) license = await client.get_license
 ( streams.media_id, challenge=challenge, token=streams.token )
 cdm.parse_license(session_id, license) for key in cdm.get_keys(session_id,
-"CONTENT"): print(f"{key.kid.hex}:{key.key.hex()}") cdm.close(session_id) ```
-Output: ```bash 056ec1ca849e350181753cacc9bd404b:
-2307a188ecd8de3859b71b30791f171d ``` > [!TIP] > Decryption keys are universally
-applicable to both video and audio streams, maintaining consistency across all
-available formats. --- #### TODO List ð - [ ] Add support for token login -
-[ ] Add support for visitor view (authless) - [ ] Add support for Music - [ ]
-Add missing documentation - [ ] Add missing API methods - [ ] Add support for
-PlayReady DRM --- > Stay informed about the latest developments by joining our
-[Telegram Channel](https://t.me/crunpyroll).
+"CONTENT"): print(f"{key.kid.hex}:{key.key.hex()}") cdm.close(session_id) #
+Deleting active streams will prevent Crunchyroll HTTP 420
+(too_many_queued_streams) error. await client.delete_active_stream
+( streams.media_id, token=streams.token ) ``` Output: ```bash
+056ec1ca849e350181753cacc9bd404b:2307a188ecd8de3859b71b30791f171d ``` > [!TIP]
+> Decryption keys are universally applicable to both video and audio streams,
+maintaining consistency across all available formats. --- #### TODO List ð -
+[ ] Add support for token login - [ ] Add support for visitor view (authless) -
+[ ] Add support for Music - [ ] Add missing documentation - [ ] Add missing API
+methods - [ ] Add support for PlayReady DRM --- > Stay informed about the
+latest developments by joining our [Telegram Channel](https://t.me/crunpyroll).
```

### Comparing `crunpyroll-2.3.5/crunpyroll/client.py` & `crunpyroll-2.4/crunpyroll/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 from .methods import Methods
-from .utils import get_api_headers
+from .utils import (
+    get_api_headers,
+    DEVICE_ID,
+    DEVICE_NAME,
+    DEVICE_TYPE
+)
 
 from .session import Session
 from .errors import CrunpyrollException
 from .enums import APIHost
 from .types.obj import Object
 
 from typing import (
@@ -18,53 +23,77 @@
     """Initialize Crunchyroll Client
     
     Parameters:
         email (``str``):
             Email or username of the account.
         password (``str``):
             Password of the account.
+        preferred_audio_language (``str``, *optional*):
+            The audio language to use in Crunchyroll.
+            Default to 'ja-JP'
         locale (``str``, *optional*):
             The language to use in Crunchyroll.
             Default to 'en-US'
+        device_id (``str``, *optional*):
+            The device identifier to use, in string form, e.g. '01234567-89AB-CDEF-0123-456789ABCDEF' where the 32 hexadecimal digits represent the UUID.
+            Default to a random UUID
+        device_name (``str``, *optional*):
+            The device name to use (Crunchyroll app uses [About phone → Device name] field).
+        device_type (``str``, *optional*):
+            The device type to use (Crunchyroll app uses Manufacturer + Model).
         proxies (``str`` | ``dict``, *optional*):
             Proxies for HTTP requests.
             Default to None
     """
     def __init__(
         self,
         *,
         email: str,
         password: str,
+        preferred_audio_language: str = "ja-JP",
         locale: str = "en-US",
+        device_id: str = DEVICE_ID,
+        device_name: str = DEVICE_NAME,
+        device_type: str = DEVICE_TYPE,
         proxies: Union[Dict, str] = None
     ) -> None:
         self.email: str = email
         self.password: str = password
+        self.preferred_audio_language: str = preferred_audio_language
         self.locale: str = locale
+        self.device_id: str = device_id
+        self.device_name: str = device_name
+        self.device_type: str = device_type
 
         self.http = httpx.AsyncClient(proxies=proxies, timeout=15)
         self.session = Session(self)
 
     async def start(self):
         if self.session.is_authorized:
             raise CrunpyrollException("Client is already authorized and started.")
         return await self.session.authorize()
 
     @staticmethod
-    def parse_response(response: httpx.Response) -> Optional[Union[Dict, str]]:
+    def parse_response(
+        response: httpx.Response,
+        *,
+        method: str = "GET",
+    ) -> Optional[Union[Dict, str]]:
         status_code = response.status_code
         text_content = response.text
         message = f"[{status_code}] {text_content}"
         try:
             content = response.json()
         except json.JSONDecodeError:
             content = response.text
-        if status_code != 200:
-            raise CrunpyrollException(message)
-        return content
+        if status_code == 200:
+            return content
+        if status_code == 204 and method in {"PUT", "DELETE"}:
+            return content
+        raise CrunpyrollException(message)
 
     async def api_request(
         self,
         method: str,
         endpoint: str,
         host: APIHost = APIHost.BETA,
         url: str = None,
@@ -83,15 +112,15 @@
         response = await self.http.request(
             method=method,
             url=url,
             params=params,
             headers=api_headers,
             data=payload
         )
-        return Client.parse_response(response)
+        return Client.parse_response(response, method=method)
     
     async def manifest_request(
         self,
         url: str,
         headers: Dict = None,
     ) -> str:
         api_headers = get_api_headers(headers)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crunpyroll-2.3.5/crunpyroll/methods/__init__.py` & `crunpyroll-2.4/crunpyroll/methods/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from .search import Search
 from .get_index import GetIndex
 from .get_profile import GetProfile
 from .get_series import GetSeries
 from .get_seasons import GetSeasons
 from .get_episodes import GetEpisodes
+from .get_objects import GetObjects
 from .get_streams import GetStreams
 from .get_manifest import GetManifest
 from .get_license import GetLicense
 from .get_old_streams import GetOldStreams
+from .delete_active_stream import DeleteActiveStream
 
 class Methods(
     Search,
     GetIndex,
     GetProfile,
     GetSeries,
     GetSeasons,
     GetEpisodes,
     GetStreams,
     GetManifest,
     GetLicense,
-    GetOldStreams
+    GetOldStreams,
+    GetObjects,
+    DeleteActiveStream
 ):
     pass
```

### Comparing `crunpyroll-2.3.5/crunpyroll/methods/get_episodes.py` & `crunpyroll-2.4/crunpyroll/methods/get_episodes.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/methods/get_index.py` & `crunpyroll-2.4/crunpyroll/methods/get_index.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from crunpyroll import types
 
 import crunpyroll
 
 class GetIndex:
     async def get_index(
         self: "crunpyroll.Client",
-    ) -> "types.Index":
+    ) -> "types.SessionIndex":
         """
         Get session index. It's unlikely that you would use this method.
 
         Returns:
             :obj:`~crunpyroll.types.SessionIndex`:
                 On success, informations about session index are returned.
         """
```

### Comparing `crunpyroll-2.3.5/crunpyroll/methods/get_license.py` & `crunpyroll-2.4/crunpyroll/methods/get_license.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/methods/get_manifest.py` & `crunpyroll-2.4/crunpyroll/methods/get_manifest.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/methods/get_old_streams.py` & `crunpyroll-2.4/crunpyroll/methods/get_old_streams.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/methods/get_profile.py` & `crunpyroll-2.4/crunpyroll/methods/get_profile.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/methods/get_seasons.py` & `crunpyroll-2.4/crunpyroll/methods/get_series.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from crunpyroll import types
 
 import crunpyroll
 
-class GetSeasons:
-    async def get_seasons(
+class GetSeries:
+    async def get_series(
         self: "crunpyroll.Client",
         series_id: str,
         *,
         locale: str = None,
-    ) -> "types.SeasonsQuery":
+    ) -> "types.Series":
         """
-        Get list of seasons from a series.
+        Get informations about a series.
 
         Parameters:
             series_id (``str``):
                 Unique identifier of the series.
             locale (``str``, *optional*):
                 Localize request for different results.
                 Default to the one used in Client.
-                
+
         Returns:
-            :obj:`~crunpyroll.types.SeasonsQuery`:
-                On success, query of seasons is returned.
+            :obj:`~crunpyroll.types.Series`:
+                On success, series object is returned.
         """
         await self.session.retrieve()
         response = await self.api_request(
             method="GET",
-            endpoint="content/v2/cms/series/" + series_id + "/seasons",
+            endpoint="content/v2/cms/series/" + series_id,
             params={
                 "locale": locale or self.locale
             }
         )
-        return types.SeasonsQuery.parse(response)
+        return types.Series.parse(response)
```

### Comparing `crunpyroll-2.3.5/crunpyroll/methods/get_series.py` & `crunpyroll-2.4/crunpyroll/methods/get_seasons.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from crunpyroll import types
 
 import crunpyroll
 
-class GetSeries:
-    async def get_series(
+class GetSeasons:
+    async def get_seasons(
         self: "crunpyroll.Client",
         series_id: str,
         *,
+        preferred_audio_language: str = None,
         locale: str = None,
-    ) -> "types.Series":
+    ) -> "types.SeasonsQuery":
         """
-        Get informations about a series.
+        Get list of seasons from a series.
 
         Parameters:
             series_id (``str``):
                 Unique identifier of the series.
             locale (``str``, *optional*):
                 Localize request for different results.
                 Default to the one used in Client.
-
+            preferred_audio_language (``str``, *optional*):
+                Audio language request for different results.
+                Default to the one used in Client.
+                
         Returns:
-            :obj:`~crunpyroll.types.Series`:
-                On success, series object is returned.
+            :obj:`~crunpyroll.types.SeasonsQuery`:
+                On success, query of seasons is returned.
         """
         await self.session.retrieve()
         response = await self.api_request(
             method="GET",
-            endpoint="content/v2/cms/series/" + series_id,
+            endpoint="content/v2/cms/series/" + series_id + "/seasons",
             params={
+                "preferred_audio_language": preferred_audio_language or self.preferred_audio_language,
                 "locale": locale or self.locale
             }
         )
-        return types.Series.parse(response)
+        return types.SeasonsQuery.parse(response)
```

### Comparing `crunpyroll-2.3.5/crunpyroll/methods/get_streams.py` & `crunpyroll-2.4/crunpyroll/methods/get_streams.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/methods/search.py` & `crunpyroll-2.4/crunpyroll/methods/search.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/session.py` & `crunpyroll-2.4/crunpyroll/session.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from datetime import datetime, timedelta
 
 from .utils import (
     get_date,
-    PUBLIC_TOKEN,
-    DEVICE_NAME,
-    DEVICE_TYPE,
-    DEVICE_ID
+    PUBLIC_TOKEN
 )
 
 from .errors import ClientNotAuthorized
 
 from typing import Optional
 
 import crunpyroll
@@ -48,17 +45,17 @@
                 "Authorization": f"Basic {PUBLIC_TOKEN}"
             },
             payload={
                 "username": self._client.email,
                 "password": self._client.password,
                 "grant_type": "password",
                 "scope": "offline_access",
-                "device_id": DEVICE_ID,
-                "device_name": DEVICE_NAME,
-                "device_type": DEVICE_TYPE
+                "device_id": self._client.device_id,
+                "device_name": self._client.device_name,
+                "device_type": self._client.device_type
             }, include_session=False
         )
         self.access_token = response.get("access_token")
         self.refresh_token = response.get("refresh_token")
         self.expiration = get_date() + timedelta(
             seconds=response.get("expires_in")
         )
@@ -71,17 +68,17 @@
             headers={
                 "Authorization": f"Basic {PUBLIC_TOKEN}"
             },
             payload={
                 "refresh_token": self.refresh_token,
                 "grant_type": "refresh_token",
                 "scope": "offline_access",
-                "device_id": DEVICE_ID,
-                "device_name": DEVICE_NAME,
-                "device_type": DEVICE_TYPE
+                "device_id": self._client.device_id,
+                "device_name": self._client.device_name,
+                "device_type": self._client.device_type
             }, include_session=False
         )
         self.access_token = response.get("access_token")
         self.refresh_token = response.get("refresh_token")
         self.expiration = get_date() + timedelta(
             seconds=response.get("expires_in")
         )
```

### Comparing `crunpyroll-2.3.5/crunpyroll/types/__init__.py` & `crunpyroll-2.4/crunpyroll/types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,10 +7,12 @@
 from .cms import CMS
 from .index import SessionIndex
 from .profile import Profile
 from .content import Content
 from .streams import MediaStreams
 from .subtitles import SubtitlesStream
 from .hardsub import HardsubStream
+from .objects import ObjectsQuery
 from .old_streams import OldMediaStreams
+from .index import SessionIndex
 from .manifest import Manifest, ManifestVideoStream, ManifestAudioStream
 from .drm import DRM, ContentProtection
```

### Comparing `crunpyroll-2.3.5/crunpyroll/types/cms.py` & `crunpyroll-2.4/crunpyroll/types/cms.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/types/drm.py` & `crunpyroll-2.4/crunpyroll/types/drm.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/types/episodes.py` & `crunpyroll-2.4/crunpyroll/types/episodes.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/types/hardsub.py` & `crunpyroll-2.4/crunpyroll/types/hardsub.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/types/images.py` & `crunpyroll-2.4/crunpyroll/types/images.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/types/manifest.py` & `crunpyroll-2.4/crunpyroll/types/manifest.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/types/movies.py` & `crunpyroll-2.4/crunpyroll/types/movies.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/types/obj.py` & `crunpyroll-2.4/crunpyroll/types/obj.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/types/old_streams.py` & `crunpyroll-2.4/crunpyroll/types/old_streams.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/types/profile.py` & `crunpyroll-2.4/crunpyroll/types/profile.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/types/search.py` & `crunpyroll-2.4/crunpyroll/types/search.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/types/seasons.py` & `crunpyroll-2.4/crunpyroll/types/seasons.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/types/series.py` & `crunpyroll-2.4/crunpyroll/types/series.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/types/streams.py` & `crunpyroll-2.4/crunpyroll/types/streams.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/types/subtitles.py` & `crunpyroll-2.4/crunpyroll/types/subtitles.py`

 * *Files identical despite different names*

### Comparing `crunpyroll-2.3.5/crunpyroll/utils.py` & `crunpyroll-2.4/crunpyroll/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from typing import Optional, List, Dict
 from datetime import datetime
 from uuid import uuid4
 
-PUBLIC_TOKEN = "b2VkYXJteHN0bGgxanZhd2ltbnE6OWxFaHZIWkpEMzJqdVY1ZFc5Vk9TNTdkb3BkSnBnbzE="
+PUBLIC_TOKEN = "bm12anNoZmtueW14eGtnN2ZiaDk6WllJVnJCV1VQYmNYRHRiRDIyVlNMYTZiNFdRb3Mzelg="
+
+APP_VERSION = "3.54.0"
 
 DEVICE_NAME = "RMX2170"
 DEVICE_TYPE = "realme RMX2170"
 DEVICE_ID = str(uuid4())
 
 WIDEVINE_UUID = "urn:uuid:edef8ba9-79d6-4ace-a3c8-27dcd51d21ed"
 PLAYREADY_UUID = "urn:uuid:9a04f079-9840-4286-ab92-e65be0885f95"
 
-
 def get_api_headers(headers: Optional[Dict]) -> Dict:
     return {
         "Connection": "Keep-Alive",
         "Content-Type": "application/x-www-form-urlencoded",
-        "User-Agent": "Crunchyroll/3.46.2 Android/13 okhttp/4.12.0"
+        "User-Agent": f"Crunchyroll/{APP_VERSION} Android/13 okhttp/4.12.0"
     } | (headers or {})
 
 def parse_segments(repr: Dict, template: Dict) -> List[str]:
     time = 0
     segments = []
     base_url = repr["BaseURL"]
     representation_id = repr["@id"]
@@ -31,15 +32,15 @@
     )
     segments.append(initialization_url)
     for segment in template["SegmentTimeline"]["S"]:
         repeat = int(segment.get("@r", 0)) + 1
         duration = int(segment.get("@d"))
         time += repeat * duration
         for _ in range(repeat):
-            number = start_number + len(segments)
+            number = start_number + len(segments) - 1
             segment_url = format_segment_url(
                 url=base_url + template["@media"],
                 obj={
                     "Number": str(number),
                     "RepresentationID": representation_id
                 }
             )
```

### Comparing `crunpyroll-2.3.5/crunpyroll.egg-info/PKG-INFO` & `crunpyroll-2.4/crunpyroll.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crunpyroll
-Version: 2.3.5
+Version: 2.4
 Summary: Async API wrapper for Crunchyroll
 Home-page: https://github.com/stefanodvx/crunpyroll
 Author: stefanodvx
 Author-email: pp.stefanodvx@gmail.com
 Project-URL: Tracker, https://github.com/stefanodvx/crunpyroll/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -99,14 +99,19 @@
     challenge=challenge,
     token=streams.token
 )
 cdm.parse_license(session_id, license)
 for key in cdm.get_keys(session_id, "CONTENT"):
     print(f"{key.kid.hex}:{key.key.hex()}")
 cdm.close(session_id)
+# Deleting active streams will prevent Crunchyroll HTTP 420 (too_many_queued_streams) error.
+await client.delete_active_stream(
+    streams.media_id,
+    token=streams.token
+)
 ```
 Output:
 ```bash
 056ec1ca849e350181753cacc9bd404b:2307a188ecd8de3859b71b30791f171d
 ```
 > [!TIP]
 > Decryption keys are universally applicable to both video and audio streams, maintaining consistency across all available formats.
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: crunpyroll Version: 2.3.5 Summary: Async API
-wrapper for Crunchyroll Home-page: https://github.com/stefanodvx/crunpyroll
-Author: stefanodvx Author-email: pp.stefanodvx@gmail.com Project-URL: Tracker,
-https://github.com/stefanodvx/crunpyroll/issues Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-httpx Requires-Dist: xmltodict
+Metadata-Version: 2.1 Name: crunpyroll Version: 2.4 Summary: Async API wrapper
+for Crunchyroll Home-page: https://github.com/stefanodvx/crunpyroll Author:
+stefanodvx Author-email: pp.stefanodvx@gmail.com Project-URL: Tracker, https://
+github.com/stefanodvx/crunpyroll/issues Requires-Python: >=3.7 Description-
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: httpx
+Requires-Dist: xmltodict
                                  _[_C_r_u_n_p_y_r_o_l_l_]
 --- #### Features ð¥ - Fully async ([httpx](https://www.python-httpx.org/)) -
 Python 3.7+ support - Clean and modern code - Updated to latest Crunchyroll API
 --- #### Installation âï¸ ```bash # Using Git pip install -U git+https://
 github.com/stefanodvx/crunpyroll # Using PyPi (Recommended) pip install -
 U crunpyroll ``` --- #### Documentation ð The documentation page undergoes
 automatic updates with each push. To access the latest documentation page,
@@ -39,16 +39,18 @@
 client.get_streams("GRVDQ1G4R") # Get manifest of the format you prefer
 manifest = await client.get_manifest(streams.hardsubs[0].url) # print(manifest)
 # Get Widevine PSSH from manifest pssh = PSSH
 (manifest.content_protection.widevine.pssh) session_id = cdm.open() challenge =
 cdm.get_license_challenge(session_id, pssh) license = await client.get_license
 ( streams.media_id, challenge=challenge, token=streams.token )
 cdm.parse_license(session_id, license) for key in cdm.get_keys(session_id,
-"CONTENT"): print(f"{key.kid.hex}:{key.key.hex()}") cdm.close(session_id) ```
-Output: ```bash 056ec1ca849e350181753cacc9bd404b:
-2307a188ecd8de3859b71b30791f171d ``` > [!TIP] > Decryption keys are universally
-applicable to both video and audio streams, maintaining consistency across all
-available formats. --- #### TODO List ð - [ ] Add support for token login -
-[ ] Add support for visitor view (authless) - [ ] Add support for Music - [ ]
-Add missing documentation - [ ] Add missing API methods - [ ] Add support for
-PlayReady DRM --- > Stay informed about the latest developments by joining our
-[Telegram Channel](https://t.me/crunpyroll).
+"CONTENT"): print(f"{key.kid.hex}:{key.key.hex()}") cdm.close(session_id) #
+Deleting active streams will prevent Crunchyroll HTTP 420
+(too_many_queued_streams) error. await client.delete_active_stream
+( streams.media_id, token=streams.token ) ``` Output: ```bash
+056ec1ca849e350181753cacc9bd404b:2307a188ecd8de3859b71b30791f171d ``` > [!TIP]
+> Decryption keys are universally applicable to both video and audio streams,
+maintaining consistency across all available formats. --- #### TODO List ð -
+[ ] Add support for token login - [ ] Add support for visitor view (authless) -
+[ ] Add support for Music - [ ] Add missing documentation - [ ] Add missing API
+methods - [ ] Add support for PlayReady DRM --- > Stay informed about the
+latest developments by joining our [Telegram Channel](https://t.me/crunpyroll).
```

### Comparing `crunpyroll-2.3.5/crunpyroll.egg-info/SOURCES.txt` & `crunpyroll-2.4/crunpyroll.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 crunpyroll.egg-info/requires.txt
 crunpyroll.egg-info/top_level.txt
 crunpyroll/enums/__init__.py
 crunpyroll/enums/api_host.py
 crunpyroll/enums/content_type.py
 crunpyroll/enums/image_type.py
 crunpyroll/methods/__init__.py
+crunpyroll/methods/delete_active_stream.py
 crunpyroll/methods/get_episodes.py
 crunpyroll/methods/get_index.py
 crunpyroll/methods/get_license.py
 crunpyroll/methods/get_manifest.py
+crunpyroll/methods/get_objects.py
 crunpyroll/methods/get_old_streams.py
 crunpyroll/methods/get_profile.py
 crunpyroll/methods/get_seasons.py
 crunpyroll/methods/get_series.py
 crunpyroll/methods/get_streams.py
 crunpyroll/methods/search.py
 crunpyroll/types/__init__.py
@@ -33,14 +35,15 @@
 crunpyroll/types/episodes.py
 crunpyroll/types/hardsub.py
 crunpyroll/types/images.py
 crunpyroll/types/index.py
 crunpyroll/types/manifest.py
 crunpyroll/types/movies.py
 crunpyroll/types/obj.py
+crunpyroll/types/objects.py
 crunpyroll/types/old_streams.py
 crunpyroll/types/profile.py
 crunpyroll/types/search.py
 crunpyroll/types/seasons.py
 crunpyroll/types/series.py
 crunpyroll/types/streams.py
 crunpyroll/types/subtitles.py
```

### Comparing `crunpyroll-2.3.5/setup.py` & `crunpyroll-2.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="crunpyroll",
-    version="2.3.5",
+    version="2.4",
     author="stefanodvx",
     author_email="pp.stefanodvx@gmail.com",
     description="Async API wrapper for Crunchyroll",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/stefanodvx/crunpyroll",
     project_urls={
```

