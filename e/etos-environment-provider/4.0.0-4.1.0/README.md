# Comparing `tmp/etos_environment_provider-4.0.0.tar.gz` & `tmp/etos_environment_provider-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etos_environment_provider-4.0.0.tar", last modified: Thu Mar 28 07:12:42 2024, max compression
+gzip compressed data, was "etos_environment_provider-4.1.0.tar", last modified: Fri Apr 26 08:02:35 2024, max compression
```

## Comparing `etos_environment_provider-4.0.0.tar` & `etos_environment_provider-4.1.0.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.014511 etos_environment_provider-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:41.990511 etos_environment_provider-4.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:41.998511 etos_environment_provider-4.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/.github/workflows/build-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-03-28 07:12:42.014511 etos_environment_provider-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:41.998511 etos_environment_provider-4.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:41.998511 etos_environment_provider-4.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:41.994511 etos_environment_provider-4.0.0/manifests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:41.998511 etos_environment_provider-4.0.0/manifests/base/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:41.998511 etos_environment_provider-4.0.0/manifests/base/api/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/manifests/base/api/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/manifests/base/api/service-account.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/manifests/base/api/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/manifests/base/kustomization.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:41.998511 etos_environment_provider-4.0.0/manifests/base/worker/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/manifests/base/worker/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/manifests/base/worker/service-account.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-28 07:12:42.014511 etos_environment_provider-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:41.994511 etos_environment_provider-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.002511 etos_environment_provider-4.0.0/src/environment_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    22823 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/environment_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.002511 etos_environment_provider-4.0.0/src/environment_provider/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/encrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/join.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/json_dumps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/log_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/uuid_generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.002511 etos_environment_provider-4.0.0/src/environment_provider/splitter/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/splitter/split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.014511 etos_environment_provider-4.0.0/src/etos_environment_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-03-28 07:12:41.000000 etos_environment_provider-4.0.0/src/etos_environment_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-03-28 07:12:41.000000 etos_environment_provider-4.0.0/src/etos_environment_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 07:12:41.000000 etos_environment_provider-4.0.0/src/etos_environment_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 07:12:41.000000 etos_environment_provider-4.0.0/src/etos_environment_provider.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-28 07:12:41.000000 etos_environment_provider-4.0.0/src/etos_environment_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-28 07:12:41.000000 etos_environment_provider-4.0.0/src/etos_environment_provider.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.006511 etos_environment_provider-4.0.0/src/execution_space_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/execution_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/execution_space_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.006511 etos_environment_provider-4.0.0/src/execution_space_provider/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/schemas/external_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/schemas/jsontas_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.006511 etos_environment_provider-4.0.0/src/execution_space_provider/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/utilities/checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/utilities/checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    14757 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/utilities/external_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/utilities/instructions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/utilities/jsontas_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/utilities/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.006511 etos_environment_provider-4.0.0/src/iut_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/iut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/iut_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.006511 etos_environment_provider-4.0.0/src/iut_provider/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/schemas/external_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/schemas/jsontas_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.006511 etos_environment_provider-4.0.0/src/iut_provider/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/utilities/checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/utilities/checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    12054 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/utilities/external_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/utilities/jsontas_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/utilities/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/utilities/prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.010511 etos_environment_provider-4.0.0/src/log_area_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/log_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/log_area_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.010511 etos_environment_provider-4.0.0/src/log_area_provider/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/schemas/external_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/schemas/jsontas_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.010511 etos_environment_provider-4.0.0/src/log_area_provider/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/utilities/checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/utilities/checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/utilities/external_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/utilities/jsontas_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/utilities/list.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.010511 etos_environment_provider-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.010511 etos_environment_provider-4.0.0/tests/external_execution_space/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/external_execution_space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25624 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/external_execution_space/test_external_execution_space.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.010511 etos_environment_provider-4.0.0/tests/external_iut/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/external_iut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24107 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/external_iut/test_external_iut.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.010511 etos_environment_provider-4.0.0/tests/external_log_area/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/external_log_area/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24737 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/external_log_area/test_external_log_area.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.010511 etos_environment_provider-4.0.0/tests/library/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/library/fake_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/library/fake_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/library/graphql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.010511 etos_environment_provider-4.0.0/tests/splitter/
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/splitter/test_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7967 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/tercc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/test_environment_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.482992 etos_environment_provider-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.458991 etos_environment_provider-4.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.462991 etos_environment_provider-4.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/.github/workflows/build-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-26 08:02:35.482992 etos_environment_provider-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.462991 etos_environment_provider-4.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.466992 etos_environment_provider-4.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.458991 etos_environment_provider-4.1.0/manifests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.466992 etos_environment_provider-4.1.0/manifests/base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.466992 etos_environment_provider-4.1.0/manifests/base/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/manifests/base/api/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/manifests/base/api/service-account.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/manifests/base/api/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/manifests/base/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.466992 etos_environment_provider-4.1.0/manifests/base/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/manifests/base/worker/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/manifests/base/worker/service-account.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-26 08:02:35.482992 etos_environment_provider-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.458991 etos_environment_provider-4.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.466992 etos_environment_provider-4.1.0/src/environment_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22823 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/environment_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.466992 etos_environment_provider-4.1.0/src/environment_provider/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/json_dumps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/log_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/uuid_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.470991 etos_environment_provider-4.1.0/src/environment_provider/splitter/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/splitter/split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.482992 etos_environment_provider-4.1.0/src/etos_environment_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-26 08:02:35.000000 etos_environment_provider-4.1.0/src/etos_environment_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-26 08:02:35.000000 etos_environment_provider-4.1.0/src/etos_environment_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:02:35.000000 etos_environment_provider-4.1.0/src/etos_environment_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:02:35.000000 etos_environment_provider-4.1.0/src/etos_environment_provider.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-26 08:02:35.000000 etos_environment_provider-4.1.0/src/etos_environment_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-26 08:02:35.000000 etos_environment_provider-4.1.0/src/etos_environment_provider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.470991 etos_environment_provider-4.1.0/src/execution_space_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/execution_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/execution_space_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.470991 etos_environment_provider-4.1.0/src/execution_space_provider/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/schemas/external_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/schemas/jsontas_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.470991 etos_environment_provider-4.1.0/src/execution_space_provider/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/utilities/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/utilities/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15049 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/utilities/external_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/utilities/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/utilities/jsontas_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/utilities/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.474991 etos_environment_provider-4.1.0/src/iut_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/iut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/iut_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.474991 etos_environment_provider-4.1.0/src/iut_provider/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/schemas/external_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/schemas/jsontas_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.474991 etos_environment_provider-4.1.0/src/iut_provider/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/utilities/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/utilities/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12346 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/utilities/external_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/utilities/jsontas_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/utilities/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/utilities/prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.474991 etos_environment_provider-4.1.0/src/log_area_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/log_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/log_area_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.474991 etos_environment_provider-4.1.0/src/log_area_provider/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/schemas/external_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/schemas/jsontas_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.478991 etos_environment_provider-4.1.0/src/log_area_provider/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/utilities/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/utilities/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/utilities/external_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/utilities/jsontas_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/utilities/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.478991 etos_environment_provider-4.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.478991 etos_environment_provider-4.1.0/tests/external_execution_space/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/external_execution_space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25624 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/external_execution_space/test_external_execution_space.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.482992 etos_environment_provider-4.1.0/tests/external_iut/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/external_iut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24107 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/external_iut/test_external_iut.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.482992 etos_environment_provider-4.1.0/tests/external_log_area/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/external_log_area/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24737 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/external_log_area/test_external_log_area.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.482992 etos_environment_provider-4.1.0/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/library/fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/library/fake_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/library/graphql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.482992 etos_environment_provider-4.1.0/tests/splitter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/splitter/test_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7967 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/tercc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/test_environment_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tox.ini
```

### Comparing `etos_environment_provider-4.0.0/.coveragerc` & `etos_environment_provider-4.1.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/.github/workflows/build-push.yml` & `etos_environment_provider-4.1.0/.github/workflows/build-push.yml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/.github/workflows/main.yml` & `etos_environment_provider-4.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/.gitignore` & `etos_environment_provider-4.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/LICENSE.txt` & `etos_environment_provider-4.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/PKG-INFO` & `etos_environment_provider-4.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos_environment_provider
-Version: 4.0.0
+Version: 4.1.0
 Summary: Environment provider for ETOS.
 Home-page: https://github.com/eiffel-community/etos-environment-provider
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
```

### Comparing `etos_environment_provider-4.0.0/README.rst` & `etos_environment_provider-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/docs/Makefile` & `etos_environment_provider-4.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/docs/conf.py` & `etos_environment_provider-4.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/manifests/base/api/deployment.yaml` & `etos_environment_provider-4.1.0/manifests/base/api/deployment.yaml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/manifests/base/kustomization.yaml` & `etos_environment_provider-4.1.0/manifests/base/kustomization.yaml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/manifests/base/worker/deployment.yaml` & `etos_environment_provider-4.1.0/manifests/base/worker/deployment.yaml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/requirements.txt` & `etos_environment_provider-4.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/setup.cfg` & `etos_environment_provider-4.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/setup.py` & `etos_environment_provider-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/environment_provider/__init__.py` & `etos_environment_provider-4.1.0/src/environment_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/environment_provider/environment.py` & `etos_environment_provider-4.1.0/src/environment_provider/environment.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/environment_provider/environment_provider.py` & `etos_environment_provider-4.1.0/src/environment_provider/environment_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/environment_provider/lib/__init__.py` & `etos_environment_provider-4.1.0/src/environment_provider/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/environment_provider/lib/celery.py` & `etos_environment_provider-4.1.0/src/environment_provider/lib/celery.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/environment_provider/lib/config.py` & `etos_environment_provider-4.1.0/src/environment_provider/lib/config.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/environment_provider/lib/database.py` & `etos_environment_provider-4.1.0/src/environment_provider/lib/database.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/environment_provider/lib/encrypt.py` & `etos_environment_provider-4.1.0/src/environment_provider/lib/encrypt.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/environment_provider/lib/graphql.py` & `etos_environment_provider-4.1.0/src/environment_provider/lib/graphql.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/environment_provider/lib/join.py` & `etos_environment_provider-4.1.0/src/environment_provider/lib/join.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/environment_provider/lib/json_dumps.py` & `etos_environment_provider-4.1.0/src/environment_provider/lib/json_dumps.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/environment_provider/lib/log_area.py` & `etos_environment_provider-4.1.0/src/environment_provider/lib/log_area.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/environment_provider/lib/registry.py` & `etos_environment_provider-4.1.0/src/environment_provider/lib/registry.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/environment_provider/lib/test_suite.py` & `etos_environment_provider-4.1.0/src/environment_provider/lib/test_suite.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/environment_provider/lib/uuid_generate.py` & `etos_environment_provider-4.1.0/src/environment_provider/lib/uuid_generate.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/environment_provider/splitter/__init__.py` & `etos_environment_provider-4.1.0/src/environment_provider/splitter/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/environment_provider/splitter/split.py` & `etos_environment_provider-4.1.0/src/environment_provider/splitter/split.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/etos_environment_provider.egg-info/PKG-INFO` & `etos_environment_provider-4.1.0/src/etos_environment_provider.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos_environment_provider
-Version: 4.0.0
+Version: 4.1.0
 Summary: Environment provider for ETOS.
 Home-page: https://github.com/eiffel-community/etos-environment-provider
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
```

### Comparing `etos_environment_provider-4.0.0/src/etos_environment_provider.egg-info/SOURCES.txt` & `etos_environment_provider-4.1.0/src/etos_environment_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/execution_space_provider/__init__.py` & `etos_environment_provider-4.1.0/src/execution_space_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/execution_space_provider/exceptions.py` & `etos_environment_provider-4.1.0/src/execution_space_provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/execution_space_provider/execution_space.py` & `etos_environment_provider-4.1.0/src/execution_space_provider/execution_space.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/execution_space_provider/execution_space_provider.py` & `etos_environment_provider-4.1.0/src/execution_space_provider/execution_space_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/execution_space_provider/schemas/external_schema.json` & `etos_environment_provider-4.1.0/src/execution_space_provider/schemas/external_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/execution_space_provider/schemas/jsontas_schema.json` & `etos_environment_provider-4.1.0/src/execution_space_provider/schemas/jsontas_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/execution_space_provider/utilities/__init__.py` & `etos_environment_provider-4.1.0/src/execution_space_provider/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/execution_space_provider/utilities/checkin.py` & `etos_environment_provider-4.1.0/src/execution_space_provider/utilities/checkin.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/execution_space_provider/utilities/checkout.py` & `etos_environment_provider-4.1.0/src/execution_space_provider/utilities/checkout.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/execution_space_provider/utilities/external_provider.py` & `etos_environment_provider-4.1.0/src/execution_space_provider/utilities/external_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from json.decoder import JSONDecodeError
 
 import requests
 from etos_lib import ETOS
 from etos_lib.lib.http import Http
 from jsontas.jsontas import JsonTas
 from packageurl import PackageURL
