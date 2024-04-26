# Comparing `tmp/buildarr-0.7.1.tar.gz` & `tmp/buildarr-0.8.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildarr-0.7.1.tar", max compression
+gzip compressed data, was "buildarr-0.8.0b1.tar", last modified: Fri Apr 26 07:37:44 2024, max compression
```

## Comparing `buildarr-0.7.1.tar` & `buildarr-0.8.0b1.tar`

### file list

```diff
@@ -1,50 +1,170 @@
--rw-r--r--   0        0        0    35149 2023-11-13 06:32:47.517005 buildarr-0.7.1/LICENSE
--rw-r--r--   0        0        0    17108 2023-11-13 06:32:47.517005 buildarr-0.7.1/README.md
--rw-r--r--   0        0        0      946 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/__init__.py
--rw-r--r--   0        0        0     1783 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/cli/__init__.py
--rw-r--r--   0        0        0    11333 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/cli/compose.py
--rw-r--r--   0        0        0    20322 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/cli/daemon.py
--rw-r--r--   0        0        0     2486 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/cli/exceptions.py
--rw-r--r--   0        0        0     1254 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/cli/main.py
--rw-r--r--   0        0        0    12799 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/cli/run.py
--rw-r--r--   0        0        0     7885 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/cli/test_config.py
--rw-r--r--   0        0        0     1473 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/config/__init__.py
--rw-r--r--   0        0        0    35323 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/config/base.py
--rw-r--r--   0        0        0     4635 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/config/buildarr.py
--rw-r--r--   0        0        0     1071 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/config/exceptions.py
--rw-r--r--   0        0        0    11620 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/config/load.py
--rw-r--r--   0        0        0    11532 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/config/models.py
--rw-r--r--   0        0        0     2607 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/config/post_init_render.py
--rw-r--r--   0        0        0     2434 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/config/render_instance_configs.py
--rw-r--r--   0        0        0     5326 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/config/resolve_instance_dependencies.py
--rw-r--r--   0        0        0     2164 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/config/types.py
--rw-r--r--   0        0        0      827 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/exceptions.py
--rw-r--r--   0        0        0     3046 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/logging.py
--rw-r--r--   0        0        0     9693 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/manager/__init__.py
--rw-r--r--   0        0        0      877 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/manager/exceptions.py
--rw-r--r--   0        0        0      872 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/plugins/dummy/__init__.py
--rw-r--r--   0        0        0     7635 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/plugins/dummy/api.py
--rw-r--r--   0        0        0     2922 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/plugins/dummy/cli.py
--rw-r--r--   0        0        0     5814 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/plugins/dummy/config/__init__.py
--rw-r--r--   0        0        0     7516 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/plugins/dummy/config/settings.py
--rw-r--r--   0        0        0     1186 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/plugins/dummy/config/types.py
--rw-r--r--   0        0        0     1360 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/plugins/dummy/exceptions.py
--rw-r--r--   0        0        0      932 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/plugins/dummy/manager.py
--rw-r--r--   0        0        0     1160 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/plugins/dummy/plugin.py
--rw-r--r--   0        0        0     4038 2023-11-13 06:32:47.517005 buildarr-0.7.1/buildarr/plugins/dummy/secrets.py
--rw-r--r--   0        0        0     5853 2023-11-13 06:32:47.521005 buildarr-0.7.1/buildarr/plugins/dummy/server.py
--rw-r--r--   0        0        0     1386 2023-11-13 06:32:47.521005 buildarr-0.7.1/buildarr/plugins/dummy/types.py
--rw-r--r--   0        0        0     2236 2023-11-13 06:32:47.521005 buildarr-0.7.1/buildarr/plugins/load.py
--rw-r--r--   0        0        0     3728 2023-11-13 06:32:47.521005 buildarr-0.7.1/buildarr/plugins/models.py
--rw-r--r--   0        0        0     1239 2023-11-13 06:32:47.521005 buildarr-0.7.1/buildarr/plugins/types.py
--rw-r--r--   0        0        0        0 2023-11-13 06:32:47.521005 buildarr-0.7.1/buildarr/py.typed
--rw-r--r--   0        0        0      850 2023-11-13 06:32:47.521005 buildarr-0.7.1/buildarr/secrets/__init__.py
--rw-r--r--   0        0        0     1960 2023-11-13 06:32:47.521005 buildarr-0.7.1/buildarr/secrets/base.py
--rw-r--r--   0        0        0     3210 2023-11-13 06:32:47.521005 buildarr-0.7.1/buildarr/secrets/models.py
--rw-r--r--   0        0        0     7729 2023-11-13 06:32:47.521005 buildarr-0.7.1/buildarr/state.py
--rw-r--r--   0        0        0     3579 2023-11-13 06:32:47.521005 buildarr-0.7.1/buildarr/trash.py
--rw-r--r--   0        0        0    19089 2023-11-13 06:32:47.521005 buildarr-0.7.1/buildarr/types.py
--rw-r--r--   0        0        0     5021 2023-11-13 06:32:47.521005 buildarr-0.7.1/buildarr/util.py
--rw-r--r--   0        0        0     2514 2023-11-13 06:32:47.521005 buildarr-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    18786 1970-01-01 00:00:00.000000 buildarr-0.7.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.462775 buildarr-0.8.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.434774 buildarr-0.8.0b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.438774 buildarr-0.8.0b1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/.github/ISSUE_TEMPLATE/release.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.438774 buildarr-0.8.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18747 2024-04-26 07:37:44.462775 buildarr-0.8.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17116 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.442774 buildarr-0.8.0b1/buildarr/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.442774 buildarr-0.8.0b1/buildarr/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14928 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/cli/compose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20624 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/cli/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12831 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8432 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/cli/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.446774 buildarr-0.8.0b1/buildarr/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/config/buildarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/config/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11660 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/config/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12169 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/config/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/config/post_init_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/config/render_instance_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/config/resolve_instance_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/config/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.446774 buildarr-0.8.0b1/buildarr/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/manager/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.446774 buildarr-0.8.0b1/buildarr/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.446774 buildarr-0.8.0b1/buildarr/plugins/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8415 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.446774 buildarr-0.8.0b1/buildarr/plugins/dummy/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    11649 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy/config/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy/config/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.450775 buildarr-0.8.0b1/buildarr/plugins/dummy2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy2/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.450775 buildarr-0.8.0b1/buildarr/plugins/dummy2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy2/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy2/config/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy2/config/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy2/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy2/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy2/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/dummy2/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/plugins/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.450775 buildarr-0.8.0b1/buildarr/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/secrets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/secrets/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/trash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/buildarr/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.462775 buildarr-0.8.0b1/buildarr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18747 2024-04-26 07:37:44.000000 buildarr-0.8.0b1/buildarr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-26 07:37:44.000000 buildarr-0.8.0b1/buildarr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 07:37:44.000000 buildarr-0.8.0b1/buildarr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-26 07:37:44.000000 buildarr-0.8.0b1/buildarr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-26 07:37:44.000000 buildarr-0.8.0b1/buildarr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 07:37:44.000000 buildarr-0.8.0b1/buildarr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.450775 buildarr-0.8.0b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16843 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.450775 buildarr-0.8.0b1/docs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/docs/plugins/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    33417 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/docs/release-notes.md
+-rw-r--r--   0 runner    (1001) docker     (127)    19330 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    94714 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/pdm.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/pyrightconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.450775 buildarr-0.8.0b1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1789 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/scripts/bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 07:37:44.462775 buildarr-0.8.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/test.Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.450775 buildarr-0.8.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.454774 buildarr-0.8.0b1/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.454774 buildarr-0.8.0b1/tests/functional/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.454774 buildarr-0.8.0b1/tests/functional/cli/compose/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/compose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/compose/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/compose/test_opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/compose/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/compose/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.454774 buildarr-0.8.0b1/tests/functional/cli/daemon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/daemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20958 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/daemon/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/daemon/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/daemon/test_opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/daemon/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.454774 buildarr-0.8.0b1/tests/functional/cli/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/dummy/test_dump_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.454774 buildarr-0.8.0b1/tests/functional/cli/run/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15832 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/run/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/run/test_opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13937 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/run/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9108 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/run/test_secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.458774 buildarr-0.8.0b1/tests/functional/cli/test_config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/test_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26331 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/test_config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/test_config/test_opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/cli/test_config/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/functional/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.458774 buildarr-0.8.0b1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.458774 buildarr-0.8.0b1/tests/unit/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.458774 buildarr-0.8.0b1/tests/unit/config/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/config/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/config/base/test_decode_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/config/base/test_delete_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/config/base/test_encode_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/config/base/test_from_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9745 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/config/base/test_get_create_remote_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/config/base/test_get_local_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16386 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/config/base/test_get_update_remote_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/config/base/test_log_delete_remote_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/config/base/test_model_dump_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/config/base/test_update_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:44.462775 buildarr-0.8.0b1/tests/unit/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/types/test_baseenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/types/test_emailstr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/types/test_localpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/types/test_lowercasenonemptystr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/types/test_lowercasestr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/types/test_model_config_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/types/test_nameemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/types/test_nonemptystr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/types/test_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/types/test_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/types/test_pureposixpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/types/test_purewindowspath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/types/test_rssurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/types/test_secretstr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/types/test_trashid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/types/test_uppercasenonemptystr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-26 07:37:29.000000 buildarr-0.8.0b1/tests/unit/types/test_uppercasestr.py
```

### Comparing `buildarr-0.7.1/LICENSE` & `buildarr-0.8.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `buildarr-0.7.1/README.md` & `buildarr-0.8.0b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Welcome to Buildarr!
 
-[![Docker Version](https://img.shields.io/docker/v/callum027/buildarr?sort=semver)](https://hub.docker.com/r/callum027/buildarr) [![PyPI](https://img.shields.io/pypi/v/buildarr)](https://pypi.org/project/buildarr) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/buildarr) [![GitHub](https://img.shields.io/github/license/buildarr/buildarr)](https://github.com/buildarr/buildarr/blob/main/LICENSE) ![Pre-commit hooks](https://github.com/buildarr/buildarr/actions/workflows/pre-commit.yml/badge.svg) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Docker Version](https://img.shields.io/docker/v/callum027/buildarr?sort=semver)](https://hub.docker.com/r/callum027/buildarr) [![PyPI](https://img.shields.io/pypi/v/buildarr)](https://pypi.org/project/buildarr) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/buildarr) [![GitHub](https://img.shields.io/github/license/buildarr/buildarr)](https://github.com/buildarr/buildarr/blob/main/LICENSE) ![Test Status](https://img.shields.io/github/actions/workflow/status/buildarr/buildarr/test.yml?label=tests) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This is Buildarr, a solution to automating deployment and configuration of your *Arr stack.
 
 Have you spent many hours getting your setup for one or more linked Sonarr/Radarr/Prowlarr instances just right, only to have no way to reproduce this setup apart from UI screenshots and database backups?
 
 Buildarr aims to alleviate those concerns by using a static configuration file to store settings for all your *Arr applications, and automatically configure them as defined. It can just once using an ad-hoc user command, or as a service to keep your application configurations up to date. Buildarr runs idempotently, only making changes to your instance if they are required.
```

### Comparing `buildarr-0.7.1/buildarr/__init__.py` & `buildarr-0.8.0b1/buildarr/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,18 +12,17 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr root module.
 """
 
-
 from __future__ import annotations
 
 from importlib_metadata import PackageNotFoundError, version as package_version
 
 __all__ = ["__version__"]
 
 try:
     __version__: str = package_version("buildarr")
-except PackageNotFoundError:
+except PackageNotFoundError:  # pragma: no cover
     __version__ = "0.1.0"
```

### Comparing `buildarr-0.7.1/buildarr/cli/__init__.py` & `buildarr-0.8.0b1/buildarr/cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -13,15 +13,14 @@
 
 
 """
 buildarr/cli/__init__.py
 Buildarr command line interface (CLI) global group.
 """
 
-
 from __future__ import annotations
 
 import os
 
 import click
 
 from ..logging import setup_logger
```

### Comparing `buildarr-0.7.1/buildarr/cli/compose.py` & `buildarr-0.8.0b1/buildarr/cli/compose.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,41 +12,43 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 `buildarr compose` CLI command.
 """
 
-
 from __future__ import annotations
 
+import sys
+
 from ipaddress import ip_address
 from logging import getLogger
 from pathlib import Path
 from textwrap import indent
 from typing import TYPE_CHECKING, cast
 
 import click
 import yaml
 
 from .. import __version__
 from ..config import load_config, load_instance_configs, resolve_instance_dependencies
 from ..logging import get_log_level
 from ..manager import load_managers
 from ..state import state
-from ..util import get_resolved_path
+from ..util import get_resolved_path, windows_to_posix
 from . import cli
 from .exceptions import (
     ComposeInvalidHostnameError,
+    ComposeInvalidVolumeDefinitionError,
     ComposeNoPluginsDefinedError,
     ComposeNotSupportedError,
 )
 
 if TYPE_CHECKING:
