# Comparing `tmp/yabadaba-0.2.1.tar.gz` & `tmp/yabadaba-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\lmh1\Documents\Python-packages\yabadaba\dist\.tmp-xvwqrz8l\yabadaba-0.2.1.tar", last modified: Thu Jul 27 15:26:16 2023, max compression
+gzip compressed data, was "yabadaba-0.2.2.tar", last modified: Fri Apr 26 14:05:48 2024, max compression
```

## Comparing `yabadaba-0.2.1.tar` & `yabadaba-0.2.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/
--rw-rw-rw-   0        0        0     2776 2022-02-03 20:26:52.000000 yabadaba-0.2.1/LICENSE.TXT
--rw-rw-rw-   0        0        0     3636 2023-07-27 15:26:16.000000 yabadaba-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2868 2022-10-03 13:54:02.000000 yabadaba-0.2.1/README.rst
--rw-rw-rw-   0        0        0      108 2022-02-03 20:26:52.000000 yabadaba-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 15:26:16.000000 yabadaba-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1602 2023-07-27 15:25:08.000000 yabadaba-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/tests/
--rw-rw-rw-   0        0        0    11546 2022-03-03 19:56:36.000000 yabadaba-0.2.1/tests/test_Settings.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba/
--rw-rw-rw-   0        0        0    16425 2023-04-10 16:33:33.000000 yabadaba-0.2.1/yabadaba/Settings.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba/UnitConverter/
--rw-rw-rw-   0        0        0    19559 2023-03-28 18:17:55.000000 yabadaba-0.2.1/yabadaba/UnitConverter/__init__.py
--rw-rw-rw-   0        0        0      360 2023-03-22 16:04:46.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_acceleration.py
--rw-rw-rw-   0        0        0      853 2023-03-22 16:08:23.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_capacitance.py
--rw-rw-rw-   0        0        0      430 2023-03-22 16:10:01.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_charge.py
--rw-rw-rw-   0        0        0     1018 2023-03-22 14:52:27.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_concentration.py
--rw-rw-rw-   0        0        0     4403 2023-03-22 15:46:30.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_constants.py
--rw-rw-rw-   0        0        0      508 2023-03-22 16:14:00.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_current.py
--rw-rw-rw-   0        0        0     1930 2023-03-22 15:56:01.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_energy.py
--rw-rw-rw-   0        0        0     1004 2023-03-22 14:52:23.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_force.py
--rw-rw-rw-   0        0        0     1723 2023-03-22 16:15:59.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_frequency.py
--rw-rw-rw-   0        0        0     1764 2023-03-22 16:14:55.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_length.py
--rw-rw-rw-   0        0        0      871 2023-03-22 16:21:43.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_magnetic.py
--rw-rw-rw-   0        0        0      973 2023-03-22 14:44:22.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_mass.py
--rw-rw-rw-   0        0        0     1046 2023-03-22 16:25:12.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_power.py
--rw-rw-rw-   0        0        0     1337 2023-03-22 15:13:37.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_pressure.py
--rw-rw-rw-   0        0        0     1151 2023-03-22 16:29:43.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_resistance.py
--rw-rw-rw-   0        0        0      591 2023-03-22 16:32:05.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_temperature.py
--rw-rw-rw-   0        0        0      864 2023-03-22 14:44:23.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_time.py
--rw-rw-rw-   0        0        0      657 2023-03-22 16:34:29.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_voltage.py
--rw-rw-rw-   0        0        0      837 2023-03-22 14:44:25.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_volume.py
--rw-rw-rw-   0        0        0        5 2023-07-26 14:08:45.000000 yabadaba-0.2.1/yabadaba/VERSION
--rw-rw-rw-   0        0        0      949 2023-07-27 15:01:17.000000 yabadaba-0.2.1/yabadaba/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba/database/
--rw-rw-rw-   0        0        0    25382 2023-07-26 19:09:37.000000 yabadaba-0.2.1/yabadaba/database/CDCSDatabase.py
--rw-rw-rw-   0        0        0    21607 2023-05-24 01:58:18.000000 yabadaba-0.2.1/yabadaba/database/Database.py
--rw-rw-rw-   0        0        0    33742 2023-07-26 14:08:45.000000 yabadaba-0.2.1/yabadaba/database/LocalDatabase.py
--rw-rw-rw-   0        0        0    23457 2023-07-26 14:08:45.000000 yabadaba-0.2.1/yabadaba/database/MongoDatabase.py
--rw-rw-rw-   0        0        0      579 2022-03-31 17:23:57.000000 yabadaba-0.2.1/yabadaba/database/__init__.py
--rw-rw-rw-   0        0        0     2932 2023-05-30 15:03:22.000000 yabadaba-0.2.1/yabadaba/database/load_database.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba/demo/
--rw-rw-rw-   0        0        0     1928 2022-02-03 20:26:52.000000 yabadaba-0.2.1/yabadaba/demo/BadRecord.py
--rw-rw-rw-   0        0        0     4615 2023-03-28 14:18:59.000000 yabadaba-0.2.1/yabadaba/demo/FAQ.py
--rw-rw-rw-   0        0        0      448 2022-02-03 20:26:52.000000 yabadaba-0.2.1/yabadaba/demo/FAQ.xsd
--rw-rw-rw-   0        0        0      583 2022-02-03 20:26:52.000000 yabadaba-0.2.1/yabadaba/demo/FAQ.xsl
--rw-rw-rw-   0        0        0      649 2022-02-03 20:26:52.000000 yabadaba-0.2.1/yabadaba/demo/README.rst
--rw-rw-rw-   0        0        0        0 2022-02-03 20:26:52.000000 yabadaba-0.2.1/yabadaba/demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba/query/
--rw-rw-rw-   0        0        0     4185 2023-04-06 17:56:05.000000 yabadaba-0.2.1/yabadaba/query/DateMatchQuery.py
--rw-rw-rw-   0        0        0     6728 2023-04-06 17:55:54.000000 yabadaba-0.2.1/yabadaba/query/FloatMatchQuery.py
--rw-rw-rw-   0        0        0     4264 2023-04-06 17:55:46.000000 yabadaba-0.2.1/yabadaba/query/IntMatchQuery.py
--rw-rw-rw-   0        0        0     4571 2023-04-06 17:55:40.000000 yabadaba-0.2.1/yabadaba/query/ListContainsQuery.py
--rw-rw-rw-   0        0        0     5205 2023-04-06 17:56:14.000000 yabadaba-0.2.1/yabadaba/query/Query.py
--rw-rw-rw-   0        0        0     4641 2023-04-06 17:55:27.000000 yabadaba-0.2.1/yabadaba/query/StrContainsQuery.py
--rw-rw-rw-   0        0        0     4072 2023-04-06 17:55:21.000000 yabadaba-0.2.1/yabadaba/query/StrMatchQuery.py
--rw-rw-rw-   0        0        0     1949 2023-03-28 14:16:07.000000 yabadaba-0.2.1/yabadaba/query/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba/record/
--rw-rw-rw-   0        0        0    14645 2023-05-31 15:37:50.000000 yabadaba-0.2.1/yabadaba/record/Record.py
--rw-rw-rw-   0        0        0     1379 2023-05-30 15:05:24.000000 yabadaba-0.2.1/yabadaba/record/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba/tools/
--rw-rw-rw-   0        0        0     4980 2023-07-26 14:08:45.000000 yabadaba-0.2.1/yabadaba/tools/ModuleManager.py
--rw-rw-rw-   0        0        0      227 2022-03-01 22:40:28.000000 yabadaba-0.2.1/yabadaba/tools/__init__.py
--rw-rw-rw-   0        0        0      464 2022-03-01 22:41:57.000000 yabadaba-0.2.1/yabadaba/tools/screen_input.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba.egg-info/
--rw-rw-rw-   0        0        0     3636 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1771 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-02-03 20:58:36.000000 yabadaba-0.2.1/yabadaba.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       65 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba.egg-info/top_level.txt
+drwxr-xr-x   0 lmh1      (1000) lmh1      (1000)        0 2024-04-26 14:05:48.227737 yabadaba-0.2.2/
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     2760 2023-08-31 19:58:35.000000 yabadaba-0.2.2/LICENSE.TXT
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     3739 2024-04-26 14:05:48.225736 yabadaba-0.2.2/PKG-INFO
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     2805 2023-08-31 19:58:35.000000 yabadaba-0.2.2/README.rst
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      103 2023-08-31 19:58:35.000000 yabadaba-0.2.2/pyproject.toml
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)       38 2024-04-26 14:05:48.227737 yabadaba-0.2.2/setup.cfg
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     1555 2024-04-26 14:01:20.000000 yabadaba-0.2.2/setup.py
+drwxr-xr-x   0 lmh1      (1000) lmh1      (1000)        0 2024-04-26 14:05:48.176737 yabadaba-0.2.2/tests/
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)    11273 2023-08-31 19:58:35.000000 yabadaba-0.2.2/tests/test_Settings.py
+drwxr-xr-x   0 lmh1      (1000) lmh1      (1000)        0 2024-04-26 14:05:48.177740 yabadaba-0.2.2/yabadaba/
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)    15996 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/Settings.py
+drwxr-xr-x   0 lmh1      (1000) lmh1      (1000)        0 2024-04-26 14:05:48.205736 yabadaba-0.2.2/yabadaba/UnitConverter/
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)    19006 2023-12-12 19:09:19.000000 yabadaba-0.2.2/yabadaba/UnitConverter/__init__.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      342 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_acceleration.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      805 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_capacitance.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      407 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_charge.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      960 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_concentration.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     4209 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_constants.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      480 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_current.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     1826 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_energy.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      951 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_force.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     1638 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_frequency.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     1671 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_length.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      823 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_magnetic.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      920 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_mass.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      993 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_power.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     1264 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_pressure.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     1083 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_resistance.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      563 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_temperature.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      816 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_time.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      619 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_voltage.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      789 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/UnitConverter/_volume.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)        5 2024-04-26 14:00:36.000000 yabadaba-0.2.2/yabadaba/VERSION
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      918 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/__init__.py
+drwxr-xr-x   0 lmh1      (1000) lmh1      (1000)        0 2024-04-26 14:05:48.208736 yabadaba-0.2.2/yabadaba/database/
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)    29855 2023-11-02 18:46:41.000000 yabadaba-0.2.2/yabadaba/database/CDCSDatabase.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)    24260 2023-11-02 18:55:00.000000 yabadaba-0.2.2/yabadaba/database/Database.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)    36387 2023-11-02 18:56:21.000000 yabadaba-0.2.2/yabadaba/database/LocalDatabase.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)    24334 2023-11-02 18:47:07.000000 yabadaba-0.2.2/yabadaba/database/MongoDatabase.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      563 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/database/__init__.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     3158 2023-11-02 19:12:06.000000 yabadaba-0.2.2/yabadaba/database/load_database.py
+drwxr-xr-x   0 lmh1      (1000) lmh1      (1000)        0 2024-04-26 14:05:48.217736 yabadaba-0.2.2/yabadaba/demo/
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     1862 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/demo/BadRecord.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     4471 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/demo/FAQ.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      438 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/demo/FAQ.xsd
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      566 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/demo/FAQ.xsl
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      633 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/demo/README.rst
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)        0 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/demo/__init__.py
+drwxr-xr-x   0 lmh1      (1000) lmh1      (1000)        0 2024-04-26 14:05:48.221736 yabadaba-0.2.2/yabadaba/query/
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     4056 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/query/DateMatchQuery.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     6536 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/query/FloatMatchQuery.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     4131 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/query/IntMatchQuery.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     4432 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/query/ListContainsQuery.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     5044 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/query/Query.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     4500 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/query/StrContainsQuery.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     3947 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/query/StrMatchQuery.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     2105 2023-11-02 19:17:08.000000 yabadaba-0.2.2/yabadaba/query/__init__.py
+drwxr-xr-x   0 lmh1      (1000) lmh1      (1000)        0 2024-04-26 14:05:48.222736 yabadaba-0.2.2/yabadaba/record/
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)    14182 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/record/Record.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     1333 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/record/__init__.py
+drwxr-xr-x   0 lmh1      (1000) lmh1      (1000)        0 2024-04-26 14:05:48.224736 yabadaba-0.2.2/yabadaba/tools/
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     4934 2023-11-02 19:17:00.000000 yabadaba-0.2.2/yabadaba/tools/ModuleManager.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      221 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/tools/__init__.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      446 2023-08-31 19:58:35.000000 yabadaba-0.2.2/yabadaba/tools/screen_input.py
+drwxr-xr-x   0 lmh1      (1000) lmh1      (1000)        0 2024-04-26 14:05:48.224736 yabadaba-0.2.2/yabadaba.egg-info/
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     3739 2024-04-26 14:05:48.000000 yabadaba-0.2.2/yabadaba.egg-info/PKG-INFO
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     1771 2024-04-26 14:05:48.000000 yabadaba-0.2.2/yabadaba.egg-info/SOURCES.txt
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)        1 2024-04-26 14:05:48.000000 yabadaba-0.2.2/yabadaba.egg-info/dependency_links.txt
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)        1 2023-09-01 15:41:06.000000 yabadaba-0.2.2/yabadaba.egg-info/not-zip-safe
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)       65 2024-04-26 14:05:48.000000 yabadaba-0.2.2/yabadaba.egg-info/requires.txt
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)        9 2024-04-26 14:05:48.000000 yabadaba-0.2.2/yabadaba.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yabadaba-0.2.1/LICENSE.TXT` & `yabadaba-0.2.2/LICENSE.TXT`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Licensing
-=========
-
-License Information for NIST data (other than Standard Reference Data (SRD))
-
-This data was developed by employees of the National Institute of Standards and Technology (NIST), an agency of the Federal Government. Pursuant to title 15 United States Code Section 105, works of NIST employees are not subject to copyright protection in the United States and are considered to be in the public domain.
-
-The data is provided by NIST as a public service and is expressly provided “AS IS.” NIST MAKES NO WARRANTY OF ANY KIND, EXPRESS, IMPLIED OR STATUTORY, INCLUDING, WITHOUT LIMITATION, THE IMPLIED WARRANTY OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, NON-INFRINGEMENT AND DATA ACCURACY. NIST does not warrant or make any representations regarding the use of the data or the results thereof, including but not limited to the correctness, accuracy, reliability or usefulness of the data. NIST SHALL NOT BE LIABLE AND YOU HEREBY RELEASE NIST FROM LIABILITY FOR ANY INDIRECT, CONSEQUENTIAL, SPECIAL, OR INCIDENTAL DAMAGES (INCLUDING DAMAGES FOR LOSS OF BUSINESS PROFITS, BUSINESS INTERRUPTION, LOSS OF BUSINESS INFORMATION, AND THE LIKE), WHETHER ARISING IN TORT, CONTRACT, OR OTHERWISE, ARISING FROM OR RELATING TO THE DATA (OR THE USE OF OR INABILITY TO USE THIS DATA), EVEN IF NIST HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
-To the extent that NIST may hold copyright in countries other than the United States, you are hereby granted the non-exclusive irrevocable and unconditional right to print, publish, prepare derivative works and distribute the NIST data, in any medium, or authorize others to do so on your behalf, on a royalty-free basis throughout the World.
-
-You may improve, modify, and create derivative works of the data or any portion of the data, and you may copy and distribute such modifications or works. Modified works should carry a notice stating that you changed the data and should note the date and nature of any such change. Please explicitly acknowledge the National Institute of Standards and Technology as the source of the data.
-
-Permission to use this data is contingent upon your acceptance of the terms of this agreement and upon your providing appropriate acknowledgments of NIST’s creation of the data.
-
-Copyright Protection for NIST Standard Reference Data (SRD)
-
+Licensing
+=========
+
+License Information for NIST data (other than Standard Reference Data (SRD))
+
+This data was developed by employees of the National Institute of Standards and Technology (NIST), an agency of the Federal Government. Pursuant to title 15 United States Code Section 105, works of NIST employees are not subject to copyright protection in the United States and are considered to be in the public domain.
+
+The data is provided by NIST as a public service and is expressly provided “AS IS.” NIST MAKES NO WARRANTY OF ANY KIND, EXPRESS, IMPLIED OR STATUTORY, INCLUDING, WITHOUT LIMITATION, THE IMPLIED WARRANTY OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, NON-INFRINGEMENT AND DATA ACCURACY. NIST does not warrant or make any representations regarding the use of the data or the results thereof, including but not limited to the correctness, accuracy, reliability or usefulness of the data. NIST SHALL NOT BE LIABLE AND YOU HEREBY RELEASE NIST FROM LIABILITY FOR ANY INDIRECT, CONSEQUENTIAL, SPECIAL, OR INCIDENTAL DAMAGES (INCLUDING DAMAGES FOR LOSS OF BUSINESS PROFITS, BUSINESS INTERRUPTION, LOSS OF BUSINESS INFORMATION, AND THE LIKE), WHETHER ARISING IN TORT, CONTRACT, OR OTHERWISE, ARISING FROM OR RELATING TO THE DATA (OR THE USE OF OR INABILITY TO USE THIS DATA), EVEN IF NIST HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
+To the extent that NIST may hold copyright in countries other than the United States, you are hereby granted the non-exclusive irrevocable and unconditional right to print, publish, prepare derivative works and distribute the NIST data, in any medium, or authorize others to do so on your behalf, on a royalty-free basis throughout the World.
+
+You may improve, modify, and create derivative works of the data or any portion of the data, and you may copy and distribute such modifications or works. Modified works should carry a notice stating that you changed the data and should note the date and nature of any such change. Please explicitly acknowledge the National Institute of Standards and Technology as the source of the data.
+
+Permission to use this data is contingent upon your acceptance of the terms of this agreement and upon your providing appropriate acknowledgments of NIST’s creation of the data.
+
+Copyright Protection for NIST Standard Reference Data (SRD)
+
 Copyright protection on this compilation of data has been secured by the U.S. Department of Commerce in the United States and in other countries that are parties to the Universal Copyright Convention, pursuant to Section 290(e) of Title 15 of the United States Code. NIST Standard Reference Data (SRD); ©Copyright ©2013 by the U.S. Secretary of Commerce on behalf of the United States of America. All rights reserved.
```

### Comparing `yabadaba-0.2.1/PKG-INFO` & `yabadaba-0.2.2/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,64 @@
-Metadata-Version: 2.1
-Name: yabadaba
-Version: 0.2.1
-Summary: Yay, a base database! An abstraction layer allowing for common interactions with Mongo, CDCS and local directory databases and records.
-Home-page: https://github.com/usnistgov/yabadaba
-Author: Lucas Hale
-Author-email: lucas.hale@nist.gov
-Keywords: database,mongodb,CDCS
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Physics
-License-File: LICENSE.TXT
-
-========
-yabadaba
-========
-
-The yabadaba package (short for "Yay, a base database!") provides a mid-level
-abstraction layer for interacting with databases containing JSON/XML equivalent
-data records.  The primary purpose of the yabadaba package is to make it easy
-to design user-friendly Python packages that can access and store content in a
-variety of database types.
-
-In design, the yabadaba package consists of five major components:
-
-1. Database classes that provide pythonic APIs to interact with databases.  A
-   base Database class defines common method calls for interacting with the 
-   records in a database, such as querying, adding, modifying, and deleting
-   entries.   Child classes of Database are then defined that implement the
-   universal interaction methods for a given type of database. 
-
-2. A base Record class provides a template for interpreting single database
-   entries.  Developers are meant to specify unique Record classes for each
-   unique schema that is part of their project.  In this way, users can
-   interface with the data both in its raw format and using class-specific
-   methods and attributes.  Each Record class also allows for database query
-   operations to be defined that allow for filtering of any hosted records
-   based on meaningful fields of the Record's schema.
-
-3. A ModuleManager class is defined that helps treat the child classes of
-   the Database and Record classes in a modular fashion.  In particular, the
-   ModuleManagers allow for the code to work even if there are issues with any 
-   of the child classes, and make it possible for packages that import the 
-   managers to append their own child classes.
-
-4. Generic query methods are also provided that support the construction of the
-   record-specific query operations.  In short, these are meant to allow for
-   queries to operate efficiently across all of the database types and ideally
-   return identical responses despite the underlying infrastructure
-   differences.
-
-5. A Settings class is provided that makes it possible for users to save
-   access parameters for a database under a simple name that can then be
-   reloaded in a later session.
-
-Package developers that want to provide APIs to any associated databases can
-simply import the various components of yabadaba and define their own Record
-classes that are specific to their own data.  Users of the resulting packages
-can then easily explore the data, make their own copies, etc.
-
-
-Installation
-------------
-
-The yabadaba package can easily be installed using pip or conda-forge
-
-    pip install yabadaba
-
-or 
-    conda install -c conda-forge yabadaba
-
-Documentation
--------------
-
-Documentation can be found in the doc folder in the github repository.
-
-For support, post a issue to github or email lucas.hale@nist.gov.
+========
+yabadaba
+========
+
+The yabadaba package (short for "Yay, a base database!") provides a mid-level
+abstraction layer for interacting with databases containing JSON/XML equivalent
+data records.  The primary purpose of the yabadaba package is to make it easy
+to design user-friendly Python packages that can access and store content in a
+variety of database types.
+
+In design, the yabadaba package consists of five major components:
+
+1. Database classes that provide pythonic APIs to interact with databases.  A
+   base Database class defines common method calls for interacting with the 
+   records in a database, such as querying, adding, modifying, and deleting
+   entries.   Child classes of Database are then defined that implement the
+   universal interaction methods for a given type of database. 
+
+2. A base Record class provides a template for interpreting single database
+   entries.  Developers are meant to specify unique Record classes for each
+   unique schema that is part of their project.  In this way, users can
+   interface with the data both in its raw format and using class-specific
+   methods and attributes.  Each Record class also allows for database query
+   operations to be defined that allow for filtering of any hosted records
+   based on meaningful fields of the Record's schema.
+
+3. A ModuleManager class is defined that helps treat the child classes of
+   the Database and Record classes in a modular fashion.  In particular, the
+   ModuleManagers allow for the code to work even if there are issues with any 
+   of the child classes, and make it possible for packages that import the 
+   managers to append their own child classes.
+
+4. Generic query methods are also provided that support the construction of the
+   record-specific query operations.  In short, these are meant to allow for
+   queries to operate efficiently across all of the database types and ideally
+   return identical responses despite the underlying infrastructure
+   differences.
+
+5. A Settings class is provided that makes it possible for users to save
+   access parameters for a database under a simple name that can then be
+   reloaded in a later session.
+
+Package developers that want to provide APIs to any associated databases can
+simply import the various components of yabadaba and define their own Record
+classes that are specific to their own data.  Users of the resulting packages
+can then easily explore the data, make their own copies, etc.
+
+
+Installation
+------------
+
+The yabadaba package can easily be installed using pip or conda-forge
+
+    pip install yabadaba
+
+or 
+    conda install -c conda-forge yabadaba
+
+Documentation
+-------------
+
+Documentation can be found in the doc folder in the github repository.
+
+For support, post a issue to github or email lucas.hale@nist.gov.
```

### Comparing `yabadaba-0.2.1/setup.py` & `yabadaba-0.2.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from setuptools import setup, find_packages
-
-def getreadme():
-    """Fetches long description from the README file"""
-    with open('README.rst', encoding='utf-8') as readme_file:
-        return readme_file.read()
-
-def getversion():
-    """Fetches version information from VERSION file"""
-    with open('yabadaba/VERSION', encoding='utf-8') as version_file:
-        return version_file.read().strip()
-
-setup(name = 'yabadaba',
-      version = getversion(),
-      description = 'Yay, a base database! An abstraction layer allowing for common interactions with Mongo, CDCS and local directory databases and records.',
-      long_description = getreadme(),
-      classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Science/Research',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Topic :: Scientific/Engineering :: Physics'
-      ],
-      keywords = [
-        'database', 
-        'mongodb', 
-        'CDCS',
-      ],
-      url = 'https://github.com/usnistgov/yabadaba',
-      author = 'Lucas Hale',
-      author_email = 'lucas.hale@nist.gov',
-      packages = find_packages(),
-      install_requires = [
-        'lxml',
-        'DataModelDict',
-        'IPython',
-        'numpy', 
-        'pandas',
-        'cdcs>=0.2.1',
-        'pymongo',
-        'tqdm',
-      ],
-      package_data={'': ['*']},
-      zip_safe = False)
+from setuptools import setup, find_packages
+
+def getreadme():
+    """Fetches long description from the README file"""
+    with open('README.rst', encoding='utf-8') as readme_file:
+        return readme_file.read()
+
+def getversion():
+    """Fetches version information from VERSION file"""
+    with open('yabadaba/VERSION', encoding='utf-8') as version_file:
+        return version_file.read().strip()
+
+setup(name = 'yabadaba',
+      version = getversion(),
+      description = 'Yay, a base database! An abstraction layer allowing for common interactions with Mongo, CDCS and local directory databases and records.',
+      long_description = getreadme(),
+      classifiers=[
+        'Development Status :: 4 - Beta',
+        'Intended Audience :: Science/Research',
+        'Natural Language :: English',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Topic :: Scientific/Engineering :: Physics'
+      ],
+      keywords = [
+        'database', 
+        'mongodb', 
+        'CDCS',
+      ],
+      url = 'https://github.com/usnistgov/yabadaba',
+      author = 'Lucas Hale',
+      author_email = 'lucas.hale@nist.gov',
+      packages = find_packages(),
+      install_requires = [
+        'lxml',
+        'DataModelDict',
+        'IPython',
+        'numpy', 
+        'pandas',
+        'cdcs>=0.2.3',
+        'pymongo',
+        'tqdm',
+      ],
+      package_data={'': ['*']},
+      zip_safe = False)
```

### Comparing `yabadaba-0.2.1/tests/test_Settings.py` & `yabadaba-0.2.2/tests/test_Settings.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,274 +1,274 @@
-import builtins
-from unittest.mock import patch
-import shutil
-from pathlib import Path
-
-from pytest import raises
-
-import yabadaba
-
-
-class TestSettings():
-
-    @property
-    def directoryname(self):
-        """str : The directoryname value used for initialization"""
-        return 'yabadaba_testing'
-    
-    @property
-    def fname(self):
-        """str : The filename value used for initialization"""
-        return 'yabadaba_testing_settings.json'
-
-    @property
-    def defaultdirectory(self):
-        """Path : What the defaultdirectory value should be"""
-        return Path(Path.home(), self.directoryname)
-
-    @property
-    def directory(self):
-        """Path : What the directory value should be"""
-        return self.__directory
-
-    @directory.setter
-    def directory(self, value):
-        self.__directory = Path(value).resolve()
-
-    @property
-    def defaultfilename(self):
-        """Path : What the defaultfilename value should be"""
-        return Path(self.defaultdirectory, self.fname)
-
-    @property
-    def filename(self):
-        """Path : What the filename value should be"""
-        return Path(self.directory, self.fname)
-
-    @property
-    def settings(self):
-        """yabadaba.Settings.Settings : A settings object to use for testing"""
-        if self.defaultdirectory.exists():
-            shutil.rmtree(self.defaultdirectory)
-        return yabadaba.Settings.Settings(directoryname=self.directoryname,
-                                          filename=self.fname)
-        
-    def test_initial(self):
-        """Initial testing"""
-
-        # Initialize a settings object
-        settings = self.settings
-
-        # Check status of settings attributes
-        assert settings.directory == self.defaultdirectory
-        assert settings.defaultdirectory == self.defaultdirectory 
-        assert settings.filename == self.defaultfilename
-        assert settings.defaultfilename == self.defaultfilename
-        assert settings.list_databases == []
-        assert settings.databases == {}
-
-        # Cleanup
-        if self.defaultdirectory.exists():
-            shutil.rmtree(self.defaultdirectory)
-
-    def test_databases(self):
-        """Test setting and unsetting databases"""
-
-        # Initialize a settings object
-        settings = self.settings
-
-        # Build content dict for comparison
-        content = {}
-
-        # Set a database with required terms
-        settings.set_database('pytest1', 'local', 'nowhere', key='no')
-        
-        # Update the comparison content
-        content['database'] = {}
-        content['database']['pytest1'] = {'style': 'local', 'host': 'nowhere', 'key': 'no'}
-
-        # Check status of settings attributes
-        assert settings.list_databases == ['pytest1']
-        assert settings.databases['pytest1'] == content['database']['pytest1']
-
-        # Check set database with missing name
-        with patch('builtins.input') as mock_input:
-            mock_input.return_value = 'pytest2'
-            settings.set_database(style='local', host='somewhere', key='yes')
-        
-        # Update the comparison content
-        content['database']['pytest2'] = {'style': 'local', 'host': 'somewhere', 'key': 'yes'}
-        
-        # Check status of settings attributes
-        assert settings.list_databases == ['pytest1', 'pytest2']
-        assert settings.databases['pytest2'] == content['database']['pytest2']
-
-        # Check set database with missing style
-        with patch('builtins.input') as mock_input:
-            mock_input.return_value = 'mongo'
-            settings.set_database(name='pytest3', host='everywhere', key='maybe')
-
-        # Update the comparison content
-        content['database']['pytest3'] = {'style': 'mongo', 'host': 'everywhere', 'key': 'maybe'}
-
-        # Check status of settings attributes
-        assert settings.list_databases == ['pytest1', 'pytest2', "pytest3"]
-        assert settings.databases['pytest3'] == content['database']['pytest3']
-
-        # Check set database with missing host
-        with patch('builtins.input') as mock_input:
-            mock_input.return_value = 'elsewhere'
-            settings.set_database(name='pytest4', style='cdcs', key='maybe')
-
-        # Update the comparison content
-        content['database']['pytest4'] = {'style': 'cdcs', 'host': 'elsewhere', 'key': 'maybe'}
-
-        # Check status of settings attributes
-        assert settings.list_databases == ['pytest1', 'pytest2', 'pytest3', 'pytest4']
-        assert settings.databases['pytest4'] == content['database']['pytest4']
-
-        # Check set database with missing key
-        with patch('builtins.input') as mock_input:
-            mock_input.return_value = ''
-            settings.set_database(name='pytest5', style='cdcs', host='here')
-        settings.set_database(name='pytest6', style='local', host='there', prompt=False)
-
-        # Update the comparison content
-        content['database']['pytest5'] = {'style': 'cdcs', 'host': 'here'}
-        content['database']['pytest6'] = {'style': 'local', 'host': 'there'}
-
-        # Check status of settings attributes
-        assert settings.list_databases == ['pytest1', 'pytest2', 'pytest3', 'pytest4', 'pytest5', 'pytest6']
-        assert settings.databases['pytest5'] == content['database']['pytest5']
-        assert settings.databases['pytest6'] == content['database']['pytest6']
-
-        # Test that prompt = False fails for missing values
-        with raises(TypeError):
-            settings.set_database(style='local', host='nowhere', key='no', prompt=False)
-        with raises(TypeError):
-            settings.set_database(name='asf', host='nowhere', key='no', prompt=False)
-        with raises(TypeError):
-            settings.set_database(name='asf', style='local', key='no', prompt=False)
-        
-        # Test updating existing settings with negative confirmation
-        with patch('builtins.input') as mock_input:
-            mock_input.return_value = 'no'
-            settings.set_database('pytest1', 'mongo', 'nowhere', key='no')
-        assert settings.databases['pytest1'] == content['database']['pytest1']
-        
-        # Test updating existing settings with invalid confirmation
-        with raises(ValueError):
-            with patch('builtins.input') as mock_input:
-                mock_input.return_value = 'ag'
-                settings.set_database('pytest1', 'mongo', 'nowhere', key='no')
-
-        # Test updating existing settings with positive confirmation
-        with patch('builtins.input') as mock_input:
-            mock_input.return_value = 'yes'
-            settings.set_database('pytest1', 'mongo', 'nowhere', key='no')
-        content['database']['pytest1'] = {'style': 'mongo', 'host': 'nowhere', 'key': 'no'}
-        assert settings.databases['pytest1'] == content['database']['pytest1']
-
-        # Test updating existing settings without prompt confirmation
-        settings.set_database('pytest1', 'cdcs', 'nowhere', key='no', prompt=False)
-        content['database']['pytest1'] = {'style': 'cdcs', 'host': 'nowhere', 'key': 'no'}
-        assert settings.databases['pytest1'] == content['database']['pytest1']
-
-        # Test unsetting databases
-        with patch('builtins.input') as mock_input:
-            mock_input.return_value = 'yes'
-            settings.unset_database('pytest1')
-        assert settings.list_databases == ['pytest2', 'pytest3', 'pytest4', 'pytest5', 'pytest6']
-
-        with patch('builtins.input') as mock_input:
-            mock_input.return_value = 'no'
-            settings.unset_database('pytest2')
-        assert settings.list_databases == ['pytest2', 'pytest3', 'pytest4', 'pytest5', 'pytest6']
-
-        settings.unset_database('pytest4', prompt=False)
-        assert settings.list_databases == ['pytest2', 'pytest3', 'pytest5', 'pytest6']
-
-        with raises(ValueError):
-            settings.unset_database('badname')
-
-        settings.unset_database('pytest2', prompt=False)
-        settings.unset_database('pytest3', prompt=False)
-        settings.unset_database('pytest5', prompt=False)
-        settings.unset_database('pytest6', prompt=False)
-        assert settings.content == {}
-
-        # Cleanup
-        if self.defaultdirectory.exists():
-            shutil.rmtree(self.defaultdirectory)
-
-    def test_directory(self, tmpdir):
-        
-        # Initialize a settings object
-        settings = self.settings
-        self.directory = tmpdir
-
-        # Set a database for testing purposes
-        settings.set_database('pytest1', 'local', 'nowhere', key='no')
-        assert settings.list_databases == ['pytest1']
-
-        # Set directory and move
-        with patch('builtins.input') as mock_input:
-            mock_input.return_value = 'yes'
-            settings.set_directory(tmpdir, move=True)
-
-        # Check status of settings attributes
-        assert settings.directory == self.directory
-        assert settings.defaultdirectory == self.defaultdirectory 
-        assert settings.filename == self.filename
-        assert settings.defaultfilename == self.defaultfilename
-        assert settings.list_databases == ['pytest1']
-        
-        # Set a database for testing purposes
-        settings.set_database('pytest2', 'local', 'nowhere', key='no')
-        assert settings.list_databases == ['pytest1', 'pytest2']
-
-        # unset directory and move
-        with patch('builtins.input') as mock_input:
-            mock_input.return_value = 'yes'
-            settings.unset_directory(move=True)
-
-        # Check status of settings attributes
-        assert settings.directory == self.defaultdirectory
-        assert settings.defaultdirectory == self.defaultdirectory 
-        assert settings.filename == self.defaultfilename
-        assert settings.defaultfilename == self.defaultfilename
-        assert settings.list_databases == ['pytest1', 'pytest2']
-        assert not self.filename.is_file()
-
-        # Set directory without move
-        settings.set_directory(tmpdir, move=False, prompt=False)
-        
-        settings.set_database('pytest3', 'local', 'nowhere', key='no')
-
-        # Check status of settings attributes
-        assert settings.directory == self.directory
-        assert settings.defaultdirectory == self.defaultdirectory 
-        assert settings.filename == self.filename
-        assert settings.defaultfilename == self.defaultfilename
-        assert settings.list_databases == ['pytest3']
-
-        # Error for unset+move when default location contains settings 
-        with raises(ValueError):
-            settings.unset_directory(move=True, prompt=False)
-
-        # Unset without move
-        settings.unset_directory(move=False, prompt=False)
-
-        # Check status of settings attributes
-        assert settings.directory == self.defaultdirectory
-        assert settings.defaultdirectory == self.defaultdirectory 
-        assert settings.filename == self.defaultfilename
-        assert settings.defaultfilename == self.defaultfilename
-        assert settings.list_databases == ['pytest1', 'pytest2']
-
-        # Error for set+move when new location contains settings
-        with raises(ValueError):
-            settings.set_directory(tmpdir, move=True, prompt=False)
-
-        # Cleanup
-        if self.defaultdirectory.exists():
+import builtins
+from unittest.mock import patch
+import shutil
+from pathlib import Path
+
+from pytest import raises
+
+import yabadaba
+
+
+class TestSettings():
+
+    @property
+    def directoryname(self):
+        """str : The directoryname value used for initialization"""
+        return 'yabadaba_testing'
+    
+    @property
+    def fname(self):
+        """str : The filename value used for initialization"""
+        return 'yabadaba_testing_settings.json'
+
+    @property
+    def defaultdirectory(self):
+        """Path : What the defaultdirectory value should be"""
+        return Path(Path.home(), self.directoryname)
+
+    @property
+    def directory(self):
+        """Path : What the directory value should be"""
+        return self.__directory
+
+    @directory.setter
+    def directory(self, value):
+        self.__directory = Path(value).resolve()
+
+    @property
+    def defaultfilename(self):
+        """Path : What the defaultfilename value should be"""
+        return Path(self.defaultdirectory, self.fname)
+
+    @property
+    def filename(self):
+        """Path : What the filename value should be"""
+        return Path(self.directory, self.fname)
+
+    @property
+    def settings(self):
+        """yabadaba.Settings.Settings : A settings object to use for testing"""
+        if self.defaultdirectory.exists():
+            shutil.rmtree(self.defaultdirectory)
+        return yabadaba.Settings.Settings(directoryname=self.directoryname,
+                                          filename=self.fname)
+        
+    def test_initial(self):
+        """Initial testing"""
+
+        # Initialize a settings object
+        settings = self.settings
+
+        # Check status of settings attributes
+        assert settings.directory == self.defaultdirectory
+        assert settings.defaultdirectory == self.defaultdirectory 
+        assert settings.filename == self.defaultfilename
+        assert settings.defaultfilename == self.defaultfilename
+        assert settings.list_databases == []
+        assert settings.databases == {}
+
+        # Cleanup
+        if self.defaultdirectory.exists():
+            shutil.rmtree(self.defaultdirectory)
+
+    def test_databases(self):
+        """Test setting and unsetting databases"""
+
+        # Initialize a settings object
+        settings = self.settings
+
+        # Build content dict for comparison
+        content = {}
+
+        # Set a database with required terms
+        settings.set_database('pytest1', 'local', 'nowhere', key='no')
+        
+        # Update the comparison content
+        content['database'] = {}
+        content['database']['pytest1'] = {'style': 'local', 'host': 'nowhere', 'key': 'no'}
+
+        # Check status of settings attributes
+        assert settings.list_databases == ['pytest1']
+        assert settings.databases['pytest1'] == content['database']['pytest1']
+
+        # Check set database with missing name
+        with patch('builtins.input') as mock_input:
+            mock_input.return_value = 'pytest2'
+            settings.set_database(style='local', host='somewhere', key='yes')
+        
+        # Update the comparison content
+        content['database']['pytest2'] = {'style': 'local', 'host': 'somewhere', 'key': 'yes'}
+        
+        # Check status of settings attributes
+        assert settings.list_databases == ['pytest1', 'pytest2']
+        assert settings.databases['pytest2'] == content['database']['pytest2']
+
+        # Check set database with missing style
+        with patch('builtins.input') as mock_input:
+            mock_input.return_value = 'mongo'
+            settings.set_database(name='pytest3', host='everywhere', key='maybe')
+
+        # Update the comparison content
+        content['database']['pytest3'] = {'style': 'mongo', 'host': 'everywhere', 'key': 'maybe'}
+
+        # Check status of settings attributes
+        assert settings.list_databases == ['pytest1', 'pytest2', "pytest3"]
+        assert settings.databases['pytest3'] == content['database']['pytest3']
+
+        # Check set database with missing host
+        with patch('builtins.input') as mock_input:
+            mock_input.return_value = 'elsewhere'
+            settings.set_database(name='pytest4', style='cdcs', key='maybe')
+
+        # Update the comparison content
+        content['database']['pytest4'] = {'style': 'cdcs', 'host': 'elsewhere', 'key': 'maybe'}
+
+        # Check status of settings attributes
+        assert settings.list_databases == ['pytest1', 'pytest2', 'pytest3', 'pytest4']
+        assert settings.databases['pytest4'] == content['database']['pytest4']
+
+        # Check set database with missing key
+        with patch('builtins.input') as mock_input:
+            mock_input.return_value = ''
+            settings.set_database(name='pytest5', style='cdcs', host='here')
+        settings.set_database(name='pytest6', style='local', host='there', prompt=False)
+
+        # Update the comparison content
+        content['database']['pytest5'] = {'style': 'cdcs', 'host': 'here'}
+        content['database']['pytest6'] = {'style': 'local', 'host': 'there'}
+
+        # Check status of settings attributes
+        assert settings.list_databases == ['pytest1', 'pytest2', 'pytest3', 'pytest4', 'pytest5', 'pytest6']
+        assert settings.databases['pytest5'] == content['database']['pytest5']
+        assert settings.databases['pytest6'] == content['database']['pytest6']
+
+        # Test that prompt = False fails for missing values
+        with raises(TypeError):
+            settings.set_database(style='local', host='nowhere', key='no', prompt=False)
+        with raises(TypeError):
+            settings.set_database(name='asf', host='nowhere', key='no', prompt=False)
+        with raises(TypeError):
+            settings.set_database(name='asf', style='local', key='no', prompt=False)
+        
+        # Test updating existing settings with negative confirmation
+        with patch('builtins.input') as mock_input:
+            mock_input.return_value = 'no'
+            settings.set_database('pytest1', 'mongo', 'nowhere', key='no')
+        assert settings.databases['pytest1'] == content['database']['pytest1']
+        
+        # Test updating existing settings with invalid confirmation
+        with raises(ValueError):
+            with patch('builtins.input') as mock_input:
+                mock_input.return_value = 'ag'
+                settings.set_database('pytest1', 'mongo', 'nowhere', key='no')
+
+        # Test updating existing settings with positive confirmation
+        with patch('builtins.input') as mock_input:
+            mock_input.return_value = 'yes'
+            settings.set_database('pytest1', 'mongo', 'nowhere', key='no')
+        content['database']['pytest1'] = {'style': 'mongo', 'host': 'nowhere', 'key': 'no'}
+        assert settings.databases['pytest1'] == content['database']['pytest1']
+
+        # Test updating existing settings without prompt confirmation
+        settings.set_database('pytest1', 'cdcs', 'nowhere', key='no', prompt=False)
+        content['database']['pytest1'] = {'style': 'cdcs', 'host': 'nowhere', 'key': 'no'}
+        assert settings.databases['pytest1'] == content['database']['pytest1']
+
+        # Test unsetting databases
+        with patch('builtins.input') as mock_input:
+            mock_input.return_value = 'yes'
+            settings.unset_database('pytest1')
+        assert settings.list_databases == ['pytest2', 'pytest3', 'pytest4', 'pytest5', 'pytest6']
+
+        with patch('builtins.input') as mock_input:
+            mock_input.return_value = 'no'
+            settings.unset_database('pytest2')
+        assert settings.list_databases == ['pytest2', 'pytest3', 'pytest4', 'pytest5', 'pytest6']
+
+        settings.unset_database('pytest4', prompt=False)
+        assert settings.list_databases == ['pytest2', 'pytest3', 'pytest5', 'pytest6']
+
+        with raises(ValueError):
+            settings.unset_database('badname')
+
+        settings.unset_database('pytest2', prompt=False)
+        settings.unset_database('pytest3', prompt=False)
+        settings.unset_database('pytest5', prompt=False)
+        settings.unset_database('pytest6', prompt=False)
+        assert settings.content == {}
+
+        # Cleanup
+        if self.defaultdirectory.exists():
+            shutil.rmtree(self.defaultdirectory)
+
+    def test_directory(self, tmpdir):
+        
+        # Initialize a settings object
+        settings = self.settings
+        self.directory = tmpdir
+
+        # Set a database for testing purposes
+        settings.set_database('pytest1', 'local', 'nowhere', key='no')
+        assert settings.list_databases == ['pytest1']
+
+        # Set directory and move
+        with patch('builtins.input') as mock_input:
+            mock_input.return_value = 'yes'
+            settings.set_directory(tmpdir, move=True)
+
+        # Check status of settings attributes
+        assert settings.directory == self.directory
+        assert settings.defaultdirectory == self.defaultdirectory 
+        assert settings.filename == self.filename
+        assert settings.defaultfilename == self.defaultfilename
+        assert settings.list_databases == ['pytest1']
+        
+        # Set a database for testing purposes
+        settings.set_database('pytest2', 'local', 'nowhere', key='no')
+        assert settings.list_databases == ['pytest1', 'pytest2']
+
+        # unset directory and move
+        with patch('builtins.input') as mock_input:
+            mock_input.return_value = 'yes'
+            settings.unset_directory(move=True)
+
+        # Check status of settings attributes
+        assert settings.directory == self.defaultdirectory
+        assert settings.defaultdirectory == self.defaultdirectory 
+        assert settings.filename == self.defaultfilename
+        assert settings.defaultfilename == self.defaultfilename
+        assert settings.list_databases == ['pytest1', 'pytest2']
+        assert not self.filename.is_file()
+
+        # Set directory without move
+        settings.set_directory(tmpdir, move=False, prompt=False)
+        
+        settings.set_database('pytest3', 'local', 'nowhere', key='no')
+
+        # Check status of settings attributes
+        assert settings.directory == self.directory
+        assert settings.defaultdirectory == self.defaultdirectory 
+        assert settings.filename == self.filename
+        assert settings.defaultfilename == self.defaultfilename
+        assert settings.list_databases == ['pytest3']
+
+        # Error for unset+move when default location contains settings 
+        with raises(ValueError):
+            settings.unset_directory(move=True, prompt=False)
+
+        # Unset without move
+        settings.unset_directory(move=False, prompt=False)
+
+        # Check status of settings attributes
+        assert settings.directory == self.defaultdirectory
+        assert settings.defaultdirectory == self.defaultdirectory 
+        assert settings.filename == self.defaultfilename
+        assert settings.defaultfilename == self.defaultfilename
+        assert settings.list_databases == ['pytest1', 'pytest2']
+
+        # Error for set+move when new location contains settings
+        with raises(ValueError):
+            settings.set_directory(tmpdir, move=True, prompt=False)
+
+        # Cleanup
+        if self.defaultdirectory.exists():
             shutil.rmtree(self.defaultdirectory)
```

### Comparing `yabadaba-0.2.1/yabadaba/Settings.py` & `yabadaba-0.2.2/yabadaba/Settings.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,430 +1,430 @@
-# coding: utf-8
-# Standard Python libraries
-from pathlib import Path
-import json
-from copy import deepcopy
-from typing import Union, Optional
-
-# Relative imports
-from yabadaba.tools import screen_input
-
-class Settings():
-    """
-    Class for handling saved settings.
-    """
-    def __init__(self,
-                 directoryname: str = '.NIST',
-                 filename: str = 'settings.json'):
-        """
-        Class initializer. Calls load.
-        
-        Parameters
-        ----------
-        directoryname : str, optional
-            The default directory where the settings file is expected will be
-            in a directory of this name within the user's home directory.
-            Default value is ".NIST".
-        filename, str, optional
-            The name to use for the settings file.  This will be saved in the
-            directory path and should have a ".json" extension.  Default value
-            is "settings.json".
-        """
-        self.__directoryname = directoryname
-        self.__filename = filename
-        self.__content = {}
-        self.__defaultcontent = {}
-
-        self.load()
-
-    ######################## Basic settings operations ########################
-
-    @property
-    def defaultdirectory(self) -> Path:
-        """pathlib.Path : Path to the default settings directory"""
-        return Path(Path.home(), self.__directoryname)
-
-    @property
-    def defaultfilename(self) -> Path:
-        """pathlib.Path : Path to the default settings file"""
-        return Path(self.defaultdirectory, self.__filename)
-
-    @property
-    def directory(self) -> Path:
-        """pathlib.Path : Path to the settings directory"""
-        return self.__directory
-
-    @property
-    def filename(self) -> Path:
-        """pathlib.Path : Path to the settings file"""
-        return Path(self.directory, self.__filename)
-
-    @property
-    def content(self) -> dict:
-        """dict : The contents of the settings file"""
-        return self.__content
-    
-    @property
-    def defaultcontent(self) -> dict:
-        """dict : The contents of the default settings file"""
-        return self.__defaultcontent
-    
-    def load(self):
-        """Loads the settings file."""
-        
-        # Load settings.json from the default location
-        if self.defaultfilename.is_file():
-            with open(self.defaultfilename, 'r') as f:
-                self.__defaultcontent = json.load(fp=f)
-        else:
-            self.__defaultcontent = {}
-            
-        # Check if forwarding_directory has been set
-        if 'forwarding_directory' in self.__defaultcontent:
-            self.__directory = Path(self.__defaultcontent['forwarding_directory'])
-            
-            # Load content from the forwarded location
-            if self.filename.is_file():
-                with open(self.filename, 'r') as f:
-                    self.__content = json.load(fp=f)
-            else:
-                self.__content = {}
-
-            # Check for recursive forwarding
-            if 'forwarding_directory' in self.__content:
-                raise ValueError('Multi-level forwarding not allowed.')
-        
-        # If no forwarding, default is current content
-        else:
-            self.__content = self.__defaultcontent
-            self.__directory = self.defaultdirectory
-
-    def save(self):
-        """Saves content to settings.json."""
-        if not self.directory.is_dir():
-            self.directory.mkdir(parents=True)
-
-        with open(self.filename, 'w') as f:
-            json.dump(self.content, fp=f, indent=4)
-        
-        # Reload
-        self.load()
-
-    def set_directory(self,
-                      directory: Union[str, Path] = None,
-                      move: bool = True,
-                      prompt: bool = True):
-        """
-        Changes the settings directory to a different location.
-
-        Parameters
-        ----------
-        directory : str or Path
-            The path to the new settings directory where settings.json (and the
-            default library directory) are to be located.
-        move : bool, optional
-            If True (default), will attempt to move the exiting settings file to the new
-            location.  If False, only the directory path is updated and any settings in the
-            old and new locations are left alone.
-        prompt : bool, optional
-            The default behavior is to prompt for missing details and confirmation of
-            changes being made.  Setting prompt = False will skip confirmations and
-            throw errors if required inputs are not given to the function.
-
-        Raises
-        ------
-        TypeError
-            If prompt is False and directory is not given.
-        ValueError
-            If an invalid response is given to the confirmation prompt or if move is True
-            and a non-empty settings file already exists in the new location.
-        """
-        # Manage directory values
-        if directory is None:
-            if prompt:
-                directory = screen_input("Enter the path for the new settings directory:")
-            else:
-                raise TypeError('directory must be specified if prompt is False')
-        directory = Path(directory).resolve()
-        
-        # Check if given directory path is the current set value
-        if self.directory == directory:
-            print(f'Settings directory is already set to "{self.directory}"')
-            return None
-        
-        # Prompt confirmation
-        if prompt:
-            print(f'Current settings directory is "{self.directory}"')
-            option = screen_input(f'Update to "{directory}"? (yes or no):')
-            if option.lower() in ['yes', 'y']:
-                pass
-            elif option.lower() in ['no', 'n']: 
-                return None
-            else: 
-                raise ValueError('Invalid choice')
-        
-        # Move existing settings
-        if move:
-            
-            # Check for file in the new location
-            filename = Path(directory, self.__filename)
-            if filename.is_file():
-                with open(filename, 'r') as f:
-                    test_content = f.read()
-                if test_content.strip() not in ['', '{}']:
-                    raise ValueError(f'cannot move directory as "{filename}" exists and contains content')
-
-            # Move the settings file
-            self.filename.replace(filename)
-            
-            # Clear defaultcontent if previous directory was the default
-            if self.directory == self.defaultdirectory:
-                self.__defaultcontent = {}
-            
-        # Update forwarding_directory value in default content
-        self.defaultcontent['forwarding_directory'] = directory.as_posix()
-        
-        # Save the updated default settings file
-        if not self.defaultdirectory.is_dir():
-            self.defaultdirectory.mkdir(parents=True)
-        with open(self.defaultfilename, 'w') as f:
-            json.dump(self.defaultcontent, fp=f, indent=4)
-        
-        # Reload settings
-        self.load()
-        
-    def unset_directory(self,
-                        move: bool = True,
-                        prompt: bool = True):
-        """
-        Changes the settings directory back to the default location.
-        
-        Parameters
-        ----------
-        move : bool
-            If True (default), will attempt to move the contents of the existing settings file
-            to the default location.  If False, only the directory path is updated and any settings
-            in the old and new locations are left alone.
-        prompt : bool, optional
-            The default behavior is to prompt for missing details and confirmation of
-            changes being made.  Setting prompt = False will skip confirmations and
-            throw errors if required inputs are not given to the function.
-
-        Raises
-        ------
-        ValueError
-            If an invalid response is given to the confirmation prompt or if move is True
-            and a non-empty settings file already exists in the new location.
-        """
-        
-        # Check if directory already is the default value
-        if self.directory == self.defaultdirectory:
-            print(f'Settings directory is already set to "{self.defaultdirectory}"')
-            return None
-        
-        # Prompt confirmation
-        if prompt:
-            print(f'Current settings directory is "{self.directory}"')
-            option = screen_input(f'Update to "{self.defaultdirectory}"? (yes or no):')
-            if option.lower() in ['yes', 'y']:
-                pass
-            elif option.lower() in ['no', 'n']: 
-                return None
-            else: 
-                raise ValueError('Invalid choice')
-        
-        # Move existing settings
-        if move:
-            # Check if default content contains other settings
-            for key in self.defaultcontent:
-                if key != 'forwarding_directory':
-                    raise ValueError(f'cannot move directory as "{self.defaultfilename}" contains content')
-
-            # Move the settings file to the default location
-            self.filename.replace(self.defaultfilename)
-        
-        # Unset without moving
-        else:       
-            
-            # Remove forwarding_directory pointer
-            del self.defaultcontent['forwarding_directory']
-            
-            # Save the updated default settings file
-            if not self.defaultdirectory.is_dir():
-                self.defaultdirectory.mkdir(parents=True)
-            with open(self.defaultfilename, 'w') as f:
-                json.dump(self.defaultcontent, fp=f, indent=4)
-        
-        # Reload settings
-        self.load()
-    
-    ############################ database settings ############################
-
-    @property
-    def databases(self) -> dict:
-        """dict: Any defined database settings organized by name"""
-        if 'database' in self.content:
-            return deepcopy(self.content['database'])
-        else:
-            return {}
-
-    @property
-    def list_databases(self) -> list:
-        """list: The names associated with the defined databases"""
-        return list(self.databases.keys())
-
-    def set_database(self,
-                     name: Optional[str] = None,
-                     style: Optional[str] = None,
-                     host: Optional[str] = None,
-                     prompt: bool = True,
-                     **kwargs):
-        """
-        Allows for database information to be defined in the settings file. Screen
-        prompts will be given to allow any necessary database parameters to be
-        entered.
-
-        Parameters
-        ----------
-        name : str, optional
-            The name to assign to the database. If not given, the user will be
-            prompted to enter one.
-        style : str, optional
-            The database style associated with the database. If not given, the
-            user will be prompted to enter one.
-        host : str, optional
-            The database host (directory path or url) where the database is
-            located. If not given, the user will be prompted to enter one.
-        prompt : bool, optional
-            The default behavior is to prompt for missing details and confirmation of
-            changes being made.  Setting prompt = False will skip confirmations and
-            throw errors if required inputs are not given to the function.
-        **kwargs : any, optional
-            Any other database style-specific parameter settings required to
-            properly access the database.
-
-        Raises
-        ------
-        ValueError
-            If the answer to the overwrite question is invalid.
-        """
-        # Ask for name if not given
-        if name is None:
-            if prompt:
-                name = screen_input('Enter a name for the database:')
-            else:
-                raise TypeError('name must be specified if prompt is False')
-
-        # Load database if it exists
-        if name in self.list_databases:
-            
-           # Ask if existing database should be overwritten
-            if prompt:
-                print(f'Database {name} already defined.')
-                option = screen_input('Overwrite? (yes or no):')
-                if option.lower() in ['yes', 'y']:
-                    pass
-                elif option.lower() in ['no', 'n']: 
-                    return None
-                else: 
-                    raise ValueError('Invalid choice')
-
-        # Ask for style if not given
-        if style is None: 
-            if prompt:
-                style = screen_input("Enter the database's style:")
-            else:
-                raise TypeError('style must be specified if prompt is False')
-        
-        # Ask for host if not given
-        if host is None: 
-            if prompt:
-                host = screen_input("Enter the database's host:")
-            else:
-                raise TypeError('host must be specified if prompt is False')
-        
-        if len(kwargs) == 0 and prompt:
-            print('Enter any other database parameters as key, value')
-            print('Exit by leaving key blank')
-            while True:
-                key = screen_input('key:')
-                if key == '': 
-                    break
-                kwargs[key] = screen_input('value:')
-
-        # Create database entry
-        if 'database' not in self.content:
-            self.content['database'] = {}
-        self.content['database'][name] = entry = {}
-        entry['style'] = style
-        entry['host'] = str(host)
-        for key, value in kwargs.items():
-            entry[key] = value
-
-        # Save changes
-        self.save()
-    
-    def unset_database(self,
-                       name: Optional[str] = None,
-                       prompt: bool = True):
-        """
-        Deletes the settings for a pre-defined database from the settings file.
-
-        Parameters
-        ----------
-        name : str, optional
-            The name assigned to a pre-defined database.
-        prompt : bool, optional
-            The default behavior is to prompt for missing details and confirmation of
-            changes being made.  Setting prompt = False will skip confirmations and
-            throw errors if required inputs are not given to the function.
-
-        Raises
-        ------
-        TypeError
-            If prompt is False and name is not given.
-        ValueError
-            If the database name is not found
-        """
-        database_names = self.list_databases
-                  
-        # Ask for name if not given
-        if name is None:
-            if len(database_names) > 0:
-                if prompt:
-                    print('Select a database:')
-                    for i, database in enumerate(database_names):
-                        print(i+1, database)
-                    choice = screen_input(':')
-                    try:
-                        choice = int(choice)
-                    except:
-                        name = choice
-                    else:
-                        name = database_names[choice-1]
-                else:
-                    raise TypeError('name must be specified if prompt is False')
-            else:
-                print('No databases currently set')
-                return None
-
-        # Verify listed name exists 
-        try:
-            i = database_names.index(name)
-        except:
-            raise ValueError(f'Database {name} not found')
-
-        # Confirmation prompt
-        if prompt:
-            print(f'Database {name} found')
-            test = screen_input('Delete settings? (must type yes):').lower()
-            if test != 'yes':
-                return None
-
-        # Delete database and save
-        del(self.content['database'][name])
-        if len(self.content['database']) == 0:
-            del(self.content['database'])
-        self.save()
-
-# Initialize settings
+# coding: utf-8
+# Standard Python libraries
+from pathlib import Path
+import json
+from copy import deepcopy
+from typing import Union, Optional
+
+# Relative imports
+from yabadaba.tools import screen_input
+
+class Settings():
+    """
+    Class for handling saved settings.
+    """
+    def __init__(self,
+                 directoryname: str = '.NIST',
+                 filename: str = 'settings.json'):
+        """
+        Class initializer. Calls load.
+        
+        Parameters
+        ----------
+        directoryname : str, optional
+            The default directory where the settings file is expected will be
+            in a directory of this name within the user's home directory.
+            Default value is ".NIST".
+        filename, str, optional
+            The name to use for the settings file.  This will be saved in the
+            directory path and should have a ".json" extension.  Default value
+            is "settings.json".
+        """
+        self.__directoryname = directoryname
+        self.__filename = filename
+        self.__content = {}
+        self.__defaultcontent = {}
+
+        self.load()
+
+    ######################## Basic settings operations ########################
+
+    @property
+    def defaultdirectory(self) -> Path:
+        """pathlib.Path : Path to the default settings directory"""
+        return Path(Path.home(), self.__directoryname)
+
+    @property
+    def defaultfilename(self) -> Path:
+        """pathlib.Path : Path to the default settings file"""
+        return Path(self.defaultdirectory, self.__filename)
+
+    @property
+    def directory(self) -> Path:
+        """pathlib.Path : Path to the settings directory"""
+        return self.__directory
+
+    @property
+    def filename(self) -> Path:
+        """pathlib.Path : Path to the settings file"""
+        return Path(self.directory, self.__filename)
+
+    @property
+    def content(self) -> dict:
+        """dict : The contents of the settings file"""
+        return self.__content
+    
+    @property
+    def defaultcontent(self) -> dict:
+        """dict : The contents of the default settings file"""
+        return self.__defaultcontent
+    
+    def load(self):
+        """Loads the settings file."""
+        
+        # Load settings.json from the default location
+        if self.defaultfilename.is_file():
+            with open(self.defaultfilename, 'r') as f:
+                self.__defaultcontent = json.load(fp=f)
+        else:
+            self.__defaultcontent = {}
+            
+        # Check if forwarding_directory has been set
+        if 'forwarding_directory' in self.__defaultcontent:
+            self.__directory = Path(self.__defaultcontent['forwarding_directory'])
+            
+            # Load content from the forwarded location
+            if self.filename.is_file():
+                with open(self.filename, 'r') as f:
+                    self.__content = json.load(fp=f)
+            else:
+                self.__content = {}
+
+            # Check for recursive forwarding
+            if 'forwarding_directory' in self.__content:
+                raise ValueError('Multi-level forwarding not allowed.')
+        
+        # If no forwarding, default is current content
+        else:
+            self.__content = self.__defaultcontent
+            self.__directory = self.defaultdirectory
+
+    def save(self):
+        """Saves content to settings.json."""
+        if not self.directory.is_dir():
+            self.directory.mkdir(parents=True)
+
+        with open(self.filename, 'w') as f:
+            json.dump(self.content, fp=f, indent=4)
+        
+        # Reload
+        self.load()
+
+    def set_directory(self,
+                      directory: Union[str, Path] = None,
+                      move: bool = True,
+                      prompt: bool = True):
+        """
+        Changes the settings directory to a different location.
+
+        Parameters
+        ----------
+        directory : str or Path
+            The path to the new settings directory where settings.json (and the
+            default library directory) are to be located.
+        move : bool, optional
+            If True (default), will attempt to move the exiting settings file to the new
+            location.  If False, only the directory path is updated and any settings in the
+            old and new locations are left alone.
+        prompt : bool, optional
+            The default behavior is to prompt for missing details and confirmation of
+            changes being made.  Setting prompt = False will skip confirmations and
+            throw errors if required inputs are not given to the function.
+
+        Raises
+        ------
+        TypeError
+            If prompt is False and directory is not given.
+        ValueError
+            If an invalid response is given to the confirmation prompt or if move is True
+            and a non-empty settings file already exists in the new location.
+        """
+        # Manage directory values
+        if directory is None:
+            if prompt:
+                directory = screen_input("Enter the path for the new settings directory:")
+            else:
+                raise TypeError('directory must be specified if prompt is False')
+        directory = Path(directory).resolve()
+        
+        # Check if given directory path is the current set value
+        if self.directory == directory:
+            print(f'Settings directory is already set to "{self.directory}"')
+            return None
+        
+        # Prompt confirmation
+        if prompt:
+            print(f'Current settings directory is "{self.directory}"')
+            option = screen_input(f'Update to "{directory}"? (yes or no):')
+            if option.lower() in ['yes', 'y']:
+                pass
+            elif option.lower() in ['no', 'n']: 
+                return None
+            else: 
+                raise ValueError('Invalid choice')
+        
+        # Move existing settings
+        if move:
+            
+            # Check for file in the new location
+            filename = Path(directory, self.__filename)
+            if filename.is_file():
+                with open(filename, 'r') as f:
+                    test_content = f.read()
+                if test_content.strip() not in ['', '{}']:
+                    raise ValueError(f'cannot move directory as "{filename}" exists and contains content')
+
+            # Move the settings file
+            self.filename.replace(filename)
+            
+            # Clear defaultcontent if previous directory was the default
+            if self.directory == self.defaultdirectory:
+                self.__defaultcontent = {}
+            
+        # Update forwarding_directory value in default content
+        self.defaultcontent['forwarding_directory'] = directory.as_posix()
+        
+        # Save the updated default settings file
+        if not self.defaultdirectory.is_dir():
+            self.defaultdirectory.mkdir(parents=True)
+        with open(self.defaultfilename, 'w') as f:
+            json.dump(self.defaultcontent, fp=f, indent=4)
+        
+        # Reload settings
+        self.load()
+        
+    def unset_directory(self,
+                        move: bool = True,
+                        prompt: bool = True):
+        """
+        Changes the settings directory back to the default location.
+        
+        Parameters
+        ----------
+        move : bool
+            If True (default), will attempt to move the contents of the existing settings file
+            to the default location.  If False, only the directory path is updated and any settings
+            in the old and new locations are left alone.
+        prompt : bool, optional
+            The default behavior is to prompt for missing details and confirmation of
+            changes being made.  Setting prompt = False will skip confirmations and
+            throw errors if required inputs are not given to the function.
+
+        Raises
+        ------
+        ValueError
+            If an invalid response is given to the confirmation prompt or if move is True
+            and a non-empty settings file already exists in the new location.
+        """
+        
+        # Check if directory already is the default value
+        if self.directory == self.defaultdirectory:
+            print(f'Settings directory is already set to "{self.defaultdirectory}"')
+            return None
+        
+        # Prompt confirmation
+        if prompt:
+            print(f'Current settings directory is "{self.directory}"')
+            option = screen_input(f'Update to "{self.defaultdirectory}"? (yes or no):')
+            if option.lower() in ['yes', 'y']:
+                pass
+            elif option.lower() in ['no', 'n']: 
+                return None
+            else: 
+                raise ValueError('Invalid choice')
+        
+        # Move existing settings
+        if move:
+            # Check if default content contains other settings
+            for key in self.defaultcontent:
+                if key != 'forwarding_directory':
+                    raise ValueError(f'cannot move directory as "{self.defaultfilename}" contains content')
+
+            # Move the settings file to the default location
+            self.filename.replace(self.defaultfilename)
+        
+        # Unset without moving
+        else:       
+            
+            # Remove forwarding_directory pointer
+            del self.defaultcontent['forwarding_directory']
+            
+            # Save the updated default settings file
+            if not self.defaultdirectory.is_dir():
+                self.defaultdirectory.mkdir(parents=True)
+            with open(self.defaultfilename, 'w') as f:
+                json.dump(self.defaultcontent, fp=f, indent=4)
+        
+        # Reload settings
+        self.load()
+    
+    ############################ database settings ############################
+
+    @property
+    def databases(self) -> dict:
+        """dict: Any defined database settings organized by name"""
+        if 'database' in self.content:
+            return deepcopy(self.content['database'])
+        else:
+            return {}
+
+    @property
+    def list_databases(self) -> list:
+        """list: The names associated with the defined databases"""
+        return list(self.databases.keys())
+
+    def set_database(self,
+                     name: Optional[str] = None,
+                     style: Optional[str] = None,
+                     host: Optional[str] = None,
+                     prompt: bool = True,
+                     **kwargs):
+        """
+        Allows for database information to be defined in the settings file. Screen
+        prompts will be given to allow any necessary database parameters to be
+        entered.
+
+        Parameters
+        ----------
+        name : str, optional
+            The name to assign to the database. If not given, the user will be
+            prompted to enter one.
+        style : str, optional
+            The database style associated with the database. If not given, the
+            user will be prompted to enter one.
+        host : str, optional
+            The database host (directory path or url) where the database is
+            located. If not given, the user will be prompted to enter one.
+        prompt : bool, optional
+            The default behavior is to prompt for missing details and confirmation of
+            changes being made.  Setting prompt = False will skip confirmations and
+            throw errors if required inputs are not given to the function.
+        **kwargs : any, optional
+            Any other database style-specific parameter settings required to
+            properly access the database.
+
+        Raises
+        ------
+        ValueError
+            If the answer to the overwrite question is invalid.
+        """
+        # Ask for name if not given
+        if name is None:
+            if prompt:
+                name = screen_input('Enter a name for the database:')
+            else:
+                raise TypeError('name must be specified if prompt is False')
+
+        # Load database if it exists
+        if name in self.list_databases:
+            
+           # Ask if existing database should be overwritten
+            if prompt:
+                print(f'Database {name} already defined.')
+                option = screen_input('Overwrite? (yes or no):')
+                if option.lower() in ['yes', 'y']:
+                    pass
+                elif option.lower() in ['no', 'n']: 
+                    return None
+                else: 
+                    raise ValueError('Invalid choice')
+
+        # Ask for style if not given
+        if style is None: 
+            if prompt:
+                style = screen_input("Enter the database's style:")
+            else:
+                raise TypeError('style must be specified if prompt is False')
+        
+        # Ask for host if not given
+        if host is None: 
+            if prompt:
+                host = screen_input("Enter the database's host:")
+            else:
+                raise TypeError('host must be specified if prompt is False')
+        
+        if len(kwargs) == 0 and prompt:
+            print('Enter any other database parameters as key, value')
+            print('Exit by leaving key blank')
+            while True:
+                key = screen_input('key:')
+                if key == '': 
+                    break
+                kwargs[key] = screen_input('value:')
+
+        # Create database entry
+        if 'database' not in self.content:
+            self.content['database'] = {}
+        self.content['database'][name] = entry = {}
+        entry['style'] = style
+        entry['host'] = str(host)
+        for key, value in kwargs.items():
+            entry[key] = value
+
+        # Save changes
+        self.save()
+    
+    def unset_database(self,
+                       name: Optional[str] = None,
+                       prompt: bool = True):
+        """
+        Deletes the settings for a pre-defined database from the settings file.
+
+        Parameters
+        ----------
+        name : str, optional
+            The name assigned to a pre-defined database.
+        prompt : bool, optional
+            The default behavior is to prompt for missing details and confirmation of
+            changes being made.  Setting prompt = False will skip confirmations and
+            throw errors if required inputs are not given to the function.
+
+        Raises
+        ------
+        TypeError
+            If prompt is False and name is not given.
+        ValueError
+            If the database name is not found
+        """
+        database_names = self.list_databases
+                  
+        # Ask for name if not given
+        if name is None:
+            if len(database_names) > 0:
+                if prompt:
+                    print('Select a database:')
+                    for i, database in enumerate(database_names):
+                        print(i+1, database)
+                    choice = screen_input(':')
+                    try:
+                        choice = int(choice)
+                    except:
+                        name = choice
+                    else:
+                        name = database_names[choice-1]
+                else:
+                    raise TypeError('name must be specified if prompt is False')
+            else:
+                print('No databases currently set')
+                return None
+
+        # Verify listed name exists 
+        try:
+            i = database_names.index(name)
+        except:
+            raise ValueError(f'Database {name} not found')
+
+        # Confirmation prompt
+        if prompt:
+            print(f'Database {name} found')
+            test = screen_input('Delete settings? (must type yes):').lower()
+            if test != 'yes':
+                return None
+
+        # Delete database and save
+        del(self.content['database'][name])
+        if len(self.content['database']) == 0:
+            del(self.content['database'])
+        self.save()
+
+# Initialize settings
 settings = Settings()
```

### Comparing `yabadaba-0.2.1/yabadaba/UnitConverter/__init__.py` & `yabadaba-0.2.2/yabadaba/UnitConverter/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,562 +1,562 @@
-# coding: utf-8
-
-# Standard Python libraries
-import ast
-from typing import Optional, Union
-
-# https://github.com/usnistgov/DataModelDict
-from DataModelDict import DataModelDict as DM
-
-# http://www.numpy.org/
-import numpy as np
-import numpy.typing as npt
-
-class UnitConverter():
-
-    # Import derived units defined in separate files
-    from ._length import (cm, mm, um, nm, pm, fm, km,
-                          angstrom, Å,
-                          lightyear, astro_unit,
-                          pc, kpc, Mpc, Gpc,
-                          inch, foot, mile, thou)
-    from ._volume import (L, mL, uL, nL, pL, fL, aL, kL, ML, GL)
-    from ._time import (ms, us, ns, ps, fs,
-                        minute, hour, day, week, year)
-    from ._frequency import (Hz, mHz, kHz, MHz, GHz, THz, PHz, rtHz, rpm,
-                             Hz·2π, mHz·2π, kHz·2π, MHz·2π, GHz·2π, THz·2π, PHz·2π, rpm·2π)
-    from ._mass import (g, mg, ug, ng, pg, fg,
-                        tonne, amu, Da, kDa, lbm)
-    from ._energy import (J, mJ, uJ, nJ, pJ, fJ, kJ, MJ, GJ, erg,
-                          eV, meV, keV, MeV, GeV, TeV,
-                          btu, smallcal, kcal, Wh, kWh)
-    from ._concentration import (mol, mmol, umol, nmol, pmol, fmol,
-                                 M, mM, uM, nM, pM, fM)
-    from ._force import (N, mN, uN, nN, pN, fN, kN, MN, GN, dyn, lbf)
-    from ._pressure import (Pa, hPa, kPa, MPa, GPa, bar,
-                            mbar, cbar, dbar, kbar, Mbar,
-                            atm, torr, mtorr, psi)
-    from ._power import (W, mW, uW, nW, pW, kW, MW, GW, TW,
-                         horsepower_imperial, horsepower_metric)
-    from ._acceleration import (Gal, mGal, uGal, eotvos)
-    from ._temperature import (degFinterval, degCinterval, mK, uK, nK, pK)
-    from ._charge import (mC, uC, nC, Ah, mAh)
-    from ._current import (A, mA, uA, nA, pA, fA)
-    from ._voltage import (V, mV, uV, nV, kV, MV, GV, TV)
-    from ._resistance import (ohm, Ω, mohm, mΩ, kohm, kΩ, Mohm, MΩ, Gohm, GΩ,
-                              S, mS, uS, nS)
-    from ._magnetic import (T, mT, uT, nT, G, mG, uG, kG, Oe, Wb)
-    from ._capacitance import (F, uF, nF, pF, fF, aF, H, mH, uH, nH)
-    from ._constants import (NA, pi, π, c0, mu0, μ0, eps0, ε0, Z0,
-                             hPlanck, hbar, ħ, kB, GNewton, sigmaSB, σSB, alphaFS, αFS,
-                             Rgas, e, uBohr, uNuc, aBohr, me, mp, mn,
-                             Rinf, Ry, Hartree, ARichardson, Phi0, KJos, RKlitz, debye,
-                             REarth, g0, Msolar, MEarth)
-
-    def __init__(self):
-        """Initialize a unit manager and set core units"""
-        
-        # Init core Si units
-        self.__m = 1.
-        self.__kg = 1.
-        self.__s = 1.
-        self.__C = 1.
-        self.__K = 1.
-
-        # Init unit and unitdoc dicts
-        self.__unit = {}
-        self.__unitdoc = {}
-        self.build_unit()
-
-    @property
-    def m(self) -> float:
-        """meter"""
-        return self.__m
-
-    @property
-    def kg(self) -> float:
-        """kilogram"""
-        return self.__kg
-
-    @property
-    def s(self) -> float:
-        """second"""
-        return self.__s
-    
-    @property
-    def C(self) -> float:
-        """coulomb"""
-        return self.__C
-    
-    @property
-    def K(self) -> float:
-        """kelvin"""
-        return self.__K
-
-    @property
-    def display_core_values(self) -> str:
-        """str: the current values of the core units"""
-        return '\n'.join([
-            f'm  = {self.m:.15}',
-            f'kg = {self.kg:.15}',
-            f's  = {self.s:.15}',
-            f'C  = {self.C:.15}',
-            f'K  = {self.K:.15}',
-        ])
-
-    def reset_units(self, 
-                    seed: Union[int, str, None] = None,
-                    **kwargs):
-        """
-        Resets the core units from which all others are derived.  Based on the
-        given inputs, three behaviors can occur:
-
-        1. If no kwargs are given and seed is int or None, then the core units
-           will be set to random values using the seed value.
-        
-        2. If no kwargs are given and seed is set as 'SI', then the working
-           units will be set to SI units.
-        
-        3. If kwargs are given, then the working units will be set/derived
-           based on which are given and SI units if needed.  At most 4 kwargs
-           of length, mass, time, energy, and charge can be given.  And seed
-           must be left as None.
-        
-        Parameters
-        ----------
-        seed : int, str or None, optional
-            random number seed to use in generating random working units.
-            seed='SI' will use SI units.  Must be None (default) if any other
-            parameters are given.
-        length : str, optional
-            Unit of length to use for the working units.
-        mass : str, optional
-            Unit of mass to use for the working units.
-        time : str, optional
-            Unit of time to use for the working units.
-        energy : str, optional
-            Unit of energy to use for the working units.
-        charge : str, optional
-            Unit of charge to use for the working units.
-            
-        Raises
-        ------
-        ValueError
-            If seed is given with any other parameters, or if more than four of
-            the working unit parameters are given.
-        """
-        
-        # Set known units
-        if isinstance(seed, str):
-            
-            if len(kwargs) > 0:
-                raise ValueError('seed cannot be given with any other parameters')
-            
-            if seed == 'SI':
-                self.__m = 1.
-                self.__kg = 1.
-                self.__s = 1.
-                self.__C = 1.
-                self.__K = 1.
-
-            else:
-                raise ValueError(f'str seed value {seed} not supported')
-
-        # Set random units
-        elif len(kwargs) == 0:
-            
-            import random
-
-            prior_random_state = random.getstate()
-
-            if seed is None:
-                random.seed()
-            else:
-                random.seed(seed)
-
-            self.__m = 10 ** random.uniform(-2,2)
-            self.__kg = 10 ** random.uniform(-2,2)
-            self.__s = 10 ** random.uniform(-2,2)
-            self.__C = 10 ** random.uniform(-2,2)
-            self.__K = 10 ** random.uniform(-2,2)
-
-            # Leave the random generator like I found it, in case something else is
-            # using it.
-            random.setstate(prior_random_state)
-
-        elif seed is None:
-            
-            # Check that no more than 4 working units are defined
-            if len(kwargs) > 4:
-                raise ValueError('Only four working units can be defined')
-            
-            # Set base units to 1 (working units to SI)
-            self.reset_units('SI')
-            
-            # Scale base units by working units
-            if 'length' in kwargs:
-                self.__m = self.m / self.unit[kwargs['length']]
-            
-            if 'mass' in kwargs:
-                self.__kg = self.kg / self.unit[kwargs['mass']]
-            
-            if 'time' in kwargs:
-                self.__s = self.s / self.unit[kwargs['time']]
-            
-            if 'charge' in kwargs:
-                self.__C = self.C / self.unit[kwargs['charge']]
-            
-            # Scale derived units by working units
-            if 'energy' in kwargs:
-                J = self.J / self.unit[kwargs['energy']]
-                
-                # Scale base units by derived units
-                if 'mass' not in kwargs:
-                    self.__kg = J * self.s**2 / self.m**2
-                elif 'time' not in kwargs:
-                    self.__s = (self.kg * self.m**2 / J)**0.5
-                elif 'length' not in kwargs:
-                    self.__m = (J * self.s**2 / self.kg)
-            
-        else:
-            raise ValueError('seed cannot be given with any other parameters')
-        
-        # Build unit and unitdoc dicts
-        self.build_unit()
-        
-    @property
-    def unit(self) -> dict:
-        """dict: All available unit names and set values"""
-        return self.__unit
-    
-    @property
-    def unitdoc(self) -> dict:
-        """dict: All available unit names and their descriptions"""
-        return self.__unitdoc
-
-    def build_unit(self):
-        """
-        Saves numericalunits attributes to global dictionary unit so the values
-        can be retrieved by their string names.
-        """
-        
-        self.__unit = {}
-        self.__unitdoc = {}
-        
-        # Copy all float attributes of numericalunits to unit
-        for key in dir(self):
-            
-            value = getattr(self, key)
-            
-            if key[:1] != '_' and isinstance(value, float):
-                self.unit[key] = value
-                self.unitdoc[key] = getattr(UnitConverter, key).__doc__
-
-    def set_literal(self, term: str) -> npt.ArrayLike:
-        """
-        Convert string 'value unit' to numbers in working units.
-        
-        Parameters
-        ----------
-        term : str
-            String containing value and associated unit. If unit is not given,
-            then the value is converted to a float and assumed to be in working
-            units.
-            
-        Returns
-        -------
-        float or numpy.ndarray
-            The numerical value of term in working units.
-            
-        Raises
-        ------
-        ValueError
-            If no valid float value can be parsed.
-        """
-        
-        # Set splitting point j to end of term (i.e. assume no units given)
-        j = len(term)
-        
-        # Loop until done
-        while True:
-            
-            # Split term into value, unit terms
-            value = term[:j].strip()
-            unit = term[j:].strip()
-            if len(unit) == 0:
-                unit = None
-
-            # Return number if value, unit pair is valid
-            try: 
-                return self.set_in_units(ast.literal_eval(value), unit)
-            except: 
-                # Find the next splitting point
-                try:
-                    j = term[:j].rindex(' ')
-                except ValueError as err:
-                    raise ValueError('Failed to parse term') from err
-
-    def set_in_units(self, 
-                     value: npt.ArrayLike,
-                     units: str) -> npt.ArrayLike:
-        """
-        Convert value from specified units to working units.
-        
-        Parameters
-        ----------
-        value : array-like object
-            A numerical value or list/array of values.
-        units : str
-            The units that value is in.
-            
-        Returns
-        -------
-        float or numpy.ndarray
-            The given value converted from the specified units to working units.
-        """
-        units = self.parse(units)
-        return np.asarray(value) * units
-
-    def get_in_units(self, 
-                     value: npt.ArrayLike,
-                     units: str) -> npt.ArrayLike:
-        """
-        Convert value from working units to specified units.
-        
-        Parameters
-        ----------
-        value : array-like object
-            A numerical value or list/array of values.
-        units : str
-            The units to convert value to (from working units).
-            
-        Returns
-        -------
-        float or numpy.ndarray
-            The given value converted to the specified units from working units.
-        """
-        units = self.parse(units)
-        return np.asarray(value) / units
-
-    def value_unit(self, term: dict) -> npt.ArrayLike:
-        """
-        Reads numerical value from dictionary containing 'value' and 'unit' keys.
-        
-        Parameters
-        ----------
-        term : dict
-            Dictionary containing 'value' and 'unit' keys.
-            
-        Returns
-        -------
-        float or numpy.ndarray
-            The result of calling set_in_units() by passing the dictionary keys 
-            'value' and 'unit' as parameters.
-        
-        """
-        unit = term.get('unit', None)
-        if unit is None:
-            value = np.asarray(term['value'])
-        else:
-            value = self.set_in_units(term['value'], unit)
-        
-        if 'shape' in term:
-            shape = tuple(term['shape'])
-            value = value.reshape(shape)
-        
-        return value
-        
-    def error_unit(self, term: dict) -> npt.ArrayLike:
-        """
-        Reads numerical error from dictionary containing 'error' and 'unit' keys.
-        
-        Parameters
-        ----------
-        term : dict
-            Dictionary containing 'error' and 'unit' keys.
-            
-        Returns
-        -------
-        float or numpy.ndarray
-            The result of calling set_in_units() by passing the dictionary keys 
-            'error' and 'unit' as parameters.
-        
-        """
-        unit = term.get('unit', None)
-        if unit is None:
-            error = np.asarray(term['error'])
-        else:
-            error = self.set_in_units(term['error'], unit)
-        
-        if 'shape' in term:
-            shape = tuple(term['shape'])
-            error = error.reshape(shape)
-        
-        return error
-        
-    def model(self,
-              value: npt.ArrayLike,
-              units: Optional[str] = None,
-              error: Optional[npt.ArrayLike] = None) -> DM:
-        """
-        Generates DataModelDict representation of data.
-        
-        Parameters
-        ----------
-        value : array-like object
-            A numerical value or list/array of values.
-        units : str, optional
-            The units to convert value to (from working units).
-        error : array-like object or None, optional
-            A value error to include.  If given, must be the same
-            size/shape as value.
-        
-        Returns
-        -------
-        DataModelDict
-            Model representation of the value(s).
-        """
-        
-        datamodel = DM()
-        
-        if units is not None:
-            value = self.get_in_units(value, units)
-        
-        if error is not None:
-            error = self.get_in_units(error, units)
-        
-        # Single value
-        if value.ndim == 0:
-            datamodel['value'] = value
-            if error is not None:
-                datamodel['error'] = error
-        
-        # 1D array
-        elif value.ndim == 1:
-            datamodel['value'] = value.tolist()
-            if error is not None:
-                datamodel['error'] = error.tolist()
-                
-        # Higher-order array requires shape
-        else:
-            shape = value.shape
-            datamodel['value'] = value.flatten().tolist()
-            if error is not None:
-                datamodel['error'] = error.flatten().tolist()
-            datamodel['shape'] = list(shape)
-        
-        if units is not None:
-            datamodel['unit'] = units
-        
-        return datamodel
-
-    def parse(self, units: Optional[str]) -> float:
-        """
-        Convert units as strings (or None) into scaling numbers.  This function
-        allows for complex unit definitions with operators:
-        
-        - '()' for defining order of operations
-        - '*' for multiplication.
-        - '/' for division.
-        - '^' for powers.
-        
-        Parameters
-        ----------
-        units : str or None
-            String consisting of defined unit names, operators, and numerical 
-            values to interpret.
-            
-        Returns
-        -------
-        float
-            The scaling factor for converting numbers in the given units to
-            working units. If units is None or == 'scaled', then this value is
-            1.0.
-        """
-        
-        # Units of None does no scaling
-        if units is None or units == 'scaled':
-            return 1
-
-        # Parse string and return number value
-        elif isinstance(units, str):
-            i = 0
-            terms = []
-            
-            # Break into terms
-            while i < len(units):
-                
-                # parse terms in parentheses first
-                if units[i] == '(':
-                    j = i + 1
-                    pcount = 0
-                    while True:
-                        if j == len(units):
-                            raise ValueError('Invalid () terms.')
-                        elif units[j] == ')':
-                            if pcount == 0:
-                                break
-                            else:
-                                pcount -= 1
-                        elif units[j] == '(':
-                            pcount += 1
-                        j += 1
-                        
-                    terms.append(self.parse(units[i+1: j]))
-                    i = j + 1
-                
-                # append string terms
-                elif units[i].isalpha():
-                    term = ''
-                    while i < len(units) and units[i] not in ' */^\n\r\t':
-                        term += units[i]
-                        i += 1
-                    terms.append(self.unit[term])
-                
-                # append numeric terms
-                elif units[i].isdigit() or units[i] == '-' or units[i] == '.':
-                    term = ''
-                    while i < len(units) and units[i] not in ' */^\n\r\t':
-                        term += units[i]
-                        i += 1
-                    terms.append(float(term))
-                
-                # append operators
-                elif units[i] in '*/^':
-                    terms.append(units[i])
-                    i += 1
-                
-                # ignore excess white characters
-                elif units[i] in ' \n\r\t':
-                    i += 1
-                
-                # issue error for unmatched ) parentheses
-                elif units[i] == ')':
-                    raise ValueError('Invalid () terms.')
-                
-                else:
-                    raise ValueError('Unknown character: %s' % units[i])
-            
-            # Compute powers
-            while '^' in terms:
-                c = terms.index('^')
-                value = [terms[c-1] ** terms[c+1]]
-                terms = terms[:c-1] + value + terms[c+2:]
-            
-            # Compute multiplication and division
-            while len(terms) > 1:
-                if terms[1] == '*':
-                    value = [terms[0] * terms[2]]
-                    terms = value + terms[3:]
-                elif terms[1] == '/':
-                    value = [terms[0] / terms[2]]
-                    terms = value + terms[3:]
-                else:
-                    raise ValueError('Invalid string format')
-            
-            return terms[0]
-
-        # Else assume units is already a number
-        else:
-            return units
-        
+# coding: utf-8
+
+# Standard Python libraries
+import ast
+from typing import Optional, Union
+
+# https://github.com/usnistgov/DataModelDict
+from DataModelDict import DataModelDict as DM
+
+# http://www.numpy.org/
+import numpy as np
+import numpy.typing as npt
+
+class UnitConverter():
+
+    # Import derived units defined in separate files
+    from ._length import (cm, mm, um, nm, pm, fm, km,
+                          angstrom, Å,
+                          lightyear, astro_unit,
+                          pc, kpc, Mpc, Gpc,
+                          inch, foot, mile, thou)
+    from ._volume import (L, mL, uL, nL, pL, fL, aL, kL, ML, GL)
+    from ._time import (ms, us, ns, ps, fs,
+                        minute, hour, day, week, year)
+    from ._frequency import (Hz, mHz, kHz, MHz, GHz, THz, PHz, rtHz, rpm,
+                             Hz·2π, mHz·2π, kHz·2π, MHz·2π, GHz·2π, THz·2π, PHz·2π, rpm·2π)
+    from ._mass import (g, mg, ug, ng, pg, fg,
+                        tonne, amu, Da, kDa, lbm)
+    from ._energy import (J, mJ, uJ, nJ, pJ, fJ, kJ, MJ, GJ, erg,
+                          eV, meV, keV, MeV, GeV, TeV,
+                          btu, smallcal, kcal, Wh, kWh)
+    from ._concentration import (mol, mmol, umol, nmol, pmol, fmol,
+                                 M, mM, uM, nM, pM, fM)
+    from ._force import (N, mN, uN, nN, pN, fN, kN, MN, GN, dyn, lbf)
+    from ._pressure import (Pa, hPa, kPa, MPa, GPa, bar,
+                            mbar, cbar, dbar, kbar, Mbar,
+                            atm, torr, mtorr, psi)
+    from ._power import (W, mW, uW, nW, pW, kW, MW, GW, TW,
+                         horsepower_imperial, horsepower_metric)
+    from ._acceleration import (Gal, mGal, uGal, eotvos)
+    from ._temperature import (degFinterval, degCinterval, mK, uK, nK, pK)
+    from ._charge import (mC, uC, nC, Ah, mAh)
+    from ._current import (A, mA, uA, nA, pA, fA)
+    from ._voltage import (V, mV, uV, nV, kV, MV, GV, TV)
+    from ._resistance import (ohm, Ω, mohm, mΩ, kohm, kΩ, Mohm, MΩ, Gohm, GΩ,
+                              S, mS, uS, nS)
+    from ._magnetic import (T, mT, uT, nT, G, mG, uG, kG, Oe, Wb)
+    from ._capacitance import (F, uF, nF, pF, fF, aF, H, mH, uH, nH)
+    from ._constants import (NA, pi, π, c0, mu0, μ0, eps0, ε0, Z0,
+                             hPlanck, hbar, ħ, kB, GNewton, sigmaSB, σSB, alphaFS, αFS,
+                             Rgas, e, uBohr, uNuc, aBohr, me, mp, mn,
+                             Rinf, Ry, Hartree, ARichardson, Phi0, KJos, RKlitz, debye,
+                             REarth, g0, Msolar, MEarth)
+
+    def __init__(self):
+        """Initialize a unit manager and set core units"""
+        
+        # Init core Si units
+        self.__m = 1.
+        self.__kg = 1.
+        self.__s = 1.
+        self.__C = 1.
+        self.__K = 1.
+
+        # Init unit and unitdoc dicts
+        self.__unit = {}
+        self.__unitdoc = {}
+        self.build_unit()
+
+    @property
+    def m(self) -> float:
+        """meter"""
+        return self.__m
+
+    @property
+    def kg(self) -> float:
+        """kilogram"""
+        return self.__kg
+
+    @property
+    def s(self) -> float:
+        """second"""
+        return self.__s
+    
+    @property
+    def C(self) -> float:
+        """coulomb"""
+        return self.__C
+    
+    @property
+    def K(self) -> float:
+        """kelvin"""
+        return self.__K
+
+    @property
+    def display_core_values(self) -> str:
+        """str: the current values of the core units"""
+        return '\n'.join([
+            f'm  = {self.m:.15}',
+            f'kg = {self.kg:.15}',
+            f's  = {self.s:.15}',
+            f'C  = {self.C:.15}',
+            f'K  = {self.K:.15}',
+        ])
+
+    def reset_units(self, 
+                    seed: Union[int, str, None] = None,
+                    **kwargs):
+        """
+        Resets the core units from which all others are derived.  Based on the
+        given inputs, three behaviors can occur:
+
+        1. If no kwargs are given and seed is int or None, then the core units
+           will be set to random values using the seed value.
+        
+        2. If no kwargs are given and seed is set as 'SI', then the working
+           units will be set to SI units.
+        
+        3. If kwargs are given, then the working units will be set/derived
+           based on which are given and SI units if needed.  At most 4 kwargs
+           of length, mass, time, energy, and charge can be given.  And seed
+           must be left as None.
+        
+        Parameters
+        ----------
+        seed : int, str or None, optional
+            random number seed to use in generating random working units.
+            seed='SI' will use SI units.  Must be None (default) if any other
+            parameters are given.
+        length : str, optional
+            Unit of length to use for the working units.
+        mass : str, optional
+            Unit of mass to use for the working units.
+        time : str, optional
+            Unit of time to use for the working units.
+        energy : str, optional
+            Unit of energy to use for the working units.
+        charge : str, optional
+            Unit of charge to use for the working units.
+            
+        Raises
+        ------
+        ValueError
+            If seed is given with any other parameters, or if more than four of
+            the working unit parameters are given.
+        """
+        
+        # Set known units
+        if isinstance(seed, str):
+            
+            if len(kwargs) > 0:
+                raise ValueError('seed cannot be given with any other parameters')
+            
+            if seed == 'SI':
+                self.__m = 1.
+                self.__kg = 1.
+                self.__s = 1.
+                self.__C = 1.
+                self.__K = 1.
+
+            else:
+                raise ValueError(f'str seed value {seed} not supported')
+
+        # Set random units
+        elif len(kwargs) == 0:
+            
+            import random
+
+            prior_random_state = random.getstate()
+
+            if seed is None:
+                random.seed()
+            else:
+                random.seed(seed)
+
+            self.__m = 10 ** random.uniform(-2,2)
+            self.__kg = 10 ** random.uniform(-2,2)
+            self.__s = 10 ** random.uniform(-2,2)
+            self.__C = 10 ** random.uniform(-2,2)
+            self.__K = 10 ** random.uniform(-2,2)
+
+            # Leave the random generator like I found it, in case something else is
+            # using it.
+            random.setstate(prior_random_state)
+
+        elif seed is None:
+            
+            # Check that no more than 4 working units are defined
+            if len(kwargs) > 4:
+                raise ValueError('Only four working units can be defined')
+            
+            # Set base units to 1 (working units to SI)
+            self.reset_units('SI')
+            
+            # Scale base units by working units
+            if 'length' in kwargs:
+                self.__m = self.m / self.unit[kwargs['length']]
+            
+            if 'mass' in kwargs:
+                self.__kg = self.kg / self.unit[kwargs['mass']]
+            
+            if 'time' in kwargs:
+                self.__s = self.s / self.unit[kwargs['time']]
+            
+            if 'charge' in kwargs:
+                self.__C = self.C / self.unit[kwargs['charge']]
+            
+            # Scale derived units by working units
+            if 'energy' in kwargs:
+                J = self.unit['J'] / self.unit[kwargs['energy']]
+                
+                # Scale base units by derived units
+                if 'mass' not in kwargs:
+                    self.__kg = J * self.s**2 / self.m**2
+                elif 'time' not in kwargs:
+                    self.__s = (self.kg * self.m**2 / J)**0.5
+                elif 'length' not in kwargs:
+                    self.__m = (J * self.s**2 / self.kg)
+            
+        else:
+            raise ValueError('seed cannot be given with any other parameters')
+        
+        # Build unit and unitdoc dicts
+        self.build_unit()
+        
+    @property
+    def unit(self) -> dict:
+        """dict: All available unit names and set values"""
+        return self.__unit
+    
+    @property
+    def unitdoc(self) -> dict:
+        """dict: All available unit names and their descriptions"""
+        return self.__unitdoc
+
+    def build_unit(self):
+        """
+        Saves numericalunits attributes to global dictionary unit so the values
+        can be retrieved by their string names.
+        """
+        
+        self.__unit = {}
+        self.__unitdoc = {}
+        
+        # Copy all float attributes of numericalunits to unit
+        for key in dir(self):
+            
+            value = getattr(self, key)
+            
+            if key[:1] != '_' and isinstance(value, float):
+                self.unit[key] = value
+                self.unitdoc[key] = getattr(UnitConverter, key).__doc__
+
+    def set_literal(self, term: str) -> npt.ArrayLike:
+        """
+        Convert string 'value unit' to numbers in working units.
+        
+        Parameters
+        ----------
+        term : str
+            String containing value and associated unit. If unit is not given,
+            then the value is converted to a float and assumed to be in working
+            units.
+            
+        Returns
+        -------
+        float or numpy.ndarray
+            The numerical value of term in working units.
+            
+        Raises
+        ------
+        ValueError
+            If no valid float value can be parsed.
+        """
+        
+        # Set splitting point j to end of term (i.e. assume no units given)
+        j = len(term)
+        
+        # Loop until done
+        while True:
+            
+            # Split term into value, unit terms
+            value = term[:j].strip()
+            unit = term[j:].strip()
+            if len(unit) == 0:
+                unit = None
+
+            # Return number if value, unit pair is valid
+            try: 
+                return self.set_in_units(ast.literal_eval(value), unit)
+            except: 
+                # Find the next splitting point
+                try:
+                    j = term[:j].rindex(' ')
+                except ValueError as err:
+                    raise ValueError('Failed to parse term') from err
+
+    def set_in_units(self, 
+                     value: npt.ArrayLike,
+                     units: str) -> npt.ArrayLike:
+        """
+        Convert value from specified units to working units.
+        
+        Parameters
+        ----------
+        value : array-like object
+            A numerical value or list/array of values.
+        units : str
+            The units that value is in.
+            
+        Returns
+        -------
+        float or numpy.ndarray
+            The given value converted from the specified units to working units.
+        """
+        units = self.parse(units)
+        return np.asarray(value) * units
+
+    def get_in_units(self, 
+                     value: npt.ArrayLike,
+                     units: str) -> npt.ArrayLike:
+        """
+        Convert value from working units to specified units.
+        
+        Parameters
+        ----------
+        value : array-like object
+            A numerical value or list/array of values.
+        units : str
+            The units to convert value to (from working units).
+            
+        Returns
+        -------
+        float or numpy.ndarray
+            The given value converted to the specified units from working units.
+        """
+        units = self.parse(units)
+        return np.asarray(value) / units
+
+    def value_unit(self, term: dict) -> npt.ArrayLike:
+        """
+        Reads numerical value from dictionary containing 'value' and 'unit' keys.
+        
+        Parameters
+        ----------
+        term : dict
+            Dictionary containing 'value' and 'unit' keys.
+            
+        Returns
+        -------
+        float or numpy.ndarray
+            The result of calling set_in_units() by passing the dictionary keys 
+            'value' and 'unit' as parameters.
+        
+        """
+        unit = term.get('unit', None)
+        if unit is None:
+            value = np.asarray(term['value'])
+        else:
+            value = self.set_in_units(term['value'], unit)
+        
+        if 'shape' in term:
+            shape = tuple(term['shape'])
+            value = value.reshape(shape)
+        
+        return value
+        
+    def error_unit(self, term: dict) -> npt.ArrayLike:
+        """
+        Reads numerical error from dictionary containing 'error' and 'unit' keys.
+        
+        Parameters
+        ----------
+        term : dict
+            Dictionary containing 'error' and 'unit' keys.
+            
+        Returns
+        -------
+        float or numpy.ndarray
+            The result of calling set_in_units() by passing the dictionary keys 
+            'error' and 'unit' as parameters.
+        
+        """
+        unit = term.get('unit', None)
+        if unit is None:
+            error = np.asarray(term['error'])
+        else:
+            error = self.set_in_units(term['error'], unit)
+        
+        if 'shape' in term:
+            shape = tuple(term['shape'])
+            error = error.reshape(shape)
+        
+        return error
+        
+    def model(self,
+              value: npt.ArrayLike,
+              units: Optional[str] = None,
+              error: Optional[npt.ArrayLike] = None) -> DM:
+        """
+        Generates DataModelDict representation of data.
+        
+        Parameters
+        ----------
+        value : array-like object
+            A numerical value or list/array of values.
+        units : str, optional
+            The units to convert value to (from working units).
+        error : array-like object or None, optional
+            A value error to include.  If given, must be the same
+            size/shape as value.
+        
+        Returns
+        -------
+        DataModelDict
+            Model representation of the value(s).
+        """
+        
+        datamodel = DM()
+        
+        if units is not None:
+            value = self.get_in_units(value, units)
+        
+        if error is not None:
+            error = self.get_in_units(error, units)
+        
+        # Single value
+        if value.ndim == 0:
+            datamodel['value'] = value
+            if error is not None:
+                datamodel['error'] = error
+        
+        # 1D array
+        elif value.ndim == 1:
+            datamodel['value'] = value.tolist()
+            if error is not None:
+                datamodel['error'] = error.tolist()
+                
+        # Higher-order array requires shape
+        else:
+            shape = value.shape
+            datamodel['value'] = value.flatten().tolist()
+            if error is not None:
+                datamodel['error'] = error.flatten().tolist()
+            datamodel['shape'] = list(shape)
+        
+        if units is not None:
+            datamodel['unit'] = units
+        
+        return datamodel
+
+    def parse(self, units: Optional[str]) -> float:
+        """
+        Convert units as strings (or None) into scaling numbers.  This function
+        allows for complex unit definitions with operators:
+        
+        - '()' for defining order of operations
+        - '*' for multiplication.
+        - '/' for division.
+        - '^' for powers.
+        
+        Parameters
+        ----------
+        units : str or None
+            String consisting of defined unit names, operators, and numerical 
+            values to interpret.
+            
+        Returns
+        -------
+        float
+            The scaling factor for converting numbers in the given units to
+            working units. If units is None or == 'scaled', then this value is
+            1.0.
+        """
+        
+        # Units of None does no scaling
+        if units is None or units == 'scaled':
+            return 1
+
+        # Parse string and return number value
+        elif isinstance(units, str):
+            i = 0
+            terms = []
+            
+            # Break into terms
+            while i < len(units):
+                
+                # parse terms in parentheses first
+                if units[i] == '(':
+                    j = i + 1
+                    pcount = 0
+                    while True:
+                        if j == len(units):
+                            raise ValueError('Invalid () terms.')
+                        elif units[j] == ')':
+                            if pcount == 0:
+                                break
+                            else:
+                                pcount -= 1
+                        elif units[j] == '(':
+                            pcount += 1
+                        j += 1
+                        
+                    terms.append(self.parse(units[i+1: j]))
+                    i = j + 1
+                
+                # append string terms
+                elif units[i].isalpha():
+                    term = ''
+                    while i < len(units) and units[i] not in ' */^\n\r\t':
+                        term += units[i]
+                        i += 1
+                    terms.append(self.unit[term])
+                
+                # append numeric terms
+                elif units[i].isdigit() or units[i] == '-' or units[i] == '.':
+                    term = ''
+                    while i < len(units) and units[i] not in ' */^\n\r\t':
+                        term += units[i]
+                        i += 1
+                    terms.append(float(term))
+                
+                # append operators
+                elif units[i] in '*/^':
+                    terms.append(units[i])
+                    i += 1
+                
+                # ignore excess white characters
+                elif units[i] in ' \n\r\t':
+                    i += 1
+                
+                # issue error for unmatched ) parentheses
+                elif units[i] == ')':
+                    raise ValueError('Invalid () terms.')
+                
+                else:
+                    raise ValueError('Unknown character: %s' % units[i])
+            
+            # Compute powers
+            while '^' in terms:
+                c = terms.index('^')
+                value = [terms[c-1] ** terms[c+1]]
+                terms = terms[:c-1] + value + terms[c+2:]
+            
+            # Compute multiplication and division
+            while len(terms) > 1:
+                if terms[1] == '*':
+                    value = [terms[0] * terms[2]]
+                    terms = value + terms[3:]
+                elif terms[1] == '/':
+                    value = [terms[0] / terms[2]]
+                    terms = value + terms[3:]
+                else:
+                    raise ValueError('Invalid string format')
+            
+            return terms[0]
+
+        # Else assume units is already a number
+        else:
+            return units
+        
 unitconvert = UnitConverter()
```

### Comparing `yabadaba-0.2.1/yabadaba/UnitConverter/_capacitance.py` & `yabadaba-0.2.2/yabadaba/UnitConverter/_mass.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,54 @@
-@property
-def F(self) -> float:
-    """farad"""
-    return self.C / self.V
-
-@property
-def uF(self) -> float:
-    """microfarad"""
-    return 1e-6 * self.F
-
-@property
-def nF(self) -> float:
-    """nanofarad"""
-    return 1e-9 * self.F
-
-@property
-def pF(self) -> float:
-    """picofarad"""
-    return 1e-12 * self.F
-
-@property
-def fF(self) -> float:
-    """femtofarad"""
-    return 1e-15 * self.F
-
-@property
-def aF(self) -> float:
-    """attofarad"""
-    return 1e-18 * self.F
-
-@property
-def H(self) -> float:
-    """henry"""
-    return self.m**2 * self.kg / self.C**2
-
-@property
-def mH(self) -> float:
-    """millihenry"""
-    return 1e-3 * self.H
-
-@property
-def uH(self) -> float:
-    """microhenry"""
-    return 1e-6 * self.H
-
-@property
-def nH(self) -> float:
-    """nanohenry"""
-    return 1e-9 * self.H
+@property
+def g(self) -> float:
+    """gram"""
+    return 1e-3 * self.kg
+
+@property
+def mg(self) -> float:
+    """milligram"""
+    return 1e-3 * self.g
+
+@property
+def ug(self) -> float:
+    """microgram"""
+    return 1e-6 * self.g
+
+@property
+def ng(self) -> float:
+    """nanogram"""
+    return 1e-9 * self.g
+
+@property
+def pg(self) -> float:
+    """picogram"""
+    return 1e-12 * self.g
+
+@property
+def fg(self) -> float:
+    """femtogram"""
+    return 1e-15 * self.g
+
+@property
+def tonne(self) -> float:
+    """tonne"""
+    return 1e3 * self.kg
+
+@property
+def amu(self) -> float:
+    """atomic mass unit"""
+    return 1.66053906660e-27 * self.kg
+
+@property
+def Da(self) -> float:
+    """dalton"""
+    return self.amu
+
+@property
+def kDa(self) -> float:
+    """kilodalton"""
+    return 1e3 * self.Da
+
+@property
+def lbm(self) -> float:
+    """pound mass (international avoirdupois pound)"""
+    return 0.45359237 * self.kg
```

### Comparing `yabadaba-0.2.1/yabadaba/UnitConverter/_concentration.py` & `yabadaba-0.2.2/yabadaba/UnitConverter/_capacitance.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,49 @@
-@property
-def mol(self) -> float:
-    """mole"""
-    return self.NA
-
-@property
-def mmol(self) -> float:
-    """millimole"""
-    return 1e-3 * self.mol
-
-@property
-def umol(self) -> float:
-    """micromole"""
-    return 1e-6 * self.mol
-
-@property
-def nmol(self) -> float:
-    """nanomole"""
-    return 1e-9 * self.mol
-
-@property
-def pmol(self) -> float:
-    """picomole"""
-    return 1e-12 * self.mol
-
-@property
-def fmol(self) -> float:
-    """femtomole"""
-    return 1e-15 * self.mol
-
-@property
-def M(self) -> float:
-    """molar"""
-    return self.mol / self.L
-
-@property
-def mM(self) -> float:
-    """millimolar"""
-    return 1e-3 * self.M
-
-@property
-def uM(self) -> float:
-    """micromolar"""
-    return 1e-6 * self.M
-
-@property
-def nM(self) -> float:
-    """nanomolar"""
-    return 1e-9 * self.M
-
-@property
-def pM(self) -> float:
-    """picomolar"""
-    return 1e-12 * self.M
-
-@property
-def fM(self) -> float:
-    """femtomolar"""
-    return 1e-15 * self.M
+@property
+def F(self) -> float:
+    """farad"""
+    return self.C / self.V
+
+@property
+def uF(self) -> float:
+    """microfarad"""
+    return 1e-6 * self.F
+
+@property
+def nF(self) -> float:
+    """nanofarad"""
+    return 1e-9 * self.F
+
+@property
+def pF(self) -> float:
+    """picofarad"""
+    return 1e-12 * self.F
+
+@property
+def fF(self) -> float:
+    """femtofarad"""
+    return 1e-15 * self.F
+
+@property
+def aF(self) -> float:
+    """attofarad"""
+    return 1e-18 * self.F
+
+@property
+def H(self) -> float:
+    """henry"""
+    return self.m**2 * self.kg / self.C**2
+
+@property
+def mH(self) -> float:
+    """millihenry"""
+    return 1e-3 * self.H
+
+@property
+def uH(self) -> float:
+    """microhenry"""
+    return 1e-6 * self.H
+
+@property
+def nH(self) -> float:
+    """nanohenry"""
+    return 1e-9 * self.H
```

### Comparing `yabadaba-0.2.1/yabadaba/UnitConverter/_energy.py` & `yabadaba-0.2.2/yabadaba/UnitConverter/_power.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,104 +1,54 @@
-@property
-def J(self) -> float:
-    """joule"""
-    return (self.kg * self.m**2) / self.s**2
-
-@property
-def mJ(self) -> float:
-    """milligram"""
-    return 1e-3 * self.J
-
-@property
-def uJ(self) -> float:
-    """microgram"""
-    return 1e-6 * self.J
-
-@property
-def nJ(self) -> float:
-    """nanogram"""
-    return 1e-9 * self.J
-
-@property
-def pJ(self) -> float:
-    """picogram"""
-    return 1e-12 * self.J
-
-@property
-def fJ(self) -> float:
-    """femtogram"""
-    return 1e-15 * self.J
-
-@property
-def kJ(self) -> float:
-    """kilojoule"""
-    return 1e3 * self.J
-
-@property
-def MJ(self) -> float:
-    """megajoule"""
-    return 1e6 * self.J
-
-@property
-def GJ(self) -> float:
-    """gigajoule"""
-    return 1e9 * self.J
-
-@property
-def erg(self) -> float:
-    """erg"""
-    return 1e-7 * self.J
-
-@property
-def eV(self) -> float:
-    """electron volt"""
-    return 1.602176634e-19 * self.J
-
-@property
-def meV(self) -> float:
-    """millielectron volt"""
-    return 1e-3 * self.eV
-
-@property
-def keV(self) -> float:
-    """kiloelectron volt"""
-    return 1e3 * self.eV
-
-@property
-def MeV(self) -> float:
-    """megaelectron volt"""
-    return 1e6 * self.eV
-
-@property
-def GeV(self) -> float:
-    """gigaelectron volt"""
-    return 1e9 * self.eV
-
-@property
-def TeV(self) -> float:
-    """teraelectron volt"""
-    return 1e12 * self.eV
-
-@property
-def btu(self) -> float:
-    """British thermal unit"""
-    return 1055.06 * self.J
-
-@property
-def smallcal(self) -> float:
-    """small calorie (a.k.a. gram calorie)"""
-    return 4.184 * self.J
-
-@property
-def kcal(self) -> float:
-    """kilocalorie (a.k.a large Calorie, dietary Calorie)"""
-    return 4184. * self.J
-
-@property
-def Wh(self) -> float:
-    """watt-hour"""
-    return 3600. * self.J
-
-@property
-def kWh(self) -> float:
-    """kilowatt-hour"""
-    return 1e3 * self.Wh
+@property 
+def W(self) -> float:
+    """watt"""
+    return self.J / self.s
+
+@property
+def mW(self) -> float:
+    """milliwatt"""
+    return 1e-3 * self.W
+
+@property
+def uW(self) -> float:
+    """microwatt"""
+    return 1e-6 * self.W
+
+@property
+def nW(self) -> float:
+    """nanowatt"""
+    return 1e-9 * self.W
+
+@property
+def pW(self) -> float:
+    """picowatt"""
+    return 1e-12 * self.W
+
+@property
+def kW(self) -> float:
+    """kilowatt"""
+    return 1e3 * self.W
+
+@property
+def MW(self) -> float:
+    """megawatt"""
+    return 1e6 * self.W
+
+@property
+def GW(self) -> float:
+    """gigawatt"""
+    return 1e9 * self.W
+
+@property
+def TW(self) -> float:
+    """terawatt"""
+    return 1e12 * self.W
+
+@property
+def horsepower_imperial(self) -> float:
+    """imperial horsepower"""
+    return 33000 * self.foot * self.lbf / self.minute
+
+@property
+def horsepower_metric(self) -> float:
+    """metric horsepower"""
+    return (75 * self.kg) * (9.80665 * self.m / self.s**2) * (1 * self.m / self.s)
```

### Comparing `yabadaba-0.2.1/yabadaba/UnitConverter/_force.py` & `yabadaba-0.2.2/yabadaba/UnitConverter/_pressure.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,74 @@
-@property
-def N(self) -> float:
-    """newton"""
-    return (self.kg * self.m) / self.s**2
-
-@property
-def mN(self) -> float:
-    """millinewton"""
-    return 1e-3 * self.N
-
-@property
-def uN(self) -> float:
-    """micronewton"""
-    return 1e-6 * self.N
-
-@property
-def nN(self) -> float:
-    """nanonewton"""
-    return 1e-9 * self.N
-
-@property
-def pN(self) -> float:
-    """piconewton"""
-    return 1e-12 * self.N
-
-@property
-def fN(self) -> float:
-    """femtonewton"""
-    return 1e-15 * self.N
-
-@property
-def kN(self) -> float:
-    """kilonewton"""
-    return 1e3 * self.N
-
-@property
-def MN(self) -> float:
-    """meganewton"""
-    return 1e6 * self.N
-
-@property
-def GN(self) -> float:
-    """giganewton"""
-    return 1e9 * self.N
-
-@property
-def dyn(self) -> float:
-    """dyne"""
-    return 1e-5 * self.N
-
-@property
-def lbf(self) -> float:
-    """pound-force (international avoirdupois pound)"""
-    return self.lbm * (9.80665 * self.m / self.s**2)
+@property
+def Pa(self) -> float:
+    """pascal"""
+    return self.N / self.m**2
+
+@property
+def hPa(self) -> float:
+    """hectopascal"""
+    return 1e2 * self.Pa
+
+@property
+def kPa(self) -> float:
+    """kilopascal"""
+    return 1e3 * self.Pa
+
+@property
+def MPa(self) -> float:
+    """megapascal"""
+    return 1e6 * self.Pa
+
+@property
+def GPa(self) -> float:
+    """gigapascal"""
+    return 1e9 * self.Pa
+
+@property
+def bar(self) -> float:
+    """bar"""
+    return 1e5 * self.Pa
+
+@property
+def mbar(self) -> float:
+    """millibar"""
+    return 1e-3 * self.bar
+
+@property
+def cbar(self) -> float:
+    """centibar"""
+    return 1e-2 * self.bar
+
+@property
+def dbar(self) -> float:
+    """decibar"""
+    return 0.1 * self.bar
+
+@property
+def kbar(self) -> float:
+    """kilobar"""
+    return 1e3 * self.bar
+
+@property
+def Mbar(self) -> float:
+    """megabar"""
+    return 1e6 * self.bar
+
+@property
+def atm(self) -> float:
+    """standard atmosphere pressure"""
+    return 101325. * self.Pa
+
+@property
+def torr(self) -> float:
+    """torr"""
+    return (1. / 760.) * self.atm
+
+@property
+def mtorr(self) -> float:
+    """millitorr"""
+    return 1e-3 * self.torr
+
+@property
+def psi(self) -> float:
+    """pounds force per square inch"""
+    return self.lbf / self.inch**2
```

### Comparing `yabadaba-0.2.1/yabadaba/UnitConverter/_magnetic.py` & `yabadaba-0.2.2/yabadaba/UnitConverter/_magnetic.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-@property 
-def T(self) -> float:
-    """tesla"""
-    return (self.V * self.s) / self.m**2
-
-@property
-def mT(self) -> float:
-    """millitesla"""
-    return 1e-3 * self.T
-
-@property
-def uT(self) -> float:
-    """microtesla"""
-    return 1e-6 * self.T
-
-@property
-def nT(self) -> float:
-    """nanotesla"""
-    return 1e-9 * self.T
-
-@property
-def G(self) -> float:
-    """gauss"""
-    return 1e-4 * self.T
-
-@property
-def mG(self) -> float:
-    """milligauss"""
-    return 1e-3 * self.G
-
-@property
-def uG(self) -> float:
-    """microgauss"""
-    return 1e-6 * self.G
-
-@property
-def kG(self) -> float:
-    """kilogauss"""
-    return 1e3 * self.G
-
-@property
-def Oe(self) -> float:
-    """oersted"""
-    return (1000. / (4. * self.pi)) * self.A / self.m
-
-@property
-def Wb(self) -> float:
-    """weber"""
+@property 
+def T(self) -> float:
+    """tesla"""
+    return (self.V * self.s) / self.m**2
+
+@property
+def mT(self) -> float:
+    """millitesla"""
+    return 1e-3 * self.T
+
+@property
+def uT(self) -> float:
+    """microtesla"""
+    return 1e-6 * self.T
+
+@property
+def nT(self) -> float:
+    """nanotesla"""
+    return 1e-9 * self.T
+
+@property
+def G(self) -> float:
+    """gauss"""
+    return 1e-4 * self.T
+
+@property
+def mG(self) -> float:
+    """milligauss"""
+    return 1e-3 * self.G
+
+@property
+def uG(self) -> float:
+    """microgauss"""
+    return 1e-6 * self.G
+
+@property
+def kG(self) -> float:
+    """kilogauss"""
+    return 1e3 * self.G
+
+@property
+def Oe(self) -> float:
+    """oersted"""
+    return (1000. / (4. * self.pi)) * self.A / self.m
+
+@property
+def Wb(self) -> float:
+    """weber"""
     return self.J / self.A
```

### Comparing `yabadaba-0.2.1/yabadaba/UnitConverter/_mass.py` & `yabadaba-0.2.2/yabadaba/UnitConverter/_force.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-@property
-def g(self) -> float:
-    """gram"""
-    return 1e-3 * self.kg
-
-@property
-def mg(self) -> float:
-    """milligram"""
-    return 1e-3 * self.g
-
-@property
-def ug(self) -> float:
-    """microgram"""
-    return 1e-6 * self.g
-
-@property
-def ng(self) -> float:
-    """nanogram"""
-    return 1e-9 * self.g
-
-@property
-def pg(self) -> float:
-    """picogram"""
-    return 1e-12 * self.g
-
-@property
-def fg(self) -> float:
-    """femtogram"""
-    return 1e-15 * self.g
-
-@property
-def tonne(self) -> float:
-    """tonne"""
-    return 1e3 * self.kg
-
-@property
-def amu(self) -> float:
-    """atomic mass unit"""
-    return 1.66053906660e-27 * self.kg
-
-@property
-def Da(self) -> float:
-    """dalton"""
-    return self.amu
-
-@property
-def kDa(self) -> float:
-    """kilodalton"""
-    return 1e3 * self.Da
-
-@property
-def lbm(self) -> float:
-    """pound mass (international avoirdupois pound)"""
-    return 0.45359237 * self.kg
+@property
+def N(self) -> float:
+    """newton"""
+    return (self.kg * self.m) / self.s**2
+
+@property
+def mN(self) -> float:
+    """millinewton"""
+    return 1e-3 * self.N
+
+@property
+def uN(self) -> float:
+    """micronewton"""
+    return 1e-6 * self.N
+
+@property
+def nN(self) -> float:
+    """nanonewton"""
+    return 1e-9 * self.N
+
+@property
+def pN(self) -> float:
+    """piconewton"""
+    return 1e-12 * self.N
+
+@property
+def fN(self) -> float:
+    """femtonewton"""
+    return 1e-15 * self.N
+
+@property
+def kN(self) -> float:
+    """kilonewton"""
+    return 1e3 * self.N
+
+@property
+def MN(self) -> float:
+    """meganewton"""
+    return 1e6 * self.N
+
+@property
+def GN(self) -> float:
+    """giganewton"""
+    return 1e9 * self.N
+
+@property
+def dyn(self) -> float:
+    """dyne"""
+    return 1e-5 * self.N
+
+@property
+def lbf(self) -> float:
+    """pound-force (international avoirdupois pound)"""
+    return self.lbm * (9.80665 * self.m / self.s**2)
```

### Comparing `yabadaba-0.2.1/yabadaba/UnitConverter/_pressure.py` & `yabadaba-0.2.2/yabadaba/UnitConverter/_frequency.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,86 @@
-@property
-def Pa(self) -> float:
-    """pascal"""
-    return self.N / self.m**2
-
-@property
-def hPa(self) -> float:
-    """hectopascal"""
-    return 1e2 * self.Pa
-
-@property
-def kPa(self) -> float:
-    """kilopascal"""
-    return 1e3 * self.Pa
-
-@property
-def MPa(self) -> float:
-    """megapascal"""
-    return 1e6 * self.Pa
-
-@property
-def GPa(self) -> float:
-    """gigapascal"""
-    return 1e9 * self.Pa
-
-@property
-def bar(self) -> float:
-    """bar"""
-    return 1e5 * self.Pa
-
-@property
-def mbar(self) -> float:
-    """millibar"""
-    return 1e-3 * self.bar
-
-@property
-def cbar(self) -> float:
-    """centibar"""
-    return 1e-2 * self.bar
-
-@property
-def dbar(self) -> float:
-    """decibar"""
-    return 0.1 * self.bar
-
-@property
-def kbar(self) -> float:
-    """kilobar"""
-    return 1e3 * self.bar
-
-@property
-def Mbar(self) -> float:
-    """megabar"""
-    return 1e6 * self.bar
-
-@property
-def atm(self) -> float:
-    """standard atmosphere pressure"""
-    return 101325. * self.Pa
-
-@property
-def torr(self) -> float:
-    """torr"""
-    return (1. / 760.) * self.atm
-
-@property
-def mtorr(self) -> float:
-    """millitorr"""
-    return 1e-3 * self.torr
-
-@property
-def psi(self) -> float:
-    """pounds force per square inch"""
-    return self.lbf / self.inch**2
+@property
+def Hz(self) -> float:
+    """hertz"""
+    return 1. / self.s
+
+@property
+def mHz(self) -> float:
+    """megahertz"""
+    return 1e-3 * self.Hz
+
+@property
+def kHz(self) -> float:
+    """kilohertz"""
+    return 1e3 * self.Hz
+
+@property
+def MHz(self) -> float:
+    """megahertz"""
+    return 1e6 * self.Hz
+    
+@property
+def GHz(self) -> float:
+    """gigahertz"""
+    return 1e9 * self.Hz
+
+@property
+def THz(self) -> float:
+    """terahertz"""
+    return 1e12 * self.Hz
+
+@property
+def PHz(self) -> float:
+    """petahertz"""
+    return 1e15 * self.Hz
+
+@property
+def rtHz(self) -> float:
+    """root Hertz"""
+    return self.Hz**0.5 
+
+@property
+def rpm(self) -> float:
+    """revolutions per minute"""
+    return 1 / self.minute
+
+############ Angular frequency below ################
+
+@property
+def Hz·2π(self) -> float:
+    """hertz times 2 pi"""
+    return self.Hz * 2 * self.pi
+
+@property
+def mHz·2π(self) -> float:
+    """millihertz times 2 pi"""
+    return self.mHz * 2 * self.pi
+
+@property
+def kHz·2π(self) -> float:
+    """kilohertz times 2 pi"""
+    return self.kHz * 2 * self.pi
+
+@property
+def MHz·2π(self) -> float:
+    """megahertz times 2 pi"""
+    return self.MHz * 2 * self.pi
+
+@property
+def GHz·2π(self) -> float:
+    """gigahertz times 2 pi"""
+    return self.GHz * 2 * self.pi
+
+@property
+def THz·2π(self) -> float:
+    """terahertz times 2 pi"""
+    return self.THz * 2 * self.pi
+
+@property
+def PHz·2π(self) -> float:
+    """petahertz times 2 pi"""
+    return self.PHz * 2 * self.pi
+
+@property
+def rpm·2π(self) -> float:
+    """revolutions per minute times 2 pi"""
+    return self.rpm * 2 * self.pi
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yabadaba-0.2.1/yabadaba/UnitConverter/_temperature.py` & `yabadaba-0.2.2/yabadaba/UnitConverter/_voltage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,39 @@
-@property 
-def degFinterval(self) -> float:
-    """temperature difference in degrees Fahrenheit"""
-    return (5./9.) * self.K
-
-@property
-def degCinterval(self) -> float:
-    """temperature difference in degrees Celsius"""
-    return self.K
-
-@property
-def mK(self) -> float:
-    """millikelvin"""
-    return 1e-3 * self.K
-
-@property
-def uK(self) -> float:
-    """microkelvin"""
-    return 1e-6 * self.K
-
-@property
-def nK(self) -> float:
-    """nanokelvin"""
-    return 1e-9 * self.K
-
-@property
-def pK(self) -> float:
-    """picokelvin"""
-    return 1e-12 * self.K
+@property 
+def V(self) -> float:
+    """volt"""
+    return self.J / self.C
+
+@property
+def mV(self) -> float:
+    """millivolt"""
+    return 1e-3 * self.V
+
+@property
+def uV(self) -> float:
+    """microvolt"""
+    return 1e-6 * self.V
+
+@property
+def nV(self) -> float:
+    """nanovolt"""
+    return 1e-9 * self.V
+
+@property
+def kV(self) -> float:
+    """kilovolt"""
+    return 1e3 * self.V
+
+@property
+def MV(self) -> float:
+    """megavolt"""
+    return 1e6 * self.V
+
+@property
+def GV(self) -> float:
+    """gigavolt"""
+    return 1e9 * self.V
+
+@property
+def TV(self) -> float:
+    """teravolt"""
+    return 1e12 * self.V
```

### Comparing `yabadaba-0.2.1/yabadaba/UnitConverter/_time.py` & `yabadaba-0.2.2/yabadaba/UnitConverter/_concentration.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,59 @@
-@property
-def ms(self) -> float:
-    """millisecond"""
-    return 1e-3 * self.s
-
-@property
-def us(self) -> float:
-    """microsecond"""
-    return 1e-6 * self.s
-
-@property
-def ns(self) -> float:
-    """nanosecond"""
-    return 1e-9 * self.s
-
-@property
-def ps(self) -> float:
-    """picosecond"""
-    return 1e-12 * self.s
-
-@property
-def fs(self) -> float:
-    """femtosecond"""
-    return 1e-15 * self.s
-
-@property
-def minute(self) -> float:
-    """minute"""
-    return 60. * self.s
-
-@property
-def hour(self) -> float:
-    """hour"""
-    return 60. * self.minute
-
-@property
-def day(self) -> float:
-    """solar day"""
-    return 24. * self.hour
-
-@property
-def week(self) -> float:
-    """week"""
-    return 7. * self.day
-
-@property
-def year(self) -> float:
-    """sidereal year"""
-    return 365.256363004 * self.day
+@property
+def mol(self) -> float:
+    """mole"""
+    return self.NA
+
+@property
+def mmol(self) -> float:
+    """millimole"""
+    return 1e-3 * self.mol
+
+@property
+def umol(self) -> float:
+    """micromole"""
+    return 1e-6 * self.mol
+
+@property
+def nmol(self) -> float:
+    """nanomole"""
+    return 1e-9 * self.mol
+
+@property
+def pmol(self) -> float:
+    """picomole"""
+    return 1e-12 * self.mol
+
+@property
+def fmol(self) -> float:
+    """femtomole"""
+    return 1e-15 * self.mol
+
+@property
+def M(self) -> float:
+    """molar"""
+    return self.mol / self.L
+
+@property
+def mM(self) -> float:
+    """millimolar"""
+    return 1e-3 * self.M
+
+@property
+def uM(self) -> float:
+    """micromolar"""
+    return 1e-6 * self.M
+
+@property
+def nM(self) -> float:
+    """nanomolar"""
+    return 1e-9 * self.M
+
+@property
+def pM(self) -> float:
+    """picomolar"""
+    return 1e-12 * self.M
+
+@property
+def fM(self) -> float:
+    """femtomolar"""
+    return 1e-15 * self.M
```

### Comparing `yabadaba-0.2.1/yabadaba/UnitConverter/_voltage.py` & `yabadaba-0.2.2/yabadaba/UnitConverter/_volume.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,49 @@
-@property 
-def V(self) -> float:
-    """volt"""
-    return self.J / self.C
-
-@property
-def mV(self) -> float:
-    """millivolt"""
-    return 1e-3 * self.V
-
-@property
-def uV(self) -> float:
-    """microvolt"""
-    return 1e-6 * self.V
-
-@property
-def nV(self) -> float:
-    """nanovolt"""
-    return 1e-9 * self.V
-
-@property
-def kV(self) -> float:
-    """kilovolt"""
-    return 1e3 * self.V
-
-@property
-def MV(self) -> float:
-    """megavolt"""
-    return 1e6 * self.V
-
-@property
-def GV(self) -> float:
-    """gigavolt"""
-    return 1e9 * self.V
-
-@property
-def TV(self) -> float:
-    """teravolt"""
-    return 1e12 * self.V
+@property
+def L(self) -> float:
+    """liter"""
+    return 1e-3 * self.m**3
+
+@property
+def mL(self) -> float:
+    """milliliter"""
+    return 1e-3 * self.L
+
+@property
+def uL(self) -> float:
+    """microliter"""
+    return 1e-6 * self.L
+
+@property
+def nL(self) -> float:
+    """nanoliter"""
+    return 1e-9 * self.L
+
+@property
+def pL(self) -> float:
+    """picoliter"""
+    return 1e-12 * self.L
+
+@property
+def fL(self) -> float:
+    """femtoliter"""
+    return 1e-15 * self.L
+
+@property
+def aL(self) -> float:
+    """attoliter"""
+    return 1e-18 * self.L
+
+@property
+def kL(self) -> float:
+    """kiloliter"""
+    return 1e3 * self.L
+
+@property
+def ML(self) -> float:
+    """megaliter"""
+    return 1e6 * self.L
+
+@property
+def GL(self) -> float:
+    """gigaliter"""
+    return 1e9 * self.L
```

### Comparing `yabadaba-0.2.1/yabadaba/__init__.py` & `yabadaba-0.2.2/yabadaba/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# coding: utf-8
-# Standard Python libraries
-from importlib import resources
-
-# Read version from VERSION file
-if hasattr(resources, 'files'):
-    __version__ = resources.files('yabadaba').joinpath('VERSION').read_text(encoding='UTF-8')
-else:
-    __version__ = resources.read_text('yabadaba', 'VERSION', encoding='UTF-8').strip()
-
-# Relative imports
-from .UnitConverter import unitconvert
-from . import tools
-from .Settings import settings
-
-from . import demo
-
-from . import query
-from .query import querymanager, load_query
-
-from . import record
-from .record import recordmanager, load_record
-
-from . import database
-from .database import databasemanager, load_database
-
-__all__ = ['__version__', 'tools', 'settings', 'unitconvert',
-           'query', 'load_query', 'querymanager', 'demo',
-           'record', 'load_record', 'recordmanager',
-           'database', 'load_database', 'databasemanager']
-__all__.sort()
+# coding: utf-8
+# Standard Python libraries
+from importlib import resources
+
+# Read version from VERSION file
+if hasattr(resources, 'files'):
+    __version__ = resources.files('yabadaba').joinpath('VERSION').read_text(encoding='UTF-8')
+else:
+    __version__ = resources.read_text('yabadaba', 'VERSION', encoding='UTF-8').strip()
+
+# Relative imports
+from .UnitConverter import unitconvert
+from . import tools
+from .Settings import settings
+
+from . import demo
+
+from . import query
+from .query import querymanager, load_query
+
+from . import record
+from .record import recordmanager, load_record
+
+from . import database
+from .database import databasemanager, load_database
+
+__all__ = ['__version__', 'tools', 'settings', 'unitconvert',
+           'query', 'load_query', 'querymanager', 'demo',
+           'record', 'load_record', 'recordmanager',
+           'database', 'load_database', 'databasemanager']
+__all__.sort()
```

### Comparing `yabadaba-0.2.1/yabadaba/database/CDCSDatabase.py` & `yabadaba-0.2.2/yabadaba/database/MongoDatabase.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,664 +1,696 @@
-# coding: utf-8
-# Standard Python libraries
-from pathlib import Path
-import shutil
-import tarfile
-from io import BytesIO
-from typing import Optional, Tuple, Union
-
-# https://github.com/usnistgov/pycdcs
-from cdcs import CDCS
-
-# http://www.numpy.org/
-import numpy as np
-
-# https://pandas.pydata.org/
-import pandas as pd
-
-# Relative imports
-from ..tools import aslist, iaslist
-from . import Database
-from .. import load_record, recordmanager
-
-class CDCSDatabase(Database):
-
-    def __init__(self,
-                 host: str,
-                 username: Optional[str] = None,
-                 password: Optional[str] = None,
-                 auth: Optional[Tuple[str]] = None,
-                 cert: Union[str, Tuple[str], None] = None, 
-                 certification: Union[str, Tuple[str], None] = None,
-                 verify: Optional[bool] = True,
-                 cdcsversion: Optional[str] = None):
-        """
-        Initializes a database of style curator.
-        
-        Parameters
-        ----------
-        host : str
-            The host name (url) for the database.
-        username : str, optional
-            Username of desired account on the server. A prompt will ask for
-            the username if not given.
-        password : str, optional
-            Password of desired account on the server.  This can either be the
-            password as a str, or a str path to a file containing only the
-            password.  A prompt will ask for the password if not given.
-        auth : tuple, optional
-            Auth tuple to enable Basic/Digest/Custom HTTP Auth.  Alternative to
-            giving username and password separately.
-        cert : str, optional
-            if String, path to ssl client cert file (.pem). If Tuple,
-            ('cert', 'key') pair.
-        certification : str, optional
-            Alias for cert. Retained for compatibility.
-        verify : bool or str, optional
-            Either a boolean, in which case it controls whether we verify the
-            server's TLS certificate, or a string, in which case it must be a
-            path to a CA bundle to use. Defaults to True.
-        cdcsversion : str, optional
-            For CDCS versions 2.X.X, this allows for specifying the full CDCS
-            version to ensure the class methods perform the correct REST
-            calls.  This can be specified as "#.#.#", or if None is given will
-            default to "2.15.0".  For CDCS versions 3.X.X, this is ignored as
-            version info is obtained directly from the database.
-        """
-        # Fetch password from file if needed
-        try:
-            with open(password, encoding='UTF-8') as f:
-                password = f.read().strip()
-        except Exception:
-            pass
-
-        # Pass parameters to cdcs object
-        self.__cdcs = CDCS(host, username=username, password=password, auth=auth,
-                           cert=cert, certification=certification, verify=verify,
-                           cdcsversion=cdcsversion)
-
-        # Pass host to Database initializer
-        Database.__init__(self, host)
-
-    @property
-    def style(self):
-        """str: The database style"""
-        return 'cdcs'
-
-    @property
-    def cdcs(self):
-        """cdcs.CDCS : The underlying database API object."""
-        return self.__cdcs
-
-    def get_records(self, style=None, return_df=False, name=None,
-                    query=None, keyword=None, **kwargs):
-        """
-        Produces a list of all matching records in the database.
-        
-        Parameters
-        ----------
-        style : str, optional
-            The record style to search. If not given, a prompt will ask for it.
-        name : str or list, optional
-            Record name(s) to delimit by. 
-        return_df : bool, optional
-            If True, then the corresponding pandas.Dataframe of metadata
-            will also be returned
-        query : dict, optional
-            A custom-built CDCS-style query to use for the record search.
-            Alternative to passing in the record-specific metadata kwargs.
-            Note that name can be given with query.
-        keyword : str, optional
-            Allows for a search of records whose contents contain a keyword.
-            Alternative to giving query or kwargs.
-        **kwargs : any, optional
-            Any of the record-specific metadata keywords that can be searched
-            for.
-        
-        Returns
-        ------
-        records : numpy.NDArray
-            All records from the database matching the given parameters.
-        records_df : pandas.DataFrame
-            The corresponding metadata values for the records.  Only returned
-            if return_df is True.
-        """
-        # Set default search parameters
-        if style is None:
-            style = self.select_record_style()
-
-        # Setup keyword search
-        if keyword is not None:
-            assert len(kwargs) == 0, 'keyword cannot be given with kwargs'
-            assert query is None, 'keyword cannot be given with query'
-
-        # Setup query
-        elif query is not None:
-            assert len(kwargs) == 0, 'query cannot be given with kwargs'
-        else:
-            query = load_record(style).cdcsquery(**kwargs)
-
-        def build_records(series):
-            return load_record(series.template_title, model=series.xml_content,
-                               name=series.title, database=self)
-
-        # Build records by querying for each record name (or None)
-        records = []
-        for n in iaslist(name):
-            data = self.cdcs.query(title=n, template=style, mongoquery=query, keyword=keyword)
-            if len(data) > 0:
-                records.extend(data.apply(build_records, axis=1))
-        records = np.array(records)
-
-        # Build df
-        if len(records) > 0:
-            df = []
-            for record in records:
-                df.append(record.metadata())
-            df = pd.DataFrame(df)
-        else:
-            df = pd.DataFrame({'name':[]})
-
-        # Sort by name
-        df = df.sort_values('name')
-        records = records[df.index.tolist()]
-
-        # Return records (and df)
-        if return_df:
-            return records, df.reset_index(drop=True)
-        else:
-            return records
-
-    def get_records_df(self, style=None, name=None, query=None, keyword=None, **kwargs):
-        """
-        Produces a list of all matching records in the database.
-        
-        Parameters
-        ----------
-        style : str, optional
-            The record style to search. If not given, a prompt will ask for it.
-        name : str or list, optional
-            Record name(s) to delimit by. 
-        query : dict, optional
-            A custom-built CDCS-style query to use for the record search.
-            Alternative to passing in the record-specific metadata kwargs.
-            Note that name can be given with query.
-        keyword : str, optional
-            Allows for a search of records whose contents contain a keyword.
-            Alternative to giving query or kwargs.
-        **kwargs : any, optional
-            Any of the record-specific metadata keywords that can be searched
-            for.
-            
-        Returns
-        -------
-        records_df : pandas.DataFrame
-            The corresponding metadata values for the records.
-        """
-        return self.get_records(style, name=name, query=query, keyword=keyword, return_df=True, **kwargs)[1]
-
-    def get_record(self, style=None, name=None, query=None, keyword=None, **kwargs):
-        """
-        Returns a single matching record from the database.
-        
-        Parameters
-        ----------
-        style : str, optional
-            Record style(s) to limit the search by.
-        name : str or list, optional
-            Record name(s) to delimit by. 
-        query : dict, optional
-            A custom-built CDCS-style query to use for the record search.
-            Alternative to passing in the record-specific metadata kwargs.
-            Note that name can be given with query.
-        keyword : str, optional
-            Allows for a search of records whose contents contain a keyword.
-            Alternative to giving query or kwargs.
-        **kwargs : any, optional
-            Any of the record-specific metadata keywords that can be searched
-            for.
-            
-        Returns
-        ------
-        Record
-            The single record from the database matching the given parameters.
-        
-        Raises
-        ------
-        ValueError
-            If multiple or no matching records found.
-        """
-        if style is None:
-            styles = recordmanager.loaded_style_names
-        else:
-            styles = aslist(style)
-
-        # Get records
-        records = []
-        for style in styles:
-            records.append(self.get_records(style, name=name, query=query, keyword=keyword, **kwargs))
-        records = np.hstack(records)
-
-        # Verify that there is only one matching record
-        if len(records) == 1:
-            return records[0]
-        elif len(records) == 0:
-            raise ValueError('No matching records found')
-        else:
-            raise ValueError('Multiple matching records found')
-    
-    def add_record(self, record=None, style=None, name=None, model=None,
-                   build=False, verbose=False, workspace=None):
-        """
-        Adds a new record to the database.
-        
-        Parameters
-        ----------
-        record : iprPy.Record, optional
-            The new record to add to the database.  If not given, then name,
-            style and content are required.
-        style : str, optional
-            The record style for the new record.  Required if record is not
-            given.
-        name : str, optional
-            The name to assign to the new record.  Required if record is not
-            given.
-        model : str or DataModelDict, optional
-            The model contents of the new record.  Required if record is not
-            given.
-        build : bool, optional
-            If True, then the uploaded content will be (re)built based on the
-            record's attributes.  If False (default), then record's existing
-            content will be loaded if it exists, or built if it doesn't exist.
-        workspace : str or pandas.Series, optional
-            The name of a workspace to assign the record to.  If not given
-            then the record is not assigned to a workspace and will only be
-            accessible to the user who uploaded it.
-        verbose : bool, optional
-            If True, info messages will be printed during operations.  Default
-            value is False.
-
-        Returns
-        ------
-        Record
-            Either the given record or a record composed of the name, style, 
-            and model.
-        
-        Raises
-        ------
-        ValueError
-            If style, name and/or model given with record, or a matching record
-            already exists.
-        """
-
-        # Create Record object if not given
-        if record is None:
-            record = load_record(style, model=model, name=name)
-
-        # Issue a ValueError for competing kwargs
-        elif style is not None or name is not None or model is not None:
-            raise ValueError('kwargs style, name, and model cannot be given with kwarg record')
-
-        # Retrieve/build model contents
-        try:
-            assert build is False
-            content = record.model.xml()
-        except Exception:
-            content = record.build_model().xml()
-
-        # Upload to database
-        self.cdcs.upload_record(template=record.style, content=content,
-                                title=record.name)
-        if verbose:
-            print(f'{record} added to {self.host}')
-
-        if workspace is not None:
-            self.assign_records(record, workspace, verbose=verbose)
-
-        return record
-
-    def update_record(self, record=None, style=None, name=None, model=None,
-                      build=False, verbose=False, workspace=None):
-        """
-        Replaces an existing record with a new record of matching name and 
-        style, but new content.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record with new content to update in the database.  If not
-            given, content is required along with name and/or style to
-            uniquely define a record to update.
-        style : str, optional
-            The style of the record to update.
-        name : str, optional
-            The name to uniquely identify the record to update.
-        model : str or DataModelDict, optional
-            The model contents of the new record.  Required if record is not
-            given.
-        build : bool, optional
-            If True, then the uploaded content will be (re)built based on the
-            record's attributes.  If False (default), then record's existing
-            content will be loaded if it exists, or built if it doesn't exist.
-        workspace : str or pandas.Series, optional
-            The name of a workspace to assign the record to.  If not given
-            then the record is not assigned to a workspace and will only be
-            accessible to the user who uploaded it.
-        verbose : bool, optional
-            If True, info messages will be printed during operations.  Default
-            value is False.
-
-        Returns
-        ------
-        Record
-            Either the given record or a record composed of the name, style, 
-            and model.
-            
-        Raises
-        ------
-        TypeError
-            If no new content is given.
-        ValueError
-            If style, model, and/or name given with record.
-        """
-
-        # Create Record object if not given
-        if record is None:
-            if model is None:
-                raise TypeError('no new model given')
-            oldrecord = self.get_record(name=name, style=style)
-            record = load_record(oldrecord.style, model=model, name=oldrecord.name)
-
-        # Use given record object
-        else:
-            if style is not None or name is not None:
-                raise ValueError('kwargs style and name cannot be given with kwarg record')
-
-            # Replace model in record object
-            if model is not None:
-                record = load_record(record.style, model=model, name=record.name)
-
-        # Retrieve/build model contents
-        try:
-            assert build is False
-            content = record.model.xml()
-        except Exception:
-            content = record.build_model().xml()
-
-        # Upload to database
-        self.cdcs.update_record(template=record.style, content=content,
-                                title=record.name)
-
-        if verbose:
-            print(f'{record} updated in {self.host}')
-
-        if workspace is not None:
-            self.assign_records(record, workspace, verbose=verbose)
-
-        return record
-
-    def delete_record(self, record=None, style=None, name=None, verbose=False):
-        """
-        Permanently deletes a record from the database.  Will issue an error 
-        if exactly one matching record is not found in the database.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record to delete from the database.  If not given, name and/or
-            style are needed to uniquely define the record to delete.
-        name : str, optional
-            The name of the record to delete.
-        style : str, optional
-            The style of the record to delete.
-        verbose : bool, optional
-            If True, info messages will be printed during operations.  Default
-            value is False.
-            
-        Raises
-        ------
-        ValueError
-            If style and/or name content given with record.
-        """
-        # Extract values from Record object if given
-        if record is not None:
-            if style is not None or name is not None:
-                raise ValueError('kwargs style and name cannot be given with kwarg record')
-            name = record.name
-            style = record.style
-
-        # Delete record
-        self.cdcs.delete_record(template=style, title=name)
-
-        if verbose:
-            print(f'{record} deleted from {self.host}')
-
-    def assign_records(self, records, workspace, verbose=False):
-        """
-        Assigns one or more records to a CDCS workspace.
-
-        Parameters
-        ----------
-        records : Record or list
-            The record(s) to assign to the workspace.
-        workspace : str
-            The workspace to assign the records to.
-        verbose : bool, optional
-            Setting this to True will print extra status messages.  Default
-            value is False.
-        """
-        #ids = []
-        for record in aslist(records):
-            self.cdcs.assign_records(workspace, template=record.style,
-                                     title=record.name)
-            if verbose:
-                print(f'{record} assigned to workspace {workspace}')
-
-    def add_tar(self, record=None, style=None, name=None, tar=None, root_dir=None):
-        """
-        Archives and stores a folder associated with a record.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record to associate the tar archive with.  If not given, then
-            name and/or style necessary to uniquely identify the record are
-            needed.
-        name : str, optional
-            The name to use in uniquely identifying the record.
-        style : str, optional
-            The style to use in uniquely identifying the record.
-        tar : bytes, optional
-            The bytes content of a tar file to save.  tar cannot be given
-            with root_dir.
-        root_dir : str, optional
-            Specifies the root directory for finding the directory to archive.
-            The directory to archive is at <root_dir>/<name>.  (Default is to
-            set root_dir to the current working directory.)  tar cannot be given
-            with root_dir.
-        
-        Raises
-        ------
-        ValueError
-            If style and/or name content given with record or the record already
-            has an archive.
-        """
-
-        # Get Record object if not given
-        if record is None:
-            record = self.get_record(name=name, style=style)
-
-        else:
-            # Issue a ValueError for competing kwargs
-            if style is not None or name is not None:
-                raise ValueError('kwargs style and name cannot be given with kwarg record')
-
-            # Verify that record exists
-            record = self.get_record(name=record.name, style=record.style)
-
-        # Check if an archive already exists
-        blobs = self.cdcs.get_blobs(filename=record.name)
-        if len(blobs) > 0:
-            raise ValueError('Record already has an archive')
-
-        # Create directory archive and upload
-        if tar is None: 
-            if root_dir is None:
-                root_dir = Path.cwd()
-
-            # Make archive
-            basename = Path(root_dir, record.name)
-            filename = Path(root_dir, record.name + '.tar.gz')
-            shutil.make_archive(basename, 'gztar', root_dir=root_dir,
-                                base_dir=record.name)
-
-            # Upload archive
-            tries = 0
-            while tries < 2:
-                tries += 1
-                try:
-                    url = self.cdcs.upload_blob(filename.as_posix())
-                    break
-                except Exception as err:
-                    if tries == 2:
-                        raise ValueError('Failed to upload archive 2 times') from err
-
-            # Remove local archive copy
-            filename.unlink()
-
-        # Upload pre-existing tar object
-        elif root_dir is None:
-            filename = Path(record.name + '.tar.gz')
-
-            # Upload archive
-            tries = 0
-            while tries < 2:
-                tries += 1
-                try:
-                    url = self.cdcs.upload_blob(filename=filename, blobbytes=BytesIO(tar))
-                    break
-                except Exception as err:
-                    if tries == 2:
-                        raise ValueError('Failed to upload archive 2 times') from err
-
-        else:
-            raise ValueError('tar and root_dir cannot both be given')
-
-    def get_tar(self, record=None, style=None, name=None, raw=False):
-        """
-        Retrives the tar archive associated with a record in the database.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record to retrive the associated tar archive for.
-        name : str, optional
-            The name to use in uniquely identifying the record.
-        style : str, optional
-            The style to use in uniquely identifying the record.
-        raw : bool, optional
-            If True, return the archive as raw binary content. If 
-            False, return as an open tarfile. (Default is False)
-            
-        Returns
-        -------
-        tarfile or str
-            The tar archive as an open tarfile if raw=False, or as a binary str if
-            raw=True.
-            
-        Raises
-        ------
-        ValueError
-            If style and/or name content given with record.
-        """
-
-        # Create Record object if not given
-        if record is None:
-            record = self.get_record(name=name, style=style)
-
-        # Issue a TypeError for competing kwargs
-        elif style is not None or name is not None:
-            raise TypeError('kwargs style and name cannot be given with kwarg record')
-
-        # Verify that record exists
-        #else:
-        #    record = self.get_record(name=record.name, style=record.style)
-
-        filename = Path(record.name + '.tar.gz')
-
-        # Download tar file
-        tardata = self.cdcs.get_blob_contents(filename=filename)
-
-        tar = tarfile.open(fileobj = BytesIO(tardata))
-
-        record.tar = tar
-
-        # Return contents
-        if raw is True:
-            return tardata
-        else:
-            return tar
-
-    def delete_tar(self, record=None, style=None, name=None):
-        """
-        Deletes a tar file from the database.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record associated with the tar archive to delete.  If not
-            given, then name and/or style necessary to uniquely identify
-            the record are needed.
-        name : str, optional
-            The name to use in uniquely identifying the record.
-        style : str, optional
-            The style to use in uniquely identifying the record.
-        """
-
-        # Create Record object if not given
-        if record is None:
-            record = self.get_record(name=name, style=style)
-
-        # Issue a TypeError for competing kwargs
-        elif style is not None or name is not None:
-            raise TypeError('kwargs style and name cannot be given with kwarg record')
-
-        # Verify that record exists
-        else:
-            record = self.get_record(name=record.name, style=record.style)
-
-        filename = Path(record.name + '.tar.gz')
-
-        self.cdcs.delete_blob(filename=filename)
-
-    def update_tar(self, record=None, style=None, name=None, tar=None, root_dir=None):
-        """
-        Archives and stores a folder associated with a record.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record to associate the tar archive with.  If not given, then
-            name and/or style necessary to uniquely identify the record are
-            needed.
-        name : str, optional
-            The name to use in uniquely identifying the record.
-        style : str, optional
-            The style to use in uniquely identifying the record.
-        tar : bytes, optional
-            The bytes content of a tar file to save.  tar cannot be given
-            with root_dir.
-        root_dir : str, optional
-            Specifies the root directory for finding the directory to archive.
-            The directory to archive is at <root_dir>/<name>.  (Default is to
-            set root_dir to the current working directory.)  tar cannot be given
-            with root_dir.
-        
-        Raises
-        ------
-        ValueError
-            If style and/or name content given with record or the record already
-            has an archive.
-        """
-
-        self.delete_tar(record=record, name=name, style=style)
-        self.add_tar(record=record, name=name, style=style, tar=tar, root_dir=root_dir)
+# coding: utf-8
+# Standard Python libraries
+from pathlib import Path
+import shutil
+import tarfile
+from collections import OrderedDict
+from typing import Optional, Tuple, Union
+
+# http://www.numpy.org/
+import numpy as np
+
+# https://pandas.pydata.org/
+import pandas as pd
+
+# https://api.mongodb.com/python/current/
+import pymongo
+from pymongo import MongoClient
+from gridfs import GridFS
+
+# https://github.com/usnistgov/DataModelDict
+from DataModelDict import DataModelDict as DM
+
+# Relative imports
+from ..tools import aslist
+from . import Database
+from ..record import recordmanager, load_record, Record
+
+class MongoDatabase(Database):
+
+    def __init__(self,
+                 host: str = 'localhost',
+                 port: int = 27017,
+                 database: str = 'iprPy',
+                 **kwargs):
+        """
+        Initializes a connection to a Mongo database.
+        
+        Parameters
+        ----------
+        host : str, optional
+            The mongo host to connect to.  Default value is 'localhost'.
+        port : int, optional
+            Then port to use in connecting to the mongo host.  Default value
+            is 27017.
+        database : str, optional
+            The name of the database in the mongo host to interact with.
+            Default value is 'iprPy'
+        **kwargs : dict, optional
+            Any extra keyword arguments needed to initialize a
+            pymongo.MongoClient object.
+        """
+
+        # Connect to underlying class
+        self.__mongodb = MongoClient(host=host, port=port, document_class=DM, **kwargs)[database]
+
+        # Define class host using client's host, port and database name
+        host = f'{host}:{port}.{database}'
+
+        # Pass host to Database initializer
+        Database.__init__(self, host)
+
+    @property
+    def style(self) -> str:
+        """str: The database style"""
+        return 'mongo'
+
+    @property
+    def mongodb(self) -> pymongo.database.Database:
+        """pymongo.Database : The underlying database API object."""
+        return self.__mongodb
+
+    def get_records(self,
+                    style: Optional[str] = None,
+                    return_df: bool = False,
+                    query: Optional[dict] = None,
+                    **kwargs) -> Union[list, Tuple[list, pd.DataFrame]]:
+        """
+        Produces a list of all matching records in the database.
+        
+        Parameters
+        ----------
+        style : str, optional
+            The record style to search.  If not given, a prompt will ask for it.
+        return_df : bool, optional
+            If True, then the corresponding pandas.Dataframe of metadata
+            will also be returned
+        query : dict, optional
+            A custom-built Mongo-style query to use for the record search.
+            Alternative to passing in the record-specific metadata kwargs.
+        **kwargs : any, optional
+            Any of the record-specific metadata keywords that can be searched
+            for.
+            
+        Returns
+        ------
+        records : numpy.NDArray
+            All records from the database matching the given parameters.
+        records_df : pandas.DataFrame
+            The corresponding metadata values for the records.  Only returned
+            if return_df is True.
+        """
+        # Set default search parameters
+        if style is None:
+            style = self.select_record_style()
+
+        # Use given query
+        if query is not None:
+            assert len(kwargs) == 0, 'query cannot be given with kwargs'
+        else:
+            query = load_record(style).mongoquery(**kwargs)
+
+        # Query the collection to construct records
+        records = []
+        collection = self.mongodb[style]
+        for entry in collection.find(query):
+            record = load_record(style, model=entry['content'],
+                                 name=entry['name'], database=self)
+            records.append(record)
+        records = np.array(records)
+
+        # Build df
+        if len(records) > 0:
+            df = []
+            for record in records:
+                df.append(record.metadata())
+            df = pd.DataFrame(df)
+        else:
+            df = pd.DataFrame({'name':[]})
+
+        # Sort by name
+        df = df.sort_values('name')
+        records = records[df.index.tolist()]
+
+        # Return records (and df)
+        if return_df:
+            return records, df.reset_index(drop=True)
+        else:
+            return records
+
+    def get_records_df(self,
+                       style: Optional[str] = None,
+                       query: Optional[dict] = None,
+                       **kwargs) -> pd.DataFrame:
+        """
+        Produces a pandas.Dataframe of all matching records in the database.
+        
+        Parameters
+        ----------
+        style : str, optional
+            The record style to search.
+        query : dict, optional
+            A custom-built Mongo-style query to use for the record search.
+            Alternative to passing in the record-specific metadata keywords.
+        **kwargs : any, optional
+            Any of the record-specific metadata keywords that can be searched
+            for.
+            
+        Returns
+        -------
+        records_df : pandas.DataFrame
+            The corresponding metadata values for the records.
+        """
+        return self.get_records(style, query=query, return_df=True, **kwargs)[1]
+
+    def get_record(self,
+                   style: Optional[str] = None,
+                   query: Optional[dict] = None,
+                   **kwargs) -> Record:
+        """
+        Retrieves a single matching record from the database.
+        
+        Parameters
+        ----------
+        style : str, optional
+            The record style to search.
+        query : dict, optional
+            A custom-built Mongo-style query to use for the record search.
+            Alternative to passing in the record-specific metadata keywords.
+        **kwargs : any, optional
+            Any of the record-specific metadata keywords that can be searched
+            for.
+            
+        Returns
+        ------
+        Record
+            The record from the database matching the given parameters.
+        
+        Raises
+        ------
+        ValueError
+            If multiple or no matching records found.
+        """
+
+        if style is None:
+            styles = recordmanager.loaded_style_names
+        else:
+            styles = aslist(style)
+
+        # Get records
+        records = []
+        for style in styles:
+            records.append(self.get_records(style, query=query, **kwargs))
+        records = np.hstack(records)
+
+        # Verify that there is only one matching record
+        if len(records) == 1:
+            return records[0]
+        elif len(records) == 0:
+            raise ValueError('No matching records found')
+        else:
+            raise ValueError('Multiple matching records found')
+
+    def count_records(self,
+                      style: Optional[str] = None,
+                      query: Optional[dict] = None,
+                      **kwargs) -> int:
+        """
+        Retrieves a count of matching records from the database.  Much faster
+        than get_records if you only want to know the number of matches.
+        
+        Parameters
+        ----------
+        style : str, optional
+            The record style to search.
+        query : dict, optional
+            A custom-built Mongo-style query to use for the record search.
+            Alternative to passing in the record-specific metadata keywords.
+        **kwargs : any, optional
+            Any of the record-specific metadata keywords that can be searched
+            for.
+            
+        Returns
+        ------
+        int
+            The count of records in the database matching the given parameters.
+        """
+        # Set default search parameters
+        if style is None:
+            style = self.select_record_style()
+
+        # Use given query
+        if query is not None:
+            assert len(kwargs) == 0, 'query cannot be given with kwargs'
+        else:
+            query = load_record(style).mongoquery(**kwargs)
+
+        # Query the collection to construct records
+        collection = self.mongodb[style]
+        count = collection.count_documents(query)
+
+        return count
+
+    def add_record(self,
+                   record: Optional[Record] = None,
+                   style: Optional[str] = None,
+                   name: Optional[str] = None,
+                   model: Union[str, DM, None] = None,
+                   build: bool = False,
+                   verbose: bool = False) -> Record:
+        """
+        Adds a new record to the database.
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The new record to add to the database.  If not given, then name,
+            style and content are required.
+        style : str, optional
+            The record style for the new record.  Required if record is not
+            given.
+        name : str, optional
+            The name to assign to the new record.  Required if record is not
+            given.
+        model : str or DataModelDict, optional
+            The model contents of the new record.  Required if record is not
+            given.
+        build : bool, optional
+            If True, then the uploaded content will be (re)built based on the
+            record's attributes.  If False (default), then record's existing
+            content will be loaded if it exists, or built if it doesn't exist.
+        verbose : bool, optional
+            If True, info messages will be printed during operations.  Default
+            value is False.
+
+        Returns
+        ------
+        Record
+            Either the given record or a record composed of the name, style,
+            and content.
+        
+        Raises
+        ------
+        ValueError
+            If style, name and/or content given with record, or a matching record
+            already exists.
+        """
+
+        # Create Record object if not given
+        if record is None:
+            record = load_record(style, model=model, name=name)
+
+        # Issue a ValueError for competing kwargs
+        elif style is not None or name is not None or model is not None:
+            raise ValueError('kwargs style, name, and content cannot be given with kwarg record')
+
+        # Verify that there isn't already a record with a matching name
+        if len(self.get_records(name=record.name, style=record.style)) > 0:
+            raise ValueError(f'Record {record.name} already exists')
+
+        # Retrieve/build model contents
+        try:
+            assert build is False
+            model = record.model
+        except:
+            model = record.build_model()
+
+        # Create meta mongo entry
+        entry = OrderedDict()
+        entry['name'] = record.name
+        entry['content'] = model
+
+        # Upload to mongodb
+        self.mongodb[record.style].insert_one(entry)
+
+        if verbose:
+            print(f'{record} added to {self.host}')
+
+        return record
+
+    def update_record(self,
+                      record: Optional[Record] = None,
+                      style: Optional[str] = None,
+                      name: Optional[str] = None,
+                      model: Union[str, DM, None] = None,
+                      build: bool = False,
+                      verbose: bool = False) -> Record:
+        """
+        Replaces an existing record with a new record of matching name and
+        style, but new content.
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The record with new content to update in the database.  If not
+            given, content is required along with name and/or style to
+            uniquely define a record to update.
+        style : str, optional
+            The style of the record to update.
+        name : str, optional
+            The name to uniquely identify the record to update.
+        model : str or DataModelDict, optional
+            The model contents of the new record.  Required if record is not
+            given.
+        build : bool, optional
+            If True, then the uploaded content will be (re)built based on the
+            record's attributes.  If False (default), then record's existing
+            content will be loaded if it exists, or built if it doesn't exist.
+        verbose : bool, optional
+            If True, info messages will be printed during operations.  Default
+            value is False.
+        
+        Returns
+        ------
+        Record
+            Either the given record or a record composed of the name, style,
+            and content.
+        
+        Raises
+        ------
+        TypeError
+            If no new content is given.
+        ValueError
+            If style and/or name content given with record.
+        """
+
+        # Create Record object if not given
+        if record is None:
+            if model is None:
+                raise TypeError('no new model given')
+            oldrecord = self.get_record(name=name, style=style)
+            record = load_record(oldrecord.style, model=model, name=oldrecord.name)
+
+        # Issue a ValueError for competing kwargs
+        elif style is not None or name is not None:
+            raise ValueError('kwargs style and name cannot be given with kwarg record')
+
+        # Replace model in record object
+        elif model is not None:
+            oldrecord = record
+            record = load_record(oldrecord.style, model=model, name=oldrecord.name)
+
+        # Find oldrecord matching record
+        else:
+            oldrecord = self.get_record(name=record.name, style=record.style)
+
+        # Delete oldrecord
+        self.delete_record(record=oldrecord)
+
+        # Add new record
+        self.add_record(record=record, build=build)
+
+        if verbose:
+            print(f'{record} updated in {self.host}')
+
+        return record
+
+    def delete_record(self,
+                      record: Optional[Record] = None,
+                      style: Optional[str] = None,
+                      name: Optional[str] = None,
+                      verbose: bool = False):
+        """
+        Permanently deletes a record from the database. 
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The record to delete from the database.  If not given, name and/or
+            style are needed to uniquely define the record to delete.
+        name : str, optional
+            The name of the record to delete.
+        style : str, optional
+            The style of the record to delete.
+        verbose : bool, optional
+            If True, info messages will be printed during operations.  Default
+            value is False.
+
+        Raises
+        ------
+        ValueError
+            If style and/or name content given with record.
+        """
+
+        # Create Record object if not given
+        if record is None:
+            record = self.get_record(name=name, style=style)
+
+        # Issue a ValueError for competing kwargs
+        elif style is not None or name is not None:
+            raise ValueError('kwargs style and name cannot be given with kwarg record')
+
+        # Verify that record exists
+        else:
+            record = self.get_record(name=record.name, style=record.style)
+
+        # Build delete query
+        query = {}
+        query['name'] = record.name
+
+        # Delete record 
+        self.mongodb[record.style].delete_one(query)
+
+        if verbose:
+            print(f'{record} deleted from {self.host}')
+
+    def add_tar(self, 
+                record: Optional[Record] = None,
+                style: Optional[str] = None,
+                name: Optional[str] = None,
+                tar: Optional[bytes] = None,
+                root_dir: Optional[Path] = None):
+        """
+        Archives and stores a folder associated with a record.
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The record to associate the tar archive with.  If not given, then
+            name and/or style necessary to uniquely identify the record are
+            needed.
+        name : str, optional
+            .The name to use in uniquely identifying the record.
+        style : str, optional
+            .The style to use in uniquely identifying the record.
+        tar : bytes, optional
+            The bytes content of a tar file to save.  tar cannot be given
+            with root_dir.
+        root_dir : str, optional
+            Specifies the root directory for finding the directory to archive.
+            The directory to archive is at <root_dir>/<name>.  (Default is to
+            set root_dir to the current working directory.)  tar cannot be given
+            with root_dir.
+        
+        Raises
+        ------
+        ValueError
+            If style and/or name content given with record or the record already
+            has an archive.
+        """
+        # Create Record object if not given
+        if record is None:
+            record = self.get_record(name=name, style=style)
+
+        # Issue a ValueError for competing kwargs
+        elif style is not None or name is not None:
+            raise ValueError('kwargs style and name cannot be given with kwarg record')
+
+        # Verify that record exists
+        else:
+            record = self.get_record(name=record.name, style=record.style)
+
+        # Define mongofs
+        mongofs = GridFS(self.mongodb, collection=record.style)
+
+        # Check if an archive already exists
+        if mongofs.exists({"recordname": record.name}):
+            raise ValueError('Record already has an archive')
+
+        if tar is None:
+            if root_dir is None:
+                root_dir = Path.cwd()
+
+            # Make archive
+            basename = Path(root_dir, record.name)
+            filename = Path(root_dir, record.name + '.tar.gz')
+            shutil.make_archive(basename, 'gztar', root_dir=root_dir,
+                                base_dir=record.name)
+
+            # Upload archive
+            with open(filename, 'rb') as f:
+                tries = 0
+                while tries < 2:
+                    tries += 1
+                    try:
+                        mongofs.put(f, recordname=record.name)
+                        break
+                    except Exception as err:
+                        if tries == 2:
+                            raise ValueError('Failed to upload archive 2 times') from err
+
+            # Remove local archive copy
+            filename.unlink()
+
+        elif root_dir is None:
+            # Upload archive
+            tries = 0
+            while tries < 2:
+                tries += 1
+                try:
+                    mongofs.put(tar, recordname=record.name)
+                    break
+                except Exception as err:
+                    if tries == 2:
+                        raise ValueError('Failed to upload archive 2 times') from err
+        else:
+            raise ValueError('tar and root_dir cannot both be given')
+
+    def get_tar(self,
+                record: Optional[Record] = None,
+                style: Optional[str] = None,
+                name: Optional[str] = None,
+                raw: bool = False) -> Union[tarfile.TarFile, bytes]:
+        """
+        Retrieves the tar archive associated with a record in the database.
+                
+        Parameters
+        ----------
+        record : Record, optional
+            The record to retrieve the associated tar archive for.
+        name : str, optional
+            .The name to use in uniquely identifying the record.
+        style : str, optional
+            .The style to use in uniquely identifying the record.
+        raw : bool, optional
+            If True, return the archive as raw binary content. If 
+            False, return as an open tarfile. (Default is False)
+        
+        Returns
+        -------
+        tarfile or str
+            The tar archive as an open tarfile if raw=False, or as a binary str if
+            raw=True.
+        
+        Raises
+        ------
+        ValueError
+            If style and/or name content given with record.
+        """
+
+        # Create Record object if not given
+        if record is None:
+            record = self.get_record(name=name, style=style)
+
+        # Issue a TypeError for competing kwargs
+        elif style is not None or name is not None:
+            raise TypeError('kwargs style and name cannot be given with kwarg record')
+
+        # Define mongofs
+        mongofs = GridFS(self.mongodb, collection=record.style)
+
+        # Build query
+        query = {}
+        query['recordname'] = record.name
+
+        # Get tar
+        matches = list(mongofs.find(query))
+        if len(matches) == 1:
+            tar = matches[0]
+        elif len(matches) == 0:
+            raise ValueError('No tar found for the record')
+        else:
+            raise ValueError('Multiple tars found for the record')
+
+        # Return content
+        if raw is True:
+            return tar.read()
+        else:
+            tarobj = tarfile.open(fileobj=tar)
+            record.tar = tarobj
+            return tarobj
+
+    def delete_tar(self, 
+                   record: Optional[Record] = None,
+                   style: Optional[str] = None,
+                   name: Optional[str] = None):
+        """
+        Deletes a tar file from the database.
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The record associated with the tar archive to delete.  If not
+            given, then name and/or style necessary to uniquely identify
+            the record are needed.
+        name : str, optional
+            The name to use in uniquely identifying the record.
+        style : str, optional
+            The style to use in uniquely identifying the record.
+        
+        Raises
+        ------
+        ValueError
+            If style and/or name content given with record.
+        """
+
+        # Create Record object if not given
+        if record is None:
+            record = self.get_record(name=name, style=style)
+
+        # Issue a ValueError for competing kwargs
+        elif style is not None or name is not None:
+            raise ValueError('kwargs style and name cannot be given with kwarg record')
+
+        # Define mongofs
+        mongofs = GridFS(self.mongodb, collection=record.style)
+
+        # Build query
+        query = {}
+        query['recordname'] = record.name
+
+        # Get tar
+        matches = list(mongofs.find(query))
+        if len(matches) == 1:
+            tar = matches[0]
+        elif len(matches) == 0:
+            raise ValueError('No tar found for the record')
+        else:
+            raise ValueError('Multiple tars found for the record')
+
+        # Delete tar
+        mongofs.delete(tar._id)
+
+    def update_tar(self,
+                   record: Optional[Record] = None,
+                   style: Optional[str] = None,
+                   name: Optional[str] = None,
+                   tar: Optional[bytes] = None,
+                   root_dir: Optional[Path] = None):
+        """
+        Replaces an existing tar archive for a record with a new one. 
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The record to associate the tar archive with.  If not given, then 
+            name and/or style necessary to uniquely identify the record are 
+            needed.
+        name : str, optional
+            The name to use in uniquely identifying the record.
+        style : str, optional
+            The style to use in uniquely identifying the record.
+        tar : bytes, optional
+            The bytes content of a tar file to save.  tar cannot be given
+            with root_dir.
+        root_dir : str, optional
+            Specifies the root directory for finding the directory to archive.
+            The directory to archive is at <root_dir>/<name>.  (Default is to
+            set root_dir to the current working directory.)  tar cannot be given
+            with root_dir.
+        """
+
+        # Delete the existing tar archive stored in the database
+        self.delete_tar(record=record, name=name, style=style)
+
+        # Add the new tar archive
+        self.add_tar(record=record, name=name, style=style, tar=tar, root_dir=root_dir)
```

### Comparing `yabadaba-0.2.1/yabadaba/database/Database.py` & `yabadaba-0.2.2/yabadaba/database/Database.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,574 +1,662 @@
-# coding: utf-8
-# Standard Python libraries
-from pathlib import Path
-
-from tqdm import tqdm
-
-# iprPy imports
-from ..record import recordmanager, load_record
-from ..tools import screen_input
-
-class Database():
-    """
-    Class for handling different database styles in the same fashion.  This
-    base class defines the common methods and attributes.
-    """
-
-    def __init__(self, host):
-        """
-        Initializes a connection to a database.
-        
-        Parameters
-        ----------
-        host : str
-            The host name (path, url, etc.) for the database.
-        """
-        # Check that object is a subclass
-        if self.__module__ == __name__:
-            raise TypeError("Don't use Database itself, only use derived classes")
-
-        # Set property values
-        self.__host = host
-
-    def __str__(self):
-        """
-        Returns
-        -------
-        str
-            The string representation of the database.
-        """
-        return f'database style {self.style} at {self.host}'
-
-    @property
-    def style(self):
-        """str: The database style"""
-        raise NotImplementedError('Not defined for base class')
-
-    @property
-    def host(self):
-        """str: The database's host."""
-        return self.__host
-
-    def get_records(self, style=None, return_df=False, **kwargs):
-        """
-        Produces a list of all matching records in the database.
-        
-        Parameters
-        ----------
-        style : str, optional
-            The record style to search. If not given, a prompt will ask for it.
-        return_df : bool, optional
-            If True, then the corresponding pandas.Dataframe of metadata
-            will also be returned
-        **kwargs : any, optional
-            Any extra options specific to the database style or metadata search
-            parameters specific to the record style.
-            
-        Returns
-        ------
-        records : numpy.NDArray
-            All records from the database matching the given parameters.
-        records_df : pandas.DataFrame
-            The corresponding metadata values for the records.  Only returned
-            if return_df is True.
-        
-        Raises
-        ------
-        AttributeError
-            If get_records is not defined for database style.
-        """
-        raise AttributeError('get_records not defined for Database style')
-
-    def get_record(self, style=None, **kwargs):
-        """
-        Returns a single matching record from the database.  Issues an error
-        if multiple or no matching records are found.
-        
-        Parameters
-        ----------
-        style : str, optional
-            The record style to limit the search by.
-        **kwargs : any, optional
-            Any extra options specific to the database style or metadata search
-            parameters specific to the record style.
-
-        Returns
-        ------
-        Record
-            The single record from the database matching the given parameters.
-        
-        Raises
-        ------
-        AttributeError
-            If get_record is not defined for database style.
-        """
-        raise AttributeError('get_record not defined for Database style')
-
-    def get_records_df(self, style=None, **kwargs):
-        """
-        Produces a pandas.DataFrame of all matching records in the database.
-        
-        Parameters
-        ----------
-        style : str
-            The record style to collect records of.
-        **kwargs : any, optional
-            Any extra options specific to the database style or metadata search
-            parameters specific to the record style.
-
-        Returns
-        ------
-        pandas.DataFrame
-            All records from the database of the given record style.
-        
-        Raises
-        ------
-        AttributeError
-            If get_record is not defined for database style.
-        """
-        raise AttributeError('get_records_df not defined for Database style')
-
-    def retrieve_record(self, style=None, dest=None, format='json', indent=4,
-                        verbose=False, **kwargs):
-        """
-        Gets a single matching record from the database and saves it to a
-        file based on the record's name.
-
-        Parameters
-        ----------
-        style : str, optional
-            The record style to search. If not given, a prompt will ask for it.
-        dest : path, optional
-            The parent directory where the record will be saved to.  If not given,
-            will use the current working directory.
-        format : str, optional
-            The file format to save the record in: 'json' or 'xml'.  Default
-            is 'json'.
-        indent : int, optional
-            The number of space indentation spacings to use in the saved
-            record for the different tiered levels.  Default is 4.  Giving None
-            will create a compact record.
-        verbose : bool, optional
-            If True, info messages will be printed during operations.  Default
-            value is False.
-        **kwargs : any, optional
-            Any extra options specific to the database style or metadata search
-            parameters specific to the record style.
-        """
-        # Set default dest
-        if dest is None:
-            dest = Path.cwd()
-
-        # Get the record
-        record = self.get_record(style=style, **kwargs)
-
-        # Save as json
-        if format == 'json':
-            fname = Path(dest, f'{record.name}.json')
-            with open(fname, 'w', encoding='UTF-8') as f:
-                record.model.json(fp=f, indent=indent, ensure_ascii=False)
-            if verbose:
-                print(f'{fname} saved')
-
-        # Save as xml
-        elif format == 'xml':
-            fname = Path(dest, f'{record.name}.xml')
-            with open(fname, 'w', encoding='UTF-8') as f:
-                record.model.xml(fp=f, indent=indent)
-            if verbose:
-                print(f'{fname} saved')
-
-        else:
-            raise ValueError('Invalid format: must be json or xml.')
-
-    def add_record(self, record=None, style=None, name=None, model=None,
-                   build=False, verbose=False):
-        """
-        Adds a new record to the database.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The new record to add to the database.  If not given, then name,
-            style and content are required.
-        style : str, optional
-            The record style for the new record.  Required if record is not
-            given.
-        name : str, optional
-            The name to assign to the new record.  Required if record is not
-            given.
-        model : str or DataModelDict, optional
-            The model contents of the new record.  Required if record is not
-            given.
-        build : bool, optional
-            If True, then the uploaded content will be (re)built based on the
-            record's attributes.  If False (default), then record's existing
-            content will be loaded if it exists, or built if it doesn't exist.
-        verbose : bool, optional
-            If True, info messages will be printed during operations.  Default
-            value is False.
-            
-        Returns
-        ------
-        Record
-            Either the given record or a record composed of the name, style,
-            and content.
-        
-        Raises
-        ------
-        AttributeError
-            If add_record is not defined for database style.
-        """
-        raise AttributeError('add_record not defined for Database style')
-
-    def update_record(self, record=None, style=None, name=None, model=None,
-                      build=False, verbose=False):
-        """
-        Replaces an existing record with a new record of matching name and
-        style, but new content.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record with new content to update in the database.  If not
-            given, content is required along with name and/or style to
-            uniquely define a record to update.
-        style : str, optional
-            The style of the record to update.
-        name : str, optional
-            The name to uniquely identify the record to update.
-        model : str or DataModelDict, optional
-            The model contents of the new record.  Required if record is not
-            given.
-        build : bool, optional
-            If True, then the uploaded content will be (re)built based on the
-            record's attributes.  If False (default), then record's existing
-            content will be loaded if it exists, or built if it doesn't exist.
-        verbose : bool, optional
-            If True, info messages will be printed during operations.  Default
-            value is False.
-
-        Returns
-        ------
-        Record
-            Either the given record or a record composed of the name, style,
-            and content.
-        
-        Raises
-        ------
-        AttributeError
-            If update_record is not defined for database style.
-        """
-        raise AttributeError('update_record not defined for Database style')
-
-    def delete_record(self, record=None, style=None, name=None):
-        """
-        Permanently deletes a record from the database.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record to delete from the database.  If not given, name and/or
-            style are needed to uniquely define the record to delete.
-        style : str, optional
-            The style of the record to delete.
-        name : str, optional
-            The name of the record to delete.
-        
-        
-        Raises
-        ------
-        AttributeError
-            If delete_record is not defined for database style.
-        """
-        raise AttributeError('delete_record not defined for Database style')
-
-    def get_tar(self, record=None, style=None, name=None, raw=False):
-        """
-        Retrives the tar archive associated with a record in the database.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record to retrieve the associated tar archive for.
-        style : str, optional
-            The style to use in uniquely identifying the record.
-        name : str, optional
-            The name to use in uniquely identifying the record.
-        raw : bool, optional
-            If True, return the archive as raw binary content. If
-            False, return as an open tarfile. (Default is False)
-            
-        Returns
-        -------
-        tarfile or str
-            The tar archive as an open tarfile if raw=False, or as a binary
-            str if raw=True.
-        
-        Raises
-        ------
-        AttributeError
-            If get_tar is not defined for database style.
-        """
-        raise AttributeError('get_tar not defined for Database style')
-
-    def add_tar(self, record=None, style=None, name=None, tar=None, root_dir=None):
-        """
-        Archives and stores a folder associated with a record.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record to associate the tar archive with.  If not given, then
-            name and/or style necessary to uniquely identify the record are
-            needed.
-        style : str, optional
-            The style to use in uniquely identifying the record.
-        name : str, optional
-            The name to use in uniquely identifying the record.
-        tar : bytes, optional
-            The bytes content of a tar file to save.  tar cannot be given
-            with root_dir.
-        root_dir : str, optional
-            Specifies the root directory for finding the directory to archive.
-            The directory to archive is at <root_dir>/<name>.  (Default is to
-            set root_dir to the current working directory.)  tar cannot be given
-            with root_dir.
-        
-        Raises
-        ------
-        ValueError
-            If style and/or name content given with record or the record already
-            has an archive.
-        """
-        raise AttributeError('add_tar not defined for Database style')
-
-    def update_tar(self, record=None, style=None, name=None, tar=None, root_dir=None):
-        """
-        Replaces an existing tar archive for a record with a new one.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record to associate the tar archive with.  If not given, then 
-            name and/or style necessary to uniquely identify the record are 
-            needed.
-        style : str, optional
-            The style to use in uniquely identifying the record.
-        name : str, optional
-            The name to use in uniquely identifying the record.
-        tar : bytes, optional
-            The bytes content of a tar file to save.  tar cannot be given
-            with root_dir.
-        root_dir : str, optional
-            Specifies the root directory for finding the directory to archive.
-            The directory to archive is at <root_dir>/<name>.  (Default is to
-            set root_dir to the current working directory.)  tar cannot be given
-            with root_dir.
-        
-        Raises
-        ------
-        AttributeError
-            If update_tar is not defined for database style.
-        """
-        raise AttributeError('update_tar not defined for Database style')
-
-    def delete_tar(self, record=None, style=None, name=None):
-        """
-        Deletes a tar file from the database.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record associated with the tar archive to delete.  If not
-            given, then name and/or style are necessary to uniquely identify
-            the record.
-        style : str, optional
-            The style to use in uniquely identifying the record.
-        name : str, optional
-            The name to use in uniquely identifying the record.
-        
-        Raises
-        ------
-        AttributeError
-            If delete_tar is not defined for database style.
-        """
-        raise AttributeError('delete_tar not defined for Database style')
-
-    def copy_records(self, dest, record_style=None, records=None, includetar=True, overwrite=False):
-        """
-        Copies records from the current database to another database.
-        
-        Parameters
-        ----------
-        dest :  Database
-            The destination database to copy records to.
-        record_style : str, optional
-            The record style to copy.  If record_style and records not
-            given, then the available record styles will be listed and the
-            user prompted to pick one.  Cannot be given with records.
-        records : list, optional
-            A list of Record objects from the current database to copy
-            to dbase2.  Allows the user full control on which records to
-            copy/update.  Cannot be given with record_style.
-        includetar : bool, optional
-            If True, the tar archives will be copied along with the records.
-            If False, only the records will be copied. (Default is True).
-        overwrite : bool, optional
-            If False (default) only new records and tars will be copied.
-            If True, all existing content will be updated.
-        """
-        if record_style is None and records is None:
-            # Prompt for record_style
-            record_style = self.select_record_style()
-
-        if record_style is not None:
-            if records is not None:
-                raise ValueError('record_style and records cannot both be given')
-
-            # Retrieve records from self
-            records = self.get_records(style=record_style)
-
-        elif records is None:
-            # Set empty list if record_style is still None and no records given
-            records = []
-
-        print(len(records), 'records to try to copy')
-
-        record_count = 0
-        tar_count = 0
-        # Copy records
-        for record in tqdm(records, 'copying records', ascii=True):
-            try:
-                # Add new records
-                dest.add_record(record=record)
-                record_count += 1
-            except:
-                # Update existing records
-                if overwrite:
-                    dest.update_record(record=record)
-                    record_count += 1
-
-            # Copy archives
-            if includetar:
-                try:
-                    # Get tar if it exists
-                    tar = self.get_tar(record=record, raw=True) 
-                except:
-
-                    # Get folder if it exists
-                    try:
-                        root_dir = self.get_folder(record=record).parent
-                    except:
-                        pass
-                    else:
-                        try:
-                            # Copy tar over
-                            dest.add_tar(record=record, root_dir=root_dir)
-                            tar_count += 1
-                        except:
-                            # Update existing tar
-                            if overwrite:
-                                dest.update_tar(record=record, root_dir=root_dir)
-                                tar_count += 1
-
-                else:
-                    try:
-                        # Copy tar over
-                        dest.add_tar(record=record, tar=tar)
-                        tar_count += 1
-                    except:
-                        # Update existing tar
-                        if overwrite:
-                            dest.update_tar(record=record, tar=tar)
-                            tar_count += 1
-
-        print(record_count, 'records added/updated')
-        if includetar:
-            print(tar_count, 'tars added/updated')
-
-    def destroy_records(self, record_style=None, records=None):
-        """
-        Permanently deletes multiple records and their associated tars all at
-        once.
-        
-        Parameters
-        ----------
-        record_style : str, optional
-            The record style to delete.  If given, all records of that style
-            will be deleted. If neither record_style nor records given, then
-            the available record styles will be listed and the user prompted
-            to pick one.
-        records : list, optional
-            A list of pre-selected records to delete. 
-        """
-        # Select record_style if needed
-        if record_style is None and records is None:
-            record_style = self.select_record_style()
-
-        # Get records by record_style
-        if record_style is not None:
-            if records is not None:
-                raise ValueError('record_style and records cannot both be given')
-
-            # Retrieve records with errors from self
-            records = self.get_records(style=record_style) 
-
-        elif records is None:
-            # Set empty list if record_style is still None and no records given
-            records = []
-
-        print(f'{len(records)} records found to be destroyed')
-
-        if len(records) > 0:
-            test = screen_input('Delete records? (must type yes):')
-            if test == 'yes':
-                count = 0
-                record_styles = set()
-                for record in tqdm(records, 'destroying records', ascii=True):
-                    try:
-                        self.delete_tar(record=record)
-                    except:
-                        pass
-                    try:
-                        self.delete_record(record=record)
-                        count += 1
-                        record_styles.add(record.style)
-                    except:
-                        pass
-                if self.style == 'local':
-                    for record_style in record_styles:
-                        cache = self.cache(record_style, refresh=True)
-                print(count, 'records successfully deleted')
-
-    def select_record_style(self):
-        """
-        Console prompt for selecting a record_style
-        """
-        # Build list of calculation records
-        styles = recordmanager.loaded_style_names
-
-        # Ask for selection
-        print('Select record_style:')
-        for i, style in enumerate(styles):
-            print(i+1, style)
-        choice = screen_input(':')
-        try:
-            choice = int(choice)
-        except:
-            record_style = choice
-        else:
-            record_style = styles[choice-1]
-        print()
-
-        return record_style
-
-    def record_querynames(self,
-                          style: str) -> list:
-        """Return the list of query parameter names for a given record style"""
-        return load_record(style).querynames
-
-    def record_querydoc(self,
-                        style: str) -> str:
-        """Return the description of query parameters for a given record style"""
-        return load_record(style).querydoc
+# coding: utf-8
+# Standard Python libraries
+from pathlib import Path
+from typing import Optional, Tuple, Union
+import tarfile
+
+from tqdm import tqdm
+
+import pandas as pd
+
+# https://github.com/usnistgov/DataModelDict
+from DataModelDict import DataModelDict as DM
+
+# iprPy imports
+from ..record import recordmanager, load_record, Record
+from ..tools import screen_input
+
+class Database():
+    """
+    Class for handling different database styles in the same fashion.  This
+    base class defines the common methods and attributes.
+    """
+
+    def __init__(self,
+                 host: str):
+        """
+        Initializes a connection to a database.
+        
+        Parameters
+        ----------
+        host : str
+            The host name (path, url, etc.) for the database.
+        """
+        # Check that object is a subclass
+        if self.__module__ == __name__:
+            raise TypeError("Don't use Database itself, only use derived classes")
+
+        # Set property values
+        self.__host = host
+
+    def __str__(self) -> str:
+        """
+        Returns
+        -------
+        str
+            The string representation of the database.
+        """
+        return f'database style {self.style} at {self.host}'
+
+    @property
+    def style(self) -> str:
+        """str: The database style"""
+        raise NotImplementedError('Not defined for base class')
+
+    @property
+    def host(self) -> str:
+        """str: The database's host."""
+        return self.__host
+
+    def get_records(self, 
+                    style: Optional[str] = None,
+                    return_df: bool = False,
+                    **kwargs) -> Union[list, Tuple[list, pd.DataFrame]]:
+        """
+        Produces a list of all matching records in the database.
+        
+        Parameters
+        ----------
+        style : str, optional
+            The record style to search. If not given, a prompt will ask for it.
+        return_df : bool, optional
+            If True, then the corresponding pandas.Dataframe of metadata
+            will also be returned
+        **kwargs : any, optional
+            Any extra options specific to the database style or metadata search
+            parameters specific to the record style.
+            
+        Returns
+        ------
+        records : numpy.NDArray
+            All records from the database matching the given parameters.
+        records_df : pandas.DataFrame
+            The corresponding metadata values for the records.  Only returned
+            if return_df is True.
+        
+        Raises
+        ------
+        AttributeError
+            If get_records is not defined for database style.
+        """
+        raise AttributeError('get_records not defined for Database style')
+
+    def get_record(self,
+                   style: Optional[str] = None,
+                   **kwargs) -> Record:
+        """
+        Returns a single matching record from the database.  Issues an error
+        if multiple or no matching records are found.
+        
+        Parameters
+        ----------
+        style : str, optional
+            The record style to limit the search by.
+        **kwargs : any, optional
+            Any extra options specific to the database style or metadata search
+            parameters specific to the record style.
+
+        Returns
+        ------
+        Record
+            The single record from the database matching the given parameters.
+        
+        Raises
+        ------
+        AttributeError
+            If get_record is not defined for database style.
+        """
+        raise AttributeError('get_record not defined for Database style')
+
+    def get_records_df(self,
+                       style: Optional[str] = None,
+                       **kwargs) -> pd.DataFrame:
+        """
+        Produces a pandas.DataFrame of all matching records in the database.
+        
+        Parameters
+        ----------
+        style : str
+            The record style to collect records of.
+        **kwargs : any, optional
+            Any extra options specific to the database style or metadata search
+            parameters specific to the record style.
+
+        Returns
+        ------
+        pandas.DataFrame
+            All records from the database of the given record style.
+        
+        Raises
+        ------
+        AttributeError
+            If get_records_df is not defined for database style.
+        """
+        raise AttributeError('get_records_df not defined for Database style')
+
+    def count_records(self,
+                      style: Optional[str] = None,
+                      **kwargs) -> int:
+        """
+        Retrieves a count of matching records from the database.  Depending on the
+        database style, this may be much faster than get_records if you only want
+        to know the number of records
+        
+        Parameters
+        ----------
+        style : str
+            The record style to collect records of.
+        **kwargs : any, optional
+            Any extra options specific to the database style or metadata search
+            parameters specific to the record style.
+
+        Returns
+        ------
+        int
+            A count of the number of matching records in the database
+        
+        Raises
+        ------
+        AttributeError
+            If count_records is not defined for database style.
+        """
+        raise AttributeError('count_records not defined for Database style')
+
+    def retrieve_record(self,
+                        style: Optional[str] = None,
+                        dest: Optional[Path] = None,
+                        format: str = 'json',
+                        indent: Optional[int] = 4,
+                        verbose: bool = False,
+                        **kwargs):
+        """
+        Gets a single matching record from the database and saves it to a
+        file based on the record's name.
+
+        Parameters
+        ----------
+        style : str, optional
+            The record style to search. If not given, a prompt will ask for it.
+        dest : path, optional
+            The parent directory where the record will be saved to.  If not given,
+            will use the current working directory.
+        format : str, optional
+            The file format to save the record in: 'json' or 'xml'.  Default
+            is 'json'.
+        indent : int or None, optional
+            The number of space indentation spacings to use in the saved
+            record for the different tiered levels.  Default is 4.  Giving None
+            will create a compact record.
+        verbose : bool, optional
+            If True, info messages will be printed during operations.  Default
+            value is False.
+        **kwargs : any, optional
+            Any extra options specific to the database style or metadata search
+            parameters specific to the record style.
+        """
+        # Set default dest
+        if dest is None:
+            dest = Path.cwd()
+
+        # Get the record
+        record = self.get_record(style=style, **kwargs)
+
+        # Save as json
+        if format == 'json':
+            fname = Path(dest, f'{record.name}.json')
+            with open(fname, 'w', encoding='UTF-8') as f:
+                record.model.json(fp=f, indent=indent, ensure_ascii=False)
+            if verbose:
+                print(f'{fname} saved')
+
+        # Save as xml
+        elif format == 'xml':
+            fname = Path(dest, f'{record.name}.xml')
+            with open(fname, 'w', encoding='UTF-8') as f:
+                record.model.xml(fp=f, indent=indent)
+            if verbose:
+                print(f'{fname} saved')
+
+        else:
+            raise ValueError('Invalid format: must be json or xml.')
+
+    def add_record(self,
+                   record: Optional[Record] = None,
+                   style: Optional[str] = None,
+                   name: Optional[str] = None,
+                   model: Union[str, DM, None] = None,
+                   build: bool = False,
+                   verbose: bool = False) -> Record:
+        """
+        Adds a new record to the database.
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The new record to add to the database.  If not given, then name,
+            style and content are required.
+        style : str, optional
+            The record style for the new record.  Required if record is not
+            given.
+        name : str, optional
+            The name to assign to the new record.  Required if record is not
+            given.
+        model : str or DataModelDict, optional
+            The model contents of the new record.  Required if record is not
+            given.
+        build : bool, optional
+            If True, then the uploaded content will be (re)built based on the
+            record's attributes.  If False (default), then record's existing
+            content will be loaded if it exists, or built if it doesn't exist.
+        verbose : bool, optional
+            If True, info messages will be printed during operations.  Default
+            value is False.
+            
+        Returns
+        ------
+        Record
+            Either the given record or a record composed of the name, style,
+            and content.
+        
+        Raises
+        ------
+        AttributeError
+            If add_record is not defined for database style.
+        """
+        raise AttributeError('add_record not defined for Database style')
+
+    def update_record(self,
+                      record: Optional[Record] = None,
+                      style: Optional[str] = None,
+                      name: Optional[str] = None,
+                      model: Union[str, DM, None] = None,
+                      build: bool = False,
+                      verbose: bool = False) -> Record:
+        """
+        Replaces an existing record with a new record of matching name and
+        style, but new content.
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The record with new content to update in the database.  If not
+            given, content is required along with name and/or style to
+            uniquely define a record to update.
+        style : str, optional
+            The style of the record to update.
+        name : str, optional
+            The name to uniquely identify the record to update.
+        model : str or DataModelDict, optional
+            The model contents of the new record.  Required if record is not
+            given.
+        build : bool, optional
+            If True, then the uploaded content will be (re)built based on the
+            record's attributes.  If False (default), then record's existing
+            content will be loaded if it exists, or built if it doesn't exist.
+        verbose : bool, optional
+            If True, info messages will be printed during operations.  Default
+            value is False.
+
+        Returns
+        ------
+        Record
+            Either the given record or a record composed of the name, style,
+            and content.
+        
+        Raises
+        ------
+        AttributeError
+            If update_record is not defined for database style.
+        """
+        raise AttributeError('update_record not defined for Database style')
+
+    def delete_record(self,
+                      record: Optional[Record] = None,
+                      style: Optional[str] = None,
+                      name: Optional[str] = None,
+                      verbose: bool = False):
+        """
+        Permanently deletes a record from the database.
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The record to delete from the database.  If not given, name and/or
+            style are needed to uniquely define the record to delete.
+        style : str, optional
+            The style of the record to delete.
+        name : str, optional
+            The name of the record to delete.
+        verbose : bool, optional
+            If True, info messages will be printed during operations.  Default
+            value is False.
+        
+        Raises
+        ------
+        AttributeError
+            If delete_record is not defined for database style.
+        """
+        raise AttributeError('delete_record not defined for Database style')
+
+    def get_tar(self,
+                record: Optional[Record] = None,
+                style: Optional[str] = None,
+                name: Optional[str] = None,
+                raw: bool = False) -> Union[tarfile.TarFile, bytes]:
+        """
+        Retrieves the tar archive associated with a record in the database.
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The record to retrieve the associated tar archive for.
+        style : str, optional
+            The style to use in uniquely identifying the record.
+        name : str, optional
+            The name to use in uniquely identifying the record.
+        raw : bool, optional
+            If True, return the archive as raw binary content. If
+            False, return as an open tarfile. (Default is False)
+            
+        Returns
+        -------
+        tarfile or str
+            The tar archive as an open tarfile if raw=False, or as a binary
+            str if raw=True.
+        
+        Raises
+        ------
+        AttributeError
+            If get_tar is not defined for database style.
+        """
+        raise AttributeError('get_tar not defined for Database style')
+
+    def add_tar(self, 
+                record: Optional[Record] = None,
+                style: Optional[str] = None,
+                name: Optional[str] = None,
+                tar: Optional[bytes] = None,
+                root_dir: Optional[Path] = None):
+        """
+        Archives and stores a folder associated with a record.
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The record to associate the tar archive with.  If not given, then
+            name and/or style necessary to uniquely identify the record are
+            needed.
+        style : str, optional
+            The style to use in uniquely identifying the record.
+        name : str, optional
+            The name to use in uniquely identifying the record.
+        tar : bytes, optional
+            The bytes content of a tar file to save.  tar cannot be given
+            with root_dir.
+        root_dir : str, optional
+            Specifies the root directory for finding the directory to archive.
+            The directory to archive is at <root_dir>/<name>.  (Default is to
+            set root_dir to the current working directory.)  tar cannot be given
+            with root_dir.
+        
+        Raises
+        ------
+        ValueError
+            If style and/or name content given with record or the record already
+            has an archive.
+        """
+        raise AttributeError('add_tar not defined for Database style')
+
+    def update_tar(self,
+                   record: Optional[Record] = None,
+                   style: Optional[str] = None,
+                   name: Optional[str] = None,
+                   tar: Optional[bytes] = None,
+                   root_dir: Optional[Path] = None):
+        """
+        Replaces an existing tar archive for a record with a new one.
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The record to associate the tar archive with.  If not given, then 
+            name and/or style necessary to uniquely identify the record are 
+            needed.
+        style : str, optional
+            The style to use in uniquely identifying the record.
+        name : str, optional
+            The name to use in uniquely identifying the record.
+        tar : bytes, optional
+            The bytes content of a tar file to save.  tar cannot be given
+            with root_dir.
+        root_dir : str, optional
+            Specifies the root directory for finding the directory to archive.
+            The directory to archive is at <root_dir>/<name>.  (Default is to
+            set root_dir to the current working directory.)  tar cannot be given
+            with root_dir.
+        
+        Raises
+        ------
+        AttributeError
+            If update_tar is not defined for database style.
+        """
+        raise AttributeError('update_tar not defined for Database style')
+
+    def delete_tar(self, 
+                   record: Optional[Record] = None,
+                   style: Optional[str] = None,
+                   name: Optional[str] = None):
+        """
+        Deletes a tar file from the database.
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The record associated with the tar archive to delete.  If not
+            given, then name and/or style are necessary to uniquely identify
+            the record.
+        style : str, optional
+            The style to use in uniquely identifying the record.
+        name : str, optional
+            The name to use in uniquely identifying the record.
+        
+        Raises
+        ------
+        AttributeError
+            If delete_tar is not defined for database style.
+        """
+        raise AttributeError('delete_tar not defined for Database style')
+
+    def copy_records(self,
+                     dest,
+                     record_style: Optional[str]  = None,
+                     records: Optional[list] = None,
+                     includetar: bool = True,
+                     overwrite: bool = False):
+        """
+        Copies records from the current database to another database.
+        
+        Parameters
+        ----------
+        dest :  Database
+            The destination database to copy records to.
+        record_style : str, optional
+            The record style to copy.  If record_style and records not
+            given, then the available record styles will be listed and the
+            user prompted to pick one.  Cannot be given with records.
+        records : list, optional
+            A list of Record objects from the current database to copy
+            to dbase2.  Allows the user full control on which records to
+            copy/update.  Cannot be given with record_style.
+        includetar : bool, optional
+            If True, the tar archives will be copied along with the records.
+            If False, only the records will be copied. (Default is True).
+        overwrite : bool, optional
+            If False (default) only new records and tars will be copied.
+            If True, all existing content will be updated.
+        """
+        if record_style is None and records is None:
+            # Prompt for record_style
+            record_style = self.select_record_style()
+
+        if record_style is not None:
+            if records is not None:
+                raise ValueError('record_style and records cannot both be given')
+
+            # Retrieve records from self
+            records = self.get_records(style=record_style)
+
+        elif records is None:
+            # Set empty list if record_style is still None and no records given
+            records = []
+
+        print(len(records), 'records to try to copy')
+
+        record_count = 0
+        tar_count = 0
+        # Copy records
+        for record in tqdm(records, 'copying records', ascii=True):
+            try:
+                # Add new records
+                dest.add_record(record=record)
+                record_count += 1
+            except:
+                # Update existing records
+                if overwrite:
+                    dest.update_record(record=record)
+                    record_count += 1
+
+            # Copy archives
+            if includetar:
+                try:
+                    # Get tar if it exists
+                    tar = self.get_tar(record=record, raw=True) 
+                except:
+
+                    # Get folder if it exists
+                    try:
+                        root_dir = self.get_folder(record=record).parent
+                    except:
+                        pass
+                    else:
+                        try:
+                            # Copy tar over
+                            dest.add_tar(record=record, root_dir=root_dir)
+                            tar_count += 1
+                        except:
+                            # Update existing tar
+                            if overwrite:
+                                dest.update_tar(record=record, root_dir=root_dir)
+                                tar_count += 1
+
+                else:
+                    try:
+                        # Copy tar over
+                        dest.add_tar(record=record, tar=tar)
+                        tar_count += 1
+                    except:
+                        # Update existing tar
+                        if overwrite:
+                            dest.update_tar(record=record, tar=tar)
+                            tar_count += 1
+
+        print(record_count, 'records added/updated')
+        if includetar:
+            print(tar_count, 'tars added/updated')
+
+    def destroy_records(self,
+                        record_style: Optional[str] = None,
+                        records: Optional[list] = None):
+        """
+        Permanently deletes multiple records and their associated tars all at
+        once.
+        
+        Parameters
+        ----------
+        record_style : str, optional
+            The record style to delete.  If given, all records of that style
+            will be deleted. If neither record_style nor records given, then
+            the available record styles will be listed and the user prompted
+            to pick one.
+        records : list, optional
+            A list of pre-selected records to delete. 
+        """
+        # Select record_style if needed
+        if record_style is None and records is None:
+            record_style = self.select_record_style()
+
+        # Get records by record_style
+        if record_style is not None:
+            if records is not None:
+                raise ValueError('record_style and records cannot both be given')
+
+            # Retrieve records with errors from self
+            records = self.get_records(style=record_style) 
+
+        elif records is None:
+            # Set empty list if record_style is still None and no records given
+            records = []
+
+        print(f'{len(records)} records found to be destroyed')
+
+        if len(records) > 0:
+            test = screen_input('Delete records? (must type yes):')
+            if test == 'yes':
+                count = 0
+                record_styles = set()
+                for record in tqdm(records, 'destroying records', ascii=True):
+                    try:
+                        self.delete_tar(record=record)
+                    except:
+                        pass
+                    try:
+                        self.delete_record(record=record)
+                        count += 1
+                        record_styles.add(record.style)
+                    except:
+                        pass
+                if self.style == 'local':
+                    for record_style in record_styles:
+                        cache = self.cache(record_style, refresh=True)
+                print(count, 'records successfully deleted')
+
+    def select_record_style(self) -> str:
+        """
+        Console prompt for selecting a record_style
+        """
+        # Build list of calculation records
+        styles = recordmanager.loaded_style_names
+
+        # Ask for selection
+        print('Select record_style:')
+        for i, style in enumerate(styles):
+            print(i+1, style)
+        choice = screen_input(':')
+        try:
+            choice = int(choice)
+        except:
+            record_style = choice
+        else:
+            record_style = styles[choice-1]
+        print()
+
+        return record_style
+
+    def record_querynames(self,
+                          style: str) -> list:
+        """Return the list of query parameter names for a given record style"""
+        return load_record(style).querynames
+
+    def record_querydoc(self,
+                        style: str) -> str:
+        """Return the description of query parameters for a given record style"""
+        return load_record(style).querydoc
```

### Comparing `yabadaba-0.2.1/yabadaba/database/LocalDatabase.py` & `yabadaba-0.2.2/yabadaba/database/CDCSDatabase.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,913 +1,778 @@
-# coding: utf-8
-# Standard Python libraries
-from pathlib import Path
-import ast
-import shutil
-import tarfile
-
-# http://www.numpy.org/
-import numpy as np
-
-# https://pandas.pydata.org/
-import pandas as pd
-
-# iprPy imports
-from ..tools import aslist, iaslist
-from . import Database
-from .. import load_record, recordmanager
-
-class LocalDatabase(Database):
-
-    def __init__(self, host, format='json', indent=None):
-        """
-        Initializes a connection to a local database of JSON/XML records
-        stored in a local directory.
-        
-        Parameters
-        ----------
-        host : str
-            The host name (local directory path) for the database.
-        format : str, optional
-            The format that the model records are saved as.  Can be either
-            JSON or XML.  Default value is JSON.
-        indent : int or None, optional
-            The indentation used when saving the records.  If None (default)
-            then the saved records are compact.  Otherwise, the lines in the
-            file will be indented by multiples of this value based on the
-            model's element recursion.
-        """
-        # Make the path if needed
-        host = Path(host)
-        if not host.is_dir():
-            host.mkdir(parents=True)
-
-        # Get absolute path to host
-        host = host.resolve()
-
-        # Pass host to Database initializer
-        Database.__init__(self, host)
-
-        # Set default format and indent values
-        self.__format = format
-        self.__indent = indent
-
-    @property
-    def style(self):
-        """str: The database style"""
-        return 'local'
-
-    @property
-    def format(self):
-        """str: The format that records are saved as: 'json' or 'xml'"""
-        return self.__format
-
-    @property
-    def indent(self):
-        """int or None: The record indentation setting to use when saving records."""
-        return self.__indent
-
-    def cache(self, style, refresh=False, addnew=True):
-        """
-        Loads/generates the metadata cache csv file for a given record style.
-
-        Parameters
-        ----------
-        style : str 
-            The record style to retrieve the metadata content for.
-        refresh : bool, optional
-            If True, then the metadata content will be rebuilt by loading every
-            record of the given style.  If False (default), the stored metadata
-            for records will be used rather than loading from the files.
-        addnew : bool, optional
-            If True (default), then the metadata for new records will be
-            appended to the stored metadata cache.  If False, then the stored
-            metadata is returned as is.
-        """
-        recordmanager.assert_style(style)
-        cachefile = Path(self.host, f'{style}.csv')
-
-        if cachefile.is_file() and refresh is False:
-
-            # Load cache file
-            cache = pd.read_csv(cachefile)
-
-            def interpret(series, key):
-                """Safely convert dict and list elements from str"""
-                try:
-                    assert series[key][0] in '{['
-                    return ast.literal_eval(series[key])
-                except:
-                    return series[key]
-
-            def toint(column):
-                """Convert int columns as needed"""
-                try:
-                    newcolumn = column.astype(int)
-                    assert np.allclose(column, newcolumn)
-                except:
-                    return column
-                else:
-                    return newcolumn
-
-            # Interpret int, dict and list elements
-            if len(cache) > 0:
-                cache = cache.apply(toint, axis=0)
-                for key in cache.keys():
-                    cache[key] = cache.apply(interpret, axis=1, args=[key])
-
-        else:
-            # Initialize new cache
-            cache = pd.DataFrame({'name':[]})
-
-        if addnew is True:
-
-            # Compare names in the cache to file names in the directory
-            cachenames = set(cache.name)
-            filenames = set([fname.stem for fname in Path(self.host, style).glob(f'*.{self.format}')])
-            newnames = filenames.difference(cachenames)
-            deletednames = cachenames.difference(filenames)
-
-            # Load new entries
-            if len(newnames) > 0:
-                newrecords = []
-                for name in newnames:
-                    fname = Path(self.host, style, f'{name}.{self.format}')
-                    record = load_record(style, model=fname, name=name)
-                    newrecords.append(record.metadata())
-                newrecords = pd.DataFrame(newrecords)
-                cache = cache.append(newrecords, sort=False).sort_values('name')
-                #cache = pd.concat([cache, newrecords], sort=False).sort_values('name')
-                refresh = True
-
-            # Delete missing entries
-            if len(deletednames) > 0:
-                cache = cache[~cache.name.isin(deletednames)]
-                refresh = True
-
-        # Refresh cache file
-        if refresh:
-            cache.to_csv(cachefile, index=False)
-
-        return cache
-
-    def get_records(self, style=None, return_df=False, refresh_cache=False, **kwargs):
-        """
-        Produces a list of all matching records in the database.
-        
-        Parameters
-        ----------
-        style : str, optional
-            The record style to search.
-        refresh_cache : bool, optional
-            Indicates if the metadata cache file is to be refreshed.  If False,
-            metadata for new records will be added but the old record metadata
-            fields will not be updated.  If True, then the metadata for all
-            records will be regenerated, which is needed to update the metadata
-            for modified records.
-        return_df : bool, optional
-            If True, then the corresponding pandas.Dataframe of metadata
-            will also be returned
-        **kwargs : any, optional
-            Any of the record-specific metadata keywords that can be searched
-            for.
-
-        Returns
-        ------
-        records : numpy.NDArray
-            All records from the database matching the given parameters.
-        records_df : pandas.DataFrame
-            The corresponding metadata values for the records.  Only returned
-            if return_df is True.
-        """
-        # Get df
-        df = self.get_records_df(style, refresh_cache=refresh_cache, **kwargs)
-
-        # Load only the matching records
-        records = []
-        if len(df) > 0:
-            for name in df.name:
-                fname = Path(self.host, style, f'{name}.{self.format}')
-                records.append(load_record(style, model=fname, database=self))
-
-        records = np.array(records)
-
-        if return_df:
-            return records, df
-        else:
-            return records
-
-    def get_records_df(self, style=None, refresh_cache=False, **kwargs):
-        """
-        Produces a table of metadata for matching records in the database.
-        
-        Parameters
-        ----------
-        style : str, optional
-            The record style to limit the search by.
-        refresh_cache : bool, optional
-            Indicates if the metadata cache file is to be refreshed.  If False,
-            metadata for new records will be added but the old record metadata
-            fields will not be updated.  If True, then the metadata for all
-            records will be regenerated, which is needed to update the metadata
-            for modified records.
-        **kwargs : any, optional
-            Any of the record-specific metadata keywords that can be searched
-            for.
-        
-        Returns
-        ------
-        records_df : pandas.DataFrame
-            The corresponding metadata values for the records.
-        """
-
-        # Set default search parameters
-        if style is None:
-            style = self.select_record_style()
-
-        if 'name' in kwargs and kwargs['name'] is not None:
-            # Load named records
-            cache = []
-            for name in aslist(kwargs['name']):
-                fname = Path(self.host, style, f'{name}.{self.format}')
-                if fname.exists():
-                    record = load_record(style, model=fname)
-                    cache.append(record.metadata())
-
-            # Build cache DataFrame
-            if len(cache) == 0:
-                cache = pd.DataFrame({'name':[]})
-            else:
-                cache = pd.DataFrame(cache)
-
-        else:
-            # Load cache file
-            cache = self.cache(style, refresh=refresh_cache)
-
-        # Filter based on the record's pandasfilter method
-        mask = load_record(style).pandasfilter(cache, **kwargs)
-        df = cache[mask].reset_index(drop=True)
-
-        return df
-
-    def get_record(self, style=None, refresh_cache=False, **kwargs):
-        """
-        Returns a single matching record from the database.
-        
-        Parameters
-        ----------
-        style : str, optional
-            The record style to limit the search by.
-        refresh_cache : bool, optional
-            Indicates if the metadata cache file is to be refreshed.  If False,
-            metadata for new records will be added but the old record metadata
-            fields will not be updated.  If True, then the metadata for all
-            records will be regenerated, which is needed to update the metadata
-            for modified records.
-        **kwargs : any, optional
-            Any of the record-specific metadata keywords that can be searched
-            for.
-        
-        Returns
-        -------
-        Record
-            The single record from the database matching the given parameters.
-        
-        Raises
-        ------
-        ValueError
-            If multiple or no matching records found.
-        """
-
-        if style is None:
-            styles = recordmanager.loaded_style_names
-        else:
-            styles = aslist(style)
-
-        # Get records
-        records = []
-        for style in styles:
-            records.append(self.get_records(style, refresh_cache=refresh_cache, **kwargs))
-        records = np.hstack(records)
-
-        # Verify that there is only one matching record
-        if len(records) == 1:
-            return records[0]
-        elif len(records) == 0:
-            raise ValueError('No matching records found')
-        else:
-            raise ValueError('Multiple matching records found')
-
-    def add_record(self, record=None, style=None, name=None, model=None,
-                   build=False, verbose=False):
-        """
-        Adds a new record to the database.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The new record to add to the database.  If not given, then name,
-            style and model are required.
-        style : str, optional
-            The record style for the new record.  Required if record is not
-            given.
-        name : str, optional
-            The name to assign to the new record.  Required if record is not
-            given.
-        model : str or DataModelDict, optional
-            The model contents of the new record.  Required if record is not
-            given.
-        build : bool, optional
-            If True, then the uploaded content will be (re)built based on the
-            record's attributes.  If False (default), then record's existing
-            content will be loaded if it exists, or built if it doesn't exist.
-        verbose : bool, optional
-            If True, info messages will be printed during operations.  Default
-            value is False.
-
-        Returns
-        ------
-        Record
-            Either the given record or a record composed of the name, style,
-            and model.
-        
-        Raises
-        ------
-        ValueError
-            If style, name and/or model given with record, or a matching record
-            already exists.
-        """
-
-        # Create Record object if not given
-        if record is None:
-            record = load_record(style, model=model, name=name)
-
-        # Issue a ValueError for competing kwargs
-        elif style is not None or name is not None or model is not None:
-            raise ValueError('kwargs style, name, and model cannot be given with kwarg record')
-
-        # Verify that there isn't already a record with a matching name
-        style_dir = Path(self.host, record.style)
-        fname = Path(style_dir, f'{record.name}.{self.format}')
-        if fname.is_file():
-            raise ValueError(f'Record {record.name} already exists')
-
-        # Make record style directory if needed
-        if not style_dir.is_dir():
-            style_dir.mkdir()
-
-        # Retrieve/build model contents
-        try:
-            assert build is False
-            model = record.model
-        except:
-            model = record.build_model()
-
-        # Save record
-        with open(fname, 'w', encoding='UTF-8') as f:
-            if self.format == 'json':
-                model.json(fp=f, indent=self.indent, ensure_ascii=False)
-            elif self.format == 'xml':
-                model.xml(fp=f, indent=self.indent)
-
-        if verbose:
-            print(f'{record} added to {self.host}')
-
-        return record
-
-    def update_record(self, record=None, style=None, name=None, model=None,
-                      build=False, verbose=False):
-        """
-        Replaces an existing record with a new record of matching name and
-        style, but new content.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record with new content to update in the database.  If not
-            given, content is required along with name and/or style to
-            uniquely define a record to update.
-        style : str, optional
-            The style of the record to update.
-        name : str, optional
-            The name to uniquely identify the record to update.
-        model : str or DataModelDict, optional
-            The model contents of the new record.  Required if record is not
-            given.
-        build : bool, optional
-            If True, then the uploaded content will be (re)built based on the
-            record's attributes.  If False (default), then record's existing
-            content will be loaded if it exists, or built if it doesn't exist.
-        verbose : bool, optional
-            If True, info messages will be printed during operations.  Default
-            value is False.
-
-        Returns
-        ------
-        Record
-            Either the given record or a record composed of the name, style,
-            and content.
-        
-        Raises
-        ------
-        TypeError
-            If no new content is given.
-        ValueError
-            If style and/or name content given with record.
-        """
-
-        # Create Record object if not given
-        if record is None:
-            if model is None:
-                raise TypeError('no new model given')
-
-            record = load_record(style, model=model, name=name)
-
-        # Issue a ValueError for competing kwargs
-        elif style is not None or name is not None:
-            raise ValueError('kwargs style and name cannot be given with kwarg record')
-
-        # Replace content in record object
-        elif model is not None:
-            record = load_record(record.style, model=model, name=record.name)
-
-        # Check if record already exists
-        style_dir = Path(self.host, record.style)
-        fname = Path(style_dir, f'{record.name}.{self.format}')
-        if not fname.is_file():
-            raise ValueError(f'No existing record {record.name} found')
-
-        # Retrieve/build model contents
-        try:
-            assert build is False
-            model = record.model
-        except:
-            model = record.build_model()
-
-        # Save record
-        with open(fname, 'w', encoding='UTF-8') as f:
-            if self.format == 'json':
-                model.json(fp=f, indent=self.indent, ensure_ascii=False)
-            elif self.format == 'xml':
-                model.xml(fp=f, indent=self.indent)
-
-        if verbose:
-            print(f'{record} updated in {self.host}')
-
-        return record
-
-    def delete_record(self, record=None, style=None, name=None, verbose=False):
-        """
-        Permanently deletes a record from the database.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record to delete from the database.  If not given, name and/or
-            style are needed to uniquely define the record to delete.
-        name : str, optional
-            The name of the record to delete.
-        style : str, optional
-            The style of the record to delete.
-        verbose : bool, optional
-            If True, info messages will be printed during operations.  Default
-            value is False.
-            
-        Raises
-        ------
-        ValueError
-            If style and/or name given with record.
-        """
-
-        # Create Record object if not given
-        if record is None:
-            record = self.get_record(name=name, style=style)
-
-        # Issue a ValueError for competing kwargs
-        elif style is not None or name is not None:
-            raise ValueError('kwargs style and name cannot be given with kwarg record')
-
-         # Delete record file
-        fname = Path(self.host, record.style, f'{record.name}.{self.format}')
-        if fname.is_file():
-            fname.unlink()
-        else:
-            raise ValueError(f'No existing {record.style} record {record.name} found')
-
-        if verbose:
-            print(f'{record} deleted from {self.host}')
-
-    def add_tar(self, record=None, style=None, name=None, tar=None,
-                root_dir=None):
-        """
-        Archives and stores a folder associated with a record.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record to associate the tar archive with.  If not given, then
-            name and/or style necessary to uniquely identify the record are
-            needed.
-        name : str, optional
-            The name to use in uniquely identifying the record.
-        style : str, optional
-            The style to use in uniquely identifying the record.
-        tar : bytes, optional
-            The bytes content of a tar file to save.  tar cannot be given
-            with root_dir.
-        root_dir : str, optional
-            Specifies the root directory for finding the directory to archive.
-            The directory to archive is at <root_dir>/<name>.  (Default is to
-            set root_dir to the current working directory.)  tar cannot be given
-            with root_dir.
-        
-        Raises
-        ------
-        ValueError
-            If style and/or name content given with record or the record already
-            has a folder or a tar archive.
-        """
-
-        # Create Record object if not given
-        if record is None:
-            record = self.get_record(name=name, style=style)
-
-        # Issue a ValueError for competing kwargs
-        elif style is not None or name is not None:
-            raise ValueError('kwargs style and name cannot be given with kwarg record')
-
-        # Verify that record exists
-        else:
-            record = self.get_record(name=record.name, style=record.style)
-
-        # Build path to record
-        dir_path = Path(self.host, record.style, record.name)
-        tar_path = Path(self.host, record.style, f'{record.name}.tar.gz')
-
-        # Check if an archive or folder already exists
-        if tar_path.exists():
-            raise ValueError('Record already has an archive')
-        elif dir_path.exists():
-            raise ValueError('Record already has a folder')
-
-        # Make archive
-        if tar is None:
-            if root_dir is None:
-                root_dir = '.'
-            target = Path(root_dir, record.name)
-
-            tar = tarfile.open(tar_path, 'w:gz')
-            tar.add(target, target.name)
-            tar.close()
-
-        elif root_dir is None:
-            with open(tar_path, 'wb') as f:
-                f.write(tar)
-        else:
-            raise ValueError('tar and root_dir cannot both be given')
-
-    def get_tar(self, record=None, style=None, name=None, raw=False):
-        """
-        Retrives the tar archive associated with a record in the database.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record to retrieve the associated tar archive for.
-        name : str, optional
-            The name to use in uniquely identifying the record.
-        style : str, optional
-            The style to use in uniquely identifying the record.
-        raw : bool, optional
-            If True, return the archive as raw binary content. If 
-            False, return as an open tarfile. (Default is False)
-        
-        Returns
-        -------
-        tarfile or str
-            The tar archive as an open tarfile if raw=False, or as a binary str if
-            raw=True.
-        
-        Raises
-        ------
-        ValueError
-            If style and/or name content given with record.
-        """
-
-        # Create Record object if not given
-        if record is None:
-            record = self.get_record(name=name, style=style)
-
-        # Issue a ValueError for competing kwargs
-        elif style is not None or name is not None:
-            raise ValueError('kwargs style and name cannot be given with kwarg record')
-
-        # Verify that record exists
-        #else:
-        #    record = self.get_record(name=record.name, style=record.style)
-
-        # Build path to record
-        tar_path = Path(self.host, record.style, record.name+'.tar.gz')
-
-        tar = tarfile.open(tar_path)
-        record.tar = tar
-
-        # Return content
-        if raw is True:
-            with open(tar_path, 'rb') as f:
-                return f.read()
-        else:
-            return tar
-
-    def delete_tar(self, record=None, style=None, name=None):
-        """
-        Deletes a tar file from the database.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record associated with the tar archive to delete.  If not
-            given, then name and/or style necessary to uniquely identify
-            the record are needed.
-        name : str, optional
-            The name to use in uniquely identifying the record.
-        style : str, optional
-            The style to use in uniquely identifying the record.
-        
-        Raises
-        ------
-        ValueError
-            If style and/or name content given with record.
-        """
-
-        # Create Record object if not given
-        if record is None:
-            record = self.get_record(name=name, style=style)
-
-        # Issue a ValueError for competing kwargs
-        elif style is not None or name is not None:
-            raise ValueError('kwargs style and name cannot be given with kwarg record')
-
-        # Verify that record exists
-        #else:
-        #    record = self.get_record(name=record.name, style=record.style)
-
-        # Build path to tar file
-        tar_path = Path(self.host, record.style, record.name+'.tar.gz')
-
-        # Delete record if it exists
-        if tar_path.is_file():
-            tar_path.unlink()
-
-    def update_tar(self, record=None, style=None, name=None, tar=None,
-                   root_dir=None):
-        """
-        Replaces an existing tar archive for a record with a new one.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record to associate the tar archive with.  If not given, then 
-            name and/or style necessary to uniquely identify the record are 
-            needed.
-        name : str, optional
-            The name to use in uniquely identifying the record.
-        style : str, optional
-            The style to use in uniquely identifying the record.
-        tar : bytes, optional
-            The bytes content of a tar file to save.  tar cannot be given
-            with root_dir.
-        root_dir : str, optional
-            Specifies the root directory for finding the directory to archive.
-            The directory to archive is at <root_dir>/<name>.  (Default is to
-            set root_dir to the current working directory.)  tar cannot be given
-            with root_dir.
-        """
-
-        # Delete the existing tar archive stored in the database
-        self.delete_tar(record=record, name=name)
-
-        # Add the new tar archive
-        self.add_tar(record=record, name=name, style=style, tar=tar,
-                     root_dir=root_dir)
-
-    def add_folder(self, record=None, name=None, style=None, filenames=None,
-                   root_dir=None):
-        """
-        Stores a folder associated with a record.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record to associate the folder with.  If not given, then
-            name and/or style necessary to uniquely identify the record are
-            needed.
-        name : str, optional
-            The name to use in uniquely identifying the record.
-        style : str, optional
-            The style to use in uniquely identifying the record.
-        filenames : str or list, optional
-            The paths to files that are to be added to the record's folder.
-            Cannot be given with root_dir.
-        root_dir : str, optional
-            Specifies the root directory for finding the folder to add.
-            The directory to add is at <root_dir>/<name>.  (Default is to
-            set root_dir to the current working directory.)  Cannot be given
-            with filenames.
-        
-        Raises
-        ------
-        ValueError
-            If style and/or name content given with record or the record already
-            has a folder or a tar archive.
-        """
-
-        # Create Record object if not given
-        if record is None:
-            record = self.get_record(name=name, style=style)
-
-        # Issue a ValueError for competing kwargs
-        elif style is not None or name is not None:
-            raise ValueError('kwargs style and name cannot be given with kwarg record')
-
-        # Verify that record exists
-        else:
-            record = self.get_record(name=record.name, style=record.style)
-
-        # Build database paths
-        dir_path = Path(self.host, record.style, record.name)
-        tar_path = Path(self.host, record.style, f'{record.name}.tar.gz')
-
-        # Check if an archive or folder already exists
-        if tar_path.exists():
-            raise ValueError('Record already has an archive')
-        elif dir_path.exists():
-            raise ValueError('Record already has a folder')
-
-        # Copy folder
-        if filenames is None:
-            if root_dir is None:
-                root_dir = '.'
-            source = Path(root_dir, record.name)
-            shutil.copytree(source, dir_path)
-
-        # Copy files
-        elif root_dir is None:
-            dir_path.mkdir(parents=True)
-            for filename in iaslist(filenames):
-                shutil.copy2(filename, Path(dir_path, Path(filename).name))
-
-        else:
-            raise ValueError('filenames and root_dir cannot both be given')
-
-    def get_folder(self, record=None, style=None, name=None):
-        """
-        Retrives the location of the folder associated with a record in the
-        database. 
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record to retrieve the associated folder location for.
-        name : str, optional
-            The name to use in uniquely identifying the record.
-        style : str, optional
-            The style to use in uniquely identifying the record.
-        
-        Returns
-        -------
-        pathlib.Path
-            The path to the record's folder
-        
-        Raises
-        ------
-        ValueError
-            If style and/or name content given with record.
-        NotADirectoryError
-            If the record's folder doesn't exist.
-        """
-
-        # Create Record object if not given
-        if record is None:
-            record = self.get_record(name=name, style=style)
-
-        # Issue a ValueError for competing kwargs
-        elif style is not None or name is not None:
-            raise ValueError('kwargs style and name cannot be given with kwarg record')
-
-        # Verify that record exists
-        else:
-            record = self.get_record(name=record.name, style=record.style)
-
-        # Build path to folder
-        dir_path = Path(self.host, record.style, record.name)
-
-        # Return path
-        if dir_path.exists():
-            return dir_path
-        else:
-            raise NotADirectoryError('No folder saved for the record')
-
-    def delete_folder(self, record=None, name=None, style=None):
-        """
-        Deletes a folder from the database.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record associated with the folder to delete.  If not
-            given, then name and/or style necessary to uniquely identify
-            the record are needed.
-        name : str, optional
-            The name to use in uniquely identifying the record.
-        style : str, optional
-            The style to use in uniquely identifying the record.
-        
-        Raises
-        ------
-        ValueError
-            If style and/or name content given with record.
-        """
-
-        # Create Record object if not given
-        if record is None:
-            record = self.get_record(name=name, style=style)
-
-        # Issue a ValueError for competing kwargs
-        elif style is not None or name is not None:
-            raise ValueError('kwargs style and name cannot be given with kwarg record')
-
-        # Verify that record exists
-        else:
-            record = self.get_record(name=record.name, style=record.style)
-
-        # Build path to tar file
-        dir_path = Path(self.host, record.style, record.name)
-
-        # Delete record if it exists
-        if dir_path.exists():
-            shutil.rmtree(dir_path)
-
-    def update_folder(self, record=None, style=None, name=None, filenames=None,
-                      root_dir=None, clear=True):
-        """
-        Updates an existing folder for a record.
-        
-        Parameters
-        ----------
-        record : Record, optional
-            The record to associate the folder with.  If not given, then 
-            name and/or style necessary to uniquely identify the record are 
-            needed.
-        name : str, optional
-            The name to use in uniquely identifying the record.
-        style : str, optional
-            The style to use in uniquely identifying the record.
-        filenames : str or list, optional
-            The paths to files that are to be added to the record's folder.
-            Cannot be given with root_dir.
-        root_dir : str, optional
-            Specifies the root directory for finding the folder to add.
-            The directory to add is at <root_dir>/<name>.  (Default is to
-            set root_dir to the current working directory.)  Cannot be given
-            with filenames.
-        clear : bool, optional
-            If True (default), then the current folder contents will be deleted
-            before the new contents are added.  If False, existing files may
-            remain if the new content does not overwrite it.
-        """
-        # Check competing parameters
-        if filenames is not None and root_dir is not None:
-            raise ValueError('filenames and root_dir cannot both be given')
-
-        # Create Record object if not given
-        if record is None:
-            record = self.get_record(name=name, style=style)
-
-        # Issue a ValueError for competing kwargs
-        elif style is not None or name is not None:
-            raise ValueError('kwargs style and name cannot be given with kwarg record')
-
-        # Verify that record exists
-        else:
-            record = self.get_record(name=record.name, style=record.style)
-
-        # Build database paths
-        dir_path = Path(self.host, record.style, record.name)
-
-        # Delete existing folder
-        if clear is True:
-            if dir_path.exists():
-                shutil.rmtree(dir_path)
-
-        # Copy folder
-        if filenames is None:
-            if root_dir is None:
-                root_dir = '.'
-            source = Path(root_dir, record.name)
-            shutil.copytree(source, dir_path)
-
-        # Copy files
-        elif root_dir is None:
-            dir_path.mkdir(parents=True)
-            for filename in iaslist(filenames):
-                shutil.copy2(filename, Path(dir_path, Path(filename).name))
+# coding: utf-8
+# Standard Python libraries
+from pathlib import Path
+import shutil
+import tarfile
+from io import BytesIO
+from typing import Optional, Tuple, Union
+
+# https://github.com/usnistgov/pycdcs
+from cdcs import CDCS
+
+# http://www.numpy.org/
+import numpy as np
+
+# https://pandas.pydata.org/
+import pandas as pd
+
+# https://github.com/usnistgov/DataModelDict
+from DataModelDict import DataModelDict as DM
+
+# Relative imports
+from ..tools import aslist, iaslist
+from . import Database
+from ..record import recordmanager, load_record, Record
+
+class CDCSDatabase(Database):
+
+    def __init__(self,
+                 host: str,
+                 username: Optional[str] = None,
+                 password: Optional[str] = None,
+                 auth: Optional[Tuple[str]] = None,
+                 cert: Union[str, Tuple[str], None] = None, 
+                 certification: Union[str, Tuple[str], None] = None,
+                 verify: Optional[bool] = True,
+                 cdcsversion: Optional[str] = None):
+        """
+        Initializes a database of style curator.
+        
+        Parameters
+        ----------
+        host : str
+            The host name (url) for the database.
+        username : str, optional
+            Username of desired account on the server. A prompt will ask for
+            the username if not given.
+        password : str, optional
+            Password of desired account on the server.  This can either be the
+            password as a str, or a str path to a file containing only the
+            password.  A prompt will ask for the password if not given.
+        auth : tuple, optional
+            Auth tuple to enable Basic/Digest/Custom HTTP Auth.  Alternative to
+            giving username and password separately.
+        cert : str, optional
+            if String, path to ssl client cert file (.pem). If Tuple,
+            ('cert', 'key') pair.
+        certification : str, optional
+            Alias for cert. Retained for compatibility.
+        verify : bool or str, optional
+            Either a boolean, in which case it controls whether we verify the
+            server's TLS certificate, or a string, in which case it must be a
+            path to a CA bundle to use. Defaults to True.
+        cdcsversion : str, optional
+            For CDCS versions 2.X.X, this allows for specifying the full CDCS
+            version to ensure the class methods perform the correct REST
+            calls.  This can be specified as "#.#.#", or if None is given will
+            default to "2.15.0".  For CDCS versions 3.X.X, this is ignored as
+            version info is obtained directly from the database.
+        """
+        # Fetch password from file if needed
+        try:
+            with open(password, encoding='UTF-8') as f:
+                password = f.read().strip()
+        except Exception:
+            pass
+
+        # Pass parameters to cdcs object
+        self.__cdcs = CDCS(host, username=username, password=password, auth=auth,
+                           cert=cert, certification=certification, verify=verify,
+                           cdcsversion=cdcsversion)
+
+        # Pass host to Database initializer
+        Database.__init__(self, host)
+
+    @property
+    def style(self) -> str:
+        """str: The database style"""
+        return 'cdcs'
+
+    @property
+    def cdcs(self) -> CDCS:
+        """cdcs.CDCS : The underlying database API object."""
+        return self.__cdcs
+
+    def get_records(self,
+                    style: Optional[str] = None,
+                    return_df: bool = False,
+                    name: Union[str, list, None] = None,
+                    query: Optional[dict] = None,
+                    keyword: Optional[str] = None,
+                    **kwargs) -> Union[list, Tuple[list, pd.DataFrame]]:
+        """
+        Produces a list of all matching records in the database.
+        
+        Parameters
+        ----------
+        style : str, optional
+            The record style to search. If not given, a prompt will ask for it.
+        name : str or list, optional
+            Record name(s) to delimit by. 
+        return_df : bool, optional
+            If True, then the corresponding pandas.Dataframe of metadata
+            will also be returned
+        query : dict, optional
+            A custom-built CDCS-style query to use for the record search.
+            Alternative to passing in the record-specific metadata kwargs.
+            Note that name can be given with query.
+        keyword : str, optional
+            Allows for a search of records whose contents contain a keyword.
+            Alternative to giving query or kwargs.
+        **kwargs : any, optional
+            Any of the record-specific metadata keywords that can be searched
+            for.
+        
+        Returns
+        ------
+        records : numpy.NDArray
+            All records from the database matching the given parameters.
+        records_df : pandas.DataFrame
+            The corresponding metadata values for the records.  Only returned
+            if return_df is True.
+        """
+        # Set default search parameters
+        if style is None:
+            style = self.select_record_style()
+
+        # Setup keyword search
+        if keyword is not None:
+            assert len(kwargs) == 0, 'keyword cannot be given with kwargs'
+            assert query is None, 'keyword cannot be given with query'
+
+        # Setup query
+        elif query is not None:
+            assert len(kwargs) == 0, 'query cannot be given with kwargs'
+        else:
+            query = load_record(style).cdcsquery(**kwargs)
+
+        def build_records(series):
+            return load_record(series.template_title, model=series.xml_content,
+                               name=series.title, database=self)
+
+        # Build records by querying for each record name (or None)
+        records = []
+        for n in iaslist(name):
+            data = self.cdcs.query(title=n, template=style, mongoquery=query, keyword=keyword)
+            if len(data) > 0:
+                records.extend(data.apply(build_records, axis=1))
+        records = np.array(records)
+
+        # Build df
+        if len(records) > 0:
+            df = []
+            for record in records:
+                df.append(record.metadata())
+            df = pd.DataFrame(df)
+        else:
+            df = pd.DataFrame({'name':[]})
+
+        # Sort by name
+        df = df.sort_values('name')
+        records = records[df.index.tolist()]
+
+        # Return records (and df)
+        if return_df:
+            return records, df.reset_index(drop=True)
+        else:
+            return records
+
+    def get_records_df(self,
+                       style: Optional[str] = None,
+                       name: Union[str, list, None] = None,
+                       query: Optional[dict] = None,
+                       keyword: Optional[str] = None,
+                       **kwargs) -> pd.DataFrame:
+        """
+        Produces a list of all matching records in the database.
+        
+        Parameters
+        ----------
+        style : str, optional
+            The record style to search. If not given, a prompt will ask for it.
+        name : str or list, optional
+            Record name(s) to delimit by. 
+        query : dict, optional
+            A custom-built CDCS-style query to use for the record search.
+            Alternative to passing in the record-specific metadata kwargs.
+            Note that name can be given with query.
+        keyword : str, optional
+            Allows for a search of records whose contents contain a keyword.
+            Alternative to giving query or kwargs.
+        **kwargs : any, optional
+            Any of the record-specific metadata keywords that can be searched
+            for.
+            
+        Returns
+        -------
+        records_df : pandas.DataFrame
+            The corresponding metadata values for the records.
+        """
+        return self.get_records(style, name=name, query=query, keyword=keyword, return_df=True, **kwargs)[1]
+
+    def get_record(self, 
+                   style: Optional[str] = None,
+                   name: Union[str, list, None] = None,
+                   query: Optional[dict] = None,
+                   keyword: Optional[str] = None,
+                   **kwargs) -> Record:
+        """
+        Returns a single matching record from the database.
+        
+        Parameters
+        ----------
+        style : str, optional
+            Record style(s) to limit the search by.
+        name : str or list, optional
+            Record name(s) to delimit by. 
+        query : dict, optional
+            A custom-built CDCS-style query to use for the record search.
+            Alternative to passing in the record-specific metadata kwargs.
+            Note that name can be given with query.
+        keyword : str, optional
+            Allows for a search of records whose contents contain a keyword.
+            Alternative to giving query or kwargs.
+        **kwargs : any, optional
+            Any of the record-specific metadata keywords that can be searched
+            for.
+            
+        Returns
+        ------
+        Record
+            The single record from the database matching the given parameters.
+        
+        Raises
+        ------
+        ValueError
+            If multiple or no matching records found.
+        """
+        if style is None:
+            styles = recordmanager.loaded_style_names
+        else:
+            styles = aslist(style)
+
+        # Get records
+        records = []
+        for style in styles:
+            records.append(self.get_records(style, name=name, query=query, keyword=keyword, **kwargs))
+        records = np.hstack(records)
+
+        # Verify that there is only one matching record
+        if len(records) == 1:
+            return records[0]
+        elif len(records) == 0:
+            raise ValueError('No matching records found')
+        else:
+            raise ValueError('Multiple matching records found')
+    
+    def count_records(self,
+                      style: Optional[str] = None,
+                      name: Union[str, list, None] = None,
+                      query: Optional[dict] = None,
+                      keyword: Optional[str] = None,
+                      **kwargs) -> int:
+        """
+        Retrieves a count of matching records from the database.  Much faster
+        than get_records if you only want to know the number of matches.
+        
+        Parameters
+        ----------
+        style : str, optional
+            The record style to search. If not given, a prompt will ask for it.
+        name : str or list, optional
+            Record name(s) to delimit by. 
+        query : dict, optional
+            A custom-built CDCS-style query to use for the record search.
+            Alternative to passing in the record-specific metadata kwargs.
+            Note that name can be given with query.
+        keyword : str, optional
+            Allows for a search of records whose contents contain a keyword.
+            Alternative to giving query or kwargs.
+        **kwargs : any, optional
+            Any of the record-specific metadata keywords that can be searched
+            for.
+        
+        Returns
+        ------
+        int
+            The count of records in the database matching the given parameters.
+        """
+        # Set default search parameters
+        if style is None:
+            style = self.select_record_style()
+
+        # Setup keyword search
+        if keyword is not None:
+            assert len(kwargs) == 0, 'keyword cannot be given with kwargs'
+            assert query is None, 'keyword cannot be given with query'
+
+        # Setup query
+        elif query is not None:
+            assert len(kwargs) == 0, 'query cannot be given with kwargs'
+        else:
+            query = load_record(style).cdcsquery(**kwargs)
+
+        count = 0
+        for n in iaslist(name):
+            count += self.cdcs.query_count(title=n, template=style, mongoquery=query, keyword=keyword)
+
+        return count
+
+    def add_record(self,
+                   record: Optional[Record] = None,
+                   style: Optional[str] = None,
+                   name: Optional[str] = None,
+                   model: Union[str, DM, None] = None,
+                   build: bool = False,
+                   verbose: bool = False,
+                   workspace: Union[str, pd.Series, None] = None,
+                   auto_set_pid_off: bool = False) -> Record:
+        """
+        Adds a new record to the database.
+        
+        Parameters
+        ----------
+        record : iprPy.Record, optional
+            The new record to add to the database.  If not given, then name,
+            style and content are required.
+        style : str, optional
+            The record style for the new record.  Required if record is not
+            given.
+        name : str, optional
+            The name to assign to the new record.  Required if record is not
+            given.
+        model : str or DataModelDict, optional
+            The model contents of the new record.  Required if record is not
+            given.
+        build : bool, optional
+            If True, then the uploaded content will be (re)built based on the
+            record's attributes.  If False (default), then record's existing
+            content will be loaded if it exists, or built if it doesn't exist.
+        verbose : bool, optional
+            If True, info messages will be printed during operations.  Default
+            value is False.
+        workspace : str or pandas.Series, optional
+            The name of a workspace to assign the record to.  If not given
+            then the record is not assigned to a workspace and will only be
+            accessible to the user who uploaded it.
+        auto_set_pid_off : bool
+            If True, the database's auto_set_pid setting will temporarily be
+            turned off for the record upload.  This is only needed if the
+            record contains a PID URL corresponding to a set PID xpath.  If
+            uploading multiple records, it is better to use the CDCS object's
+            auto_set_pid_off() context manager or to manually change the
+            setting off/on with CDCS.auto_set_pid.
+
+        Returns
+        ------
+        Record
+            Either the given record or a record composed of the name, style, 
+            and model.
+        
+        Raises
+        ------
+        ValueError
+            If style, name and/or model given with record, or a matching record
+            already exists.
+        """
+
+        # Create Record object if not given
+        if record is None:
+            record = load_record(style, model=model, name=name)
+
+        # Issue a ValueError for competing kwargs
+        elif style is not None or name is not None or model is not None:
+            raise ValueError('kwargs style, name, and model cannot be given with kwarg record')
+
+        # Retrieve/build model contents
+        try:
+            assert build is False
+            content = record.model.xml()
+        except Exception:
+            content = record.build_model().xml()
+
+        # Upload to database
+        self.cdcs.upload_record(template=record.style, content=content,
+                                title=record.name,
+                                auto_set_pid_off=auto_set_pid_off)
+        if verbose:
+            print(f'{record} added to {self.host}')
+
+        if workspace is not None:
+            self.assign_records(record, workspace, verbose=verbose)
+
+        return record
+
+    def update_record(self,
+                      record: Optional[Record] = None,
+                      style: Optional[str] = None,
+                      name: Optional[str] = None,
+                      model: Union[str, DM, None] = None,
+                      build: bool = False,
+                      verbose: bool = False,
+                      workspace: Union[str, pd.Series, None] = None,
+                      auto_set_pid_off: bool = False) -> Record:
+        """
+        Replaces an existing record with a new record of matching name and 
+        style, but new content.
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The record with new content to update in the database.  If not
+            given, content is required along with name and/or style to
+            uniquely define a record to update.
+        style : str, optional
+            The style of the record to update.
+        name : str, optional
+            The name to uniquely identify the record to update.
+        model : str or DataModelDict, optional
+            The model contents of the new record.  Required if record is not
+            given.
+        build : bool, optional
+            If True, then the uploaded content will be (re)built based on the
+            record's attributes.  If False (default), then record's existing
+            content will be loaded if it exists, or built if it doesn't exist.
+        verbose : bool, optional
+            If True, info messages will be printed during operations.  Default
+            value is False.
+        workspace : str or pandas.Series, optional
+            The name of a workspace to assign the record to.  If not given
+            then the record is not assigned to a workspace and will only be
+            accessible to the user who uploaded it.
+        auto_set_pid_off : bool
+            If True, the database's auto_set_pid setting will temporarily be
+            turned off for the record upload.  This is only needed if the
+            record contains a PID URL corresponding to a set PID xpath.  If
+            uploading multiple records, it is better to use the CDCS object's
+            auto_set_pid_off() context manager or to manually change the
+            setting off/on with CDCS.auto_set_pid.
+        Returns
+        ------
+        Record
+            Either the given record or a record composed of the name, style, 
+            and model.
+            
+        Raises
+        ------
+        TypeError
+            If no new content is given.
+        ValueError
+            If style, model, and/or name given with record.
+        """
+
+        # Create Record object if not given
+        if record is None:
+            if model is None:
+                raise TypeError('no new model given')
+            oldrecord = self.get_record(name=name, style=style)
+            record = load_record(oldrecord.style, model=model, name=oldrecord.name)
+
+        # Use given record object
+        else:
+            if style is not None or name is not None:
+                raise ValueError('kwargs style and name cannot be given with kwarg record')
+
+            # Replace model in record object
+            if model is not None:
+                record = load_record(record.style, model=model, name=record.name)
+
+        # Retrieve/build model contents
+        try:
+            assert build is False
+            content = record.model.xml()
+        except Exception:
+            content = record.build_model().xml()
+
+        # Upload to database
+        self.cdcs.update_record(template=record.style, content=content,
+                                title=record.name,
+                                auto_set_pid_off=auto_set_pid_off)
+
+        if verbose:
+            print(f'{record} updated in {self.host}')
+
+        if workspace is not None:
+            self.assign_records(record, workspace, verbose=verbose)
+
+        return record
+
+    def delete_record(self,
+                      record: Optional[Record] = None,
+                      style: Optional[str] = None,
+                      name: Optional[str] = None,
+                      verbose: bool = False):
+        """
+        Permanently deletes a record from the database.  Will issue an error 
+        if exactly one matching record is not found in the database.
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The record to delete from the database.  If not given, name and/or
+            style are needed to uniquely define the record to delete.
+        name : str, optional
+            The name of the record to delete.
+        style : str, optional
+            The style of the record to delete.
+        verbose : bool, optional
+            If True, info messages will be printed during operations.  Default
+            value is False.
+            
+        Raises
+        ------
+        ValueError
+            If style and/or name content given with record.
+        """
+        # Extract values from Record object if given
+        if record is not None:
+            if style is not None or name is not None:
+                raise ValueError('kwargs style and name cannot be given with kwarg record')
+            name = record.name
+            style = record.style
+
+        # Delete record
+        self.cdcs.delete_record(template=style, title=name)
+
+        if verbose:
+            print(f'{record} deleted from {self.host}')
+
+    def assign_records(self,
+                       records: Union[Record, list],
+                       workspace: Union[str, pd.Series],
+                       verbose: bool = False):
+        """
+        Assigns one or more records to a CDCS workspace.
+
+        Parameters
+        ----------
+        records : Record or list
+            The record(s) to assign to the workspace.
+        workspace : str or pandas.Series
+            The workspace to assign the records to.
+        verbose : bool, optional
+            Setting this to True will print extra status messages.  Default
+            value is False.
+        """
+        #ids = []
+        for record in aslist(records):
+            self.cdcs.assign_records(workspace, template=record.style,
+                                     title=record.name)
+            if verbose:
+                print(f'{record} assigned to workspace {workspace}')
+
+    def add_tar(self, 
+                record: Optional[Record] = None,
+                style: Optional[str] = None,
+                name: Optional[str] = None,
+                tar: Optional[bytes] = None,
+                root_dir: Optional[Path] = None):
+        """
+        Archives and stores a folder associated with a record.
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The record to associate the tar archive with.  If not given, then
+            name and/or style necessary to uniquely identify the record are
+            needed.
+        name : str, optional
+            The name to use in uniquely identifying the record.
+        style : str, optional
+            The style to use in uniquely identifying the record.
+        tar : bytes, optional
+            The bytes content of a tar file to save.  tar cannot be given
+            with root_dir.
+        root_dir : str, optional
+            Specifies the root directory for finding the directory to archive.
+            The directory to archive is at <root_dir>/<name>.  (Default is to
+            set root_dir to the current working directory.)  tar cannot be given
+            with root_dir.
+        
+        Raises
+        ------
+        ValueError
+            If style and/or name content given with record or the record already
+            has an archive.
+        """
+
+        # Get Record object if not given
+        if record is None:
+            record = self.get_record(name=name, style=style)
+
+        else:
+            # Issue a ValueError for competing kwargs
+            if style is not None or name is not None:
+                raise ValueError('kwargs style and name cannot be given with kwarg record')
+
+            # Verify that record exists
+            record = self.get_record(name=record.name, style=record.style)
+
+        # Check if an archive already exists
+        blobs = self.cdcs.get_blobs(filename=record.name)
+        if len(blobs) > 0:
+            raise ValueError('Record already has an archive')
+
+        # Create directory archive and upload
+        if tar is None: 
+            if root_dir is None:
+                root_dir = Path.cwd()
+
+            # Make archive
+            basename = Path(root_dir, record.name)
+            filename = Path(root_dir, record.name + '.tar.gz')
+            shutil.make_archive(basename, 'gztar', root_dir=root_dir,
+                                base_dir=record.name)
+
+            # Upload archive
+            tries = 0
+            while tries < 2:
+                tries += 1
+                try:
+                    url = self.cdcs.upload_blob(filename.as_posix())
+                    break
+                except Exception as err:
+                    if tries == 2:
+                        raise ValueError('Failed to upload archive 2 times') from err
+
+            # Remove local archive copy
+            filename.unlink()
+
+        # Upload pre-existing tar object
+        elif root_dir is None:
+            filename = Path(record.name + '.tar.gz')
+
+            # Upload archive
+            tries = 0
+            while tries < 2:
+                tries += 1
+                try:
+                    url = self.cdcs.upload_blob(filename=filename, blobbytes=BytesIO(tar))
+                    break
+                except Exception as err:
+                    if tries == 2:
+                        raise ValueError('Failed to upload archive 2 times') from err
+
+        else:
+            raise ValueError('tar and root_dir cannot both be given')
+
+    def get_tar(self,
+                record: Optional[Record] = None,
+                style: Optional[str] = None,
+                name: Optional[str] = None,
+                raw: bool = False) -> Union[tarfile.TarFile, bytes]:
+        """
+        Retrieves the tar archive associated with a record in the database.
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The record to retrieve the associated tar archive for.
+        name : str, optional
+            The name to use in uniquely identifying the record.
+        style : str, optional
+            The style to use in uniquely identifying the record.
+        raw : bool, optional
+            If True, return the archive as raw binary content. If 
+            False, return as an open tarfile. (Default is False)
+            
+        Returns
+        -------
+        tarfile or str
+            The tar archive as an open tarfile if raw=False, or as a binary str if
+            raw=True.
+            
+        Raises
+        ------
+        ValueError
+            If style and/or name content given with record.
+        """
+
+        # Create Record object if not given
+        if record is None:
+            record = self.get_record(name=name, style=style)
+
+        # Issue a TypeError for competing kwargs
+        elif style is not None or name is not None:
+            raise TypeError('kwargs style and name cannot be given with kwarg record')
+
+        filename = Path(record.name + '.tar.gz')
+
+        # Download tar file
+        tardata = self.cdcs.get_blob_contents(filename=filename)
+
+        # Return contents
+        if raw is True:
+            return tardata
+        else:
+            tar = tarfile.open(fileobj = BytesIO(tardata))
+            record.tar = tar
+            return tar
+
+    def delete_tar(self, 
+                   record: Optional[Record] = None,
+                   style: Optional[str] = None,
+                   name: Optional[str] = None):
+        """
+        Deletes a tar file from the database.
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The record associated with the tar archive to delete.  If not
+            given, then name and/or style necessary to uniquely identify
+            the record are needed.
+        name : str, optional
+            The name to use in uniquely identifying the record.
+        style : str, optional
+            The style to use in uniquely identifying the record.
+        """
+
+        # Create Record object if not given
+        if record is None:
+            record = self.get_record(name=name, style=style)
+
+        # Issue a TypeError for competing kwargs
+        elif style is not None or name is not None:
+            raise TypeError('kwargs style and name cannot be given with kwarg record')
+
+        filename = Path(record.name + '.tar.gz')
+
+        self.cdcs.delete_blob(filename=filename)
+
+    def update_tar(self,
+                   record: Optional[Record] = None,
+                   style: Optional[str] = None,
+                   name: Optional[str] = None,
+                   tar: Optional[bytes] = None,
+                   root_dir: Optional[Path] = None):
+        """
+        Archives and stores a folder associated with a record.
+        
+        Parameters
+        ----------
+        record : Record, optional
+            The record to associate the tar archive with.  If not given, then
+            name and/or style necessary to uniquely identify the record are
+            needed.
+        name : str, optional
+            The name to use in uniquely identifying the record.
+        style : str, optional
+            The style to use in uniquely identifying the record.
+        tar : bytes, optional
+            The bytes content of a tar file to save.  tar cannot be given
+            with root_dir.
+        root_dir : str, optional
+            Specifies the root directory for finding the directory to archive.
+            The directory to archive is at <root_dir>/<name>.  (Default is to
+            set root_dir to the current working directory.)  tar cannot be given
+            with root_dir.
+        
+        Raises
+        ------
+        ValueError
+            If style and/or name content given with record or the record already
+            has an archive.
+        """
+
+        self.delete_tar(record=record, name=name, style=style)
+        self.add_tar(record=record, name=name, style=style, tar=tar, root_dir=root_dir)
```

### Comparing `yabadaba-0.2.1/yabadaba/database/__init__.py` & `yabadaba-0.2.2/yabadaba/database/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# coding: utf-8
-__all__ = ['Database', 'databasemanager', 'load_database']
-
-# Import base Database class
-from .Database import Database
-
-# Initialize a ModuleManager for the database styles
-from ..tools import ModuleManager
-databasemanager = ModuleManager('Database')
-
-# Import load_database
-from .load_database import load_database
-
-# Add the modular Database styles
-databasemanager.import_style('local', '.LocalDatabase', __name__)
-databasemanager.import_style('mongo', '.MongoDatabase', __name__)
+# coding: utf-8
+__all__ = ['Database', 'databasemanager', 'load_database']
+
+# Import base Database class
+from .Database import Database
+
+# Initialize a ModuleManager for the database styles
+from ..tools import ModuleManager
+databasemanager = ModuleManager('Database')
+
+# Import load_database
+from .load_database import load_database
+
+# Add the modular Database styles
+databasemanager.import_style('local', '.LocalDatabase', __name__)
+databasemanager.import_style('mongo', '.MongoDatabase', __name__)
 databasemanager.import_style('cdcs', '.CDCSDatabase', __name__)
```

### Comparing `yabadaba-0.2.1/yabadaba/database/load_database.py` & `yabadaba-0.2.2/yabadaba/database/load_database.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,92 @@
-# coding: utf-8
-
-# Relative imports
-from ..tools import screen_input
-from . import databasemanager as default_databasemanager
-from .. import settings as default_settings
-
-__all__ = ['load_database']
-
-def load_database(name=None, style=None, host=None, settings=None, 
-                  databasemanager=None, **kwargs):
-    """
-    Loads a database object.  Can be either loaded from stored settings or
-    by defining all needed access information.
-    
-    Parameters
-    ----------
-    name : str, optional
-        The name assigned to a pre-defined database.  If given, can be the only
-        parameter.
-    style : str, optional
-        The database style to use.
-    host : str, optional
-        The URL/file path where the database is hosted.
-    settings : datamodelbase.Settings, optional
-        A Settings object.  Allows for different settings files to be used
-        by downstream packages.
-    databasemanager : datamodelbase.tools.ModuleManager, optional
-        Allows for an alternate databasemanager to be specified by downstream
-        packages. 
-    kwargs : dict, optional
-        Any other keyword parameters defining necessary access information.
-        Allowed keywords are database style-specific.
-    
-    Returns
-    -------
-    Subclass of datamodelbase.Database
-        The database object.
-    """
-
-    # Check that style and name are both not given
-    if style is not None and name is not None:
-        raise ValueError('name and style cannot both be given')
-
-    # Set default package values 
-    if settings is None:
-        settings = default_settings
-    if databasemanager is None:
-        databasemanager = default_databasemanager
-
-    # Load Database info from saved settings
-    if style is None:
-
-        if host is not None or len(kwargs) > 0:
-            raise ValueError('style is required if host and/or kwargs are given')
-
-        # Get information from settings file
-        database_names = settings.list_databases
-        
-        # Ask for name if not given
-        if name is None:
-            if len(database_names) > 0:
-                print('Select a database:')
-                for i, database in enumerate(database_names):
-                    print(i+1, database)
-                choice = screen_input(':')
-                try:
-                    choice = int(choice)
-                except ValueError:
-                    name = choice
-                else:
-                    name = database_names[choice-1]
-            else:
-                raise KeyError('No databases currently set')
-        
-        try:
-            kwargs = settings.databases[name]
-        except KeyError as err:
-            raise KeyError(f'database {name} not found') from err
-
-        style = kwargs.pop('style')
-        host = kwargs.pop('host')
-
-    return databasemanager.init(style, host=host, **kwargs)
+# coding: utf-8
+# Standard Python libraries
+from typing import Optional
+
+# Relative imports
+from ..tools import screen_input, ModuleManager
+from . import databasemanager as default_databasemanager
+from . import Database
+from .. import settings as default_settings
+from .. import Settings
+
+__all__ = ['load_database']
+
+def load_database(name: Optional[str] = None,
+                  style: Optional[str] = None,
+                  host: Optional[str] = None,
+                  settings: Optional[Settings.Settings] = None, 
+                  databasemanager: Optional[ModuleManager] = None,
+                  **kwargs) -> Database:
+    """
+    Loads a database object.  Can be either loaded from stored settings or
+    by defining all needed access information.
+    
+    Parameters
+    ----------
+    name : str, optional
+        The name assigned to a pre-defined database.  If given, can be the only
+        parameter.
+    style : str, optional
+        The database style to use.
+    host : str, optional
+        The URL/file path where the database is hosted.
+    settings : yabadaba.Settings.Settings, optional
+        A Settings object.  Allows for different settings files to be used
+        by downstream packages.
+    databasemanager : yabadaba.tools.ModuleManager, optional
+        Allows for an alternate databasemanager to be specified by downstream
+        packages. 
+    kwargs : dict, optional
+        Any other keyword parameters defining necessary access information.
+        Allowed keywords are database style-specific.
+    
+    Returns
+    -------
+    Subclass of datamodelbase.Database
+        The database object.
+    """
+
+    # Check that style and name are both not given
+    if style is not None and name is not None:
+        raise ValueError('name and style cannot both be given')
+
+    # Set default package values 
+    if settings is None:
+        settings = default_settings
+    if databasemanager is None:
+        databasemanager = default_databasemanager
+
+    # Load Database info from saved settings
+    if style is None:
+
+        if host is not None or len(kwargs) > 0:
+            raise ValueError('style is required if host and/or kwargs are given')
+
+        # Get information from settings file
+        database_names = settings.list_databases
+        
+        # Ask for name if not given
+        if name is None:
+            if len(database_names) > 0:
+                print('Select a database:')
+                for i, database in enumerate(database_names):
+                    print(i+1, database)
+                choice = screen_input(':')
+                try:
+                    choice = int(choice)
+                except ValueError:
+                    name = choice
+                else:
+                    name = database_names[choice-1]
+            else:
+                raise KeyError('No databases currently set')
+        
+        try:
+            kwargs = settings.databases[name]
+        except KeyError as err:
+            raise KeyError(f'database {name} not found') from err
+
+        style = kwargs.pop('style')
+        host = kwargs.pop('host')
+
+    return databasemanager.init(style, host=host, **kwargs)
```

### Comparing `yabadaba-0.2.1/yabadaba/demo/BadRecord.py` & `yabadaba-0.2.2/yabadaba/demo/BadRecord.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from yabadaba.record import Record
-
-from DataModelDict import DataModelDict as DM
-
-raise NotImplementedError('BadRecord is meant to fail import!')
-class BadRecord(Record):
-    """
-    Class for representing FAQ (frequently asked question) records.
-    """
-    @property
-    def style(self):
-        """str: The record style"""
-        return 'BadRecord'
-
-    @property
-    def modelroot(self):
-        """str: The root element of the content"""
-        return 'bad-record'
-
-    def load_model(self, model, name=None):
-        """
-        Loads record contents from a given model.
-
-        Parameters
-        ----------
-        model : str or DataModelDict
-            The model contents of the record to load.
-        name : str, optional
-            The name to assign to the record.  Often inferred from other
-            attributes if not given.
-        """
-        super().load_model(model, name=name)
-
-        bad = self.model[self.modelroot]
-
-    def set_values(self, name=None):
-        """
-        Set multiple object attributes at the same time.
-
-        Parameters
-        ----------
-        name : str, optional
-            The name to assign to the record.  Often inferred from other
-            attributes if not given.
-        """
-        if name is not None:
-            self.name = name
-
-    def build_model(self):
-        """
-        Generates and returns model content based on the values set to object.
-        """
-        model = DM()
-        model['bad'] = DM()
-
-        self._set_model(model)
-        return model
-
-    def metadata(self):
-        """
-        Generates a dict of simple metadata values associated with the record.
-        Useful for quickly comparing records and for building pandas.DataFrames
-        for multiple records of the same style.
-        """
-        meta = {}
-        meta['name'] = self.name
+from yabadaba.record import Record
+
+from DataModelDict import DataModelDict as DM
+
+raise NotImplementedError('BadRecord is meant to fail import!')
+class BadRecord(Record):
+    """
+    Class for representing FAQ (frequently asked question) records.
+    """
+    @property
+    def style(self):
+        """str: The record style"""
+        return 'BadRecord'
+
+    @property
+    def modelroot(self):
+        """str: The root element of the content"""
+        return 'bad-record'
+
+    def load_model(self, model, name=None):
+        """
+        Loads record contents from a given model.
+
+        Parameters
+        ----------
+        model : str or DataModelDict
+            The model contents of the record to load.
+        name : str, optional
+            The name to assign to the record.  Often inferred from other
+            attributes if not given.
+        """
+        super().load_model(model, name=name)
+
+        bad = self.model[self.modelroot]
+
+    def set_values(self, name=None):
+        """
+        Set multiple object attributes at the same time.
+
+        Parameters
+        ----------
+        name : str, optional
+            The name to assign to the record.  Often inferred from other
+            attributes if not given.
+        """
+        if name is not None:
+            self.name = name
+
+    def build_model(self):
+        """
+        Generates and returns model content based on the values set to object.
+        """
+        model = DM()
+        model['bad'] = DM()
+
+        self._set_model(model)
+        return model
+
+    def metadata(self):
+        """
+        Generates a dict of simple metadata values associated with the record.
+        Useful for quickly comparing records and for building pandas.DataFrames
+        for multiple records of the same style.
+        """
+        meta = {}
+        meta['name'] = self.name
         return meta
```

### Comparing `yabadaba-0.2.1/yabadaba/demo/FAQ.py` & `yabadaba-0.2.2/yabadaba/demo/FAQ.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-from yabadaba.record import Record
-from yabadaba import load_query
-
-from DataModelDict import DataModelDict as DM
-
-class FAQ(Record):
-    """
-    Class for representing FAQ (frequently asked question) records.
-    """
-    def __init__(self, model=None, name=None, **kwargs):
-        """
-        Initializes a Record object for a given style.
-        
-        Parameters
-        ----------
-        model : str, file-like object, DataModelDict
-            The contents of the record.
-        name : str, optional
-            The unique name to assign to the record.  If model is a file
-            path, then the default record name is the file name without
-            extension.
-        """
-        self.__question = None
-        self.__answer = None
-        super().__init__(model=model, name=name, **kwargs)
-
-    @property
-    def style(self):
-        """str: The record style"""
-        return 'FAQ'
-
-    @property
-    def modelroot(self):
-        """str: The root element of the content"""
-        return 'faq'
-    
-    @property
-    def xsl_filename(self):
-        """tuple: The module path and file name of the record's xsl html transformer"""
-        return ('yabadaba.demo', 'FAQ.xsl')
-
-    @property
-    def xsd_filename(self):
-        """tuple: The module path and file name of the record's xsd schema"""
-        return ('yabadaba.demo', 'FAQ.xsd')
-
-    @property
-    def question(self):
-        """str: The frequently asked question."""
-        return self.__question
-
-    @question.setter
-    def question(self, value):
-        if value is None:
-            self.__question = None
-        else:
-            self.__question = str(value)
-
-    @property
-    def answer(self):
-        """str: The answer to the frequently asked question."""
-        return self.__answer
-
-    @answer.setter
-    def answer(self, value):
-        if value is None:
-            self.__answer = None
-        else:
-            self.__answer = str(value)
-
-    def load_model(self, model, name=None):
-        """
-        Loads record contents from a given model.
-
-        Parameters
-        ----------
-        model : str or DataModelDict
-            The model contents of the record to load.
-        name : str, optional
-            The name to assign to the record.  Often inferred from other
-            attributes if not given.
-        """
-        super().load_model(model, name=name)
-
-        faq = self.model[self.modelroot]
-        self.question = faq['question']
-        self.answer = faq['answer']
-
-    def set_values(self, name=None, question=None, answer=None):
-        """
-        Set multiple object attributes at the same time.
-
-        Parameters
-        ----------
-        name : str, optional
-            The name to assign to the record.  Often inferred from other
-            attributes if not given.
-        question : str, optional
-            The frequently asked question.
-        answer : str, optional
-            The answer to the frequently asked question.
-        """
-        if question is not None:
-            self.question = question
-        if answer is not None:
-            self.answer = answer
-        if name is not None:
-            self.name = name
-
-    def build_model(self):
-        """
-        Generates and returns model content based on the values set to object.
-        """
-        model = DM()
-        model['faq'] = DM()
-        model['faq']['question'] = self.question
-        model['faq']['answer'] = self.answer
-
-        self._set_model(model)
-        return model
-
-    def metadata(self):
-        """
-        Generates a dict of simple metadata values associated with the record.
-        Useful for quickly comparing records and for building pandas.DataFrames
-        for multiple records of the same style.
-        """
-        meta = {}
-        meta['name'] = self.name
-        meta['question'] = self.question
-        meta['answer'] = self.answer
-        return meta
-
-    @property
-    def queries(self):
-        """dict: Query objects and their associated parameter names."""
-        return {
-            'question': load_query('str_contains',
-                name='question', path=f'{self.modelroot}.question',
-                description='Search the FAQ question field to see if it contains certain strings.'),
-            'answer': load_query('str_contains',
-                name='answer', path=f'{self.modelroot}.answer',
-                description='Search the FAQ answer field to see if it contains certain strings.')
-        }
+from yabadaba.record import Record
+from yabadaba import load_query
+
+from DataModelDict import DataModelDict as DM
+
+class FAQ(Record):
+    """
+    Class for representing FAQ (frequently asked question) records.
+    """
+    def __init__(self, model=None, name=None, **kwargs):
+        """
+        Initializes a Record object for a given style.
+        
+        Parameters
+        ----------
+        model : str, file-like object, DataModelDict
+            The contents of the record.
+        name : str, optional
+            The unique name to assign to the record.  If model is a file
+            path, then the default record name is the file name without
+            extension.
+        """
+        self.__question = None
+        self.__answer = None
+        super().__init__(model=model, name=name, **kwargs)
+
+    @property
+    def style(self):
+        """str: The record style"""
+        return 'FAQ'
+
+    @property
+    def modelroot(self):
+        """str: The root element of the content"""
+        return 'faq'
+    
+    @property
+    def xsl_filename(self):
+        """tuple: The module path and file name of the record's xsl html transformer"""
+        return ('yabadaba.demo', 'FAQ.xsl')
+
+    @property
+    def xsd_filename(self):
+        """tuple: The module path and file name of the record's xsd schema"""
+        return ('yabadaba.demo', 'FAQ.xsd')
+
+    @property
+    def question(self):
+        """str: The frequently asked question."""
+        return self.__question
+
+    @question.setter
+    def question(self, value):
+        if value is None:
+            self.__question = None
+        else:
+            self.__question = str(value)
+
+    @property
+    def answer(self):
+        """str: The answer to the frequently asked question."""
+        return self.__answer
+
+    @answer.setter
+    def answer(self, value):
+        if value is None:
+            self.__answer = None
+        else:
+            self.__answer = str(value)
+
+    def load_model(self, model, name=None):
+        """
+        Loads record contents from a given model.
+
+        Parameters
+        ----------
+        model : str or DataModelDict
+            The model contents of the record to load.
+        name : str, optional
+            The name to assign to the record.  Often inferred from other
+            attributes if not given.
+        """
+        super().load_model(model, name=name)
+
+        faq = self.model[self.modelroot]
+        self.question = faq['question']
+        self.answer = faq['answer']
+
+    def set_values(self, name=None, question=None, answer=None):
+        """
+        Set multiple object attributes at the same time.
+
+        Parameters
+        ----------
+        name : str, optional
+            The name to assign to the record.  Often inferred from other
+            attributes if not given.
+        question : str, optional
+            The frequently asked question.
+        answer : str, optional
+            The answer to the frequently asked question.
+        """
+        if question is not None:
+            self.question = question
+        if answer is not None:
+            self.answer = answer
+        if name is not None:
+            self.name = name
+
+    def build_model(self):
+        """
+        Generates and returns model content based on the values set to object.
+        """
+        model = DM()
+        model['faq'] = DM()
+        model['faq']['question'] = self.question
+        model['faq']['answer'] = self.answer
+
+        self._set_model(model)
+        return model
+
+    def metadata(self):
+        """
+        Generates a dict of simple metadata values associated with the record.
+        Useful for quickly comparing records and for building pandas.DataFrames
+        for multiple records of the same style.
+        """
+        meta = {}
+        meta['name'] = self.name
+        meta['question'] = self.question
+        meta['answer'] = self.answer
+        return meta
+
+    @property
+    def queries(self):
+        """dict: Query objects and their associated parameter names."""
+        return {
+            'question': load_query('str_contains',
+                name='question', path=f'{self.modelroot}.question',
+                description='Search the FAQ question field to see if it contains certain strings.'),
+            'answer': load_query('str_contains',
+                name='answer', path=f'{self.modelroot}.answer',
+                description='Search the FAQ answer field to see if it contains certain strings.')
+        }
```

### Comparing `yabadaba-0.2.1/yabadaba/demo/README.rst` & `yabadaba-0.2.2/yabadaba/demo/README.rst`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-----------
-Demo files
-----------
-
-The files in this directory are meant to provide a demonstration of how to
-build Record objects and link them to the recordmanager.
-
-- FAQ.py defines an example FAQ Record class.  It is meant to serve as a simple
-  example as the data model itself only has two fields: a question and an answer.
-
-- FAQ.xsd provides a XML schema for the FAQ Record's data model.
-
-- FAQ.xsl gives an example transformation of the XML to HTML.
-
-- BadRecord.py defines an example BadRecord that is used by the demo to show
-  how the recordmanager (and other ModuleManager objects) handles modules that
+----------
+Demo files
+----------
+
+The files in this directory are meant to provide a demonstration of how to
+build Record objects and link them to the recordmanager.
+
+- FAQ.py defines an example FAQ Record class.  It is meant to serve as a simple
+  example as the data model itself only has two fields: a question and an answer.
+
+- FAQ.xsd provides a XML schema for the FAQ Record's data model.
+
+- FAQ.xsl gives an example transformation of the XML to HTML.
+
+- BadRecord.py defines an example BadRecord that is used by the demo to show
+  how the recordmanager (and other ModuleManager objects) handles modules that
   fail to import.
```

### Comparing `yabadaba-0.2.1/yabadaba/query/DateMatchQuery.py` & `yabadaba-0.2.2/yabadaba/query/ListContainsQuery.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,129 +1,139 @@
-# coding: utf-8
-
-# Standard Python libraries
-from typing import Any, Optional
-
-import pandas as pd
-
-# Relative imports
-from ..tools import iaslist
-from .Query import Query
-
-class DateMatchQuery(Query):
-    """Class for querying date fields for matching values"""
-
-    @property
-    def style(self) -> str:
-        """str: The query style"""
-        return 'date_match'
-
-    @property
-    def parameter_type(self) -> str:
-        """str: The types of query parameter values accepted by this query style"""
-        return 'str or list, optional'
-
-    def mongo(self,
-              querylist: list,
-              value: Any,
-              prefix: str = ''):
-        """
-        Builds a Mongo query operation for the field.
-
-        Parameters
-        ----------
-        querylist : list
-            The working list of mongo query operations which is to be appended
-            with the operation for this query object.
-        value : any
-            The value of the field to query on.  If None, then no new query
-            operation will be added.
-        prefix : str, optional
-            An optional prefix to add before the query path.  Used by Record's
-            mongoquery to start each path with "content."
-        """
-        # Get path and add prefix
-        path = f'{prefix}{self.path}'
-
-        if value is not None:
-        
-            # Build the query
-            value = [str(v) for v in iaslist(value)]
-            querylist.append( {path: {'$in': value} } )
-
-    def pandas(self,
-               df: pd.DataFrame,
-               value: Any) -> pd.Series:
-        """
-        Applies a query filter to the metadata for the field.
-        
-        Parameters
-        ----------
-        df : pandas.DataFrame
-            A table of metadata for multiple records of the record style.
-        value : any
-            The value of the field to query on.  If None, then it should return
-            True for all rows of df.
-        
-        Returns
-        -------
-        pandas.Series
-            Boolean map of matching values
-        """
-
-        def apply_function(series: pd.Series,
-                           name: str,
-                           value: Any,
-                           parent: Optional[str]) -> bool:
-            """
-            function for pandas.DataFrame.apply with axis=1
-            
-            Parameters
-            ----------
-            series : pd.Series
-                A series of the DataFrame being operated on.
-            name : str
-                The element name.
-            value : any
-                The values to search for.
-            parent : str or None
-                The parent element name, if there is one.
-
-            Returns
-            -------
-            bool
-                True if value is None or if one given value matches the
-                element being checked.
-            """
-            # Return True for all fields if value is None
-            if value is None:
-                return True
-
-            # Convert value to list of strings
-            value = [str(v) for v in iaslist(value)]
-
-            if parent is None:
-
-                # Check if name is in series
-                if name not in series or pd.isna(series[name]):
-                    return False
-
-                # Check for a value match
-                return str(series[name]) in value
-            
-            else:
-
-                # Loop over all child elements
-                for child in iaslist(series[parent]):
-
-                    # Check if child element has name
-                    if name in child and pd.notna(child[name]):
-                    
-                        # Check if child element matches a value
-                        if str(child[name]) in value:
-                            return True
-                
-                # Return default False for no matching child elements
-                return False
-
-        # Use apply_function on df using value and object attributes
-        return df.apply(apply_function, axis=1, args=(self.name, value, self.parent))
+# coding: utf-8
+
+# Standard Python libraries
+from typing import Any, Optional
+
+import pandas as pd
+
+# Relative imports
+from ..tools import iaslist
+from .Query import Query
+
+class ListContainsQuery(Query):
+    """Class for querying list fields for contained values"""
+
+    @property
+    def style(self) -> str:
+        """str: The query style"""
+        return 'list_contains'
+
+    @property
+    def parameter_type(self) -> str:
+        """str: The types of query parameter values accepted by this query style"""
+        return 'str or list, optional'
+
+    def mongo(self,
+              querylist: list,
+              value: Any,
+              prefix: str = ''):
+        """
+        Builds a Mongo query operation for the field.
+
+        Parameters
+        ----------
+        querylist : list
+            The working list of mongo query operations which is to be appended
+            with the operation for this query object.
+        value : any
+            The value of the field to query on.  If None, then no new query
+            operation will be added.
+        prefix : str, optional
+            An optional prefix to add before the query path.  Used by 
+            Record.mongoquery() to start each path with "content."
+        """
+        # Get path and add prefix
+        path = f'{prefix}{self.path}'
+
+        if value is not None:
+        
+            # Init new query
+            newquery = {'$and': []}
+
+            # Build a query for each given value
+            for v in iaslist(value):
+                newquery['$and'].append({path:v})
+
+            # Append newquery to querylist
+            querylist.append(newquery)
+
+    def pandas(self,
+               df: pd.DataFrame,
+               value: Any) -> pd.Series:
+        """
+        Applies a query filter to the metadata for the field.
+        
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            A table of metadata for multiple records of the record style.
+        value : any
+            The value of the field to query on.  If None, then it should return
+            True for all rows of df.
+        
+        Returns
+        -------
+        pandas.Series
+            Boolean map of matching values
+        """
+
+        def apply_function(series: pd.Series,
+                           name: str,
+                           value: Any,
+                           parent: Optional[str] = None) -> bool:
+            """
+            function for pandas.DataFrame.apply with axis=1
+            
+            Parameters
+            ----------
+            series : pd.Series
+                A series of the DataFrame being operated on.
+            name : str
+                The element name.
+            value : any
+                The values to search for.
+            parent : str or None
+                The parent element name, if there is one.
+
+            Returns
+            -------
+            bool
+                True if value is None or if all values are contained in the/an
+                element being checked.
+            """
+            # Return True for all fields if value is None
+            if value is None:
+                return True
+            
+            if parent is None:
+
+                # Check if name is in series
+                if name not in series or not isinstance(series[name], list):
+                    return False
+                
+                # Check if all values are in series[name]
+                for v in iaslist(value):
+                    if v not in series[name]:
+                        return False
+                return True
+            
+            else:
+
+                # Loop over all child elements
+                for child in iaslist(series[parent]):
+
+                    # Check if child element has name
+                    if name in child and isinstance(series[name], list):
+                        match = True
+
+                    # Check if all values are in child[name]
+                        for v in iaslist(value):
+                            if v not in child[name]:
+                                match = False
+                        if match:
+                            return True
+                
+                # Return default False for no matching child elements
+                return False
+
+        # Use apply_function on df using value and object attributes
+        return df.apply(apply_function, axis=1, args=(self.name, value, self.parent))
```

### Comparing `yabadaba-0.2.1/yabadaba/query/IntMatchQuery.py` & `yabadaba-0.2.2/yabadaba/query/StrContainsQuery.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,133 +1,141 @@
-# coding: utf-8
-
-# Standard Python libraries
-from typing import Any, Optional
-
-import pandas as pd
-
-# Relative imports
-from ..tools import iaslist
-
-from .Query import Query
-
-class IntMatchQuery(Query):
-    """Class for querying int fields for matching values"""
-
-    @property
-    def style(self) -> str:
-        """str: The query style"""
-        return 'int_match'
-
-    @property
-    def parameter_type(self) -> str:
-        """str: The types of query parameter values accepted by this query style"""
-        return 'int or list, optional'
-
-    def mongo(self,
-              querylist: list,
-              value: Any,
-              prefix: str = ''):
-        """
-        Builds a Mongo query operation for the field.
-
-        Parameters
-        ----------
-        querylist : list
-            The working list of mongo query operations which is to be appended
-            with the operation for this query object.
-        value : any
-            The value of the field to query on.  If None, then no new query
-            operation will be added.
-        prefix : str, optional
-            An optional prefix to add before the query path.  Used by Record's
-            mongoquery to start each path with "content."
-        """
-        # Get path and add prefix
-        path = f'{prefix}{self.path}'
-
-        if value is not None:
-        
-            # Build the query 
-            val = [int(v) for v in iaslist(value)]
-            querylist.append( {path: {'$in': val} } )
-
-    def pandas(self,
-               df: pd.DataFrame,
-               value: Any) -> pd.Series:
-        """
-        Applies a query filter to the metadata for the field.
-        
-        Parameters
-        ----------
-        df : pandas.DataFrame
-            A table of metadata for multiple records of the record style.
-        value : any
-            The value of the field to query on.  If None, then it should return
-            True for all rows of df.
-        
-        Returns
-        -------
-        pandas.Series
-            Boolean map of matching values
-        """
-
-        def apply_function(series: pd.Series,
-                           name: str,
-                           value: Any,
-                           parent: Optional[str]) -> bool:
-            """
-            function for pandas.DataFrame.apply with axis=1
-            
-            Parameters
-            ----------
-            series : pd.Series
-                A series of the DataFrame being operated on.
-            name : str
-                The element name.
-            value : any
-                The values to search for.
-            parent : str or None
-                The parent element name, if there is one.
-
-            Returns
-            -------
-            bool
-                True if value is None or if one given value matches the
-                element being checked.
-            """
-            # Return True for all fields if value is None
-            if value is None:
-                return True
-            
-            # Convert value to list of ints
-            value = [int(v) for v in iaslist(value)]
-
-            if parent is None:
-
-                # Check if name is in series
-                if name not in series or pd.isna(series[name]):
-                    return False
-                
-                # Check for a value match
-                return int(series[name]) in value
-            
-            else:
-
-                if parent not in series:
-                    return False
-                
-                # Loop over all child elements
-                for child in iaslist(series[parent]):
-
-                    # Check if child element has name
-                    if name in child and pd.notna(child[name]):
-
-                        # Check if child element matches a value
-                        if int(child[name]) in value:
-                            return True
-
-                # Return default False for no matching child elements
-                return False
-
-        # Use apply_function on df using value and object attributes
-        return df.apply(apply_function, axis=1, args=(self.name, value, self.parent))
+# coding: utf-8
+
+# Standard Python libraries
+from typing import Any, Optional
+
+# Relative imports
+from ..tools import iaslist
+from .Query import Query
+
+# https://pandas.pydata.org/
+import pandas as pd
+
+class StrContainsQuery(Query):
+    """Class for querying str fields for contained values"""
+
+    @property
+    def style(self) -> str:
+        """str: The query style"""
+        return 'str_contains'
+
+    @property
+    def parameter_type(self) -> str:
+        """str: The types of query parameter values accepted by this query style"""
+        return 'str or list, optional'
+
+    def mongo(self,
+              querylist: list,
+              value: Any,
+              prefix: str = ''):
+        """
+        Builds a Mongo query operation for the field.
+
+        Parameters
+        ----------
+        querylist : list
+            The working list of mongo query operations which is to be appended
+            with the operation for this query object.
+        value : any
+            The value of the field to query on.  If None, then no new query
+            operation will be added.
+        prefix : str, optional
+            An optional prefix to add before the query path.  Used by Record's
+            mongoquery to start each path with "content."
+        """
+        # Get path and add prefix
+        path = f'{prefix}{self.path}'
+
+        if value is not None:
+            
+            # Init new query
+            newquery = {'$and': []}
+
+            # Build a regex query for each given value
+            for v in iaslist(value):
+                newquery['$and'].append({path:{'$regex': str(v)}})
+
+            # Append newquery to querylist
+            querylist.append(newquery)
+
+    def pandas(self,
+               df: pd.DataFrame,
+               value: Any) -> pd.Series:
+        """
+        Applies a query filter to the metadata for the field.
+        
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            A table of metadata for multiple records of the record style.
+        value : any
+            The value of the field to query on.  If None, then it should return
+            True for all rows of df.
+        
+        Returns
+        -------
+        pandas.Series
+            Boolean map of matching values
+        """
+
+        def apply_function(series: pd.Series,
+                           name: str,
+                           value: Any,
+                           parent: Optional[str]) -> bool:
+            """
+            function for pandas.DataFrame.apply with axis=1
+            
+            Parameters
+            ----------
+            series : pd.Series
+                A series of the DataFrame being operated on.
+            name : str
+                The element name.
+            value : any
+                The values to search for.
+            parent : str or None
+                The parent element name, if there is one.
+
+            Returns
+            -------
+            bool
+                True if value is None or if all values are contained in the/an
+                element being checked.
+            """
+            
+            # Return True for all fields if value is None
+            if value is None:
+                return True
+            
+            if parent is None:
+
+                # Check if name is in series
+                if name not in series or pd.isna(series[name]):
+                    return False
+
+                # Check if all values are in series[name]
+                for v in iaslist(value):
+                    if v not in series[name]:
+                        return False
+                return True
+            
+            else:
+
+                # Loop over all child elements
+                for child in iaslist(series[parent]):
+                    
+                    # Check if child element has name
+                    if name in child and pd.notna(child[name]):
+                        match = True
+                        
+                        # Check if all values are in child[name]
+                        for v in iaslist(value):
+                            if v not in child[name]:
+                                match = False
+                        if match:
+                            return True
+                
+                # Return default False for no matching child elements
+                return False
+
+        # Use apply_function on df using value and object attributes
+        return df.apply(apply_function, axis=1, args=(self.name, value, self.parent))
```

### Comparing `yabadaba-0.2.1/yabadaba/query/Query.py` & `yabadaba-0.2.2/yabadaba/query/Query.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-# coding: utf-8
-
-# Standard Python libraries
-from typing import Any, Optional
-
-import pandas as pd
-class Query():
-    """
-    Base Query class.  Each Query class defines a query operation and each
-    Query object is associated with a specific data field.
-    """
-    
-    def __init__(self,
-                 name: Optional[str] = None,
-                 parent: Optional[str] = None,
-                 path: Optional[str] = None,
-                 description: str = ''):
-        """
-        Query initialization
-
-        Parameters
-        ----------
-        name : str or None, optional
-            The metadata key associated with the data field.  Must be set
-            to use the pandas query method.
-        parent : str or None, optional
-            Allows for the pandas query operations to work on embedded
-            metadata dicts.  If given, the pandas query method will check the
-            value of metadata[parent][name].
-        path : str or None, optional
-            The record data path to the data field.  Levels are delimited by
-            periods.  Must be given to use the mongo query method.
-        description : str, optional
-            Description of the query operation, i.e. what it is searching.
-        """
-        # Check that object is a subclass
-        if self.__module__ == __name__:
-            raise TypeError("Don't use Query itself, only use derived classes")
-
-        self.name = name
-        self.parent = parent
-        self.path = path
-        self.description = description
-
-    def __str__(self) -> str:
-        """
-        Returns
-        -------
-        str
-            The string representation of the query.
-        """
-        return f'query style {self.style}'
-
-    @property
-    def style(self) -> str:
-        """str: The query style"""
-        raise NotImplementedError('Not defined for base class')
-
-    @property
-    def parameter_type(self) -> str:
-        """str: The types of query parameter values accepted by this query style"""
-        return 'str or list, optional'
-
-    @property
-    def name(self) -> str:
-        """str: The metadata key associated with the data field"""
-        if self.__name is None:
-            raise AttributeError('name not set')
-        return self.__name
-
-    @name.setter
-    def name(self, value: Optional[str]):
-        if value is None:
-            self.__name = None
-        elif isinstance(value, str):
-            self.__name = value
-        else:
-            raise TypeError('name must be None or a string')
-
-    @property
-    def parent(self) -> Optional[str]:
-        """str or None: The parent metadata key, if any."""
-        return self.__parent
-
-    @parent.setter
-    def parent(self, value: Optional[str]):
-        if value is None:
-            self.__parent = None
-        elif isinstance(value, str):
-            self.__parent = value
-        else:
-            raise TypeError('parent must be None or a string')
-
-    @property
-    def path(self) -> str:
-        """str: The period delimited path to the associated field."""
-        if self.__path is None:
-            raise AttributeError('path not set')
-        return self.__path
-
-    @path.setter
-    def path(self, value: Optional[str]):
-        if value is None:
-            self.__path = None
-        elif isinstance(value, str):
-            self.__path = value
-        else:
-            raise TypeError('path must be None or a string')
-
-    @property
-    def description(self) -> str:
-        """str: Describes the query operation"""
-        return self.__description
-    
-    @description.setter
-    def description(self, value: str):
-        self.__description = str(value)
-
-    def mongo(self,
-              querylist: list,
-              value: Any,
-              prefix: str = ''):
-        """
-        Builds a Mongo query operation for the field.
-
-        Parameters
-        ----------
-        querylist : list
-            The working list of mongo query operations which is to be appended
-            with the operation for this query object.
-        value : any
-            The value of the field to query on.  If None, then no new query
-            operation will be added.
-        prefix : str, optional
-            An optional prefix to add before the query path.  Used by Record's
-            mongoquery to start each path with "content."
-        """
-        # Do nothing - base class
-        pass
-
-    def pandas(self,
-               df: pd.DataFrame, 
-               value: Any) -> pd.Series:
-        """
-        Applies a query filter to the metadata for the field.
-        
-        Parameters
-        ----------
-        df : pandas.DataFrame
-            A table of metadata for multiple records of the record style.
-        value : any
-            The value of the field to query on.  If None, then it should return
-            True for all rows of df.
-        
-        Returns
-        -------
-        pandas.Series
-            Boolean map of matching values
-        """
-        # Do nothing - base class
-        return df.apply(lambda series:True, axis=1)
+# coding: utf-8
+
+# Standard Python libraries
+from typing import Any, Optional
+
+import pandas as pd
+class Query():
+    """
+    Base Query class.  Each Query class defines a query operation and each
+    Query object is associated with a specific data field.
+    """
+    
+    def __init__(self,
+                 name: Optional[str] = None,
+                 parent: Optional[str] = None,
+                 path: Optional[str] = None,
+                 description: str = ''):
+        """
+        Query initialization
+
+        Parameters
+        ----------
+        name : str or None, optional
+            The metadata key associated with the data field.  Must be set
+            to use the pandas query method.
+        parent : str or None, optional
+            Allows for the pandas query operations to work on embedded
+            metadata dicts.  If given, the pandas query method will check the
+            value of metadata[parent][name].
+        path : str or None, optional
+            The record data path to the data field.  Levels are delimited by
+            periods.  Must be given to use the mongo query method.
+        description : str, optional
+            Description of the query operation, i.e. what it is searching.
+        """
+        # Check that object is a subclass
+        if self.__module__ == __name__:
+            raise TypeError("Don't use Query itself, only use derived classes")
+
+        self.name = name
+        self.parent = parent
+        self.path = path
+        self.description = description
+
+    def __str__(self) -> str:
+        """
+        Returns
+        -------
+        str
+            The string representation of the query.
+        """
+        return f'query style {self.style}'
+
+    @property
+    def style(self) -> str:
+        """str: The query style"""
+        raise NotImplementedError('Not defined for base class')
+
+    @property
+    def parameter_type(self) -> str:
+        """str: The types of query parameter values accepted by this query style"""
+        return 'str or list, optional'
+
+    @property
+    def name(self) -> str:
+        """str: The metadata key associated with the data field"""
+        if self.__name is None:
+            raise AttributeError('name not set')
+        return self.__name
+
+    @name.setter
+    def name(self, value: Optional[str]):
+        if value is None:
+            self.__name = None
+        elif isinstance(value, str):
+            self.__name = value
+        else:
+            raise TypeError('name must be None or a string')
+
+    @property
+    def parent(self) -> Optional[str]:
+        """str or None: The parent metadata key, if any."""
+        return self.__parent
+
+    @parent.setter
+    def parent(self, value: Optional[str]):
+        if value is None:
+            self.__parent = None
+        elif isinstance(value, str):
+            self.__parent = value
+        else:
+            raise TypeError('parent must be None or a string')
+
+    @property
+    def path(self) -> str:
+        """str: The period delimited path to the associated field."""
+        if self.__path is None:
+            raise AttributeError('path not set')
+        return self.__path
+
+    @path.setter
+    def path(self, value: Optional[str]):
+        if value is None:
+            self.__path = None
+        elif isinstance(value, str):
+            self.__path = value
+        else:
+            raise TypeError('path must be None or a string')
+
+    @property
+    def description(self) -> str:
+        """str: Describes the query operation"""
+        return self.__description
+    
+    @description.setter
+    def description(self, value: str):
+        self.__description = str(value)
+
+    def mongo(self,
+              querylist: list,
+              value: Any,
+              prefix: str = ''):
+        """
+        Builds a Mongo query operation for the field.
+
+        Parameters
+        ----------
+        querylist : list
+            The working list of mongo query operations which is to be appended
+            with the operation for this query object.
+        value : any
+            The value of the field to query on.  If None, then no new query
+            operation will be added.
+        prefix : str, optional
+            An optional prefix to add before the query path.  Used by Record's
+            mongoquery to start each path with "content."
+        """
+        # Do nothing - base class
+        pass
+
+    def pandas(self,
+               df: pd.DataFrame, 
+               value: Any) -> pd.Series:
+        """
+        Applies a query filter to the metadata for the field.
+        
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            A table of metadata for multiple records of the record style.
+        value : any
+            The value of the field to query on.  If None, then it should return
+            True for all rows of df.
+        
+        Returns
+        -------
+        pandas.Series
+            Boolean map of matching values
+        """
+        # Do nothing - base class
+        return df.apply(lambda series:True, axis=1)
```

### Comparing `yabadaba-0.2.1/yabadaba/query/__init__.py` & `yabadaba-0.2.2/yabadaba/query/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,53 @@
-# coding: utf-8
-__all__ = ['querymanager', 'Query', 'load_query']
-
-# Relative imports
-#from . import str_contains, str_match, in_list, int_match, list_contains, date_match, float_match
-from .Query import Query
-
-# Initialize a ModuleManager for the query styles
-from ..tools import ModuleManager
-querymanager = ModuleManager('Query')
-
-# Add the modular Query styles (future)
-querymanager.import_style('str_contains', '.StrContainsQuery', __name__)
-querymanager.import_style('str_match', '.StrMatchQuery', __name__)
-querymanager.import_style('list_contains', '.ListContainsQuery', __name__)
-querymanager.import_style('int_match', '.IntMatchQuery', __name__)
-querymanager.import_style('float_match', '.FloatMatchQuery', __name__)
-querymanager.import_style('date_match', '.DateMatchQuery', __name__)
-
-def load_query(style, name=None, parent=None, path=None, description=None,
-               **kwargs):
-    """
-    Loads a Query subclass associated with a given query style.
-
-    Parameters
-    ----------
-    style : str
-        The query style.
-    name : str or None, optional
-        The metadata key associated with the data field.  Must be set
-        to use the pandas query method.
-    parent : str or None, optional
-        Allows for the pandas query operations to work on embedded
-        metadata dicts.  If given, the pandas query method will check the
-        value of metadata[parent][name].
-    path : str or None, optional
-        The record data path to the data field.  Levels are delimited by
-        periods.  Must be given to use the mongo query method.
-    description : str, optional
-        Description of the query operation, i.e. what it is searching.
-    **kwargs : any, optional
-        Any additional style-specific keyword parameters.
-    """
-    return querymanager.init(style, name=name, parent=parent, path=path,
+# coding: utf-8
+__all__ = ['querymanager', 'Query', 'load_query']
+
+# Standard Python libraries
+from typing import Optional
+
+
+# Relative imports
+#from . import str_contains, str_match, in_list, int_match, list_contains, date_match, float_match
+from .Query import Query
+
+# Initialize a ModuleManager for the query styles
+from ..tools import ModuleManager
+querymanager = ModuleManager('Query')
+
+# Add the modular Query styles (future)
+querymanager.import_style('str_contains', '.StrContainsQuery', __name__)
+querymanager.import_style('str_match', '.StrMatchQuery', __name__)
+querymanager.import_style('list_contains', '.ListContainsQuery', __name__)
+querymanager.import_style('int_match', '.IntMatchQuery', __name__)
+querymanager.import_style('float_match', '.FloatMatchQuery', __name__)
+querymanager.import_style('date_match', '.DateMatchQuery', __name__)
+
+def load_query(style: str,
+               name: Optional[str] = None,
+               parent: Optional[str] = None,
+               path: Optional[str] = None,
+               description: Optional[str] = None,
+               **kwargs) -> Query:
+    """
+    Loads a Query subclass associated with a given query style.
+
+    Parameters
+    ----------
+    style : str
+        The query style.
+    name : str or None, optional
+        The metadata key associated with the data field.  Must be set
+        to use the pandas query method.
+    parent : str or None, optional
+        Allows for the pandas query operations to work on embedded
+        metadata dicts.  If given, the pandas query method will check the
+        value of metadata[parent][name].
+    path : str or None, optional
+        The record data path to the data field.  Levels are delimited by
+        periods.  Must be given to use the mongo query method.
+    description : str, optional
+        Description of the query operation, i.e. what it is searching.
+    **kwargs : any, optional
+        Any additional style-specific keyword parameters.
+    """
+    return querymanager.init(style, name=name, parent=parent, path=path,
                              description=description, **kwargs)
```

### Comparing `yabadaba-0.2.1/yabadaba/record/Record.py` & `yabadaba-0.2.2/yabadaba/record/Record.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,458 +1,458 @@
-# coding: utf-8
-# Standard Python libraries
-from pathlib import Path
-from importlib import resources
-from typing import Union, Optional
-import io
-from tarfile import TarFile
-
-# https://ipython.org/
-from IPython.core.display import display, HTML
-
-# https://lxml.de/
-import lxml.etree as ET
-
-import pandas as pd
-
-# https://github.com/usnistgov/DataModelDict
-from DataModelDict import DataModelDict as DM
-
-from .. import load_query
-
-class Record():
-    """
-    Class for handling different record styles in the same fashion.  The
-    base class defines the common methods and attributes.
-    """
-
-    def __init__(self,
-                 model: Union[str, io.IOBase, DM, None] = None,
-                 name: Optional[str] = None,
-                 database = None,
-                 **kwargs: any):
-        """
-        Initializes a Record object for a given style.
-        
-        Parameters
-        ----------
-        model : str, file-like object, or DataModelDict, optional
-            The contents of the record.
-        name : str, optional
-            The unique name to assign to the record.  If model is a file
-            path, then the default record name is the file name without
-            extension.
-        database : yabadaba.Database, optional
-            A default Database to associate with the Record, typically the
-            Database that the Record was obtained from.  Can allow for Record
-            methods to perform Database operations without needing to specify
-            which Database to use.
-        kwargs : any
-            Any record-specific attributes to assign.
-        """
-        self.__model = None
-        self.__name = None
-        self.tar = None
-        self.database = database
-
-        if model is not None:
-            assert len(kwargs) == 0, f"cannot specify kwargs with model: '{kwargs.keys()}'"
-            self.load_model(model, name=name)
-        else:
-            self.set_values(name=name, **kwargs)
-
-    def load_model(self,
-                   model: Union[str, io.IOBase, DM],
-                   name: Optional[str] = None):
-        """
-        Loads record contents from a given model.
-
-        Parameters
-        ----------
-        model : str, file-like object, or DataModelDict
-            The model contents of the record to load.
-        name : str, optional
-            The name to assign to the record.  Often inferred from other
-            attributes if not given.
-        """
-        # Get name if model is a filename
-        if name is None:
-            try:
-                if Path(model).is_file():
-                    self.name = Path(model).stem
-            except (ValueError, OSError, TypeError):
-                pass
-        else:
-            self.name = name
-
-        self._set_model(model)
-
-    def set_values(self, name: Optional[str] = None):
-        """
-        Set multiple object attributes at the same time.
-
-        Parameters
-        ----------
-        name : str, optional
-            The name to assign to the record.  Often inferred from other
-            attributes if not given.
-        """
-        # Set name if given
-        if name is not None:
-            self.name = name
-
-    def __str__(self) -> str:
-        """str: The string representation of the record"""
-        return f'{self.style} record named {self.name}'
-
-    @property
-    def style(self) -> str:
-        """str: The record style"""
-        return 'base'
-
-    @property
-    def xsd_filename(self) -> tuple:
-        """tuple: The module path and file name of the record's xsd schema"""
-        raise NotImplementedError('Not implemented')
-
-    @property
-    def xsd(self) -> bytes:
-        """bytes: The xml schema for the record style."""
-        return resources.read_binary(*self.xsd_filename)
-
-    @property
-    def xsl_filename(self) -> tuple:
-        """tuple: The module path and file name of the record's xsl html transformer"""
-        raise NotImplementedError('Not implemented')
-
-    @property
-    def xsl(self) -> bytes:
-        """bytes: The xsl transformer for the record style."""
-        return resources.read_binary(*self.xsl_filename)
-
-    @property
-    def name(self) -> str:
-        """str: The record's name."""
-        if self.__name is not None:
-            return self.__name
-        else:
-            raise AttributeError('record name not set')
-
-    @name.setter
-    def name(self, value: Optional[str]):
-        if value is not None:
-            self.__name = str(value)
-        else:
-            self.__name = None
-
-    @property
-    def modelroot(self) -> str:
-        """str : The name of the root element in the model contents."""
-        raise NotImplementedError('Specific to subclasses')
-
-    @property
-    def model(self) -> DM:
-        """DataModelDict: The record's model content."""
-        if self.__model is not None:
-            return self.__model
-        else:
-            raise AttributeError('model content has not been loaded or built')
-
-    def reload_model(self):
-        """
-        Reloads the record based on the model content.  This allows for direct
-        changes to the model to be updated to the object. 
-        """
-        self.load_model(model=self.model, name=self.name)
-
-    def _set_model(self, model: DM):
-        """
-        Sets model content - called by build_model() and load_model() to update
-        content.  Use load_model() if you are passing in an external model.
-        """
-        try:
-            modelroot = self.modelroot
-        except NotImplementedError:
-            self.__model = DM(model)
-        else:
-            # Load model as DataModelDict
-            content = DM(model).find(modelroot)
-            self.__model = DM([(modelroot, content)])
-
-    def build_model(self):
-        """
-        Generates and returns model content based on the values set to object.
-        """
-        raise NotImplementedError('Not defined for this class')
-
-    def metadata(self) -> dict:
-        """
-        Generates a dict of simple metadata values associated with the record.
-        Useful for quickly comparing records and for building pandas.DataFrames
-        for multiple records of the same style.
-        """
-        return {}
-
-    @property
-    def queries(self) -> dict:
-        """dict: Query objects and their associated parameter names."""
-        return {}
-
-    @property
-    def querynames(self) -> list:
-        """list: The query parameter names supported by the record."""
-        return list(self.queries.keys())
-
-    @property
-    def querydoc(self) -> str:
-        """str: A description of all the queries supported by the record."""
-        doc = f'# {self.style} Query Parameters\n\n'
-        for name, query in self.queries.items():
-            doc += f'- __{name}__ (*{query.parameter_type}*): {query.description}\n'
-
-        return doc
-
-    def pandasfilter(self,
-                     dataframe: pd.DataFrame,
-                     name: Union[str, list, None] = None,
-                     **kwargs: any) -> pd.Series:
-        """
-        Filters a pandas.DataFrame based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        dataframe : pandas.DataFrame
-            A table of metadata for multiple records of the record style.
-        name : str or list, optional
-            The record name(s) to parse by.
-        **kwargs : any
-            Any of the record style-specific search parameters.
-
-        Returns
-        -------
-        pandas.Series
-            Boolean map of matching values
-        """
-        # Get defined queries
-        queries = self.queries
-
-        # Query name
-        matches = load_query('str_match', name='name').pandas(dataframe, name)
-
-        # Apply queries based on given kwargs
-        for key in kwargs:
-            matches = (matches & queries[key].pandas(dataframe, kwargs[key]))
-
-        return matches
-
-    def mongoquery(self,
-                   name: Union[str, list, None] = None,
-                   **kwargs: any) -> dict:
-        """
-        Builds a Mongo-style query based on kwargs values for the record style.
-
-        Parameters
-        ----------
-        name : str or list, optional
-            The record name(s) to parse by.
-        **kwargs : any
-            Any of the record style-specific search parameters.
-
-        Returns
-        -------
-        dict
-            The Mongo-style query
-        """
-        # Get the dict of queries
-        queries = self.queries
-
-        # Initialize the full query dict and list of query operations
-        querydict = {}
-        querydict['$and'] = querylist = [{}]
-
-        # Query name
-        load_query('str_match', path='name').mongo(querylist, name)
-
-        # Apply queries based on given kwargs
-        for key in kwargs:
-            queries[key].mongo(querylist, kwargs[key], prefix='content.')
-
-        return querydict
-
-    def cdcsquery(self,
-                  **kwargs: any) -> dict:
-        """
-        Builds a CDCS-style query based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        **kwargs : any
-            Any of the record style-specific search parameters.
-        
-        Returns
-        -------
-        dict
-            The CDCS-style query
-        """
-        # Get the dict of queries
-        queries = self.queries
-
-        # Initialize the query dictionary
-        querydict = {}
-        querydict['$and'] = querylist = [{}]
-
-        # Apply queries based on given kwargs
-        for key in kwargs:
-            queries[key].mongo(querylist, kwargs[key])
-
-        return querydict
-
-    def html(self,
-             render: bool = False) -> Optional[str]:
-        """
-        Returns an HTML representation of the object.
-        
-        Parameters
-        ----------
-        render : bool, optional
-            If True, then IPython is used to render the HTML.  If False
-            (default), then the HTML code is returned as a str.
-
-        Returns
-        -------
-        str
-            The HTML code contents.  Returned if render=False.
-        """
-
-        # Build xml content
-        xml_content = self.model.xml()
-
-        xml = ET.fromstring(xml_content.encode('UTF-8'))
-
-        # Read xsl content
-        xsl = ET.fromstring(self.xsl)
-
-        # Transform to html
-        transform = ET.XSLT(xsl)
-        html = transform(xml)
-        html_content = ET.tostring(html).decode('UTF-8')
-
-        if render:
-            display(HTML(html_content))
-        else:
-            return html_content
-
-    def valid_xml(self,
-                  xml_content: Optional[str] = None) -> bool:
-        """
-        Tests if XML content is valid with schema.
-        
-        Parameters
-        ----------
-        xml_content : str, optional
-            XML content to test against the record's schema.
-            If not given, will generate the xml using build_model.
-        
-        Returns
-        -------
-        bool
-            Indicating if XML is valid.
-        """
-
-        # Build xml content
-        if xml_content is None:
-            xml_content = self.model.xml()
-
-        xml = ET.fromstring(xml_content.encode('UTF-8'))
-
-        # Read xsd content
-        xsd = ET.fromstring(self.xsd)
-
-        schema = ET.XMLSchema(xsd)
-        return schema.validate(xml)
-
-    @property
-    def database(self):
-        """yabadaba.Database or None: The default Database associated with the Record"""
-        return self.__database
-
-    @database.setter
-    def database(self, value):
-        if value is None or hasattr(value, 'get_records'):
-            self.__database = value
-        else:
-            raise TypeError('database must be a yabadaba.Database or None')
-
-    @property
-    def tar(self):
-        """tarfile.TarFile: The tar archive associated with the record"""
-        # Return tarfile if set
-        if self.__tar is not None:
-            return self.__tar
-
-        # Check if database is set
-        if self.database is None:
-            raise ValueError('tar not loaded and no database set')
-
-        # Fetch tar from database, set to cache and return
-        self.tar = self.database.get_tar(record=self)
-        return self.__tar
-
-    @tar.setter
-    def tar(self, value: Optional[TarFile]):
-        if value is None or isinstance(value, TarFile):
-            self.__tar = value
-        else:
-            raise TypeError('tar must ne a TarFile or None')
-
-    def clear_tar(self):
-        """Closes and unsets the record's tar file to save memory"""
-        if self.__tar is not None:
-            self.__tar.close()
-            self.tar = None
-
-    def get_file(self,
-                 filename: Union[str, Path],
-                 localroot: Union[str, Path, None] = None):
-        """
-        Retrieves a file either locally or from the record's tar archive.
-
-        Parameters
-        ----------
-        filename : str or Path
-            The name/path for the file.  For local files, this is taken
-            relative to localroot.  For files in the tar archive, this is taken
-            relative to the tar's root directory which is always named for the
-            record, i.e., {self.name}/{filename}.
-        localroot : str, Path or None, optional
-            The local root directory that filename (if it exists) is relative
-            to.  The default value of None will use the current working
-            directory.
-        
-        Raises
-        ------
-        ValueError
-            If filename exists in the tar but is not a file.
-
-        Returns
-        -------
-        io.IOBase
-            A file-like object in binary read mode that allows for the file
-            contents to be read.
-        """
-        # Set default root path
-        if localroot is None:
-            localroot = Path.cwd()
-        else:
-            localroot = Path(localroot)
-
-        # Return local copy of file if it exists
-        localfile = Path(localroot, filename)
-        if Path(localfile).is_file():
-            return open(localfile, 'rb')
-
-        # Return file extracted from tar
-        fileio = self.tar.extractfile(f'{self.name}/{filename}')
-        if fileio is not None:
-            return fileio
-        else:
-            raise ValueError(f'{filename} exists in tar, but is not a file')
+# coding: utf-8
+# Standard Python libraries
+from pathlib import Path
+from importlib import resources
+from typing import Union, Optional
+import io
+from tarfile import TarFile
+
+# https://ipython.org/
+from IPython.display import display, HTML
+
+# https://lxml.de/
+import lxml.etree as ET
+
+import pandas as pd
+
+# https://github.com/usnistgov/DataModelDict
+from DataModelDict import DataModelDict as DM
+
+from .. import load_query
+
+class Record():
+    """
+    Class for handling different record styles in the same fashion.  The
+    base class defines the common methods and attributes.
+    """
+
+    def __init__(self,
+                 model: Union[str, io.IOBase, DM, None] = None,
+                 name: Optional[str] = None,
+                 database = None,
+                 **kwargs: any):
+        """
+        Initializes a Record object for a given style.
+        
+        Parameters
+        ----------
+        model : str, file-like object, or DataModelDict, optional
+            The contents of the record.
+        name : str, optional
+            The unique name to assign to the record.  If model is a file
+            path, then the default record name is the file name without
+            extension.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
+        kwargs : any
+            Any record-specific attributes to assign.
+        """
+        self.__model = None
+        self.__name = None
+        self.tar = None
+        self.database = database
+
+        if model is not None:
+            assert len(kwargs) == 0, f"cannot specify kwargs with model: '{kwargs.keys()}'"
+            self.load_model(model, name=name)
+        else:
+            self.set_values(name=name, **kwargs)
+
+    def load_model(self,
+                   model: Union[str, io.IOBase, DM],
+                   name: Optional[str] = None):
+        """
+        Loads record contents from a given model.
+
+        Parameters
+        ----------
+        model : str, file-like object, or DataModelDict
+            The model contents of the record to load.
+        name : str, optional
+            The name to assign to the record.  Often inferred from other
+            attributes if not given.
+        """
+        # Get name if model is a filename
+        if name is None:
+            try:
+                if Path(model).is_file():
+                    self.name = Path(model).stem
+            except (ValueError, OSError, TypeError):
+                pass
+        else:
+            self.name = name
+
+        self._set_model(model)
+
+    def set_values(self, name: Optional[str] = None):
+        """
+        Set multiple object attributes at the same time.
+
+        Parameters
+        ----------
+        name : str, optional
+            The name to assign to the record.  Often inferred from other
+            attributes if not given.
+        """
+        # Set name if given
+        if name is not None:
+            self.name = name
+
+    def __str__(self) -> str:
+        """str: The string representation of the record"""
+        return f'{self.style} record named {self.name}'
+
+    @property
+    def style(self) -> str:
+        """str: The record style"""
+        return 'base'
+
+    @property
+    def xsd_filename(self) -> tuple:
+        """tuple: The module path and file name of the record's xsd schema"""
+        raise NotImplementedError('Not implemented')
+
+    @property
+    def xsd(self) -> bytes:
+        """bytes: The xml schema for the record style."""
+        return resources.read_binary(*self.xsd_filename)
+
+    @property
+    def xsl_filename(self) -> tuple:
+        """tuple: The module path and file name of the record's xsl html transformer"""
+        raise NotImplementedError('Not implemented')
+
+    @property
+    def xsl(self) -> bytes:
+        """bytes: The xsl transformer for the record style."""
+        return resources.read_binary(*self.xsl_filename)
+
+    @property
+    def name(self) -> str:
+        """str: The record's name."""
+        if self.__name is not None:
+            return self.__name
+        else:
+            raise AttributeError('record name not set')
+
+    @name.setter
+    def name(self, value: Optional[str]):
+        if value is not None:
+            self.__name = str(value)
+        else:
+            self.__name = None
+
+    @property
+    def modelroot(self) -> str:
+        """str : The name of the root element in the model contents."""
+        raise NotImplementedError('Specific to subclasses')
+
+    @property
+    def model(self) -> DM:
+        """DataModelDict: The record's model content."""
+        if self.__model is not None:
+            return self.__model
+        else:
+            raise AttributeError('model content has not been loaded or built')
+
+    def reload_model(self):
+        """
+        Reloads the record based on the model content.  This allows for direct
+        changes to the model to be updated to the object. 
+        """
+        self.load_model(model=self.model, name=self.name)
+
+    def _set_model(self, model: DM):
+        """
+        Sets model content - called by build_model() and load_model() to update
+        content.  Use load_model() if you are passing in an external model.
+        """
+        try:
+            modelroot = self.modelroot
+        except NotImplementedError:
+            self.__model = DM(model)
+        else:
+            # Load model as DataModelDict
+            content = DM(model).find(modelroot)
+            self.__model = DM([(modelroot, content)])
+
+    def build_model(self):
+        """
+        Generates and returns model content based on the values set to object.
+        """
+        raise NotImplementedError('Not defined for this class')
+
+    def metadata(self) -> dict:
+        """
+        Generates a dict of simple metadata values associated with the record.
+        Useful for quickly comparing records and for building pandas.DataFrames
+        for multiple records of the same style.
+        """
+        return {}
+
+    @property
+    def queries(self) -> dict:
+        """dict: Query objects and their associated parameter names."""
+        return {}
+
+    @property
+    def querynames(self) -> list:
+        """list: The query parameter names supported by the record."""
+        return list(self.queries.keys())
+
+    @property
+    def querydoc(self) -> str:
+        """str: A description of all the queries supported by the record."""
+        doc = f'# {self.style} Query Parameters\n\n'
+        for name, query in self.queries.items():
+            doc += f'- __{name}__ (*{query.parameter_type}*): {query.description}\n'
+
+        return doc
+
+    def pandasfilter(self,
+                     dataframe: pd.DataFrame,
+                     name: Union[str, list, None] = None,
+                     **kwargs: any) -> pd.Series:
+        """
+        Filters a pandas.DataFrame based on kwargs values for the record style.
+        
+        Parameters
+        ----------
+        dataframe : pandas.DataFrame
+            A table of metadata for multiple records of the record style.
+        name : str or list, optional
+            The record name(s) to parse by.
+        **kwargs : any
+            Any of the record style-specific search parameters.
+
+        Returns
+        -------
+        pandas.Series
+            Boolean map of matching values
+        """
+        # Get defined queries
+        queries = self.queries
+
+        # Query name
+        matches = load_query('str_match', name='name').pandas(dataframe, name)
+
+        # Apply queries based on given kwargs
+        for key in kwargs:
+            matches = (matches & queries[key].pandas(dataframe, kwargs[key]))
+
+        return matches
+
+    def mongoquery(self,
+                   name: Union[str, list, None] = None,
+                   **kwargs: any) -> dict:
+        """
+        Builds a Mongo-style query based on kwargs values for the record style.
+
+        Parameters
+        ----------
+        name : str or list, optional
+            The record name(s) to parse by.
+        **kwargs : any
+            Any of the record style-specific search parameters.
+
+        Returns
+        -------
+        dict
+            The Mongo-style query
+        """
+        # Get the dict of queries
+        queries = self.queries
+
+        # Initialize the full query dict and list of query operations
+        querydict = {}
+        querydict['$and'] = querylist = [{}]
+
+        # Query name
+        load_query('str_match', path='name').mongo(querylist, name)
+
+        # Apply queries based on given kwargs
+        for key in kwargs:
+            queries[key].mongo(querylist, kwargs[key], prefix='content.')
+
+        return querydict
+
+    def cdcsquery(self,
+                  **kwargs: any) -> dict:
+        """
+        Builds a CDCS-style query based on kwargs values for the record style.
+        
+        Parameters
+        ----------
+        **kwargs : any
+            Any of the record style-specific search parameters.
+        
+        Returns
+        -------
+        dict
+            The CDCS-style query
+        """
+        # Get the dict of queries
+        queries = self.queries
+
+        # Initialize the query dictionary
+        querydict = {}
+        querydict['$and'] = querylist = [{}]
+
+        # Apply queries based on given kwargs
+        for key in kwargs:
+            queries[key].mongo(querylist, kwargs[key])
+
+        return querydict
+
+    def html(self,
+             render: bool = False) -> Optional[str]:
+        """
+        Returns an HTML representation of the object.
+        
+        Parameters
+        ----------
+        render : bool, optional
+            If True, then IPython is used to render the HTML.  If False
+            (default), then the HTML code is returned as a str.
+
+        Returns
+        -------
+        str
+            The HTML code contents.  Returned if render=False.
+        """
+
+        # Build xml content
+        xml_content = self.model.xml()
+
+        xml = ET.fromstring(xml_content.encode('UTF-8'))
+
+        # Read xsl content
+        xsl = ET.fromstring(self.xsl)
+
+        # Transform to html
+        transform = ET.XSLT(xsl)
+        html = transform(xml)
+        html_content = ET.tostring(html).decode('UTF-8')
+
+        if render:
+            display(HTML(html_content))
+        else:
+            return html_content
+
+    def valid_xml(self,
+                  xml_content: Optional[str] = None) -> bool:
+        """
+        Tests if XML content is valid with schema.
+        
+        Parameters
+        ----------
+        xml_content : str, optional
+            XML content to test against the record's schema.
+            If not given, will generate the xml using build_model.
+        
+        Returns
+        -------
+        bool
+            Indicating if XML is valid.
+        """
+
+        # Build xml content
+        if xml_content is None:
+            xml_content = self.model.xml()
+
+        xml = ET.fromstring(xml_content.encode('UTF-8'))
+
+        # Read xsd content
+        xsd = ET.fromstring(self.xsd)
+
+        schema = ET.XMLSchema(xsd)
+        return schema.validate(xml)
+
+    @property
+    def database(self):
+        """yabadaba.Database or None: The default Database associated with the Record"""
+        return self.__database
+
+    @database.setter
+    def database(self, value):
+        if value is None or hasattr(value, 'get_records'):
+            self.__database = value
+        else:
+            raise TypeError('database must be a yabadaba.Database or None')
+
+    @property
+    def tar(self):
+        """tarfile.TarFile: The tar archive associated with the record"""
+        # Return tarfile if set
+        if self.__tar is not None:
+            return self.__tar
+
+        # Check if database is set
+        if self.database is None:
+            raise ValueError('tar not loaded and no database set')
+
+        # Fetch tar from database, set to cache and return
+        self.tar = self.database.get_tar(record=self)
+        return self.__tar
+
+    @tar.setter
+    def tar(self, value: Optional[TarFile]):
+        if value is None or isinstance(value, TarFile):
+            self.__tar = value
+        else:
+            raise TypeError('tar must ne a TarFile or None')
+
+    def clear_tar(self):
+        """Closes and unsets the record's tar file to save memory"""
+        if self.__tar is not None:
+            self.__tar.close()
+            self.tar = None
+
+    def get_file(self,
+                 filename: Union[str, Path],
+                 localroot: Union[str, Path, None] = None):
+        """
+        Retrieves a file either locally or from the record's tar archive.
+
+        Parameters
+        ----------
+        filename : str or Path
+            The name/path for the file.  For local files, this is taken
+            relative to localroot.  For files in the tar archive, this is taken
+            relative to the tar's root directory which is always named for the
+            record, i.e., {self.name}/{filename}.
+        localroot : str, Path or None, optional
+            The local root directory that filename (if it exists) is relative
+            to.  The default value of None will use the current working
+            directory.
+        
+        Raises
+        ------
+        ValueError
+            If filename exists in the tar but is not a file.
+
+        Returns
+        -------
+        io.IOBase
+            A file-like object in binary read mode that allows for the file
+            contents to be read.
+        """
+        # Set default root path
+        if localroot is None:
+            localroot = Path.cwd()
+        else:
+            localroot = Path(localroot)
+
+        # Return local copy of file if it exists
+        localfile = Path(localroot, filename)
+        if Path(localfile).is_file():
+            return open(localfile, 'rb')
+
+        # Return file extracted from tar
+        fileio = self.tar.extractfile(f'{self.name}/{filename}')
+        if fileio is not None:
+            return fileio
+        else:
+            raise ValueError(f'{filename} exists in tar, but is not a file')
```

### Comparing `yabadaba-0.2.1/yabadaba/record/__init__.py` & `yabadaba-0.2.2/yabadaba/record/__init__.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# coding: utf-8
-__all__ = ['Record', 'recordmanager', 'load_record']
-
-# Standard Python libraries
-from typing import Optional, Union
-
-from DataModelDict import DataModelDict as DM
-
-# Relative imports
-from .Record import Record
-from ..tools import ModuleManager
-
-# Initialize ModuleManager for records
-recordmanager = ModuleManager('Record')
-
-# Define load_record
-def load_record(style: str,
-                model: Union[str, DM, None] = None,
-                name: Optional[str] = None,
-                database = None,
-                **kwargs) -> Record:
-    """
-    Loads a Record subclass associated with a given record style.
-
-    Parameters
-    ----------
-    style : str
-        The record style.
-    name : str, optional
-        The name to give to the specific record.
-    model : str, DataModelDict, optional
-        Data model content to load for the given record style.
-    database : yabadaba.Database, optional
-        Allows for a default database to be associated with the record.
-    **kwargs : any
-        Any extra keyword parameter supported by the record style.
-
-    Returns
-    -------
-    subclass of Record 
-        A Record object for the style
-    """
-    record = recordmanager.init(style, model=model, name=name, **kwargs)
-    if database is not None:
-        record.database = database
-    return record
+# coding: utf-8
+__all__ = ['Record', 'recordmanager', 'load_record']
+
+# Standard Python libraries
+from typing import Optional, Union
+
+from DataModelDict import DataModelDict as DM
+
+# Relative imports
+from .Record import Record
+from ..tools import ModuleManager
+
+# Initialize ModuleManager for records
+recordmanager = ModuleManager('Record')
+
+# Define load_record
+def load_record(style: str,
+                model: Union[str, DM, None] = None,
+                name: Optional[str] = None,
+                database = None,
+                **kwargs) -> Record:
+    """
+    Loads a Record subclass associated with a given record style.
+
+    Parameters
+    ----------
+    style : str
+        The record style.
+    name : str, optional
+        The name to give to the specific record.
+    model : str, DataModelDict, optional
+        Data model content to load for the given record style.
+    database : yabadaba.Database, optional
+        Allows for a default database to be associated with the record.
+    **kwargs : any
+        Any extra keyword parameter supported by the record style.
+
+    Returns
+    -------
+    subclass of Record 
+        A Record object for the style
+    """
+    record = recordmanager.init(style, model=model, name=name, **kwargs)
+    if database is not None:
+        record.database = database
+    return record
```

### Comparing `yabadaba-0.2.1/yabadaba/tools/ModuleManager.py` & `yabadaba-0.2.2/yabadaba/tools/ModuleManager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,152 +1,158 @@
-# coding: utf-8
-# Standard Python libraries
-import sys
-from importlib import import_module
-from typing import Optional
-class ModuleManager():
-    """
-    Base class for managing module subclasses
-    """
-    def __init__(self, parentname: str):
-        """
-        Creates a ModuleManager object
-
-        Parameters
-        ----------
-        parentname : str
-            Name of the parent class.  Used solely for messages.
-        """
-        
-        self.__parentname = parentname
-        self.__loaded_styles = {}
-        self.__failed_styles = {}
-
-    def import_style(self, style: str,
-                     modulename: str,
-                     package: Optional[str] = None,
-                     classname: Optional[str] = None):
-        """
-        Tries to import a modular class and appends the results to loaded_styles or
-        failed_styles accordingly.
-
-        Parameters
-        ----------
-        style : str
-            The style name to associate with the modular class.
-        modulename : str
-            The name of the module to try to import.
-        package : str, optional
-            The name of the package which is to act as the anchor for resolving
-            relative package names.
-        classname : str, optional
-            The name of the class in the imported module to associate with
-            the style.  If not given, will use the final name of the modulename
-            path.
-        """
-        if classname is None:
-            classname = modulename.split('.')[-1]
-        
-        try:
-            obj = getattr(import_module(modulename, package=package), classname)
-        except Exception as e:
-            self.failed_styles[style] = '%s: %s' % sys.exc_info()[:2]
-        else:
-            self.loaded_styles[style] = obj
-
-    @property
-    def parentname(self) -> str:
-        """str : The name of the parent class (used for messages)"""
-        return self.__parentname
-
-    @property
-    def loaded_styles(self) -> dict:
-        """dict : The styles that were successfully imported.  Values are the loaded modules"""
-        return self.__loaded_styles
-    
-    @property
-    def failed_styles(self) -> dict:
-        """dict : The styles that were unsuccessfully imported.  Values are the error messages"""
-        return self.__failed_styles
-    
-    @property
-    def loaded_style_names(self) -> list:
-        """list : The names of the loaded styles"""
-        return list(self.loaded_styles.keys())
-
-    @property
-    def failed_style_names(self) -> list:
-        """list : The names of the loaded styles"""
-        return list(self.failed_styles.keys())
-    
-    def check_styles(self):
-        """
-        Prints the list of styles that were successfully and
-        unsuccessfully loaded.
-        """
-        print(f'{self.parentname} styles that passed import:')
-        for style in self.loaded_style_names:
-            print(f'- {style}: {self.loaded_styles[style]}')
-
-        print(f'{self.parentname} styles that failed import:')
-        for style in self.failed_style_names:
-            print(f'- {style}: {self.failed_styles[style]}')
-        print()
-
-    def assert_style(self, style: str):
-        """
-        Checks if the style successfully loaded, throws an error otherwise.
-        
-        Parameters
-        ----------
-        style : str
-            The style name to check.
-
-        Raises
-        ------
-        ImportError
-            If the style is found in failed_styles
-        KeyError
-            If the style is not found in either loaded_styles or failed_styles
-        """
-        if style in self.failed_style_names:
-            raise ImportError(f'{self.parentname} style {style} failed import: {self.failed_styles[style]}')
-        elif style not in self.loaded_style_names:
-            raise KeyError(f'Unknown {self.parentname} style {style}')
-
-    def get_class(self, style):
-        """
-        Retrieves the class of the given style.
-
-        Parameters
-        ----------
-        style : str
-            The style name.
-
-        Returns
-        -------
-        class
-            The uninitialized class.
-        """
-        self.assert_style(style)
-        return self.loaded_styles[style]
-
-    def init(self, style, *args, **kwargs):
-        """
-        Initializes an object of the given style.
-
-        Parameters
-        ----------
-        style : str
-            The style name.
-        *args : any
-            Any additional position-based arguments for the subclass being
-            created.  RECOMMENDED TO USE KWARGS OVER ARGS!!!
-        **kwargs : any
-            Any additional keyword arguments for the subclass being created.
-        Returns
-        -------
-        Object
-            The initialized object.
-        """
-        self.assert_style(style)
+# coding: utf-8
+# Standard Python libraries
+import sys
+from importlib import import_module
+from typing import Optional
+class ModuleManager():
+    """
+    Base class for managing module subclasses
+    """
+    def __init__(self,
+                 parentname: str):
+        """
+        Creates a ModuleManager object
+
+        Parameters
+        ----------
+        parentname : str
+            Name of the parent class.  Used solely for messages.
+        """
+        
+        self.__parentname = parentname
+        self.__loaded_styles = {}
+        self.__failed_styles = {}
+
+    def import_style(self, style: str,
+                     modulename: str,
+                     package: Optional[str] = None,
+                     classname: Optional[str] = None):
+        """
+        Tries to import a modular class and appends the results to loaded_styles or
+        failed_styles accordingly.
+
+        Parameters
+        ----------
+        style : str
+            The style name to associate with the modular class.
+        modulename : str
+            The name of the module to try to import.
+        package : str, optional
+            The name of the package which is to act as the anchor for resolving
+            relative package names.
+        classname : str, optional
+            The name of the class in the imported module to associate with
+            the style.  If not given, will use the final name of the modulename
+            path.
+        """
+        if classname is None:
+            classname = modulename.split('.')[-1]
+        
+        try:
+            obj = getattr(import_module(modulename, package=package), classname)
+        except Exception as e:
+            self.failed_styles[style] = '%s: %s' % sys.exc_info()[:2]
+        else:
+            self.loaded_styles[style] = obj
+
+    @property
+    def parentname(self) -> str:
+        """str : The name of the parent class (used for messages)"""
+        return self.__parentname
+
+    @property
+    def loaded_styles(self) -> dict:
+        """dict : The styles that were successfully imported.  Values are the loaded modules"""
+        return self.__loaded_styles
+    
+    @property
+    def failed_styles(self) -> dict:
+        """dict : The styles that were unsuccessfully imported.  Values are the error messages"""
+        return self.__failed_styles
+    
+    @property
+    def loaded_style_names(self) -> list:
+        """list : The names of the loaded styles"""
+        return list(self.loaded_styles.keys())
+
+    @property
+    def failed_style_names(self) -> list:
+        """list : The names of the loaded styles"""
+        return list(self.failed_styles.keys())
+    
+    def check_styles(self):
+        """
+        Prints the list of styles that were successfully and
+        unsuccessfully loaded.
+        """
+        print(f'{self.parentname} styles that passed import:')
+        for style in self.loaded_style_names:
+            print(f'- {style}: {self.loaded_styles[style]}')
+
+        print(f'{self.parentname} styles that failed import:')
+        for style in self.failed_style_names:
+            print(f'- {style}: {self.failed_styles[style]}')
+        print()
+
+    def assert_style(self,
+                     style: str):
+        """
+        Checks if the style successfully loaded, throws an error otherwise.
+        
+        Parameters
+        ----------
+        style : str
+            The style name to check.
+
+        Raises
+        ------
+        ImportError
+            If the style is found in failed_styles
+        KeyError
+            If the style is not found in either loaded_styles or failed_styles
+        """
+        if style in self.failed_style_names:
+            raise ImportError(f'{self.parentname} style {style} failed import: {self.failed_styles[style]}')
+        elif style not in self.loaded_style_names:
+            raise KeyError(f'Unknown {self.parentname} style {style}')
+
+    def get_class(self,
+                  style: str):
+        """
+        Retrieves the class of the given style.
+
+        Parameters
+        ----------
+        style : str
+            The style name.
+
+        Returns
+        -------
+        class
+            The uninitialized class.
+        """
+        self.assert_style(style)
+        return self.loaded_styles[style]
+
+    def init(self,
+             style: str,
+             *args,
+             **kwargs):
+        """
+        Initializes an object of the given style.
+
+        Parameters
+        ----------
+        style : str
+            The style name.
+        *args : any
+            Any additional position-based arguments for the subclass being
+            created.  RECOMMENDED TO USE KWARGS OVER ARGS!!!
+        **kwargs : any
+            Any additional keyword arguments for the subclass being created.
+        Returns
+        -------
+        Object
+            The initialized object.
+        """
+        self.assert_style(style)
         return self.loaded_styles[style](*args, **kwargs)
```

### Comparing `yabadaba-0.2.1/yabadaba.egg-info/PKG-INFO` & `yabadaba-0.2.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,90 @@
-Metadata-Version: 2.1
-Name: yabadaba
-Version: 0.2.1
-Summary: Yay, a base database! An abstraction layer allowing for common interactions with Mongo, CDCS and local directory databases and records.
-Home-page: https://github.com/usnistgov/yabadaba
-Author: Lucas Hale
-Author-email: lucas.hale@nist.gov
-Keywords: database,mongodb,CDCS
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Physics
-License-File: LICENSE.TXT
-
-========
-yabadaba
-========
-
-The yabadaba package (short for "Yay, a base database!") provides a mid-level
-abstraction layer for interacting with databases containing JSON/XML equivalent
-data records.  The primary purpose of the yabadaba package is to make it easy
-to design user-friendly Python packages that can access and store content in a
-variety of database types.
-
-In design, the yabadaba package consists of five major components:
-
-1. Database classes that provide pythonic APIs to interact with databases.  A
-   base Database class defines common method calls for interacting with the 
-   records in a database, such as querying, adding, modifying, and deleting
-   entries.   Child classes of Database are then defined that implement the
-   universal interaction methods for a given type of database. 
-
-2. A base Record class provides a template for interpreting single database
-   entries.  Developers are meant to specify unique Record classes for each
-   unique schema that is part of their project.  In this way, users can
-   interface with the data both in its raw format and using class-specific
-   methods and attributes.  Each Record class also allows for database query
-   operations to be defined that allow for filtering of any hosted records
-   based on meaningful fields of the Record's schema.
-
-3. A ModuleManager class is defined that helps treat the child classes of
-   the Database and Record classes in a modular fashion.  In particular, the
-   ModuleManagers allow for the code to work even if there are issues with any 
-   of the child classes, and make it possible for packages that import the 
-   managers to append their own child classes.
-
-4. Generic query methods are also provided that support the construction of the
-   record-specific query operations.  In short, these are meant to allow for
-   queries to operate efficiently across all of the database types and ideally
-   return identical responses despite the underlying infrastructure
-   differences.
-
-5. A Settings class is provided that makes it possible for users to save
-   access parameters for a database under a simple name that can then be
-   reloaded in a later session.
-
-Package developers that want to provide APIs to any associated databases can
-simply import the various components of yabadaba and define their own Record
-classes that are specific to their own data.  Users of the resulting packages
-can then easily explore the data, make their own copies, etc.
-
-
-Installation
-------------
-
-The yabadaba package can easily be installed using pip or conda-forge
-
-    pip install yabadaba
-
-or 
-    conda install -c conda-forge yabadaba
-
-Documentation
--------------
-
-Documentation can be found in the doc folder in the github repository.
-
-For support, post a issue to github or email lucas.hale@nist.gov.
+Metadata-Version: 2.1
+Name: yabadaba
+Version: 0.2.2
+Summary: Yay, a base database! An abstraction layer allowing for common interactions with Mongo, CDCS and local directory databases and records.
+Home-page: https://github.com/usnistgov/yabadaba
+Author: Lucas Hale
+Author-email: lucas.hale@nist.gov
+Keywords: database,mongodb,CDCS
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Physics
+License-File: LICENSE.TXT
+Requires-Dist: lxml
+Requires-Dist: DataModelDict
+Requires-Dist: IPython
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: cdcs>=0.2.3
+Requires-Dist: pymongo
+Requires-Dist: tqdm
+
+========
+yabadaba
+========
+
+The yabadaba package (short for "Yay, a base database!") provides a mid-level
+abstraction layer for interacting with databases containing JSON/XML equivalent
+data records.  The primary purpose of the yabadaba package is to make it easy
+to design user-friendly Python packages that can access and store content in a
+variety of database types.
+
+In design, the yabadaba package consists of five major components:
+
+1. Database classes that provide pythonic APIs to interact with databases.  A
+   base Database class defines common method calls for interacting with the 
+   records in a database, such as querying, adding, modifying, and deleting
+   entries.   Child classes of Database are then defined that implement the
+   universal interaction methods for a given type of database. 
+
+2. A base Record class provides a template for interpreting single database
+   entries.  Developers are meant to specify unique Record classes for each
+   unique schema that is part of their project.  In this way, users can
+   interface with the data both in its raw format and using class-specific
+   methods and attributes.  Each Record class also allows for database query
+   operations to be defined that allow for filtering of any hosted records
+   based on meaningful fields of the Record's schema.
+
+3. A ModuleManager class is defined that helps treat the child classes of
+   the Database and Record classes in a modular fashion.  In particular, the
+   ModuleManagers allow for the code to work even if there are issues with any 
+   of the child classes, and make it possible for packages that import the 
+   managers to append their own child classes.
+
+4. Generic query methods are also provided that support the construction of the
+   record-specific query operations.  In short, these are meant to allow for
+   queries to operate efficiently across all of the database types and ideally
+   return identical responses despite the underlying infrastructure
+   differences.
+
+5. A Settings class is provided that makes it possible for users to save
+   access parameters for a database under a simple name that can then be
+   reloaded in a later session.
+
+Package developers that want to provide APIs to any associated databases can
+simply import the various components of yabadaba and define their own Record
+classes that are specific to their own data.  Users of the resulting packages
+can then easily explore the data, make their own copies, etc.
+
+
+Installation
+------------
+
+The yabadaba package can easily be installed using pip or conda-forge
+
+    pip install yabadaba
+
+or 
+    conda install -c conda-forge yabadaba
+
+Documentation
+-------------
+
+Documentation can be found in the doc folder in the github repository.
+
+For support, post a issue to github or email lucas.hale@nist.gov.
```

### Comparing `yabadaba-0.2.1/yabadaba.egg-info/SOURCES.txt` & `yabadaba-0.2.2/yabadaba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

