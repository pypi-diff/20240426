# Comparing `tmp/BicycleParameters-1.0.0.tar.gz` & `tmp/bicycleparameters-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BicycleParameters-1.0.0.tar", last modified: Sun Aug 27 08:32:13 2017, max compression
+gzip compressed data, was "bicycleparameters-1.1.0.tar", last modified: Fri Apr 26 12:12:21 2024, max compression
```

## Comparing `BicycleParameters-1.0.0.tar` & `bicycleparameters-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,95 @@
-drwxr-xr-x   0 moorepants  (1000) moorepants  (1000)        0 2017-08-27 08:32:13.000000 BicycleParameters-1.0.0/
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)     1532 2017-05-19 04:40:25.000000 BicycleParameters-1.0.0/LICENSE.txt
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)     4238 2017-05-19 04:40:25.000000 BicycleParameters-1.0.0/README.rst
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      553 2016-07-25 23:51:59.000000 BicycleParameters-1.0.0/TODO.rst
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      508 2016-07-25 23:51:59.000000 BicycleParameters-1.0.0/RELEASE.rst
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)       38 2017-08-27 08:32:13.000000 BicycleParameters-1.0.0/setup.cfg
-drwxr-xr-x   0 moorepants  (1000) moorepants  (1000)        0 2017-08-27 08:32:13.000000 BicycleParameters-1.0.0/docs/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1515 2016-07-25 23:51:59.000000 BicycleParameters-1.0.0/docs/bicycleparameters.rst
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      698 2016-07-25 23:51:59.000000 BicycleParameters-1.0.0/docs/index.rst
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      222 2016-07-25 23:51:59.000000 BicycleParameters-1.0.0/docs/bicycleparameters.test.rst
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     4634 2016-07-25 23:51:59.000000 BicycleParameters-1.0.0/docs/description.rst
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)     1512 2017-05-19 04:40:25.000000 BicycleParameters-1.0.0/docs/installation.rst
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    20094 2016-07-25 23:51:59.000000 BicycleParameters-1.0.0/docs/examples.rst
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    13141 2016-07-25 23:51:59.000000 BicycleParameters-1.0.0/docs/data.rst
-drwxr-xr-x   0 moorepants  (1000) moorepants  (1000)        0 2017-08-27 08:32:13.000000 BicycleParameters-1.0.0/BicycleParameters.egg-info/
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)     6287 2017-08-27 08:32:12.000000 BicycleParameters-1.0.0/BicycleParameters.egg-info/PKG-INFO
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)      127 2017-08-27 08:32:12.000000 BicycleParameters-1.0.0/BicycleParameters.egg-info/requires.txt
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)      871 2017-08-27 08:32:12.000000 BicycleParameters-1.0.0/BicycleParameters.egg-info/SOURCES.txt
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)       18 2017-08-27 08:32:12.000000 BicycleParameters-1.0.0/BicycleParameters.egg-info/top_level.txt
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)        1 2017-08-27 08:32:12.000000 BicycleParameters-1.0.0/BicycleParameters.egg-info/dependency_links.txt
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)     6287 2017-08-27 08:32:13.000000 BicycleParameters-1.0.0/PKG-INFO
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       58 2016-07-25 23:51:59.000000 BicycleParameters-1.0.0/MANIFEST.in
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)     1493 2017-05-19 04:40:25.000000 BicycleParameters-1.0.0/setup.py
-drwxr-xr-x   0 moorepants  (1000) moorepants  (1000)        0 2017-08-27 08:32:13.000000 BicycleParameters-1.0.0/bicycleparameters/
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)       80 2017-05-19 04:40:25.000000 BicycleParameters-1.0.0/bicycleparameters/version.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     7786 2016-07-25 23:51:59.000000 BicycleParameters-1.0.0/bicycleparameters/tables.py
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)     2638 2017-05-18 22:17:03.000000 BicycleParameters-1.0.0/bicycleparameters/plot.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    10093 2016-07-25 23:51:59.000000 BicycleParameters-1.0.0/bicycleparameters/bicycle.py
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)    13348 2017-05-19 04:21:47.000000 BicycleParameters-1.0.0/bicycleparameters/rider.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      519 2016-07-25 23:51:59.000000 BicycleParameters-1.0.0/bicycleparameters/__init__.py
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)     7694 2017-05-19 04:21:47.000000 BicycleParameters-1.0.0/bicycleparameters/inertia.py
-drwxr-xr-x   0 moorepants  (1000) moorepants  (1000)        0 2017-08-27 08:32:13.000000 BicycleParameters-1.0.0/bicycleparameters/test/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      304 2016-07-25 23:51:59.000000 BicycleParameters-1.0.0/bicycleparameters/test/test_bicycleparameters.py
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)       38 2017-05-19 04:21:47.000000 BicycleParameters-1.0.0/bicycleparameters/test/__init__.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1142 2016-07-25 23:51:59.000000 BicycleParameters-1.0.0/bicycleparameters/test/test_bicycle.py
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)     6713 2017-05-19 04:21:47.000000 BicycleParameters-1.0.0/bicycleparameters/io.py
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)     9600 2017-05-19 04:21:47.000000 BicycleParameters-1.0.0/bicycleparameters/geometry.py
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)    15849 2017-05-19 04:21:47.000000 BicycleParameters-1.0.0/bicycleparameters/period.py
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)     7207 2017-05-19 04:21:47.000000 BicycleParameters-1.0.0/bicycleparameters/com.py
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)    47310 2017-08-26 23:32:35.000000 BicycleParameters-1.0.0/bicycleparameters/main.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.920733 bicycleparameters-1.1.0/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       93 2024-04-26 09:43:49.000000 bicycleparameters-1.1.0/AUTHORS
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.920733 bicycleparameters-1.1.0/BicycleParameters.egg-info/
+-rw-r--r--   0 moorepants  (1000) moorepants  (1000)     5438 2024-04-26 12:12:21.000000 bicycleparameters-1.1.0/BicycleParameters.egg-info/PKG-INFO
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     2607 2024-04-26 12:12:21.000000 bicycleparameters-1.1.0/BicycleParameters.egg-info/SOURCES.txt
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        1 2024-04-26 12:12:21.000000 bicycleparameters-1.1.0/BicycleParameters.egg-info/dependency_links.txt
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       75 2024-04-26 12:12:21.000000 bicycleparameters-1.1.0/BicycleParameters.egg-info/entry_points.txt
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      209 2024-04-26 12:12:21.000000 bicycleparameters-1.1.0/BicycleParameters.egg-info/requires.txt
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       18 2024-04-26 12:12:21.000000 bicycleparameters-1.1.0/BicycleParameters.egg-info/top_level.txt
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     2305 2024-04-26 12:07:50.000000 bicycleparameters-1.1.0/CHANGELOG.rst
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1540 2024-04-26 09:43:49.000000 bicycleparameters-1.1.0/LICENSE.txt
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      203 2024-04-26 12:05:37.000000 bicycleparameters-1.1.0/MANIFEST.in
+-rw-r--r--   0 moorepants  (1000) moorepants  (1000)     5438 2024-04-26 12:12:21.920733 bicycleparameters-1.1.0/PKG-INFO
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     3959 2024-04-26 09:43:49.000000 bicycleparameters-1.1.0/README.rst
+-rw-r--r--   0 moorepants  (1000) moorepants  (1000)      508 2020-03-27 22:53:27.000000 bicycleparameters-1.1.0/RELEASE.rst
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.916733 bicycleparameters-1.1.0/bicycleparameters/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      463 2024-04-26 11:21:36.000000 bicycleparameters-1.1.0/bicycleparameters/__init__.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.908733 bicycleparameters-1.1.0/bicycleparameters/app-data/
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.912733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.908733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Benchmark/
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.916733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Benchmark/Parameters/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      459 2020-07-02 21:17:40.000000 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Benchmark/Parameters/BenchmarkBenchmark.txt
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.908733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Browser/
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.916733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Browser/Parameters/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      751 2020-07-02 21:17:40.000000 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Browser/Parameters/BrowserBenchmark.txt
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.908733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Browserins/
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.916733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Browserins/Parameters/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      750 2020-07-02 21:17:40.000000 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Browserins/Parameters/BrowserinsBenchmark.txt
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.908733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Crescendo/
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.916733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Crescendo/Parameters/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      748 2020-07-02 21:17:40.000000 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Crescendo/Parameters/CrescendoBenchmark.txt
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.908733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Fisher/
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.916733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Fisher/Parameters/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      748 2020-07-02 21:17:40.000000 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Fisher/Parameters/FisherBenchmark.txt
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.912733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Pista/
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.916733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Pista/Parameters/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      751 2020-07-02 21:17:40.000000 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Pista/Parameters/PistaBenchmark.txt
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.912733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Rigid/
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.916733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Rigid/Parameters/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1199 2020-07-02 21:17:40.000000 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Rigid/Parameters/RigidBenchmark.txt
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.912733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Silver/
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.916733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Silver/Parameters/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      532 2020-07-02 21:17:40.000000 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Silver/Parameters/SilverBenchmark.txt
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.912733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Yellow/
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.916733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Yellow/Parameters/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      755 2020-07-02 21:17:40.000000 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Yellow/Parameters/YellowBenchmark.txt
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.912733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Yellowrev/
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.916733 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Yellowrev/Parameters/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      754 2020-07-02 21:17:40.000000 bicycleparameters-1.1.0/bicycleparameters/app-data/bicycles/Yellowrev/Parameters/YellowrevBenchmark.txt
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    20384 2024-04-26 11:21:36.000000 bicycleparameters-1.1.0/bicycleparameters/app.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.916733 bicycleparameters-1.1.0/bicycleparameters/assets/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     4715 2024-04-26 09:43:49.000000 bicycleparameters-1.1.0/bicycleparameters/assets/app-explanation.md
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      345 2020-07-02 21:17:40.000000 bicycleparameters-1.1.0/bicycleparameters/assets/styles.css
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    11690 2024-04-26 11:47:52.000000 bicycleparameters-1.1.0/bicycleparameters/bicycle.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     7308 2024-04-26 09:43:49.000000 bicycleparameters-1.1.0/bicycleparameters/com.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     5231 2024-04-26 11:21:36.000000 bicycleparameters-1.1.0/bicycleparameters/conversions.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     9614 2023-05-07 17:53:04.000000 bicycleparameters-1.1.0/bicycleparameters/geometry.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     7698 2024-04-26 09:43:49.000000 bicycleparameters-1.1.0/bicycleparameters/inertia.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     6593 2023-05-07 17:53:04.000000 bicycleparameters-1.1.0/bicycleparameters/io.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    70146 2024-04-26 11:21:36.000000 bicycleparameters-1.1.0/bicycleparameters/main.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    33785 2024-04-26 11:21:36.000000 bicycleparameters-1.1.0/bicycleparameters/models.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1705 2023-05-07 17:53:04.000000 bicycleparameters-1.1.0/bicycleparameters/parameter_dicts.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    44558 2024-04-26 11:21:36.000000 bicycleparameters-1.1.0/bicycleparameters/parameter_sets.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    15869 2023-05-07 17:53:04.000000 bicycleparameters-1.1.0/bicycleparameters/period.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     3331 2022-05-02 06:35:38.000000 bicycleparameters-1.1.0/bicycleparameters/plot.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    13358 2024-04-26 09:43:49.000000 bicycleparameters-1.1.0/bicycleparameters/rider.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     7812 2023-05-07 17:53:04.000000 bicycleparameters-1.1.0/bicycleparameters/tables.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.916733 bicycleparameters-1.1.0/bicycleparameters/tests/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2022-05-02 06:35:38.000000 bicycleparameters-1.1.0/bicycleparameters/tests/__init__.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.920733 bicycleparameters-1.1.0/bicycleparameters/tests/parameter_sets/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      916 2022-05-02 06:35:38.000000 bicycleparameters-1.1.0/bicycleparameters/tests/parameter_sets/benchmark-benchmark.yml
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      537 2022-05-02 06:35:38.000000 bicycleparameters-1.1.0/bicycleparameters/tests/parameter_sets/benchmark-browser.yml
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      487 2022-05-02 06:35:38.000000 bicycleparameters-1.1.0/bicycleparameters/tests/parameter_sets/benchmark-extendedoptc.yml
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      554 2022-05-02 06:35:38.000000 bicycleparameters-1.1.0/bicycleparameters/tests/parameter_sets/benchmark-pista.yml
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      850 2022-05-02 06:35:38.000000 bicycleparameters-1.1.0/bicycleparameters/tests/parameter_sets/benchmark-pistarider.yml
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      661 2022-05-02 06:35:38.000000 bicycleparameters-1.1.0/bicycleparameters/tests/parameter_sets/benchmark-pistarideroptimized3ms.yml
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      529 2022-05-02 06:35:38.000000 bicycleparameters-1.1.0/bicycleparameters/tests/parameter_sets/benchmark-realizedopttwo.yml
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      788 2022-05-02 06:35:38.000000 bicycleparameters-1.1.0/bicycleparameters/tests/parameter_sets/principal-browserjason.yml
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      646 2022-05-02 06:35:38.000000 bicycleparameters-1.1.0/bicycleparameters/tests/parameter_sets/principal-extendedoptf.yml
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     4267 2022-10-26 08:23:16.000000 bicycleparameters-1.1.0/bicycleparameters/tests/test_bicycle.py
+-rw-r--r--   0 moorepants  (1000) moorepants  (1000)      304 2020-03-27 22:53:27.000000 bicycleparameters-1.1.0/bicycleparameters/tests/test_bicycleparameters.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     4549 2022-10-19 12:36:30.000000 bicycleparameters-1.1.0/bicycleparameters/tests/test_models.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     3486 2024-04-26 11:21:36.000000 bicycleparameters-1.1.0/bicycleparameters/tests/test_parameter_sets.py
+-rw-r--r--   0 moorepants  (1000) moorepants  (1000)       80 2024-04-26 12:08:54.000000 bicycleparameters-1.1.0/bicycleparameters/version.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-26 12:12:21.920733 bicycleparameters-1.1.0/docs/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     4802 2022-10-26 09:33:43.000000 bicycleparameters-1.1.0/docs/app.rst
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1720 2022-10-26 09:34:04.000000 bicycleparameters-1.1.0/docs/bicycleparameters.rst
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    13143 2024-04-26 11:21:36.000000 bicycleparameters-1.1.0/docs/data.rst
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     4646 2022-10-19 12:36:30.000000 bicycleparameters-1.1.0/docs/description.rst
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    24094 2024-04-26 11:21:36.000000 bicycleparameters-1.1.0/docs/examples.rst
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      709 2022-10-26 09:33:52.000000 bicycleparameters-1.1.0/docs/index.rst
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1929 2024-04-26 09:43:49.000000 bicycleparameters-1.1.0/docs/installation.rst
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      162 2022-10-26 08:46:49.000000 bicycleparameters-1.1.0/requirements.txt
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       38 2024-04-26 12:12:21.920733 bicycleparameters-1.1.0/setup.cfg
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1850 2024-04-26 11:50:27.000000 bicycleparameters-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `BicycleParameters-1.0.0/LICENSE.txt` & `bicycleparameters-1.1.0/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2011-2016, Jason Keith Moore
+Copyright (c) 2011-2024, BicycleParameters Authors
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
   1. Redistributions of source code must retain the above copyright notice, this
      list of conditions and the following disclaimer.
```

### Comparing `BicycleParameters-1.0.0/README.rst` & `bicycleparameters-1.1.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,107 @@
-=========================
-Bicycle Parameters Module
-=========================
+=================
+BicycleParameters
+=================
 
-A python program designed to produce and manipulate the basic parameters needed
-for the Whipple bicycle model.
+A Python program designed to generate, manipulate, and visualize the parameters
+of the Whipple-Carvallo bicycle model.
 
-.. image:: https://travis-ci.org/moorepants/BicycleParameters.svg?branch=master
-   :target: https://travis-ci.org/moorepants/BicycleParameters
+.. list-table::
+
+   * - Download from PyPi
+     - |PyPi|
+   * - Download from Anaconda
+     - |Anaconda|
+   * - Documentation
+     - |RTD|
+   * - CI Status
+     - |GHCI|
+   * - Render App
+     - `Bicycle Dynamics App <https://bicycle-dynamics.onrender.com>`_
+
+.. |PyPi| image:: https://img.shields.io/pypi/v/BicycleParameters.svg
+   :target: https://pypi.org/project/BicycleParameters/
+
+.. |Anaconda| image:: https://anaconda.org/conda-forge/bicycleparameters/badges/version.svg
+   :target: https://anaconda.org/conda-forge/bicycleparameters
+
+.. |GHCI| image:: https://github.com/moorepants/BicycleParameters/actions/workflows/test.yml/badge.svg
+
+.. |RTD| image:: https://readthedocs.org/projects/bicycleparameters/badge/?version=latest
+   :target: https://bicycleparameters.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
 
 Dependencies
 ============
 
 Required
 --------
-- `Python 2.7 or >= 3.3 <http://www.python.org/>`_
-- `Numpy >= 1.6.1 <http://numpy.scipy.org/>`_
-- `Scipy >= 0.9.0 <http://www.scipy.org/>`_
-- `Matplotlib >= 1.1.1 <http://matplotlib.sourceforge.net/>`_
-- `Uncertainties >= 2.0.0 <http://pypi.python.org/pypi/uncertainties/>`_
-- `yeadon >= 1.1.0 <http://pypi.python.org/pypi/yeadon/>`_
-- `DynamicistToolKit >= 0.1.0
-  <http://pypi.python.org/pypi/DynamicistToolKit>`_
+
+- `DynamicistToolKit >= 0.5.3 <http://pypi.python.org/pypi/DynamicistToolKit>`_
+- `Matplotlib >= 3.5.1 <https://matplotlib.org/>`_
+- `NumPy >= 1.21.5 <https://numpy.org/>`_
+- `Python >= 3.8 <http://www.python.org/>`_
+- `SciPy >= 1.8.0 <https://scipy.org/>`_
+- `Uncertainties >= 3.1.5 <https://pythonhosted.org/uncertainties/>`_
+- `yeadon >= 1.3.0 <http://pypi.python.org/pypi/yeadon/>`_
 
 Optional
 --------
 
+These are required to run the Dash web application:
+
+- `Dash >= 2.0 <https://plotly.com/dash/>`_
+- `dash-bootstrap-components <https://github.com/facultyai/dash-bootstrap-components>`_
+- `Pandas >= 1.3.5 <https://pandas.pydata.org/>`_
+
 These are required to build the documentation:
 
-- `Sphinx <http://sphinx.pocoo.org/>`_
-- `Numpydoc <http://pypi.python.org/pypi/numpydoc>`_
+- `Sphinx >= 4.3.2 <http://sphinx.pocoo.org/>`_
+- `Numpydoc >= 1.2 <http://pypi.python.org/pypi/numpydoc>`_
 
 Installation
 ============
 
-The easiest method to download and install is with ``pip``::
+We recommend installing BicycleParameters with conda_ or pip_.
+
+.. _conda: https://docs.conda.io
+.. _pip: https://pip.pypa.io
+
+For conda::
+
+  $ conda install -c conda-forge bicycleparameters
+
+For pip::
 
   $ pip install BicycleParameters
 
-There are other options for getting the source code:
+The package can also be installed from the source code. The options for getting
+the source code are:
 
 1. Clone the source code with Git: ``git clone
    git://github.com/moorepants/BicycleParameters.git``
 2. `Download the source from Github`__.
 3. Download the source from pypi__.
 
 .. __: https://github.com/moorepants/BicycleParameters
 .. __: http://pypi.python.org/pypi/BicycleParameters
 
 Once you have the source code navigate to the directory and run::
 
   >>> python setup.py install
 
-This will install the software into your system and you should be able to
-import it with::
+This will install the software into your system. You can check if it installs
+with::
 
-  >>> import bicycleparameters
+   $ python -c "import bicycleparameters"
 
 Example Code
 ============
 
-::
+.. code-block:: python
 
     >>> import bicycleparameters as bp
     >>> import numpy as np
     >>> rigid = bp.Bicycle('Rigid')
     >>> par = rigid.parameters['Benchmark']
     >>> rigid.plot_bicycle_geometry()
     >>> speeds = np.linspace(0., 10., num=100)
