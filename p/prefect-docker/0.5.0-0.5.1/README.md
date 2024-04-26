# Comparing `tmp/prefect_docker-0.5.0.tar.gz` & `tmp/prefect_docker-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_docker-0.5.0.tar", last modified: Thu Apr 25 19:20:11 2024, max compression
+gzip compressed data, was "prefect_docker-0.5.1.tar", last modified: Fri Apr 26 15:03:55 2024, max compression
```

## Comparing `prefect_docker-0.5.0.tar` & `prefect_docker-0.5.1.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:11.304209 prefect_docker-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-25 19:20:11.304209 prefect_docker-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:11.296209 prefect_docker-0.5.0/prefect_docker/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/prefect_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:10.000000 prefect_docker-0.5.0/prefect_docker/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/prefect_docker/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/prefect_docker/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:11.300209 prefect_docker-0.5.0/prefect_docker/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/prefect_docker/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/prefect_docker/deployments/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/prefect_docker/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/prefect_docker/images.py
--rw-r--r--   0 runner    (1001) docker     (127)    30166 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/prefect_docker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:11.300209 prefect_docker-0.5.0/prefect_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-25 19:20:11.000000 prefect_docker-0.5.0/prefect_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-25 19:20:11.000000 prefect_docker-0.5.0/prefect_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:11.000000 prefect_docker-0.5.0/prefect_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 19:20:11.000000 prefect_docker-0.5.0/prefect_docker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-25 19:20:11.000000 prefect_docker-0.5.0/prefect_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 19:20:11.000000 prefect_docker-0.5.0/prefect_docker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:11.304209 prefect_docker-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:11.300209 prefect_docker-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:11.300209 prefect_docker-0.5.0/tests/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/deployments/test_steps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:11.300209 prefect_docker-0.5.0/tests/test-project/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/test-project/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/test-project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/test_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    46168 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/test_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:55.648860 prefect_docker-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-26 15:03:55.648860 prefect_docker-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:55.644860 prefect_docker-0.5.1/prefect_docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/prefect_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:03:55.000000 prefect_docker-0.5.1/prefect_docker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/prefect_docker/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/prefect_docker/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:55.644860 prefect_docker-0.5.1/prefect_docker/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/prefect_docker/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/prefect_docker/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/prefect_docker/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/prefect_docker/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30166 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/prefect_docker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:55.648860 prefect_docker-0.5.1/prefect_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-26 15:03:55.000000 prefect_docker-0.5.1/prefect_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-26 15:03:55.000000 prefect_docker-0.5.1/prefect_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:03:55.000000 prefect_docker-0.5.1/prefect_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 15:03:55.000000 prefect_docker-0.5.1/prefect_docker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-26 15:03:55.000000 prefect_docker-0.5.1/prefect_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 15:03:55.000000 prefect_docker-0.5.1/prefect_docker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:03:55.648860 prefect_docker-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:55.644860 prefect_docker-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:55.644860 prefect_docker-0.5.1/tests/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/deployments/test_steps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:55.648860 prefect_docker-0.5.1/tests/test-project/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/test-project/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/test-project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/test_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46168 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/test_worker.py
```

### Comparing `prefect_docker-0.5.0/PKG-INFO` & `prefect_docker-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-docker
-Version: 0.5.0
+Version: 0.5.1
 Summary: Prefect integrations for interacting with Docker.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-docker
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: prefect>=2.13.5
 Requires-Dist: docker>=6.1.1
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
```

### Comparing `prefect_docker-0.5.0/README.md` & `prefect_docker-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.0/prefect_docker/containers.py` & `prefect_docker-0.5.1/prefect_docker/containers.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.0/prefect_docker/credentials.py` & `prefect_docker-0.5.1/prefect_docker/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.0/prefect_docker/deployments/steps.py` & `prefect_docker-0.5.1/prefect_docker/deployments/steps.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.0/prefect_docker/host.py` & `prefect_docker-0.5.1/prefect_docker/host.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.0/prefect_docker/images.py` & `prefect_docker-0.5.1/prefect_docker/images.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.0/prefect_docker/worker.py` & `prefect_docker-0.5.1/prefect_docker/worker.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.0/prefect_docker.egg-info/PKG-INFO` & `prefect_docker-0.5.1/prefect_docker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-docker
-Version: 0.5.0
+Version: 0.5.1
 Summary: Prefect integrations for interacting with Docker.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-docker
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: prefect>=2.13.5
 Requires-Dist: docker>=6.1.1
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
```

### Comparing `prefect_docker-0.5.0/prefect_docker.egg-info/SOURCES.txt` & `prefect_docker-0.5.1/prefect_docker.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 prefect_docker/__init__.py
 prefect_docker/_version.py
 prefect_docker/containers.py
 prefect_docker/credentials.py
 prefect_docker/host.py
```

### Comparing `prefect_docker-0.5.0/pyproject.toml` & `prefect_docker-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.0/tests/conftest.py` & `prefect_docker-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.0/tests/deployments/test_steps.py` & `prefect_docker-0.5.1/tests/deployments/test_steps.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.0/tests/test-project/flow.py` & `prefect_docker-0.5.1/tests/test-project/flow.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.0/tests/test_containers.py` & `prefect_docker-0.5.1/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.0/tests/test_host.py` & `prefect_docker-0.5.1/tests/test_host.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.0/tests/test_images.py` & `prefect_docker-0.5.1/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.0/tests/test_worker.py` & `prefect_docker-0.5.1/tests/test_worker.py`

 * *Files identical despite different names*

