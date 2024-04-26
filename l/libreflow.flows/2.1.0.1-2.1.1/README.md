# Comparing `tmp/libreflow.flows-2.1.0.1.tar.gz` & `tmp/libreflow_flows-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreflow.flows-2.1.0.1.tar", last modified: Wed Jan 10 14:23:26 2024, max compression
+gzip compressed data, was "libreflow_flows-2.1.1.tar", last modified: Fri Apr 26 09:12:37 2024, max compression
```

## Comparing `libreflow.flows-2.1.0.1.tar` & `libreflow_flows-2.1.1.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.945415 libreflow.flows-2.1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)      480 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)     4130 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1053 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5012 2024-01-10 14:23:26.945415 libreflow.flows-2.1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      192 2024-01-10 14:23:26.945415 libreflow.flows-2.1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1678 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.930415 libreflow.flows-2.1.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.934415 libreflow.flows-2.1.0.1/src/libreflow/
--rw-rw-rw-   0 root         (0) root         (0)       64 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.945415 libreflow.flows-2.1.0.1/src/libreflow/flows/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/__init__.py
--rw-r--r--   0 root         (0) root         (0)      499 2024-01-10 14:23:26.945415 libreflow.flows-2.1.0.1/src/libreflow/flows/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.937415 libreflow.flows-2.1.0.1/src/libreflow/flows/custom_home/
--rw-rw-rw-   0 root         (0) root         (0)     6343 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/custom_home/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7386 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/custom_home/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.937415 libreflow.flows-2.1.0.1/src/libreflow/flows/default/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/default/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.939415 libreflow.flows-2.1.0.1/src/libreflow/flows/default/flow/
--rw-rw-rw-   0 root         (0) root         (0)     7258 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/default/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5611 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/default/flow/asset.py
--rw-rw-rw-   0 root         (0) root         (0)     1784 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/default/flow/entity_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    16548 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/default/flow/file.py
--rw-rw-rw-   0 root         (0) root         (0)     1478 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/default/flow/film.py
--rw-rw-rw-   0 root         (0) root         (0)     2649 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/default/flow/shot.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/default/flow/task.py
--rw-rw-rw-   0 root         (0) root         (0)     7938 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/default/flow/user.py
--rw-rw-rw-   0 root         (0) root         (0)     5156 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/gui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.939415 libreflow.flows-2.1.0.1/src/libreflow/flows/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.939415 libreflow.flows-2.1.0.1/src/libreflow/flows/resources/file_templates/
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/resources/file_templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   149688 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/resources/file_templates/template.blend
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.940415 libreflow.flows-2.1.0.1/src/libreflow/flows/resources/gifs/
--rw-rw-rw-   0 root         (0) root         (0)      144 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/resources/gifs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   744158 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/resources/gifs/magic_word.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.941415 libreflow.flows-2.1.0.1/src/libreflow/flows/resources/gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/resources/gui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.941415 libreflow.flows-2.1.0.1/src/libreflow/flows/resources/gui/styles/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/resources/gui/styles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.941415 libreflow.flows-2.1.0.1/src/libreflow/flows/resources/gui/styles/default_style/
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/resources/gui/styles/default_style/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8358 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/resources/gui/styles/default_style/default_style.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.942415 libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.943415 libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/flow/
--rw-rw-rw-   0 root         (0) root         (0)     5702 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13809 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/flow/file.py
--rw-rw-rw-   0 root         (0) root         (0)    45139 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/flow/film.py
--rw-rw-rw-   0 root         (0) root         (0)    22662 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/flow/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     3125 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/flow/users.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.943415 libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.943415 libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/resources/file_templates/
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/resources/file_templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    94110 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/resources/file_templates/template.blend
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.944415 libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/resources/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/resources/icons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.944415 libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/resources/icons/flow/
--rw-rw-rw-   0 root         (0) root         (0)      163 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/resources/icons/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1287 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/resources/icons/flow/publish-ok.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 14:23:26.944415 libreflow.flows-2.1.0.1/src/libreflow.flows.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5012 2024-01-10 14:23:26.000000 libreflow.flows-2.1.0.1/src/libreflow.flows.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2014 2024-01-10 14:23:26.000000 libreflow.flows-2.1.0.1/src/libreflow.flows.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-10 14:23:26.000000 libreflow.flows-2.1.0.1/src/libreflow.flows.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-01-10 14:23:26.000000 libreflow.flows-2.1.0.1/src/libreflow.flows.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-01-10 14:23:26.000000 libreflow.flows-2.1.0.1/src/libreflow.flows.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    80044 2024-01-10 14:23:18.000000 libreflow.flows-2.1.0.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.444964 libreflow_flows-2.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)      480 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)     4385 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5265 2024-04-26 09:12:37.444964 libreflow_flows-2.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      192 2024-04-26 09:12:37.444964 libreflow_flows-2.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2060 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.428964 libreflow_flows-2.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.433964 libreflow_flows-2.1.1/src/libreflow/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.445964 libreflow_flows-2.1.1/src/libreflow/flows/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2024-04-26 09:12:37.445964 libreflow_flows-2.1.1/src/libreflow/flows/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.435964 libreflow_flows-2.1.1/src/libreflow/flows/custom_home/
+-rw-rw-rw-   0 root         (0) root         (0)     6343 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/custom_home/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7386 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/custom_home/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.436964 libreflow_flows-2.1.1/src/libreflow/flows/default/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/default/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.437964 libreflow_flows-2.1.1/src/libreflow/flows/default/flow/
+-rw-rw-rw-   0 root         (0) root         (0)     7258 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/default/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5816 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/default/flow/asset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1784 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/default/flow/entity_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    16548 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/default/flow/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/default/flow/film.py
+-rw-rw-rw-   0 root         (0) root         (0)     2757 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/default/flow/shot.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/default/flow/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     7961 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/default/flow/user.py
+-rw-rw-rw-   0 root         (0) root         (0)     5156 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/gui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.438964 libreflow_flows-2.1.1/src/libreflow/flows/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.439964 libreflow_flows-2.1.1/src/libreflow/flows/resources/file_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/file_templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   149688 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/file_templates/template.blend
+-rw-rw-rw-   0 root         (0) root         (0)    88244 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/file_templates/template.wav
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.439964 libreflow_flows-2.1.1/src/libreflow/flows/resources/gifs/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/gifs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   744158 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/gifs/magic_word.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.440964 libreflow_flows-2.1.1/src/libreflow/flows/resources/gui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/gui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.440964 libreflow_flows-2.1.1/src/libreflow/flows/resources/gui/styles/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/gui/styles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.440964 libreflow_flows-2.1.1/src/libreflow/flows/resources/gui/styles/default_style/
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/gui/styles/default_style/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8358 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/gui/styles/default_style/default_style.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.441964 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.442964 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/
+-rw-rw-rw-   0 root         (0) root         (0)     5702 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13809 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/file.py
+-rw-rw-rw-   0 root         (0) root         (0)    45139 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/film.py
+-rw-rw-rw-   0 root         (0) root         (0)    22662 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     3125 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/users.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.442964 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.443964 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/file_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/file_templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    94110 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/file_templates/template.blend
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.443964 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/icons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.443964 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/icons/flow/
+-rw-rw-rw-   0 root         (0) root         (0)      163 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/icons/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/icons/flow/publish-ok.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.444964 libreflow_flows-2.1.1/src/libreflow.flows.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5265 2024-04-26 09:12:37.000000 libreflow_flows-2.1.1/src/libreflow.flows.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-04-26 09:12:37.000000 libreflow_flows-2.1.1/src/libreflow.flows.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 09:12:37.000000 libreflow_flows-2.1.1/src/libreflow.flows.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-26 09:12:37.000000 libreflow_flows-2.1.1/src/libreflow.flows.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-26 09:12:37.000000 libreflow_flows-2.1.1/src/libreflow.flows.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    80044 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/versioneer.py
```

### Comparing `libreflow.flows-2.1.0.1/CHANGELOG.md` & `libreflow_flows-2.1.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,24 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [2.1.1] - 2024-04-26
+
+### Added
+
+* Create Shots, Asset Types and Assets from Kitsu: for existing entities, default tasks are now updated, in case new tasks need to be added.
+
+### Changed
+
+* Improved log messages for create objects from Kitsu actions.
+
 ## [2.1.0] - 2024-10-01
 
 ### Added
 
 * Creation of shots and assets from Kitsu: an option can be checked to create the task default files enabled by default in the task manager.
 * File references are now stored in a collection in the project's entity manager.
 * The session provides a new command-line option `--search-auto-indexing` to enable the search engine's automatic indexing. This feature can also be enabled by defining the `SEARCH_AUTO_INDEXING` variable in the environment of the session launch script.