@@ -77,75 +115,21 @@
 
 http://dx.doi.org/10.6084/m9.figshare.1198429
 
 Documentation
 =============
 
 Please refer to the `online documentation
-<http://packages.python.org/BicycleParameters>`_ for more information.
+<https://bicycleparameters.readthedocs.io/>`_ for more information.
 
 Grant Information
 =================
 
 This material is partially based upon work supported by the National Science
-Foundation under Grant No. 0928339. Any opinions, findings, and conclusions or
-recommendations expressed in this material are those of the authors and do not
-necessarily reflect the views of the National Science Foundation.
-
-Release Notes
-=============
-
-1.0.0
------
-
-- Support Python 3
-
-0.2.0
------
-
-- Commands using the state space form of the Whipple model have been reordered
-  to [roll angle, steer angle, roll rate, steer rate]
-- Added another rider's measurments.
-- Added a module for printing tables of data.
-- Added the Gyrobike and the ability to manage it's flywheel rigidbody.
-- Fixed a bug in `calculate_abc_geometry()` that gave incorrect geometry
-  values.
-- Handles two additional points for the Davis Instrumented Bicycle.
-- Added a child sized person based on scaling Charlie's measurements.
-- Added Bode plot commands.
-- Added nominal output options for several methods.
-- Added a dependency to DynamicistToolKit
-- Updated core dependencies to a minimum from the Ubuntu 12.04 release.
-- Tested with DTK 0.1.0 to 0.3.5.
-- Added Travis support.
-- The minimum yeadon version is bumped to 1.1.1 and code updated to reflect the
-  new yeadon api.
-- The minimum version of uncertainties is bumped to 2.0.
-
-0.1.3
------
-
-- Speed increase for the eigenvalue calculations.
-- Added measurements for the human configuration on some bikes.
-
-0.1.2
------
-
-- Fixed the tex related bug for the pendulum fit plots
-- Fixed some import bugs affecting the split fork/handlebar calcs
-
-0.1.1
------
-
-- changed the default directory to .
-- added pip install notes
-- fixed urls in setup.py and the readme
-- added version number to the package
-- removed the human machine classifier
-- reduced the size of the images in the docs
-- broke bicycleparameters.py into several modules
-- updated the documentation
+Foundation under `Grant No. 0928339`_. Any opinions, findings, and conclusions
+or recommendations expressed in this material are those of the authors and do
+not necessarily reflect the views of the National Science Foundation.
 
-0.1.0
------
+.. _Grant No. 0928339: https://www.nsf.gov/awardsearch/showAward?AWD_ID=0928339
 
-- Initial release.
+This material is partially based upon work supported by the TKI CLICKNL grant
+"Fiets van de Toekomst"(Grant No. TKI1706).
```

### Comparing `BicycleParameters-1.0.0/docs/bicycleparameters.rst` & `bicycleparameters-1.1.0/docs/bicycleparameters.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,89 +1,98 @@
 bicycleparameters Package
 =========================
 
 :mod:`main` Module
 ------------------
 
 .. automodule:: bicycleparameters.main
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 :mod:`com` Module
 -----------------
 
 .. automodule:: bicycleparameters.com
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 :mod:`bicycle` Module
 ---------------------
 
 .. automodule:: bicycleparameters.bicycle
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 :mod:`geometry` Module
 ----------------------
 
 .. automodule:: bicycleparameters.geometry
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 :mod:`inertia` Module
 ---------------------
 
 .. automodule:: bicycleparameters.inertia
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 :mod:`io` Module
 ----------------
 
 .. automodule:: bicycleparameters.io
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+:mod:`models` Module
+--------------------
+
+.. automodule:: bicycleparameters.models
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+:mod:`parameter_sets` Module
+----------------------------
+
+.. automodule:: bicycleparameters.parameter_sets
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 :mod:`period` Module
 --------------------
 
 .. automodule:: bicycleparameters.period
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 :mod:`plot` Module
 ------------------
 
 .. automodule:: bicycleparameters.plot
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 :mod:`rider` Module
 -------------------
 
 .. automodule:: bicycleparameters.rider
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 :mod:`tables` Module
 --------------------
 
 .. automodule:: bicycleparameters.tables
-    :members:
-    :undoc-members:
-    :show-inheritance:
-
-Subpackages
------------
-
-.. toctree::
-
-    bicycleparameters.test
+   :members:
+   :undoc-members:
+   :show-inheritance:
```

### Comparing `BicycleParameters-1.0.0/docs/index.rst` & `bicycleparameters-1.1.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,12 +16,13 @@
 .. toctree::
    :maxdepth: 2
 
    description.rst
    installation.rst
    examples.rst
    data.rst
+   app.rst
    bicycleparameters.rst
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `BicycleParameters-1.0.0/docs/description.rst` & `bicycleparameters-1.1.0/docs/description.rst`

 * *Files 2% similar despite different names*

```diff
@@ -58,20 +58,21 @@
 
     >>> import bicycleparameters as bp
     >>> import numpy as np
     >>> rigid = bp.Bicycle('Rigid')
     >>> par = rigid.parameters['Benchmark']
     >>> rigid.plot_bicycle_geometry()
     >>> speeds = np.linspace(0., 10., num=100)
-    >>> rigid.plot_eigenvalues_vs_speed(speeds)
+    >>> rigid.plot_eigenvalues_vs_speed(speeds, show=True)
 
 .. _references:
 
 References
 ==========
+
 The methods associated with this software were built upon these previous works,
 among others.
 
 .. [Roland1971] Roland J R ., R. D., and Massing , D. E. A digital computer simulation of
    bicycle dynamics. Calspan Report YA-3063-K-1, Cornell Aeronautical
    Laboratory, Inc., Buffalo, NY, 14221, Jun 1971. Prepared for Schwinn Bicycle
    Company, Chicago, IL 60639.
```

### Comparing `BicycleParameters-1.0.0/docs/installation.rst` & `bicycleparameters-1.1.0/docs/installation.rst`

 * *Files 12% similar despite different names*

```diff
@@ -5,49 +5,65 @@
 Dependencies
 ============
 These are the versions that I tested the code with, but the code will most
 likely work with older versions.
 
 Required
 --------
-- `Python 2.7 or >= 3.3 <http://www.python.org/>`_
-- `Numpy >= 1.6.1 <http://numpy.scipy.org/>`_
-- `Scipy >= 0.9.0 <http://www.scipy.org/>`_
-- `Matplotlib >= 1.1.1 <http://matplotlib.sourceforge.net/>`_
-- `Uncertainties >= 2.0.0 <http://pypi.python.org/pypi/uncertainties/>`_
-- `yeadon >= 1.1.0 <http://pypi.python.org/pypi/yeadon/>`_
-- `DynamicistToolKit >= 0.1.0
-  <http://pypi.python.org/pypi/DynamicistToolKit>`_
+
+- `DynamicistToolKit >= 0.5.3 <http://pypi.python.org/pypi/DynamicistToolKit>`_
+- `Matplotlib >= 3.5.1 <https://matplotlib.org/>`_
+- `NumPy >= 1.21.5 <https://numpy.org/>`_
+- `Python >= 3.8 <http://www.python.org/>`_
+- `SciPy >= 1.8.0 <https://scipy.org/>`_
+- `Uncertainties >= 3.1.5 <https://pythonhosted.org/uncertainties/>`_
+- `yeadon >= 1.3.0 <http://pypi.python.org/pypi/yeadon/>`_
 
 Optional
 --------
 
+These are required to run the Dash web application:
+
+- `Dash >= 2.0 <https://plotly.com/dash/>`_
+- `dash-bootstrap-components <https://github.com/facultyai/dash-bootstrap-components>`_
+- `Pandas >= 1.3.5 <https://pandas.pydata.org/>`_
+
 These are required to build the documentation:
 
-- `Sphinx <http://sphinx.pocoo.org/>`_
-- `Numpydoc <http://pypi.python.org/pypi/numpydoc>`_
+- `Sphinx >= 4.3.2 <http://sphinx.pocoo.org/>`_
+- `Numpydoc >= 1.2 <http://pypi.python.org/pypi/numpydoc>`_
 
 Installation
 ============
 
-The easiest method to download and install is with ``pip``::
+We recommend installing BicycleParameters with conda_ or pip_.
+
+.. _conda: https://docs.conda.io
+.. _pip: https://pip.pypa.io
+
+For conda::
+
+  $ conda install -c conda-forge bicycleparameters
+
+For pip::
 
   $ pip install BicycleParameters
 
-There are other options for getting the source code:
+The package can also be installed from the source code. The options for getting
+the source code are:
 
 1. Clone the source code with Git: ``git clone
    git://github.com/moorepants/BicycleParameters.git``
 2. `Download the source from Github`__.
 3. Download the source from pypi__.
 
 .. __: https://github.com/moorepants/BicycleParameters
 .. __: http://pypi.python.org/pypi/BicycleParameters
 
 Once you have the source code navigate to the directory and run::
 
   >>> python setup.py install
 
-This will install the software into your system and you should be able to
-import it with::
+This will install the software into your system. You can check if it installs
+with::
 
-  >>> import bicycleparameters
+   $ python -c "import bicycleparameters"
```

### Comparing `BicycleParameters-1.0.0/docs/examples.rst` & `bicycleparameters-1.1.0/docs/examples.rst`

 * *Files 15% similar despite different names*

```diff
@@ -176,15 +176,15 @@
   >>> bicycle.parameters['Measurements']
 
 All parameter sets are stored in the parameter dictionary of the bicycle
 instance.
 
 To modify a parameter type::
 