-    from typing import Any, Dict, Set
+    from typing import Any, Dict, List, Set
 
 
 logger = getLogger(__name__)
 
 
 @cli.command(
     help=(
@@ -143,15 +145,15 @@
         str(config_path),
     )
 
     logger.debug("Loading configuration file '%s'", config_path)
     load_config(path=config_path, use_plugins=use_plugins)
     logger.debug("Finished loading configuration file")
     logger.debug("Buildarr configuration:")
-    for config_line in state.config.yaml(exclude_unset=True).splitlines():
+    for config_line in state.config.model_dump_yaml(exclude_unset=True).splitlines():
         logger.debug(indent(config_line, "  "))
 
     logger.debug("Loading plugin managers")
     load_managers(use_plugins)
     logger.debug("Finished loading plugin managers")
     logger.debug("Managers loaded for the following plugins:")
     for plugin_name in state.managers.keys():
@@ -160,29 +162,29 @@
     logger.debug("Loading instance configurations")
     load_instance_configs(use_plugins)
     logger.debug("Finished loading instance configurations")
     for plugin_name, instance_configs in state.instance_configs.items():
         for instance_name, instance_config in instance_configs.items():
             with state._with_context(plugin_name=plugin_name, instance_name=instance_name):
                 logger.debug("Instance configuration:")
-                for config_line in instance_config.yaml(exclude_unset=True).splitlines():
+                for config_line in instance_config.model_dump_yaml(exclude_unset=True).splitlines():
                     logger.debug(indent(config_line, "  "))
 
     if not state.active_plugins:
         raise ComposeNoPluginsDefinedError("No loaded plugins configured in Buildarr")
 
     logger.debug("Resolving instance dependencies")
     resolve_instance_dependencies()
     logger.debug("Finished resolving instance dependencies")
     logger.debug("Execution order:")
     for i, (plugin_name, instance_name) in enumerate(state._execution_order, 1):
         logger.debug("  %i. %s.instances[%s]", i, plugin_name, repr(instance_name))
 
     compose_obj: Dict[str, Any] = {"version": compose_version, "services": {}}
-    hostnames: Dict[str, str] = {}
+    used_hostnames: Dict[str, Dict[str, str]] = {}
     volumes: Set[str] = set()
 
     for plugin_name, instance_name in state._execution_order:
         manager = state.managers[plugin_name]
         instance_config = state.instance_configs[plugin_name][instance_name]
         with state._with_context(plugin_name=plugin_name, instance_name=instance_name):
             service_name = f"{plugin_name}_{instance_name}"
@@ -201,77 +203,142 @@
             except ValueError:
                 pass
             if hostname == "localhost":
                 raise ComposeInvalidHostnameError(
                     f"Invalid hostname '{hostname}' for {plugin_name} instance '{instance_name}': "
                     "Hostname must not be localhost for Docker Compose services",
                 )
-            if hostname in hostnames:
+            if hostname in used_hostnames:
+                used_by = used_hostnames[hostname]
                 raise ComposeInvalidHostnameError(
-                    f"Invalid hostname '{hostname}' for {plugin_name} instance '{instance_name}': "
-                    f"Hostname already used by service '{hostnames[hostname]}'",
+                    (
+                        f"Invalid hostname '{hostname}' for "
+                        f"{plugin_name} instance '{instance_name}': "
+                        "Hostname already used by "
+                        f"{used_by['plugin_name']} instance '{used_by['instance_name']}'"
+                    ),
                 )
-            hostnames[hostname] = service_name
+            used_hostnames[hostname] = {"plugin_name": plugin_name, "instance_name": instance_name}
             logger.debug("Finished validating service hostname")
+            logger.debug("Generating service-specific configuration")
             try:
-                logger.debug("Generating service-specific configuration")
-                service: Dict[str, Any] = {
-                    **manager.to_compose_service(
-                        instance_config=instance_config,
-                        compose_version=compose_version,
-                        service_name=service_name,
-                    ),
-                    "hostname": hostname,
-                    "restart": compose_restart,
-                }
-                logger.debug("Finished generating service-specific configuration")
+                service_config = manager.to_compose_service(
+                    instance_config=instance_config,
+                    compose_version=compose_version,
+                    service_name=service_name,
+                )
             except NotImplementedError:
                 raise ComposeNotSupportedError(
                     f"Plugin '{plugin_name}' does not support Docker Compose "
                     "service generation from instance configurations",
                 ) from None
+            if "volumes" in service_config:
+                # Convert the old-style dictionary volume definitions
+                # to the new-style list structure with long-form syntax.
+                if isinstance(service_config["volumes"], dict):
+                    service_config["volumes"] = [
+                        {
+                            "type": (
+                                "volume" if "/" not in source and "\\" not in source else "bind"
+                            ),
+                            "source": source,
+                            "target": target,
+                        }
+                        for source, target in service_config["volumes"].items()
+                    ]
+                # Otherwise, assume the definition is a list structure.
+                # Convert tuples replicating short-form Docker volume syntax to long-form syntax.
+                else:
+                    new_volumes: List[Dict[str, Any]] = []
+                    for volume in service_config["volumes"]:
+                        if isinstance(volume, tuple):
+                            try:
+                                source, target, options = volume
+                            except ValueError:
+                                try:
+                                    source, target = volume
+                                    options = []
+                                except ValueError:
+                                    raise ComposeInvalidVolumeDefinitionError(
+                                        (
+                                            "Invalid tuple volume definition for "
+                                            f"{plugin_name} instance '{instance_name}' "
+                                            "(expecting a 2-tuple, or 3-tuple): "
+                                            f"{volume}"
+                                        ),
+                                    ) from None
+                            options_set = set(opt.strip().lower() for opt in options)
+                            new_volume = {
+                                "type": (
+                                    "volume" if "/" not in source and "\\" not in source else "bind"
+                                ),
+                                "source": source,
+                                "target": target,
+                                "read_only": "ro" in options_set and "rw" not in options_set,
+                            }
+                            if new_volume["type"] == "bind":
+                                new_volume["bind"] = {"create_host_path": True}
+                            new_volumes.append(new_volume)
+                        else:
+                            new_volumes.append(volume)
+                    service_config["volumes"] = new_volumes
+                # If we are running on Windows, convert the source and target
+                # fields to POSIX paths, as required.
+                if sys.platform == "win32":
+                    for volume in service_config["volumes"]:
+                        for key in ("source", "target"):
+                            volume[key] = windows_to_posix(volume[key])
+            service: Dict[str, Any] = {
+                **service_config,
+                "hostname": hostname,
+                "restart": compose_restart,
+            }
+            logger.debug("Finished generating service-specific configuration")
             if (plugin_name, instance_name) in state._instance_dependencies:
                 depends_on: Set[str] = set()
                 logger.debug("Generating service dependencies")
                 for target_plugin, target_instance in state._instance_dependencies[
                     (plugin_name, instance_name)
                 ]:
                     target_service = f"{target_plugin}_{target_instance}"
                     logger.debug("Adding dependency to service '%s'", target_service)
                     depends_on.add(target_service)
                 service["depends_on"] = list(depends_on)
                 logger.debug("Finished generating service dependencies")
-            # TODO: Handle more types of volume definitions
-            # (e.g. volume lists, modern-style mount definitions).
-            for volume_name in service.get("volumes", {}).keys():
-                if "/" not in volume_name and "\\" not in volume_name:
+            for volume in service.get("volumes", []):
+                if volume["type"] == "volume":
                     logger.debug(
                         "Adding named volume '%s' to the list of internal volumes",
-                        volume_name,
+                        volume["source"],
                     )
-                    volumes.add(volume_name)
+                    volumes.add(volume["source"])
                 else:
                     logger.debug(
                         (
-                            "Volume '%s' determined to likely be a bind mount, "
+                            "Volume '%s:%s' is a bind mount, "
                             "not adding to the list of internal volumes"
                         ),
-                        volume_name,
+                        volume["source"],
+                        volume["target"],
                     )
             compose_obj["services"][service_name] = service
             logger.debug("Finished generating Docker Compose service configuration")
 
     logger.debug("Generating Docker Compose configuration for service 'buildarr'")
     compose_obj["services"]["buildarr"] = {
         "image": f"{state.config.buildarr.docker_image_uri}:{__version__}",
         "command": ["daemon", f"/config/{state.config_files[0].name}"],
         "volumes": [
             {
                 "type": "bind",
-                "source": str(state.config_files[0].parent),
+                "source": (
+                    windows_to_posix(state.config_files[0].parent)
+                    if sys.platform == "win32"
+                    else str(state.config_files[0].parent)
+                ),
                 "target": "/config",
                 "read_only": True,
             },
         ],
         "restart": compose_restart,
         "depends_on": [
             f"{plugin_name}_{instance_name}"
@@ -279,8 +346,8 @@
         ],
     }
     logger.debug("Finished generating Docker Compose configuration for service 'buildarr'")
 
     if volumes:
         compose_obj["volumes"] = list(volumes)
 
-    click.echo(yaml.safe_dump(compose_obj, explicit_start=True, sort_keys=False))
+    click.echo(yaml.safe_dump(compose_obj, explicit_start=True, sort_keys=False), nl=False)
```

### Comparing `buildarr-0.7.1/buildarr/cli/daemon.py` & `buildarr-0.8.0b1/buildarr/cli/daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 `buildarr daemon` CLI command.
 """
 
-
 from __future__ import annotations
 
 import itertools
 import signal
 
 from contextlib import contextmanager
 from datetime import datetime, time
@@ -263,15 +262,15 @@
             logger.info("Buildarr ready.")
 
     def _log_next_run(self) -> None:
         """
         Print a log alerting the user to the next scheduled run time.
         """
         now = datetime.now()
-        for job in sorted(self._scheduler.jobs):
+        for job in sorted(self._scheduler.jobs):  # pragma: no branch
             if not job.next_run or (job.next_run - now).total_seconds() < 0:
                 continue
             logger.info(
                 "The next run will be at %s",
                 job.next_run.strftime("%Y-%m-%d %H:%M"),
             )
             return
@@ -326,37 +325,43 @@
         """
         with self._run_lock():
             try:
                 logger.info("Config file '%s' has been %s", changed_file, action)
                 logger.info("Reloading config")
                 self._initial_run()
                 logger.info("Finished reloading config")
-                self._log_next_run()
             except Exception as err:
                 logger.exception(
                     "Unexpected exception occurred while handling config file event: %s",
                     err,
                 )
+                logger.warning("Aborted reloading config")
             finally:
+                self._log_next_run()
                 logger.info("Buildarr ready.")
 
     def _setup_signal_handlers(self) -> None:
         """
         Setup `SIGINT`, `SIGTERM` and `SIGHUP` signal handers.
 
         SIGHUP can be used to reload the configuration, even if `watch_config` is disabled.
         """
         logger.info("Setting up signal handlers")
         logger.debug("Setting up SIGINT signal handler")
         signal.signal(signal.SIGINT, self._sigterm_handler)
         logger.debug("Setting up SIGTERM signal handler")
         signal.signal(signal.SIGTERM, self._sigterm_handler)
+        if hasattr(signal, "SIGBREAK"):
+            logger.debug("Setting up SIGBREAK signal handler")
+            signal.signal(signal.SIGBREAK, self._sigterm_handler)
+        else:
+            logger.debug("SIGBREAK is not available on this platform")
         if hasattr(signal, "SIGHUP"):
             logger.debug("Setting up SIGHUP signal handler")
-            signal.signal(signal.SIGHUP, self._sighup_handler)  # type: ignore[attr-defined]
+            signal.signal(signal.SIGHUP, self._sighup_handler)
         else:
             logger.debug("SIGHUP is not available on this platform")
         logger.info("Finished setting up signal handlers")
 
     def _stop_handlers(self) -> None:
         """
         Shutdown the config file monitors and clear the automatic update job schedule.
@@ -458,15 +463,15 @@
     """
 
     times: List[time] = []
     for time_str in time_strs:
         try:
             times.append(datetime.strptime(time_str, "%H:%M").time())
         except ValueError:
-            raise click.BadParameter(f"Invalid 24 hour time '{time_str}'") from None
+            raise click.BadParameter(time_str) from None
     return tuple(times)
 
 
 @cli.command(
     help=(
         "Run as a daemon and periodically update defined instances.\n\n"
         "If CONFIG-PATH is not defined, use `buildarr.yml' from the current directory."
@@ -498,16 +503,16 @@
     ),
 )
 @click.option(
     "-d",
     "--update-day",
     "update_days",
     metavar="DAY",
-    type=click.Choice([day.name for day in DayOfWeek], case_sensitive=False),
-    callback=lambda ctx, param, days: tuple(DayOfWeek(day) for day in days),
+    type=click.Choice([day.name.capitalize() for day in DayOfWeek], case_sensitive=False),
+    callback=lambda ctx, param, days: tuple(DayOfWeek.from_name_str(day) for day in days),
     multiple=True,
     help=(
         "Update defined instances on the specified day. "
         "Overrides the `buildarr.update_days' config field. "
         "(can be defined multiple times)"
     ),
 )
```

### Comparing `buildarr-0.7.1/buildarr/cli/exceptions.py` & `buildarr-0.8.0b1/buildarr/cli/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr CLI exceptions.
 """
 
-
 from __future__ import annotations
 
 from ..exceptions import BuildarrError
 
 
 class CLIError(BuildarrError):
     """
@@ -69,14 +68,22 @@
     """
     Exception raised when the hostname configuration for Docker Compose services is invalid.
     """
 
     pass
 
 
+class ComposeInvalidVolumeDefinitionError(ComposeError):
+    """
+    Exception raised when an invalid volume definition is returned by a plugin.
+    """
+
+    pass
+
+
 class ComposeNoPluginsDefinedError(ComposeError):
     """
     Exception raised when no plugin is configured or loaded when
     generating a Docker Compose environment.
     """
 
     pass
```

### Comparing `buildarr-0.7.1/buildarr/cli/main.py` & `buildarr-0.8.0b1/buildarr/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -14,15 +14,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr CLI main routine.
 """
 
-
 from __future__ import annotations
 
 from ..plugins import load as load_plugins
 from ..state import state
 from . import cli as main
 from .compose import compose
 from .daemon import daemon
```

### Comparing `buildarr-0.7.1/buildarr/cli/run.py` & `buildarr-0.8.0b1/buildarr/cli/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 `buildarr run` CLI command.
 """
 
-
 from __future__ import annotations
 
 from logging import getLogger
 from pathlib import Path
 from textwrap import indent
 from typing import Dict, Optional, Set, cast
 
@@ -113,15 +112,15 @@
     """
 
     if not use_plugins:
         use_plugins = set()
 
     # Dump the currently active Buildarr configuration file to the debug log.
     logger.debug("Buildarr configuration:")
-    for config_line in state.config.yaml(exclude_unset=True).splitlines():
+    for config_line in state.config.model_dump_yaml(exclude_unset=True).splitlines():
         logger.debug(indent(config_line, "  "))
 
     # Output the currently loaded plugins to the logs.
     plugin_strs = [f"{pn} ({state.plugins[pn].version})" for pn in sorted(state.plugins.keys())]
     logger.info(
         "Loaded plugins: %s",
         ", ".join(plugin_strs) if plugin_strs else "(no plugins found)",
@@ -235,15 +234,15 @@
             remote_instance_config = manager.from_remote(instance_config, instance_secrets)
             logger.info("Finished fetching remote configuration")
             for config_type, config in (
                 ("Local", instance_config),
                 ("Remote", remote_instance_config),
             ):
                 logger.debug("%s configuration:", config_type)
-                for config_line in config.yaml(exclude_unset=True).splitlines():
+                for config_line in config.model_dump_yaml(exclude_unset=True).splitlines():
                     logger.debug(indent(config_line, "  "))
             logger.info("Updating remote configuration")
             logger.info(
                 (
                     "Remote configuration successfully updated"
                     if manager.update_remote(
                         plugin_name,
@@ -273,15 +272,15 @@
             remote_instance_config = manager.from_remote(instance_config, instance_secrets)
             logger.info("Finished refetching remote configuration")
             for config_type, config in (
                 ("Local", instance_config),
                 ("Remote", remote_instance_config),
             ):
                 logger.debug("%s configuration:", config_type)
-                for config_line in config.yaml(exclude_unset=True).splitlines():
+                for config_line in config.model_dump_yaml(exclude_unset=True).splitlines():
                     logger.debug(indent(config_line, "  "))
             logger.info("Deleting unmanaged/unused resources on the remote instance")
             logger.info(
                 (
                     "Unused resources successfully deleted"
                     if manager.delete_remote(
                         plugin_name,
```

### Comparing `buildarr-0.7.1/buildarr/cli/test_config.py` & `buildarr-0.8.0b1/buildarr/cli/test_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 `buildarr test-config` CLI command.
 """
 
-
 from __future__ import annotations
 
 from logging import getLogger
 from pathlib import Path
 from textwrap import indent
 from typing import TYPE_CHECKING
 
@@ -105,15 +104,15 @@
     try:
         load_config(path=config_path, use_plugins=use_plugins)
     except Exception:
         logger.error("Loading configuration: FAILED")
         raise
     else:
         logger.debug("Buildarr configuration:")
-        for config_line in state.config.yaml(exclude_unset=True).splitlines():
+        for config_line in state.config.model_dump_yaml(exclude_unset=True).splitlines():
             logger.debug(indent(config_line, "  "))
         logger.info("Loading configuration: PASSED")
 
     # Load the manager objects for the selected plugins.
     try:
         load_managers(use_plugins)
     except Exception:
@@ -132,15 +131,17 @@
         logger.error("Loading instance configurations: FAILED")
         raise
     else:
         for plugin_name, instance_configs in state.instance_configs.items():
             for instance_name, instance_config in instance_configs.items():
                 with state._with_context(plugin_name=plugin_name, instance_name=instance_name):
                     logger.debug("Instance configuration:")
-                    for config_line in instance_config.yaml(exclude_unset=True).splitlines():
+                    for config_line in instance_config.model_dump_yaml(
+                        exclude_unset=True,
+                    ).splitlines():
                         logger.debug(indent(config_line, "  "))
         logger.info("Loading instance configurations: PASSED")
 
     # Check if configuration was found for any selected plugins.
     if state.active_plugins:
         logger.debug("Running with plugins: %s", ", ".join(state.active_plugins))
         logger.info("Checking configured plugins: PASSED")
@@ -156,47 +157,62 @@
         raise
     else:
         logger.debug("Execution order:")
         for i, (plugin_name, instance_name) in enumerate(state._execution_order, 1):
             logger.debug("  %i. %s.instances[%s]", i, plugin_name, repr(instance_name))
         logger.info("Resolving instance dependencies: PASSED")
 
-    # Check if any instances are configured to get metadata from TRaSH-Guides.
-    if trash_metadata_used():
-        # Test fetching TRaSH-Guides metadata.
+    # Test fetching TRaSH-Guides metadata, if the configuration uses it.
+    downloaded_trash_metadata = trash_metadata_used()
+    if downloaded_trash_metadata:
         try:
             logger.debug("Fetching TRaSH metadata")
             fetch_trash_metadata()
             logger.debug("Finished fetching TRaSH metadata")
         except Exception:
             logger.error("Fetching TRaSH-Guides metadata: FAILED")
             raise
         else:
             logger.info("Fetching TRaSH-Guides metadata: PASSED")
-        # Test pre-initialisation rendering of the instance configuration.
+    else:
+        logger.info("Fetching TRaSH-Guides metadata: SKIPPED (not required)")
+
+    # Test pre-initialisation rendering of the instance configuration.
+    try:
+        logger.debug("Performing pre-initialisation configuration render")
+        render_instance_configs()
+        logger.debug("Finished performing pre-initialisation configuration render")
+    except Exception:
+        logger.error("Pre-initialisation configuration render: FAILED")
+        raise
+    else:
+        logger.info("Pre-initialisation configuration render: PASSED")
+
+    # Clean up the TRaSH-Guides metadata, now that rendering has completed.
+    if downloaded_trash_metadata:
         try:
-            logger.debug("Performing pre-initialisation configuration render")
-            render_instance_configs()
-            logger.debug("Finished performing pre-initialisation configuration render")
+            logger.debug("Cleaning up TRaSH metadata")
+            cleanup_trash_metadata()
+            logger.debug("Finished cleaning up TRaSH metadata")
         except Exception:
-            logger.error("Pre-initialisation configuration render: FAILED")
+            logger.error("Cleaning up TRaSH-Guides metadata: FAILED")
             raise
         else:
-            logger.info("Pre-initialisation configuration render: PASSED")
-        # Clean up the TRaSH-Guides metadata, now that rendering has completed.
-        cleanup_trash_metadata()
+            logger.info("Cleaning up TRaSH-Guides metadata: PASSED")
     else:
-        logger.info("Fetching TRaSH-Guides metadata: SKIPPED (not required)")
+        logger.info("Cleaning up TRaSH-Guides metadata: SKIPPED (not required)")
 
     # Log the pre-initialisation rendered configuration to debug output.
     for plugin_name, instance_configs in state.instance_configs.items():
         for instance_name, instance_config in instance_configs.items():
             with state._with_context(plugin_name=plugin_name, instance_name=instance_name):
                 if state.managers[plugin_name].uses_trash_metadata(instance_config):
                     logger.debug("Rendered instance configuration:")
-                    for config_line in instance_config.yaml(exclude_unset=True).splitlines():
+                    for config_line in instance_config.model_dump_yaml(
+                        exclude_unset=True,
+                    ).splitlines():
                         logger.debug(indent(config_line, "  "))
 
     # If we get to this point, this configuration is pretty much guaranteed to be valid.
     # Incorrect values for a remote application instance notwithstanding, it should
     # work properly in a real Buildarr run.
     logger.info("Configuration test successful.")
```

### Comparing `buildarr-0.7.1/buildarr/config/__init__.py` & `buildarr-0.8.0b1/buildarr/config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr configuration interface.
 """
 
-
 from __future__ import annotations
 
 from .base import ConfigBase
 from .exceptions import ConfigError, ConfigTrashIDNotFoundError
 from .load import load_config, load_instance_configs
 from .models import ConfigPlugin, ConfigPluginType, ConfigType
 from .post_init_render import post_init_render
```

### Comparing `buildarr-0.7.1/buildarr/config/base.py` & `buildarr-0.8.0b1/buildarr/config/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,21 +12,18 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr configuration base class.
 """
 
-
 from __future__ import annotations
 
-import json
-
 from logging import getLogger
-from pathlib import Path, PurePath, PurePosixPath, PureWindowsPath
+from pathlib import PurePosixPath, PureWindowsPath
 from typing import (
     Any,
     Callable,
     Dict,
     Generic,
     Iterable,
     List,
@@ -39,20 +36,19 @@
     get_args as get_type_args,
     get_origin as get_type_origin,
 )
 from uuid import UUID
 
 import yaml
 
-from pydantic import AnyUrl, BaseModel, NameEmail, SecretStr
-from pydantic.validators import _VALIDATORS
+from pydantic import AnyUrl, BaseModel, NameEmail, SecretStr as PydanticSecretStr
 from typing_extensions import Self
 
 from ..plugins import Secrets
-from ..types import BaseEnum, ModelConfigBase
+from ..types import BaseEnum, model_config_base
 from .types import RemoteMapEntry
 
 logger = getLogger(__name__)
 
 OPTIONAL_TYPE_UNION_SIZE = 2
 
 
@@ -76,17 +72,17 @@
         Args:
             secrets (Secrets): Remote instance host and secrets information.
 
         Returns:
             Remote instance configuration object
         """
         fields: Dict[str, ConfigBase] = {}
-        for field_name, field in cls.__fields__.items():
-            if issubclass(field.type_, ConfigBase):
-                fields[field_name] = field.type_.from_remote(secrets)
+        for field_name, field in cls.model_fields.items():
+            if issubclass(field.annotation, ConfigBase):
+                fields[field_name] = field.annotation.from_remote(secrets)
         return cls(**fields)
 
     @classmethod
     def get_local_attrs(
         cls,
         remote_map: Iterable[RemoteMapEntry],
         remote_attrs: Mapping[str, Any],
@@ -103,46 +99,44 @@
         It parses the inputs and returns a `dict` storing key-value pairs
         of the local equivalents, suitable for being passed as arguments
         to Buildarr configuration class constructors.
 
         ```python
         from __future__ import annotations
 
-        from typing import TYPE_CHECKING, Any, Dict, List, Optional
+        from typing import TYPE_CHECKING, Any, ClassVar, Dict, List, Optional
+
+        from buildarr.config import RemoteMapEntry
         from typing_extensions import Self
-        from buildarr.config import ConfigBase, RemoteMapEntry
+
+        from .types import ExampleConfigBase
 
         if TYPE_CHECKING:
-            from .secrets import ExampleSecrets
-            class ExampleConfigBase(ConfigBase[ExampleSecrets]):
-                ...
-        else:
-            class ExampleConfigBase(ConfigBase):
-                ...
+            from ..secrets import ExampleSecrets
+
 
         class ExampleConfig(ExampleConfigBase):
             local_attr_1: bool
             local_attr_2: Optional[str] = None
 
-            _remote_map: List[RemoteMapEntry] = [
+            _remote_map: ClassVar[List[RemoteMapEntry]] = [
                 ("local_attr_1", "remoteAttr1", {}),
                 (
                     "local_attr_2",
                     "remoteAttr2",
                     {
                         "is_field": True,
                         "decoder": lambda v: v or None,
                         "encoder": lambda v: v or "",
                     },
                 ),
             ]
 
             @classmethod
-            def _api_get(cls, secrets: ExampleSecrets) -> Dict[str, Any]:
-                ...
+            def _api_get(cls, secrets: ExampleSecrets) -> Dict[str, Any]: ...
 
             @classmethod
             def from_remote(cls, secrets: ExampleSecrets) -> Self:
                 return cls(
                     **cls.get_local_attrs(
                         remote_map=cls._remote_map,
                         remote_attrs=cls._api_get(secrets),
@@ -216,29 +210,29 @@
                                         "'value' attribute not included "
                                         f"for remote field '{remote_attr_name}' "
                                         "and 'field_default' not defined in local attribute",
                                     ) from None
                             break
                     else:
                         if attr_metadata.get("optional", False):
-                            local_attrs[attr_name] = cls.__fields__[attr_name].default
+                            local_attrs[attr_name] = cls.model_fields[attr_name].default
                             continue
                         else:
                             raise ValueError(f"Remote field '{remote_attr_name}' not found")
                     # If the local attribute was set to the field default value,
                     # we're done with this attribute. Move onto the next one.
                     if field_default_set:
                         continue
                 # If the remote attribute is a regular key, get the value directly.
                 else:
                     try:
                         remote_attr = remote_attrs[remote_attr_name]
                     except KeyError:
                         if attr_metadata.get("optional", False):
-                            local_attrs[attr_name] = cls.__fields__[attr_name].default
+                            local_attrs[attr_name] = cls.model_fields[attr_name].default
                             continue
                         else:
                             raise
                 # If we got to this point, the remote value has been retrieved.
                 # Decode to get the local value, and add it to the results.
                 local_attrs[attr_name] = decoder(remote_attr)
         # Return a dictionary containing all parsed local attributes.
@@ -294,59 +288,59 @@
         It takes in a list of `RemoteMapEntry` objects determining
         what values should be parsed. The configuration object's values
         are then parsed, returning a `dict` storing key-value pairs
         of the remote equivalents, suitable for being parsed into
         JSON objects to be sent in `POST` requests to the remote server.
 
         ```python
-        from typing import TYPE_CHECKING, Any, List, Mapping, Optional
-        from buildarr.config import ConfigBase, RemoteMapEntry
-        from buildarr.secrets import Secrets
+        from __future__ import annotations
+
+        from typing import TYPE_CHECKING, Any, ClassVar, Dict, List, Mapping, Optional
+
+        from buildarr.config import RemoteMapEntry
+
+        from .types import ExampleConfigBase
 
         if TYPE_CHECKING:
-            from .secrets import ExampleSecrets
-            class ExampleConfigBase(ConfigBase[ExampleSecrets]):
-                ...
-        else:
-            class ExampleConfigBase(ConfigBase):
-                ...
+            from ..secrets import ExampleSecrets
+
 
         class ExampleObj(ExampleConfigBase):
+            local_attr_1: bool
             obj_attr1: int
             obj_attr2: Optional[str] = None
 
-            _remote_map: List[RemoteMapEntry] = [
+            _remote_map: ClassVar[List[RemoteMapEntry]] = [
                 ("obj_attr_1", "objAttr1", {}),
                 (
                     "obj_attr_2",
                     "objAttr2",
                     {
                         "is_field": True,
                         "decoder": lambda v: v or None,
                         "encoder": lambda v: v or "",
                     },
                 ),
             ]
 
             @classmethod
-            def _api_post(cls, secrets: ExampleSecrets, obj: Mapping[str, Any]) -> None:
-                ...
+            def _api_post(cls, secrets: ExampleSecrets, obj: Mapping[str, Any]) -> None: ...
 
-            def _exists_on_remote(self, secrets: ExampleSecrets) -> bool:
-                ...
+            def _exists_on_remote(self, secrets: ExampleSecrets) -> bool: ...
 
             def _create_remote(self, secrets: ExampleSecrets) -> None:
                 self._api_post(
                     secrets,
                     self.get_create_remote_attrs(  # <--- Used here
                         tree=tree,
                         remote_map=self._remote_map,
                     ),
                 )
 
+
         class ExampleConfig(ExampleConfigBase):
             local_objs: Dict[str, ExampleObj]
 
             def update_remote(
                 self,
                 tree: str,
                 secrets: ExampleSecrets,
@@ -393,15 +387,15 @@
                 nonlocal attr_metadata
                 return repr(attr_metadata.get("formatter", self._format_attr)(v))
 
             # Determine whether or not the attribute should be set in
             # the remote attribute dictonary.
             if (
                 attr_metadata.get("set_unmanaged", set_unmanaged)
-                or attr_name in self.__fields_set__
+                or attr_name in self.model_fields_set
             ):
                 set_value = True
                 value = getattr(self, attr_name)
                 if attr_name not in already_logged:
                     logger.info("%s.%s: %s -> (created)", tree, attr_name, formatter(value))
                     already_logged.add(attr_name)
             else:
@@ -456,51 +450,48 @@
 
         * A flag that is `True` if the local and remote configuration are different
         * The updated remote instance attributes as a `dict`
 
         ```python
         from __future__ import annotations
 
-        from typing import TYPE_CHECKING, Any, List, Mapping, Optional
-        from buildarr.config import ConfigBase, RemoteMapEntry
-        from buildarr.secrets import Secrets
+        from typing import TYPE_CHECKING, ClassVar, Any, List, Mapping, Optional
+
+        from buildarr.config import RemoteMapEntry
+
+        from .types import ExampleConfigBase
 
         if TYPE_CHECKING:
-            from .secrets import ExampleSecrets
-            class ExampleConfigBase(ConfigBase[ExampleSecrets]):
-                ...
-        else:
-            class ExampleConfigBase(ConfigBase):
-                ...
+            from ..secrets import ExampleSecrets
+
 
         class ExampleConfig(ExampleConfigBase):
             local_attr_1: bool
             local_attr_2: Optional[str] = None
 
-            _remote_map: List[RemoteMapEntry] = [
+            _remote_map: ClassVar[List[RemoteMapEntry]] = [
                 ("local_attr_1", "remoteAttr1", {}),
                 (
                     "local_attr_2",
                     "remoteAttr2",
                     {
                         "is_field": True,
                         "decoder": lambda v: v or None,
                         "encoder": lambda v: v or "",
                     },
                 ),
             ]
 
             @classmethod
-            def _api_put(cls, secrets: Secrets, obj: Mapping[str, Any]) -> None:
-                ...
+            def _api_put(cls, secrets: ExampleSecrets, obj: Mapping[str, Any]) -> None: ...
 
             def update_remote(
                 self,
                 tree: str,
-                secrets: Secrets,
+                secrets: ExampleSecrets,
                 remote: Self,
                 check_unmanaged: bool = False,
             ) -> bool:
                 changed, remote_attrs = self.get_update_remote_attrs(
                     tree=tree,
                     remote=remote,
                     remote_map=self._remote_map,
@@ -565,15 +556,15 @@
             #
             remote_value = getattr(remote, attr_name)
             # Handle the case where the attribute is managed, either
             # by virtue of it being explicitly set in the Buildarr config,
             # or check_unmanaged is set to True.
             if (
                 attr_metadata.get("check_unmanaged", check_unmanaged)
-                or attr_name in self.__fields_set__
+                or attr_name in self.model_fields_set
             ):
                 local_value = getattr(self, attr_name)
                 # If the local and remote attributes are set to the same
                 # value, unless set_unchanged is set to True, do nothing.
                 if attr_metadata.get("equals", equals)(local_value, remote_value):
                     if attr_name not in already_logged:
                         logger.debug(
@@ -712,17 +703,17 @@
         """
         if isinstance(value, BaseEnum):
             return value.to_name_str()
         elif isinstance(value, AnyUrl):
             return str(value)
         elif isinstance(value, NameEmail):
             return str(value)
-        elif isinstance(value, SecretStr):
+        elif isinstance(value, PydanticSecretStr):
             return str(value)
-        elif isinstance(value, Path):
+        elif isinstance(value, (PureWindowsPath, PurePosixPath)):
             return str(value)
         elif isinstance(value, UUID):
             return str(value)
         elif isinstance(value, list):
             return [cls._format_attr(v) for v in value]
         elif isinstance(value, set):
             return set(cls._format_attr(v) for v in value)
@@ -736,41 +727,45 @@
         Args:
             attr_name (str): Name of attribute to decode
             value (Any): Remote attribute value
 
         Returns:
             Local attribute value
         """
-        return cls._decode_attr_(cls.__fields__[attr_name].outer_type_, value)
+        return cls._decode_attr_(cls.model_fields[attr_name].annotation, value)
 
     @classmethod
     def _decode_attr_(cls, attr_type: Type[Any], value: Any) -> Any:
         type_tree: List[Type[Any]] = [attr_type]
         while get_type_origin(type_tree[-1]) is not None:
             origin_type = get_type_origin(type_tree[-1])
             if origin_type is not None:
                 type_tree.append(origin_type)
         if type_tree[-1] is list:
             return [cls._decode_attr_(get_type_args(type_tree[-2])[0], v) for v in value]
         elif type_tree[-1] is set:
             return set(cls._decode_attr_(get_type_args(type_tree[-2])[0], v) for v in value)
+        elif type_tree[-1] is dict:
+            key_type, value_type = get_type_args(type_tree[-2])
+            return {
+                cls._decode_attr_(key_type, k): cls._decode_attr_(value_type, v)
+                for k, v in value.items()
+            }
         elif type_tree[-1] is Union:
             attr_union_types = get_type_args(type_tree[-2])
             #
             if (
                 len(attr_union_types) == OPTIONAL_TYPE_UNION_SIZE
                 and type(None) in attr_union_types
                 and value is not None
             ):
-                return cls._decode_attr(
+                return cls._decode_attr_(
                     next(t for t in attr_union_types if t is not type(None)),
                     value,
                 )
-        elif issubclass(type_tree[-1], BaseEnum):
-            return type_tree[-1](value)
         return value
 
     @classmethod
     def _encode_attr(cls, value: Any) -> Any:
         """
         Default local-to-remote instance attribute encoding function.
 
@@ -782,82 +777,82 @@
         """
         if isinstance(value, BaseEnum):
             return value.value
         elif isinstance(value, AnyUrl):
             return str(value)
         elif isinstance(value, NameEmail):
             return str(value)
-        elif isinstance(value, SecretStr):
+        elif isinstance(value, PydanticSecretStr):
             return value.get_secret_value()
+        elif isinstance(value, (PurePosixPath, PureWindowsPath)):
+            return str(value)
         elif isinstance(value, UUID):
             return str(value)
         elif isinstance(value, (list, set)):
             return [cls._encode_attr(v) for v in value]
+        elif isinstance(value, dict):
+            return {cls._encode_attr(k): cls._encode_attr(v) for k, v in value.items()}
         return value
 
-    def yaml(
+    def yaml(self, **kwargs) -> str:
+        """
+        Alias to `ConfigBase.model_dump_yaml`.
+
+        Returns:
+            str: YAML representation of the model
+        """
+        return self.model_dump_yaml(**kwargs)
+
+    def model_dump_yaml(
         self,
-        *args,
+        *,
         sort_keys: bool = False,
         yaml_kwargs: Optional[Mapping[str, Any]] = None,
         **kwargs,
     ) -> str:
         """
         Generate a YAML representation of the model.
 
-        Internally this uses the Pydantic JSON generation function, with all arguments
-        forwarded to `BaseModel.json()`. The JSON output is then re-processed using PyYAML.
+        Internally this uses the Pydantic `BaseModel.model_dump` function.
+        With the exception of the two additional options below,
+        all keyword arguments are forwarded to that function call.
 
         Args:
             sort_keys (bool, optional): Sort keys in the output YAML file. Defaults to `False`.
             yaml_kwargs (Optional[Mapping[str, Any]], optional): YAML encoder keyword args.
 
         Returns:
             YAML representation of the model
         """
         return yaml.safe_dump(  # type: ignore[call-overload]
-            json.loads(self.json(*args, **kwargs)),
+            self.model_dump(mode="json", **kwargs),
             **{**(yaml_kwargs or {}), "sort_keys": sort_keys},
         )
 
-    class Config(ModelConfigBase):
-        """
-        Buildarr configuration model class settings.
-
-        Sets some required parameters for serialisation,
-        parsing and validation to work correctly.
+    model_config = model_config_base
+    """
+    Buildarr configuration model configuration.
 
-        To set additional parameters in your implementing class, subclass this class:
+    Sets some required parameters for parsing and validation to work correctly.
 
-        ```python
-        from __future__ import annotations
+    To set additional parameters in your implementing class, override this attribute:
 
-        from typing import TYPE_CHECKING
-        from buildarr.config import ConfigBase
+    ```python
+    from __future__ import annotations
 
-        if TYPE_CHECKING:
-            from .secrets import ExampleSecrets
-            class _ExampleConfig(ConfigBase[ExampleSecrets]):
-                ...
-        else:
-            class _ExampleConfig(ConfigBase):
-                ...
+    from typing import TYPE_CHECKING
 
-        class ExampleConfig(_ExampleConfig):
-            ...
+    from buildarr.config import ConfigBase
 
-            class Config(_ExampleConfig.Config):
-                ...  # Add model configuration attributes here.
-        ```
-        """
+    if TYPE_CHECKING:
+        from .secrets import ExampleSecrets
 
-        pass
 
+    class ExampleConfigBase(ConfigBase["ExampleSecrets"]):
+        ...
 
-# Add custom validators which are not provided by Pydantic.
-_VALIDATORS.extend(
-    [
-        (PurePath, [lambda v: PurePath(v)]),
-        (PurePosixPath, [lambda v: PurePosixPath(v)]),
-        (PureWindowsPath, [lambda v: PureWindowsPath(v)]),
-    ],
-)
+        model_config = {
+            **ConfigBase.model_config,
+            ...  # Add model configuration attributes here.
+        }
+    ```
+    """
```

### Comparing `buildarr-0.7.1/buildarr/config/buildarr.py` & `buildarr-0.8.0b1/buildarr/config/buildarr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,22 +12,21 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr settings configuration.
 """
 
-
 from __future__ import annotations
 
 import os
 
 from datetime import time
 from pathlib import Path
-from typing import Set
+from typing import Optional, Set
 
 from pydantic import AnyHttpUrl, PositiveFloat
 
 from ..types import DayOfWeek, NonEmptyStr
 from .base import ConfigBase
 
 
@@ -44,21 +43,21 @@
 
     ```yaml
     ---
 
     buildarr:
       watch_config: true
       update_days:
-        - "monday"
-        - "tuesday"
-        - "wednesday"
-        - "thursday"
-        - "friday"
-        - "saturday"
-        - "sunday"
+        - "Monday"
+        - "Tuesday"
+        - "Wednesday"
+        - "Thursday"
+        - "Friday"
+        - "Saturday"
+        - "Sunday"
       update_times:
         - "03:00"
     ```
     """
 
     watch_config: bool = False
     """
@@ -96,17 +95,14 @@
     The times Buildarr daemon will run update operations on each scheduled day.
 
     By default, updates are scheduled to run at 3:00am local time.
 
     Times are specified in the `HH:MM` format, in 24-hour time.
     The times do not need to be in order.
 
-    Days are specified as a list of case-insensitive strings, in English.
-    The days do not need to be in order.
-
     ```yaml
     buildarr:
       update_times:
         - "06:00"
         - "12:00"
         - "18:00"
         - "00:00"
@@ -120,27 +116,30 @@
     The timeout for any API requests Buildarr makes (in seconds).
 
     If the timeout is reached, an error will occur and Buildarr will stop the update process.
 
     *New in version 0.3.0.*
     """
 
-    trash_metadata_download_url: AnyHttpUrl = (
-        "https://github.com/TRaSH-/Guides/archive/refs/heads/master.zip"  # type: ignore[assignment]
+    trash_metadata_download_url: AnyHttpUrl = AnyHttpUrl(
+        "https://github.com/TRaSH-/Guides/archive/refs/heads/master.zip"
     )
     """
     URL to download the latest TRaSH-Guides metadata from.
     """
 
-    trash_metadata_dir_prefix: Path = "Guides-master"  # type: ignore[assignment]
+    trash_metadata_dir_prefix: Optional[Path] = Path("Guides-master")
     """
     Metadata directory name within the downloaded ZIP file.
+
+    *Changed in version 0.8.0*: Now can be set to `null` if the metadata directories
+    are located in the root of the ZIP file.
     """
 
-    docker_image_uri: NonEmptyStr = os.environ.get(  # type: ignore[assignment]
+    docker_image_uri: NonEmptyStr = os.environ.get(
         "BUILDARR_DOCKER_IMAGE_URI",
         "callum027/buildarr",
     )
     """
     Default image URI to use for the Buildarr service when generating Docker Compose files.
 
     If undefined in the configuration file, use the value defined in the
```

### Comparing `buildarr-0.7.1/buildarr/config/exceptions.py` & `buildarr-0.8.0b1/buildarr/config/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr config exception classes.
 """
 
-
 from __future__ import annotations
 
 from ..exceptions import BuildarrError
 
 
 class ConfigError(BuildarrError):
     """
```

### Comparing `buildarr-0.7.1/buildarr/config/load.py` & `buildarr-0.8.0b1/buildarr/config/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr configuration loading function.
 """
 
-
 from __future__ import annotations
 
 from logging import getLogger
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Type,
@@ -65,17 +64,17 @@
 
     logger.debug("Building configuration model")
     model = cast(
         Type[ConfigType],
         create_model(  # type: ignore[call-overload]
             "Config",
             __base__=ConfigBase,
-            buildarr=BuildarrConfig(),
+            buildarr=(BuildarrConfig, BuildarrConfig()),
             **{
-                plugin_name: plugin.config()
+                plugin_name: (plugin.config, plugin.config())
                 for plugin_name, plugin in state.plugins.items()
                 if not use_plugins or plugin_name in use_plugins
             },
         ),
     )
     logger.debug("Finished building configuration model")
 
@@ -235,18 +234,18 @@
             )
             for dict_key, dict_value in value.items()
         }
     if _is_subclass(type_tree[-1], ConfigBase):
         return {
             key: _expand_relative_paths(
                 config_dir=config_dir,
-                value_type=field.outer_type_,
+                value_type=field.annotation,
                 value=value[key],
             )
-            for key, field in type_tree[-1].__fields__.items()
+            for key, field in type_tree[-1].model_fields.items()
             if key in value
         }
     return value
 
 
 def _get_type_tree(type_obj: Type[Any]) -> List[Type[Any]]:
     # Generate the full type tree of a type hint, or actual type.
@@ -268,43 +267,43 @@
 
 
 def load_instance_configs(use_plugins: Optional[Set[str]] = None) -> None:
     """
     Parse fully-qualified configuration for each instance under each selected plugin.
 
     This will also cause the `state._instance_dependencies` dependency tree structure
-    to be populated through validation of any `InstanceName` attributes present
+    to be populated through any `InstanceReference` annotations present
     in each instance-specific configuration.
 
     Args:
         use_plugins (Optional[Set[str]]): Plugins to use. Default is to use all plugins.
     """
 
     configs: Dict[str, Dict[str, ConfigPlugin]] = {}
     active_plugins: Set[str] = set()
 
     for plugin_name in state.plugins.keys():
         if use_plugins and plugin_name not in use_plugins:
             continue
-        if plugin_name not in state.config.__fields_set__:
+        if plugin_name not in state.config.model_fields_set:
             continue
         plugin_manager = state.managers[plugin_name]
         plugin_config: ConfigPluginType = getattr(state.config, plugin_name)
         active_plugins.add(plugin_name)
         configs[plugin_name] = {}
         for instance_name in (
             plugin_config.instances.keys() if plugin_config.instances else ["default"]
         ):
             # Load the instance-specific configuration under aninstance-specific context,
             # so that when the configuration gets evaluated by the parser,
-            # `InstanceName` references are properly validated and dependencies get added
-            # to `state._instance_dependencies`.
+            # `InstanceReference` annotations are properly validated, and
+            # dependencies get added to `state._instance_dependencies`.
             with state._with_context(plugin_name=plugin_name, instance_name=instance_name):
                 instance_config = plugin_manager.get_instance_config(
                     plugin_config,
                     instance_name,
                 )
                 configs[plugin_name][instance_name] = instance_config
 
     # Update global application state with the fully qualified instance configurations.
     state.instance_configs = configs
-    state.active_plugins = frozenset(active_plugins)
+    state.active_plugins = tuple(sorted(active_plugins))
```

### Comparing `buildarr-0.7.1/buildarr/config/models.py` & `buildarr-0.8.0b1/buildarr/config/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,20 +12,19 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr plugin configuration object models.
 """
 
-
 from __future__ import annotations
 
-from typing import Any, Dict, Type, cast
+from typing import Any, Dict, Optional, Type, cast, get_args as get_type_args
 
-from pydantic import root_validator
+from pydantic import field_validator, model_validator
 from typing_extensions import Self
 
 from ..plugins import Secrets
 from ..types import NonEmptyStr, Port
 from ..util import merge_dicts
 from .base import ConfigBase
 from .buildarr import BuildarrConfig
@@ -42,34 +41,33 @@
     Note that the `instances` attribute is not directly defined by `ConfigPlugin`,
     but it MUST be defined on the implementing class.
 
     ```python
     from __future__ import annotations
 
     from typing import TYPE_CHECKING, Literal
-    from buildarr.config import ConfigPlugin, NonEmptyStr, Port
+
+    from buildarr.config import ConfigPlugin
+    from buildarr.types import NonEmptyStr, Port
 
     if TYPE_CHECKING:
         from .secrets import ExampleSecrets
-        class _ExampleInstanceConfig(ConfigPlugin[ExampleSecrets]):
-            ...
-    else:
-        class _ExampleInstanceConfig(ConfigPlugin):
-            ...
 
-    class ExampleInstanceConfig(_ExampleInstanceConfig):
+
+    class ExampleInstanceConfig(ConfigPlugin["ExampleSecrets"]):
         # Required configuration overrides from `ConfigPlugin`
         hostname: NonEmptyStr = "example"
         port: Port = 1234
         protocol: Literal["http", "https"] = "http"
 
         # Custom configuration options go here
         local_value_1: bool = False
         local_value_2: str = "local"
 
+
     class ExampleConfig(ExampleInstanceConfig):
         # Inherit all configuration attributes from the instance-specific config.
         # This is the class to specify in the plugin's `Plugin` interface definition.
 
         # Required `instances` definition
         instances: Dict[str, ExampleInstanceConfig] = {}
     ```
@@ -113,22 +111,46 @@
     protocol: NonEmptyStr
     """
     Remote instance communication protocol.
 
     Implementing configuration classes should override this with a default value.
     """
 
+    url_base: Optional[str] = None
+    """
+    The URL path the remote instance API is available under, if behind a reverse proxy.
+
+    API URLs are rendered like this: `<protocol>://<hostname>:<port><url_base>/...`
+
+    When unset, the URL root will be used as the API endpoint
+    (e.g. `<protocol>://<hostname>:<port>/...`).
+    """
+
     # `instances` is not defined here, but it MUST be defined on the implementing class.
 
+    @field_validator("url_base")
+    def validate_url_base(cls, value: Optional[str]) -> Optional[str]:
+        """
+        Process the defined `url_base` value, and make sure the value in the secrets objects
+        is consistently formatted.
+
+        Args:
+            value (Optional[str]): `url_base` value.
+
+        Returns:
+            Validated value
+        """
+        return f"/{value.strip('/')}" if value and value.strip("/") else None
+
     @property
     def host_url(self) -> str:
         """
         Fully qualified URL for the instance.
         """
-        return f"{self.protocol}://{self.hostname}:{self.port}"
+        return f"{self.protocol}://{self.hostname}:{self.port}{self.url_base or ''}"
 
     def uses_trash_metadata(self) -> bool:
         """
         Return whether or not this instance configuration uses TRaSH-Guides metadata.
 
         Configuration plugins should implement this function if TRaSH-Guides metadata is used.
 
@@ -141,15 +163,15 @@
     def has_instance_configs(self) -> bool:
         """
         Whether or not this plugin has instance-specific configurations defined.
 
         This property should not need to be overloaded in most cases.
         """
         return bool(
-            "instances" in self.__fields_set__ and self.instances,  # type: ignore[attr-defined]
+            "instances" in self.model_fields_set and self.instances,  # type: ignore[attr-defined]
         )
 
     def get_instance_config(self, instance_name: str) -> Self:
         """
         Combine explicitly defined instance-local and global configuration,
         and return a fully qualified instance-specific plugin configuration object.
 
@@ -157,30 +179,34 @@
 
         Args:
             instance_name (str): Name of the instance to get the configuration of.
 
         Returns:
             Fully qualified instance-specific configuration object
         """
-        instance_config_class: Type[Self] = self.__fields__["instances"].type_
+        instance_config_class: Type[Self] = get_type_args(
+            self.model_fields["instances"].annotation,
+        )[1]
         if instance_name == "default":
-            return instance_config_class(**self.dict(exclude={"instances"}, exclude_unset=True))
+            return instance_config_class(
+                **self.model_dump(exclude={"instances"}, exclude_unset=True),
+            )
         return instance_config_class(
             **merge_dicts(
                 # Merge attribute values in order of priority (lowest to highest).
                 #
                 # Lowest priority are global configuration attribute defaults,
                 # which are defined in the class attributes.
                 #
                 # Next are instance-specific configuration attribute defaults.
                 {"hostname": instance_name},
                 # Explicitly defined global configuration attributes.
-                self.dict(exclude=set(["instances"]), exclude_unset=True),
+                self.model_dump(exclude=set(["instances"]), exclude_unset=True),
                 # Explicitly defined instance-specific attributes.
-                self.instances[instance_name].dict(  # type: ignore[attr-defined]
+                self.instances[instance_name].model_dump(  # type: ignore[attr-defined]
                     exclude=set(["instances"]),
                     exclude_unset=True,
                 ),
             ),
         )
 
     def render(self) -> Self:
@@ -274,40 +300,33 @@
             service_name (str): The unique name for the generated Docker Compose service.
 
         Returns:
             Docker Compose service definition dictionary
         """
         raise NotImplementedError()
 
-    @root_validator
-    def _set_default_hostname(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+    @model_validator(mode="after")
+    def _set_default_hostname(self) -> Self:
         """
         Set the default value for `hostname` on instance-specific configurations.
-
-        The `instances` value on the global (default instance) configuration is left alone.
-
-        Args:
-            values (Dict[str, Any]): Input values for all local fields
-
-        Returns:
-            Dict[str, Any]: Changed field structure
         """
-        if "instances" in values:
+        if hasattr(self, "instances"):
             for instance_name, instance in cast(
                 Dict[str, ConfigPlugin],
-                values["instances"],
+                self.instances,
             ).items():
                 if instance_name == "default":
                     raise ValueError(
-                        "instance name 'default' is reserved within Buildarr, "
+                        "there is an instance named 'default' defined for this plugin, "
+                        "the instance name 'default' is reserved within Buildarr, "
                         "please choose a different name for this instance",
                     )
-                if "hostname" not in instance.__fields_set__:
-                    instance.hostname = instance_name  # type: ignore[assignment]
-        return values
+                if "hostname" not in instance.model_fields_set:
+                    instance.hostname = instance_name
+        return self
 
 
 class ConfigPluginType(ConfigPlugin):
     """
     Basic type hint containing the attributes and functions Buildarr
     (and plugins referring to other plugins) should use to interface
     with a global plugin configuration.
```

### Comparing `buildarr-0.7.1/buildarr/config/post_init_render.py` & `buildarr-0.8.0b1/buildarr/config/post_init_render.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Post-initialisation configuration rendering stage.
 """
 
-
 from __future__ import annotations
 
 from collections import defaultdict
 from logging import getLogger
 from typing import TYPE_CHECKING
 
 from ..state import state
```

### Comparing `buildarr-0.7.1/buildarr/config/render_instance_configs.py` & `buildarr-0.8.0b1/buildarr/config/render_instance_configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr configuration rendering function.
 """
 
-
 from __future__ import annotations
 
 from collections import defaultdict
 from logging import getLogger
 from typing import TYPE_CHECKING
 
 from ..state import state
```

### Comparing `buildarr-0.7.1/buildarr/config/resolve_instance_dependencies.py` & `buildarr-0.8.0b1/buildarr/config/resolve_instance_dependencies.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr configuration instance-to-instance dependency resolution functions.
 """
 
-
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from ..state import state
 
 if TYPE_CHECKING:
@@ -41,19 +40,16 @@
     is performed, which is generated using instance name references defined within
     Buildarr instance configurations.
     """
 
     added_plugin_instances: Set[PluginInstanceRef] = set()
     execution_order: List[PluginInstanceRef] = []
 
-    for plugin_name, instance_configs in state.instance_configs.items():
-        for instance_name in instance_configs.keys():
-            instance = (plugin_name, instance_name)
-            if instance in added_plugin_instances:
-                continue
+    for plugin_name in state.active_plugins:
+        for instance_name in sorted(state.instance_configs[plugin_name].keys()):
             _resolve_instance_dependencies(
                 added_plugin_instances=added_plugin_instances,
                 execution_order=execution_order,
                 plugin_name=plugin_name,
                 instance_name=instance_name,
             )
 
@@ -84,15 +80,18 @@
     """
 
     if not dependency_tree:
         dependency_tree = []
 
     plugin_instance: PluginInstanceRef = (plugin_name, instance_name)
 
-    if plugin_name not in state.instance_configs:
+    # NOTE: Due to similar checks being run in the instance configuration loading
+    # stage in the `InstanceReference` annotation, in practice the checks within this block
+    # will never actually be used. They are still defined here as well, just in case.
+    if plugin_name not in state.instance_configs:  # pragma: no cover
         error_message = 'Unable to resolve instance dependency "'
         try:
             previous_pi = dependency_tree[-1]
             error_message += f"{previous_pi[0]}.instances[{previous_pi[1]!r}] -> "
         except IndexError:
             # Shouldn't happen because dependency keys are generated from
             # instance configuration, but handle it just in case.
@@ -112,15 +111,15 @@
                     f"  {i}. {pname}.instances[{iname!r}]"
                     for i, (pname, iname) in enumerate([*dependency_tree, plugin_instance], 1)
                 )
             ),
         )
 
     if plugin_instance in state._instance_dependencies:
-        for target_plugin_instance in state._instance_dependencies[plugin_instance]:
+        for target_plugin_instance in sorted(state._instance_dependencies[plugin_instance]):
             if target_plugin_instance not in added_plugin_instances:
                 target_plugin, target_instance = target_plugin_instance
                 _resolve_instance_dependencies(
                     added_plugin_instances=added_plugin_instances,
                     execution_order=execution_order,
                     plugin_name=target_plugin,
                     instance_name=target_instance,
```

### Comparing `buildarr-0.7.1/buildarr/config/types.py` & `buildarr-0.8.0b1/buildarr/config/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Type hints for Buildarr configuration models.
 """
 
-
 from __future__ import annotations
 
 from typing import Any, Mapping, Tuple
 
 RemoteMapEntry = Tuple[str, str, Mapping[str, Any]]
 """
 Helper type hint for defining parameters for the `remote_map` argument
@@ -33,30 +32,26 @@
 
 * `local_attr` (`str`) - the local attribute name
 * `remote_attr` (`str`) - the remote attribute name
 * `params` (`Mapping[str, Any]`) - option parameters that define how to convert
    between local and remote attributes (for more details, check the handling function)
 
 ```python
-from typing import TYPE_CHECKING, Any, Dict, List, Optional
-from buildarr.config import ConfigBase, RemoteMapEntry
+from typing import ClassVar, List, Optional
+
+from buildarr.config import RemoteMapEntry
+
+from .types import ExampleConfigBase
 
-if TYPE_CHECKING:
-    from .secrets import ExampleSecrets
-    class ExampleConfigBase(ConfigBase[ExampleSecrets]):
-        ...
-else:
-    class ExampleConfigBase(ConfigBase):
-        ...
 
 class ExampleConfig(ExampleConfigBase):
     local_attr_1: bool
     local_attr_2: Optional[str] = None
 
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("local_attr_1", "remoteAttr1", {}),
         (
             "local_attr_2",
             "remoteAttr2",
             {
                 "is_field": True,
                 "decoder": lambda v: v or None,
```

### Comparing `buildarr-0.7.1/buildarr/exceptions.py` & `buildarr-0.8.0b1/buildarr/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr exception classes.
 """
 
-
 from __future__ import annotations
 
 
 class BuildarrError(Exception):
     """
     Buildarr exception base class.
     """
```

### Comparing `buildarr-0.7.1/buildarr/logging.py` & `buildarr-0.8.0b1/buildarr/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr logging functions.
 """
 
-
 from __future__ import annotations
 
 import logging
 
 from pathlib import Path
 from sys import argv, stderr, stdout
```

### Comparing `buildarr-0.7.1/buildarr/manager/__init__.py` & `buildarr-0.8.0b1/buildarr/manager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr manager interface.
 """
 
-
 from __future__ import annotations
 
 from logging import getLogger
 from typing import TYPE_CHECKING, Generic
 
 from ..plugins import Config, Secrets
 from ..state import state
@@ -45,18 +44,22 @@
 
     `ManagerPlugin` is a generic interface, so to create the manager class
     for your plugin, create a class with `ManagerPlugin` as the superclass,
     with the configuration and secrets classes for your plugin passed into
     the appropriate type parameters.
 
     ```python
+    from __future__ import annotations
+
     from buildarr.manager import ManagerPlugin
+
     from .config import ExampleConfig
     from .secrets import ExampleSecrets
 
+
     class ExampleManager(ManagerPlugin[ExampleConfig, ExampleSecrets]):
         pass
     ```
 
     If your plugin has distinct classes for global configuration and
     instance-specific configuration (e.g. `ExampleConfig` and `ExampleInstanceConfig`),
     pass `ExampleInstanceConfig` to `ExampleManager`.
@@ -253,15 +256,15 @@
     """
 
     managers: Dict[str, ManagerPlugin] = {}
 
     for plugin_name, plugin in state.plugins.items():
         if use_plugins and plugin_name not in use_plugins:
             continue
-        if plugin_name not in state.config.__fields_set__:
+        if plugin_name not in state.config.model_fields_set:
             continue
         with state._with_context(plugin_name=plugin_name):
             logger.debug("Loading plugin manager")
             managers[plugin_name] = plugin.manager()
             logger.debug("Finished loading plugin manager")
 
     state.managers = managers
```

### Comparing `buildarr-0.7.1/buildarr/manager/exceptions.py` & `buildarr-0.8.0b1/buildarr/manager/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr manager exception classes.
 """
 
-
 from __future__ import annotations
 
 from ..exceptions import BuildarrError
 
 
 class ManagerError(BuildarrError):
     """
```

### Comparing `buildarr-0.7.1/buildarr/plugins/__init__.py` & `buildarr-0.8.0b1/buildarr/plugins/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr plugin specification.
 """
 
-
 from __future__ import annotations
 
 from .load import load
 from .models import Plugin
 from .types import Config, Secrets
 
 __all__ = ["Plugin", "Config", "Secrets", "load"]
```

### Comparing `buildarr-0.7.1/buildarr/plugins/dummy/api.py` & `buildarr-0.8.0b1/buildarr/plugins/dummy2/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,250 +1,232 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with Buildarr.
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
-Dummy plugin API functions.
+Dummy2 plugin API functions.
 """
 
-
 from __future__ import annotations
 
 import json
 
 from http import HTTPStatus
 from logging import getLogger
 from typing import TYPE_CHECKING
 
 import requests
 
 from buildarr.state import state
 
-from .exceptions import DummyAPIError
+from .exceptions import Dummy2APIError
 
 if TYPE_CHECKING:
     from typing import Any, Optional, Union
 
-    from .secrets import DummySecrets
+    from .secrets import Dummy2Secrets
 
 
 logger = getLogger(__name__)
 
 
 def api_get(
-    secrets: Union[DummySecrets, str],
+    secrets: Union[Dummy2Secrets, str],
     api_url: str,
-    session: Optional[requests.Session] = None,
-    use_api_key: bool = True,
+    *,
     expected_status_code: HTTPStatus = HTTPStatus.OK,
+    session: Optional[requests.Session] = None,
 ) -> Any:
     """
-    Send a `GET` request to a Dummy instance.
+    Send an API `GET` request.
 
     Args:
-        secrets (Union[DummySecrets, str]): Dummy secrets metadata, or host URL.
-        api_url (str): Dummy API command.
+        secrets (Union[Dummy2Secrets, str]): Secrets metadata, or host URL.
+        api_url (str): API command.
         expected_status_code (HTTPStatus): Expected response status. Defaults to `200 OK`.
 
     Returns:
         Response object
     """
 
-    if isinstance(secrets, str):
-        host_url = secrets
-        api_key = None
-    else:
-        host_url = secrets.host_url
-        api_key = secrets.api_key.get_secret_value() if use_api_key else None
+    host_url = secrets if isinstance(secrets, str) else secrets.host_url
+
     url = f"{host_url}/{api_url.lstrip('/')}"
 
     logger.debug("GET %s", url)
 
     if not session:
         session = requests.Session()
-    res = session.get(
-        url,
-        headers={"X-Api-Key": api_key} if api_key else None,
-        timeout=state.request_timeout,
-    )
-    res_json = res.json()
+    res = session.get(url, timeout=state.request_timeout)
+    try:
+        res_json = res.json()
+    except requests.JSONDecodeError:
+        api_error(method="GET", url=url, response=res)
 
     logger.debug("GET %s -> status_code=%i res=%s", url, res.status_code, repr(res_json))
 
     if res.status_code != expected_status_code:
         api_error(method="GET", url=url, response=res)
 
     return res_json
 
 
 def api_post(
-    secrets: Union[DummySecrets, str],
+    secrets: Union[Dummy2Secrets, str],
     api_url: str,
-    req: Any = None,
+    req: Any,
+    *,
     session: Optional[requests.Session] = None,
-    use_api_key: bool = True,
     expected_status_code: HTTPStatus = HTTPStatus.CREATED,
 ) -> Any:
     """
-    Send a `POST` request to a Dummy instance.
+    Send a `POST` request to a Sonarr instance.
 
     Args:
-        secrets (Union[DummySecrets, str]): Dummy secrets metadata, or host URL.
-        api_url (str): Dummy API command.
+        secrets (Union[Dummy2Secrets, str]): Secrets metadata, or host URL.
+        api_url (str): API command.
         req (Any): Request (JSON-serialisable).
         expected_status_code (HTTPStatus): Expected response status. Defaults to `201 Created`.
 
     Returns:
         Response object
     """
 
-    if isinstance(secrets, str):
-        host_url = secrets
-        api_key = None
-    else:
-        host_url = secrets.host_url
-        api_key = secrets.api_key.get_secret_value() if use_api_key else None
+    host_url = secrets if isinstance(secrets, str) else secrets.host_url
+
     url = f"{host_url}/{api_url.lstrip('/')}"
 
     logger.debug("POST %s <- req=%s", url, repr(req))
 
     if not session:
         session = requests.Session()
     res = session.post(
         url,
-        headers={"X-Api-Key": api_key} if api_key else None,
         timeout=state.request_timeout,
         **({"json": req} if req is not None else {}),
     )
-    res_json = res.json()
+    try:
+        res_json = res.json()
+    except requests.JSONDecodeError:
+        api_error(method="POST", url=url, response=res)
 
     logger.debug("POST %s -> status_code=%i res=%s", url, res.status_code, repr(res_json))
 
     if res.status_code != expected_status_code:
         api_error(method="POST", url=url, response=res)
 
     return res_json
 
 
 def api_put(
-    secrets: Union[DummySecrets, str],
+    secrets: Union[Dummy2Secrets, str],
     api_url: str,
     req: Any,
+    *,
     session: Optional[requests.Session] = None,
-    use_api_key: bool = True,
-    expected_status_code: HTTPStatus = HTTPStatus.OK,
+    expected_status_code: HTTPStatus = HTTPStatus.ACCEPTED,
 ) -> Any:
     """
-    Send a `PUT` request to a Dummy instance.
+    Send a `PUT` request to a Sonarr instance.
 
     Args:
-        secrets (Union[DummySecrets, str]): Dummy secrets metadata, or host URL.
-        api_url (str): Dummy API command.
+        secrets (Union[Dummy2Secrets, str]): Secrets metadata, or host URL.
+        api_url (str): API command.
         req (Any): Request (JSON-serialisable).
         expected_status_code (HTTPStatus): Expected response status. Defaults to `200 OK`.
 
     Returns:
         Response object
     """
 
-    if isinstance(secrets, str):
-        host_url = secrets
-        api_key = None
-    else:
-        host_url = secrets.host_url
-        api_key = secrets.api_key.get_secret_value() if use_api_key else None
+    host_url = secrets if isinstance(secrets, str) else secrets.host_url
+
     url = f"{host_url}/{api_url.lstrip('/')}"
 
     logger.debug("PUT %s <- req=%s", url, repr(req))
 
     if not session:
         session = requests.Session()
     res = session.put(
         url,
-        headers={"X-Api-Key": api_key} if api_key else None,
         json=req,
         timeout=state.request_timeout,
     )
-    res_json = res.json()
+    try:
+        res_json = res.json()
+    except requests.JSONDecodeError:
+        api_error(method="PUT", url=url, response=res)
 
     logger.debug("PUT %s -> status_code=%i res=%s", url, res.status_code, repr(res_json))
 
     if res.status_code != expected_status_code:
         api_error(method="PUT", url=url, response=res)
 
     return res_json
 
 
 def api_delete(
-    secrets: Union[DummySecrets, str],
+    secrets: Union[Dummy2Secrets, str],
     api_url: str,
+    *,
     session: Optional[requests.Session] = None,
-    use_api_key: bool = True,
     expected_status_code: HTTPStatus = HTTPStatus.OK,
 ) -> None:
     """
-    Send a `DELETE` request to a Dummy instance.
+    Send a `DELETE` request to a Sonarr instance.
 
     Args:
-        secrets (Union[DummySecrets, str]): Dummy secrets metadata, or host URL.
-        api_url (str): Dummy API command.
+        secrets (Union[Dummy2Secrets, str]): Secrets metadata, or host URL.
+        api_url (str): API command.
         expected_status_code (HTTPStatus): Expected response status. Defaults to `200 OK`.
     """
 
-    if isinstance(secrets, str):
-        host_url = secrets
-        api_key = None
-    else:
-        host_url = secrets.host_url
-        api_key = secrets.api_key.get_secret_value() if use_api_key else None
+    host_url = secrets if isinstance(secrets, str) else secrets.host_url
+
     url = f"{host_url}/{api_url.lstrip('/')}"
 
     logger.debug("DELETE %s", url)
 
     if not session:
         session = requests.Session()
-    res = session.delete(
-        url,
-        headers={"X-Api-Key": api_key} if api_key else None,
-        timeout=state.request_timeout,
-    )
+    res = session.delete(url, timeout=state.request_timeout)
 
     logger.debug("DELETE %s -> status_code=%i", url, res.status_code)
 
     if res.status_code != expected_status_code:
         api_error(method="DELETE", url=url, response=res, parse_response=False)
 
 
 def api_error(
     method: str,
     url: str,
     response: requests.Response,
     parse_response: bool = True,
 ) -> None:
     """
-    Process an error response from the Dummy API.
+    Process an error response from the Dummy2 API.
 
     Args:
         method (str): HTTP method.
         url (str): API command URL.
         response (requests.Response): Response metadata.
         parse_response (bool, optional): Parse response error JSON. Defaults to True.
 
     Raises:
-        Dummy API exception
+        Dummy2 API exception
     """
 
     error_message = (
         f"Unexpected response with status code {response.status_code} from from '{method} {url}'"
     )
 
     if parse_response:
@@ -257,11 +239,11 @@
                 try:
                     error_message += res_json["message"]
                 except KeyError:
                     try:
                         error_message += res_json["error"]
                     except KeyError:
                         error_message += f"(Unsupported error JSON format) {res_json}"
-        except json.JSONDecodeError:
+        except (json.JSONDecodeError, requests.exceptions.JSONDecodeError):
             f"(Non-JSON error response)\n{response.text}"
 
-    raise DummyAPIError(error_message, status_code=response.status_code)
+    raise Dummy2APIError(error_message, status_code=response.status_code)
```

### Comparing `buildarr-0.7.1/buildarr/plugins/dummy/cli.py` & `buildarr-0.8.0b1/buildarr/plugins/dummy/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,29 +12,31 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Dummy plugin CLI commands.
 """
 
-
 from __future__ import annotations
 
 import functools
 
 from getpass import getpass
+from typing import TYPE_CHECKING
 from urllib.parse import urlparse
 
 import click
-import click_params  # type: ignore[import]
 
 from .config import DummyInstanceConfig
 from .manager import DummyManager
 from .secrets import DummySecrets
 
+if TYPE_CHECKING:
+    from urllib.parse import ParseResult as Url
+
 HOSTNAME_PORT_TUPLE_LENGTH = 2
 
 
 @click.group(help="Dummy instance ad-hoc commands.")
 def dummy():
     """
     Dummy instance ad-hoc commands.
@@ -45,52 +47,63 @@
 
 @dummy.command(
     help=(
         "Dump configuration from a remote Dummy instance.\n\n"
         "The configuration is dumped to standard output in Buildarr-compatible YAML format."
     ),
 )
-@click.argument("url", type=click_params.URL)
+@click.argument("url", type=urlparse)
 @click.option(
     "-k",
     "--api-key",
     "api_key",
     metavar="API-KEY",
-    default=functools.partial(getpass, "Dummy instance API key: "),
+    default=functools.partial(
+        getpass,
+        "Dummy instance API key (or leave blank to auto-fetch): ",
+    ),
     help="API key of the Dummy instance. The user will be prompted if undefined.",
 )
-def dump_config(url: str, api_key: str) -> int:
+def dump_config(url: Url, api_key: str) -> int:
     """
     Dump configuration from a remote Dummy instance.
     The configuration is dumped to standard output in Buildarr-compatible YAML format.
     """
 
-    # Parse the specified instance URL to get its constituent components.
-    url_obj = urlparse(url)
-    protocol = url_obj.scheme
-    hostname_port = url_obj.netloc.split(":", 1)
+    protocol = url.scheme
+    hostname_port = url.netloc.split(":", 1)
     hostname = hostname_port[0]
     port = (
         int(hostname_port[1])
         if len(hostname_port) == HOSTNAME_PORT_TUPLE_LENGTH
         else (443 if protocol == "https" else 80)
     )
+    url_base = url.path
 
-    # Create a default configuration object for the Dummy instance,
-    # storing the connection information.
-    dummy_config = DummyInstanceConfig(hostname=hostname, port=port, protocol=protocol)
-
-    # Generate the secrets metadata for the Dummy instance.
-    dummy_secrets = DummySecrets(
-        hostname=hostname,
-        port=port,
-        protocol=protocol,
-        api_key=api_key,
+    instance_config = DummyInstanceConfig(
+        **{  # type: ignore[arg-type]
+            "hostname": hostname,
+            "port": port,
+            "protocol": protocol,
+            "url_base": url_base,
+        },
     )
 
-    # Pull the remote Dummy instance configuration, and create the configuration object.
-    dummy_config = DummyManager().from_remote(instance_config=dummy_config, secrets=dummy_secrets)
-
-    # Serialise the Dummy instance configuration into YAML, and write it to standard output.
-    click.echo(dummy_config.yaml())
+    click.echo(
+        (
+            DummyManager()
+            .from_remote(
+                instance_config=instance_config,
+                secrets=DummySecrets.get_from_url(
+                    hostname=hostname,
+                    port=port,
+                    protocol=protocol,
+                    url_base=url_base,
+                    api_key=api_key if api_key else None,
+                ),
+            )
+            .model_dump_yaml(exclude_unset=True)
+        ),
+        nl=False,
+    )
 
     return 0
```

### Comparing `buildarr-0.7.1/buildarr/plugins/dummy/config/__init__.py` & `buildarr-0.8.0b1/buildarr/plugins/dummy2/config/settings.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,206 +1,167 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with Buildarr.
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
-Dummy plugin configuration.
+Dummy2 plugin settings configuration.
 """
 
-
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Dict, Optional
-
-from typing_extensions import Self
-
-from buildarr.config import ConfigPlugin
-from buildarr.types import NonEmptyStr, Port
-
-from ..api import api_get
-from ..secrets import DummySecrets
-from ..types import DummyApiKey, DummyProtocol
-from .settings import DummySettingsConfig
-
-# Allow Mypy to properly resolve secrets type declarations in configuration classes.
-if TYPE_CHECKING:
+from typing import ClassVar, List, Optional, cast
+from uuid import UUID, uuid4
 
-    class _DummyInstanceConfig(ConfigPlugin[DummySecrets]):
-        ...
+from pydantic import Field
+from typing_extensions import Annotated, Self
 
-else:
+from buildarr.config import RemoteMapEntry
+from buildarr.state import state
+from buildarr.types import InstanceReference
 
-    class _DummyInstanceConfig(ConfigPlugin):
-        ...
+from ..api import api_get, api_post
+from ..secrets import Dummy2Secrets
+from .types import Dummy2ConfigBase
 
 
-class DummyInstanceConfig(_DummyInstanceConfig):
+class Dummy2SettingsConfig(Dummy2ConfigBase):
     """
-    By default, Buildarr will look for a single instance at `http://dummy:5000`.
-    Most configurations are different, and to accommodate those, you can configure
-    how Buildarr connects to individual Dummy instances.
+    Dummy2 settings configuration.
 
-    Configuration of a single Dummy instance:
+    Specify any of the following attributes to ensure the attribute
+    on the remote Dummy2 instance is set accordingly.
 
     ```yaml
-    dummy:
-      hostname: "localhost"
-      port: 5000
-      protocol: "http"
+    dummy2:
       settings:
-        ...
+        trash_value: 5
     ```
 
-    Configuration of multiple instances:
+    Specify `trash_id` to get a value from TRaSH-Guides metadata and set it to `trash_value`.
 
     ```yaml
-    dummy:
-      # Configuration and settings common to all instances.
-      hostname: "localhost"
-      protocol: "http"
+    dummy2:
       settings:
-        ...
-      instances:
-        # Dummy instance 1-specific configuration.
-        dummy1:
-          port: 5000
-          settings:
-            ...
-        # Dummy instance 2-specific configuration.
-        dummy:
-          port: 5001
-          api_key: "..." # Explicitly define API key
-          settings:
-            ...
+        trash_id: "387e6278d8e06083d813358762e0ac63" # anime
     ```
     """
 
-    hostname: NonEmptyStr = "dummy"  # type: ignore[assignment]
+    instance_name: Annotated[Optional[str], InstanceReference(plugin_name="dummy")] = None
     """
-    Hostname of the Dummy instance to connect to.
-
-    When defining a single instance using the global `dummy` configuration block,
-    the default hostname is `dummy`.
-
-    When using multiple instance-specific configurations, the default hostname
-    is the name given to the instance in the `instances` attribute.
-
-    ```yaml
-    dummy:
-      instances:
-        dummy1: # <--- This becomes the default hostname
-          ...
-    ```
+    The name of the Dummy instance within Buildarr, if linking this Dummy2 instance
+    with a Buildarr-defined Dummy instance.
     """
 
-    port: Port = 5000  # type: ignore[assignment]
-    """
-    Port number of the Dummy instance to connect to.
+    instance_value: Optional[UUID] = Field(default_factory=uuid4)
     """
+    Instance-specific UUID generated by Buildarr, which is unique on each execution
+    (unless explicitly defined within the Buildarr configuration).
 
-    protocol: DummyProtocol = "http"  # type: ignore[assignment]
+    If `instance_name` is defined, this value will instead be read from the target instance.
     """
-    Communication protocol to use to connect to Dummy.
-
-    Values:
 
-    * `http`
+    nonexistent_plugin_instance: Annotated[
+        Optional[str],
+        InstanceReference(plugin_name="dummy3"),
+    ] = None
     """
+    The name of an instance that belongs to a non-existent plugin.
 
-    api_key: Optional[DummyApiKey] = None
+    Used for validating instance dependency error checking within the functional tests.
     """
-    API key to use to authenticate with the Dummy instance.
 
-    If undefined or set to `None`, automatically retrieve the API key.
-    This can only be done on Dummy instances with authentication disabled.
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
+        (
+            "instance_value",  # Buildarr config attribute name.
+            "instanceValue",  # Dummy2 instance API attribute name.
+            {"check_unmanaged": True},  # Local/remote map conversion function parameters.
+        ),
+    ]
     """
+    A list of remote map entries containing metadata for how to convert
+    between local and remote Dummy2 instance configuration values.
 
-    version: Optional[str] = None
-    """
-    The expected version of the Dummy instance.
-    If undefined or set to `None`, the version is auto-detected.
+    For more information on how to create this structure,
+    see the documentation for the following methods in `buildarr/config/__init__.py`:
 
-    At the moment this attribute is unused, and there is likely no need to explicitly set it.
+    * `ConfigBase.get_local_attrs`
+    * `ConfigBase.get_create_remote_attrs`
+    * `ConfigBase.get_update_remote_attrs`
     """
 
-    settings: DummySettingsConfig = DummySettingsConfig()
-    """
-    Dummy settings.
-    Configuration options for Dummy itself are set within this structure.
-    """
-
-    def uses_trash_metadata(self) -> bool:
+    def _resolve(self) -> Self:
         """
-        Return whether or not this instance configuration uses TRaSH-Guides metadata.
+        Resolve any instance references in this configuration, and
+        return an object with fully qualified attribute values.
 
         Returns:
-            `True` if TRaSH-Guides metadata is used, otherwise `False`
-        """
-        return self.settings.uses_trash_metadata()
-
-    def render(self) -> Self:
+            Fully qualified Dummy2 configuration object
         """
-        Render dynamic configuration attributes, and return the resulting configuration object.
-
-        Returns:
-            Rendered configuration object
-        """
-        if not self.settings.uses_trash_metadata():
+        if not self.instance_name:
             return self
-        copy = self.copy(deep=True)
-        copy._render()
-        return copy
-
-    def _render(self) -> None:
-        """
-        Render dynamic configuration attributes in place.
-        """
-        self.settings._render()
+        secrets = cast(Dummy2Secrets, state.instance_secrets["dummy2"][self.instance_name])
+        return self.model_copy(
+            update={
+                "instance_name": self.instance_name,
+                "instance_value": api_get(secrets, "/api/v1/settings")["instanceValue"],
+            },
+        )
 
     @classmethod
-    def from_remote(cls, secrets: DummySecrets) -> Self:
+    def from_remote(cls, secrets: Dummy2Secrets) -> Self:
         """
         Read configuration from a remote instance and return it as a configuration object.
 
         Args:
-            secrets (DummySecrets): Instance host and secrets information
+            secrets (Dummy2Secrets): Instance host and secrets information
 
         Returns:
             Configuration object for remote instance
         """
         return cls(
-            hostname=secrets.hostname,
-            port=secrets.port,
-            protocol=secrets.protocol,
-            api_key=secrets.api_key,
-            version=api_get(secrets, "/api/v1/status")["version"],
-            settings=DummySettingsConfig.from_remote(secrets),
+            trash_id=None,
+            **cls.get_local_attrs(
+                remote_map=cls._remote_map,
+                remote_attrs=api_get(secrets, "/api/v1/settings"),
+            ),
         )
 
+    def update_remote(
+        self,
+        tree: str,
+        secrets: Dummy2Secrets,
+        remote: Self,
+        check_unmanaged: bool = False,
+    ) -> bool:
+        """
+        Compare this configuration to a remote instance's, and update the remote to match.
 
-class DummyConfig(DummyInstanceConfig):
-    """
-    Dummy plugin global configuration class.
-
-    Subclasses the instance-specific configuration to allow
-    attributes common to all instances to be defined in one place.
-    """
-
-    instances: Dict[str, DummyInstanceConfig] = {}
-    """
-    Instance-specific Dummy configuration.
-
-    Can only be defined on the global `dummy` configuration block.
+        Args:
+            tree (str): Configuration tree represented as a string. Mainly used in logging.
+            secrets (Dummy2Secrets): Remote instance host and secrets information.
+            remote (Self): Remote instance configuration for the current section.
+            check_unmanaged (bool, optional): Set unmanaged fields to defaults (default `False`).
 
-    Globally specified configuration values apply to all instances.
-    Configuration values specified on an instance-level take precedence at runtime.
-    """
+        Returns:
+            `True` if the remote configuration changed, otherwise `False`
+        """
+        changed, remote_attrs = self._resolve().get_update_remote_attrs(
+            tree=tree,
+            remote=remote,
+            remote_map=self._remote_map,
+            check_unmanaged=check_unmanaged,
+            set_unchanged=True,
+        )
+        if changed:
+            api_post(secrets, "/api/v1/settings", remote_attrs)
+            return True
+        return False
```

### Comparing `buildarr-0.7.1/buildarr/plugins/dummy/config/settings.py` & `buildarr-0.8.0b1/buildarr/plugins/dummy/config/settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,28 +12,27 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Dummy plugin settings configuration.
 """
 
-
 from __future__ import annotations
 
 import json
 
-from typing import Any, List, Mapping, Optional, Union, cast
+from typing import Any, ClassVar, List, Mapping, Optional, Union, cast
 from uuid import UUID, uuid4
 
 from pydantic import Field
-from typing_extensions import Self
+from typing_extensions import Annotated, Self
 
 from buildarr.config import ConfigTrashIDNotFoundError, RemoteMapEntry
 from buildarr.state import state
-from buildarr.types import InstanceName, TrashID
+from buildarr.types import InstanceReference, TrashID
 
 from ..api import api_get, api_post
 from ..secrets import DummySecrets
 from .types import DummyConfigBase
 
 
 class DummySettingsConfig(DummyConfigBase):
@@ -54,47 +53,59 @@
     ```yaml
     dummy:
       settings:
         trash_id: "387e6278d8e06083d813358762e0ac63" # anime
     ```
     """
 
-    instance_name: Optional[InstanceName] = Field(None, plugin="dummy")
+    instance_name: Annotated[Optional[str], InstanceReference(plugin_name="dummy")] = None
     """
     The name of the Dummy instance within Buildarr, if linking this Dummy instance
     with another Buildarr-defined Dummy instance.
     """
 
-    trash_id: Optional[TrashID] = None  # type: ignore[assignment]
+    trash_id: Optional[TrashID] = None
     """
     TRaSH-Guides Sonarr quality definition profile ID to use when filling out `trash_value`.
     """
 
     trash_value: Union[float, None] = None
     """
     Value retrieved from the TRaSH-Guides repository.
 
     If this value is explicitly specified in the configuration, it does not get overwritten.
     """
 
+    trash_value_2: Union[float, None] = None
+    """
+    Another value retrieved from the TRaSH-Guides repository.
+
+    If this value is explicitly specified in the configuration, it does not get overwritten.
+    """
+
     instance_value: Optional[UUID] = Field(default_factory=uuid4)
     """
     Instance-specific UUID generated by Buildarr, which is unique on each execution
     (unless explicitly defined within the Buildarr configuration).
 
     If `instance_name` is defined, this value will instead be read from the target instance.
     """
 
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         (
             "trash_value",  # Buildarr config attribute name.
             "trashValue",  # Dummy instance API attribute name.
             {},  # Local/remote map conversion function parameters.
         ),
         (
+            "trash_value_2",  # Buildarr config attribute name.
+            "trashValue2",  # Dummy instance API attribute name.
+            {},  # Local/remote map conversion function parameters.
+        ),
+        (
             "instance_value",  # Buildarr config attribute name.
             "instanceValue",  # Dummy instance API attribute name.
             {"check_unmanaged": True},  # Local/remote map conversion function parameters.
         ),
     ]
     """
     A list of remote map entries containing metadata for how to convert
@@ -118,21 +129,23 @@
         return bool(self.trash_id)
 
     def _render(self) -> None:
         """
         Render dynamic configuration attributes in place.
 
         Specifically, this function reads a value from the TRaSH-Guides metadata
-        and populates the `trash_value` attribute with it.
+        and populates the `trash_value` attribute with it (if not already defined).
 
         Set `trash_value` to the minimum data rate value for the
         `Bluray-1080p` quality definition in the profile.
         """
         if not self.trash_id:
             return
+        if self.trash_value:
+            return
         for quality_file in (
             state.trash_metadata_dir / "docs" / "json" / "sonarr" / "quality-size"
         ).iterdir():
             with quality_file.open() as f:
                 quality_json: Mapping[str, Any] = json.load(f)
                 if cast(str, quality_json["trash_id"]).lower() == self.trash_id:
                     for definition_json in quality_json["qualities"]:
@@ -145,26 +158,60 @@
                         )
                     break
         else:
             raise ConfigTrashIDNotFoundError(
                 f"Unable to find Sonarr quality definition file with trash ID '{self.trash_id}'",
             )
 
+    def _post_init_render(self) -> None:
+        """
+        Post-init render dynamic configuration attributes in place.
+
+        Specifically, this function reads a value from the TRaSH-Guides metadata
+        and populates the `trash_value_2` attribute with it (if not already defined).
+
+        Set `trash_value` to the minimum data rate value for the
+        `Bluray-2160p` quality definition in the profile.
+        """
+        if not self.trash_id:
+            return
+        if self.trash_value_2:
+            return
+        for quality_file in (
+            state.trash_metadata_dir / "docs" / "json" / "sonarr" / "quality-size"
+        ).iterdir():
+            with quality_file.open() as f:
+                quality_json: Mapping[str, Any] = json.load(f)
+                if cast(str, quality_json["trash_id"]).lower() == self.trash_id:
+                    for definition_json in quality_json["qualities"]:
+                        if definition_json["quality"] == "Bluray-2160p":
+                            self.trash_value_2 = cast(float, definition_json["min"])
+                            break
+                    else:
+                        raise ValueError(
+                            "Quality definition 'Bluray-1080p' not found in TRaSH-Guides profile",
+                        )
+                    break
+        else:
+            raise ConfigTrashIDNotFoundError(
+                f"Unable to find Sonarr quality definition file with trash ID '{self.trash_id}'",
+            )
+
     def _resolve(self) -> Self:
         """
         Resolve any instance references in this configuration, and
         return an object with fully qualified attribute values.
 
         Returns:
             Fully qualified Dummy configuration object
         """
         if not self.instance_name:
             return self
         secrets = cast(DummySecrets, state.instance_secrets["dummy"][self.instance_name])
-        return self.copy(
+        return self.model_copy(
             update={
                 "instance_name": self.instance_name,
                 "instance_value": api_get(secrets, "/api/v1/settings")["instanceValue"],
             },
         )
 
     @classmethod
```

### Comparing `buildarr-0.7.1/buildarr/plugins/dummy/config/types.py` & `buildarr-0.8.0b1/buildarr/plugins/dummy2/manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,28 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with Buildarr.
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
-Dummy plugin configuration utility classes and functions.
+Dummy2 plugin manager class.
 """
 
-
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
-
-from buildarr.config import ConfigBase
-
-# Define the base class for Dummy configuration classes.
-# Subclassing this conditionally-created class allows Mypy to
-# properly resolve secrets type declarations.
-if TYPE_CHECKING:
-    from ..secrets import DummySecrets
+from buildarr.manager import ManagerPlugin
 
-    class DummyConfigBase(ConfigBase[DummySecrets]):
-        pass
+from .config import Dummy2InstanceConfig
+from .secrets import Dummy2Secrets
 
-else:
 
-    class DummyConfigBase(ConfigBase):
-        pass
+class Dummy2Manager(ManagerPlugin[Dummy2InstanceConfig, Dummy2Secrets]):
+    pass
```

### Comparing `buildarr-0.7.1/buildarr/plugins/dummy/exceptions.py` & `buildarr-0.8.0b1/buildarr/plugins/dummy/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Dummy plugin exception classes.
 """
 
-
 from __future__ import annotations
 
 from buildarr.exceptions import BuildarrError
 
 
 class DummyError(BuildarrError):
     """
```

### Comparing `buildarr-0.7.1/buildarr/plugins/dummy/manager.py` & `buildarr-0.8.0b1/buildarr/plugins/dummy/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Dummy plugin manager class.
 """
 
-
 from __future__ import annotations
 
 from buildarr.manager import ManagerPlugin
 
 from .config import DummyInstanceConfig
 from .secrets import DummySecrets
```

### Comparing `buildarr-0.7.1/buildarr/plugins/dummy/plugin.py` & `buildarr-0.8.0b1/buildarr/plugins/dummy/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Dummy plugin interface.
 """
 
-
 from __future__ import annotations
 
 from buildarr import __version__
 from buildarr.plugins import Plugin
 
 from .cli import dummy
 from .config import DummyConfig
```

### Comparing `buildarr-0.7.1/buildarr/plugins/dummy/secrets.py` & `buildarr-0.8.0b1/buildarr/plugins/dummy2/secrets.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,135 +1,178 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with Buildarr.
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
-Dummy plugin secrets file model.
+Dummy2 plugin secrets file model.
 """
 
-
 from __future__ import annotations
 
 from http import HTTPStatus
-from typing import TYPE_CHECKING
-from urllib.parse import urlparse
+from typing import TYPE_CHECKING, Optional
+
+from pydantic import field_validator
 
 from buildarr.secrets import SecretsPlugin
 from buildarr.types import NonEmptyStr, Port
 
 from .api import api_get
-from .exceptions import DummyAPIError, DummySecretsUnauthorizedError
-from .types import DummyApiKey, DummyProtocol
+from .exceptions import Dummy2APIError
+from .types import Dummy2Protocol
 
 # Allow Mypy to properly resolve configuration type declarations in secrets classes.
 if TYPE_CHECKING:
     from typing_extensions import Self
 
-    from .config import DummyConfig
+    from .config import Dummy2Config
 
-    class _DummySecrets(SecretsPlugin[DummyConfig]):
+    class _Dummy2Secrets(SecretsPlugin[Dummy2Config]):
         pass
 
 else:
 
-    class _DummySecrets(SecretsPlugin):
+    class _Dummy2Secrets(SecretsPlugin):
         pass
 
 
-class DummySecrets(_DummySecrets):
+class Dummy2Secrets(_Dummy2Secrets):
     """
-    Dummy API secrets.
+    Dummy2 API secrets.
     """
 
     hostname: NonEmptyStr
     port: Port
-    protocol: DummyProtocol
-
-    api_key: DummyApiKey
+    protocol: Dummy2Protocol
+    url_base: Optional[str]
+    version: NonEmptyStr
 
     @property
     def host_url(self) -> str:
         """
         Full host URL for the Dummy instance.
         """
-        return f"{self.protocol}://{self.hostname}:{self.port}"
+        return self._get_host_url(
+            protocol=self.protocol,
+            hostname=self.hostname,
+            port=self.port,
+            url_base=self.url_base,
+        )
+
+    @field_validator("url_base")
+    def validate_url_base(cls, value: Optional[str]) -> Optional[str]:
+        """
+        Process the defined `url_base` value, and make sure the value in the secrets objects
+        is consistently formatted.
+
+        Args:
+            value (Optional[str]): `url_base` value.
+
+        Returns:
+            Validated value
+        """
+        return f"/{value.strip('/')}" if value and value.strip("/") else None
+
+    @classmethod
+    def _get_host_url(
+        cls,
+        protocol: str,
+        hostname: str,
+        port: int,
+        url_base: Optional[str],
+    ) -> str:
+        """
+        Helper method to create a fully-qualified host URL.
+
+        Args:
+            hostname (str): Instance hostname.
+            port (int): Instance access port.
+            protocol (str): Instance access protocol.
+            url_base (Optional[str], optional): Instance URL base.
+
+        Returns:
+            Full host URL
+        """
+        return f"{protocol}://{hostname}:{port}{cls.validate_url_base(url_base) or ''}"
 
     @classmethod
-    def from_url(cls, host_url: str, api_key: str) -> Self:
+    def get(cls, config: Dummy2Config) -> Self:
         """
-        Generate a secrets object from its constituent host URL and API key.
+        Generate a secrets object from the given instance configuration,
+        retrieving any necessary secrets in the process.
 
         Args:
-            host_url (str): Full host URL of the instance
-            api_key (str): API key used to authenticate with the instance
+            config (DummyConfig): Instance configuration.
 
         Returns:
             Secrets object
         """
-        url_obj = urlparse(host_url)
-        hostname_port = url_obj.netloc.rsplit(":", 1)
-        hostname = hostname_port[0]
-        protocol = url_obj.scheme
-        port = (
-            int(hostname_port[1])
-            if len(hostname_port) > 1
-            else (443 if protocol == "https" else 80)
+        return cls.get_from_url(
+            hostname=config.hostname,
+            port=config.port,
+            protocol=config.protocol,
+            url_base=config.url_base,
         )
-        return cls(hostname=hostname, port=port, protocol=protocol, api_key=api_key)
 
     @classmethod
-    def get(cls, config: DummyConfig) -> Self:
+    def get_from_url(
+        cls,
+        hostname: str,
+        port: int,
+        protocol: str,
+        url_base: Optional[str] = None,
+    ) -> Self:
         """
-        Generate a secrets object from the given instance configuration,
+        Generate a secrets object from the given instance access details,
         retrieving any necessary secrets in the process.
 
         Args:
-            config (DummyConfig): Instance configuration
+            hostname (str): Instance hostname.
+            port (int): Instance access port.
+            protocol (str): Instance access protocol.
+            url_base (Optional[str], optional): Instance URL base. Default is `None`.
 
         Returns:
             Secrets object
         """
-        try:
-            return cls(
-                hostname=config.hostname,
-                port=config.port,
-                protocol=config.protocol,
-                api_key=(
-                    config.api_key
-                    if config.api_key
-                    else api_get(config.host_url, "/initialize.json")["apiKey"]
-                ),
-            )
-        except DummyAPIError as err:
-            if err.status_code == HTTPStatus.UNAUTHORIZED:
-                raise DummySecretsUnauthorizedError(
-                    "Unable to retrieve the API key for the Dummy instance "
-                    f"at '{config.host_url}': Authentication is enabled",
-                ) from None
-            else:
-                raise
+        url_base = cls.validate_url_base(url_base)
+        host_url = cls._get_host_url(
+            protocol=protocol,
+            hostname=hostname,
+            port=port,
+            url_base=url_base,
+        )
+        initialize_json = api_get(host_url, "/initialize.json")
+        return cls(
+            hostname=hostname,
+            port=port,
+            protocol=protocol,
+            url_base=url_base,
+            version=initialize_json["version"],
+        )
 
     def test(self) -> bool:
         """
         Test whether or not the secrets metadata is valid for connecting to the instance.
 
         Returns:
             `True` if the test was successful, otherwise `False`
         """
         try:
-            api_get(self, "/api/v1/settings")
-            return True
-        except DummyAPIError as err:
+            api_get(self.host_url, "/api/v1/status")
+        except Dummy2APIError as err:
             if err.status_code == HTTPStatus.UNAUTHORIZED:
                 return False
             else:
                 raise
+        else:
+            return True
```

### Comparing `buildarr-0.7.1/buildarr/plugins/dummy/server.py` & `buildarr-0.8.0b1/buildarr/plugins/dummy/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -25,43 +25,99 @@
 
 This file is not required when creating a new plugin.
 
 This is simply for convenience when testing, to give the Dummy plugin something
 to communicate with for testing purposes.
 """
 
-
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Mapping, cast
 
 from flask import Flask, Response, jsonify, request
-from werkzeug.exceptions import Unauthorized
+from werkzeug.exceptions import InternalServerError, NotFound, Unauthorized
 
 from buildarr import __version__
 
 if TYPE_CHECKING:
     from typing import Any, Dict, Tuple
 
 
 __all__ = ["app"]
 
 app = Flask("buildarr-dummy-server")
 
 app.config.from_prefixed_env(prefix="BUILDARR_DUMMY")
 if "API_ROOT" not in app.config:
     app.config["API_ROOT"] = "/api/v1"
+if "API_FORCE_AUTH" not in app.config:
+    app.config["API_FORCE_AUTH"] = False
+if "API_SUPPORTS_INIT" not in app.config:
+    app.config["API_SUPPORTS_INIT"] = False
+if "API_REQUIRES_INIT" not in app.config:
+    app.config["API_REQUIRES_INIT"] = False
+
+_is_initialized: bool = not app.config["API_REQUIRES_INIT"]
 
 _settings: Dict[str, Any] = {
     "isUpdated": False,  # bool
     "trashValue": None,  # Optional[float]
+    "trashValue2": None,  # Optional[float]
     "instanceValue": None,  # Optional[str] (UUID)
 }
 
 
+@app.errorhandler(401)
+def unauthorized(error: Unauthorized) -> Tuple[Response, int]:
+    """
+    Handle a `401 Unauthorized` error.
+
+    Args:
+        error (Unauthorized): Unauthorized exception object
+
+    Returns:
+        Error responses
+    """
+
+    return (jsonify({"message": "Unauthorized", "description": error.description}), 401)
+
+
+@app.errorhandler(404)
+def not_found(error: NotFound) -> Tuple[Response, int]:
+    """
+    Handle a `404 Not Found` error.
+
+    Args:
+        error (NotFound): Not found exception object
+
+    Returns:
+        Error responses
+    """
+
+    return (jsonify({"message": "Not Found", "description": error.description}), 404)
+
+
+@app.errorhandler(500)
+def internal_server_error(error: NotFound) -> Tuple[Response, int]:
+    """
+    Handle a `500 Internal Server Error` error.
+
+    Args:
+        error (InternalServerError): Internal server error exception object
+
+    Returns:
+        Error responses
+    """
+
+    return (
+        jsonify({"message": "Internal Server Error", "description": error.description}),
+        500,
+    )
+
+
 def check_api_key() -> None:
     """
     Check if a valid API key was supplied in the request headers.
 
     If invalid or not specified when required, raise an error to make
     Flask return a `401 Unauthorized` response.
     """
@@ -72,27 +128,23 @@
     if "X-Api-Key" not in request.headers:
         raise Unauthorized(description="API key required but not provided")
 
     if request.headers["X-Api-Key"] != app.config["API_KEY"]:
         raise Unauthorized(description="Incorrect API key")
 
 
-@app.errorhandler(401)
-def unauthorized(error: Unauthorized) -> Tuple[Response, int]:
+def check_initialised() -> None:
     """
-    Handle a `401 Unauthorized` error.
+    Check if the Dummy server has been initialised.
 
-    Args:
-        error (Unauthorized): Unauthorized exception object
-
-    Returns:
-        Error responses
+    If not, return a 500 Internal Server Error.
     """
 
-    return (jsonify({"message": "Unauthorized", "description": error.description}), 401)
+    if app.config["API_SUPPORTS_INIT"] and not _is_initialized:
+        raise InternalServerError()
 
 
 @app.get("/initialize.json")
 def get_initialize_json() -> Tuple[Response, int]:
     """
     Return the Dummy API access metadata.
 
@@ -102,21 +154,58 @@
     ```
 
     Returns:
         Dummy API access metadata
     """
 
     res = {"apiRoot": app.config["API_ROOT"]}
-    if "API_KEY" in app.config and app.config["API_KEY"]:
-        res["apiKey"] = app.config["API_KEY"]
-    res["version"] = __version__
+
+    if app.config.get("API_SUPPORTS_INIT"):
+        res["initialized"] = _is_initialized
+
+    if _is_initialized:
+        if app.config["API_FORCE_AUTH"]:
+            check_api_key()
+        if app.config.get("API_KEY"):
+            res["apiKey"] = app.config["API_KEY"]
+        res["version"] = __version__
 
     return (jsonify(res), 200)
 
 
+@app.post(f"{app.config['API_ROOT']}/init")
+def init() -> Tuple[Response, int]:
+    """
+    Initialise the Dummy server.
+
+    If successful, the 200 OK status code will be set,
+    and the previous initialized status will be returned in the response.
+
+     ```bash
+    $ curl http://localhost:5000/api/v1/init
+    {"initialized":false}
+    ```
+
+    If initialisation is configured to not be supported, return a 404 Not Found error.
+
+    Returns:
+        Dummy server status
+    """
+
+    global _is_initialized  # noqa: PLW0603
+
+    if not app.config.get("API_SUPPORTS_INIT"):
+        raise NotFound()
+
+    _old_is_initialized = _is_initialized
+    _is_initialized = True
+
+    return (jsonify({"initialized": _old_is_initialized}), 200)
+
+
 @app.get(f"{app.config['API_ROOT']}/status")
 def get_status() -> Tuple[Response, int]:
     """
     Return the Dummy server current status.
 
      ```bash
     $ curl -H "X-Api-Key: 1a2b3c4d5e" http://localhost:5000/api/v1/status
@@ -124,14 +213,15 @@
     ```
 
     Returns:
         Dummy server status
     """
 
     check_api_key()
+    check_initialised()
 
     return (jsonify({"version": __version__}), 200)
 
 
 @app.get(f"{app.config['API_ROOT']}/settings")
 def get_settings() -> Tuple[Response, int]:
     """
@@ -143,14 +233,15 @@
     ```
 
     Returns:
         Current Dummy server settings
     """
 
     check_api_key()
+    check_initialised()
 
     return (jsonify(_settings), 200)
 
 
 @app.route(f"{app.config['API_ROOT']}/settings", methods=["POST", "PUT"])
 def update_settings() -> Tuple[Response, int]:
     """
@@ -176,17 +267,18 @@
 
     Updated settings will be lost when the server shuts down.
 
     Returns:
         Old Dummy server settings
     """
 
-    global _settings  # noqa: PLW0603 RUF100
+    global _settings  # noqa: PLW0603
 
     check_api_key()
+    check_initialised()
 
     old_settings = _settings
     _settings = merge_dicts(old_settings, cast(Mapping, request.json), {"isUpdated": True})
     return (jsonify(old_settings), 201)
 
 
 def merge_dicts(*dicts: Mapping[Any, Any]) -> Dict[Any, Any]:
```

### Comparing `buildarr-0.7.1/buildarr/plugins/dummy/types.py` & `buildarr-0.8.0b1/buildarr/plugins/dummy/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,35 +12,35 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Dummy plugin type hints.
 """
 
-
 from __future__ import annotations
 
 from typing import Literal
 
 from buildarr.types import Password
 
 DummyApiKey = Password
 """
 Constrained string type for a Dummy instance API key.
 
 The type `Password` allows anything as long as it is not an empty string, but is a subclass
-of type `pydantic.SecretStr`, allowing Buildarr to hide the value in any logging.
+of the Buildarr type `SecretStr`, allowing Buildarr to hide the value in any logging.
 
 A more complex type for API key might look something like this:
 
 ```python
-from pydantic import Field, SecretStr
+from buildarr.types import SecretStr
+from pydantic import StringConstraints
 from typing_extensions import Annotated
 
-DummyApiKey = Annotated[SecretStr, Field(min_length=32, max_length=32)]
+DummyApiKey = Annotated[SecretStr, StringConstraints(min_length=32, max_length=32)]
 ```
 """
 
 DummyProtocol = Literal["http"]
 """
 Allowed protocols for communicating with a Dummy instance.
 """
```

### Comparing `buildarr-0.7.1/buildarr/plugins/load.py` & `buildarr-0.8.0b1/buildarr/plugins/load.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,21 +12,20 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr plugin loading functions.
 """
 
-
 from __future__ import annotations
 
 from logging import getLogger
 from typing import TYPE_CHECKING
 
-from stevedore.extension import ExtensionManager  # type: ignore[import]
+from stevedore.extension import ExtensionManager
 
 from ..state import state
 
 if TYPE_CHECKING:
     from typing import Dict
 
     from importlib_metadata import EntryPoint
@@ -48,29 +47,28 @@
     plugins: Dict[str, Plugin] = {}
 
     for plugin in ExtensionManager(
         namespace=namespace,
         invoke_on_load=True,
         on_load_failure_callback=_on_plugin_failure,
     ):
-        # Do not load the built-in `buildarr-dummy` plugin
+        # Do not load the built-in dummy plugins
         # if Buildarr was not started in testing mode.
-        if not state.testing and plugin.name == "dummy":
+        if not state.testing and plugin.name in ("dummy", "dummy2"):
             continue
-        if plugin.name not in plugins:
+        if plugin.name not in plugins:  # pragma: no branch
             plugins[plugin.name] = plugin.entry_point.load()
 
     state.plugins = plugins
 
 
-def _on_plugin_failure(manager: ExtensionManager, entrypoint: EntryPoint, err: Exception) -> None:
+def _on_plugin_failure(manager: ExtensionManager, entry_point: EntryPoint, err: Exception) -> None:
     """
     Plugin load error handler.
 
     Args:
         manager (ExtensionManager): Extension manager used to load the plugin
-        entrypoint (EntryPoint): Entry point metadata of the plugin
+        entry_point (EntryPoint): Entry point metadata of the plugin
         err (Exception): Exception raised during loading
     """
 
-    logger.error("An error occured while loading plugin '%s':", entrypoint.name)
-    logger.exception(err)
+    logger.exception("An error occurred while loading plugin '%s': %s", entry_point.name, err)
```

### Comparing `buildarr-0.7.1/buildarr/plugins/models.py` & `buildarr-0.8.0b1/buildarr/plugins/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr plugin models.
 """
 
-
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Optional, Type
 
@@ -35,59 +34,37 @@
     """
     Buildarr plugin definition.
 
     To create a Buildarr plugin, set the appropriate
     plugin classes as class attributes to an implementation of this class.
 
     ```python
+    from __future__ import annotations
+
     from buildarr.plugins import Plugin
-    from buildarr_example.cli import example
-    from buildarr_example.config import ExampleConfig
-    from buildarr_example.secrets import ExampleSecrets
+
+    from .cli import example
+    from .config import ExampleConfig
+    from .secrets import ExampleSecrets
+
 
     class ExamplePlugin(Plugin):
         cli = example
         config = ExampleConfig
         secrets = ExampleSecrets
     ```
 
     Then, set this class as the entry point for the plugin in your
     Python package configuration.
 
-    Setuptools `setup.py` entry point definition example:
-    ```python
-    from setuptools import setup
-
-    setup(
-        # ...,
-        entry_points={
-            "buildarr.plugins": [
-                "example = buildarr_example.plugin:ExamplePlugin",
-            ],
-        },
-    )
-    ```
-
-    Setuptools `setup.cfg` entry point definition example:
-    ```ini
-    [options.entry_points]
-    buildarr.plugins =
-        example = buildarr_example.plugin:ExamplePlugin
-    ```
-
     Setuptools `pyproject.toml` entry point definition example:
-    ```toml
-    [project.entry-points."buildarr.plugins"]
-    "example" = "buildarr_example.plugin:ExamplePlugin"
-    ```
 
-    Poetry plugin definition example:
     ```toml
-    [tool.poetry.plugins."buildarr.plugins"]
-    "example" = "buildarr_example.plugin:ExamplePlugin"
+    [project.entry-points."buildarr.plugins"]
+    example = "buildarr_example.plugin:ExamplePlugin"
     ```
     """
 
     cli: Optional[ClickGroup] = None
     """
     CLI command group for the plugin.
```

### Comparing `buildarr-0.7.1/buildarr/plugins/types.py` & `buildarr-0.8.0b1/buildarr/plugins/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr plugin type hints.
 """
 
-
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, TypeVar
 
 if TYPE_CHECKING:
     from ..config import ConfigPlugin
     from ..secrets import SecretsPlugin
```

### Comparing `buildarr-0.7.1/buildarr/secrets/__init__.py` & `buildarr-0.8.0b1/buildarr/secrets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,14 +12,13 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr secrets metadata interface.
 """
 
-
 from __future__ import annotations
 
 from .base import SecretsBase
 from .models import SecretsPlugin
 
 __all__ = ["SecretsBase", "SecretsPlugin"]
```

### Comparing `buildarr-0.7.1/buildarr/secrets/base.py` & `buildarr-0.8.0b1/buildarr/secrets/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,57 +12,52 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr secrets metadata base class.
 """
 
-
 from __future__ import annotations
 
 from typing import Generic
 
 from pydantic import BaseModel
 
 from ..plugins import Config
-from ..types import ModelConfigBase
+from ..types import model_config_base
 
 
 class SecretsBase(BaseModel, Generic[Config]):
     """
     Secrets metadata section base class.
 
     When implementing nested sections in a secrets plugin, this class should be used.
     """
 
-    class Config(ModelConfigBase):
-        """
-        Buildarr secrets model class settings.
-
-        Sets some required parameters for serialisation,
-        parsing and validation to work correctly.
-
-        To set additional parameters in your implementing class, subclass this class:
-
-        ```python
-        from __future__ import annotations
-
-        from typing import TYPE_CHECKING
-        from buildarr.secrets import SecretsBase
-
-        if TYPE_CHECKING:
-            from .config import ExampleConfig
-            class _ExampleSecrets(SecretsBase[ExampleSecrets]):
-                ...
-        else:
-            class _ExampleSecrets(SecretsBase):
-                ...
-
-        class ExampleSecrets(_ExampleSecrets):
-            ...
-
-            class Config(_ExampleSecrets.Config):
-                ...  # Add model configuration attributes here.
-        ```
-        """
+    model_config = model_config_base
+    """
+    Buildarr secrets model class settings.
+
+    Sets some required parameters for parsing and validation to work correctly.
+
+    To set additional parameters in your implementing class, override this attribute:
+
+    ```python
+    from __future__ import annotations
+
+    from typing import TYPE_CHECKING
 
-        pass
+    from buildarr.secrets import SecretsBase
+
+    if TYPE_CHECKING:
+        from .config import ExampleConfig
+
+
+    class ExampleSecrets(SecretsBase["ExampleConfig"]):
+        ...
+
+        model_config = {
+            **SecretsBase.model_config,
+            ...  # Add model configuration attributes here.
+        }
+    ```
+    """
```

### Comparing `buildarr-0.7.1/buildarr/secrets/models.py` & `buildarr-0.8.0b1/buildarr/secrets/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr plugin secrets metadata models.
 """
 
-
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from ..plugins import Config
 from .base import SecretsBase
 
@@ -42,28 +41,24 @@
     has access.
 
     The secrets plugin is a Pydantic model, so
     class attributes and type hints are used to specify
     configuration field names and how they should be parsed.
 
     ```python
-    from typing import TYPE_CHECKING, Literal
+    from typing import TYPE_CHECKING, Literal, Self
+
     from buildarr.secrets import SecretsPlugin
     from buildarr.types import NonEmptyStr, Port, Password
 
     if TYPE_CHECKING:
-        from typing import Self
-        from  .config import ExampleConfig
-        class _ExampleSecrets(SecretsPlugin[ExampleConfig]):
-            ...
-    else:
-        class _ExampleSecrets(SecretsPlugin):
-            ...
+        from .config import ExampleConfig
+
 
-    class ExampleSecrets(_ExampleSecrets):
+    class ExampleSecrets(SecretsPlugin["ExampleConfig"]):
         hostname: NonEmptyStr
         port: Port
         protocol: Literal["http", "https"]
         username: NonEmptyStr
         password: Password
 
         @classmethod
```

### Comparing `buildarr-0.7.1/buildarr/state.py` & `buildarr-0.8.0b1/buildarr/state.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,27 +12,27 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr global runtime state.
 """
 
-
 from __future__ import annotations
 
 import os
 
 from collections import defaultdict
 from contextlib import contextmanager
-from distutils.util import strtobool
 from pathlib import Path
 from typing import TYPE_CHECKING, Tuple
 
+from buildarr.util import str_to_bool
+
 if TYPE_CHECKING:
-    from typing import DefaultDict, FrozenSet, Generator, Mapping, Optional, Sequence, Set
+    from typing import DefaultDict, Generator, Mapping, Optional, Sequence, Set
 
     from .config import ConfigPlugin, ConfigType
     from .manager import ManagerPlugin
     from .plugins import Plugin
     from .secrets import SecretsPlugin
 
 
@@ -50,15 +50,15 @@
     """
     Active Buildarr state tracking class.
 
     If anything needs to be shared between plugins or different parts of Buildarr
     over the life of an update run, generally it goes here.
     """
 
-    testing: bool = bool(strtobool(os.environ.get("BUILDARR_TESTING", "false")))
+    testing: bool = str_to_bool(os.environ.get("BUILDARR_TESTING", "false"))
     """
     Whether Buildarr is in testing mode or not.
     """
 
     @property
     def dry_run(self) -> bool:
         """
@@ -104,17 +104,18 @@
     """
 
     instance_configs: Mapping[str, Mapping[str, ConfigPlugin]]
     """
     Fully qualified configuration objects for each instance, under each plugin.
     """
 
-    active_plugins: FrozenSet[str]
+    active_plugins: Sequence[str]
     """
-    A data structure containing the names of all the currently active plugins.
+    A data structure containing the names of all the currently active plugins,
+    in alphabetical order.
     """
 
     trash_metadata_dir: Path
     """
     TRaSH-Guides metadata directory.
 
     Only available if required by at least one instance configuration,
@@ -218,23 +219,27 @@
 
         Args:
             plugin_name (Optional[str], optional): Plugin name to set in the context.
             instance_name (Optional[str], optional): Instance name to set in the context.
         """
         if plugin_name:
             old_current_plugin = self._current_plugin
-            self._current_plugin = plugin_name
         if instance_name:
             old_current_instance = self._current_instance
-            self._current_instance = instance_name
-        yield
-        if plugin_name:
-            self._current_plugin = old_current_plugin
-        if instance_name:
-            self._current_instance = old_current_instance
+        try:
+            if plugin_name:
+                self._current_plugin = plugin_name
+            if instance_name:
+                self._current_instance = instance_name
+            yield
+        finally:
+            if plugin_name:
+                self._current_plugin = old_current_plugin
+            if instance_name:
+                self._current_instance = old_current_instance
 
 
 state = State()
 """
 Global variable for tracking active Buildarr state.
 
 If anything needs to be shared between plugins or different parts of Buildarr
```

### Comparing `buildarr-0.7.1/buildarr/trash.py` & `buildarr-0.8.0b1/buildarr/trash.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr TRaSH-Guides metadata functions.
 """
 
-
 from __future__ import annotations
 
 from logging import getLogger
 from shutil import move, rmtree
 from urllib.request import urlretrieve
 from zipfile import ZipFile
 
@@ -61,30 +60,31 @@
         logger.debug("Creating TRaSH metadata download temporary directory")
         temp_dir = create_temp_dir()
         logger.debug("Finished creating TRaSH metadata download temporary directory")
 
         trash_metadata_filename = temp_dir / "trash-metadata.zip"
 
         logger.debug("Downloading TRaSH metadata")
-        urlretrieve(  # noqa: S310  # `trash_metadata_download_url` is constrained to HTTP URLs.
-            state.config.buildarr.trash_metadata_download_url,
+        urlretrieve(  # noqa: S310
+            str(state.config.buildarr.trash_metadata_download_url),
             trash_metadata_filename,
         )
         logger.debug("Finished downloading TRaSH metadata")
 
         logger.debug("Extracting TRaSH metadata")
         with ZipFile(trash_metadata_filename) as zip_file:
             zip_file.extractall(path=temp_dir / "__trash-metadata__")
         trash_metadata_filename.unlink()
         logger.debug("Finished extracting TRaSH metadata")
 
         logger.debug("Moving TRaSH metadata files to target directory")
-        for subfile in (
-            temp_dir / "__trash-metadata__" / state.config.buildarr.trash_metadata_dir_prefix
-        ).iterdir():
+        trash_metadata_dir = temp_dir / "__trash-metadata__"
+        if state.config.buildarr.trash_metadata_dir_prefix:
+            trash_metadata_dir /= state.config.buildarr.trash_metadata_dir_prefix
+        for subfile in trash_metadata_dir.iterdir():
             move(str(subfile), temp_dir)
         rmtree(temp_dir / "__trash-metadata__")
         logger.debug("Finished moving TRaSH metadata files to target directory")
 
         state.trash_metadata_dir = temp_dir
 
     except Exception:
@@ -94,9 +94,10 @@
 
 def cleanup_trash_metadata() -> None:
     """
     Remove the TRaSH-Guides metadata temporary directory after use,
     and remove it from Buildarr global state.
     """
 
-    remove_dir(state.trash_metadata_dir)
+    if state.trash_metadata_dir:
+        remove_dir(state.trash_metadata_dir)
     state.trash_metadata_dir = None  # type: ignore[assignment]
```

### Comparing `buildarr-0.7.1/buildarr/types.py` & `buildarr-0.8.0b1/buildarr/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,26 +12,33 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr general purpose type hints, used in plugin models.
 """
 
-
 from __future__ import annotations
 
-import re
-
 from functools import total_ordering
-from pathlib import Path, PurePosixPath, PureWindowsPath
-from typing import TYPE_CHECKING, Any, Callable, Dict, Generator, Mapping, Sequence, Type
+from pathlib import Path
+from typing import TYPE_CHECKING, Any, Mapping, Optional, Sequence, Type
 
-from pydantic import AnyUrl, ConstrainedInt, ConstrainedStr, SecretStr
-from pydantic.fields import ModelField
-from typing_extensions import Self
+from pydantic import (
+    AfterValidator,
+    AnyUrl,
+    ConfigDict,
+    Field,
+    GetCoreSchemaHandler,
+    PlainSerializer,
+    SecretStr as PydanticSecretStr,
+    StringConstraints,
+    UrlConstraints,
+)
+from pydantic_core import core_schema
+from typing_extensions import Annotated, Self
 
 from .state import state
 from .util import get_absolute_path
 
 if TYPE_CHECKING:
     from enum import Enum
 
@@ -42,220 +49,221 @@
         values: Sequence[Any]
 
 else:
     # This gets imported when actually running.
     from aenum import MultiValueEnum  # type: ignore[import-untyped]
 
 
-class Password(SecretStr):
-    """
-    Constrained secrets string type for password fields. Required to be non-empty.
-    """
+SecretStr = Annotated[
+    PydanticSecretStr,
+    PlainSerializer(lambda v: v.get_secret_value(), return_type=str),
+]
+"""
+A type for storing string values that contain sensitive information,
+and must be obfuscated when output in logging.
 
-    min_length = 1
+This type is **not** the same as the `pydantic.SecretStr` type,
+as this one has a custom serialiser defined on it to allow
+Buildarr configuration objects to be serialised and dumped.
 
+When defining secret string attributes in Buildarr,
+**this `SecretStr` class must be used.**
+"""
 
-class RssUrl(AnyUrl):
-    """
-    Constrained URL type for RSS URLs.
 
-    ```python
-    from typing import TYPE_CHECKING
-    from buildarr.config import ConfigBase, RssUrl
+Password = Annotated[SecretStr, StringConstraints(min_length=1)]
+"""
+Constrained secret string type for password fields. Required to be non-empty.
+"""
 
-    if TYPE_CHECKING:
-        from .secrets import ExampleSecrets
-        class ExampleConfigBase(ConfigBase[ExampleSecrets]):
-            ...
-    else:
-        class ExampleConfigBase(ConfigBase):
-            ...
 
-    class ExampleConfig(ExampleConfigBase):
-        rss_url: RssUrl
-    ```
-    """
+RssUrl = Annotated[AnyUrl, UrlConstraints(allowed_schemes=["rss"])]
+"""
+Constrained URL type for RSS URLs.
 
-    allowed_schemes = ["rss"]
+```python
+from __future__ import annotations
 
+from buildarr.types import RssUrl
 
-class Port(ConstrainedInt):
-    """
-    Constrained integer type for TCP/UDP port numbers.
+from .types import ExampleConfigBase
 
-    Valid ports range from 1 to 65535 (a 16-bit integer).
 
-    ```python
-    from typing import TYPE_CHECKING
-    from buildarr.config import ConfigBase, NonEmptyStr, Port
+class ExampleConfig(ExampleConfigBase):
+    rss_url: RssUrl
+```
+"""
 
-    if TYPE_CHECKING:
-        from .secrets import ExampleSecrets
-        class ExampleConfigBase(ConfigBase[ExampleSecrets]):
-            ...
-    else:
-        class ExampleConfigBase(ConfigBase):
-            ...
 
-    class ExampleConfig(ExampleConfigBase):
-        host: NonEmptyStr
-        port: Port
-    ```
-    """
+Port = Annotated[int, Field(ge=1, le=65535)]
+"""
+Constrained integer type for TCP/UDP port numbers.
 
-    ge = 1
-    le = 65535
+Valid ports range from 1 to 65535 (a 16-bit integer).
 
+```python
+from __future__ import annotations
 
-class NonEmptyStr(ConstrainedStr):
-    """
-    Constrained string type for non-empty strings.
+from buildarr.types import NonEmptyStr, Port
 
-    When validated in a Buildarr configuration, empty strings
-    or strings composed only of whitespace will fail validation.
+from .types import ExampleConfigBase
 
-    Values are also stripped of whitespace at the start and the end
-    of the strings.
 
-    ```python
-    from buildarr.config import ConfigBase, NonEmptyStr, Port
+class ExampleConfig(ExampleConfigBase):
+    hostname: NonEmptyStr
+    port: Port
+```
+"""
 
-    class ExampleConfig(ConfigBase):
-        host: NonEmptyStr
-        port: Port
-    ```
-    """
 
-    min_length = 1
-    strip_whitespace = True
+NonEmptyStr = Annotated[str, StringConstraints(min_length=1, strip_whitespace=True)]
+"""
+Constrained string type for non-empty strings.
 
+When validated in a Buildarr configuration, empty strings
+or strings composed only of whitespace will fail validation.
 
-class LowerCaseStr(ConstrainedStr):
-    """
-    Constrained string type for lower-case strings.
+Values are also stripped of whitespace at the start and the end
+of the strings.
 
-    When validated in a Buildarr configuration,
-    all upper-case characters in the value will be converted to lower-case.
+```python
+from __future__ import annotations
 
-    ```python
-    from buildarr.config import LowerCaseStr
+from buildarr.types import NonEmptyStr, Port
 
-    class ExampleConfig(ConfigBase):
-        lowercase_name: LowerCaseStr
-    ```
-    """
+from .types import ExampleConfigBase
 
-    to_lower = True
 
+class ExampleConfig(ExampleConfigBase):
+    hostname: NonEmptyStr
+    port: Port
+```
+"""
 
-class LowerCaseNonEmptyStr(LowerCaseStr):
-    """
-    Constrained string type for non-empty lower-case strings.
 
-    This is a combination of `LowerCaseStr` and `NonEmptyStr`,
-    with the validations of both types applying to the value.
+LowerCaseStr = Annotated[str, StringConstraints(to_lower=True)]
+"""
+Constrained string type for lower-case strings.
 
-    ```python
-    from buildarr.config import LowerCaseNonEmptyStr
+When validated in a Buildarr configuration,
+all upper-case characters in the value will be converted to lower-case.
 
-    class ExampleConfig(ConfigBase):
-        lowercase_name: LowerCaseNonEmptyStr
-    ```
-    """
+```python
+from __future__ import annotations
 
-    min_length = 1
-    strip_whitespace = True
+from buildarr.types import LowerCaseStr
 
+from .types import ExampleConfigBase
 
-class UpperCaseStr(ConstrainedStr):
-    """
-    Constrained string type for upper-case strings.
 
-    When validated in a Buildarr configuration,
-    all lower-case characters in the value will be converted to upper-case.
+class ExampleConfig(ExampleConfigBase):
+    lowercase_name: LowerCaseStr
+```
+"""
 
-    ```python
-    from buildarr.config import UpperCaseStr
 
-    class ExampleConfig(ConfigBase):
-        uppercase_name: UpperCaseStr
-    ```
-    """
+LowerCaseNonEmptyStr = Annotated[
+    LowerCaseStr,
+    StringConstraints(min_length=1, strip_whitespace=True),
+]
+"""
+Constrained string type for non-empty lower-case strings.
 
-    to_upper = True
+This is a combination of `LowerCaseStr` and `NonEmptyStr`,
+with the validations of both types applying to the value.
 
+```python
+from __future__ import annotations
 
-class UpperCaseNonEmptyStr(UpperCaseStr):
-    """
-    Constrained string type for non-empty lower-case strings.
+from buildarr.types import LowerCaseNonEmptyStr
 
-    This is a combination of `UpperCaseStr` and `NonEmptyStr`,
-    with the validations of both types applying to the value.
+from .types import ExampleConfigBase
 
-    ```python
-    from buildarr.config import UpperCaseNonEmptyStr
 
-    class ExampleConfig(ConfigBase):
-        uppercase_name: UpperCaseNonEmptyStr
-    ```
-    """
+class ExampleConfig(ExampleConfigBase):
+    lowercase_name: LowerCaseNonEmptyStr
+```
+"""
 
-    min_length = 1
-    strip_whitespace = True
 
+UpperCaseStr = Annotated[str, StringConstraints(to_upper=True)]
+"""
+Constrained string type for upper-case strings.
 
-class TrashID(ConstrainedStr):
-    """
-    Constrained string type for TRaSH-Guides resource IDs.
+When validated in a Buildarr configuration,
+all lower-case characters in the value will be converted to upper-case.
 
-    Accepts any valid TRaSH-Guides ID, and is case-insensitive,
-    converting to lower case internally.
+```python
+from __future__ import annotations
 
-    ```python
-    from typing import TYPE_CHECKING
-    from buildarr.config import ConfigBase, TrashID
+from buildarr.types import UpperCaseStr
 
-    if TYPE_CHECKING:
-        from .secrets import ExampleSecrets
-        class ExampleConfigBase(ConfigBase[ExampleSecrets]):
-            ...
-    else:
-        class ExampleConfigBase(ConfigBase):
-            ...
+from .types import ExampleConfigBase
 
-    class ExampleConfig(ExampleConfigBase):
-        trash_id: TrashID
-    ```
-    """
 
-    regex = re.compile("[A-Fa-f0-9]+")
-    min_length = 32
-    max_length = 32
-    to_lower = True
+class ExampleConfig(ExampleConfigBase):
+    uppercase_name: UpperCaseStr
+```
+"""
+
+
+UpperCaseNonEmptyStr = Annotated[
+    UpperCaseStr,
+    StringConstraints(min_length=1, strip_whitespace=True),
+]
+
+
+TrashID = Annotated[
+    LowerCaseStr,
+    StringConstraints(min_length=32, max_length=32, pattern="^[A-Fa-f0-9]+$"),
+]
+"""
+Constrained string type for TRaSH-Guides resource IDs.
+
+Accepts any valid TRaSH-Guides ID, and is case-insensitive,
+converting to lower case internally.
+
+```python
+from __future__ import annotations
+
+from buildarr.types import TrashID
+
+from .types import ExampleConfigBase
+
+
+class ExampleConfig(ExampleConfigBase):
+    trash_id: TrashID
+```
+"""
 
 
 class BaseEnum(MultiValueEnum):
     """
     Enumeration base class for use in Buildarr configurations.
 
     When configurating an enumeration-type attribute in the Buildarr configuration,
     the user will be able to specify either the name of the enumeration,
     or any of the possible values. Parsing of enumerations is case-insensitive.
 
     For example, given the following example:
 
     ```python
-    from buildarr.config import ConfigBase
+    from __future__ import annotations
+
     from buildarr.types import BaseEnum
 
+    from .types import ExampleConfigBase
+
+
     class Animal(BaseEnum):
         value_1 = 0
         value_2 = 1
 
-    class ExampleConfig(ConfigBase):
+
+    class ExampleConfig(ExampleConfigBase):
         animal: Animal
     ```
 
     The user would be able to configure it in the Buildarr configuration like so:
 
     ```yaml
     ---
@@ -264,16 +272,14 @@
       animal: value-1  # value-1, VALUE_1 or 0 can also be specified here.
     ```
 
     This class also supports specifying multiple values for an enumeration,
     by passing a `tuple` containing all the possible values.
 
     ```python
-    from buildarr.types import BaseEnum
-
     class Animal(BaseEnum):
         value_1 = (0, "dog")
         value_2 = (1, "cat")
     ```
 
     When an enumeration is serialised for a remote instance,
     the first provided value will be used. In the above examples,
@@ -325,35 +331,43 @@
                     and value.lower().replace("/", "_").replace("-", "_") == name
                 ):
                     return obj
         raise KeyError(repr(name))
 
     def to_name_str(self) -> str:
         """
-        Return the name for this enumaration object.
+        Return the name for this enumeration object.
 
         Returns:
             First `str`-type value in list of values (if available),
             otherwise the enumeration name.
         """
         if len(self.values) > 1:
             for value in self.values:
                 if isinstance(value, str):
                     return value
         return self.name.replace("_", "-")
 
     @classmethod
