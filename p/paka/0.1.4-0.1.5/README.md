# Comparing `tmp/paka-0.1.4.tar.gz` & `tmp/paka-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paka-0.1.4.tar", max compression
+gzip compressed data, was "paka-0.1.5.tar", max compression
```

## Comparing `paka-0.1.4.tar` & `paka-0.1.5.tar`

### file list

```diff
@@ -1,64 +1,65 @@
--rw-r--r--   0        0        0     1072 2024-04-19 04:36:42.330546 paka-0.1.4/LICENSE
--rw-r--r--   0        0        0     4570 2024-04-19 04:36:42.330546 paka-0.1.4/README.md
--rw-r--r--   0        0        0      153 2024-04-19 04:36:42.334546 paka-0.1.4/paka/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/__init__.py
--rw-r--r--   0        0        0     1608 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/__main__.py
--rw-r--r--   0        0        0     1141 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/build.py
--rw-r--r--   0        0        0     3891 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/cluster.py
--rw-r--r--   0        0        0     6726 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/function.py
--rw-r--r--   0        0        0     5910 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/job.py
--rw-r--r--   0        0        0      427 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/kubeconfig.py
--rw-r--r--   0        0        0     2233 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/model_group.py
--rw-r--r--   0        0        0     3188 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/run.py
--rw-r--r--   0        0        0     8815 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/utils.py
--rw-r--r--   0        0        0        0 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/__init__.py
--rw-r--r--   0        0        0     1037 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/cloudwatch.py
--rw-r--r--   0        0        0     3113 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/cluster_autoscaler.py
--rw-r--r--   0        0        0      722 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/container_registry.py
--rw-r--r--   0        0        0     2521 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/ebs_csi_driver.py
--rw-r--r--   0        0        0    12154 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/eks.py
--rw-r--r--   0        0        0     1468 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/elb.py
--rw-r--r--   0        0        0      725 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/object_store.py
--rw-r--r--   0        0        0     4078 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/service_account.py
--rw-r--r--   0        0        0     1932 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/utils.py
--rw-r--r--   0        0        0     4643 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/fluentbit.py
--rw-r--r--   0        0        0     1228 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/keda.py
--rw-r--r--   0        0        0     4956 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/knative.py
--rw-r--r--   0        0        0        0 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/manager/__init__.py
--rw-r--r--   0        0        0     1210 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/manager/aws.py
--rw-r--r--   0        0        0     2773 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/manager/base.py
--rw-r--r--   0        0        0      879 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/namespace.py
--rw-r--r--   0        0        0     3414 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/nvidia_device_plugin.py
--rw-r--r--   0        0        0     4273 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/prometheus.py
--rw-r--r--   0        0        0     4000 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/qdrant.py
--rw-r--r--   0        0        0     2325 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/redis.py
--rw-r--r--   0        0        0      935 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/zipkin.py
--rw-r--r--   0        0        0    15395 2024-04-19 04:36:42.334546 paka-0.1.4/paka/config.py
--rw-r--r--   0        0        0      115 2024-04-19 04:36:42.334546 paka-0.1.4/paka/constants.py
--rw-r--r--   0        0        0     3015 2024-04-19 04:36:42.334546 paka-0.1.4/paka/container/ecr.py
--rw-r--r--   0        0        0     2374 2024-04-19 04:36:42.334546 paka-0.1.4/paka/container/pack.py
--rw-r--r--   0        0        0    19188 2024-04-19 04:36:42.334546 paka-0.1.4/paka/k8s.py
--rw-r--r--   0        0        0        0 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/function/__init__.py
--rw-r--r--   0        0        0     5742 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/function/service.py
--rw-r--r--   0        0        0        0 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/job/__init__.py
--rw-r--r--   0        0        0     2342 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/job/autoscaler.py
--rw-r--r--   0        0        0     4142 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/job/worker.py
--rw-r--r--   0        0        0        0 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/model_group/__init__.py
--rw-r--r--   0        0        0     2048 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/model_group/ingress.py
--rw-r--r--   0        0        0      131 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/model_group/manifest.py
--rw-r--r--   0        0        0    10074 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/model_group/model.py
--rw-r--r--   0        0        0    17498 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/model_group/service.py
--rw-r--r--   0        0        0     1105 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/model_group/supported_models.py
--rw-r--r--   0        0        0      761 2024-04-19 04:36:42.334546 paka-0.1.4/paka/logger.py
--rw-r--r--   0        0        0        0 2024-04-19 04:36:42.334546 paka-0.1.4/paka/model/__init__.py
--rw-r--r--   0        0        0     3188 2024-04-19 04:36:42.334546 paka-0.1.4/paka/model/base_model.py
--rw-r--r--   0        0        0     2473 2024-04-19 04:36:42.334546 paka-0.1.4/paka/model/hf_model.py
--rw-r--r--   0        0        0     1485 2024-04-19 04:36:42.334546 paka-0.1.4/paka/model/http_model.py
--rw-r--r--   0        0        0     1648 2024-04-19 04:36:42.334546 paka-0.1.4/paka/model/manifest.py
--rw-r--r--   0        0        0     2565 2024-04-19 04:36:42.334546 paka-0.1.4/paka/model/progress_bar.py
--rw-r--r--   0        0        0     2671 2024-04-19 04:36:42.334546 paka-0.1.4/paka/model/settings.py
--rw-r--r--   0        0        0     9467 2024-04-19 04:36:42.334546 paka-0.1.4/paka/model/store.py
--rw-r--r--   0        0        0     9786 2024-04-19 04:36:42.334546 paka-0.1.4/paka/utils.py
--rw-r--r--   0        0        0     1456 2024-04-19 04:36:42.334546 paka-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5816 1970-01-01 00:00:00.000000 paka-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-25 22:57:30.021339 paka-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4570 2024-04-25 22:57:30.021339 paka-0.1.5/README.md
+-rw-r--r--   0        0        0      153 2024-04-25 22:57:30.025339 paka-0.1.5/paka/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/__init__.py
+-rw-r--r--   0        0        0     1608 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/__main__.py
+-rw-r--r--   0        0        0     1141 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/build.py
+-rw-r--r--   0        0        0     3891 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/cluster.py
+-rw-r--r--   0        0        0     6726 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/function.py
+-rw-r--r--   0        0        0     5910 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/job.py
+-rw-r--r--   0        0        0      427 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/kubeconfig.py
+-rw-r--r--   0        0        0     1943 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/model_group.py
+-rw-r--r--   0        0        0     3188 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/run.py
+-rw-r--r--   0        0        0     8815 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/cloudwatch.py
+-rw-r--r--   0        0        0     3113 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/cluster_autoscaler.py
+-rw-r--r--   0        0        0      722 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/container_registry.py
+-rw-r--r--   0        0        0     2521 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/ebs_csi_driver.py
+-rw-r--r--   0        0        0    12154 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/eks.py
+-rw-r--r--   0        0        0     1468 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/elb.py
+-rw-r--r--   0        0        0      725 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/object_store.py
+-rw-r--r--   0        0        0     4078 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/service_account.py
+-rw-r--r--   0        0        0     1932 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/utils.py
+-rw-r--r--   0        0        0     4643 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/fluentbit.py
+-rw-r--r--   0        0        0     1228 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/keda.py
+-rw-r--r--   0        0        0     4956 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/knative.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/manager/__init__.py
+-rw-r--r--   0        0        0     1210 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/manager/aws.py
+-rw-r--r--   0        0        0     2686 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/manager/base.py
+-rw-r--r--   0        0        0      879 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/namespace.py
+-rw-r--r--   0        0        0     3414 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/nvidia_device_plugin.py
+-rw-r--r--   0        0        0     4273 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/prometheus.py
+-rw-r--r--   0        0        0     4000 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/qdrant.py
+-rw-r--r--   0        0        0     2325 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/redis.py
+-rw-r--r--   0        0        0      935 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/zipkin.py
+-rw-r--r--   0        0        0    16434 2024-04-25 22:57:30.025339 paka-0.1.5/paka/config.py
+-rw-r--r--   0        0        0      115 2024-04-25 22:57:30.025339 paka-0.1.5/paka/constants.py
+-rw-r--r--   0        0        0     3015 2024-04-25 22:57:30.025339 paka-0.1.5/paka/container/ecr.py
+-rw-r--r--   0        0        0     2374 2024-04-25 22:57:30.025339 paka-0.1.5/paka/container/pack.py
+-rw-r--r--   0        0        0    19188 2024-04-25 22:57:30.025339 paka-0.1.5/paka/k8s.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:57:30.025339 paka-0.1.5/paka/kube_resources/function/__init__.py
+-rw-r--r--   0        0        0     5742 2024-04-25 22:57:30.025339 paka-0.1.5/paka/kube_resources/function/service.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:57:30.025339 paka-0.1.5/paka/kube_resources/job/__init__.py
+-rw-r--r--   0        0        0     2342 2024-04-25 22:57:30.025339 paka-0.1.5/paka/kube_resources/job/autoscaler.py
+-rw-r--r--   0        0        0     4142 2024-04-25 22:57:30.025339 paka-0.1.5/paka/kube_resources/job/worker.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:57:30.025339 paka-0.1.5/paka/kube_resources/model_group/__init__.py
+-rw-r--r--   0        0        0     1358 2024-04-25 22:57:30.025339 paka-0.1.5/paka/kube_resources/model_group/ingress.py
+-rw-r--r--   0        0        0      131 2024-04-25 22:57:30.029339 paka-0.1.5/paka/kube_resources/model_group/manifest.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:57:30.029339 paka-0.1.5/paka/kube_resources/model_group/runtime/__init__.py
+-rw-r--r--   0        0        0     4306 2024-04-25 22:57:30.029339 paka-0.1.5/paka/kube_resources/model_group/runtime/llama_cpp.py
+-rw-r--r--   0        0        0    17973 2024-04-25 22:57:30.029339 paka-0.1.5/paka/kube_resources/model_group/service.py
+-rw-r--r--   0        0        0      761 2024-04-25 22:57:30.029339 paka-0.1.5/paka/logger.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:57:30.029339 paka-0.1.5/paka/model/__init__.py
+-rw-r--r--   0        0        0     2946 2024-04-25 22:57:30.029339 paka-0.1.5/paka/model/base_model.py
+-rw-r--r--   0        0        0     2352 2024-04-25 22:57:30.029339 paka-0.1.5/paka/model/hf_model.py
+-rw-r--r--   0        0        0     1378 2024-04-25 22:57:30.029339 paka-0.1.5/paka/model/http_model.py
+-rw-r--r--   0        0        0     1444 2024-04-25 22:57:30.029339 paka-0.1.5/paka/model/manifest.py
+-rw-r--r--   0        0        0     2565 2024-04-25 22:57:30.029339 paka-0.1.5/paka/model/progress_bar.py
+-rw-r--r--   0        0        0     7621 2024-04-25 22:57:30.029339 paka-0.1.5/paka/model/registry.py
+-rw-r--r--   0        0        0     2086 2024-04-25 22:57:30.029339 paka-0.1.5/paka/model/settings.py
+-rw-r--r--   0        0        0    10074 2024-04-25 22:57:30.029339 paka-0.1.5/paka/model/store.py
+-rw-r--r--   0        0        0     9786 2024-04-25 22:57:30.029339 paka-0.1.5/paka/utils.py
+-rw-r--r--   0        0        0     1379 2024-04-25 22:57:30.029339 paka-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5816 1970-01-01 00:00:00.000000 paka-0.1.5/PKG-INFO
```

### Comparing `paka-0.1.4/LICENSE` & `paka-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/README.md` & `paka-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cli/__main__.py` & `paka-0.1.5/paka/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cli/build.py` & `paka-0.1.5/paka/cli/build.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cli/cluster.py` & `paka-0.1.5/paka/cli/cluster.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cli/function.py` & `paka-0.1.5/paka/cli/function.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cli/job.py` & `paka-0.1.5/paka/cli/job.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cli/model_group.py` & `paka-0.1.5/paka/cli/model_group.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,34 +4,24 @@
 
 import boto3
 import typer
 from kubernetes import client
 from tabulate import tabulate
 
 from paka.k8s import try_load_kubeconfig
