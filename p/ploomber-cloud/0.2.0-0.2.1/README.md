# Comparing `tmp/ploomber-cloud-0.2.0.tar.gz` & `tmp/ploomber-cloud-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomber-cloud-0.2.0.tar", last modified: Tue Apr 23 00:37:33 2024, max compression
+gzip compressed data, was "ploomber-cloud-0.2.1.tar", last modified: Thu Apr 25 21:27:41 2024, max compression
```

## Comparing `ploomber-cloud-0.2.0.tar` & `ploomber-cloud-0.2.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:37:33.369985 ploomber-cloud-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 00:37:33.369985 ploomber-cloud-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-23 00:37:33.369985 ploomber-cloud-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:37:33.365985 ploomber-cloud-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:37:33.369985 ploomber-cloud-0.2.0/src/ploomber_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:37:33.369985 ploomber-cloud-0.2.0/src/ploomber_cloud/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:37:33.369985 ploomber-cloud-0.2.0/src/ploomber_cloud/assets/vllm/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/assets/vllm/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/assets/vllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/assets/vllm/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/assets/vllm/test-vllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:37:33.369985 ploomber-cloud-0.2.0/src/ploomber_cloud/configurations/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/configurations/community.json
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/configurations/premium.json
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/zip_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:37:33.369985 ploomber-cloud-0.2.0/src/ploomber_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 00:37:33.000000 ploomber-cloud-0.2.0/src/ploomber_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-23 00:37:33.000000 ploomber-cloud-0.2.0/src/ploomber_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 00:37:33.000000 ploomber-cloud-0.2.0/src/ploomber_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-23 00:37:33.000000 ploomber-cloud-0.2.0/src/ploomber_cloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-23 00:37:33.000000 ploomber-cloud-0.2.0/src/ploomber_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 00:37:33.000000 ploomber-cloud-0.2.0/src/ploomber_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:27:41.263800 ploomber-cloud-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-25 21:27:41.263800 ploomber-cloud-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-25 21:27:41.263800 ploomber-cloud-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:27:41.255800 ploomber-cloud-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:27:41.263800 ploomber-cloud-0.2.1/src/ploomber_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:27:41.263800 ploomber-cloud-0.2.1/src/ploomber_cloud/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:27:41.263800 ploomber-cloud-0.2.1/src/ploomber_cloud/assets/vllm/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/assets/vllm/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/assets/vllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/assets/vllm/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/assets/vllm/test-vllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:27:41.263800 ploomber-cloud-0.2.1/src/ploomber_cloud/configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/configurations/community.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/configurations/premium.json
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/zip_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:27:41.263800 ploomber-cloud-0.2.1/src/ploomber_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-25 21:27:41.000000 ploomber-cloud-0.2.1/src/ploomber_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-25 21:27:41.000000 ploomber-cloud-0.2.1/src/ploomber_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:27:41.000000 ploomber-cloud-0.2.1/src/ploomber_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 21:27:41.000000 ploomber-cloud-0.2.1/src/ploomber_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-25 21:27:41.000000 ploomber-cloud-0.2.1/src/ploomber_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 21:27:41.000000 ploomber-cloud-0.2.1/src/ploomber_cloud.egg-info/top_level.txt
```

### Comparing `ploomber-cloud-0.2.0/CHANGELOG.md` & `ploomber-cloud-0.2.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # CHANGELOG
 
+## 0.2.1 (2024-04-25)
+
+- [Feature] Handles 500 errors
+- [Feature] Add `ploomber-cloud templates auth0`
+
 ## 0.2.0 (2024-04-22)
 
 - [Feature] Add `ploomber-cloud resources` to enable custom resources
 
 ## 0.1.29 (2024-04-17)
 
 - [Fix] Improve output message for the delete command
```

### Comparing `ploomber-cloud-0.2.0/pyproject.toml` & `ploomber-cloud-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.0/setup.py` & `ploomber-cloud-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/api.py` & `ploomber-cloud-0.2.1/src/ploomber_cloud/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,14 +54,17 @@
     """Client for the Ploomber Cloud API"""
 
     def _process_response(self, response):
         """Process response and raise an exception if the status code is not 200"""
         if response.ok:
             return response.json()
         else:
