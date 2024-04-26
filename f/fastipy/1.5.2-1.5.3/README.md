# Comparing `tmp/fastipy-1.5.2.tar.gz` & `tmp/fastipy-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastipy-1.5.2.tar", last modified: Fri Apr 19 17:20:15 2024, max compression
+gzip compressed data, was "fastipy-1.5.3.tar", last modified: Fri Apr 26 18:27:59 2024, max compression
```

## Comparing `fastipy-1.5.2.tar` & `fastipy-1.5.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.506116 fastipy-1.5.2/
--rw-rw-rw-   0        0        0    35823 2024-04-14 01:52:52.000000 fastipy-1.5.2/LICENSE
--rw-rw-rw-   0        0        0     8007 2024-04-19 17:20:15.505123 fastipy-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     6755 2024-04-19 17:19:55.000000 fastipy-1.5.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.444010 fastipy-1.5.2/app/
-drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.452022 fastipy-1.5.2/app/fastipy/
--rw-rw-rw-   0        0        0      694 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.458535 fastipy-1.5.2/app/fastipy/src/
--rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.2/app/fastipy/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.463391 fastipy-1.5.2/app/fastipy/src/classes/
--rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.2/app/fastipy/src/classes/__init__.py
--rw-rw-rw-   0        0        0      484 2024-04-14 19:33:49.000000 fastipy-1.5.2/app/fastipy/src/classes/decorators_base.py
--rw-rw-rw-   0        0        0     6074 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/classes/json_database.py
--rw-rw-rw-   0        0        0     6751 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/classes/mailer.py
--rw-rw-rw-   0        0        0     3843 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/classes/template_render.py
-drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.470950 fastipy-1.5.2/app/fastipy/src/constants/
--rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.2/app/fastipy/src/constants/__init__.py
--rw-rw-rw-   0        0        0      802 2024-04-14 19:33:49.000000 fastipy-1.5.2/app/fastipy/src/constants/content_types.py
--rw-rw-rw-   0        0        0       42 2024-04-14 19:33:49.000000 fastipy-1.5.2/app/fastipy/src/constants/decorators.py
--rw-rw-rw-   0        0        0      108 2024-04-14 19:33:49.000000 fastipy-1.5.2/app/fastipy/src/constants/events.py
--rw-rw-rw-   0        0        0      164 2024-04-14 19:33:49.000000 fastipy-1.5.2/app/fastipy/src/constants/hooks.py
--rw-rw-rw-   0        0        0      171 2024-04-14 19:33:49.000000 fastipy-1.5.2/app/fastipy/src/constants/http_methods.py
--rw-rw-rw-   0        0        0     2957 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/constants/http_status_code.py
--rw-rw-rw-   0        0        0     1032 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/constants/serializers.py
-drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.475946 fastipy-1.5.2/app/fastipy/src/core/
--rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.2/app/fastipy/src/core/__init__.py
--rw-rw-rw-   0        0        0    20996 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/core/fastipy.py
--rw-rw-rw-   0        0        0    26458 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/core/reply.py
--rw-rw-rw-   0        0        0     5379 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/core/request.py
--rw-rw-rw-   0        0        0     7757 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/core/request_handler.py
-drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.486742 fastipy-1.5.2/app/fastipy/src/exceptions/
--rw-rw-rw-   0        0        0      918 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/__init__.py
--rw-rw-rw-   0        0        0      121 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/decorator_already_exists_exception.py
--rw-rw-rw-   0        0        0      113 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/duplicate_route_exception.py
--rw-rw-rw-   0        0        0     2458 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/exception_handler.py
--rw-rw-rw-   0        0        0      936 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/fastipy_exception.py
--rw-rw-rw-   0        0        0      103 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/file_exception.py
--rw-rw-rw-   0        0        0      110 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/invalid_path_exception.py
--rw-rw-rw-   0        0        0      110 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/no_event_type.py
--rw-rw-rw-   0        0        0      109 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/no_hook_type.py
--rw-rw-rw-   0        0        0      111 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/no_http_method_exception.py
--rw-rw-rw-   0        0        0      105 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/plugin_exception.py
--rw-rw-rw-   0        0        0      104 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/reply_exception.py
-drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.490551 fastipy-1.5.2/app/fastipy/src/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.2/app/fastipy/src/helpers/__init__.py
--rw-rw-rw-   0        0        0     1538 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/helpers/async_sync_helpers.py
--rw-rw-rw-   0        0        0      880 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/helpers/content_type.py
--rw-rw-rw-   0        0        0     2236 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/helpers/route_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.492550 fastipy-1.5.2/app/fastipy/src/middlewares/
--rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.2/app/fastipy/src/middlewares/__init__.py
--rw-rw-rw-   0        0        0     2591 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/middlewares/cors.py
-drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.496551 fastipy-1.5.2/app/fastipy/src/models/
--rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.2/app/fastipy/src/models/__init__.py
--rw-rw-rw-   0        0        0     2874 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/models/body.py
--rw-rw-rw-   0        0        0     4535 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/models/file.py
--rw-rw-rw-   0        0        0     2518 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/models/form.py
-drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.499111 fastipy-1.5.2/app/fastipy/src/routes/
--rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.2/app/fastipy/src/routes/__init__.py
--rw-rw-rw-   0        0        0     2212 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/routes/plugin_tree.py
--rw-rw-rw-   0        0        0     6781 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/routes/router.py
-drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.502124 fastipy-1.5.2/app/fastipy/src/types/
--rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.2/app/fastipy/src/types/__init__.py
--rw-rw-rw-   0        0        0      275 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/types/fastipy.py
--rw-rw-rw-   0        0        0      225 2024-04-14 19:33:49.000000 fastipy-1.5.2/app/fastipy/src/types/plugins.py
--rw-rw-rw-   0        0        0      683 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/types/routes.py
-drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.504123 fastipy-1.5.2/app/fastipy.egg-info/
--rw-rw-rw-   0        0        0     8007 2024-04-19 17:20:15.000000 fastipy-1.5.2/app/fastipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2131 2024-04-19 17:20:15.000000 fastipy-1.5.2/app/fastipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 17:20:15.000000 fastipy-1.5.2/app/fastipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-19 17:20:15.000000 fastipy-1.5.2/app/fastipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-19 17:20:15.000000 fastipy-1.5.2/app/fastipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 17:20:15.506116 fastipy-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1544 2024-04-19 17:19:36.000000 fastipy-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:27:59.085262 fastipy-1.5.3/
+-rw-rw-rw-   0        0        0    35823 2024-04-14 01:52:52.000000 fastipy-1.5.3/LICENSE
+-rw-rw-rw-   0        0        0     7422 2024-04-26 18:27:59.084261 fastipy-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6170 2024-04-26 18:27:54.000000 fastipy-1.5.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 18:27:59.010365 fastipy-1.5.3/app/
+drwxrwxrwx   0        0        0        0 2024-04-26 18:27:59.018966 fastipy-1.5.3/app/fastipy/
+-rw-rw-rw-   0        0        0      785 2024-04-26 18:26:17.000000 fastipy-1.5.3/app/fastipy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:27:59.025567 fastipy-1.5.3/app/fastipy/src/
+-rw-rw-rw-   0        0        0        0 2024-04-20 17:26:27.000000 fastipy-1.5.3/app/fastipy/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:27:59.032075 fastipy-1.5.3/app/fastipy/src/classes/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.3/app/fastipy/src/classes/__init__.py
+-rw-rw-rw-   0        0        0      577 2024-04-26 18:26:17.000000 fastipy-1.5.3/app/fastipy/src/classes/decorators_base.py
+-rw-rw-rw-   0        0        0     6123 2024-04-26 18:26:17.000000 fastipy-1.5.3/app/fastipy/src/classes/json_database.py
+-rw-rw-rw-   0        0        0     6799 2024-04-26 18:26:17.000000 fastipy-1.5.3/app/fastipy/src/classes/mailer.py
+-rw-rw-rw-   0        0        0     3843 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/classes/template_render.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:27:59.042097 fastipy-1.5.3/app/fastipy/src/constants/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.3/app/fastipy/src/constants/__init__.py
+-rw-rw-rw-   0        0        0      802 2024-04-14 19:33:49.000000 fastipy-1.5.3/app/fastipy/src/constants/content_types.py
+-rw-rw-rw-   0        0        0       42 2024-04-14 19:33:49.000000 fastipy-1.5.3/app/fastipy/src/constants/decorators.py
+-rw-rw-rw-   0        0        0      108 2024-04-14 19:33:49.000000 fastipy-1.5.3/app/fastipy/src/constants/events.py
+-rw-rw-rw-   0        0        0      164 2024-04-14 19:33:49.000000 fastipy-1.5.3/app/fastipy/src/constants/hooks.py
+-rw-rw-rw-   0        0        0      171 2024-04-14 19:33:49.000000 fastipy-1.5.3/app/fastipy/src/constants/http_methods.py
+-rw-rw-rw-   0        0        0     2957 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/constants/http_status_code.py
+-rw-rw-rw-   0        0        0     1032 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/constants/serializers.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:27:59.048020 fastipy-1.5.3/app/fastipy/src/core/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.3/app/fastipy/src/core/__init__.py
+-rw-rw-rw-   0        0        0    21271 2024-04-26 18:26:17.000000 fastipy-1.5.3/app/fastipy/src/core/fastipy.py
+-rw-rw-rw-   0        0        0    26461 2024-04-26 18:26:17.000000 fastipy-1.5.3/app/fastipy/src/core/reply.py
+-rw-rw-rw-   0        0        0     5237 2024-04-26 18:26:17.000000 fastipy-1.5.3/app/fastipy/src/core/request.py
+-rw-rw-rw-   0        0        0     7705 2024-04-26 18:26:17.000000 fastipy-1.5.3/app/fastipy/src/core/request_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:27:59.062609 fastipy-1.5.3/app/fastipy/src/exceptions/
+-rw-rw-rw-   0        0        0      918 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      121 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/exceptions/decorator_already_exists_exception.py
+-rw-rw-rw-   0        0        0      113 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/exceptions/duplicate_route_exception.py
+-rw-rw-rw-   0        0        0     2458 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/exceptions/exception_handler.py
+-rw-rw-rw-   0        0        0      936 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/exceptions/fastipy_exception.py
+-rw-rw-rw-   0        0        0      103 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/exceptions/file_exception.py
+-rw-rw-rw-   0        0        0      110 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/exceptions/invalid_path_exception.py
+-rw-rw-rw-   0        0        0      110 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/exceptions/no_event_type.py
+-rw-rw-rw-   0        0        0      109 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/exceptions/no_hook_type.py
+-rw-rw-rw-   0        0        0      111 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/exceptions/no_http_method_exception.py
+-rw-rw-rw-   0        0        0      105 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/exceptions/plugin_exception.py
+-rw-rw-rw-   0        0        0      104 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/exceptions/reply_exception.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:27:59.066629 fastipy-1.5.3/app/fastipy/src/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.3/app/fastipy/src/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1538 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/helpers/async_sync_helpers.py
+-rw-rw-rw-   0        0        0      880 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/helpers/content_type.py
+-rw-rw-rw-   0        0        0     2236 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/helpers/route_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:27:59.068629 fastipy-1.5.3/app/fastipy/src/middlewares/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.3/app/fastipy/src/middlewares/__init__.py
+-rw-rw-rw-   0        0        0     3868 2024-04-26 18:26:17.000000 fastipy-1.5.3/app/fastipy/src/middlewares/cors.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:27:59.074238 fastipy-1.5.3/app/fastipy/src/models/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.3/app/fastipy/src/models/__init__.py
+-rw-rw-rw-   0        0        0     2874 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/models/body.py
+-rw-rw-rw-   0        0        0     4535 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/models/file.py
+-rw-rw-rw-   0        0        0     2518 2024-04-20 17:26:27.000000 fastipy-1.5.3/app/fastipy/src/models/form.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:27:59.077237 fastipy-1.5.3/app/fastipy/src/routes/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.3/app/fastipy/src/routes/__init__.py
+-rw-rw-rw-   0        0        0     2212 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/routes/plugin_tree.py
+-rw-rw-rw-   0        0        0     6781 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/routes/router.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:27:59.081243 fastipy-1.5.3/app/fastipy/src/types/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.3/app/fastipy/src/types/__init__.py
+-rw-rw-rw-   0        0        0      275 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/types/fastipy.py
+-rw-rw-rw-   0        0        0      225 2024-04-14 19:33:49.000000 fastipy-1.5.3/app/fastipy/src/types/plugins.py
+-rw-rw-rw-   0        0        0      683 2024-04-19 17:19:36.000000 fastipy-1.5.3/app/fastipy/src/types/routes.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:27:59.083256 fastipy-1.5.3/app/fastipy.egg-info/
+-rw-rw-rw-   0        0        0     7422 2024-04-26 18:27:58.000000 fastipy-1.5.3/app/fastipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2131 2024-04-26 18:27:58.000000 fastipy-1.5.3/app/fastipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 18:27:58.000000 fastipy-1.5.3/app/fastipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-26 18:27:58.000000 fastipy-1.5.3/app/fastipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-26 18:27:58.000000 fastipy-1.5.3/app/fastipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 18:27:59.085262 fastipy-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1544 2024-04-26 18:26:17.000000 fastipy-1.5.3/setup.py
```

### Comparing `fastipy-1.5.2/LICENSE` & `fastipy-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.2/PKG-INFO` & `fastipy-1.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastipy
-Version: 1.5.2
+Version: 1.5.3
 Summary: Fastipy is a fast and easy-to-use open source Python library for developing RESTful APIs. Inspired by the FastAPI and Fastify syntax and powered by uvicorn ASGI web server.
 Home-page: https://github.com/Bielgomes/Fastipy
 Author: Bielgomes
 Author-email: bielgomesdasilva@hotmail.com
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/Bielgomes/Fastipy/issues
 Classifier: Development Status :: 4 - Beta
