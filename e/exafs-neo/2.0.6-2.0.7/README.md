# Comparing `tmp/exafs_neo-2.0.6.tar.gz` & `tmp/exafs_neo-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exafs_neo-2.0.6.tar", last modified: Wed Apr 24 22:22:35 2024, max compression
+gzip compressed data, was "exafs_neo-2.0.7.tar", last modified: Fri Apr 26 21:42:40 2024, max compression
```

## Comparing `exafs_neo-2.0.6.tar` & `exafs_neo-2.0.7.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-24 22:22:35.781775 exafs_neo-2.0.6/
--rw-r--r--   0 andy       (501) staff       (20)    35198 2021-08-14 12:28:51.000000 exafs_neo-2.0.6/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)     5782 2024-04-24 22:22:35.781875 exafs_neo-2.0.6/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)     5337 2024-04-24 22:21:42.000000 exafs_neo-2.0.6/README.md
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-24 22:22:35.767691 exafs_neo-2.0.6/exafs_neo/
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-02-03 07:16:06.000000 exafs_neo-2.0.6/exafs_neo/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)      152 2024-04-24 22:22:15.000000 exafs_neo-2.0.6/exafs_neo/_version.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-24 22:22:35.771966 exafs_neo-2.0.6/exafs_neo/analysis/
--rw-r--r--   0 andy       (501) staff       (20)    28217 2024-04-02 02:45:54.000000 exafs_neo-2.0.6/exafs_neo/analysis/EXAFS_Analysis.py
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-19 04:33:48.000000 exafs_neo-2.0.6/exafs_neo/analysis/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)    20093 2024-03-19 06:15:52.000000 exafs_neo-2.0.6/exafs_neo/analysis/larch_score.py
--rw-r--r--   0 andy       (501) staff       (20)     4335 2024-04-24 22:17:00.000000 exafs_neo-2.0.6/exafs_neo/exafs.py
--rw-r--r--   0 andy       (501) staff       (20)     5812 2024-04-02 02:57:21.000000 exafs_neo-2.0.6/exafs_neo/exafs_pop.py
--rw-r--r--   0 andy       (501) staff       (20)     5263 2024-04-02 02:59:48.000000 exafs_neo-2.0.6/exafs_neo/exafsfileobj.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-24 22:22:35.775113 exafs_neo-2.0.6/exafs_neo/gui/
--rw-r--r--   0 andy       (501) staff       (20)     3079 2024-03-19 04:34:51.000000 exafs_neo-2.0.6/exafs_neo/gui/Analysis_plot.py
--rw-r--r--   0 andy       (501) staff       (20)     5721 2024-03-18 17:12:48.000000 exafs_neo-2.0.6/exafs_neo/gui/Background_plot.py
--rw-r--r--   0 andy       (501) staff       (20)     2124 2024-03-18 17:11:48.000000 exafs_neo-2.0.6/exafs_neo/gui/Console.py
--rw-r--r--   0 andy       (501) staff       (20)     1575 2024-04-20 17:28:50.000000 exafs_neo-2.0.6/exafs_neo/gui/Misc_Function.py
--rw-r--r--   0 andy       (501) staff       (20)    54782 2024-04-24 22:01:45.000000 exafs_neo-2.0.6/exafs_neo/gui/XAFS_GUI.py
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-18 05:23:32.000000 exafs_neo-2.0.6/exafs_neo/gui/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     3268 2024-03-18 17:10:18.000000 exafs_neo-2.0.6/exafs_neo/gui/feff_folder_larch.py
--rw-r--r--   0 andy       (501) staff       (20)      265 2023-05-16 01:15:35.000000 exafs_neo-2.0.6/exafs_neo/gui/first_shell_fits.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-24 22:22:35.776948 exafs_neo-2.0.6/exafs_neo/gui/media/
--rw-r--r--   0 andy       (501) staff       (20)      539 2023-07-01 21:09:31.000000 exafs_neo-2.0.6/exafs_neo/gui/media/Citation
--rw-r--r--   0 andy       (501) staff       (20)    35198 2024-04-02 19:10:46.000000 exafs_neo-2.0.6/exafs_neo/gui/media/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)     3848 2021-08-14 12:28:51.000000 exafs_neo-2.0.6/exafs_neo/gui/media/icon.png
--rw-r--r--   0 andy       (501) staff       (20)      983 2024-04-02 03:00:16.000000 exafs_neo-2.0.6/exafs_neo/helper.py
--rw-r--r--   0 andy       (501) staff       (20)     3909 2024-04-02 03:07:35.000000 exafs_neo-2.0.6/exafs_neo/individual.py
--rw-r--r--   0 andy       (501) staff       (20)     6206 2024-04-02 03:12:20.000000 exafs_neo-2.0.6/exafs_neo/ini_parser.py
--rwxr-xr-x   0 andy       (501) staff       (20)     1317 2024-04-02 03:13:29.000000 exafs_neo-2.0.6/exafs_neo/input_arg.py
--rw-r--r--   0 andy       (501) staff       (20)     9228 2024-03-23 23:40:18.000000 exafs_neo-2.0.6/exafs_neo/neoCrossOver.py
--rw-r--r--   0 andy       (501) staff       (20)     3364 2024-04-02 03:14:48.000000 exafs_neo-2.0.6/exafs_neo/neoFilePars.py
--rw-r--r--   0 andy       (501) staff       (20)     9223 2024-04-02 03:15:32.000000 exafs_neo-2.0.6/exafs_neo/neoMutator.py
--rw-r--r--   0 andy       (501) staff       (20)    13873 2024-04-24 02:27:00.000000 exafs_neo-2.0.6/exafs_neo/neoPars.py
--rw-r--r--   0 andy       (501) staff       (20)     3122 2024-04-02 03:23:54.000000 exafs_neo-2.0.6/exafs_neo/neoResult.py
--rw-r--r--   0 andy       (501) staff       (20)     3904 2024-04-24 02:04:22.000000 exafs_neo-2.0.6/exafs_neo/neoSelector.py
--rw-r--r--   0 andy       (501) staff       (20)     3419 2024-04-24 02:27:04.000000 exafs_neo-2.0.6/exafs_neo/neoSolver.py
--rwxr-xr-x   0 andy       (501) staff       (20)     5748 2024-04-02 05:25:47.000000 exafs_neo-2.0.6/exafs_neo/parser.py
--rw-r--r--   0 andy       (501) staff       (20)     2953 2024-04-02 05:26:13.000000 exafs_neo-2.0.6/exafs_neo/pathObj.py
--rw-r--r--   0 andy       (501) staff       (20)     5121 2024-04-02 03:36:53.000000 exafs_neo-2.0.6/exafs_neo/pathrange.py
--rw-r--r--   0 andy       (501) staff       (20)     1321 2024-04-02 03:39:27.000000 exafs_neo-2.0.6/exafs_neo/pathrange_file.py
--rw-r--r--   0 andy       (501) staff       (20)    19175 2024-04-02 05:26:30.000000 exafs_neo-2.0.6/exafs_neo/utils.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-24 22:22:35.770919 exafs_neo-2.0.6/exafs_neo.egg-info/
--rw-r--r--   0 andy       (501) staff       (20)     5782 2024-04-24 22:22:35.000000 exafs_neo-2.0.6/exafs_neo.egg-info/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)     1529 2024-04-24 22:22:35.000000 exafs_neo-2.0.6/exafs_neo.egg-info/SOURCES.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-04-24 22:22:35.000000 exafs_neo-2.0.6/exafs_neo.egg-info/dependency_links.txt
--rw-r--r--   0 andy       (501) staff       (20)       99 2024-04-24 22:22:35.000000 exafs_neo-2.0.6/exafs_neo.egg-info/entry_points.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-02-18 07:51:41.000000 exafs_neo-2.0.6/exafs_neo.egg-info/not-zip-safe
--rw-r--r--   0 andy       (501) staff       (20)       40 2024-04-24 22:22:35.000000 exafs_neo-2.0.6/exafs_neo.egg-info/requires.txt
--rw-r--r--   0 andy       (501) staff       (20)       16 2024-04-24 22:22:35.000000 exafs_neo-2.0.6/exafs_neo.egg-info/top_level.txt
--rw-r--r--   0 andy       (501) staff       (20)       79 2024-04-24 22:22:35.782114 exafs_neo-2.0.6/setup.cfg
--rw-r--r--   0 andy       (501) staff       (20)     1240 2024-04-19 05:22:39.000000 exafs_neo-2.0.6/setup.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-24 22:22:35.781518 exafs_neo-2.0.6/tests/
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-17 22:01:17.000000 exafs_neo-2.0.6/tests/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     4089 2024-03-23 20:03:07.000000 exafs_neo-2.0.6/tests/test_EXAFS_analysis.py
--rw-r--r--   0 andy       (501) staff       (20)     1607 2024-03-23 19:26:46.000000 exafs_neo-2.0.6/tests/test_exafs_fileobj.py
--rw-r--r--   0 andy       (501) staff       (20)     3857 2024-03-23 20:01:49.000000 exafs_neo-2.0.6/tests/test_exafs_pars.py
--rw-r--r--   0 andy       (501) staff       (20)     2280 2024-03-20 02:02:00.000000 exafs_neo-2.0.6/tests/test_exafs_pathObj.py
--rw-r--r--   0 andy       (501) staff       (20)     1573 2024-02-03 07:05:06.000000 exafs_neo-2.0.6/tests/test_exafs_pathrange.py
--rw-r--r--   0 andy       (501) staff       (20)     1053 2024-03-20 03:41:05.000000 exafs_neo-2.0.6/tests/test_individual.py
--rw-r--r--   0 andy       (501) staff       (20)      514 2024-03-17 20:09:18.000000 exafs_neo-2.0.6/tests/test_ini_parser.py
--rw-r--r--   0 andy       (501) staff       (20)     3385 2024-03-23 20:03:36.000000 exafs_neo-2.0.6/tests/test_larchscore.py
--rw-r--r--   0 andy       (501) staff       (20)      976 2024-03-23 23:13:20.000000 exafs_neo-2.0.6/tests/test_neo_pop.py
--rw-r--r--   0 andy       (501) staff       (20)     5754 2024-03-31 00:14:43.000000 exafs_neo-2.0.6/tests/test_neocrossover.py
--rw-r--r--   0 andy       (501) staff       (20)     3771 2024-04-03 00:18:39.000000 exafs_neo-2.0.6/tests/test_neomutator.py
--rw-r--r--   0 andy       (501) staff       (20)     3725 2024-04-24 06:01:42.000000 exafs_neo-2.0.6/tests/test_neosolver.py
--rw-r--r--   0 andy       (501) staff       (20)      338 2024-02-18 20:02:49.000000 exafs_neo-2.0.6/tests/test_utils.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-26 21:42:40.966621 exafs_neo-2.0.7/
+-rw-r--r--   0 andy       (501) staff       (20)    35198 2021-08-14 12:28:51.000000 exafs_neo-2.0.7/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)     5782 2024-04-26 21:42:40.966747 exafs_neo-2.0.7/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)     5337 2024-04-24 22:21:42.000000 exafs_neo-2.0.7/README.md
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-26 21:42:40.958024 exafs_neo-2.0.7/exafs_neo/
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-02-03 07:16:06.000000 exafs_neo-2.0.7/exafs_neo/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)      152 2024-04-26 21:42:38.000000 exafs_neo-2.0.7/exafs_neo/_version.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-26 21:42:40.959884 exafs_neo-2.0.7/exafs_neo/analysis/
+-rw-r--r--   0 andy       (501) staff       (20)    28217 2024-04-02 02:45:54.000000 exafs_neo-2.0.7/exafs_neo/analysis/EXAFS_Analysis.py
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-19 04:33:48.000000 exafs_neo-2.0.7/exafs_neo/analysis/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)    20093 2024-03-19 06:15:52.000000 exafs_neo-2.0.7/exafs_neo/analysis/larch_score.py
+-rw-r--r--   0 andy       (501) staff       (20)     4478 2024-04-26 06:10:02.000000 exafs_neo-2.0.7/exafs_neo/exafs.py
+-rw-r--r--   0 andy       (501) staff       (20)     5812 2024-04-02 02:57:21.000000 exafs_neo-2.0.7/exafs_neo/exafs_pop.py
+-rw-r--r--   0 andy       (501) staff       (20)     5293 2024-04-25 22:22:56.000000 exafs_neo-2.0.7/exafs_neo/exafsfileobj.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-26 21:42:40.962020 exafs_neo-2.0.7/exafs_neo/gui/
+-rw-r--r--   0 andy       (501) staff       (20)     3079 2024-03-19 04:34:51.000000 exafs_neo-2.0.7/exafs_neo/gui/Analysis_plot.py
+-rw-r--r--   0 andy       (501) staff       (20)     5721 2024-03-18 17:12:48.000000 exafs_neo-2.0.7/exafs_neo/gui/Background_plot.py
+-rw-r--r--   0 andy       (501) staff       (20)     2124 2024-03-18 17:11:48.000000 exafs_neo-2.0.7/exafs_neo/gui/Console.py
+-rw-r--r--   0 andy       (501) staff       (20)     1575 2024-04-20 17:28:50.000000 exafs_neo-2.0.7/exafs_neo/gui/Misc_Function.py
+-rw-r--r--   0 andy       (501) staff       (20)    56143 2024-04-26 06:57:47.000000 exafs_neo-2.0.7/exafs_neo/gui/XAFS_GUI.py
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-18 05:23:32.000000 exafs_neo-2.0.7/exafs_neo/gui/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     3268 2024-03-18 17:10:18.000000 exafs_neo-2.0.7/exafs_neo/gui/feff_folder_larch.py
+-rw-r--r--   0 andy       (501) staff       (20)      265 2023-05-16 01:15:35.000000 exafs_neo-2.0.7/exafs_neo/gui/first_shell_fits.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-26 21:42:40.962924 exafs_neo-2.0.7/exafs_neo/gui/media/
+-rw-r--r--   0 andy       (501) staff       (20)      539 2023-07-01 21:09:31.000000 exafs_neo-2.0.7/exafs_neo/gui/media/Citation
+-rw-r--r--   0 andy       (501) staff       (20)    35198 2024-04-02 19:10:46.000000 exafs_neo-2.0.7/exafs_neo/gui/media/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)     3848 2021-08-14 12:28:51.000000 exafs_neo-2.0.7/exafs_neo/gui/media/icon.png
+-rw-r--r--   0 andy       (501) staff       (20)      983 2024-04-02 03:00:16.000000 exafs_neo-2.0.7/exafs_neo/helper.py
+-rw-r--r--   0 andy       (501) staff       (20)     3909 2024-04-02 03:07:35.000000 exafs_neo-2.0.7/exafs_neo/individual.py
+-rw-r--r--   0 andy       (501) staff       (20)     6206 2024-04-02 03:12:20.000000 exafs_neo-2.0.7/exafs_neo/ini_parser.py
+-rwxr-xr-x   0 andy       (501) staff       (20)     1317 2024-04-02 03:13:29.000000 exafs_neo-2.0.7/exafs_neo/input_arg.py
+-rw-r--r--   0 andy       (501) staff       (20)     9291 2024-04-26 05:59:11.000000 exafs_neo-2.0.7/exafs_neo/neoCrossOver.py
+-rw-r--r--   0 andy       (501) staff       (20)     4310 2024-04-26 06:10:55.000000 exafs_neo-2.0.7/exafs_neo/neoFilePars.py
+-rw-r--r--   0 andy       (501) staff       (20)     9294 2024-04-26 06:13:20.000000 exafs_neo-2.0.7/exafs_neo/neoMutator.py
+-rw-r--r--   0 andy       (501) staff       (20)    14134 2024-04-26 06:13:35.000000 exafs_neo-2.0.7/exafs_neo/neoPars.py
+-rw-r--r--   0 andy       (501) staff       (20)     3289 2024-04-26 05:59:28.000000 exafs_neo-2.0.7/exafs_neo/neoResult.py
+-rw-r--r--   0 andy       (501) staff       (20)     3904 2024-04-24 02:04:22.000000 exafs_neo-2.0.7/exafs_neo/neoSelector.py
+-rw-r--r--   0 andy       (501) staff       (20)     3835 2024-04-25 02:28:34.000000 exafs_neo-2.0.7/exafs_neo/neoSolver.py
+-rwxr-xr-x   0 andy       (501) staff       (20)     5748 2024-04-02 05:25:47.000000 exafs_neo-2.0.7/exafs_neo/parser.py
+-rw-r--r--   0 andy       (501) staff       (20)     2953 2024-04-02 05:26:13.000000 exafs_neo-2.0.7/exafs_neo/pathObj.py
+-rw-r--r--   0 andy       (501) staff       (20)     5121 2024-04-02 03:36:53.000000 exafs_neo-2.0.7/exafs_neo/pathrange.py
+-rw-r--r--   0 andy       (501) staff       (20)     1321 2024-04-02 03:39:27.000000 exafs_neo-2.0.7/exafs_neo/pathrange_file.py
+-rw-r--r--   0 andy       (501) staff       (20)    19175 2024-04-02 05:26:30.000000 exafs_neo-2.0.7/exafs_neo/utils.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-26 21:42:40.959257 exafs_neo-2.0.7/exafs_neo.egg-info/
+-rw-r--r--   0 andy       (501) staff       (20)     5782 2024-04-26 21:42:40.000000 exafs_neo-2.0.7/exafs_neo.egg-info/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)     1529 2024-04-26 21:42:40.000000 exafs_neo-2.0.7/exafs_neo.egg-info/SOURCES.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-04-26 21:42:40.000000 exafs_neo-2.0.7/exafs_neo.egg-info/dependency_links.txt
+-rw-r--r--   0 andy       (501) staff       (20)       99 2024-04-26 21:42:40.000000 exafs_neo-2.0.7/exafs_neo.egg-info/entry_points.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-02-18 07:51:41.000000 exafs_neo-2.0.7/exafs_neo.egg-info/not-zip-safe
+-rw-r--r--   0 andy       (501) staff       (20)       40 2024-04-26 21:42:40.000000 exafs_neo-2.0.7/exafs_neo.egg-info/requires.txt
+-rw-r--r--   0 andy       (501) staff       (20)       16 2024-04-26 21:42:40.000000 exafs_neo-2.0.7/exafs_neo.egg-info/top_level.txt
+-rw-r--r--   0 andy       (501) staff       (20)       79 2024-04-26 21:42:40.966982 exafs_neo-2.0.7/setup.cfg
+-rw-r--r--   0 andy       (501) staff       (20)     1240 2024-04-19 05:22:39.000000 exafs_neo-2.0.7/setup.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-26 21:42:40.966379 exafs_neo-2.0.7/tests/
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-17 22:01:17.000000 exafs_neo-2.0.7/tests/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     4089 2024-03-23 20:03:07.000000 exafs_neo-2.0.7/tests/test_EXAFS_analysis.py
+-rw-r--r--   0 andy       (501) staff       (20)     1589 2024-04-25 05:22:20.000000 exafs_neo-2.0.7/tests/test_exafs_fileobj.py
+-rw-r--r--   0 andy       (501) staff       (20)     3857 2024-03-23 20:01:49.000000 exafs_neo-2.0.7/tests/test_exafs_pars.py
+-rw-r--r--   0 andy       (501) staff       (20)     2280 2024-03-20 02:02:00.000000 exafs_neo-2.0.7/tests/test_exafs_pathObj.py
+-rw-r--r--   0 andy       (501) staff       (20)     1573 2024-02-03 07:05:06.000000 exafs_neo-2.0.7/tests/test_exafs_pathrange.py
+-rw-r--r--   0 andy       (501) staff       (20)     1053 2024-03-20 03:41:05.000000 exafs_neo-2.0.7/tests/test_individual.py
+-rw-r--r--   0 andy       (501) staff       (20)      514 2024-03-17 20:09:18.000000 exafs_neo-2.0.7/tests/test_ini_parser.py
+-rw-r--r--   0 andy       (501) staff       (20)     3385 2024-03-23 20:03:36.000000 exafs_neo-2.0.7/tests/test_larchscore.py
+-rw-r--r--   0 andy       (501) staff       (20)      976 2024-03-23 23:13:20.000000 exafs_neo-2.0.7/tests/test_neo_pop.py
+-rw-r--r--   0 andy       (501) staff       (20)     5754 2024-03-31 00:14:43.000000 exafs_neo-2.0.7/tests/test_neocrossover.py
+-rw-r--r--   0 andy       (501) staff       (20)     3771 2024-04-03 00:18:39.000000 exafs_neo-2.0.7/tests/test_neomutator.py
+-rw-r--r--   0 andy       (501) staff       (20)     3725 2024-04-24 06:01:42.000000 exafs_neo-2.0.7/tests/test_neosolver.py
+-rw-r--r--   0 andy       (501) staff       (20)      338 2024-02-18 20:02:49.000000 exafs_neo-2.0.7/tests/test_utils.py
```

### Comparing `exafs_neo-2.0.6/LICENSE` & `exafs_neo-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/PKG-INFO` & `exafs_neo-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exafs_neo
-Version: 2.0.6
+Version: 2.0.7
 Summary: exafs_neo AI analysis using GA
 Home-page: https://github.com/laumiulun/EXAFS_Neo
 Download-URL: https://github.com/laumiulun/EXAFS_Neo/tarball/master
 Author: Miu Lun Lau, Jeff Terry, Min Long
 Author-email: andylau@u.boisestate.edu, jterry98@iit.edu, minlong@boisestate.edu
 License: GPLv3
 Keywords: exafs_neo,AI,analysis
