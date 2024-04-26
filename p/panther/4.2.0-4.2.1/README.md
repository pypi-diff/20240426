# Comparing `tmp/panther-4.2.0.tar.gz` & `tmp/panther-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panther-4.2.0.tar", last modified: Sat Apr 13 16:21:00 2024, max compression
+gzip compressed data, was "panther-4.2.1.tar", last modified: Fri Apr 26 13:43:19 2024, max compression
```

## Comparing `panther-4.2.0.tar` & `panther-4.2.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:21:00.673551 panther-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-13 16:20:52.000000 panther-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-13 16:21:00.673551 panther-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-13 16:20:52.000000 panther-4.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:21:00.665551 panther-4.2.0/panther/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-13 16:20:52.000000 panther-4.2.0/panther/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-13 16:20:52.000000 panther-4.2.0/panther/_load_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-13 16:20:52.000000 panther-4.2.0/panther/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-04-13 16:20:52.000000 panther-4.2.0/panther/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-13 16:20:52.000000 panther-4.2.0/panther/authentications.py
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-13 16:20:52.000000 panther-4.2.0/panther/background_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-13 16:20:52.000000 panther-4.2.0/panther/base_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-04-13 16:20:52.000000 panther-4.2.0/panther/base_websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-13 16:20:52.000000 panther-4.2.0/panther/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:21:00.665551 panther-4.2.0/panther/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:52.000000 panther-4.2.0/panther/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10292 2024-04-13 16:20:52.000000 panther-4.2.0/panther/cli/create_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-13 16:20:52.000000 panther-4.2.0/panther/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-13 16:20:52.000000 panther-4.2.0/panther/cli/monitor_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-13 16:20:52.000000 panther-4.2.0/panther/cli/run_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-13 16:20:52.000000 panther-4.2.0/panther/cli/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-13 16:20:52.000000 panther-4.2.0/panther/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-13 16:20:52.000000 panther-4.2.0/panther/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:21:00.665551 panther-4.2.0/panther/db/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:21:00.669551 panther-4.2.0/panther/db/queries/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/queries/base_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/queries/mongodb_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/queries/pantherdb_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/queries/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-13 16:20:52.000000 panther-4.2.0/panther/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-13 16:20:52.000000 panther-4.2.0/panther/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-13 16:20:52.000000 panther-4.2.0/panther/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-13 16:20:52.000000 panther-4.2.0/panther/generics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-13 16:20:52.000000 panther-4.2.0/panther/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-13 16:20:52.000000 panther-4.2.0/panther/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:21:00.669551 panther-4.2.0/panther/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-13 16:20:52.000000 panther-4.2.0/panther/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-13 16:20:52.000000 panther-4.2.0/panther/middlewares/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-13 16:20:52.000000 panther-4.2.0/panther/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-13 16:20:52.000000 panther-4.2.0/panther/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:21:00.669551 panther-4.2.0/panther/panel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:52.000000 panther-4.2.0/panther/panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-13 16:20:52.000000 panther-4.2.0/panther/panel/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-13 16:20:52.000000 panther-4.2.0/panther/panel/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-13 16:20:52.000000 panther-4.2.0/panther/panel/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-13 16:20:52.000000 panther-4.2.0/panther/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-13 16:20:52.000000 panther-4.2.0/panther/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-04-13 16:20:52.000000 panther-4.2.0/panther/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-13 16:20:52.000000 panther-4.2.0/panther/routings.py
--rw-r--r--   0 runner    (1001) docker     (127)     9096 2024-04-13 16:20:52.000000 panther-4.2.0/panther/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-13 16:20:52.000000 panther-4.2.0/panther/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-13 16:20:52.000000 panther-4.2.0/panther/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-13 16:20:52.000000 panther-4.2.0/panther/throttling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-13 16:20:52.000000 panther-4.2.0/panther/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-13 16:20:52.000000 panther-4.2.0/panther/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:21:00.673551 panther-4.2.0/panther.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-13 16:21:00.000000 panther-4.2.0/panther.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-13 16:21:00.000000 panther-4.2.0/panther.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:21:00.000000 panther-4.2.0/panther.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-13 16:21:00.000000 panther-4.2.0/panther.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-13 16:21:00.000000 panther-4.2.0/panther.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-13 16:21:00.000000 panther-4.2.0/panther.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-13 16:20:52.000000 panther-4.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 16:21:00.673551 panther-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-13 16:20:52.000000 panther-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:21:00.673551 panther-4.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_background_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    16071 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_generics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_multipart.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_panel_apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17425 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    30959 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    13457 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_throttling.py
--rw-r--r--   0 runner    (1001) docker     (127)    12984 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11207 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_websockets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:43:19.087301 panther-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-26 13:43:04.000000 panther-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-26 13:43:19.087301 panther-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-26 13:43:04.000000 panther-4.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:43:19.079300 panther-4.2.1/panther/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-26 13:43:04.000000 panther-4.2.1/panther/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-26 13:43:04.000000 panther-4.2.1/panther/_load_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-26 13:43:04.000000 panther-4.2.1/panther/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-04-26 13:43:04.000000 panther-4.2.1/panther/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-26 13:43:04.000000 panther-4.2.1/panther/authentications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-26 13:43:04.000000 panther-4.2.1/panther/background_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-26 13:43:04.000000 panther-4.2.1/panther/base_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-04-26 13:43:04.000000 panther-4.2.1/panther/base_websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-26 13:43:04.000000 panther-4.2.1/panther/caching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:43:19.079300 panther-4.2.1/panther/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:43:04.000000 panther-4.2.1/panther/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10292 2024-04-26 13:43:04.000000 panther-4.2.1/panther/cli/create_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-26 13:43:04.000000 panther-4.2.1/panther/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-26 13:43:04.000000 panther-4.2.1/panther/cli/monitor_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-26 13:43:04.000000 panther-4.2.1/panther/cli/run_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-26 13:43:04.000000 panther-4.2.1/panther/cli/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-26 13:43:04.000000 panther-4.2.1/panther/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-26 13:43:04.000000 panther-4.2.1/panther/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:43:19.079300 panther-4.2.1/panther/db/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-26 13:43:04.000000 panther-4.2.1/panther/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-26 13:43:04.000000 panther-4.2.1/panther/db/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-26 13:43:04.000000 panther-4.2.1/panther/db/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-26 13:43:04.000000 panther-4.2.1/panther/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:43:19.083300 panther-4.2.1/panther/db/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-26 13:43:04.000000 panther-4.2.1/panther/db/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-26 13:43:04.000000 panther-4.2.1/panther/db/queries/base_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-26 13:43:04.000000 panther-4.2.1/panther/db/queries/mongodb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-04-26 13:43:04.000000 panther-4.2.1/panther/db/queries/pantherdb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-04-26 13:43:04.000000 panther-4.2.1/panther/db/queries/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-26 13:43:04.000000 panther-4.2.1/panther/db/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-26 13:43:04.000000 panther-4.2.1/panther/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-26 13:43:04.000000 panther-4.2.1/panther/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-26 13:43:04.000000 panther-4.2.1/panther/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-26 13:43:04.000000 panther-4.2.1/panther/generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-26 13:43:04.000000 panther-4.2.1/panther/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-26 13:43:04.000000 panther-4.2.1/panther/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:43:19.083300 panther-4.2.1/panther/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-26 13:43:04.000000 panther-4.2.1/panther/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-26 13:43:04.000000 panther-4.2.1/panther/middlewares/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-26 13:43:04.000000 panther-4.2.1/panther/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-26 13:43:04.000000 panther-4.2.1/panther/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:43:19.083300 panther-4.2.1/panther/panel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:43:04.000000 panther-4.2.1/panther/panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-26 13:43:04.000000 panther-4.2.1/panther/panel/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-26 13:43:04.000000 panther-4.2.1/panther/panel/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-26 13:43:04.000000 panther-4.2.1/panther/panel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-26 13:43:04.000000 panther-4.2.1/panther/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-26 13:43:04.000000 panther-4.2.1/panther/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-04-26 13:43:04.000000 panther-4.2.1/panther/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-26 13:43:04.000000 panther-4.2.1/panther/routings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9096 2024-04-26 13:43:04.000000 panther-4.2.1/panther/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-26 13:43:04.000000 panther-4.2.1/panther/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-26 13:43:04.000000 panther-4.2.1/panther/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-26 13:43:04.000000 panther-4.2.1/panther/throttling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-26 13:43:04.000000 panther-4.2.1/panther/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-26 13:43:04.000000 panther-4.2.1/panther/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:43:19.087301 panther-4.2.1/panther.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-26 13:43:19.000000 panther-4.2.1/panther.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-26 13:43:19.000000 panther-4.2.1/panther.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:43:19.000000 panther-4.2.1/panther.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 13:43:19.000000 panther-4.2.1/panther.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-26 13:43:19.000000 panther-4.2.1/panther.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 13:43:19.000000 panther-4.2.1/panther.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-26 13:43:04.000000 panther-4.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 13:43:19.087301 panther-4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-26 13:43:04.000000 panther-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:43:19.087301 panther-4.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-26 13:43:04.000000 panther-4.2.1/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-26 13:43:04.000000 panther-4.2.1/tests/test_background_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-26 13:43:04.000000 panther-4.2.1/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-26 13:43:04.000000 panther-4.2.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16071 2024-04-26 13:43:04.000000 panther-4.2.1/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-26 13:43:04.000000 panther-4.2.1/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-04-26 13:43:04.000000 panther-4.2.1/tests/test_generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-26 13:43:04.000000 panther-4.2.1/tests/test_multipart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-26 13:43:04.000000 panther-4.2.1/tests/test_panel_apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-04-26 13:43:04.000000 panther-4.2.1/tests/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17425 2024-04-26 13:43:04.000000 panther-4.2.1/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30959 2024-04-26 13:43:04.000000 panther-4.2.1/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-26 13:43:04.000000 panther-4.2.1/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13457 2024-04-26 13:43:04.000000 panther-4.2.1/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-26 13:43:04.000000 panther-4.2.1/tests/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-26 13:43:04.000000 panther-4.2.1/tests/test_throttling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12984 2024-04-26 13:43:04.000000 panther-4.2.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11207 2024-04-26 13:43:04.000000 panther-4.2.1/tests/test_websockets.py
```

### Comparing `panther-4.2.0/LICENSE` & `panther-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/PKG-INFO` & `panther-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panther
-Version: 4.2.0
+Version: 4.2.1
 Summary: Fast &  Friendly, Web Framework For Building Async APIs
 Home-page: https://github.com/alirn76/panther
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: BSD-3-Clause license
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `panther-4.2.0/README.md` & `panther-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/_load_configs.py` & `panther-4.2.1/panther/_load_configs.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/_utils.py` & `panther-4.2.1/panther/_utils.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/app.py` & `panther-4.2.1/panther/app.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/authentications.py` & `panther-4.2.1/panther/authentications.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/background_tasks.py` & `panther-4.2.1/panther/background_tasks.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/base_request.py` & `panther-4.2.1/panther/base_request.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/base_websocket.py` & `panther-4.2.1/panther/base_websocket.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/caching.py` & `panther-4.2.1/panther/caching.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/cli/create_command.py` & `panther-4.2.1/panther/cli/create_command.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/cli/main.py` & `panther-4.2.1/panther/cli/main.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/cli/monitor_command.py` & `panther-4.2.1/panther/cli/monitor_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import contextlib
 import logging
 import os
+import platform
 import signal
 from collections import deque
 from pathlib import Path
 
 from rich import box
 from rich.align import Align
 from rich.console import Group
@@ -39,15 +40,20 @@
                 vertical_overflow='visible',
                 screen=True,
             ) as live,
             contextlib.suppress(KeyboardInterrupt)
         ):
             f.readlines()  # Set cursor at the end of the file
 
-            for _ in watch(self.monitoring_log_file):
+            if platform.system() == 'Windows':
+                watching = watch(self.monitoring_log_file, force_polling=True)
+            else:
+                watching = watch(self.monitoring_log_file)
+
+            for _ in watching:
                 for line in f.readlines():
                     self.rows.append(line.split('|'))
                     live.update(self.generate_table())
 
     def initialize(self) -> str:
         # Check requirements
         try:
@@ -59,15 +65,16 @@
         if not self.monitoring_log_file.exists():
             return f'`{self.monitoring_log_file}` file not found. (Make sure `MONITORING` is `True` in `configs` and you have at least one record)'
 
         # Initialize Deque
         self.update_rows()
 
         # Register the signal handler
-        signal.signal(signal.SIGWINCH, self.update_rows)
+        if platform.system() != 'Windows':
+            signal.signal(signal.SIGWINCH, self.update_rows)
 
     def generate_table(self) -> Panel:
         # 2023-03-24 01:42:52 | GET | /user/317/ | 127.0.0.1:48856 |  0.0366 ms | 200
 
         table = Table(box=box.MINIMAL_DOUBLE_HEAD)
         table.add_column('Datetime', justify='center', style='magenta', no_wrap=True)
         table.add_column('Method', justify='center', style='cyan', no_wrap=True)
```