-from paka.kube_resources.model_group.model import SUPPORTED_MODELS
 from paka.kube_resources.model_group.service import MODEL_PATH_PREFIX, filter_services
 from paka.logger import logger
 from paka.utils import read_current_cluster_data
 
 try_load_kubeconfig()
 
 model_group_app = typer.Typer()
 
 
 @model_group_app.command()
-def list_all_models() -> None:
-    """
-    List all supported models.
-    """
-    for model_name in SUPPORTED_MODELS:
-        logger.info(model_name)
-
-
-@model_group_app.command()
 def list_downloaded_models() -> None:
     """
     List all models that have been downloaded to the object store.
     """
     bucket = read_current_cluster_data("bucket")
     s3 = boto3.client("s3")
     response = s3.list_objects_v2(Bucket=bucket, Prefix=MODEL_PATH_PREFIX)
@@ -39,16 +29,15 @@
         unique_models: Set[str] = set()
         for obj in response["Contents"]:
             key = obj["Key"]
             if key.startswith(f"{MODEL_PATH_PREFIX}/"):
                 key = key[len(f"{MODEL_PATH_PREFIX}/") :]
 
             key = key.split("/")[0]
-            if key in SUPPORTED_MODELS:
-                unique_models.add(key)
+            unique_models.add(key)
 
         for key in unique_models:
             logger.info(key)
     else:
         logger.info("No models found.")
