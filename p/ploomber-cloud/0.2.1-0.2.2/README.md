# Comparing `tmp/ploomber-cloud-0.2.1.tar.gz` & `tmp/ploomber-cloud-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomber-cloud-0.2.1.tar", last modified: Thu Apr 25 21:27:41 2024, max compression
+gzip compressed data, was "ploomber-cloud-0.2.2.tar", last modified: Fri Apr 26 17:24:58 2024, max compression
```

## Comparing `ploomber-cloud-0.2.1.tar` & `ploomber-cloud-0.2.2.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:27:41.263800 ploomber-cloud-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-25 21:27:41.263800 ploomber-cloud-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-25 21:27:41.263800 ploomber-cloud-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:27:41.255800 ploomber-cloud-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:27:41.263800 ploomber-cloud-0.2.1/src/ploomber_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:27:41.263800 ploomber-cloud-0.2.1/src/ploomber_cloud/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:27:41.263800 ploomber-cloud-0.2.1/src/ploomber_cloud/assets/vllm/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/assets/vllm/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/assets/vllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/assets/vllm/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/assets/vllm/test-vllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:27:41.263800 ploomber-cloud-0.2.1/src/ploomber_cloud/configurations/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/configurations/community.json
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/configurations/premium.json
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-25 21:27:28.000000 ploomber-cloud-0.2.1/src/ploomber_cloud/zip_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:27:41.263800 ploomber-cloud-0.2.1/src/ploomber_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-25 21:27:41.000000 ploomber-cloud-0.2.1/src/ploomber_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-25 21:27:41.000000 ploomber-cloud-0.2.1/src/ploomber_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:27:41.000000 ploomber-cloud-0.2.1/src/ploomber_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 21:27:41.000000 ploomber-cloud-0.2.1/src/ploomber_cloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-25 21:27:41.000000 ploomber-cloud-0.2.1/src/ploomber_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 21:27:41.000000 ploomber-cloud-0.2.1/src/ploomber_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:24:58.576445 ploomber-cloud-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 17:24:58.576445 ploomber-cloud-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 17:24:58.576445 ploomber-cloud-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:24:58.568446 ploomber-cloud-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:24:58.572445 ploomber-cloud-0.2.2/src/ploomber_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:24:58.572445 ploomber-cloud-0.2.2/src/ploomber_cloud/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:24:58.576445 ploomber-cloud-0.2.2/src/ploomber_cloud/assets/vllm/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/assets/vllm/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/assets/vllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/assets/vllm/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/assets/vllm/test-vllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:24:58.576445 ploomber-cloud-0.2.2/src/ploomber_cloud/configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/configurations/community.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/configurations/premium.json
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-26 17:24:45.000000 ploomber-cloud-0.2.2/src/ploomber_cloud/zip_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:24:58.572445 ploomber-cloud-0.2.2/src/ploomber_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 17:24:58.000000 ploomber-cloud-0.2.2/src/ploomber_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-26 17:24:58.000000 ploomber-cloud-0.2.2/src/ploomber_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 17:24:58.000000 ploomber-cloud-0.2.2/src/ploomber_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-26 17:24:58.000000 ploomber-cloud-0.2.2/src/ploomber_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-26 17:24:58.000000 ploomber-cloud-0.2.2/src/ploomber_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 17:24:58.000000 ploomber-cloud-0.2.2/src/ploomber_cloud.egg-info/top_level.txt
```

### Comparing `ploomber-cloud-0.2.1/CHANGELOG.md` & `ploomber-cloud-0.2.2/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # CHANGELOG
 
+## 0.2.2 (2024-04-26)
+
+- [Feature] Better validation when running `ploomber-cloud templates auth0`
+- [Feature] Automatically generated `AUTH_SCRET` when using `ploomber-cloud templates auth0`
+
 ## 0.2.1 (2024-04-25)
 
 - [Feature] Handles 500 errors
 - [Feature] Add `ploomber-cloud templates auth0`
 
 ## 0.2.0 (2024-04-22)
