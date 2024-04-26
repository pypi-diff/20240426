# Comparing `tmp/proximl-0.5.6.tar.gz` & `tmp/proximl-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proximl-0.5.6.tar", last modified: Fri Apr 12 19:06:44 2024, max compression
+gzip compressed data, was "proximl-0.5.7.tar", last modified: Fri Apr 26 21:07:09 2024, max compression
```

## Comparing `proximl-0.5.6.tar` & `proximl-0.5.7.tar`

### file list

```diff
@@ -1,123 +1,126 @@
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.193520 proximl-0.5.6/
--rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2024-04-12 17:04:07.000000 proximl-0.5.6/LICENSE
--rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-04-12 19:06:44.193363 proximl-0.5.6/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2024-04-12 17:04:07.000000 proximl-0.5.6/README.md
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.175377 proximl-0.5.6/examples/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-12 17:04:07.000000 proximl-0.5.6/examples/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2024-04-12 17:04:07.000000 proximl-0.5.6/examples/create_dataset_and_training_job.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2024-04-12 17:04:07.000000 proximl-0.5.6/examples/local_storage.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2024-04-12 17:04:07.000000 proximl-0.5.6/examples/training_inference_pipeline.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.179232 proximl-0.5.6/proximl/
--rw-r--r--   0 akowalsk   (501) staff       (20)      432 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)       59 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/__main__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26565 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8274 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/checkpoints.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.181314 proximl-0.5.6/proximl/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)     4346 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/checkpoint.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.182253 proximl-0.5.6/proximl/cli/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)      526 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/cloudbender/datastore.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3453 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/cloudbender/device.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/cloudbender/node.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/cloudbender/provider.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/cloudbender/region.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2869 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/cloudbender/service.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/connection.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6871 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/dataset.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/environment.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      883 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/gpu.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.182568 proximl-0.5.6/proximl/cli/job/
--rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/job/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    34288 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/job/create.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6111 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/model.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3314 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/project.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6246 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/volume.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.183916 proximl-0.5.6/proximl/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)       64 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      618 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cloudbender/cloudbender.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3506 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cloudbender/datastores.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3399 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cloudbender/device_configs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5660 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cloudbender/devices.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4332 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cloudbender/nodes.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2036 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cloudbender/providers.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3570 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cloudbender/regions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3222 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cloudbender/services.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    20035 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/connections.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7935 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/datasets.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/environments.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4094 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1901 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/gpu_types.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    17838 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/jobs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7750 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/models.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5001 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/projects.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    10864 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/proximl.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8094 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/volumes.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.179968 proximl-0.5.6/proximl.egg-info/
--rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-04-12 19:06:44.000000 proximl-0.5.6/proximl.egg-info/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     3490 2024-04-12 19:06:44.000000 proximl-0.5.6/proximl.egg-info/SOURCES.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)        1 2024-04-12 19:06:44.000000 proximl-0.5.6/proximl.egg-info/dependency_links.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       63 2024-04-12 19:06:44.000000 proximl-0.5.6/proximl.egg-info/entry_points.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       67 2024-04-12 19:06:44.000000 proximl-0.5.6/proximl.egg-info/requires.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       23 2024-04-12 19:06:44.000000 proximl-0.5.6/proximl.egg-info/top_level.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)      992 2024-04-12 17:04:07.000000 proximl-0.5.6/pyproject.toml
--rw-r--r--   0 akowalsk   (501) staff       (20)       38 2024-04-12 19:06:44.193565 proximl-0.5.6/setup.cfg
--rw-r--r--   0 akowalsk   (501) staff       (20)     1225 2024-04-12 17:04:07.000000 proximl-0.5.6/setup.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.173766 proximl-0.5.6/tests/
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.185226 proximl-0.5.6/tests/integration/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.185443 proximl-0.5.6/tests/integration/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/cloudbender/test_providers_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3230 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/test_checkpoints_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3499 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/test_datasets_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/test_environments_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/test_gpu_types_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    24730 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/test_jobs_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2902 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/test_models_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1446 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/test_projects_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3270 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/test_volumes_integration.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.188844 proximl-0.5.6/tests/unit/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.190508 proximl-0.5.6/tests/unit/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.191471 proximl-0.5.6/tests/unit/cli/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1342 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_device_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_node_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      781 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_provider_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_region_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1311 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_reservation_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      236 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      702 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/test_cli_checkpoint_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      653 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/test_cli_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      683 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/test_cli_environment_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      650 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/test_cli_gpu_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      611 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/test_cli_job_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      629 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/test_cli_model_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1688 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/test_cli_project_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      644 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/test_cli_volume_unit.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.193117 proximl-0.5.6/tests/unit/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5398 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cloudbender/test_datastores_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5714 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cloudbender/test_device_configs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     9103 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cloudbender/test_devices_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6231 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cloudbender/test_nodes_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4373 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cloudbender/test_providers_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6299 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cloudbender/test_regions_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5043 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cloudbender/test_services_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    31129 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      858 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_checkpoints_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_connections_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_environments_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      906 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_gpu_types_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_jobs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_models_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     9238 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_projects_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_proximl.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15305 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_volumes_unit.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.794194 proximl-0.5.7/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2024-04-26 21:06:15.000000 proximl-0.5.7/LICENSE
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-04-26 21:07:09.794030 proximl-0.5.7/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2024-04-26 21:06:15.000000 proximl-0.5.7/README.md
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.771521 proximl-0.5.7/examples/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:15.000000 proximl-0.5.7/examples/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2024-04-26 21:06:15.000000 proximl-0.5.7/examples/create_dataset_and_training_job.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2024-04-26 21:06:15.000000 proximl-0.5.7/examples/local_storage.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2024-04-26 21:06:15.000000 proximl-0.5.7/examples/training_inference_pipeline.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.775450 proximl-0.5.7/proximl/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      432 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)       59 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/__main__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26565 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8430 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/checkpoints.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.778289 proximl-0.5.7/proximl/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4346 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/checkpoint.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.780049 proximl-0.5.7/proximl/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      592 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3606 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/cloudbender/data_connector.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/cloudbender/datastore.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3453 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/cloudbender/device.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/cloudbender/node.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/cloudbender/provider.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/cloudbender/region.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3147 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/cloudbender/service.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/connection.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6871 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/dataset.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/environment.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      883 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/gpu.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.780475 proximl-0.5.7/proximl/cli/job/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/job/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    34288 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/job/create.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6111 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/model.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3314 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/project.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6246 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/volume.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.783110 proximl-0.5.7/proximl/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)       64 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      717 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/cloudbender.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3297 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/data_connectors.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3506 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/datastores.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3399 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/device_configs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5660 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/devices.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4332 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/nodes.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2036 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/providers.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3570 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/regions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5126 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/services.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    20035 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/connections.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8249 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/datasets.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/environments.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4094 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1901 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/gpu_types.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    18056 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/jobs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7961 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/models.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6585 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/projects.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    10864 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/proximl.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8312 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/volumes.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.776254 proximl-0.5.7/proximl.egg-info/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-04-26 21:07:09.000000 proximl-0.5.7/proximl.egg-info/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3619 2024-04-26 21:07:09.000000 proximl-0.5.7/proximl.egg-info/SOURCES.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)        1 2024-04-26 21:07:09.000000 proximl-0.5.7/proximl.egg-info/dependency_links.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       63 2024-04-26 21:07:09.000000 proximl-0.5.7/proximl.egg-info/entry_points.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       67 2024-04-26 21:07:09.000000 proximl-0.5.7/proximl.egg-info/requires.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       23 2024-04-26 21:07:09.000000 proximl-0.5.7/proximl.egg-info/top_level.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1037 2024-04-26 21:06:15.000000 proximl-0.5.7/pyproject.toml
+-rw-r--r--   0 akowalsk   (501) staff       (20)       38 2024-04-26 21:07:09.794242 proximl-0.5.7/setup.cfg
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1225 2024-04-26 21:06:15.000000 proximl-0.5.7/setup.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.769940 proximl-0.5.7/tests/
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.784846 proximl-0.5.7/tests/integration/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.785074 proximl-0.5.7/tests/integration/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/cloudbender/test_providers_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3230 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/test_checkpoints_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3499 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/test_datasets_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/test_environments_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/test_gpu_types_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    25117 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/test_jobs_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2902 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/test_models_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1446 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/test_projects_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3270 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/test_volumes_integration.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.788187 proximl-0.5.7/tests/unit/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.790012 proximl-0.5.7/tests/unit/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.791510 proximl-0.5.7/tests/unit/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1342 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_device_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_node_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      781 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_provider_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_region_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1311 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_service_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      236 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      702 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/test_cli_checkpoint_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      653 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/test_cli_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      683 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/test_cli_environment_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      650 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/test_cli_gpu_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      611 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/test_cli_job_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      629 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/test_cli_model_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1688 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/test_cli_project_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      644 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/test_cli_volume_unit.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.793670 proximl-0.5.7/tests/unit/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5783 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cloudbender/test_data_connectors_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5398 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cloudbender/test_datastores_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5714 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cloudbender/test_device_configs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     9103 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cloudbender/test_devices_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6231 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cloudbender/test_nodes_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4373 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cloudbender/test_providers_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6299 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cloudbender/test_regions_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5220 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cloudbender/test_services_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    31129 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      858 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_checkpoints_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_connections_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_environments_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      906 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_gpu_types_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_jobs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_models_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    10743 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_projects_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_proximl.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15305 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_volumes_unit.py
```

### Comparing `proximl-0.5.6/LICENSE` & `proximl-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/PKG-INFO` & `proximl-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proximl
-Version: 0.5.6
+Version: 0.5.7
 Summary: proxiML client SDK and command line utilities
 Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML
 Author-email: support@proximl.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.proximl.ai/"><img src="https://www.proximl.ai/static/img/proxiML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proximl Version: 0.5.6 Summary: proxiML client SDK