-    def __get_validators__(cls) -> Generator[Callable[[Any], Self], None, None]:
-        """
-        Pass class validation functions to Pydantic.
-
-        Yields:
-            Validation class functions
-        """
-        yield cls.validate
+    def __get_pydantic_core_schema__(
+        cls,
+        source: Type[Any],
+        handler: GetCoreSchemaHandler,
+    ) -> core_schema.CoreSchema:
+        return core_schema.no_info_before_validator_function(
+            function=cls.validate,
+            schema=core_schema.enum_schema(
+                cls,
+                list(cls.__members__.values()),
+                serialization=core_schema.plain_serializer_function_ser_schema(
+                    lambda v: v.to_name_str(),
+                    return_schema=core_schema.str_schema(),
+                ),
+            ),
+        )
 
     @classmethod
     def validate(cls, value: Any) -> Self:
         """
         Validate and coerce the given value to an enumeration object.
 
         Args:
@@ -441,123 +455,107 @@
         try:
             other_obj = DayOfWeek(other)
         except ValueError:
             raise NotImplementedError() from None
         return self.value < other_obj.value
 
 
-class InstanceName(str):
+def InstanceReference(plugin_name: str) -> AfterValidator:  # noqa: N802
     """
-    A type for creating references to an instance in another plugin.
+    A validator generator for creating references to an instance in another plugin.
 
     When loading the instance-specific configurations, Buildarr will dereference
     defined instance references, and order the execution of updates so that
     instances used by another instance get updated first.
 
     This ensures that all instances are in the state expected by the user
     when the instance gets processed.
 
