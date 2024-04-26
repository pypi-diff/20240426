# Comparing `tmp/skypilot_nightly-1.0.0.dev20240424.tar.gz` & `tmp/skypilot_nightly-1.0.0.dev20240425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot_nightly-1.0.0.dev20240424.tar", last modified: Wed Apr 24 10:39:23 2024, max compression
+gzip compressed data, was "skypilot_nightly-1.0.0.dev20240425.tar", last modified: Thu Apr 25 10:38:08 2024, max compression
```

## Comparing `skypilot_nightly-1.0.0.dev20240424.tar` & `skypilot_nightly-1.0.0.dev20240425.tar`

### file list

```diff
@@ -1,338 +1,338 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.661096 skypilot_nightly-1.0.0.dev20240424/
--rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-24 10:39:23.661096 skypilot_nightly-1.0.0.dev20240424/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:39:23.661096 skypilot_nightly-1.0.0.dev20240424/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-24 10:39:20.000000 skypilot_nightly-1.0.0.dev20240424/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.597096 skypilot_nightly-1.0.0.dev20240424/sky/
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-24 10:39:23.000000 skypilot_nightly-1.0.0.dev20240424/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.597096 skypilot_nightly-1.0.0.dev20240424/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/adaptors/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/adaptors/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/adaptors/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/adaptors/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/adaptors/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    21410 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.601096 skypilot_nightly-1.0.0.dev20240424/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)   118820 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   223223 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.601096 skypilot_nightly-1.0.0.dev20240424/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.601096 skypilot_nightly-1.0.0.dev20240424/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    26440 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (127)   186846 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.605096 skypilot_nightly-1.0.0.dev20240424/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43129 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    31006 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    30820 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/cloud_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    46901 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    21044 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)    17186 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/paperspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11166 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.605096 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/cudo_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.609096 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/fluidstack_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/kubernetes_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/paperspace_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/runpod_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/vsphere_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.609096 skypilot_nightly-1.0.0.dev20240424/sky/clouds/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/utils/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/utils/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/utils/oci_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/utils/scp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/clouds/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.609096 skypilot_nightly-1.0.0.dev20240424/sky/data/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   119221 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    24916 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    54101 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.609096 skypilot_nightly-1.0.0.dev20240424/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.613096 skypilot_nightly-1.0.0.dev20240424/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    36603 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/aws/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.613096 skypilot_nightly-1.0.0.dev20240424/sky/provision/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/azure/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.613096 skypilot_nightly-1.0.0.dev20240424/sky/provision/cudo/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/cudo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/cudo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/cudo/cudo_machine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/cudo/cudo_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/cudo/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    16696 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/docker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.613096 skypilot_nightly-1.0.0.dev20240424/sky/provision/fluidstack/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/fluidstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/fluidstack/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/fluidstack/fluidstack_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14870 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/fluidstack/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.613096 skypilot_nightly-1.0.0.dev20240424/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    24482 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22258 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/instance_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.617096 skypilot_nightly-1.0.0.dev20240424/sky/provision/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17388 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    32523 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/kubernetes/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.617096 skypilot_nightly-1.0.0.dev20240424/sky/provision/kubernetes/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/kubernetes/manifests/smarter-device-manager-configmap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/kubernetes/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/kubernetes/network_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    54541 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/kubernetes/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.617096 skypilot_nightly-1.0.0.dev20240424/sky/provision/paperspace/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/paperspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/paperspace/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/paperspace/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/paperspace/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/paperspace/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25255 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/provisioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.617096 skypilot_nightly-1.0.0.dev20240424/sky/provision/runpod/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/runpod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/runpod/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/runpod/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/runpod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.617096 skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.621096 skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/cls_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/cls_api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/custom_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/metadata_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/service_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/service_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/ssl_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/vapiconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/vim_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24476 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/vsphere_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    61936 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.625096 skypilot_nightly-1.0.0.dev20240424/sky/serve/
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30137 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/serve/autoscalers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/serve/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/serve/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    28185 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/serve/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/serve/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/serve/load_balancing_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    55738 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/serve/replica_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/serve/serve_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    36837 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/serve/serve_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/serve/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/serve/service_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.625096 skypilot_nightly-1.0.0.dev20240424/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-24 10:39:20.000000 skypilot_nightly-1.0.0.dev20240424/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.625096 skypilot_nightly-1.0.0.dev20240424/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11542 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    35113 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18788 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/log_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/log_lib.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.625096 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.629096 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    18603 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/azure/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    16238 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/command_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.629096 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.629096 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.629096 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.629096 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/scp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.633096 skypilot_nightly-1.0.0.dev20240424/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/skypilot_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.633096 skypilot_nightly-1.0.0.dev20240424/sky/spot/
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/spot/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    25830 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/spot/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/spot/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.633096 skypilot_nightly-1.0.0.dev20240424/sky/spot/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/spot/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.633096 skypilot_nightly-1.0.0.dev20240424/sky/spot/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/spot/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.633096 skypilot_nightly-1.0.0.dev20240424/sky/spot/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/spot/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/spot/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    22487 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/spot/spot_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    31559 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/spot/spot_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    47182 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.637096 skypilot_nightly-1.0.0.dev20240424/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/cudo-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/fluidstack-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/kubernetes-ingress.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/kubernetes-loadbalancer.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/kubernetes-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/kubernetes-ssh-jump.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/paperspace-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/runpod-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/sky-serve-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/spot-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/templates/vsphere-ray.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.637096 skypilot_nightly-1.0.0.dev20240424/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.641096 skypilot_nightly-1.0.0.dev20240424/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.641096 skypilot_nightly-1.0.0.dev20240424/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/cluster_yaml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/command_runner.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22349 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    28915 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/controller_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/env_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.645096 skypilot_nightly-1.0.0.dev20240424/sky/utils/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/kubernetes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9667 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/kubernetes/create_cluster.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/kubernetes/delete_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/kubernetes/generate_kind_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/kubernetes/gpu_labeler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/kubernetes_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/resources_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19133 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.649096 skypilot_nightly-1.0.0.dev20240424/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-24 10:39:23.000000 skypilot_nightly-1.0.0.dev20240424/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9308 2024-04-24 10:39:23.000000 skypilot_nightly-1.0.0.dev20240424/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:39:23.000000 skypilot_nightly-1.0.0.dev20240424/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-24 10:39:23.000000 skypilot_nightly-1.0.0.dev20240424/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-24 10:39:23.000000 skypilot_nightly-1.0.0.dev20240424/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-24 10:39:23.000000 skypilot_nightly-1.0.0.dev20240424/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:23.649096 skypilot_nightly-1.0.0.dev20240424/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/tests/test_serve_autoscaler.py
--rw-r--r--   0 runner    (1001) docker     (127)   212180 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/tests/test_spot_serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/tests/test_wheels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-24 10:39:11.000000 skypilot_nightly-1.0.0.dev20240424/tests/test_yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.435466 skypilot_nightly-1.0.0.dev20240425/
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-25 10:38:08.435466 skypilot_nightly-1.0.0.dev20240425/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 10:38:08.435466 skypilot_nightly-1.0.0.dev20240425/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-25 10:38:05.000000 skypilot_nightly-1.0.0.dev20240425/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.371466 skypilot_nightly-1.0.0.dev20240425/sky/
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-25 10:38:08.000000 skypilot_nightly-1.0.0.dev20240425/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.371466 skypilot_nightly-1.0.0.dev20240425/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/adaptors/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/adaptors/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/adaptors/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/adaptors/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/adaptors/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21410 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.375466 skypilot_nightly-1.0.0.dev20240425/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118820 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   223223 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.375466 skypilot_nightly-1.0.0.dev20240425/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.375466 skypilot_nightly-1.0.0.dev20240425/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26440 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)   186846 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.379466 skypilot_nightly-1.0.0.dev20240425/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43129 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31006 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30820 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/cloud_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46901 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21044 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17186 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/paperspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11166 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.383466 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/cudo_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.383466 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/fluidstack_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/kubernetes_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/paperspace_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/runpod_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/vsphere_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.383466 skypilot_nightly-1.0.0.dev20240425/sky/clouds/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/utils/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/utils/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/utils/oci_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/utils/scp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/clouds/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.387466 skypilot_nightly-1.0.0.dev20240425/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118872 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24916 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54101 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.387466 skypilot_nightly-1.0.0.dev20240425/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.387466 skypilot_nightly-1.0.0.dev20240425/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36603 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/aws/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.387466 skypilot_nightly-1.0.0.dev20240425/sky/provision/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/azure/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.387466 skypilot_nightly-1.0.0.dev20240425/sky/provision/cudo/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/cudo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/cudo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/cudo/cudo_machine_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/cudo/cudo_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/cudo/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16696 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/docker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.391466 skypilot_nightly-1.0.0.dev20240425/sky/provision/fluidstack/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/fluidstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/fluidstack/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/fluidstack/fluidstack_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14870 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/fluidstack/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.391466 skypilot_nightly-1.0.0.dev20240425/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24482 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22258 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/instance_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.391466 skypilot_nightly-1.0.0.dev20240425/sky/provision/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17388 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32523 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/kubernetes/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.391466 skypilot_nightly-1.0.0.dev20240425/sky/provision/kubernetes/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/kubernetes/manifests/smarter-device-manager-configmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/kubernetes/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/kubernetes/network_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54541 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/kubernetes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.395466 skypilot_nightly-1.0.0.dev20240425/sky/provision/paperspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/paperspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/paperspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/paperspace/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/paperspace/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/paperspace/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25255 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/provisioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.395466 skypilot_nightly-1.0.0.dev20240425/sky/provision/runpod/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/runpod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/runpod/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/runpod/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/runpod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.395466 skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.395466 skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/cls_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/cls_api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/custom_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/metadata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/service_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/ssl_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/vapiconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/vim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24476 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/vsphere_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61936 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.399466 skypilot_nightly-1.0.0.dev20240425/sky/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30137 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/serve/autoscalers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/serve/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/serve/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28185 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/serve/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/serve/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/serve/load_balancing_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55738 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/serve/replica_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/serve/serve_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36837 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/serve/serve_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/serve/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/serve/service_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.399466 skypilot_nightly-1.0.0.dev20240425/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-25 10:38:05.000000 skypilot_nightly-1.0.0.dev20240425/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.403466 skypilot_nightly-1.0.0.dev20240425/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35167 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18788 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/log_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/log_lib.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.403466 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.403466 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18603 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/azure/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16238 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/command_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.403466 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.403466 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.407466 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.407466 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/scp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.407466 skypilot_nightly-1.0.0.dev20240425/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/skypilot_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.411466 skypilot_nightly-1.0.0.dev20240425/sky/spot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/spot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25830 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/spot/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/spot/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.411466 skypilot_nightly-1.0.0.dev20240425/sky/spot/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/spot/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.411466 skypilot_nightly-1.0.0.dev20240425/sky/spot/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/spot/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.411466 skypilot_nightly-1.0.0.dev20240425/sky/spot/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/spot/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/spot/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22487 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/spot/spot_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31559 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/spot/spot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47239 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.415466 skypilot_nightly-1.0.0.dev20240425/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/cudo-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/fluidstack-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/kubernetes-ingress.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/kubernetes-loadbalancer.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/kubernetes-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/kubernetes-ssh-jump.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/paperspace-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/runpod-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/sky-serve-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/spot-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/templates/vsphere-ray.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.415466 skypilot_nightly-1.0.0.dev20240425/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.419466 skypilot_nightly-1.0.0.dev20240425/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.419466 skypilot_nightly-1.0.0.dev20240425/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/cluster_yaml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/command_runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22547 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28443 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/controller_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/env_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.419466 skypilot_nightly-1.0.0.dev20240425/sky/utils/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/kubernetes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9667 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/kubernetes/create_cluster.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/kubernetes/delete_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/kubernetes/generate_kind_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/kubernetes/gpu_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/kubernetes_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/resources_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19133 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.423466 skypilot_nightly-1.0.0.dev20240425/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-25 10:38:08.000000 skypilot_nightly-1.0.0.dev20240425/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9308 2024-04-25 10:38:08.000000 skypilot_nightly-1.0.0.dev20240425/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 10:38:08.000000 skypilot_nightly-1.0.0.dev20240425/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 10:38:08.000000 skypilot_nightly-1.0.0.dev20240425/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-25 10:38:08.000000 skypilot_nightly-1.0.0.dev20240425/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-25 10:38:08.000000 skypilot_nightly-1.0.0.dev20240425/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:38:08.423466 skypilot_nightly-1.0.0.dev20240425/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/tests/test_serve_autoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)   212180 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/tests/test_spot_serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/tests/test_wheels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-25 10:38:03.000000 skypilot_nightly-1.0.0.dev20240425/tests/test_yaml_parser.py
```

### Comparing `skypilot_nightly-1.0.0.dev20240424/LICENSE` & `skypilot_nightly-1.0.0.dev20240425/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/MANIFEST.in` & `skypilot_nightly-1.0.0.dev20240425/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/PKG-INFO` & `skypilot_nightly-1.0.0.dev20240425/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240424
+Version: 1.0.0.dev20240425
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot_nightly-1.0.0.dev20240424/README.md` & `skypilot_nightly-1.0.0.dev20240425/README.md`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/pyproject.toml` & `skypilot_nightly-1.0.0.dev20240425/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/setup.py` & `skypilot_nightly-1.0.0.dev20240425/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/__init__.py` & `skypilot_nightly-1.0.0.dev20240425/sky/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """The SkyPilot package."""
 import os
 import subprocess
 from typing import Optional
 import urllib.request
 
 # Replaced with the current commit when building the wheels.
-_SKYPILOT_COMMIT_SHA = 'f3be7732a1d9890e24dd9d87f9bdc19faeeeca8b'
+_SKYPILOT_COMMIT_SHA = '34b55f9694a7ad635957fd3a2631e0eeed06f07e'
 
 
 def _get_git_commit():
     if 'SKYPILOT_COMMIT_SHA' not in _SKYPILOT_COMMIT_SHA:
         # This is a release build, so we don't need to get the commit hash from
         # git, as it's already been set.
         return _SKYPILOT_COMMIT_SHA
@@ -31,15 +31,15 @@
             commit_hash += '-dirty'
         return commit_hash
     except Exception:  # pylint: disable=broad-except
         return _SKYPILOT_COMMIT_SHA
 
 
 __commit__ = _get_git_commit()
-__version__ = '1.0.0.dev20240424'
+__version__ = '1.0.0.dev20240425'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 
 # ---------------------- Proxy Configuration ---------------------- #
 def _set_http_proxy_env_vars() -> None:
     urllib_proxies = dict(urllib.request.getproxies())
```

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/adaptors/aws.py` & `skypilot_nightly-1.0.0.dev20240425/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/adaptors/azure.py` & `skypilot_nightly-1.0.0.dev20240425/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/adaptors/cloudflare.py` & `skypilot_nightly-1.0.0.dev20240425/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/adaptors/common.py` & `skypilot_nightly-1.0.0.dev20240425/sky/adaptors/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/adaptors/gcp.py` & `skypilot_nightly-1.0.0.dev20240425/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/adaptors/ibm.py` & `skypilot_nightly-1.0.0.dev20240425/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/adaptors/kubernetes.py` & `skypilot_nightly-1.0.0.dev20240425/sky/adaptors/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/adaptors/oci.py` & `skypilot_nightly-1.0.0.dev20240425/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/adaptors/vsphere.py` & `skypilot_nightly-1.0.0.dev20240425/sky/adaptors/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/authentication.py` & `skypilot_nightly-1.0.0.dev20240425/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/backends/__init__.py` & `skypilot_nightly-1.0.0.dev20240425/sky/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/backends/backend.py` & `skypilot_nightly-1.0.0.dev20240425/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/backends/backend_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/backends/backend_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/backends/cloud_vm_ray_backend.py` & `skypilot_nightly-1.0.0.dev20240425/sky/backends/cloud_vm_ray_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/backends/docker_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/backends/local_docker_backend.py` & `skypilot_nightly-1.0.0.dev20240425/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot_nightly-1.0.0.dev20240425/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/backends/wheel_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/benchmark/benchmark_state.py` & `skypilot_nightly-1.0.0.dev20240425/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/benchmark/benchmark_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/check.py` & `skypilot_nightly-1.0.0.dev20240425/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/cli.py` & `skypilot_nightly-1.0.0.dev20240425/sky/cli.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/cloud_stores.py` & `skypilot_nightly-1.0.0.dev20240425/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/__init__.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/aws.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/azure.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/cloud.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/cloud_registry.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/cloud_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/cudo.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/fluidstack.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/gcp.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/ibm.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/kubernetes.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/lambda_cloud.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/oci.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/paperspace.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/paperspace.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/runpod.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/runpod.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/scp.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/scp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/__init__.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/aws_catalog.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/azure_catalog.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/common.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/config.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/cudo_catalog.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/cudo_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/fluidstack_catalog.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/fluidstack_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/kubernetes_catalog.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/kubernetes_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/oci_catalog.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/paperspace_catalog.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/paperspace_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/runpod_catalog.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/runpod_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/scp_catalog.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/service_catalog/vsphere_catalog.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/service_catalog/vsphere_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/utils/gcp_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/utils/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/utils/lambda_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/utils/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/utils/oci_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/utils/oci_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/utils/scp_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/utils/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/clouds/vsphere.py` & `skypilot_nightly-1.0.0.dev20240425/sky/clouds/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/core.py` & `skypilot_nightly-1.0.0.dev20240425/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/dag.py` & `skypilot_nightly-1.0.0.dev20240425/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/data/data_transfer.py` & `skypilot_nightly-1.0.0.dev20240425/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/data/data_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/data/mounting_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/data/storage.py` & `skypilot_nightly-1.0.0.dev20240425/sky/data/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,23 +106,32 @@
     S3 = 'S3'
     GCS = 'GCS'
     AZURE = 'AZURE'
     R2 = 'R2'
     IBM = 'IBM'
 
     @classmethod
