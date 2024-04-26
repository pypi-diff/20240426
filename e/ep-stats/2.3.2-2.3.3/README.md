# Comparing `tmp/ep-stats-2.3.2.tar.gz` & `tmp/ep-stats-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ep-stats-2.3.2.tar", last modified: Wed Apr 24 12:57:27 2024, max compression
+gzip compressed data, was "ep-stats-2.3.3.tar", last modified: Fri Apr 26 09:03:20 2024, max compression
```

## Comparing `ep-stats-2.3.2.tar` & `ep-stats-2.3.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:27.017111 ep-stats-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 12:57:04.000000 ep-stats-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-24 12:57:27.021111 ep-stats-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-24 12:57:04.000000 ep-stats-2.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-24 12:57:04.000000 ep-stats-2.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-24 12:57:27.021111 ep-stats-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-24 12:57:04.000000 ep-stats-2.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:27.013111 ep-stats-2.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:27.013111 ep-stats-2.3.2/src/ep_stats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-24 12:57:26.000000 ep-stats-2.3.2/src/ep_stats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-24 12:57:26.000000 ep-stats-2.3.2/src/ep_stats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:57:26.000000 ep-stats-2.3.2/src/ep_stats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 12:57:26.000000 ep-stats-2.3.2/src/ep_stats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-24 12:57:26.000000 ep-stats-2.3.2/src/ep_stats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 12:57:26.000000 ep-stats-2.3.2/src/ep_stats.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:27.017111 ep-stats-2.3.2/src/epstats/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/locust.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:27.017111 ep-stats-2.3.2/src/epstats/server/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/server/api_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/server/api_sample_size_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/server/api_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/server/json_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15127 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/server/req.py
--rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/server/res.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:27.017111 ep-stats-2.3.2/src/epstats/toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/dao.py
--rw-r--r--   0 runner    (1001) docker     (127)    32779 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    17549 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:27.017111 ep-stats-2.3.2/src/epstats/toolkit/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:27.017111 ep-stats-2.3.2/src/epstats/toolkit/testing/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/resources/evaluations_checks.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/resources/evaluations_exposures.csv
--rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/resources/evaluations_metrics.csv
--rw-r--r--   0 runner    (1001) docker     (127)    14946 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/resources/goals_agg.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/resources/goals_by_unit.csv
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/resources/goals_simple_agg.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/test_dao.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:03:20.954699 ep-stats-2.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-26 09:03:09.000000 ep-stats-2.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-26 09:03:20.954699 ep-stats-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-26 09:03:09.000000 ep-stats-2.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-26 09:03:09.000000 ep-stats-2.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-26 09:03:20.954699 ep-stats-2.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-26 09:03:09.000000 ep-stats-2.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:03:20.946699 ep-stats-2.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:03:20.950699 ep-stats-2.3.3/src/ep_stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-26 09:03:20.000000 ep-stats-2.3.3/src/ep_stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-26 09:03:20.000000 ep-stats-2.3.3/src/ep_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:03:20.000000 ep-stats-2.3.3/src/ep_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 09:03:20.000000 ep-stats-2.3.3/src/ep_stats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-26 09:03:20.000000 ep-stats-2.3.3/src/ep_stats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 09:03:20.000000 ep-stats-2.3.3/src/ep_stats.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:03:20.950699 ep-stats-2.3.3/src/epstats/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/locust.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:03:20.950699 ep-stats-2.3.3/src/epstats/server/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/server/api_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/server/api_sample_size_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/server/api_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/server/json_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15127 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/server/req.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/server/res.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:03:20.954699 ep-stats-2.3.3/src/epstats/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32779 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17549 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:03:20.954699 ep-stats-2.3.3/src/epstats/toolkit/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:03:20.954699 ep-stats-2.3.3/src/epstats/toolkit/testing/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/testing/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/testing/resources/evaluations_checks.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/testing/resources/evaluations_exposures.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/testing/resources/evaluations_metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    14946 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/testing/resources/goals_agg.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/testing/resources/goals_by_unit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/testing/resources/goals_simple_agg.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/testing/test_dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/testing/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/testing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-26 09:03:09.000000 ep-stats-2.3.3/src/epstats/toolkit/utils.py
```

### Comparing `ep-stats-2.3.2/LICENSE` & `ep-stats-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/PKG-INFO` & `ep-stats-2.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ep-stats
-Version: 2.3.2
+Version: 2.3.3
 Summary: Statistical package to evaluate ab tests in experimentation platform.
 Home-page: https://github.com/avast/ep-stats
 Author: Ondrej Zahradnik
 Author-email: ondrej.zahradnik@avast.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ep-stats-2.3.2/README.md` & `ep-stats-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/setup.cfg` & `ep-stats-2.3.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ep-stats
