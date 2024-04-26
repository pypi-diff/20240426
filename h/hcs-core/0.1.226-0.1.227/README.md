# Comparing `tmp/hcs_core-0.1.226.tar.gz` & `tmp/hcs_core-0.1.227.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs_core-0.1.226.tar", last modified: Wed Apr 17 16:56:49 2024, max compression
+gzip compressed data, was "hcs_core-0.1.227.tar", last modified: Fri Apr 26 16:00:10 2024, max compression
```

## Comparing `hcs_core-0.1.226.tar` & `hcs_core-0.1.227.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.954002 hcs_core-0.1.226/
--rw-r--r--   0 nanw       (501) staff       (20)     1371 2024-04-17 16:56:49.952642 hcs_core-0.1.226/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)       25 2024-04-09 21:58:38.000000 hcs_core-0.1.226/README.md
--rw-r--r--   0 nanw       (501) staff       (20)        7 2024-04-17 16:56:42.000000 hcs_core-0.1.226/VERSION
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.410520 hcs_core-0.1.226/hcs_core/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.597107 hcs_core-0.1.226/hcs_core/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)      790 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/_init.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.609506 hcs_core-0.1.226/hcs_core/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3086 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/built_in_cmds/_ut.py
--rw-r--r--   0 nanw       (501) staff       (20)     2387 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     4034 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     2274 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/cli_options.py
--rw-r--r--   0 nanw       (501) staff       (20)     5791 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)      936 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1160 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)    14088 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/data_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2856 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     1623 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/extension.py
--rw-r--r--   0 nanw       (501) staff       (20)     6432 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)     1200 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     3792 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     6346 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/logger.py
--rw-r--r--   0 nanw       (501) staff       (20)     6518 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     1565 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/profile_store.py
--rw-r--r--   0 nanw       (501) staff       (20)     1767 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/recent.py
--rw-r--r--   0 nanw       (501) staff       (20)     1597 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/state.py
--rw-r--r--   0 nanw       (501) staff       (20)     7933 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     3245 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/var_template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.660148 hcs_core-0.1.226/hcs_core/plan/
--rw-r--r--   0 nanw       (501) staff       (20)      203 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      125 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/actions.py
--rw-r--r--   0 nanw       (501) staff       (20)     1298 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/base_provider.py
--rw-r--r--   0 nanw       (501) staff       (20)      116 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/context.py
--rw-r--r--   0 nanw       (501) staff       (20)    20914 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/core.py
--rw-r--r--   0 nanw       (501) staff       (20)    12918 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/dag.py
--rw-r--r--   0 nanw       (501) staff       (20)     7784 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     5363 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/kop.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.661334 hcs_core-0.1.226/hcs_core/plan/provider/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/provider/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.698263 hcs_core-0.1.226/hcs_core/plan/provider/dev/
--rw-r--r--   0 nanw       (501) staff       (20)       30 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/provider/dev/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       34 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/provider/dev/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1994 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/provider/dev/dummy.py
--rw-r--r--   0 nanw       (501) staff       (20)     1104 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/provider/dev/fibonacci.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.756372 hcs_core-0.1.226/hcs_core/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)      654 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     5194 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     1790 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/sglib/cli_options.py
--rw-r--r--   0 nanw       (501) staff       (20)     8378 2024-04-11 21:31:53.000000 hcs_core-0.1.226/hcs_core/sglib/client_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     8043 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     5167 2024-04-16 17:06:43.000000 hcs_core-0.1.226/hcs_core/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      901 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)    10056 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/sglib/login_support.py
--rw-r--r--   0 nanw       (501) staff       (20)      684 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/sglib/payload_util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.949971 hcs_core-0.1.226/hcs_core/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/__init__.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/check_license.py
--rw-r--r--   0 nanw       (501) staff       (20)     3482 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)      838 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/exit.py
--rw-r--r--   0 nanw       (501) staff       (20)     1755 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/hcs_constants.py
--rw-r--r--   0 nanw       (501) staff       (20)     8438 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/job_view.py
--rw-r--r--   0 nanw       (501) staff       (20)     5288 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1946 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2958 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/scheduler.py
--rw-r--r--   0 nanw       (501) staff       (20)     1239 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/ssl_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1727 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/versions.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.951318 hcs_core-0.1.226/hcs_core.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     1371 2024-04-17 16:56:49.000000 hcs_core-0.1.226/hcs_core.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     1810 2024-04-17 16:56:49.000000 hcs_core-0.1.226/hcs_core.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2024-04-17 16:56:49.000000 hcs_core-0.1.226/hcs_core.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)      265 2024-04-17 16:56:49.000000 hcs_core-0.1.226/hcs_core.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)        9 2024-04-17 16:56:49.000000 hcs_core-0.1.226/hcs_core.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)     1250 2024-04-09 21:58:38.000000 hcs_core-0.1.226/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      265 2024-04-09 21:58:38.000000 hcs_core-0.1.226/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2024-04-17 16:56:49.954342 hcs_core-0.1.226/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)      808 2024-04-09 21:58:38.000000 hcs_core-0.1.226/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-26 16:00:10.689056 hcs_core-0.1.227/
+-rw-r--r--   0 nanw       (501) staff       (20)     1405 2024-04-26 16:00:10.687761 hcs_core-0.1.227/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)       25 2024-04-09 21:58:38.000000 hcs_core-0.1.227/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)        7 2024-04-26 16:00:06.000000 hcs_core-0.1.227/VERSION
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-26 16:00:10.612357 hcs_core-0.1.227/hcs_core/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-26 16:00:10.633339 hcs_core-0.1.227/hcs_core/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)      790 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/_init.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-26 16:00:10.636468 hcs_core-0.1.227/hcs_core/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3086 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/built_in_cmds/_ut.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2387 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4034 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2274 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/cli_options.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5791 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)      936 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1160 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)    14088 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/data_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2856 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1623 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/extension.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6801 2024-04-26 15:58:03.000000 hcs_core-0.1.227/hcs_core/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1200 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4666 2024-04-26 16:00:06.000000 hcs_core-0.1.227/hcs_core/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6346 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/logger.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6518 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1565 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/profile_store.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1767 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/recent.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1619 2024-04-26 15:58:03.000000 hcs_core-0.1.227/hcs_core/ctxp/state.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7933 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3245 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/ctxp/var_template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-26 16:00:10.644169 hcs_core-0.1.227/hcs_core/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)      203 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      125 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/plan/actions.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1298 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/plan/base_provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)      116 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/plan/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)    20914 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/plan/core.py
+-rw-r--r--   0 nanw       (501) staff       (20)    12918 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/plan/dag.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7784 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/plan/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5363 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/plan/kop.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-26 16:00:10.645737 hcs_core-0.1.227/hcs_core/plan/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/plan/provider/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-26 16:00:10.651095 hcs_core-0.1.227/hcs_core/plan/provider/dev/
+-rw-r--r--   0 nanw       (501) staff       (20)       30 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/plan/provider/dev/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       34 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/plan/provider/dev/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1994 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/plan/provider/dev/dummy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1104 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/plan/provider/dev/fibonacci.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-26 16:00:10.668174 hcs_core-0.1.227/hcs_core/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)      654 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5194 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1790 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/sglib/cli_options.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8378 2024-04-11 21:31:53.000000 hcs_core-0.1.227/hcs_core/sglib/client_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8043 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5167 2024-04-20 00:00:21.000000 hcs_core-0.1.227/hcs_core/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      901 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)    10056 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/sglib/login_support.py
+-rw-r--r--   0 nanw       (501) staff       (20)      684 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/sglib/payload_util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-26 16:00:10.684297 hcs_core-0.1.227/hcs_core/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/util/__init__.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/util/check_license.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3482 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)      838 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/util/exit.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1755 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/util/hcs_constants.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8438 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/util/job_view.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5288 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1946 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2958 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/util/scheduler.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1239 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/util/ssl_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1727 2024-04-09 21:58:38.000000 hcs_core-0.1.227/hcs_core/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-26 16:00:10.686101 hcs_core-0.1.227/hcs_core.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     1405 2024-04-26 16:00:10.000000 hcs_core-0.1.227/hcs_core.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     1810 2024-04-26 16:00:10.000000 hcs_core-0.1.227/hcs_core.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2024-04-26 16:00:10.000000 hcs_core-0.1.227/hcs_core.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      284 2024-04-26 16:00:10.000000 hcs_core-0.1.227/hcs_core.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        9 2024-04-26 16:00:10.000000 hcs_core-0.1.227/hcs_core.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (501) staff       (20)     1250 2024-04-09 21:58:38.000000 hcs_core-0.1.227/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      284 2024-04-26 15:58:03.000000 hcs_core-0.1.227/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2024-04-26 16:00:10.689297 hcs_core-0.1.227/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)      808 2024-04-09 21:58:38.000000 hcs_core-0.1.227/setup.py
```

### Comparing `hcs_core-0.1.226/PKG-INFO` & `hcs_core-0.1.227/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-core
-Version: 0.1.226
+Version: 0.1.227
 Summary: Horizon Cloud Service CLI module.
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
@@ -27,10 +27,11 @@
 Requires-Dist: questionary==1.10.0
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: setuptools_scm==7.1.0
 Requires-Dist: python-ulid>=1.1.0
 Requires-Dist: retry>=0.9.2
 Requires-Dist: graphviz>=0.20.1
 Requires-Dist: rich>=13.4.2
