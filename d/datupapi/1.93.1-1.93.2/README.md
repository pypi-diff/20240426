# Comparing `tmp/datupapi-1.93.1.tar.gz` & `tmp/datupapi-1.93.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datupapi-1.93.1.tar", last modified: Wed Apr 24 22:10:44 2024, max compression
+gzip compressed data, was "datupapi-1.93.2.tar", last modified: Fri Apr 26 16:49:13 2024, max compression
```

## Comparing `datupapi-1.93.1.tar` & `datupapi-1.93.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.456163 datupapi-1.93.1/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-04-24 22:10:44.456163 datupapi-1.93.1/PKG-INFO
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.439163 datupapi-1.93.1/datupapi/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.441163 datupapi-1.93.1/datupapi/configure/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/configure/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5750 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/configure/config.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.437163 datupapi-1.93.1/datupapi/distribution/
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.441163 datupapi-1.93.1/datupapi/distribution/conf/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.93.1/datupapi/distribution/conf/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.437163 datupapi-1.93.1/datupapi/distribution/src/
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.442163 datupapi-1.93.1/datupapi/distribution/src/DistributionFunctions/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.93.1/datupapi/distribution/src/DistributionFunctions/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9390 2023-12-22 18:43:58.000000 datupapi-1.93.1/datupapi/distribution/src/DistributionFunctions/functions_distribution.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.443163 datupapi-1.93.1/datupapi/evaluate/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/evaluate/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7039 2023-07-06 13:37:00.000000 datupapi-1.93.1/datupapi/evaluate/errors.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.444163 datupapi-1.93.1/datupapi/extract/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/extract/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    66939 2024-02-22 19:20:36.000000 datupapi-1.93.1/datupapi/extract/io.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9338 2023-08-28 15:15:16.000000 datupapi-1.93.1/datupapi/extract/io_citrix.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.445163 datupapi-1.93.1/datupapi/feateng/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/feateng/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7922 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/feateng/relation.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4425 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/feateng/scale.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.445163 datupapi-1.93.1/datupapi/inventory/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/inventory/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.446163 datupapi-1.93.1/datupapi/inventory/conf/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.1/datupapi/inventory/conf/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.438163 datupapi-1.93.1/datupapi/inventory/src/
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.446163 datupapi-1.93.1/datupapi/inventory/src/DailyUsage/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.1/datupapi/inventory/src/DailyUsage/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7915 2023-08-28 15:14:13.000000 datupapi-1.93.1/datupapi/inventory/src/DailyUsage/daily_usage.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.447163 datupapi-1.93.1/datupapi/inventory/src/Format/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.1/datupapi/inventory/src/Format/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5433 2024-02-26 21:37:34.000000 datupapi-1.93.1/datupapi/inventory/src/Format/inventory_format.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.447163 datupapi-1.93.1/datupapi/inventory/src/InventoryFunctions/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.1/datupapi/inventory/src/InventoryFunctions/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    10157 2024-02-26 21:37:34.000000 datupapi-1.93.1/datupapi/inventory/src/InventoryFunctions/functions_inventory.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.448163 datupapi-1.93.1/datupapi/inventory/src/ProcessForecast/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.1/datupapi/inventory/src/ProcessForecast/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    10560 2023-08-28 15:14:13.000000 datupapi-1.93.1/datupapi/inventory/src/ProcessForecast/define_periods.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7391 2023-08-28 15:14:13.000000 datupapi-1.93.1/datupapi/inventory/src/ProcessForecast/extract_forecast.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.449163 datupapi-1.93.1/datupapi/inventory/src/SuggestedForecast/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.1/datupapi/inventory/src/SuggestedForecast/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    14066 2023-08-28 15:14:13.000000 datupapi-1.93.1/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.449163 datupapi-1.93.1/datupapi/inventory/src/Transformation/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.1/datupapi/inventory/src/Transformation/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1219 2023-08-28 15:14:13.000000 datupapi-1.93.1/datupapi/inventory/src/Transformation/inventory_transformation.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    80578 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/inventory/stocks.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.450163 datupapi-1.93.1/datupapi/predict/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/predict/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    27677 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/predict/forecast.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.451163 datupapi-1.93.1/datupapi/prepare/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/prepare/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1922 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/prepare/cleanse.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    20602 2023-10-25 22:17:02.000000 datupapi-1.93.1/datupapi/prepare/format.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4800 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/prepare/format_dask.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.453163 datupapi-1.93.1/datupapi/training/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/training/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    25158 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/training/attup.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    31654 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/training/deepar.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    22222 2024-04-24 22:09:00.000000 datupapi-1.93.1/datupapi/training/tft.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.454163 datupapi-1.93.1/datupapi/transform/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/transform/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    18233 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/transform/backtesting.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    52714 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/transform/forecasting.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7943 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/transform/ranking.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.455163 datupapi-1.93.1/datupapi/utils/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/utils/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4637 2023-06-26 23:14:24.000000 datupapi-1.93.1/datupapi/utils/utils.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 22:10:44.455163 datupapi-1.93.1/datupapi.egg-info/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-04-24 22:10:44.000000 datupapi-1.93.1/datupapi.egg-info/PKG-INFO
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1925 2024-04-24 22:10:44.000000 datupapi-1.93.1/datupapi.egg-info/SOURCES.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        1 2024-04-24 22:10:44.000000 datupapi-1.93.1/datupapi.egg-info/dependency_links.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)      539 2024-04-24 22:10:44.000000 datupapi-1.93.1/datupapi.egg-info/requires.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        9 2024-04-24 22:10:44.000000 datupapi-1.93.1/datupapi.egg-info/top_level.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)       87 2023-12-19 15:43:19.000000 datupapi-1.93.1/pyproject.toml
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)       38 2024-04-24 22:10:44.456163 datupapi-1.93.1/setup.cfg
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     2129 2024-04-24 22:09:20.000000 datupapi-1.93.1/setup.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.792054 datupapi-1.93.2/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-04-26 16:49:13.791054 datupapi-1.93.2/PKG-INFO
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.776054 datupapi-1.93.2/datupapi/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.777054 datupapi-1.93.2/datupapi/configure/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/configure/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5750 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/configure/config.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.774054 datupapi-1.93.2/datupapi/distribution/
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.778054 datupapi-1.93.2/datupapi/distribution/conf/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.93.2/datupapi/distribution/conf/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.774054 datupapi-1.93.2/datupapi/distribution/src/
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.778054 datupapi-1.93.2/datupapi/distribution/src/DistributionFunctions/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.93.2/datupapi/distribution/src/DistributionFunctions/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9390 2023-12-22 18:43:58.000000 datupapi-1.93.2/datupapi/distribution/src/DistributionFunctions/functions_distribution.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.778054 datupapi-1.93.2/datupapi/evaluate/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/evaluate/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7039 2023-07-06 13:37:00.000000 datupapi-1.93.2/datupapi/evaluate/errors.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.779054 datupapi-1.93.2/datupapi/extract/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/extract/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    66939 2024-02-22 19:20:36.000000 datupapi-1.93.2/datupapi/extract/io.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9338 2023-08-28 15:15:16.000000 datupapi-1.93.2/datupapi/extract/io_citrix.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.780054 datupapi-1.93.2/datupapi/feateng/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/feateng/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7922 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/feateng/relation.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4425 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/feateng/scale.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.781054 datupapi-1.93.2/datupapi/inventory/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/inventory/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.782054 datupapi-1.93.2/datupapi/inventory/conf/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/conf/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.775054 datupapi-1.93.2/datupapi/inventory/src/
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.782054 datupapi-1.93.2/datupapi/inventory/src/DailyUsage/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/DailyUsage/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7915 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/DailyUsage/daily_usage.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.782054 datupapi-1.93.2/datupapi/inventory/src/Format/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/Format/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5433 2024-02-26 21:37:34.000000 datupapi-1.93.2/datupapi/inventory/src/Format/inventory_format.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.783054 datupapi-1.93.2/datupapi/inventory/src/InventoryFunctions/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/InventoryFunctions/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    10157 2024-02-26 21:37:34.000000 datupapi-1.93.2/datupapi/inventory/src/InventoryFunctions/functions_inventory.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.784054 datupapi-1.93.2/datupapi/inventory/src/ProcessForecast/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/ProcessForecast/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    10560 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/ProcessForecast/define_periods.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7391 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/ProcessForecast/extract_forecast.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.785054 datupapi-1.93.2/datupapi/inventory/src/SuggestedForecast/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/SuggestedForecast/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    14066 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.785054 datupapi-1.93.2/datupapi/inventory/src/Transformation/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/Transformation/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1219 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/Transformation/inventory_transformation.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    80578 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/inventory/stocks.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.786054 datupapi-1.93.2/datupapi/predict/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/predict/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    27677 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/predict/forecast.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.787054 datupapi-1.93.2/datupapi/prepare/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/prepare/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1922 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/prepare/cleanse.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    20602 2023-10-25 22:17:02.000000 datupapi-1.93.2/datupapi/prepare/format.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4800 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/prepare/format_dask.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.789054 datupapi-1.93.2/datupapi/training/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/training/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    25158 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/training/attup.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    31654 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/training/deepar.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    22291 2024-04-26 16:48:36.000000 datupapi-1.93.2/datupapi/training/tft.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.790054 datupapi-1.93.2/datupapi/transform/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/transform/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    18233 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/transform/backtesting.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    52714 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/transform/forecasting.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7943 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/transform/ranking.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.790054 datupapi-1.93.2/datupapi/utils/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/utils/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4637 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/utils/utils.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.791054 datupapi-1.93.2/datupapi.egg-info/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-04-26 16:49:13.000000 datupapi-1.93.2/datupapi.egg-info/PKG-INFO
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1925 2024-04-26 16:49:13.000000 datupapi-1.93.2/datupapi.egg-info/SOURCES.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        1 2024-04-26 16:49:13.000000 datupapi-1.93.2/datupapi.egg-info/dependency_links.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)      539 2024-04-26 16:49:13.000000 datupapi-1.93.2/datupapi.egg-info/requires.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        9 2024-04-26 16:49:13.000000 datupapi-1.93.2/datupapi.egg-info/top_level.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)       87 2023-12-19 15:43:19.000000 datupapi-1.93.2/pyproject.toml
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)       38 2024-04-26 16:49:13.792054 datupapi-1.93.2/setup.cfg
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     2129 2024-04-26 16:48:48.000000 datupapi-1.93.2/setup.py
```

### Comparing `datupapi-1.93.1/PKG-INFO` & `datupapi-1.93.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datupapi
-Version: 1.93.1
+Version: 1.93.2
 Summary: Utility library to support Datup AI MLOps processes
 Author: Datup AI
 Author-email: ramiro@datup.ai
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4>=4.9.3
 Requires-Dist: boto3>=1.16.54
 Requires-Dist: catboost>=1.0.4