```

### Comparing `exafs_neo-2.0.6/README.md` & `exafs_neo-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/analysis/EXAFS_Analysis.py` & `exafs_neo-2.0.7/exafs_neo/analysis/EXAFS_Analysis.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/analysis/larch_score.py` & `exafs_neo-2.0.7/exafs_neo/analysis/larch_score.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/exafs.py` & `exafs_neo-2.0.7/exafs_neo/exafs.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,45 +83,49 @@
 
             self.selector.select(self.neo_population)
             self.crossOver.crossover(self.neo_population)
             self.mutator.mutate(self.neo_population)
 
             self.neo_population.eval_population()
 
+            # self.solver.solve()
+
             # End of generation verbose
             STRColors.run_verbose_gen(self.logger, self.exafs_neo_pars, self.neo_population,
                                       verbose_lvl=self.verbose_lvl)
             self.result.collect(self.neo_population, self.exafs_neo_pars)
-            self.exafs_neo_pars.runPars.end_gen(self.neo_population)
 
+            # self.exafs_neo_pars.runPars.end_gen(self.neo_population)
+            self.exafs_neo_pars.end_gen(self.neo_population)
         # End of run verbose
         STRColors.run_verbose_end(self.logger, self.exafs_neo_pars, verbose_lvl=self.verbose_lvl)
         return self.result
 
 
 if __name__ == "__main__":
     initializer_override = {
         'printGraph': False
     }
 
     exafs_temp = ExafsNeo(verbose_lvl=5)
 
     input_dict = {
         'data_file': '../path_files/Cu/cu_10k.xmu',
-        'output_file': 'test.log',
+        'output_file': 'test.csv',
         'feff_file': '../path_files/Cu/path_75/feff',
         'nGen': 20,
         'kmin': 0.95,
         'kmax': 9.775,
         'kweight': 3.0,
         'deltak': 0.05,
         'rbkg': 1.1,
         'bkgkw': 1.0,
         'bkgkmax': 15.0,
         'printGraph': False,
         'pathrange': [1, 2, 3, 4, 5],
 
     }
