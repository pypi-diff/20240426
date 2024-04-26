# Comparing `tmp/python_dev_utils-1.4.0.tar.gz` & `tmp/python_dev_utils-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_dev_utils-1.4.0.tar", last modified: Tue Apr 23 09:10:19 2024, max compression
+gzip compressed data, was "python_dev_utils-1.5.0.tar", last modified: Fri Apr 26 11:58:12 2024, max compression
```

## Comparing `python_dev_utils-1.4.0.tar` & `python_dev_utils-1.5.0.tar`

### file list

```diff
@@ -1,74 +1,80 @@
--rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-1.4.0/LICENCE
--rw-r--r--   0        0        0     5120 2024-04-23 09:09:42.701197 python_dev_utils-1.4.0/README.md
--rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-1.4.0/dev_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 06:33:01.146013 python_dev_utils-1.4.0/dev_utils/core/__init__.py
--rw-r--r--   0        0        0     5015 2024-04-12 09:11:29.068964 python_dev_utils-1.4.0/dev_utils/core/abstract.py
--rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-1.4.0/dev_utils/core/exc.py
--rw-r--r--   0        0        0      571 2024-04-12 12:22:55.526998 python_dev_utils-1.4.0/dev_utils/core/guards.py
--rw-r--r--   0        0        0      823 2024-04-12 09:11:29.068964 python_dev_utils-1.4.0/dev_utils/core/logging.py
--rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-1.4.0/dev_utils/core/results.py
--rw-r--r--   0        0        0      215 2024-04-16 09:16:58.960481 python_dev_utils-1.4.0/dev_utils/core/utils/__init__.py
--rw-r--r--   0        0        0      293 2024-04-16 09:15:43.772084 python_dev_utils-1.4.0/dev_utils/core/utils/datetime.py
--rw-r--r--   0        0        0      677 2024-04-16 09:16:22.025777 python_dev_utils-1.4.0/dev_utils/core/utils/inspect.py
--rw-r--r--   0        0        0      209 2024-04-16 09:13:36.355106 python_dev_utils-1.4.0/dev_utils/core/utils/text.py
--rw-r--r--   0        0        0     1618 2024-04-12 10:34:31.616028 python_dev_utils-1.4.0/dev_utils/fastapi/__init__.py
--rw-r--r--   0        0        0      315 2024-04-12 10:32:28.920904 python_dev_utils-1.4.0/dev_utils/fastapi/middlewares/__init__.py
--rw-r--r--   0        0        0     2889 2024-04-12 09:11:29.068964 python_dev_utils-1.4.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py
--rw-r--r--   0        0        0        0 2024-04-22 08:05:13.247824 python_dev_utils-1.4.0/dev_utils/fastapi/openapi/__init__.py
--rw-r--r--   0        0        0     1901 2024-04-23 07:13:12.131657 python_dev_utils-1.4.0/dev_utils/fastapi/openapi/exporter.py
--rw-r--r--   0        0        0     1564 2024-04-12 10:31:39.700255 python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/__init__.py
--rw-r--r--   0        0        0     3474 2024-04-22 09:15:05.523504 python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/constants.py
--rw-r--r--   0        0        0    12499 2024-04-22 09:09:07.827456 python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/exc.py
--rw-r--r--   0        0        0     3724 2024-04-22 13:05:32.395150 python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/handlers.py
--rw-r--r--   0        0        0     2184 2024-04-22 12:42:55.028588 python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/openapi_override.py
--rw-r--r--   0        0        0     1265 2024-04-22 09:31:33.905990 python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/utils.py
--rw-r--r--   0        0        0        0 2024-04-16 07:40:41.209053 python_dev_utils-1.4.0/dev_utils/py.typed
--rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-1.4.0/dev_utils/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-1.4.0/dev_utils/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    16338 2024-04-16 06:54:27.234711 python_dev_utils-1.4.0/dev_utils/sqlalchemy/filters/converters.py
--rw-r--r--   0        0        0     1538 2024-04-12 09:11:29.068964 python_dev_utils-1.4.0/dev_utils/sqlalchemy/filters/guards.py
--rw-r--r--   0        0        0     9556 2024-04-12 09:11:29.069965 python_dev_utils-1.4.0/dev_utils/sqlalchemy/filters/operators.py
--rw-r--r--   0        0        0     1283 2024-04-12 09:11:29.068964 python_dev_utils-1.4.0/dev_utils/sqlalchemy/filters/types.py
--rw-r--r--   0        0        0        0 2024-04-09 13:34:17.832279 python_dev_utils-1.4.0/dev_utils/sqlalchemy/mixins/__init__.py
--rw-r--r--   0        0        0     3050 2024-04-10 14:09:42.769706 python_dev_utils-1.4.0/dev_utils/sqlalchemy/mixins/audit.py
--rw-r--r--   0        0        0     1141 2024-04-10 08:55:37.140201 python_dev_utils-1.4.0/dev_utils/sqlalchemy/mixins/base.py
--rw-r--r--   0        0        0     1302 2024-04-10 10:08:21.445027 python_dev_utils-1.4.0/dev_utils/sqlalchemy/mixins/general.py
--rw-r--r--   0        0        0      888 2024-04-12 09:11:29.068964 python_dev_utils-1.4.0/dev_utils/sqlalchemy/mixins/ids.py
--rw-r--r--   0        0        0        0 2024-04-11 07:41:17.195661 python_dev_utils-1.4.0/dev_utils/sqlalchemy/profiling/__init__.py
--rw-r--r--   0        0        0     1737 2024-04-12 09:11:29.068964 python_dev_utils-1.4.0/dev_utils/sqlalchemy/profiling/containers.py
--rw-r--r--   0        0        0     9776 2024-04-12 09:11:29.069965 python_dev_utils-1.4.0/dev_utils/sqlalchemy/profiling/profilers.py
--rw-r--r--   0        0        0      951 2024-04-12 09:11:29.068964 python_dev_utils-1.4.0/dev_utils/sqlalchemy/profiling/utils.py
--rw-r--r--   0        0        0        0 2024-04-10 14:06:40.669620 python_dev_utils-1.4.0/dev_utils/sqlalchemy/types/__init__.py
--rw-r--r--   0        0        0     2244 2024-04-16 07:24:43.054226 python_dev_utils-1.4.0/dev_utils/sqlalchemy/types/datetime.py
--rw-r--r--   0        0        0    12968 2024-04-23 07:39:23.870346 python_dev_utils-1.4.0/dev_utils/sqlalchemy/utils.py
--rw-r--r--   0        0        0     3222 2024-04-23 09:10:19.654825 python_dev_utils-1.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-1.4.0/tests/__init__.py
--rw-r--r--   0        0        0     9123 2024-04-12 09:01:52.921056 python_dev_utils-1.4.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-1.4.0/tests/core/__init__.py
--rw-r--r--   0        0        0     2110 2024-04-12 09:01:52.921056 python_dev_utils-1.4.0/tests/core/test_abstract.py
--rw-r--r--   0        0        0      876 2024-04-16 09:26:13.267072 python_dev_utils-1.4.0/tests/core/test_guards.py
--rw-r--r--   0        0        0     1040 2024-04-12 09:01:52.921056 python_dev_utils-1.4.0/tests/core/test_results.py
--rw-r--r--   0        0        0     1278 2024-04-16 09:18:12.890888 python_dev_utils-1.4.0/tests/core/test_utils.py
--rw-r--r--   0        0        0        0 2024-04-11 07:48:56.872907 python_dev_utils-1.4.0/tests/fastapi/__init__.py
--rw-r--r--   0        0        0     1409 2024-04-22 12:43:33.722241 python_dev_utils-1.4.0/tests/fastapi/conftest.py
--rw-r--r--   0        0        0      342 2024-04-12 09:01:52.921056 python_dev_utils-1.4.0/tests/fastapi/test_middlewares.py
--rw-r--r--   0        0        0     6068 2024-04-12 12:24:15.157626 python_dev_utils-1.4.0/tests/fastapi/test_verbose_http_exceptions.py
--rw-r--r--   0        0        0     2074 2024-04-22 12:16:38.058690 python_dev_utils-1.4.0/tests/fastapi/test_verbose_http_exceptions_handlers.py
--rw-r--r--   0        0        0     1609 2024-04-22 13:12:15.337384 python_dev_utils-1.4.0/tests/fastapi/test_verbose_http_exceptions_utils.py
--rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-1.4.0/tests/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 09:04:52.305307 python_dev_utils-1.4.0/tests/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    17186 2024-04-12 09:01:52.922056 python_dev_utils-1.4.0/tests/sqlalchemy/filters/test_converters.py
--rw-r--r--   0        0        0     1210 2024-04-12 09:01:52.921056 python_dev_utils-1.4.0/tests/sqlalchemy/filters/test_guards.py
--rw-r--r--   0        0        0     7428 2024-04-12 09:01:52.929056 python_dev_utils-1.4.0/tests/sqlalchemy/filters/test_operators.py
--rw-r--r--   0        0        0        0 2024-04-10 09:04:47.480359 python_dev_utils-1.4.0/tests/sqlalchemy/mixins/__init__.py
--rw-r--r--   0        0        0     1263 2024-04-10 09:43:27.113285 python_dev_utils-1.4.0/tests/sqlalchemy/mixins/test_audit.py
--rw-r--r--   0        0        0     1241 2024-04-12 09:01:52.921056 python_dev_utils-1.4.0/tests/sqlalchemy/mixins/test_base.py
--rw-r--r--   0        0        0     1122 2024-04-12 09:01:52.921056 python_dev_utils-1.4.0/tests/sqlalchemy/mixins/test_general.py
--rw-r--r--   0        0        0      452 2024-04-12 09:01:52.920056 python_dev_utils-1.4.0/tests/sqlalchemy/mixins/test_ids.py
--rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-1.4.0/tests/sqlalchemy/profiling/__init__.py
--rw-r--r--   0        0        0     3038 2024-04-12 09:01:52.921056 python_dev_utils-1.4.0/tests/sqlalchemy/profiling/test_profilers.py
--rw-r--r--   0        0        0     1423 2024-04-22 12:17:27.599234 python_dev_utils-1.4.0/tests/sqlalchemy/test_types.py
--rw-r--r--   0        0        0     7531 2024-04-23 07:55:54.751248 python_dev_utils-1.4.0/tests/sqlalchemy/test_utils.py
--rw-r--r--   0        0        0      804 2024-04-12 09:01:52.920056 python_dev_utils-1.4.0/tests/types.py
--rw-r--r--   0        0        0     7568 2024-04-22 12:17:42.133100 python_dev_utils-1.4.0/tests/utils.py
--rw-r--r--   0        0        0     5823 1970-01-01 00:00:00.000000 python_dev_utils-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-1.5.0/LICENCE
+-rw-r--r--   0        0        0     5120 2024-04-23 09:09:42.701197 python_dev_utils-1.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-1.5.0/dev_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:24:56.058018 python_dev_utils-1.5.0/dev_utils/alembic/__init__.py
+-rw-r--r--   0        0        0      921 2024-04-25 13:19:12.947590 python_dev_utils-1.5.0/dev_utils/alembic/migration_numbering.py
+-rw-r--r--   0        0        0        0 2024-03-20 06:33:01.146013 python_dev_utils-1.5.0/dev_utils/core/__init__.py
+-rw-r--r--   0        0        0     5015 2024-04-12 09:11:29.068964 python_dev_utils-1.5.0/dev_utils/core/abstract.py
+-rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-1.5.0/dev_utils/core/exc.py
+-rw-r--r--   0        0        0      571 2024-04-12 12:22:55.526998 python_dev_utils-1.5.0/dev_utils/core/guards.py
+-rw-r--r--   0        0        0      823 2024-04-12 09:11:29.068964 python_dev_utils-1.5.0/dev_utils/core/logging.py
+-rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-1.5.0/dev_utils/core/results.py
+-rw-r--r--   0        0        0      215 2024-04-16 09:16:58.960481 python_dev_utils-1.5.0/dev_utils/core/utils/__init__.py
+-rw-r--r--   0        0        0      265 2024-04-26 08:51:43.164520 python_dev_utils-1.5.0/dev_utils/core/utils/datetime.py
+-rw-r--r--   0        0        0      677 2024-04-16 09:16:22.025777 python_dev_utils-1.5.0/dev_utils/core/utils/inspect.py
+-rw-r--r--   0        0        0      209 2024-04-16 09:13:36.355106 python_dev_utils-1.5.0/dev_utils/core/utils/text.py
+-rw-r--r--   0        0        0     1618 2024-04-12 10:34:31.616028 python_dev_utils-1.5.0/dev_utils/fastapi/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-12 10:32:28.920904 python_dev_utils-1.5.0/dev_utils/fastapi/middlewares/__init__.py
+-rw-r--r--   0        0        0     2889 2024-04-12 09:11:29.068964 python_dev_utils-1.5.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py
+-rw-r--r--   0        0        0        0 2024-04-22 08:05:13.247824 python_dev_utils-1.5.0/dev_utils/fastapi/openapi/__init__.py
+-rw-r--r--   0        0        0     1901 2024-04-23 07:13:12.131657 python_dev_utils-1.5.0/dev_utils/fastapi/openapi/exporter.py
+-rw-r--r--   0        0        0     1564 2024-04-12 10:31:39.700255 python_dev_utils-1.5.0/dev_utils/fastapi/verbose_http_exceptions/__init__.py
+-rw-r--r--   0        0        0     3474 2024-04-22 09:15:05.523504 python_dev_utils-1.5.0/dev_utils/fastapi/verbose_http_exceptions/constants.py
+-rw-r--r--   0        0        0    12499 2024-04-22 09:09:07.827456 python_dev_utils-1.5.0/dev_utils/fastapi/verbose_http_exceptions/exc.py
+-rw-r--r--   0        0        0     3724 2024-04-22 13:05:32.395150 python_dev_utils-1.5.0/dev_utils/fastapi/verbose_http_exceptions/handlers.py
+-rw-r--r--   0        0        0     2184 2024-04-22 12:42:55.028588 python_dev_utils-1.5.0/dev_utils/fastapi/verbose_http_exceptions/openapi_override.py
+-rw-r--r--   0        0        0     1265 2024-04-22 09:31:33.905990 python_dev_utils-1.5.0/dev_utils/fastapi/verbose_http_exceptions/utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 07:40:41.209053 python_dev_utils-1.5.0/dev_utils/py.typed
+-rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-1.5.0/dev_utils/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-1.5.0/dev_utils/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    16338 2024-04-16 06:54:27.234711 python_dev_utils-1.5.0/dev_utils/sqlalchemy/filters/converters.py
+-rw-r--r--   0        0        0     1538 2024-04-12 09:11:29.068964 python_dev_utils-1.5.0/dev_utils/sqlalchemy/filters/guards.py
+-rw-r--r--   0        0        0     9556 2024-04-12 09:11:29.069965 python_dev_utils-1.5.0/dev_utils/sqlalchemy/filters/operators.py
+-rw-r--r--   0        0        0     1283 2024-04-12 09:11:29.068964 python_dev_utils-1.5.0/dev_utils/sqlalchemy/filters/types.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:34:17.832279 python_dev_utils-1.5.0/dev_utils/sqlalchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     3050 2024-04-10 14:09:42.769706 python_dev_utils-1.5.0/dev_utils/sqlalchemy/mixins/audit.py
+-rw-r--r--   0        0        0     1187 2024-04-25 09:18:45.437647 python_dev_utils-1.5.0/dev_utils/sqlalchemy/mixins/base.py
+-rw-r--r--   0        0        0     6474 2024-04-26 09:53:43.191401 python_dev_utils-1.5.0/dev_utils/sqlalchemy/mixins/general.py
+-rw-r--r--   0        0        0      888 2024-04-12 09:11:29.068964 python_dev_utils-1.5.0/dev_utils/sqlalchemy/mixins/ids.py
+-rw-r--r--   0        0        0     1005 2024-04-25 11:36:06.219628 python_dev_utils-1.5.0/dev_utils/sqlalchemy/naming_conventions.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:41:17.195661 python_dev_utils-1.5.0/dev_utils/sqlalchemy/profiling/__init__.py
+-rw-r--r--   0        0        0     1737 2024-04-12 09:11:29.068964 python_dev_utils-1.5.0/dev_utils/sqlalchemy/profiling/containers.py
+-rw-r--r--   0        0        0     9776 2024-04-12 09:11:29.069965 python_dev_utils-1.5.0/dev_utils/sqlalchemy/profiling/profilers.py
+-rw-r--r--   0        0        0      951 2024-04-12 09:11:29.068964 python_dev_utils-1.5.0/dev_utils/sqlalchemy/profiling/utils.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:06:40.669620 python_dev_utils-1.5.0/dev_utils/sqlalchemy/types/__init__.py
+-rw-r--r--   0        0        0     2244 2024-04-16 07:24:43.054226 python_dev_utils-1.5.0/dev_utils/sqlalchemy/types/datetime.py
+-rw-r--r--   0        0        0    14281 2024-04-25 13:17:22.836564 python_dev_utils-1.5.0/dev_utils/sqlalchemy/utils.py
+-rw-r--r--   0        0        0     3263 2024-04-26 11:58:12.639850 python_dev_utils-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-1.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     9123 2024-04-12 09:01:52.921056 python_dev_utils-1.5.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-1.5.0/tests/core/__init__.py
+-rw-r--r--   0        0        0     2110 2024-04-12 09:01:52.921056 python_dev_utils-1.5.0/tests/core/test_abstract.py
+-rw-r--r--   0        0        0      876 2024-04-16 09:26:13.267072 python_dev_utils-1.5.0/tests/core/test_guards.py
+-rw-r--r--   0        0        0     1040 2024-04-12 09:01:52.921056 python_dev_utils-1.5.0/tests/core/test_results.py
+-rw-r--r--   0        0        0     1278 2024-04-16 09:18:12.890888 python_dev_utils-1.5.0/tests/core/test_utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:48:56.872907 python_dev_utils-1.5.0/tests/fastapi/__init__.py
+-rw-r--r--   0        0        0     1409 2024-04-22 12:43:33.722241 python_dev_utils-1.5.0/tests/fastapi/conftest.py
+-rw-r--r--   0        0        0      342 2024-04-12 09:01:52.921056 python_dev_utils-1.5.0/tests/fastapi/test_middlewares.py
+-rw-r--r--   0        0        0     6068 2024-04-12 12:24:15.157626 python_dev_utils-1.5.0/tests/fastapi/test_verbose_http_exceptions.py
+-rw-r--r--   0        0        0     2074 2024-04-22 12:16:38.058690 python_dev_utils-1.5.0/tests/fastapi/test_verbose_http_exceptions_handlers.py
+-rw-r--r--   0        0        0     1609 2024-04-22 13:12:15.337384 python_dev_utils-1.5.0/tests/fastapi/test_verbose_http_exceptions_utils.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-1.5.0/tests/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:04:52.305307 python_dev_utils-1.5.0/tests/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    17186 2024-04-12 09:01:52.922056 python_dev_utils-1.5.0/tests/sqlalchemy/filters/test_converters.py
+-rw-r--r--   0        0        0     1210 2024-04-12 09:01:52.921056 python_dev_utils-1.5.0/tests/sqlalchemy/filters/test_guards.py
+-rw-r--r--   0        0        0     7428 2024-04-12 09:01:52.929056 python_dev_utils-1.5.0/tests/sqlalchemy/filters/test_operators.py
+-rw-r--r--   0        0        0        0 2024-04-26 06:25:13.597435 python_dev_utils-1.5.0/tests/sqlalchemy/migrations/__init__.py
+-rw-r--r--   0        0        0      772 2024-04-26 09:16:01.643863 python_dev_utils-1.5.0/tests/sqlalchemy/migrations/test_migration_numbering.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:04:47.480359 python_dev_utils-1.5.0/tests/sqlalchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     1263 2024-04-10 09:43:27.113285 python_dev_utils-1.5.0/tests/sqlalchemy/mixins/test_audit.py
+-rw-r--r--   0        0        0     1241 2024-04-12 09:01:52.921056 python_dev_utils-1.5.0/tests/sqlalchemy/mixins/test_base.py
+-rw-r--r--   0        0        0     7544 2024-04-26 09:36:52.825485 python_dev_utils-1.5.0/tests/sqlalchemy/mixins/test_general.py
+-rw-r--r--   0        0        0      452 2024-04-12 09:01:52.920056 python_dev_utils-1.5.0/tests/sqlalchemy/mixins/test_ids.py
+-rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-1.5.0/tests/sqlalchemy/profiling/__init__.py
+-rw-r--r--   0        0        0     3038 2024-04-12 09:01:52.921056 python_dev_utils-1.5.0/tests/sqlalchemy/profiling/test_profilers.py
+-rw-r--r--   0        0        0      394 2024-04-26 09:26:06.714312 python_dev_utils-1.5.0/tests/sqlalchemy/test_naming_conventions.py
+-rw-r--r--   0        0        0     1423 2024-04-22 12:17:27.599234 python_dev_utils-1.5.0/tests/sqlalchemy/test_types.py
+-rw-r--r--   0        0        0     9789 2024-04-25 13:18:24.229021 python_dev_utils-1.5.0/tests/sqlalchemy/test_utils.py
+-rw-r--r--   0        0        0      804 2024-04-12 09:01:52.920056 python_dev_utils-1.5.0/tests/types.py
+-rw-r--r--   0        0        0     7683 2024-04-25 12:36:46.358159 python_dev_utils-1.5.0/tests/utils.py
+-rw-r--r--   0        0        0     5914 1970-01-01 00:00:00.000000 python_dev_utils-1.5.0/PKG-INFO
```

### Comparing `python_dev_utils-1.4.0/LICENCE` & `python_dev_utils-1.5.0/LICENCE`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/README.md` & `python_dev_utils-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/core/abstract.py` & `python_dev_utils-1.5.0/dev_utils/core/abstract.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/core/exc.py` & `python_dev_utils-1.5.0/dev_utils/core/exc.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/core/guards.py` & `python_dev_utils-1.5.0/dev_utils/core/guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/core/logging.py` & `python_dev_utils-1.5.0/dev_utils/core/logging.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/core/results.py` & `python_dev_utils-1.5.0/dev_utils/core/results.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/core/utils/inspect.py` & `python_dev_utils-1.5.0/dev_utils/core/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/fastapi/__init__.py` & `python_dev_utils-1.5.0/dev_utils/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py` & `python_dev_utils-1.5.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/fastapi/openapi/exporter.py` & `python_dev_utils-1.5.0/dev_utils/fastapi/openapi/exporter.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/__init__.py` & `python_dev_utils-1.5.0/dev_utils/fastapi/verbose_http_exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/constants.py` & `python_dev_utils-1.5.0/dev_utils/fastapi/verbose_http_exceptions/constants.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/exc.py` & `python_dev_utils-1.5.0/dev_utils/fastapi/verbose_http_exceptions/exc.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/handlers.py` & `python_dev_utils-1.5.0/dev_utils/fastapi/verbose_http_exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/openapi_override.py` & `python_dev_utils-1.5.0/dev_utils/fastapi/verbose_http_exceptions/openapi_override.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/utils.py` & `python_dev_utils-1.5.0/dev_utils/fastapi/verbose_http_exceptions/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/sqlalchemy/filters/converters.py` & `python_dev_utils-1.5.0/dev_utils/sqlalchemy/filters/converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/sqlalchemy/filters/guards.py` & `python_dev_utils-1.5.0/dev_utils/sqlalchemy/filters/guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/sqlalchemy/filters/operators.py` & `python_dev_utils-1.5.0/dev_utils/sqlalchemy/filters/operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/sqlalchemy/filters/types.py` & `python_dev_utils-1.5.0/dev_utils/sqlalchemy/filters/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/sqlalchemy/mixins/audit.py` & `python_dev_utils-1.5.0/dev_utils/sqlalchemy/mixins/audit.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/sqlalchemy/mixins/base.py` & `python_dev_utils-1.5.0/dev_utils/sqlalchemy/mixins/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from typing import TYPE_CHECKING, Any, TypeGuard
 
 from dev_utils.core.exc import NoDeclarativeModelError
 from dev_utils.core.utils import get_object_class_absolute_name
 from dev_utils.sqlalchemy.utils import is_declarative
 
 if TYPE_CHECKING:
-    from sqlalchemy.orm import DeclarativeBase, Mapper
+    from sqlalchemy.orm.decl_api import DeclarativeBase
+    from sqlalchemy.orm.mapper import Mapper
 
 
 class BaseModelMixin:
     """Base model mixin."""
 
     @cached_property
     def _is_mixin_in_declarative_model(self) -> "TypeGuard[Mapper[Any]]":  # type: ignore
```

