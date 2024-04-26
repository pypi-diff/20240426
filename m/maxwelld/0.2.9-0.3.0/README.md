# Comparing `tmp/maxwelld-0.2.9.tar.gz` & `tmp/maxwelld-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxwelld-0.2.9.tar", last modified: Sat Mar  9 07:58:42 2024, max compression
+gzip compressed data, was "maxwelld-0.3.0.tar", last modified: Fri Apr 26 03:40:43 2024, max compression
```

## Comparing `maxwelld-0.2.9.tar` & `maxwelld-0.3.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.526072 maxwelld-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-03-09 07:58:32.000000 maxwelld-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-03-09 07:58:42.526072 maxwelld-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-09 07:58:32.000000 maxwelld-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.518072 maxwelld-0.2.9/maxwelld/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.518072 maxwelld-0.2.9/maxwelld/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/client/maxwell_client.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/client/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.522072 maxwelld-0.2.9/maxwelld/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/core/compose_data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/core/compose_files_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/core/compose_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/core/compose_run_sequences.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/core/sequence_run_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/core/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.522072 maxwelld-0.2.9/maxwelld/env_description/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/env_description/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/env_description/env_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/env_description/env_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.522072 maxwelld-0.2.9/maxwelld/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/helpers/bytes_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/helpers/countdown_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/helpers/state_keeper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.522072 maxwelld-0.2.9/maxwelld/output/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/output/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/output/styles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.522072 maxwelld-0.2.9/maxwelld/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/server/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.522072 maxwelld-0.2.9/maxwelld/server/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/server/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/server/handlers/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/server/handlers/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/server/handlers/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/server/handlers/up.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/server/maxwelld_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.526072 maxwelld-0.2.9/maxwelld/vedro_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/vedro_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/vedro_plugin/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10726 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/vedro_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/vedro_plugin/scenario_ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/vedro_plugin/scenario_tag_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/vedro_plugin/state_waiting.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/version
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.526072 maxwelld-0.2.9/maxwelld.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-03-09 07:58:42.000000 maxwelld-0.2.9/maxwelld.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-03-09 07:58:42.000000 maxwelld-0.2.9/maxwelld.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 07:58:42.000000 maxwelld-0.2.9/maxwelld.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-09 07:58:42.000000 maxwelld-0.2.9/maxwelld.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-09 07:58:42.000000 maxwelld-0.2.9/maxwelld.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 07:58:42.526072 maxwelld-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-09 07:58:32.000000 maxwelld-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:40:43.783270 maxwelld-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-26 03:40:35.000000 maxwelld-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-26 03:40:43.783270 maxwelld-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-26 03:40:35.000000 maxwelld-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:40:43.775270 maxwelld-0.3.0/maxwelld/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:40:43.775270 maxwelld-0.3.0/maxwelld/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/client/maxwell_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/client/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:40:43.775270 maxwelld-0.3.0/maxwelld/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/core/compose_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/core/compose_files_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/core/compose_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/core/compose_run_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/core/sequence_run_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/core/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:40:43.779270 maxwelld-0.3.0/maxwelld/env_description/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/env_description/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/env_description/env_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/env_description/env_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:40:43.779270 maxwelld-0.3.0/maxwelld/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/helpers/bytes_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/helpers/countdown_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/helpers/state_keeper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:40:43.779270 maxwelld-0.3.0/maxwelld/output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/output/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/output/styles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:40:43.779270 maxwelld-0.3.0/maxwelld/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/server/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:40:43.779270 maxwelld-0.3.0/maxwelld/server/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/server/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/server/handlers/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/server/handlers/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/server/handlers/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/server/handlers/up.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/server/maxwelld_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:40:43.779270 maxwelld-0.3.0/maxwelld/vedro_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/vedro_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/vedro_plugin/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/vedro_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/vedro_plugin/scenario_ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/vedro_plugin/scenario_tag_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/vedro_plugin/state_waiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/version
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-26 03:40:35.000000 maxwelld-0.3.0/maxwelld/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:40:43.783270 maxwelld-0.3.0/maxwelld.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-26 03:40:43.000000 maxwelld-0.3.0/maxwelld.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-26 03:40:43.000000 maxwelld-0.3.0/maxwelld.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 03:40:43.000000 maxwelld-0.3.0/maxwelld.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-26 03:40:43.000000 maxwelld-0.3.0/maxwelld.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 03:40:43.000000 maxwelld-0.3.0/maxwelld.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 03:40:43.783270 maxwelld-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-26 03:40:35.000000 maxwelld-0.3.0/setup.py
```

### Comparing `maxwelld-0.2.9/LICENSE` & `maxwelld-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.9/PKG-INFO` & `maxwelld-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxwelld
-Version: 0.2.9
+Version: 0.3.0
 Summary: docker compose testing env orchestrator
 Home-page: https://github.com/ko10ok/maxwelld
 Author: Yuriy Sagitov
 Author-email: pro100.ko10ok@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -19,52 +19,73 @@
 Requires-Dist: PyYAML<6.1,>=6.0.1
 Requires-Dist: rtry<2.0,>=1.4.0
 Requires-Dist: rich<16.0,>=11.0
 Requires-Dist: aiohttp<3.10,>=3.9.3
 
 # Maxwell's demon of test enviroment
 