-    def from_cloud(cls, cloud: clouds.Cloud) -> 'StoreType':
-        if isinstance(cloud, clouds.AWS):
+    def from_cloud(cls, cloud: str) -> 'StoreType':
+        if cloud.lower() == str(clouds.AWS()).lower():
             return StoreType.S3
-        elif isinstance(cloud, clouds.GCP):
+        elif cloud.lower() == str(clouds.GCP()).lower():
             return StoreType.GCS
-        elif isinstance(cloud, clouds.Azure):
-            return StoreType.AZURE
-        elif isinstance(cloud, clouds.IBM):
+        elif cloud.lower() == str(clouds.IBM()).lower():
             return StoreType.IBM
+        elif cloud.lower() == cloudflare.NAME.lower():
+            return StoreType.R2
+        elif cloud.lower() == str(clouds.Azure()).lower():
+            with ux_utils.print_exception_no_traceback():
+                raise ValueError('Azure Blob Storage is not supported yet.')
+        elif cloud.lower() == str(clouds.Lambda()).lower():
+            with ux_utils.print_exception_no_traceback():
+                raise ValueError('Lambda Cloud does not provide cloud storage.')
+        elif cloud.lower() == str(clouds.SCP()).lower():
+            with ux_utils.print_exception_no_traceback():
+                raise ValueError('SCP does not provide cloud storage.')
 
         raise ValueError(f'Unsupported cloud for StoreType: {cloud}')
 
     @classmethod
     def from_store(cls, store: 'AbstractStore') -> 'StoreType':
         if isinstance(store, S3Store):
             return StoreType.S3
