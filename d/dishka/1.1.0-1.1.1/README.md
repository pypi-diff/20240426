# Comparing `tmp/dishka-1.1.0.tar.gz` & `tmp/dishka-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dishka-1.1.0.tar", last modified: Sun Apr 21 10:25:11 2024, max compression
+gzip compressed data, was "dishka-1.1.1.tar", last modified: Fri Apr 26 21:44:04 2024, max compression
```

## Comparing `dishka-1.1.0.tar` & `dishka-1.1.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-21 10:25:11.330739 dishka-1.1.0/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    11357 2024-01-25 16:39:00.000000 dishka-1.1.0/LICENSE
--rw-r--r--   0 tishka17  (1000) tishka17  (1000)    12011 2024-04-21 10:25:11.330739 dishka-1.1.0/PKG-INFO
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    11074 2024-04-21 10:24:38.000000 dishka-1.1.0/README.md
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1097 2024-04-21 10:24:45.000000 dishka-1.1.0/pyproject.toml
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       38 2024-04-21 10:25:11.330739 dishka-1.1.0/setup.cfg
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-21 10:25:11.326739 dishka-1.1.0/src/
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-21 10:25:11.330739 dishka-1.1.0/src/dishka/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      843 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/__init__.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-21 10:25:11.330739 dishka-1.1.0/src/dishka/_adaptix/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      639 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/common.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     5460 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/feature_requirement.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-21 10:25:11.330739 dishka-1.1.0/src/dishka/_adaptix/type_tools/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      609 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/type_tools/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     4141 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/type_tools/basic_utils.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      994 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/type_tools/constants.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1530 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/type_tools/fundamentals.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3907 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/type_tools/generic_resolver.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1828 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/type_tools/implicit_params.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1059 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/type_tools/norm_utils.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    25528 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/type_tools/normalize_type.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     7025 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/async_container.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     6664 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/container.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      476 2024-03-24 23:55:01.000000 dishka-1.1.0/src/dishka/container_objects.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-21 10:25:11.330739 dishka-1.1.0/src/dishka/dependency_source/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      542 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/dependency_source/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1038 2024-03-19 22:45:31.000000 dishka-1.1.0/src/dishka/dependency_source/alias.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1416 2024-03-19 22:45:31.000000 dishka-1.1.0/src/dishka/dependency_source/composite.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1515 2024-03-19 22:45:31.000000 dishka-1.1.0/src/dishka/dependency_source/context_var.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1324 2024-03-19 22:45:31.000000 dishka-1.1.0/src/dishka/dependency_source/decorator.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2164 2024-03-27 22:27:14.000000 dishka-1.1.0/src/dishka/dependency_source/factory.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      905 2024-03-19 22:45:31.000000 dishka-1.1.0/src/dishka/dependency_source/make_alias.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      678 2024-03-19 22:45:31.000000 dishka-1.1.0/src/dishka/dependency_source/make_context_var.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1462 2024-04-01 21:05:02.000000 dishka-1.1.0/src/dishka/dependency_source/make_decorator.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    16303 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/dependency_source/make_factory.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1949 2024-03-19 22:45:31.000000 dishka-1.1.0/src/dishka/dependency_source/unpack_provides.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-21 10:25:11.330739 dishka-1.1.0/src/dishka/entities/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-29 00:39:11.000000 dishka-1.1.0/src/dishka/entities/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       40 2024-02-29 00:39:11.000000 dishka-1.1.0/src/dishka/entities/component.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1178 2024-04-20 19:15:28.000000 dishka-1.1.0/src/dishka/entities/depends_marker.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1123 2024-03-04 22:02:38.000000 dishka-1.1.0/src/dishka/entities/key.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      347 2024-03-19 22:45:31.000000 dishka-1.1.0/src/dishka/entities/provides_marker.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      783 2024-03-24 23:55:01.000000 dishka-1.1.0/src/dishka/entities/scope.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2730 2024-03-26 23:39:41.000000 dishka-1.1.0/src/dishka/error_rendering.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1715 2024-03-04 22:02:38.000000 dishka-1.1.0/src/dishka/exceptions.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3398 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/factory_compiler.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-21 10:25:11.330739 dishka-1.1.0/src/dishka/integrations/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-08 23:15:26.000000 dishka-1.1.0/src/dishka/integrations/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2279 2024-03-24 23:55:01.000000 dishka-1.1.0/src/dishka/integrations/aiogram.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1232 2024-03-24 23:55:01.000000 dishka-1.1.0/src/dishka/integrations/aiohttp.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2445 2024-03-04 22:02:38.000000 dishka-1.1.0/src/dishka/integrations/arq.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     5268 2024-03-24 23:55:01.000000 dishka-1.1.0/src/dishka/integrations/base.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1417 2024-03-24 23:55:01.000000 dishka-1.1.0/src/dishka/integrations/fastapi.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3676 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/integrations/faststream.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1421 2024-03-24 23:55:01.000000 dishka-1.1.0/src/dishka/integrations/flask.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1749 2024-03-24 23:55:01.000000 dishka-1.1.0/src/dishka/integrations/litestar.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1617 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/integrations/sanic.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1248 2024-03-24 23:55:01.000000 dishka-1.1.0/src/dishka/integrations/starlette.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2226 2024-04-02 21:16:55.000000 dishka-1.1.0/src/dishka/integrations/taskiq.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1379 2024-03-28 15:28:45.000000 dishka-1.1.0/src/dishka/integrations/telebot.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     6855 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/provider.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-18 18:04:06.000000 dishka-1.1.0/src/dishka/py.typed
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    13009 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/registry.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-21 10:25:11.330739 dishka-1.1.0/src/dishka.egg-info/
--rw-r--r--   0 tishka17  (1000) tishka17  (1000)    12011 2024-04-21 10:25:11.000000 dishka-1.1.0/src/dishka.egg-info/PKG-INFO
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2037 2024-04-21 10:25:11.000000 dishka-1.1.0/src/dishka.egg-info/SOURCES.txt
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        1 2024-04-21 10:25:11.000000 dishka-1.1.0/src/dishka.egg-info/dependency_links.txt
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       50 2024-04-21 10:25:11.000000 dishka-1.1.0/src/dishka.egg-info/requires.txt
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        7 2024-04-21 10:25:11.000000 dishka-1.1.0/src/dishka.egg-info/top_level.txt
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-26 21:44:04.023128 dishka-1.1.1/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    11357 2024-01-25 16:39:00.000000 dishka-1.1.1/LICENSE
+-rw-r--r--   0 tishka17  (1000) tishka17  (1000)    12011 2024-04-26 21:44:04.023128 dishka-1.1.1/PKG-INFO
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    11074 2024-04-21 10:24:38.000000 dishka-1.1.1/README.md
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1097 2024-04-26 21:43:35.000000 dishka-1.1.1/pyproject.toml
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       38 2024-04-26 21:44:04.023128 dishka-1.1.1/setup.cfg
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-26 21:44:04.019128 dishka-1.1.1/src/
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-26 21:44:04.019128 dishka-1.1.1/src/dishka/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      843 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/__init__.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-26 21:44:04.019128 dishka-1.1.1/src/dishka/_adaptix/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      639 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/common.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     5460 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/feature_requirement.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-26 21:44:04.019128 dishka-1.1.1/src/dishka/_adaptix/type_tools/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      609 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/type_tools/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     4141 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/type_tools/basic_utils.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      994 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/type_tools/constants.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1530 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/type_tools/fundamentals.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3907 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/type_tools/generic_resolver.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1828 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/type_tools/implicit_params.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1059 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/type_tools/norm_utils.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    25528 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/type_tools/normalize_type.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     7025 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/async_container.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     6664 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/container.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      476 2024-03-24 23:55:01.000000 dishka-1.1.1/src/dishka/container_objects.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-26 21:44:04.019128 dishka-1.1.1/src/dishka/dependency_source/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      542 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/dependency_source/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1038 2024-03-19 22:45:31.000000 dishka-1.1.1/src/dishka/dependency_source/alias.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1416 2024-04-24 19:42:27.000000 dishka-1.1.1/src/dishka/dependency_source/composite.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1515 2024-03-19 22:45:31.000000 dishka-1.1.1/src/dishka/dependency_source/context_var.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1324 2024-03-19 22:45:31.000000 dishka-1.1.1/src/dishka/dependency_source/decorator.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2164 2024-04-26 21:28:12.000000 dishka-1.1.1/src/dishka/dependency_source/factory.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      905 2024-03-19 22:45:31.000000 dishka-1.1.1/src/dishka/dependency_source/make_alias.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      678 2024-03-19 22:45:31.000000 dishka-1.1.1/src/dishka/dependency_source/make_context_var.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1462 2024-04-01 21:05:02.000000 dishka-1.1.1/src/dishka/dependency_source/make_decorator.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    16505 2024-04-26 21:43:29.000000 dishka-1.1.1/src/dishka/dependency_source/make_factory.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1949 2024-03-19 22:45:31.000000 dishka-1.1.1/src/dishka/dependency_source/unpack_provides.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-26 21:44:04.019128 dishka-1.1.1/src/dishka/entities/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-29 00:39:11.000000 dishka-1.1.1/src/dishka/entities/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       40 2024-02-29 00:39:11.000000 dishka-1.1.1/src/dishka/entities/component.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1178 2024-04-20 19:15:28.000000 dishka-1.1.1/src/dishka/entities/depends_marker.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1123 2024-03-04 22:02:38.000000 dishka-1.1.1/src/dishka/entities/key.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      347 2024-03-19 22:45:31.000000 dishka-1.1.1/src/dishka/entities/provides_marker.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      783 2024-03-24 23:55:01.000000 dishka-1.1.1/src/dishka/entities/scope.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2730 2024-03-26 23:39:41.000000 dishka-1.1.1/src/dishka/error_rendering.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1715 2024-03-04 22:02:38.000000 dishka-1.1.1/src/dishka/exceptions.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3398 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/factory_compiler.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-26 21:44:04.023128 dishka-1.1.1/src/dishka/integrations/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-08 23:15:26.000000 dishka-1.1.1/src/dishka/integrations/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2279 2024-03-24 23:55:01.000000 dishka-1.1.1/src/dishka/integrations/aiogram.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1232 2024-03-24 23:55:01.000000 dishka-1.1.1/src/dishka/integrations/aiohttp.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2445 2024-03-04 22:02:38.000000 dishka-1.1.1/src/dishka/integrations/arq.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     5268 2024-03-24 23:55:01.000000 dishka-1.1.1/src/dishka/integrations/base.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1417 2024-03-24 23:55:01.000000 dishka-1.1.1/src/dishka/integrations/fastapi.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3676 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/integrations/faststream.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1421 2024-03-24 23:55:01.000000 dishka-1.1.1/src/dishka/integrations/flask.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1749 2024-03-24 23:55:01.000000 dishka-1.1.1/src/dishka/integrations/litestar.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1617 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/integrations/sanic.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1248 2024-03-24 23:55:01.000000 dishka-1.1.1/src/dishka/integrations/starlette.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2226 2024-04-02 21:16:55.000000 dishka-1.1.1/src/dishka/integrations/taskiq.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1379 2024-03-28 15:28:45.000000 dishka-1.1.1/src/dishka/integrations/telebot.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     6855 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/provider.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-18 18:04:06.000000 dishka-1.1.1/src/dishka/py.typed
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    13177 2024-04-26 21:43:29.000000 dishka-1.1.1/src/dishka/registry.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-26 21:44:04.023128 dishka-1.1.1/src/dishka.egg-info/
+-rw-r--r--   0 tishka17  (1000) tishka17  (1000)    12011 2024-04-26 21:44:04.000000 dishka-1.1.1/src/dishka.egg-info/PKG-INFO
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2037 2024-04-26 21:44:04.000000 dishka-1.1.1/src/dishka.egg-info/SOURCES.txt
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        1 2024-04-26 21:44:04.000000 dishka-1.1.1/src/dishka.egg-info/dependency_links.txt
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       50 2024-04-26 21:44:04.000000 dishka-1.1.1/src/dishka.egg-info/requires.txt
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        7 2024-04-26 21:44:04.000000 dishka-1.1.1/src/dishka.egg-info/top_level.txt
```

### Comparing `dishka-1.1.0/LICENSE` & `dishka-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/PKG-INFO` & `dishka-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dishka
-Version: 1.1.0
+Version: 1.1.1
 Summary: Minimal DI framework
 Author-email: Andrey Tikhonov <17@itishka.org>
 License: Apache-2.0
 Project-URL: Source, https://github.com/reagento/dishka
 Project-URL: Homepage, https://github.com/reagento/dishka
 Project-URL: Documentation, https://dishka.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/reagento/dishka/issues