-Orchestrate testing env easily
+Orchestrate testing env easily.
 
-# Install & activate
-## Install package
-```shell
-$ pip3 install maxwelld
+Wraps docker-compose and it's dependencies into it's own container with http api.
+
+Execute docker-compose commands sequences for starting requested services set from volumed docker-compose files.
+Rerun environment when in-flight one is different from new requested.
+
+# Vedro usage
+## Add "supervisor" container
+```docker-compose
+  maxwelld:
+    image: docker.io/ko10ok/maxwelld:0.2.9
+    volumes:
+      - .:/project
+      - ./docker-composes:/docker-composes
+      - ./env-tmp:/env-tmp
+    environment:
+      - DOCKER_HOST=tcp://dockersock:2375
+      - COMPOSE_PROJECT_NAME=${COMPOSE_PROJECT_NAME}
+      - NON_STOP_CONTAINERS=dockersock,maxwelld,e2e
+      - HOST_PROJECT_ROOT_DIRECTORY=${HOST_PROJECT_ROOT_DIRECTORY}
 ```
 
 ## Define services config
 ```python
+# env_set.py
 from maxwelld import Environments
 from maxwelld import Environment
 from maxwelld import DEFAULT_ENV
+from maxwelld import Service
+
+web = Service('web')
+web_gallery = Service('web-gallery')  # Service names "web-gallery", "mq", etc from docker-compose.yml
+mq = Service('mq')
+db = Service('db')
 
 class Envs(Environments):
     DEFAULT = Environment(
         DEFAULT_ENV,
-        builder, web, web_gallery, wep_ext_app, cli,
+        web, web_gallery,
         db,
-        mq,
-        e2e
+        mq
     )
 ```
 
 ## Enable plugin
 ```python
 from maxwelld import vedro_plugin as vedro_maxwell
 from maxwelld import ComposeConfig
+from env_set import Envs
 
 class Config(vedro.Config):
 
     class Plugins(vedro.Config.Plugins):
         
         class VedroMaxwell(vedro_maxwell.VedroMaxwell):
             enabled = True
             envs = Envs()
             compose_cfgs = {
-                'default': ComposeConfig(os.environ.get('DC_FILES')),
-                'dev': ComposeConfig(os.environ.get(f'DC_FILES_1'), parallel_env_limit=1),
+                'default': ComposeConfig('docker-compose.yml', parallel_env_limit=1),
+                'dev': ComposeConfig('docker-compose.yml:docker-compose.dev.yml', parallel_env_limit=1),
             }
-            project = os.environ.get('COMPOSE_PROJECT_NAME', default='some_project')
 ```
 
-## Architecture design draft
-![Architecture design draft](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/ko10ok/maxwelld/server_split_prototype/ARCH.puml)
+## Architecture design
+![Architecture design](https://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/ko10ok/maxwelld/server_split_prototype/ARCH.puml)
```

### Comparing `maxwelld-0.2.9/maxwelld/__init__.py` & `maxwelld-0.3.0/maxwelld/__init__.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.9/maxwelld/client/maxwell_client.py` & `maxwelld-0.3.0/maxwelld/client/maxwell_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,15 @@
 from maxwelld.server.handlers.env import EnvResponseParams
 from maxwelld.server.handlers.status import StatusResponseParams
 from maxwelld.server.handlers.up import UpRequestParams
 from maxwelld.server.handlers.up import UpResponseParams
 
 
 class MaxwellDemonClient:
-    def __init__(self, host, project, non_stop_containers, port=80):
-        self._project = project
-        self._non_stop_containers = non_stop_containers
+    def __init__(self, host, port=80):
         self._server_host = host
         self._server_port = port
         self._server_url = f'{self._server_host}:{self._server_port}'
 
     async def healthcheck(self):
         async with aiohttp.ClientSession() as session:
             url = f'{self._server_url}{HEALTHCHECK_PATH}'