-    exafs_temp.exafs_setup(input_dict)
+    exafs_temp.exafs_read(input_parameters=input_dict)
+    exafs_temp.exafs_setup()
 
     result = exafs_temp.run()
     print(result)
```

### Comparing `exafs_neo-2.0.6/exafs_neo/exafs_pop.py` & `exafs_neo-2.0.7/exafs_neo/exafs_pop.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/exafsfileobj.py` & `exafs_neo-2.0.7/exafs_neo/exafsfileobj.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
                             stdout=subprocess.PIPE)
         if p == 0:
             if logger != None:
                 logger.print('Sabcor Finished')
             return os.path.splitext(data_path)[0] + "_sac.csv"
 
 
+
 class ExafsFileobj:
     sabcorFile: str
 
     def __init__(self):
         self.sabcor_toggle = None
         self.end = None
         self.base = None
@@ -80,15 +81,15 @@
         """
 
         Args:
             i (int, optional): the i-th file. Defaults to 0.
             firstPass (bool, optional): if is the first pass through the dataset. Defaults to False.
             path_optimize (bool, optional): if path optimize. Defaults to False.
         """
-    def initialize_filepath(self, data_dict, i=0, firstPass=False, path_optimize=False, logger=None):
+    def initialize(self, data_dict, i=0, firstPass=False, path_optimize=False, logger=None):
         """
         Initialize file paths for each of the file first
 
         @param dict data_dict:
         @param int i: the i-th file. Defaults to 0.
         @param bool firstPass: if is the first pass through the dataset. Defaults to False.
         @param bool path_optimize: if path optimization
@@ -135,22 +136,25 @@
 
         if self.sabcor_toggle:
             sabcor_executable(self.base,
                               self.sabcorFile,
                               self.data_file,
                               logger=logger)
 
+    def write_generations(self):
+
+        pass
 
 if __name__ == "__main__":
     exafs_File = ExafsFileobj()
 
     data_dict = {
         "data_file": "path_files/Pu_C/pu3in_t030_sac.chi",
         "feff_file": ["path_files/Pu_C/feff/feff","path_files/Pu_C/feff/feff2"],
         "output_file": "result/test/PuC.csv",
         "nComp": 2,
         "sabcor_toggle": False
     }
 
-    exafs_File.initialize_filepath(data_dict)
+    exafs_File.initialize(data_dict)
 
     print(exafs_File.output_file)
```

### Comparing `exafs_neo-2.0.6/exafs_neo/gui/Analysis_plot.py` & `exafs_neo-2.0.7/exafs_neo/gui/Analysis_plot.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/gui/Background_plot.py` & `exafs_neo-2.0.7/exafs_neo/gui/Background_plot.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/gui/Console.py` & `exafs_neo-2.0.7/exafs_neo/gui/Console.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/gui/Misc_Function.py` & `exafs_neo-2.0.7/exafs_neo/gui/Misc_Function.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/gui/XAFS_GUI.py` & `exafs_neo-2.0.7/exafs_neo/gui/XAFS_GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,15 @@
         self.steady_state_exit = BooleanVar(self.root, True)
 
         # Pertubutuions
         self.n_ini = IntVar(self.root, 100)
 
         # Sabcor initalizes variables
         self.sabcor_input_file = StringVar(self.root, 'Please choose a file')
+        self.sabcor_executable = StringVar(self.root,'Please choose the sabcor executable')
         self.sabcor_toggle = BooleanVar(self.root, False)
 
     def initialize_tab(self):
         """
         Initialize tab for the main frame. more tabs
         """
 
@@ -295,15 +296,15 @@
         """
         self.stop_term()
 
         # command = 'exafs_neo -i test_temp.i'
         if self.sabcor_toggle.get() == True:
             # excut_path = check_executable()
             import sabcor