```

### Comparing `libreflow.flows-2.1.0.1/LICENSE` & `libreflow_flows-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libreflow.flows-2.1.0.1/PKG-INFO` & `libreflow_flows-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.flows
-Version: 2.1.0.1
+Version: 2.1.1
 Summary: A set of flows specific to projects handled by Libreflow at Les Fées Spéciales.
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow.flows
 Author: Baptiste Delos, Flavio Perez
 Author-email: baptiste@les-fees-speciales.coop, flavio@lfs.coop
 License: LGPLv3+
 Keywords: kabaret cgwire kitsu gazu animation pipeline libreflow
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,24 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [2.1.1] - 2024-04-26
+
+### Added
+
+* Create Shots, Asset Types and Assets from Kitsu: for existing entities, default tasks are now updated, in case new tasks need to be added.
+
+### Changed
+
+* Improved log messages for create objects from Kitsu actions.
+
 ## [2.1.0] - 2024-10-01
 
 ### Added
 
 * Creation of shots and assets from Kitsu: an option can be checked to create the task default files enabled by default in the task manager.
 * File references are now stored in a collection in the project's entity manager.
 * The session provides a new command-line option `--search-auto-indexing` to enable the search engine's automatic indexing. This feature can also be enabled by defining the `SEARCH_AUTO_INDEXING` variable in the environment of the session launch script.