```

### Comparing `dishka-1.1.0/README.md` & `dishka-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/pyproject.toml` & `dishka-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "dishka"
-version = "1.1.0"
+version = "1.1.1"
 readme = "README.md"
 authors = [
     { name = "Andrey Tikhonov", email = "17@itishka.org" },
 ]
 license = { text = "Apache-2.0" }
 description = "Minimal DI framework"
 requires-python = ">=3.10"
```

### Comparing `dishka-1.1.0/src/dishka/__init__.py` & `dishka-1.1.1/src/dishka/__init__.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/_adaptix/common.py` & `dishka-1.1.1/src/dishka/_adaptix/common.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/_adaptix/feature_requirement.py` & `dishka-1.1.1/src/dishka/_adaptix/feature_requirement.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/_adaptix/type_tools/__init__.py` & `dishka-1.1.1/src/dishka/_adaptix/type_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/_adaptix/type_tools/basic_utils.py` & `dishka-1.1.1/src/dishka/_adaptix/type_tools/basic_utils.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/_adaptix/type_tools/constants.py` & `dishka-1.1.1/src/dishka/_adaptix/type_tools/constants.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/_adaptix/type_tools/fundamentals.py` & `dishka-1.1.1/src/dishka/_adaptix/type_tools/fundamentals.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/_adaptix/type_tools/generic_resolver.py` & `dishka-1.1.1/src/dishka/_adaptix/type_tools/generic_resolver.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/_adaptix/type_tools/implicit_params.py` & `dishka-1.1.1/src/dishka/_adaptix/type_tools/implicit_params.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/_adaptix/type_tools/norm_utils.py` & `dishka-1.1.1/src/dishka/_adaptix/type_tools/norm_utils.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/_adaptix/type_tools/normalize_type.py` & `dishka-1.1.1/src/dishka/_adaptix/type_tools/normalize_type.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/async_container.py` & `dishka-1.1.1/src/dishka/async_container.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/container.py` & `dishka-1.1.1/src/dishka/container.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/dependency_source/__init__.py` & `dishka-1.1.1/src/dishka/dependency_source/__init__.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/dependency_source/alias.py` & `dishka-1.1.1/src/dishka/dependency_source/alias.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/dependency_source/composite.py` & `dishka-1.1.1/src/dishka/dependency_source/composite.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/dependency_source/context_var.py` & `dishka-1.1.1/src/dishka/dependency_source/context_var.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/dependency_source/decorator.py` & `dishka-1.1.1/src/dishka/dependency_source/decorator.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/dependency_source/factory.py` & `dishka-1.1.1/src/dishka/dependency_source/factory.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/dependency_source/make_alias.py` & `dishka-1.1.1/src/dishka/dependency_source/make_alias.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/dependency_source/make_context_var.py` & `dishka-1.1.1/src/dishka/dependency_source/make_context_var.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/dependency_source/make_decorator.py` & `dishka-1.1.1/src/dishka/dependency_source/make_decorator.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/dependency_source/make_factory.py` & `dishka-1.1.1/src/dishka/dependency_source/make_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     Generator,
     Iterable,
     Iterator,
     Sequence,
 )
 from inspect import (
     isasyncgenfunction,
+    isbuiltin,
     isclass,
     iscoroutinefunction,
     isfunction,
     isgeneratorfunction,
     ismethod,
     signature,
     unwrap,
@@ -222,15 +223,15 @@
         scope=scope,
         provides=hint_to_dependency_key(provides),
         is_to_bind=False,
         cache=cache,
     )
 
 