```

### Comparing `datupapi-1.93.1/datupapi/configure/config.py` & `datupapi-1.93.2/datupapi/configure/config.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/distribution/src/DistributionFunctions/functions_distribution.py` & `datupapi-1.93.2/datupapi/distribution/src/DistributionFunctions/functions_distribution.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/evaluate/errors.py` & `datupapi-1.93.2/datupapi/evaluate/errors.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/extract/io.py` & `datupapi-1.93.2/datupapi/extract/io.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/extract/io_citrix.py` & `datupapi-1.93.2/datupapi/extract/io_citrix.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/feateng/relation.py` & `datupapi-1.93.2/datupapi/feateng/relation.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/feateng/scale.py` & `datupapi-1.93.2/datupapi/feateng/scale.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/inventory/src/DailyUsage/daily_usage.py` & `datupapi-1.93.2/datupapi/inventory/src/DailyUsage/daily_usage.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/inventory/src/Format/inventory_format.py` & `datupapi-1.93.2/datupapi/inventory/src/Format/inventory_format.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/inventory/src/InventoryFunctions/functions_inventory.py` & `datupapi-1.93.2/datupapi/inventory/src/InventoryFunctions/functions_inventory.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/inventory/src/ProcessForecast/define_periods.py` & `datupapi-1.93.2/datupapi/inventory/src/ProcessForecast/define_periods.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/inventory/src/ProcessForecast/extract_forecast.py` & `datupapi-1.93.2/datupapi/inventory/src/ProcessForecast/extract_forecast.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py` & `datupapi-1.93.2/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/inventory/src/Transformation/inventory_transformation.py` & `datupapi-1.93.2/datupapi/inventory/src/Transformation/inventory_transformation.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/inventory/stocks.py` & `datupapi-1.93.2/datupapi/inventory/stocks.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/predict/forecast.py` & `datupapi-1.93.2/datupapi/predict/forecast.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/prepare/cleanse.py` & `datupapi-1.93.2/datupapi/prepare/cleanse.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/prepare/format.py` & `datupapi-1.93.2/datupapi/prepare/format.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/prepare/format_dask.py` & `datupapi-1.93.2/datupapi/prepare/format_dask.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/training/attup.py` & `datupapi-1.93.2/datupapi/training/attup.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/training/deepar.py` & `datupapi-1.93.2/datupapi/training/deepar.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/training/tft.py` & `datupapi-1.93.2/datupapi/training/tft.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,16 @@
         print("string")
         for key in scalers.keys():
             aux = pd.DataFrame()
             scaler = scalers[key]
             l_columns = ["p5", "p20", "p40", "p50", "p60", "p80", "p95", "demand"
                         ] if backtest != 0 else ["p5", "p20", "p40", "p50", "p60", "p80", "p95"]
             aux = pd.DataFrame(scaler.inverse_transform(p0[p0.item_id == key.replace("scaler_", "")][l_columns]), columns=l_columns)
