# Comparing `tmp/runes-client-0.9.3.tar.gz` & `tmp/runes-client-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runes-client-0.9.3.tar", last modified: Thu Apr 25 05:06:04 2024, max compression
+gzip compressed data, was "runes-client-0.9.4.tar", last modified: Fri Apr 26 15:54:55 2024, max compression
```

## Comparing `runes-client-0.9.3.tar` & `runes-client-0.9.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-25 05:06:04.382776 runes-client-0.9.3/
--rw-r--r--   0 stevehiehn   (501) staff       (20)    35140 2024-03-13 21:22:47.000000 runes-client-0.9.3/LICENSE.md
--rw-r--r--   0 stevehiehn   (501) staff       (20)     7974 2024-04-25 05:06:04.382551 runes-client-0.9.3/PKG-INFO
--rw-r--r--   0 stevehiehn   (501) staff       (20)     7426 2024-04-18 17:41:49.000000 runes-client-0.9.3/README.md
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-25 05:06:04.378862 runes-client-0.9.3/runes_client/
--rw-r--r--   0 stevehiehn   (501) staff       (20)      677 2024-04-25 04:38:12.000000 runes-client-0.9.3/runes_client/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    10445 2024-04-25 04:30:29.000000 runes-client-0.9.3/runes_client/api_client.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1193 2024-04-12 01:39:49.000000 runes-client-0.9.3/runes_client/config.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    39212 2024-04-25 05:02:57.000000 runes-client-0.9.3/runes_client/core.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      277 2024-03-13 21:22:47.000000 runes-client-0.9.3/runes_client/decorators.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     4446 2024-03-13 21:22:47.000000 runes-client-0.9.3/runes_client/dn_tracer.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1404 2024-03-13 21:22:47.000000 runes-client-0.9.3/runes_client/file_uploader.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-25 05:06:04.380318 runes-client-0.9.3/runes_client/output/
--rw-r--r--   0 stevehiehn   (501) staff       (20)       63 2024-03-13 21:22:47.000000 runes-client-0.9.3/runes_client/output/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6956 2024-04-25 00:34:32.000000 runes-client-0.9.3/runes_client/output/results_handler.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-25 05:06:04.380994 runes-client-0.9.3/runes_client/utils/
--rw-r--r--   0 stevehiehn   (501) staff       (20)       61 2024-03-13 21:22:47.000000 runes-client-0.9.3/runes_client/utils/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     3060 2024-03-13 21:22:47.000000 runes-client-0.9.3/runes_client/utils/audio_utils.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      654 2024-04-25 00:34:47.000000 runes-client-0.9.3/runes_client/utils/file_type_classifier.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-25 05:06:04.382320 runes-client-0.9.3/runes_client.egg-info/
--rw-r--r--   0 stevehiehn   (501) staff       (20)     7974 2024-04-25 05:06:04.000000 runes-client-0.9.3/runes_client.egg-info/PKG-INFO
--rw-r--r--   0 stevehiehn   (501) staff       (20)      725 2024-04-25 05:06:04.000000 runes-client-0.9.3/runes_client.egg-info/SOURCES.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)        1 2024-04-25 05:06:04.000000 runes-client-0.9.3/runes_client.egg-info/dependency_links.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       56 2024-04-25 05:06:04.000000 runes-client-0.9.3/runes_client.egg-info/entry_points.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       72 2024-04-25 05:06:04.000000 runes-client-0.9.3/runes_client.egg-info/requires.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       19 2024-04-25 05:06:04.000000 runes-client-0.9.3/runes_client.egg-info/top_level.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       38 2024-04-25 05:06:04.382815 runes-client-0.9.3/setup.cfg
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1565 2024-04-25 05:03:33.000000 runes-client-0.9.3/setup.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-25 05:06:04.382109 runes-client-0.9.3/tests/
--rw-r--r--   0 stevehiehn   (501) staff       (20)        0 2024-03-13 21:22:47.000000 runes-client-0.9.3/tests/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     5372 2024-03-13 21:50:56.000000 runes-client-0.9.3/tests/test_audio_utils.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6956 2024-03-13 21:50:43.000000 runes-client-0.9.3/tests/test_core.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    13164 2024-04-09 00:18:41.000000 runes-client-0.9.3/tests/test_registration.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      683 2024-03-13 21:50:56.000000 runes-client-0.9.3/tests/test_results_handler.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-26 15:54:55.884822 runes-client-0.9.4/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    35140 2024-03-13 21:22:47.000000 runes-client-0.9.4/LICENSE.md
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     7974 2024-04-26 15:54:55.884606 runes-client-0.9.4/PKG-INFO
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     7426 2024-04-18 17:41:49.000000 runes-client-0.9.4/README.md
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-26 15:54:55.880889 runes-client-0.9.4/runes_client/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      677 2024-04-25 04:38:12.000000 runes-client-0.9.4/runes_client/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    10445 2024-04-25 04:30:29.000000 runes-client-0.9.4/runes_client/api_client.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1193 2024-04-12 01:39:49.000000 runes-client-0.9.4/runes_client/config.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    39212 2024-04-25 05:02:57.000000 runes-client-0.9.4/runes_client/core.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      277 2024-03-13 21:22:47.000000 runes-client-0.9.4/runes_client/decorators.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     4446 2024-03-13 21:22:47.000000 runes-client-0.9.4/runes_client/dn_tracer.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1404 2024-03-13 21:22:47.000000 runes-client-0.9.4/runes_client/file_uploader.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-26 15:54:55.882355 runes-client-0.9.4/runes_client/output/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       63 2024-03-13 21:22:47.000000 runes-client-0.9.4/runes_client/output/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     8228 2024-04-26 15:34:31.000000 runes-client-0.9.4/runes_client/output/results_handler.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-26 15:54:55.883068 runes-client-0.9.4/runes_client/utils/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       61 2024-03-13 21:22:47.000000 runes-client-0.9.4/runes_client/utils/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     3060 2024-03-13 21:22:47.000000 runes-client-0.9.4/runes_client/utils/audio_utils.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      654 2024-04-25 00:34:47.000000 runes-client-0.9.4/runes_client/utils/file_type_classifier.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-26 15:54:55.884395 runes-client-0.9.4/runes_client.egg-info/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     7974 2024-04-26 15:54:55.000000 runes-client-0.9.4/runes_client.egg-info/PKG-INFO
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      725 2024-04-26 15:54:55.000000 runes-client-0.9.4/runes_client.egg-info/SOURCES.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)        1 2024-04-26 15:54:55.000000 runes-client-0.9.4/runes_client.egg-info/dependency_links.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       56 2024-04-26 15:54:55.000000 runes-client-0.9.4/runes_client.egg-info/entry_points.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       72 2024-04-26 15:54:55.000000 runes-client-0.9.4/runes_client.egg-info/requires.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       19 2024-04-26 15:54:55.000000 runes-client-0.9.4/runes_client.egg-info/top_level.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       38 2024-04-26 15:54:55.884864 runes-client-0.9.4/setup.cfg
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1565 2024-04-26 15:36:36.000000 runes-client-0.9.4/setup.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-26 15:54:55.884179 runes-client-0.9.4/tests/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)        0 2024-03-13 21:22:47.000000 runes-client-0.9.4/tests/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     5372 2024-03-13 21:50:56.000000 runes-client-0.9.4/tests/test_audio_utils.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6956 2024-03-13 21:50:43.000000 runes-client-0.9.4/tests/test_core.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    13164 2024-04-09 00:18:41.000000 runes-client-0.9.4/tests/test_registration.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      683 2024-03-13 21:50:56.000000 runes-client-0.9.4/tests/test_results_handler.py
```

### Comparing `runes-client-0.9.3/LICENSE.md` & `runes-client-0.9.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.3/PKG-INFO` & `runes-client-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runes-client
-Version: 0.9.3
+Version: 0.9.4
 Summary: Runes client enables remote execution of python code triggered from a Crucible Plugin on the Signals & Sorcery platform.
 Home-page: https://signalsandsorcery.app
 Author: Steve Hiehn
 Author-email: stevehiehn@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `runes-client-0.9.3/README.md` & `runes-client-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.3/runes_client/__init__.py` & `runes-client-0.9.4/runes_client/__init__.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.3/runes_client/api_client.py` & `runes-client-0.9.4/runes_client/api_client.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.3/runes_client/config.py` & `runes-client-0.9.4/runes_client/config.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.3/runes_client/core.py` & `runes-client-0.9.4/runes_client/core.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.3/runes_client/dn_tracer.py` & `runes-client-0.9.4/runes_client/dn_tracer.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.3/runes_client/file_uploader.py` & `runes-client-0.9.4/runes_client/file_uploader.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.3/runes_client/output/results_handler.py` & `runes-client-0.9.4/runes_client/output/results_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Existing imports...
 import json
 import os
 import subprocess
+from urllib.parse import urlparse, urlsplit
 
 from ..api_client import APIClient
 from ..config import API_BASE_URL
 from ..dn_tracer import SentryEventLogger, DNSystemType, DNMsgStage, DNTag
 from ..file_uploader import FileUploader
 from ..utils.audio_utils import process_audio_file
 from ..utils.file_type_classifier import FileTypeClassifier
@@ -61,14 +62,56 @@
     async def add_error(self, error):
         self.errors.append(error)
         return True
 
     def set_message_id(self, message_id):
         self.message_id = message_id
 
+    async def add_file_url(self, file_url: str, file_type: str):
+        # List of supported file types
+        supported_file_types = [
+            "audio",
+            "midi",
+            "text",
+            "video",
+            "image",
+        ]
+
+        # Check if the file type is supported
+        if file_type.lower() not in supported_file_types:
+            await self.add_error(f"File type {file_type} is not supported.")
+            return False
+
+        # Validate URL
+        try:
+            parsed_url = urlparse(file_url)
+            if not (parsed_url.scheme and parsed_url.netloc):
+                raise ValueError("Invalid URL")
+        except Exception as e:
+            await self.add_error(f"Invalid file URL: {e}")
+            return False
+
+        # Extract base name from URL
+        file_name = os.path.basename(parsed_url.path)
+
+        # If the extracted base name is empty or invalid, set a default name
+        if not file_name:
+            file_name = "default_filename"
+
+        # Add the file to the list
+        self.files.append(
+            {
+                "name": file_name,
+                "url": file_url,
+                "type": file_type,
+            }
+        )
+
+        return True
+
     async def add_file(self, file_path):
         classifier = FileTypeClassifier()
         input_type = classifier.classify(file_path)
 
         if input_type == "audio":
             if not self.ffmpeg_installed:
                 error_message = (
```

