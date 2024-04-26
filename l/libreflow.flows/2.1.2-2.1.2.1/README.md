# Comparing `tmp/libreflow_flows-2.1.2.tar.gz` & `tmp/libreflow_flows-2.1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreflow_flows-2.1.2.tar", last modified: Fri Apr 26 13:59:24 2024, max compression
+gzip compressed data, was "libreflow_flows-2.1.2.1.tar", last modified: Fri Apr 26 14:03:38 2024, max compression
```

## Comparing `libreflow_flows-2.1.2.tar` & `libreflow_flows-2.1.2.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.299532 libreflow_flows-2.1.2/
--rw-rw-rw-   0 root         (0) root         (0)      480 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)     4563 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1053 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5443 2024-04-26 13:59:24.299532 libreflow_flows-2.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      192 2024-04-26 13:59:24.299532 libreflow_flows-2.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2060 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.282532 libreflow_flows-2.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.287532 libreflow_flows-2.1.2/src/libreflow/
--rw-rw-rw-   0 root         (0) root         (0)       64 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.299532 libreflow_flows-2.1.2/src/libreflow/flows/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2024-04-26 13:59:24.300532 libreflow_flows-2.1.2/src/libreflow/flows/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.290532 libreflow_flows-2.1.2/src/libreflow/flows/custom_home/
--rw-rw-rw-   0 root         (0) root         (0)     6343 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/custom_home/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7386 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/custom_home/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.290532 libreflow_flows-2.1.2/src/libreflow/flows/default/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/default/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.292532 libreflow_flows-2.1.2/src/libreflow/flows/default/flow/
--rw-rw-rw-   0 root         (0) root         (0)     7258 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/default/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5816 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/default/flow/asset.py
--rw-rw-rw-   0 root         (0) root         (0)     1784 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/default/flow/entity_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    16548 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/default/flow/file.py
--rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/default/flow/film.py
--rw-rw-rw-   0 root         (0) root         (0)     2757 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/default/flow/shot.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/default/flow/task.py
--rw-rw-rw-   0 root         (0) root         (0)     7961 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/default/flow/user.py
--rw-rw-rw-   0 root         (0) root         (0)     5156 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/gui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.293532 libreflow_flows-2.1.2/src/libreflow/flows/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.293532 libreflow_flows-2.1.2/src/libreflow/flows/resources/file_templates/
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/file_templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   149688 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/file_templates/template.blend
--rw-rw-rw-   0 root         (0) root         (0)    88244 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/file_templates/template.wav
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.294532 libreflow_flows-2.1.2/src/libreflow/flows/resources/gifs/
--rw-rw-rw-   0 root         (0) root         (0)      144 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/gifs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   744158 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/gifs/magic_word.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.295532 libreflow_flows-2.1.2/src/libreflow/flows/resources/gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/gui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.295532 libreflow_flows-2.1.2/src/libreflow/flows/resources/gui/styles/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/gui/styles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.295532 libreflow_flows-2.1.2/src/libreflow/flows/resources/gui/styles/default_style/
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/gui/styles/default_style/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8358 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/gui/styles/default_style/default_style.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.296532 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.297532 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/
--rw-rw-rw-   0 root         (0) root         (0)     5702 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13809 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/file.py
--rw-rw-rw-   0 root         (0) root         (0)    45139 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/film.py
--rw-rw-rw-   0 root         (0) root         (0)    22662 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     3125 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/users.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.297532 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.297532 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/file_templates/
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/file_templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    94110 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/file_templates/template.blend
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.298532 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/icons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.298532 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/icons/flow/
--rw-rw-rw-   0 root         (0) root         (0)      163 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/icons/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1287 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/icons/flow/publish-ok.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.298532 libreflow_flows-2.1.2/src/libreflow.flows.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5443 2024-04-26 13:59:24.000000 libreflow_flows-2.1.2/src/libreflow.flows.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2072 2024-04-26 13:59:24.000000 libreflow_flows-2.1.2/src/libreflow.flows.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 13:59:24.000000 libreflow_flows-2.1.2/src/libreflow.flows.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-26 13:59:24.000000 libreflow_flows-2.1.2/src/libreflow.flows.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-26 13:59:24.000000 libreflow_flows-2.1.2/src/libreflow.flows.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    80044 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.261820 libreflow_flows-2.1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)      480 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)     4563 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5445 2024-04-26 14:03:38.261820 libreflow_flows-2.1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      192 2024-04-26 14:03:38.261820 libreflow_flows-2.1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2074 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.245820 libreflow_flows-2.1.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.250820 libreflow_flows-2.1.2.1/src/libreflow/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.262820 libreflow_flows-2.1.2.1/src/libreflow/flows/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      499 2024-04-26 14:03:38.262820 libreflow_flows-2.1.2.1/src/libreflow/flows/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.252820 libreflow_flows-2.1.2.1/src/libreflow/flows/custom_home/
+-rw-rw-rw-   0 root         (0) root         (0)     6343 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/custom_home/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7386 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/custom_home/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.253820 libreflow_flows-2.1.2.1/src/libreflow/flows/default/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/default/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.254820 libreflow_flows-2.1.2.1/src/libreflow/flows/default/flow/
+-rw-rw-rw-   0 root         (0) root         (0)     7258 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/default/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5816 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/default/flow/asset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1784 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/default/flow/entity_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    16548 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/default/flow/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/default/flow/film.py
+-rw-rw-rw-   0 root         (0) root         (0)     2757 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/default/flow/shot.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/default/flow/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     7961 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/default/flow/user.py
+-rw-rw-rw-   0 root         (0) root         (0)     5156 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/gui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.255820 libreflow_flows-2.1.2.1/src/libreflow/flows/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.255820 libreflow_flows-2.1.2.1/src/libreflow/flows/resources/file_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/resources/file_templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   149688 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/resources/file_templates/template.blend
+-rw-rw-rw-   0 root         (0) root         (0)    88244 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/resources/file_templates/template.wav
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.256820 libreflow_flows-2.1.2.1/src/libreflow/flows/resources/gifs/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/resources/gifs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   744158 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/resources/gifs/magic_word.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.257820 libreflow_flows-2.1.2.1/src/libreflow/flows/resources/gui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/resources/gui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.257820 libreflow_flows-2.1.2.1/src/libreflow/flows/resources/gui/styles/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/resources/gui/styles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.257820 libreflow_flows-2.1.2.1/src/libreflow/flows/resources/gui/styles/default_style/
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/resources/gui/styles/default_style/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8358 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/resources/gui/styles/default_style/default_style.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.258820 libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.259820 libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/flow/
+-rw-rw-rw-   0 root         (0) root         (0)     5702 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13809 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/flow/file.py
+-rw-rw-rw-   0 root         (0) root         (0)    45139 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/flow/film.py
+-rw-rw-rw-   0 root         (0) root         (0)    22662 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/flow/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     3125 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/flow/users.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.259820 libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.260820 libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/resources/file_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/resources/file_templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    94110 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/resources/file_templates/template.blend
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.260820 libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/resources/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/resources/icons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.260820 libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/resources/icons/flow/
+-rw-rw-rw-   0 root         (0) root         (0)      163 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/resources/icons/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/resources/icons/flow/publish-ok.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:03:38.261820 libreflow_flows-2.1.2.1/src/libreflow.flows.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5445 2024-04-26 14:03:38.000000 libreflow_flows-2.1.2.1/src/libreflow.flows.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-04-26 14:03:38.000000 libreflow_flows-2.1.2.1/src/libreflow.flows.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 14:03:38.000000 libreflow_flows-2.1.2.1/src/libreflow.flows.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-26 14:03:38.000000 libreflow_flows-2.1.2.1/src/libreflow.flows.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-26 14:03:38.000000 libreflow_flows-2.1.2.1/src/libreflow.flows.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    80044 2024-04-26 14:03:28.000000 libreflow_flows-2.1.2.1/versioneer.py
```

### Comparing `libreflow_flows-2.1.2/CHANGELOG.md` & `libreflow_flows-2.1.2.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/LICENSE` & `libreflow_flows-2.1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/PKG-INFO` & `libreflow_flows-2.1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.flows
-Version: 2.1.2
+Version: 2.1.2.1
 Summary: A set of flows specific to projects handled by Libreflow at Les Fées Spéciales.
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow.flows
 Author: Baptiste Delos, Flavio Perez
 Author-email: baptiste@les-fees-speciales.coop, flavio@lfs.coop
 License: LGPLv3+
 Keywords: kabaret cgwire kitsu gazu animation pipeline libreflow
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: libreflow>=2.3.0
+Requires-Dist: libreflow~=2.3.0
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html)[^1].
```

### Comparing `libreflow_flows-2.1.2/setup.py` & `libreflow_flows-2.1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,17 @@
         "Intended Audience :: Developers",
         "Intended Audience :: End Users/Desktop",
         "Intended Audience :: Information Technology",
         "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
         "Operating System :: OS Independent",
     ],
     keywords="kabaret cgwire kitsu gazu animation pipeline libreflow",