+Requires-Dist: portalocker>=2.8.2
 
 hcs-cli core component.
```

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/__init__.py` & `hcs_core-0.1.227/hcs_core/ctxp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/_init.py` & `hcs_core-0.1.227/hcs_core/ctxp/_init.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/built_in_cmds/_ut.py` & `hcs_core-0.1.227/hcs_core/ctxp/built_in_cmds/_ut.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/built_in_cmds/context.py` & `hcs_core-0.1.227/hcs_core/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/built_in_cmds/profile.py` & `hcs_core-0.1.227/hcs_core/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/cli_options.py` & `hcs_core-0.1.227/hcs_core/ctxp/cli_options.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/cli_processor.py` & `hcs_core-0.1.227/hcs_core/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/config.py` & `hcs_core-0.1.227/hcs_core/ctxp/config.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/context.py` & `hcs_core-0.1.227/hcs_core/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/data_util.py` & `hcs_core-0.1.227/hcs_core/ctxp/data_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/duration.py` & `hcs_core-0.1.227/hcs_core/ctxp/duration.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/extension.py` & `hcs_core-0.1.227/hcs_core/ctxp/extension.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/fstore.py` & `hcs_core-0.1.227/hcs_core/ctxp/fstore.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,71 +16,75 @@
 import os
 import logging
 from os import path, listdir
 from typing import Any
 from collections.abc import Generator
 from . import jsondot
 from .jsondot import dotdict
+import yaml
+import shutil
+
 
 log = logging.getLogger(__name__)
 
 
 def _validate_key(key: str):
     # if key.find(os.pathsep) >= 0:
     if key.find("/") >= 0 or key.find("\\") >= 0:
         raise Exception("Invalid profile name: " + key)
 
 
 def _load_yaml(file_name: str):
     if not os.path.exists(file_name):
         return
-    with open(file_name, "r") as stream:
-        import yaml
-
-        ret = yaml.safe_load(stream)
+    with open(file_name, "r") as file:
+        ret = yaml.safe_load(file)
         return jsondot.dotify(ret)
 
 
 def _load_text(file_name: str) -> str:
     if not os.path.exists(file_name):
         return
     with open(file_name, "r", encoding="utf-8") as file:
         return file.read()
 
 
 def _load_file(file_path: str, format: str):
-    _, ext = path.splitext(file_path)
-
-    if ext == ".json" or (ext == "" and format == "json"):
-        return jsondot.load(file_path)
-    if ext == ".yaml" or ext == ".yml" or (ext == "" and (format == "yaml" or format == "yml")):
-        return _load_yaml(file_path)
-    if ext == ".txt" or (ext == "" and format in ["text", "plain", "txt"]):
-        return _load_text(file_path)
-
-    if format != "auto":
-        raise Exception(f"Invalid store format: {format}")
-
-    # The specified path has no ext name, and format is auto.
-    if os.path.exists(file_path):
-        return jsondot.load(file_path)
-
-    tmp = file_path + ".json"
-    if os.path.exists(tmp):
-        return jsondot.load(file_path + ".json")
-
-    tmp = file_path + ".yaml"
-    if os.path.exists(tmp):
-        return _load_yaml(tmp)
-
-    tmp = file_path + ".yml"
-    if os.path.exists(tmp):
-        return _load_yaml(tmp)
+    try:
+        _, ext = path.splitext(file_path)
 
-    # Not found
+        if ext == ".json" or (ext == "" and format == "json"):
+            return jsondot.load(file_path, lock=True)
+        if ext == ".yaml" or ext == ".yml" or (ext == "" and (format == "yaml" or format == "yml")):
+            return _load_yaml(file_path)
+        if ext == ".txt" or (ext == "" and format in ["text", "plain", "txt"]):
+            return _load_text(file_path)
+
+        if format != "auto":
+            raise Exception(f"Invalid store format: {format}")
+
+        # The specified path has no ext name, and format is auto.
+        if os.path.exists(file_path):
+            return jsondot.load(file_path, lock=True)
+
+        tmp = file_path + ".json"
+        if os.path.exists(tmp):
+            return jsondot.load(file_path + ".json", lock=True)
+
+        tmp = file_path + ".yaml"
+        if os.path.exists(tmp):
+            return _load_yaml(tmp)
+
+        tmp = file_path + ".yml"
+        if os.path.exists(tmp):
+            return _load_yaml(tmp)
+
+        # Not found
+    except Exception as e:
+        raise Exception(f"Fail with file {file_path}") from e
 
 
 class fstore:
     """A key-value store, optionally backed by a file system directory and files in it."""
 
     def __init__(self, store_path: str = None, create: bool = True):
         """Initialize the store
@@ -138,22 +142,25 @@
         data = jsondot.dotify(data)
 
         self._cache[key] = data
         if self._path:
             file_path = self._get_path(key)
             log.debug(f"Write {file_path}")
             if format == "json":
-                jsondot.save(data, file_path)
+                jsondot.save(data, file_path, lock=True)
             elif format == "text":
                 with open(file_path, "w", encoding="utf-8") as outfile:
+                    # TODO lock
                     outfile.write(str(data))
             elif format == "json-compact":
-                jsondot.save(data, file_path, False)
+                jsondot.save(data, file_path, format=False, lock=True)
             elif format == "yaml":
-                raise Exception("TODO")
+                with open(file_path, "w", encoding="utf-8") as outfile:
+                    # TODO lock
+                    yaml.safe_dump(data, outfile)
             else:
                 raise Exception(f"Invalid format. key={key}, format={format}")
 
         return data
 
     def delete(self, key: str) -> None:
         _validate_key(key)
@@ -179,16 +186,14 @@
     def clear(self) -> None:
         for k in self.keys():
             self.delete(k)
 
     def destroy(self) -> None:
         self._cache.clear()
         if self._path:
-            import shutil
-
             shutil.rmtree(self._path)
 
     def size(self) -> int:
         return len(self.keys())
 
     def contains(self, key: str) -> bool:
         if key in self._cache:
```

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/init.py` & `hcs_core-0.1.227/hcs_core/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/jsondot.py` & `hcs_core-0.1.227/hcs_core/ctxp/jsondot.py`

 * *Files 21% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 my_dict = jsondot.dotify(my_dict)
 print(my_dict.key1.key2)
 """
 
 import json
 import os.path
 import copy
+import time
+import random
+import portalocker
 from typing import Any
 
 
 class dotdict(dict):
     """dot.notation access to dictionary attributes"""
 
     __getattr__ = dict.get
@@ -118,26 +121,52 @@
         return target
     if isinstance(target, dict):
         for k in target:
             target[k] = plain(target[k])
         return dict(target)
 
 
-def load(file: str, default: Any = None) -> Any:
+def parse(text: str) -> dotdict:
+    dict = json.loads(text)
+    return dotify(dict)
+
+
+def _lock_with_retry(file, for_read: bool):
+    if for_read:
+        flags = portalocker.LockFlags.SHARED
+    else:
+        flags = portalocker.LockFlags.EXCLUSIVE  # | portalocker.LockFlags.NON_BLOCKING
+
+    max_retry = 6
+    retry = 0
+    backoff_seconds = 0.05
+    while True:
+        try:
+            portalocker.lock(file, flags)
+            return
+        except Exception as e:
+            retry += 1
+            if retry > max_retry:
+                raise Exception(f"Fail locking file {file}") from e
+            random_delay = backoff_seconds + random.uniform(0, 0.1)
+            time.sleep(random_delay)
+            backoff_seconds += backoff_seconds
+
+
+def load(file: str, default: Any = None, lock: bool = False) -> Any:
     if not os.path.exists(file):
         return dotify(default)
     with open(file) as json_file:
+        if lock:
+            _lock_with_retry(json_file, True)
         dict = json.load(json_file)
     return dotify(dict)
 
 
-def parse(text: str) -> dotdict:
-    dict = json.loads(text)
-    return dotify(dict)
-
-
-def save(data: dict, file, format=True) -> None:
+def save(data: dict, file, format=True, lock: bool = False) -> None:
     with open(file, "w") as outfile:
+        if lock:
+            _lock_with_retry(outfile, False)
         if format:
             json.dump(data, outfile, indent="\t", default=vars)
         else:
             json.dump(data, outfile)
```

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/logger.py` & `hcs_core-0.1.227/hcs_core/ctxp/logger.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/profile.py` & `hcs_core-0.1.227/hcs_core/ctxp/profile.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/profile_store.py` & `hcs_core-0.1.227/hcs_core/ctxp/profile_store.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/recent.py` & `hcs_core-0.1.227/hcs_core/ctxp/recent.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/state.py` & `hcs_core-0.1.227/hcs_core/ctxp/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,23 +23,23 @@
     def __init__(self, file_path: str):
         self._path = file_path
         self._cache = None
         pathlib.Path(os.path.dirname(file_path)).mkdir(parents=True, exist_ok=True)
 
     def _data(self, reload: bool = False):
         if self._cache is None or reload:
