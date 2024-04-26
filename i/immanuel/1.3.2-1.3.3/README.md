# Comparing `tmp/immanuel-1.3.2.tar.gz` & `tmp/immanuel-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "immanuel-1.3.2.tar", last modified: Tue Apr 16 01:51:30 2024, max compression
+gzip compressed data, was "immanuel-1.3.3.tar", last modified: Fri Apr 26 02:31:29 2024, max compression
```

## Comparing `immanuel-1.3.2.tar` & `immanuel-1.3.3.tar`

### file list

```diff
@@ -1,80 +1,84 @@
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:51:30.840770 immanuel-1.3.2/
--rw-r--r--   0 robert     (501) staff       (20)    32096 2023-12-02 01:56:03.000000 immanuel-1.3.2/LICENSE.md
--rw-r--r--   0 robert     (501) staff       (20)       26 2024-04-16 01:50:25.000000 immanuel-1.3.2/MANIFEST.in
--rw-r--r--   0 robert     (501) staff       (20)    49211 2024-04-16 01:51:30.840395 immanuel-1.3.2/PKG-INFO
--rw-r--r--   0 robert     (501) staff       (20)    11218 2024-04-16 01:30:39.000000 immanuel-1.3.2/README.md
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:51:30.764593 immanuel-1.3.2/immanuel/
--rw-r--r--   0 robert     (501) staff       (20)       66 2024-04-16 01:27:34.000000 immanuel-1.3.2/immanuel/__init__.py
--rw-r--r--   0 robert     (501) staff       (20)    18861 2024-04-16 01:27:34.000000 immanuel-1.3.2/immanuel/charts.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:51:30.770066 immanuel-1.3.2/immanuel/classes/
--rw-r--r--   0 robert     (501) staff       (20)      619 2024-04-01 00:34:17.000000 immanuel-1.3.2/immanuel/classes/cache.py
--rw-r--r--   0 robert     (501) staff       (20)     2158 2024-04-16 01:25:04.000000 immanuel-1.3.2/immanuel/classes/localize.py
--rw-r--r--   0 robert     (501) staff       (20)      558 2024-01-16 22:54:01.000000 immanuel-1.3.2/immanuel/classes/serialize.py
--rw-r--r--   0 robert     (501) staff       (20)    12561 2024-04-16 01:27:34.000000 immanuel-1.3.2/immanuel/classes/wrap.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:51:30.774135 immanuel-1.3.2/immanuel/const/
--rw-r--r--   0 robert     (501) staff       (20)     2325 2024-01-20 20:33:35.000000 immanuel-1.3.2/immanuel/const/calc.py
--rw-r--r--   0 robert     (501) staff       (20)     2613 2023-12-15 16:02:49.000000 immanuel-1.3.2/immanuel/const/chart.py
--rw-r--r--   0 robert     (501) staff       (20)      770 2024-01-16 22:54:01.000000 immanuel-1.3.2/immanuel/const/data.py
--rw-r--r--   0 robert     (501) staff       (20)    11276 2024-01-16 22:54:01.000000 immanuel-1.3.2/immanuel/const/dignities.py
--rw-r--r--   0 robert     (501) staff       (20)      255 2024-04-08 01:17:15.000000 immanuel-1.3.2/immanuel/const/genders.py
--rw-r--r--   0 robert     (501) staff       (20)     5692 2024-01-16 22:54:01.000000 immanuel-1.3.2/immanuel/const/names.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:51:30.759361 immanuel-1.3.2/immanuel/locales/
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:51:30.774734 immanuel-1.3.2/immanuel/locales/pt_BR/
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:51:30.777709 immanuel-1.3.2/immanuel/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 robert     (501) staff       (20)     8005 2024-04-15 00:27:49.000000 immanuel-1.3.2/immanuel/locales/pt_BR/LC_MESSAGES/immanuel.mo
--rw-r--r--   0 robert     (501) staff       (20)     2045 2024-04-15 00:27:49.000000 immanuel-1.3.2/immanuel/locales/pt_BR/mappings.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:51:30.785574 immanuel-1.3.2/immanuel/reports/
--rw-r--r--   0 robert     (501) staff       (20)     4658 2024-04-16 01:27:34.000000 immanuel-1.3.2/immanuel/reports/aspect.py
--rw-r--r--   0 robert     (501) staff       (20)     7581 2024-04-16 01:27:34.000000 immanuel-1.3.2/immanuel/reports/dignity.py
--rw-r--r--   0 robert     (501) staff       (20)     2186 2024-04-16 01:27:34.000000 immanuel-1.3.2/immanuel/reports/pattern.py
--rw-r--r--   0 robert     (501) staff       (20)     1497 2024-01-16 22:54:01.000000 immanuel-1.3.2/immanuel/reports/weighting.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:51:30.759647 immanuel-1.3.2/immanuel/resources/
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:51:30.825035 immanuel-1.3.2/immanuel/resources/ephemeris/
--rw-r--r--   0 robert     (501) staff       (20)   225863 2024-03-29 02:29:31.000000 immanuel-1.3.2/immanuel/resources/ephemeris/seas_12.se1
--rw-r--r--   0 robert     (501) staff       (20)   225440 2024-03-29 02:29:31.000000 immanuel-1.3.2/immanuel/resources/ephemeris/seas_18.se1
--rw-r--r--   0 robert     (501) staff       (20)   225108 2024-03-29 02:29:31.000000 immanuel-1.3.2/immanuel/resources/ephemeris/seas_24.se1
--rw-r--r--   0 robert     (501) staff       (20)  1306782 2024-03-29 02:29:31.000000 immanuel-1.3.2/immanuel/resources/ephemeris/semo_12.se1
--rw-r--r--   0 robert     (501) staff       (20)  1305686 2024-03-29 02:29:31.000000 immanuel-1.3.2/immanuel/resources/ephemeris/semo_18.se1
--rw-r--r--   0 robert     (501) staff       (20)  1309017 2024-03-29 02:29:31.000000 immanuel-1.3.2/immanuel/resources/ephemeris/semo_24.se1
--rw-r--r--   0 robert     (501) staff       (20)  1326257 2024-03-29 02:29:31.000000 immanuel-1.3.2/immanuel/resources/ephemeris/semo_36.se1
--rw-r--r--   0 robert     (501) staff       (20)  1339659 2024-03-29 02:29:31.000000 immanuel-1.3.2/immanuel/resources/ephemeris/semo_42.se1
--rw-r--r--   0 robert     (501) staff       (20)   483763 2024-03-29 02:29:31.000000 immanuel-1.3.2/immanuel/resources/ephemeris/sepl_12.se1
--rw-r--r--   0 robert     (501) staff       (20)   484065 2024-03-29 02:29:31.000000 immanuel-1.3.2/immanuel/resources/ephemeris/sepl_18.se1
--rw-r--r--   0 robert     (501) staff       (20)   483399 2024-03-29 02:29:31.000000 immanuel-1.3.2/immanuel/resources/ephemeris/sepl_24.se1
--rw-r--r--   0 robert     (501) staff       (20)   484686 2024-03-29 02:29:31.000000 immanuel-1.3.2/immanuel/resources/ephemeris/sepl_36.se1
--rw-r--r--   0 robert     (501) staff       (20)   483628 2024-03-29 02:29:31.000000 immanuel-1.3.2/immanuel/resources/ephemeris/sepl_42.se1
--rw-r--r--   0 robert     (501) staff       (20)    11845 2024-04-16 01:24:46.000000 immanuel-1.3.2/immanuel/setup.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:51:30.832425 immanuel-1.3.2/immanuel/tools/
--rw-r--r--   0 robert     (501) staff       (20)     3197 2024-02-02 15:17:22.000000 immanuel-1.3.2/immanuel/tools/calculate.py
--rw-r--r--   0 robert     (501) staff       (20)     6023 2024-01-16 22:54:01.000000 immanuel-1.3.2/immanuel/tools/convert.py
--rw-r--r--   0 robert     (501) staff       (20)     3181 2024-01-17 23:18:15.000000 immanuel-1.3.2/immanuel/tools/date.py
--rw-r--r--   0 robert     (501) staff       (20)    21046 2024-04-01 00:06:06.000000 immanuel-1.3.2/immanuel/tools/ephemeris.py
--rw-r--r--   0 robert     (501) staff       (20)     5702 2024-04-09 19:59:42.000000 immanuel-1.3.2/immanuel/tools/find.py
--rw-r--r--   0 robert     (501) staff       (20)     2027 2024-01-16 22:54:01.000000 immanuel-1.3.2/immanuel/tools/forecast.py
--rw-r--r--   0 robert     (501) staff       (20)     1824 2024-01-16 22:54:01.000000 immanuel-1.3.2/immanuel/tools/midpoint.py
--rw-r--r--   0 robert     (501) staff       (20)     2786 2024-01-16 22:54:01.000000 immanuel-1.3.2/immanuel/tools/position.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:51:30.839808 immanuel-1.3.2/immanuel.egg-info/
--rw-r--r--   0 robert     (501) staff       (20)    49211 2024-04-16 01:51:30.000000 immanuel-1.3.2/immanuel.egg-info/PKG-INFO
--rw-r--r--   0 robert     (501) staff       (20)     1812 2024-04-16 01:51:30.000000 immanuel-1.3.2/immanuel.egg-info/SOURCES.txt
--rw-r--r--   0 robert     (501) staff       (20)        1 2024-04-16 01:51:30.000000 immanuel-1.3.2/immanuel.egg-info/dependency_links.txt
--rw-r--r--   0 robert     (501) staff       (20)       60 2024-04-16 01:51:30.000000 immanuel-1.3.2/immanuel.egg-info/requires.txt
--rw-r--r--   0 robert     (501) staff       (20)        9 2024-04-16 01:51:30.000000 immanuel-1.3.2/immanuel.egg-info/top_level.txt
--rw-r--r--   0 robert     (501) staff       (20)     1070 2024-04-16 01:51:21.000000 immanuel-1.3.2/pyproject.toml
--rw-r--r--   0 robert     (501) staff       (20)       38 2024-04-16 01:51:30.840820 immanuel-1.3.2/setup.cfg
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:51:30.839513 immanuel-1.3.2/tests/
--rw-r--r--   0 robert     (501) staff       (20)    40905 2023-12-02 01:56:03.000000 immanuel-1.3.2/tests/se01181s.se1
--rw-r--r--   0 robert     (501) staff       (20)     3920 2024-04-16 01:27:34.000000 immanuel-1.3.2/tests/test_aspect.py
--rw-r--r--   0 robert     (501) staff       (20)     3530 2024-01-20 00:34:00.000000 immanuel-1.3.2/tests/test_calculate.py
--rw-r--r--   0 robert     (501) staff       (20)    23308 2024-04-16 01:27:34.000000 immanuel-1.3.2/tests/test_charts.py
--rw-r--r--   0 robert     (501) staff       (20)    28783 2024-01-17 23:16:08.000000 immanuel-1.3.2/tests/test_convert.py
--rw-r--r--   0 robert     (501) staff       (20)     4579 2024-01-17 23:18:15.000000 immanuel-1.3.2/tests/test_date.py
--rw-r--r--   0 robert     (501) staff       (20)     9521 2024-04-16 01:27:34.000000 immanuel-1.3.2/tests/test_dignity.py
--rw-r--r--   0 robert     (501) staff       (20)    15068 2024-04-16 01:27:34.000000 immanuel-1.3.2/tests/test_ephemeris.py
--rw-r--r--   0 robert     (501) staff       (20)     3714 2024-01-20 20:35:37.000000 immanuel-1.3.2/tests/test_find.py
--rw-r--r--   0 robert     (501) staff       (20)     6735 2024-01-20 20:36:29.000000 immanuel-1.3.2/tests/test_forecast.py
--rw-r--r--   0 robert     (501) staff       (20)    18927 2024-04-16 01:27:34.000000 immanuel-1.3.2/tests/test_localization.py
--rw-r--r--   0 robert     (501) staff       (20)     5374 2024-01-20 20:36:20.000000 immanuel-1.3.2/tests/test_midpoint.py
--rw-r--r--   0 robert     (501) staff       (20)     2393 2024-01-16 22:54:01.000000 immanuel-1.3.2/tests/test_pattern.py
--rw-r--r--   0 robert     (501) staff       (20)     5157 2024-04-16 01:27:34.000000 immanuel-1.3.2/tests/test_position.py
--rw-r--r--   0 robert     (501) staff       (20)     3169 2024-04-16 01:27:34.000000 immanuel-1.3.2/tests/test_setup.py
--rw-r--r--   0 robert     (501) staff       (20)     2286 2024-04-01 00:40:36.000000 immanuel-1.3.2/tests/test_weighting.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.194582 immanuel-1.3.3/
+-rw-r--r--   0 robert     (501) staff       (20)    32096 2023-12-02 01:56:03.000000 immanuel-1.3.3/LICENSE.md
+-rw-r--r--   0 robert     (501) staff       (20)       26 2024-04-16 01:50:25.000000 immanuel-1.3.3/MANIFEST.in
+-rw-r--r--   0 robert     (501) staff       (20)    47556 2024-04-26 02:31:29.194167 immanuel-1.3.3/PKG-INFO
+-rw-r--r--   0 robert     (501) staff       (20)     9563 2024-04-26 02:27:25.000000 immanuel-1.3.3/README.md
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.101087 immanuel-1.3.3/immanuel/
+-rw-r--r--   0 robert     (501) staff       (20)       66 2024-04-16 01:27:34.000000 immanuel-1.3.3/immanuel/__init__.py
+-rw-r--r--   0 robert     (501) staff       (20)    18861 2024-04-21 20:24:34.000000 immanuel-1.3.3/immanuel/charts.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.124369 immanuel-1.3.3/immanuel/classes/
+-rw-r--r--   0 robert     (501) staff       (20)      619 2024-04-01 00:34:17.000000 immanuel-1.3.3/immanuel/classes/cache.py
+-rw-r--r--   0 robert     (501) staff       (20)     2158 2024-04-16 01:25:04.000000 immanuel-1.3.3/immanuel/classes/localize.py
+-rw-r--r--   0 robert     (501) staff       (20)      558 2024-01-16 22:54:01.000000 immanuel-1.3.3/immanuel/classes/serialize.py
+-rw-r--r--   0 robert     (501) staff       (20)    12699 2024-04-26 01:40:11.000000 immanuel-1.3.3/immanuel/classes/wrap.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.127755 immanuel-1.3.3/immanuel/const/
+-rw-r--r--   0 robert     (501) staff       (20)     2399 2024-04-26 00:50:04.000000 immanuel-1.3.3/immanuel/const/calc.py
+-rw-r--r--   0 robert     (501) staff       (20)     2613 2024-04-21 20:24:34.000000 immanuel-1.3.3/immanuel/const/chart.py
+-rw-r--r--   0 robert     (501) staff       (20)      770 2024-01-16 22:54:01.000000 immanuel-1.3.3/immanuel/const/data.py
+-rw-r--r--   0 robert     (501) staff       (20)    11276 2024-01-16 22:54:01.000000 immanuel-1.3.3/immanuel/const/dignities.py
+-rw-r--r--   0 robert     (501) staff       (20)      255 2024-04-08 01:17:15.000000 immanuel-1.3.3/immanuel/const/genders.py
+-rw-r--r--   0 robert     (501) staff       (20)     5692 2024-04-21 20:24:34.000000 immanuel-1.3.3/immanuel/const/names.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.089329 immanuel-1.3.3/immanuel/locales/
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.128547 immanuel-1.3.3/immanuel/locales/es_ES/
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.129390 immanuel-1.3.3/immanuel/locales/es_ES/LC_MESSAGES/
+-rw-r--r--   0 robert     (501) staff       (20)     7895 2024-04-22 13:27:14.000000 immanuel-1.3.3/immanuel/locales/es_ES/LC_MESSAGES/immanuel.mo
+-rw-r--r--   0 robert     (501) staff       (20)     2130 2024-04-23 00:05:08.000000 immanuel-1.3.3/immanuel/locales/es_ES/mappings.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.130160 immanuel-1.3.3/immanuel/locales/pt_BR/
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.130720 immanuel-1.3.3/immanuel/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 robert     (501) staff       (20)     8005 2024-04-15 00:27:49.000000 immanuel-1.3.3/immanuel/locales/pt_BR/LC_MESSAGES/immanuel.mo
+-rw-r--r--   0 robert     (501) staff       (20)     2065 2024-04-23 00:05:21.000000 immanuel-1.3.3/immanuel/locales/pt_BR/mappings.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.132623 immanuel-1.3.3/immanuel/reports/
+-rw-r--r--   0 robert     (501) staff       (20)     4658 2024-04-16 01:27:34.000000 immanuel-1.3.3/immanuel/reports/aspect.py
+-rw-r--r--   0 robert     (501) staff       (20)     7581 2024-04-16 01:27:34.000000 immanuel-1.3.3/immanuel/reports/dignity.py
+-rw-r--r--   0 robert     (501) staff       (20)     2186 2024-04-16 01:27:34.000000 immanuel-1.3.3/immanuel/reports/pattern.py
+-rw-r--r--   0 robert     (501) staff       (20)     1497 2024-01-16 22:54:01.000000 immanuel-1.3.3/immanuel/reports/weighting.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.089609 immanuel-1.3.3/immanuel/resources/
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.175200 immanuel-1.3.3/immanuel/resources/ephemeris/
+-rw-r--r--   0 robert     (501) staff       (20)   225863 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/seas_12.se1
+-rw-r--r--   0 robert     (501) staff       (20)   225440 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/seas_18.se1
+-rw-r--r--   0 robert     (501) staff       (20)   225108 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/seas_24.se1
+-rw-r--r--   0 robert     (501) staff       (20)  1306782 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/semo_12.se1
+-rw-r--r--   0 robert     (501) staff       (20)  1305686 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/semo_18.se1
+-rw-r--r--   0 robert     (501) staff       (20)  1309017 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/semo_24.se1
+-rw-r--r--   0 robert     (501) staff       (20)  1326257 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/semo_36.se1
+-rw-r--r--   0 robert     (501) staff       (20)  1339659 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/semo_42.se1
+-rw-r--r--   0 robert     (501) staff       (20)   483763 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/sepl_12.se1
+-rw-r--r--   0 robert     (501) staff       (20)   484065 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/sepl_18.se1
+-rw-r--r--   0 robert     (501) staff       (20)   483399 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/sepl_24.se1
+-rw-r--r--   0 robert     (501) staff       (20)   484686 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/sepl_36.se1
+-rw-r--r--   0 robert     (501) staff       (20)   483628 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/sepl_42.se1
+-rw-r--r--   0 robert     (501) staff       (20)    12066 2024-04-21 20:24:34.000000 immanuel-1.3.3/immanuel/setup.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.179799 immanuel-1.3.3/immanuel/tools/
+-rw-r--r--   0 robert     (501) staff       (20)     4211 2024-04-26 01:06:56.000000 immanuel-1.3.3/immanuel/tools/calculate.py
+-rw-r--r--   0 robert     (501) staff       (20)     6023 2024-01-16 22:54:01.000000 immanuel-1.3.3/immanuel/tools/convert.py
+-rw-r--r--   0 robert     (501) staff       (20)     3181 2024-01-17 23:18:15.000000 immanuel-1.3.3/immanuel/tools/date.py
+-rw-r--r--   0 robert     (501) staff       (20)    21046 2024-04-21 20:24:34.000000 immanuel-1.3.3/immanuel/tools/ephemeris.py
+-rw-r--r--   0 robert     (501) staff       (20)     5702 2024-04-09 19:59:42.000000 immanuel-1.3.3/immanuel/tools/find.py
+-rw-r--r--   0 robert     (501) staff       (20)     2027 2024-01-16 22:54:01.000000 immanuel-1.3.3/immanuel/tools/forecast.py
+-rw-r--r--   0 robert     (501) staff       (20)     1824 2024-01-16 22:54:01.000000 immanuel-1.3.3/immanuel/tools/midpoint.py
+-rw-r--r--   0 robert     (501) staff       (20)     2709 2024-04-22 00:25:50.000000 immanuel-1.3.3/immanuel/tools/position.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.193389 immanuel-1.3.3/immanuel.egg-info/
+-rw-r--r--   0 robert     (501) staff       (20)    47556 2024-04-26 02:31:28.000000 immanuel-1.3.3/immanuel.egg-info/PKG-INFO
+-rw-r--r--   0 robert     (501) staff       (20)     1894 2024-04-26 02:31:29.000000 immanuel-1.3.3/immanuel.egg-info/SOURCES.txt
+-rw-r--r--   0 robert     (501) staff       (20)        1 2024-04-26 02:31:28.000000 immanuel-1.3.3/immanuel.egg-info/dependency_links.txt
+-rw-r--r--   0 robert     (501) staff       (20)       60 2024-04-26 02:31:28.000000 immanuel-1.3.3/immanuel.egg-info/requires.txt
+-rw-r--r--   0 robert     (501) staff       (20)        9 2024-04-26 02:31:28.000000 immanuel-1.3.3/immanuel.egg-info/top_level.txt
+-rw-r--r--   0 robert     (501) staff       (20)     1070 2024-04-26 02:27:12.000000 immanuel-1.3.3/pyproject.toml
+-rw-r--r--   0 robert     (501) staff       (20)       38 2024-04-26 02:31:29.194646 immanuel-1.3.3/setup.cfg
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.192888 immanuel-1.3.3/tests/
+-rw-r--r--   0 robert     (501) staff       (20)    40905 2023-12-02 01:56:03.000000 immanuel-1.3.3/tests/se01181s.se1
+-rw-r--r--   0 robert     (501) staff       (20)     3920 2024-04-21 20:24:34.000000 immanuel-1.3.3/tests/test_aspect.py
+-rw-r--r--   0 robert     (501) staff       (20)     3530 2024-04-21 20:24:34.000000 immanuel-1.3.3/tests/test_calculate.py
+-rw-r--r--   0 robert     (501) staff       (20)    23308 2024-04-21 20:24:34.000000 immanuel-1.3.3/tests/test_charts.py
+-rw-r--r--   0 robert     (501) staff       (20)    28783 2024-01-17 23:16:08.000000 immanuel-1.3.3/tests/test_convert.py
+-rw-r--r--   0 robert     (501) staff       (20)     4579 2024-01-17 23:18:15.000000 immanuel-1.3.3/tests/test_date.py
+-rw-r--r--   0 robert     (501) staff       (20)     9521 2024-04-16 01:27:34.000000 immanuel-1.3.3/tests/test_dignity.py
+-rw-r--r--   0 robert     (501) staff       (20)    15068 2024-04-21 20:24:34.000000 immanuel-1.3.3/tests/test_ephemeris.py
+-rw-r--r--   0 robert     (501) staff       (20)     3714 2024-01-20 20:35:37.000000 immanuel-1.3.3/tests/test_find.py
+-rw-r--r--   0 robert     (501) staff       (20)     6735 2024-01-20 20:36:29.000000 immanuel-1.3.3/tests/test_forecast.py
+-rw-r--r--   0 robert     (501) staff       (20)    18927 2024-04-21 20:24:34.000000 immanuel-1.3.3/tests/test_localization.py
+-rw-r--r--   0 robert     (501) staff       (20)     5374 2024-04-21 20:24:34.000000 immanuel-1.3.3/tests/test_midpoint.py
+-rw-r--r--   0 robert     (501) staff       (20)     2393 2024-01-16 22:54:01.000000 immanuel-1.3.3/tests/test_pattern.py
+-rw-r--r--   0 robert     (501) staff       (20)     5157 2024-04-21 20:24:34.000000 immanuel-1.3.3/tests/test_position.py
+-rw-r--r--   0 robert     (501) staff       (20)     3169 2024-04-16 01:27:34.000000 immanuel-1.3.3/tests/test_setup.py
+-rw-r--r--   0 robert     (501) staff       (20)     2286 2024-04-01 00:40:36.000000 immanuel-1.3.3/tests/test_weighting.py
```

### Comparing `immanuel-1.3.2/LICENSE.md` & `immanuel-1.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/PKG-INFO` & `immanuel-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: immanuel
-Version: 1.3.2
+Version: 1.3.3
 Summary: Quickly produce both human-readable and JSON-formatted astrology chart data based on the Swiss Ephemeris and astro.com.
 Author-email: Robert Davies <robert@theriftlab.com>
 License: # GNU AFFERO GENERAL PUBLIC LICENSE
         
         Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -646,27 +646,27 @@
 
 Immanuel is a Python >= 3.10 package to painlessly provide your application with simple yet detailed chart-centric astrology data for planets, points, signs, houses, aspects, weightings, etc. all based on the [Swiss Ephemeris](https://github.com/astrorigin/pyswisseph). Extra calculations, notably secondary progressions and dignity scores, are modeled on those of [astro.com](https://astro.com) and [Astro Gold](https://www.astrogold.io).
 
 Data for natal charts, solar returns, progressions, and composites are available, as well as the ability to point the aspects from any one chart instance to the planets in another, creating a flexible method to build synastries.
 
 Simply pass in a date and coordinates to one of the available chart classes, and the returned instance will contain all data necessary to construct a full astrological chart. A serializer is bundled to easily output all data as JSON, or it can simply be printed out as human-readable text.
 
-## Documentation
-
-Full documentation is available [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.1/docs/0-contents.md), or follow the Quick Start below to see how to quickly generate a natal chart.
-
 ## Translations
 
-Immanuel is currently available in the following locales / languages:
+Immanuel's output is currently available in the following locales / languages:
 
 * **en_US:** (default) US English
 * **pt_BR:** Brazilian Portuguese
-* Coming soon: Spanish translation
+* **es_ES:** Spanish
+
+See [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.3/docs/5-settings.md#locale) for details on how to switch. The documentation itself is not currently available in other translations. To contribute in-software translations, see [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.3/docs/7-contributions.md).
+
+## Documentation
 
-See [the documentation](https://github.com/theriftlab/immanuel-python/tree/v1.3.1/docs/5-settings.md#locale) on how to switch. The documentation itself is not currently available in other translations. To contribute translations, see [below](#contributions).
+Full documentation is available [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.3/docs/0-contents.md), or follow the Quick Start below to see how to quickly generate a natal chart.
 
 ## Quick Start
 
 You can get started with full natal chart data in minutes. Simply install Immanuel:
 
 ```bash
 pip install immanuel
@@ -689,24 +689,24 @@
 for object in natal.objects.values():
     print(object)
 ```
 
 This will output all the chart objects (planets, points, asteroids etc.) in this format:
 
 ```
-Sun 10°37'26" in Capricorn, 11th House, Direct
-Moon 16°19'29" in Scorpio, 8th House, Direct
-Mercury 02°16'43" in Capricorn, 10th House, Direct
-Venus 01°52'05" in Sagittarius, 9th House, Direct
-Mars 28°09'26" in Aquarius, 12th House, Direct
-Jupiter 25°15'48" in Aries, 2nd House, Direct
+Sun 10°37'26" in Capricorn, 11th House
+Moon 16°19'29" in Scorpio, 8th House
+Mercury 02°16'43" in Capricorn, 10th House
+Venus 01°52'05" in Sagittarius, 9th House
+Mars 28°09'26" in Aquarius, 12th House
+Jupiter 25°15'48" in Aries, 2nd House
 Saturn 10°23'27" in Taurus, 2nd House, Retrograde
-Uranus 14°49'19" in Aquarius, 12th House, Direct
-Neptune 03°12'07" in Aquarius, 12th House, Direct
-Pluto 11°27'49" in Sagittarius, 9th House, Direct
+Uranus 14°49'19" in Aquarius, 12th House
+Neptune 03°12'07" in Aquarius, 12th House
+Pluto 11°27'49" in Sagittarius, 9th House
 ...
 ```
 
 Add asteroid Ceres into the mix:
 
 ```python
 from immanuel import charts
@@ -726,15 +726,15 @@
 for object in natal.objects.values():
     print(object)
 ```
 
 Now you will see this appended to the list:
 
 ```
-Ceres 04°30'28" in Libra, 7th House, Direct
+Ceres 04°30'28" in Libra, 7th House
 ```
 
 More on the settings & constants in the full documentation - for now, we can see much more data by serializing the chart's `objects` property to JSON like this:
 
 ```python
 import json
 
@@ -882,14 +882,15 @@
 
 Planetary dignity scores are based on those of Astro Gold, although these are somewhat flexible via the settings.
 
 ## Settings
 
 The full documentation covers settings in detail, but much of the output can be customized. The settings class allows you to specify and personalize:
 
+* Locale / language
 * The house system to use
 * What data each chart returns
 * What planets, points, asteroid etc. to include
 * Details of the aspect calculations
 * Which dignities to use and their scores
 * The progression method to use for secondary progressions
 * ...and much more.
@@ -908,34 +909,12 @@
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the [GNU Affero General Public License](LICENSE.md) for more details.
 
 ## Credits
 
 Immanuel is forever indebted to the pioneering work of Alois Treindl and Dieter Koch at Astrodienst, and to João Ventura for the incredibly detailed [flatlib](https://github.com/flatangle/flatlib) which first inspired the development of this package.
 
-A big thank-you goes to Nathan Octavio who suggested translations, and who translated Immanuel into Brazilian Portuguese.
-
-## Contributions
-
-New translations for Immanuel's output are always welcome, although it is currently geared to Western-European languages. If you would like to contribute a translation, follow these steps:
-
-* Fork the repo.
-* Create a branch named after the locale, eg. `translations/pr_BR` - locale names for various languages can be found online, for example [here](https://learn.microsoft.com/en-us/openspecs/office_standards/ms-oe376/6c085406-a698-4e12-9d4d-c3b0ee3dbc4a), although you should use an underscore rather than a hyphen.
-* Create a subdirectory in `/immanuel/locales` named after your locale code, and another sub-directory under this called `LC_MESSAGES`.
-* Copy `locales/immanuel.pot` into the new `LC_MESSAGES` sub-directory and rename it `immanuel.po`.
-* Within `immanuel.po`, for every English word or sentence in a `msgid` string, if there is a direct translation in your language, enter it in the following empty `msgstr`. For gendered adjectives, you will need to add all gendered variants using `msgctxt` like this:
-```
-msgctxt "masculine"
-msgid "Applicative"
-msgstr "Aplicativo"
-
-msgctxt "feminine"
-msgid "Applicative"
-msgstr "Aplicativa"
-```
-* To map genders, a file `mappings.py` will need to be created under your new locale directory alongside `LC_MESSAGES`. See existing mapping files for an example of how to assign all of Immanuel's objects a gender for your language.
-* Once all translations and gender-mapping is complete, you can either compile your `.po` file to an `.mo` file or simply leave this out and I will compile it. Commit your changes and create a pull request.
-* If everything looks good, I will merge to master & prep a new release!
+A big thank-you goes to Nathan Octavio who suggested translations, and who translated Immanuel into both Brazilian Portuguese and Spanish.
 
 ## Contact
 
 Please post any issues, feature requests, PRs etc. on GitHub. For anything else email robert@theriftlab.com.
```

### Comparing `immanuel-1.3.2/README.md` & `immanuel-1.3.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 
 Immanuel is a Python >= 3.10 package to painlessly provide your application with simple yet detailed chart-centric astrology data for planets, points, signs, houses, aspects, weightings, etc. all based on the [Swiss Ephemeris](https://github.com/astrorigin/pyswisseph). Extra calculations, notably secondary progressions and dignity scores, are modeled on those of [astro.com](https://astro.com) and [Astro Gold](https://www.astrogold.io).
 
 Data for natal charts, solar returns, progressions, and composites are available, as well as the ability to point the aspects from any one chart instance to the planets in another, creating a flexible method to build synastries.
 
 Simply pass in a date and coordinates to one of the available chart classes, and the returned instance will contain all data necessary to construct a full astrological chart. A serializer is bundled to easily output all data as JSON, or it can simply be printed out as human-readable text.
 
-## Documentation
-
-Full documentation is available [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.1/docs/0-contents.md), or follow the Quick Start below to see how to quickly generate a natal chart.
-
 ## Translations
 
-Immanuel is currently available in the following locales / languages:
+Immanuel's output is currently available in the following locales / languages:
 
 * **en_US:** (default) US English
 * **pt_BR:** Brazilian Portuguese
-* Coming soon: Spanish translation
+* **es_ES:** Spanish
+
+See [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.3/docs/5-settings.md#locale) for details on how to switch. The documentation itself is not currently available in other translations. To contribute in-software translations, see [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.3/docs/7-contributions.md).
+
+## Documentation
 
-See [the documentation](https://github.com/theriftlab/immanuel-python/tree/v1.3.1/docs/5-settings.md#locale) on how to switch. The documentation itself is not currently available in other translations. To contribute translations, see [below](#contributions).
+Full documentation is available [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.3/docs/0-contents.md), or follow the Quick Start below to see how to quickly generate a natal chart.
 
 ## Quick Start
 
 You can get started with full natal chart data in minutes. Simply install Immanuel:
 
 ```bash
 pip install immanuel
@@ -52,24 +52,24 @@
 for object in natal.objects.values():
     print(object)
 ```
 
 This will output all the chart objects (planets, points, asteroids etc.) in this format:
 
 ```
-Sun 10°37'26" in Capricorn, 11th House, Direct
-Moon 16°19'29" in Scorpio, 8th House, Direct
-Mercury 02°16'43" in Capricorn, 10th House, Direct
-Venus 01°52'05" in Sagittarius, 9th House, Direct
-Mars 28°09'26" in Aquarius, 12th House, Direct
-Jupiter 25°15'48" in Aries, 2nd House, Direct
+Sun 10°37'26" in Capricorn, 11th House
+Moon 16°19'29" in Scorpio, 8th House
+Mercury 02°16'43" in Capricorn, 10th House
+Venus 01°52'05" in Sagittarius, 9th House
+Mars 28°09'26" in Aquarius, 12th House
+Jupiter 25°15'48" in Aries, 2nd House
 Saturn 10°23'27" in Taurus, 2nd House, Retrograde
-Uranus 14°49'19" in Aquarius, 12th House, Direct
-Neptune 03°12'07" in Aquarius, 12th House, Direct
-Pluto 11°27'49" in Sagittarius, 9th House, Direct
+Uranus 14°49'19" in Aquarius, 12th House
+Neptune 03°12'07" in Aquarius, 12th House
+Pluto 11°27'49" in Sagittarius, 9th House
 ...
 ```
 
 Add asteroid Ceres into the mix:
 
 ```python
 from immanuel import charts
@@ -89,15 +89,15 @@
 for object in natal.objects.values():
     print(object)
 ```
 
 Now you will see this appended to the list:
 
 ```
-Ceres 04°30'28" in Libra, 7th House, Direct
+Ceres 04°30'28" in Libra, 7th House
 ```
 
 More on the settings & constants in the full documentation - for now, we can see much more data by serializing the chart's `objects` property to JSON like this:
 
 ```python
 import json
 
@@ -245,14 +245,15 @@
 
 Planetary dignity scores are based on those of Astro Gold, although these are somewhat flexible via the settings.
 
 ## Settings
 
 The full documentation covers settings in detail, but much of the output can be customized. The settings class allows you to specify and personalize:
 
+* Locale / language
 * The house system to use
 * What data each chart returns
 * What planets, points, asteroid etc. to include
 * Details of the aspect calculations
 * Which dignities to use and their scores
 * The progression method to use for secondary progressions
 * ...and much more.
@@ -271,34 +272,12 @@
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the [GNU Affero General Public License](LICENSE.md) for more details.
 
 ## Credits
 
 Immanuel is forever indebted to the pioneering work of Alois Treindl and Dieter Koch at Astrodienst, and to João Ventura for the incredibly detailed [flatlib](https://github.com/flatangle/flatlib) which first inspired the development of this package.
 
-A big thank-you goes to Nathan Octavio who suggested translations, and who translated Immanuel into Brazilian Portuguese.
-
-## Contributions
-
-New translations for Immanuel's output are always welcome, although it is currently geared to Western-European languages. If you would like to contribute a translation, follow these steps:
-
-* Fork the repo.
-* Create a branch named after the locale, eg. `translations/pr_BR` - locale names for various languages can be found online, for example [here](https://learn.microsoft.com/en-us/openspecs/office_standards/ms-oe376/6c085406-a698-4e12-9d4d-c3b0ee3dbc4a), although you should use an underscore rather than a hyphen.
-* Create a subdirectory in `/immanuel/locales` named after your locale code, and another sub-directory under this called `LC_MESSAGES`.
-* Copy `locales/immanuel.pot` into the new `LC_MESSAGES` sub-directory and rename it `immanuel.po`.
-* Within `immanuel.po`, for every English word or sentence in a `msgid` string, if there is a direct translation in your language, enter it in the following empty `msgstr`. For gendered adjectives, you will need to add all gendered variants using `msgctxt` like this:
-```
-msgctxt "masculine"
-msgid "Applicative"
-msgstr "Aplicativo"
-
-msgctxt "feminine"
-msgid "Applicative"
-msgstr "Aplicativa"
-```
-* To map genders, a file `mappings.py` will need to be created under your new locale directory alongside `LC_MESSAGES`. See existing mapping files for an example of how to assign all of Immanuel's objects a gender for your language.
-* Once all translations and gender-mapping is complete, you can either compile your `.po` file to an `.mo` file or simply leave this out and I will compile it. Commit your changes and create a pull request.
-* If everything looks good, I will merge to master & prep a new release!
+A big thank-you goes to Nathan Octavio who suggested translations, and who translated Immanuel into both Brazilian Portuguese and Spanish.
 
 ## Contact
 
 Please post any issues, feature requests, PRs etc. on GitHub. For anything else email robert@theriftlab.com.
```

### Comparing `immanuel-1.3.2/immanuel/charts.py` & `immanuel-1.3.3/immanuel/charts.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/classes/cache.py` & `immanuel-1.3.3/immanuel/classes/cache.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/classes/localize.py` & `immanuel-1.3.3/immanuel/classes/localize.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/classes/serialize.py` & `immanuel-1.3.3/immanuel/classes/serialize.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/classes/wrap.py` & `immanuel-1.3.3/immanuel/classes/wrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,26 +231,27 @@
                 longitude=self.sign_longitude,
                 sign=self.sign,
             )
 
         if hasattr(self, 'house'):
             formatted += f', {_(self.house)}'
 
-        if hasattr(self, 'movement'):
+        if hasattr(self, 'movement') and (settings.output_typical_object_motion or not self.movement.typical):
             formatted += f', {_(self.movement)}'
 
         return formatted
 
 
 class ObjectMovement:
     def __init__(self, object: dict) -> None:
         self._movement = calculate.object_movement(object)
         self.direct = self._movement == calc.DIRECT
         self.stationary = self._movement == calc.STATIONARY
         self.retrograde = self._movement == calc.RETROGRADE
+        self.typical = calculate.object_movement_typical(object)
         self.formatted = _(names.OBJECT_MOVEMENTS[self._movement], gender(object['index']))
 
     def __str__(self) -> str:
         return self.formatted
 
 
 class ObjectType:
```

### Comparing `immanuel-1.3.2/immanuel/const/calc.py` & `immanuel-1.3.3/immanuel/const/calc.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,14 +71,18 @@
 BALSAMIC = 360
 
 """ Object movements. """
 DIRECT = 0
 RETROGRADE = 1
 STATIONARY = 2
 
+""" Relative planetary rising / setting. """
+OCCIDENTAL = 0
+ORIENTAL = 1
+
 """ MC progression formulae. """
 NAIBOD = 0
 SOLAR_ARC = 1
 DAILY_HOUSES = 2
 
 """ Part of Fortune formulae. """
 DAY_FORMULA = 0
```

### Comparing `immanuel-1.3.2/immanuel/const/chart.py` & `immanuel-1.3.3/immanuel/const/chart.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/const/data.py` & `immanuel-1.3.3/immanuel/const/data.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/const/dignities.py` & `immanuel-1.3.3/immanuel/const/dignities.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/const/names.py` & `immanuel-1.3.3/immanuel/const/names.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/locales/pt_BR/LC_MESSAGES/immanuel.mo` & `immanuel-1.3.3/immanuel/locales/pt_BR/LC_MESSAGES/immanuel.mo`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/locales/pt_BR/mappings.py` & `immanuel-1.3.3/immanuel/locales/pt_BR/mappings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
     This file is part of immanuel - (C) The Rift Lab
-    Author: Robert Davies (robert@theriftlab.com)
+    Authors: Robert Davies (robert@theriftlab.com) and Nathan Octavio
 
 
     Gendered list of relevant nouns for correct adjective translation.
 
 """
 
 from immanuel.const import calc, chart, genders
```

### Comparing `immanuel-1.3.2/immanuel/reports/aspect.py` & `immanuel-1.3.3/immanuel/reports/aspect.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/reports/dignity.py` & `immanuel-1.3.3/immanuel/reports/dignity.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/reports/pattern.py` & `immanuel-1.3.3/immanuel/reports/pattern.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/reports/weighting.py` & `immanuel-1.3.3/immanuel/reports/weighting.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/resources/ephemeris/seas_12.se1` & `immanuel-1.3.3/immanuel/resources/ephemeris/seas_12.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/resources/ephemeris/seas_18.se1` & `immanuel-1.3.3/immanuel/resources/ephemeris/seas_18.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/resources/ephemeris/seas_24.se1` & `immanuel-1.3.3/immanuel/resources/ephemeris/seas_24.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/resources/ephemeris/semo_12.se1` & `immanuel-1.3.3/immanuel/resources/ephemeris/semo_12.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/resources/ephemeris/semo_18.se1` & `immanuel-1.3.3/immanuel/resources/ephemeris/semo_18.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/resources/ephemeris/semo_24.se1` & `immanuel-1.3.3/immanuel/resources/ephemeris/semo_24.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/resources/ephemeris/semo_36.se1` & `immanuel-1.3.3/immanuel/resources/ephemeris/semo_36.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/resources/ephemeris/semo_42.se1` & `immanuel-1.3.3/immanuel/resources/ephemeris/semo_42.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/resources/ephemeris/sepl_12.se1` & `immanuel-1.3.3/immanuel/resources/ephemeris/sepl_12.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/resources/ephemeris/sepl_18.se1` & `immanuel-1.3.3/immanuel/resources/ephemeris/sepl_18.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/resources/ephemeris/sepl_24.se1` & `immanuel-1.3.3/immanuel/resources/ephemeris/sepl_24.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/resources/ephemeris/sepl_36.se1` & `immanuel-1.3.3/immanuel/resources/ephemeris/sepl_36.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/resources/ephemeris/sepl_42.se1` & `immanuel-1.3.3/immanuel/resources/ephemeris/sepl_42.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/setup.py` & `immanuel-1.3.3/immanuel/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,19 @@
 
         """ Default coordinates when none are supplied. Currently points to
         the GMT prime meridian. """
         self.default_latitude = 51.4779
 
         self.default_longitude = -0.0015
 
+        """ Whether or not the stringified output of chart objects should
+        always display the object's motion even when it is typical for
+        that object. """
+        self.output_typical_object_motion = False
+
         """ House system as supported by pyswisseph. """
         self.house_system = chart.PLACIDUS
 
         """ Which planets, points etc. to show. """
         self.objects = [
             chart.ASC, chart.DESC, chart.MC, chart.IC,
             chart.TRUE_NORTH_NODE, chart.TRUE_SOUTH_NODE,
```

### Comparing `immanuel-1.3.2/immanuel/tools/calculate.py` & `immanuel-1.3.3/immanuel/tools/calculate.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     and object information from the data returned from the ephemeris module.
     These functions will accept both an object and a float.
 
 """
 
 import swisseph as swe
 
-from immanuel.const import calc
+from immanuel.const import calc, chart
 from immanuel.tools import ephemeris
 
 
 def moon_phase(sun: dict | float, moon: dict | float) -> int:
     """ Returns the moon phase given the positions of the Sun and Moon. """
     sun_lon, moon_lon = (object['lon'] if isinstance(object, dict) else object for object in (sun, moon))
     distance = swe.difdegn(moon_lon, sun_lon)
@@ -54,14 +54,34 @@
 
     if -calc.STATION_SPEED <= speed <= calc.STATION_SPEED:
         return calc.STATIONARY
 
     return calc.DIRECT if speed > calc.STATION_SPEED else calc.RETROGRADE
 
 
+def object_movement_typical(object: dict) -> bool:
+    """ Returns whether an object's movement is typical, ie. direct for planets,
+    retrograde for nodes, stationary for Part of Fortune and eclipses. """
+    if object['index'] in (chart.PARS_FORTUNA, chart.PRE_NATAL_SOLAR_ECLIPSE, chart.PRE_NATAL_LUNAR_ECLIPSE, chart.POST_NATAL_SOLAR_ECLIPSE, chart.POST_NATAL_SOLAR_ECLIPSE):
+        return object['speed'] == 0.0
+
+    movement = object_movement(object)
+    is_node = object['index'] in (chart.NORTH_NODE, chart.SOUTH_NODE, chart.TRUE_NORTH_NODE, chart.TRUE_SOUTH_NODE)
+
+    return movement == calc.RETROGRADE if is_node else movement == calc.DIRECT
+
+
+def relative_position(object1: dict | float, object2: dict | float) -> int:
+    """ Calculate which side of object1 object2 is. """
+    lon1 = object1['lon'] if isinstance(object1, dict) else object1
+    lon2 = object2['lon'] if isinstance(object2, dict) else object2
+
+    return calc.OCCIDENTAL if swe.difdegn(lon1, lon2) > 180 else calc.ORIENTAL
+
+
 def is_out_of_bounds(object: dict | float, jd: float = None, obliquity: float = None) -> bool:
     """ Returns whether the passed object is out of bounds either on the passed
     Julian date or relative to the passed obliquity. """
     if isinstance(object, dict):
         if 'dec' not in object:
             return None
         dec = object['dec']
```

### Comparing `immanuel-1.3.2/immanuel/tools/convert.py` & `immanuel-1.3.3/immanuel/tools/convert.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/tools/date.py` & `immanuel-1.3.3/immanuel/tools/date.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/tools/ephemeris.py` & `immanuel-1.3.3/immanuel/tools/ephemeris.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/tools/find.py` & `immanuel-1.3.3/immanuel/tools/find.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/tools/forecast.py` & `immanuel-1.3.3/immanuel/tools/forecast.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/tools/midpoint.py` & `immanuel-1.3.3/immanuel/tools/midpoint.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/immanuel/tools/position.py` & `immanuel-1.3.3/immanuel/tools/position.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 def sign(object: dict | float) -> int:
     """ Returns the index of the zodiac sign the
     passed object belongs to. """
     return int((object['lon'] if isinstance(object, dict) else object) / 30) + 1
 
 
 def sign_longitude(object: dict | float) -> tuple:
-    """ Returns the index of the zodiac sign the passed object
-    belongs to, and the sign-specific longitude inside it. """
+    """ Returns the sign-specific longitude. """
     return (object['lon'] if isinstance(object, dict) else object) % 30
 
 
 def opposite_sign(object: dict | float) -> int:
     """ Returns the index of the zodiac sign opposite
     where the passed object belongs to. """
     sign_number = sign(object)
```

### Comparing `immanuel-1.3.2/immanuel.egg-info/PKG-INFO` & `immanuel-1.3.3/immanuel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: immanuel
-Version: 1.3.2
+Version: 1.3.3
 Summary: Quickly produce both human-readable and JSON-formatted astrology chart data based on the Swiss Ephemeris and astro.com.
 Author-email: Robert Davies <robert@theriftlab.com>
 License: # GNU AFFERO GENERAL PUBLIC LICENSE
         
         Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -646,27 +646,27 @@
 
 Immanuel is a Python >= 3.10 package to painlessly provide your application with simple yet detailed chart-centric astrology data for planets, points, signs, houses, aspects, weightings, etc. all based on the [Swiss Ephemeris](https://github.com/astrorigin/pyswisseph). Extra calculations, notably secondary progressions and dignity scores, are modeled on those of [astro.com](https://astro.com) and [Astro Gold](https://www.astrogold.io).
 
 Data for natal charts, solar returns, progressions, and composites are available, as well as the ability to point the aspects from any one chart instance to the planets in another, creating a flexible method to build synastries.
 
 Simply pass in a date and coordinates to one of the available chart classes, and the returned instance will contain all data necessary to construct a full astrological chart. A serializer is bundled to easily output all data as JSON, or it can simply be printed out as human-readable text.
 
-## Documentation
-
-Full documentation is available [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.1/docs/0-contents.md), or follow the Quick Start below to see how to quickly generate a natal chart.
-
 ## Translations
 
-Immanuel is currently available in the following locales / languages:
+Immanuel's output is currently available in the following locales / languages:
 
 * **en_US:** (default) US English
 * **pt_BR:** Brazilian Portuguese
-* Coming soon: Spanish translation
+* **es_ES:** Spanish
+
+See [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.3/docs/5-settings.md#locale) for details on how to switch. The documentation itself is not currently available in other translations. To contribute in-software translations, see [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.3/docs/7-contributions.md).
+
+## Documentation
 
-See [the documentation](https://github.com/theriftlab/immanuel-python/tree/v1.3.1/docs/5-settings.md#locale) on how to switch. The documentation itself is not currently available in other translations. To contribute translations, see [below](#contributions).
+Full documentation is available [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.3/docs/0-contents.md), or follow the Quick Start below to see how to quickly generate a natal chart.
 
 ## Quick Start
 
 You can get started with full natal chart data in minutes. Simply install Immanuel:
 
 ```bash
 pip install immanuel
@@ -689,24 +689,24 @@
 for object in natal.objects.values():
     print(object)
 ```
 
 This will output all the chart objects (planets, points, asteroids etc.) in this format:
 
 ```
-Sun 10°37'26" in Capricorn, 11th House, Direct
-Moon 16°19'29" in Scorpio, 8th House, Direct
-Mercury 02°16'43" in Capricorn, 10th House, Direct
-Venus 01°52'05" in Sagittarius, 9th House, Direct
-Mars 28°09'26" in Aquarius, 12th House, Direct
-Jupiter 25°15'48" in Aries, 2nd House, Direct
+Sun 10°37'26" in Capricorn, 11th House
+Moon 16°19'29" in Scorpio, 8th House
+Mercury 02°16'43" in Capricorn, 10th House
+Venus 01°52'05" in Sagittarius, 9th House
+Mars 28°09'26" in Aquarius, 12th House
+Jupiter 25°15'48" in Aries, 2nd House
 Saturn 10°23'27" in Taurus, 2nd House, Retrograde
-Uranus 14°49'19" in Aquarius, 12th House, Direct
-Neptune 03°12'07" in Aquarius, 12th House, Direct
-Pluto 11°27'49" in Sagittarius, 9th House, Direct
+Uranus 14°49'19" in Aquarius, 12th House
+Neptune 03°12'07" in Aquarius, 12th House
+Pluto 11°27'49" in Sagittarius, 9th House
 ...
 ```
 
 Add asteroid Ceres into the mix:
 
 ```python
 from immanuel import charts
@@ -726,15 +726,15 @@
 for object in natal.objects.values():
     print(object)
 ```
 
 Now you will see this appended to the list:
 
 ```
-Ceres 04°30'28" in Libra, 7th House, Direct
+Ceres 04°30'28" in Libra, 7th House
 ```
 
 More on the settings & constants in the full documentation - for now, we can see much more data by serializing the chart's `objects` property to JSON like this:
 
 ```python
 import json
 
@@ -882,14 +882,15 @@
 
 Planetary dignity scores are based on those of Astro Gold, although these are somewhat flexible via the settings.
 
 ## Settings
 
 The full documentation covers settings in detail, but much of the output can be customized. The settings class allows you to specify and personalize:
 
+* Locale / language
 * The house system to use
 * What data each chart returns
 * What planets, points, asteroid etc. to include
 * Details of the aspect calculations
 * Which dignities to use and their scores
 * The progression method to use for secondary progressions
 * ...and much more.
@@ -908,34 +909,12 @@
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the [GNU Affero General Public License](LICENSE.md) for more details.
 
 ## Credits
 
 Immanuel is forever indebted to the pioneering work of Alois Treindl and Dieter Koch at Astrodienst, and to João Ventura for the incredibly detailed [flatlib](https://github.com/flatangle/flatlib) which first inspired the development of this package.
 
-A big thank-you goes to Nathan Octavio who suggested translations, and who translated Immanuel into Brazilian Portuguese.
-
-## Contributions
-
-New translations for Immanuel's output are always welcome, although it is currently geared to Western-European languages. If you would like to contribute a translation, follow these steps:
-
-* Fork the repo.
-* Create a branch named after the locale, eg. `translations/pr_BR` - locale names for various languages can be found online, for example [here](https://learn.microsoft.com/en-us/openspecs/office_standards/ms-oe376/6c085406-a698-4e12-9d4d-c3b0ee3dbc4a), although you should use an underscore rather than a hyphen.
-* Create a subdirectory in `/immanuel/locales` named after your locale code, and another sub-directory under this called `LC_MESSAGES`.
-* Copy `locales/immanuel.pot` into the new `LC_MESSAGES` sub-directory and rename it `immanuel.po`.
-* Within `immanuel.po`, for every English word or sentence in a `msgid` string, if there is a direct translation in your language, enter it in the following empty `msgstr`. For gendered adjectives, you will need to add all gendered variants using `msgctxt` like this:
-```
-msgctxt "masculine"
-msgid "Applicative"
-msgstr "Aplicativo"
-
-msgctxt "feminine"
-msgid "Applicative"
-msgstr "Aplicativa"
-```
-* To map genders, a file `mappings.py` will need to be created under your new locale directory alongside `LC_MESSAGES`. See existing mapping files for an example of how to assign all of Immanuel's objects a gender for your language.
-* Once all translations and gender-mapping is complete, you can either compile your `.po` file to an `.mo` file or simply leave this out and I will compile it. Commit your changes and create a pull request.
-* If everything looks good, I will merge to master & prep a new release!
+A big thank-you goes to Nathan Octavio who suggested translations, and who translated Immanuel into both Brazilian Portuguese and Spanish.
 
 ## Contact
 
 Please post any issues, feature requests, PRs etc. on GitHub. For anything else email robert@theriftlab.com.
```

### Comparing `immanuel-1.3.2/immanuel.egg-info/SOURCES.txt` & `immanuel-1.3.3/immanuel.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 immanuel/classes/wrap.py
 immanuel/const/calc.py
 immanuel/const/chart.py
 immanuel/const/data.py
 immanuel/const/dignities.py
 immanuel/const/genders.py
 immanuel/const/names.py
+immanuel/locales/es_ES/mappings.py
+immanuel/locales/es_ES/LC_MESSAGES/immanuel.mo
 immanuel/locales/pt_BR/mappings.py
 immanuel/locales/pt_BR/LC_MESSAGES/immanuel.mo
 immanuel/reports/aspect.py
 immanuel/reports/dignity.py
 immanuel/reports/pattern.py
 immanuel/reports/weighting.py
 immanuel/resources/ephemeris/seas_12.se1
```

### Comparing `immanuel-1.3.2/pyproject.toml` & `immanuel-1.3.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "immanuel"
-version = "1.3.2"
+version = "1.3.3"
 description = "Quickly produce both human-readable and JSON-formatted astrology chart data based on the Swiss Ephemeris and astro.com."
 authors = [
   { name = "Robert Davies", email = "robert@theriftlab.com" },
 ]
 license = { file = "LICENSE.md" }
 readme = "README.md"
 keywords = ["astrology", "api", "pyswisseph", "swisseph", "swiss ephemeris", "astro.com", "astro gold"]
```

### Comparing `immanuel-1.3.2/tests/se01181s.se1` & `immanuel-1.3.3/tests/se01181s.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/tests/test_aspect.py` & `immanuel-1.3.3/tests/test_aspect.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/tests/test_calculate.py` & `immanuel-1.3.3/tests/test_calculate.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/tests/test_charts.py` & `immanuel-1.3.3/tests/test_charts.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/tests/test_convert.py` & `immanuel-1.3.3/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/tests/test_date.py` & `immanuel-1.3.3/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/tests/test_dignity.py` & `immanuel-1.3.3/tests/test_dignity.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/tests/test_ephemeris.py` & `immanuel-1.3.3/tests/test_ephemeris.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/tests/test_find.py` & `immanuel-1.3.3/tests/test_find.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/tests/test_forecast.py` & `immanuel-1.3.3/tests/test_forecast.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/tests/test_localization.py` & `immanuel-1.3.3/tests/test_localization.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/tests/test_midpoint.py` & `immanuel-1.3.3/tests/test_midpoint.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/tests/test_pattern.py` & `immanuel-1.3.3/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/tests/test_position.py` & `immanuel-1.3.3/tests/test_position.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/tests/test_setup.py` & `immanuel-1.3.3/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.2/tests/test_weighting.py` & `immanuel-1.3.3/tests/test_weighting.py`

 * *Files identical despite different names*