-  >>> bicycle.parameters['Benchmark']['mB] = 50.
+  >>> bicycle.parameters['Benchmark']['mB'] = 50.
 
 You can regenerate the parameter sets from the raw data stored in the bicycle's
 directory by calling::
 
   >>> bicycle.calculate_from_measured()
 
 Basic Analysis
@@ -275,22 +275,22 @@
 .. image:: bicycleGeometry.png
 
 For visualization of the linear analysis you can plot the root loci of the
 real and imaginary parts of the eigenvalues as a function of speed::
 
   >>> import numpy as np
   >>> speeds = np.linspace(0., 10., num=100)
-  >>> bicycle.plot_eigenvalues_vs_speed(speeds)
+  >>> bicycle.plot_eigenvalues_vs_speed(speeds, show=True)
 
 .. image:: eigenvaluesVsSpeed.png
 
 You can also compare the eigenvalues of two or more bicycles::
 
   >>> yellowrev = bp.Bicycle('Yellowrev')
-  >>> bp.plot_eigenvalues([bicycle, yellowrev], speeds)
+  >>> bp.plot_eigenvalues([bicycle, yellowrev], speeds, show=True)
 
 .. image:: eigCompare.png
 
 Tables
 ------
 You can generate reStructuredText tables of the bicycle parameters with the
 ``Table`` class::
@@ -488,21 +488,184 @@
 
   >>> bicycle.plot_bicycle_geometry()
 
 .. image:: bicycleRiderGeometry.png
 
 The eigenvalue plot also relfects the changes::
 
-  >>> bicycle.plot_eigenvalues_vs_speed(speeds)
+  >>> bicycle.plot_eigenvalues_vs_speed(speeds, show=True)
 
 .. image:: bicycleRiderEig.png
 
 Rider Visualization
 -------------------
 If you have the optional dependency, visual python, for yeadon installed then
 you can output a three dimensional picture of the Yeadon model configured to be
 seated on the bicycle. This is a bit buggy due to the nature of visual python,
 but is useful none-the-less.::
 
   >>> bicycle.add_rider('Jason', draw=True)
 
 .. image:: human.png
+
+Using Models and Parameter Sets
+===============================
+
+Parameter Sets
+--------------
+
+Parameter sets represent a set of constants in a multibody dynamics model.
+These constants have a name and an associated floating point value. This
+mapping from name to value is stored in a dictionary and then passed to a
+:py:class:`ParameterSet`. Below are the parameters for the Meijaard et al. 2007
+paper with some realistic initial values.
+
+.. plot::
+   :include-source: True
+   :context: close-figs
+
+   par = {
+       'IBxx': 11.3557360401,
+       'IBxz': -1.96756380745,
+       'IByy': 12.2177848012,
+       'IBzz': 3.12354397008,
+       'IFxx': 0.0904106601579,
+       'IFyy': 0.149389340425,
+       'IHxx': 0.253379594731,
+       'IHxz': -0.0720452391817,
+       'IHyy': 0.246138810935,
+       'IHzz': 0.0955770796289,
+       'IRxx': 0.0883819364527,
+       'IRyy': 0.152467620286,
+       'c': 0.0685808540382,
+       'g': 9.81,
+       'lam': 0.399680398707,
+       'mB': 81.86,
+       'mF': 2.02,
+       'mH': 3.22,
+       'mR': 3.11,
+       'rF': 0.34352982332,
+       'rR': 0.340958858855,
+       'v': 1.0,
+       'w': 1.121,
+       'xB': 0.289099434117,
+       'xH': 0.866949640247,
+       'zB': -1.04029228321,
+       'zH': -0.748236400835,
+   }
+
+The associated parameter set can be created with this dictionary:
+
+.. plot::
+   :include-source: True
+   :context: close-figs
+
+   from bicycleparameters.parameter_sets import Meijaard2007ParameterSet
+
+   par_set = Meijaard2007ParameterSet(par, True)
+
+Once the parameter set is available there are various methods that help you
+calculate and visualize the properties of this parameter set. This set
+describes the geometry, mass, and inertia of a bicycle. You can plot the
+geometry like so:
+
+.. plot::
+   :include-source: True
+   :context: close-figs
+
+   par_set.plot_geometry()
+
+You can then add symbols representing the mass centers of the four bodies like
+so:
+
+.. plot::
+   :include-source: True
+   :context: close-figs
+
+   ax = par_set.plot_geometry()
+   par_set.plot_mass_centers(ax=ax)
+
+The geometry, mass, and inertial information can all be plotted:
+
+.. plot::
+   :include-source: True
+   :context: close-figs
+
+   par_set.plot_all()
+
+Models
+------
+
+Parameter sets can be associated with a model and the model can be used to
+compute and visualize properties of the model's dynamics.
+
+.. plot::
+   :include-source: True
+   :context: close-figs
+
+   from bicycleparameters.models import Meijaard2007Model
+
+   model = Meijaard2007Model(par_set)
+
+The root locus with respect to any parameter, for example speed ``v``, can be
+plotted:
+
+.. plot::
+   :include-source: True
+   :context: close-figs
+
+   speeds = np.linspace(-10.0, 10.0, num=200)
+
+   model.plot_eigenvalue_parts(v=speeds)
+
+You can choose any parameter in the dictionary to generate the root locus and
+also override other parameters.
+
+.. plot::
+   :include-source: True
+   :context: close-figs
+
+   wheelbases = np.linspace(0.2, 5.0, num=50)
+
+   model.plot_eigenvalue_parts(v=6.0, w=wheelbases)
+
+The eigenvector components can be created for each mode and for a series of
+parameter values:
+
+.. plot::
+   :include-source: True
+   :context: close-figs
+
+   model.plot_eigenvectors(v=[1.0, 3.0, 5.0, 7.0])
+
+The eigenmodes can be simulated for specific parameter values:
+
+.. plot::
+   :include-source: True
+   :context: close-figs
+
+   times = np.linspace(0.0, 5.0, num=100)
+
+   model.plot_mode_simulations(times, v=6.0)
+
+A general simulation from initial conditions can also be run:
+
+.. plot::
+   :include-source: True
+   :context: close-figs
+
+   x0 = np.deg2rad([5.0, -3.0, 0.0, 0.0])
+
+   model.plot_simulation(times, x0, v=6.0)
+
+Inputs can be applied in the simulation, for example a simple positive feedback
+derivative controller on roll:
+
+.. plot::
+   :include-source: True
+   :context: close-figs
+
+   x0 = np.deg2rad([5.0, -3.0, 0.0, 0.0])
+
+   model.plot_simulation(times, x0,
+       input_func=lambda t, x: np.array([0.0, 50.0*x[2]]),
+       v=2.0)
```

### Comparing `BicycleParameters-1.0.0/docs/data.rst` & `bicycleparameters-1.1.0/docs/data.rst`

 * *Files 0% similar despite different names*

```diff
@@ -280,15 +280,15 @@
 This is an input file to set the configuration of the joint angles for the
 `yeadon package`_. All values should be set to zero except the ``sommersault``
 value. The ``sommersault`` value is pi minus the hunch angle of the rider on
 the bicycle. The hunch angle is the angle between the horizontal and the
 rider's torso mid line. It is essentially the angle at which the rider is
 leaned forward.
 
-<rider name><bicycle name>YeadonCFG.txt
----------------------------------------
+<rider name><bicycle name>YeadonMeas.txt
+----------------------------------------
 This is the yeadon measurement input file for the `yeadon package`_. It contains
 all of the geometric measurements of the rider. See the `yeadon documentation`_
 for more details.
 
 .. _yeadon package: http://pypi.python.org/pypi/yeadon
 .. _yeadon documentation : http://packages.python.org/yeadon/
```

### Comparing `BicycleParameters-1.0.0/BicycleParameters.egg-info/PKG-INFO` & `bicycleparameters-1.1.0/bicycleparameters/com.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,172 +1,237 @@
-Metadata-Version: 1.1
-Name: BicycleParameters
-Version: 1.0.0
-Summary: Generates and manipulates the physical parameters of a bicycle.
-Home-page: http://pypi.python.org/pypi/BicycleParameters
-Author: Jason Keith Moore
-Author-email: moorepants@gmail.com
-License: LICENSE.txt
-Description: =========================
-        Bicycle Parameters Module
-        =========================
-        
-        A python program designed to produce and manipulate the basic parameters needed
-        for the Whipple bicycle model.
-        
-        .. image:: https://travis-ci.org/moorepants/BicycleParameters.svg?branch=master
-           :target: https://travis-ci.org/moorepants/BicycleParameters
-        
-        Dependencies
-        ============
-        
-        Required
-        --------
-        - `Python 2.7 or >= 3.3 <http://www.python.org/>`_
-        - `Numpy >= 1.6.1 <http://numpy.scipy.org/>`_
-        - `Scipy >= 0.9.0 <http://www.scipy.org/>`_
-        - `Matplotlib >= 1.1.1 <http://matplotlib.sourceforge.net/>`_
-        - `Uncertainties >= 2.0.0 <http://pypi.python.org/pypi/uncertainties/>`_
-        - `yeadon >= 1.1.0 <http://pypi.python.org/pypi/yeadon/>`_
-        - `DynamicistToolKit >= 0.1.0
-          <http://pypi.python.org/pypi/DynamicistToolKit>`_
-        
-        Optional
-        --------
-        
-        These are required to build the documentation:
-        
-        - `Sphinx <http://sphinx.pocoo.org/>`_
-        - `Numpydoc <http://pypi.python.org/pypi/numpydoc>`_
-        
-        Installation
-        ============
-        
-        The easiest method to download and install is with ``pip``::
-        
-          $ pip install BicycleParameters
-        
-        There are other options for getting the source code:
-        
-        1. Clone the source code with Git: ``git clone
-           git://github.com/moorepants/BicycleParameters.git``
-        2. `Download the source from Github`__.
-        3. Download the source from pypi__.
-        
-        .. __: https://github.com/moorepants/BicycleParameters
-        .. __: http://pypi.python.org/pypi/BicycleParameters
-        
-        Once you have the source code navigate to the directory and run::
-        
-          >>> python setup.py install
-        
-        This will install the software into your system and you should be able to
-        import it with::
-        
-          >>> import bicycleparameters
-        
-        Example Code
-        ============
-        
-        ::
-        
-            >>> import bicycleparameters as bp
-            >>> import numpy as np
-            >>> rigid = bp.Bicycle('Rigid')
-            >>> par = rigid.parameters['Benchmark']
-            >>> rigid.plot_bicycle_geometry()
-            >>> speeds = np.linspace(0., 10., num=100)
-            >>> rigid.plot_eigenvalues_vs_speed(speeds)
-        
-        Sample Data
-        ===========
-        
-        Some sample data is included in the repository but a full source with all the
-        raw data files can be downloaded from here:
-        
-        http://dx.doi.org/10.6084/m9.figshare.1198429
-        
-        Documentation
-        =============
-        
-        Please refer to the `online documentation
-        <http://packages.python.org/BicycleParameters>`_ for more information.
-        
-        Grant Information
-        =================
-        
-        This material is partially based upon work supported by the National Science
-        Foundation under Grant No. 0928339. Any opinions, findings, and conclusions or
-        recommendations expressed in this material are those of the authors and do not
-        necessarily reflect the views of the National Science Foundation.
-        
-        Release Notes
-        =============
-        
-        1.0.0
-        -----
-        
-        - Support Python 3
-        
-        0.2.0
-        -----
-        
-        - Commands using the state space form of the Whipple model have been reordered
-          to [roll angle, steer angle, roll rate, steer rate]
-        - Added another rider's measurments.
-        - Added a module for printing tables of data.
-        - Added the Gyrobike and the ability to manage it's flywheel rigidbody.
-        - Fixed a bug in `calculate_abc_geometry()` that gave incorrect geometry
-          values.
-        - Handles two additional points for the Davis Instrumented Bicycle.
-        - Added a child sized person based on scaling Charlie's measurements.
-        - Added Bode plot commands.
-        - Added nominal output options for several methods.
-        - Added a dependency to DynamicistToolKit
-        - Updated core dependencies to a minimum from the Ubuntu 12.04 release.
-        - Tested with DTK 0.1.0 to 0.3.5.
-        - Added Travis support.
-        - The minimum yeadon version is bumped to 1.1.1 and code updated to reflect the
-          new yeadon api.
-        - The minimum version of uncertainties is bumped to 2.0.
-        
-        0.1.3
-        -----
-        
-        - Speed increase for the eigenvalue calculations.
-        - Added measurements for the human configuration on some bikes.
-        
-        0.1.2
-        -----
-        
-        - Fixed the tex related bug for the pendulum fit plots
-        - Fixed some import bugs affecting the split fork/handlebar calcs
-        
-        0.1.1
-        -----
-        
-        - changed the default directory to .
-        - added pip install notes
-        - fixed urls in setup.py and the readme
-        - added version number to the package
-        - removed the human machine classifier
-        - reduced the size of the images in the docs
-        - broke bicycleparameters.py into several modules
-        - updated the documentation
-        
-        0.1.0
-        -----
-        
-        - Initial release.
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Physics
+#!/usr/bin/env python
+
+from math import pi
+import numpy as np
+from uncertainties import umath, unumpy
+
+# local modules
+from .geometry import calculate_l1_l2, fwheel_to_handlebar_ref
+
+
+def cartesian(arrays, out=None):
+    """Generate a cartesian product of input arrays.
+
+    Parameters
+    ----------
+    arrays : list of array-like
+        1-D arrays to form the cartesian product of.
+    out : ndarray
+        Array to place the cartesian product in.
+
+    Returns
+    -------
+    out : ndarray
+        2-D array of shape (M, len(arrays)) containing cartesian products
+        formed of input arrays.
+
+    Examples
+    --------
+    >>> cartesian(([1, 2, 3], [4, 5], [6, 7]))
+    array([[1, 4, 6],
+           [1, 4, 7],
+           [1, 5, 6],
+           [1, 5, 7],
+           [2, 4, 6],
+           [2, 4, 7],
+           [2, 5, 6],
+           [2, 5, 7],
+           [3, 4, 6],
+           [3, 4, 7],
+           [3, 5, 6],
+           [3, 5, 7]])
+
+    """
+
+    arrays = [np.asarray(x) for x in arrays]
+    dtype = arrays[0].dtype
+
+    n = np.prod([x.size for x in arrays])
+    if out is None:
+        out = np.zeros([n, len(arrays)], dtype=dtype)
+
+    m = n // arrays[0].size
+    out[:, 0] = np.repeat(arrays[0], m)
+    if arrays[1:]:
+        cartesian(arrays[1:], out=out[0:m, 1:])
+        for j in range(1, arrays[0].size):
+            out[j*m:(j+1)*m, 1:] = out[0:m, 1:]
+    return out
+
+
+def center_of_mass(slopes, intercepts):
+    '''Returns the center of mass relative to the slopes and intercepts
+    coordinate system.
+
+    Parameters
+    ----------
+    slopes : ndarray, shape(n,)
+        The slope of every line used to calculate the center of mass.
+    intercepts : ndarray, shape(n,)
+        The intercept of every line used to calculate the center of mass.
+
+    Returns
+    -------
+    x : float
+        The abscissa of the center of mass.
+    y : float
+        The ordinate of the center of mass.
+
+    '''
+    num = range(len(slopes))
+    allComb = cartesian((num, num))
+    comb = []
+    # remove doubles
+    for row in allComb:
+        if row[0] != row[1]:
+            comb.append(row)
+    comb = np.array(comb)
+
+    # initialize the matrix to store the line intersections
+    lineX = np.zeros((len(comb), 2), dtype='object')
+    # for each line intersection...
+    for j, row in enumerate(comb):
+        sl = np.array([slopes[row[0]], slopes[row[1]]])
+        a = unumpy.array(np.vstack((-sl, np.ones((2)))).T)
+        b = np.array([intercepts[row[0]], intercepts[row[1]]])
+        lineX[j] = np.dot(a.I, b)
+    com = np.mean(lineX, axis=0)
+
+    return com[0], com[1]
+
+
+def com_line(alpha, a, par, part, l1, l2):
+    '''Returns the slope and intercept for the line that passes through the
+    part's center of mass with reference to the benchmark bicycle coordinate
+    system.
+
+    Parameters
+    ----------
+    alpha : float
+        The angle the head tube makes with the horizontal. When looking at the
+        bicycle from the right side this is the angle between a vector point
+        out upwards along the steer axis and the earth horizontal with the
+        positve direction pointing from the left to the right. If the bike is
+        in its normal configuration this would be 90 degrees plus the steer
+        axis tilt (lambda).
+    a : float
+        The distance from the pendulum axis to a reference point on the part,
+        typically the wheel centers. This is positive if the point falls to the
+        left of the axis and negative otherwise.
+    par : dictionary
+        Benchmark parameters. Must include lam, rR, rF, w
+    part : string
+        The subscript denoting which part this refers to.
+    l1, l2 : floats
+        The location of the handlebar reference point relative to the front
+        wheel center when the fork is split. This is measured perpendicular to
+        and along the steer axis, respectively.
+
+    Returns
+    -------
+    m : float
+        The slope of the line in the benchmark coordinate system.
+    b : float
+        The z intercept in the benchmark coordinate system.
+
+    '''
+
+    # beta is the angle between the x bike frame and the x pendulum frame,
+    # rotation about positive y
+    beta = par['lam'] - alpha * pi / 180
+
+    # calculate the slope of the center of mass line
+    m = -umath.tan(beta)
+
+    # calculate the z intercept
+    # this the bicycle frame
+    if part == 'B':
+        b = -a / umath.cos(beta) - par['rR']
+    # this is the fork (without handlebar) or the fork and handlebar combined
+    elif part == 'S' or part == 'H':
+        b = -a / umath.cos(beta) - par['rF'] + par['w'] * umath.tan(beta)
+    # this is the handlebar (without fork)
+    elif part == 'G':
+        u1, u2 = fwheel_to_handlebar_ref(par['lam'], l1, l2)
+        b = (-a/umath.cos(beta) - (par['rF'] + u2) + (par['w'] -
+                                                      u1)*umath.tan(beta))
+    else:
+        print(part, "doesn't exist")
+        raise KeyError
+
+    return m, b, beta
+
+
+def part_com_lines(mp, par, forkIsSplit):
+    '''Returns the slopes and intercepts for all of the center of mass lines
+    for each part.
+
+    Parameters
+    ----------
+    mp : dictionary
+        Dictionary with the measured parameters.
+
+    Returns
+    -------
+    slopes : dictionary
+        Contains a list of slopes for each part.
+    intercepts : dictionary
+        Contains a list of intercepts for each part.
+
+    The slopes and intercepts lists are in order with respect to each other and
+    the keyword is either 'B', 'H', 'G' or 'S' for Frame, Handlebar/Fork,
+    Handlerbar, and Fork respectively.
+
+    '''
+    # find the slope and intercept for pendulum axis
+    if forkIsSplit:
+        l1, l2 = calculate_l1_l2(mp['h6'], mp['h7'], mp['d5'],
+                                 mp['d6'], mp['l'])
+        slopes = {'B': [], 'G': [], 'S': []}
+        intercepts = {'B': [], 'G': [], 'S': []}
+        betas = {'B': [], 'G': [], 'S': []}
+    else:
+        l1, l2 = 0., 0.
+        slopes = {'B': [], 'H': []}
+        intercepts = {'B': [], 'H': []}
+        betas = {'B': [], 'H': []}
+
+    # get the alpha keys and put them in order
+    listOfAlphaKeys = [x for x in mp.keys() if x.startswith('alpha')]
+    listOfAlphaKeys.sort()
+
+    # caluclate m, b and beta for each orientation
+    for key in listOfAlphaKeys:
+        alpha = mp[key]
+        a = mp['a' + key[5:]]
+        part = key[5]
+        m, b, beta = com_line(alpha, a, par, part, l1, l2)
+        slopes[part].append(m)
+        intercepts[part].append(b)
+        betas[part].append(beta)
+
+    return slopes, intercepts, betas
+
+
+def total_com(coordinates, masses):
+    '''Returns the center of mass of a group of objects if the indivdual
+    centers of mass and mass is provided.
+
+    coordinates : array_like, shape(3,n)
+        The rows are the x, y and z coordinates, respectively and the columns
+        are for each object.
+    masses : array_like, shape(3,)
+        An array of the masses of multiple objects, the order should correspond
+        to the columns of coordinates.
+
+    Returns
+    -------
+    mT : float
+        Total mass of the objects.
+    cT : ndarray, shape(3,)
+        The x, y, and z coordinates of the total center of mass.
+
+    '''
+    products = np.asarray(masses) * np.asarray(coordinates)
+    mT = np.sum(masses)
+    cT = np.sum(products, axis=1) / mT
+    return mT, cT
```

### Comparing `BicycleParameters-1.0.0/setup.py` & `bicycleparameters-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,27 +10,43 @@
     author='Jason Keith Moore',
     author_email='moorepants@gmail.com',
     packages=find_packages(),
     url='http://pypi.python.org/pypi/BicycleParameters',
     license='LICENSE.txt',
     description='Generates and manipulates the physical parameters of a bicycle.',
     long_description=open('README.rst').read(),
-    install_requires=['numpy>=1.6.1',
-                      'scipy>=0.9.0',
-                      'matplotlib>=1.1.1',
-                      'uncertainties>=2.0.0',
-                      'yeadon>=1.1.0',
-                      'DynamicistToolKit>=0.1.0'],
-    extras_require={'doc': ['sphinx', 'numpydoc']},
-    tests_require=['nose'],
-    test_suite='nose.collector',
+    install_requires=[
+        'DynamicistToolKit>=0.5.3',
+        'matplotlib>=3.5.1',
+        'numpy>=1.21.5',
+        'pyyaml>=5.4.1',
+        'scipy>=1.8.0',
+        'uncertainties>=3.1.5',
+        'yeadon>=1.3.0',
+    ],
+    python_requires='>=3.8',
+    extras_require={
+        'doc': [
+            'sphinx>=4.3.2',
+            'numpydoc>=1.2'
+        ],
+        'app': [
+            'dash>=2',
+            'dash-bootstrap-components',
+            'pandas>=1.3.5'
+        ],
+    },
+    entry_points={'console_scripts':
+                  ['bicycleparameters = bicycleparameters.app:app.run_server']},
     classifiers=['Programming Language :: Python',
-                 'Programming Language :: Python :: 2.7',
-                 'Programming Language :: Python :: 3.4',
-                 'Programming Language :: Python :: 3.5',
+                 'Programming Language :: Python :: 3.8',
+                 'Programming Language :: Python :: 3.9',
+                 'Programming Language :: Python :: 3.10',
+                 'Programming Language :: Python :: 3.11',
+                 'Programming Language :: Python :: 3.12',
                  'Operating System :: OS Independent',
                  'Development Status :: 5 - Production/Stable',
                  'Intended Audience :: Science/Research',
                  'License :: OSI Approved :: BSD License',
                  'Natural Language :: English',
                  'Topic :: Scientific/Engineering',
                  'Topic :: Scientific/Engineering :: Physics']
```

### Comparing `BicycleParameters-1.0.0/bicycleparameters/tables.py` & `bicycleparameters-1.1.0/bicycleparameters/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from math import ceil
 
+
 class Table():
     """A class for generating tables of the measurment and parameter data
     associated with a bicycle. """
 
     def __init__(self, source, latex, bicycles):
         """Sets the basic attributes of the table.
 
@@ -32,16 +33,16 @@
         allVariables = []
         try:
             for bicycle in self.bicycles:
                 allVariables += bicycle.parameters[self.source].keys()
         except TypeError:
             allVariables += self.bicycle.parameters[self.source].keys()
         # remove duplicates and sort
-        self.allVariables = sorted(list(set(allVariables)),
-                key=lambda x: x.lower())
+        self.allVariables = sorted(list(set(allVariables)), key=lambda x:
+                                   x.lower())
 
     def generate_table_data(self):
         """Generates a list of data for a table."""
         table = []
         for var in self.allVariables:
             # add a new line
             table.append([])
@@ -87,15 +88,15 @@
             for i, row in enumerate(table):
                 self.tableData[i][0] = ':math:`' + row[0] + '`'
 
         # add a sub header
         table.insert(0, ['Variable'])
         for i, bicycle in enumerate(self.bicycles):
             if self.latex:
-                table[0] += [':math:`v`', ':math:`\sigma`']
+                table[0] += [':math:`v`', r':math:`\sigma`']
             else:
                 table[0] += ['v', 'sigma']
 
         # find the longest string in each column
         largest = [0] # the top left is empty
         for bicycle in self.bicycles:
             l = int(ceil(len(bicycle.bicycleName) / 2.0))
@@ -142,14 +143,15 @@
         if fileName is not None:
             f = open(fileName, 'w')
             f.write(rstTable)
             f.close()
 
         return rstTable
 
+
 def to_latex(var):
     """Returns a latex representation for a given variable string name.
 
     Parameters
     ----------
     var : string
         One of the variable names used in the bicycleparameters package.
@@ -159,28 +161,28 @@
     latex : string
         A string formatting for pretty LaTeX math print.
 
     """
 
     latexMap = {'f': 'f',
                 'w': 'w',
-                'gamma': '\gamma',
+                'gamma': r'\gamma',
                 'g': 'g',
                 'lcs': 'l_{cs}',
                 'hbb': 'h_{bb}',
                 'lsp': 'l_{sp}',
                 'lst': 'l_{st}',
-                'lamst': '\lambda_{st}',
+                'lamst': r'\lambda_{st}',
                 'whb': 'w_{hb}',
                 'LhbF': 'l_{hbF}',
                 'LhbR': 'l_{hbR}',
                 'd': 'd',
                 'l': 'l',
                 'c': 'c',
-                'lam': '\lambda',
+                'lam': r'\lambda',
                 'xcl': 'x_{cl}',
                 'zcl': 'z_{cl}',
                 'ds1': 'd_{s1}',
                 'ds3': 'd_{s3}'}
     try:
         latex = latexMap[var]
     except KeyError:
@@ -195,14 +197,15 @@
         elif var.startswith('I'):
             latex = var[0] + '_{' + var[1:] + '}'
         else:
             raise
 
     return latex
 
+
 def uround(value):
     '''Returns a string representation of a value with an uncertainity which
     has been rounded to significant digits based on the uncertainty value.
 
     Parameters
     ----------
     value : ufloat
```

### Comparing `BicycleParameters-1.0.0/bicycleparameters/plot.py` & `bicycleparameters-1.1.0/bicycleparameters/plot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 
 import numpy as np
 import matplotlib.pyplot as plt
 
+
 def compare_bode_bicycles(bikes, speed, u, y, fig=None):
     """Returns a figure with the Bode plots of multiple bicycles.
 
     Parameters
     ----------
     bikes : list
         A list of bicycleparameters.Bicycle instances.
@@ -42,16 +43,17 @@
     for line in phaseLines:
         firstValue = line.get_ydata()[0]
         n = np.ceil(np.floor(abs(firstValue / 180.)) / 2.)
         line.set_ydata(line.get_ydata() - np.sign(firstValue) * n * 360.)
 
     return fig
 
+
 def plot_eigenvalues(bikes, speeds, colors=None, linestyles=None,
-        largest=False, show=False):
+                     largest=False, show=False):
     '''Returns a figure with the eigenvalues vs speed for multiple bicycles.
 
     Parameters
     ----------
     bikes : list
         A list of Bicycle objects.
     speeds : ndarray, shape(n,)
@@ -91,7 +93,26 @@
         plt.legend()
         plt.axis('tight')
 
     if show is True:
         plt.show()
 
     return fig
+
+
+def _generate_ellipse_plot_data(x_center, y_center, ax1, ax2, a, b, N):
+    # x_center, y_center the coordinates of ellipse center
+    # ax1 ax2 two orthonormal vectors representing the ellipse axis directions
+    # a, b the ellipse parameters
+    t = np.linspace(0, 2 * np.pi, N)
+    # ellipse parameterization with respect to a system of axes of directions
+    # a1, a2
+    xs = a * np.cos(t)
+    ys = b * np.sin(t)
+    # rotation matrix
+    R = np.array([ax1, ax2]).T
+    # coordinate of the ellipse points with respect to the system of axes[1,
+    # 0], [0, 1] with origin(0, 0)
+    xp, yp = np.dot(R, [xs, ys])
+    x = xp + x_center
+    y = yp + y_center
+    return x, y
```

### Comparing `BicycleParameters-1.0.0/bicycleparameters/bicycle.py` & `bicycleparameters-1.1.0/bicycleparameters/bicycle.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 
 import numpy as np
 from scipy.optimize import newton
 from uncertainties import umath, ufloat
 
+
 def ab_matrix(M, C1, K0, K2, v, g):
     '''Calculate the A and B matrices for the Whipple bicycle model linearized
     about the upright configuration.
 
     Parameters
     ----------
     M : ndarray, shape(2,2)
@@ -36,28 +37,30 @@
                     steer rate]
     The inputs are [roll torque,
                     steer torque]
 
     '''
 
     invM = (1. / (M[0, 0] * M[1, 1] - M[0, 1] * M[1, 0]) *
-           np.array([[M[1, 1], -M[0, 1]], [-M[1, 0], M[0, 0]]], dtype=M.dtype))
+            np.array([[M[1, 1], -M[0, 1]], [-M[1, 0], M[0, 0]]],
+                     dtype=M.dtype))
 
     a11 = np.zeros((2, 2))
     a12 = np.eye(2)
     # stiffness based terms
     a21 = -np.dot(invM, (g * K0 + v**2 * K2))
     # damping based terms
     a22 = -np.dot(invM, v * C1)
 
     A = np.vstack((np.hstack((a11, a12)), np.hstack((a21, a22))))
     B = np.vstack((np.zeros((2, 2)), invM))
 
     return A, B
 
+
 def benchmark_par_to_canonical(p):
     '''Returns the canonical matrices of the Whipple bicycle model linearized
     about the upright constant velocity configuration. It uses the parameter
     definitions from Meijaard et al. 2007.
 
     Parameters
     ----------