+            if response.status_code == 500:
+                raise exceptions.InternalServerErrorException
+
             error_message = response.json()["detail"]
             # if project is deleted from app re-initialization
             # required with new config file
             if response.status_code == 404:
                 error_message = f"{error_message}\n{FORCE_INIT_MESSAGE}"
             raise exceptions.BasePloomberCloudException(
                 f"An error occurred: {error_message}"
@@ -122,29 +125,33 @@
             f"{API_ROOT}/projects/",
             headers=self._get_headers(),
         )
 
         return self._process_response(response)
 
     def deploy(
-        self, path_to_zip, project_type, project_id, secrets=None, resources=None
+        self,
+        path_to_zip,
+        project_type,
+        project_id,
+        secrets=None,
+        resources=None,
+        template=None,
     ):
         """Deploy a project"""
 
         with open(path_to_zip, "rb") as file:
             files = {
                 "files": (
                     "app.zip",
                     file,
                     "application/zip",
                 ),
             }
-            data = {
-                "secrets": secrets,
-            }
+            data = {"secrets": secrets, "template": template}
 
             if resources:
                 data["cpu"] = resources["cpu"]
                 data["ram"] = resources["ram"]
                 data["gpu"] = resources["gpu"]
 
             response = requests.post(
```

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/api_key.py` & `ploomber-cloud-0.2.1/src/ploomber_cloud/api_key.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/assets/vllm/requirements.txt` & `ploomber-cloud-0.2.1/src/ploomber_cloud/assets/vllm/requirements.txt`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/assets/vllm/test-vllm.py` & `ploomber-cloud-0.2.1/src/ploomber_cloud/assets/vllm/test-vllm.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/cli.py` & `ploomber-cloud-0.2.1/src/ploomber_cloud/cli.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/config.py` & `ploomber-cloud-0.2.1/src/ploomber_cloud/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,16 @@
 
         return error
 
     def _validate_config(self):
         """Method to validate the ploomber-cloud.json file
         for common issues"""
         KEYS_REQUIRED = {"id", "type"}
-        KEYS_OPTIONAL = {"resources"}
-        TYPES = {"id": str, "type": str, "resources": dict}
+        KEYS_OPTIONAL = {"resources", "template"}
+        TYPES = {"id": str, "type": str, "resources": dict, "template": str}
 
         error = ""
 
         for key in KEYS_REQUIRED:
             if key not in self._data.keys():
                 error = f"{error}Mandatory key '{key}' is missing.\n"
```

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/configurations/community.json` & `ploomber-cloud-0.2.1/src/ploomber_cloud/configurations/community.json`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/configurations/premium.json` & `ploomber-cloud-0.2.1/src/ploomber_cloud/configurations/premium.json`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/constants.py` & `ploomber-cloud-0.2.1/src/ploomber_cloud/constants.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/delete.py` & `ploomber-cloud-0.2.1/src/ploomber_cloud/delete.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/deploy.py` & `ploomber-cloud-0.2.1/src/ploomber_cloud/deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,15 @@
         try:
             output = client.deploy(
                 path_to_zip=path_to_zip,
                 project_type=config.data["type"],
                 project_id=config.data["id"],
                 secrets=secrets,
                 resources=config.data.get("resources"),
+                template=config.data.get("template"),
             )
         except BasePloomberCloudException as e:
             if "Invalid Resource" in e.get_message():
                 cpu_options, ram_options, gpu_options = _get_resource_choices()
                 cpu_options = [float(opt) for opt in cpu_options]
                 ram_options = [int(float(opt)) for opt in ram_options]
```

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/examples.py` & `ploomber-cloud-0.2.1/src/ploomber_cloud/examples.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/exceptions.py` & `ploomber-cloud-0.2.1/src/ploomber_cloud/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,7 +53,15 @@
     pass
 
 
 class InvalidPloomberResourcesException(BasePloomberCloudException):
     """Exception for invalid resource choices"""
 
     pass
+
+
+class InternalServerErrorException(BasePloomberCloudException):
+    """Exception for 500 errors"""
+
+    def __init__(self):
+        message = "Internal server error. Please contact support: contact@ploomber.io"
+        super().__init__(message)
```

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/functions.py` & `ploomber-cloud-0.2.1/src/ploomber_cloud/functions.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/github.py` & `ploomber-cloud-0.2.1/src/ploomber_cloud/github.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/init.py` & `ploomber-cloud-0.2.1/src/ploomber_cloud/init.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/resources.py` & `ploomber-cloud-0.2.1/src/ploomber_cloud/resources.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/util.py` & `ploomber-cloud-0.2.1/src/ploomber_cloud/util.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud/zip_.py` & `ploomber-cloud-0.2.1/src/ploomber_cloud/zip_.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.0/src/ploomber_cloud.egg-info/SOURCES.txt` & `ploomber-cloud-0.2.1/src/ploomber_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

