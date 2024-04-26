# Comparing `tmp/rcds_umdcsec-0.1.5.tar.gz` & `tmp/rcds_umdcsec-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcds_umdcsec-0.1.5.tar", max compression
+gzip compressed data, was "rcds_umdcsec-0.1.6.tar", max compression
```

## Comparing `rcds_umdcsec-0.1.5.tar` & `rcds_umdcsec-0.1.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1476 2024-04-26 03:35:00.856037 rcds_umdcsec-0.1.5/LICENSE
--rw-r--r--   0        0        0     1751 2024-04-26 03:35:00.856037 rcds_umdcsec-0.1.5/README.rst
--rw-r--r--   0        0        0     1315 2024-04-26 06:17:20.186526 rcds_umdcsec-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      155 2024-04-26 03:35:00.856037 rcds_umdcsec-0.1.5/rcds/__init__.py
--rw-r--r--   0        0        0      262 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/backend/__init__.py
--rw-r--r--   0        0        0     1155 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/backend/backend.py
--rw-r--r--   0        0        0        0 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/backends/__init__.py
--rw-r--r--   0        0        0       44 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/backends/k8s/__init__.py
--rw-r--r--   0        0        0     4806 2024-04-26 05:03:43.987350 rcds_umdcsec-0.1.5/rcds/backends/k8s/backend.py
--rw-r--r--   0        0        0      890 2024-04-26 05:03:17.031263 rcds_umdcsec-0.1.5/rcds/backends/k8s/jinja.py
--rw-r--r--   0        0        0     5619 2024-04-26 05:22:44.418103 rcds_umdcsec-0.1.5/rcds/backends/k8s/manifests.py
--rw-r--r--   0        0        0     1433 2024-04-26 04:43:02.525214 rcds_umdcsec-0.1.5/rcds/backends/k8s/options.schema.yaml
--rw-r--r--   0        0        0      326 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/backends/k8s/templates/_helpers.jinja
--rw-r--r--   0        0        0     1819 2024-04-26 05:39:50.421352 rcds_umdcsec-0.1.5/rcds/backends/k8s/templates/deployment.yaml
--rw-r--r--   0        0        0      837 2024-04-26 06:16:55.563425 rcds_umdcsec-0.1.5/rcds/backends/k8s/templates/ingress.yaml
--rw-r--r--   0        0        0      201 2024-04-26 04:50:08.569142 rcds_umdcsec-0.1.5/rcds/backends/k8s/templates/namespace.yaml
--rw-r--r--   0        0        0      668 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/backends/k8s/templates/network-policy.yaml
--rw-r--r--   0        0        0      328 2024-04-26 05:08:10.325752 rcds_umdcsec-0.1.5/rcds/backends/k8s/templates/secret.yaml
--rw-r--r--   0        0        0     1024 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/backends/k8s/templates/service.yaml
--rw-r--r--   0        0        0       44 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/backends/rctf/__init__.py
--rw-r--r--   0        0        0     6168 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/backends/rctf/backend.py
--rw-r--r--   0        0        0      777 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/backends/rctf/options.schema.yaml
--rw-r--r--   0        0        0     2729 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/backends/rctf/rctf.py
--rw-r--r--   0        0        0      100 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/challenge/__init__.py
--rw-r--r--   0        0        0     5168 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/challenge/challenge.py
--rw-r--r--   0        0        0     9061 2024-04-26 04:07:03.029775 rcds_umdcsec-0.1.5/rcds/challenge/challenge.schema.yaml
--rw-r--r--   0        0        0     9335 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/challenge/config.py
--rw-r--r--   0        0        0     9434 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/challenge/docker.py
--rw-r--r--   0        0        0       40 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/cli/__init__.py
--rw-r--r--   0        0        0      143 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/cli/__main__.py
--rw-r--r--   0        0        0     1625 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/cli/deploy.py
--rw-r--r--   0        0        0      381 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/errors.py
--rw-r--r--   0        0        0       43 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/project/__init__.py
--rw-r--r--   0        0        0    12737 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/project/assets.py
--rw-r--r--   0        0        0     2983 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/project/config.py
--rw-r--r--   0        0        0     2819 2024-04-26 04:08:46.195757 rcds_umdcsec-0.1.5/rcds/project/project.py
--rw-r--r--   0        0        0     2233 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/project/rcds.schema.yaml
--rw-r--r--   0        0        0       64 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/py.typed
--rw-r--r--   0        0        0      155 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/util/__init__.py
--rw-r--r--   0        0        0      723 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/util/deep_merge.py
--rw-r--r--   0        0        0      832 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/util/find.py
--rw-r--r--   0        0        0      787 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/util/jsonschema.py
--rw-r--r--   0        0        0      847 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.5/rcds/util/load.py
--rw-r--r--   0        0        0     2932 1970-01-01 00:00:00.000000 rcds_umdcsec-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1476 2024-04-26 03:35:00.856037 rcds_umdcsec-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1751 2024-04-26 03:35:00.856037 rcds_umdcsec-0.1.6/README.rst
+-rw-r--r--   0        0        0     1315 2024-04-26 06:24:38.046115 rcds_umdcsec-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      155 2024-04-26 03:35:00.856037 rcds_umdcsec-0.1.6/rcds/__init__.py
+-rw-r--r--   0        0        0      262 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/backend/__init__.py
+-rw-r--r--   0        0        0     1155 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/backend/backend.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/backends/__init__.py
+-rw-r--r--   0        0        0       44 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/backends/k8s/__init__.py
+-rw-r--r--   0        0        0     4806 2024-04-26 05:03:43.987350 rcds_umdcsec-0.1.6/rcds/backends/k8s/backend.py
+-rw-r--r--   0        0        0      890 2024-04-26 05:03:17.031263 rcds_umdcsec-0.1.6/rcds/backends/k8s/jinja.py
+-rw-r--r--   0        0        0     5619 2024-04-26 05:22:44.418103 rcds_umdcsec-0.1.6/rcds/backends/k8s/manifests.py
+-rw-r--r--   0        0        0     1433 2024-04-26 04:43:02.525214 rcds_umdcsec-0.1.6/rcds/backends/k8s/options.schema.yaml
+-rw-r--r--   0        0        0      326 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/backends/k8s/templates/_helpers.jinja
+-rw-r--r--   0        0        0     1819 2024-04-26 05:39:50.421352 rcds_umdcsec-0.1.6/rcds/backends/k8s/templates/deployment.yaml
+-rw-r--r--   0        0        0      905 2024-04-26 06:24:04.466383 rcds_umdcsec-0.1.6/rcds/backends/k8s/templates/ingress.yaml
+-rw-r--r--   0        0        0      201 2024-04-26 04:50:08.569142 rcds_umdcsec-0.1.6/rcds/backends/k8s/templates/namespace.yaml
+-rw-r--r--   0        0        0      668 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/backends/k8s/templates/network-policy.yaml
+-rw-r--r--   0        0        0      328 2024-04-26 05:08:10.325752 rcds_umdcsec-0.1.6/rcds/backends/k8s/templates/secret.yaml
+-rw-r--r--   0        0        0     1024 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/backends/k8s/templates/service.yaml
+-rw-r--r--   0        0        0       44 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/backends/rctf/__init__.py
+-rw-r--r--   0        0        0     6168 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/backends/rctf/backend.py
+-rw-r--r--   0        0        0      777 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/backends/rctf/options.schema.yaml
+-rw-r--r--   0        0        0     2729 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/backends/rctf/rctf.py
+-rw-r--r--   0        0        0      100 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/challenge/__init__.py
+-rw-r--r--   0        0        0     5168 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/challenge/challenge.py
+-rw-r--r--   0        0        0     9061 2024-04-26 04:07:03.029775 rcds_umdcsec-0.1.6/rcds/challenge/challenge.schema.yaml
+-rw-r--r--   0        0        0     9335 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/challenge/config.py
+-rw-r--r--   0        0        0     9434 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/challenge/docker.py
+-rw-r--r--   0        0        0       40 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/cli/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/cli/__main__.py
+-rw-r--r--   0        0        0     1625 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/cli/deploy.py
+-rw-r--r--   0        0        0      381 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/errors.py
+-rw-r--r--   0        0        0       43 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/project/__init__.py
+-rw-r--r--   0        0        0    12737 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/project/assets.py
+-rw-r--r--   0        0        0     2983 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/project/config.py
+-rw-r--r--   0        0        0     2819 2024-04-26 04:08:46.195757 rcds_umdcsec-0.1.6/rcds/project/project.py
+-rw-r--r--   0        0        0     2233 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/project/rcds.schema.yaml
+-rw-r--r--   0        0        0       64 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/py.typed
+-rw-r--r--   0        0        0      155 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/util/__init__.py
+-rw-r--r--   0        0        0      723 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/util/deep_merge.py
+-rw-r--r--   0        0        0      832 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/util/find.py
+-rw-r--r--   0        0        0      787 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/util/jsonschema.py
+-rw-r--r--   0        0        0      847 2024-04-26 03:35:00.859370 rcds_umdcsec-0.1.6/rcds/util/load.py
+-rw-r--r--   0        0        0     2932 1970-01-01 00:00:00.000000 rcds_umdcsec-0.1.6/PKG-INFO
```

### Comparing `rcds_umdcsec-0.1.5/LICENSE` & `rcds_umdcsec-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/README.rst` & `rcds_umdcsec-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/pyproject.toml` & `rcds_umdcsec-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rcds-umdcsec"
-version = "0.1.5"
+version = "0.1.6"
 description = "An automated CTF challenge deployment tool"
 readme = "README.rst"
 authors = ["redpwn <contact@redpwn.net>"]
 homepage = "https://rcds.redpwn.net"
 repository = "https://github.com/redpwn/rCDS"
 license = "BSD-3-Clause"
 packages = [
```

### Comparing `rcds_umdcsec-0.1.5/rcds/backend/backend.py` & `rcds_umdcsec-0.1.6/rcds/backend/backend.py`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/backends/k8s/backend.py` & `rcds_umdcsec-0.1.6/rcds/backends/k8s/backend.py`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/backends/k8s/jinja.py` & `rcds_umdcsec-0.1.6/rcds/backends/k8s/jinja.py`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/backends/k8s/manifests.py` & `rcds_umdcsec-0.1.6/rcds/backends/k8s/manifests.py`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/backends/k8s/options.schema.yaml` & `rcds_umdcsec-0.1.6/rcds/backends/k8s/options.schema.yaml`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/backends/k8s/templates/deployment.yaml` & `rcds_umdcsec-0.1.6/rcds/backends/k8s/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/backends/k8s/templates/ingress.yaml` & `rcds_umdcsec-0.1.6/rcds/backends/k8s/templates/ingress.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -17,13 +17,16 @@
 spec:
   rules:
   {% for httpPort in httpPorts %}
     - host: {{ httpPort.http }}
       http:
         paths:
           - path: /
+            pathType: Prefix
             backend:
-              serviceName: {{ container.name }}
-              servicePort: {{ httpPort.target }}
+              service:
+                name: {{ container.name }}
+                port:
+                  number: {{ httpPort.target }}
   {% endfor %}
 {% endif %}
 {% endif %}
```

### Comparing `rcds_umdcsec-0.1.5/rcds/backends/k8s/templates/network-policy.yaml` & `rcds_umdcsec-0.1.6/rcds/backends/k8s/templates/network-policy.yaml`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/backends/k8s/templates/service.yaml` & `rcds_umdcsec-0.1.6/rcds/backends/k8s/templates/service.yaml`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/backends/rctf/backend.py` & `rcds_umdcsec-0.1.6/rcds/backends/rctf/backend.py`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/backends/rctf/options.schema.yaml` & `rcds_umdcsec-0.1.6/rcds/backends/rctf/options.schema.yaml`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/backends/rctf/rctf.py` & `rcds_umdcsec-0.1.6/rcds/backends/rctf/rctf.py`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/challenge/challenge.py` & `rcds_umdcsec-0.1.6/rcds/challenge/challenge.py`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/challenge/challenge.schema.yaml` & `rcds_umdcsec-0.1.6/rcds/challenge/challenge.schema.yaml`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/challenge/config.py` & `rcds_umdcsec-0.1.6/rcds/challenge/config.py`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/challenge/docker.py` & `rcds_umdcsec-0.1.6/rcds/challenge/docker.py`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/cli/deploy.py` & `rcds_umdcsec-0.1.6/rcds/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/project/assets.py` & `rcds_umdcsec-0.1.6/rcds/project/assets.py`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/project/config.py` & `rcds_umdcsec-0.1.6/rcds/project/config.py`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/project/project.py` & `rcds_umdcsec-0.1.6/rcds/project/project.py`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/project/rcds.schema.yaml` & `rcds_umdcsec-0.1.6/rcds/project/rcds.schema.yaml`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/util/deep_merge.py` & `rcds_umdcsec-0.1.6/rcds/util/deep_merge.py`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/util/find.py` & `rcds_umdcsec-0.1.6/rcds/util/find.py`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/util/jsonschema.py` & `rcds_umdcsec-0.1.6/rcds/util/jsonschema.py`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/rcds/util/load.py` & `rcds_umdcsec-0.1.6/rcds/util/load.py`

 * *Files identical despite different names*

### Comparing `rcds_umdcsec-0.1.5/PKG-INFO` & `rcds_umdcsec-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcds-umdcsec
-Version: 0.1.5
+Version: 0.1.6
 Summary: An automated CTF challenge deployment tool
 Home-page: https://rcds.redpwn.net
 License: BSD-3-Clause
 Author: redpwn
 Author-email: contact@redpwn.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