@@ -132,59 +141,36 @@
             return StoreType.R2
         elif isinstance(store, IBMCosStore):
             return StoreType.IBM
         else:
             with ux_utils.print_exception_no_traceback():
                 raise ValueError(f'Unknown store type: {store}')
 
+    def store_prefix(self) -> str:
+        if self == StoreType.S3:
+            return 's3://'
+        elif self == StoreType.GCS:
+            return 'gs://'
+        elif self == StoreType.R2:
+            return 'r2://'
+        elif self == StoreType.IBM:
+            return 'cos://'
+        elif self == StoreType.AZURE:
+            with ux_utils.print_exception_no_traceback():
+                raise ValueError('Azure Blob Storage is not supported yet.')
+        else:
+            with ux_utils.print_exception_no_traceback():
+                raise ValueError(f'Unknown store type: {self}')
+
 
 class StorageMode(enum.Enum):
     MOUNT = 'MOUNT'
     COPY = 'COPY'
 
 
-def get_storetype_from_cloud(cloud: clouds.Cloud) -> StoreType:
-    if isinstance(cloud, clouds.AWS):
-        return StoreType.S3
-    elif isinstance(cloud, clouds.GCP):
-        return StoreType.GCS
-    elif isinstance(cloud, clouds.IBM):
-        return StoreType.IBM
-    elif isinstance(cloud, clouds.Azure):
-        with ux_utils.print_exception_no_traceback():
-            raise ValueError('Azure Blob Storage is not supported yet.')
-    elif isinstance(cloud, clouds.Lambda):
-        with ux_utils.print_exception_no_traceback():
-            raise ValueError('Lambda Cloud does not provide cloud storage.')
-    elif isinstance(cloud, clouds.SCP):
-        with ux_utils.print_exception_no_traceback():
-            raise ValueError('SCP does not provide cloud storage.')
-    else:
-        with ux_utils.print_exception_no_traceback():
-            raise ValueError(f'Unknown cloud type: {cloud}')
-
-
-def get_store_prefix(storetype: StoreType) -> str:
-    if storetype == StoreType.S3:
-        return 's3://'
-    elif storetype == StoreType.GCS:
-        return 'gs://'
-    # R2 storages use 's3://' as a prefix for various aws cli commands
-    elif storetype == StoreType.R2:
-        return 's3://'
-    elif storetype == StoreType.IBM:
-        return 'cos://'
-    elif storetype == StoreType.AZURE:
-        with ux_utils.print_exception_no_traceback():
-            raise ValueError('Azure Blob Storage is not supported yet.')
-    else:
-        with ux_utils.print_exception_no_traceback():
-            raise ValueError(f'Unknown store type: {storetype}')
-
-
 class AbstractStore:
     """AbstractStore abstracts away the different storage types exposed by
     different clouds.
 
     Storage objects are backed by AbstractStores, each representing a store
     present in a cloud.
     """