-    When defining `InstanceName`, a Pydantic `Field` needs to be defined
-    with the special `plugin` argument passed to tell Buildarr what plugin
-    to search for the linked instance under.
+    Instances references are defined by using `Annotated`, as shown below:
 
     ```python
-    from typing import TYPE_CHECKING, Optional
-    from pydantic import Field
-    from buildarr.config import ConfigBase, RssUrl
-
-    if TYPE_CHECKING:
-        from .secrets import ExampleSecrets
-        class ExampleConfigBase(ConfigBase[ExampleSecrets]):
-            ...
-    else:
-        class ExampleConfigBase(ConfigBase):
-            ...
+    from __future__ import annotations
+
+    from typing import Optional
+
+    from buildarr.types import InstanceReference
+    from typing_extensions import Annotated
+
+    from .types import ExampleConfigBase
+
 
     class ExampleConfig(ExampleConfigBase):
-        instance_name: Optional[InstanceName] = Field(None, plugin="example")
+        instance_name: Annotated[Optional[str], InstanceReference(plugin_name="example")] = None
     ```
 
     The user will then be able to specify the name of the target instance in
     the Buildarr configuration.
 
     ```yaml
     example:
       instances:
         instance-1:
           ...
         instance-2:
           instance_name: "instance-1"
           ...
     ```