-def _make_factory_by_method(
+def _make_factory_by_function(
         *,
         provides: Any,
         scope: BaseScope | None,
         source: Callable | classmethod,
         cache: bool,
         is_in_class: bool,
 ) -> Factory:
@@ -383,18 +384,23 @@
         source = source[get_type_vars(source)]
 
     if isclass(source) or get_origin(source):
         return _make_factory_by_class(
             provides=provides, scope=scope, source=source, cache=cache,
         )
     elif isfunction(source) or isinstance(source, classmethod):
-        return _make_factory_by_method(
+        return _make_factory_by_function(
             provides=provides, scope=scope, source=source, cache=cache,
             is_in_class=is_in_class,
         )
+    elif isbuiltin(source):
+        return _make_factory_by_function(
+            provides=provides, scope=scope, source=source, cache=cache,
+            is_in_class=False,
+        )
     elif isinstance(source, staticmethod):
         return _make_factory_by_static_method(
             provides=provides, scope=scope, source=source, cache=cache,
         )
     elif callable(source):
         return _make_factory_by_other_callable(
             provides=provides, scope=scope, source=source, cache=cache,
```

### Comparing `dishka-1.1.0/src/dishka/dependency_source/unpack_provides.py` & `dishka-1.1.1/src/dishka/dependency_source/unpack_provides.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/entities/depends_marker.py` & `dishka-1.1.1/src/dishka/entities/depends_marker.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/entities/key.py` & `dishka-1.1.1/src/dishka/entities/key.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/entities/scope.py` & `dishka-1.1.1/src/dishka/entities/scope.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/error_rendering.py` & `dishka-1.1.1/src/dishka/error_rendering.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/exceptions.py` & `dishka-1.1.1/src/dishka/exceptions.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/factory_compiler.py` & `dishka-1.1.1/src/dishka/factory_compiler.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/integrations/aiogram.py` & `dishka-1.1.1/src/dishka/integrations/aiogram.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/integrations/aiohttp.py` & `dishka-1.1.1/src/dishka/integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/integrations/arq.py` & `dishka-1.1.1/src/dishka/integrations/arq.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/integrations/base.py` & `dishka-1.1.1/src/dishka/integrations/base.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/integrations/fastapi.py` & `dishka-1.1.1/src/dishka/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/integrations/faststream.py` & `dishka-1.1.1/src/dishka/integrations/faststream.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/integrations/flask.py` & `dishka-1.1.1/src/dishka/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/integrations/litestar.py` & `dishka-1.1.1/src/dishka/integrations/litestar.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/integrations/sanic.py` & `dishka-1.1.1/src/dishka/integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/integrations/starlette.py` & `dishka-1.1.1/src/dishka/integrations/starlette.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/integrations/taskiq.py` & `dishka-1.1.1/src/dishka/integrations/taskiq.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/integrations/telebot.py` & `dishka-1.1.1/src/dishka/integrations/telebot.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/provider.py` & `dishka-1.1.1/src/dishka/provider.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.0/src/dishka/registry.py` & `dishka-1.1.1/src/dishka/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,16 +84,21 @@
             self.factories[dependency] = factory
             return factory
 
     def _specialize_generic(
             self, factory: Factory, dependency_key: DependencyKey,
     ) -> Factory:
         dependency = dependency_key.type_hint
+        type_var_deps = (
+            d.type_hint
+            for d in factory.dependencies
+            if isinstance(d.type_hint, TypeVar)
+        )
         params_replacement = dict(zip(
-            get_args(factory.provides.type_hint),
+            type_var_deps,
             get_args(dependency),
             strict=False,
         ))
         new_dependencies: list[DependencyKey] = []
         for source_dependency in factory.dependencies:
             hint = source_dependency.type_hint
             if isinstance(hint, TypeVar):
@@ -154,15 +159,16 @@
             raise
         finally:
             self.path.pop(factory.provides)
         self.valid_keys[factory.provides] = True
 
     def validate(self):
         for registry_index, registry in enumerate(self.registries):
-            for factory in registry.factories.values():
+            factories = tuple(registry.factories.values())
+            for factory in factories:
                 self.path = {}
                 try:
                     self._validate_factory(factory, registry_index)
                 except NoFactoryError as e:
                     raise GraphMissingFactoryError(
                         e.requested, e.path,
                     ) from None
```

### Comparing `dishka-1.1.0/src/dishka.egg-info/PKG-INFO` & `dishka-1.1.1/src/dishka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dishka
-Version: 1.1.0
+Version: 1.1.1
 Summary: Minimal DI framework
 Author-email: Andrey Tikhonov <17@itishka.org>
 License: Apache-2.0
 Project-URL: Source, https://github.com/reagento/dishka
 Project-URL: Homepage, https://github.com/reagento/dishka
 Project-URL: Documentation, https://dishka.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/reagento/dishka/issues
```

### Comparing `dishka-1.1.0/src/dishka.egg-info/SOURCES.txt` & `dishka-1.1.1/src/dishka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