@@ -349,15 +335,15 @@
             handle = global_user_state.get_handle_from_storage_name(self.name)
             # If handle is None, it implies the bucket is created
             # externally and not managed by Skypilot. For mounting such
             # externally created buckets, users must provide the
             # bucket's URL as 'source'.
             if handle is None:
                 with ux_utils.print_exception_no_traceback():
-                    store_prefix = get_store_prefix(StoreType.from_store(self))
+                    store_prefix = StoreType.from_store(self).store_prefix()
                     raise exceptions.StorageSpecError(
                         'Attempted to mount a non-sky managed bucket '
                         f'{self.name!r} without specifying the storage source.'
                         f' Bucket {self.name!r} already exists. \n'
                         '    • To create a new bucket, specify a unique name.\n'
                         '    • To mount an externally created bucket (e.g., '
                         'created through cloud console or cloud cli), '
```

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/data/storage_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/exceptions.py` & `skypilot_nightly-1.0.0.dev20240425/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/execution.py` & `skypilot_nightly-1.0.0.dev20240425/sky/execution.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/global_user_state.py` & `skypilot_nightly-1.0.0.dev20240425/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/optimizer.py` & `skypilot_nightly-1.0.0.dev20240425/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/__init__.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/aws/__init__.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/aws/config.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/aws/instance.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/aws/utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/azure/instance.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/azure/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/common.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/cudo/__init__.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/cudo/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/cudo/cudo_machine_type.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/cudo/cudo_machine_type.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/cudo/cudo_wrapper.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/cudo/cudo_wrapper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/cudo/instance.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/cudo/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/docker_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/fluidstack/__init__.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/fluidstack/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/fluidstack/fluidstack_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/fluidstack/fluidstack_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/fluidstack/instance.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/fluidstack/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/gcp/__init__.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/gcp/config.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/gcp/constants.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/gcp/instance.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/gcp/instance_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/instance_setup.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/instance_setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/kubernetes/__init__.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/kubernetes/config.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/kubernetes/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/kubernetes/instance.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/kubernetes/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/kubernetes/network.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/kubernetes/network.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/kubernetes/network_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/kubernetes/network_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/kubernetes/utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/logging.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/logging.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/metadata_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/paperspace/__init__.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/paperspace/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/paperspace/config.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/paperspace/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/paperspace/constants.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/paperspace/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/paperspace/instance.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/paperspace/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/paperspace/utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/paperspace/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/provisioner.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/provisioner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/runpod/instance.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/runpod/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/runpod/utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/runpod/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/__init__.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/cls_api_client.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/cls_api_client.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/cls_api_helper.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/cls_api_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/metadata_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/service_manager.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/service_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/service_manager_factory.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/service_manager_factory.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/ssl_helper.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/ssl_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/vapiconnect.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/vapiconnect.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/common/vim_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/common/vim_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/instance.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/provision/vsphere/vsphere_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/provision/vsphere/vsphere_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/resources.py` & `skypilot_nightly-1.0.0.dev20240425/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/serve/__init__.py` & `skypilot_nightly-1.0.0.dev20240425/sky/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/serve/autoscalers.py` & `skypilot_nightly-1.0.0.dev20240425/sky/serve/autoscalers.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/serve/constants.py` & `skypilot_nightly-1.0.0.dev20240425/sky/serve/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/serve/controller.py` & `skypilot_nightly-1.0.0.dev20240425/sky/serve/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/serve/core.py` & `skypilot_nightly-1.0.0.dev20240425/sky/serve/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/serve/load_balancer.py` & `skypilot_nightly-1.0.0.dev20240425/sky/serve/load_balancer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/serve/load_balancing_policies.py` & `skypilot_nightly-1.0.0.dev20240425/sky/serve/load_balancing_policies.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/serve/replica_managers.py` & `skypilot_nightly-1.0.0.dev20240425/sky/serve/replica_managers.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/serve/serve_state.py` & `skypilot_nightly-1.0.0.dev20240425/sky/serve/serve_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/serve/serve_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/serve/serve_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/serve/service.py` & `skypilot_nightly-1.0.0.dev20240425/sky/serve/service.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/serve/service_spec.py` & `skypilot_nightly-1.0.0.dev20240425/sky/serve/service_spec.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/setup_files/MANIFEST.in` & `skypilot_nightly-1.0.0.dev20240425/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/setup_files/setup.py` & `skypilot_nightly-1.0.0.dev20240425/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/sky_logging.py` & `skypilot_nightly-1.0.0.dev20240425/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/LICENSE` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/attempt_skylet.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/autostop_lib.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/configs.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/constants.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/events.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 
 class JobSchedulerEvent(SkyletEvent):
     """Skylet event for scheduling jobs"""
     EVENT_INTERVAL_SECONDS = 300
 
     def _run(self):
-        job_lib.scheduler.schedule_step()
+        job_lib.scheduler.schedule_step(force_update_jobs=True)
 
 
 class SpotJobUpdateEvent(SkyletEvent):
     """Skylet event for updating spot job status."""
     EVENT_INTERVAL_SECONDS = 300
 
     def _run(self):
```

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/job_lib.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/job_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,17 +161,17 @@
 
     def _run_job(self, job_id: int, run_cmd: str):
         _CURSOR.execute((f'UPDATE pending_jobs SET submit={int(time.time())} '
                          f'WHERE job_id={job_id!r}'))
         _CONN.commit()
         subprocess.Popen(run_cmd, shell=True, stdout=subprocess.DEVNULL)
 
-    def schedule_step(self) -> None:
+    def schedule_step(self, force_update_jobs: bool = False) -> None:
         jobs = self._get_jobs()
-        if len(jobs) > 0:
+        if len(jobs) > 0 or force_update_jobs:
             update_status()
         # TODO(zhwu, mraheja): One optimization can be allowing more than one
         # job staying in the pending state after ray job submit, so that to be
         # faster to schedule a large amount of jobs.
         for job_id, run_cmd, submit, created_time in jobs:
             with filelock.FileLock(_get_lock_path(job_id)):
                 status = get_status_no_lock(job_id)
```

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/log_lib.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/log_lib.pyi` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/log_lib.pyi`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/azure/azure-config-template.json` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/azure/config.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/azure/node_provider.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/command_runner.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/ibm/node_provider.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/ibm/utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/oci/node_provider.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/oci/query_helper.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/scp/config.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/providers/scp/node_provider.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/ray_patches/__init__.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/ray_patches/worker.py.patch` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/skylet.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skylet/subprocess_daemon.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/skypilot_config.py` & `skypilot_nightly-1.0.0.dev20240425/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/spot/__init__.py` & `skypilot_nightly-1.0.0.dev20240425/sky/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/spot/constants.py` & `skypilot_nightly-1.0.0.dev20240425/sky/spot/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/spot/controller.py` & `skypilot_nightly-1.0.0.dev20240425/sky/spot/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/spot/core.py` & `skypilot_nightly-1.0.0.dev20240425/sky/spot/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/spot/dashboard/dashboard.py` & `skypilot_nightly-1.0.0.dev20240425/sky/spot/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/spot/dashboard/static/favicon.ico` & `skypilot_nightly-1.0.0.dev20240425/sky/spot/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/spot/dashboard/templates/index.html` & `skypilot_nightly-1.0.0.dev20240425/sky/spot/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/spot/recovery_strategy.py` & `skypilot_nightly-1.0.0.dev20240425/sky/spot/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/spot/spot_state.py` & `skypilot_nightly-1.0.0.dev20240425/sky/spot/spot_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/spot/spot_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/spot/spot_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/status_lib.py` & `skypilot_nightly-1.0.0.dev20240425/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/task.py` & `skypilot_nightly-1.0.0.dev20240425/sky/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,35 +344,34 @@
                         f'a symlink to a directory). {self.workdir} not found.')
 
     @staticmethod
     def from_yaml_config(
         config: Dict[str, Any],
         env_overrides: Optional[List[Tuple[str, str]]] = None,
     ) -> 'Task':