@@ -33,29 +31,28 @@
                 assert response.status == 200, response
                 state = await response.json()
                 assert 'status' in state, response
                 assert state['status'] == 'ok', response
 
     @retry(attempts=10, delay=1, swallow=ClientConnectorError)
     async def up(self, name, config_template: Environment, compose_files: str, isolation=None,
-                 parallelism_limit=None, force_restart: bool = False) -> tuple[EnvironmentId, bool]:
+                 parallelism_limit=None, force_restart: bool = False) -> EnvironmentId:
         url = f'{self._server_url}{UP_PATH}'
         async with aiohttp.ClientSession() as session:
             async with session.post(url, json=UpRequestParams(
                 name=name,
                 config_template=base64_pickled(config_template),
                 compose_files=compose_files,
                 isolation=isolation,
                 parallelism_limit=parallelism_limit,
-                non_stop_containers=self._non_stop_containers,
                 force_restart=force_restart,
             )) as response:
                 assert response.status == 200, response
                 response_body = UpResponseParams(**await response.json())
-                return response_body['env_id'], response_body['new']
+                return response_body['env_id']
 
     @retry(attempts=5, delay=1, swallow=Exception)
     async def env(self, env_id: EnvironmentId) -> Environment:
         url = f'{self._server_url}{ENV_PATH}'
         async with aiohttp.ClientSession() as session:
             async with session.get(url, json=EnvRequestParams(id=env_id)) as response:
                 assert response.status == 200, response
```

### Comparing `maxwelld-0.2.9/maxwelld/core/compose_data_types.py` & `maxwelld-0.3.0/maxwelld/core/compose_data_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         ))
         service_string.append(Text(
             self.status, style=style.regular
         ))
         service_string.append(Text('\n', style=style.regular))
         return service_string
 
-    def as_json(self):
+    def as_json(self) -> dict[str, str]:
         return {
             'name': self.name,
             'state': self.state,
             'health': self.health,
             'status': self.status,
         }
```

### Comparing `maxwelld-0.2.9/maxwelld/core/compose_files_utils.py` & `maxwelld-0.3.0/maxwelld/core/compose_files_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                 dc_cfg['services'][service]['volumes'],
                 root_path
             )
             new_dc_cfg['services'][service]['volumes'] = updated_volumes
     return new_dc_cfg
 
 
-def list_key_exist(key, env: list[str]):
+def list_key_exist(key, env: list[str]) -> None | str:
     for item in env:
         if key in item:
             return item
     else:
         return None
 
 
@@ -130,16 +130,17 @@
                 }
     return new_service_dc_cfg
 
 
 def patch_docker_compose_file_services(filename: Path,
                                        host_root: Path,
                                        services_environment_vars: Environment,
-                                       network_name: str, services_map: dict[
-        str, str]):  # TODO network_name = [projectname]_default
+                                       network_name: str,
+                                       # TODO network_name = [projectname]_default
+                                       services_map: dict[str, str]) -> None:
     dc_cfg = read_dc_file(filename)
 
     dc_cfg = patch_network(dc_cfg, network_name=network_name)
 
     dc_cfg = patch_service_set(dc_cfg, services_map)  # todo use servcie_map
 
     dc_cfg = patch_envs(dc_cfg, services_environment_vars)  # todo use servcie_map
@@ -147,15 +148,15 @@
     dc_cfg = patch_services_names(dc_cfg, services_map)  # todo use servcie_map istead postfix
 
     dc_cfg = patch_services_volumes(dc_cfg, host_root)
 
     write_dc_file(filename, dc_cfg)
 
 
-def parse_migration(migration: dict):
+def parse_migration(migration: dict) -> Handler:
     assert isinstance(migration, dict), f'{migration} should be "stage: command" entry'
     assert len(migration) == 1, f'{migration} should have only one "stage: command" entry'
     assert list(migration.keys())[0] in EventStage.get_all_compose_stages(), f"{migration} stage should only be one of {EventStage.get_all_compose_stages()}"
 
     for stage, command in migration.items():
         if isinstance(command, str):
             return Handler(
@@ -193,24 +194,24 @@
                        '  - stage: { cmd: command, executor: executor_container_name}\n'
                        f'  - stage:\n'
                        f'      cmd: command\n'
                        f'      executor: executor_container_name\n'
                        f'formats')
 
 