+Metadata-Version: 2.1 Name: proximl Version: 0.5.7 Summary: proxiML client SDK
 and command line utilities Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML Author-email: support@proximl.ai License: MIT Description:
           _[_h_t_t_p_s_:_/_/_w_w_w_._p_r_o_x_i_m_l_._a_i_/_s_t_a_t_i_c_/_i_m_g_/_p_r_o_x_i_M_L_-_l_o_g_o_-_p_u_r_p_l_e_._p_n_g_]
 # proxiML Python SDK and Command Line Tools Provides programmatic access to
 [proxiML platform](https://app.proximl.ai). ## Installation Python 3.8 or above
 is required. ``` pip install proximl ``` ## Authentication ### Prerequisites
 You must have a valid [proxiML account](https://app.proximl.ai). On the
```

### Comparing `proximl-0.5.6/README.md` & `proximl-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/examples/create_dataset_and_training_job.py` & `proximl-0.5.7/examples/create_dataset_and_training_job.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/examples/local_storage.py` & `proximl-0.5.7/examples/local_storage.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/examples/training_inference_pipeline.py` & `proximl-0.5.7/examples/training_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/auth.py` & `proximl-0.5.7/proximl/auth.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/checkpoints.py` & `proximl-0.5.7/proximl/checkpoints.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,32 +19,29 @@
 
     async def get(self, id, **kwargs):
         resp = await self.proximl._query(f"/checkpoint/{id}", "GET", kwargs)
         return Checkpoint(self.proximl, **resp)
 
     async def list(self, **kwargs):
         resp = await self.proximl._query(f"/checkpoint", "GET", kwargs)
-        checkpoints = [
-            Checkpoint(self.proximl, **checkpoint) for checkpoint in resp
-        ]
+        checkpoints = [Checkpoint(self.proximl, **checkpoint) for checkpoint in resp]
         return checkpoints
 
     async def list_public(self, **kwargs):
         resp = await self.proximl._query(f"/checkpoint/public", "GET", kwargs)
         datasets = [Checkpoint(self.proximl, **dataset) for dataset in resp]
         return datasets
 
     async def create(self, name, source_type, source_uri, **kwargs):
         data = dict(
             name=name,
             source_type=source_type,
             source_uri=source_uri,
             source_options=kwargs.get("source_options"),
-            project_uuid=kwargs.get("project_uuid")
-            or self.proximl.active_project,
+            project_uuid=kwargs.get("project_uuid") or self.proximl.active_project,
         )
         payload = {k: v for k, v in data.items() if v is not None}
         logging.info(f"Creating Checkpoint {name}")
         resp = await self.proximl._query("/checkpoint", "POST", None, payload)
         checkpoint = Checkpoint(self.proximl, **resp)
         logging.info(f"Created Checkpoint {name} with id {checkpoint.id}")
 
@@ -56,17 +53,15 @@
         )
 
 
 class Checkpoint:
     def __init__(self, proximl, **kwargs):
         self.proximl = proximl
         self._checkpoint = kwargs
-        self._id = self._checkpoint.get(
-            "id", self._checkpoint.get("checkpoint_uuid")
-        )
+        self._id = self._checkpoint.get("id", self._checkpoint.get("checkpoint_uuid"))
         self._status = self._checkpoint.get("status")
         self._name = self._checkpoint.get("name")
         self._size = self._checkpoint.get("size")
         self._project_uuid = self._checkpoint.get("project_uuid")
 
     @property
     def id(self) -> str:
@@ -119,23 +114,25 @@
 
     def get_connection_details(self):
         if self._checkpoint.get("vpn"):
             details = dict(
                 entity_type="checkpoint",
                 project_uuid=self._checkpoint.get("project_uuid"),
                 cidr=self._checkpoint.get("vpn").get("cidr"),
-                ssh_port=self._checkpoint.get("vpn")
-                .get("client")
-                .get("ssh_port"),
-                input_path=self._checkpoint.get("source_uri")
-                if self.status in ["new", "downloading"]
-                else None,
-                output_path=self._checkpoint.get("output_uri")
-                if self.status == "exporting"
-                else None,
+                ssh_port=self._checkpoint.get("vpn").get("client").get("ssh_port"),
+                input_path=(
+                    self._checkpoint.get("source_uri")
+                    if self.status in ["new", "downloading"]
+                    else None
+                ),
+                output_path=(
+                    self._checkpoint.get("output_uri")
+                    if self.status == "exporting"
+                    else None
+                ),
             )
         else:
             details = dict()
         return details
 
     async def connect(self):
         if self.status in ["ready", "failed"]:
@@ -191,17 +188,15 @@
 
     def _get_msg_handler(self, msg_handler):
         def handler(data):
             if data.get("type") == "subscription":
                 if msg_handler:
                     msg_handler(data)
                 else:
-                    timestamp = datetime.fromtimestamp(
-                        int(data.get("time")) / 1000
-                    )
+                    timestamp = datetime.fromtimestamp(int(data.get("time")) / 1000)
                     print(
                         f"{timestamp.strftime('%m/%d/%Y, %H:%M:%S')}: {data.get('msg').rstrip()}"
                     )
 
         return handler
 
     async def attach(self, msg_handler=None):
@@ -220,27 +215,32 @@
             "GET",
             dict(project_uuid=self._project_uuid),
         )
         self.__init__(self.proximl, **resp)
         return self
 
     async def wait_for(self, status, timeout=300):
