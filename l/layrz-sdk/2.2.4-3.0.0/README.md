# Comparing `tmp/layrz-sdk-2.2.4.tar.gz` & `tmp/layrz_sdk-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layrz-sdk-2.2.4.tar", last modified: Wed Feb 28 13:05:32 2024, max compression
+gzip compressed data, was "layrz_sdk-3.0.0.tar", last modified: Fri Apr 26 06:22:50 2024, max compression
```

## Comparing `layrz-sdk-2.2.4.tar` & `layrz_sdk-3.0.0.tar`

### file list

```diff
@@ -1,90 +1,88 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:05:31.999399 layrz-sdk-2.2.4/
--rw-rw-r--   0 root         (0) root         (0)     1057 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1413 2024-02-28 13:05:31.999399 layrz-sdk-2.2.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      628 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:05:31.987399 layrz-sdk-2.2.4/layrz/
--rw-rw-r--   0 root         (0) root         (0)      210 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:05:31.987399 layrz-sdk-2.2.4/layrz/sdk/
--rw-rw-r--   0 root         (0) root         (0)       28 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:05:31.987399 layrz-sdk-2.2.4/layrz/sdk/entities/
--rw-rw-r--   0 root         (0) root         (0)     1327 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:05:31.987399 layrz-sdk-2.2.4/layrz/sdk/entities/broadcasts/
--rw-rw-r--   0 root         (0) root         (0)      215 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/broadcasts/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      566 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/broadcasts/request.py
--rw-rw-r--   0 root         (0) root         (0)      586 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/broadcasts/response.py
--rw-rw-r--   0 root         (0) root         (0)     1291 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/broadcasts/result.py
--rw-rw-r--   0 root         (0) root         (0)      543 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/broadcasts/service.py
--rw-rw-r--   0 root         (0) root         (0)      569 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/broadcasts/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:05:31.987399 layrz-sdk-2.2.4/layrz/sdk/entities/cases/
--rw-rw-r--   0 root         (0) root         (0)      135 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/cases/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2786 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/cases/case.py
--rw-rw-r--   0 root         (0) root         (0)      902 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/cases/comment.py
--rw-rw-r--   0 root         (0) root         (0)      629 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/cases/trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:05:31.991399 layrz-sdk-2.2.4/layrz/sdk/entities/charts/
--rw-rw-r--   0 root         (0) root         (0)      753 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      438 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/alignment.py
--rw-rw-r--   0 root         (0) root         (0)     3867 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/bar.py
--rw-rw-r--   0 root         (0) root         (0)     4928 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/column.py
--rw-rw-r--   0 root         (0) root         (0)      514 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/configuration.py
--rw-rw-r--   0 root         (0) root         (0)      447 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/data_type.py
--rw-rw-r--   0 root         (0) root         (0)      558 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)      995 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/html.py
--rw-rw-r--   0 root         (0) root         (0)     5175 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/line.py
--rw-rw-r--   0 root         (0) root         (0)     4230 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/map.py
--rw-rw-r--   0 root         (0) root         (0)      811 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/number.py
--rw-rw-r--   0 root         (0) root         (0)     2972 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/pie.py
--rw-rw-r--   0 root         (0) root         (0)     3155 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/radar.py
--rw-rw-r--   0 root         (0) root         (0)     3011 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/radial_bar.py
--rw-rw-r--   0 root         (0) root         (0)     4871 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/scatter.py
--rw-rw-r--   0 root         (0) root         (0)     1509 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/serie.py
--rw-rw-r--   0 root         (0) root         (0)      463 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/serie_type.py
--rw-rw-r--   0 root         (0) root         (0)     1344 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/table.py
--rw-rw-r--   0 root         (0) root         (0)     3985 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/charts/timeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:05:31.991399 layrz-sdk-2.2.4/layrz/sdk/entities/checkpoints/
--rw-rw-r--   0 root         (0) root         (0)      126 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/checkpoints/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1040 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/checkpoints/checkpoint.py
--rw-rw-r--   0 root         (0) root         (0)      653 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/checkpoints/geofence.py
--rw-rw-r--   0 root         (0) root         (0)     1236 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/checkpoints/waypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:05:31.995399 layrz-sdk-2.2.4/layrz/sdk/entities/events/
--rw-rw-r--   0 root         (0) root         (0)       49 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/events/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1175 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/events/event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:05:31.995399 layrz-sdk-2.2.4/layrz/sdk/entities/formatting/
--rw-rw-r--   0 root         (0) root         (0)       66 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/formatting/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      467 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/formatting/text_align.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:05:31.995399 layrz-sdk-2.2.4/layrz/sdk/entities/general/
--rw-rw-r--   0 root         (0) root         (0)      218 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/general/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1786 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/general/asset.py
--rw-rw-r--   0 root         (0) root         (0)      569 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/general/asset_operation_mode.py
--rw-rw-r--   0 root         (0) root         (0)      606 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/general/custom_field.py
--rw-rw-r--   0 root         (0) root         (0)      973 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/general/device.py
--rw-rw-r--   0 root         (0) root         (0)      615 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/general/sensor.py
--rw-rw-r--   0 root         (0) root         (0)      527 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/general/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:05:31.995399 layrz-sdk-2.2.4/layrz/sdk/entities/repcom/
--rw-rw-r--   0 root         (0) root         (0)       61 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/repcom/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1461 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/repcom/transaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:05:31.995399 layrz-sdk-2.2.4/layrz/sdk/entities/reports/
--rw-rw-r--   0 root         (0) root         (0)      249 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/reports/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1961 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/reports/col.py
--rw-rw-r--   0 root         (0) root         (0)      442 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/reports/format.py
--rw-rw-r--   0 root         (0) root         (0)     1408 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/reports/header.py
--rw-rw-r--   0 root         (0) root         (0)     1574 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/reports/page.py
--rw-rw-r--   0 root         (0) root         (0)     6444 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/reports/report.py
--rw-rw-r--   0 root         (0) root         (0)      881 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/reports/row.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:05:31.999399 layrz-sdk-2.2.4/layrz/sdk/entities/telemetry/
--rw-rw-r--   0 root         (0) root         (0)       87 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/telemetry/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      789 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/telemetry/message.py
--rw-rw-r--   0 root         (0) root         (0)     1327 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/entities/telemetry/position.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:05:31.999399 layrz-sdk-2.2.4/layrz/sdk/helpers/
--rw-rw-r--   0 root         (0) root         (0)       72 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/helpers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1102 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/helpers/color.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:05:31.999399 layrz-sdk-2.2.4/layrz/sdk/lcl/
--rw-rw-r--   0 root         (0) root         (0)       67 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/lcl/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    20611 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/layrz/sdk/lcl/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:05:31.999399 layrz-sdk-2.2.4/layrz_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1413 2024-02-28 13:05:31.000000 layrz-sdk-2.2.4/layrz_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2523 2024-02-28 13:05:31.000000 layrz-sdk-2.2.4/layrz_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 13:05:31.000000 layrz-sdk-2.2.4/layrz_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-02-28 13:05:31.000000 layrz-sdk-2.2.4/layrz_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-02-28 13:05:31.000000 layrz-sdk-2.2.4/layrz_sdk.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)     7661 2024-02-28 13:04:30.000000 layrz-sdk-2.2.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-28 13:05:31.999399 layrz-sdk-2.2.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.182030 layrz_sdk-3.0.0/
+-rw-rw-r--   0 root         (0) root         (0)     1057 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1458 2024-04-26 06:22:50.182030 layrz_sdk-3.0.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      628 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.170030 layrz_sdk-3.0.0/layrz_sdk/
+-rw-rw-r--   0 root         (0) root         (0)       28 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.170030 layrz_sdk-3.0.0/layrz_sdk/entities/
+-rw-rw-r--   0 root         (0) root         (0)     1327 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.170030 layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/
+-rw-rw-r--   0 root         (0) root         (0)      215 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      566 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/request.py
+-rw-rw-r--   0 root         (0) root         (0)      586 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/response.py
+-rw-rw-r--   0 root         (0) root         (0)     1291 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/result.py
+-rw-rw-r--   0 root         (0) root         (0)      543 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/service.py
+-rw-rw-r--   0 root         (0) root         (0)      569 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.170030 layrz_sdk-3.0.0/layrz_sdk/entities/cases/
+-rw-rw-r--   0 root         (0) root         (0)      135 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/cases/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2786 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/cases/case.py
+-rw-rw-r--   0 root         (0) root         (0)      902 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/cases/comment.py
+-rw-rw-r--   0 root         (0) root         (0)      629 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/cases/trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.174030 layrz_sdk-3.0.0/layrz_sdk/entities/charts/
+-rw-rw-r--   0 root         (0) root         (0)      753 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      438 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/alignment.py
+-rw-rw-r--   0 root         (0) root         (0)     3867 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/bar.py
+-rw-rw-r--   0 root         (0) root         (0)     4928 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/column.py
+-rw-rw-r--   0 root         (0) root         (0)      514 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)      447 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/data_type.py
+-rw-rw-r--   0 root         (0) root         (0)      558 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)      995 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/html.py
+-rw-rw-r--   0 root         (0) root         (0)     5175 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/line.py
+-rw-rw-r--   0 root         (0) root         (0)     4230 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/map.py
+-rw-rw-r--   0 root         (0) root         (0)      811 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/number.py
+-rw-rw-r--   0 root         (0) root         (0)     2972 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/pie.py
+-rw-rw-r--   0 root         (0) root         (0)     3155 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/radar.py
+-rw-rw-r--   0 root         (0) root         (0)     3011 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/radial_bar.py
+-rw-rw-r--   0 root         (0) root         (0)     4871 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/scatter.py
+-rw-rw-r--   0 root         (0) root         (0)     1509 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/serie.py
+-rw-rw-r--   0 root         (0) root         (0)      463 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/serie_type.py
+-rw-rw-r--   0 root         (0) root         (0)     1344 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/table.py
+-rw-rw-r--   0 root         (0) root         (0)     3985 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/timeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.178030 layrz_sdk-3.0.0/layrz_sdk/entities/checkpoints/
+-rw-rw-r--   0 root         (0) root         (0)      126 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/checkpoints/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1040 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/checkpoints/checkpoint.py
+-rw-rw-r--   0 root         (0) root         (0)      653 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/checkpoints/geofence.py
+-rw-rw-r--   0 root         (0) root         (0)     1236 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/checkpoints/waypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.178030 layrz_sdk-3.0.0/layrz_sdk/entities/events/
+-rw-rw-r--   0 root         (0) root         (0)       49 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/events/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1175 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/events/event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.178030 layrz_sdk-3.0.0/layrz_sdk/entities/formatting/
+-rw-rw-r--   0 root         (0) root         (0)       66 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/formatting/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      467 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/formatting/text_align.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.178030 layrz_sdk-3.0.0/layrz_sdk/entities/general/
+-rw-rw-r--   0 root         (0) root         (0)      218 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/general/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1786 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/general/asset.py
+-rw-rw-r--   0 root         (0) root         (0)      569 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/general/asset_operation_mode.py
+-rw-rw-r--   0 root         (0) root         (0)      606 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/general/custom_field.py
+-rw-rw-r--   0 root         (0) root         (0)      973 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/general/device.py
+-rw-rw-r--   0 root         (0) root         (0)      615 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/general/sensor.py
+-rw-rw-r--   0 root         (0) root         (0)      527 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/general/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.178030 layrz_sdk-3.0.0/layrz_sdk/entities/repcom/
+-rw-rw-r--   0 root         (0) root         (0)       61 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/repcom/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1461 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/repcom/transaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.182030 layrz_sdk-3.0.0/layrz_sdk/entities/reports/
+-rw-rw-r--   0 root         (0) root         (0)      249 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/reports/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1961 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/reports/col.py
+-rw-rw-r--   0 root         (0) root         (0)      442 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/reports/format.py
+-rw-rw-r--   0 root         (0) root         (0)     1408 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/reports/header.py
+-rw-rw-r--   0 root         (0) root         (0)     1574 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/reports/page.py
+-rw-rw-r--   0 root         (0) root         (0)     6444 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/reports/report.py
+-rw-rw-r--   0 root         (0) root         (0)      881 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/reports/row.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.182030 layrz_sdk-3.0.0/layrz_sdk/entities/telemetry/
+-rw-rw-r--   0 root         (0) root         (0)       87 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/telemetry/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      789 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/telemetry/message.py
+-rw-rw-r--   0 root         (0) root         (0)     1327 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/telemetry/position.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.182030 layrz_sdk-3.0.0/layrz_sdk/helpers/
+-rw-rw-r--   0 root         (0) root         (0)       72 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/helpers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1102 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/helpers/color.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.182030 layrz_sdk-3.0.0/layrz_sdk/lcl/
+-rw-rw-r--   0 root         (0) root         (0)       67 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/lcl/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    20608 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/lcl/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.182030 layrz_sdk-3.0.0/layrz_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1458 2024-04-26 06:22:50.000000 layrz_sdk-3.0.0/layrz_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2505 2024-04-26 06:22:50.000000 layrz_sdk-3.0.0/layrz_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 06:22:50.000000 layrz_sdk-3.0.0/layrz_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-26 06:22:50.000000 layrz_sdk-3.0.0/layrz_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-26 06:22:50.000000 layrz_sdk-3.0.0/layrz_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     7589 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 06:22:50.182030 layrz_sdk-3.0.0/setup.cfg
```

### Comparing `layrz-sdk-2.2.4/LICENSE` & `layrz_sdk-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/PKG-INFO` & `layrz_sdk-3.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: layrz-sdk
-Version: 2.2.4
+Version: 3.0.0
 Summary: Layrz SDK for Python
 Author-email: "Golden M, Inc." <software@goldenm.com>
 Maintainer-email: Kenny Mochizuki <kenny@goldenm.com>, Luis Reyes <lreyes@goldenm.com>, Kasen Li <kli@goldenm.com>
 License: MIT License
 Project-URL: Repository, https://github.com/goldenm-software/layrz-sdk
 Project-URL: Changelog, https://github.com/goldenm-software/layrz-sdk/blob/main/CHANGELOG.md
 Keywords: sdk,goldenm,lcl,layrz compute language,layrz
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: <3.12,>=3.10
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: xlsxwriter
 
 # Layrz SDK