-version = 2.3.2
+version = 2.3.3
 description = Statistical package to evaluate ab tests in experimentation platform.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Ondrej Zahradnik
 author_email = ondrej.zahradnik@avast.com
 url = https://github.com/avast/ep-stats
 classifiers =
```

### Comparing `ep-stats-2.3.2/src/ep_stats.egg-info/PKG-INFO` & `ep-stats-2.3.3/src/ep_stats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ep-stats
-Version: 2.3.2
+Version: 2.3.3
 Summary: Statistical package to evaluate ab tests in experimentation platform.
 Home-page: https://github.com/avast/ep-stats
 Author: Ondrej Zahradnik
 Author-email: ondrej.zahradnik@avast.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ep-stats-2.3.2/src/ep_stats.egg-info/SOURCES.txt` & `ep-stats-2.3.3/src/ep_stats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/config.py` & `ep-stats-2.3.3/src/epstats/config.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/locust.py` & `ep-stats-2.3.3/src/epstats/locust.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/main.py` & `ep-stats-2.3.3/src/epstats/main.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/prometheus.py` & `ep-stats-2.3.3/src/epstats/prometheus.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/server/api.py` & `ep-stats-2.3.3/src/epstats/server/api.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/server/api_evaluate.py` & `ep-stats-2.3.3/src/epstats/server/api_evaluate.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/server/api_sample_size_calculation.py` & `ep-stats-2.3.3/src/epstats/server/api_sample_size_calculation.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/server/req.py` & `ep-stats-2.3.3/src/epstats/server/req.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/server/res.py` & `ep-stats-2.3.3/src/epstats/server/res.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/toolkit/check.py` & `ep-stats-2.3.3/src/epstats/toolkit/check.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
             "count(test_unit_type.global.exposure)"
         )
         ```
         """
         super().__init__(id, name, denominator)
         self.max_sum_ratio = max_sum_ratio
         self.confidence_level = confidence_level
-        self._nominator = nominator
+        self.nominator = nominator
         self._nominator_parser = Parser(nominator, nominator)
         self._goals = self._goals.union(self._nominator_parser.get_goals())
 
     def evaluate_agg(self, goals: pd.DataFrame, default_exp_variant_id: str) -> pd.DataFrame:
         """
         See [`Check.evaluate_agg`][epstats.toolkit.check.Check.evaluate_agg].
         """
```

### Comparing `ep-stats-2.3.2/src/epstats/toolkit/dao.py` & `ep-stats-2.3.3/src/epstats/toolkit/dao.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/toolkit/experiment.py` & `ep-stats-2.3.3/src/epstats/toolkit/experiment.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/toolkit/metric.py` & `ep-stats-2.3.3/src/epstats/toolkit/metric.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/toolkit/parser.py` & `ep-stats-2.3.3/src/epstats/toolkit/parser.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/toolkit/results.py` & `ep-stats-2.3.3/src/epstats/toolkit/results.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/toolkit/statistics.py` & `ep-stats-2.3.3/src/epstats/toolkit/statistics.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/toolkit/testing/resources/evaluations_checks.csv` & `ep-stats-2.3.3/src/epstats/toolkit/testing/resources/evaluations_checks.csv`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/toolkit/testing/resources/evaluations_exposures.csv` & `ep-stats-2.3.3/src/epstats/toolkit/testing/resources/evaluations_exposures.csv`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/toolkit/testing/resources/evaluations_metrics.csv` & `ep-stats-2.3.3/src/epstats/toolkit/testing/resources/evaluations_metrics.csv`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/toolkit/testing/resources/goals_agg.csv` & `ep-stats-2.3.3/src/epstats/toolkit/testing/resources/goals_agg.csv`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/toolkit/testing/resources/goals_by_unit.csv` & `ep-stats-2.3.3/src/epstats/toolkit/testing/resources/goals_by_unit.csv`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/toolkit/testing/test_dao.py` & `ep-stats-2.3.3/src/epstats/toolkit/testing/test_dao.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/toolkit/testing/test_data.py` & `ep-stats-2.3.3/src/epstats/toolkit/testing/test_data.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/toolkit/testing/utils.py` & `ep-stats-2.3.3/src/epstats/toolkit/testing/utils.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.2/src/epstats/toolkit/utils.py` & `ep-stats-2.3.3/src/epstats/toolkit/utils.py`

 * *Files identical despite different names*

