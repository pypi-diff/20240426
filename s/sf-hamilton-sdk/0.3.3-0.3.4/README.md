# Comparing `tmp/sf_hamilton_sdk-0.3.3.tar.gz` & `tmp/sf_hamilton_sdk-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sf_hamilton_sdk-0.3.3.tar", last modified: Thu Apr 25 06:34:58 2024, max compression
+gzip compressed data, was "sf_hamilton_sdk-0.3.4.tar", last modified: Thu Apr 25 22:55:58 2024, max compression
```

## Comparing `sf_hamilton_sdk-0.3.3.tar` & `sf_hamilton_sdk-0.3.4.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.134060 sf_hamilton_sdk-0.3.3/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3529 2024-04-25 06:34:58.133170 sf_hamilton_sdk-0.3.3/PKG-INFO
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2130 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/README.md
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1916 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/pyproject.toml
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       18 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/requirements-test.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      140 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/requirements.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       38 2024-04-25 06:34:58.134242 sf_hamilton_sdk-0.3.3/setup.cfg
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      115 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/setup.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.069525 sf_hamilton_sdk-0.3.3/src/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.075127 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       24 2024-04-25 06:33:40.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)    24683 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/adapters.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.077949 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/api/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/api/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)    30765 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/api/clients.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       85 2024-04-24 23:04:38.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/api/constants.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      243 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/api/projecttypes.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.080062 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      960 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/cli.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5453 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/initialize.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.080964 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.085893 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/common/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      123 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/common/.env.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      307 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/common/README.md.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       51 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/common/requirements.txt.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2702 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/common/run.py.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      697 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/common/run.sh.jinja2
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.086801 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.089658 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      352 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      520 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/components/common.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2529 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/components/data_loader.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.090345 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/config/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       26 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/config/config.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.092819 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      232 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/data/order_details.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      480 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/data/orders_new.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      309 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/data/orders_old.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      678 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.093677 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.095066 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1577 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/components/transforms.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.096552 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      157 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/data/signups.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      149 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/data/spend.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      674 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.097563 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.101936 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      469 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3738 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/feature_transforms.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      600 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/iris_loader.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2532 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/model_fitting.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1403 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/models.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      477 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.102751 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.108416 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1450 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      370 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/data_loader.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      711 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      932 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      745 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.109160 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)   991302 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/train_sample.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      679 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/template_data.json
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)    31210 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/driver.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.124149 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2401 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/dataframe_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4908 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/example_tracking.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1037 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/numpy_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5440 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/pandas_col_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4833 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/pandas_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6277 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/polars_col_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4683 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/polars_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8470 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/runs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      638 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/sql_utils.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6235 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1428 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/trackingtypes.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1980 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/utils.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.131130 sf_hamilton_sdk-0.3.3/src/sf_hamilton_sdk.egg-info/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3529 2024-04-25 06:34:58.000000 sf_hamilton_sdk-0.3.3/src/sf_hamilton_sdk.egg-info/PKG-INFO
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3700 2024-04-25 06:34:58.000000 sf_hamilton_sdk-0.3.3/src/sf_hamilton_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        1 2024-04-25 06:34:58.000000 sf_hamilton_sdk-0.3.3/src/sf_hamilton_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       58 2024-04-25 06:34:58.000000 sf_hamilton_sdk-0.3.3/src/sf_hamilton_sdk.egg-info/entry_points.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      109 2024-04-25 06:34:58.000000 sf_hamilton_sdk-0.3.3/src/sf_hamilton_sdk.egg-info/requires.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       13 2024-04-25 06:34:58.000000 sf_hamilton_sdk-0.3.3/src/sf_hamilton_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.130377 sf_hamilton_sdk-0.3.3/tests/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5387 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/tests/test_adapters.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3535 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/tests/test_driver.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9605 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/tests/test_tracking.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.454638 sf_hamilton_sdk-0.3.4/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3535 2024-04-25 22:55:58.454067 sf_hamilton_sdk-0.3.4/PKG-INFO
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2136 2024-04-25 22:55:11.000000 sf_hamilton_sdk-0.3.4/README.md
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1916 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/pyproject.toml
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       18 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/requirements-test.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      140 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/requirements.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       38 2024-04-25 22:55:58.454812 sf_hamilton_sdk-0.3.4/setup.cfg
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      115 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/setup.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.415105 sf_hamilton_sdk-0.3.4/src/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.419609 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       24 2024-04-25 22:55:11.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)    24683 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/adapters.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.422670 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/api/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/api/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)    30765 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/api/clients.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       85 2024-04-24 23:04:38.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/api/constants.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      243 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/api/projecttypes.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.423885 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      960 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/cli.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5453 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/initialize.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.424373 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.426721 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/common/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      123 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/common/.env.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      307 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/common/README.md.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       51 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/common/requirements.txt.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2702 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/common/run.py.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      697 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/common/run.sh.jinja2
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.427185 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/data_processing/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.429041 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/data_processing/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/data_processing/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      352 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/data_processing/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      520 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/data_processing/components/common.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2529 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/data_processing/components/data_loader.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.429615 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/data_processing/config/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       26 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/data_processing/config/config.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.431081 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/data_processing/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      232 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/data_processing/data/order_details.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      480 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/data_processing/data/orders_new.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      309 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/data_processing/data/orders_old.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      678 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/data_processing/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.431525 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/hello_world/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.432371 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/hello_world/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/hello_world/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1577 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/hello_world/components/transforms.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.433309 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/hello_world/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      157 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/hello_world/data/signups.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      149 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/hello_world/data/spend.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      674 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/hello_world/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.433725 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/machine_learning/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.436523 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/machine_learning/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/machine_learning/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      469 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/machine_learning/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3738 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/machine_learning/components/feature_transforms.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      600 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/machine_learning/components/iris_loader.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2532 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/machine_learning/components/model_fitting.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1403 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/machine_learning/components/models.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      477 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/machine_learning/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.436903 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/time_series_feature_engineering/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.439860 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1450 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      370 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/data_loader.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      711 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      932 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      745 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.440294 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)   991302 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/train_sample.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      679 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/time_series_feature_engineering/template_data.json
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)    31210 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/driver.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.448796 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2401 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/dataframe_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4908 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/example_tracking.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1037 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/numpy_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5440 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/pandas_col_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4833 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/pandas_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6277 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/polars_col_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4683 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/polars_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8470 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/runs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      638 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/sql_utils.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6235 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1428 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/trackingtypes.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2212 2024-04-25 22:55:11.000000 sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/utils.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.452954 sf_hamilton_sdk-0.3.4/src/sf_hamilton_sdk.egg-info/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3535 2024-04-25 22:55:58.000000 sf_hamilton_sdk-0.3.4/src/sf_hamilton_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3700 2024-04-25 22:55:58.000000 sf_hamilton_sdk-0.3.4/src/sf_hamilton_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        1 2024-04-25 22:55:58.000000 sf_hamilton_sdk-0.3.4/src/sf_hamilton_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       58 2024-04-25 22:55:58.000000 sf_hamilton_sdk-0.3.4/src/sf_hamilton_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      109 2024-04-25 22:55:58.000000 sf_hamilton_sdk-0.3.4/src/sf_hamilton_sdk.egg-info/requires.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       13 2024-04-25 22:55:58.000000 sf_hamilton_sdk-0.3.4/src/sf_hamilton_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 22:55:58.452258 sf_hamilton_sdk-0.3.4/tests/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5387 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/tests/test_adapters.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3535 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/tests/test_driver.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9605 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.4/tests/test_tracking.py
```

### Comparing `sf_hamilton_sdk-0.3.3/PKG-INFO` & `sf_hamilton_sdk-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sf-hamilton-sdk
-Version: 0.3.3
+Version: 0.3.4
 Summary: Hamilton SDK for reading and writing to the Hamilton backend APIs that support the UI.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://github.com/dagworks-inc/hamilton/
 Project-URL: Bug Reports, https://github.com/dagworks-inc/hamilton/issues
 Project-URL: Source, https://github.com/dagworks-inc/hamilton/ui/sdk
 Project-URL: Documenation, https://hamilton.dagworks.io/
 Keywords: hamilton,dagworks,observability