-    """
 
-    @classmethod
-    def __get_validators__(cls) -> Generator[Callable[[str, ModelField], str], None, None]:
-        """
-        Pass the defined validation functions to Pydantic.
-        """
-        yield cls.validate
+    Args:
+        plugin_name (str): Name of the plugin to create an instance reference for.
 
-    @classmethod
-    def validate(cls, value: str, field: ModelField) -> Self:
-        """
-        Validate the type of the instance name reference,
-        evaluate the reference and add the link to the dependency tree structure.
+    Returns:
+        AfterValidator: Validator annotation for the instance reference processing.
+    """
 
-        Args:
-            value (str): Instance name reference.
-            field (ModelField): Field metadata. Used to get the linked plugin name.
+    return AfterValidator(
+        lambda instance_name: _instance_reference(
+            plugin_name=plugin_name,
+            instance_name=instance_name,
+        ),
+    )
+
+
+def _instance_reference(plugin_name: str, instance_name: Optional[str]) -> Optional[str]:
+    if not instance_name:
+        return None
+
+    if plugin_name not in state.plugins:
+        raise ValueError(f"target plugin '{plugin_name}' not installed")
+
+    if not state.config:
+        return instance_name
+
+    instances: Mapping[str, ConfigPlugin] = getattr(state.config, plugin_name).instances
+
+    if instance_name == "default":
+        if instances:
+            raise ValueError(
+                (
+                    "unable to use default instance as the target instance, "
+                    "instance-specific configurations are defined "
+                    f"in plugin '{plugin_name}' configuration ("
+                    f"available instances: {', '.join(repr(i) for i in instances.keys())}"
+                    ")"
+                ),
+            )
+    elif instance_name not in instances:
+        raise ValueError(
+            (
+                f"target instance '{instance_name}' "
+                f"not defined in plugin '{plugin_name}' configuration"
+            ),
+        )
+
+    if state._current_plugin and state._current_instance:
+        state._instance_dependencies[(state._current_plugin, state._current_instance)].add(
+            (plugin_name, instance_name),
+        )
 
-        Raises:
-            ValueError: If the target plugin is not defined as field metadata
-
-        Returns:
-            Instance name object (string-compatible)
-        """
-        NonEmptyStr.validate(value)
-        try:
-            plugin_name: str = field.field_info.extra["plugin"]
-            instance_name = value
-            if plugin_name not in state.plugins:
-                raise ValueError(f"Target plugin '{plugin_name}' not installed")
-            if state.config:
-                instances: Mapping[str, ConfigPlugin] = getattr(
-                    state.config,
-                    plugin_name,
-                ).instances
-                if instance_name == "default":
-                    if instances:
-                        raise ValueError(
-                            "unable to use default instance as the target instance, "
-                            "instance-specific configurations are defined "
-                            f"in plugin '{plugin_name}' configuration ("
-                            f"available instances: {', '.join(repr(i) for i in instances.keys())}"
-                            ")",
-                        )
-                elif instance_name not in instances:
-                    raise ValueError(
-                        f"target instance '{instance_name}' "
-                        f"not defined in plugin '{plugin_name}' configuration",
-                    )
-                if state._current_plugin and state._current_instance:
-                    state._instance_dependencies[
-                        (state._current_plugin, state._current_instance)
-                    ].add(
-                        (plugin_name, instance_name),
-                    )
-        except KeyError as err:
-            if err.args[0] == "plugin":
-                raise ValueError(
-                    "Target plugin not defined in instance name metadata, "
-                    "make sure the default value is set to `Field(None, plugin='<plugin-name>')`",
-                ) from None
-            else:
-                raise
-        return cls(value)
+    return instance_name
 
 
 class LocalPath(type(Path()), Path):  # type: ignore[misc]
     """
     Model type for a local path.
 
     If the supplied path is relative, it is parsed as an absolute path
@@ -572,25 +570,24 @@
     buildarr:
       # Removed in v0.7.0, but still useful as an example in developer docs.
       secrets_file_path: "../secrets/buildarr.json"
     ```
 
     Even when executing Buildarr from a different folder e.g. `/opt/buildarr`,
     the `buildarr.secrets_file_path` attribute would be evaluated as
-    `/path/secrets/buildarr.json`, *not* `/opt/secrets/buildarr.json`.
+    `/path/secrets/buildarr.json`, *not* `/opt/buildarr/buildarr.json`.
     """
 
     @classmethod