```

### Comparing `libreflow.flows-2.1.0.1/setup.py` & `libreflow_flows-2.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,11 +34,36 @@
     ],
     keywords="kabaret cgwire kitsu gazu animation pipeline libreflow",
     install_requires=["libreflow>=2.3.0"],
     python_requires=">=3.8",
     packages=setuptools.find_packages("src"),
     package_dir={"": "src"},
     package_data={
-        "": ["*.css", "*.png", "*.svg", "*.gif", "*.abc", "*.aep", "*.ai", "*.blend", "*.jpg", "*.kra", "*.mov", "*.psd", "*.txt", "*.usd", "*.fbx", "*.json", "*.obj"],
+        '': [
+            "*.css",
+            '*.png',
+            '*.svg',
+            '*.gif',
+            '*.abc',
+            '*.aep',
+            '*.ai',
+            '*.blend',
+            '*.jpg',
+            '*.kra',
+            '*.mov',
+            '*.psd',
+            '*.psb',
+            '*.txt',
+            '*.usd',
+            '*.fbx',
+            '*.json',
+            '*.obj',
+            '*.wav',
+            '*.pproj',
+            '*.ttf',
+            '*.otf',
+            '*.nk',
+            '*.jsx',
+            '*.mp4'
+        ],
     },
-
 )
```

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/custom_home/__init__.py` & `libreflow_flows-2.1.1/src/libreflow/flows/custom_home/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/custom_home/ui.py` & `libreflow_flows-2.1.1/src/libreflow/flows/custom_home/ui.py`

 * *Files identical despite different names*

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/default/flow/__init__.py` & `libreflow_flows-2.1.1/src/libreflow/flows/default/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/default/flow/asset.py` & `libreflow_flows-2.1.1/src/libreflow/flows/default/flow/asset.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,27 +52,28 @@
         
         skip_existing = self.skip_existing.get()
         assets_data = self.root().project().kitsu_api().get_assets_data(self._asset_type.name())
         for data in assets_data:
             name = data['name']
 
             if not self._assets.has_mapped_name(name):
-                s = self._assets.add(name)
+                print(f'Create Kitsu Assets : Creating Asset {name}')
+                a = self._assets.add(name)
             elif not skip_existing:
-                s = self._assets[name]
+                a = self._assets[name]
+                print(f'Create Kitsu Assets : Updating Default Tasks {name}')
+                a.ensure_tasks()
             else:
                 continue
 
             if self.create_task_default_files.get():
-                for t in s.tasks.mapped_items():
-                    print(f'{self._asset_type.name()} {s.name()} {t.name()}')
+                for t in a.tasks.mapped_items():
+                    print(f'Create Kitsu Assets : Updating Default Files {name} {t.name()}')
                     t.create_dft_files.files.update()
                     t.create_dft_files.run(None)