-def parse_migrations(migrations: list[dict]):
+def parse_migrations(migrations: list[dict]) -> list[Handler]:
     assert isinstance(migrations, list), (f'{migrations} should be list '
                                           f'of {{stage: [cmd, params]}}')
     result_hooks = []
     for migration in migrations:
         result_hooks += [parse_migration(migration)]
     return result_hooks
 
 
-def extract_services_inline_migration(compose_files: list[str]):
+def extract_services_inline_migration(compose_files: list[str]) -> dict[str, list[str]]:
     migrations = collections.defaultdict(lambda: [])
     for filename in compose_files:
         dc_cfg = read_dc_file(filename)
         if 'services' in dc_cfg:
             for service in dc_cfg['services']:
                 if service not in migrations:
                     migrations[service] = []
```

### Comparing `maxwelld-0.2.9/maxwelld/core/compose_interface.py` & `maxwelld-0.3.0/maxwelld/core/compose_interface.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.9/maxwelld/core/compose_run_sequences.py` & `maxwelld-0.3.0/maxwelld/core/compose_run_sequences.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,17 +108,16 @@
     return services
 
 
 def make_env_compose_instance_files(env_config_instance: EnvConfigInstance,
                                     compose_files: str,
                                     project_network_name: str,  # without "_default"
                                     host_project_root_directory,
-                                    compose_files_path: Path = Path('/compose-files'),
-                                    # dot_env_files_path: Path = Path('/docker-composes/envs'),
-                                    tmp_env_path: Path = Path('/env-tmp'),
+                                    compose_files_path: Path,
+                                    tmp_env_path: Path,
                                     ) -> EnvConfigComposeInstance:
     dst = tmp_env_path / env_config_instance.env_id
     dst.mkdir(parents=True, exist_ok=True)
 
     for file in compose_files.split(':'):
         src_file = compose_files_path / file
         dst_file = dst / file
@@ -159,14 +158,15 @@
         f.write(f'alias deactivate-env="unset COMPOSE_FILE"\n')
         # TODO Envs
         # for k,value in updated_envs.items():
         #     f.write(f'{k}={value}\n')
         # f.write(f'export COMPOSE_PROJECT_NAME={new_project_name}\n')
 
 