-    def __get_validators__(cls) -> Generator[Callable[[Any], Self], None, None]:
-        """
-        Pass class validation functions to Pydantic.
-        Yields:
-            Validation class functions
-        """
-        yield cls.validate
+    def __get_pydantic_core_schema__(
+        cls,
+        source: Type[Any],
+        handler: GetCoreSchemaHandler,
+    ) -> core_schema.CoreSchema:
+        return core_schema.no_info_plain_validator_function(cls.validate)
 
     @classmethod
     def validate(cls, value: Any) -> Self:
         """
         Validate the local path value, and return an absolute path.
         Args:
             value (Any): Object to validate and coerce
@@ -599,65 +596,28 @@
         """
         path = cls(value)
         if not path.is_absolute():
             return cls(get_absolute_path(state._current_dir / path))
         return path
 
 
-config_encoders: Dict[Type[Any], Callable[[Any], Any]] = {
-    BaseEnum: lambda v: v.to_name_str(),
-    PurePosixPath: str,
-    PureWindowsPath: str,
-    SecretStr: lambda v: v.get_secret_value(),
-}
-"""
-The canonical data structure Buildarr uses to serialise custom Python types
-to a type serialisable into JSON and YAML.
-
-When using a custom type that Buildarr does not automatically support
-in plugins, add the required type to this structure, as shown in this example:
-
-```python
-from buildarr.types import config_encoders
-
-class CustomType:
-    ...
-    def __str__(self) -> str:
-        ...
-
-config_encoders[CustomType] = lambda v: str(v)
-```
-"""
-
-
-class ModelConfigBase:
-    """
-    Buildarr model configuration base class.
-
-    Sets some required configuration parameters for
-    serialisation, parsing and validation to work correctly.
-    """
-
-    # Mapping between custom type and encoding function to pass to `json.dumps`.
-    # When adding custom types to encode, **do not override this attribute**,
-    # as it will have no effect.
-    # Instead, add the custom type to `buildarr.types:config_encoders`.
-    json_encoders = config_encoders
-
-    # Required to avoid coersion with same-name but different-typed fields
-    # in objects for which there are multiple types that can be defined.
-    smart_union = True
-
+model_config_base: ConfigDict = {
     # When aliases are defined, allow attributes to be referenced by their
     # internal name, as well as the alias.
-    allow_population_by_field_name = True
-
-    # Validate all configuration attributes, even the default ones.
+    "populate_by_name": True,
+    # Validate model default values.
     # This is necessary because the default attributes sometimes need to
     # be validated for correctness in non-default contexts.
     # (For example, a normally optional attribute becoming required due to
     # another attribute being enabled.)
-    validate_all = True
-
+    "validate_default": True,
     # Validate any values that have been modified in-place, to ensure the model
     # still fits the constraints.
-    validate_assignment = True
+    "validate_assignment": True,
+    # Expose model attribute docstrings as field descriptions.
+    "use_attribute_docstrings": True,
+}
+"""
+Buildarr model configuration base class.
+
+Sets some required configuration parameters for parsing and validation to work correctly.
+"""
```

### Comparing `buildarr-0.7.1/buildarr/util.py` & `buildarr-0.8.0b1/buildarr/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Callum Dickinson
+# Copyright (C) 2024 Callum Dickinson
 #
 # Buildarr is free software: you can redistribute it and/or modify it under the terms of the
 # GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 #
 # Buildarr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