+        if self.status == status:
+            return
         valid_statuses = ["downloading", "ready", "archived"]
         if not status in valid_statuses:
             raise SpecificationError(
                 "status",
                 f"Invalid wait_for status {status}.  Valid statuses are: {valid_statuses}",
             )
-        if self.status == status:
-            return
+
+        MAX_TIMEOUT = 24 * 60 * 60
+        if timeout > MAX_TIMEOUT:
+            raise SpecificationError(
+                "timeout",
+                f"timeout must be less than {MAX_TIMEOUT} seconds.",
+            )
         POLL_INTERVAL_MIN = 5
         POLL_INTERVAL_MAX = 60
-        POLL_INTERVAL = max(
-            min(timeout / 60, POLL_INTERVAL_MAX), POLL_INTERVAL_MIN
-        )
+        POLL_INTERVAL = max(min(timeout / 60, POLL_INTERVAL_MAX), POLL_INTERVAL_MIN)
         retry_count = math.ceil(timeout / POLL_INTERVAL)
         count = 0
         while count < retry_count:
             await asyncio.sleep(POLL_INTERVAL)
             try:
                 await self.refresh()
             except ApiError as e:
```

### Comparing `proximl-0.5.6/proximl/cli/__init__.py` & `proximl-0.5.7/proximl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cli/checkpoint.py` & `proximl-0.5.7/proximl/cli/checkpoint.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cli/cloudbender/__init__.py` & `proximl-0.5.7/proximl/cli/cloudbender/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,8 +11,9 @@
 
 
 from proximl.cli.cloudbender.provider import provider
 from proximl.cli.cloudbender.region import region
 from proximl.cli.cloudbender.node import node
 from proximl.cli.cloudbender.device import device
 from proximl.cli.cloudbender.datastore import datastore
+from proximl.cli.cloudbender.data_connector import data_connector
 from proximl.cli.cloudbender.service import service
```

### Comparing `proximl-0.5.6/proximl/cli/cloudbender/datastore.py` & `proximl-0.5.7/proximl/cli/cloudbender/datastore.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cli/cloudbender/device.py` & `proximl-0.5.7/proximl/cli/cloudbender/device.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cli/cloudbender/node.py` & `proximl-0.5.7/proximl/cli/cloudbender/node.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cli/cloudbender/provider.py` & `proximl-0.5.7/proximl/cli/cloudbender/provider.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cli/cloudbender/region.py` & `proximl-0.5.7/proximl/cli/cloudbender/region.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cli/cloudbender/service.py` & `proximl-0.5.7/proximl/cli/cloudbender/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,28 +71,45 @@
     "--region",
     "-r",
     type=click.STRING,
     required=True,
     help="The region ID to create the service in.",
 )
 @click.option(
+    "--type",
+    "-t",
+    type=click.Choice(
+        [
+            "https",
+            "tcp",
+            "udp",
+        ],
+    ),
+    required=True,
+    help="The type of regional service.",
+)
+@click.option(
     "--public/--no-public",
     default=True,
     show_default=True,
     help="Service should be accessible from the public internet.",
 )
 @click.argument("name", type=click.STRING, required=True)
 @pass_config