+# TODO move into compose_interface.py
 def print_state(execution_envs, in_docker_project_root):
     status = subprocess.call(
         shlex.split(
             "docker-compose --project-directory . ps -a --format='table "
             "{{.Service}}\t{{.ExitCode}}\t{{.Health}}\t{{.Image}}\t{{.State}}\t{{.Status}}'"
         ),
         env=execution_envs,
@@ -208,14 +208,16 @@
                 target_service = dc_env_config.env_config_instance.env_services_map[handler.executor or service]
                 substituted_cmd = handler.cmd % dc_env_config.env_config_instance.env_services_map
 
                 migrate_result = await dc_exec(target_service, substituted_cmd, execution_envs, in_docker_project_root)
                 assert migrate_result == JobResult.GOOD, (f"Can't migrate service {target_service}, "
                                                           f"with {substituted_cmd}")
 
+
+# TODO move into compose_interface.py
 def down_in_flight_envs(tmp_envs_path: Path, env_id, in_docker_project_root, except_containers: list[str]):
     dirpath, dirnames, filenames = next(os.walk(tmp_envs_path / env_id))
     filenames.remove('.env')
     docker_files = get_new_instance_compose_files(':'.join(filenames),
                                                   tmp_envs_path / env_id)
 
     execution_envs = dict(os.environ)
```

### Comparing `maxwelld-0.2.9/maxwelld/core/sequence_run_types.py` & `maxwelld-0.3.0/maxwelld/core/sequence_run_types.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.9/maxwelld/core/service.py` & `maxwelld-0.3.0/maxwelld/core/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,37 +24,39 @@
 from maxwelld.helpers.bytes_pickle import base64_pickled
 from maxwelld.helpers.bytes_pickle import debase64_pickled
 from maxwelld.output.console import CONSOLE
 from maxwelld.output.styles import Style
 
 
 class MaxwellDemonService:
-    def __init__(self, project: str, non_stop_containers: list[str]):
+    def __init__(self):
         assert shutil.which("docker"), 'Docker not installed'
         assert shutil.which("docker-compose"), 'Docker-compose not installed'
-        assert os.environ.get('COMPOSE_FILES_DIRECTORY'), \
-            'COMPOSE_FILES_DIRECTORY env should be set'
-        assert os.environ.get('PROJECT_ROOT_DIRECTORY'), \
-            'PROJECT_ROOT_DIRECTORY env should be set'
+
+        assert os.environ.get('COMPOSE_PROJECT_NAME'), \
+            'COMPOSE_PROJECT_NAME env should be set'
+        assert os.environ.get('NON_STOP_CONTAINERS'), \
+            'NON_STOP_CONTAINERS env should be set'
         assert os.environ.get('HOST_PROJECT_ROOT_DIRECTORY'), \
             'HOST_PROJECT_ROOT_DIRECTORY env should be set'
-        assert os.environ.get('HOST_TMP_ENV_DIRECTORY'), \
-            'HOST_TMP_ENV_DIRECTORY env should be set'
 
-        self._project = project
-        self._non_stop_containers = non_stop_containers
-        self.tmp_envs_path = Path('/env-tmp')  # TODO get from envs
+        # TODO print service paths for *.yml files, project root and etc.
+        self._project = os.environ.get('COMPOSE_PROJECT_NAME')
+        self._non_stop_containers = os.environ.get('NON_STOP_CONTAINERS').split(',')
+        self.tmp_envs_path = Path(os.environ.get('TMP_ENVS_DIRECTORY'))
         self.compose_files_path = Path(os.environ.get('COMPOSE_FILES_DIRECTORY'))
-        # self.dot_env_files_path = Path('/compose-files/envs')
         self.in_docker_project_root_path = Path(os.environ.get('PROJECT_ROOT_DIRECTORY'))
-        self.env_file_name = 'envs.json'
+        self.env_file_name = os.environ.get('TMP_ENVS_REGISTER_FILE')
         self.env_file_path = self.tmp_envs_path / self.env_file_name
         self.host_project_root_directory = Path(os.environ.get('HOST_PROJECT_ROOT_DIRECTORY'))
-        self.host_env_tmp_directory = \
-            self.host_project_root_directory / os.environ.get('HOST_TMP_ENV_DIRECTORY')
+        self.env_tmp_directory = Path(os.environ.get('TMP_ENVS_DIRECTORY'))
+        self.host_env_tmp_directory = Path(os.environ.get(
+                'HOST_TMP_ENV_DIRECTORY',
+                self.host_project_root_directory / self.env_tmp_directory.name
+        ))
         self._started_envs: dict[str, dict] = actualize_in_flight(
             self.tmp_envs_path,
             self.env_file_name
         )
 
     def update_inflight_envs(self, name, config_template: Environment, compose_files: str, env_id: str):
         self._started_envs[name] = {
@@ -124,15 +126,16 @@
     ) -> tuple[EnvironmentId, bool]:
 
         existing_inflight_env = self.get_existing_inflight_env(
             name, config_template, compose_files
         )
         if existing_inflight_env and not force_restart:
             CONSOLE.print(f'Existing env for {name}: {existing_inflight_env.env_id}. Access: '
-                          f'> source ./env-tmp/{existing_inflight_env.env_id}/.env')
+                          f'> cd {self.host_project_root_directory} && '
+                          f'source ./env-tmp/{existing_inflight_env.env_id}/.env')
             return existing_inflight_env.env_id, False
 
         CONSOLE.print(
             Text('Starting new environment: ', style=Style.info)
             .append(Text(name, style=Style.mark))
         )
         new_env_id = get_new_env_id()
@@ -149,33 +152,35 @@
 
         compose_files_instance = make_env_compose_instance_files(
             env_config_instance,
             compose_files,
             project_network_name=self._project,
             host_project_root_directory=self.host_project_root_directory,
             compose_files_path=self.compose_files_path,
-            # dot_env_files_path=self.dot_env_files_path,
             tmp_env_path=self.tmp_envs_path,
         )
 
         make_debug_bash_env(compose_files_instance, self.host_env_tmp_directory)