@@ -78,82 +81,81 @@
 
     Notes
     -----
     This function handles parameters with uncertanties.
 
     '''
     mT = p['mR'] + p['mB'] + p['mH'] + p['mF']
-    xT = (p['xB'] * p['mB'] + p['xH'] * p['mH'] + p['w'] * p['mF']) / mT
-    zT = (-p['rR'] * p['mR'] + p['zB'] * p['mB'] +
-          p['zH'] * p['mH'] - p['rF'] * p['mF']) / mT
+    xT = (p['xB']*p['mB'] + p['xH']*p['mH'] + p['w']*p['mF']) / mT
+    zT = (-p['rR']*p['mR'] + p['zB']*p['mB'] +
+          p['zH']*p['mH'] - p['rF']*p['mF']) / mT
 
     ITxx = (p['IRxx'] + p['IBxx'] + p['IHxx'] + p['IFxx'] + p['mR'] *
-            p['rR']**2 + p['mB'] * p['zB']**2 + p['mH'] * p['zH']**2 + p['mF']
-            * p['rF']**2)
-    ITxz = (p['IBxz'] + p['IHxz'] - p['mB'] * p['xB'] * p['zB'] -
-            p['mH'] * p['xH'] * p['zH'] + p['mF'] * p['w'] * p['rF'])
+            p['rR']**2 + p['mB']*p['zB']**2 + p['mH']*p['zH']**2 +
+            p['mF']*p['rF']**2)
+    ITxz = (p['IBxz'] + p['IHxz'] - p['mB']*p['xB']*p['zB'] -
+            p['mH']*p['xH']*p['zH'] + p['mF']*p['w']*p['rF'])
     p['IRzz'] = p['IRxx']
     p['IFzz'] = p['IFxx']
     ITzz = (p['IRzz'] + p['IBzz'] + p['IHzz'] + p['IFzz'] +
-            p['mB'] * p['xB']**2 + p['mH'] * p['xH']**2 + p['mF'] * p['w']**2)
+            p['mB']*p['xB']**2 + p['mH']*p['xH']**2 + p['mF']*p['w']**2)
 
     mA = p['mH'] + p['mF']
-    xA = (p['xH'] * p['mH'] + p['w'] * p['mF']) / mA
-    zA = (p['zH'] * p['mH'] - p['rF']* p['mF']) / mA
+    xA = (p['xH']*p['mH'] + p['w']*p['mF']) / mA
+    zA = (p['zH']*p['mH'] - p['rF']*p['mF']) / mA
 
-    IAxx = (p['IHxx'] + p['IFxx'] + p['mH'] * (p['zH'] - zA)**2 +
-            p['mF'] * (p['rF'] + zA)**2)
-    IAxz = (p['IHxz'] - p['mH'] * (p['xH'] - xA) * (p['zH'] - zA) + p['mF'] *
-            (p['w'] - xA) * (p['rF'] + zA))
-    IAzz = (p['IHzz'] + p['IFzz'] + p['mH'] * (p['xH'] - xA)**2 + p['mF'] *
+    IAxx = (p['IHxx'] + p['IFxx'] + p['mH']*(p['zH'] - zA)**2 +
+            p['mF']*(p['rF'] + zA)**2)
+    IAxz = (p['IHxz'] - p['mH']*(p['xH'] - xA)*(p['zH'] - zA) + p['mF'] *
+            (p['w'] - xA)*(p['rF'] + zA))
+    IAzz = (p['IHzz'] + p['IFzz'] + p['mH']*(p['xH'] - xA)**2 + p['mF'] *
             (p['w'] - xA)**2)
-    uA = (xA - p['w'] - p['c']) * umath.cos(p['lam']) - zA * umath.sin(p['lam'])
-    IAll = (mA * uA**2 + IAxx * umath.sin(p['lam'])**2 +
-            2 * IAxz * umath.sin(p['lam']) * umath.cos(p['lam']) +
-            IAzz * umath.cos(p['lam'])**2)
-    IAlx = (-mA * uA * zA + IAxx * umath.sin(p['lam']) + IAxz *
-            umath.cos(p['lam']))
-    IAlz = (mA * uA * xA + IAxz * umath.sin(p['lam']) + IAzz *
-            umath.cos(p['lam']))
+    uA = (xA - p['w'] - p['c'])*umath.cos(p['lam']) - zA*umath.sin(p['lam'])
+    IAll = (mA*uA**2 + IAxx*umath.sin(p['lam'])**2 +
+            2*IAxz*umath.sin(p['lam'])*umath.cos(p['lam']) +
+            IAzz*umath.cos(p['lam'])**2)
+    IAlx = (-mA*uA*zA + IAxx*umath.sin(p['lam']) + IAxz*umath.cos(p['lam']))
+    IAlz = (mA*uA*xA + IAxz*umath.sin(p['lam']) + IAzz*umath.cos(p['lam']))
 
-    mu = p['c'] / p['w'] * umath.cos(p['lam'])
+    mu = p['c'] / p['w']*umath.cos(p['lam'])
 
     SR = p['IRyy'] / p['rR']
     SF = p['IFyy'] / p['rF']
     ST = SR + SF
-    SA = mA * uA + mu * mT * xT
+    SA = mA*uA + mu*mT*xT
 
     Mpp = ITxx
-    Mpd = IAlx + mu * ITxz
+    Mpd = IAlx + mu*ITxz
     Mdp = Mpd
-    Mdd = IAll + 2 * mu * IAlz + mu**2 * ITzz
+    Mdd = IAll + 2*mu*IAlz + mu**2*ITzz
     M = np.array([[Mpp, Mpd], [Mdp, Mdd]])
 
-    K0pp = mT * zT # this value only reports to 13 digit precision it seems?
+    K0pp = mT*zT  # this value only reports to 13 digit precision it seems?
     K0pd = -SA
     K0dp = K0pd
-    K0dd = -SA * umath.sin(p['lam'])
+    K0dd = -SA*umath.sin(p['lam'])
     K0 = np.array([[K0pp, K0pd], [K0dp, K0dd]])
 
     K2pp = 0.
-    K2pd = (ST - mT * zT) / p['w'] * umath.cos(p['lam'])
+    K2pd = (ST - mT*zT) / p['w']*umath.cos(p['lam'])
     K2dp = 0.
-    K2dd = (SA + SF * umath.sin(p['lam'])) / p['w'] * umath.cos(p['lam'])
+    K2dd = (SA + SF*umath.sin(p['lam'])) / p['w']*umath.cos(p['lam'])
     K2 = np.array([[K2pp, K2pd], [K2dp, K2dd]])
 
     C1pp = 0.
     C1pd = (mu*ST + SF*umath.cos(p['lam']) + ITxz / p['w'] *
             umath.cos(p['lam']) - mu*mT*zT)
-    C1dp = -(mu * ST + SF * umath.cos(p['lam']))
-    C1dd = (IAlz / p['w'] * umath.cos(p['lam']) + mu * (SA +
-            ITzz / p['w'] * umath.cos(p['lam'])))
+    C1dp = -(mu*ST + SF*umath.cos(p['lam']))
+    C1dd = (IAlz / p['w']*umath.cos(p['lam']) + mu*(SA +
+            ITzz / p['w']*umath.cos(p['lam'])))
     C1 = np.array([[C1pp, C1pd], [C1dp, C1dd]])
 
     return M, C1, K0, K2
 
+
 def lambda_from_abc(rF, rR, a, b, c):
     '''Returns the steer axis tilt, lamba, for the parameter set based on the
     offsets from the steer axis.
 
     Parameters
     ----------
     rF : float or ufloat
@@ -169,29 +171,80 @@
     c : float or ufloat
         The steer axis distance. The distance along the steer axis between the
         intersection of the front and rear wheel offset lines.
 
     '''
     def lam_equality(lam, rF, rR, a, b, c):
         return umath.sin(lam) - (rF - rR + c * umath.cos(lam)) / (a + b)
-    guess = umath.atan(c / (a + b)) # guess based on equal wheel radii
+    guess = umath.atan(c / (a + b))  # guess based on equal wheel radii
 
     # The following assumes that the uncertainty calculated for the guess is
     # the same as the uncertainty for the true solution. This is not true! and
     # will surely breakdown the further the guess is away from the true
     # solution. There may be a way to calculate the correct uncertainity, but
     # that needs to be figured out. I guess I could use least squares and do it
     # the same way as get_period.
 
     args = (rF.nominal_value, rR.nominal_value, a.nominal_value,
             b.nominal_value, c.nominal_value)
 
     lam = newton(lam_equality, guess.nominal_value, args=args)
     return ufloat(lam, guess.std_dev)
 
+
+def sort_eigenmodes(evals, evecs):
+    """Sort eigenvalues and eigenvectors.
+
+    Parameters
+    ==========
+    evals : ndarray, shape (n, 4)
+        A sequence of n sets of eigenvalues.
+    evecs : ndarray, shape (n, 4, 4)
+        A sequence of n sets of eigenvectors.
+
+    Returns
+    =======
+    evalsorg : ndarray, shape (n, 4)
+        A sequence of n sets of eigenvalues.
+    evecsorg : ndarray, shape (n, 4, 4)
+        A sequence of n sets of eigenvectors.
+
+    """
+    evalsorg = np.zeros_like(evals)
+    evecsorg = np.zeros_like(evecs)
+    # set the first row to be the same
+    evalsorg[0] = evals[0]
+    evecsorg[0] = evecs[0]
+    # for each speed
+    for i, speed in enumerate(evals):
+        if i == evals.shape[0] - 1:
+            break
+        # for each current eigenvalue
+        used = []
+        for j, e in enumerate(speed):
+            x, y = np.real(evalsorg[i, j]), np.imag(evalsorg[i, j])
+            # for each eigenvalue at the next speed
+            dist = np.zeros(4)
+            for k, eignext in enumerate(evals[i + 1]):
+                xn, yn = np.real(eignext), np.imag(eignext)
+                # distance between points in the real/imag plane
+                dist[k] = np.abs(((xn - x)**2 + (yn - y)**2)**0.5)
+            if np.argmin(dist) in used:
+                # set the already used indice higher
+                dist[np.argmin(dist)] = np.max(dist) + 1.
+            else:
+                pass
+            evalsorg[i + 1, j] = evals[i + 1, np.argmin(dist)]
+            evecsorg[i + 1, :, j] = evecs[i + 1, :, np.argmin(dist)]
+            # keep track of the indices we've used
+            used.append(np.argmin(dist))
+
+    return evalsorg, evecsorg
+
+
 def sort_modes(evals, evecs):
     '''Sort eigenvalues and eigenvectors into weave, capsize, caster modes.
 
     Parameters
     ----------
     evals : ndarray, shape (n, 4)
         eigenvalues
@@ -230,40 +283,43 @@
     for i, speed in enumerate(evals):
         if i == evals.shape[0] - 1:
             break
         # for each current eigenvalue
         used = []
         for j, e in enumerate(speed):
             try:
-                x, y = np.real(evalsorg[i, j].nominal_value), np.imag(evalsorg[i, j].nominal_value)
+                x = np.real(evalsorg[i, j].nominal_value)
+                y = np.imag(evalsorg[i, j].nominal_value)
             except:
                 x, y = np.real(evalsorg[i, j]), np.imag(evalsorg[i, j])
             # for each eigenvalue at the next speed
             dist = np.zeros(4)
             for k, eignext in enumerate(evals[i + 1]):
                 try:
-                    xn, yn = np.real(eignext.nominal_value), np.imag(eignext.nominal_value)
+                    xn = np.real(eignext.nominal_value)
+                    yn = np.imag(eignext.nominal_value)
                 except:
                     xn, yn = np.real(eignext), np.imag(eignext)
                 # distance between points in the real/imag plane
                 dist[k] = np.abs(((xn - x)**2 + (yn - y)**2)**0.5)
             if np.argmin(dist) in used:
                 # set the already used indice higher
                 dist[np.argmin(dist)] = np.max(dist) + 1.
             else:
                 pass
             evalsorg[i + 1, j] = evals[i + 1, np.argmin(dist)]
             evecsorg[i + 1, :, j] = evecs[i + 1, :, np.argmin(dist)]
             # keep track of the indices we've used
             used.append(np.argmin(dist))
-    weave = {'evals' : evalsorg[:, 2:], 'evecs' : evecsorg[:, :, 2:]}
-    capsize = {'evals' : evalsorg[:, 1], 'evecs' : evecsorg[:, :, 1]}
-    caster = {'evals' : evalsorg[:, 0], 'evecs' : evecsorg[:, :, 0]}
+    weave = {'evals': evalsorg[:, 2:], 'evecs': evecsorg[:, :, 2:]}
+    capsize = {'evals': evalsorg[:, 1], 'evecs': evecsorg[:, :, 1]}
+    caster = {'evals': evalsorg[:, 0], 'evecs': evecsorg[:, :, 0]}
     return weave, capsize, caster
 
+
 def trail(rF, lam, fo):
     '''Calculate the trail and mechanical trail.
 
     Parameters
     ----------
     rF : float
         The front wheel radius
```

### Comparing `BicycleParameters-1.0.0/bicycleparameters/rider.py` & `bicycleparameters-1.1.0/bicycleparameters/rider.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,34 +11,34 @@
 
 
 def yeadon_vec_to_bicycle_vec(vector, measured_bicycle_par,
                               benchmark_bicycle_par):
     """
     Parameters
     ----------
-    vector : np.matrix, shape(3, 1)
+    vector : ndarray, shape(3, 1)
         A vector from the Yeadon origin to a point expressed in the Yeadon
         reference frame.
     measured_bicycle_par : dictionary
         The raw bicycle measurements.
     benchmark_bicycle_par : dictionary
         The Meijaard 2007 et. al parameters for this bicycle.
 
     Returns
     -------
-    vector_wrt_bike : np.matrix, shape(3, 1)
+    vector_wrt_bike : ndarray, shape(3, 1)
         The vector from the bicycle origin to the same point above expressed
         in the bicycle reference frame.
 
     """
 
     # This is the rotation matrix that relates Yeadon's reference frame
     # to the bicycle reference frame.
     # vector_expressed_in_bike = rot_mat * vector_expressed_in_yeadon)
-    rot_mat = np.matrix([[0.0, -1.0, 0.0],
+    rot_mat = np.array([[0.0, -1.0, 0.0],
                         [-1.0, 0.0, 0.0],
                         [0.0, 0.0, -1.0]])
 
     # The relevant bicycle parameters:
     measuredPar = remove_uncertainties(measured_bicycle_par)
     benchmarkPar = remove_uncertainties(benchmark_bicycle_par)
     # bottom bracket height
@@ -52,19 +52,20 @@
     # seat tube length
     lst = measuredPar['lst']
     # seat tube angle
     lambdast = measuredPar['lamst']
 
     # bicycle origin to yeadon origin expressed in bicycle frame
     yeadon_origin_in_bike_frame = \
-        np.matrix([[np.sqrt(lcs**2 - (-hbb + rR)**2) + (-lsp - lst) * np.cos(lambdast)],  # bx
-                   [0.0],
-                   [-hbb + (-lsp - lst) * np.sin(lambdast)]])  # bz
+        np.array([[np.sqrt(lcs**2 - (-hbb + rR)**2) +
+                   (-lsp - lst) * np.cos(lambdast)],  # bx
+                  [0.0],
+                  [-hbb + (-lsp - lst) * np.sin(lambdast)]])  # bz
 
-    vector_wrt_bike =  yeadon_origin_in_bike_frame + rot_mat * vector
+    vector_wrt_bike = yeadon_origin_in_bike_frame + rot_mat @ vector
 
     return vector_wrt_bike
 
 
 def configure_rider(pathToRider, bicycle, bicyclePar, measuredPar, draw):
     """
     Returns the rider parameters, bicycle paramaters with a rider and a
```

### Comparing `BicycleParameters-1.0.0/bicycleparameters/inertia.py` & `bicycleparameters-1.1.0/bicycleparameters/inertia.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from math import pi
 from uncertainties import unumpy, umath, UFloat
 import numpy as np
 
 # local modules
 from .com import total_com
 
+
 def combine_bike_rider(bicyclePar, riderPar):
     """
     Combines the inertia of the bicycle frame with the
     inertia of a rider.
 
     Parameters
     ----------
@@ -58,14 +59,15 @@
     bicyclePar['IBxx'] = I[0, 0]
     bicyclePar['IBxz'] = I[0, 2]
     bicyclePar['IByy'] = I[1, 1]
     bicyclePar['IBzz'] = I[2, 2]
 
     return bicyclePar
 
+
 def compound_pendulum_inertia(m, g, l, T):
     '''Returns the moment of inertia for an object hung as a compound
     pendulum.
 
     Parameters
     ----------
     m : float
@@ -84,14 +86,15 @@
 
     '''
 
     I = (T / 2. / pi)**2. * m * g * l - m * l**2.
 
     return I
 
+
 def inertia_components(jay, beta):
     '''Returns the 2D orthogonal inertia tensor.
 
     When at least three moments of inertia and their axes orientations are
     known relative to a common inertial frame of a planar object, the orthoganl
     moments of inertia relative the frame are computed.
 
@@ -107,18 +110,19 @@
     -------
     eye : ndarray, shape(3,)
         Ixx, Ixz, Izz
 
     '''
     sb = unumpy.sin(beta)
     cb = unumpy.cos(beta)
-    betaMat = unumpy.matrix(np.vstack((cb**2, -2 * sb * cb, sb**2)).T)
+    betaMat = unumpy.array(np.vstack((cb**2, -2 * sb * cb, sb**2)).T)
     eye = np.squeeze(np.asarray(np.dot(betaMat.I, jay)))
     return eye
 
+
 def parallel_axis(Ic, m, d):
     '''Returns the moment of inertia of a body about a different point.
 
     Parameters
     ----------
     Ic : ndarray, shape(3,3)
         The moment of inertia about the center of mass of the body with respect
@@ -140,14 +144,15 @@
     c = d[2]
     dMat = np.zeros((3, 3), dtype=object)
     dMat[0] = np.array([b**2 + c**2, -a * b, -a * c])
     dMat[1] = np.array([-a * b, c**2 + a**2, -b * c])
     dMat[2] = np.array([-a * c, -b * c, a**2 + b**2])
     return Ic + m * dMat
 
+
 def part_inertia_tensor(par, part):
     '''Returns an inertia tensor for a particular part for the benchmark
     parameter set.
 
     Parameters
     ----------
     par : dictionary
@@ -164,34 +169,35 @@
     -----
     Parts G, S, and D are additional parts not included in the published paper
     on the benchmark bicycle, they are only relavant if used. See the
     documentation.
 
     '''
     if isinstance(par['mB'], UFloat):
-        dtype=object
+        dtype = object
     else:
-        dtype='float64'
+        dtype = 'float64'
     I = np.zeros((3, 3), dtype=dtype)
     # front or rear wheel
     if part in 'FRD':
         axes = np.array([['xx', None, None],
                          [None, 'yy', None],
                          [None, None, 'xx']])
     # all other parts
     else:
         axes = np.array([['xx', None, 'xz'],
                          [None, 'yy', None],
                          ['xz', None, 'zz']])
     for i, row in enumerate(axes):
         for j, col in enumerate(row):
-            if col != None:
+            if col is not None:
                 I[i, j] = par['I' + part + col]
     return I
 
+
 def principal_axes(I):
     '''Returns the principal moments of inertia and the orientation.
 
     Parameters
     ----------
     I : ndarray, shape(3,3)
         An inertia tensor.
@@ -206,24 +212,26 @@
     '''
     Ip, C = np.linalg.eig(I)
     indices = np.argsort(Ip)
     Ip = Ip[indices]
     C = C.T[indices]
     return Ip, C
 
+
 def rotate_inertia_tensor(I, angle):
     '''Returns inertia tensor rotated through angle. Only for 2D'''
     ca = umath.cos(angle)
     sa = umath.sin(angle)
-    C    =  np.array([[ca, 0., -sa],
-                      [0., 1., 0.],
-                      [sa, 0., ca]])
-    Irot =  np.dot(C, np.dot(I, C.T))
+    C = np.array([[ca, 0., -sa],
+                  [0., 1., 0.],
+                  [sa, 0., ca]])
+    Irot = np.dot(C, np.dot(I, C.T))
     return Irot
 
+
 def tor_inertia(k, T):
     '''Calculate the moment of inertia for an ideal torsional pendulm
 
     Parameters
     ----------
     k: torsional stiffness
     T: period
@@ -234,14 +242,15 @@
 
     '''
 
     I = k * T**2 / 4. / pi**2
 
     return I
 
+
 def torsional_pendulum_stiffness(I, T):
     '''Calculate the stiffness of a torsional pendulum with a known moment of
     inertia.
 
     Parameters
     ----------
     I : moment of inertia
@@ -251,14 +260,15 @@
     -------
     k : stiffness
 
     '''
     k = 4. * I * pi**2 / T**2
     return k
 