@@ -50,15 +50,15 @@
 ## Using the HamiltonTracker
 
 First, you'll need to install the Hamilton SDK package. Assuming you're using pip, you
 can do this with:
 
 ```bash
 # install the package & cli into your favorite python environment.
-pip install hamilton-sdk
+pip install "sf-hamilton[sdk]"
 
 # And validate -- this should not error.
 python -c "from hamilton_sdk import adapters"
 ```
 
 Next, you'll need to modify your Hamilton driver. You'll only need to use one line of code to
 replace your driver with ours:
```

### Comparing `sf_hamilton_sdk-0.3.3/README.md` & `sf_hamilton_sdk-0.3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ## Using the HamiltonTracker
 
 First, you'll need to install the Hamilton SDK package. Assuming you're using pip, you
 can do this with:
 
 ```bash
 # install the package & cli into your favorite python environment.
-pip install hamilton-sdk
+pip install "sf-hamilton[sdk]"
 
 # And validate -- this should not error.
 python -c "from hamilton_sdk import adapters"
 ```
 
 Next, you'll need to modify your Hamilton driver. You'll only need to use one line of code to
 replace your driver with ours:
```

### Comparing `sf_hamilton_sdk-0.3.3/pyproject.toml` & `sf_hamilton_sdk-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/adapters.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/adapters.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/api/clients.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/api/clients.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/cli.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/cli.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/initialize.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/initialize.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/common/run.py.jinja2` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/common/run.py.jinja2`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/common/run.sh.jinja2` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/common/run.sh.jinja2`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/components/common.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/data_processing/components/common.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/components/data_loader.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/data_processing/components/data_loader.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/template_data.json` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/data_processing/template_data.json`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/components/transforms.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/hello_world/components/transforms.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/template_data.json` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/hello_world/template_data.json`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/feature_transforms.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/machine_learning/components/feature_transforms.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/iris_loader.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/machine_learning/components/iris_loader.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/model_fitting.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/machine_learning/components/model_fitting.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/models.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/machine_learning/components/models.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/_run.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/_run.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/train_sample.csv` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/train_sample.csv`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/template_data.json` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/cli/templates/time_series_feature_engineering/template_data.json`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/driver.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/driver.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/dataframe_stats.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/dataframe_stats.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/example_tracking.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/example_tracking.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/numpy_stats.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/numpy_stats.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/pandas_col_stats.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/pandas_col_stats.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/pandas_stats.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/pandas_stats.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/polars_col_stats.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/polars_col_stats.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/polars_stats.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/polars_stats.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/runs.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/runs.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/sql_utils.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/sql_utils.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/stats.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/stats.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/trackingtypes.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/trackingtypes.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/utils.py` & `sf_hamilton_sdk-0.3.4/src/hamilton_sdk/tracking/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,10 +45,14 @@
     elif isinstance(item, Enum):
         return item.value  # Convert enum to its corresponding value
     elif hasattr(item, "to_dict"):
         return make_json_safe(item.to_dict())
     else:
         try:
             json.dumps(item)  # Check if item is json serializable