-            execut_path = Path.cwd().parent / 'contrib/sabcor/bin/sabcor'
+            execut_path = self.sabcor_executable.get()
             sabcor.check_executable(paths=execut_path)
             # print(self.sabcor_input_file.get())
             params = sabcor.read_sab(self.sabcor_input_file.get())
             sabcor.write_sab(params)
             print(self.data_file.get())
 
             sabcor.call_executable(execut_path, self.data_file.get())
@@ -1121,29 +1122,40 @@
             file_name = filedialog.askopenfilename(initialdir=os.getcwd(), title="Choose Sabcor Input File",
                                                    filetypes=(("inp file", "*.inp"), ("all files", "*.*")))
             if not file_name:
                 self.sabcor_input_file.set('Please choose a file')
             else:
                 self.sabcor_input_file.set(file_name)
 
+        def select_sabcor_executable():
+            file_name = filedialog.askopenfilename(initialdir=os.getcwd(), title="Choose Sabcor Executable",
+                                                   filetypes=(("exe file", "*.exe"), ("all files", "*.*")))
+            if not file_name:
+                self.sabcor_executable.set('Please choose a file')
+            else:
+                self.sabcor_executable.set(file_name)
         def checkbox_sabcor():
             if self.sabcor_toggle.get() == True:
                 sabcor_input_file.config(state='normal')
                 button_sabcor_input_file.config(state='normal')