+
 def tube_inertia(l, m, ro, ri):
     '''Calculate the moment of inertia for a tube (or rod) where the x axis is
     aligned with the tube's axis.
 
     Parameters
     ----------
     l : float
```

### Comparing `BicycleParameters-1.0.0/bicycleparameters/io.py` & `bicycleparameters-1.1.0/bicycleparameters/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,34 @@
 
 import re
 import os
 import numpy as np
 from uncertainties import ufloat_fromstr
 from scipy.io import loadmat
 
+
 def filename_to_dict(filename):
     '''Returns a dictionay of values based on the pendulum data file name.
 
     '''
     o = space_out_camel_case(os.path.splitext(filename)[0], output='list')
     # this only accounts for single digit trial numbers
     trial = o[-1][-1]
     o[-1] = o[-1][:-1]
     o.append(trial)
     breakdown = ['bicycle', 'part', 'pendulum', 'angleOrder', 'trial']
     dat = {}
-    for word, val  in zip(breakdown, o):
+    for word, val in zip(breakdown, o):
         dat[word] = val
     return dat
 
+
 def load_parameter_text_file(pathToFile):
-    """
-    Returns a dictionary of float and/or ufloat parameters from a parameter file.
+    """Returns a dictionary of float and/or ufloat parameters from a parameter
+    file.
 
     Parameters
     ----------
     pathToFile : string
         The path to the text file with the parameters listed in the specified
         format.
 
@@ -67,38 +69,40 @@
                 else:
                     values = [float(x) for x in valList]
                 # store in dictionary
                 parameters[equality[0].strip()] = np.mean(values)
 
     return parameters
 
+
 def load_pendulum_mat_file(pathToFile):
     '''Returns a dictionay containing the data from the pendulum data mat file.
 
     '''
     pendDat = {}
     loadmat(pathToFile, mdict=pendDat)
-    #clean up the matlab imports
+    # clean up the matlab imports
     del(pendDat['__globals__'], pendDat['__header__'], pendDat['__version__'])
     for k, v in pendDat.items():
         try:
-            #change to an ascii string
+            # change to an ascii string
             pendDat[k] = v[0].encode('ascii')
         except:
-            #if an array of a single number
+            # if an array of a single number
             if np.shape(v)[0] == 1:
                 pendDat[k] = v[0][0]
-            #else if the notes are empty
+            # else if the notes are empty
             elif np.shape(v)[0] == 0:
                 pendDat[k] = ''
-            #else it is the data which needs to be a one dimensional array
+            # else it is the data which needs to be a one dimensional array
             else:
                 pendDat[k] = v.reshape((len(v),))
     return pendDat
 
+
 def remove_uncertainties(dictionary):
     '''Returns a dictionary with the uncertainties removed.'''
     noUncert = {}
     for k, v in dictionary.items():
         try:
             # this is the case if the value is a single uncertainty
             noUncert[k] = v.nominal_value
@@ -107,14 +111,15 @@
             try:
                 noUncert[k] = [x.nominal_value for x in v]
             except TypeError:
                 # this is the case if the value is a float
                 noUncert[k] = v
     return noUncert
 
+
 def write_parameter_text_file(pathToTxtFile, parDict):
     '''Writes parameter set to file.
 
     Parameters
     ----------
     pathToTxtFile : string
         The path to the file to write the parameters.
@@ -135,17 +140,17 @@
         os.makedirs(head)
 
     try:
         f = open(pathToTxtFile)
         f.close()
         del f
         ans = None
-        while ans !=  'y' and ans != 'n':
-            ans = raw_input("%s exists already. Are you sure you want" \
-                            " to overwrite it? (y or n)\n" % pathToTxtFile)
+        while ans != 'y' and ans != 'n':
+            ans = input("%s exists already. Are you sure you want"
+                        " to overwrite it? (y or n)\n" % pathToTxtFile)
         if ans == 'y':
             f = open(pathToTxtFile, 'w')
     except IOError:
         f = open(pathToTxtFile, 'w')
 
     try:
         f
@@ -155,35 +160,35 @@
         f.close()
         print("Parameters saved to %s" % pathToTxtFile)
         return True
     except UnboundLocalError:
         print("%s was not saved." % pathToTxtFile)
         return False
 
+
 def space_out_camel_case(s, output='string'):
-        """Adds spaces to a camel case string.  Failure to space out string
-        returns the original string.
+    """Adds spaces to a camel case string. Failure to space out string returns
+    the original string.
+
+    Examples
+    --------
+    >>> space_out_camel_case('DMLSServicesOtherBSTextLLC')
+    'DMLS Services Other BS Text LLC'
+    >>> space_out_camel_case('DMLSServicesOtherBSTextLLC', output='list')
+    ['DMLS', 'Services', 'Other', 'BS', 'Text', 'LLC']
+
+    """
+    if output == 'string':
+        return re.sub('((?=[A-Z][a-z])|(?<=[a-z])(?=[A-Z]))', ' ', s).strip()
+    elif output == 'list':
+        string = re.sub('((?=[A-Z][a-z])|(?<=[a-z])(?=[A-Z]))', ' ', s).strip()
+        return string.split(' ')
+    else:
+        raise ValueError
 
-        Examples
-        --------
-        >>> space_out_camel_case('DMLSServicesOtherBSTextLLC')
-        'DMLS Services Other BS Text LLC'
-        >>> space_out_camel_case('DMLSServicesOtherBSTextLLC', output='list')
-        ['DMLS', 'Services', 'Other', 'BS', 'Text', 'LLC']
-
-        """
-        if output == 'string':
-            return re.sub('((?=[A-Z][a-z])|(?<=[a-z])(?=[A-Z]))', ' ',
-                          s).strip()
-        elif output == 'list':
-            string = re.sub('((?=[A-Z][a-z])|(?<=[a-z])(?=[A-Z]))', ' ',
-                            s).strip()
-            return string.split(' ')
-        else:
-            raise ValueError
 
 def write_periods_to_file(pathToRawFile, mp):
     '''Writes the provided periods to file.
 
     Parameters
     ----------
     pathToRawFile : string
```

### Comparing `BicycleParameters-1.0.0/bicycleparameters/geometry.py` & `bicycleparameters-1.1.0/bicycleparameters/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from math import pi
 import numpy as np
 from uncertainties import unumpy, umath
 
 from .bicycle import trail, lambda_from_abc
 
+
 def calculate_benchmark_geometry(mp, par):
     '''Returns the wheelbase, steer axis tilt and the trail.
 
     Parameters
     ----------
     mp : dictionary
         Dictionary with the measured parameters.
@@ -19,19 +20,19 @@
     Returns
     -------
     par : dictionary
         par with the benchmark geometry added.
 
     '''
     # calculate the wheel radii
-    par['rF'] = mp['dF'] / 2./ pi / mp['nF']
-    par['rR'] = mp['dR'] / 2./ pi / mp['nR']
+    par['rF'] = mp['dF'] / 2. / pi / mp['nF']
+    par['rR'] = mp['dR'] / 2. / pi / mp['nR']
 
     # calculate the frame/fork fundamental geometry
-    if 'w' in mp.keys(): # if there is a wheelbase
+    if 'w' in mp.keys():  # if there is a wheelbase
         # steer axis tilt in radians
         par['lam'] = pi / 180. * (90. - mp['gamma'])
         # wheelbase
         par['w'] = mp['w']
         # fork offset
         forkOffset = mp['f']
     else:
@@ -51,14 +52,15 @@
         par['xcl'] = mp['xcl']
         par['zcl'] = mp['zcl']
     except KeyError:
         pass
 
     return par
 
+
 def calculate_abc_geometry(h, d):
     '''Returns the perpendicular distance geometry for the bicycle from the raw
     measurements.
 
     Parameters
     ----------
     h : tuple
@@ -83,17 +85,18 @@
     d1, d2, d3, d4, d = d
     # get the perpendicular distances
     a = h1 + h2 - h3 + .5 * d1 - .5 * d2
     b = h4 - .5 * d3 - h5 + .5 * d4
     c = umath.sqrt(-(a - b)**2 + (d + .5 * (d2 + d3))**2)
     return a, b, c
 
+
 def calculate_l1_l2(h6, h7, d5, d6, l):
-    '''Returns the distance along (l2) and perpendicular (l1) to the steer axis from the
-    front wheel center to the handlebar reference point.
+    '''Returns the distance along (l2) and perpendicular (l1) to the steer axis
+    from the front wheel center to the handlebar reference point.
 
     Parameters
     ----------
     h6 : float
         Distance from the table to the top of the front axle.
     h7 : float
         Distance from the table to the top of the handlebar reference circle.
@@ -122,18 +125,19 @@
     r6 = d6 / 2.
     l1 = h7 - h6 + r5 - r6
     l0 = l - r5 - r6
     gamma = umath.asin(l1 / l0)
     l2 = l0 * umath.cos(gamma)
     return l1, l2
 
+
 def calc_two_link_angles(L1, L2, D):
-    '''Solves a simple case of the two-link revolute joint inverse
-    kinematics problem. Both output angles are positive. The simple case
-    is taht the end of the second link lies on the x-axis.
+    '''Solves a simple case of the two-link revolute joint inverse kinematics
+    problem. Both output angles are positive. The simple case is that the end
+    of the second link lies on the x-axis.
 
     Parameters
     ----------
     L1 : float
         Length of the first link.
     L2 : float
         Length of the second link.
@@ -145,19 +149,20 @@
     theta1 : float
         (radians) Angle between x-axis and first link; always positive.
     theta2 : float
         (radians) Angle between first link and second link; always positive.
 
     '''
 
-    theta1 = np.arccos( (L1**2 + D**2 - L2**2) / (2.0 * L1 * D) )
-    theta2 = theta1 + np.arcsin( L1 / L2 * np.sin( theta1 ) )
+    theta1 = np.arccos((L1**2 + D**2 - L2**2) / (2.0 * L1 * D))
+    theta2 = theta1 + np.arcsin(L1 / L2 * np.sin(theta1))
 
     return theta1, theta2
 
+
 def fwheel_to_handlebar_ref(lam, l1, l2):
     '''Returns the distance along the benchmark coordinates from the front
     wheel center to the handlebar reference center.
 
     Parameters
     ----------
     lam : float
@@ -172,14 +177,15 @@
 
     '''
 
     u1 = l2 * umath.sin(lam) - l1 * umath.cos(lam)
     u2 = u1 / umath.tan(lam) + l1 / umath.sin(lam)
     return u1, u2
 
+
 def fundamental_geometry_plot_data(par):
     '''Returns the coordinates for line end points of the bicycle fundamental
     geometry.
 
     Parameters
     ----------
     par : dictionary
@@ -187,31 +193,31 @@
 
     Returns
     -------
     x : ndarray
     z : ndarray
 
     '''
-    d1 = np.cos(par['lam']) * (par['c'] + par['w'] -
-                par['rR'] * np.tan(par['lam']))
-    d3 = -np.cos(par['lam']) * (par['c'] - par['rF'] *
-                np.tan(par['lam']))
+    d1 = np.cos(par['lam']) * (par['c'] + par['w'] - par['rR'] *
+                               np.tan(par['lam']))
+    d3 = -np.cos(par['lam']) * (par['c'] - par['rF'] * np.tan(par['lam']))
     x = np.zeros(4, dtype=object)
     z = np.zeros(4, dtype=object)
     x[0] = 0.
     x[1] = d1 * np.cos(par['lam'])
     x[2] = par['w'] - d3 * np.cos(par['lam'])
     x[3] = par['w']
     z[0] = -par['rR']
     z[1] = -par['rR'] - d1 * np.sin(par['lam'])
     z[2] = -par['rF'] + d3 * np.sin(par['lam'])
     z[3] = -par['rF']
 
     return x, z
 
+
 def distance_to_steer_axis(w, c, lam, point):
     """Returns the minimal distance from the steer axis to the given point when
     the bicycle is in the nominal configuration.
 
     Parameters
     ----------
     w : float or ufloat
@@ -228,23 +234,22 @@
     d : float or ufloat
         The minimal distance from the given point to the steer axis.
 
     """
     pointOnAxis1 = np.array([w + c,
                              0.,
                              0.])
-    pointOnAxis2 = pointOnAxis1 +\
-                   np.array([-umath.sin(lam),
-                             0.,
-                             -umath.cos(lam)])
+    pointOnAxis2 = (pointOnAxis1 + np.array([-umath.sin(lam), 0.,
+                                             -umath.cos(lam)]))
     pointsOnLine = np.array([pointOnAxis1, pointOnAxis2]).T
 
     # this is the distance from the assembly com to the steer axis
     return point_to_line_distance(point, pointsOnLine)
 
+
 def point_to_line_distance(point, pointsOnLine):
     '''Returns the minimal distance from a point to a line in three
     dimensional space.
 
     Parameters
     ----------
     point : ndarray, shape(3,)
@@ -266,14 +271,15 @@
     def norm(v):
         return unumpy.sqrt(np.dot(v, v))
 
     distance = norm(np.cross((x0 - x1), (x0 - x2))) / norm(x2 - x1)
 
     return distance
 
+
 def project_point_on_line(line, point):
     '''Returns point of projection.
 
     Parameters
     ----------
     line : tuple
         Slope and intercept of the line.
@@ -283,36 +289,39 @@
     Returns
     -------
     newPoint : tuple
         The location of the projected point.
 
     '''
     m, b = line
-    c , d = point
+    c, d = point
     x = (m * d + c - m * b) / (m**2. + 1.)
     y = (m**2. * d + m * c + b) / (m**2. + 1.)
     return x, y
 
-def vec_angle(v1,v2):
-    '''Returns the interior angle between two vectors using the dot product. Inputs do not need to be unit vectors.
+
+def vec_angle(v1, v2):
+    '''Returns the interior angle between two vectors using the dot product.
+    Inputs do not need to be unit vectors.
 
     Parameters
     ----------
     v1 : np.array (3,1)
         input vector.
     v2 : np.array (3,1)
         input vector.
 
     Returns
     -------
     angle : float
         (radians) interior angle between v1 and v2.
     '''
-    return np.arccos( float(np.dot(v1.T,v2)) / (
-           np.linalg.norm(v1) * np.linalg.norm(v2) ) )
+    return np.arccos(float(np.dot(v1.T, v2)) / (np.linalg.norm(v1) *
+                                                np.linalg.norm(v2)))
+
 
 def vec_project(vec, direction):
     '''Vector projection into a plane, where the plane is defined by a
     normal vector.
 
     Parameters
     ----------
```

### Comparing `BicycleParameters-1.0.0/bicycleparameters/period.py` & `bicycleparameters-1.1.0/bicycleparameters/period.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from scipy.optimize import leastsq
 import matplotlib.pyplot as plt
 from uncertainties import ufloat
 
 # local modules
 from .io import load_pendulum_mat_file
 
+
 def average_rectified_sections(data):
     '''Returns a slice of an oscillating data vector based on the max and min
     of the mean of the sections created by retifiying the data.
 
     Parameters
     ----------
     data : ndarray, shape(n,)
@@ -59,14 +60,15 @@
             indice.append(meanInd[i])
     # now return the data based on the max value and the min value
     maxInd = indice[np.argmax(secMeanOverThresh)]
     minInd = indice[np.argmin(secMeanOverThresh)]
 
     return data[maxInd:minInd]
 
+
 def calc_periods_for_files(directory, filenames, forkIsSplit):
     '''Calculates the period for all filenames in directory.
 
     Parameters
     ----------
     directory : string
         This is the path to the RawData directory.
@@ -85,15 +87,15 @@
 
     periods = {}
 
     def pathParts(path):
         '''Splits a path into a list of its parts.'''
         components = []
         while True:
-            (path,tail) = os.path.split(path)
+            (path, tail) = os.path.split(path)
             if tail == "":
                 components.reverse()
                 return components
             components.append(tail)
 
     pathToRawDataParts = pathParts(directory)
     pathToRawDataParts.pop()
@@ -131,14 +133,15 @@
     # now average all the periods
     for k, v in periods.items():
         if k.startswith('T'):
             periods[k] = np.mean(v)
 
     return periods
 
+
 def check_for_period(mp, forkIsSplit):
     '''Returns whether the fork is split into two pieces and whether the period
     calculations need to happen again.
 
     Parameters
     ----------
     mp : dictionary
@@ -153,15 +156,15 @@
         True if there wasn't enough period data in mp, false if there was.
     forkIsSplit : boolean
         True if the fork is broken into a handlebar and fork and false if the
         fork and handlebar was measured together.
 
     '''
     forcePeriodCalc = False
-    #Check to see if mp contains at enough periods to not need
+    # Check to see if mp contains at enough periods to not need
     # recalculation
     ncTSum = 0
     ntTSum = 0
     for key in mp.keys():
         # check for any periods in the keys
         if key[:2] == 'Tc':
             ncTSum += 1
@@ -174,14 +177,15 @@
             forcePeriodCalc = True
     else:
         if ncTSum < 4 or ntTSum < 8:
             forcePeriodCalc = True
 
     return forcePeriodCalc
 
+
 def fit_goodness(ym, yp):
     '''
     Calculate the goodness of fit.
 
     Parameters
     ----------
     ym : ndarray, shape(n,)
@@ -203,14 +207,15 @@
     '''
     SSR = np.sum((yp - np.mean(ym))**2)
     SST = np.sum((ym - np.mean(ym))**2)
     SSE = SST - SSR
     rsq = SSR / SST
     return rsq, SSE, SST, SSR
 
+
 def get_period(data, sampleRate, pathToPlotFile):
     '''Returns the period and uncertainty for data resembling a decaying
     oscillation.
 
     Parameters
     ----------
     data : ndarray, shape(n,)
@@ -235,17 +240,17 @@
         a = p[0]
         b = np.exp(-p[3] * p[4] * t)
         c = p[1] * np.sin(p[4] * np.sqrt(1 - p[3]**2) * t)
         d = p[2] * np.cos(p[4] * np.sqrt(1 - p[3]**2) * t)
         return a + b * (c + d)
 
     # initial guesses
-    #p0 = np.array([1.35, -.5, -.75, 0.01, 3.93]) # guess from delft
-    #p0 = np.array([2.5, -.75, -.75, 0.001, 4.3]) # guess from ucd
-    p0 = make_guess(data, sampleRate) # tries to make a good guess
+    # p0 = np.array([1.35, -.5, -.75, 0.01, 3.93]) # guess from delft
+    # p0 = np.array([2.5, -.75, -.75, 0.001, 4.3]) # guess from ucd
+    p0 = make_guess(data, sampleRate)  # tries to make a good guess
 
     # create the error function
     errfunc = lambda p, t, y: fitfunc(p, t) - y
 
     # minimize the error function
     p1, success = leastsq(errfunc, p0[:], args=(x, y))
 
@@ -283,20 +288,22 @@
     plot_osfit(x, y, lscurve, p1, rsq, T, m=np.max(x), fig=fig)
     plt.savefig(pathToPlotFile)
     plt.close()
 
     # return the period
     return T
 
+
 def get_period_from_truncated(data, sampleRate, pathToPlotFile):
-    #dataRec = average_rectified_sections(data)
+    # dataRec = average_rectified_sections(data)
     dataRec = data
     dataGood = select_good_data(dataRec, 0.1)
     return get_period(dataGood, sampleRate, pathToPlotFile)
 
+
 def get_period_key(matData, forkIsSplit):
     '''Returns a dictionary key for the period entries.
 
     Parameters
     ----------
     matData : dictionary
         The data imported from a pendulum mat file.
@@ -328,37 +335,39 @@
         subscripts['Fork'] = 'H'
     try:
         subscripts[matData['rod']] = 'P'
     except KeyError:
         subscripts['Rod'] = 'P'
 
     # used to convert word ordinals to numbers
-    ordinal = {'First' : '1',
-               'Second' : '2',
-               'Third' : '3',
-               'Fourth' : '4',
-               'Fifth' : '5',
-               'Sixth' : '6'}
+    ordinal = {'First': '1',
+               'Second': '2',
+               'Third': '3',
+               'Fourth': '4',
+               'Fifth': '5',
+               'Sixth': '6'}
     try:
         orienWord = matData['angleOrder']
     except:
         orienWord = matData['angle']
     pend = matData['pendulum'][0].lower()
     part = subscripts[matData['part']]
     orienNum = ordinal[orienWord]
     return 'T' + pend + part + orienNum
 
+
 def get_sample_rate(matData):
     '''Returns the sample rate for the data.'''
     if 'ActualRate' in matData.keys():
         sampleRate = matData['ActualRate']
     else:
         sampleRate = matData['sampleRate']
     return sampleRate
 
