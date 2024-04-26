# Comparing `tmp/alphaz-next-0.5.5.tar.gz` & `tmp/alphaz-next-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphaz-next-0.5.5.tar", last modified: Fri Apr 26 08:41:44 2024, max compression
+gzip compressed data, was "alphaz-next-0.5.6.tar", last modified: Fri Apr 26 08:56:31 2024, max compression
```

## Comparing `alphaz-next-0.5.5.tar` & `alphaz-next-0.5.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:44.989345 alphaz-next-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-26 08:41:44.985345 alphaz-next-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:44.981346 alphaz-next-0.5.5/alphaz_next/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:44.981346 alphaz-next-0.5.5/alphaz_next/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/asyncio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:44.981346 alphaz-next-0.5.5/alphaz_next/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:44.981346 alphaz-next-0.5.5/alphaz_next/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/core/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/core/_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/core/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/core/exception_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:44.985345 alphaz-next-0.5.5/alphaz_next/core/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/core/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/core/responses/file_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/core/responses/html_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/core/responses/json_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/core/responses/orjson_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/core/responses/plaintext_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/core/responses/redirect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/core/responses/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/core/responses/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/core/responses/ujson_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:44.985345 alphaz-next-0.5.5/alphaz_next/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/libs/file_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/libs/httpx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:44.977345 alphaz-next-0.5.5/alphaz_next/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:44.985345 alphaz-next-0.5.5/alphaz_next/models/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/models/auth/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:44.985345 alphaz-next-0.5.5/alphaz_next/models/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:44.985345 alphaz-next-0.5.5/alphaz_next/models/config/_base/
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/models/config/_base/internal_config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/models/config/_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/models/config/alpha_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/models/config/api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/models/config/apm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/models/config/config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/models/config/database_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/models/config/directories_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/models/config/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/models/config/openapi_config_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:44.981346 alphaz-next-0.5.5/alphaz_next/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:44.985345 alphaz-next-0.5.5/alphaz_next/tests/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:44.985345 alphaz-next-0.5.5/alphaz_next/tests/utils/mocking/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/tests/utils/mocking/mock_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/tests/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:44.985345 alphaz-next-0.5.5/alphaz_next/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/utils/logging_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-26 08:41:34.000000 alphaz-next-0.5.5/alphaz_next/utils/loguru.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:44.981346 alphaz-next-0.5.5/alphaz_next.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-26 08:41:44.000000 alphaz-next-0.5.5/alphaz_next.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-26 08:41:44.000000 alphaz-next-0.5.5/alphaz_next.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:41:44.000000 alphaz-next-0.5.5/alphaz_next.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-26 08:41:44.000000 alphaz-next-0.5.5/alphaz_next.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 08:41:44.000000 alphaz-next-0.5.5/alphaz_next.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 08:41:44.989345 alphaz-next-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-26 08:41:43.000000 alphaz-next-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:56:31.931859 alphaz-next-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-26 08:56:31.931859 alphaz-next-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:56:31.923859 alphaz-next-0.5.6/alphaz_next/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:56:31.927859 alphaz-next-0.5.6/alphaz_next/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/asyncio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:56:31.927859 alphaz-next-0.5.6/alphaz_next/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:56:31.927859 alphaz-next-0.5.6/alphaz_next/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/core/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/core/_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/core/exception_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:56:31.927859 alphaz-next-0.5.6/alphaz_next/core/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/core/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/core/responses/file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/core/responses/html_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/core/responses/json_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/core/responses/orjson_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/core/responses/plaintext_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/core/responses/redirect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/core/responses/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/core/responses/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/core/responses/ujson_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:56:31.927859 alphaz-next-0.5.6/alphaz_next/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/libs/file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/libs/httpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:56:31.923859 alphaz-next-0.5.6/alphaz_next/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:56:31.927859 alphaz-next-0.5.6/alphaz_next/models/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/models/auth/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:56:31.931859 alphaz-next-0.5.6/alphaz_next/models/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:56:31.931859 alphaz-next-0.5.6/alphaz_next/models/config/_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/models/config/_base/internal_config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/models/config/_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/models/config/alpha_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/models/config/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/models/config/apm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/models/config/config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/models/config/database_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/models/config/directories_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/models/config/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/models/config/openapi_config_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:56:31.923859 alphaz-next-0.5.6/alphaz_next/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:56:31.931859 alphaz-next-0.5.6/alphaz_next/tests/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:56:31.931859 alphaz-next-0.5.6/alphaz_next/tests/utils/mocking/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/tests/utils/mocking/mock_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/tests/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:56:31.931859 alphaz-next-0.5.6/alphaz_next/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/utils/logging_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-26 08:56:29.000000 alphaz-next-0.5.6/alphaz_next/utils/loguru.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:56:31.927859 alphaz-next-0.5.6/alphaz_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-26 08:56:31.000000 alphaz-next-0.5.6/alphaz_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-26 08:56:31.000000 alphaz-next-0.5.6/alphaz_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:56:31.000000 alphaz-next-0.5.6/alphaz_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-26 08:56:31.000000 alphaz-next-0.5.6/alphaz_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 08:56:31.000000 alphaz-next-0.5.6/alphaz_next.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 08:56:31.931859 alphaz-next-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-26 08:56:30.000000 alphaz-next-0.5.6/setup.py
```

### Comparing `alphaz-next-0.5.5/PKG-INFO` & `alphaz-next-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.5.5
+Version: 0.5.6
 Summary: A project to make a lib to start FASTAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.5.5.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.5.6.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.5.5/README.md` & `alphaz-next-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/auth/auth.py` & `alphaz-next-0.5.6/alphaz_next/auth/auth.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/core/_base.py` & `alphaz-next-0.5.6/alphaz_next/core/_base.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/core/_middleware.py` & `alphaz-next-0.5.6/alphaz_next/core/_middleware.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/core/application.py` & `alphaz-next-0.5.6/alphaz_next/core/application.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/core/exception_handlers.py` & `alphaz-next-0.5.6/alphaz_next/core/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/core/exceptions.py` & `alphaz-next-0.5.6/alphaz_next/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/core/responses/__init__.py` & `alphaz-next-0.5.6/alphaz_next/core/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/core/responses/file_response.py` & `alphaz-next-0.5.6/alphaz_next/core/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/core/responses/html_response.py` & `alphaz-next-0.5.6/alphaz_next/core/responses/html_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/core/responses/json_response.py` & `alphaz-next-0.5.6/alphaz_next/core/responses/json_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/core/responses/orjson_response.py` & `alphaz-next-0.5.6/alphaz_next/core/responses/orjson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/core/responses/plaintext_response.py` & `alphaz-next-0.5.6/alphaz_next/core/responses/plaintext_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/core/responses/redirect_response.py` & `alphaz-next-0.5.6/alphaz_next/core/responses/redirect_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/core/responses/response.py` & `alphaz-next-0.5.6/alphaz_next/core/responses/response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/core/responses/streaming_response.py` & `alphaz-next-0.5.6/alphaz_next/core/responses/streaming_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/core/responses/ujson_response.py` & `alphaz-next-0.5.6/alphaz_next/core/responses/ujson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/libs/httpx.py` & `alphaz-next-0.5.6/alphaz_next/libs/httpx.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/models/config/_base/internal_config_settings.py` & `alphaz-next-0.5.6/alphaz_next/models/config/_base/internal_config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/models/config/_base/utils.py` & `alphaz-next-0.5.6/alphaz_next/models/config/_base/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/models/config/alpha_config.py` & `alphaz-next-0.5.6/alphaz_next/models/config/alpha_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/models/config/api_config.py` & `alphaz-next-0.5.6/alphaz_next/models/config/api_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/models/config/apm_config.py` & `alphaz-next-0.5.6/alphaz_next/models/config/apm_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/models/config/config_settings.py` & `alphaz-next-0.5.6/alphaz_next/models/config/config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/models/config/database_config.py` & `alphaz-next-0.5.6/alphaz_next/models/config/database_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/models/config/logging_config.py` & `alphaz-next-0.5.6/alphaz_next/models/config/logging_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/models/config/openapi_config_schema.py` & `alphaz-next-0.5.6/alphaz_next/models/config/openapi_config_schema.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/tests/utils/utils.py` & `alphaz-next-0.5.6/alphaz_next/tests/utils/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/utils/format.py` & `alphaz-next-0.5.6/alphaz_next/utils/format.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/utils/logger.py` & `alphaz-next-0.5.6/alphaz_next/utils/logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/utils/logging_filters.py` & `alphaz-next-0.5.6/alphaz_next/utils/logging_filters.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/alphaz_next/utils/loguru.py` & `alphaz-next-0.5.6/alphaz_next/utils/loguru.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,29 +14,49 @@
         name: str,
         level: str = "INFO",
         enqueue: bool = False,
         stream_output: bool = False,
         colorize=True,
         format: _Optional[str] = None,
     ):
