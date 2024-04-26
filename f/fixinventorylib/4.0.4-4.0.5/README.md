# Comparing `tmp/fixinventorylib-4.0.4.tar.gz` & `tmp/fixinventorylib-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventorylib-4.0.4.tar", last modified: Wed Apr 24 19:31:24 2024, max compression
+gzip compressed data, was "fixinventorylib-4.0.5.tar", last modified: Fri Apr 26 20:26:49 2024, max compression
```

## Comparing `fixinventorylib-4.0.4.tar` & `fixinventorylib-4.0.5.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:24.293125 fixinventorylib-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-24 19:31:24.293125 fixinventorylib-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:24.289125 fixinventorylib-4.0.4/fixinventorylib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-24 19:31:24.000000 fixinventorylib-4.0.4/fixinventorylib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-24 19:31:24.000000 fixinventorylib-4.0.4/fixinventorylib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:31:24.000000 fixinventorylib-4.0.4/fixinventorylib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:27:57.000000 fixinventorylib-4.0.4/fixinventorylib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-24 19:31:24.000000 fixinventorylib-4.0.4/fixinventorylib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 19:31:24.000000 fixinventorylib-4.0.4/fixinventorylib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:24.281125 fixinventorylib-4.0.4/fixlib/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:24.281125 fixinventorylib-4.0.4/fixlib/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/asynchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/asynchronous/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:24.285125 fixinventorylib-4.0.4/fixlib/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/asynchronous/web/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/asynchronous/web/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/baseplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    50078 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/baseresources.py
--rw-r--r--   0 runner    (1001) docker     (127)    17402 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:24.285125 fixinventorylib-4.0.4/fixlib/core/
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/core/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/core/ca.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/core/custom_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/core/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/core/model_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    16100 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/core/model_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/core/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/core/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8679 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/durations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:24.285125 fixinventorylib-4.0.4/fixlib/graph/
--rw-r--r--   0 runner    (1001) docker     (127)    28662 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/graph/graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    17747 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/json_bender.py
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/lock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:24.285125 fixinventorylib-4.0.4/fixlib/log/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/parse_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/proc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/threading.py
--rw-r--r--   0 runner    (1001) docker     (127)    33802 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/units.py
--rw-r--r--   0 runner    (1001) docker     (127)    20401 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:24.285125 fixinventorylib-4.0.4/fixlib/web/
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/web/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:24.289125 fixinventorylib-4.0.4/fixlib/web/static/
--rw-r--r--   0 runner    (1001) docker     (127)    14848 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/web/static/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    31503 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/web/static/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/web/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/web/static/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/web/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/web/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/web/static/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/web/static/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (127)    39028 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/web/static/picnic.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/web/static/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/fixlib/x509.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-24 19:31:24.293125 fixinventorylib-4.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:24.289125 fixinventorylib-4.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/test/test_baseresources.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/test/test_ca.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/test/test_graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/test/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/test/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    21349 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/test/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    17394 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-24 19:27:06.000000 fixinventorylib-4.0.4/test/test_x509.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:26:49.486448 fixinventorylib-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-26 20:26:49.486448 fixinventorylib-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:26:49.482448 fixinventorylib-4.0.5/fixinventorylib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-26 20:26:49.000000 fixinventorylib-4.0.5/fixinventorylib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-26 20:26:49.000000 fixinventorylib-4.0.5/fixinventorylib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:26:49.000000 fixinventorylib-4.0.5/fixinventorylib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:23:16.000000 fixinventorylib-4.0.5/fixinventorylib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-26 20:26:49.000000 fixinventorylib-4.0.5/fixinventorylib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 20:26:49.000000 fixinventorylib-4.0.5/fixinventorylib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:26:49.474448 fixinventorylib-4.0.5/fixlib/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:26:49.474448 fixinventorylib-4.0.5/fixlib/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/asynchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/asynchronous/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:26:49.474448 fixinventorylib-4.0.5/fixlib/asynchronous/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/asynchronous/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/asynchronous/web/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/asynchronous/web/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/baseplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52662 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17402 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:26:49.478448 fixinventorylib-4.0.5/fixlib/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/core/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/core/ca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/core/custom_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/core/model_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16100 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/core/model_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/core/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8679 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/durations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:26:49.478448 fixinventorylib-4.0.5/fixlib/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)    28662 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/graph/graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17747 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/json_bender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/lock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:26:49.478448 fixinventorylib-4.0.5/fixlib/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/parse_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33802 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20401 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:26:49.478448 fixinventorylib-4.0.5/fixlib/web/
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/web/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:26:49.482448 fixinventorylib-4.0.5/fixlib/web/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14848 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/web/static/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31503 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/web/static/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/web/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/web/static/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/web/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/web/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/web/static/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/web/static/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39028 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/web/static/picnic.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/web/static/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/fixlib/x509.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-26 20:26:49.486448 fixinventorylib-4.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:26:49.482448 fixinventorylib-4.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/test/test_baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/test/test_ca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/test/test_graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/test/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/test/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21349 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/test/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17394 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-26 20:22:22.000000 fixinventorylib-4.0.5/test/test_x509.py
```

### Comparing `fixinventorylib-4.0.4/PKG-INFO` & `fixinventorylib-4.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventorylib
-Version: 4.0.4
+Version: 4.0.5
 Summary: Fix Inventory common library.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fixinventory/tree/main/fixlib
 Keywords: cloud security
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fixinventorylib-4.0.4/README.md` & `fixinventorylib-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixinventorylib.egg-info/PKG-INFO` & `fixinventorylib-4.0.5/fixinventorylib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventorylib
-Version: 4.0.4
+Version: 4.0.5
 Summary: Fix Inventory common library.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fixinventory/tree/main/fixlib
 Keywords: cloud security
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fixinventorylib-4.0.4/fixinventorylib.egg-info/SOURCES.txt` & `fixinventorylib-4.0.5/fixinventorylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/args.py` & `fixinventorylib-4.0.5/fixlib/args.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/asynchronous/utils.py` & `fixinventorylib-4.0.5/fixlib/asynchronous/utils.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/asynchronous/web/runner.py` & `fixinventorylib-4.0.5/fixlib/asynchronous/web/runner.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/asynchronous/web/ws_handler.py` & `fixinventorylib-4.0.5/fixlib/asynchronous/web/ws_handler.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/baseplugin.py` & `fixinventorylib-4.0.5/fixlib/baseplugin.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/baseresources.py` & `fixinventorylib-4.0.5/fixlib/baseresources.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,52 +121,103 @@
 
     # instances
     CpuUtilization = "cpu_utilization"
     NetworkIn = "network_in"
     NetworkOut = "network_out"
     DiskRead = "disk_read"
     DiskWrite = "disk_write"