### Comparing `panther-4.2.0/panther/cli/run_command.py` & `panther-4.2.1/panther/cli/run_command.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/cli/template.py` & `panther-4.2.1/panther/cli/template.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/cli/utils.py` & `panther-4.2.1/panther/cli/utils.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/configs.py` & `panther-4.2.1/panther/configs.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/db/connections.py` & `panther-4.2.1/panther/db/connections.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/db/cursor.py` & `panther-4.2.1/panther/db/cursor.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/db/models.py` & `panther-4.2.1/panther/db/models.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/db/queries/base_queries.py` & `panther-4.2.1/panther/db/queries/base_queries.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/db/queries/mongodb_queries.py` & `panther-4.2.1/panther/db/queries/mongodb_queries.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/db/queries/pantherdb_queries.py` & `panther-4.2.1/panther/db/queries/pantherdb_queries.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/db/queries/queries.py` & `panther-4.2.1/panther/db/queries/queries.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/db/utils.py` & `panther-4.2.1/panther/db/utils.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/events.py` & `panther-4.2.1/panther/events.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/exceptions.py` & `panther-4.2.1/panther/exceptions.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/file_handler.py` & `panther-4.2.1/panther/file_handler.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/generics.py` & `panther-4.2.1/panther/generics.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/logging.py` & `panther-4.2.1/panther/logging.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/main.py` & `panther-4.2.1/panther/main.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/middlewares/base.py` & `panther-4.2.1/panther/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/monitoring.py` & `panther-4.2.1/panther/monitoring.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/pagination.py` & `panther-4.2.1/panther/pagination.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/panel/apis.py` & `panther-4.2.1/panther/panel/apis.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/request.py` & `panther-4.2.1/panther/request.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/response.py` & `panther-4.2.1/panther/response.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/routings.py` & `panther-4.2.1/panther/routings.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/serializer.py` & `panther-4.2.1/panther/serializer.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/status.py` & `panther-4.2.1/panther/status.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/test.py` & `panther-4.2.1/panther/test.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/utils.py` & `panther-4.2.1/panther/utils.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther/websocket.py` & `panther-4.2.1/panther/websocket.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/panther.egg-info/PKG-INFO` & `panther-4.2.1/panther.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panther
-Version: 4.2.0
+Version: 4.2.1
 Summary: Fast &  Friendly, Web Framework For Building Async APIs
 Home-page: https://github.com/alirn76/panther
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: BSD-3-Clause license
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `panther-4.2.0/panther.egg-info/SOURCES.txt` & `panther-4.2.1/panther.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/setup.py` & `panther-4.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/tests/test_authentication.py` & `panther-4.2.1/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/tests/test_background_tasks.py` & `panther-4.2.1/tests/test_background_tasks.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/tests/test_caching.py` & `panther-4.2.1/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/tests/test_cli.py` & `panther-4.2.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/tests/test_database.py` & `panther-4.2.1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/tests/test_events.py` & `panther-4.2.1/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/tests/test_generics.py` & `panther-4.2.1/tests/test_generics.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/tests/test_multipart.py` & `panther-4.2.1/tests/test_multipart.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/tests/test_panel_apis.py` & `panther-4.2.1/tests/test_panel_apis.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/tests/test_request.py` & `panther-4.2.1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/tests/test_response.py` & `panther-4.2.1/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/tests/test_routing.py` & `panther-4.2.1/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/tests/test_run.py` & `panther-4.2.1/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/tests/test_serializer.py` & `panther-4.2.1/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/tests/test_status.py` & `panther-4.2.1/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/tests/test_throttling.py` & `panther-4.2.1/tests/test_throttling.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/tests/test_utils.py` & `panther-4.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `panther-4.2.0/tests/test_websockets.py` & `panther-4.2.1/tests/test_websockets.py`

 * *Files identical despite different names*