-            self._cache = jsondot.load(self._path, {})
+            self._cache = jsondot.load(self._path, {}, lock=True)
         return self._cache
 
     def get(self, key: str, default: Any, reload: bool = False):
         return self._data(reload).get(key, default)
 
     def set(self, key: str, value: Any):
         self._data()[key] = value
-        jsondot.save(self._cache, self._path)
+        jsondot.save(self._cache, self._path, lock=True)
 
 
 _file: _StateFile = None
 
 
 def init(store_path: str, name: str):
     global _file
```

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/util.py` & `hcs_core-0.1.227/hcs_core/ctxp/util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/ctxp/var_template.py` & `hcs_core-0.1.227/hcs_core/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/plan/base_provider.py` & `hcs_core-0.1.227/hcs_core/plan/base_provider.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/plan/core.py` & `hcs_core-0.1.227/hcs_core/plan/core.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/plan/dag.py` & `hcs_core-0.1.227/hcs_core/plan/dag.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/plan/helper.py` & `hcs_core-0.1.227/hcs_core/plan/helper.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/plan/kop.py` & `hcs_core-0.1.227/hcs_core/plan/kop.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/plan/provider/dev/dummy.py` & `hcs_core-0.1.227/hcs_core/plan/provider/dev/dummy.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/plan/provider/dev/fibonacci.py` & `hcs_core-0.1.227/hcs_core/plan/provider/dev/fibonacci.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/sglib/__init__.py` & `hcs_core-0.1.227/hcs_core/sglib/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/sglib/auth.py` & `hcs_core-0.1.227/hcs_core/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/sglib/cli_options.py` & `hcs_core-0.1.227/hcs_core/sglib/cli_options.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/sglib/client_util.py` & `hcs_core-0.1.227/hcs_core/sglib/client_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/sglib/csp.py` & `hcs_core-0.1.227/hcs_core/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/sglib/ez_client.py` & `hcs_core-0.1.227/hcs_core/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/sglib/hcs_client.py` & `hcs_core-0.1.227/hcs_core/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/sglib/login_support.py` & `hcs_core-0.1.227/hcs_core/sglib/login_support.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/sglib/payload_util.py` & `hcs_core-0.1.227/hcs_core/sglib/payload_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/util/check_license.py` & `hcs_core-0.1.227/hcs_core/util/check_license.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/util/duration.py` & `hcs_core-0.1.227/hcs_core/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/util/exit.py` & `hcs_core-0.1.227/hcs_core/util/exit.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/util/hcs_constants.py` & `hcs_core-0.1.227/hcs_core/util/hcs_constants.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/util/job_view.py` & `hcs_core-0.1.227/hcs_core/util/job_view.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/util/pki_util.py` & `hcs_core-0.1.227/hcs_core/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/util/query_util.py` & `hcs_core-0.1.227/hcs_core/util/query_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/util/scheduler.py` & `hcs_core-0.1.227/hcs_core/util/scheduler.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/util/ssl_util.py` & `hcs_core-0.1.227/hcs_core/util/ssl_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core/util/versions.py` & `hcs_core-0.1.227/hcs_core/util/versions.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/hcs_core.egg-info/PKG-INFO` & `hcs_core-0.1.227/hcs_core.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-core
-Version: 0.1.226
+Version: 0.1.227
 Summary: Horizon Cloud Service CLI module.
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
@@ -27,10 +27,11 @@
 Requires-Dist: questionary==1.10.0
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: setuptools_scm==7.1.0
 Requires-Dist: python-ulid>=1.1.0
 Requires-Dist: retry>=0.9.2
 Requires-Dist: graphviz>=0.20.1
 Requires-Dist: rich>=13.4.2
+Requires-Dist: portalocker>=2.8.2
 
 hcs-cli core component.
```

### Comparing `hcs_core-0.1.226/hcs_core.egg-info/SOURCES.txt` & `hcs_core-0.1.227/hcs_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/pyproject.toml` & `hcs_core-0.1.227/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.226/setup.py` & `hcs_core-0.1.227/setup.py`

 * *Files identical despite different names*