+            if isinstance(item, str):
+                # escape null byte -- postgres doesn't like null bytes at least.
+                # we might need to escape more things; TBD.
+                return item.replace("\x00", "\\x00")
             return item
         except TypeError:
             return str(item)  # Convert item to string if not json serializable
```

### Comparing `sf_hamilton_sdk-0.3.3/src/sf_hamilton_sdk.egg-info/PKG-INFO` & `sf_hamilton_sdk-0.3.4/src/sf_hamilton_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sf-hamilton-sdk
-Version: 0.3.3
+Version: 0.3.4
 Summary: Hamilton SDK for reading and writing to the Hamilton backend APIs that support the UI.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://github.com/dagworks-inc/hamilton/
 Project-URL: Bug Reports, https://github.com/dagworks-inc/hamilton/issues
 Project-URL: Source, https://github.com/dagworks-inc/hamilton/ui/sdk
 Project-URL: Documenation, https://hamilton.dagworks.io/
 Keywords: hamilton,dagworks,observability
@@ -50,15 +50,15 @@
 ## Using the HamiltonTracker
 
 First, you'll need to install the Hamilton SDK package. Assuming you're using pip, you
 can do this with:
 
 ```bash
 # install the package & cli into your favorite python environment.
-pip install hamilton-sdk
+pip install "sf-hamilton[sdk]"
 
 # And validate -- this should not error.
 python -c "from hamilton_sdk import adapters"
 ```
 
 Next, you'll need to modify your Hamilton driver. You'll only need to use one line of code to
 replace your driver with ours:
```

### Comparing `sf_hamilton_sdk-0.3.3/src/sf_hamilton_sdk.egg-info/SOURCES.txt` & `sf_hamilton_sdk-0.3.4/src/sf_hamilton_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/tests/test_adapters.py` & `sf_hamilton_sdk-0.3.4/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/tests/test_driver.py` & `sf_hamilton_sdk-0.3.4/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.3/tests/test_tracking.py` & `sf_hamilton_sdk-0.3.4/tests/test_tracking.py`

 * *Files identical despite different names*