-def create(config, provider, region, public, name):
+def create(config, provider, region, type, public, name):
     """
     Creates a service.
     """
     return config.proximl.run(
         config.proximl.client.cloudbender.services.create(
-            provider_uuid=provider, region_uuid=region, name=name, public=public
+            provider_uuid=provider,
+            region_uuid=region,
+            name=name,
+            type=type,
+            public=public,
         )
     )
 
 
 @service.command()
 @click.option(
     "--provider",
```

### Comparing `proximl-0.5.6/proximl/cli/connection.py` & `proximl-0.5.7/proximl/cli/connection.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cli/dataset.py` & `proximl-0.5.7/proximl/cli/dataset.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cli/environment.py` & `proximl-0.5.7/proximl/cli/environment.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cli/gpu.py` & `proximl-0.5.7/proximl/cli/gpu.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cli/job/__init__.py` & `proximl-0.5.7/proximl/cli/job/__init__.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cli/job/create.py` & `proximl-0.5.7/proximl/cli/job/create.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cli/model.py` & `proximl-0.5.7/proximl/cli/model.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cli/project.py` & `proximl-0.5.7/proximl/cli/project.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cli/volume.py` & `proximl-0.5.7/proximl/cli/volume.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cloudbender/cloudbender.py` & `proximl-0.5.7/proximl/cloudbender/cloudbender.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from .providers import Providers
 from .regions import Regions
 from .nodes import Nodes
 from .devices import Devices
 from .datastores import Datastores
+from .data_connectors import DataConnectors
 from .services import Services
 from .device_configs import DeviceConfigs
 
 
 class Cloudbender(object):
     def __init__(self, proximl):
         self.proximl = proximl
         self.providers = Providers(proximl)
         self.regions = Regions(proximl)
         self.nodes = Nodes(proximl)
         self.devices = Devices(proximl)
         self.datastores = Datastores(proximl)
+        self.data_connectors = DataConnectors(proximl)
         self.services = Services(proximl)
         self.device_configs = DeviceConfigs(proximl)
```

### Comparing `proximl-0.5.6/proximl/cloudbender/datastores.py` & `proximl-0.5.7/proximl/cloudbender/datastores.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cloudbender/device_configs.py` & `proximl-0.5.7/proximl/cloudbender/device_configs.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cloudbender/devices.py` & `proximl-0.5.7/proximl/cloudbender/devices.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cloudbender/nodes.py` & `proximl-0.5.7/proximl/cloudbender/nodes.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cloudbender/providers.py` & `proximl-0.5.7/proximl/cloudbender/providers.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cloudbender/regions.py` & `proximl-0.5.7/proximl/cloudbender/regions.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/cloudbender/services.py` & `proximl-0.5.7/proximl/cloudbender/data_connectors.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,115 +1,112 @@
 import json
 import logging
 
 
-class Services(object):
+class DataConnectors(object):
     def __init__(self, proximl):
         self.proximl = proximl
 
     async def get(self, provider_uuid, region_uuid, id, **kwargs):
         resp = await self.proximl._query(
-            f"/provider/{provider_uuid}/region/{region_uuid}/service/{id}",
+            f"/provider/{provider_uuid}/region/{region_uuid}/data_connector/{id}",
             "GET",
             kwargs,
         )
-        return Service(self.proximl, **resp)
+        return DataConnector(self.proximl, **resp)
 
     async def list(self, provider_uuid, region_uuid, **kwargs):
         resp = await self.proximl._query(
-            f"/provider/{provider_uuid}/region/{region_uuid}/service",
+            f"/provider/{provider_uuid}/region/{region_uuid}/data_connector",
             "GET",
             kwargs,
         )
-        services = [Service(self.proximl, **service) for service in resp]
-        return services
+        data_connectors = [
+            DataConnector(self.proximl, **data_connector) for data_connector in resp
+        ]
+        return data_connectors
 
     async def create(
         self,
         provider_uuid,
         region_uuid,
         name,
-        public,
+        type,
         **kwargs,
     ):
-        logging.info(f"Creating Service {name}")
+        logging.info(f"Creating Data Connector {name}")
         data = dict(
             name=name,
-            public=public,
+            type=type,
             **kwargs,
         )
         payload = {k: v for k, v in data.items() if v is not None}
         resp = await self.proximl._query(
-            f"/provider/{provider_uuid}/region/{region_uuid}/service",
+            f"/provider/{provider_uuid}/region/{region_uuid}/data_connector",
             "POST",
             None,
             payload,
         )
-        service = Service(self.proximl, **resp)
-        logging.info(f"Created Service {name} with id {service.id}")
-        return service
+        data_connector = DataConnector(self.proximl, **resp)
+        logging.info(f"Created Data Connector {name} with id {data_connector.id}")
+        return data_connector
 
     async def remove(self, provider_uuid, region_uuid, id, **kwargs):
         await self.proximl._query(
-            f"/provider/{provider_uuid}/region/{region_uuid}/service/{id}",
+            f"/provider/{provider_uuid}/region/{region_uuid}/data_connector/{id}",
             "DELETE",
             kwargs,
         )
 
 
-class Service:
+class DataConnector:
     def __init__(self, proximl, **kwargs):
         self.proximl = proximl
-        self._service = kwargs
-        self._id = self._service.get("service_id")
-        self._provider_uuid = self._service.get("provider_uuid")
-        self._region_uuid = self._service.get("region_uuid")
-        self._public = self._service.get("public")
-        self._name = self._service.get("name")
-        self._hostname = self._service.get("hostname")
+        self._data_connector = kwargs
+        self._id = self._data_connector.get("connector_id")
+        self._provider_uuid = self._data_connector.get("provider_uuid")
+        self._region_uuid = self._data_connector.get("region_uuid")
+        self._type = self._data_connector.get("type")
+        self._name = self._data_connector.get("name")
 
     @property
     def id(self) -> str:
         return self._id
 
     @property
     def provider_uuid(self) -> str:
         return self._provider_uuid
 
     @property
     def region_uuid(self) -> str:
         return self._region_uuid
 
     @property
-    def public(self) -> bool:
-        return self._public
+    def type(self) -> str:
+        return self._type
 
     @property
     def name(self) -> str:
         return self._name
 
-    @property
-    def hostname(self) -> str:
-        return self._hostname
-
     def __str__(self):
-        return json.dumps({k: v for k, v in self._service.items()})
+        return json.dumps({k: v for k, v in self._data_connector.items()})
 
     def __repr__(self):
-        return f"Service( proximl , **{self._service.__repr__()})"
+        return f"DataConnector( proximl , **{self._data_connector.__repr__()})"
 
     def __bool__(self):
         return bool(self._id)
 
     async def remove(self):
         await self.proximl._query(
-            f"/provider/{self._provider_uuid}/region/{self._region_uuid}/service/{self._id}",
+            f"/provider/{self._provider_uuid}/region/{self._region_uuid}/data_connector/{self._id}",
             "DELETE",
         )
 
     async def refresh(self):
         resp = await self.proximl._query(
-            f"/provider/{self._provider_uuid}/region/{self._region_uuid}/service/{self._id}",
+            f"/provider/{self._provider_uuid}/region/{self._region_uuid}/data_connector/{self._id}",
             "GET",
         )
         self.__init__(self.proximl, **resp)
         return self
```

### Comparing `proximl-0.5.6/proximl/connections.py` & `proximl-0.5.7/proximl/connections.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/datasets.py` & `proximl-0.5.7/proximl/datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,20 +115,24 @@
     def get_connection_details(self):
         if self._dataset.get("vpn"):
             details = dict(
                 entity_type="dataset",
                 project_uuid=self._dataset.get("project_uuid"),
                 cidr=self._dataset.get("vpn").get("cidr"),
                 ssh_port=self._dataset.get("vpn").get("client").get("ssh_port"),
-                input_path=self._dataset.get("source_uri")
-                if self.status in ["new", "downloading"]
-                else None,
-                output_path=self._dataset.get("output_uri")
-                if self.status == "exporting"
-                else None,
+                input_path=(
+                    self._dataset.get("source_uri")
+                    if self.status in ["new", "downloading"]
+                    else None
+                ),
+                output_path=(
+                    self._dataset.get("output_uri")
+                    if self.status == "exporting"
+                    else None
+                ),
             )
         else:
             details = dict()
         return details
 
     async def connect(self):
         if self.status in ["ready", "failed"]:
@@ -211,22 +215,29 @@
             "GET",
             dict(project_uuid=self._project_uuid),
         )
         self.__init__(self.proximl, **resp)
         return self
 
     async def wait_for(self, status, timeout=300):
+        if self.status == status:
+            return
         valid_statuses = ["downloading", "ready", "archived"]
         if not status in valid_statuses:
             raise SpecificationError(
                 "status",
                 f"Invalid wait_for status {status}.  Valid statuses are: {valid_statuses}",
             )
-        if self.status == status:
-            return
+        MAX_TIMEOUT = 24 * 60 * 60
+        if timeout > MAX_TIMEOUT:
+            raise SpecificationError(
+                "timeout",
+                f"timeout must be less than {MAX_TIMEOUT} seconds.",
+            )
+
         POLL_INTERVAL_MIN = 5
         POLL_INTERVAL_MAX = 60
         POLL_INTERVAL = max(min(timeout / 60, POLL_INTERVAL_MAX), POLL_INTERVAL_MIN)
         retry_count = math.ceil(timeout / POLL_INTERVAL)
         count = 0
         while count < retry_count:
             await asyncio.sleep(POLL_INTERVAL)
