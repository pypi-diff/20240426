# Comparing `tmp/ovos-tts-server-0.0.3a8.tar.gz` & `tmp/ovos-tts-server-0.0.3a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-tts-server-0.0.3a8.tar", last modified: Thu Jun 22 16:03:24 2023, max compression
+gzip compressed data, was "ovos-tts-server-0.0.3a9.tar", last modified: Sat Oct 14 21:20:34 2023, max compression
```

## Comparing `ovos-tts-server-0.0.3a8.tar` & `ovos-tts-server-0.0.3a9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:03:24.666341 ovos-tts-server-0.0.3a8/
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-22 16:03:24.000000 ovos-tts-server-0.0.3a8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-22 16:03:24.662341 ovos-tts-server-0.0.3a8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:03:24.662341 ovos-tts-server-0.0.3a8/ovos_tts_server/
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-22 16:03:24.000000 ovos-tts-server-0.0.3a8/ovos_tts_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-22 16:03:24.000000 ovos-tts-server-0.0.3a8/ovos_tts_server/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:03:24.662341 ovos-tts-server-0.0.3a8/ovos_tts_server/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-06-22 16:03:24.000000 ovos-tts-server-0.0.3a8/ovos_tts_server/examples/rainbow.json
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-22 16:03:24.000000 ovos-tts-server-0.0.3a8/ovos_tts_server/gradio_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-22 16:03:24.000000 ovos-tts-server-0.0.3a8/ovos_tts_server/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:03:24.662341 ovos-tts-server-0.0.3a8/ovos_tts_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-22 16:03:24.000000 ovos-tts-server-0.0.3a8/ovos_tts_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-22 16:03:24.000000 ovos-tts-server-0.0.3a8/ovos_tts_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:03:24.000000 ovos-tts-server-0.0.3a8/ovos_tts_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-22 16:03:24.000000 ovos-tts-server-0.0.3a8/ovos_tts_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-22 16:03:24.000000 ovos-tts-server-0.0.3a8/ovos_tts_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 16:03:24.000000 ovos-tts-server-0.0.3a8/ovos_tts_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:03:24.000000 ovos-tts-server-0.0.3a8/ovos_tts_server.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 16:03:24.666341 ovos-tts-server-0.0.3a8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3054 2023-06-22 16:03:24.000000 ovos-tts-server-0.0.3a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 21:20:34.841049 ovos-tts-server-0.0.3a9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2023-10-14 21:20:33.000000 ovos-tts-server-0.0.3a9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-10-14 21:20:34.841049 ovos-tts-server-0.0.3a9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 21:20:34.837049 ovos-tts-server-0.0.3a9/ovos_tts_server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2023-10-14 21:20:33.000000 ovos-tts-server-0.0.3a9/ovos_tts_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2023-10-14 21:20:33.000000 ovos-tts-server-0.0.3a9/ovos_tts_server/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 21:20:34.841049 ovos-tts-server-0.0.3a9/ovos_tts_server/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2023-10-14 21:20:33.000000 ovos-tts-server-0.0.3a9/ovos_tts_server/examples/rainbow.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2023-10-14 21:20:33.000000 ovos-tts-server-0.0.3a9/ovos_tts_server/gradio_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2023-10-14 21:20:33.000000 ovos-tts-server-0.0.3a9/ovos_tts_server/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 21:20:34.841049 ovos-tts-server-0.0.3a9/ovos_tts_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-10-14 21:20:34.000000 ovos-tts-server-0.0.3a9/ovos_tts_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2023-10-14 21:20:34.000000 ovos-tts-server-0.0.3a9/ovos_tts_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-14 21:20:34.000000 ovos-tts-server-0.0.3a9/ovos_tts_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-14 21:20:34.000000 ovos-tts-server-0.0.3a9/ovos_tts_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-10-14 21:20:34.000000 ovos-tts-server-0.0.3a9/ovos_tts_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-14 21:20:34.000000 ovos-tts-server-0.0.3a9/ovos_tts_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-14 21:20:34.000000 ovos-tts-server-0.0.3a9/ovos_tts_server.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-14 21:20:34.841049 ovos-tts-server-0.0.3a9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3054 2023-10-14 21:20:33.000000 ovos-tts-server-0.0.3a9/setup.py
```

### Comparing `ovos-tts-server-0.0.3a8/LICENSE.md` & `ovos-tts-server-0.0.3a9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-tts-server-0.0.3a8/PKG-INFO` & `ovos-tts-server-0.0.3a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-server
-Version: 0.0.3a8
+Version: 0.0.3a9
 Summary: simple FastAPI server to host TTS plugins as a service
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-server
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: plugin TTS OVOS OpenVoiceOS
 Platform: UNKNOWN
```

### Comparing `ovos-tts-server-0.0.3a8/ovos_tts_server/__init__.py` & `ovos-tts-server-0.0.3a9/ovos_tts_server/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,29 +12,31 @@
 from fastapi import FastAPI
 from fastapi.responses import FileResponse
 from ovos_plugin_manager.tts import load_tts_plugin
 from ovos_utils.log import LOG
 from ovos_config import Configuration
 from starlette.requests import Request
 
+
+LOG.set_level("ERROR")  # avoid server side logs
+
 TTS = None
 
 
 def create_app(tts_plugin, has_gradio=False):
     app = FastAPI()
 
     @app.get("/status")
     def stats(request: Request):
         return {"status": "ok",
                 "plugin": tts_plugin,
                 "gradio": has_gradio}
 
     @app.get("/synthesize/{utterance}")
     def synth(utterance: str, request: Request):
-        LOG.debug(f"{utterance}|{request.query_params}")
         utterance = TTS.validate_ssml(utterance)
         audio, phonemes = TTS.synth(utterance, **request.query_params)
         return FileResponse(audio.path)
 
     return app
```

### Comparing `ovos-tts-server-0.0.3a8/ovos_tts_server/__main__.py` & `ovos-tts-server-0.0.3a9/ovos_tts_server/__main__.py`

 * *Files identical despite different names*

### Comparing `ovos-tts-server-0.0.3a8/ovos_tts_server/examples/rainbow.json` & `ovos-tts-server-0.0.3a9/ovos_tts_server/examples/rainbow.json`

 * *Files identical despite different names*

### Comparing `ovos-tts-server-0.0.3a8/ovos_tts_server/gradio_app.py` & `ovos-tts-server-0.0.3a9/ovos_tts_server/gradio_app.py`

 * *Files identical despite different names*

### Comparing `ovos-tts-server-0.0.3a8/ovos_tts_server.egg-info/PKG-INFO` & `ovos-tts-server-0.0.3a9/ovos_tts_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-server
-Version: 0.0.3a8
+Version: 0.0.3a9
 Summary: simple FastAPI server to host TTS plugins as a service
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-server
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: plugin TTS OVOS OpenVoiceOS
 Platform: UNKNOWN
```

### Comparing `ovos-tts-server-0.0.3a8/setup.py` & `ovos-tts-server-0.0.3a9/setup.py`

 * *Files identical despite different names*

