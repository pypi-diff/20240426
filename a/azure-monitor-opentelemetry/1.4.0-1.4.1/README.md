# Comparing `tmp/azure-monitor-opentelemetry-1.4.0.tar.gz` & `tmp/azure-monitor-opentelemetry-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-monitor-opentelemetry-1.4.0.tar", last modified: Mon Apr  8 22:28:42 2024, max compression
+gzip compressed data, was "azure-monitor-opentelemetry-1.4.1.tar", last modified: Fri Apr 26 19:16:06 2024, max compression
```

## Comparing `azure-monitor-opentelemetry-1.4.0.tar` & `azure-monitor-opentelemetry-1.4.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.302276 azure-monitor-opentelemetry-1.4.0/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10782 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      199 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/MANIFEST.in
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8273 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/NOTICE.txt
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    20741 2024-04-08 22:28:42.302276 azure-monitor-opentelemetry-1.4.0/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19172 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.290276 azure-monitor-opentelemetry-1.4.0/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.290276 azure-monitor-opentelemetry-1.4.0/azure/monitor/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.290276 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      480 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.290276 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_autoinstrumentation/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      305 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_autoinstrumentation/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1560 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_autoinstrumentation/configurator.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3018 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_autoinstrumentation/distro.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8753 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_configure.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1893 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_constants.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.290276 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_diagnostics/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_diagnostics/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3582 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_diagnostics/diagnostic_logging.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2157 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_diagnostics/status_logger.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      709 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_types.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.290276 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_utils/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2065 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_utils/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5914 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_utils/configurations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      325 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_version.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      193 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.302276 azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    20741 2024-04-08 22:28:42.000000 azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3081 2024-04-08 22:28:42.000000 azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-08 22:28:42.000000 azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      295 2024-04-08 22:28:42.000000 azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/entry_points.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-08 22:28:42.000000 azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      481 2024-04-08 22:28:42.000000 azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-08 22:28:42.000000 azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      135 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/pyproject.toml
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.294276 azure-monitor-opentelemetry-1.4.0/samples/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5377 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.294276 azure-monitor-opentelemetry-1.4.0/samples/logging/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1285 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/logging/basic.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      845 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/logging/correlated_logs.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      634 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/logging/custom_properties.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      818 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/logging/exception_logs.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/logging/logs_with_traces.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.294276 azure-monitor-opentelemetry-1.4.0/samples/metrics/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      904 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/metrics/attributes.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1579 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/metrics/instruments.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.298276 azure-monitor-opentelemetry-1.4.0/samples/tracing/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      542 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/azure_core.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      740 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/db_psycopg2.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.286276 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.298276 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.298276 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      157 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/admin.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      240 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/apps.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.298276 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/migrations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/migrations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      151 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/models.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      154 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/tests.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      262 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/urls.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      626 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/views.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1130 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/manage.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.298276 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      871 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/asgi.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3404 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/settings.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      820 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/urls.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      837 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/wsgi.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2096 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/filter_spans.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1217 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/http_fastapi.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1088 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/http_flask.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1302 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/http_requests.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1106 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/http_urllib.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1087 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/http_urllib3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      834 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/instrumentation_options.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1005 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/manually_instrumented.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1306 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/modify_spans.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      801 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/sampling.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      548 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/simple.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-08 22:28:42.302276 azure-monitor-opentelemetry-1.4.0/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3719 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.298276 azure-monitor-opentelemetry-1.4.0/tests/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.302276 azure-monitor-opentelemetry-1.4.0/tests/autoinstrumentation/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2454 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/autoinstrumentation/test_configurator.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3782 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/autoinstrumentation/test_distro.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      515 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/conftest.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.302276 azure-monitor-opentelemetry-1.4.0/tests/diagnostics/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6878 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/diagnostics/test_diagnostic_logging.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5030 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/diagnostics/test_status_logger.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.302276 azure-monitor-opentelemetry-1.4.0/tests/exporter/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1365 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/exporter/test_exporter.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.302276 azure-monitor-opentelemetry-1.4.0/tests/instrumentation/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      764 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_django.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      849 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_fastapi.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      839 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_flask.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      953 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_psycopg2.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      774 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_requests.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      764 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_urllib.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      769 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_urllib3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17585 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/test_configure.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.302276 azure-monitor-opentelemetry-1.4.0/tests/utils/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10091 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/utils/test_configurations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4396 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/utils/test_utils.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.925412 azure-monitor-opentelemetry-1.4.1/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10928 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      199 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8273 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/NOTICE.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20095 2024-04-26 19:16:06.925412 azure-monitor-opentelemetry-1.4.1/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19172 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.909411 azure-monitor-opentelemetry-1.4.1/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.913411 azure-monitor-opentelemetry-1.4.1/azure/monitor/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.913411 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      480 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.913411 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_autoinstrumentation/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      305 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_autoinstrumentation/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1560 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_autoinstrumentation/configurator.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3140 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_autoinstrumentation/distro.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8768 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_configure.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1893 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_constants.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.913411 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_diagnostics/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_diagnostics/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3582 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_diagnostics/diagnostic_logging.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2157 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_diagnostics/status_logger.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      709 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_types.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.913411 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_utils/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2065 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_utils/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5914 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_utils/configurations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      325 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_version.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      193 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.917411 azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20095 2024-04-26 19:16:06.000000 azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3081 2024-04-26 19:16:06.000000 azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-26 19:16:06.000000 azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      295 2024-04-26 19:16:06.000000 azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/entry_points.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-26 19:16:06.000000 azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      481 2024-04-26 19:16:06.000000 azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-26 19:16:06.000000 azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      135 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/pyproject.toml
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.917411 azure-monitor-opentelemetry-1.4.1/samples/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5377 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.917411 azure-monitor-opentelemetry-1.4.1/samples/logging/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1285 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/logging/basic.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      845 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/logging/correlated_logs.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      634 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/logging/custom_properties.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      818 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/logging/exception_logs.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/logging/logs_with_traces.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.917411 azure-monitor-opentelemetry-1.4.1/samples/metrics/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      904 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/metrics/attributes.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1579 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/metrics/instruments.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.921411 azure-monitor-opentelemetry-1.4.1/samples/tracing/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      542 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/azure_core.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      740 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/db_psycopg2.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.909411 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.921411 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.921411 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      157 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/admin.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      240 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/apps.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.921411 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/migrations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/migrations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      151 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/models.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      154 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/tests.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      262 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/urls.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      626 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/views.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1130 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/manage.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.921411 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      871 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/asgi.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3404 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/settings.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      820 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/urls.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      837 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/wsgi.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2096 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/filter_spans.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1217 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/http_fastapi.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1088 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/http_flask.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1302 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/http_requests.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1106 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/http_urllib.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1087 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/http_urllib3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      834 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/instrumentation_options.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1005 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/manually_instrumented.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1306 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/modify_spans.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      801 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/sampling.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      548 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/simple.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-26 19:16:06.925412 azure-monitor-opentelemetry-1.4.1/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3719 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.921411 azure-monitor-opentelemetry-1.4.1/tests/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.921411 azure-monitor-opentelemetry-1.4.1/tests/autoinstrumentation/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2454 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/autoinstrumentation/test_configurator.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6167 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/autoinstrumentation/test_distro.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      515 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/conftest.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.921411 azure-monitor-opentelemetry-1.4.1/tests/diagnostics/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6878 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/diagnostics/test_diagnostic_logging.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5030 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/diagnostics/test_status_logger.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.921411 azure-monitor-opentelemetry-1.4.1/tests/exporter/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1365 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/exporter/test_exporter.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.925412 azure-monitor-opentelemetry-1.4.1/tests/instrumentation/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      764 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_django.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      849 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_fastapi.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      839 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_flask.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      953 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_psycopg2.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      774 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_requests.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      764 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_urllib.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      769 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_urllib3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17585 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/test_configure.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.925412 azure-monitor-opentelemetry-1.4.1/tests/utils/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10091 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/utils/test_configurations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4396 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/utils/test_utils.py
```

### Comparing `azure-monitor-opentelemetry-1.4.0/CHANGELOG.md` & `azure-monitor-opentelemetry-1.4.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Release History
 