```

### Comparing `proximl-0.5.6/proximl/environments.py` & `proximl-0.5.7/proximl/environments.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/exceptions.py` & `proximl-0.5.7/proximl/exceptions.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/gpu_types.py` & `proximl-0.5.7/proximl/gpu_types.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/jobs.py` & `proximl-0.5.7/proximl/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,14 +464,20 @@
             model=kwargs.get("model"),
             source_job_uuid=self.id,
         )
         logging.debug(f"copy result: {job}")
         return job
 
     async def wait_for(self, status, timeout=300):
+        if self.status == status or (
+            self.type == "training"
+            and status == "finished"
+            and self.status == "stopped"
+        ):
+            return
         valid_statuses = [
             "waiting for data/model download",
             "waiting for GPUs",
             "waiting for resources",
             "running",
             "stopped",
             "finished",
@@ -488,20 +494,21 @@
                 DeprecationWarning,
             )
         if (self.type == "training") and status == "stopped":
             warnings.warn(
                 "'stopped' status is deprecated for training jobs, use 'finished' instead.",
                 DeprecationWarning,
             )
-        if self.status == status or (
-            self.type == "training"
-            and status == "finished"
-            and self.status == "stopped"
-        ):
-            return
+
+        MAX_TIMEOUT = 24 * 60 * 60
+        if timeout > MAX_TIMEOUT:
+            raise SpecificationError(
+                "timeout",
+                f"timeout must be less than {MAX_TIMEOUT} seconds.",
+            )
 
         POLL_INTERVAL_MIN = 5
         POLL_INTERVAL_MAX = 60
         POLL_INTERVAL = max(min(timeout / 60, POLL_INTERVAL_MAX), POLL_INTERVAL_MIN)
         retry_count = math.ceil(timeout / POLL_INTERVAL)
         count = 0
         while count < retry_count:
```

### Comparing `proximl-0.5.6/proximl/models.py` & `proximl-0.5.7/proximl/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,29 +28,26 @@
 
     async def create(self, name, source_type, source_uri, **kwargs):
         data = dict(
             name=name,
             source_type=source_type,
             source_uri=source_uri,
             source_options=kwargs.get("source_options"),
-            project_uuid=kwargs.get("project_uuid")
-            or self.proximl.active_project,
+            project_uuid=kwargs.get("project_uuid") or self.proximl.active_project,
         )
         payload = {k: v for k, v in data.items() if v is not None}
         logging.info(f"Creating Model {name}")
         resp = await self.proximl._query("/model", "POST", None, payload)
         model = Model(self.proximl, **resp)
         logging.info(f"Created Model {name} with id {model.id}")
 
         return model
 
     async def remove(self, id, **kwargs):
-        await self.proximl._query(
-            f"/model/{id}", "DELETE", dict(**kwargs, force=True)
-        )
+        await self.proximl._query(f"/model/{id}", "DELETE", dict(**kwargs, force=True))
 
 
 class Model:
     def __init__(self, proximl, **kwargs):
         self.proximl = proximl
         self._model = kwargs
         self._id = self._model.get("id", self._model.get("model_uuid"))
@@ -111,20 +108,24 @@
     def get_connection_details(self):
         if self._model.get("vpn"):
             details = dict(
                 entity_type="model",
                 project_uuid=self._model.get("project_uuid"),
                 cidr=self._model.get("vpn").get("cidr"),
                 ssh_port=self._model.get("vpn").get("client").get("ssh_port"),
-                input_path=self._model.get("source_uri")
-                if self.status in ["new", "downloading"]
-                else None,
-                output_path=self._model.get("output_uri")
-                if self.status == "exporting"
-                else None,
+                input_path=(
+                    self._model.get("source_uri")
+                    if self.status in ["new", "downloading"]
+                    else None
+                ),
+                output_path=(
+                    self._model.get("output_uri")
+                    if self.status == "exporting"
+                    else None
+                ),
             )
         else:
             details = dict()
         logging.debug(f"Connection Details: {details}")
         return details
 
     async def connect(self):
@@ -181,17 +182,15 @@
 
     def _get_msg_handler(self, msg_handler):
         def handler(data):
             if data.get("type") == "subscription":
                 if msg_handler:
                     msg_handler(data)
                 else:
-                    timestamp = datetime.fromtimestamp(
-                        int(data.get("time")) / 1000
-                    )
+                    timestamp = datetime.fromtimestamp(int(data.get("time")) / 1000)
                     print(
                         f"{timestamp.strftime('%m/%d/%Y, %H:%M:%S')}: {data.get('msg').rstrip()}"
                     )
 
         return handler
 
     async def attach(self, msg_handler=None):
@@ -210,27 +209,31 @@
             "GET",
             dict(project_uuid=self._project_uuid),
         )
         self.__init__(self.proximl, **resp)
         return self
 
     async def wait_for(self, status, timeout=300):
+        if self.status == status:
+            return
         valid_statuses = ["downloading", "ready", "archived"]
         if not status in valid_statuses:
             raise SpecificationError(
                 "status",
                 f"Invalid wait_for status {status}.  Valid statuses are: {valid_statuses}",
             )
-        if self.status == status:
-            return
+        MAX_TIMEOUT = 24 * 60 * 60
+        if timeout > MAX_TIMEOUT:
+            raise SpecificationError(
+                "timeout",
+                f"timeout must be less than {MAX_TIMEOUT} seconds.",
+            )
         POLL_INTERVAL_MIN = 5
         POLL_INTERVAL_MAX = 60
-        POLL_INTERVAL = max(
-            min(timeout / 60, POLL_INTERVAL_MAX), POLL_INTERVAL_MIN
-        )
+        POLL_INTERVAL = max(min(timeout / 60, POLL_INTERVAL_MAX), POLL_INTERVAL_MIN)
         retry_count = math.ceil(timeout / POLL_INTERVAL)
         count = 0
         while count < retry_count:
             await asyncio.sleep(POLL_INTERVAL)
             try:
                 await self.refresh()
             except ApiError as e:
```

### Comparing `proximl-0.5.6/proximl/projects.py` & `proximl-0.5.7/proximl/projects.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,20 @@
     def __init__(self, proximl):
         self.proximl = proximl
 
     async def get(self, id, **kwargs):
         resp = await self.proximl._query(f"/project/{id}", "GET", kwargs)
         return Project(self.proximl, **resp)
 