+                sabcor_executable.config(state='normal')
+                button_sabcor_executable.config(state='normal')
                 # allow only single entry
                 self.ncomp.set(1)
                 entry_ncomp.config(state='disabled')
 
             else:
                 sabcor_input_file.config(state='disabled')
                 button_sabcor_input_file.config(state='disabled')
+                sabcor_executable.config(state='disabled')
+                button_sabcor_executable.config(state='disabled')
                 entry_ncomp.config(state='normal')
 
-        arr_expert = ["Override Num Compounds", "Sabcor Toggle", "Sabcor Input File"]
-        self.description_tabs(arr_expert, self.tab_Expert, row=[0, 2, 3])
+        arr_expert = ["Override Num Compounds", "Sabcor Toggle", "Sabcor Input File","Sabcor Executable"]
+        self.description_tabs(arr_expert, self.tab_Expert, row=[0, 2, 3, 4])
 
         self.tab_Expert.grid_columnconfigure(1, weight=1)
 
         ncomp_list = list(range(1, 101))
         entry_ncomp = ttk.Combobox(self.tab_Expert, width=7, values=ncomp_list, textvariable=self.ncomp,
                                    font=self.entryFont)
         entry_ncomp.grid(column=1, row=0, sticky=(W, E), padx=self.padx)
