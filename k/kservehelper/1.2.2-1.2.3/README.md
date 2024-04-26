# Comparing `tmp/kservehelper-1.2.2.tar.gz` & `tmp/kservehelper-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kservehelper-1.2.2.tar", last modified: Wed Apr  3 03:06:00 2024, max compression
+gzip compressed data, was "kservehelper-1.2.3.tar", last modified: Fri Apr 26 06:31:23 2024, max compression
```

## Comparing `kservehelper-1.2.2.tar` & `kservehelper-1.2.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.181577 kservehelper-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-03 03:06:00.181577 kservehelper-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-03 03:05:52.000000 kservehelper-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.173577 kservehelper-1.2.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.173577 kservehelper-1.2.2/examples/blur-image/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-03 03:05:52.000000 kservehelper-1.2.2/examples/blur-image/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.173577 kservehelper-1.2.2/examples/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-03 03:05:52.000000 kservehelper-1.2.2/examples/dummy/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.173577 kservehelper-1.2.2/examples/rotate-image/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-03 03:05:52.000000 kservehelper-1.2.2/examples/rotate-image/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.173577 kservehelper-1.2.2/examples/stable-diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-03 03:05:52.000000 kservehelper-1.2.2/examples/stable-diffusion/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-03 03:05:52.000000 kservehelper-1.2.2/examples/stable-diffusion/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.173577 kservehelper-1.2.2/examples/stable-diffusion-xl/
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-03 03:05:52.000000 kservehelper-1.2.2/examples/stable-diffusion-xl/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.177577 kservehelper-1.2.2/kservehelper/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14033 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/docker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.177577 kservehelper-1.2.2/kservehelper/kserve/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/kserve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/kserve/model_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.177577 kservehelper-1.2.2/kservehelper/kserve/rest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/kserve/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/kserve/rest/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/kserve/rest/v1_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    11422 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9883 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.181577 kservehelper-1.2.2/kservehelper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-03 03:06:00.000000 kservehelper-1.2.2/kservehelper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-03 03:06:00.000000 kservehelper-1.2.2/kservehelper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 03:06:00.000000 kservehelper-1.2.2/kservehelper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 03:06:00.000000 kservehelper-1.2.2/kservehelper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 03:05:59.000000 kservehelper-1.2.2/kservehelper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 03:06:00.000000 kservehelper-1.2.2/kservehelper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 03:06:00.000000 kservehelper-1.2.2/kservehelper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 03:06:00.181577 kservehelper-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-03 03:05:52.000000 kservehelper-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.181577 kservehelper-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-03 03:05:52.000000 kservehelper-1.2.2/tests/test_batch_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-03 03:05:52.000000 kservehelper-1.2.2/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-03 03:05:52.000000 kservehelper-1.2.2/tests/test_model_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-03 03:05:52.000000 kservehelper-1.2.2/tests/test_predict.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-03 03:05:52.000000 kservehelper-1.2.2/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-03 03:05:52.000000 kservehelper-1.2.2/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-03 03:05:52.000000 kservehelper-1.2.2/tests/test_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:31:23.891567 kservehelper-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-26 06:31:23.891567 kservehelper-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-26 06:31:19.000000 kservehelper-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:31:23.883566 kservehelper-1.2.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:31:23.883566 kservehelper-1.2.3/examples/blur-image/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-26 06:31:19.000000 kservehelper-1.2.3/examples/blur-image/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:31:23.883566 kservehelper-1.2.3/examples/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-26 06:31:19.000000 kservehelper-1.2.3/examples/dummy/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:31:23.883566 kservehelper-1.2.3/examples/rotate-image/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-26 06:31:19.000000 kservehelper-1.2.3/examples/rotate-image/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:31:23.883566 kservehelper-1.2.3/examples/stable-diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-26 06:31:19.000000 kservehelper-1.2.3/examples/stable-diffusion/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-26 06:31:19.000000 kservehelper-1.2.3/examples/stable-diffusion/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:31:23.883566 kservehelper-1.2.3/examples/stable-diffusion-xl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-26 06:31:19.000000 kservehelper-1.2.3/examples/stable-diffusion-xl/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:31:23.887567 kservehelper-1.2.3/kservehelper/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-26 06:31:19.000000 kservehelper-1.2.3/kservehelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14033 2024-04-26 06:31:19.000000 kservehelper-1.2.3/kservehelper/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-26 06:31:19.000000 kservehelper-1.2.3/kservehelper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9400 2024-04-26 06:31:19.000000 kservehelper-1.2.3/kservehelper/docker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:31:23.887567 kservehelper-1.2.3/kservehelper/kserve/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-26 06:31:19.000000 kservehelper-1.2.3/kservehelper/kserve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-04-26 06:31:19.000000 kservehelper-1.2.3/kservehelper/kserve/model_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:31:23.887567 kservehelper-1.2.3/kservehelper/kserve/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 06:31:19.000000 kservehelper-1.2.3/kservehelper/kserve/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-04-26 06:31:19.000000 kservehelper-1.2.3/kservehelper/kserve/rest/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-26 06:31:19.000000 kservehelper-1.2.3/kservehelper/kserve/rest/v1_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11422 2024-04-26 06:31:19.000000 kservehelper-1.2.3/kservehelper/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-26 06:31:19.000000 kservehelper-1.2.3/kservehelper/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9883 2024-04-26 06:31:19.000000 kservehelper-1.2.3/kservehelper/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-26 06:31:19.000000 kservehelper-1.2.3/kservehelper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:31:23.891567 kservehelper-1.2.3/kservehelper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-26 06:31:23.000000 kservehelper-1.2.3/kservehelper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-26 06:31:23.000000 kservehelper-1.2.3/kservehelper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 06:31:23.000000 kservehelper-1.2.3/kservehelper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-26 06:31:23.000000 kservehelper-1.2.3/kservehelper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 06:31:23.000000 kservehelper-1.2.3/kservehelper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-26 06:31:23.000000 kservehelper-1.2.3/kservehelper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-26 06:31:23.000000 kservehelper-1.2.3/kservehelper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 06:31:23.891567 kservehelper-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-26 06:31:19.000000 kservehelper-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:31:23.891567 kservehelper-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-26 06:31:19.000000 kservehelper-1.2.3/tests/test_batch_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-26 06:31:19.000000 kservehelper-1.2.3/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-26 06:31:19.000000 kservehelper-1.2.3/tests/test_model_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-26 06:31:19.000000 kservehelper-1.2.3/tests/test_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-26 06:31:19.000000 kservehelper-1.2.3/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-26 06:31:19.000000 kservehelper-1.2.3/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-26 06:31:19.000000 kservehelper-1.2.3/tests/test_upload.py
```

### Comparing `kservehelper-1.2.2/PKG-INFO` & `kservehelper-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kservehelper
-Version: 1.2.2
+Version: 1.2.3
 Summary: A KServe Model Wrapper
 Home-page: https://github.com/yangwenz/kserve-helper
 Author: Wenzhuo Yang
 License: 3-Clause BSD
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Requires-Dist: kserve==0.10.2
```

### Comparing `kservehelper-1.2.2/README.md` & `kservehelper-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/examples/blur-image/model.py` & `kservehelper-1.2.3/examples/blur-image/model.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/examples/dummy/model.py` & `kservehelper-1.2.3/examples/dummy/model.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/examples/rotate-image/model.py` & `kservehelper-1.2.3/examples/rotate-image/model.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/examples/stable-diffusion/model.py` & `kservehelper-1.2.3/examples/stable-diffusion/model.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/examples/stable-diffusion-xl/model.py` & `kservehelper-1.2.3/examples/stable-diffusion-xl/model.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/kservehelper/cache.py` & `kservehelper-1.2.3/kservehelper/cache.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/kservehelper/cli.py` & `kservehelper-1.2.3/kservehelper/cli.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/kservehelper/docker.py` & `kservehelper-1.2.3/kservehelper/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
             Optional("cuda_image_type"): lambda x: x in ["base", "runtime", "devel"],
             Optional("cudnn"): bool,
             Optional("ngc"): bool,
             Optional("commands"): list,
             Optional("system_packages"): list,
             Optional("python_requirements"): list,
             Optional("python_packages"): list,