```

### Comparing `layrz-sdk-2.2.4/README.md` & `layrz_sdk-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/__init__.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/broadcasts/request.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/request.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/broadcasts/response.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/response.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/broadcasts/result.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/result.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/broadcasts/service.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/service.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/broadcasts/status.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/status.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/cases/case.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/cases/case.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/cases/comment.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/cases/comment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Comment entity """
 from datetime import datetime
 
-from layrz.sdk.entities.general.user import User
+from layrz_sdk.entities.general.user import User
 
 
 class Comment:
   """
   Case comment entity definition
   ---
   Attributes
```

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/cases/trigger.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/cases/trigger.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/charts/__init__.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/charts/bar.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/charts/bar.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/charts/column.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/charts/column.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """ Column chart """
-from layrz.sdk.helpers import convert_to_rgba
+from layrz_sdk.helpers import convert_to_rgba
 
 from .alignment import ChartAlignment
 from .exceptions import ChartException
 from .serie import ChartDataSerie
 from .serie_type import ChartDataSerieType
```

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/charts/configuration.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/charts/configuration.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/charts/exceptions.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/charts/exceptions.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/charts/html.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/charts/html.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/charts/line.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/charts/line.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/charts/map.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/charts/map.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/charts/number.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/charts/number.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/charts/pie.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/charts/pie.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/charts/radar.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/charts/radar.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/charts/radial_bar.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/charts/radial_bar.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/charts/scatter.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/charts/scatter.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/charts/serie.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/charts/serie.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/charts/table.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/charts/table.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/charts/timeline.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/charts/timeline.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/checkpoints/checkpoint.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/checkpoints/checkpoint.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/checkpoints/geofence.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/checkpoints/geofence.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/checkpoints/waypoint.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/checkpoints/waypoint.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/events/event.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/events/event.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Event entity """
 from datetime import datetime
 
-from layrz.sdk.entities.cases.trigger import Trigger
-from layrz.sdk.entities.telemetry.message import Message
+from layrz_sdk.entities.cases.trigger import Trigger
+from layrz_sdk.entities.telemetry.message import Message
 
 
 class Event:
   """
   Event entity definition
 
   Available attributes