@@ -1162,14 +1174,23 @@
         sabcor_input_file.config(state='disabled')
 
         button_sabcor_input_file = ttk.Button(self.tab_Expert, text="Choose",
                                               command=select_sabcor_file, style='my.TButton')
         button_sabcor_input_file.grid(column=3, row=3, sticky=W, padx=self.padx, pady=self.pady)
         button_sabcor_input_file.config(state='disabled')
 
+        sabcor_executable = tk.Entry(self.tab_Expert, textvariable=self.sabcor_executable, font=self.entryFont)
+        sabcor_executable.grid(column=1, row=4, sticky=(W, E), padx=self.padx, pady=self.pady)
+        sabcor_executable.config(state='disabled')
+
+        button_sabcor_executable = ttk.Button(self.tab_Expert, text="Choose",
+                                              command=select_sabcor_executable, style='my.TButton')
+        button_sabcor_executable.grid(column=3, row=4, sticky=W, padx=self.padx, pady=self.pady)
+        button_sabcor_executable.config(state='disabled')
+
     def On_closing(self):
         """
         on closing function
         """
         if messagebox.askokcancel("Quit", "Do you want to quit?"):
             self.stop_term()
             if hasattr(self, 'terminal'):
```

### Comparing `exafs_neo-2.0.6/exafs_neo/gui/feff_folder_larch.py` & `exafs_neo-2.0.7/exafs_neo/gui/feff_folder_larch.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/gui/media/Citation` & `exafs_neo-2.0.7/exafs_neo/gui/media/Citation`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/gui/media/LICENSE` & `exafs_neo-2.0.7/exafs_neo/gui/media/LICENSE`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/gui/media/icon.png` & `exafs_neo-2.0.7/exafs_neo/gui/media/icon.png`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/helper.py` & `exafs_neo-2.0.7/exafs_neo/helper.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/individual.py` & `exafs_neo-2.0.7/exafs_neo/individual.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/ini_parser.py` & `exafs_neo-2.0.7/exafs_neo/ini_parser.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/input_arg.py` & `exafs_neo-2.0.7/exafs_neo/input_arg.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/neoCrossOver.py` & `exafs_neo-2.0.7/exafs_neo/neoCrossOver.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
 class NeoCrossover:
     def __init__(self, logger=None):
         self.logger = logger
         self.exafs_pars = None
         self.crossover_type = None
         self.crossover_operator = None
-
+        self.crossover_score = 0 # TODO: maybe implement this?
     def initialize(self, exafs_pars):
         self.exafs_pars = exafs_pars
 
         self.crossover_type = exafs_pars.crossPars.croOpt
         if self.crossover_type == 0:
             self.crossover_operator = EXAFS_UniformCrossover(exafs_pars, logger=self.logger)
         elif self.crossover_type == 1:
@@ -221,14 +221,15 @@
                     ind2 = pops.next_population[par_ind[1]]
                     child = self.crossover_operator.crossover(pops, ind1, ind2)
                     temp_population.append(child)
 
                 pops.next_population.extend(temp_population)
                 pops.population = pops.next_population
 
+
     def crossover_single(self, pops, ind1, ind2):
         if self.crossover_operator is None:
             raise ValueError("Crossover is not initialized")
         else:
             return self.crossover_operator.crossover(pops, ind1, ind2)
```