### Comparing `runes-client-0.9.3/runes_client/utils/audio_utils.py` & `runes-client-0.9.4/runes_client/utils/audio_utils.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.3/runes_client/utils/file_type_classifier.py` & `runes-client-0.9.4/runes_client/utils/file_type_classifier.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.3/runes_client.egg-info/PKG-INFO` & `runes-client-0.9.4/runes_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runes-client
-Version: 0.9.3
+Version: 0.9.4
 Summary: Runes client enables remote execution of python code triggered from a Crucible Plugin on the Signals & Sorcery platform.
 Home-page: https://signalsandsorcery.app
 Author: Steve Hiehn
 Author-email: stevehiehn@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `runes-client-0.9.3/runes_client.egg-info/SOURCES.txt` & `runes-client-0.9.4/runes_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.3/setup.py` & `runes-client-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 if not is_ffmpeg_installed():
     print(ffmpeg_warning_msg)
 
 setup(
     name="runes-client",
-    version="0.9.3",
+    version="0.9.4",
     packages=find_packages(),
     install_requires=[
         "aiohttp",
         "websockets",
         "nest-asyncio",
         "sentry-sdk",
         "pydub",
```

### Comparing `runes-client-0.9.3/tests/test_audio_utils.py` & `runes-client-0.9.4/tests/test_audio_utils.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.3/tests/test_core.py` & `runes-client-0.9.4/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.3/tests/test_registration.py` & `runes-client-0.9.4/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.3/tests/test_results_handler.py` & `runes-client-0.9.4/tests/test_results_handler.py`

 * *Files identical despite different names*