### Comparing `python_dev_utils-1.4.0/dev_utils/sqlalchemy/mixins/ids.py` & `python_dev_utils-1.5.0/dev_utils/sqlalchemy/mixins/ids.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/sqlalchemy/profiling/containers.py` & `python_dev_utils-1.5.0/dev_utils/sqlalchemy/profiling/containers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/sqlalchemy/profiling/profilers.py` & `python_dev_utils-1.5.0/dev_utils/sqlalchemy/profiling/profilers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/sqlalchemy/profiling/utils.py` & `python_dev_utils-1.5.0/dev_utils/sqlalchemy/profiling/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/sqlalchemy/types/datetime.py` & `python_dev_utils-1.5.0/dev_utils/sqlalchemy/types/datetime.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/dev_utils/sqlalchemy/utils.py` & `python_dev_utils-1.5.0/dev_utils/sqlalchemy/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,14 +57,59 @@
         return False
     else:
         if not hasattr(mapper, "is_mapper"):
             return False
         return mapper.is_mapper
 
 
+def get_unloaded_fields(instance: "DeclarativeBase") -> set[str]:
+    """Get unloaded fields from instance.
+
+    Args
+    ----
+    instance : DeclarativeBase
+        SQLAlchemy declarative model instance.
+
+    Returns
+    -------
+    set[str]
+        set of instance fields, which were not loaded.
+    """
+    inspector = inspect(instance)
+    return inspector.unloaded
+
+
+def get_model_instance_data_as_dict(
+    instance: "DeclarativeBase",
+    exclude: set[str] | None = None,
+) -> dict[str, Any]:
+    """Get SQLAlchemy model instance data as dict.
+
+    Args
+    ----
+    instance : DeclarativeBase
+        SQLAlchemy declarative model instance.
+    exclude : set[str] | None (default None)
+        set of string fields, which must be excluded from return result.
+
+    Returns
+    -------
+    dict[str, Any]
+        dict of instance fields with values, but without fields, which were not loaded or excluded.
+    """
+    if exclude is None:
+        exclude = set()
+    exclude = exclude.union(get_unloaded_fields(instance))
+    return {
+        col.name: getattr(instance, col.name)
+        for col in instance.__table__.columns
+        if col.name not in exclude
+    }
+
+
 @overload
 def get_sqlalchemy_attribute(
     model: type["DeclarativeBase"],
     field_name: str,
     *,
     only_columns: Literal[True],
 ) -> "InstrumentedAttribute[Any]": ...