```

### Comparing `paka-0.1.4/paka/cli/run.py` & `paka-0.1.5/paka/cli/run.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cli/utils.py` & `paka-0.1.5/paka/cli/utils.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/aws/cloudwatch.py` & `paka-0.1.5/paka/cluster/aws/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/aws/cluster_autoscaler.py` & `paka-0.1.5/paka/cluster/aws/cluster_autoscaler.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/aws/container_registry.py` & `paka-0.1.5/paka/cluster/aws/container_registry.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/aws/ebs_csi_driver.py` & `paka-0.1.5/paka/cluster/aws/ebs_csi_driver.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/aws/eks.py` & `paka-0.1.5/paka/cluster/aws/eks.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/aws/elb.py` & `paka-0.1.5/paka/cluster/aws/elb.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/aws/object_store.py` & `paka-0.1.5/paka/cluster/aws/object_store.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/aws/service_account.py` & `paka-0.1.5/paka/cluster/aws/service_account.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/aws/utils.py` & `paka-0.1.5/paka/cluster/aws/utils.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/fluentbit.py` & `paka-0.1.5/paka/cluster/fluentbit.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/keda.py` & `paka-0.1.5/paka/cluster/keda.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/knative.py` & `paka-0.1.5/paka/cluster/knative.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/manager/aws.py` & `paka-0.1.5/paka/cluster/manager/aws.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/manager/base.py` & `paka-0.1.5/paka/cluster/manager/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 
 from abc import ABC, abstractmethod
 from typing import Any
 
 from pulumi import automation as auto
 
 from paka.config import CloudConfig, Config
-from paka.kube_resources.model_group.ingress import (
-    create_model_group_ingress,
-    create_model_vservice,
-)
+from paka.kube_resources.model_group.ingress import create_model_vservice
 from paka.kube_resources.model_group.service import create_model_group_service
 from paka.logger import logger
 from paka.utils import read_cluster_data, save_cluster_data
 
 STACK_NAME = "default"
 
 
@@ -69,15 +66,14 @@
         self._stack.up(on_output=logger.info)
 
         if self.config.modelGroups is None:
             return
 
         namespace = read_cluster_data(self.config.cluster.name, "namespace")
 
-        create_model_group_ingress(namespace)
         for model_group in self.config.modelGroups:
             create_model_group_service(namespace, self._orig_config, model_group)
             create_model_vservice(namespace, model_group.name)
 
     def destroy(self) -> None:
         logger.info("Destroying resources...")
         self._stack.destroy(on_output=logger.info)
```

### Comparing `paka-0.1.4/paka/cluster/namespace.py` & `paka-0.1.5/paka/cluster/namespace.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/nvidia_device_plugin.py` & `paka-0.1.5/paka/cluster/nvidia_device_plugin.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/prometheus.py` & `paka-0.1.5/paka/cluster/prometheus.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/qdrant.py` & `paka-0.1.5/paka/cluster/qdrant.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/redis.py` & `paka-0.1.5/paka/cluster/redis.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/cluster/zipkin.py` & `paka-0.1.5/paka/cluster/zipkin.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/config.py` & `paka-0.1.5/paka/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,28 +146,62 @@
         cls, values: Dict[str, Union[AwsGpuNode, GcpGpuNode]]
     ) -> Dict[str, Union[AwsGpuNode, GcpGpuNode]]:
         if values.get("awsGpu") and values.get("gcpGpu"):
             raise ValueError("At most one of awsGpu or gcpGpu can exist")
         return values
 
 
+class Runtime(BaseModel):
+    """
+    Represents a runtime for a model.
+
+    Attributes:
+        image (str): The Docker image to use for the runtime.
+        command (List[str], optional): The command to run in the Docker container.
+    """
+
+    image: str
+    command: Optional[List[str]] = None
+
+
+class Model(BaseModel):
+    """
+    Represents a model.
+
+    Attributes:
+        hfRepoId (str, optional): The HuggingFace repository ID for the model.
+        files (List[str], optional): The list of files to include from the repository. Defaults to all files ("*").
+        useModelStore (bool, optional): Whether to save the model to a model store, such as s3. Defaults to True.
+    """
+
+    hfRepoId: Optional[str] = None
+    files: List[str] = ["*"]
+
+    useModelStore: bool = True
+
+
 class ModelGroup(BaseModel):
     """
     Represents a group of VMs that serve the inference for a specific type of model.
 
     Attributes:
         name (str): The name of the model group.
         minInstances (int): The minimum number of instances to provision.
         maxInstances (int): The maximum number of instances to provision.
+        model (Optional[Model]): The model to deploy in the model group. If None, runtime image is responsible for loading the model.
+        runtime (Runtime): The runtime for the model group.
     """
 
     name: str
     minInstances: int
     maxInstances: int
 