-    install_requires=["libreflow>=2.3.0"],
+    install_requires=[
+        "libreflow~=2.3.0"
+    ],
     python_requires=">=3.8",
     packages=setuptools.find_packages("src"),
     package_dir={"": "src"},
     package_data={
         '': [
             "*.css",
             '*.png',
```

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/custom_home/__init__.py` & `libreflow_flows-2.1.2.1/src/libreflow/flows/custom_home/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/custom_home/ui.py` & `libreflow_flows-2.1.2.1/src/libreflow/flows/custom_home/ui.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/default/flow/__init__.py` & `libreflow_flows-2.1.2.1/src/libreflow/flows/default/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/default/flow/asset.py` & `libreflow_flows-2.1.2.1/src/libreflow/flows/default/flow/asset.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/default/flow/entity_manager.py` & `libreflow_flows-2.1.2.1/src/libreflow/flows/default/flow/entity_manager.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/default/flow/file.py` & `libreflow_flows-2.1.2.1/src/libreflow/flows/default/flow/file.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/default/flow/film.py` & `libreflow_flows-2.1.2.1/src/libreflow/flows/default/flow/film.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/default/flow/shot.py` & `libreflow_flows-2.1.2.1/src/libreflow/flows/default/flow/shot.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/default/flow/user.py` & `libreflow_flows-2.1.2.1/src/libreflow/flows/default/flow/user.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/gui.py` & `libreflow_flows-2.1.2.1/src/libreflow/flows/gui.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/resources/file_templates/template.blend` & `libreflow_flows-2.1.2.1/src/libreflow/flows/resources/file_templates/template.blend`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/resources/file_templates/template.wav` & `libreflow_flows-2.1.2.1/src/libreflow/flows/resources/file_templates/template.wav`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/resources/gifs/magic_word.gif` & `libreflow_flows-2.1.2.1/src/libreflow/flows/resources/gifs/magic_word.gif`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/resources/gui/styles/default_style/__init__.py` & `libreflow_flows-2.1.2.1/src/libreflow/flows/resources/gui/styles/default_style/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/resources/gui/styles/default_style/default_style.css` & `libreflow_flows-2.1.2.1/src/libreflow/flows/resources/gui/styles/default_style/default_style.css`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/__init__.py` & `libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/file.py` & `libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/flow/file.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/film.py` & `libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/flow/film.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/lib.py` & `libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/flow/lib.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/users.py` & `libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/flow/users.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/file_templates/template.blend` & `libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/resources/file_templates/template.blend`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/icons/flow/publish-ok.png` & `libreflow_flows-2.1.2.1/src/libreflow/flows/tinykin/resources/icons/flow/publish-ok.png`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/src/libreflow.flows.egg-info/PKG-INFO` & `libreflow_flows-2.1.2.1/src/libreflow.flows.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.flows
-Version: 2.1.2
+Version: 2.1.2.1
 Summary: A set of flows specific to projects handled by Libreflow at Les Fées Spéciales.
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow.flows
 Author: Baptiste Delos, Flavio Perez
 Author-email: baptiste@les-fees-speciales.coop, flavio@lfs.coop
 License: LGPLv3+
 Keywords: kabaret cgwire kitsu gazu animation pipeline libreflow
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: libreflow>=2.3.0
+Requires-Dist: libreflow~=2.3.0
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html)[^1].
```

### Comparing `libreflow_flows-2.1.2/src/libreflow.flows.egg-info/SOURCES.txt` & `libreflow_flows-2.1.2.1/src/libreflow.flows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.2/versioneer.py` & `libreflow_flows-2.1.2.1/versioneer.py`

 * *Files identical despite different names*