```

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/general/asset.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/general/asset.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/general/asset_operation_mode.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/general/asset_operation_mode.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/general/custom_field.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/general/custom_field.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/general/device.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/general/device.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/general/sensor.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/general/sensor.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/general/user.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/general/user.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/repcom/transaction.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/repcom/transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Transaction entity """
 from datetime import datetime, timedelta
 
-from layrz.sdk.entities.general.asset import Asset
+from layrz_sdk.entities.general.asset import Asset
 
 
 class Transaction:
   """
   Transaction definition
   ---
   Attributes
```

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/reports/col.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/reports/col.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/reports/header.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/reports/header.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/reports/page.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/reports/page.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/reports/report.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/reports/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Report class """
 import os
 import time
 import warnings
 
 import xlsxwriter
 
-from layrz.sdk.helpers.color import use_black
+from layrz_sdk.helpers.color import use_black
 
 from .col import ReportDataType
 from .format import ReportFormat
 from .page import CustomReportPage, ReportPage
 
 
 class Report:
```

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/reports/row.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/reports/row.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/telemetry/message.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/telemetry/message.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/entities/telemetry/position.py` & `layrz_sdk-3.0.0/layrz_sdk/entities/telemetry/position.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/helpers/color.py` & `layrz_sdk-3.0.0/layrz_sdk/helpers/color.py`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.2.4/layrz/sdk/lcl/core.py` & `layrz_sdk-3.0.0/layrz_sdk/lcl/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,15 +533,15 @@
 
     return args[1] if args[0] else args[2]
 
   def NOW(self, *args: list[Any]) -> float:  # pylint: disable=unused-argument
     """ NOW Function """
     import zoneinfo
     from datetime import datetime
-    return datetime.utcnow(tz=zoneinfo.ZoneInfo('UTC')).timestamp()
+    return datetime.now(tz=zoneinfo.ZoneInfo('UTC')).timestamp()
 
   def REGEX(self, *args: list[Any]) -> str | None | bool:
     """ REGEX Function """
     if len(args) != 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=2, received=len(args))
 
     if args[0] is None or args[1] is None:
```

### Comparing `layrz-sdk-2.2.4/layrz_sdk.egg-info/PKG-INFO` & `layrz_sdk-3.0.0/layrz_sdk.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: layrz-sdk
-Version: 2.2.4
+Version: 3.0.0
 Summary: Layrz SDK for Python
 Author-email: "Golden M, Inc." <software@goldenm.com>
 Maintainer-email: Kenny Mochizuki <kenny@goldenm.com>, Luis Reyes <lreyes@goldenm.com>, Kasen Li <kli@goldenm.com>
 License: MIT License
 Project-URL: Repository, https://github.com/goldenm-software/layrz-sdk
 Project-URL: Changelog, https://github.com/goldenm-software/layrz-sdk/blob/main/CHANGELOG.md
 Keywords: sdk,goldenm,lcl,layrz compute language,layrz
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: <3.12,>=3.10
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: xlsxwriter
 
 # Layrz SDK
```

### Comparing `layrz-sdk-2.2.4/layrz_sdk.egg-info/SOURCES.txt` & `layrz_sdk-3.0.0/layrz_sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,70 @@
 LICENSE
 README.md
 pyproject.toml
-layrz/__init__.py
-layrz/sdk/__init__.py
-layrz/sdk/entities/__init__.py
-layrz/sdk/entities/broadcasts/__init__.py
-layrz/sdk/entities/broadcasts/request.py
-layrz/sdk/entities/broadcasts/response.py
-layrz/sdk/entities/broadcasts/result.py
-layrz/sdk/entities/broadcasts/service.py
-layrz/sdk/entities/broadcasts/status.py
-layrz/sdk/entities/cases/__init__.py
-layrz/sdk/entities/cases/case.py
-layrz/sdk/entities/cases/comment.py
-layrz/sdk/entities/cases/trigger.py
-layrz/sdk/entities/charts/__init__.py
-layrz/sdk/entities/charts/alignment.py
-layrz/sdk/entities/charts/bar.py
-layrz/sdk/entities/charts/column.py
-layrz/sdk/entities/charts/configuration.py
-layrz/sdk/entities/charts/data_type.py
-layrz/sdk/entities/charts/exceptions.py
-layrz/sdk/entities/charts/html.py
-layrz/sdk/entities/charts/line.py
-layrz/sdk/entities/charts/map.py
-layrz/sdk/entities/charts/number.py
-layrz/sdk/entities/charts/pie.py
-layrz/sdk/entities/charts/radar.py
-layrz/sdk/entities/charts/radial_bar.py
-layrz/sdk/entities/charts/scatter.py
-layrz/sdk/entities/charts/serie.py
-layrz/sdk/entities/charts/serie_type.py
-layrz/sdk/entities/charts/table.py
-layrz/sdk/entities/charts/timeline.py
-layrz/sdk/entities/checkpoints/__init__.py
-layrz/sdk/entities/checkpoints/checkpoint.py
-layrz/sdk/entities/checkpoints/geofence.py
-layrz/sdk/entities/checkpoints/waypoint.py
-layrz/sdk/entities/events/__init__.py
-layrz/sdk/entities/events/event.py
-layrz/sdk/entities/formatting/__init__.py
-layrz/sdk/entities/formatting/text_align.py
-layrz/sdk/entities/general/__init__.py
-layrz/sdk/entities/general/asset.py
-layrz/sdk/entities/general/asset_operation_mode.py
-layrz/sdk/entities/general/custom_field.py
-layrz/sdk/entities/general/device.py
-layrz/sdk/entities/general/sensor.py
-layrz/sdk/entities/general/user.py
-layrz/sdk/entities/repcom/__init__.py
-layrz/sdk/entities/repcom/transaction.py
-layrz/sdk/entities/reports/__init__.py
-layrz/sdk/entities/reports/col.py
-layrz/sdk/entities/reports/format.py
-layrz/sdk/entities/reports/header.py
-layrz/sdk/entities/reports/page.py
-layrz/sdk/entities/reports/report.py
-layrz/sdk/entities/reports/row.py
-layrz/sdk/entities/telemetry/__init__.py
-layrz/sdk/entities/telemetry/message.py
-layrz/sdk/entities/telemetry/position.py
-layrz/sdk/helpers/__init__.py
-layrz/sdk/helpers/color.py
-layrz/sdk/lcl/__init__.py
-layrz/sdk/lcl/core.py
+layrz_sdk/__init__.py
 layrz_sdk.egg-info/PKG-INFO
 layrz_sdk.egg-info/SOURCES.txt
 layrz_sdk.egg-info/dependency_links.txt
 layrz_sdk.egg-info/requires.txt
-layrz_sdk.egg-info/top_level.txt
+layrz_sdk.egg-info/top_level.txt
+layrz_sdk/entities/__init__.py
+layrz_sdk/entities/broadcasts/__init__.py
+layrz_sdk/entities/broadcasts/request.py
+layrz_sdk/entities/broadcasts/response.py
+layrz_sdk/entities/broadcasts/result.py
+layrz_sdk/entities/broadcasts/service.py
+layrz_sdk/entities/broadcasts/status.py
+layrz_sdk/entities/cases/__init__.py
+layrz_sdk/entities/cases/case.py
+layrz_sdk/entities/cases/comment.py
+layrz_sdk/entities/cases/trigger.py
+layrz_sdk/entities/charts/__init__.py
+layrz_sdk/entities/charts/alignment.py
+layrz_sdk/entities/charts/bar.py
+layrz_sdk/entities/charts/column.py
+layrz_sdk/entities/charts/configuration.py
+layrz_sdk/entities/charts/data_type.py
+layrz_sdk/entities/charts/exceptions.py
+layrz_sdk/entities/charts/html.py
+layrz_sdk/entities/charts/line.py
+layrz_sdk/entities/charts/map.py
+layrz_sdk/entities/charts/number.py
+layrz_sdk/entities/charts/pie.py
+layrz_sdk/entities/charts/radar.py
+layrz_sdk/entities/charts/radial_bar.py
+layrz_sdk/entities/charts/scatter.py
+layrz_sdk/entities/charts/serie.py
+layrz_sdk/entities/charts/serie_type.py
+layrz_sdk/entities/charts/table.py
+layrz_sdk/entities/charts/timeline.py
+layrz_sdk/entities/checkpoints/__init__.py
+layrz_sdk/entities/checkpoints/checkpoint.py
+layrz_sdk/entities/checkpoints/geofence.py
+layrz_sdk/entities/checkpoints/waypoint.py
+layrz_sdk/entities/events/__init__.py
+layrz_sdk/entities/events/event.py
+layrz_sdk/entities/formatting/__init__.py
+layrz_sdk/entities/formatting/text_align.py
+layrz_sdk/entities/general/__init__.py
+layrz_sdk/entities/general/asset.py
+layrz_sdk/entities/general/asset_operation_mode.py
+layrz_sdk/entities/general/custom_field.py
+layrz_sdk/entities/general/device.py
+layrz_sdk/entities/general/sensor.py
+layrz_sdk/entities/general/user.py
+layrz_sdk/entities/repcom/__init__.py
+layrz_sdk/entities/repcom/transaction.py
+layrz_sdk/entities/reports/__init__.py
+layrz_sdk/entities/reports/col.py
+layrz_sdk/entities/reports/format.py
+layrz_sdk/entities/reports/header.py
+layrz_sdk/entities/reports/page.py
+layrz_sdk/entities/reports/report.py
+layrz_sdk/entities/reports/row.py
+layrz_sdk/entities/telemetry/__init__.py
+layrz_sdk/entities/telemetry/message.py
+layrz_sdk/entities/telemetry/position.py
+layrz_sdk/helpers/__init__.py
+layrz_sdk/helpers/color.py
+layrz_sdk/lcl/__init__.py
+layrz_sdk/lcl/core.py
```

### Comparing `layrz-sdk-2.2.4/pyproject.toml` & `layrz_sdk-3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "layrz-sdk"
-version = "2.2.4"
+version = "3.0.0"
 description = "Layrz SDK for Python"
 authors = [
   {name = "Golden M, Inc.", email = "software@goldenm.com"}
 ]
-requires-python = ">=3.10,<3.12"
+requires-python = ">=3.10"
 
 maintainers = [
   {name = "Kenny Mochizuki", email = "kenny@goldenm.com"},
   {name = "Luis Reyes", email = "lreyes@goldenm.com"},
   {name = "Kasen Li", email = "kli@goldenm.com"},
 ]
 
@@ -24,32 +24,25 @@
   "layrz compute language",
   "layrz",
 ]
 classifiers = [
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
   "requests",
   "xlsxwriter",
 ]
 
 [project.urls]
 Repository = "https://github.com/goldenm-software/layrz-sdk"
 Changelog = "https://github.com/goldenm-software/layrz-sdk/blob/main/CHANGELOG.md"
 
-[tool.setuptools.packages.find]
-where = ["."]
-include = [
-  "layrz",
-  "layrz.*",
-]
-namespaces = true
-
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [tool.yapf]
 indent_width = 2
 use_tabs = false
```