+## 1.4.1 (2024-04-25)
+
+### Features Added
+
+- Enable sampling for attach
+    ([#35218](https://github.com/Azure/azure-sdk-for-python/pull/35218))
+
 ## 1.4.0 (2024-04-09)
 
 ### Features Added
 
 - Adding diagnostic warning when distro detects RP attach
     ([#34971](https://github.com/Azure/azure-sdk-for-python/pull/34971))
 - Added `resource` parameter
```

### Comparing `azure-monitor-opentelemetry-1.4.0/LICENSE` & `azure-monitor-opentelemetry-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/NOTICE.txt` & `azure-monitor-opentelemetry-1.4.1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/PKG-INFO` & `azure-monitor-opentelemetry-1.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,7 @@
-Metadata-Version: 2.1
-Name: azure-monitor-opentelemetry
-Version: 1.4.0
-Summary: Microsoft Azure Monitor Opentelemetry Distro Client Library for Python
-Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry
-Author: Microsoft Corporation
-Author-email: ascl@microsoft.com
-License: MIT License
-Keywords: azure,azure sdk
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: NOTICE.txt
-Requires-Dist: azure-core<2.0.0,>=1.28.0
-Requires-Dist: azure-core-tracing-opentelemetry~=1.0.0b11
-Requires-Dist: azure-monitor-opentelemetry-exporter~=1.0.0b24
-Requires-Dist: opentelemetry-instrumentation-django~=0.42b0
-Requires-Dist: opentelemetry-instrumentation-fastapi~=0.42b0
-Requires-Dist: opentelemetry-instrumentation-flask~=0.42b0
-Requires-Dist: opentelemetry-instrumentation-psycopg2~=0.42b0
-Requires-Dist: opentelemetry-instrumentation-requests~=0.42b0
-Requires-Dist: opentelemetry-instrumentation-urllib~=0.42b0
-Requires-Dist: opentelemetry-instrumentation-urllib3~=0.42b0
-Requires-Dist: opentelemetry-resource-detector-azure~=0.1.4
-
 # Azure Monitor Opentelemetry Distro client library for Python
 
 The Azure Monitor Distro of [Opentelemetry Python][ot_sdk_python] is a "one-stop-shop" telemetry solution, requiring only one line of code to instrument your application. The distro captures telemetry via [OpenTelemetry instrumentations][azure_monitor_opentelemetry_exporters] and reports telemetry to Azure Monitor via the [Azure Monitor exporters][azure_monitor_opentelemetry_exporters].
 
 Prior to using this SDK, please read and understand [Data Collection Basics](https://learn.microsoft.com/azure/azure-monitor/app/opentelemetry-overview?tabs=python), especially the section on [telemetry types](https://learn.microsoft.com/azure/azure-monitor/app/opentelemetry-overview?tabs=python#telemetry-types). OpenTelemetry terminology differs from Application Insights terminology so it is important to understand the way the telemetry types map to each other.
 
 This distro automatically installs the following libraries:
```

### Comparing `azure-monitor-opentelemetry-1.4.0/README.md` & `azure-monitor-opentelemetry-1.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: azure-monitor-opentelemetry
+Version: 1.4.1
+Summary: Microsoft Azure Monitor Opentelemetry Distro Client Library for Python
+Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry
+Author: Microsoft Corporation
+Author-email: ascl@microsoft.com
+License: MIT License
+Keywords: azure,azure sdk
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE.txt
+
 # Azure Monitor Opentelemetry Distro client library for Python
 
 The Azure Monitor Distro of [Opentelemetry Python][ot_sdk_python] is a "one-stop-shop" telemetry solution, requiring only one line of code to instrument your application. The distro captures telemetry via [OpenTelemetry instrumentations][azure_monitor_opentelemetry_exporters] and reports telemetry to Azure Monitor via the [Azure Monitor exporters][azure_monitor_opentelemetry_exporters].
 
 Prior to using this SDK, please read and understand [Data Collection Basics](https://learn.microsoft.com/azure/azure-monitor/app/opentelemetry-overview?tabs=python), especially the section on [telemetry types](https://learn.microsoft.com/azure/azure-monitor/app/opentelemetry-overview?tabs=python#telemetry-types). OpenTelemetry terminology differs from Application Insights terminology so it is important to understand the way the telemetry types map to each other.
 
 This distro automatically installs the following libraries:
```

### Comparing `azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_autoinstrumentation/configurator.py` & `azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_autoinstrumentation/configurator.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_autoinstrumentation/distro.py` & `azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_autoinstrumentation/distro.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 )
 from opentelemetry.instrumentation.distro import ( # type: ignore
     BaseDistro,
 )
 from opentelemetry.sdk.environment_variables import (
     _OTEL_PYTHON_LOGGING_AUTO_INSTRUMENTATION_ENABLED,
     OTEL_EXPERIMENTAL_RESOURCE_DETECTORS,
+    OTEL_TRACES_SAMPLER,
 )
 
 from azure.core.settings import settings
 from azure.core.tracing.ext.opentelemetry_span import OpenTelemetrySpan
 from azure.monitor.opentelemetry.exporter._utils import _is_attach_enabled # pylint: disable=import-error,no-name-in-module
 from azure.monitor.opentelemetry._constants import (
     _AZURE_APP_SERVICE_RESOURCE_DETECTOR_NAME,
@@ -67,14 +68,17 @@
     environ.setdefault(
         OTEL_TRACES_EXPORTER, "azure_monitor_opentelemetry_exporter"
     )
     environ.setdefault(
         OTEL_LOGS_EXPORTER, "azure_monitor_opentelemetry_exporter"
     )
     environ.setdefault(
+        OTEL_TRACES_SAMPLER, "azure_monitor_opentelemetry_sampler"
+    )
+    environ.setdefault(
         _OTEL_PYTHON_LOGGING_AUTO_INSTRUMENTATION_ENABLED, "true"
     )
     environ.setdefault(
         OTEL_EXPERIMENTAL_RESOURCE_DETECTORS, _AZURE_APP_SERVICE_RESOURCE_DETECTOR_NAME
     )
     otel_disabled_instrumentations = _get_otel_disabled_instrumentations()
     if _AZURE_SDK_INSTRUMENTATION_NAME not in otel_disabled_instrumentations:
```

### Comparing `azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_configure.py` & `azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_configure.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         if not _is_instrumentation_enabled(configurations, lib_name):
             _logger.debug(
                 "Instrumentation skipped for library %s", entry_point.name
             )
             continue
         try:
             # Check if dependent libraries/version are installed
-            conflict = get_dist_dependency_conflicts(entry_point.dist)
+            conflict = get_dist_dependency_conflicts(entry_point.dist) # type: ignore
             if conflict:
                 _logger.debug(
                     "Skipping instrumentation %s: %s",
                     entry_point.name,
                     conflict,
                 )
                 continue
```

### Comparing `azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_constants.py` & `azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_constants.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_diagnostics/diagnostic_logging.py` & `azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_diagnostics/diagnostic_logging.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_diagnostics/status_logger.py` & `azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_diagnostics/status_logger.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_types.py` & `azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_types.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_utils/__init__.py` & `azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_utils/configurations.py` & `azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_utils/configurations.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/PKG-INFO` & `azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-monitor-opentelemetry
-Version: 1.4.0
+Version: 1.4.1
 Summary: Microsoft Azure Monitor Opentelemetry Distro Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,25 +16,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE.txt
-Requires-Dist: azure-core<2.0.0,>=1.28.0
-Requires-Dist: azure-core-tracing-opentelemetry~=1.0.0b11
-Requires-Dist: azure-monitor-opentelemetry-exporter~=1.0.0b24
-Requires-Dist: opentelemetry-instrumentation-django~=0.42b0
-Requires-Dist: opentelemetry-instrumentation-fastapi~=0.42b0
-Requires-Dist: opentelemetry-instrumentation-flask~=0.42b0
-Requires-Dist: opentelemetry-instrumentation-psycopg2~=0.42b0
-Requires-Dist: opentelemetry-instrumentation-requests~=0.42b0
-Requires-Dist: opentelemetry-instrumentation-urllib~=0.42b0
-Requires-Dist: opentelemetry-instrumentation-urllib3~=0.42b0
-Requires-Dist: opentelemetry-resource-detector-azure~=0.1.4
 
 # Azure Monitor Opentelemetry Distro client library for Python
 
 The Azure Monitor Distro of [Opentelemetry Python][ot_sdk_python] is a "one-stop-shop" telemetry solution, requiring only one line of code to instrument your application. The distro captures telemetry via [OpenTelemetry instrumentations][azure_monitor_opentelemetry_exporters] and reports telemetry to Azure Monitor via the [Azure Monitor exporters][azure_monitor_opentelemetry_exporters].
 
 Prior to using this SDK, please read and understand [Data Collection Basics](https://learn.microsoft.com/azure/azure-monitor/app/opentelemetry-overview?tabs=python), especially the section on [telemetry types](https://learn.microsoft.com/azure/azure-monitor/app/opentelemetry-overview?tabs=python#telemetry-types). OpenTelemetry terminology differs from Application Insights terminology so it is important to understand the way the telemetry types map to each other.
```

### Comparing `azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/SOURCES.txt` & `azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/README.md` & `azure-monitor-opentelemetry-1.4.1/samples/README.md`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/logging/basic.py` & `azure-monitor-opentelemetry-1.4.1/samples/logging/basic.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/logging/correlated_logs.py` & `azure-monitor-opentelemetry-1.4.1/samples/logging/correlated_logs.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/logging/custom_properties.py` & `azure-monitor-opentelemetry-1.4.1/samples/logging/custom_properties.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/logging/exception_logs.py` & `azure-monitor-opentelemetry-1.4.1/samples/logging/exception_logs.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/logging/logs_with_traces.py` & `azure-monitor-opentelemetry-1.4.1/samples/logging/logs_with_traces.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/metrics/attributes.py` & `azure-monitor-opentelemetry-1.4.1/samples/metrics/attributes.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/metrics/instruments.py` & `azure-monitor-opentelemetry-1.4.1/samples/metrics/instruments.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/azure_core.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/azure_core.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/db_psycopg2.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/db_psycopg2.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/views.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/views.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/manage.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/manage.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/asgi.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/asgi.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/settings.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/settings.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/urls.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/urls.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/wsgi.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/wsgi.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/filter_spans.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/filter_spans.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/http_fastapi.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/http_fastapi.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/http_flask.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/http_flask.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/http_requests.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/http_requests.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/http_urllib.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/http_urllib.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/http_urllib3.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/http_urllib3.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/instrumentation_options.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/instrumentation_options.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/manually_instrumented.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/manually_instrumented.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/modify_spans.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/modify_spans.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/sampling.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/sampling.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/samples/tracing/simple.py` & `azure-monitor-opentelemetry-1.4.1/samples/tracing/simple.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/setup.py` & `azure-monitor-opentelemetry-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     package_data={
         "pytyped": ["py.typed"],
     },
     python_requires=">=3.8",
     install_requires=[
         "azure-core<2.0.0,>=1.28.0",
         "azure-core-tracing-opentelemetry~=1.0.0b11",
-        "azure-monitor-opentelemetry-exporter~=1.0.0b24",
+        "azure-monitor-opentelemetry-exporter~=1.0.0b25",
         "opentelemetry-instrumentation-django~=0.42b0",
         "opentelemetry-instrumentation-fastapi~=0.42b0",
         "opentelemetry-instrumentation-flask~=0.42b0",
         "opentelemetry-instrumentation-psycopg2~=0.42b0",
         "opentelemetry-instrumentation-requests~=0.42b0",
         "opentelemetry-instrumentation-urllib~=0.42b0",
         "opentelemetry-instrumentation-urllib3~=0.42b0",
```

### Comparing `azure-monitor-opentelemetry-1.4.0/tests/autoinstrumentation/test_configurator.py` & `azure-monitor-opentelemetry-1.4.1/tests/autoinstrumentation/test_configurator.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/tests/conftest.py` & `azure-monitor-opentelemetry-1.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/tests/diagnostics/test_diagnostic_logging.py` & `azure-monitor-opentelemetry-1.4.1/tests/diagnostics/test_diagnostic_logging.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/tests/diagnostics/test_status_logger.py` & `azure-monitor-opentelemetry-1.4.1/tests/diagnostics/test_status_logger.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/tests/exporter/test_exporter.py` & `azure-monitor-opentelemetry-1.4.1/tests/exporter/test_exporter.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_django.py` & `azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_django.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_fastapi.py` & `azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_flask.py` & `azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_flask.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_psycopg2.py` & `azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_psycopg2.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_requests.py` & `azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_requests.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_urllib.py` & `azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_urllib.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_urllib3.py` & `azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_urllib3.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/tests/test_configure.py` & `azure-monitor-opentelemetry-1.4.1/tests/test_configure.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/tests/utils/test_configurations.py` & `azure-monitor-opentelemetry-1.4.1/tests/utils/test_configurations.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.0/tests/utils/test_utils.py` & `azure-monitor-opentelemetry-1.4.1/tests/utils/test_utils.py`

 * *Files identical despite different names*