@@ -12,32 +12,58 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Buildarr general utility functions.
 """
 
-
 from __future__ import annotations
 
 import os
 
 from contextlib import contextmanager
-from pathlib import Path
+from pathlib import Path, PurePosixPath, PureWindowsPath
 from shutil import rmtree
 from tempfile import TemporaryDirectory, mkdtemp
 from typing import TYPE_CHECKING, Mapping
 
 if TYPE_CHECKING:
     from typing import Any, Dict, Generator, Union
 
 
 __all__ = ["get_absolute_path", "merge_dicts"]
 
 
+def str_to_bool(val: str) -> bool:
+    """
+    Convert a string representation of truth to `True` or `False`.
+
+    `True` values are `y`, `yes`, `t`, `true`, `on`, and `1`.
+    `False` values are `n`, `no`, `f`, `false`, `off`, and `0`.
+
+    Args:
+        val (str): Value to convert to a boolean.
+
+    Returns:
+        `True` if the value represents a truthy value, otherwise `False`.
+
+    Raises:
+        ValueError: If `val` is anything other than the allowed values.
+    """
+
+    val = val.lower()
+
+    if val in ("y", "yes", "t", "true", "on", "1"):
+        return True
+    elif val in ("n", "no", "f", "false", "off", "0"):
+        return False
+    else:
+        raise ValueError(f"Invalid truth value {val!r}")
+
+
 def get_absolute_path(path: Union[str, os.PathLike]) -> Path:
     """
     Return the absolute version of the given path, *without* resolving symbolic links.
 
     The reason why, in some cases, we don't want to resolve symbolic links is because
     in long lived applications such as daemons, the link target could have changed while the
     file was not being accessed, therefore making our stored reference to the file invalid.