@@ -246,34 +291,41 @@
     -------
     set[str]
         set of model relationships as strings.
     """
     return set(inspect(model).relationships.keys())
 
 
-def get_valid_field_names(model: type["DeclarativeBase"]) -> set[str]:
+def get_valid_field_names(
+    model: type["DeclarativeBase"],
+    *,
+    only_columns: bool = False,
+) -> set[str]:
     """Get sqlalchemy field names as strings from given model.
 
     It includes hybrid properties and hybrid methods, because they can be used in queries.
 
     Args
     ----
     model : type[DeclarativeBase]
         SQLAlchemy declarative model.
+    only_columns : bool (Default False)
 
     Returns
     -------
     set[str]
         set of model fields as strings.
     """
     inspect_mapper: "Mapper[Any]" = inspect(model)  # type: ignore
     columns = inspect_mapper.columns
     orm_descriptors = inspect_mapper.all_orm_descriptors
 
     column_names = columns.keys()
+    if only_columns:
+        return set(column_names)
     hybrid_names = [
         key
         for key, item in orm_descriptors.items()
         if is_hybrid_property(item) or is_hybrid_method(item)
     ]
 
     return set(column_names) | set(hybrid_names)
```

### Comparing `python_dev_utils-1.4.0/pyproject.toml` & `python_dev_utils-1.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     "asyncpg>=0.29.0",
     "pytest-asyncio>=0.23.6",
     "httpx>=0.27.0",
 ]
 
 [project]
 name = "python_dev_utils"
-version = "1.4.0"
+version = "1.5.0"
 description = "My project utils package, that I use in my projects."
 authors = [
     { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = []
@@ -198,13 +198,16 @@
 sqlalchemy_filters = [
     "sqlalchemy>=2.0.28",
 ]
 extract_openapi = [
     "fastapi",
     "uvicorn",
 ]
+migration_numbering = [
+    "alembic",
+]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `python_dev_utils-1.4.0/tests/conftest.py` & `python_dev_utils-1.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/tests/core/test_abstract.py` & `python_dev_utils-1.5.0/tests/core/test_abstract.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/tests/core/test_guards.py` & `python_dev_utils-1.5.0/tests/core/test_guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/tests/core/test_results.py` & `python_dev_utils-1.5.0/tests/core/test_results.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/tests/core/test_utils.py` & `python_dev_utils-1.5.0/tests/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/tests/fastapi/conftest.py` & `python_dev_utils-1.5.0/tests/fastapi/conftest.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/tests/fastapi/test_verbose_http_exceptions.py` & `python_dev_utils-1.5.0/tests/fastapi/test_verbose_http_exceptions.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/tests/fastapi/test_verbose_http_exceptions_handlers.py` & `python_dev_utils-1.5.0/tests/fastapi/test_verbose_http_exceptions_handlers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/tests/fastapi/test_verbose_http_exceptions_utils.py` & `python_dev_utils-1.5.0/tests/fastapi/test_verbose_http_exceptions_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/tests/sqlalchemy/filters/test_converters.py` & `python_dev_utils-1.5.0/tests/sqlalchemy/filters/test_converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/tests/sqlalchemy/filters/test_guards.py` & `python_dev_utils-1.5.0/tests/sqlalchemy/filters/test_guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/tests/sqlalchemy/filters/test_operators.py` & `python_dev_utils-1.5.0/tests/sqlalchemy/filters/test_operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/tests/sqlalchemy/mixins/test_audit.py` & `python_dev_utils-1.5.0/tests/sqlalchemy/mixins/test_audit.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/tests/sqlalchemy/mixins/test_base.py` & `python_dev_utils-1.5.0/tests/sqlalchemy/mixins/test_base.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/tests/sqlalchemy/profiling/test_profilers.py` & `python_dev_utils-1.5.0/tests/sqlalchemy/profiling/test_profilers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/tests/sqlalchemy/test_types.py` & `python_dev_utils-1.5.0/tests/sqlalchemy/test_types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/tests/sqlalchemy/test_utils.py` & `python_dev_utils-1.5.0/tests/sqlalchemy/test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,100 @@
+import datetime
 from collections.abc import Sequence
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 import pytest
 from sqlalchemy import delete, func, insert, inspect, select, update
-from sqlalchemy.orm import DeclarativeBase, joinedload, selectinload, subqueryload
+from sqlalchemy.orm import (
+    DeclarativeBase,
+    Session,
+    joinedload,
+    load_only,
+    selectinload,
+    subqueryload,
+)
 
 from dev_utils.core.exc import NoModelAttributeError, NoModelRelationshipError
 from dev_utils.sqlalchemy import utils
 from tests.utils import Base, MyModel, OtherModel
 
+if TYPE_CHECKING:
+    from tests.types import SyncFactoryFunctionProtocol
+
 
 @pytest.mark.parametrize(
     ("obj", "expected_result"),
     [
         (MyModel, True),
         (254, False),
         (MyModel.__table__, False),
     ],
 )
 def test_is_declarative(obj: Any, expected_result: bool) -> None:  # noqa: D103, ANN401, FBT001
     assert utils.is_declarative(obj) == expected_result
 
 
+def test_get_unloaded_fields(
+    db_sync_session: "Session",
+    mymodel_sync_factory: "SyncFactoryFunctionProtocol[MyModel]",
+) -> None:
+    mymodel_sync_factory(db_sync_session)
+    selected_with_unload = db_sync_session.scalar(
+        select(MyModel).options(load_only(MyModel.bl), selectinload(MyModel.other_models)),
+    )
+    assert selected_with_unload is not None, "model not found (but should be presented in db)"
+    assert utils.get_unloaded_fields(selected_with_unload) == {"name", "other_name", "dt"}
+
+
+@pytest.mark.parametrize(
+    ("exclude", "data", "expected_result"),
+    [
+        (
+            None,
+            dict(
+                id=1,
+                name="name",
+                other_name="other_name",
+                dt=datetime.datetime(2023, 5, 25, 12, 25, 25, tzinfo=datetime.UTC),
+                bl=True,
+            ),
+            dict(
+                id=1,
+                name="name",
+                other_name="other_name",
+                dt=datetime.datetime(2023, 5, 25, 12, 25, 25, tzinfo=datetime.UTC),
+                bl=True,
+            ),
+        ),
+        (
+            {"id", "dt", "bl"},
+            dict(
+                id=1,
+                name="name",
+                other_name="other_name",
+                dt=datetime.datetime(2023, 5, 25, 12, 25, 25, tzinfo=datetime.UTC),
+                bl=True,
+            ),
+            dict(name="name", other_name="other_name"),
+        ),
+    ],
+)
+def test_get_model_instance_data_as_dict(
+    exclude: set[str] | None,
+    data: dict[str, Any],
+    expected_result: dict[str, Any],
+    db_sync_session: "Session",
+    mymodel_sync_factory: "SyncFactoryFunctionProtocol[MyModel]",
+) -> None:
+    instance = mymodel_sync_factory(db_sync_session, **data)
+    assert (
+        utils.get_model_instance_data_as_dict(instance=instance, exclude=exclude) == expected_result
+    )
+
+
 @pytest.mark.parametrize(
     ("field", "only_columns", "expected_result"),
     [
         ("id", False, MyModel.id),
         ("id", True, MyModel.id),
         ("name", False, MyModel.name),
         ("name", True, MyModel.name),
@@ -138,14 +207,24 @@
         "dt",
         "bl",
         "full_name",
         "get_full_name",
     }
 
 
+def test_get_valid_field_names_only_columns() -> None:  # noqa
+    assert utils.get_valid_field_names(MyModel, only_columns=True) == {
+        "id",
+        "name",
+        "other_name",
+        "dt",
+        "bl",
+    }
+
+
 @pytest.mark.parametrize(
     ("field", "expected_result"),
     [
         ("id", False),
         ("name", False),
         ("other_name", False),
         ("full_name", True),
```

### Comparing `python_dev_utils-1.4.0/tests/types.py` & `python_dev_utils-1.5.0/tests/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.4.0/tests/utils.py` & `python_dev_utils-1.5.0/tests/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pydantic import BaseModel
 from sqlalchemy import ForeignKey, inspect
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.ext.hybrid import hybrid_method, hybrid_property
 from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column, relationship
 from sqlalchemy_utils import create_database, database_exists, drop_database  # type: ignore
 
+from dev_utils.sqlalchemy.mixins.general import BetterReprMixin, DifferenceMixin
 from dev_utils.sqlalchemy.types.datetime import UTCDateTime
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from sqlalchemy.ext.asyncio import AsyncSession
     from sqlalchemy.orm import Session
@@ -193,15 +194,15 @@
     c: int
 
 
 class Base(DeclarativeBase):  # noqa
     pass
 
 
-class MyModel(Base):  # noqa
+class MyModel(BetterReprMixin, DifferenceMixin, Base):  # noqa
     __tablename__ = "my_model"
 
     id: Mapped[int] = mapped_column(primary_key=True)  # noqa
     name: Mapped[str | None]
     other_name: Mapped[str | None]
     dt: Mapped[datetime.datetime | None]
     bl: Mapped[bool | None]
```

### Comparing `python_dev_utils-1.4.0/PKG-INFO` & `python_dev_utils-1.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: python_dev_utils
-Version: 1.4.0
+Version: 1.5.0
 Summary: My project utils package, that I use in my projects.
 Author-Email: Dmitriy Lunev <dima.lunev14@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Provides-Extra: fastapi-exceptions
 Provides-Extra: profiling
 Provides-Extra: sqlalchemy-filters
 Provides-Extra: extract-openapi
+Provides-Extra: migration-numbering
 Requires-Dist: fastapi; extra == "fastapi-exceptions"
 Requires-Dist: fastapi; extra == "profiling"
 Requires-Dist: sqlalchemy>=2.0.28; extra == "profiling"
 Requires-Dist: sqlalchemy>=2.0.28; extra == "sqlalchemy-filters"
 Requires-Dist: fastapi; extra == "extract-openapi"
 Requires-Dist: uvicorn; extra == "extract-openapi"
+Requires-Dist: alembic; extra == "migration-numbering"
 Description-Content-Type: text/markdown
 
 
 # Dev utils
 
 ![coverage](./coverage.svg)
```