-            p1 = p1.append(aux, ignore_index=True)
+            #p1 = p1.append(aux, ignore_index=True)
+            p1 = pd.concat([p1,aux], ignore_index=True) #ADDED IVAN
         p1["item_id"] = p0.apply(lambda row: row["item_id"].split("*-+")[0], axis=1) if self.use_location else p0["item_id"]
         p1["time_idx"] = p0["time_idx"]
         if self.use_location:
             p1["location"] = p0["location"]
         return p1
 
     def transform_to_matrix(self, df, value=None, method=None, freq='M'):
```

### Comparing `datupapi-1.93.1/datupapi/transform/backtesting.py` & `datupapi-1.93.2/datupapi/transform/backtesting.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/transform/forecasting.py` & `datupapi-1.93.2/datupapi/transform/forecasting.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/transform/ranking.py` & `datupapi-1.93.2/datupapi/transform/ranking.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi/utils/utils.py` & `datupapi-1.93.2/datupapi/utils/utils.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi.egg-info/PKG-INFO` & `datupapi-1.93.2/datupapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datupapi
-Version: 1.93.1
+Version: 1.93.2
 Summary: Utility library to support Datup AI MLOps processes
 Author: Datup AI
 Author-email: ramiro@datup.ai
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4>=4.9.3
 Requires-Dist: boto3>=1.16.54
 Requires-Dist: catboost>=1.0.4
```

### Comparing `datupapi-1.93.1/datupapi.egg-info/SOURCES.txt` & `datupapi-1.93.2/datupapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/datupapi.egg-info/requires.txt` & `datupapi-1.93.2/datupapi.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.1/setup.py` & `datupapi-1.93.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='datupapi',
-      version='1.93.1',
+      version='1.93.2',
       description='Utility library to support Datup AI MLOps processes',
       long_description_content_type="text/markdown",
       long_description="foo bar baz",
       author='Datup AI',
       author_email='ramiro@datup.ai',
       packages=[
           'datupapi',
```