+    ReadThroughput = "read_throughput"
+    WriteThroughput = "write_throughput"
 
     # volumes
     VolumeWrite = "volume_write"
     VolumeRead = "volume_read"
     VolumeTotalWriteTime = "volume_total_write_time"
     VolumeIdleTime = "volume_idle_time"
     VolumeQueueLength = "volume_queue_length"
+    NumberOfObjects = "number_of_objects"
+    BucketSizeBytes = "bucket_size"
 
     # load balancers
     RequestCount = "request"  # _count will be added to the end because of the unit
     ActiveConnection = "active_connection"
+    ConnectionAttemptCount = "connection_attempt"  # _count will be added to the end because of the unit
+    ConnectionEstablishedCount = "connection_established"  # _count will be added to the end because of the unit
     StatusCode2XX = "status_code_2xx"
     StatusCode4XX = "status_code_4xx"
     StatusCode5XX = "status_code_5xx"
     Latency = "latency"
     ProcessedBytes = "processed"  # _bytes will be added to the end because of the unit
     HealthyHostCount = "healthy_host"  # _count will be added to the end because of the unit
     UnhealthyHostCount = "unhealthy_host"  # _count will be added to the end because of the unit
     HealthyStateRouting = "healthy_state_routing"
     UnhealthyStateRouting = "unhealthy_state_routing"
     HealthyStateDNS = "healthy_state_dns"
     UnhealthyStateDNS = "unhealthy_state_dns"