+        self._name = name
+        self._level = level
+        self._is_new = True
         if name in _LOGGERS:
+            self._is_new = False
             return _LOGGERS[name]
 
         self._logger = _logger.bind(service=name)
 
         if stream_output:
             self._logger.add(
                 _sys.stderr,
                 format=format,
                 level=level,
                 colorize=colorize,
                 filter=lambda record: record["extra"].get("service") == name,
                 enqueue=enqueue,
             )
 
+    @property
+    def name(self) -> str:
+        return self._name
+
+    @property
+    def level(self) -> str:
+        return self._level
+
+    @property
+    def is_new(self) -> bool:
+        return self._is_new
+
+    @property
+    def sub_logger(self):
+        return self._logger
+
     def _log(self, level: str, message: str):
         span = _trace.get_current_span()
         otelSpanID = _trace.format_span_id(span.get_span_context().span_id)
         otelTraceID = _trace.format_trace_id(span.get_span_context().trace_id)
 
         with self._logger.contextualize(
             otelTraceID=otelTraceID,
```

### Comparing `alphaz-next-0.5.5/alphaz_next.egg-info/PKG-INFO` & `alphaz-next-0.5.6/alphaz_next.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.5.5
+Version: 0.5.6
 Summary: A project to make a lib to start FASTAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.5.5.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.5.6.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.5.5/alphaz_next.egg-info/SOURCES.txt` & `alphaz-next-0.5.6/alphaz_next.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.5/setup.py` & `alphaz-next-0.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.5.5"
+version = "0.5.6"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 
 EXTRAS_REQUIRE = {
     "dependency-injector": ["dependency-injector"],
```