```

### Comparing `ploomber-cloud-0.2.1/pyproject.toml` & `ploomber-cloud-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/setup.py` & `ploomber-cloud-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/api.py` & `ploomber-cloud-0.2.2/src/ploomber_cloud/api.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/api_key.py` & `ploomber-cloud-0.2.2/src/ploomber_cloud/api_key.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/assets/vllm/requirements.txt` & `ploomber-cloud-0.2.2/src/ploomber_cloud/assets/vllm/requirements.txt`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/assets/vllm/test-vllm.py` & `ploomber-cloud-0.2.2/src/ploomber_cloud/assets/vllm/test-vllm.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/cli.py` & `ploomber-cloud-0.2.2/src/ploomber_cloud/cli.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/config.py` & `ploomber-cloud-0.2.2/src/ploomber_cloud/config.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/configurations/community.json` & `ploomber-cloud-0.2.2/src/ploomber_cloud/configurations/community.json`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/configurations/premium.json` & `ploomber-cloud-0.2.2/src/ploomber_cloud/configurations/premium.json`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/constants.py` & `ploomber-cloud-0.2.2/src/ploomber_cloud/constants.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/delete.py` & `ploomber-cloud-0.2.2/src/ploomber_cloud/delete.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/deploy.py` & `ploomber-cloud-0.2.2/src/ploomber_cloud/deploy.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/examples.py` & `ploomber-cloud-0.2.2/src/ploomber_cloud/examples.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/exceptions.py` & `ploomber-cloud-0.2.2/src/ploomber_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/functions.py` & `ploomber-cloud-0.2.2/src/ploomber_cloud/functions.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/github.py` & `ploomber-cloud-0.2.2/src/ploomber_cloud/github.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/init.py` & `ploomber-cloud-0.2.2/src/ploomber_cloud/init.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/resources.py` & `ploomber-cloud-0.2.2/src/ploomber_cloud/resources.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/templates.py` & `ploomber-cloud-0.2.2/src/ploomber_cloud/templates.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import click
 
 from ploomber_cloud.assets import vllm as vllm_resources
 from ploomber_cloud.config import PloomberCloudConfig
 from ploomber_cloud.util import pretty_print
 from ploomber_cloud.exceptions import BasePloomberCloudException
 from ploomber_cloud import init, deploy
+from ploomber_cloud import io
 
 
 def validate_model_name(model_name):
     """Verify that HF model exists by name"""
     response = requests.get(f"https://huggingface.co/api/models/{model_name}")
 
     if response.ok:
@@ -151,14 +152,42 @@
         )
         return
     else:
         deploy.deploy(watch=False)
         click.secho("Deployment started, should take about 12 minutes.", fg="green")
 
 
+def validate_auth_issues_base_url(value):
+    if value.startswith("https://"):
+        return io.ValidationResult(
+            is_valid=True,
+            error_message=None,
+            value_validated=value,
+        )
+    else:
+        # the auth0 console doesn't show the protocol, so we add it in case the
+        # user copied and paste the value
+        if (
+            ".auth0.com" in value
+            and not value.startswith("https://")
+            and not value.startswith("http://")
+        ):
+            return io.ValidationResult(
+                is_valid=True,
+                error_message=None,
+                value_validated=f"https://{value}",
+            )
+
+        return io.ValidationResult(
+            is_valid=False,
+            error_message="must start with https://",
+            value_validated=None,
+        )
+
+
 def auth0():
     """Configure auth0 for an existing project"""
     # Check for init, if not, prompt and run init flow
     if not Path("ploomber-cloud.json").exists():
         run_init = click.confirm(
             "Project must be initialized to continue. Would you like to initialize?"
         )
@@ -169,24 +198,31 @@
                 "Run 'ploomber-cloud init' to initialize your project."
             )
 
         init.init(from_existing=False, force=False)
 
     # Prompt for secrets
     auth0_secrets = {
-        "AUTH_SECRET": None,
         "AUTH_CLIENT_ID": None,
         "AUTH_ISSUER_BASE_URL": None,
     }
 
+    validators = {"AUTH_ISSUER_BASE_URL": validate_auth_issues_base_url}
+
     for key in auth0_secrets.keys():
-        auth0_secrets[key] = click.prompt(f"Enter the value for {key}")
+        auth0_secrets[key] = io.prompt(
+            validator=validators.get(key),
+            text=f"Enter the value for {key}",
+        )
+
+    auth0_secrets["AUTH_SECRET"] = secrets.token_urlsafe()
 
     # Check for `.env` and load secrets if they exist
     final_secrets = {}
+
     if Path(".env").exists():
         final_secrets = dotenv_values(".env")
 
     # Add user-input secrets. Overrides keys if they already exist.
     final_secrets.update(auth0_secrets)
 
     # Write old and new secrets to .env
```

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/util.py` & `ploomber-cloud-0.2.2/src/ploomber_cloud/util.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud/zip_.py` & `ploomber-cloud-0.2.2/src/ploomber_cloud/zip_.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.1/src/ploomber_cloud.egg-info/SOURCES.txt` & `ploomber-cloud-0.2.2/src/ploomber_cloud.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 src/ploomber_cloud/delete.py
 src/ploomber_cloud/deploy.py
 src/ploomber_cloud/examples.py
 src/ploomber_cloud/exceptions.py
 src/ploomber_cloud/functions.py
 src/ploomber_cloud/github.py
 src/ploomber_cloud/init.py
+src/ploomber_cloud/io.py
 src/ploomber_cloud/resources.py
 src/ploomber_cloud/templates.py
 src/ploomber_cloud/util.py
 src/ploomber_cloud/zip_.py
 src/ploomber_cloud.egg-info/PKG-INFO
 src/ploomber_cloud.egg-info/SOURCES.txt
 src/ploomber_cloud.egg-info/dependency_links.txt
```

