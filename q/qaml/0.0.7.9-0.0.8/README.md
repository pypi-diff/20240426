# Comparing `tmp/qaml-0.0.7.9.tar.gz` & `tmp/qaml-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaml-0.0.7.9.tar", last modified: Fri Apr 19 14:19:14 2024, max compression
+gzip compressed data, was "qaml-0.0.8.tar", last modified: Fri Apr 26 14:52:42 2024, max compression
```

## Comparing `qaml-0.0.7.9.tar` & `qaml-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-19 14:19:14.713387 qaml-0.0.7.9/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.7.9/LICENSE
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-19 14:19:14.713245 qaml-0.0.7.9/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.7.9/README.md
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      735 2024-04-19 14:18:58.000000 qaml-0.0.7.9/pyproject.toml
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-19 14:19:14.712391 qaml-0.0.7.9/qaml/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.7.9/qaml/__init__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      948 2024-04-18 00:07:26.000000 qaml-0.0.7.9/qaml/__main__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)    12871 2024-04-19 14:15:29.000000 qaml-0.0.7.9/qaml/client.py
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-19 14:19:14.713089 qaml-0.0.7.9/qaml.egg-info/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-19 14:19:14.000000 qaml-0.0.7.9/qaml.egg-info/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-19 14:19:14.000000 qaml-0.0.7.9/qaml.egg-info/SOURCES.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-19 14:19:14.000000 qaml-0.0.7.9/qaml.egg-info/dependency_links.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-19 14:19:14.000000 qaml-0.0.7.9/qaml.egg-info/entry_points.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-19 14:19:14.000000 qaml-0.0.7.9/qaml.egg-info/requires.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-19 14:19:14.000000 qaml-0.0.7.9/qaml.egg-info/top_level.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-19 14:19:14.713420 qaml-0.0.7.9/setup.cfg
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-26 14:52:42.457144 qaml-0.0.8/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.8/LICENSE
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1561 2024-04-26 14:52:42.457001 qaml-0.0.8/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.8/README.md
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      733 2024-04-26 14:52:38.000000 qaml-0.0.8/pyproject.toml
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-26 14:52:42.456153 qaml-0.0.8/qaml/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.8/qaml/__init__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      948 2024-04-18 00:07:26.000000 qaml-0.0.8/qaml/__main__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)    13893 2024-04-26 03:13:02.000000 qaml-0.0.8/qaml/client.py
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-26 14:52:42.456866 qaml-0.0.8/qaml.egg-info/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1561 2024-04-26 14:52:42.000000 qaml-0.0.8/qaml.egg-info/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-26 14:52:42.000000 qaml-0.0.8/qaml.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-26 14:52:42.000000 qaml-0.0.8/qaml.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-26 14:52:42.000000 qaml-0.0.8/qaml.egg-info/entry_points.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-26 14:52:42.000000 qaml-0.0.8/qaml.egg-info/requires.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-26 14:52:42.000000 qaml-0.0.8/qaml.egg-info/top_level.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-26 14:52:42.457189 qaml-0.0.8/setup.cfg
```

### Comparing `qaml-0.0.7.9/LICENSE` & `qaml-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.9/PKG-INFO` & `qaml-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.7.9
+Version: 0.0.8
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `qaml-0.0.7.9/README.md` & `qaml-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.9/pyproject.toml` & `qaml-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qaml"
-version = "0.0.7.9"
+version = "0.0.8"
 authors = [
     {name = "Miguel Salinas", email = "miguel@camelqa.com"},
 ]
 description = "Control your devices with natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qaml-0.0.7.9/qaml/__main__.py` & `qaml-0.0.8/qaml/__main__.py`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.9/qaml/client.py` & `qaml-0.0.8/qaml/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,22 +12,23 @@
 import requests
 import os
 
 class QAMLExecException(Exception):
     pass
 
 class BaseClient:
-    def __init__(self, api_key):
+    def __init__(self, api_key, api_base_url="https://api.camelqa.com"):
         self.api_key = api_key or os.environ.get("QAML_API_KEY")