+        # More robust handling for 'envs': explicitly convert keys and values to
+        # str, since users may pass '123' as keys/values which will get parsed
+        # as int causing validate_schema() to fail.
+        envs = config.get('envs')
+        if envs is not None and isinstance(envs, dict):
+            config['envs'] = {str(k): str(v) for k, v in envs.items()}
+
+        common_utils.validate_schema(config, schemas.get_task_schema(),
+                                     'Invalid task YAML: ')
         if env_overrides is not None:
             # We must override env vars before constructing the Task, because
             # the Storage object creation is eager and it (its name/source
             # fields) may depend on env vars.
             #
             # FIXME(zongheng): The eagerness / how we construct Task's from
             # entrypoint (YAML, CLI args) should be fixed.
             new_envs = config.get('envs', {})
             new_envs.update(env_overrides)
             config['envs'] = new_envs
 
-        # More robust handling for 'envs': explicitly convert keys and values to
-        # str, since users may pass '123' as keys/values which will get parsed
-        # as int causing validate_schema() to fail.
-        envs = config.get('envs')
-        if envs is not None and isinstance(envs, dict):
-            config['envs'] = {str(k): str(v) for k, v in envs.items()}
-
-        common_utils.validate_schema(config, schemas.get_task_schema(),
-                                     'Invalid task YAML: ')
-
         # Fill in any Task.envs into file_mounts (src/dst paths, storage
         # name/source).
         if config.get('file_mounts') is not None:
             config['file_mounts'] = _fill_in_env_vars(config['file_mounts'],
                                                       config.get('envs', {}))
 
         # Fill in any Task.envs into service (e.g. MODEL_NAME).