+
 def jac_fitfunc(p, t):
     '''
     Calculate the Jacobian of a decaying oscillation function.
 
     Uses the analytical formulations of the partial derivatives.
 
     Parameters
@@ -382,14 +391,15 @@
     jac[2] = e * c
     jac[3] = (-p[4] * t * e * (p[1] * s + p[2] * c) + e * (-p[1] * p[3] * p[4]
               * t / dampsq * c + p[2] * p[3] * p[4] * t / dampsq * s))
     jac[4] = (-p[3] * t * e * (p[1] * s + p[2] * c) + e * dampsq * t * (p[1] *
               c - p[2] * s))
     return jac.T
 
+
 def make_guess(data, sampleRate):
     '''Returns a decent starting point for fitting the decaying oscillation
     function.
 
     '''
     p = np.zeros(5)
 
@@ -407,15 +417,16 @@
 
     # the second is the amplitude for the sin function
     p[1] = slope * np.max(data) / 2
 
     # the third is the amplitude for the cos function
     p[2] = slope * np.max(data)
 
-    # the fourth is the damping ratio and is typically small, 0.001 < zeta < 0.02
+    # the fourth is the damping ratio and is typically small, 0.001 < zeta <
+    # 0.02
     p[3] = 0.001
 
     # the fifth is the undamped natural frequency
     # first remove the data around zero
     dataMasked = ma.masked_inside(data, -0.1, 0.1)
     # find the zero crossings
     zeroCrossings = np.where(np.diff(np.sign(dataMasked)))[0]
@@ -423,20 +434,21 @@
     zero = []
     for i, v in enumerate(zeroCrossings):
         if abs(v - zeroCrossings[i - 1]) > 20:
             zero.append(v)
     # get the samples per period
     samplesPerPeriod = 2*np.mean(np.diff(zero))
     # now the frequency
-    p[4] = (samplesPerPeriod / float(sampleRate) /2. / pi)**-1
+    p[4] = (samplesPerPeriod / float(sampleRate) / 2. / pi)**-1
     if np.isnan(p[4]):
         p[4] = 4.
 
     return p
 
+
 def plot_osfit(t, ym, yf, p, rsq, T, m=None, fig=None):
     '''Plot fitted data over the measured
 
     Parameters
     ----------
     t : ndarray (n,)
         Measurement time in seconds
@@ -454,15 +466,15 @@
 
     Returns
     -------
     fig : the figure
 
     '''
     # figure properties
-    figwidth = 4. # in inches
+    figwidth = 4.  # in inches
     goldenMean = (np.sqrt(5) - 1.0) / 2.0
     figsize = [figwidth, figwidth * goldenMean]
     params = {#'backend': 'ps',
         'axes.labelsize': 8,
         'axes.titlesize': 8,
         'text.fontsize': 8,
         'legend.fontsize': 8,
@@ -493,14 +505,15 @@
     plt.legend(['Measured', 'Fit'])
     if m is not None:
         plt.xlim((0, m))
     else:
         pass
     return fig
 
+
 def select_good_data(data, percent):
 
     '''Returns a slice of the data from the index at maximum value to the index
     at a percent of the maximum value.
 
     Parameters
     ----------
```

### Comparing `BicycleParameters-1.0.0/bicycleparameters/main.py` & `bicycleparameters-1.1.0/bicycleparameters/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,73 @@
 #!/usr/bin/env python
 
 # builtin modules
 import os
 
 # dependencies
-import numpy as np
-import matplotlib.pyplot as plt
+from dtk import control
 from matplotlib.patches import Ellipse, Wedge
 from uncertainties import unumpy
-from dtk import control
+import matplotlib.pyplot as plt
+import numpy as np
+
+try:
+    import plotly
+except ImportError:
+    px = None
+    go = None
+else:
+    del plotly
+    import plotly.express as px
+    import plotly.graph_objects as go
 
 # local module imports
 from . import bicycle
 from . import inertia
 from . import com
 from . import io
 from . import geometry
 from . import period
 from . import rider
-#from plot import plot_eigenvalues
+from . import plot
+
+GOLDEN_RATIO = (1.0 + np.sqrt(5.0))/2.0
+
 
 class Bicycle(object):
     """
     An object for a bicycle. A bicycle has parameters and can have a rider
     attached to it. That's about it for now.
 
     """
 
     def __new__(cls, bicycleName, pathToData='.', forceRawCalc=False,
-            forcePeriodCalc=False):
-        '''Returns a NoneType object if there is no directory for the bicycle.'''
+                forcePeriodCalc=False):
+        '''Returns a NoneType object if there is no directory for the
+        bicycle.'''
         # is there a data directory for this bicycle? if not, tell the user to
         # put some data in the folder so we have something to work with!
         try:
             pathToBicycle = os.path.join(pathToData, 'bicycles', bicycleName)
-            if os.path.isdir(pathToBicycle) == True:
+            if os.path.isdir(pathToBicycle):
                 print("We have foundeth a directory named: " +
                       "{0}.".format(pathToBicycle))
                 return super(Bicycle, cls).__new__(cls)
             else:
                 raise ValueError
         except:
-            mes = """Are you nuts?! Make a directory called '{0}' with basic data
-for your bicycle in this directory: '{1}'. Then I can actually
-create a bicycle object. You may either need to change to the
-correct directory or reset the pathToData argument.""".format(bicycleName, pathToData)
+            mes = """Are you nuts?! Make a directory called '{0}' with basic
+data for your bicycle in this directory: '{1}'. Then I can actually create a
+bicycle object. You may either need to change to the correct directory or reset
+the pathToData argument.""".format(bicycleName, pathToData)
             print(mes)
             return None
 
     def __init__(self, bicycleName, pathToData='.', forceRawCalc=False,
-            forcePeriodCalc=False):
+                 forcePeriodCalc=False):
         """
         Creates a bicycle object and sets the parameters based on the available
         data.
 
         Parameters
         ----------
         bicycleName : string
@@ -62,17 +76,17 @@
             should have a matching directory under `<pathToData>/bicycles/`.
             For example: `<pathToData>/bicycles/Shortname`.
         pathToData : string
             This is the path to the folder where the bicycle/rider parameters
             and raw data are stored. The default is the current working
             directory.
         forceRawCalc : boolean
-            Forces a recalculation of the benchmark parameters from the measured
-            parameters. Otherwise it will only run the calculation if there is
-            no benchmark parameter file.
+            Forces a recalculation of the benchmark parameters from the
+            measured parameters. Otherwise it will only run the calculation if
+            there is no benchmark parameter file.
         forcePeriodCalc : boolean
             Forces a recalculation of the periods from the oscillation data.
 
         Notes
         -----
         Bicycles are assumed not to have a rider when initially loaded.
 
@@ -96,29 +110,31 @@
             for parFile in parFiles:
                 # remove the extension
                 fname = os.path.splitext(parFile)[0]
                 # get the bike and the parameter set type
                 bike, ptype = io.space_out_camel_case(fname, output='list')
                 # load the parameters
                 pathToFile = os.path.join(parDir, parFile)
-                self.parameters[ptype] = io.load_parameter_text_file(pathToFile)
+                self.parameters[ptype] = io.load_parameter_text_file(
+                    pathToFile)
 
         # this is where the raw data files from the pendulum oscillations are
         # stored
         rawDataDir = os.path.join(self.directory, 'RawData')
 
         # it would be more robust to see if there are enough files in the
         # RawData directory, but that isn't implemented yet. For now you'll
         # just get and error sometime down the road when a period for the
         # missing files is needed.
         isRawDataDir = 'RawData' in os.listdir(self.directory)
 
         if isRawDataDir:
             print("Found the RawData directory:", rawDataDir)
-            isMeasuredFile = bicycleName + 'Measured.txt' in os.listdir(rawDataDir)
+            fname = bicycleName + 'Measured.txt'
+            isMeasuredFile = fname in os.listdir(rawDataDir)
         else:
             isMeasuredFile = False
 
         isBenchmark = 'Benchmark' in self.parameters.keys()
 
         # the user wants to force a recalc and the data is there
         conOne = forceRawCalc and isRawDataDir and isMeasuredFile
@@ -136,43 +152,43 @@
                   % self.bicycleName)
         elif not forceRawCalc and isBenchmark:
             # we already have what we need
             stmt1 = "Looks like you've already got some parameters for %s, "
             stmt2 = "use forceRawCalc to recalculate."
             print((stmt1 + stmt2) % self.bicycleName)
             # load the measured.txt file if it exists
-            pathToRawFile = os.path.join(rawDataDir,
-                    self.bicycleName + 'Measured.txt')
+            pathToRawFile = os.path.join(rawDataDir, self.bicycleName +
+                                         'Measured.txt')
             try:
                 self.parameters['Measured'] = \
                         io.load_parameter_text_file(pathToRawFile)
             except IOError:
                 pass
         else:
             print('''There is no data available. Create
             bicycles/{sn}/Parameters/{sn}Benchmark.txt and/or fill
             bicycle/{sn}/RawData/ with pendulum data mat files and the
             {sn}Measured.txt file'''.format(sn=bicycleName))
 
     def __str__(self):
         if self.hasRider:
             desc = "{0} with {1} on board.".format(self.bicycleName,
-                self.riderName)
+                                                   self.riderName)
         else:
             desc = "{0} with no one on board.".format(self.bicycleName)
         return desc
 
     def save_parameters(self, filetype='text'):
-        """
-        Saves all the parameter sets to file.
+        """Saves all the parameter sets to file.
 
         Parameters
-        ----------
+        ==========
+
         filetype : string, optional
-            - 'text' : a text file with parameters as `c = 0.10+/-0.01\n`
+            - 'text' : a text file with parameters as ``c = 0.10+/-0.01``
             - 'matlab' : matlab .mat file
             - 'pickle' : python pickled dictionary
 
         """
         if self.hasRider:
             pathToData = os.path.split(os.path.split(self.directory)[0])[0]
             pathToParDir = os.path.join(pathToData, 'riders', self.riderName,
@@ -199,15 +215,15 @@
             for pset in psets:
                 fileName = fileName + pset + '.txt'
                 pathToTxtFile = os.path.join(pathToParDir, fileName)
                 io.write_parameter_text_file(pathToTxtFile, parameters[pset])
                 if self.hasRider:
                     pathToCombFile = os.path.join(pathToCombDir, fileName)
                     io.write_parameter_text_file(pathToCombFile,
-                                              self.parameters[pset])
+                                                 self.parameters[pset])
 
         elif filetype == 'matlab':
             # this should handle the uncertainties properly
             raise NotImplementedError("Doesn't work yet.")
 
         elif filetype == 'pickle':
             raise NotImplementedError("Doesn't work yet.")
@@ -224,18 +240,19 @@
         try:
             if os.path.isdir(photoDir):
                 os.system('eog ' + os.path.join(photoDir, '*.*'))
             else:
                 print("There are no photos of your bicycle.")
         except:
             raise NotImplementedError("This works only works for linux with " +
-                    "Eye of Gnome installed.")
+                                      "Eye of Gnome installed.")
 
     def steer_assembly_moment_of_inertia(self, handlebar=True, fork=True,
-            wheel=True, aboutSteerAxis=False, nominal=False):
+                                         wheel=True, aboutSteerAxis=False,
+                                         nominal=False):
         """
         Returns the inertia tensor of the steer assembly with respect to a
         reference frame aligned with the steer axis.
 
         Parameters
         ----------
         handlebar : boolean, optional
@@ -268,16 +285,16 @@
 
         """
         # load in the Benchmark parameter set
         par = self.parameters['Benchmark']
 
         if 'mD' in par.keys():
             print("You have a flywheel defined. Beware that it is ignored in "
-                + "the calculations and the results do not reflect that it is "
-                + "there.")
+                  "the calculations and the results do not reflect that it is "
+                  "there.")
 
         # there should always be either an H (handlebar/fork) and sometimes
         # there is a G (handlebar) and S (fork) if the fork and handlebar were
         # measured separately
         try:
             if fork and handlebar:
                 # handlebar/fork
@@ -336,64 +353,69 @@
                            -par['rF'] - cAss[2]])
 
             # this is the inertia of the assembly about the com with reference
             # to the benchmark bicycle reference frame
             iAss = (inertia.parallel_axis(I, m, d) +
                     inertia.parallel_axis(IF, par['mF'], dF))
 
-            # this is the inertia of the assembly about a reference frame aligned with
-            # the steer axis and through the center of mass
+            # this is the inertia of the assembly about a reference frame
+            # aligned with the steer axis and through the center of mass
             iAssRot = inertia.rotate_inertia_tensor(iAss, par['lam'])
 
-        else: # don't add the wheel
+        else:  # don't add the wheel
             mAss = m
             cAss = np.array([x, 0., z])
             iAssRot = inertia.rotate_inertia_tensor(I, par['lam'])
 
         if aboutSteerAxis:
             # this is the distance from the assembly com to the steer axis
             distance = geometry.distance_to_steer_axis(par['w'], par['c'],
-                    par['lam'], cAss)
+                                                       par['lam'], cAss)
             print("handlebar cg distance", distance)
 
-            # now calculate the inertia about the steer axis of the rotated frame
-            iAss = inertia.parallel_axis(iAssRot, mAss, np.array([distance, 0., 0.]))
+            # now calculate the inertia about the steer axis of the rotated
+            # frame
+            iAss = inertia.parallel_axis(iAssRot, mAss,
+                                         np.array([distance, 0., 0.]))
         else:
             iAss = iAssRot
 
         if nominal:
             return unumpy.nominal_values(iAss)
         else:
             return iAss
 
     def calculate_from_measured(self, forcePeriodCalc=False):
         '''Calculates the parameters from measured data.'''
 
         rawDataDir = os.path.join(self.directory, 'RawData')
-        pathToRawFile = os.path.join(rawDataDir, self.bicycleName + 'Measured.txt')
+        pathToRawFile = os.path.join(rawDataDir,
+                                     self.bicycleName + 'Measured.txt')
 
         # load the measured parameters
-        self.parameters['Measured'] = io.load_parameter_text_file(pathToRawFile)
+        self.parameters['Measured'] = io.load_parameter_text_file(
+            pathToRawFile)
 
         forkIsSplit = is_fork_split(self.parameters['Measured'])
 
         # if the the user doesn't specifiy to force period calculation, then
         # see if enough data is actually available in the *Measured.txt file to
         # do the calculations
         if not forcePeriodCalc:
-            forcePeriodCalc = period.check_for_period(self.parameters['Measured'],
-                                               forkIsSplit)
+            forcePeriodCalc = period.check_for_period(
+                self.parameters['Measured'], forkIsSplit)
 
-        if forcePeriodCalc == True:
+        if forcePeriodCalc:
             # get the list of mat files associated with this bike
             matFiles = [x for x in os.listdir(rawDataDir)
                         if x.endswith('.mat')]
             matFiles.sort()
             # calculate the period for each file for this bicycle
-            periods = period.calc_periods_for_files(rawDataDir, matFiles, forkIsSplit)
+            periods = period.calc_periods_for_files(rawDataDir, matFiles,
+                                                    forkIsSplit)
             # add the periods to the measured parameters
             self.parameters['Measured'].update(periods)
 
             io.write_periods_to_file(pathToRawFile, periods)
 
         return calculate_benchmark_from_measured(self.parameters['Measured'])
 
@@ -412,100 +434,121 @@
             If true, visual python will be used to draw a three dimensional
             image of the rider.
 
         """
 
         # can't draw the rider model without the human object
         if draw:
-            reCalc=True
+            reCalc = True
 
         # first check to see if a rider has already been added
-        if self.hasRider == True:
+        if self.hasRider:
             print(("D'oh! This bicycle already has {0} as a " +
                   "rider!").format(self.riderName))
         else:
             print("There is no rider on the bicycle, now adding " +
                   "{0}.".format(riderName))
             pathToData = os.path.split(os.path.split(self.directory)[0])[0]
             # get the path to the rider's folder
             pathToRider = os.path.join(pathToData, 'riders', riderName)
             # load in the parameters
             bicyclePar = self.parameters['Benchmark']
             bicycleName = self.bicycleName
 
-            if reCalc == True:
+            if reCalc:
                 print("Calculating the human configuration.")
                 # run the calculations
                 try:
                     measuredPar = self.parameters['Measured']
                 except KeyError:
                     print('The measured bicycle parameters need to be ' +
                           'available, create your bicycle such that they ' +
                           'are available.')
                     raise
                 riderPar, human, bicycleRiderPar =\
                     rider.configure_rider(pathToRider, bicycleName, bicyclePar,
-                            measuredPar, draw)
+                                          measuredPar, draw)
             else:
                 pathToParFile = os.path.join(pathToRider, 'Parameters',
-                    riderName + self.bicycleName + 'Benchmark.txt')
+                                             riderName + self.bicycleName +
+                                             'Benchmark.txt')
                 try:
                     # load the parameter file
                     riderPar = io.load_parameter_text_file(pathToParFile)
                 except IOError:
                     # file doesn't exist so run the calculations
                     print("No parameter files found, calculating the human " +
                           "configuration.")
                     try:
                         measuredPar = self.parameters['Measured']
                     except KeyError:
-                        print('The measured bicycle parameters need to be ' +
-                              'available, create your bicycle such that they ' +
+                        print('The measured bicycle parameters need to be '
+                              'available, create your bicycle such that they '
                               'are available.')
                         raise
                     riderPar, human, bicycleRiderPar =\
                         rider.configure_rider(pathToRider, bicycleName,
-                                bicyclePar, measuredPar, draw)
+                                              bicyclePar, measuredPar, draw)
                 else:
                     print("Loaded the precalculated parameters from " +
                           "{0}".format(pathToParFile))
-                    bicycleRiderPar = inertia.combine_bike_rider(bicyclePar, riderPar)
+                    bicycleRiderPar = inertia.combine_bike_rider(bicyclePar,
+                                                                 riderPar)
             # set the attributes
             self.riderPar['Benchmark'] = riderPar
             try:
                 self.human = human
             except NameError:
                 self.human = None
             self.parameters['Benchmark'] = bicycleRiderPar
             self.riderName = riderName
             self.hasRider = True
 
     def plot_bicycle_geometry(self, show=True, pendulum=True,
                               centerOfMass=True, inertiaEllipse=True):
-        '''Returns a figure showing the basic bicycle geometry, the centers of
+        """Returns a figure showing the basic bicycle geometry, the centers of
         mass and the moments of inertia.
 
+        Parameters
+        ==========
+        show : boolean, optional
+            If true ``matplotlib.pyplot.show()`` will be called before exiting
+            the function.
+        pendulum : boolean, optional
+            If true the axes of the torsional pendulum will be displayed (only
+            useful if raw measurement data is availabe).
+        centerOfMass : boolean, optional
+            If true the mass center of each rigid body will be displayed.
+        inertiaEllipse : boolean optional
+            If true inertia ellipses for each rigid body will be displayed.
+
+        Returns
+        =======
+        fig : matplotlib.pyplot.Figure
+
         Notes
-        -----
+        =====
         If the flywheel is defined, it's center of mass corresponds to the
         front wheel and is not depicted in the plot.
 
