# Comparing `tmp/seqerakit-0.4.6.tar.gz` & `tmp/seqerakit-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqerakit-0.4.6.tar", last modified: Mon Mar  4 06:52:06 2024, max compression
+gzip compressed data, was "seqerakit-0.4.7.tar", last modified: Fri Apr 26 01:30:57 2024, max compression
```

## Comparing `seqerakit-0.4.6.tar` & `seqerakit-0.4.7.tar`

### file list

```diff
@@ -1,94 +1,98 @@
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-03-04 06:52:06.814179 seqerakit-0.4.6/
--rw-r--r--   0 eshajoshi   (501) staff       (20)      239 2023-10-13 03:44:10.000000 seqerakit-0.4.6/.dockerignore
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-03-04 06:52:06.794950 seqerakit-0.4.6/.github/
--rw-r--r--   0 eshajoshi   (501) staff       (20)     5024 2023-10-13 03:44:10.000000 seqerakit-0.4.6/.github/CONTRIBUTING.md
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-03-04 06:52:06.795749 seqerakit-0.4.6/.github/workflows/
--rw-r--r--   0 eshajoshi   (501) staff       (20)     3042 2024-01-10 03:27:27.000000 seqerakit-0.4.6/.github/workflows/e2e-testing.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      724 2024-01-10 03:27:27.000000 seqerakit-0.4.6/.github/workflows/python-testing.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1804 2024-01-10 03:27:27.000000 seqerakit-0.4.6/.github/workflows/teardown.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      259 2024-03-04 06:40:27.000000 seqerakit-0.4.6/.gitignore
--rw-r--r--   0 eshajoshi   (501) staff       (20)      763 2023-11-10 19:39:47.000000 seqerakit-0.4.6/.pre-commit-config.yaml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      286 2023-11-25 22:33:31.000000 seqerakit-0.4.6/.prettierrc
--rw-r--r--   0 eshajoshi   (501) staff       (20)    11358 2023-11-15 02:34:37.000000 seqerakit-0.4.6/LICENSE.txt
--rw-r--r--   0 eshajoshi   (501) staff       (20)    16698 2024-03-04 06:52:06.813968 seqerakit-0.4.6/PKG-INFO
--rw-r--r--   0 eshajoshi   (501) staff       (20)    16218 2024-03-04 06:50:02.000000 seqerakit-0.4.6/README.md
--rw-r--r--   0 eshajoshi   (501) staff       (20)       25 2023-10-13 03:44:10.000000 seqerakit-0.4.6/__init__.py
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-03-04 06:52:06.796485 seqerakit-0.4.6/assets/
--rw-r--r--   0 eshajoshi   (501) staff       (20)    21635 2023-10-13 03:44:10.000000 seqerakit-0.4.6/assets/seqerakit.svg
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-03-04 06:52:06.792120 seqerakit-0.4.6/examples/
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-03-04 06:52:06.796742 seqerakit-0.4.6/examples/python/
--rwxr-xr-x   0 eshajoshi   (501) staff       (20)      783 2023-10-13 03:44:10.000000 seqerakit-0.4.6/examples/python/launch_hello_world.py
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-03-04 06:52:06.796952 seqerakit-0.4.6/examples/yaml/
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-03-04 06:52:06.797939 seqerakit-0.4.6/examples/yaml/compute-envs/
--rw-r--r--   0 eshajoshi   (501) staff       (20)      627 2023-10-13 03:44:10.000000 seqerakit-0.4.6/examples/yaml/compute-envs/seqera_aws_ireland_fusionv2_nvme.json
--rw-r--r--   0 eshajoshi   (501) staff       (20)      622 2023-10-13 03:44:10.000000 seqerakit-0.4.6/examples/yaml/compute-envs/seqera_aws_virginia_fusionv2_nvme.json
--rw-r--r--   0 eshajoshi   (501) staff       (20)      335 2023-10-13 03:44:10.000000 seqerakit-0.4.6/examples/yaml/compute-envs/seqera_azure_virginia.json
--rw-r--r--   0 eshajoshi   (501) staff       (20)      257 2023-10-13 03:44:10.000000 seqerakit-0.4.6/examples/yaml/compute-envs/seqera_gcp_finland.json
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-03-04 06:52:06.798866 seqerakit-0.4.6/examples/yaml/datasets/
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1012 2023-10-13 03:44:10.000000 seqerakit-0.4.6/examples/yaml/datasets/rnaseq_samples.csv
--rw-r--r--   0 eshajoshi   (501) staff       (20)      314 2023-10-13 03:44:10.000000 seqerakit-0.4.6/examples/yaml/datasets/sarek_samples.csv
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1181 2023-10-13 03:44:10.000000 seqerakit-0.4.6/examples/yaml/datasets/sentieon_samples.csv
--rw-r--r--   0 eshajoshi   (501) staff       (20)      699 2023-10-13 03:44:10.000000 seqerakit-0.4.6/examples/yaml/datasets/viralrecon_illumina_samples.csv
--rw-r--r--   0 eshajoshi   (501) staff       (20)      149 2023-10-13 03:44:10.000000 seqerakit-0.4.6/examples/yaml/datasets/viralrecon_nanopore_samples.csv
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-03-04 06:52:06.800711 seqerakit-0.4.6/examples/yaml/e2e/
--rw-r--r--   0 eshajoshi   (501) staff       (20)      376 2024-01-10 03:27:27.000000 seqerakit-0.4.6/examples/yaml/e2e/actions.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      709 2024-01-10 03:27:27.000000 seqerakit-0.4.6/examples/yaml/e2e/compute-envs.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      994 2024-01-10 03:27:27.000000 seqerakit-0.4.6/examples/yaml/e2e/credentials.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1352 2024-01-10 03:27:27.000000 seqerakit-0.4.6/examples/yaml/e2e/datasets.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      222 2024-01-10 03:27:27.000000 seqerakit-0.4.6/examples/yaml/e2e/organizations.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      265 2024-01-10 03:27:27.000000 seqerakit-0.4.6/examples/yaml/e2e/participants.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1590 2024-01-10 03:27:27.000000 seqerakit-0.4.6/examples/yaml/e2e/pipelines.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      143 2024-01-10 03:27:27.000000 seqerakit-0.4.6/examples/yaml/e2e/secrets.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      252 2024-01-10 03:27:27.000000 seqerakit-0.4.6/examples/yaml/e2e/teams.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      209 2024-01-10 03:27:27.000000 seqerakit-0.4.6/examples/yaml/e2e/workspaces.yml
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-03-04 06:52:06.802548 seqerakit-0.4.6/examples/yaml/pipelines/
--rw-r--r--   0 eshajoshi   (501) staff       (20)       22 2023-10-13 03:44:10.000000 seqerakit-0.4.6/examples/yaml/pipelines/nextflow.config
--rw-r--r--   0 eshajoshi   (501) staff       (20)      537 2023-10-13 03:44:10.000000 seqerakit-0.4.6/examples/yaml/pipelines/nf-core-sarek_pipeline.json
--rw-r--r--   0 eshajoshi   (501) staff       (20)       57 2023-10-13 03:44:10.000000 seqerakit-0.4.6/examples/yaml/pipelines/nf_core_rnaseq_params.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      581 2023-10-13 03:44:10.000000 seqerakit-0.4.6/examples/yaml/pipelines/nf_core_rnaseq_pipeline.json
--rw-r--r--   0 eshajoshi   (501) staff       (20)       81 2023-10-13 03:44:10.000000 seqerakit-0.4.6/examples/yaml/pipelines/nf_core_viralrecon_illumina_params.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      503 2023-10-13 03:44:10.000000 seqerakit-0.4.6/examples/yaml/pipelines/nf_core_viralrecon_illumina_pipeline.json
--rw-r--r--   0 eshajoshi   (501) staff       (20)      512 2023-10-13 03:44:10.000000 seqerakit-0.4.6/examples/yaml/pipelines/nf_core_viralrecon_nanopore_pipeline.json
--rw-r--r--   0 eshajoshi   (501) staff       (20)      576 2023-10-13 03:44:10.000000 seqerakit-0.4.6/examples/yaml/pipelines/nf_sentieon_pipeline.json
--rw-r--r--   0 eshajoshi   (501) staff       (20)       23 2024-01-10 03:27:27.000000 seqerakit-0.4.6/examples/yaml/pipelines/pre_run.txt
--rw-r--r--   0 eshajoshi   (501) staff       (20)     6702 2023-12-05 22:59:42.000000 seqerakit-0.4.6/examples/yaml/seqerakit-e2e.yml
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-03-04 06:52:06.805219 seqerakit-0.4.6/seqerakit/
--rw-r--r--   0 eshajoshi   (501) staff       (20)      100 2024-03-04 04:14:34.000000 seqerakit-0.4.6/seqerakit/__init__.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)     6615 2024-03-04 06:40:31.000000 seqerakit-0.4.6/seqerakit/cli.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1641 2023-11-15 02:34:37.000000 seqerakit-0.4.6/seqerakit/computeenvs.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)    12550 2024-01-10 03:09:05.000000 seqerakit-0.4.6/seqerakit/dump_yaml.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)    10779 2024-03-04 06:40:31.000000 seqerakit-0.4.6/seqerakit/helper.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)    10461 2024-03-04 03:19:03.000000 seqerakit-0.4.6/seqerakit/overwrite.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1619 2023-11-15 02:34:37.000000 seqerakit-0.4.6/seqerakit/pipelines.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)     5039 2024-01-10 03:27:27.000000 seqerakit-0.4.6/seqerakit/seqeraplatform.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)     5111 2024-01-10 03:27:27.000000 seqerakit-0.4.6/seqerakit/utils.py
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-03-04 06:52:06.808555 seqerakit-0.4.6/seqerakit.egg-info/
--rw-r--r--   0 eshajoshi   (501) staff       (20)    16698 2024-03-04 06:52:06.000000 seqerakit-0.4.6/seqerakit.egg-info/PKG-INFO
--rw-r--r--   0 eshajoshi   (501) staff       (20)     2426 2024-03-04 06:52:06.000000 seqerakit-0.4.6/seqerakit.egg-info/SOURCES.txt
--rw-r--r--   0 eshajoshi   (501) staff       (20)        1 2024-03-04 06:52:06.000000 seqerakit-0.4.6/seqerakit.egg-info/dependency_links.txt
--rw-r--r--   0 eshajoshi   (501) staff       (20)       49 2024-03-04 06:52:06.000000 seqerakit-0.4.6/seqerakit.egg-info/entry_points.txt
--rw-r--r--   0 eshajoshi   (501) staff       (20)        1 2023-11-29 04:33:12.000000 seqerakit-0.4.6/seqerakit.egg-info/not-zip-safe
--rw-r--r--   0 eshajoshi   (501) staff       (20)       14 2024-03-04 06:52:06.000000 seqerakit-0.4.6/seqerakit.egg-info/requires.txt
--rw-r--r--   0 eshajoshi   (501) staff       (20)       10 2024-03-04 06:52:06.000000 seqerakit-0.4.6/seqerakit.egg-info/top_level.txt
--rw-r--r--   0 eshajoshi   (501) staff       (20)       38 2024-03-04 06:52:06.814232 seqerakit-0.4.6/setup.cfg
--rw-r--r--   0 eshajoshi   (501) staff       (20)      964 2024-03-04 06:50:23.000000 seqerakit-0.4.6/setup.py
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-03-04 06:52:06.811133 seqerakit-0.4.6/templates/
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1540 2024-01-10 03:27:27.000000 seqerakit-0.4.6/templates/actions.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)     2847 2024-01-10 03:27:27.000000 seqerakit-0.4.6/templates/compute-envs.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)     2163 2024-01-10 03:27:27.000000 seqerakit-0.4.6/templates/credentials.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      419 2023-10-13 03:44:10.000000 seqerakit-0.4.6/templates/datasets.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1394 2024-01-10 03:27:27.000000 seqerakit-0.4.6/templates/launch.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      405 2023-10-13 03:44:10.000000 seqerakit-0.4.6/templates/organizations.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      541 2023-10-13 03:44:10.000000 seqerakit-0.4.6/templates/participants.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1478 2024-01-10 03:27:27.000000 seqerakit-0.4.6/templates/pipelines.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      303 2023-10-13 03:44:10.000000 seqerakit-0.4.6/templates/secrets.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      341 2023-10-13 03:44:10.000000 seqerakit-0.4.6/templates/teams.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      375 2023-10-13 03:44:10.000000 seqerakit-0.4.6/templates/workspaces.yml
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-03-04 06:52:06.792969 seqerakit-0.4.6/tests/
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-03-04 06:52:06.811320 seqerakit-0.4.6/tests/e2e/
--rw-r--r--   0 eshajoshi   (501) staff       (20)     2735 2024-01-10 03:27:27.000000 seqerakit-0.4.6/tests/e2e/aws-e2e.yml
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-03-04 06:52:06.813687 seqerakit-0.4.6/tests/unit/
--rw-r--r--   0 eshajoshi   (501) staff       (20)       25 2024-02-28 20:36:16.000000 seqerakit-0.4.6/tests/unit/__init__.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)     8788 2024-03-04 06:40:27.000000 seqerakit-0.4.6/tests/unit/test_helper.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)     8092 2023-11-15 02:34:37.000000 seqerakit-0.4.6/tests/unit/test_seqeraplatform.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)     5835 2023-10-13 03:44:10.000000 seqerakit-0.4.6/tests/unit/test_subcommands.py
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.718180 seqerakit-0.4.7/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      239 2023-10-13 03:44:10.000000 seqerakit-0.4.7/.dockerignore
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.695945 seqerakit-0.4.7/.github/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     5024 2023-10-13 03:44:10.000000 seqerakit-0.4.7/.github/CONTRIBUTING.md
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.696832 seqerakit-0.4.7/.github/workflows/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     3042 2024-01-10 03:27:27.000000 seqerakit-0.4.7/.github/workflows/e2e-testing.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      724 2024-01-10 03:27:27.000000 seqerakit-0.4.7/.github/workflows/python-testing.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1804 2024-01-10 03:27:27.000000 seqerakit-0.4.7/.github/workflows/teardown.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      278 2024-04-26 01:13:08.000000 seqerakit-0.4.7/.gitignore
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      763 2023-11-10 19:39:47.000000 seqerakit-0.4.7/.pre-commit-config.yaml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      286 2023-11-25 22:33:31.000000 seqerakit-0.4.7/.prettierrc
+-rw-r--r--   0 eshajoshi   (501) staff       (20)    11358 2023-11-15 02:34:37.000000 seqerakit-0.4.7/LICENSE.txt
+-rw-r--r--   0 eshajoshi   (501) staff       (20)    16525 2024-04-26 01:30:57.717707 seqerakit-0.4.7/PKG-INFO
+-rw-r--r--   0 eshajoshi   (501) staff       (20)    16016 2024-04-26 01:30:01.000000 seqerakit-0.4.7/README.md
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       25 2023-10-13 03:44:10.000000 seqerakit-0.4.7/__init__.py
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.697478 seqerakit-0.4.7/assets/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)    15390 2024-04-26 01:13:08.000000 seqerakit-0.4.7/assets/seqerakit.svg
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.692713 seqerakit-0.4.7/examples/
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.697657 seqerakit-0.4.7/examples/python/
+-rwxr-xr-x   0 eshajoshi   (501) staff       (20)      783 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/python/launch_hello_world.py
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.697915 seqerakit-0.4.7/examples/yaml/
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.699468 seqerakit-0.4.7/examples/yaml/compute-envs/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      627 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/compute-envs/seqera_aws_ireland_fusionv2_nvme.json
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      622 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/compute-envs/seqera_aws_virginia_fusionv2_nvme.json
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      335 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/compute-envs/seqera_azure_virginia.json
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      257 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/compute-envs/seqera_gcp_finland.json
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.700441 seqerakit-0.4.7/examples/yaml/datasets/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1012 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/datasets/rnaseq_samples.csv
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      314 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/datasets/sarek_samples.csv
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1181 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/datasets/sentieon_samples.csv
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      699 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/datasets/viralrecon_illumina_samples.csv
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      149 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/datasets/viralrecon_nanopore_samples.csv
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.705041 seqerakit-0.4.7/examples/yaml/e2e/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      376 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/actions.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      709 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/compute-envs.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      994 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/credentials.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1352 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/datasets.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      108 2024-04-26 01:06:21.000000 seqerakit-0.4.7/examples/yaml/e2e/labels.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      111 2024-04-26 01:06:21.000000 seqerakit-0.4.7/examples/yaml/e2e/members.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      222 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/organizations.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      265 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/participants.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1590 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/pipelines.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      143 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/secrets.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      252 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/teams.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      209 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/workspaces.yml
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.707036 seqerakit-0.4.7/examples/yaml/pipelines/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       22 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/pipelines/nextflow.config
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      537 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/pipelines/nf-core-sarek_pipeline.json
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       57 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/pipelines/nf_core_rnaseq_params.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      581 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/pipelines/nf_core_rnaseq_pipeline.json
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       81 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/pipelines/nf_core_viralrecon_illumina_params.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      503 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/pipelines/nf_core_viralrecon_illumina_pipeline.json
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      512 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/pipelines/nf_core_viralrecon_nanopore_pipeline.json
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      576 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/pipelines/nf_sentieon_pipeline.json
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       23 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/pipelines/pre_run.txt
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     6702 2024-04-26 00:48:24.000000 seqerakit-0.4.7/examples/yaml/seqerakit-e2e.yml
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.710502 seqerakit-0.4.7/seqerakit/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      100 2024-03-18 04:58:40.000000 seqerakit-0.4.7/seqerakit/__init__.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     6904 2024-04-25 23:44:28.000000 seqerakit-0.4.7/seqerakit/cli.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1641 2023-11-15 02:34:37.000000 seqerakit-0.4.7/seqerakit/computeenvs.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)    12973 2024-04-25 23:34:42.000000 seqerakit-0.4.7/seqerakit/dump_yaml.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)    12576 2024-04-25 23:48:34.000000 seqerakit-0.4.7/seqerakit/helper.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)    12623 2024-04-26 00:46:21.000000 seqerakit-0.4.7/seqerakit/overwrite.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1619 2023-11-15 02:34:37.000000 seqerakit-0.4.7/seqerakit/pipelines.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     5069 2024-04-25 23:44:28.000000 seqerakit-0.4.7/seqerakit/seqeraplatform.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     5112 2024-04-26 00:46:21.000000 seqerakit-0.4.7/seqerakit/utils.py
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.711731 seqerakit-0.4.7/seqerakit.egg-info/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)    16525 2024-04-26 01:30:57.000000 seqerakit-0.4.7/seqerakit.egg-info/PKG-INFO
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     2528 2024-04-26 01:30:57.000000 seqerakit-0.4.7/seqerakit.egg-info/SOURCES.txt
+-rw-r--r--   0 eshajoshi   (501) staff       (20)        1 2024-04-26 01:30:57.000000 seqerakit-0.4.7/seqerakit.egg-info/dependency_links.txt
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       49 2024-04-26 01:30:57.000000 seqerakit-0.4.7/seqerakit.egg-info/entry_points.txt
+-rw-r--r--   0 eshajoshi   (501) staff       (20)        1 2023-11-29 04:33:12.000000 seqerakit-0.4.7/seqerakit.egg-info/not-zip-safe
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       14 2024-04-26 01:30:57.000000 seqerakit-0.4.7/seqerakit.egg-info/requires.txt
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       10 2024-04-26 01:30:57.000000 seqerakit-0.4.7/seqerakit.egg-info/top_level.txt
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       38 2024-04-26 01:30:57.718229 seqerakit-0.4.7/setup.cfg
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      964 2024-04-26 01:17:35.000000 seqerakit-0.4.7/setup.py
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.715416 seqerakit-0.4.7/templates/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1540 2024-01-10 03:27:27.000000 seqerakit-0.4.7/templates/actions.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     2847 2024-01-10 03:27:27.000000 seqerakit-0.4.7/templates/compute-envs.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     2163 2024-01-10 03:27:27.000000 seqerakit-0.4.7/templates/credentials.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      419 2023-10-13 03:44:10.000000 seqerakit-0.4.7/templates/datasets.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      310 2024-04-05 23:44:56.000000 seqerakit-0.4.7/templates/labels.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1394 2024-01-10 03:27:27.000000 seqerakit-0.4.7/templates/launch.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      266 2024-04-05 23:44:56.000000 seqerakit-0.4.7/templates/members.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      405 2023-10-13 03:44:10.000000 seqerakit-0.4.7/templates/organizations.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      541 2024-03-20 19:32:10.000000 seqerakit-0.4.7/templates/participants.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1478 2024-01-10 03:27:27.000000 seqerakit-0.4.7/templates/pipelines.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      303 2023-10-13 03:44:10.000000 seqerakit-0.4.7/templates/secrets.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      341 2023-10-13 03:44:10.000000 seqerakit-0.4.7/templates/teams.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      375 2023-10-13 03:44:10.000000 seqerakit-0.4.7/templates/workspaces.yml
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.693463 seqerakit-0.4.7/tests/
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.715595 seqerakit-0.4.7/tests/e2e/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     2735 2024-01-10 03:27:27.000000 seqerakit-0.4.7/tests/e2e/aws-e2e.yml
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.716897 seqerakit-0.4.7/tests/unit/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       25 2024-02-28 20:36:16.000000 seqerakit-0.4.7/tests/unit/__init__.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)    13003 2024-04-25 23:44:28.000000 seqerakit-0.4.7/tests/unit/test_helper.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     8359 2024-04-25 23:44:28.000000 seqerakit-0.4.7/tests/unit/test_seqeraplatform.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     5835 2023-10-13 03:44:10.000000 seqerakit-0.4.7/tests/unit/test_subcommands.py
```

### Comparing `seqerakit-0.4.6/.github/CONTRIBUTING.md` & `seqerakit-0.4.7/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/.github/workflows/e2e-testing.yml` & `seqerakit-0.4.7/.github/workflows/e2e-testing.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/.github/workflows/python-testing.yml` & `seqerakit-0.4.7/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/.github/workflows/teardown.yml` & `seqerakit-0.4.7/.github/workflows/teardown.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/.pre-commit-config.yaml` & `seqerakit-0.4.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/LICENSE.txt` & `seqerakit-0.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/PKG-INFO` & `seqerakit-0.4.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: seqerakit
-Version: 0.4.6
+Version: 0.4.7
 Summary: Automate creation of Seqera Platform resources
 Home-page: https://github.com/seqeralabs/seqera-kit
 Author: Esha Joshi, Adam Talbot, Harshil Patel
 Author-email: esha.joshi@seqera.io, adam.talbot@seqera.io, harshil.patel@seqera.io
 License: Apache 2.0
 Keywords: nextflow,bioinformatics,workflow,pipeline,seqera-platform,seqera
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: pyyaml>=6.0.0
 
 # <img src="https://raw.githubusercontent.com/seqeralabs/seqera-kit/main/assets/seqerakit.svg" width=50 alt="seqerakit logo"> seqerakit
 
