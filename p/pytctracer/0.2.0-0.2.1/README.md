# Comparing `tmp/pytctracer-0.2.0.tar.gz` & `tmp/pytctracer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytctracer-0.2.0.tar", last modified: Wed Apr 24 03:17:28 2024, max compression
+gzip compressed data, was "pytctracer-0.2.1.tar", last modified: Fri Apr 26 01:47:12 2024, max compression
```

## Comparing `pytctracer-0.2.0.tar` & `pytctracer-0.2.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.413494 pytctracer-0.2.0/
--rw-rw-rw-   0        0        0    17287 2024-04-24 03:17:28.411855 pytctracer-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    16293 2024-04-24 03:00:56.000000 pytctracer-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.291186 pytctracer-0.2.0/data/
-drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.278504 pytctracer-0.2.0/data/ground-truth-data/
-drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.293703 pytctracer-0.2.0/data/ground-truth-data/pyopenssl/
--rw-rw-rw-   0        0        0    14927 2023-12-12 17:26:56.000000 pytctracer-0.2.0/data/ground-truth-data/pyopenssl/pyopenssl_all_functions.py
--rw-rw-rw-   0        0        0     2737 2024-01-17 14:14:19.000000 pytctracer-0.2.0/data/ground-truth-data/pyopenssl/pyopenssl_chosen_tests.py
--rw-rw-rw-   0        0        0     2195 2024-04-09 23:53:27.000000 pytctracer-0.2.0/data/t.py
--rw-rw-rw-   0        0        0      464 2024-02-25 02:21:54.000000 pytctracer-0.2.0/data/tes.py
--rw-rw-rw-   0        0        0    81882 2024-04-10 01:44:54.000000 pytctracer-0.2.0/data/trace_parser_dynamic.py
--rw-rw-rw-   0        0        0     1045 2024-04-24 03:16:49.000000 pytctracer-0.2.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.299840 pytctracer-0.2.0/pytctracer/
--rw-rw-rw-   0        0        0      104 2024-03-31 18:38:21.000000 pytctracer-0.2.0/pytctracer/__init__.py
--rw-rw-rw-   0        0        0    19325 2024-04-24 00:24:50.000000 pytctracer-0.2.0/pytctracer/analyser.py
--rw-rw-rw-   0        0        0     9121 2024-04-24 00:28:28.000000 pytctracer-0.2.0/pytctracer/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.337488 pytctracer-0.2.0/pytctracer/config/
--rw-rw-rw-   0        0        0       49 2024-03-30 00:46:49.000000 pytctracer-0.2.0/pytctracer/config/__init__.py
--rw-rw-rw-   0        0        0     1101 2024-04-24 01:08:28.000000 pytctracer-0.2.0/pytctracer/config/config.py
-drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.354537 pytctracer-0.2.0/pytctracer/config/constants/
--rw-rw-rw-   0        0        0      904 2024-04-03 23:07:54.000000 pytctracer-0.2.0/pytctracer/config/constants/__init__.py
--rw-rw-rw-   0        0        0      180 2024-04-03 23:05:28.000000 pytctracer-0.2.0/pytctracer/config/constants/classification_type.py
--rw-rw-rw-   0        0        0      380 2024-04-03 23:05:47.000000 pytctracer-0.2.0/pytctracer/config/constants/event_type.py
--rw-rw-rw-   0        0        0      216 2024-04-03 23:05:58.000000 pytctracer-0.2.0/pytctracer/config/constants/function_type.py
--rw-rw-rw-   0        0        0      129 2024-04-03 23:06:06.000000 pytctracer-0.2.0/pytctracer/config/constants/instruction_opname.py
--rw-rw-rw-   0        0        0       99 2024-04-03 23:07:08.000000 pytctracer-0.2.0/pytctracer/config/constants/level_type.py
--rw-rw-rw-   0        0        0      202 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/config/constants/metric_score_type.py
--rw-rw-rw-   0        0        0      535 2024-04-03 23:07:28.000000 pytctracer-0.2.0/pytctracer/config/constants/technique_parameter.py
--rw-rw-rw-   0        0        0      915 2024-04-24 01:14:30.000000 pytctracer-0.2.0/pytctracer/config/constants/technique_threshold.py
--rw-rw-rw-   0        0        0      149 2024-04-03 23:07:44.000000 pytctracer-0.2.0/pytctracer/config/constants/testing_method_event_type.py
--rw-rw-rw-   0        0        0      572 2024-04-03 23:07:50.000000 pytctracer-0.2.0/pytctracer/config/constants/trace_data_header.py
--rw-rw-rw-   0        0        0      507 2024-04-03 23:07:54.000000 pytctracer-0.2.0/pytctracer/config/constants/trace_data_variable.py
-drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.358893 pytctracer-0.2.0/pytctracer/evaluation/
--rw-rw-rw-   0        0        0      170 2024-03-26 14:14:33.000000 pytctracer-0.2.0/pytctracer/evaluation/__init__.py
--rw-rw-rw-   0        0        0     2358 2024-04-24 01:05:02.000000 pytctracer-0.2.0/pytctracer/evaluation/classify_predictions.py
--rw-rw-rw-   0        0        0     2808 2024-04-24 01:06:16.000000 pytctracer-0.2.0/pytctracer/evaluation/evaluate_predictions.py
-drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.373440 pytctracer-0.2.0/pytctracer/evaluation/metrics/
--rw-rw-rw-   0        0        0      613 2024-03-30 00:46:46.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/__init__.py
--rw-rw-rw-   0        0        0     1581 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/area_under_curve.py
--rw-rw-rw-   0        0        0     2967 2024-03-30 00:46:45.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py
--rw-rw-rw-   0        0        0      914 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/f1.py
--rw-rw-rw-   0        0        0      989 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/false_negatives.py
--rw-rw-rw-   0        0        0      989 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/false_positives.py
--rw-rw-rw-   0        0        0     1470 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/mean_average_precision.py
--rw-rw-rw-   0        0        0      744 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/metric.py
--rw-rw-rw-   0        0        0     1084 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/precision.py
--rw-rw-rw-   0        0        0     1060 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/recall.py
--rw-rw-rw-   0        0        0      995 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/true_positives.py
-drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.375742 pytctracer-0.2.0/pytctracer/io/
--rw-rw-rw-   0        0        0        0 2024-03-30 00:46:30.000000 pytctracer-0.2.0/pytctracer/io/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.377740 pytctracer-0.2.0/pytctracer/io/input/
--rw-rw-rw-   0        0        0      110 2024-03-30 00:46:37.000000 pytctracer-0.2.0/pytctracer/io/input/__init__.py
--rw-rw-rw-   0        0        0     2337 2024-04-24 01:04:25.000000 pytctracer-0.2.0/pytctracer/io/input/from_file.py
-drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.382738 pytctracer-0.2.0/pytctracer/io/output/
--rw-rw-rw-   0        0        0      367 2024-03-30 00:46:35.000000 pytctracer-0.2.0/pytctracer/io/output/__init__.py
--rw-rw-rw-   0        0        0     3167 2024-04-24 01:02:45.000000 pytctracer-0.2.0/pytctracer/io/output/to_display.py
--rw-rw-rw-   0        0        0     2372 2024-04-24 01:00:34.000000 pytctracer-0.2.0/pytctracer/io/output/to_file.py
-drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.392564 pytctracer-0.2.0/pytctracer/parsing/
--rw-rw-rw-   0        0        0     1382 2024-03-30 00:46:28.000000 pytctracer-0.2.0/pytctracer/parsing/__init__.py
--rw-rw-rw-   0        0        0     7243 2024-04-24 00:56:25.000000 pytctracer-0.2.0/pytctracer/parsing/find_class_level_calls.py
--rw-rw-rw-   0        0        0     2124 2024-04-24 00:54:18.000000 pytctracer-0.2.0/pytctracer/parsing/find_class_level_names.py
--rw-rw-rw-   0        0        0     6552 2024-04-24 00:53:40.000000 pytctracer-0.2.0/pytctracer/parsing/find_function_level_calls.py
--rw-rw-rw-   0        0        0     2032 2024-04-24 00:51:05.000000 pytctracer-0.2.0/pytctracer/parsing/find_function_level_names.py
--rw-rw-rw-   0        0        0     4285 2024-04-24 00:49:28.000000 pytctracer-0.2.0/pytctracer/parsing/functions_called_before_assert.py
-drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.408011 pytctracer-0.2.0/pytctracer/techniques/
--rw-rw-rw-   0        0        0      883 2024-03-27 16:49:38.000000 pytctracer-0.2.0/pytctracer/techniques/__init__.py
--rw-rw-rw-   0        0        0     4333 2024-04-24 00:24:31.000000 pytctracer-0.2.0/pytctracer/techniques/arg_name_to_technique_mapper.py
--rw-rw-rw-   0        0        0     3510 2024-04-24 00:47:26.000000 pytctracer-0.2.0/pytctracer/techniques/combined.py
--rw-rw-rw-   0        0        0     4021 2024-04-03 23:07:28.000000 pytctracer-0.2.0/pytctracer/techniques/last_call_before_assert.py
--rw-rw-rw-   0        0        0     5118 2024-04-24 00:41:57.000000 pytctracer-0.2.0/pytctracer/techniques/levenshtein_distance.py
--rw-rw-rw-   0        0        0    11089 2024-04-24 00:41:20.000000 pytctracer-0.2.0/pytctracer/techniques/longest_common_subsequence.py
--rw-rw-rw-   0        0        0     6043 2024-04-24 00:40:03.000000 pytctracer-0.2.0/pytctracer/techniques/naming_conventions.py
--rw-rw-rw-   0        0        0     4976 2024-04-24 00:39:20.000000 pytctracer-0.2.0/pytctracer/techniques/tarantula.py
--rw-rw-rw-   0        0        0     6966 2024-04-24 00:44:46.000000 pytctracer-0.2.0/pytctracer/techniques/technique.py
--rw-rw-rw-   0        0        0    11270 2024-04-24 00:36:56.000000 pytctracer-0.2.0/pytctracer/techniques/tfidf.py
--rw-rw-rw-   0        0        0    21573 2024-04-24 01:38:40.000000 pytctracer-0.2.0/pytctracer/tracer.py
-drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.410112 pytctracer-0.2.0/pytctracer.egg-info/
--rw-rw-rw-   0        0        0    17287 2024-04-24 03:17:28.000000 pytctracer-0.2.0/pytctracer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2634 2024-04-24 03:17:28.000000 pytctracer-0.2.0/pytctracer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 03:17:28.000000 pytctracer-0.2.0/pytctracer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-24 03:17:28.000000 pytctracer-0.2.0/pytctracer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      166 2024-04-24 03:17:28.000000 pytctracer-0.2.0/pytctracer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2024-04-24 03:17:28.000000 pytctracer-0.2.0/pytctracer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 03:17:28.413494 pytctracer-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.572296 pytctracer-0.2.1/
+-rw-rw-rw-   0        0        0    17285 2024-04-26 01:47:12.570299 pytctracer-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    16291 2024-04-26 01:45:21.000000 pytctracer-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.419804 pytctracer-0.2.1/data/
+drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.408037 pytctracer-0.2.1/data/ground-truth-data/
+drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.423313 pytctracer-0.2.1/data/ground-truth-data/pyopenssl/
+-rw-rw-rw-   0        0        0    14927 2023-12-12 17:26:56.000000 pytctracer-0.2.1/data/ground-truth-data/pyopenssl/pyopenssl_all_functions.py
+-rw-rw-rw-   0        0        0     2737 2024-01-17 14:14:19.000000 pytctracer-0.2.1/data/ground-truth-data/pyopenssl/pyopenssl_chosen_tests.py
+-rw-rw-rw-   0        0        0     2195 2024-04-09 23:53:27.000000 pytctracer-0.2.1/data/t.py
+-rw-rw-rw-   0        0        0      464 2024-02-25 02:21:54.000000 pytctracer-0.2.1/data/tes.py
+-rw-rw-rw-   0        0        0    81882 2024-04-10 01:44:54.000000 pytctracer-0.2.1/data/trace_parser_dynamic.py
+-rw-rw-rw-   0        0        0     1045 2024-04-26 01:46:22.000000 pytctracer-0.2.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.439552 pytctracer-0.2.1/pytctracer/
+-rw-rw-rw-   0        0        0      104 2024-03-31 18:38:21.000000 pytctracer-0.2.1/pytctracer/__init__.py
+-rw-rw-rw-   0        0        0    22580 2024-04-26 01:41:25.000000 pytctracer-0.2.1/pytctracer/analyser.py
+-rw-rw-rw-   0        0        0     9139 2024-04-26 01:35:00.000000 pytctracer-0.2.1/pytctracer/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.471716 pytctracer-0.2.1/pytctracer/config/
+-rw-rw-rw-   0        0        0       49 2024-03-30 00:46:49.000000 pytctracer-0.2.1/pytctracer/config/__init__.py
+-rw-rw-rw-   0        0        0     1101 2024-04-24 01:08:28.000000 pytctracer-0.2.1/pytctracer/config/config.py
+drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.498332 pytctracer-0.2.1/pytctracer/config/constants/
+-rw-rw-rw-   0        0        0      904 2024-04-03 23:07:54.000000 pytctracer-0.2.1/pytctracer/config/constants/__init__.py
+-rw-rw-rw-   0        0        0      180 2024-04-03 23:05:28.000000 pytctracer-0.2.1/pytctracer/config/constants/classification_type.py
+-rw-rw-rw-   0        0        0      380 2024-04-03 23:05:47.000000 pytctracer-0.2.1/pytctracer/config/constants/event_type.py
+-rw-rw-rw-   0        0        0      216 2024-04-03 23:05:58.000000 pytctracer-0.2.1/pytctracer/config/constants/function_type.py
+-rw-rw-rw-   0        0        0      129 2024-04-03 23:06:06.000000 pytctracer-0.2.1/pytctracer/config/constants/instruction_opname.py
+-rw-rw-rw-   0        0        0       99 2024-04-03 23:07:08.000000 pytctracer-0.2.1/pytctracer/config/constants/level_type.py
+-rw-rw-rw-   0        0        0      202 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/config/constants/metric_score_type.py
+-rw-rw-rw-   0        0        0      535 2024-04-03 23:07:28.000000 pytctracer-0.2.1/pytctracer/config/constants/technique_parameter.py
+-rw-rw-rw-   0        0        0      915 2024-04-24 01:14:30.000000 pytctracer-0.2.1/pytctracer/config/constants/technique_threshold.py
+-rw-rw-rw-   0        0        0      149 2024-04-03 23:07:44.000000 pytctracer-0.2.1/pytctracer/config/constants/testing_method_event_type.py
+-rw-rw-rw-   0        0        0      572 2024-04-03 23:07:50.000000 pytctracer-0.2.1/pytctracer/config/constants/trace_data_header.py
+-rw-rw-rw-   0        0        0      507 2024-04-03 23:07:54.000000 pytctracer-0.2.1/pytctracer/config/constants/trace_data_variable.py
+drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.505999 pytctracer-0.2.1/pytctracer/evaluation/
+-rw-rw-rw-   0        0        0      170 2024-03-26 14:14:33.000000 pytctracer-0.2.1/pytctracer/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     2358 2024-04-24 01:05:02.000000 pytctracer-0.2.1/pytctracer/evaluation/classify_predictions.py
+-rw-rw-rw-   0        0        0     2808 2024-04-24 01:06:16.000000 pytctracer-0.2.1/pytctracer/evaluation/evaluate_predictions.py
+drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.529089 pytctracer-0.2.1/pytctracer/evaluation/metrics/
+-rw-rw-rw-   0        0        0      613 2024-03-30 00:46:46.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1581 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/area_under_curve.py
+-rw-rw-rw-   0        0        0     2967 2024-03-30 00:46:45.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py
+-rw-rw-rw-   0        0        0      914 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/f1.py
+-rw-rw-rw-   0        0        0      989 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/false_negatives.py
+-rw-rw-rw-   0        0        0      989 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/false_positives.py
+-rw-rw-rw-   0        0        0     1470 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/mean_average_precision.py
+-rw-rw-rw-   0        0        0      744 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/metric.py
+-rw-rw-rw-   0        0        0     1084 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/precision.py
+-rw-rw-rw-   0        0        0     1060 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/recall.py
+-rw-rw-rw-   0        0        0      995 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/true_positives.py
+drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.531101 pytctracer-0.2.1/pytctracer/io/
+-rw-rw-rw-   0        0        0        0 2024-03-30 00:46:30.000000 pytctracer-0.2.1/pytctracer/io/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.535129 pytctracer-0.2.1/pytctracer/io/input/
+-rw-rw-rw-   0        0        0      110 2024-03-30 00:46:37.000000 pytctracer-0.2.1/pytctracer/io/input/__init__.py
+-rw-rw-rw-   0        0        0     2336 2024-04-26 01:34:44.000000 pytctracer-0.2.1/pytctracer/io/input/from_file.py
+drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.541140 pytctracer-0.2.1/pytctracer/io/output/
+-rw-rw-rw-   0        0        0      367 2024-03-30 00:46:35.000000 pytctracer-0.2.1/pytctracer/io/output/__init__.py
+-rw-rw-rw-   0        0        0     3167 2024-04-24 01:02:45.000000 pytctracer-0.2.1/pytctracer/io/output/to_display.py
+-rw-rw-rw-   0        0        0     2372 2024-04-24 01:00:34.000000 pytctracer-0.2.1/pytctracer/io/output/to_file.py
+drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.552233 pytctracer-0.2.1/pytctracer/parsing/
+-rw-rw-rw-   0        0        0     1382 2024-03-30 00:46:28.000000 pytctracer-0.2.1/pytctracer/parsing/__init__.py
+-rw-rw-rw-   0        0        0     7243 2024-04-24 00:56:25.000000 pytctracer-0.2.1/pytctracer/parsing/find_class_level_calls.py
+-rw-rw-rw-   0        0        0     2124 2024-04-24 00:54:18.000000 pytctracer-0.2.1/pytctracer/parsing/find_class_level_names.py
+-rw-rw-rw-   0        0        0     6552 2024-04-24 00:53:40.000000 pytctracer-0.2.1/pytctracer/parsing/find_function_level_calls.py
+-rw-rw-rw-   0        0        0     2032 2024-04-24 00:51:05.000000 pytctracer-0.2.1/pytctracer/parsing/find_function_level_names.py
+-rw-rw-rw-   0        0        0     4285 2024-04-24 00:49:28.000000 pytctracer-0.2.1/pytctracer/parsing/functions_called_before_assert.py
+drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.567296 pytctracer-0.2.1/pytctracer/techniques/
+-rw-rw-rw-   0        0        0      883 2024-03-27 16:49:38.000000 pytctracer-0.2.1/pytctracer/techniques/__init__.py
+-rw-rw-rw-   0        0        0     4333 2024-04-24 00:24:31.000000 pytctracer-0.2.1/pytctracer/techniques/arg_name_to_technique_mapper.py
+-rw-rw-rw-   0        0        0     3510 2024-04-24 00:47:26.000000 pytctracer-0.2.1/pytctracer/techniques/combined.py
+-rw-rw-rw-   0        0        0     4021 2024-04-03 23:07:28.000000 pytctracer-0.2.1/pytctracer/techniques/last_call_before_assert.py
+-rw-rw-rw-   0        0        0     5118 2024-04-24 00:41:57.000000 pytctracer-0.2.1/pytctracer/techniques/levenshtein_distance.py
+-rw-rw-rw-   0        0        0    11089 2024-04-24 00:41:20.000000 pytctracer-0.2.1/pytctracer/techniques/longest_common_subsequence.py
+-rw-rw-rw-   0        0        0     6043 2024-04-24 00:40:03.000000 pytctracer-0.2.1/pytctracer/techniques/naming_conventions.py
+-rw-rw-rw-   0        0        0     4976 2024-04-24 00:39:20.000000 pytctracer-0.2.1/pytctracer/techniques/tarantula.py
+-rw-rw-rw-   0        0        0     6966 2024-04-24 00:44:46.000000 pytctracer-0.2.1/pytctracer/techniques/technique.py
+-rw-rw-rw-   0        0        0    11270 2024-04-24 00:36:56.000000 pytctracer-0.2.1/pytctracer/techniques/tfidf.py
+-rw-rw-rw-   0        0        0    21573 2024-04-24 01:38:40.000000 pytctracer-0.2.1/pytctracer/tracer.py
+drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.568296 pytctracer-0.2.1/pytctracer.egg-info/
+-rw-rw-rw-   0        0        0    17285 2024-04-26 01:47:12.000000 pytctracer-0.2.1/pytctracer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2634 2024-04-26 01:47:12.000000 pytctracer-0.2.1/pytctracer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 01:47:12.000000 pytctracer-0.2.1/pytctracer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-26 01:47:12.000000 pytctracer-0.2.1/pytctracer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      166 2024-04-26 01:47:12.000000 pytctracer-0.2.1/pytctracer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      101 2024-04-26 01:47:12.000000 pytctracer-0.2.1/pytctracer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 01:47:12.572296 pytctracer-0.2.1/setup.cfg
```

### Comparing `pytctracer-0.2.0/PKG-INFO` & `pytctracer-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytctracer
-Version: 0.2.0
+Version: 0.2.1
 Summary: Research library demonstrating test-to-code traceability techniques on Python codebases that use the Pytest testing framework.
 Author: Jason Ho
 Project-URL: Repository, https://github.com/jasonho2582001/comp0138-pytctracer
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
@@ -23,15 +23,14 @@
 Requires-Dist: bump2version==1.0.1; extra == "dev"
 
 # PyTCTracer
 PyTCTracer is a test-to-code traceability approach and library, which allows for dynamic code tracing of Python repositories using the Pytest testing framework, and automatic generation of test-to-code traceability links from the trace data using a number of established traceability techniques. 
 
 This library forms part of an undergraduate research project for a Masters of Engineering in Computer Science at UCL (University College London). PyTCTracer follows from TCTracer, which is an approach and implementation for test-to-code traceability for Java projects. This was developed by Robert White, Jens Krinke and Raymond Tan in 2020, and the research expanded on in 2022. The extended research paper introducing TCTracer can be found [here](https://link.springer.com/article/10.1007/s10664-021-10079-1).
 
-
 There are two core components in the library:
 - `PytestTracer`: A class that is used to trace the execution of Pytest unit tests and record dynamic tracing information to a CSV log file.
 - `pytctracer` CLI: A CLI tool which can read and parse the dynamic information from the log file, apply traceability techniques to generate link predictions, and evaluate the predictions against a ground truth.
 
 ## Installation
 PyTCTracer can be simply installed using pip:
 ```bash
```

### Comparing `pytctracer-0.2.0/README.md` & `pytctracer-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # PyTCTracer
 PyTCTracer is a test-to-code traceability approach and library, which allows for dynamic code tracing of Python repositories using the Pytest testing framework, and automatic generation of test-to-code traceability links from the trace data using a number of established traceability techniques. 
 
 This library forms part of an undergraduate research project for a Masters of Engineering in Computer Science at UCL (University College London). PyTCTracer follows from TCTracer, which is an approach and implementation for test-to-code traceability for Java projects. This was developed by Robert White, Jens Krinke and Raymond Tan in 2020, and the research expanded on in 2022. The extended research paper introducing TCTracer can be found [here](https://link.springer.com/article/10.1007/s10664-021-10079-1).
 
-
 There are two core components in the library:
 - `PytestTracer`: A class that is used to trace the execution of Pytest unit tests and record dynamic tracing information to a CSV log file.
 - `pytctracer` CLI: A CLI tool which can read and parse the dynamic information from the log file, apply traceability techniques to generate link predictions, and evaluate the predictions against a ground truth.
 
 ## Installation
 PyTCTracer can be simply installed using pip:
 ```bash
```

### Comparing `pytctracer-0.2.0/data/ground-truth-data/pyopenssl/pyopenssl_all_functions.py` & `pytctracer-0.2.1/data/ground-truth-data/pyopenssl/pyopenssl_all_functions.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/data/ground-truth-data/pyopenssl/pyopenssl_chosen_tests.py` & `pytctracer-0.2.1/data/ground-truth-data/pyopenssl/pyopenssl_chosen_tests.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/data/t.py` & `pytctracer-0.2.1/data/t.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/data/trace_parser_dynamic.py` & `pytctracer-0.2.1/data/trace_parser_dynamic.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pyproject.toml` & `pytctracer-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 authors = [
   {name = "Jason Ho"}
 ]
 description = """Research library demonstrating test-to-code traceability techniques on Python codebases that use the Pytest testing framework."""
 readme = "README.md"
 name = "pytctracer"
-version = "0.2.0"
+version = "0.2.1"
 classifiers=[
     "Natural Language :: English",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
```

### Comparing `pytctracer-0.2.0/pytctracer/analyser.py` & `pytctracer-0.2.1/pytctracer/analyser.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,92 +37,90 @@
     """
     def __init__(self) -> None:
         self.arg_name_to_technique_map = ArgNameToTechniqueMapper()
         self.arg_name_to_metric_map = ArgNameToMetricMapper()
         self.default_technique_names = Config.DEFAULT_CHOSEN_TECHNIQUE_NAMES
         self.default_metric_names = Config.DEFAULT_CHOSEN_METRIC_NAMES
 
-    def compare_traceability_links(
+    def produce_traceability_links_for_trace(
         self,
-        predicted_links_path: str,
-        ground_truth_path: str,
-        chosen_metric_names: Optional[List[str]] = None,
-        classifications_output_path: Optional[str] = None,
-        evaluation_metrics_output_path: Optional[str] = None,
-        display_classifications_to_stdout: bool = False,
-        metric_as_percentage: bool = False,
-    ) -> int:
-        predicted_links = load_link_json(predicted_links_path)
-        ground_truth_links = load_link_json(ground_truth_path)
-
-        self._check_ground_truth_tests_in_predicted_links(
-            predicted_links, ground_truth_links
+        trace_csv_log_path: str,
+        traceability_level: LevelType,
+        add_combined_technique: bool = False,
+        chosen_technique_names: Optional[List[str]] = None,
+        prediction_output_directory_path: Optional[str] = None,
+    ) -> None:
+        """
+        Produces traceability links for a given dynamic trace log. The
+        chosen technique names, whether to add a combined technique, the
+        level to produce links at, and an output output directory path can
+        be specified. If no directory is specified, the links are printed to
+        standard output.
+
+        Args:
+            trace_csv_log_path (str): The path to the dynamic trace log CSV file.
+            traceability_level (LevelType): The level of traceability to produce links for.
+            add_combined_technique (bool): Whether to produce links with the combined technique.
+            chosen_technique_names (Optional[List[str]]): The arg names of the techniques to use.
+            prediction_output_directory_path (Optional[str]): The directory to write the output links to.
+        """
+        if not chosen_technique_names:
+            chosen_technique_names = self.default_technique_names
+        _, link_predictions_for_techniques = self._predict_links(
+            trace_csv_log_path=trace_csv_log_path,
+            chosen_technique_names=chosen_technique_names,
+            traceability_level=traceability_level,
+            add_combined_technique=add_combined_technique,
         )
-
-        if not chosen_metric_names:
-            chosen_metric_names = self.default_metric_names
-
-        chosen_metrics = self._get_chosen_metric_classes(chosen_metric_names)
-
-        evaluation_metrics = {
-            predicted_links_path: evaluate_predictions(
-                predicted_links=predicted_links,
-                ground_truth_links=ground_truth_links,
-                selected_metrics=chosen_metrics,
-                metric_as_percentage=metric_as_percentage,
-                uses_threshold=False,
+        if not prediction_output_directory_path:
+            self._display_predicted_links_for_techniques(
+                link_predictions_for_techniques
             )
-        }
-
-        classifications = classify_predictions(
-            predicted_links=predicted_links, ground_truth_links=ground_truth_links
-        )
-
-        if display_classifications_to_stdout:
-            display_classifications(classifications, predicted_links_path)
-
-        display_evaluation_results(
-            evaluation_metric_dict=evaluation_metrics,
-            title=Config.EVALUATION_METRICS_TITLE,
-        )
-
-        if classifications_output_path:
-            write_dict_to_json(classifications, classifications_output_path)
-
-        if evaluation_metrics_output_path:
-            write_evaluation_metrics_to_csv(
-                combined_evaluation_dict=evaluation_metrics,
-                csv_name=evaluation_metrics_output_path,
+        else:
+            self._write_predicted_links_for_techniques(
+                link_predictions_for_techniques,
+                prediction_output_directory_path,
+                traceability_level,
             )
 
-    def _check_ground_truth_tests_in_predicted_links(
-        self,
-        predicted_links: Dict[str, List[str]],
-        ground_truth_links: Dict[str, List[str]],
-    ) -> None:
-        tests_in_predicted_links = set(predicted_links.keys())
-        for test in ground_truth_links:
-            if test not in tests_in_predicted_links:
-                raise ValueError(
-                    f"Test '{test}' in ground truth but not in predicted links"
-                )
-
     def evaluate_traceability_links_for_trace(
         self,
         trace_csv_log_path: str,
         ground_truth_path: str,
         traceability_level: LevelType,
         add_combined_technique: bool = False,
         chosen_technique_names: Optional[List[str]] = None,
         chosen_metric_names: Optional[List[str]] = None,
         classifications_output_directory_path: Optional[str] = None,
         evaluation_metrics_output_path: Optional[str] = None,
         display_classifications_to_stdout: bool = False,
         metric_as_percentage: bool = False,
-    ) -> int:
+    ) -> None:
+        """
+        Produces traceability links for a given dynamic trace log, and then
+        evaluates them against a specified ground truth. Allows for choosing 
+        the technique names to evaluate predictions for, the metric names to
+        compute, and whether to add a combined technique as well as output 
+        paths for the classifications and metrics. 
+
+        Args:
+            trace_csv_log_path (str): The path to the dynamic trace log CSV file.
+            ground_truth_path (str): The path to the ground truth JSON file.
+            traceability_level (LevelType): The level of traceability to produce links for.
+            add_combined_technique (bool): Whether to produce links with the combined technique.
+            chosen_technique_names (Optional[List[str]]): The arg names of the techniques to use.
+            chosen_metric_names (Optional[List[str]]): The arg names of the metrics to use.
+            classifications_output_directory_path (Optional[str]): The directory to write the output
+            classifications to.
+            evaluation_metrics_output_path (Optional[str]): The path to write the CSV containing the
+            evaluation metric results to.
+            display_classifications_to_stdout (bool): Whether to display the classifications to
+            standard output.
+            metric_as_percentage (bool): Whether to report metrics as percentages.
+        """
         if not chosen_technique_names:
             chosen_technique_names = self.default_technique_names
 
         if not chosen_metric_names:
             chosen_metric_names = self.default_metric_names
 
         ground_truth_links = load_link_json(ground_truth_path)
@@ -166,41 +164,96 @@
 
         if evaluation_metrics_output_path:
             write_evaluation_metrics_to_csv(
                 combined_evaluation_dict=evaluation_metrics_for_techniques,
                 csv_name=evaluation_metrics_output_path,
             )
 
-    def produce_traceability_links_for_trace(
+    def compare_traceability_links(
         self,
-        trace_csv_log_path: str,
-        traceability_level: LevelType,
-        add_combined_technique: bool = False,
-        chosen_technique_names: Optional[List[str]] = None,
-        prediction_output_directory_path: Optional[str] = None,
-    ) -> int:
-        if not chosen_technique_names:
-            chosen_technique_names = self.default_technique_names
-        _, link_predictions_for_techniques = self._predict_links(
-            trace_csv_log_path=trace_csv_log_path,
-            chosen_technique_names=chosen_technique_names,
-            traceability_level=traceability_level,
-            add_combined_technique=add_combined_technique,
+        predicted_links_path: str,
+        ground_truth_path: str,
+        chosen_metric_names: Optional[List[str]] = None,
+        classifications_output_path: Optional[str] = None,
+        evaluation_metrics_output_path: Optional[str] = None,
+        display_classifications_to_stdout: bool = False,
+        metric_as_percentage: bool = False,
+    ) -> None:
+        """
+        Compare a JSON of predicted traceability links against a JSON of ground truth links.
+        Allows for choosing the metric names to compute, and output paths for the classifications
+        and metrics.
+
+        Args:
+            predicted_links_path (str): The path to the JSON file containing the predicted links.
+            ground_truth_path (str): The path to the JSON file containing the ground truth links.
+            chosen_metric_names (Optional[List[str]]): The arg names of the metrics to use.
+            classifications_output_path (Optional[str]): The path to write the output classifications to.
+            evaluation_metrics_output_path (Optional[str]): The path to write the CSV containing the
+            evaluation metric results to.
+            display_classifications_to_stdout (bool): Whether to display the classifications to
+            standard output.
+            metric_as_percentage (bool): Whether to report metrics as percentages.
+        """
+        predicted_links = load_link_json(predicted_links_path)
+        ground_truth_links = load_link_json(ground_truth_path)
+
+        self._check_ground_truth_tests_in_predicted_links(
+            predicted_links, ground_truth_links
         )
-        if not prediction_output_directory_path:
-            self._display_predicted_links_for_techniques(
-                link_predictions_for_techniques
+
+        if not chosen_metric_names:
+            chosen_metric_names = self.default_metric_names
+
+        chosen_metrics = self._get_chosen_metric_classes(chosen_metric_names)
+
+        evaluation_metrics = {
+            predicted_links_path: evaluate_predictions(
+                predicted_links=predicted_links,
+                ground_truth_links=ground_truth_links,
+                selected_metrics=chosen_metrics,
+                metric_as_percentage=metric_as_percentage,
+                uses_threshold=False,
             )
-        else:
-            self._write_predicted_links_for_techniques(
-                link_predictions_for_techniques,
-                prediction_output_directory_path,
-                traceability_level,
+        }
+
+        classifications = classify_predictions(
+            predicted_links=predicted_links, ground_truth_links=ground_truth_links
+        )
+
+        if display_classifications_to_stdout:
+            display_classifications(classifications, predicted_links_path)
+
+        display_evaluation_results(
+            evaluation_metric_dict=evaluation_metrics,
+            title=Config.EVALUATION_METRICS_TITLE,
+        )
+
+        if classifications_output_path:
+            write_dict_to_json(classifications, classifications_output_path)
+
+        if evaluation_metrics_output_path:
+            write_evaluation_metrics_to_csv(
+                combined_evaluation_dict=evaluation_metrics,
+                csv_name=evaluation_metrics_output_path,
             )
 
+    def _check_ground_truth_tests_in_predicted_links(
+        self,
+        predicted_links: Dict[str, List[str]],
+        ground_truth_links: Dict[str, List[str]],
+    ) -> None:
+        tests_in_predicted_links = set(predicted_links.keys())
+        for test in ground_truth_links:
+            if test not in tests_in_predicted_links:
+                raise ValueError(
+                    f"Test '{test}' in ground truth but not in predicted links"
+                )
+
+
     def _write_classifications_for_techniques(
         self,
         classifications_for_techniques: Dict[str, Dict[str, List[str]]],
         classifications_output_directory_path: str,
         traceability_level: LevelType,
     ) -> None:
         for (
```

### Comparing `pytctracer-0.2.0/pytctracer/cli.py` & `pytctracer-0.2.1/pytctracer/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             trace_csv_log_path=trace_csv_log_path,
             traceability_level=level,
             add_combined_technique=add_combined,
             chosen_technique_names=chosen_technique_names,
             prediction_output_directory_path=output_directory,
         )
     except Exception as e:
-        click.ClickException(str(e))
+        raise click.ClickException(str(e))
 
 
 @cli.command(
     "evaluate-links",
     short_help="Produce and evaluate links against a ground truth.",
     help="""Produce and evaluate test-to-code traceability links against
     ground truth links for a given trace log CSV file, 
@@ -171,15 +171,15 @@
             chosen_technique_names=chosen_technique_names,
             chosen_metric_names=chosen_metric_names,
             classifications_output_directory_path=classifications_output_directory,
             display_classifications_to_stdout=display_classifications,
             evaluation_metrics_output_path=metrics_output_path,
         )
     except Exception as e:
-        click.ClickException(str(e))
+        raise click.ClickException(str(e))
 
 
 @cli.command(
     "compare-links",
     short_help="Compare a set of links against a ground truth.",
     help="""Compare a set of test-to-code traceability links against ground truth links
     using specified evaluation metrics.
@@ -236,11 +236,11 @@
             ground_truth_path=ground_truth_path,
             chosen_metric_names=chosen_metric_names,
             metric_as_percentage=as_percentage,
             classifications_output_path=classifications_output_path,
             evaluation_metrics_output_path=metrics_output_path,
         )
     except Exception as e:
-        click.ClickException(str(e))
+        raise click.ClickException(str(e))
 
 if __name__ == "__main__":
     cli()
```

### Comparing `pytctracer-0.2.0/pytctracer/config/config.py` & `pytctracer-0.2.1/pytctracer/config/config.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/config/constants/__init__.py` & `pytctracer-0.2.1/pytctracer/config/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/config/constants/technique_parameter.py` & `pytctracer-0.2.1/pytctracer/config/constants/technique_parameter.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/config/constants/technique_threshold.py` & `pytctracer-0.2.1/pytctracer/config/constants/technique_threshold.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/config/constants/trace_data_header.py` & `pytctracer-0.2.1/pytctracer/config/constants/trace_data_header.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/evaluation/classify_predictions.py` & `pytctracer-0.2.1/pytctracer/evaluation/classify_predictions.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/evaluation/evaluate_predictions.py` & `pytctracer-0.2.1/pytctracer/evaluation/evaluate_predictions.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/evaluation/metrics/__init__.py` & `pytctracer-0.2.1/pytctracer/evaluation/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/evaluation/metrics/area_under_curve.py` & `pytctracer-0.2.1/pytctracer/evaluation/metrics/area_under_curve.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py` & `pytctracer-0.2.1/pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/evaluation/metrics/f1.py` & `pytctracer-0.2.1/pytctracer/evaluation/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/evaluation/metrics/false_negatives.py` & `pytctracer-0.2.1/pytctracer/evaluation/metrics/false_negatives.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/evaluation/metrics/false_positives.py` & `pytctracer-0.2.1/pytctracer/evaluation/metrics/false_positives.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/evaluation/metrics/mean_average_precision.py` & `pytctracer-0.2.1/pytctracer/evaluation/metrics/mean_average_precision.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/evaluation/metrics/metric.py` & `pytctracer-0.2.1/pytctracer/evaluation/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/evaluation/metrics/precision.py` & `pytctracer-0.2.1/pytctracer/evaluation/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/evaluation/metrics/recall.py` & `pytctracer-0.2.1/pytctracer/evaluation/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/evaluation/metrics/true_positives.py` & `pytctracer-0.2.1/pytctracer/evaluation/metrics/true_positives.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/io/input/from_file.py` & `pytctracer-0.2.1/pytctracer/io/input/from_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         a row in the CSV file, with the keys being the column names and the values
         being the corresponding values in the row.
     """
     data = []
     try:
         with open(file_path, encoding="utf8") as file:
             lines = csv.reader(file)
-
             # Iterate through each line in the CSV file, extract the fields
             for index, record in enumerate(lines):
                 # Extract column names from first row
                 if index == 0:
                     columns = record
                     continue
                 data.append({columns[i]: record[i] for i in range(len(columns))})
```

### Comparing `pytctracer-0.2.0/pytctracer/io/output/to_display.py` & `pytctracer-0.2.1/pytctracer/io/output/to_display.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/io/output/to_file.py` & `pytctracer-0.2.1/pytctracer/io/output/to_file.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/parsing/__init__.py` & `pytctracer-0.2.1/pytctracer/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/parsing/find_class_level_calls.py` & `pytctracer-0.2.1/pytctracer/parsing/find_class_level_calls.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/parsing/find_class_level_names.py` & `pytctracer-0.2.1/pytctracer/parsing/find_class_level_names.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/parsing/find_function_level_calls.py` & `pytctracer-0.2.1/pytctracer/parsing/find_function_level_calls.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/parsing/find_function_level_names.py` & `pytctracer-0.2.1/pytctracer/parsing/find_function_level_names.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/parsing/functions_called_before_assert.py` & `pytctracer-0.2.1/pytctracer/parsing/functions_called_before_assert.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/techniques/__init__.py` & `pytctracer-0.2.1/pytctracer/techniques/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/techniques/arg_name_to_technique_mapper.py` & `pytctracer-0.2.1/pytctracer/techniques/arg_name_to_technique_mapper.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/techniques/combined.py` & `pytctracer-0.2.1/pytctracer/techniques/combined.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/techniques/last_call_before_assert.py` & `pytctracer-0.2.1/pytctracer/techniques/last_call_before_assert.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/techniques/levenshtein_distance.py` & `pytctracer-0.2.1/pytctracer/techniques/levenshtein_distance.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/techniques/longest_common_subsequence.py` & `pytctracer-0.2.1/pytctracer/techniques/longest_common_subsequence.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/techniques/naming_conventions.py` & `pytctracer-0.2.1/pytctracer/techniques/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/techniques/tarantula.py` & `pytctracer-0.2.1/pytctracer/techniques/tarantula.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/techniques/technique.py` & `pytctracer-0.2.1/pytctracer/techniques/technique.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/techniques/tfidf.py` & `pytctracer-0.2.1/pytctracer/techniques/tfidf.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer/tracer.py` & `pytctracer-0.2.1/pytctracer/tracer.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.0/pytctracer.egg-info/PKG-INFO` & `pytctracer-0.2.1/pytctracer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytctracer
-Version: 0.2.0
+Version: 0.2.1
 Summary: Research library demonstrating test-to-code traceability techniques on Python codebases that use the Pytest testing framework.
 Author: Jason Ho
 Project-URL: Repository, https://github.com/jasonho2582001/comp0138-pytctracer
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
@@ -23,15 +23,14 @@
 Requires-Dist: bump2version==1.0.1; extra == "dev"
 
 # PyTCTracer
 PyTCTracer is a test-to-code traceability approach and library, which allows for dynamic code tracing of Python repositories using the Pytest testing framework, and automatic generation of test-to-code traceability links from the trace data using a number of established traceability techniques. 
 
 This library forms part of an undergraduate research project for a Masters of Engineering in Computer Science at UCL (University College London). PyTCTracer follows from TCTracer, which is an approach and implementation for test-to-code traceability for Java projects. This was developed by Robert White, Jens Krinke and Raymond Tan in 2020, and the research expanded on in 2022. The extended research paper introducing TCTracer can be found [here](https://link.springer.com/article/10.1007/s10664-021-10079-1).
 
-
 There are two core components in the library:
 - `PytestTracer`: A class that is used to trace the execution of Pytest unit tests and record dynamic tracing information to a CSV log file.
 - `pytctracer` CLI: A CLI tool which can read and parse the dynamic information from the log file, apply traceability techniques to generate link predictions, and evaluate the predictions against a ground truth.
 
 ## Installation
 PyTCTracer can be simply installed using pip:
 ```bash
```

### Comparing `pytctracer-0.2.0/pytctracer.egg-info/SOURCES.txt` & `pytctracer-0.2.1/pytctracer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