-        '''
+        """
         par = io.remove_uncertainties(self.parameters['Benchmark'])
         parts = get_parts_in_parameters(par)
 
         try:
             slopes = io.remove_uncertainties(self.extras['slopes'])
             intercepts = io.remove_uncertainties(self.extras['intercepts'])
-            penInertias = io.remove_uncertainties(self.extras['pendulumInertias'])
+            penInertias = io.remove_uncertainties(
+                self.extras['pendulumInertias'])
         except AttributeError:
             pendulum = False
 
-        fig = plt.figure()
-        ax = plt.axes()
+        fig, ax = plt.subplots()
+
+        fig.set_size_inches([4.0*GOLDEN_RATIO, 4.0])
 
         # define some colors for the parts
         numColors = len(parts)
         cmap = plt.get_cmap('gist_rainbow')
         partColors = {}
         for i, part in enumerate(parts):
             partColors[part] = cmap(1. * i / numColors)
@@ -527,15 +570,15 @@
                     if np.abs(np.sum(row - uy)) < 1E-10:
                         yrow = i
                 # remove the row for the y vector
                 Ip2D = np.delete(Ip, yrow, 0)
                 # remove the column and row associated with the y
                 C2D = np.delete(np.delete(C, yrow, 0), 1, 1)
                 # make an ellipse
-                Imin =  Ip2D[0]
+                Imin = Ip2D[0]
                 Imax = Ip2D[1]
                 # get width and height of a ellipse with the major axis equal
                 # to one
                 unitWidth = 1. / 2. / np.sqrt(Imin) * np.sqrt(Imin)
                 unitHeight = 1. / 2. / np.sqrt(Imax) * np.sqrt(Imin)
                 # now scaled the width and height relative to the maximum
                 # principal moment of inertia
@@ -546,54 +589,55 @@
                                   angle=angle, fill=False,
                                   color=partColors[part], alpha=0.25)
                 ax.add_patch(ellipse)
 
         # plot the ground line
         x = np.array([-par['rR'],
                       par['w'] + par['rF']])
-        plt.plot(x, np.zeros_like(x), 'k')
+        ax.plot(x, np.zeros_like(x), 'k')
 
         # plot the rear wheel
         c = plt.Circle((0., par['rR']), radius=par['rR'], fill=False)
         ax.add_patch(c)
 
         # plot the front wheel
         c = plt.Circle((par['w'], par['rF']), radius=par['rF'], fill=False)
         ax.add_patch(c)
 
         # plot the fundamental bike
         deex, deez = geometry.fundamental_geometry_plot_data(par)
-        plt.plot(deex, -deez, 'k')
+        ax.plot(deex, -deez, 'k')
 
         # plot the steer axis
         dx3 = deex[2] + deez[2] * (deex[2] - deex[1]) / (deez[1] - deez[2])
-        plt.plot([deex[2], dx3],  [-deez[2], 0.], 'k--')
+        ax.plot([deex[2], dx3],  [-deez[2], 0.], 'k--')
 
         # don't plot the pendulum lines if a rider has been added because the
         # inertia has changed
         if self.hasRider:
             pendulum = False
 
         if pendulum:
             # plot the pendulum axes for the measured parts
             for j, pair in enumerate(slopes.items()):
                 part, slopeSet = pair
                 xcom, zcom = par['x' + part], par['z' + part]
                 for i, m in enumerate(slopeSet):
                     b = intercepts[part][i]
                     xPoint, zPoint = geometry.project_point_on_line((m, b),
-                            (xcom, zcom))
+                                                                    (xcom,
+                                                                     zcom))
                     comLineLength = penInertias[part][i]
                     xPlus = comLineLength / 2. * np.cos(np.arctan(m))
                     x = np.array([xPoint - xPlus,
                                   xPoint + xPlus])
                     z = -m * x - b
-                    plt.plot(x, z, color=partColors[part])
+                    ax.plot(x, z, color=partColors[part])
                     # label the pendulum lines with a number
-                    plt.text(x[0], z[0], str(i + 1))
+                    ax.text(x[0], z[0], str(i + 1))
 
         if centerOfMass:
             # plot the center of mass location
             def com_symbol(ax, center, radius, color='b'):
                 '''Returns axis with center of mass symbol.'''
                 c = plt.Circle(center, radius=radius, fill=False)
                 w1 = Wedge(center, radius, 0., 90.,
@@ -606,76 +650,401 @@
                 return ax
 
             # radius of the CoM symbol
             sRad = 0.03
             # front wheel CoM
             ax = com_symbol(ax, (par['w'], par['rF']), sRad,
                             color=partColors['F'])
-            plt.text(par['w'] + sRad, par['rF'] + sRad, 'F')
+            ax.text(par['w'] + sRad, par['rF'] + sRad, 'F')
             # rear wheel CoM
             ax = com_symbol(ax, (0., par['rR']), sRad,
                             color=partColors['R'])
-            plt.text(0. + sRad, par['rR'] + sRad, 'R')
+            ax.text(0. + sRad, par['rR'] + sRad, 'R')
             for j, part in enumerate([x for x in parts
                                       if x not in 'RFD']):
                 xcom = par['x' + part]
                 zcom = par['z' + part]
                 ax = com_symbol(ax, (xcom, -zcom), sRad,
                                 color=partColors[part])
-                plt.text(xcom + sRad, -zcom + sRad, part)
+                ax.text(xcom + sRad, -zcom + sRad, part)
             if 'H' not in parts:
                 ax = com_symbol(ax, (par['xH'], -par['zH']), sRad)
-                plt.text(par['xH'] + sRad, -par['zH'] + sRad, 'H')
-
-
-        plt.axis('equal')
-        plt.ylim((0., 1.))
-        plt.title(self.bicycleName)
+                ax.text(par['xH'] + sRad, -par['zH'] + sRad, 'H')
 
         # if there is a rider on the bike, make a simple stick figure
+        top_of_head = 0.0
         if self.human:
             human = self.human
             mpar = self.parameters['Measured']
             bpar = self.parameters['Benchmark']
             # K2: lower leg, tip of foot to knee
-            start = rider.yeadon_vec_to_bicycle_vec(human.K2.end_pos, mpar, bpar)
+            start = rider.yeadon_vec_to_bicycle_vec(human.K2.end_pos, mpar,
+                                                    bpar)
             end = rider.yeadon_vec_to_bicycle_vec(human.K2.pos, mpar, bpar)
-            plt.plot([start[0, 0], end[0, 0]],
-                     [-start[2, 0], -end[2, 0]], 'k')
+            ax.plot([start[0, 0], end[0, 0]],
+                    [-start[2, 0], -end[2, 0]], 'k')
             # K1: upper leg, knee to hip
             start = rider.yeadon_vec_to_bicycle_vec(human.K2.pos, mpar, bpar)
             end = rider.yeadon_vec_to_bicycle_vec(human.K1.pos, mpar, bpar)
-            plt.plot([start[0, 0], end[0, 0]],
-                     [-start[2, 0], -end[2, 0]], 'k')
+            ax.plot([start[0, 0], end[0, 0]],
+                    [-start[2, 0], -end[2, 0]], 'k')
             # torso
             start = rider.yeadon_vec_to_bicycle_vec(human.K1.pos, mpar, bpar)
             end = rider.yeadon_vec_to_bicycle_vec(human.B1.pos, mpar, bpar)
-            plt.plot([start[0, 0], end[0, 0]],
-                     [-start[2, 0], -end[2, 0]], 'k')
+            ax.plot([start[0, 0], end[0, 0]],
+                    [-start[2, 0], -end[2, 0]], 'k')
             # B1: upper arm
             start = rider.yeadon_vec_to_bicycle_vec(human.B1.pos, mpar, bpar)
             end = rider.yeadon_vec_to_bicycle_vec(human.B2.pos, mpar, bpar)
-            plt.plot([start[0, 0], end[0, 0]],
-                     [-start[2, 0], -end[2, 0]], 'k')
+            ax.plot([start[0, 0], end[0, 0]],
+                    [-start[2, 0], -end[2, 0]], 'k')
             # B2: lower arm, elbow to tip of fingers
             start = rider.yeadon_vec_to_bicycle_vec(human.B2.pos, mpar, bpar)
             end = rider.yeadon_vec_to_bicycle_vec(human.B2.end_pos, mpar, bpar)
-            plt.plot([start[0, 0], end[0, 0]],
-                     [-start[2, 0], -end[2, 0]], 'k')
+            ax.plot([start[0, 0], end[0, 0]],
+                    [-start[2, 0], -end[2, 0]], 'k')
             # C: chest/head
             start = rider.yeadon_vec_to_bicycle_vec(human.B1.pos, mpar, bpar)
             end = rider.yeadon_vec_to_bicycle_vec(human.C.end_pos, mpar, bpar)
-            plt.plot([start[0, 0], end[0, 0]],
-                     [-start[2, 0], -end[2, 0]], 'k')
+            ax.plot([start[0, 0], end[0, 0]],
+                    [-start[2, 0], -end[2, 0]], 'k')
+            top_of_head = -end[2, 0]
+
+        ax.set_aspect('equal')
+
+        # set the y limits to encompass the bicycle and rider geometry
+        max_y = max([2*par['rR'],  # rear wheel diameter
+                     2*par['rF'],  # front wheel diameter
+                     max(-deez),  # max of Z values of bicycle geometry
+                     top_of_head])  # max of Z values of human head
+        min_y = min(-deez)
+        if min_y >= 0.0:
+            y_low = min([0.0, min_y])
+        else:
+            y_low = -np.ceil(np.abs(min_y))
+        ax.set_ylim((y_low, np.ceil(max_y)))
+
+        ax.set_title("{}\nBicycle Geometry".format(self.bicycleName))
+
+        ax.set_xlabel('x [m]')
+        ax.set_ylabel('-z [m]')
 
         if show:
             fig.show()
 
+        # TODO : This should return ax instead of fig to follow typical
+        # practice in other Python libraries.
+
         return fig
 
+    def _plot_bicycle_geometry_plotly(self, show=True, pendulum=True,
+                                      centerOfMass=True, inertiaEllipse=True):
+        """Returns a Plotly figure showing the basic bicycle geometry,
+        the centers of
+        mass and the moments of inertia.
+
+        Parameters
+        ==========
+        show : optional
+            If true plotly figure will show.
+        centerOfMass : boolean, optional
+            If true the mass center of each rigid body will be displayed. but
+            will have no trace in the legend since it already has a button.
+            The hoverfunction will show where the COM's are located.
+        inertiaEllipse : boolean optional
+            If true inertia ellipses for each rigid body will be displayed.
+            In some cases the ellipses are so large that they will not fit in
+            the figure. Therefor the axis of this plot are fixed.
+
+        Returns
+        =======
+        fig1 : A plotly figure
+
+        """
+        if px is None:
+            raise ImportError('plotly is not installed')
+        par = io.remove_uncertainties(self.parameters['Benchmark'])
+        parts = get_parts_in_parameters(par)
+
+        try:
+            slopes = io.remove_uncertainties(self.extras['slopes'])
+            intercepts = io.remove_uncertainties(self.extras['intercepts'])
+            penInertias = io.remove_uncertainties(
+                self.extras['pendulumInertias'])
+        except AttributeError:
+            pendulum = False
+
+        fig1 = go.Figure()
+
+        # define some colors for the parts
+        # cmap = px.colors.sequential.Agsunset
+        cmap = px.colors.qualitative.Pastel
+        partColors = {}
+
+        for i, part in enumerate(parts):
+            partColors[part] = cmap[i]
+
+        if inertiaEllipse:
+            # plot the principal moments of inertia
+            for j, part in enumerate(parts):
+                I = inertia.part_inertia_tensor(par, part)
+                Ip, C = inertia.principal_axes(I)
+                if part == 'R':
+                    center = np.array([0., par['rR']])
+                elif part in 'FD':
+                    center = np.array([par['w'], par['rF']])
+                else:
+                    center = np.array([par['x' + part], -par['z' + part]])
+                    # which row in C is the y vector
+                uy = np.array([0., 1., 0.])
+                for i, row in enumerate(C):
+                    if np.abs(np.sum(row - uy)) < 1E-10:
+                        yrow = i
+                    # remove the row for the y vector
+                Ip2D = np.delete(Ip, yrow, 0)
+                # remove the column and row associated with the y
+                C2D = np.delete(np.delete(C, yrow, 0), 1, 1)
+                # make an ellipse
+                Imin = Ip2D[0]
+                Imax = Ip2D[1]
+                # get width and height of a ellipse with
+                # the major axis equal to one
+                unitWidth = 1. / 2. / np.sqrt(Imin) * np.sqrt(Imin)
+                unitHeight = 1. / 2. / np.sqrt(Imax) * np.sqrt(Imin)
+                # now scaled the width and height relative to
+                # the maximum principal moment of inertia
+                width = Imax * unitWidth
+                height = Imax * unitHeight
+                angle = -np.degrees(np.arccos(C2D[0, 0]))
+                x_center = center[0]
+                y_center = center[1]
+                x_ep, y_ep = plot._generate_ellipse_plot_data(
+                    x_center=x_center, y_center=y_center,
+                    ax1=[np.cos(angle), np.sin(angle)],
+                    ax2=[-np.sin(angle), np.cos(angle)],
+                    a=height, b=width, N=100)
+
+                fig1.add_scatter(x=x_ep, y=y_ep, mode='lines',
+                                 name='Inertia of ' + part,
+                                 line_color=partColors[part],
+                                 fill='toself', opacity=0.5)
+
+        # plot the ground line
+        x = np.array([-par['rR'], par['w'] + par['rF']])
+        fig1.add_trace(go.Scatter(x=x, y=np.zeros_like(x),
+                       mode='lines',
+                       name='Ground',
+                       line_color='lightgrey',
+                       hovertemplate="%{x:.3f}<br>%{y:.3f}"))
+
+        def make_circle_legend(R, x_center_wheel, y_center_wheel):
+            t = np.linspace(0, 2*np.pi, 100)
+            xwh = R*np.cos(t)
+            ywh = R*np.sin(t)
+            x_wheel = xwh + x_center_wheel
+            y_wheel = ywh + y_center_wheel
+            return x_wheel, y_wheel
+
+        # plot the rear wheel
+        x_wheel_R, y_wheel_R = make_circle_legend(par['rR'], 0, par['rR'])
+        fig1.add_trace(go.Scatter(x=x_wheel_R,
+                                  y=y_wheel_R,
+                                  mode='lines',
+                                  line_color='grey',
+                                  name='Rear wheel',
+                                  hovertemplate="%{x:.3f}<br>%{y:.3f}"))
+
+        # plot the front wheel
+        x_wheel_F, y_wheel_F = make_circle_legend(par['rF'], par['w'],
+                                                  par['rF'])
+        fig1.add_trace(go.Scatter(x=x_wheel_F,
+                                  y=y_wheel_F,
+                                  mode='lines',
+                                  line_color='grey',
+                                  hovertemplate="%{x:.3f}<br>%{y:.3f}",
+                                  name='Front wheel'))
+
+        # plot the fundamental bike
+        deex, deez = geometry.fundamental_geometry_plot_data(par)
+        fig1.add_trace(go.Scatter(x=deex, y=-deez,
+                                  mode='lines',
+                                  name='Bicycle',
+                                  line_color='black',
+                                  hovertemplate="%{x:.3f}<br>%{y:.3f}"))
+
+        # plot the steer axis
+        dx3 = deex[2] + deez[2] * (deex[2] - deex[1]) / (deez[1] - deez[2])
+
+        fig1.add_trace(go.Scatter(x=[deex[2], dx3], y=[-deez[2], 0.],
+                                  mode='lines',
+                                  name='Steer axis',
+                                  hovertemplate="%{x:.3f}<br>%{y:.3f}",
+                                  line=dict(dash='dash', color='dodgerblue')))
+
+        # Update Layout so circle will be round and background white and no
+        # grid
+        fig1.update_xaxes(showgrid=False, zeroline=False)
+        fig1.update_yaxes(showgrid=False, zeroline=False)
+
+        fig1.update_xaxes(
+            range=[-par['rR'], par['w']+par['rF']],  # sets the range of xaxis
+            constrain="domain",  # meanwhile compresses the xaxis by decreasing its "domain"
+        )
+        fig1.update_yaxes(scaleanchor="x", scaleratio=1)
+        fig1.update_layout(plot_bgcolor="white")
+
+        # don't plot the pendulum lines if a rider has been added because the
+        # inertia has changed
+        if self.hasRider:
+            pendulum = False
+
+        if pendulum:
+            # plot the pendulum axes for the measured parts
+            for j, pair in enumerate(slopes.items()):
+                part, slopeSet = pair
+                xcom, zcom = par['x' + part], par['z' + part]
+                for i, m in enumerate(slopeSet):
+                    b = intercepts[part][i]
+                    xPoint, zPoint = geometry.project_point_on_line((m, b),
+                                                                    (xcom,
+                                                                     zcom))
+                    comLineLength = penInertias[part][i]
+                    xPlus = comLineLength / 2. * np.cos(np.arctan(m))
+                    xp = np.array([xPoint - xPlus,
+                                  xPoint + xPlus])
+                    zp = -m*xp - b
+
+                    fig1.add_scatter(x=xp, y=zp, mode='lines', name='Pendulum',
+                                     line=dict(dash='dash'))
+
+        if centerOfMass:
+            def com_symbol(R, x_center, y_center, partcolor):
+                t = np.linspace(0, 0.5*np.pi, 100)
+                xs = R*np.cos(t)
+                ys = R*np.sin(t)
+                xc1 = xs + x_center
+                yc1 = ys + y_center
+                t2 = np.linspace(0.5*np.pi, np.pi, 100)
+                xs2 = R*np.cos(t2)
+                ys2 = R*np.sin(t2)
+                xc2 = xs2 + x_center
+                yc2 = ys2 + y_center
+                t3 = np.linspace(np.pi, 1.5*np.pi, 100)
+                xs3 = R*np.cos(t3)
+                ys3 = R*np.sin(t3)
+                xc3 = xs3 + x_center
+                yc3 = ys3 + y_center
+                t4 = np.linspace(1.5*np.pi, 2*np.pi, 100)
+                xs4 = R*np.cos(t4)
+                ys4 = R*np.sin(t4)
+                xc4 = xs4 + x_center
+                yc4 = ys4 + y_center
+
+                fig1.add_trace(go.Scatter(x=[x_center, x_center+R],
+                                          y=[y_center, y_center], mode='lines',
+                                          line_color=partcolor,
+                                          showlegend=False, hoverinfo='none'))
+                fig1.add_trace(go.Scatter(x=[x_center, x_center],
+                                          y=[y_center, y_center + R],
+                                          mode='lines', line_color=partcolor,
+                                          showlegend=False,
+                                          hoverinfo='none'))
+                fig1.add_trace(go.Scatter(x=xc1, y=yc1, mode='lines',
+                                          line_color=partcolor,
+                                          showlegend=False, fill='tonexty',
+                                          hoverinfo='none'))
+                fig1.add_trace(go.Scatter(x=xc2, y=yc2, mode='lines',
+                                          line_color=partcolor,
+                                          showlegend=False, hoverinfo='none'))
+                fig1.add_trace(go.Scatter(x=xc3, y=yc3, mode='lines',
+                                          line_color=partcolor,
+                                          showlegend=False, hoverinfo='none'))
+                fig1.add_trace(go.Scatter(x=[x_center-R, x_center],
+                                          y=[y_center, y_center], mode='lines',
+                                          line_color=partcolor,
+                                          showlegend=False, fill='tonexty',
+                                          hoverinfo='none'))
+                fig1.add_trace(go.Scatter(x=[x_center, x_center],
+                                          y=[y_center-R, y_center],
+                                          mode='lines', line_color=partcolor,
+                                          showlegend=False,
+                                          hoverinfo='none'))
+                fig1.add_trace(go.Scatter(x=xc4, y=yc4, mode='lines',
+                                          line_color=partcolor,
+                                          showlegend=False, hoverinfo='none'))
+                fig1.add_trace(go.Scatter(x=[x_center, x_center],
+                                          y=[y_center, y_center],
+                                          mode='lines', line_color=partcolor,
+                                          hovertemplate="%{x:.3f}<br>%{y:.3f}",
+                                          name='COM', showlegend=False))
+                return fig1
+
+            # radius of the CoM symbol
+            sRad = 0.03
+            # front wheel CoM
+            x_com_Wf = par['w']
+            y_com_Wf = par['rF']
+            fig1 = com_symbol(sRad, x_com_Wf, y_com_Wf, partColors['F'])
+            fig1.add_annotation(text='F', xref='x', yref='y',
+                                x=x_com_Wf + 0.055,
+                                y=y_com_Wf+0.055, showarrow=False,
+                                font=dict(size=15))
+
+            # rear wheel CoM
+            fig1 = com_symbol(sRad, 0., par['rR'], partColors['R'])
+            fig1.add_annotation(text='R', xref='x', yref='y', x=0.055,
+                                y=par['rR']+0.055, showarrow=False,
+                                font=dict(size=15))
+
+            for j, part in enumerate([x for x in parts
+                                      if x not in 'RFD']):
+                xcom = par['x' + part]
+                zcom = par['z' + part]
+                fig1 = com_symbol(sRad, xcom, -zcom, partColors[part])
+                fig1.add_annotation(text=part, xref='x', yref='y',
+                                    x=xcom+0.055, y=-zcom+0.055,
+                                    showarrow=False, font=dict(size=15))
+
+            if 'H' not in parts:
+                fig1 = com_symbol(sRad, par['xH'], -par['zH'], partColors['H'])
+                fig1.add_annotation(text="H", xref='x', yref='y',
+                                    x=par['xH']+0.055, y=-par['zH']+0.055,
+                                    showarrow=False, font=dict(size=15))
+
+        # if there is a rider on the bike, make a simple stick figure
+        if self.human:
+            human = self.human
+            mpar = self.parameters['Measured']
+            bpar = self.parameters['Benchmark']
+            # K2: lower leg, tip of foot to knee
+            start = rider.yeadon_vec_to_bicycle_vec(human.K2.end_pos, mpar,
+                                                    bpar)
+            end = rider.yeadon_vec_to_bicycle_vec(human.K2.pos, mpar, bpar)
+            fig1.add_trace(go.Scatter(x=[start[0, 0], end[0, 0]],
+                                      y=[-start[2, 0], -end[2, 0]],
+                                      mode='lines'))
+
+            # K1: upper leg, knee to hip
+            start = rider.yeadon_vec_to_bicycle_vec(human.K2.pos, mpar, bpar)
+            end = rider.yeadon_vec_to_bicycle_vec(human.K1.pos, mpar, bpar)
+
+        fig1.update_layout(title=dict(text='Bicycle geometry',
+                           font=dict(family="Segoe UI", size=25)),
+                           yaxis_title='z-axis [m]',
+                           font_family="Source Sans Pro",
+                           hoverlabel=dict(font_family="Source Sans Pro"))
+
+        fig1.update_layout(yaxis=dict(autorange=True, showgrid=False,
+                                      ticks='outside', showticklabels=True))
+        fig1.update_layout(xaxis=dict(autorange=True, showgrid=False, ticks='',
+                                      showticklabels=False))
+        if show:
+            fig1.show()
+        return fig1
+
     def canonical(self, nominal=False):
         """
         Returns the canonical velocity and gravity independent matrices for
         the Whipple bicycle model linearized about the nominal
         configuration.
 
         Parameters
@@ -838,15 +1207,15 @@
             evals[i] = w
             evecs[i] = v
 
         return evals, evecs
 
     def plot_eigenvalues_vs_speed(self, speeds, fig=None, generic=False,
                                   color='black', show=False, largest=False,
-                                  linestyle='-'):
+                                  linestyle='-', grid=False, show_legend=True):
         """Returns a plot of the eigenvalues versus speed for the current
         benchmark parameters.
 
         Parameters
         ----------
         speeds : ndarray, shape(n,)
             An array of speeds to calculate the eigenvalues at.
@@ -855,44 +1224,57 @@
         generic : boolean
             If true the lines will all be the same color and the modes will
             not be labeled.
         color : matplotlib color
             If generic is true this will be the color of the plot lines.
         largest : boolean
             If true, only the largest eigenvalue is plotted.
+        grid : boolean, optional
+            If true, displays a grid on the plot.
+        show_legend: boolean, optional
+            If true, displays a legend describing the different parts of the
+            solution shown.
+
+        Returns
+        -------
+        fig : matpolib.pyplot.Figure
+            The figure.
 
         Notes
         -----
         If you have a flywheel defined, body D, it will completely be
         ignored in these results. These results are strictly for the Whipple
         bicycle model.
 
         """
 
         # sort the speeds in case they aren't
         speeds = np.sort(speeds)
 
         # figure properties
-        figwidth = 6. # in inches
-        goldenMean = (np.sqrt(5.0) - 1.0) / 2.0
-        figsize = [figwidth, figwidth * goldenMean]
-        params = {#'backend': 'ps',
+        fig_height = 4.0  # inches
+        figsize = [fig_height*GOLDEN_RATIO, fig_height]
+        params = {
             'axes.labelsize': 8,
             'text.fontsize': 10,
             'legend.fontsize': 8,
             'xtick.labelsize': 6,
             'ytick.labelsize': 6,
             'figure.figsize': figsize
             }
-        plt.rcParams.update(params)
-
-        if not fig:
-            fig = plt.figure(figsize=figsize)
+        # NOTE : text.fontsize no longer supported in matplotlib
+        try:
+            plt.rcParams.update(params)
+        except KeyError:
+            del params['text.fontsize']
+            params['font.size'] = 10
+            plt.rcParams.update(params)
 
-        plt.axes([0.125, 0.2, 0.95 - 0.125, 0.85 - 0.2])
+        if fig is None:
+            fig, ax = plt.subplots(figsize=figsize)
 
         evals, evecs = self.eig(speeds)
 
         if largest:
             generic = True
 
         if generic:
@@ -909,60 +1291,169 @@
             legend = ['Imaginary Weave', 'Imaginary Capsize',
                       'Imaginary Caster', 'Real Weave', 'Real Capsize',
                       'Real Caster']
             maxLabel = 'Max Eigenvalue'
 
         if largest:
             maxEval = np.max(np.real(evals), axis=1)
-            plt.plot(speeds, maxEval, color=color, label=maxLabel,
-                     linestyle=linestyle, linewidth=1.5)
+            ax.plot(speeds, maxEval, color=color, label=maxLabel,
+                    linestyle=linestyle, linewidth=1.5)
             # x axis line
-            plt.plot(speeds, np.zeros_like(speeds), 'k-',
-                     label='_nolegend_', linewidth=1.5)
-            plt.ylim((np.min(maxEval), np.max(maxEval)))
-            plt.ylabel('Real Part of the Largest Eigenvalue [1/s]')
+            ax.plot(speeds, np.zeros_like(speeds), 'k-', label='_nolegend_',
+                    linewidth=1.5)
+            ax.set_ylim((np.min(maxEval), np.max(maxEval)))
+            ax.set_ylabel('Real Part of the Largest Eigenvalue [1/s]')
         else:
             wea, cap, cas = bicycle.sort_modes(evals, evecs)
 
             # imaginary components
-            plt.plot(speeds, np.abs(np.imag(wea['evals'])), color=weaveColor,
-                     label=legend[0], linestyle='--')
-            plt.plot(speeds, np.abs(np.imag(cap['evals'])), color=capsizeColor,
-                     label=legend[1], linestyle='--')
-            plt.plot(speeds, np.abs(np.imag(cas['evals'])), color=casterColor,
-                     label=legend[2], linestyle='--')
+            ax.plot(speeds, np.abs(np.imag(wea['evals'])), color=weaveColor,
+                    label=legend[0], linestyle='--')
+            ax.plot(speeds, np.abs(np.imag(cap['evals'])), color=capsizeColor,
+                    label=legend[1], linestyle='--')
+            ax.plot(speeds, np.abs(np.imag(cas['evals'])), color=casterColor,
+                    label=legend[2], linestyle='--')
 
             # x axis line
-            plt.plot(speeds, np.zeros_like(speeds), 'k-',
-                     label='_nolegend_', linewidth=1.5)
+            ax.plot(speeds, np.zeros_like(speeds), 'k-', label='_nolegend_',
+                    linewidth=1.5)
 
             # plot the real parts of the eigenvalues
-            plt.plot(speeds, np.real(wea['evals']),
-                     color=weaveColor, label=legend[3])
-            plt.plot(speeds, np.real(cap['evals']),
-                     color=capsizeColor, label=legend[4])
-            plt.plot(speeds, np.real(cas['evals']),
-                     color=casterColor, label=legend[5])
+            ax.plot(speeds, np.real(wea['evals']), color=weaveColor,
+                    label=legend[3])
+            ax.plot(speeds, np.real(cap['evals']), color=capsizeColor,
+                    label=legend[4])
+            ax.plot(speeds, np.real(cas['evals']), color=casterColor,
+                    label=legend[5])
 
             # set labels and limits
-            plt.ylim((np.min(np.real(evals)),
-                      np.max(np.imag(evals))))
-            plt.ylabel('Real and Imaginary Parts of the Eigenvalue [1/s]')
+            ax.set_ylabel('Real and Imaginary Parts of the Eigenvalue [1/s]')
 
-        plt.xlim((speeds[0], speeds[-1]))
-        plt.xlabel('Speed [m/s]')
+        ax.set_xlim((speeds[0], speeds[-1]))
+        ax.set_xlabel('Speed [m/s]')
 
         if generic:
-            plt.title('Eigenvalues vs Speed')
+            ax.set_title('Eigenvalues vs Speed')
+        else:
+            ax.set_title('%s\nEigenvalues vs Speed' % self.bicycleName)
+            if show_legend:
+                ax.legend()
+
+        if grid:
+            ax.grid()
+
+        if show:
+            fig.show()
+
+        return fig
+
+    def _plot_eigenvalues_vs_speed_plotly(self, speeds, fig=None, show=True,
+                                          largest=False,
+                                          stability_region=True):
+        if px is None:
+            raise ImportError('plotly is not installed')
+        speeds = np.sort(speeds)
+        if fig is None:
+            fig = go.Figure(layout_yaxis_range=[-10, 10])
+            evals, evecs = self.eig(speeds)
+
+        if largest:
+            fig.add_trace(go.Scatter(x=speeds, y=np.max(evals)))
+            fig.show()
         else:
-            plt.title('%s\nEigenvalues vs Speed' % self.bicycleName)
-            plt.legend()
+            w, cap, cas = bicycle.sort_modes(evals, evecs)
+            colors_eig = px.colors.qualitative.Pastel
+            weaveColor1 = colors_eig[0]
+            weaveColor2 = colors_eig[1]
+            capsizeColor = colors_eig[2]
+            casterColor = colors_eig[5]
+        wea1 = w['evals'][:, 0]
+        wea2 = w['evals'][:, 1]
+        fig.add_trace(go.Scatter(x=speeds, y=np.real(wea1),
+                                 mode='lines',
+                                 name='Re Weave',
+                                 line=dict(color=weaveColor1),
+                                 text='Re'))
+        fig.add_trace(go.Scatter(x=speeds, y=np.real(wea2),
+                                 mode='lines',
+                                 name='Re Weave',
+                                 line=dict(color=weaveColor2),
+                                 text='Re'))
+        fig.add_trace(go.Scatter(x=speeds, y=np.real(cap['evals']),
+                                 mode='lines',
+                                 name='Re Capsize',
+                                 line=dict(color=capsizeColor),
+                                 text='Re'))
+        fig.add_trace(go.Scatter(x=speeds, y=np.real(cas['evals']),
+                                 mode='lines',
+                                 name='Re Castering',
+                                 line=dict(color=casterColor),
+                                 text='Re'))
+        fig.add_trace(go.Scatter(x=speeds, y=np.abs(np.imag(wea1)),
+                                 mode='lines',
+                                 name='Im Weave',
+                                 line=dict(color=weaveColor1, dash='dash'),
+                                 text='Im'))
+        fig.add_trace(go.Scatter(x=speeds, y=np.abs(np.imag(wea2)),
+                                 mode='lines',
+                                 name='Im Weave',
+                                 line=dict(color=weaveColor2, dash='dash'),
+                                 text='Im'))
+        fig.add_trace(go.Scatter(x=speeds, y=np.abs(np.imag(cap['evals'])),
+                                 mode='lines',
+                                 name='Im Capsize',
+                                 line=dict(color=capsizeColor, dash='dash'),
+                                 text='Im'))
+        fig.add_trace(go.Scatter(x=speeds, y=np.abs(np.imag(cas['evals'])),
+                                 mode='lines',
+                                 name='Im Castering',
+                                 line=dict(color=casterColor, dash='dash'),
+                                 text='Im'))
+        if stability_region:
+            try:
+                v_start_stab = max([min(speeds[np.real(wea2) < 0]),
+                                    min(speeds[np.real(cas['evals']) < 0]),
+                                    min(speeds[np.real(cap['evals']) < 0]),
+                                    min(speeds[np.real(wea1) < 0],
+                                        default="EMPTY")])
+                v_end_stab = min([max(speeds[np.real(wea2) < 0]),
+                                  max(speeds[np.real(cas['evals']) < 0]),
+                                  max(speeds[np.real(cap['evals']) < 0]),
+                                  max(speeds[np.real(wea1) < 0])])
+            except:  # TODO : Add explicit exception
+                fig.add_annotation(x=0.5*max(speeds), y=9,
+                                   text="No stability region",
+                                   showarrow=False)
+            if (v_start_stab > v_end_stab):
+                fig.add_annotation(x=0.5*max(speeds), y=9,
+                                   text="No stability region",
+                                   showarrow=False)
+            elif (v_end_stab - v_start_stab < 0.0001):
+                fig.add_annotation(x=0.5*max(speeds), y=9,
+                                   text="No stability region",
+                                   showarrow=False)
+            else:
+                fig.add_vrect(x0=v_start_stab, x1=v_end_stab,
+                              annotation_text="Self stability",
+                              annotation_position='top left',
+                              # fillcolor="blue", opacity=0.25,
+                              fillcolor='rgba(71,147,231,0.5)',
+                              line_width=0, row=1, col=1)
+
+        fig.update_layout(title=dict(text='Eigenvalues vs velocity',
+                          font=dict(family="Segoe UI", size=25)),
+                          font_family="Source Sans Pro",
+                          plot_bgcolor='rgba(39,128,227,0.15)',
+                          xaxis_title='Velocity [m/s]',
+                          yaxis_title='Eigenvalues [1/s]',
+                          hoverlabel=dict(font_family="Source Sans Pro"))
+        fig.update_traces(hovertemplate="%{x:.3f}<br>%{y:.3f}")
 
         if show:
-            plt.show()
+            fig.show()
 
         return fig
 
     def plot_bode(self, speed, u, y, **kwargs):
         """Returns a Bode plot.
 
         Parameters
@@ -1042,14 +1533,15 @@
         phaseLines = fig.ax2.lines
         for line in phaseLines:
             firstValue = line.get_ydata()[0]
             n = np.ceil(np.floor(abs(firstValue / 180.)) / 2.)
             line.set_ydata(line.get_ydata() - np.sign(firstValue) * n * 360.)
         return fig
 
+
 def get_parts_in_parameters(par):
     '''Returns a list of parts in a parameter dictionary.
 
     Parameters
     ----------
     par : dictionary
         Benchmark bicycle parameters.