@@ -156,7 +182,36 @@
     """
 
     try:
         rmtree(path)
     except FileNotFoundError:
         if not nonexist_ok:
             raise
+
+
+def windows_to_posix(path: os.PathLike) -> str:
+    """
+    Convert a given Windows path to the equivalent POSIX path, suitable for use in
+    e.g. Docker Desktop for Windows, or Windows Subsystem for Linux.
+
+    If the given path is already POSIX compliant, it will be unmodified.
+
+    Accepts both strings and path-like objects, but returns a string.
+
+    Args:
+        path (path-like object): Path to convert to POSIX.
+
+    Returns:
+        POSIX path string
+    """
+
+    windows_path = PureWindowsPath(path)
+
+    return (
+        str(
+            PurePosixPath(
+                f"/{windows_path.drive.rstrip(':').lower()}",
+            ).joinpath(*windows_path.parts[1:]),
+        )
+        if windows_path.drive
+        else windows_path.as_posix()
+    )
```

### Comparing `buildarr-0.7.1/PKG-INFO` & `buildarr-0.8.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 Metadata-Version: 2.1
 Name: buildarr
-Version: 0.7.1
+Version: 0.8.0b1
 Summary: Constructs and configures Arr PVR stacks
-Home-page: https://buildarr.github.io
+Author-email: Callum Dickinson <callum.dickinson.nz@gmail.com>
 License: GPL-3.0-or-later
+Project-URL: Homepage, https://buildarr.github.io
+Project-URL: Documentation, https://buildarr.github.io
+Project-URL: Repository, https://github.com/buildarr/buildarr
+Project-URL: Issues, https://github.com/buildarr/buildarr/issues
+Project-URL: Changelog, https://buildarr.github.io/release-notes
 Keywords: buildarr,sonarr,radarr,prowlarr
-Author: Callum Dickinson
-Author-email: callum.dickinson.nz@gmail.com
-Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Systems Administration
 Classifier: Typing :: Typed
-Requires-Dist: aenum
-Requires-Dist: click (>=8.0.4)
-Requires-Dist: click-params (>=0.4.1)
-Requires-Dist: importlib-metadata (>=4.6.0)
-Requires-Dist: pydantic[email] (>=1.10.0,<2.0.0)
-Requires-Dist: pyyaml (>=6.0)
-Requires-Dist: requests (>=2.28.0)
-Requires-Dist: schedule (>=1.1.0)
-Requires-Dist: stevedore (>=4.0.0)
-Requires-Dist: typing-extensions (>=4.0.1)
-Requires-Dist: watchdog (>=3.0.0)
-Project-URL: Changes, https://buildarr.github.io/release-notes
-Project-URL: Documentation, https://buildarr.github.io
-Project-URL: Issue Tracker, https://github.com/buildarr/buildarr/issues
-Project-URL: Repository, https://github.com/buildarr/buildarr
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aenum
+Requires-Dist: click>=8.0.4
+Requires-Dist: importlib-metadata>=4.6.0
+Requires-Dist: pyyaml>=6.0
+Requires-Dist: pydantic[email]<3.0.0,>=2.0.0
+Requires-Dist: requests>=2.28.0
+Requires-Dist: schedule>=1.1.0
+Requires-Dist: stevedore>=4.0.0
+Requires-Dist: typing-extensions>=4.0.1
+Requires-Dist: watchdog>=3.0.0
 
 # Welcome to Buildarr!
 
-[![Docker Version](https://img.shields.io/docker/v/callum027/buildarr?sort=semver)](https://hub.docker.com/r/callum027/buildarr) [![PyPI](https://img.shields.io/pypi/v/buildarr)](https://pypi.org/project/buildarr) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/buildarr) [![GitHub](https://img.shields.io/github/license/buildarr/buildarr)](https://github.com/buildarr/buildarr/blob/main/LICENSE) ![Pre-commit hooks](https://github.com/buildarr/buildarr/actions/workflows/pre-commit.yml/badge.svg) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Docker Version](https://img.shields.io/docker/v/callum027/buildarr?sort=semver)](https://hub.docker.com/r/callum027/buildarr) [![PyPI](https://img.shields.io/pypi/v/buildarr)](https://pypi.org/project/buildarr) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/buildarr) [![GitHub](https://img.shields.io/github/license/buildarr/buildarr)](https://github.com/buildarr/buildarr/blob/main/LICENSE) ![Test Status](https://img.shields.io/github/actions/workflow/status/buildarr/buildarr/test.yml?label=tests) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This is Buildarr, a solution to automating deployment and configuration of your *Arr stack.
 
 Have you spent many hours getting your setup for one or more linked Sonarr/Radarr/Prowlarr instances just right, only to have no way to reproduce this setup apart from UI screenshots and database backups?
 
 Buildarr aims to alleviate those concerns by using a static configuration file to store settings for all your *Arr applications, and automatically configure them as defined. It can just once using an ad-hoc user command, or as a service to keep your application configurations up to date. Buildarr runs idempotently, only making changes to your instance if they are required.
 
@@ -308,8 +307,7 @@
 ```
 
 Poetry plugin definition example:
 ```toml
 [tool.poetry.plugins."buildarr.plugins"]
 "example" = "buildarr_example.plugin:ExamplePlugin"
 ```
-
```