@@ -897,25 +896,28 @@
         if self.best_resources is not None:
             storage_cloud = self.best_resources.cloud
             storage_region = self.best_resources.region
         else:
             resources = list(self.resources)[0]
             storage_cloud = resources.cloud
             storage_region = resources.region
+
         if storage_cloud is not None:
             if str(storage_cloud) not in enabled_storage_clouds:
                 storage_cloud = None
 
+        storage_cloud_str = None
         if storage_cloud is None:
-            storage_cloud = clouds.CLOUD_REGISTRY.from_str(
-                enabled_storage_clouds[0])
-            assert storage_cloud is not None, enabled_storage_clouds[0]
+            storage_cloud_str = enabled_storage_clouds[0]
+            assert storage_cloud_str is not None, enabled_storage_clouds[0]
             storage_region = None  # Use default region in the Store class
+        else:
+            storage_cloud_str = str(storage_cloud)
 
-        store_type = storage_lib.get_storetype_from_cloud(storage_cloud)
+        store_type = storage_lib.StoreType.from_cloud(storage_cloud_str)
         return store_type, storage_region
 
     def sync_storage_mounts(self) -> None:
         """(INTERNAL) Eagerly syncs storage mounts to cloud storage.
 
         After syncing up, COPY-mode storage mounts are translated into regular
         file_mounts of the form ``{ /remote/path: {s3,gs,..}://<bucket path>
```

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/aws-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/azure-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/cudo-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/cudo-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/fluidstack-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/fluidstack-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/gcp-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/gcp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/ibm-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/kubernetes-ingress.yml.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/kubernetes-ingress.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/kubernetes-port-forward-proxy-command.sh.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/kubernetes-port-forward-proxy-command.sh.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/kubernetes-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/kubernetes-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/kubernetes-ssh-jump.yml.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/kubernetes-ssh-jump.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/lambda-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/local-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/oci-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/paperspace-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/paperspace-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/runpod-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/runpod-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/scp-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/sky-serve-controller.yaml.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/sky-serve-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/spot-controller.yaml.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/spot-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/templates/vsphere-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240425/sky/templates/vsphere-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/usage/constants.py` & `skypilot_nightly-1.0.0.dev20240425/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/usage/usage_lib.py` & `skypilot_nightly-1.0.0.dev20240425/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/accelerator_registry.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/cli_utils/status_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/cluster_yaml_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/cluster_yaml_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/command_runner.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/command_runner.pyi` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/command_runner.pyi`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/common_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/common_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -563,28 +563,32 @@
                 #
                 # This will print something like:
                 # 'hello world' does not match any of the regexes: <regex>
                 err_msg = (err_msg_prefix +
                            'The `envs` field contains invalid keys:\n' +
                            e.message)
             else:
-                err_msg = err_msg_prefix + 'The following fields are invalid:'
+                err_msg = err_msg_prefix
                 known_fields = set(e.schema.get('properties', {}).keys())
                 for field in e.instance:
                     if field not in known_fields:
                         most_similar_field = difflib.get_close_matches(
                             field, known_fields, 1)
                         if most_similar_field:
-                            err_msg += (f'\nInstead of {field!r}, did you mean '
+                            err_msg += (f'Instead of {field!r}, did you mean '
                                         f'{most_similar_field[0]!r}?')
                         else:
-                            err_msg += f'\nFound unsupported field {field!r}.'
+                            err_msg += f'Found unsupported field {field!r}.'
         else:
+            message = e.message
+            # Object in jsonschema is represented as dict in Python. Replace
+            # 'object' with 'dict' for better readability.
+            message = message.replace('type \'object\'', 'type \'dict\'')
             # Example e.json_path value: '$.resources'
-            err_msg = (err_msg_prefix + e.message +
+            err_msg = (err_msg_prefix + message +
                        f'. Check problematic field(s): {e.json_path}')
 
     if err_msg:
         with ux_utils.print_exception_no_traceback():
             raise ValueError(err_msg)
```

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/controller_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/controller_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -602,19 +602,19 @@
         logger.info(f'{colorama.Fore.YELLOW}Uploading sources to cloud storage.'
                     f'{colorama.Style.RESET_ALL} See: sky storage ls')
     task.sync_storage_mounts()
 
     # Step 5: Add the file download into the file mounts, such as
     #  /original-dst: s3://spot-fm-file-only-bucket-name/file-0
     new_file_mounts = {}
+    storage = task.storage_mounts[file_mount_remote_tmp_dir]
+    store_type = list(storage.stores.keys())[0]
+    store_prefix = store_type.store_prefix()
+    bucket_url = store_prefix + file_bucket_name
     for dst, src in copy_mounts_with_file_in_src.items():
-        storage = task.storage_mounts[file_mount_remote_tmp_dir]
-        store_type = list(storage.stores.keys())[0]
-        store_prefix = storage_lib.get_store_prefix(store_type)
-        bucket_url = store_prefix + file_bucket_name
         file_id = src_to_file_id[src]
         new_file_mounts[dst] = bucket_url + f'/file-{file_id}'
     task.update_file_mounts(new_file_mounts)
 
     # Step 6: Replace the source field that is local path in all storage_mounts
     # with bucket URI and remove the name field.
     for storage_obj in task.storage_mounts.values():
@@ -623,18 +623,10 @@
             # Need to replace the local path with bucket URI, and remove the
             # name field, so that the storage mount can work on the spot
             # controller.
             store_types = list(storage_obj.stores.keys())
             assert len(store_types) == 1, (
                 'We only support one store type for now.', storage_obj.stores)
             store_type = store_types[0]
-            if store_type == storage_lib.StoreType.S3:
-                storage_obj.source = f's3://{storage_obj.name}'
-            elif store_type == storage_lib.StoreType.GCS:
-                storage_obj.source = f'gs://{storage_obj.name}'
-            elif store_type == storage_lib.StoreType.R2:
-                storage_obj.source = f'r2://{storage_obj.name}'
-            else:
-                with ux_utils.print_exception_no_traceback():
-                    raise exceptions.NotSupportedError(
-                        f'Unsupported store type: {store_type}')
+            store_prefix = store_type.store_prefix()
+            storage_obj.source = f'{store_prefix}{storage_obj.name}'
             storage_obj.force_delete = True
```

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/dag_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/db_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/env_options.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/kubernetes/create_cluster.sh` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/kubernetes/create_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/kubernetes/delete_cluster.sh` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/kubernetes/delete_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/kubernetes/generate_kind_config.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/kubernetes/generate_kind_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/kubernetes/gpu_labeler.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/kubernetes/gpu_labeler.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/kubernetes_enums.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/kubernetes_enums.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/log_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/resources_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/resources_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/rich_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/schemas.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/subprocess_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/timeline.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/ux_utils.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/sky/utils/validator.py` & `skypilot_nightly-1.0.0.dev20240425/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/skypilot_nightly.egg-info/PKG-INFO` & `skypilot_nightly-1.0.0.dev20240425/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240424
+Version: 1.0.0.dev20240425
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot_nightly-1.0.0.dev20240424/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot_nightly-1.0.0.dev20240425/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/skypilot_nightly.egg-info/requires.txt` & `skypilot_nightly-1.0.0.dev20240425/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/tests/test_cli.py` & `skypilot_nightly-1.0.0.dev20240425/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/tests/test_config.py` & `skypilot_nightly-1.0.0.dev20240425/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/tests/test_jobs.py` & `skypilot_nightly-1.0.0.dev20240425/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/tests/test_list_accelerators.py` & `skypilot_nightly-1.0.0.dev20240425/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/tests/test_optimizer_dryruns.py` & `skypilot_nightly-1.0.0.dev20240425/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/tests/test_optimizer_random_dag.py` & `skypilot_nightly-1.0.0.dev20240425/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/tests/test_serve_autoscaler.py` & `skypilot_nightly-1.0.0.dev20240425/tests/test_serve_autoscaler.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/tests/test_smoke.py` & `skypilot_nightly-1.0.0.dev20240425/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/tests/test_spot_serve.py` & `skypilot_nightly-1.0.0.dev20240425/tests/test_spot_serve.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/tests/test_storage.py` & `skypilot_nightly-1.0.0.dev20240425/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/tests/test_wheels.py` & `skypilot_nightly-1.0.0.dev20240425/tests/test_wheels.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240424/tests/test_yaml_parser.py` & `skypilot_nightly-1.0.0.dev20240425/tests/test_yaml_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -107,7 +107,30 @@
                 /datasets-storage:
                     name: sky-dataset
                     not_a_valid_field:
             """), tmp_path)
     with pytest.raises(AssertionError) as e:
         Task.from_yaml(config_path)
     assert 'Invalid storage args' in e.value.args[0]
+
+
+def test_invalid_envs_key(tmp_path):
+    config_path = _create_config_file(
+        textwrap.dedent(f"""\
+            envs:
+                invalid_env_$_key: value
+            """), tmp_path)
+    with pytest.raises(ValueError) as e:
+        Task.from_yaml(config_path)
+    assert 'does not match any of the regexes:' in e.value.args[0]
+
+
+def test_invalid_envs_type(tmp_path):
+    config_path = _create_config_file(
+        textwrap.dedent(f"""\
+            envs:
+                - env_key1: abc
+                - env_key2: abc
+            """), tmp_path)
+    with pytest.raises(ValueError) as e:
+        Task.from_yaml(config_path)
+    assert 'is not of type \'dict\'' in e.value.args[0]
```