@@ -1060,14 +1552,15 @@
         Unique list of parts that contain one or more of 'H', 'B', 'F', 'R',
         'S', 'G', 'D'.
 
     '''
     parts = [x[1] for x in par.keys() if x.startswith('m')]
     return parts
 
+
 def calculate_benchmark_from_measured(mp):
     '''Returns the benchmark (Meijaard 2007) parameter set based on the
     measured data.
 
     Parameters
     ----------
     mp : dictionary
@@ -1106,15 +1599,15 @@
 
     # get the slopes, intercepts and betas for each part
     slopes, intercepts, betas = com.part_com_lines(mp, par, forkIsSplit)
 
     # calculate the centers of mass
     for part in slopes.keys():
         par['x' + part], par['z' + part] = com.center_of_mass(slopes[part],
-            intercepts[part])
+                                                              intercepts[part])
 
     # find the center of mass of the handlebar/fork assembly if the fork was
     # split
     if forkIsSplit:
         coordinates = np.array([[par['xS'], par['xG']],
                                 [0., 0.],
                                 [par['zS'], par['zG']]])
@@ -1125,75 +1618,76 @@
         par['zH'] = cH[2]
 
     # local accelation due to gravity
     par['g'] = mp['g']
 
     # calculate the wheel y inertias
     par['IFyy'] = inertia.compound_pendulum_inertia(mp['mF'], mp['g'],
-                                            mp['lF'], mp['TcF1'])
+                                                    mp['lF'], mp['TcF1'])
     par['IRyy'] = inertia.compound_pendulum_inertia(mp['mR'], mp['g'],
-                                            mp['lR'], mp['TcR1'])
+                                                    mp['lR'], mp['TcR1'])
     try:
         # we measured the inertia of the front wheel with the flywheel inside
-        iFlywheelPlusFwheel = inertia.compound_pendulum_inertia(mp['mD'], mp['g'], mp['lF'], mp['TcD1'])
+        iFlywheelPlusFwheel = inertia.compound_pendulum_inertia(
+            mp['mD'], mp['g'], mp['lF'], mp['TcD1'])
         par['IDyy'] = iFlywheelPlusFwheel - par['IFyy']
     except KeyError:
         pass
 
     # calculate the y inertias for the frame and fork
     lB = (par['xB']**2 + (par['zB'] + par['rR'])**2)**(0.5)
     par['IByy'] = inertia.compound_pendulum_inertia(mp['mB'], mp['g'], lB,
                                                     mp['TcB1'])
 
     if forkIsSplit:
         # fork
         lS = ((par['xS'] - par['w'])**2 +
               (par['zS'] + par['rF'])**2)**(0.5)
-        par['ISyy'] = inertia.compound_pendulum_inertia(mp['mS'], mp['g'],
-                                                lS, mp['TcS1'])
+        par['ISyy'] = inertia.compound_pendulum_inertia(mp['mS'], mp['g'], lS,
+                                                        mp['TcS1'])
         # handlebar
-        l1, l2 = geometry.calculate_l1_l2(mp['h6'], mp['h7'],
-                                 mp['d5'], mp['d6'], mp['l'])
+        l1, l2 = geometry.calculate_l1_l2(mp['h6'], mp['h7'], mp['d5'],
+                                          mp['d6'], mp['l'])
         u1, u2 = geometry.fwheel_to_handlebar_ref(par['lam'], l1, l2)
         lG = ((par['xG'] - par['w'] + u1)**2 +
               (par['zG'] + par['rF'] + u2)**2)**(.5)
-        par['IGyy'] = inertia.compound_pendulum_inertia(mp['mG'], mp['g'],
-                                                lG, mp['TcG1'])
+        par['IGyy'] = inertia.compound_pendulum_inertia(mp['mG'], mp['g'], lG,
+                                                        mp['TcG1'])
     else:
         lH = ((par['xH'] - par['w'])**2 +
               (par['zH'] + par['rF'])**2)**(0.5)
-        par['IHyy'] = inertia.compound_pendulum_inertia(mp['mH'], mp['g'],
-                                                lH, mp['TcH1'])
+        par['IHyy'] = inertia.compound_pendulum_inertia(mp['mH'], mp['g'], lH,
+                                                        mp['TcH1'])
 
     # calculate the stiffness of the torsional pendulum
     IPxx, IPyy, IPzz = inertia.tube_inertia(mp['lP'], mp['mP'],
                                             mp['dP'] / 2., 0.)
     torStiff = inertia.torsional_pendulum_stiffness(IPyy, mp['TtP1'])
-    #print("Torsional pendulum stiffness:", torStiff)
 
     # calculate the wheel x/z inertias
     par['IFxx'] = inertia.tor_inertia(torStiff, mp['TtF1'])
     par['IRxx'] = inertia.tor_inertia(torStiff, mp['TtR1'])
     try:
-        par['IDxx'] =  inertia.tor_inertia(torStiff, mp['TtD1']) - par['IFxx']
+        par['IDxx'] = inertia.tor_inertia(torStiff, mp['TtD1']) - par['IFxx']
     except KeyError:
         pass
 
     pendulumInertias = {}
 
     # calculate the in plane moments of inertia
     for part, slopeSet in slopes.items():
         # the number of orientations for this part
         numOrien = len(slopeSet)
         # intialize arrays to store the inertia values and orientation angles
         penInertia = np.zeros(numOrien, dtype=object)
         beta = np.array(betas[part])
         # fill arrays of the inertias
         for i in range(numOrien):
-            penInertia[i] = inertia.tor_inertia(torStiff, mp['Tt' + part + str(i + 1)])
+            penInertia[i] = inertia.tor_inertia(torStiff,
+                                                mp['Tt' + part + str(i + 1)])
         # store these inertias
         pendulumInertias[part] = list(penInertia)
         inert = inertia.inertia_components(penInertia, beta)
         for i, axis in enumerate(['xx', 'xz', 'zz']):
             par['I' + part + axis] = inert[i]
 
     if forkIsSplit:
@@ -1214,21 +1708,22 @@
               inertia.parallel_axis(IS, par['mS'], dS))
         par['IHxx'] = IH[0, 0]
         par['IHxz'] = IH[0, 2]
         par['IHyy'] = IH[1, 1]
         par['IHzz'] = IH[2, 2]
 
     # package the extra information that is useful outside this function
-    extras = {'slopes' : slopes,
-              'intercepts' : intercepts,
-              'betas' : betas,
-              'pendulumInertias' : pendulumInertias}
+    extras = {'slopes': slopes,
+              'intercepts': intercepts,
+              'betas': betas,
+              'pendulumInertias': pendulumInertias}
 
     return par, extras
 
+
 def is_fork_split(mp):
     '''Returns true if the fork was split into two parts and false if not.
 
     Parameters
     ----------
     mp : dictionary
         The measured data.
```