+
 `seqerakit` is a Python wrapper for the [Seqera Platform CLI](https://github.com/seqeralabs/tower-cli). It can be leveraged to automate the creation of all of the entities in Seqera Platform via a simple configuration file in YAML format.
 
 The key features are:
 
 - **Simple configuration**: All of the command-line options available when using the Seqera Platform CLI can be defined in simple YAML format.
 - **Infrastructure as Code**: Enable users to manage and provision their infrastructure specifications.
 - **Automation**: End-to-end creation of entities within Seqera Platform, all the way from adding an Organization to launching pipeline(s) within that Organization.
 
 ## Prerequisites
 
-You will need to have an account on Seqera Platform (see [Plans and pricing](https://cloud.tower.nf/pricing/)).
+You will need to have an account on Seqera Platform (see [Plans and pricing](https://seqera.io/pricing/)).
 
 ## Installation
 
 `seqerakit` requires the following dependencies:
 
 1. [Seqera Platform CLI (`>=0.9.2`)](https://github.com/seqeralabs/tower-cli#1-installation)
 
@@ -86,27 +88,27 @@
 You can verify your installation with:
 ```bash
 pip show seqerakit
 ```
 
 ## Configuration
 
-Create a Seqera Platform access token using the [Seqera Platform](https://tower.nf/) web interface via the **Your Tokens** page in your profile.
+Create a Seqera Platform access token using the [Seqera Platform](https://seqera.io/) web interface via the **Your Tokens** page in your profile.
 
 `seqerakit` reads this token from the environment variable `TOWER_ACCESS_TOKEN`. Please export it into your terminal as shown below:
 
 ```bash
 export TOWER_ACCESS_TOKEN=<Your access token>
 ```
 
 For Enterprise installations of Seqera Platform, you will also need to configure the API endpoint that will be used to connect to the Platform. You can do so by exporting the following environment variable:
 ```bash
 export TOWER_API_ENDPOINT=<Tower API URL>
 ```
-By default, this is set to `https://api.tower.nf` to connect to Seqera Platform Cloud.
+By default, this is set to `https://api.cloud.seqera.io` to connect to Seqera Platform Cloud.
 
 
 ## Usage
 
 To confirm the installation of `seqerakit`, configuration of the Seqera Platform CLI and connection to the Platform is working as expected. This will run the `tw info` command under the hood:
 
 ```bash
@@ -118,14 +120,26 @@
 seqerakit --help
 ```
 
 Use `--version` or `-v` to retrieve the current version of your seqerakit installation:
 ```bash
 seqerakit --version
 ```
+### Input
+`seqerakit` supports input through either file paths to YAMLs or directly from standard input (stdin).
+
+#### Using File Path
+```bash
+seqerakit /path/to/file.yaml
+```
+#### Using stdin
+```console
+$ cat file.yaml | seqerakit -
+```
+See the [Defining your YAML file using CLI options](#defining-your-yaml-file-using-cli-options) section for guidance on formatting your input YAML file(s).
 
 ### Dryrun
 
 To print the commands that would executed with `tw` when using a YAML file, you can run `seqerakit` with the `--dryrun` flag:
 
 ```bash
 seqerakit file.yaml --dryrun
@@ -217,15 +231,15 @@
 
 DEBUG:root: Running command: tw organizations delete --name $SEQERA_ORGANIZATION_NAME
 DEBUG:root: Running command: tw organizations add --name $SEQERA_ORGANIZATION_NAME --full-name $SEQERA_ORGANIZATION_NAME --description 'Example of an organization'
 ```
 ### 3. Specifying JSON configuration files with `file-path`
 The Seqera Platform CLI allows export and import of entities through JSON configuration files for pipelines and compute environments. To use these files to add a pipeline or compute environment to a workspace, use the `file-path` key to specify a path to a JSON configuration file.
 
-An example of the `file-path` option is provided in the [compute-envs.yml](templates/compute-envs.yml) template:
+An example of the `file-path` option is provided in the [compute-envs.yml](./templates/compute-envs.yml) template:
 
 ```yaml
 compute-envs:
   - name: 'my_aws_compute_environment'                              # required
     workspace: 'my_organization/my_workspace'                       # required
     credentials: 'my_aws_credentials'                               # required
     wait: 'AVAILABLE'                                               # optional
@@ -234,15 +248,15 @@
 ```
 
 
 ## Quick start
 
 You must provide a YAML file that defines the options for each of the entities you would like to create in Seqera Platform.
 
-You will need to have an account on Seqera Platform (see [Plans and pricing](https://cloud.tower.nf/pricing/)). You will also need access to a Workspace and a pre-defined Compute Environment where you can launch a pipeline.
+You will need to have an account on Seqera Platform (see [Plans and pricing](https://seqera.io/pricing/)). You will also need access to a Workspace and a pre-defined Compute Environment where you can launch a pipeline.
 
 ### Launch via YAML
 
 1. Create a YAML file called `hello-world-config.yml` with the contents below, and customise the `<YOUR_WORKSPACE>` and `<YOUR_COMPUTE_ENVIRONMENT>` entries as required:
 
    ```yaml # noqa
    launch:
@@ -261,15 +275,15 @@
 
 3. Login to your Seqera Platform instance and check the Runs page in the appropriate Workspace for the pipeline you just launched!
 
 ### Launch via a Python script
 
 You can also launch the same pipeline via a Python script. This will essentially allow you to extend the functionality on offer within the Seqera Platform CLI by leveraging the flexibility and customisation options available in Python.
 
-1. Download the [`launch_hello_world.py`](https://github.com/seqeralabs/seqera-kit/blob/main/examples/python/launch_hello_world.py) Python script and customise the `<YOUR_WORKSPACE>` and `<YOUR_COMPUTE_ENVIRONMENT>` entries as required.
+1. Download the [`launch_hello_world.py`](./examples/python/launch_hello_world.py) Python script and customise the `<YOUR_WORKSPACE>` and `<YOUR_COMPUTE_ENVIRONMENT>` entries as required.
 
 2. Launch the pipeline with `seqerakit`:
 
 ```bash
    python launch_hello_world.py
 ```
 
@@ -328,32 +342,33 @@
 - `name`, `url`, `workspace`, etc., are the keys derived from the CLI options.
 - The corresponding values are user-defined
 
 ### Best Practices:
 - Ensure that the indentation and structure of the YAML file are correct - YAML is sensitive to formatting.
 - Use quotes around strings that contain special characters or spaces.
 - When listing multiple values (`labels`, `instance-types`, `allow-buckets`, etc), separate them with commas as shown above.
-- For complex configurations, refer to the [Templates](/templates/) provided in this repository.
+- For complex configurations, refer to the [Templates](./templates/) provided in this repository.
 
 
 ## Templates
 
 We have provided template YAML files for each of the entities that can be created on Seqera Platform. These can be found in the [`templates/`](https://github.com/seqeralabs/blob/main/seqera-kit/templates) directory and should form a good starting point for you to add your own customization:
 
-- [organizations.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/organizations.yml)
-- [teams.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/teams.yml)
-- [workspaces.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/workspaces.yml)
-- [participants.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/participants.yml)
-- [credentials.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/credentials.yml)
-- [secrets.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/secrets.yml)
-- [compute-envs.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/compute-envs.yml)
-- [actions.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/actions.yml)
-- [datasets.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/datasets.yml)
-- [pipelines.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/pipelines.yml)
-- [launch.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/launch.yml)
+- [organizations.yml](./templates/organizations.yml)
+- [teams.yml](./templates/teams.yml)
+- [workspaces.yml](./templates/workspaces.yml)
+- [participants.yml](./templates/participants.yml)
+- [credentials.yml](./templates/credentials.yml)
+- [secrets.yml](./templates/secrets.yml)
+- [compute-envs.yml](./templates/compute-envs.yml)
+- [actions.yml](./templates/actions.yml)
+- [datasets.yml](./templates/datasets.yml)
+- [labels.yml](./templates/labels.yml)
+- [pipelines.yml](./templates/pipelines.yml)
+- [launch.yml](./templates/launch.yml)
 
 ## Real world example
 
 Please see [`seqerakit-e2e.yml`](./examples/yaml/seqerakit-e2e.yml) for an end-to-end example that highlights how you can use `seqerakit` to create everything sequentially in Seqera Platform all the way from creating a new Organization to launching a pipeline.
 
 You can modify this YAML to similarly create Seqera Platform resources end-to-end for your setup. This YAML encodes environment variables to protect sensitive keys, usernames, and passwords that are required to create or add certain resources (i.e. credentials, compute environments). Prior to running it with `seqerakit examples/yaml/seqerakit-e2e.yml`, you will have to set the following environment variables:
 
@@ -367,14 +382,14 @@
 $AZURE_STORAGE_KEY
 $GOOGLE_KEY
 $SENTIEON_LICENSE_BASE64
 ```
 
 ## Contributions and Support
 
-If you would like to contribute to `seqerakit`, please see the [contributing guidelines](https://github.com/seqeralabs/seqera-kit/blob/main/.github/CONTRIBUTING.md).
+If you would like to contribute to `seqerakit`, please see the [contributing guidelines](./.github/CONTRIBUTING.md).
 
 For further information or help, please don't hesitate to create an [issue](https://github.com/seqeralabs/seqera-kit/issues) in this repository.
 
 ## Credits
 
 `seqerakit` was written by [Esha Joshi](https://github.com/ejseqera), [Adam Talbot](https://github.com/adamrtalbot) and [Harshil Patel](https://github.com/drpatelh) from the Scientific Development Team at [Seqera Labs](https://seqera.io/).
```

### Comparing `seqerakit-0.4.6/README.md` & `seqerakit-0.4.7/seqerakit.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,35 @@
+Metadata-Version: 2.1
+Name: seqerakit
+Version: 0.4.7
+Summary: Automate creation of Seqera Platform resources
+Home-page: https://github.com/seqeralabs/seqera-kit
+Author: Esha Joshi, Adam Talbot, Harshil Patel
+Author-email: esha.joshi@seqera.io, adam.talbot@seqera.io, harshil.patel@seqera.io
+License: Apache 2.0
+Keywords: nextflow,bioinformatics,workflow,pipeline,seqera-platform,seqera
+Requires-Python: >=3.8, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: pyyaml>=6.0.0
+
 # <img src="https://raw.githubusercontent.com/seqeralabs/seqera-kit/main/assets/seqerakit.svg" width=50 alt="seqerakit logo"> seqerakit
 
+
 `seqerakit` is a Python wrapper for the [Seqera Platform CLI](https://github.com/seqeralabs/tower-cli). It can be leveraged to automate the creation of all of the entities in Seqera Platform via a simple configuration file in YAML format.
 
 The key features are:
 
 - **Simple configuration**: All of the command-line options available when using the Seqera Platform CLI can be defined in simple YAML format.
 - **Infrastructure as Code**: Enable users to manage and provision their infrastructure specifications.
 - **Automation**: End-to-end creation of entities within Seqera Platform, all the way from adding an Organization to launching pipeline(s) within that Organization.
 
 ## Prerequisites
 
-You will need to have an account on Seqera Platform (see [Plans and pricing](https://cloud.tower.nf/pricing/)).
+You will need to have an account on Seqera Platform (see [Plans and pricing](https://seqera.io/pricing/)).
 
 ## Installation
 
 `seqerakit` requires the following dependencies:
 
 1. [Seqera Platform CLI (`>=0.9.2`)](https://github.com/seqeralabs/tower-cli#1-installation)
 
@@ -73,27 +88,27 @@
 You can verify your installation with:
 ```bash
 pip show seqerakit
 ```
 
 ## Configuration
 
-Create a Seqera Platform access token using the [Seqera Platform](https://tower.nf/) web interface via the **Your Tokens** page in your profile.
+Create a Seqera Platform access token using the [Seqera Platform](https://seqera.io/) web interface via the **Your Tokens** page in your profile.
 
 `seqerakit` reads this token from the environment variable `TOWER_ACCESS_TOKEN`. Please export it into your terminal as shown below:
 
 ```bash
 export TOWER_ACCESS_TOKEN=<Your access token>
 ```
 
 For Enterprise installations of Seqera Platform, you will also need to configure the API endpoint that will be used to connect to the Platform. You can do so by exporting the following environment variable:
 ```bash
 export TOWER_API_ENDPOINT=<Tower API URL>
 ```
-By default, this is set to `https://api.tower.nf` to connect to Seqera Platform Cloud.
+By default, this is set to `https://api.cloud.seqera.io` to connect to Seqera Platform Cloud.
 
 
 ## Usage
 
 To confirm the installation of `seqerakit`, configuration of the Seqera Platform CLI and connection to the Platform is working as expected. This will run the `tw info` command under the hood:
 
 ```bash
@@ -105,14 +120,26 @@
 seqerakit --help
 ```
 
 Use `--version` or `-v` to retrieve the current version of your seqerakit installation:
 ```bash
 seqerakit --version
 ```
+### Input
+`seqerakit` supports input through either file paths to YAMLs or directly from standard input (stdin).
+
+#### Using File Path
+```bash
+seqerakit /path/to/file.yaml
+```
+#### Using stdin
+```console
+$ cat file.yaml | seqerakit -
+```
+See the [Defining your YAML file using CLI options](#defining-your-yaml-file-using-cli-options) section for guidance on formatting your input YAML file(s).
 
 ### Dryrun
 
 To print the commands that would executed with `tw` when using a YAML file, you can run `seqerakit` with the `--dryrun` flag:
 
 ```bash
 seqerakit file.yaml --dryrun
@@ -204,15 +231,15 @@
 
 DEBUG:root: Running command: tw organizations delete --name $SEQERA_ORGANIZATION_NAME
 DEBUG:root: Running command: tw organizations add --name $SEQERA_ORGANIZATION_NAME --full-name $SEQERA_ORGANIZATION_NAME --description 'Example of an organization'
 ```
 ### 3. Specifying JSON configuration files with `file-path`
 The Seqera Platform CLI allows export and import of entities through JSON configuration files for pipelines and compute environments. To use these files to add a pipeline or compute environment to a workspace, use the `file-path` key to specify a path to a JSON configuration file.
 
-An example of the `file-path` option is provided in the [compute-envs.yml](templates/compute-envs.yml) template:
+An example of the `file-path` option is provided in the [compute-envs.yml](./templates/compute-envs.yml) template:
 
 ```yaml
 compute-envs:
   - name: 'my_aws_compute_environment'                              # required
     workspace: 'my_organization/my_workspace'                       # required
     credentials: 'my_aws_credentials'                               # required
     wait: 'AVAILABLE'                                               # optional
@@ -221,15 +248,15 @@
 ```
 
 
 ## Quick start
 
 You must provide a YAML file that defines the options for each of the entities you would like to create in Seqera Platform.
 
-You will need to have an account on Seqera Platform (see [Plans and pricing](https://cloud.tower.nf/pricing/)). You will also need access to a Workspace and a pre-defined Compute Environment where you can launch a pipeline.
+You will need to have an account on Seqera Platform (see [Plans and pricing](https://seqera.io/pricing/)). You will also need access to a Workspace and a pre-defined Compute Environment where you can launch a pipeline.
 
 ### Launch via YAML
 
 1. Create a YAML file called `hello-world-config.yml` with the contents below, and customise the `<YOUR_WORKSPACE>` and `<YOUR_COMPUTE_ENVIRONMENT>` entries as required:
 
    ```yaml # noqa
    launch:
@@ -248,15 +275,15 @@
 
 3. Login to your Seqera Platform instance and check the Runs page in the appropriate Workspace for the pipeline you just launched!
 
 ### Launch via a Python script
 
 You can also launch the same pipeline via a Python script. This will essentially allow you to extend the functionality on offer within the Seqera Platform CLI by leveraging the flexibility and customisation options available in Python.
 
-1. Download the [`launch_hello_world.py`](https://github.com/seqeralabs/seqera-kit/blob/main/examples/python/launch_hello_world.py) Python script and customise the `<YOUR_WORKSPACE>` and `<YOUR_COMPUTE_ENVIRONMENT>` entries as required.
+1. Download the [`launch_hello_world.py`](./examples/python/launch_hello_world.py) Python script and customise the `<YOUR_WORKSPACE>` and `<YOUR_COMPUTE_ENVIRONMENT>` entries as required.
 
 2. Launch the pipeline with `seqerakit`:
 
 ```bash
    python launch_hello_world.py
 ```
 
@@ -315,32 +342,33 @@
 - `name`, `url`, `workspace`, etc., are the keys derived from the CLI options.
 - The corresponding values are user-defined
 
 ### Best Practices:
 - Ensure that the indentation and structure of the YAML file are correct - YAML is sensitive to formatting.
 - Use quotes around strings that contain special characters or spaces.
 - When listing multiple values (`labels`, `instance-types`, `allow-buckets`, etc), separate them with commas as shown above.
-- For complex configurations, refer to the [Templates](/templates/) provided in this repository.
+- For complex configurations, refer to the [Templates](./templates/) provided in this repository.
 
 
 ## Templates
 
 We have provided template YAML files for each of the entities that can be created on Seqera Platform. These can be found in the [`templates/`](https://github.com/seqeralabs/blob/main/seqera-kit/templates) directory and should form a good starting point for you to add your own customization:
 
-- [organizations.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/organizations.yml)
-- [teams.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/teams.yml)
-- [workspaces.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/workspaces.yml)
-- [participants.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/participants.yml)
-- [credentials.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/credentials.yml)
-- [secrets.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/secrets.yml)
-- [compute-envs.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/compute-envs.yml)
-- [actions.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/actions.yml)
-- [datasets.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/datasets.yml)
-- [pipelines.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/pipelines.yml)
-- [launch.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/launch.yml)
+- [organizations.yml](./templates/organizations.yml)
+- [teams.yml](./templates/teams.yml)
+- [workspaces.yml](./templates/workspaces.yml)
+- [participants.yml](./templates/participants.yml)
+- [credentials.yml](./templates/credentials.yml)
+- [secrets.yml](./templates/secrets.yml)
+- [compute-envs.yml](./templates/compute-envs.yml)
+- [actions.yml](./templates/actions.yml)
+- [datasets.yml](./templates/datasets.yml)
+- [labels.yml](./templates/labels.yml)
+- [pipelines.yml](./templates/pipelines.yml)
+- [launch.yml](./templates/launch.yml)
 
 ## Real world example
 
 Please see [`seqerakit-e2e.yml`](./examples/yaml/seqerakit-e2e.yml) for an end-to-end example that highlights how you can use `seqerakit` to create everything sequentially in Seqera Platform all the way from creating a new Organization to launching a pipeline.
 
 You can modify this YAML to similarly create Seqera Platform resources end-to-end for your setup. This YAML encodes environment variables to protect sensitive keys, usernames, and passwords that are required to create or add certain resources (i.e. credentials, compute environments). Prior to running it with `seqerakit examples/yaml/seqerakit-e2e.yml`, you will have to set the following environment variables:
 
@@ -354,14 +382,14 @@
 $AZURE_STORAGE_KEY
 $GOOGLE_KEY
 $SENTIEON_LICENSE_BASE64
 ```
 
 ## Contributions and Support
 
-If you would like to contribute to `seqerakit`, please see the [contributing guidelines](https://github.com/seqeralabs/seqera-kit/blob/main/.github/CONTRIBUTING.md).
+If you would like to contribute to `seqerakit`, please see the [contributing guidelines](./.github/CONTRIBUTING.md).
 
 For further information or help, please don't hesitate to create an [issue](https://github.com/seqeralabs/seqera-kit/issues) in this repository.
 
 ## Credits
 
 `seqerakit` was written by [Esha Joshi](https://github.com/ejseqera), [Adam Talbot](https://github.com/adamrtalbot) and [Harshil Patel](https://github.com/drpatelh) from the Scientific Development Team at [Seqera Labs](https://seqera.io/).
```

### Comparing `seqerakit-0.4.6/examples/python/launch_hello_world.py` & `seqerakit-0.4.7/examples/python/launch_hello_world.py`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/examples/yaml/compute-envs/seqera_aws_ireland_fusionv2_nvme.json` & `seqerakit-0.4.7/examples/yaml/compute-envs/seqera_aws_ireland_fusionv2_nvme.json`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/examples/yaml/compute-envs/seqera_aws_virginia_fusionv2_nvme.json` & `seqerakit-0.4.7/examples/yaml/compute-envs/seqera_aws_virginia_fusionv2_nvme.json`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/examples/yaml/datasets/rnaseq_samples.csv` & `seqerakit-0.4.7/examples/yaml/datasets/rnaseq_samples.csv`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/examples/yaml/datasets/sentieon_samples.csv` & `seqerakit-0.4.7/examples/yaml/datasets/sentieon_samples.csv`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/examples/yaml/datasets/viralrecon_illumina_samples.csv` & `seqerakit-0.4.7/examples/yaml/datasets/viralrecon_illumina_samples.csv`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/examples/yaml/e2e/compute-envs.yml` & `seqerakit-0.4.7/examples/yaml/e2e/compute-envs.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/examples/yaml/e2e/credentials.yml` & `seqerakit-0.4.7/examples/yaml/e2e/credentials.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/examples/yaml/e2e/datasets.yml` & `seqerakit-0.4.7/examples/yaml/e2e/datasets.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/examples/yaml/e2e/pipelines.yml` & `seqerakit-0.4.7/examples/yaml/e2e/pipelines.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/examples/yaml/pipelines/nf-core-sarek_pipeline.json` & `seqerakit-0.4.7/examples/yaml/pipelines/nf-core-sarek_pipeline.json`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/examples/yaml/pipelines/nf_core_rnaseq_pipeline.json` & `seqerakit-0.4.7/examples/yaml/pipelines/nf_core_rnaseq_pipeline.json`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/examples/yaml/pipelines/nf_core_viralrecon_nanopore_pipeline.json` & `seqerakit-0.4.7/examples/yaml/pipelines/nf_core_viralrecon_nanopore_pipeline.json`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/examples/yaml/pipelines/nf_sentieon_pipeline.json` & `seqerakit-0.4.7/examples/yaml/pipelines/nf_sentieon_pipeline.json`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/examples/yaml/seqerakit-e2e.yml` & `seqerakit-0.4.7/examples/yaml/seqerakit-e2e.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/seqerakit/cli.py` & `seqerakit-0.4.7/seqerakit/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 Requires a YAML file that defines the resources to be created in Seqera Platform and
 the required options for each resource based on the Seqera Platform CLI.
 """
 import argparse
 import logging
 import sys
 
-from pathlib import Path
 from seqerakit import seqeraplatform, helper, overwrite
 from seqerakit.seqeraplatform import ResourceExistsError, ResourceCreationError
 from seqerakit import __version__
 
 logger = logging.getLogger(__name__)
 
 
@@ -62,15 +61,14 @@
         help="Show version number and exit.",
     )
 
     # YAML processing options
     yaml_processing = parser.add_argument_group("YAML Processing Options")
     yaml_processing.add_argument(
         "yaml",
-        type=Path,
         nargs="*",
         help="One or more YAML files with Seqera Platform resource definitions.",
     )
     yaml_processing.add_argument(
         "--delete",
         action="store_true",
         help="Recursively delete resources defined in the YAML files.",
@@ -101,15 +99,15 @@
         handled by the 'add' method.
         """
         self.sp = sp
         self.list_for_add_method = list_for_add_method
         # Create an instance of Overwrite class
         self.overwrite_method = overwrite.Overwrite(self.sp)
 
-    def handle_block(self, block, args, destroy=False):
+    def handle_block(self, block, args, destroy=False, dryrun=False):
         # Check if delete is set to True, and call delete handler
         if destroy:
             logging.debug(" The '--delete' flag has been specified.\n")
             self.overwrite_method.handle_overwrite(
                 block, args["cmd_args"], overwrite=False, destroy=True
             )
             return
@@ -123,20 +121,20 @@
             "launch": lambda sp, args: helper.handle_generic_block(
                 sp, "launch", args, method_name=None
             ),
         }
 
         # Check if overwrite is set to True, and call overwrite handler
         overwrite_option = args.get("overwrite", False)
-        if overwrite_option:
+        if overwrite_option and dryrun is False:
             logging.debug(f" Overwrite is set to 'True' for {block}\n")
             self.overwrite_method.handle_overwrite(
                 block, args["cmd_args"], overwrite_option
             )
-        else:
+        elif dryrun is False:
             self.overwrite_method.handle_overwrite(block, args["cmd_args"])
 
         if block in self.list_for_add_method:
             helper.handle_generic_block(self.sp, block, args["cmd_args"])
         elif block in block_handler_map:
             block_handler_map[block](self.sp, args["cmd_args"])
         else:
@@ -150,29 +148,35 @@
     # If the info flag is set, run 'tw info'
     if options.info:
         sp = seqeraplatform.SeqeraPlatform()
         print(sp.info())
         return
 
     if not options.yaml:
-        logging.error(
-            " No YAML(s) provided. Please provide atleast one YAML configuration file."
-        )
-        sys.exit(1)
+        if sys.stdin.isatty():
+            logging.error(
+                " No YAML(s) provided and no input from stdin. Please provide "
+                "at least one YAML configuration file or pipe input from stdin."
+            )
+            sys.exit(1)
+        else:
+            options.yaml = [sys.stdin]
 
     # Parse CLI arguments into a list
     cli_args_list = options.cli_args.split() if options.cli_args else []
 
     sp = seqeraplatform.SeqeraPlatform(cli_args=cli_args_list, dryrun=options.dryrun)
 
     block_manager = BlockParser(
         sp,
         [
             "organizations",  # all use method.add
             "workspaces",
+            "labels",
+            "members",
             "credentials",
             "secrets",
             "actions",
             "datasets",
         ],
     )
 
@@ -180,15 +184,17 @@
     # and get a dictionary of command line arguments
     try:
         cmd_args_dict = helper.parse_all_yaml(options.yaml, destroy=options.delete)
         for block, args_list in cmd_args_dict.items():
             for args in args_list:
                 try:
                     # Run the 'tw' methods for each block
-                    block_manager.handle_block(block, args, destroy=options.delete)
+                    block_manager.handle_block(
+                        block, args, destroy=options.delete, dryrun=options.dryrun
+                    )
                 except (ResourceExistsError, ResourceCreationError) as e:
                     logging.error(e)
                     sys.exit(1)
     except ValueError as e:
         logging.error(e)
         sys.exit(1)
```

### Comparing `seqerakit-0.4.6/seqerakit/computeenvs.py` & `seqerakit-0.4.7/seqerakit/computeenvs.py`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/seqerakit/dump_yaml.py` & `seqerakit-0.4.7/seqerakit/dump_yaml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from seqerakit import seqeraplatform, utils
 import json
 import yaml
 import os
 from collections import OrderedDict
 
-# run json method for CEs, pipelines to retrieve names 
+# run json method for CEs, pipelines to retrieve names
 # run export to retrieve jsons
 # convert jsons to yaml with dict defining keys
 
+
 class DumpYaml:
     def __init__(self, sp, workspace):
         self.sp = sp
         self.workspace = workspace
         self.json_data = {}
         self.yaml_file_path = None
         self.workspace_objects = ["compute-envs", "pipelines"]
@@ -23,15 +24,15 @@
                     "workspace": "workspace",
                     "region": "region",
                     "workDir": "work-dir",
                     "waveEnabled": "wave",
                     "fusion2Enabled": "fusion-v2",
                     "nvnmeStorageEnabled": "fast-storage",
                     "type": "provisioning-model",
-                    "instanceType": "instance-types", # TODO
+                    "instanceType": "instance-types",  # TODO
                     "minCpus": "min-cpus",
                     "maxCpus": "max-cpus",
                     "ebsAutoScale": "no-ebs-autoscale",
                     "fargateHeadEnabled": "fargate",
                     "gpuEnabled": "gpu",
                 },
             ],
@@ -47,89 +48,96 @@
                     "paramsFile": "params-file",
                     "resume": "resume",
                     "pullLatest": "pull-latest",
                     "stubRun": "stub-run",
                     "pre-run": "pre-run",
                     "computeEnvId": "compute-env",
                 },
-            ]
+            ],
         }
 
     def generate_yaml_dump(self, yaml_file):
         # Get path to yaml file
         self.yaml_file_path = yaml_file
 
         # Initialize a dictionary to hold object names for each type of workspace object
         object_names_dict = {obj: [] for obj in self.workspace_objects}
 
         # Get names of objects defined in workspace_objects through CLI command
         # Assuming get_names returns a dictionary where keys are object types and values are lists of names
         object_names = self.get_names()
-        
+
         # Append the names to the corresponding object in object_names_dict
         for obj, names in object_names.items():
             if obj in object_names_dict:
-                object_names_dict[obj].extend(names if isinstance(names, list) else [names])
-        
+                object_names_dict[obj].extend(
+                    names if isinstance(names, list) else [names]
+                )
+
         # For each type of object, get its exports and transform the data
         for object_type, names in object_names_dict.items():
             for name in names:
                 json_output = self.get_object_exports(object_type, name)
                 if object_type == "compute-envs":
-                    json_data = self.transform_data(json_output, object_type, name, primary_key="discriminator")
+                    json_data = self.transform_data(
+                        json_output, object_type, name, primary_key="discriminator"
+                    )
                 else:
                     json_data = self.transform_data(json_output, object_type, name)
                 print(f"generating the yaml file for {object_type} - {name}")
-                
-                with open(f"{self.yaml_file_path}_{object_type}_{name}.yaml", 'w') as yaml_file:
+
+                with open(
+                    f"{self.yaml_file_path}_{object_type}_{name}.yaml", "w"
+                ) as yaml_file:
                     yaml.dump(json_data, yaml_file, sort_keys=False)
-    
+
     def get_names(self):
         object_names_dict = {}
         for object in self.workspace_objects:
             cli_method = getattr(self.sp, object)
             json_data = cli_method("list", "-w", self.workspace, to_json=True)
-            
+
             # Extract names for this specific object type
             names = self._extract_values_by_key(json_data, "name")
             print(f"names for {object} are: {names}")
 
             # Store names in dictionary under the respective object type
             object_names_dict[object] = names
 
         return object_names_dict
-    
+
     def get_object_exports(self, object, object_name):
         # Use names retrived to export jsons through CLI command
         json_data = {}
         cli_method = getattr(self.sp, object)
         # for name in object_names:
-        cli_method("export", f"{object_name}.json", "-w", self.workspace, "-n", object_name)
-        
-        with open(f"{object_name}.json", 'r') as json_file:
+        cli_method(
+            "export", f"{object_name}.json", "-w", self.workspace, "-n", object_name
+        )
+
+        with open(f"{object_name}.json", "r") as json_file:
             json_data = json.load(json_file)
 
         # remove the json file after loading it
         # os.remove(f"{object_name}.json")
         return json_data
-    
+
     # def transform_data(self, json_data, object_type, object_name=None, primary_key="name"):
     #     mapping = self.yaml_keys[object_type][0]
     #     result = {object_type: []}
 
     #     # Use a list of tuples to maintain order
     #     ordered_env = []
 
     #     # Ensure primary_key is the first key
     #     primary_mapped_key = mapping.get(primary_key, primary_key)
     #     primary_value = object_name if primary_key == 'name' else json_data.get(primary_key)
     #     if primary_value is not None:
     #         ordered_env.append((primary_mapped_key, primary_value))
 
-
     #     # Specific handling for 'compute-envs'
     #     if object_type == "compute-envs":
     #         # Determine config-mode based on the key present in json_data
     #         config_mode = next((key for key in ['forge', 'manual'] if key in json_data), 'manual')
     #         ordered_env.append(('config-mode', config_mode))
     #         ordered_env.append(("name", object_name))
 
@@ -165,81 +173,108 @@
     #     ordered_env.extend(transformed_nested.items())
 
     #     # Convert to a regular dictionary just before serialization
     #     env = dict(ordered_env)
     #     result[object_type].append(env)
     #     return result
 
-    def transform_data(self, json_data, object_type, object_name=None, primary_key="name"):
+    def transform_data(
+        self, json_data, object_type, object_name=None, primary_key="name"
+    ):
         mapping = self.yaml_keys[object_type][0]
         result = {object_type: []}
         ordered_env = []
 
         # Ensure primary_key is the first key
         primary_mapped_key = mapping.get(primary_key, primary_key)
-        primary_value = object_name if primary_key == 'name' else json_data.get(primary_key)
+        primary_value = (
+            object_name if primary_key == "name" else json_data.get(primary_key)
+        )
         if primary_value is not None:
             ordered_env.append((primary_mapped_key, primary_value))
 
         # Process keys based on object_type
         if object_type == "compute-envs":
-            self._process_compute_envs(json_data, ordered_env, mapping, object_name, primary_key)
+            self._process_compute_envs(
+                json_data, ordered_env, mapping, object_name, primary_key
+            )
 
         elif object_type == "pipelines":
             self._process_pipelines(json_data, ordered_env, mapping, object_name)
 
         # Convert to a regular dictionary just before serialization
         env = dict(ordered_env)
         result[object_type].append(env)
         return result
 
-    def _process_compute_envs(self, json_data, ordered_env, mapping, object_name, primary_key):
-        config_mode = next((key for key in ['forge', 'manual'] if key in json_data), 'manual')
-        ordered_env.append(('config-mode', config_mode))
+    def _process_compute_envs(
+        self, json_data, ordered_env, mapping, object_name, primary_key
+    ):
+        config_mode = next(
+            (key for key in ["forge", "manual"] if key in json_data), "manual"
+        )
+        ordered_env.append(("config-mode", config_mode))
         ordered_env.append(("name", object_name))
         for key, new_key in mapping.items():
             if key == primary_key:
                 continue  # Skip as primary_key is already handled
             if key in json_data:
                 # Directly assign if value is a list
-                value = json_data[key] if isinstance(json_data[key], list) else json_data[key]
+                value = (
+                    json_data[key]
+                    if isinstance(json_data[key], list)
+                    else json_data[key]
+                )
                 ordered_env.append((new_key, value))
-            if key == 'workspace':
+            if key == "workspace":
                 ordered_env.append((new_key, self.workspace))
             elif config_mode in json_data:
-                transformed_nested = self._transform_nested_structure(json_data[config_mode], mapping)
+                transformed_nested = self._transform_nested_structure(
+                    json_data[config_mode], mapping
+                )
                 ordered_env.extend(transformed_nested.items())
 
     def _process_pipelines(self, json_data, ordered_env, mapping, object_name):
-        launch_data = json_data['launch']
+        launch_data = json_data["launch"]
         transformed_nested = self._transform_nested_structure(launch_data, mapping)
 
         for key, new_key in mapping.items():
             if key == "description":
                 ordered_env.append((new_key, json_data[key]))
             elif key == "workspace":
                 ordered_env.append((new_key, self.workspace))
 
         # Handle 'configText' and 'paramsText' in 'launch'
-        for special_key, file_type, new_key in [('configText', 'config', 'config'), ('paramsText', 'yaml', 'params-file')]:
+        for special_key, file_type, new_key in [
+            ("configText", "config", "config"),
+            ("paramsText", "yaml", "params-file"),
+        ]:
             if special_key in launch_data:
-                file_path = self._write_special_file(launch_data[special_key], object_name, file_type)
-                transformed_nested[new_key] = file_path  # Use the file path as the value for the new key
+                file_path = self._write_special_file(
+                    launch_data[special_key], object_name, file_type
+                )
+                transformed_nested[
+                    new_key
+                ] = file_path  # Use the file path as the value for the new key
 
         ordered_env.extend(transformed_nested.items())
-   
+
     def _transform_nested_structure(self, nested_data, mapping):
         transformed_data = {}
         for key in nested_data:
             if key in mapping:
                 new_key = mapping[key]
                 # Directly assign the value if it's a list
-                transformed_data[new_key] = nested_data[key] if isinstance(nested_data[key], list) else nested_data[key]
+                transformed_data[new_key] = (
+                    nested_data[key]
+                    if isinstance(nested_data[key], list)
+                    else nested_data[key]
+                )
         return transformed_data
-    
+
     def _extract_values_by_key(self, json_data, target_key):
         def extract_recursively(data, key, collected_values):
             if isinstance(data, dict):
                 for k, v in data.items():
                     if k == key:
                         collected_values.append(v)
                     else:
@@ -250,32 +285,32 @@
 
         extracted_values = []
         extract_recursively(json_data, target_key, extracted_values)
         return extracted_values
 
     def _write_special_file(self, content, object_name, file_type):
         file_path = f"{object_name}.{file_type}"
-        
-        with open(file_path, 'w') as file:
-                if file_type == 'config':
-                    file.write(content)
-                elif file_type == 'yaml':
-                    # pyyaml is so annoying so I just write the string to the file manually
-                    # yaml.dump(content, file, default_flow_style=False, default_style=None)
-                    file.write(content)
+
+        with open(file_path, "w") as file:
+            if file_type == "config":
+                file.write(content)
+            elif file_type == "yaml":
+                # pyyaml is so annoying so I just write the string to the file manually
+                # yaml.dump(content, file, default_flow_style=False, default_style=None)
+                file.write(content)
 
         return file_path
 
 
-  # def _transform_nested_structure(self, nested_data, mapping):
-    #     transformed_data = {}
-    #     for key in nested_data:
-    #         if key in mapping:
-    #             new_key = mapping[key]
-    #             transformed_data[new_key] = nested_data[key]
-    #     return transformed_data
-    #   
+# def _transform_nested_structure(self, nested_data, mapping):
+#     transformed_data = {}
+#     for key in nested_data:
+#         if key in mapping:
+#             new_key = mapping[key]
+#             transformed_data[new_key] = nested_data[key]
+#     return transformed_data
+#
 # testing stuff
 sp = seqeraplatform.SeqeraPlatform()
 workspace = "quicklaunch/testing"
 dp = DumpYaml(sp, workspace)
-dp.generate_yaml_dump("test")
+dp.generate_yaml_dump("test")
```

### Comparing `seqerakit-0.4.6/seqerakit/helper.py` & `seqerakit-0.4.7/seqerakit/helper.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """
 This file contains helper functions for the library.
 Including handling methods for each block in the YAML file, and parsing
 methods for each block in the YAML file.
 """
 import yaml
 from seqerakit import utils
+import sys
 
 
 def parse_yaml_block(yaml_data, block_name):
     # Get the name of the specified block/resource.
     block = yaml_data.get(block_name)
 
     # If block is not found in the YAML, return an empty list.
@@ -32,71 +33,98 @@
     # Initialize an empty list to hold the lists of command line arguments.
     cmd_args_list = []
 
     # Initialize a set to track the --name values within the block.
     name_values = set()
 
     # Iterate over each item in the block.
+    # TODO: fix for resources that can be duplicate named in an org
     for item in block:
         cmd_args = parse_block(block_name, item)
         name = find_name(cmd_args)
         if name in name_values:
             raise ValueError(
-                f" Duplicate 'name' specified in config file"
-                f" for {block_name}: {name}. Please specify a unique name."
+                f" Duplicate name key specified in config file"
+                f" for {block_name}: {name}. Please specify a unique value."
             )
         name_values.add(name)
 
         cmd_args_list.append(cmd_args)
 
     # Return the block name and list of command line argument lists.
     return block_name, cmd_args_list
 
 
 def parse_all_yaml(file_paths, destroy=False):
     # If multiple yamls, merge them into one dictionary
     merged_data = {}
 
-    for file_path in file_paths:
-        with open(file_path, "r") as f:
-            data = yaml.safe_load(f)
+    # Special handling for stdin represented by "-"
+    if not file_paths or "-" in file_paths:
+        # Read YAML directly from stdin
+        data = yaml.safe_load(sys.stdin)
+        if not data:
+            raise ValueError(
+                " The input from stdin is empty or does not contain valid YAML data."
+            )
+        merged_data.update(data)
 
-            # Check if the YAML file is empty or contains no valid data
-            if data is None or not data:
-                raise ValueError(
-                    f" The file '{file_path}' is empty or does not contain valid data."
-                )
+    for file_path in file_paths:
+        if file_path == "-":
+            continue
+        try:
+            with open(file_path, "r") as f:
+                data = yaml.safe_load(f)
+                if not data:
+                    raise ValueError(
+                        f" The file '{file_path}' is empty or "
+                        "does not contain valid data."
+                    )
 
-            for key, value in data.items():
+            for key, new_value in data.items():
                 if key in merged_data:
-                    try:
-                        merged_data[key].extend(value)
-                    except AttributeError:
-                        merged_data[key] = [merged_data[key], value]
+                    if isinstance(new_value, list) and all(
+                        isinstance(i, dict) for i in new_value
+                    ):
+                        # Handle list of dictionaries & merge without duplication
+                        existing_items = {
+                            tuple(sorted(d.items())) for d in merged_data[key]
+                        }
+                        for item in new_value:
+                            if tuple(sorted(item.items())) not in existing_items:
+                                merged_data[key].append(item)
+                    else:
+                        # override if not list of dictionaries
+                        merged_data[key] = new_value
                 else:
-                    merged_data[key] = value
+                    merged_data[key] = new_value
+        except FileNotFoundError:
+            print(f"Error: The file '{file_path}' was not found.")
+            sys.exit(1)
 
     block_names = list(merged_data.keys())
 
     # Define the order in which the resources should be created.
     resource_order = [
         "organizations",
         "teams",
         "workspaces",
+        "labels",
+        "members",
         "participants",
         "credentials",
         "compute-envs",
         "secrets",
         "actions",
         "datasets",
         "pipelines",
         "launch",
     ]
 
-    # Reverse the order of resources if destroy is True
+    # Reverse the order of resources to delete if destroy is True
     if destroy:
         resource_order = resource_order[:-1][::-1]
 
     # Initialize an empty dictionary to hold all the command arguments.
     cmd_args_dict = {}
 
     # Iterate over each block name in the desired order.
@@ -336,14 +364,33 @@
             break
         elif ".json" in arg:
             method("import", *args)
 
 
 def find_name(cmd_args):
     """
-    Find and return the value associated with --name in the cmd_args list.
+    Find and return the value associated with --name in cmd_args, where cmd_args
+    can be a list, a tuple of lists, or nested lists/tuples.
+
+    The function searches for the following keys: --name, --user, --email.
+
+    Parameters:
+    - cmd_args: The command arguments (list, tuple, or nested structures).
+
+    Returns:
+    - The value associated with the first key found, or None if none are found.
     """
-    args_list = cmd_args.get("cmd_args", [])
-    for i in range(len(args_list) - 1):
-        if args_list[i] == "--name":
-            return args_list[i + 1]
-    return None
+    # Predefined list of keys to search for
+    keys = {"--name", "--user", "--email"}
+
+    def search(args):
+        it = iter(args)
+        for arg in it:
+            if isinstance(arg, str) and arg in keys:
+                return next(it, None)
+            elif isinstance(arg, (list, tuple)):
+                result = search(arg)
+                if result is not None:
+                    return result
+        return None
+
+    return search(cmd_args.get("cmd_args", []))
```

### Comparing `seqerakit-0.4.6/seqerakit/overwrite.py` & `seqerakit-0.4.7/seqerakit/overwrite.py`

 * *Files 13% similar despite different names*

```diff
@@ -56,14 +56,24 @@
         # Define special handlers for resources deleted with specific args
         self.block_operations = {
             "organizations": {
                 "keys": ["name"],
                 "method_args": self._get_organization_args,
                 "name_key": "orgName",
             },
+            "labels": {
+                "keys": ["name", "value", "workspace"],
+                "method_args": self._get_label_args,
+                "name_key": "name",
+            },
+            "members": {
+                "keys": ["user", "organization"],
+                "method_args": self._get_members_args,
+                "name_key": "email",
+            },
             "teams": {
                 "keys": ["name", "organization"],
                 "method_args": self._get_team_args,
                 "name_key": "name",
             },
             "participants": {
                 "keys": ["name", "type", "workspace"],
@@ -97,14 +107,17 @@
             )
 
             if block == "participants":
                 if sp_args.get("type") == "TEAM":
                     self.block_operations["participants"]["name_key"] = "teamName"
                 else:
                     self.block_operations["participants"]["name_key"] = "email"
+            elif block == "members":
+                # Rename the user key to name to correctly index JSON data
+                sp_args["name"] = sp_args.pop("user")
             if self.check_resource_exists(operation["name_key"], sp_args):
                 # if resource exists and overwrite is true, delete
                 if overwrite:
                     logging.debug(
                         f" The attempted {block} resource already exists."
                         " Overwriting.\n"
                     )
@@ -141,14 +154,26 @@
 
         # Get the teamId from the json data
         team_id = utils.find_key_value_in_dict(
             json.loads(json_out), "name", args["name"], "teamId"
         )
         return ("delete", "--id", str(team_id), "--organization", args["organization"])
 
+    def _get_members_args(self, args):
+        """
+        Returns a list of arguments for the delete() method for members.
+        """
+        return (
+            "delete",
+            "--user",
+            args["name"],
+            "--organization",
+            args["organization"],
+        )
+
     def _get_participant_args(self, args):
         """
         Returns a list of arguments for the delete() method for participants.
         Works for both teams and members where if the type is TEAM, the teamName
         is used to delete, and if the type is MEMBER, the email is used to delete.
         """
         method_args = (
@@ -167,14 +192,23 @@
         Returns a list of arguments for the delete() method for workspaces. The
         workspaceId used to delete will be retrieved using the _find_workspace_id()
         method.
         """
         workspace_id = self._find_workspace_id(args["organization"], args["name"])
         return ("delete", "--id", str(workspace_id))
 
+    def _get_label_args(self, args):
+        """
+        Returns a list of arguments for the delete() method for labels. The
+        label_id used to delete will be retrieved using the _find_label_id()
+        method.
+        """
+        label_id = self._find_label_id(args["name"], args["value"])
+        return ("delete", "--id", str(label_id), "-w", args["workspace"])
+
     def _get_generic_deletion_args(self, args):
         """
         Returns a list of arguments for the delete() method for resources that
         are deleted with --name and --workspace.
         """
         return (
             "delete",
@@ -198,27 +232,38 @@
         """
         json_method = getattr(self.sp, "-o json")
         sp_args = []  # Default value for sp_args
 
         # Check if block data already exists
         if block in self.block_jsondata:
             self.cached_jsondata = self.block_jsondata[block]
-            sp_args = self._get_values_from_cmd_args(args, keys_to_get)
+            if block == "teams":
+                sp_args = self._get_values_from_cmd_args(args[0], keys_to_get)
+            else:
+                sp_args = self._get_values_from_cmd_args(args, keys_to_get)
         else:
             # Fetch the data if it does not exist
             if block == "teams":
                 sp_args = self._get_values_from_cmd_args(args[0], keys_to_get)
                 self.cached_jsondata = json_method(
                     block, "list", "-o", sp_args["organization"]
                 )
-            elif block in Overwrite.generic_deletion or block == "participants":
+            elif block in Overwrite.generic_deletion or block in {
+                "participants",
+                "labels",
+            }:
                 sp_args = self._get_values_from_cmd_args(args, keys_to_get)
                 self.cached_jsondata = json_method(
                     block, "list", "-w", sp_args["workspace"]
                 )
+            elif block == "members" or block == "workspaces":  # TODO
+                sp_args = self._get_values_from_cmd_args(args, keys_to_get)
+                self.cached_jsondata = json_method(
+                    block, "list", "-o", sp_args["organization"]
+                )
             else:
                 sp_args = self._get_values_from_cmd_args(args, keys_to_get)
                 self.cached_jsondata = json_method(block, "list")
 
         # Store this data in the block_jsondata dict for later use
         self.block_jsondata[block] = self.cached_jsondata
         return self.cached_jsondata, sp_args
@@ -267,7 +312,19 @@
         for workspace in workspaces:
             if (
                 workspace.get("orgName") == organization
                 and workspace.get("workspaceName") == workspace_name
             ):
                 return workspace.get("workspaceId")
         return None
+
+    def _find_label_id(self, label_name, label_value):
+        """
+        Custom method to find a label ID in a nested dictionary with a given
+        workspace name. This ID will be used to delete the label.
+        """
+        jsondata = json.loads(self.cached_jsondata)
+        labels = jsondata["labels"]
+        for label in labels:
+            if label.get("name") == label_name and label.get("value") == label_value:
+                return label.get("id")
+        return None
```

### Comparing `seqerakit-0.4.6/seqerakit/pipelines.py` & `seqerakit-0.4.7/seqerakit/pipelines.py`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/seqerakit/seqeraplatform.py` & `seqerakit-0.4.7/seqerakit/seqeraplatform.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,16 +92,16 @@
         logging.debug(f" Running command: {full_cmd}")
         process = subprocess.Popen(
             full_cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True
         )
         stdout, _ = process.communicate()
         stdout = stdout.decode("utf-8").strip()
 
-        if "ERROR: " in stdout:
-            self._handle_command_errors(stdout)
+        if "ERROR: " in stdout or process.returncode != 0:
+            self._handle_command_errors(str(stdout))
 
         return json.loads(stdout) if to_json else stdout
 
     def _execute_info_command(self):
         # Directly execute 'tw info' command
         command = "tw info"
         return self._execute_command(command)
@@ -110,19 +110,19 @@
         logging.error(stdout)
 
         # Check for specific tw cli error patterns and raise custom exceptions
         if re.search(
             r"ERROR: .*already (exists|a participant)", stdout, flags=re.IGNORECASE
         ):
             raise ResourceExistsError(
-                " Resource already exists. Please delete first or set 'overwrite: true'"
+                "Resource already exists. Please delete first or set 'overwrite: true'"
             )
         else:
             raise ResourceCreationError(
-                f" Resource creation failed: '{stdout}'. "
+                f"Resource creation failed: '{stdout}'. "
                 "Check your config and try again."
             )
 
     def _tw_run(self, cmd, *args, **kwargs):
         full_cmd = self._construct_command(cmd, *args, **kwargs)
         if not full_cmd or self.dryrun:
             logging.debug(f"DRYRUN: Running command {full_cmd}")
```

### Comparing `seqerakit-0.4.6/seqerakit/utils.py` & `seqerakit-0.4.7/seqerakit/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 def check_if_exists(json_data, namekey, namevalue):
     """
     Wrapper around find_key_value_in_dict() to validate that a resource was
     created successfully in Seqera Platform by looking for the name and value.
     """
     if not json_data:
         return False
-    logging.info(f"Checking if {namekey} {namevalue} exists in Seqera Platform...")
+    logging.info(f" Checking if {namekey} {namevalue} exists in Seqera Platform...")
     # Regex pattern to match environment variables in the string
     env_var_pattern = re.compile(r"\$\{?[\w]+\}?")
 
     # Substitute environment variables in namevalue
     resolved_value = env_var_pattern.sub(replace_env_var, namevalue)
 
     data = json.loads(json_data)
```

### Comparing `seqerakit-0.4.6/seqerakit.egg-info/PKG-INFO` & `seqerakit-0.4.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,21 @@
-Metadata-Version: 2.1
-Name: seqerakit
-Version: 0.4.6
-Summary: Automate creation of Seqera Platform resources
-Home-page: https://github.com/seqeralabs/seqera-kit
-Author: Esha Joshi, Adam Talbot, Harshil Patel
-Author-email: esha.joshi@seqera.io, adam.talbot@seqera.io, harshil.patel@seqera.io
-License: Apache 2.0
-Keywords: nextflow,bioinformatics,workflow,pipeline,seqera-platform,seqera
-Requires-Python: >=3.8, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # <img src="https://raw.githubusercontent.com/seqeralabs/seqera-kit/main/assets/seqerakit.svg" width=50 alt="seqerakit logo"> seqerakit
 
+
 `seqerakit` is a Python wrapper for the [Seqera Platform CLI](https://github.com/seqeralabs/tower-cli). It can be leveraged to automate the creation of all of the entities in Seqera Platform via a simple configuration file in YAML format.
 
 The key features are:
 
 - **Simple configuration**: All of the command-line options available when using the Seqera Platform CLI can be defined in simple YAML format.
 - **Infrastructure as Code**: Enable users to manage and provision their infrastructure specifications.
 - **Automation**: End-to-end creation of entities within Seqera Platform, all the way from adding an Organization to launching pipeline(s) within that Organization.
 
 ## Prerequisites
 
-You will need to have an account on Seqera Platform (see [Plans and pricing](https://cloud.tower.nf/pricing/)).
+You will need to have an account on Seqera Platform (see [Plans and pricing](https://seqera.io/pricing/)).
 
 ## Installation
 
 `seqerakit` requires the following dependencies:
 
 1. [Seqera Platform CLI (`>=0.9.2`)](https://github.com/seqeralabs/tower-cli#1-installation)
 
@@ -86,27 +74,27 @@
 You can verify your installation with:
 ```bash
 pip show seqerakit
 ```
 
 ## Configuration
 
-Create a Seqera Platform access token using the [Seqera Platform](https://tower.nf/) web interface via the **Your Tokens** page in your profile.
+Create a Seqera Platform access token using the [Seqera Platform](https://seqera.io/) web interface via the **Your Tokens** page in your profile.
 
 `seqerakit` reads this token from the environment variable `TOWER_ACCESS_TOKEN`. Please export it into your terminal as shown below:
 
 ```bash
 export TOWER_ACCESS_TOKEN=<Your access token>
 ```
 
 For Enterprise installations of Seqera Platform, you will also need to configure the API endpoint that will be used to connect to the Platform. You can do so by exporting the following environment variable:
 ```bash
 export TOWER_API_ENDPOINT=<Tower API URL>
 ```
-By default, this is set to `https://api.tower.nf` to connect to Seqera Platform Cloud.
+By default, this is set to `https://api.cloud.seqera.io` to connect to Seqera Platform Cloud.
 
 
 ## Usage
 
 To confirm the installation of `seqerakit`, configuration of the Seqera Platform CLI and connection to the Platform is working as expected. This will run the `tw info` command under the hood:
 
 ```bash
@@ -118,14 +106,26 @@
 seqerakit --help
 ```
 
 Use `--version` or `-v` to retrieve the current version of your seqerakit installation:
 ```bash
 seqerakit --version
 ```
+### Input
+`seqerakit` supports input through either file paths to YAMLs or directly from standard input (stdin).
+
+#### Using File Path
+```bash
+seqerakit /path/to/file.yaml
+```
+#### Using stdin
+```console
+$ cat file.yaml | seqerakit -
+```
+See the [Defining your YAML file using CLI options](#defining-your-yaml-file-using-cli-options) section for guidance on formatting your input YAML file(s).
 
 ### Dryrun
 
 To print the commands that would executed with `tw` when using a YAML file, you can run `seqerakit` with the `--dryrun` flag:
 
 ```bash
 seqerakit file.yaml --dryrun
@@ -217,15 +217,15 @@
 
 DEBUG:root: Running command: tw organizations delete --name $SEQERA_ORGANIZATION_NAME
 DEBUG:root: Running command: tw organizations add --name $SEQERA_ORGANIZATION_NAME --full-name $SEQERA_ORGANIZATION_NAME --description 'Example of an organization'
 ```
 ### 3. Specifying JSON configuration files with `file-path`
 The Seqera Platform CLI allows export and import of entities through JSON configuration files for pipelines and compute environments. To use these files to add a pipeline or compute environment to a workspace, use the `file-path` key to specify a path to a JSON configuration file.
 
-An example of the `file-path` option is provided in the [compute-envs.yml](templates/compute-envs.yml) template:
+An example of the `file-path` option is provided in the [compute-envs.yml](./templates/compute-envs.yml) template:
 
 ```yaml
 compute-envs:
   - name: 'my_aws_compute_environment'                              # required
     workspace: 'my_organization/my_workspace'                       # required
     credentials: 'my_aws_credentials'                               # required
     wait: 'AVAILABLE'                                               # optional
@@ -234,15 +234,15 @@
 ```
 
 
 ## Quick start
 
 You must provide a YAML file that defines the options for each of the entities you would like to create in Seqera Platform.
 
-You will need to have an account on Seqera Platform (see [Plans and pricing](https://cloud.tower.nf/pricing/)). You will also need access to a Workspace and a pre-defined Compute Environment where you can launch a pipeline.
+You will need to have an account on Seqera Platform (see [Plans and pricing](https://seqera.io/pricing/)). You will also need access to a Workspace and a pre-defined Compute Environment where you can launch a pipeline.
 
 ### Launch via YAML
 
 1. Create a YAML file called `hello-world-config.yml` with the contents below, and customise the `<YOUR_WORKSPACE>` and `<YOUR_COMPUTE_ENVIRONMENT>` entries as required:
 
    ```yaml # noqa
    launch:
@@ -261,15 +261,15 @@
 
 3. Login to your Seqera Platform instance and check the Runs page in the appropriate Workspace for the pipeline you just launched!
 
 ### Launch via a Python script
 
 You can also launch the same pipeline via a Python script. This will essentially allow you to extend the functionality on offer within the Seqera Platform CLI by leveraging the flexibility and customisation options available in Python.
 
-1. Download the [`launch_hello_world.py`](https://github.com/seqeralabs/seqera-kit/blob/main/examples/python/launch_hello_world.py) Python script and customise the `<YOUR_WORKSPACE>` and `<YOUR_COMPUTE_ENVIRONMENT>` entries as required.
+1. Download the [`launch_hello_world.py`](./examples/python/launch_hello_world.py) Python script and customise the `<YOUR_WORKSPACE>` and `<YOUR_COMPUTE_ENVIRONMENT>` entries as required.
 
 2. Launch the pipeline with `seqerakit`:
 
 ```bash
    python launch_hello_world.py
 ```
 
@@ -328,32 +328,33 @@
 - `name`, `url`, `workspace`, etc., are the keys derived from the CLI options.
 - The corresponding values are user-defined
 
 ### Best Practices:
 - Ensure that the indentation and structure of the YAML file are correct - YAML is sensitive to formatting.
 - Use quotes around strings that contain special characters or spaces.
 - When listing multiple values (`labels`, `instance-types`, `allow-buckets`, etc), separate them with commas as shown above.
-- For complex configurations, refer to the [Templates](/templates/) provided in this repository.
+- For complex configurations, refer to the [Templates](./templates/) provided in this repository.
 
 
 ## Templates
 
 We have provided template YAML files for each of the entities that can be created on Seqera Platform. These can be found in the [`templates/`](https://github.com/seqeralabs/blob/main/seqera-kit/templates) directory and should form a good starting point for you to add your own customization:
 
-- [organizations.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/organizations.yml)
-- [teams.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/teams.yml)
-- [workspaces.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/workspaces.yml)
-- [participants.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/participants.yml)
-- [credentials.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/credentials.yml)
-- [secrets.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/secrets.yml)
-- [compute-envs.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/compute-envs.yml)
-- [actions.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/actions.yml)
-- [datasets.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/datasets.yml)
-- [pipelines.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/pipelines.yml)
-- [launch.yml](https://github.com/seqeralabs/seqera-kit/blob/main/templates/launch.yml)
+- [organizations.yml](./templates/organizations.yml)
+- [teams.yml](./templates/teams.yml)
+- [workspaces.yml](./templates/workspaces.yml)
+- [participants.yml](./templates/participants.yml)
+- [credentials.yml](./templates/credentials.yml)
+- [secrets.yml](./templates/secrets.yml)
+- [compute-envs.yml](./templates/compute-envs.yml)
+- [actions.yml](./templates/actions.yml)
+- [datasets.yml](./templates/datasets.yml)
+- [labels.yml](./templates/labels.yml)
+- [pipelines.yml](./templates/pipelines.yml)
+- [launch.yml](./templates/launch.yml)
 
 ## Real world example
 
 Please see [`seqerakit-e2e.yml`](./examples/yaml/seqerakit-e2e.yml) for an end-to-end example that highlights how you can use `seqerakit` to create everything sequentially in Seqera Platform all the way from creating a new Organization to launching a pipeline.
 
 You can modify this YAML to similarly create Seqera Platform resources end-to-end for your setup. This YAML encodes environment variables to protect sensitive keys, usernames, and passwords that are required to create or add certain resources (i.e. credentials, compute environments). Prior to running it with `seqerakit examples/yaml/seqerakit-e2e.yml`, you will have to set the following environment variables:
 
@@ -367,14 +368,14 @@
 $AZURE_STORAGE_KEY
 $GOOGLE_KEY
 $SENTIEON_LICENSE_BASE64
 ```
 
 ## Contributions and Support
 
-If you would like to contribute to `seqerakit`, please see the [contributing guidelines](https://github.com/seqeralabs/seqera-kit/blob/main/.github/CONTRIBUTING.md).
+If you would like to contribute to `seqerakit`, please see the [contributing guidelines](./.github/CONTRIBUTING.md).
 
 For further information or help, please don't hesitate to create an [issue](https://github.com/seqeralabs/seqera-kit/issues) in this repository.
 
 ## Credits
 
 `seqerakit` was written by [Esha Joshi](https://github.com/ejseqera), [Adam Talbot](https://github.com/adamrtalbot) and [Harshil Patel](https://github.com/drpatelh) from the Scientific Development Team at [Seqera Labs](https://seqera.io/).
```

### Comparing `seqerakit-0.4.6/seqerakit.egg-info/SOURCES.txt` & `seqerakit-0.4.7/seqerakit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 examples/yaml/datasets/sentieon_samples.csv
 examples/yaml/datasets/viralrecon_illumina_samples.csv
 examples/yaml/datasets/viralrecon_nanopore_samples.csv
 examples/yaml/e2e/actions.yml
 examples/yaml/e2e/compute-envs.yml
 examples/yaml/e2e/credentials.yml
 examples/yaml/e2e/datasets.yml
+examples/yaml/e2e/labels.yml
+examples/yaml/e2e/members.yml
 examples/yaml/e2e/organizations.yml
 examples/yaml/e2e/participants.yml
 examples/yaml/e2e/pipelines.yml
 examples/yaml/e2e/secrets.yml
 examples/yaml/e2e/teams.yml
 examples/yaml/e2e/workspaces.yml
 examples/yaml/pipelines/nextflow.config
@@ -57,15 +59,17 @@
 seqerakit.egg-info/not-zip-safe
 seqerakit.egg-info/requires.txt
 seqerakit.egg-info/top_level.txt
 templates/actions.yml
 templates/compute-envs.yml
 templates/credentials.yml
 templates/datasets.yml
+templates/labels.yml
 templates/launch.yml
+templates/members.yml
 templates/organizations.yml
 templates/participants.yml
 templates/pipelines.yml
 templates/secrets.yml
 templates/teams.yml
 templates/workspaces.yml
 tests/e2e/aws-e2e.yml
```

### Comparing `seqerakit-0.4.6/setup.py` & `seqerakit-0.4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
-VERSION = "0.4.6"
+VERSION = "0.4.7"
 
 with open("README.md") as f:
     readme = f.read()
 
 setup(
     name="seqerakit",
     version=VERSION,
```

### Comparing `seqerakit-0.4.6/templates/actions.yml` & `seqerakit-0.4.7/templates/actions.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/templates/compute-envs.yml` & `seqerakit-0.4.7/templates/compute-envs.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/templates/credentials.yml` & `seqerakit-0.4.7/templates/credentials.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/templates/launch.yml` & `seqerakit-0.4.7/templates/launch.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/templates/participants.yml` & `seqerakit-0.4.7/templates/participants.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/templates/pipelines.yml` & `seqerakit-0.4.7/templates/pipelines.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/tests/e2e/aws-e2e.yml` & `seqerakit-0.4.7/tests/e2e/aws-e2e.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.6/tests/unit/test_helper.py` & `seqerakit-0.4.7/tests/unit/test_helper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from unittest.mock import mock_open
+from unittest.mock import patch, mock_open
 from seqerakit import helper
 import yaml
 import pytest
+from io import StringIO
 
 
 # Fixture to mock a YAML file
 @pytest.fixture
 def mock_yaml_file(mocker):
     def _mock_yaml_file(test_data, file_name="mock_file.yaml"):
         # Convert test data to YAML format
@@ -44,16 +45,16 @@
                 "test_organization1",
                 "--url",
                 "https://example.com",
             ],
             "overwrite": True,
         }
     ]
-
     file_path = mock_yaml_file(test_data)
+    print(f"debug - file_path: {file_path}")
     result = helper.parse_all_yaml([file_path])
 
     assert "organizations" in result
     assert result["organizations"] == expected_block_output
 
 
 def test_create_mock_workspace_yaml(mock_yaml_file):
@@ -262,25 +263,138 @@
     file_path = mock_yaml_file(test_data)
     result = helper.parse_all_yaml([file_path])
 
     assert "pipelines" in result
     assert result["pipelines"] == expected_block_output
 
 
+def test_create_mock_teams_yaml(mock_yaml_file):
+    test_data = {
+        "teams": [
+            {
+                "name": "test_team1",
+                "organization": "my_organization",
+                "description": "My test team 1",
+                "members": ["user1@org.io"],
+                "overwrite": True,
+            },
+        ]
+    }
+    expected_block_output = [
+        {
+            "cmd_args": (
+                [
+                    "--description",
+                    "My test team 1",
+                    "--name",
+                    "test_team1",
+                    "--organization",
+                    "my_organization",
+                ],
+                [
+                    [
+                        "--team",
+                        "test_team1",
+                        "--organization",
+                        "my_organization",
+                        "add",
+                        "--member",
+                        "user1@org.io",
+                    ]
+                ],
+            ),
+            "overwrite": True,
+        }
+    ]
+
+    file_path = mock_yaml_file(test_data)
+    result = helper.parse_all_yaml([file_path])
+
+    assert "teams" in result
+    assert result["teams"] == expected_block_output
+
+
+def test_create_mock_members_yaml(mock_yaml_file):
+    test_data = {"members": [{"user": "bob@myorg.io", "organization": "myorg"}]}
+    expected_block_output = [
+        {
+            "cmd_args": [
+                "--organization",
+                "myorg",
+                "--user",
+                "bob@myorg.io",
+            ],
+            "overwrite": False,
+        }
+    ]
+    file_path = mock_yaml_file(test_data)
+    result = helper.parse_all_yaml([file_path])
+
+    assert "members" in result
+    assert result["members"] == expected_block_output
+
+
 def test_empty_yaml_file(mock_yaml_file):
     test_data = {}
     file_path = mock_yaml_file(test_data)
 
     with pytest.raises(ValueError) as e:
         helper.parse_all_yaml([file_path])
     assert f"The file '{file_path}' is empty or does not contain valid data." in str(
         e.value
     )
 
 
+def test_empty_stdin_file():
+    # Prepare the mock to simulate empty stdin
+    with patch("sys.stdin", StringIO("")):
+        # Use '-' to indicate that stdin should be read
+        with pytest.raises(ValueError) as e:
+            helper.parse_all_yaml(["-"])
+        assert (
+            "The input from stdin is empty or does not contain valid YAML data."
+            in str(e.value)
+        )
+
+
+def test_stdin_yaml_file():
+    # Prepare the mock to simulate stdin
+    yaml_data = """
+compute-envs:
+  - name: test_computeenv
+    config-mode: forge
+    workspace: my_organization/my_workspace
+    credentials: my_credentials
+    type: aws-batch
+    wait: AVAILABLE
+        """
+    with patch("sys.stdin", StringIO(yaml_data)):
+        result = helper.parse_all_yaml(["-"])
+
+    expected_block_output = [
+        {
+            "cmd_args": [
+                "aws-batch",
+                "forge",
+                "--name",
+                "test_computeenv",
+                "--workspace",
+                "my_organization/my_workspace",
+                "--credentials",
+                "my_credentials",
+                "--wait",
+                "AVAILABLE",
+            ],
+            "overwrite": False,
+        }
+    ]
+    assert "compute-envs" in result
+    assert result["compute-envs"] == expected_block_output
+
+
 def test_error_type_yaml_file(mock_yaml_file):
     test_data = {
         "compute-envs": [
             {
                 "name": "test_computeenv",
                 "workspace": "my_organization/my_workspace",
                 "credentials": "my_credentials",
@@ -292,7 +406,39 @@
 
     with pytest.raises(ValueError) as e:
         helper.parse_all_yaml([file_path])
     assert (
         "Please specify at least 'type' or 'file-path' for creating the resource."
         in str(e.value)
     )
+
+
+def test_error_duplicate_name_yaml_file(mock_yaml_file):
+    test_data = {
+        "compute-envs": [
+            {
+                "name": "test_computeenv",
+                "workspace": "my_organization/my_workspace",
+                "credentials": "my_credentials",
+                "type": "aws-batch",
+                "config-mode": "forge",
+                "wait": "AVAILABLE",
+            },
+            {
+                "name": "test_computeenv",
+                "workspace": "my_organization/my_workspace",
+                "credentials": "my_credentials",
+                "type": "aws-batch",
+                "config-mode": "forge",
+                "wait": "AVAILABLE",
+            },
+        ],
+    }
+    file_path = mock_yaml_file(test_data)
+
+    with pytest.raises(ValueError) as e:
+        helper.parse_all_yaml([file_path])
+    assert (
+        "Duplicate name key specified in config file for "
+        "compute-envs: test_computeenv. Please specify "
+        "a unique value." in str(e.value)
+    )
```

### Comparing `seqerakit-0.4.6/tests/unit/test_seqeraplatform.py` & `seqerakit-0.4.7/tests/unit/test_seqeraplatform.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from unittest.mock import patch
+from unittest.mock import MagicMock, patch
 from seqerakit import seqeraplatform
 import json
 import subprocess
 import os
 
 
 class TestSeqeraPlatform(unittest.TestCase):
@@ -22,14 +22,15 @@
             "paramsText": "",
             "resume": "false",
             "pullLatest": "false",
             "stubRun": "false",
             "dateCreated": "2023-02-15T13:14:30Z",
         }
         # Mock the stdout of the Popen process
+        mock_subprocess.return_value = MagicMock(returncode=0)
         mock_subprocess.return_value.communicate.return_value = (
             json.dumps(mock_pipelines_json).encode(),
             b"",
         )
 
         # Dynamically get the pipelines command
         command = getattr(self.sp, "pipelines")
@@ -89,14 +90,15 @@
             # Check that the error is raised
             with self.assertRaises(seqeraplatform.ResourceCreationError):
                 command("import", "my_pipeline.json", "--name", "pipeline_name")
 
     def test_json_parsing(self):
         with patch("subprocess.Popen") as mock_subprocess:
             # Mock the stdout of the Popen process to return JSON
+            mock_subprocess.return_value = MagicMock(returncode=0)
             mock_subprocess.return_value.communicate.return_value = (
                 b'{"key": "value"}',
                 b"",
             )
 
             command = getattr(self.sp, "pipelines")
 
@@ -108,14 +110,15 @@
     def setUp(self):
         self.cli_args = ["--url", "http://tower-api.com", "--insecure"]
         self.sp = seqeraplatform.SeqeraPlatform(cli_args=self.cli_args)
 
     @patch("subprocess.Popen")
     def test_cli_args_inclusion(self, mock_subprocess):
         # Mock the stdout of the Popen process
+        mock_subprocess.return_value = MagicMock(returncode=0)
         mock_subprocess.return_value.communicate.return_value = (
             json.dumps({"key": "value"}).encode(),
             b"",
         )
 
         # Call a method
         self.sp.pipelines("view", "--name", "pipeline_name", to_json=True)
@@ -132,14 +135,15 @@
         # Add path to custom certs store to cli_args
         self.cli_args.append("-Djavax.net.ssl.trustStore=/absolute/path/to/cacerts")
 
         # Initialize SeqeraPlatform with cli_args
         seqeraplatform.SeqeraPlatform(cli_args=self.cli_args)
 
         # Mock the stdout of the Popen process
+        mock_subprocess.return_value = MagicMock(returncode=0)
         mock_subprocess.return_value.communicate.return_value = (
             json.dumps({"key": "value"}).encode(),
             b"",
         )
 
         # Call a method
         self.sp.pipelines("view", "--name", "pipeline_name", to_json=True)
```

### Comparing `seqerakit-0.4.6/tests/unit/test_subcommands.py` & `seqerakit-0.4.7/tests/unit/test_subcommands.py`

 * *Files identical despite different names*