+    async def get_current(self, **kwargs):
+        resp = await self.proximl._query(
+            f"/project/{self.proximl.project}", "GET", kwargs
+        )
+        return Project(self.proximl, **resp)
+
     async def list(self, **kwargs):
         resp = await self.proximl._query(f"/project", "GET", kwargs)
         projects = [Project(self.proximl, **project) for project in resp]
         return projects
 
     async def create(self, name, copy_keys=False, **kwargs):
         data = dict(
@@ -68,24 +74,63 @@
     def __repr__(self):
         return f"ProjectDatastore( proximl , **{self._datastore.__repr__()})"
 
     def __bool__(self):
         return bool(self._id)
 
 
+class ProjectDataConnector:
+    def __init__(self, proximl, **kwargs):
+        self.proximl = proximl
+        self._data_connector = kwargs
+        self._id = self._data_connector.get("id")
+        self._project_uuid = self._data_connector.get("project_uuid")
+        self._name = self._data_connector.get("name")
+        self._type = self._data_connector.get("type")
+        self._region_uuid = self._data_connector.get("region_uuid")
+
+    @property
+    def id(self) -> str:
+        return self._id
+
+    @property
+    def project_uuid(self) -> str:
+        return self._project_uuid
+
+    @property
+    def name(self) -> str:
+        return self._name
+
+    @property
+    def type(self) -> str:
+        return self._type
+
+    @property
+    def region_uuid(self) -> str:
+        return self._region_uuid
+
+    def __str__(self):
+        return json.dumps({k: v for k, v in self._data_connector.items()})
+
+    def __repr__(self):
+        return f"ProjectDataConnector( proximl , **{self._data_connector.__repr__()})"
+
+    def __bool__(self):
+        return bool(self._id)
+
+
 class ProjectService:
     def __init__(self, proximl, **kwargs):
         self.proximl = proximl
         self._service = kwargs
         self._id = self._service.get("id")
         self._project_uuid = self._service.get("project_uuid")
         self._name = self._service.get("name")
-        self._type = self._service.get("type")
         self._hostname = self._service.get("hostname")
-        self._resource = self._service.get("resource")
+        self._public = self._service.get("public")
         self._region_uuid = self._service.get("region_uuid")
 
     @property
     def id(self) -> str:
         return self._id
 
     @property
@@ -93,24 +138,20 @@
         return self._project_uuid
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
-    def type(self) -> str:
-        return self._type
-
-    @property
     def hostname(self) -> str:
         return self._hostname
 
     @property
-    def resource(self) -> str:
-        return self._resource
+    def public(self) -> bool:
+        return self._public
 
     @property
     def region_uuid(self) -> str:
         return self._region_uuid
 
     def __str__(self):
         return json.dumps({k: v for k, v in self._service.items()})
@@ -160,17 +201,28 @@
         await self.proximl._query(f"/project/{self._id}", "DELETE")
 
     async def list_datastores(self):
         resp = await self.proximl._query(f"/project/{self._id}/datastores", "GET")
         datastores = [ProjectDatastore(self.proximl, **datastore) for datastore in resp]
         return datastores
 
+    async def list_data_connectors(self):
+        resp = await self.proximl._query(f"/project/{self._id}/data_connectors", "GET")
+        data_connectors = [
+            ProjectDataConnector(self.proximl, **data_connector)
+            for data_connector in resp
+        ]
+        return data_connectors
+
     async def list_services(self):
         resp = await self.proximl._query(f"/project/{self._id}/services", "GET")
         services = [ProjectService(self.proximl, **service) for service in resp]
         return services
 
     async def refresh_datastores(self):
         await self.proximl._query(f"/project/{self._id}/datastores", "PATCH")
 
+    async def refresh_data_connectors(self):
+        await self.proximl._query(f"/project/{self._id}/data_connectors", "PATCH")
+
     async def refresh_services(self):
         await self.proximl._query(f"/project/{self._id}/services", "PATCH")
```

### Comparing `proximl-0.5.6/proximl/proximl.py` & `proximl-0.5.7/proximl/proximl.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/proximl/volumes.py` & `proximl-0.5.7/proximl/volumes.py`

 * *Files 5% similar despite different names*

```diff
@@ -219,22 +219,29 @@
             "GET",
             dict(project_uuid=self._project_uuid),
         )
         self.__init__(self.proximl, **resp)
         return self
 
     async def wait_for(self, status, timeout=300):
+        if self.status == status:
+            return
         valid_statuses = ["downloading", "ready", "archived"]
         if not status in valid_statuses:
             raise SpecificationError(
                 "status",
                 f"Invalid wait_for status {status}.  Valid statuses are: {valid_statuses}",
             )
-        if self.status == status:
-            return
+
+        MAX_TIMEOUT = 24 * 60 * 60
+        if timeout > MAX_TIMEOUT:
+            raise SpecificationError(
+                "timeout",
+                f"timeout must be less than {MAX_TIMEOUT} seconds.",
+            )
         POLL_INTERVAL_MIN = 5
         POLL_INTERVAL_MAX = 60
         POLL_INTERVAL = max(min(timeout / 60, POLL_INTERVAL_MAX), POLL_INTERVAL_MIN)
         retry_count = math.ceil(timeout / POLL_INTERVAL)
         count = 0
         while count < retry_count:
             await asyncio.sleep(POLL_INTERVAL)
```

### Comparing `proximl-0.5.6/proximl.egg-info/PKG-INFO` & `proximl-0.5.7/proximl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proximl
-Version: 0.5.6
+Version: 0.5.7
 Summary: proxiML client SDK and command line utilities
 Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML
 Author-email: support@proximl.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.proximl.ai/"><img src="https://www.proximl.ai/static/img/proxiML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proximl Version: 0.5.6 Summary: proxiML client SDK