### Comparing `exafs_neo-2.0.6/exafs_neo/neoMutator.py` & `exafs_neo-2.0.7/exafs_neo/neoMutator.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
 
 class NeoMutator:
     def __init__(self, logger=None):
         self.mutator = None
         self.logger = logger
         self.mutator_type = None
         self.exafs_pars = None
+        self.mutator_score = 0 # TODO: need to check if this is needed
 
     def initialize(self, exafs_pars):
         self.exafs_pars = exafs_pars
 
         self.mutator_type = exafs_pars.mutPars.mutOpt
         if self.mutator_type == 0:
             self.mutator = ExafsMutator_PerIndividual(self.exafs_pars, logger=self.logger)
```

### Comparing `exafs_neo-2.0.6/exafs_neo/neoPars.py` & `exafs_neo-2.0.7/exafs_neo/neoPars.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,21 @@
         self.neoFilePars.initialize_filepath(cycles=0)
 
         self.exafsRangePars.read_inputs(input_dicts, self.exafsPars)
         self.exafsPathPars.read_inputs(self.neoFilePars, self.exafsPars)
 
         self.exafsPathPars.initialize()
 
+    def output(self):
+        self.neoFilePars.write_outputs(self.runPars, self.bestFitPars)
+        self.neoFilePars.write_data_outputs(self.bestFitPars)
+
+    def end_gen(self,neo_population):
+        self.output()
+        self.runPars.end_gen(neo_population)
 
 @define
 class EXAFSPathRange:
     pathrange_file: str = ''
     pathrange_pars: list = field(default=[])
     npath: int = 0
```

### Comparing `exafs_neo-2.0.6/exafs_neo/neoResult.py` & `exafs_neo-2.0.7/exafs_neo/neoResult.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 import pickle
 
 from matplotlib import pyplot as plt
 
 from exafs_neo.neoPars import NeoPars
 from exafs_neo.utils import NeoLogger
 from exafs_neo.individual import Individual
+from exafs_neo.exafsfileobj import ExafsFileobj
 
 
 @define
 class NeoResult:
     exafs_pars: NeoPars = None
     best_individual: Individual = None
     historyBest: list[float] = field(factory=list)
     historyBestChiR: list[float] = field(factory=list)
+    crossover_scorelist: list[float] = field(factory=list)
+    mutation_scorelist: list[float] = field(factory=list)
     logger: NeoLogger = None
 
+
     def __str__(self):
         if self.best_individual is None:
             return f"Best Individual: None"
         else:
             return f"Best Individual: {self.best_individual}"
 
     def save(self, filename):
@@ -65,14 +69,15 @@
         self.exafs_pars = exafs_pars
         self.best_individual = neo_population.population_sorted[0][0]
         self.historyBest.append(exafs_pars.bestFitPars.globBestVal)
         global_r = exafs_pars.bestFitPars.globBestVal / (
                 len(exafs_pars.exafsPars.intervalK) - 3 * exafs_pars.exafsPars.npath + 1)
         self.historyBestChiR.append(global_r)
 
+
     def plot_fitness(self):
         """
         Plot the fitness function
         :return:
         """
         x = np.arange(0, len(self.historyBest), 1)
```

### Comparing `exafs_neo-2.0.6/exafs_neo/neoSelector.py` & `exafs_neo-2.0.7/exafs_neo/neoSelector.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/neoSolver.py` & `exafs_neo-2.0.7/exafs_neo/neoSolver.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         :param logger:
         """
         self.logger = logger
         self.exafs_pars = exafs_pars
 
         self.sol_list = []
 
-    def select(self, pops):
+    def solve(self, pops, selector,crossover,mutator):
         pass
 
     def __str__(self):
         # return f"Top Percentage: {100 * self.nBest_Percent}%, Lucky: {100 * self.nLucky_Percent}%"
         return f"Neo Solver"
 
 
@@ -28,32 +28,47 @@
     """
 
     def __init__(self, exafs_pars, logger):
         super().__init__(exafs_pars, logger)
         self.solver_type = 0
         self.solver_operator = "Genetic Algorithm"
 
-    def solve(self, pops):
+    def solve(self, pops, selector,crossover,mutator):
         pass
 
 
 class NeoSolver_GA_Rechenberg(NeoSolverBase):
     """
     Standard GA with Rechenberg addition
     """
 
     def __init__(self, exafs_pars, logger):
         super().__init__(exafs_pars, logger)
         self.solver_type = 1
         self.solver_operator = "Genetic Algorithm with Rechenberg"
 