-            
-            print(f'Create asset: {self._asset_type.name()} - {data["name"]}')
         
         self._assets.touch()
 
 
 class Assets(AssetCollection):
 
     create_assets = flow.Child(CreateKitsuAssets)
@@ -143,22 +144,22 @@
         for data in asset_types_data:
             name = data['name']
 
             if name == 'x':
                 continue
 
             if not self._asset_types.has_mapped_name(name):
+                print(f'Create Kitsu Asset Types : Creating Asset Type {name}')
                 a = self._asset_types.add(name)
             elif not skip_existing:
+                print(f'Create Kitsu Asset Types : Asset Type {name} exists')
                 a = self._asset_types[name]
             else:
                 continue
             
-            print(f'Create asset type: {data["name"]}')
-
             if create_assets:
                 a.assets.create_assets.skip_existing.set(skip_existing)
                 a.assets.create_assets.create_task_default_files.set(self.create_task_default_files.get())
                 a.assets.create_assets.run('Create assets')
         
         self._asset_types.touch()
```

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/default/flow/entity_manager.py` & `libreflow_flows-2.1.1/src/libreflow/flows/default/flow/entity_manager.py`

 * *Files identical despite different names*

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/default/flow/file.py` & `libreflow_flows-2.1.1/src/libreflow/flows/default/flow/file.py`

 * *Files identical despite different names*

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/default/flow/film.py` & `libreflow_flows-2.1.1/src/libreflow/flows/default/flow/film.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,20 +24,20 @@
         skip_existing = self.skip_existing.get()
 
         for data in sequences_data:
             name = data['name']
 
             if not self._film.sequences.has_mapped_name(name):
                 s = self._film.sequences.add(name)
+                print(f'Create Kitsu Sequences : Creating Sequence {name}')
             elif not skip_existing:
+                print(f'Create Kitsu Sequences : Sequence {name} exists')
                 s = self._film.sequences[name]
             else:
                 continue
-            
-            print(f'Create sequence {data["name"]}')
 
             if create_shots:
                 s.create_shots.skip_existing.set(skip_existing)
                 s.create_shots.create_task_default_files.set(self.create_task_default_files.get())
                 s.create_shots.run('Create shots')
         
         self._film.sequences.touch()
```

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/default/flow/shot.py` & `libreflow_flows-2.1.1/src/libreflow/flows/default/flow/shot.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,27 +60,28 @@
         
         skip_existing = self.skip_existing.get()
         shots_data = self.root().project().kitsu_api().get_shots_data(self._sequence.name())
         for data in shots_data:
             name = data['name']
 
             if not self._sequence.shots.has_mapped_name(name):
+                print(f'Create Kitsu Shots : Creating Shot {name}')
                 s = self._sequence.shots.add(name)
             elif not skip_existing:
                 s = self._sequence.shots[name]
+                print(f'Create Kitsu Shots : Updating Default Tasks {name}')
+                s.ensure_tasks()
             else:
                 continue
             
             if self.create_task_default_files.get():
                 for t in s.tasks.mapped_items():
-                    print(f'{self._sequence.name()} {s.name()} {t.name()}')
+                    print(f'Create Kitsu Shots : Updating Default Files {name} {t.name()}')
                     t.create_dft_files.files.update()
                     t.create_dft_files.run(None)