+    model: Optional[Model] = None
+    runtime: Runtime
+
     @model_validator(mode="before")
     def check_instances_num(cls, values: Dict[str, int]) -> Dict[str, int]:
         min_instances, max_instances = values.get("minInstances"), values.get(
             "maxInstances"
         )
         if min_instances and max_instances and max_instances < min_instances:
             raise ValueError(
```

### Comparing `paka-0.1.4/paka/container/ecr.py` & `paka-0.1.5/paka/container/ecr.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/container/pack.py` & `paka-0.1.5/paka/container/pack.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/k8s.py` & `paka-0.1.5/paka/k8s.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/kube_resources/function/service.py` & `paka-0.1.5/paka/kube_resources/function/service.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/kube_resources/job/autoscaler.py` & `paka-0.1.5/paka/kube_resources/job/autoscaler.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/kube_resources/job/worker.py` & `paka-0.1.5/paka/kube_resources/job/worker.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/kube_resources/model_group/model.py` & `paka-0.1.5/paka/model/store.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,283 +1,320 @@
 from __future__ import annotations
 
 import concurrent.futures
+import functools
 import hashlib
-from typing import TYPE_CHECKING, Any, Dict, List
+import re
+from abc import ABC, abstractmethod
+from io import IOBase
+from typing import Any, Callable, Dict, List, TypeVar, Union, cast
 
 import boto3
 import requests
 from botocore.client import Config
 from botocore.exceptions import ClientError
+from typing_extensions import TypeAlias
 
-from paka.kube_resources.model_group.manifest import Manifest
-from paka.kube_resources.model_group.supported_models import SUPPORTED_MODELS
 from paka.logger import logger
-from paka.utils import read_current_cluster_data, to_yaml
-
-if TYPE_CHECKING:
-    from mypy_boto3_s3.client import S3Client
+from paka.model.progress_bar import NullProgressBar, ProgressBar
+from paka.utils import read_current_cluster_data
 
 MODEL_PATH_PREFIX = "models"
 
+StreamLike: TypeAlias = Union[requests.Response, IOBase]
 
-def delete_s3_file(bucket_name: str, s3_file_name: str) -> None:
-    s3 = boto3.client("s3")
-    if s3_file_exists(bucket_name, s3_file_name):
-        s3.delete_object(Bucket=bucket_name, Key=s3_file_name)
-        logger.info(f"{s3_file_name} deleted.")
-    else:
-        logger.info(f"{s3_file_name} not found.")
-
-
-def s3_file_exists(bucket_name: str, s3_file_name: str) -> bool:
-    s3 = boto3.client("s3")
-    try:
-        s3.head_object(Bucket=bucket_name, Key=s3_file_name)
-        return True
-    except ClientError as e:
-        if e.response["Error"]["Code"] == "404":
-            return False
-        else:
-            raise  # some other error occurred
+T = TypeVar("T", bound=Callable[..., Any])
 
 
-def s3_file_prefix_exists(bucket_name: str, s3_file_name: str) -> bool:
-    s3 = boto3.resource("s3")
-    bucket = s3.Bucket(bucket_name)
-    return any(bucket.objects.filter(Prefix=s3_file_name))
-
-
-def save_string_to_s3(bucket_name: str, file_name: str, data: str) -> None:
-    s3 = boto3.resource("s3")
-    s3.Object(bucket_name, file_name).put(Body=data)
-
-
-def upload_part(
-    s3: "S3Client",
-    bucket_name: str,
-    s3_file_name: str,
-    upload_id: str,
-    part_number: int,
-    chunk: bytes,
-) -> Dict[str, Any]:
-    part = s3.upload_part(
-        Body=chunk,
-        Bucket=bucket_name,
-        Key=s3_file_name,
-        UploadId=upload_id,
-        PartNumber=part_number,
-    )
-    return {"PartNumber": part_number, "ETag": part["ETag"]}
-
-
-def download_file_to_s3(
-    url: str,
-    bucket_name: str,
-    s3_file_name: str,
-    chunk_size: int = 5 * 1024 * 1024,
-    max_parallel_uploads: int = 20,
-) -> str:
-    """
-    Downloads a file from a URL and uploads it to an S3 bucket in chunks.
+def resolve_path(func: T) -> T:
+    @functools.wraps(func)
+    def wrapper(self: Any, path: str, *args: Any, **kwargs: Any) -> Any:
+        resolved_path = (
+            f"{MODEL_PATH_PREFIX}/{path}"
+            if not path.startswith(f"{MODEL_PATH_PREFIX}/")
+            else path
+        )
+        return func(self, resolved_path, *args, **kwargs)
 
-    This function downloads a file from the specified URL and uploads it to the specified S3 bucket.
-    The file is uploaded in chunks of the specified size. The function uses a ThreadPoolExecutor to
-    upload the chunks in parallel, with the specified maximum number of parallel uploads.
-
-    The function calculates the SHA256 hash of the file while it is being downloaded and uploaded.
-    If the upload is successful, the function returns the SHA256 hash.
-
-    If an error occurs during the download or upload, the function logs the error and raises an exception.
-    If an error occurs during the upload, the function aborts the multipart upload.
-
-    Args:
-        url (str): The URL to download the file from.
-        bucket_name (str): The name of the S3 bucket to upload the file to.
-        s3_file_name (str): The name to give to the file in the S3 bucket.
-        chunk_size (int, optional): The size of the chunks to upload. Defaults to 5 * 1024 * 1024.
-        max_parallel_uploads (int, optional): The maximum number of parallel uploads. Defaults to 20.
+    return cast(T, wrapper)
 
-    Raises:
-        Exception: If an error occurs during the download or upload.
 
-    Returns:
-        str: The SHA256 hash of the file.
-    """
+class ModelStore(ABC):
+    @abstractmethod
+    def save_stream(
+        self,
+        path: str,
+        stream: StreamLike,
+        total_size: int,
+        sha256: str = "",
+    ) -> None:
+        pass
 
-    s3 = boto3.client("s3", config=Config(signature_version="s3v4"))
-    upload_id = None
-    upload_completed = False
-
-    try:
-        with requests.get(url, stream=True) as response:
-            if response.status_code == 200:
-                sha256 = hashlib.sha256()
-                total_size = int(response.headers.get("content-length", 0))
-                processed_size = 0
+    @abstractmethod
+    def save(self, path: str, data: bytes) -> None:
+        pass
 
-                upload = s3.create_multipart_upload(
-                    Bucket=bucket_name, Key=s3_file_name
-                )
-                upload_id = upload["UploadId"]
-                parts = []
+    @abstractmethod
+    def file_exists(self, path: str, prefix_match: bool = False) -> bool:
+        pass
 
-                with concurrent.futures.ThreadPoolExecutor(
-                    max_workers=max_parallel_uploads
-                ) as executor:
-                    futures: List[concurrent.futures.Future] = []
-                    part_number = 1
-
-                    for chunk in response.iter_content(chunk_size=chunk_size):
-                        sha256.update(chunk)
-                        while len(futures) >= max_parallel_uploads:
-                            # Wait for one of the uploads to complete
-                            done, _ = concurrent.futures.wait(
-                                futures, return_when=concurrent.futures.FIRST_COMPLETED
-                            )
-                            for future in done:
-                                parts.append(future.result())
-                                futures.remove(future)
-
-                        # Submit new chunk for upload
-                        future = executor.submit(
-                            upload_part,
-                            s3,
-                            bucket_name,
-                            s3_file_name,
-                            upload_id,
-                            part_number,
-                            chunk,
-                        )
-                        futures.append(future)
-                        part_number += 1
-                        processed_size += len(chunk)
-                        progress = (processed_size / total_size) * 100
-                        print(f"Progress: {progress:.2f}%", end="\r")
-
-                    # Wait for all remaining uploads to complete
-                    for future in concurrent.futures.as_completed(futures):
-                        parts.append(future.result())
-
-                parts.sort(key=lambda part: part["PartNumber"])
-                s3.complete_multipart_upload(
-                    Bucket=bucket_name,
-                    Key=s3_file_name,
-                    UploadId=upload_id,
-                    MultipartUpload={"Parts": parts},
-                )
+    @abstractmethod
+    def delete_file(self, path: str) -> None:
+        pass
 
-                upload_completed = True
-                logger.info(f"File uploaded to S3: {s3_file_name}")
-                sha256_value = sha256.hexdigest()
-                logger.info(f"SHA256 hash of the file: {sha256_value}")
-                return sha256_value
-            else:
-                error_message = f"Unable to download the file. HTTP Status Code: {response.status_code}"
-                logger.error(error_message)
-                raise Exception(error_message)
-
-    except Exception as e:
-        logger.error(f"An error occurred: {str(e)}")
-        raise
-
-    finally:
-        if upload_id is not None and not upload_completed:
-            # If an error occurred and upload was not completed
-            s3.abort_multipart_upload(
-                Bucket=bucket_name, Key=s3_file_name, UploadId=upload_id
-            )
+    @abstractmethod
+    def glob(self, path_pattern: str) -> List[str]:
+        pass
 
 
-def download_model(name: str) -> None:
+class S3ModelStore(ModelStore):
     """
-    Downloads a machine learning model from a URL and uploads it to an S3 bucket.
-
-    This function checks if the model is supported and if it already exists in the S3 bucket.
-    If the model is supported and does not exist, the function downloads the model from the URL
-    and uploads it to the S3 bucket. The function also saves a manifest file in the S3 bucket
-    with metadata about the model.
-
-    If the SHA256 hash of the downloaded file does not match the expected hash, the function
-    deletes the file from the S3 bucket and raises an exception.
+    A store for storing models in S3.
 
-    Args:
-        name (str): The name of the model to download.
-
-    Raises:
-        Exception: If the model is not supported or if the SHA256 hash of the downloaded file does not match.
-
-    Returns:
-        None
+    This class provides methods for saving and retrieving models
+    from an S3 bucket.
     """
 
-    if name not in SUPPORTED_MODELS:
-        logger.error(
-            f"Model {name} is not supported."
-            f"Available models are: {', '.join(SUPPORTED_MODELS.keys())}"
-        )
-        raise Exception(f"Model {name} is not supported.")
-
-    model = SUPPORTED_MODELS[name]
-
-    logger.info(f"Downloading model from {model.url}...")
-    # Get the model name from the URL
-    model_file_name = model.url.split("/")[-1]
-    model_path = f"{MODEL_PATH_PREFIX}/{name}"
+    progress_bar: Union[ProgressBar, NullProgressBar]
 
-    full_model_file_path = f"{model_path}/{model_file_name}"
-    bucket = read_current_cluster_data("bucket")
+    def __init__(
+        self,
+        s3_chunk_size: int = 8 * 1024 * 1024,
+        s3_max_concurrency: int = 20,
+        with_progress_bar: bool = True,
+    ) -> None:
+        # s3 bucket
+        self.s3_bucket = read_current_cluster_data("bucket")
+        self.s3_chunk_size = s3_chunk_size
+        self.s3_max_concurrency = s3_max_concurrency
+        self.s3 = boto3.client("s3", config=Config(signature_version="s3v4"))
+        self.with_progress_bar = with_progress_bar
 
-    if s3_file_prefix_exists(bucket, f"{model_path}/"):
-        logger.info(f"Model {name} already exists.")
-        return
-
-    sha256 = download_file_to_s3(model.url, bucket, full_model_file_path)
-    if sha256 != model.sha256:
-        logger.error(f"SHA256 hash of the downloaded file does not match.")
-        # Delete the file
-        delete_s3_file(bucket, full_model_file_path)
-        raise Exception(f"SHA256 hash of the downloaded file does not match.")
+        if with_progress_bar:
+            self.progress_bar = ProgressBar("Saving model(s) to S3")
+        else:
+            self.progress_bar = NullProgressBar()
 
-    # Save model manifest
-    manifest = Manifest(
-        name=name,
-        sha256=model.sha256,
-        url=model.url,
-        type="gguf",  # TODO: hard-coded for now
-        file=model_file_name,
-    )
+    @resolve_path
+    def save(self, path: str, data: bytes) -> None:
+        s3 = boto3.resource("s3")
+        s3.Object(self.s3_bucket, path).put(Body=data)
+
+    @resolve_path
+    def save_stream(
+        self,
+        path: str,
+        stream: StreamLike,
+        total_size: int,
+        sha256: str = "",
+    ) -> None:
+        """
+        Downloads a single file from a URL.
+
+        Args:
+            url (str): The URL of the file to download.
+            sha256 (str, optional): The expected SHA256 hash of the downloaded file.
+
+        Raises:
+            Exception: If the SHA256 hash of the downloaded file does not match the expected value.
+        """
+        self.progress_bar.create_progress_bar(0)
+
+        self.progress_bar.update_progress_bar(path, total_size)
+
+        try:
+            if self.file_exists(path):
+                self.progress_bar.advance_progress_bar(path, total_size)
+                return
+
+            sha256_value = self._upload_to_s3(stream, path)
+            if sha256 and sha256 != sha256_value:
+                message = f"SHA256 hash of the downloaded file does not match the expected value for {path}"
+                # Log the error message so that users know why the file was deleted
+                logger.error(message)
+                self.delete_file(path)
+
+                raise Exception(message)
+
+            if not self.with_progress_bar:
+                logger.info(f"Model file {path} is saved successfully.")
+            self.progress_bar.advance_progress_bar(path, total_size)
+        except Exception:
+            self.progress_bar.close_progress_bar()
+            raise
+
+    def _upload_to_s3(
+        self,
+        stream: StreamLike,
+        s3_file_name: str,
+    ) -> str:
+        """
+        Uploads a single file to S3.
+
+        Args:
+            response (requests.Response | FileStream): The response object from the file download or the file stream object.
+            s3_file_name (str): The name of the file in S3.
+
+        Returns:
+            str: The SHA256 hash of the uploaded file.
+        """
+        upload_id = None
+        upload_completed = False
+        try:
+            self.progress_bar.set_postfix_str(s3_file_name)
+
+            sha256 = hashlib.sha256()
+            processed_size = 0
+            parts = []
 
-    manifest_yaml = to_yaml(manifest.model_dump(exclude_none=True))
-    save_string_to_s3(bucket, f"{model_path}/manifest.yaml", manifest_yaml)
+            upload = self.s3.create_multipart_upload(
+                Bucket=self.s3_bucket, Key=s3_file_name
+            )
+            upload_id = upload["UploadId"]
 
-    logger.info(f"Model {name} downloaded successfully.")
+            with concurrent.futures.ThreadPoolExecutor(
+                max_workers=self.s3_max_concurrency
+            ) as executor:
+                futures: List[concurrent.futures.Future] = []
+                part_number = 1
+
+                if isinstance(stream, requests.Response):
+                    chunks = stream.iter_content(chunk_size=self.s3_chunk_size)
+                else:
+                    response_io = cast(IOBase, stream)
+                    chunks = iter(lambda: response_io.read(self.s3_chunk_size), b"")
+
+                for chunk in chunks:
+                    sha256.update(chunk)
+                    while len(futures) >= self.s3_max_concurrency:
+                        done, _ = concurrent.futures.wait(
+                            futures, return_when=concurrent.futures.FIRST_COMPLETED
+                        )
+                        for future in done:
+                            parts.append(future.result())
+                            futures.remove(future)
+
+                    future = executor.submit(
+                        self._upload_part,
+                        s3_file_name,
+                        upload_id,
+                        part_number,
+                        chunk,
+                    )
+                    futures.append(future)
+                    part_number += 1
+                    processed_size += len(chunk)
+                    self.progress_bar.advance_progress_bar(s3_file_name, processed_size)
+
+                for future in concurrent.futures.as_completed(futures):
+                    parts.append(future.result())
+
+            parts.sort(key=lambda part: part["PartNumber"])
+            self.s3.complete_multipart_upload(
+                Bucket=self.s3_bucket,
+                Key=s3_file_name,
+                UploadId=upload_id,
+                MultipartUpload={"Parts": parts},
+            )
+            upload_completed = True
 
+            sha256_value = sha256.hexdigest()
+            return sha256_value
 
-def get_model_file_name(model_name: str) -> str:
-    """
-    Returns the file name of a machine learning model.
-
-    This function checks if the model is supported and if so, returns the file name of the model.
-    The file name is extracted from the model's URL.
+        except Exception as e:
+            logger.error(f"An error occurred in upload_to_s3: {str(e)}")
+            raise e
+
+        finally:
+            if upload_id is not None and not upload_completed:
+                self.s3.abort_multipart_upload(
+                    Bucket=self.s3_bucket, Key=s3_file_name, UploadId=upload_id
+                )
 
-    Args:
-        model_name (str): The name of the model.
+    def _upload_part(
+        self,
+        s3_file_name: str,
+        upload_id: str,
+        part_number: int,
+        chunk: bytes,
+    ) -> Dict[str, Any]:
+        """
+        Uploads a part of a file to S3.
+
+        Args:
+            s3_file_name (str): The name of the file in S3.
+            upload_id (str): The upload ID of the multipart upload.
+            part_number (int): The part number of the chunk being uploaded.
+            chunk (bytes): The chunk of data to upload.
+
+        Returns:
+            dict: A dictionary containing the part number and the ETag of the uploaded part.
+        """
+        part = self.s3.upload_part(
+            Body=chunk,
+            Bucket=self.s3_bucket,
+            Key=s3_file_name,
+            UploadId=upload_id,
+            PartNumber=part_number,
+        )
+        return {"PartNumber": part_number, "ETag": part["ETag"]}
 
-    Raises:
-        Exception: If the model is not supported.
+    @resolve_path
+    def file_exists(self, path: str, prefix_match: bool = False) -> bool:
+        """
+        Checks if a file exists in the S3 bucket.
+
+        Args:
+            path (str): The path of the file in the S3 bucket.
+            prefix_match (bool, optional): If True, checks if any file with the given path prefix exists.
+                Defaults to False.
+
+        Returns:
+            bool: True if the file exists, False otherwise.
+        """
+        if prefix_match:
+            s3 = boto3.resource("s3")
+            bucket = s3.Bucket(self.s3_bucket)
+            return any(bucket.objects.filter(Prefix=path))
+
+        try:
+            self.s3.head_object(Bucket=self.s3_bucket, Key=path)
+            return True
+        except ClientError as e:
+            if e.response["Error"]["Code"] == "404":
+                return False
+            else:
+                raise  # some other error occurred
 
-    Returns:
-        str: The file name of the model.
-    """
-    if model_name not in SUPPORTED_MODELS:
-        logger.error(
-            f"Model {model_name} is not supported."
-            f"Available models are: {', '.join(SUPPORTED_MODELS.keys())}"
-        )
-        raise Exception(f"Model {model_name} is not supported.")
+    @resolve_path
+    def delete_file(self, path: str) -> None:
+        """
+        Deletes the specified file from the S3 bucket.
+
+        Args:
+            path (str): The path of the file to be deleted.
+
+        Returns:
+            None
+        """
+        if self.file_exists(path):
+            self.s3.delete_object(Bucket=self.s3_bucket, Key=path)
+            logger.info(f"{path} deleted.")
+        else:
+            logger.info(f"{path} not found.")
 
-    model = SUPPORTED_MODELS[model_name]
+    @resolve_path
+    def glob(self, path_pattern: str) -> List[str]:
+        """
+        Lists all files in the S3 bucket that match the specified pattern.
+
+        Args:
+            path_pattern (str): The pattern to match.
+
+        Returns:
+            List[str]: A list of file paths that match the pattern.
+        """
+        s3 = boto3.resource("s3")
+        bucket = s3.Bucket(self.s3_bucket)
 
-    # Get the model name from the URL
-    model_name = model.url.split("/")[-1]
-    return model_name
+        pattern = re.compile(path_pattern)
+        return [obj.key for obj in bucket.objects.all() if pattern.match(obj.key)]
```

### Comparing `paka-0.1.4/paka/kube_resources/model_group/service.py` & `paka-0.1.5/paka/kube_resources/model_group/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,63 @@
 from __future__ import annotations
 
-from typing import Any, List, Optional
+from typing import Any, List, Optional, Tuple
 
 from kubernetes import client
 
 from paka.config import CloudConfig, CloudModelGroup, Config
 from paka.constants import ACCESS_ALL_SA
 from paka.k8s import CustomResource, apply_resource, try_load_kubeconfig
-from paka.kube_resources.model_group.model import MODEL_PATH_PREFIX, download_model
+from paka.kube_resources.model_group.runtime.llama_cpp import (
+    get_runtime_command_llama_cpp,
+    is_llama_cpp_image,
+)
+from paka.model.hf_model import HuggingFaceModel
+from paka.model.store import MODEL_PATH_PREFIX
 from paka.utils import kubify_name, read_cluster_data
 
-# `latest` will be stale because of the `IfNotPresent` policy
-# We hardcode the image here for now, we can make it configurable later
-LLAMA_CPP_PYTHON_IMAGE = "ghcr.io/abetlen/llama-cpp-python:latest"
+try_load_kubeconfig()
 
-LLAMA_CPP_PYTHON_CUDA = "jijunleng/llama-cpp-python-cuda:latest"
 
-try_load_kubeconfig()
+def get_runtime_command(model_group: CloudModelGroup, port: int) -> List[str]:
+    """
+    Gets the runtime command for a machine learning model group.
+
+    Args:
+        model_group (CloudModelGroup): The model group to get the runtime command for.
+
+    Returns:
+        List[str]: The runtime command.
+    """
+    command = []  # Default to the command in images
+    runtime = model_group.runtime
+    if runtime.command and not is_llama_cpp_image(runtime.image):
+        command = runtime.command
+
+    # If user did not provide a command, we need to provide a default command with heuristics.
+    if is_llama_cpp_image(runtime.image):
+        command = get_runtime_command_llama_cpp(model_group)
+
+        # Add or replace the port in the command
+        for i in range(len(command)):
+            if command[i] == "--port":
+                command[i + 1] = str(port)
+                break
+        else:
+            command.extend(["--port", str(port)])
+
+    return command
+
+
+def get_health_check_paths(model_group: CloudModelGroup) -> Tuple[str, str]:
+    # Return a tuple for ready and live probes
+    if is_llama_cpp_image(model_group.runtime.image):
+        return ("/health", "/health")
+
+    raise ValueError("Unsupported runtime image for health check paths.")
 
 
 def init_aws(config: CloudConfig, model_group: CloudModelGroup) -> client.V1Container:
     """
     Initializes an AWS container for downloading a model from S3.
 
     Args:
@@ -48,46 +85,18 @@
                 name="model-data",
                 mount_path="/data",
             )
         ],
     )
 
 
-def init_parse_manifest() -> client.V1Container:
-    """
-    Initializes a container for creating a symbolic link to the model file.
-
-    Returns:
-        client.V1Container: The initialized container for handling the manifest.
-    """
-    return client.V1Container(
-        name="init-parse-manifest",
-        image="busybox",
-        command=[
-            "sh",
-            "-c",
-            "model_type=$(cat /data/manifest.yaml | grep 'type' | cut -d ':' -f2 | tr -d ' '); "
-            'if [ "$model_type" != "gguf" ]; then echo \'Invalid model type\' && exit 1; fi; '
-            "model_file=$(cat /data/manifest.yaml | grep 'file' | cut -d ':' -f2 | tr -d ' '); "
-            "ln -s /data/${model_file} /data/my_model.gguf",
-        ],
-        volume_mounts=[
-            client.V1VolumeMount(
-                name="model-data",
-                mount_path="/data",
-            )
-        ],
-    )
-
-
 def create_pod(
     namespace: str,
     config: Config,
     model_group: CloudModelGroup,
-    runtime_image: str,
     port: int,
 ) -> client.V1Pod:
     """
     Creates a Kubernetes Pod for a machine learning model group.
 
     This function creates a Kubernetes Pod with the specified configuration. The Pod runs a container
     with the specified runtime image and exposes the specified port. The container runs a machine learning
@@ -105,52 +114,47 @@
 
     Returns:
         client.V1Pod: The created Pod.
     """
     if config.aws is None:
         raise ValueError("Only AWS is supported at this time")
 
+    ready_probe_path, live_probe_path = get_health_check_paths(model_group)
+
     container_args = {
         "name": f"{kubify_name(model_group.name)}",
-        "image": runtime_image,
+        "image": model_group.runtime.image,
+        "command": get_runtime_command(model_group, port),
         "volume_mounts": [
             client.V1VolumeMount(
                 name="model-data",
                 mount_path="/data",
             )
         ],
         "env": [
             client.V1EnvVar(
-                name="N_GPU_LAYERS",
-                # -1 means all layers are GPU layers, 0 means no GPU layers
-                value=("-1" if model_group.awsGpu else "0"),
-            ),
-            client.V1EnvVar(
-                name="MODEL",
-                value=f"/data/my_model.gguf",
-            ),
-            client.V1EnvVar(
                 name="PORT",
                 value=str(port),
             ),
         ],
+        "ports": [client.V1ContainerPort(container_port=port)],
         "readiness_probe": client.V1Probe(
             http_get=client.V1HTTPGetAction(
-                path="/v1/models",
+                path=ready_probe_path,
                 port=port,
             ),
             initial_delay_seconds=60,
             period_seconds=5,
             timeout_seconds=30,
             success_threshold=1,
             failure_threshold=5,
         ),
         "liveness_probe": client.V1Probe(
             http_get=client.V1HTTPGetAction(
-                path="/v1/models",
+                path=live_probe_path,
                 port=port,
             ),
             initial_delay_seconds=240,
             period_seconds=30,
             timeout_seconds=30,
             success_threshold=1,
             failure_threshold=5,
@@ -189,15 +193,20 @@
             service_account_name=ACCESS_ALL_SA,
             volumes=[
                 client.V1Volume(
                     name="model-data",
                     empty_dir=client.V1EmptyDirVolumeSource(),
                 )
             ],
-            init_containers=[init_aws(config.aws, model_group), init_parse_manifest()],
+            # Download models from s3 only when s3 is used as a model store
+            init_containers=(
+                [init_aws(config.aws, model_group)]
+                if model_group.model and model_group.model.useModelStore
+                else []
+            ),
             containers=[client.V1Container(**container_args)],
             tolerations=[
                 client.V1Toleration(
                     key="app",
                     value="model-group",
                     effect="NoSchedule",
                 ),
@@ -497,23 +506,29 @@
     Returns:
         None
     """
     if config.aws is None:
         raise ValueError("Only AWS is supported at this time")
 
     # Download the model to S3 first
-    download_model(model_group.name)
+    if model_group.model and model_group.model.useModelStore:
+        if model_group.model.hfRepoId:
+            model = HuggingFaceModel(
+                name=model_group.name,
+                repo_id=model_group.model.hfRepoId,
+                files=model_group.model.files,
+            )
+            model.save()
 
     port = 8000
 
     pod = create_pod(
         namespace,
         config,
         model_group,
-        (LLAMA_CPP_PYTHON_CUDA if model_group.awsGpu else LLAMA_CPP_PYTHON_IMAGE),
         port,
     )
 
     deployment = create_deployment(namespace, model_group, pod)
     apply_resource(deployment)
 
     svc = create_service(namespace, model_group, port)
```

### Comparing `paka-0.1.4/paka/logger.py` & `paka-0.1.5/paka/logger.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/model/base_model.py` & `paka-0.1.5/paka/model/base_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,28 +11,24 @@
 from paka.utils import read_current_cluster_data, to_yaml
 
 
 class BaseMLModel(ABC):
     def __init__(
         self,
         name: str,
-        inference_devices: List[str],
-        quantization: str,
-        runtime: str,
+        quantization: Optional[str],
         prompt_template_name: Optional[str],
         prompt_template_str: Optional[str],
         # Max concurrency for saving model streams
         concurrency: int = 1,
     ) -> None:
         self.name = name
         self.completed_files: List[Tuple[str, str]] = []
         self.settings = ModelSettings(
-            inference_devices=inference_devices,
             quantization=quantization,
-            runtime=runtime,
             prompt_template_name=prompt_template_name,
             prompt_template_str=prompt_template_str,
         )
 
         self.model_store = self.get_model_store()
         self.concurrency = concurrency
 
@@ -48,17 +44,15 @@
         if manifest is None:
             manifest = ModelManifest(
                 name=self.name,
                 files=[
                     ModelFile(name=name, sha256=sha256)
                     for (name, sha256) in self.completed_files
                 ],
-                inference_devices=self.settings.inference_devices,
                 quantization=self.settings.quantization,
-                runtime=self.settings.runtime,
                 prompt_template_name=self.settings.prompt_template_name,
                 prompt_template_str=self.settings.prompt_template_str,
             )
 
         model_store = self.get_model_store(with_progress_bar=False)
 
         manifest_yml = to_yaml(manifest.model_dump(exclude_none=True))
```

### Comparing `paka-0.1.4/paka/model/hf_model.py` & `paka-0.1.5/paka/model/hf_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,25 +13,21 @@
 
 class HuggingFaceModel(BaseMLModel):
     def __init__(
         self,
         name: str,
         repo_id: str,
         files: List[str],
-        inference_devices: List[str],
-        quantization: str,
-        runtime: str,
+        quantization: Optional[str] = None,
         prompt_template_name: Optional[str] = None,
         prompt_template_str: Optional[str] = None,
     ) -> None:
         super().__init__(
             name=name,
-            inference_devices=inference_devices,
             quantization=quantization,
-            runtime=runtime,
             prompt_template_name=prompt_template_name,
             prompt_template_str=prompt_template_str,
         )
         validate_repo_id(repo_id)
         self.repo_id: str = repo_id
         self.fs = HfFileSystem()
         self._files = files
```

### Comparing `paka-0.1.4/paka/model/http_model.py` & `paka-0.1.5/paka/model/http_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,25 +9,21 @@
 
 
 class HttpSourceModel(BaseMLModel):
     def __init__(
         self,
         name: str,
         urls: List[str],
-        inference_devices: List[str],
-        quantization: str,
-        runtime: str,
-        prompt_template_name: Optional[str],
-        prompt_template_str: Optional[str],
+        quantization: Optional[str] = None,
+        prompt_template_name: Optional[str] = None,
+        prompt_template_str: Optional[str] = None,
     ) -> None:
         super().__init__(
             name=name,
-            inference_devices=inference_devices,
             quantization=quantization,
-            runtime=runtime,
             prompt_template_name=prompt_template_name,
             prompt_template_str=prompt_template_str,
         )
         self.urls = urls
 
     def save(self) -> None:
         """
```

### Comparing `paka-0.1.4/paka/model/progress_bar.py` & `paka-0.1.5/paka/model/progress_bar.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/paka/model/settings.py` & `paka-0.1.5/paka/model/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,39 +2,29 @@
 
 from typing import List, Optional
 
 from pydantic import BaseModel, Field, field_validator
 
 
 class ModelSettings(BaseModel):
-    inference_devices: List[str] = Field(
-        description="The list of inference devices (cpu, gpu, tpu, etc) to use.",
-    )
-    quantization: str = Field(
-        description="The quantization method (GPTQ, AWQ, GGUF_Q4_0, etc) to use."
-    )
-    runtime: str = Field(
-        description="The runtime (llama.cpp, vLLM, pytorch, etc) to use."
+    quantization: Optional[str] = Field(
+        None, description="The quantization method (GPTQ, AWQ, GGUF_Q4_0, etc) to use."
     )
     prompt_template_name: Optional[str] = Field(
         None, description="The prompt template (chatml, llama-2, gemma, etc) to use."
     )
     prompt_template_str: Optional[str] = Field(
         None, description="The prompt template string to use."
     )
 
-    @field_validator("inference_devices")
-    def validate_inference_devices(cls, v: List[str]) -> List[str]:
-        valid_devices = ["cpu", "gpu"]
-        if not all(device in valid_devices for device in v):
-            raise ValueError("Invalid inference device")
-        return v
-
     @field_validator("quantization")
-    def validate_quantization(cls, v: str) -> str:
+    def validate_quantization(cls, v: Optional[str]) -> Optional[str]:
+        if v is None:
+            return v
+
         valid_methods = [
             "GPTQ",
             "AWQ",
             "GGUF_Q2_K",
             "GGUF_Q3_K_L",
             "GGUF_Q3_K_M",
             "GGUF_Q3_K_S",
@@ -42,26 +32,21 @@
             "GGUF_Q4_K_M",
             "GGUF_Q4_K_S",
             "GGUF_Q5_0",
             "GGUF_Q5_K_M",
             "GGUF_Q5_K_S",
             "GGUF_Q6_K",
             "GGUF_Q8_0",
+            "GGUF_fp16",
+            "GGUF_fp32",
         ]
         if v not in valid_methods:
             raise ValueError("Invalid quantization method")
         return v
 
-    @field_validator("runtime")
-    def validate_runtime(cls, v: str) -> str:
-        valid_runtimes = ["llama.cpp"]
-        if v not in valid_runtimes:
-            raise ValueError("Invalid runtime")
-        return v
-
     @field_validator("prompt_template_name")
     def validate_prompt_template_name(cls, v: str) -> str:
         valid_templates = [
             "chatml",
             "llama-2",
             "gemma",
             "alpaca",
@@ -79,11 +64,12 @@
             "mistrallite",
             "zephyr",
             "pygmalion",
             "mistral-instruct",
             "chatglm3",
             "openchat",
             "saiga",
+            "codellama",
         ]
         if v is not None and v not in valid_templates:
             raise ValueError("Invalid prompt template name")
         return v
```

### Comparing `paka-0.1.4/paka/utils.py` & `paka-0.1.5/paka/utils.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.4/pyproject.toml` & `paka-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paka"
-version = "0.1.4"
+version = "0.1.5"
 description = "LLMOps tool designed to simplify the deployment and management of large language model (LLM) applications"
 authors = ["Jijun Leng"]
 readme = "README.md"
 
 [tool.codespell]
 check-filenames = true
 
@@ -14,18 +14,15 @@
 check_untyped_defs = true
 plugins = "pydantic.mypy"
 
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
-filterwarnings = [
-  "ignore:pkg_resources is deprecated:DeprecationWarning",
-  "ignore:Waiting for.*:DeprecationWarning",
-]
+filterwarnings = ["ignore::DeprecationWarning"]
 
 [tool.poetry.scripts]
 paka = "paka.cli.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^2.7.0"
```

### Comparing `paka-0.1.4/PKG-INFO` & `paka-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paka
-Version: 0.1.4
+Version: 0.1.5
 Summary: LLMOps tool designed to simplify the deployment and management of large language model (LLM) applications
 Author: Jijun Leng
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