+    RejectedConnectionCount = "rejected_connection"
+    IPv6RequestCount = "ipv6_request"
+    IPv6ProcessedBytes = "ipv6_processed"
+    ErrorPortAllocation = "error_port_allocation"
+    IdleTimeoutCount = "idle_timeout"  # _count will be added to the end because of the unit
+    PacketsDropCount = "packets_drop"  # _count will be added to the end because of the unit
+    PacketsInFromDestination = "packets_in_from_destination"
+    PacketsInFromSource = "packets_in_from_source"
+    PacketsOutToDestination = "packets_out_to_destination"
+    PacketsOutToSource = "packets_out_to_source"
+    BytesInFromDestination = "bytes_in_from_destination"
+    BytesInFromSource = "bytes_in_from_source"
+    BytesOutToDestination = "bytes_out_to_destination"
+    BytesOutToSource = "bytes_out_to_source"
+    RecordsBytes = "records"  # _bytes will be added to the end because of the unit
+    RecordsIteratorAgeMilliseconds = (
+        "records_iterator_age"  # _milliseconds will be added to the end because of the unit
+    )
 
     # databases
     DatabaseConnections = "database_connections"
     ReadLatency = "read_latency"
     WriteLatency = "write_latency"
     FreeStorageSpace = "free_storage_space"
+    FreeableMemory = "freeable_memory"
+    SwapUsage = "swap_usage"
+    DiskQueueDepth = "disk_queue_depth"
+    NetworkReceiveThroughput = "network_receive_throughput"
+    NetworkTransmitThroughput = "network_transmit_throughput"
+
+    # serverless
+    Invocations = "invocations"
+    Errors = "errors"
+    Throttles = "throttles"
+    Duration = "duration"
+    ConcurrentExecutions = "concurrent_executions"
+
+    # messages
+    NumberOfMessagesPublished = "number_of_messages_published"
+    NumberOfNotificationsDelivered = "number_of_notifications_delivered"
+    NumberOfNotificationsFailed = "number_of_notifications_failed"
+    PublishSize = "publish_size"
+    ApproximateAgeOfOldestMessage = "approximate_age_of_oldest_message"
+    ApproximateNumberOfMessagesDelayed = "approximate_number_of_messages_delayed"
+    ApproximateNumberOfMessagesNotVisible = "approximate_number_of_messages_not_visible"
+    ApproximateNumberOfMessagesVisible = "approximate_number_of_messages_visible"
+    NumberOfMessagesReceived = "number_of_messages_received"
+    NumberOfMessagesSent = "number_of_messages_sent"
 
 
 class MetricUnit(str, Enum):
     def __str__(self) -> str:
         return self.value
 
     Count = "count"
     Bytes = "bytes"
     Seconds = "seconds"
+    Milliseconds = "milliseconds"
     Percent = "percent"
+    BytesPerSecond = "BytesPs"
+    CountPerSecond = "CountPs"
     MegabitsPerSecond = "Mbps"
     MegabytesPerSecond = "MBps"
     PacketsPerSecond = "pps"
     IOPS = "iops"
 
 
 class StatName(str, Enum):