+Metadata-Version: 2.1 Name: proximl Version: 0.5.7 Summary: proxiML client SDK
 and command line utilities Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML Author-email: support@proximl.ai License: MIT Description:
           _[_h_t_t_p_s_:_/_/_w_w_w_._p_r_o_x_i_m_l_._a_i_/_s_t_a_t_i_c_/_i_m_g_/_p_r_o_x_i_M_L_-_l_o_g_o_-_p_u_r_p_l_e_._p_n_g_]
 # proxiML Python SDK and Command Line Tools Provides programmatic access to
 [proxiML platform](https://app.proximl.ai). ## Installation Python 3.8 or above
 is required. ``` pip install proximl ``` ## Authentication ### Prerequisites
 You must have a valid [proxiML account](https://app.proximl.ai). On the
```

### Comparing `proximl-0.5.6/proximl.egg-info/SOURCES.txt` & `proximl-0.5.7/proximl.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -32,24 +32,26 @@
 proximl/cli/dataset.py
 proximl/cli/environment.py
 proximl/cli/gpu.py
 proximl/cli/model.py
 proximl/cli/project.py
 proximl/cli/volume.py
 proximl/cli/cloudbender/__init__.py
+proximl/cli/cloudbender/data_connector.py
 proximl/cli/cloudbender/datastore.py
 proximl/cli/cloudbender/device.py
 proximl/cli/cloudbender/node.py
 proximl/cli/cloudbender/provider.py
 proximl/cli/cloudbender/region.py
 proximl/cli/cloudbender/service.py
 proximl/cli/job/__init__.py
 proximl/cli/job/create.py
 proximl/cloudbender/__init__.py
 proximl/cloudbender/cloudbender.py
+proximl/cloudbender/data_connectors.py
 proximl/cloudbender/datastores.py
 proximl/cloudbender/device_configs.py
 proximl/cloudbender/devices.py
 proximl/cloudbender/nodes.py
 proximl/cloudbender/providers.py
 proximl/cloudbender/regions.py
 proximl/cloudbender/services.py
@@ -91,16 +93,17 @@
 tests/unit/cli/test_cli_volume_unit.py
 tests/unit/cli/cloudbender/__init__.py
 tests/unit/cli/cloudbender/test_cli_datastore_unit.py
 tests/unit/cli/cloudbender/test_cli_device_unit.py
 tests/unit/cli/cloudbender/test_cli_node_unit.py
 tests/unit/cli/cloudbender/test_cli_provider_unit.py
 tests/unit/cli/cloudbender/test_cli_region_unit.py
-tests/unit/cli/cloudbender/test_cli_reservation_unit.py
+tests/unit/cli/cloudbender/test_cli_service_unit.py
 tests/unit/cloudbender/__init__.py
+tests/unit/cloudbender/test_data_connectors_unit.py
 tests/unit/cloudbender/test_datastores_unit.py
 tests/unit/cloudbender/test_device_configs_unit.py
 tests/unit/cloudbender/test_devices_unit.py
 tests/unit/cloudbender/test_nodes_unit.py
 tests/unit/cloudbender/test_providers_unit.py
 tests/unit/cloudbender/test_regions_unit.py
 tests/unit/cloudbender/test_services_unit.py
```

### Comparing `proximl-0.5.6/pyproject.toml` & `proximl-0.5.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "projects: Projects tests",
     "cloudbender: CloudBender tests",
     "providers: Providers tests",
     "regions: Regions tests",
     "nodes: Nodes tests",
     "devices: Devices tests",
     "datastores: Datastores tests",
+    "data_connectors: Data Connector tests",
     "services: Services tests",
     "device_configs: DeviceConfigs tests",
     "unit: All unit tests (no proxiML environment required)",
     "integration: All integration tests (proxiML environment required)",
     "sdk: All tests of the SDK",
     "cli: All test of the cli",
 ]
```

### Comparing `proximl-0.5.6/setup.py` & `proximl-0.5.7/setup.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/integration/cloudbender/test_providers_integration.py` & `proximl-0.5.7/tests/integration/cloudbender/test_providers_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/integration/conftest.py` & `proximl-0.5.7/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/integration/test_checkpoints_integration.py` & `proximl-0.5.7/tests/integration/test_checkpoints_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/integration/test_datasets_integration.py` & `proximl-0.5.7/tests/integration/test_datasets_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/integration/test_environments_integration.py` & `proximl-0.5.7/tests/integration/test_environments_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/integration/test_gpu_types_integration.py` & `proximl-0.5.7/tests/integration/test_gpu_types_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/integration/test_jobs_integration.py` & `proximl-0.5.7/tests/integration/test_jobs_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,27 @@
 import sys
 import tempfile
 import os
 import asyncio
 import aiohttp
 from pytest import mark, fixture, raises
 from proximl.exceptions import ApiError
+from urllib.parse import urlparse
 
 pytestmark = [mark.sdk, mark.integration, mark.jobs]
 
 
+def extract_domain_suffix(hostname):
+    parts = hostname.split(".")
+    if len(parts) >= 2:
+        return ".".join(parts[-2:])
+    else:
+        return None
+
+
 @fixture(scope="class")
 async def job(proximl):
     job = await proximl.jobs.create(
         name="CLI Automated Tests - Job Lifecycle",
         type="notebook",
         gpu_types=["gtx1060"],
         gpu_count=1,
@@ -30,14 +39,16 @@
 @mark.create
 @mark.asyncio
 class JobLifeCycleTests:
     async def test_wait_for_running(self, job):
         assert job.status != "running"
         job = await job.wait_for("running")
         assert job.status == "running"
+        assert job.url
+        assert extract_domain_suffix(urlparse(job.url).hostname) == "proximl.cloud"
 
     async def test_stop_job(self, job):
         assert job.status == "running"
         await job.stop()
         job = await job.wait_for("stopped", 120)
         assert job.status == "stopped"
 
@@ -514,14 +525,15 @@
         await new_model.remove()
 
 
 @mark.create
 @mark.asyncio
 class JobTypeTests:
     async def test_endpoint(self, proximl):
+
         job = await proximl.jobs.create(
             "CLI Automated Tests - Endpoint",
             type="endpoint",
             gpu_type="GTX 1060",
             gpu_count=1,
             disk_size=10,
             model=dict(
@@ -540,14 +552,15 @@
                     )
                 ]
             ),
         )
         await job.wait_for("running")
         await job.refresh()
         assert job.url