-from requests.exceptions import HTTPError
+from requests.exceptions import HTTPError, ConnectionError as RequestsConnectionError
 from urllib3.util import Retry
 
 from environment_provider.lib.encrypt import encrypt
 
 from ..exceptions import (
     ExecutionSpaceCheckinFailed,
     ExecutionSpaceCheckoutFailed,
@@ -128,14 +128,19 @@
                 if response.status_code == requests.codes["no_content"]:
                     return
                 response = response.json()
                 if response.get("error") is not None:
                     raise ExecutionSpaceCheckinFailed(
                         f"Unable to check in {execution_spaces} " f"({response.get('error')})"
                     )
+            except RequestsConnectionError as error:
+                if "connection refused" in str(error).lower():
+                    self.logger.error("Error connecting to %r: %r", host, error)
+                    continue
+                raise
             except ConnectionError:
                 self.logger.error("Error connecting to %r", host)
                 continue
         raise TimeoutError(f"Unable to stop external provider {self.id!r}")
 
     def checkin_all(self) -> None:
         """Check in all execution spaces.
```

### Comparing `etos_environment_provider-4.0.0/src/execution_space_provider/utilities/instructions.py` & `etos_environment_provider-4.1.0/src/execution_space_provider/utilities/instructions.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/execution_space_provider/utilities/jsontas_provider.py` & `etos_environment_provider-4.1.0/src/execution_space_provider/utilities/jsontas_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/execution_space_provider/utilities/list.py` & `etos_environment_provider-4.1.0/src/execution_space_provider/utilities/list.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/iut_provider/__init__.py` & `etos_environment_provider-4.1.0/src/iut_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/iut_provider/exceptions.py` & `etos_environment_provider-4.1.0/src/iut_provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/iut_provider/iut.py` & `etos_environment_provider-4.1.0/src/iut_provider/iut.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/iut_provider/iut_provider.py` & `etos_environment_provider-4.1.0/src/iut_provider/iut_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/iut_provider/schemas/external_schema.json` & `etos_environment_provider-4.1.0/src/iut_provider/schemas/external_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/iut_provider/schemas/jsontas_schema.json` & `etos_environment_provider-4.1.0/src/iut_provider/schemas/jsontas_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/iut_provider/utilities/__init__.py` & `etos_environment_provider-4.1.0/src/iut_provider/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/iut_provider/utilities/checkin.py` & `etos_environment_provider-4.1.0/src/iut_provider/utilities/checkin.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/iut_provider/utilities/checkout.py` & `etos_environment_provider-4.1.0/src/iut_provider/utilities/checkout.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/iut_provider/utilities/external_provider.py` & `etos_environment_provider-4.1.0/src/iut_provider/utilities/external_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from json.decoder import JSONDecodeError
 
 import requests
 from etos_lib import ETOS
 from etos_lib.lib.http import Http
 from jsontas.jsontas import JsonTas
 from packageurl import PackageURL
-from requests.exceptions import HTTPError
+from requests.exceptions import HTTPError, ConnectionError as RequestsConnectionError
 from urllib3.util import Retry
 
 from ..exceptions import IutCheckinFailed, IutCheckoutFailed, IutNotAvailable
 from ..iut import Iut
 
 
 class ExternalProvider:
@@ -118,14 +118,19 @@
             try:
                 response = requests.post(host, json=iuts, headers={"X-ETOS-ID": self.identifier})
                 if response.status_code == requests.codes["no_content"]:
                     return
                 response = response.json()
                 if response.get("error") is not None:
                     raise IutCheckinFailed(f"Unable to check in {iuts} ({response.get('error')})")
+            except RequestsConnectionError as error:
+                if "connection refused" in str(error).lower():
+                    self.logger.error("Error connecting to %r: %r", host, error)
+                    continue
+                raise
             except ConnectionError:
                 self.logger.error("Error connecting to %r", host)
                 continue
         raise TimeoutError(f"Unable to stop external provider {self.id!r}")
 
     def checkin_all(self) -> None:
         """Check in all IUTs.
```

### Comparing `etos_environment_provider-4.0.0/src/iut_provider/utilities/jsontas_provider.py` & `etos_environment_provider-4.1.0/src/iut_provider/utilities/jsontas_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/iut_provider/utilities/list.py` & `etos_environment_provider-4.1.0/src/iut_provider/utilities/list.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/iut_provider/utilities/prepare.py` & `etos_environment_provider-4.1.0/src/iut_provider/utilities/prepare.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/log_area_provider/__init__.py` & `etos_environment_provider-4.1.0/src/log_area_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/log_area_provider/exceptions.py` & `etos_environment_provider-4.1.0/src/log_area_provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/log_area_provider/log_area.py` & `etos_environment_provider-4.1.0/src/log_area_provider/log_area.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/log_area_provider/log_area_provider.py` & `etos_environment_provider-4.1.0/src/log_area_provider/log_area_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/log_area_provider/schemas/external_schema.json` & `etos_environment_provider-4.1.0/src/log_area_provider/schemas/external_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/log_area_provider/schemas/jsontas_schema.json` & `etos_environment_provider-4.1.0/src/log_area_provider/schemas/jsontas_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/log_area_provider/utilities/__init__.py` & `etos_environment_provider-4.1.0/src/log_area_provider/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/log_area_provider/utilities/checkin.py` & `etos_environment_provider-4.1.0/src/log_area_provider/utilities/checkin.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/log_area_provider/utilities/checkout.py` & `etos_environment_provider-4.1.0/src/log_area_provider/utilities/checkout.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/log_area_provider/utilities/external_provider.py` & `etos_environment_provider-4.1.0/src/log_area_provider/utilities/external_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from json.decoder import JSONDecodeError
 
 import requests
 from etos_lib import ETOS
 from etos_lib.lib.http import Http
 from jsontas.jsontas import JsonTas
 from packageurl import PackageURL
-from requests.exceptions import HTTPError
+from requests.exceptions import HTTPError, ConnectionError as RequestsConnectionError
 from urllib3.util import Retry
 
 from ..exceptions import LogAreaCheckinFailed, LogAreaCheckoutFailed, LogAreaNotAvailable
 from ..log_area import LogArea
 
 
 class ExternalProvider:
@@ -122,14 +122,19 @@
                 if response.status_code == requests.codes["no_content"]:
                     return
                 response = response.json()
                 if response.get("error") is not None:
                     raise LogAreaCheckinFailed(
                         f"Unable to check in {log_areas} ({response.get('error')})"
                     )
+            except RequestsConnectionError as error:
+                if "connection refused" in str(error).lower():
+                    self.logger.error("Error connecting to %r: %r", host, error)
+                    continue
+                raise
             except ConnectionError:
                 self.logger.error("Error connecting to %r", host)
                 continue
         raise TimeoutError(f"Unable to stop external provider {self.id!r}")
 
     def checkin_all(self) -> None:
         """Check in all log areas.
```

### Comparing `etos_environment_provider-4.0.0/src/log_area_provider/utilities/jsontas_provider.py` & `etos_environment_provider-4.1.0/src/log_area_provider/utilities/jsontas_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/src/log_area_provider/utilities/list.py` & `etos_environment_provider-4.1.0/src/log_area_provider/utilities/list.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/tests/__init__.py` & `etos_environment_provider-4.1.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/tests/external_execution_space/__init__.py` & `etos_environment_provider-4.1.0/tests/external_execution_space/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/tests/external_execution_space/test_external_execution_space.py` & `etos_environment_provider-4.1.0/tests/external_execution_space/test_external_execution_space.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/tests/external_iut/__init__.py` & `etos_environment_provider-4.1.0/tests/external_iut/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/tests/external_iut/test_external_iut.py` & `etos_environment_provider-4.1.0/tests/external_iut/test_external_iut.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/tests/external_log_area/__init__.py` & `etos_environment_provider-4.1.0/tests/external_log_area/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/tests/external_log_area/test_external_log_area.py` & `etos_environment_provider-4.1.0/tests/external_log_area/test_external_log_area.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/tests/library/__init__.py` & `etos_environment_provider-4.1.0/tests/library/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/tests/library/fake_database.py` & `etos_environment_provider-4.1.0/tests/library/fake_database.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/tests/library/fake_server.py` & `etos_environment_provider-4.1.0/tests/library/fake_server.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/tests/library/graphql_handler.py` & `etos_environment_provider-4.1.0/tests/library/graphql_handler.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/tests/splitter/test_splitter.py` & `etos_environment_provider-4.1.0/tests/splitter/test_splitter.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/tests/tercc.py` & `etos_environment_provider-4.1.0/tests/tercc.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/tests/test_environment_provider.py` & `etos_environment_provider-4.1.0/tests/test_environment_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.0.0/tox.ini` & `etos_environment_provider-4.1.0/tox.ini`

 * *Files identical despite different names*