-            
-            print(f'Create shot {self._sequence.name()} {data["name"]}')
         
         self._sequence.shots.touch()
 
 
 class Sequence(BaseSequence):
     
     shots = flow.Child(Shots).ui(
```

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/default/flow/user.py` & `libreflow_flows-2.1.1/src/libreflow/flows/default/flow/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,17 +193,17 @@
             return
         
         kitsu_users = self.root().project().kitsu_config().users
         
         for item in self.users.mapped_items():
             user_name = item.user_login.get().replace('.', '').replace('-', '')
             if not self._map.get_user(item.user_login.get()):
+                print(f'Create Kitsu Users : Creating User {item.user_login.get()}')
                 self._map.add_user(user_name, item.user_login.get(), item.user_status.get())
                 self.root().project().kitsu_api().set_user_login(user_name, item.user_login.get())
-                print(f'Create user {item.user_login.get()}')
         
         self._map.touch()
         kitsu_users.touch()
 
 
 class Users(BaseUsers):
```

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/gui.py` & `libreflow_flows-2.1.1/src/libreflow/flows/gui.py`

 * *Files identical despite different names*

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/resources/file_templates/template.blend` & `libreflow_flows-2.1.1/src/libreflow/flows/resources/file_templates/template.blend`

 * *Files identical despite different names*

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/resources/gifs/magic_word.gif` & `libreflow_flows-2.1.1/src/libreflow/flows/resources/gifs/magic_word.gif`

 * *Files identical despite different names*

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/resources/gui/styles/default_style/__init__.py` & `libreflow_flows-2.1.1/src/libreflow/flows/resources/gui/styles/default_style/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/resources/gui/styles/default_style/default_style.css` & `libreflow_flows-2.1.1/src/libreflow/flows/resources/gui/styles/default_style/default_style.css`

 * *Files identical despite different names*

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/flow/__init__.py` & `libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/flow/file.py` & `libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/file.py`

 * *Files identical despite different names*

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/flow/film.py` & `libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/film.py`

 * *Files identical despite different names*

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/flow/lib.py` & `libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/lib.py`

 * *Files identical despite different names*

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/flow/users.py` & `libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/users.py`

 * *Files identical despite different names*

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/resources/file_templates/template.blend` & `libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/file_templates/template.blend`

 * *Files identical despite different names*

### Comparing `libreflow.flows-2.1.0.1/src/libreflow/flows/tinykin/resources/icons/flow/publish-ok.png` & `libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/icons/flow/publish-ok.png`

 * *Files identical despite different names*

### Comparing `libreflow.flows-2.1.0.1/src/libreflow.flows.egg-info/PKG-INFO` & `libreflow_flows-2.1.1/src/libreflow.flows.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.flows
-Version: 2.1.0.1
+Version: 2.1.1
 Summary: A set of flows specific to projects handled by Libreflow at Les Fées Spéciales.
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow.flows
 Author: Baptiste Delos, Flavio Perez
 Author-email: baptiste@les-fees-speciales.coop, flavio@lfs.coop
 License: LGPLv3+
 Keywords: kabaret cgwire kitsu gazu animation pipeline libreflow
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,24 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [2.1.1] - 2024-04-26
+
+### Added
+
+* Create Shots, Asset Types and Assets from Kitsu: for existing entities, default tasks are now updated, in case new tasks need to be added.
+
+### Changed
+
+* Improved log messages for create objects from Kitsu actions.
+
 ## [2.1.0] - 2024-10-01
 
 ### Added
 
 * Creation of shots and assets from Kitsu: an option can be checked to create the task default files enabled by default in the task manager.
 * File references are now stored in a collection in the project's entity manager.
 * The session provides a new command-line option `--search-auto-indexing` to enable the search engine's automatic indexing. This feature can also be enabled by defining the `SEARCH_AUTO_INDEXING` variable in the environment of the session launch script.
```

### Comparing `libreflow.flows-2.1.0.1/src/libreflow.flows.egg-info/SOURCES.txt` & `libreflow_flows-2.1.1/src/libreflow.flows.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 src/libreflow/flows/default/flow/film.py
 src/libreflow/flows/default/flow/shot.py
 src/libreflow/flows/default/flow/task.py
 src/libreflow/flows/default/flow/user.py
 src/libreflow/flows/resources/__init__.py
 src/libreflow/flows/resources/file_templates/__init__.py
 src/libreflow/flows/resources/file_templates/template.blend
+src/libreflow/flows/resources/file_templates/template.wav
 src/libreflow/flows/resources/gifs/__init__.py
 src/libreflow/flows/resources/gifs/magic_word.gif
 src/libreflow/flows/resources/gui/__init__.py
 src/libreflow/flows/resources/gui/styles/__init__.py
 src/libreflow/flows/resources/gui/styles/default_style/__init__.py
 src/libreflow/flows/resources/gui/styles/default_style/default_style.css
 src/libreflow/flows/tinykin/__init__.py
```

### Comparing `libreflow.flows-2.1.0.1/versioneer.py` & `libreflow_flows-2.1.1/versioneer.py`

 * *Files identical despite different names*

