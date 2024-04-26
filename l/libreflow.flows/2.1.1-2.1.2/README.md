# Comparing `tmp/libreflow_flows-2.1.1.tar.gz` & `tmp/libreflow_flows-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreflow_flows-2.1.1.tar", last modified: Fri Apr 26 09:12:37 2024, max compression
+gzip compressed data, was "libreflow_flows-2.1.2.tar", last modified: Fri Apr 26 13:59:24 2024, max compression
```

## Comparing `libreflow_flows-2.1.1.tar` & `libreflow_flows-2.1.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.444964 libreflow_flows-2.1.1/
--rw-rw-rw-   0 root         (0) root         (0)      480 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)     4385 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1053 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5265 2024-04-26 09:12:37.444964 libreflow_flows-2.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      192 2024-04-26 09:12:37.444964 libreflow_flows-2.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2060 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.428964 libreflow_flows-2.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.433964 libreflow_flows-2.1.1/src/libreflow/
--rw-rw-rw-   0 root         (0) root         (0)       64 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.445964 libreflow_flows-2.1.1/src/libreflow/flows/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2024-04-26 09:12:37.445964 libreflow_flows-2.1.1/src/libreflow/flows/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.435964 libreflow_flows-2.1.1/src/libreflow/flows/custom_home/
--rw-rw-rw-   0 root         (0) root         (0)     6343 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/custom_home/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7386 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/custom_home/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.436964 libreflow_flows-2.1.1/src/libreflow/flows/default/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/default/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.437964 libreflow_flows-2.1.1/src/libreflow/flows/default/flow/
--rw-rw-rw-   0 root         (0) root         (0)     7258 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/default/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5816 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/default/flow/asset.py
--rw-rw-rw-   0 root         (0) root         (0)     1784 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/default/flow/entity_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    16548 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/default/flow/file.py
--rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/default/flow/film.py
--rw-rw-rw-   0 root         (0) root         (0)     2757 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/default/flow/shot.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/default/flow/task.py
--rw-rw-rw-   0 root         (0) root         (0)     7961 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/default/flow/user.py
--rw-rw-rw-   0 root         (0) root         (0)     5156 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/gui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.438964 libreflow_flows-2.1.1/src/libreflow/flows/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.439964 libreflow_flows-2.1.1/src/libreflow/flows/resources/file_templates/
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/file_templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   149688 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/file_templates/template.blend
--rw-rw-rw-   0 root         (0) root         (0)    88244 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/file_templates/template.wav
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.439964 libreflow_flows-2.1.1/src/libreflow/flows/resources/gifs/
--rw-rw-rw-   0 root         (0) root         (0)      144 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/gifs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   744158 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/gifs/magic_word.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.440964 libreflow_flows-2.1.1/src/libreflow/flows/resources/gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/gui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.440964 libreflow_flows-2.1.1/src/libreflow/flows/resources/gui/styles/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/gui/styles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.440964 libreflow_flows-2.1.1/src/libreflow/flows/resources/gui/styles/default_style/
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/gui/styles/default_style/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8358 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/resources/gui/styles/default_style/default_style.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.441964 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.442964 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/
--rw-rw-rw-   0 root         (0) root         (0)     5702 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13809 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/file.py
--rw-rw-rw-   0 root         (0) root         (0)    45139 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/film.py
--rw-rw-rw-   0 root         (0) root         (0)    22662 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     3125 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/users.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.442964 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.443964 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/file_templates/
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/file_templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    94110 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/file_templates/template.blend
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.443964 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/icons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.443964 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/icons/flow/
--rw-rw-rw-   0 root         (0) root         (0)      163 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/icons/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1287 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/icons/flow/publish-ok.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:12:37.444964 libreflow_flows-2.1.1/src/libreflow.flows.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5265 2024-04-26 09:12:37.000000 libreflow_flows-2.1.1/src/libreflow.flows.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2072 2024-04-26 09:12:37.000000 libreflow_flows-2.1.1/src/libreflow.flows.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 09:12:37.000000 libreflow_flows-2.1.1/src/libreflow.flows.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-26 09:12:37.000000 libreflow_flows-2.1.1/src/libreflow.flows.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-26 09:12:37.000000 libreflow_flows-2.1.1/src/libreflow.flows.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    80044 2024-04-26 09:12:28.000000 libreflow_flows-2.1.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.299532 libreflow_flows-2.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)      480 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)     4563 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5443 2024-04-26 13:59:24.299532 libreflow_flows-2.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      192 2024-04-26 13:59:24.299532 libreflow_flows-2.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2060 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.282532 libreflow_flows-2.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.287532 libreflow_flows-2.1.2/src/libreflow/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.299532 libreflow_flows-2.1.2/src/libreflow/flows/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2024-04-26 13:59:24.300532 libreflow_flows-2.1.2/src/libreflow/flows/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.290532 libreflow_flows-2.1.2/src/libreflow/flows/custom_home/
+-rw-rw-rw-   0 root         (0) root         (0)     6343 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/custom_home/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7386 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/custom_home/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.290532 libreflow_flows-2.1.2/src/libreflow/flows/default/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/default/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.292532 libreflow_flows-2.1.2/src/libreflow/flows/default/flow/
+-rw-rw-rw-   0 root         (0) root         (0)     7258 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/default/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5816 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/default/flow/asset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1784 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/default/flow/entity_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    16548 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/default/flow/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/default/flow/film.py
+-rw-rw-rw-   0 root         (0) root         (0)     2757 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/default/flow/shot.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/default/flow/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     7961 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/default/flow/user.py
+-rw-rw-rw-   0 root         (0) root         (0)     5156 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/gui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.293532 libreflow_flows-2.1.2/src/libreflow/flows/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.293532 libreflow_flows-2.1.2/src/libreflow/flows/resources/file_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/file_templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   149688 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/file_templates/template.blend
+-rw-rw-rw-   0 root         (0) root         (0)    88244 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/file_templates/template.wav
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.294532 libreflow_flows-2.1.2/src/libreflow/flows/resources/gifs/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/gifs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   744158 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/gifs/magic_word.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.295532 libreflow_flows-2.1.2/src/libreflow/flows/resources/gui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/gui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.295532 libreflow_flows-2.1.2/src/libreflow/flows/resources/gui/styles/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/gui/styles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.295532 libreflow_flows-2.1.2/src/libreflow/flows/resources/gui/styles/default_style/
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/gui/styles/default_style/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8358 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/resources/gui/styles/default_style/default_style.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.296532 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.297532 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/
+-rw-rw-rw-   0 root         (0) root         (0)     5702 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13809 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/file.py
+-rw-rw-rw-   0 root         (0) root         (0)    45139 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/film.py
+-rw-rw-rw-   0 root         (0) root         (0)    22662 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     3125 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/users.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.297532 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.297532 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/file_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/file_templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    94110 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/file_templates/template.blend
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.298532 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/icons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.298532 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/icons/flow/
+-rw-rw-rw-   0 root         (0) root         (0)      163 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/icons/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/icons/flow/publish-ok.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:59:24.298532 libreflow_flows-2.1.2/src/libreflow.flows.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5443 2024-04-26 13:59:24.000000 libreflow_flows-2.1.2/src/libreflow.flows.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-04-26 13:59:24.000000 libreflow_flows-2.1.2/src/libreflow.flows.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 13:59:24.000000 libreflow_flows-2.1.2/src/libreflow.flows.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-26 13:59:24.000000 libreflow_flows-2.1.2/src/libreflow.flows.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-26 13:59:24.000000 libreflow_flows-2.1.2/src/libreflow.flows.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    80044 2024-04-26 13:59:15.000000 libreflow_flows-2.1.2/versioneer.py
```

### Comparing `libreflow_flows-2.1.1/CHANGELOG.md` & `libreflow_flows-2.1.2/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [2.1.2] - 2024-04-26
+
+### Fixed
+
+* Block libreflow minor version to 2.3 to prevent libreflow 2.4.0 or any versions above (introducing breaking changes) from being installed.
+
 ## [2.1.1] - 2024-04-26
 
 ### Added
 
 * Create Shots, Asset Types and Assets from Kitsu: for existing entities, default tasks are now updated, in case new tasks need to be added.
 
 ### Changed