-    def solve(self, pops):
+    def solve(self, pops, selector,crossover,mutator):
+        pass
+
+class NeoSolver_DE(NeoSolverBase):
+    """
+    Standard Differential Evolution
+    """
+
+    def __init__(self, exafs_pars, logger):
+        super().__init__(exafs_pars, logger)
+        self.solver_type = 2
+        self.solver_operator = "Differential Evolution"
+
+    def solve(self, pops, selector,crossover,mutator):
         pass
 
 
+
+
 class NeoSolver:
 
     def __init__(self, logger=None):
         """
         Neo Selector
         :param NeoLogger logger: logger for Neo
         """
@@ -84,15 +99,15 @@
         Perform the actual selection
         :param NeoPopulation pops:  
         :return:
         """
         if self.solver_operator is None:
             raise ValueError("Selector is not initialized")
         else:
-            return self.solver_operator.select(pops)
+            return self.solver_operator.solve(pops)
 
     def __str__(self):
         if self.solver_operator is None:
             return "None Mutator selected"
         else:
             return f"Selector Type: {self.solver_type}, {self.solver_operator}"
```

### Comparing `exafs_neo-2.0.6/exafs_neo/parser.py` & `exafs_neo-2.0.7/exafs_neo/parser.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/pathObj.py` & `exafs_neo-2.0.7/exafs_neo/pathObj.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/pathrange.py` & `exafs_neo-2.0.7/exafs_neo/pathrange.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/pathrange_file.py` & `exafs_neo-2.0.7/exafs_neo/pathrange_file.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo/utils.py` & `exafs_neo-2.0.7/exafs_neo/utils.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/exafs_neo.egg-info/PKG-INFO` & `exafs_neo-2.0.7/exafs_neo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exafs-neo
-Version: 2.0.6
+Version: 2.0.7
 Summary: exafs_neo AI analysis using GA
 Home-page: https://github.com/laumiulun/EXAFS_Neo
 Download-URL: https://github.com/laumiulun/EXAFS_Neo/tarball/master
 Author: Miu Lun Lau, Jeff Terry, Min Long
 Author-email: andylau@u.boisestate.edu, jterry98@iit.edu, minlong@boisestate.edu
 License: GPLv3
 Keywords: exafs_neo,AI,analysis
```

### Comparing `exafs_neo-2.0.6/exafs_neo.egg-info/SOURCES.txt` & `exafs_neo-2.0.7/exafs_neo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/setup.py` & `exafs_neo-2.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/tests/test_EXAFS_analysis.py` & `exafs_neo-2.0.7/tests/test_EXAFS_analysis.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/tests/test_exafs_fileobj.py` & `exafs_neo-2.0.7/tests/test_exafs_fileobj.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         data_dict = {
             "data_file": "path_files/Pu_C/pu3in_t030_sac.chi",
             "feff_file": "path_files/Pu_C/feff/feff",
             "output_file": "result/test/PuC.csv",
             "sabcor_toggle": False
         }
 
-        exafs_File.initialize_filepath(data_dict)
+        exafs_File.initialize(data_dict)
 
         self.assertEqual(exafs_File.csv_series, False)
         self.assertEqual(exafs_File.data_file,'path_files/Pu_C/pu3in_t030_sac.chi')
         self.assertEqual(exafs_File.end,'.dat')
         self.assertEqual(exafs_File.nComp,1)
         self.assertEqual(exafs_File.sabcorFile, False)
         self.assertEqual(exafs_File.sabcor_toggle, False)
@@ -31,15 +31,15 @@
             "data_file": "path_files/Pu_C/pu3in_t030_sac.chi",
             "feff_file": ["path_files/Pu_C/feff/feff", "path_files/Pu_C/feff/feff2"],
             "output_file": "result/test/PuC.csv",
             "nComp": 2,
             "sabcor_toggle": False
         }
 
-        exafs_File.initialize_filepath(data_dict)
+        exafs_File.initialize(data_dict)
 
         self.assertEqual(exafs_File.feff_file[0],'path_files/Pu_C/feff/feff')
         self.assertEqual(exafs_File.feff_file[1],'path_files/Pu_C/feff/feff2')
         self.assertEqual(exafs_File.nComp,2)
 
 
     def test_neoPars_sabcor(self):
```

### Comparing `exafs_neo-2.0.6/tests/test_exafs_pars.py` & `exafs_neo-2.0.7/tests/test_exafs_pars.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/tests/test_exafs_pathObj.py` & `exafs_neo-2.0.7/tests/test_exafs_pathObj.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/tests/test_exafs_pathrange.py` & `exafs_neo-2.0.7/tests/test_exafs_pathrange.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/tests/test_individual.py` & `exafs_neo-2.0.7/tests/test_individual.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/tests/test_ini_parser.py` & `exafs_neo-2.0.7/tests/test_ini_parser.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/tests/test_larchscore.py` & `exafs_neo-2.0.7/tests/test_larchscore.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/tests/test_neo_pop.py` & `exafs_neo-2.0.7/tests/test_neo_pop.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/tests/test_neocrossover.py` & `exafs_neo-2.0.7/tests/test_neocrossover.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/tests/test_neomutator.py` & `exafs_neo-2.0.7/tests/test_neomutator.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.6/tests/test_neosolver.py` & `exafs_neo-2.0.7/tests/test_neosolver.py`

 * *Files identical despite different names*