@@ -263,32 +263,24 @@
 
 # Application Deploy
 
 For production deployment, please refer to this **[uvicorn guide](https://www.uvicorn.org/deployment/)**.
 
 # Change Log
 
-## Version 1.5.2
+## Version 1.5.3
 
-### Added
+### Todo
 
-- [x] Added Fastipy config.
-- [x] Added Plugin timeout configuration.
-- [x] Added typing for options in print routes function.
-- [x] Added types to request handler functions parameters.
-- [x] Added the option to automatically create folders when saving files.
-- [x] Added shortcut form property inside Request class to facilitate usability.
-- [x] Added documentation for most methods and classes.
+### Added
 
 ### Changed
 
-- [x] Renaming the fastipy base exception to the fastipy exception to make it easier to handle.
-- [x] Fixed problem in the error handler for python 3.11.
-- [x] Fixed the function of saving files securely, to save them in the correct path.
-- [x] Loading text and json from body files on demand.
+- [X] Fixing and improving CORS header generation
+- [X] Fixing Reply class that didn't store decorators 
 
 # Contributors
 
 <a href="https://github.com/Bielgomes/Fastipy/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=Bielgomes/Fastipy"/>
 </a>
```

### Comparing `fastipy-1.5.2/README.md` & `fastipy-1.5.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -235,32 +235,24 @@
 
 # Application Deploy
 
 For production deployment, please refer to this **[uvicorn guide](https://www.uvicorn.org/deployment/)**.
 
 # Change Log
 
-## Version 1.5.2
+## Version 1.5.3
 
-### Added
+### Todo
 
-- [x] Added Fastipy config.
-- [x] Added Plugin timeout configuration.
-- [x] Added typing for options in print routes function.
-- [x] Added types to request handler functions parameters.
-- [x] Added the option to automatically create folders when saving files.
-- [x] Added shortcut form property inside Request class to facilitate usability.
-- [x] Added documentation for most methods and classes.
+### Added
 
 ### Changed
 
-- [x] Renaming the fastipy base exception to the fastipy exception to make it easier to handle.
-- [x] Fixed problem in the error handler for python 3.11.
-- [x] Fixed the function of saving files securely, to save them in the correct path.
-- [x] Loading text and json from body files on demand.
+- [X] Fixing and improving CORS header generation
+- [X] Fixing Reply class that didn't store decorators 
 
 # Contributors
 
 <a href="https://github.com/Bielgomes/Fastipy/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=Bielgomes/Fastipy"/>
 </a>
```

### Comparing `fastipy-1.5.2/app/fastipy/__init__.py` & `fastipy-1.5.3/app/fastipy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-__version__ = "1.5.2"
+__version__ = "1.5.3"
 
 from .src.core.fastipy import Fastipy, FastipyInstance
 
 from .src.types.plugins import PluginOptions
 
 from .src.core.request import Request
 from .src.core.reply import Reply
 
 from .src.classes.mailer import Mailer, create_message
 from .src.classes.template_render import render_template
 from .src.classes.json_database import Database
 
 from .src.constants.http_status_code import Status
 
+from .src.exceptions.exception_handler import ExceptionHandler
+
 from starlette.testclient import TestClient
 
 __all__ = [
     "Fastipy",
     "FastipyInstance",
     "PluginOptions",
     "Request",
     "Reply",
     "Mailer",
     "create_message",
     "render_template",
     "Database",
     "Status",
+    "ExceptionHandler",
     "TestClient",
 ]
```

### Comparing `fastipy-1.5.2/app/fastipy/src/classes/json_database.py` & `fastipy-1.5.3/app/fastipy/src/classes/json_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from pathlib import Path
 import json, uuid
 
 
 class Database:
+    """A simple JSON-based database class."""
+
     def __init__(self):
         """
         Initialize the Database object.
         """
         self.database = {}  # Initialize an empty dictionary to hold data
         self.path = (
             Path(__file__).parent.parent / "db.json"
```

### Comparing `fastipy-1.5.2/app/fastipy/src/classes/mailer.py` & `fastipy-1.5.3/app/fastipy/src/classes/mailer.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,16 @@
             )
             message.attach(attachment)
 
     return message
 
 
 class Mailer:
+    """A class to send emails using SMTP."""
+
     def __init__(
         self,
         smtp_host: str,
         smtp_port: int,
         auth_user: str,
         auth_password: str,
         ssl: bool = True,
```

### Comparing `fastipy-1.5.2/app/fastipy/src/classes/template_render.py` & `fastipy-1.5.3/app/fastipy/src/classes/template_render.py`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.2/app/fastipy/src/constants/content_types.py` & `fastipy-1.5.3/app/fastipy/src/constants/content_types.py`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.2/app/fastipy/src/constants/http_status_code.py` & `fastipy-1.5.3/app/fastipy/src/constants/http_status_code.py`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.2/app/fastipy/src/constants/serializers.py` & `fastipy-1.5.3/app/fastipy/src/constants/serializers.py`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.2/app/fastipy/src/core/fastipy.py` & `fastipy-1.5.3/app/fastipy/src/core/fastipy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re, copy, click, nest_asyncio
-from typing import Callable, Optional, Self
+from typing import Callable, Dict, List, Optional, Self, Union
 from uvicorn.main import logger
 
 from ..constants.hooks import HOOKS, hookType
 from ..constants.http_methods import HTTP_METHODS, httpMethodType
 from ..constants.decorators import DECORATORS
 from ..constants.events import EVENTS, eventType
 from ..constants.serializers import SERIALIZERS
@@ -253,44 +253,44 @@
             instance._plugins.name = instance._name
         self._plugins.add_child(instance._plugins)
 
         return self
 
     def cors(
         self,
-        allow_origin: str = "*",
-        allow_headers: str = "*",
-        allow_methods: str = "*",
+        allow_origins: Union[str, List[str]] = "*",
+        allow_headers: Union[str, List[str]] = "*",
+        allow_methods: Union[str, List[str]] = "*",
         allow_credentials: bool = True,
-        expose_headers: Optional[str] = None,
+        expose_headers: Optional[Union[str, List[str]]] = None,
         max_age: Optional[int] = None,
-        content_security_policy: str = "default-src 'self'",
-        custom_headers: dict = {},
+        content_security_policys: Union[str, List[str]] = "default-src 'self'",
+        custom_headers: Dict[str, Union[str, List[str]]] = {},
     ) -> Self:
         """
-        Configure CORS for the application.
+        Initialize the CORS generator with default values.
 
         Args:
-            allow_origin (str, optional): Allowed origin. Defaults to "*".
-            allow_headers (str, optional): Allowed headers. Defaults to "*".
-            allow_methods (str, optional): Allowed methods. Defaults to "*".
+            allow_origins (Union[str, List[str]], optional): Allowed origins. Defaults to "*".
+            allow_headers (Union[str, List[str]], optional): Allowed headers. Defaults to "*".
+            allow_methods (Union[str, List[str]], optional): Allowed methods. Defaults to "*".
             allow_credentials (bool, optional): Allow credentials. Defaults to True.
-            expose_headers (Optional[str], optional): Expose headers. Defaults to None.
-            max_age (Optional[int], optional): Maximum age. Defaults to None.
-            content_security_policy (str, optional): Content security policy. Defaults to "default-src 'self'".
-            custom_headers (dict, optional): Custom headers. Defaults to {}.
+            expose_headers (Optional[Union[str, List[str]]], optional): Expose headers. Defaults to None.
+            max_age (Optional[int], optional): Max age. Defaults to None.
+            content_security_policys (Union[str, List[str]], optional): Content security policies. Defaults to "default-src 'self'".
+            custom_headers (Dict[str, Union[str, List[str]]], optional): Custom headers. Defaults to {}.
         """
         self._cors = CORSGenerator(
-            allow_origin,
+            allow_origins,
             allow_headers,
             allow_methods,
             allow_credentials,
             expose_headers,
             max_age,
-            content_security_policy,
+            content_security_policys,
             custom_headers,
         )
         return self
 
     def decorate(self, name: str, value: any) -> None:
         """
         Register a decorator for the application.
```

### Comparing `fastipy-1.5.2/app/fastipy/src/core/reply.py` & `fastipy-1.5.3/app/fastipy/src/core/reply.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         self._status_code = 200
         self._content = None
         self._cookies = SimpleCookie()
         self._response_time = perf_counter()
         self._response_sent = False
         self._serializers = reversed(serializers)
 
-        self._instance_decorators = decorators.get(Self, [])
+        self._instance_decorators = decorators.get("reply", [])
 
     @property
     def status_code(self) -> int:
         """
         Get the status code of the response.
 
         Returns:
```

### Comparing `fastipy-1.5.2/app/fastipy/src/core/request.py` & `fastipy-1.5.3/app/fastipy/src/core/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Union, Dict, Tuple, List
 from http.cookies import SimpleCookie
 from urllib.parse import parse_qsl
-from logging import Logger
 
 from ..types.routes import FunctionType
 
 from ..classes.decorators_base import DecoratorsBase
 
 from ..models.body import Body
 from ..models.form import Form
@@ -16,30 +15,27 @@
     Represents the HTTP request object for handling incoming requests in a Fastipy application.
     """
 
     def __init__(
         self,
         scope,
         receive,
-        logger: Logger,
         decorators: Dict[str, List[FunctionType]] = {},
     ) -> None:
         """
         Initialize the Request object.
 
         Args:
             scope: The ASGI scope of the request.
             receive: The coroutine function to receive messages from the client.
-            logger (Logger): The logger object for logging.
             decorators (Dict[str, List[FunctionType]], optional): The decorators for the request. Defaults to {}.
         """
         self.__scope = scope
         self.__receive = receive
         self._instance_decorators = decorators.get("request", [])
-        self._log = logger
         self._body = None
 
         self.__headers()
         self.__query_params()
         self._cookies = SimpleCookie(self.__scope["headers"].get("cookie", None))
 
     @property
```

### Comparing `fastipy-1.5.2/app/fastipy/src/core/request_handler.py` & `fastipy-1.5.3/app/fastipy/src/core/request_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,14 @@
         )
         if route is None:
             await self._handle_route_not_found(send, cors)
             return
 
         scope["params"] = params
         request = Request(scope, receive, self._decorators)
-        self._serializers: list = self._serializers
         reply = Reply(
             send,
             request,
             cors,
             self._static_path,
             self._decorators,
             route["hooks"],
@@ -188,15 +187,15 @@
             exception (Exception): The exception that occurred.
             reply (Reply): The Reply object.
             exception_handler (ExceptionHandler): Exception handler object.
             internal (bool, optional): Indicates if the exception is internal. Defaults to False.
         """
         if internal or issubclass(type(exception), FastipyException):
             await reply._send_error(
-                message=f"{exception_handler.type}:"
+                message=f"{exception_handler.type}: "
                 + exception_handler.message.replace('"', "'"),
                 code=500,
             )
             print(traceback.format_exc())
         else:
             raise exception
```

### Comparing `fastipy-1.5.2/app/fastipy/src/exceptions/__init__.py` & `fastipy-1.5.3/app/fastipy/src/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.2/app/fastipy/src/exceptions/exception_handler.py` & `fastipy-1.5.3/app/fastipy/src/exceptions/exception_handler.py`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.2/app/fastipy/src/exceptions/fastipy_exception.py` & `fastipy-1.5.3/app/fastipy/src/exceptions/fastipy_exception.py`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.2/app/fastipy/src/helpers/async_sync_helpers.py` & `fastipy-1.5.3/app/fastipy/src/helpers/async_sync_helpers.py`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.2/app/fastipy/src/helpers/content_type.py` & `fastipy-1.5.3/app/fastipy/src/helpers/content_type.py`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.2/app/fastipy/src/helpers/route_helpers.py` & `fastipy-1.5.3/app/fastipy/src/helpers/route_helpers.py`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.2/app/fastipy/src/models/body.py` & `fastipy-1.5.3/app/fastipy/src/models/body.py`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.2/app/fastipy/src/models/file.py` & `fastipy-1.5.3/app/fastipy/src/models/file.py`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.2/app/fastipy/src/models/form.py` & `fastipy-1.5.3/app/fastipy/src/models/form.py`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.2/app/fastipy/src/routes/plugin_tree.py` & `fastipy-1.5.3/app/fastipy/src/routes/plugin_tree.py`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.2/app/fastipy/src/routes/router.py` & `fastipy-1.5.3/app/fastipy/src/routes/router.py`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.2/app/fastipy/src/types/routes.py` & `fastipy-1.5.3/app/fastipy/src/types/routes.py`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.2/app/fastipy.egg-info/PKG-INFO` & `fastipy-1.5.3/app/fastipy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastipy
-Version: 1.5.2
+Version: 1.5.3
 Summary: Fastipy is a fast and easy-to-use open source Python library for developing RESTful APIs. Inspired by the FastAPI and Fastify syntax and powered by uvicorn ASGI web server.
 Home-page: https://github.com/Bielgomes/Fastipy
 Author: Bielgomes
 Author-email: bielgomesdasilva@hotmail.com
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/Bielgomes/Fastipy/issues
 Classifier: Development Status :: 4 - Beta
@@ -263,32 +263,24 @@
 
 # Application Deploy
 
 For production deployment, please refer to this **[uvicorn guide](https://www.uvicorn.org/deployment/)**.
 
 # Change Log
 
-## Version 1.5.2
+## Version 1.5.3
 
-### Added
+### Todo
 
-- [x] Added Fastipy config.
-- [x] Added Plugin timeout configuration.
-- [x] Added typing for options in print routes function.
-- [x] Added types to request handler functions parameters.
-- [x] Added the option to automatically create folders when saving files.
-- [x] Added shortcut form property inside Request class to facilitate usability.
-- [x] Added documentation for most methods and classes.
+### Added
 
 ### Changed
 
-- [x] Renaming the fastipy base exception to the fastipy exception to make it easier to handle.
-- [x] Fixed problem in the error handler for python 3.11.
-- [x] Fixed the function of saving files securely, to save them in the correct path.
-- [x] Loading text and json from body files on demand.
+- [X] Fixing and improving CORS header generation
+- [X] Fixing Reply class that didn't store decorators 
 
 # Contributors
 
 <a href="https://github.com/Bielgomes/Fastipy/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=Bielgomes/Fastipy"/>
 </a>
```

### Comparing `fastipy-1.5.2/app/fastipy.egg-info/SOURCES.txt` & `fastipy-1.5.3/app/fastipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.2/setup.py` & `fastipy-1.5.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="fastipy",
-    version="1.5.2",
+    version="1.5.3",
     description="Fastipy is a fast and easy-to-use open source Python library for developing RESTful APIs. Inspired by the FastAPI and Fastify syntax and powered by uvicorn ASGI web server.",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bielgomes/Fastipy",
     author="Bielgomes",
```