```

### Comparing `libreflow_flows-2.1.1/LICENSE` & `libreflow_flows-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/PKG-INFO` & `libreflow_flows-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.flows
-Version: 2.1.1
+Version: 2.1.2
 Summary: A set of flows specific to projects handled by Libreflow at Les Fées Spéciales.
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow.flows
 Author: Baptiste Delos, Flavio Perez
 Author-email: baptiste@les-fees-speciales.coop, flavio@lfs.coop
 License: LGPLv3+
 Keywords: kabaret cgwire kitsu gazu animation pipeline libreflow
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [2.1.2] - 2024-04-26
+
+### Fixed
+
+* Block libreflow minor version to 2.3 to prevent libreflow 2.4.0 or any versions above (introducing breaking changes) from being installed.
+
 ## [2.1.1] - 2024-04-26
 
 ### Added
 
 * Create Shots, Asset Types and Assets from Kitsu: for existing entities, default tasks are now updated, in case new tasks need to be added.
 
 ### Changed
```

### Comparing `libreflow_flows-2.1.1/setup.py` & `libreflow_flows-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/custom_home/__init__.py` & `libreflow_flows-2.1.2/src/libreflow/flows/custom_home/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/custom_home/ui.py` & `libreflow_flows-2.1.2/src/libreflow/flows/custom_home/ui.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/default/flow/__init__.py` & `libreflow_flows-2.1.2/src/libreflow/flows/default/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/default/flow/asset.py` & `libreflow_flows-2.1.2/src/libreflow/flows/default/flow/asset.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/default/flow/entity_manager.py` & `libreflow_flows-2.1.2/src/libreflow/flows/default/flow/entity_manager.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/default/flow/file.py` & `libreflow_flows-2.1.2/src/libreflow/flows/default/flow/file.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/default/flow/film.py` & `libreflow_flows-2.1.2/src/libreflow/flows/default/flow/film.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/default/flow/shot.py` & `libreflow_flows-2.1.2/src/libreflow/flows/default/flow/shot.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/default/flow/user.py` & `libreflow_flows-2.1.2/src/libreflow/flows/default/flow/user.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/gui.py` & `libreflow_flows-2.1.2/src/libreflow/flows/gui.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/resources/file_templates/template.blend` & `libreflow_flows-2.1.2/src/libreflow/flows/resources/file_templates/template.blend`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/resources/file_templates/template.wav` & `libreflow_flows-2.1.2/src/libreflow/flows/resources/file_templates/template.wav`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/resources/gifs/magic_word.gif` & `libreflow_flows-2.1.2/src/libreflow/flows/resources/gifs/magic_word.gif`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/resources/gui/styles/default_style/__init__.py` & `libreflow_flows-2.1.2/src/libreflow/flows/resources/gui/styles/default_style/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/resources/gui/styles/default_style/default_style.css` & `libreflow_flows-2.1.2/src/libreflow/flows/resources/gui/styles/default_style/default_style.css`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/__init__.py` & `libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/file.py` & `libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/file.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/film.py` & `libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/film.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/lib.py` & `libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/lib.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/tinykin/flow/users.py` & `libreflow_flows-2.1.2/src/libreflow/flows/tinykin/flow/users.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/file_templates/template.blend` & `libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/file_templates/template.blend`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow/flows/tinykin/resources/icons/flow/publish-ok.png` & `libreflow_flows-2.1.2/src/libreflow/flows/tinykin/resources/icons/flow/publish-ok.png`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/src/libreflow.flows.egg-info/PKG-INFO` & `libreflow_flows-2.1.2/src/libreflow.flows.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.flows
-Version: 2.1.1
+Version: 2.1.2
 Summary: A set of flows specific to projects handled by Libreflow at Les Fées Spéciales.
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow.flows
 Author: Baptiste Delos, Flavio Perez
 Author-email: baptiste@les-fees-speciales.coop, flavio@lfs.coop
 License: LGPLv3+
 Keywords: kabaret cgwire kitsu gazu animation pipeline libreflow
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [2.1.2] - 2024-04-26
+
+### Fixed
+
+* Block libreflow minor version to 2.3 to prevent libreflow 2.4.0 or any versions above (introducing breaking changes) from being installed.
+
 ## [2.1.1] - 2024-04-26
 
 ### Added
 
 * Create Shots, Asset Types and Assets from Kitsu: for existing entities, default tasks are now updated, in case new tasks need to be added.
 
 ### Changed
```

### Comparing `libreflow_flows-2.1.1/src/libreflow.flows.egg-info/SOURCES.txt` & `libreflow_flows-2.1.2/src/libreflow.flows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.1.1/versioneer.py` & `libreflow_flows-2.1.2/versioneer.py`

 * *Files identical despite different names*