+        assert extract_domain_suffix(urlparse(job.url).hostname) == "proximl.cloud"
         tries = 0
         await asyncio.sleep(30)
         async with aiohttp.ClientSession() as session:
             retry = True
             while retry:
                 async with session.request(
                     "GET",
```

### Comparing `proximl-0.5.6/tests/integration/test_models_integration.py` & `proximl-0.5.7/tests/integration/test_models_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/integration/test_projects_integration.py` & `proximl-0.5.7/tests/integration/test_projects_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/integration/test_volumes_integration.py` & `proximl-0.5.7/tests/integration/test_volumes_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_datastore_unit.py` & `proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_datastore_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_device_unit.py` & `proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_device_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_node_unit.py` & `proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_node_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_provider_unit.py` & `proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_provider_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_region_unit.py` & `proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_region_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_reservation_unit.py` & `proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_service_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cli/test_cli_checkpoint_unit.py` & `proximl-0.5.7/tests/unit/cli/test_cli_checkpoint_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cli/test_cli_datasets_unit.py` & `proximl-0.5.7/tests/unit/cli/test_cli_datasets_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cli/test_cli_environment_unit.py` & `proximl-0.5.7/tests/unit/cli/test_cli_environment_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cli/test_cli_gpu_unit.py` & `proximl-0.5.7/tests/unit/cli/test_cli_gpu_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cli/test_cli_job_unit.py` & `proximl-0.5.7/tests/unit/cli/test_cli_job_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cli/test_cli_model_unit.py` & `proximl-0.5.7/tests/unit/cli/test_cli_model_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cli/test_cli_project_unit.py` & `proximl-0.5.7/tests/unit/cli/test_cli_project_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cli/test_cli_volume_unit.py` & `proximl-0.5.7/tests/unit/cli/test_cli_volume_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cloudbender/test_datastores_unit.py` & `proximl-0.5.7/tests/unit/cloudbender/test_datastores_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cloudbender/test_device_configs_unit.py` & `proximl-0.5.7/tests/unit/cloudbender/test_device_configs_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cloudbender/test_devices_unit.py` & `proximl-0.5.7/tests/unit/cloudbender/test_devices_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cloudbender/test_nodes_unit.py` & `proximl-0.5.7/tests/unit/cloudbender/test_nodes_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cloudbender/test_providers_unit.py` & `proximl-0.5.7/tests/unit/cloudbender/test_providers_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cloudbender/test_regions_unit.py` & `proximl-0.5.7/tests/unit/cloudbender/test_regions_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/cloudbender/test_services_unit.py` & `proximl-0.5.7/tests/unit/cloudbender/test_services_unit.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 def service(mock_proximl):
     yield specimen.Service(
         mock_proximl,
         provider_uuid="1",
         region_uuid="a",
         service_id="x",
         name="On-Prem Service",
+        type="https",
         public=False,
         hostname="app1.proximl.cloud",
     )
 
 
 class RegionsTests:
     @mark.asyncio
@@ -75,25 +76,28 @@
 
     @mark.asyncio
     async def test_create_service(self, services, mock_proximl):
         requested_config = dict(
             provider_uuid="provider-id-1",
             region_uuid="region-id-1",
             name="On-Prem Service",
+            type="https",
             public=False,
         )
         expected_payload = dict(
             name="On-Prem Service",
+            type="https",
             public=False,
         )
         api_response = {
             "provider_uuid": "provider-id-1",
             "region_uuid": "region-id-1",
             "service_id": "service-id-1",
             "name": "On-Prem Service",
+            "type": "https",
             "public": False,
             "hostname": "app1.proximl.cloud",
             "createdAt": "2020-12-31T23:59:59.000Z",
         }
 
         mock_proximl._query = AsyncMock(return_value=api_response)
         response = await services.create(**requested_config)
@@ -110,14 +114,15 @@
     def test_service_properties(self, service):
         assert isinstance(service.id, str)
         assert isinstance(service.provider_uuid, str)
         assert isinstance(service.region_uuid, str)
         assert isinstance(service.public, bool)
         assert isinstance(service.name, str)
         assert isinstance(service.hostname, str)
+        assert isinstance(service.type, str)
 
     def test_service_str(self, service):
         string = str(service)
         regex = r"^{.*\"service_id\": \"" + service.id + r"\".*}$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
@@ -144,14 +149,15 @@
     @mark.asyncio
     async def test_service_refresh(self, service, mock_proximl):
         api_response = {
             "provider_uuid": "provider-id-1",
             "region_uuid": "region-id-1",
             "service_id": "service-id-1",
             "name": "On-Prem Service",
+            "type": "https",
             "public": False,
             "hostname": "app1.proximl.cloud",
             "createdAt": "2020-12-31T23:59:59.000Z",
         }
         mock_proximl._query = AsyncMock(return_value=api_response)
         response = await service.refresh()
         mock_proximl._query.assert_called_once_with(
```

### Comparing `proximl-0.5.6/tests/unit/conftest.py` & `proximl-0.5.7/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/test_auth.py` & `proximl-0.5.7/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/test_checkpoints_unit.py` & `proximl-0.5.7/tests/unit/test_checkpoints_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/test_connections_unit.py` & `proximl-0.5.7/tests/unit/test_connections_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/test_datasets_unit.py` & `proximl-0.5.7/tests/unit/test_datasets_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/test_environments_unit.py` & `proximl-0.5.7/tests/unit/test_environments_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/test_exceptions.py` & `proximl-0.5.7/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/test_gpu_types_unit.py` & `proximl-0.5.7/tests/unit/test_gpu_types_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/test_jobs_unit.py` & `proximl-0.5.7/tests/unit/test_jobs_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/test_models_unit.py` & `proximl-0.5.7/tests/unit/test_models_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/test_projects_unit.py` & `proximl-0.5.7/tests/unit/test_projects_unit.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,24 +45,35 @@
         project_uuid="proj-id-1",
         type="nfs",
         region_uuid="reg-id-1",
     )
 
 
 @fixture
+def project_data_connector(mock_proximl):
+    yield specimen.ProjectDataConnector(
+        mock_proximl,
+        id="ds-id-1",
+        name="connector 1",
+        project_uuid="proj-id-1",
+        type="custom",
+        region_uuid="reg-id-1",
+    )
+
+
+@fixture
 def project_service(mock_proximl):
     yield specimen.ProjectService(
         mock_proximl,
         id="res-id-1",
         name="service 1",
         project_uuid="proj-id-1",
         region_uuid="reg-id-1",
-        type="port",
-        resource="8001",
-        hostname="service.local",
+        public=False,
+        hostname="asdf.proximl.cloud",
     )
 
 
 class ProjectsTests:
     @mark.asyncio
     async def test_get_project(
         self,
@@ -148,22 +159,51 @@
 
     def test_project_datastore_bool(self, project_datastore, mock_proximl):
         empty_project_datastore = specimen.ProjectDatastore(mock_proximl)
         assert bool(project_datastore)
         assert not bool(empty_project_datastore)
 
 
+class ProjectDataConnectorTests:
+    def test_project_data_connector_properties(self, project_data_connector):
+        assert isinstance(project_data_connector.id, str)
+        assert isinstance(project_data_connector.name, str)
+        assert isinstance(project_data_connector.project_uuid, str)
+        assert isinstance(project_data_connector.type, str)
+        assert isinstance(project_data_connector.region_uuid, str)
+
+    def test_project_data_connector_str(self, project_data_connector):
+        string = str(project_data_connector)
+        regex = r"^{.*\"id\": \"" + project_data_connector.id + r"\".*}$"
+        assert isinstance(string, str)
+        assert re.match(regex, string)
+
+    def test_project_data_connector_repr(self, project_data_connector):
+        string = repr(project_data_connector)
+        regex = (
+            r"^ProjectDataConnector\( proximl , \*\*{.*'id': '"
+            + project_data_connector.id
+            + r"'.*}\)$"
+        )
+        assert isinstance(string, str)
+        assert re.match(regex, string)
+
+    def test_project_data_connector_bool(self, project_data_connector, mock_proximl):
+        empty_project_data_connector = specimen.ProjectDataConnector(mock_proximl)
+        assert bool(project_data_connector)
+        assert not bool(empty_project_data_connector)
+
+
 class ProjectServiceTests:
     def test_project_service_properties(self, project_service):
         assert isinstance(project_service.id, str)
         assert isinstance(project_service.name, str)
         assert isinstance(project_service.project_uuid, str)
-        assert isinstance(project_service.type, str)
         assert isinstance(project_service.hostname, str)
-        assert isinstance(project_service.resource, str)
+        assert isinstance(project_service.public, bool)
         assert isinstance(project_service.region_uuid, str)
 
     def test_project_service_str(self, project_service):
         string = str(project_service)
         regex = r"^{.*\"id\": \"" + project_service.id + r"\".*}$"
         assert isinstance(string, str)
         assert re.match(regex, string)
```

### Comparing `proximl-0.5.6/tests/unit/test_proximl.py` & `proximl-0.5.7/tests/unit/test_proximl.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.6/tests/unit/test_volumes_unit.py` & `proximl-0.5.7/tests/unit/test_volumes_unit.py`

 * *Files identical despite different names*