+            Optional("additional_commands"): list,
         },
         "image": str,
         "entrypoint": str
     }
 )
 
 DOCKER_IMAGES = {
@@ -175,14 +176,20 @@
         commands.append("RUN pip install --no-cache-dir --upgrade pip")
         commands.append("RUN pip install --no-cache-dir \\")
         for package in config["build"]["python_packages"][:-1]:
             commands.append(f"    {package} \\")
         commands.append(f"    {config['build']['python_packages'][-1]}")
         commands.append("")
 
+    # Extra commands
+    if "additional_commands" in config["build"] and len(config["build"]["additional_commands"]) > 0:
+        for command in config["build"]["additional_commands"]:
+            commands.append(f"RUN {command}")
+        commands.append("")
+
     # Copy the code and artifacts
     commands.append("WORKDIR /app")
     commands.append("")
     for file in os.listdir(folder):
         if file not in IGNORED_FILES:
             if not os.path.isdir(file):
                 commands.append(f"COPY {file} .")
```

### Comparing `kservehelper-1.2.2/kservehelper/kserve/model_server.py` & `kservehelper-1.2.3/kservehelper/kserve/model_server.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/kservehelper/kserve/rest/server.py` & `kservehelper-1.2.3/kservehelper/kserve/rest/server.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/kservehelper/kserve/rest/v1_endpoints.py` & `kservehelper-1.2.3/kservehelper/kserve/rest/v1_endpoints.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/kservehelper/model.py` & `kservehelper-1.2.3/kservehelper/model.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/kservehelper/storage.py` & `kservehelper-1.2.3/kservehelper/storage.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/kservehelper/types.py` & `kservehelper-1.2.3/kservehelper/types.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/kservehelper/utils.py` & `kservehelper-1.2.3/kservehelper/utils.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/kservehelper.egg-info/PKG-INFO` & `kservehelper-1.2.3/kservehelper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kservehelper
-Version: 1.2.2
+Version: 1.2.3
 Summary: A KServe Model Wrapper
 Home-page: https://github.com/yangwenz/kserve-helper
 Author: Wenzhuo Yang
 License: 3-Clause BSD
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Requires-Dist: kserve==0.10.2
```

### Comparing `kservehelper-1.2.2/kservehelper.egg-info/SOURCES.txt` & `kservehelper-1.2.3/kservehelper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/setup.py` & `kservehelper-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="kservehelper",
-    version="1.2.2",
+    version="1.2.3",
     author="Wenzhuo Yang",
     description="A KServe Model Wrapper",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/yangwenz/kserve-helper",
     license="3-Clause BSD",
     packages=find_namespace_packages(include="kservehelper.*"),
```

### Comparing `kservehelper-1.2.2/tests/test_batch_inputs.py` & `kservehelper-1.2.3/tests/test_batch_inputs.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/tests/test_cache.py` & `kservehelper-1.2.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/tests/test_model_cache.py` & `kservehelper-1.2.3/tests/test_model_cache.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/tests/test_predict.py` & `kservehelper-1.2.3/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/tests/test_s3.py` & `kservehelper-1.2.3/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/tests/test_transform.py` & `kservehelper-1.2.3/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.2/tests/test_upload.py` & `kservehelper-1.2.3/tests/test_upload.py`

 * *Files identical despite different names*