```

### Comparing `fixinventorylib-4.0.4/fixlib/config.py` & `fixinventorylib-4.0.5/fixlib/config.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/core/__init__.py` & `fixinventorylib-4.0.5/fixlib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/core/actions.py` & `fixinventorylib-4.0.5/fixlib/core/actions.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/core/ca.py` & `fixinventorylib-4.0.5/fixlib/core/ca.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/core/config.py` & `fixinventorylib-4.0.5/fixlib/core/config.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/core/custom_command.py` & `fixinventorylib-4.0.5/fixlib/core/custom_command.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/core/events.py` & `fixinventorylib-4.0.5/fixlib/core/events.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/core/model_check.py` & `fixinventorylib-4.0.5/fixlib/core/model_check.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/core/model_export.py` & `fixinventorylib-4.0.5/fixlib/core/model_export.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/core/progress.py` & `fixinventorylib-4.0.5/fixlib/core/progress.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/core/search.py` & `fixinventorylib-4.0.5/fixlib/core/search.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/core/tasks.py` & `fixinventorylib-4.0.5/fixlib/core/tasks.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/durations.py` & `fixinventorylib-4.0.5/fixlib/durations.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/event.py` & `fixinventorylib-4.0.5/fixlib/event.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/graph/__init__.py` & `fixinventorylib-4.0.5/fixlib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/graph/graph_extensions.py` & `fixinventorylib-4.0.5/fixlib/graph/graph_extensions.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/json.py` & `fixinventorylib-4.0.5/fixlib/json.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/json_bender.py` & `fixinventorylib-4.0.5/fixlib/json_bender.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/jwt.py` & `fixinventorylib-4.0.5/fixlib/jwt.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/lock.py` & `fixinventorylib-4.0.5/fixlib/lock.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/logger.py` & `fixinventorylib-4.0.5/fixlib/logger.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/parse_util.py` & `fixinventorylib-4.0.5/fixlib/parse_util.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/proc.py` & `fixinventorylib-4.0.5/fixlib/proc.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/threading.py` & `fixinventorylib-4.0.5/fixlib/threading.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/tree.py` & `fixinventorylib-4.0.5/fixlib/tree.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/utils.py` & `fixinventorylib-4.0.5/fixlib/utils.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/web/__init__.py` & `fixinventorylib-4.0.5/fixlib/web/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/web/metrics.py` & `fixinventorylib-4.0.5/fixlib/web/metrics.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/web/static/android-chrome-192x192.png` & `fixinventorylib-4.0.5/fixlib/web/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/web/static/android-chrome-512x512.png` & `fixinventorylib-4.0.5/fixlib/web/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/web/static/apple-touch-icon.png` & `fixinventorylib-4.0.5/fixlib/web/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/web/static/favicon-16x16.png` & `fixinventorylib-4.0.5/fixlib/web/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/web/static/favicon-32x32.png` & `fixinventorylib-4.0.5/fixlib/web/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/web/static/index.html` & `fixinventorylib-4.0.5/fixlib/web/static/index.html`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/web/static/mstile-150x150.png` & `fixinventorylib-4.0.5/fixlib/web/static/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/web/static/picnic.min.css` & `fixinventorylib-4.0.5/fixlib/web/static/picnic.min.css`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/fixlib/x509.py` & `fixinventorylib-4.0.5/fixlib/x509.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/pyproject.toml` & `fixinventorylib-4.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fixinventorylib"
-version = "4.0.4"
+version = "4.0.5"
 authors = [{ name = "Some Engineering Inc." }]
 description = "Fix Inventory common library."
 license = { text = "AGPLv3" }
 requires-python = ">=3.11"
 classifiers = [
     # Current project status
     "Development Status :: 5 - Production/Stable",
```

### Comparing `fixinventorylib-4.0.4/test/test_args.py` & `fixinventorylib-4.0.5/test/test_args.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/test/test_baseresources.py` & `fixinventorylib-4.0.5/test/test_baseresources.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/test/test_config.py` & `fixinventorylib-4.0.5/test/test_config.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/test/test_graph.py` & `fixinventorylib-4.0.5/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/test/test_graph_extensions.py` & `fixinventorylib-4.0.5/test/test_graph_extensions.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/test/test_json.py` & `fixinventorylib-4.0.5/test/test_json.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/test/test_jwt.py` & `fixinventorylib-4.0.5/test/test_jwt.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/test/test_plugin.py` & `fixinventorylib-4.0.5/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/test/test_tree.py` & `fixinventorylib-4.0.5/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/test/test_utils.py` & `fixinventorylib-4.0.5/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/test/test_web.py` & `fixinventorylib-4.0.5/test/test_web.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.4/test/test_x509.py` & `fixinventorylib-4.0.5/test/test_x509.py`

 * *Files identical despite different names*