-        CONSOLE.print(f'Docker-compose access: > source ./env-tmp/{new_env_id}/.env')
+        CONSOLE.print(f'Docker-compose access: > cd {self.host_project_root_directory} && '
+                      f'source ./env-tmp/{new_env_id}/.env')
 
         # TODO uncomment
         in_flight_env = await run_env(
             compose_files_instance, self.in_docker_project_root_path, self._non_stop_containers
         )
 
         # TODO should be transactional with file
         CONSOLE.print(Text(f'New environment for {name} started'))
         if verbose:
             CONSOLE.print(f'Config params: {unpack_services_env_template_params(env_config_instance.env)}')
         CONSOLE.print(
             Text(f'Docker-compose access: > ', style=Style.info)
-            .append(Text(f'source ./env-tmp/{new_env_id}/.env', style=Style.mark_neutral))
+            .append(Text(
+                f'cd {self.host_project_root_directory} && source ./env-tmp/{new_env_id}/.env',
+                style=Style.mark_neutral))
         )
 
         self.update_inflight_envs(
             name,
             config_template=config_template,
             compose_files=compose_files_instance.compose_files,
             env_id=new_env_id,
@@ -199,14 +204,11 @@
 
 
 class MaxwellDemonServiceManager:
     maxwell_demon_service = None
 
     def __init__(self):
         if MaxwellDemonServiceManager.maxwell_demon_service is None:
-            MaxwellDemonServiceManager.maxwell_demon_service = MaxwellDemonService(
-                project=os.environ.get('COMPOSE_PROJECT_NAME'),
-                non_stop_containers=os.environ.get('NON_STOP_CONTAINERS').split(',')
-            )
+            MaxwellDemonServiceManager.maxwell_demon_service = MaxwellDemonService()
 
     def get(self) -> MaxwellDemonService:
         return MaxwellDemonServiceManager.maxwell_demon_service
```

### Comparing `maxwelld-0.2.9/maxwelld/env_description/env_tools.py` & `maxwelld-0.3.0/maxwelld/env_description/env_tools.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.9/maxwelld/env_description/env_types.py` & `maxwelld-0.3.0/maxwelld/env_description/env_types.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.9/maxwelld/helpers/state_keeper.py` & `maxwelld-0.3.0/maxwelld/helpers/state_keeper.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.9/maxwelld/server/handlers/env.py` & `maxwelld-0.3.0/maxwelld/server/handlers/env.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.9/maxwelld/server/handlers/status.py` & `maxwelld-0.3.0/maxwelld/server/handlers/status.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.9/maxwelld/server/handlers/up.py` & `maxwelld-0.3.0/maxwelld/server/handlers/up.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,28 +13,26 @@
 
 class UpRequestParams(TypedDict):
     name: str
     config_template: str
     compose_files: str
     isolation: bool
     parallelism_limit: int
-    non_stop_containers: list[str]
     force_restart: bool
 
 
 class UpResponseParams(TypedDict):
     env_id: EnvironmentId
-    new: bool
 
 
 async def up_compose(request: Request) -> web.Response:
     params: UpRequestParams = await request.json()
     async with UP_LOCK:
-        env_id, new = await MaxwellDemonServiceManager().get().up_compose(
+        env_id, is_new = await MaxwellDemonServiceManager().get().up_compose(
             name=params['name'],
             config_template=debase64_pickled(params['config_template']),
             compose_files=params['compose_files'],
             isolation=params['isolation'],
             parallelism_limit=params['parallelism_limit'],
             force_restart=params['force_restart'],
         )
-    return web.json_response(UpResponseParams(env_id=env_id, new=new), status=200)
+    return web.json_response(UpResponseParams(env_id=env_id), status=200)
```

### Comparing `maxwelld-0.2.9/maxwelld/server/maxwelld_server.py` & `maxwelld-0.3.0/maxwelld/server/maxwelld_server.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.9/maxwelld/vedro_plugin/plugin.py` & `maxwelld-0.3.0/maxwelld/vedro_plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,21 +41,15 @@
 
 
 class VedroMaxwellPlugin(Plugin):
     def __init__(self, config: Type["VedroMaxwell"]) -> None:
         super().__init__(config)
         self._enabled = config.enabled
         self._envs: Environments = config.envs
-        self._project = config.project
-        self._non_stop_containers = config.non_stop_containers
-        self._maxwell_demon = MaxwellDemonClient(
-            host="http://127.0.0.1",
-            project=self._project,
-            non_stop_containers=self._non_stop_containers
-        )
+        self._maxwell_demon = MaxwellDemonClient(host="http://127.0.0.1")
         if config.maxwell_demon_client:
             self._maxwell_demon = config.maxwell_demon_client
         self._list_envs = None
 
         self._compose_configs: dict[str, ComposeConfig] = config.compose_cfgs
         assert DEFAULT_COMPOSE in self._compose_configs, \
             'Need to set up at least {DEFAULT_COMPOSE: ComposeConfig(...)} config'
@@ -112,15 +106,15 @@
             CONSOLE.print(
                 Text('Starting ', style=Style.regular)
                 .append(Text(env_name, style=Style.mark))
                 .append(Text(' services for tests ...', style=Style.regular))
             )
 
         env = getattr(self._envs, env_name)
-        started_env_id, restarted = await self._maxwell_demon.up(
+        started_env_id = await self._maxwell_demon.up(
             name=env_name + self._chosen_config_name_postfix,
             config_template=env,
             compose_files=self._compose_choice.compose_files,
             parallelism_limit=self._compose_choice.parallel_env_limit,
             force_restart=self._force_restart
         )
 
@@ -263,15 +257,9 @@
 
     # Maxwell Demon To control the world
     maxwell_demon_client: MaxwellDemonClient = None
 
     # ComposeConfig set of compose files and defaulr parallelism restrictions
     compose_cfgs: dict[str, ComposeConfig] = None
 
-    # Project name directory and {project}_default network
-    project: str = None
-
-    # Containers which shouldn't stop
-    non_stop_containers = ['e2e', 'dockersock']
-
     # services waiter
     wait_all_service_func = wait_all_services_up()
```

### Comparing `maxwelld-0.2.9/maxwelld/vedro_plugin/scenario_tag_processing.py` & `maxwelld-0.3.0/maxwelld/vedro_plugin/scenario_tag_processing.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.9/maxwelld/vedro_plugin/state_waiting.py` & `maxwelld-0.3.0/maxwelld/vedro_plugin/state_waiting.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from maxwelld.helpers.state_keeper import StateKeeper
 from maxwelld.output.console import CONSOLE
 from maxwelld.output.styles import Style
 from maxwelld.vedro_plugin.logger import Logger
 from maxwelld.vedro_plugin.logger import WaitVerbosity
 
 
-def is_service_running_and_healthy(service_state: ServiceComposeState) -> bool:
+def is_service_not_running_or_not_healthy(service_state: ServiceComposeState) -> bool:
     return (service_state.state != ComposeState.RUNNING
             or service_state.health not in (ComposeHealth.EMPTY, ComposeHealth.HEALTHY))
 
 
 class JobResult(Enum):
     GOOD = auto()
     BAD = auto()
@@ -34,75 +34,56 @@
 async def check_all_services_up(
     get_services_state: Callable[[], Awaitable[ServicesComposeState]],
     services: List[str],
     counter_keeper: CountdownCounterKeeper,
     state_keeper: StateKeeper,
     verbose: WaitVerbosity = WaitVerbosity.FULL,
 ) -> JobResult:
-    # print(verbose, counter_keeper._count)
     output_style = Style()
     logger = Logger(CONSOLE)
 
     if state_keeper.in_state(ServicesState.FIRST_STATE):
         logger.log(Text('Starting services check up', style=output_style.info))
         state_keeper.update_state(ServicesState.DEFAULT_STATE)
 
     services_state = await get_services_state()
-    all_up = (all([
+    is_all_up = (all([
         service.state == ComposeState.RUNNING
         for service in services_state if service.name in services
     ]) and all([
         service.health in (ComposeHealth.EMPTY, ComposeHealth.HEALTHY)
         for service in services_state if service.name in services
     ]))
 
-    if all_up:
-        # if verbose == WaitVerbosity.COMPACT:
-        #     logger.log(Text(f' ✔ All services up', style=output_style.good))
-        #     logger.flush()
+    if is_all_up:
         if verbose == WaitVerbosity.FULL:
             logger.log(Text(f' ✔ All services up:', style=output_style.good))
             logger.log(services_state.as_rich_text(style=output_style))
             logger.flush()
         return JobResult.GOOD
 
     counter_keeper.tick()
     if counter_keeper.is_done():
-        logger.log(Text(' ✗ Stop retries. Services still not ready:', style=output_style.bad))
+        logger.log(Text(' ✗ Stop retries. Still not ready services:', style=output_style.bad))
         logger.log(services_state.as_rich_text(style=output_style))
         logger.flush()
         return JobResult.BAD
 
     if state_keeper.not_in_state(services_state):
-        logger.log(Text(f' ✗ Services still not ready:', style=output_style.bad))
+        logger.log(Text(f' ✗ Still not ready services:', style=output_style.bad))
         logger.log(services_state.as_rich_text(
-            filter=is_service_running_and_healthy,
+            filter=is_service_not_running_or_not_healthy,
             style=output_style
         ))
-        if verbose == WaitVerbosity.FULL or verbose == WaitVerbosity.COMPACT or verbose == WaitVerbosity.ON_ERROR:
-            logger.flush()
+        logger.flush()
         state_keeper.update_state(services_state)
 
     return JobResult.BAD
 
 
-def wait_all_services_up(
-    attempts=100,
-    delay_s=3,
-) -> Callable[[Callable, list[str]], ServicesComposeState]:
-    return partial(
-        retry(
-            attempts=attempts,
-            delay=delay_s,
-            until=lambda x: x != JobResult.GOOD
-        )(check_all_services_up),
-        counter_keeper=CountdownCounterKeeper(attempts),
-        state_keeper=StateKeeper(),
-    )
-
 class WaitAllServicesUp:
     def __init__(self, attempts: int = 100, delay_s: int = 3):
         self._attempts = attempts
         self._delay_s = delay_s
 
     def make_checker(self) -> Callable:
         return partial(
@@ -111,8 +92,9 @@
                 delay=self._delay_s,
                 until=lambda x: x != JobResult.GOOD
             )(check_all_services_up),
             counter_keeper=CountdownCounterKeeper(self._attempts),
             state_keeper=StateKeeper(),
         )
 
+
 wait_all_services_up = WaitAllServicesUp
```

### Comparing `maxwelld-0.2.9/maxwelld.egg-info/PKG-INFO` & `maxwelld-0.3.0/maxwelld.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxwelld
-Version: 0.2.9
+Version: 0.3.0
 Summary: docker compose testing env orchestrator
 Home-page: https://github.com/ko10ok/maxwelld
 Author: Yuriy Sagitov
 Author-email: pro100.ko10ok@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -19,52 +19,73 @@
 Requires-Dist: PyYAML<6.1,>=6.0.1
 Requires-Dist: rtry<2.0,>=1.4.0
 Requires-Dist: rich<16.0,>=11.0
 Requires-Dist: aiohttp<3.10,>=3.9.3
 
 # Maxwell's demon of test enviroment
 
-Orchestrate testing env easily
+Orchestrate testing env easily.
 
-# Install & activate
-## Install package
-```shell
-$ pip3 install maxwelld
+Wraps docker-compose and it's dependencies into it's own container with http api.
+
+Execute docker-compose commands sequences for starting requested services set from volumed docker-compose files.
+Rerun environment when in-flight one is different from new requested.
+
+# Vedro usage
+## Add "supervisor" container
+```docker-compose
+  maxwelld:
+    image: docker.io/ko10ok/maxwelld:0.2.9
+    volumes:
+      - .:/project
+      - ./docker-composes:/docker-composes
+      - ./env-tmp:/env-tmp
+    environment:
+      - DOCKER_HOST=tcp://dockersock:2375
+      - COMPOSE_PROJECT_NAME=${COMPOSE_PROJECT_NAME}
+      - NON_STOP_CONTAINERS=dockersock,maxwelld,e2e
+      - HOST_PROJECT_ROOT_DIRECTORY=${HOST_PROJECT_ROOT_DIRECTORY}
 ```
 
 ## Define services config
 ```python
+# env_set.py
 from maxwelld import Environments
 from maxwelld import Environment
 from maxwelld import DEFAULT_ENV
+from maxwelld import Service
+
+web = Service('web')
+web_gallery = Service('web-gallery')  # Service names "web-gallery", "mq", etc from docker-compose.yml
+mq = Service('mq')
+db = Service('db')
 
 class Envs(Environments):
     DEFAULT = Environment(
         DEFAULT_ENV,
-        builder, web, web_gallery, wep_ext_app, cli,
+        web, web_gallery,
         db,
-        mq,
-        e2e
+        mq
     )
 ```
 
 ## Enable plugin
 ```python
 from maxwelld import vedro_plugin as vedro_maxwell
 from maxwelld import ComposeConfig
+from env_set import Envs
 
 class Config(vedro.Config):
 
     class Plugins(vedro.Config.Plugins):
         
         class VedroMaxwell(vedro_maxwell.VedroMaxwell):
             enabled = True
             envs = Envs()
             compose_cfgs = {
-                'default': ComposeConfig(os.environ.get('DC_FILES')),
-                'dev': ComposeConfig(os.environ.get(f'DC_FILES_1'), parallel_env_limit=1),
+                'default': ComposeConfig('docker-compose.yml', parallel_env_limit=1),
+                'dev': ComposeConfig('docker-compose.yml:docker-compose.dev.yml', parallel_env_limit=1),
             }
-            project = os.environ.get('COMPOSE_PROJECT_NAME', default='some_project')
 ```
 
-## Architecture design draft
-![Architecture design draft](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/ko10ok/maxwelld/server_split_prototype/ARCH.puml)
+## Architecture design
+![Architecture design](https://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/ko10ok/maxwelld/server_split_prototype/ARCH.puml)
```

### Comparing `maxwelld-0.2.9/maxwelld.egg-info/SOURCES.txt` & `maxwelld-0.3.0/maxwelld.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.9/setup.py` & `maxwelld-0.3.0/setup.py`

 * *Files identical despite different names*