+        self.api_base_url = os.environ.get("QAML_API_BASE_URL", api_base_url)
         self.driver = None
         self.platform = None
         self.screen_size = None
         self.req_session = requests.Session()
         self.req_session.headers.update({"Authorization": f"Bearer {api_key}"})
-        self.context = ''
+        self.system_prompt = None
         self.available_functions = {
             "tap": self.tap_coordinates,
             "drag": self.drag,
             "swipe": self.swipe,
             "scroll": self.scroll,
             "type_text": self.type_text,
             "sleep": self.sleep,
@@ -54,17 +55,14 @@
 
     def sleep(self, duration):
         time.sleep(duration)
 
     def report_error(self, reason):
         raise QAMLExecException(reason)
 
-    def set_context(self, context):
-        self.context = context
-
     def get_screenshot(self):
         screenshot = self.driver.get_screenshot_as_base64()
         PIL_image = Image.open(BytesIO(base64.b64decode(screenshot)))
         longer_side = max(PIL_image.size)
         aspect_ratio = PIL_image.size[0] / PIL_image.size[1]
         new_size = (960, int(960 / aspect_ratio)) if PIL_image.size[0] == longer_side else (int(960 * aspect_ratio), 960)
         PIL_image = PIL_image.resize(new_size)
@@ -76,27 +74,47 @@
     def _execute_function(self, function_name, **kwargs):
         function = self.available_functions.get(function_name)
         if function:
             function(**kwargs)
 
     def execute(self, script):
         screenshot = self.get_screenshot()
-        payload = {"action": script, "screen_size": self.screen_size, "screenshot": screenshot, "platform": self.platform, "extra_context": self.context}
-        response = self.req_session.post("https://api.camelqa.com/v1/execute", json=payload, headers={"Authorization": f"Bearer {self.api_key}"})
+        """
+        now = time.time()
+        appium_page_source = self.driver.page_source
+        print(f"Page source: {appium_page_source}", time.time() - now)
+        """
+        payload = {"action": script, "screen_size": self.screen_size, "screenshot": screenshot, "platform": self.platform, "extra_context": self.system_prompt}
+        response = self.req_session.post(f"{self.api_base_url}/v1/execute", json=payload, headers={"Authorization": f"Bearer {self.api_key}"})
+        print(f"Action: {script} - Response: {response.text}")
+        try:
+            actions = response.json()
+            for action in actions:
+                self._execute_function(action["name"], **json.loads(action["arguments"]))
+        except Exception as e:
+            print(e)
+            pass
+
+    def assert_condition(self, script):
+        screenshot = self.get_screenshot()
+        payload = {"assertion": script, "screen_size": self.screen_size, "screenshot": screenshot, "platform": self.platform, "extra_context": self.system_prompt}
+        response = self.req_session.post(f"{self.api_base_url}/v1/assert", json=payload, headers={"Authorization": f"Bearer {self.api_key}"})
         print(f"Action: {script} - Response: {response.text}")
-        actions = response.json()
-        for action in actions:
-            self._execute_function(action["name"], **json.loads(action["arguments"]))
+        assertion = response.json()[0]
+        args = json.loads(assertion["arguments"])
+        if not args["result"]:
+            raise QAMLExecException(f"Assertion failed: {script}. Reason: {args['reason']}")
+        return response.json()
 
     def agent(self, task):
         progress = []
         while True:
             screenshot = self.get_screenshot()
             payload = {"task": task, "progress": progress, "platform": self.platform, "screenshot": screenshot}
-            response = self.req_session.post("https://api.camelqa.com/v1/agent", json=payload)
+            response = self.req_session.post(f"{self.api_base_url}/v1/agent", json=payload)
             response_json = response.json()
             status = response_json["status"]
             progress += response_json["progress"]
             actions = response_json["actions"]
             if status != "in_progress":
                 return status, progress
             for action in actions:
```

### Comparing `qaml-0.0.7.9/qaml.egg-info/PKG-INFO` & `qaml-0.0.8/qaml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.7.9
+Version: 0.0.8
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

