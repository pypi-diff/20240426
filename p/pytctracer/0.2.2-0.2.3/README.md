# Comparing `tmp/pytctracer-0.2.2.tar.gz` & `tmp/pytctracer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytctracer-0.2.2.tar", last modified: Fri Apr 26 02:44:59 2024, max compression
+gzip compressed data, was "pytctracer-0.2.3.tar", last modified: Fri Apr 26 03:58:18 2024, max compression
```

## Comparing `pytctracer-0.2.2.tar` & `pytctracer-0.2.3.tar`

### file list

```diff
@@ -1,84 +1,76 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.959673 pytctracer-0.2.2/
--rw-rw-rw-   0        0        0    17285 2024-04-26 02:44:59.957673 pytctracer-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    16291 2024-04-26 01:45:21.000000 pytctracer-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.834769 pytctracer-0.2.2/data/
-drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.821139 pytctracer-0.2.2/data/ground-truth-data/
-drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.838776 pytctracer-0.2.2/data/ground-truth-data/pyopenssl/
--rw-rw-rw-   0        0        0    14927 2023-12-12 17:26:56.000000 pytctracer-0.2.2/data/ground-truth-data/pyopenssl/pyopenssl_all_functions.py
--rw-rw-rw-   0        0        0     2737 2024-01-17 14:14:19.000000 pytctracer-0.2.2/data/ground-truth-data/pyopenssl/pyopenssl_chosen_tests.py
--rw-rw-rw-   0        0        0     2195 2024-04-09 23:53:27.000000 pytctracer-0.2.2/data/t.py
--rw-rw-rw-   0        0        0      464 2024-02-25 02:21:54.000000 pytctracer-0.2.2/data/tes.py
--rw-rw-rw-   0        0        0    81858 2024-04-26 02:23:42.000000 pytctracer-0.2.2/data/trace_parser_dynamic.py
--rw-rw-rw-   0        0        0     1045 2024-04-26 02:44:32.000000 pytctracer-0.2.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.845410 pytctracer-0.2.2/pytctracer/
--rw-rw-rw-   0        0        0      104 2024-03-31 18:38:21.000000 pytctracer-0.2.2/pytctracer/__init__.py
--rw-rw-rw-   0        0        0    22577 2024-04-26 02:42:32.000000 pytctracer-0.2.2/pytctracer/analyser.py
--rw-rw-rw-   0        0        0     9141 2024-04-26 02:42:31.000000 pytctracer-0.2.2/pytctracer/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.890238 pytctracer-0.2.2/pytctracer/config/
--rw-rw-rw-   0        0        0       49 2024-03-30 00:46:49.000000 pytctracer-0.2.2/pytctracer/config/__init__.py
--rw-rw-rw-   0        0        0     1103 2024-04-26 02:42:31.000000 pytctracer-0.2.2/pytctracer/config/config.py
-drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.904814 pytctracer-0.2.2/pytctracer/config/constants/
--rw-rw-rw-   0        0        0      904 2024-04-03 23:07:54.000000 pytctracer-0.2.2/pytctracer/config/constants/__init__.py
--rw-rw-rw-   0        0        0      180 2024-04-03 23:05:28.000000 pytctracer-0.2.2/pytctracer/config/constants/classification_type.py
--rw-rw-rw-   0        0        0      380 2024-04-03 23:05:47.000000 pytctracer-0.2.2/pytctracer/config/constants/event_type.py
--rw-rw-rw-   0        0        0      216 2024-04-03 23:05:58.000000 pytctracer-0.2.2/pytctracer/config/constants/function_type.py
--rw-rw-rw-   0        0        0      129 2024-04-03 23:06:06.000000 pytctracer-0.2.2/pytctracer/config/constants/instruction_opname.py
--rw-rw-rw-   0        0        0       99 2024-04-03 23:07:08.000000 pytctracer-0.2.2/pytctracer/config/constants/level_type.py
--rw-rw-rw-   0        0        0      202 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/config/constants/metric_score_type.py
--rw-rw-rw-   0        0        0      535 2024-04-03 23:07:28.000000 pytctracer-0.2.2/pytctracer/config/constants/technique_parameter.py
--rw-rw-rw-   0        0        0     1014 2024-04-26 02:42:32.000000 pytctracer-0.2.2/pytctracer/config/constants/technique_threshold.py
--rw-rw-rw-   0        0        0      149 2024-04-03 23:07:44.000000 pytctracer-0.2.2/pytctracer/config/constants/testing_method_event_type.py
--rw-rw-rw-   0        0        0      572 2024-04-03 23:07:50.000000 pytctracer-0.2.2/pytctracer/config/constants/trace_data_header.py
--rw-rw-rw-   0        0        0      507 2024-04-03 23:07:54.000000 pytctracer-0.2.2/pytctracer/config/constants/trace_data_variable.py
-drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.909408 pytctracer-0.2.2/pytctracer/evaluation/
--rw-rw-rw-   0        0        0      170 2024-03-26 14:14:33.000000 pytctracer-0.2.2/pytctracer/evaluation/__init__.py
--rw-rw-rw-   0        0        0     2350 2024-04-26 02:42:31.000000 pytctracer-0.2.2/pytctracer/evaluation/classify_predictions.py
--rw-rw-rw-   0        0        0     2804 2024-04-26 02:42:31.000000 pytctracer-0.2.2/pytctracer/evaluation/evaluate_predictions.py
-drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.924377 pytctracer-0.2.2/pytctracer/evaluation/metrics/
--rw-rw-rw-   0        0        0      613 2024-03-30 00:46:46.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/__init__.py
--rw-rw-rw-   0        0        0     1581 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/area_under_curve.py
--rw-rw-rw-   0        0        0     2967 2024-03-30 00:46:45.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py
--rw-rw-rw-   0        0        0      914 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/f1.py
--rw-rw-rw-   0        0        0      989 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/false_negatives.py
--rw-rw-rw-   0        0        0      989 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/false_positives.py
--rw-rw-rw-   0        0        0     1470 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/mean_average_precision.py
--rw-rw-rw-   0        0        0      744 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/metric.py
--rw-rw-rw-   0        0        0     1084 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/precision.py
--rw-rw-rw-   0        0        0     1060 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/recall.py
--rw-rw-rw-   0        0        0      995 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/true_positives.py
-drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.925583 pytctracer-0.2.2/pytctracer/io/
--rw-rw-rw-   0        0        0        0 2024-03-30 00:46:30.000000 pytctracer-0.2.2/pytctracer/io/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.928591 pytctracer-0.2.2/pytctracer/io/input/
--rw-rw-rw-   0        0        0      110 2024-03-30 00:46:37.000000 pytctracer-0.2.2/pytctracer/io/input/__init__.py
--rw-rw-rw-   0        0        0     2372 2024-04-26 02:42:31.000000 pytctracer-0.2.2/pytctracer/io/input/from_file.py
-drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.932591 pytctracer-0.2.2/pytctracer/io/output/
--rw-rw-rw-   0        0        0      367 2024-03-30 00:46:35.000000 pytctracer-0.2.2/pytctracer/io/output/__init__.py
--rw-rw-rw-   0        0        0     3167 2024-04-24 01:02:45.000000 pytctracer-0.2.2/pytctracer/io/output/to_display.py
--rw-rw-rw-   0        0        0     2455 2024-04-26 02:42:31.000000 pytctracer-0.2.2/pytctracer/io/output/to_file.py
-drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.940619 pytctracer-0.2.2/pytctracer/parsing/
--rw-rw-rw-   0        0        0     1382 2024-03-30 00:46:28.000000 pytctracer-0.2.2/pytctracer/parsing/__init__.py
--rw-rw-rw-   0        0        0     7226 2024-04-26 02:42:32.000000 pytctracer-0.2.2/pytctracer/parsing/find_class_level_calls.py
--rw-rw-rw-   0        0        0     2120 2024-04-26 02:42:31.000000 pytctracer-0.2.2/pytctracer/parsing/find_class_level_names.py
--rw-rw-rw-   0        0        0     6548 2024-04-26 02:42:32.000000 pytctracer-0.2.2/pytctracer/parsing/find_function_level_calls.py
--rw-rw-rw-   0        0        0     2022 2024-04-26 02:42:31.000000 pytctracer-0.2.2/pytctracer/parsing/find_function_level_names.py
--rw-rw-rw-   0        0        0     4273 2024-04-26 02:42:31.000000 pytctracer-0.2.2/pytctracer/parsing/functions_called_before_assert.py
-drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.954652 pytctracer-0.2.2/pytctracer/techniques/
--rw-rw-rw-   0        0        0      883 2024-03-27 16:49:38.000000 pytctracer-0.2.2/pytctracer/techniques/__init__.py
--rw-rw-rw-   0        0        0     4325 2024-04-26 02:42:32.000000 pytctracer-0.2.2/pytctracer/techniques/arg_name_to_technique_mapper.py
--rw-rw-rw-   0        0        0     3479 2024-04-26 02:42:32.000000 pytctracer-0.2.2/pytctracer/techniques/combined.py
--rw-rw-rw-   0        0        0     4021 2024-04-03 23:07:28.000000 pytctracer-0.2.2/pytctracer/techniques/last_call_before_assert.py
--rw-rw-rw-   0        0        0     5118 2024-04-24 00:41:57.000000 pytctracer-0.2.2/pytctracer/techniques/levenshtein_distance.py
--rw-rw-rw-   0        0        0    11089 2024-04-24 00:41:20.000000 pytctracer-0.2.2/pytctracer/techniques/longest_common_subsequence.py
--rw-rw-rw-   0        0        0     6043 2024-04-24 00:40:03.000000 pytctracer-0.2.2/pytctracer/techniques/naming_conventions.py
--rw-rw-rw-   0        0        0     4976 2024-04-24 00:39:20.000000 pytctracer-0.2.2/pytctracer/techniques/tarantula.py
--rw-rw-rw-   0        0        0     6954 2024-04-26 02:42:32.000000 pytctracer-0.2.2/pytctracer/techniques/technique.py
--rw-rw-rw-   0        0        0    11270 2024-04-24 00:36:56.000000 pytctracer-0.2.2/pytctracer/techniques/tfidf.py
--rw-rw-rw-   0        0        0    21533 2024-04-26 02:42:32.000000 pytctracer-0.2.2/pytctracer/tracer.py
-drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.956666 pytctracer-0.2.2/pytctracer.egg-info/
--rw-rw-rw-   0        0        0    17285 2024-04-26 02:44:59.000000 pytctracer-0.2.2/pytctracer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2634 2024-04-26 02:44:59.000000 pytctracer-0.2.2/pytctracer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 02:44:59.000000 pytctracer-0.2.2/pytctracer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-26 02:44:59.000000 pytctracer-0.2.2/pytctracer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      166 2024-04-26 02:44:59.000000 pytctracer-0.2.2/pytctracer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       43 2024-04-26 02:44:59.000000 pytctracer-0.2.2/pytctracer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 02:44:59.959673 pytctracer-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 03:58:18.788729 pytctracer-0.2.3/
+-rw-rw-rw-   0        0        0    17285 2024-04-26 03:58:18.780728 pytctracer-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    16291 2024-04-26 01:45:21.000000 pytctracer-0.2.3/README.md
+-rw-rw-rw-   0        0        0     1045 2024-04-26 03:57:50.000000 pytctracer-0.2.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-26 03:58:18.416129 pytctracer-0.2.3/pytctracer/
+-rw-rw-rw-   0        0        0      104 2024-03-31 18:38:21.000000 pytctracer-0.2.3/pytctracer/__init__.py
+-rw-rw-rw-   0        0        0    22577 2024-04-26 02:42:32.000000 pytctracer-0.2.3/pytctracer/analyser.py
+-rw-rw-rw-   0        0        0     9141 2024-04-26 02:42:31.000000 pytctracer-0.2.3/pytctracer/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:58:18.484129 pytctracer-0.2.3/pytctracer/config/
+-rw-rw-rw-   0        0        0       49 2024-03-30 00:46:49.000000 pytctracer-0.2.3/pytctracer/config/__init__.py
+-rw-rw-rw-   0        0        0     1103 2024-04-26 02:42:31.000000 pytctracer-0.2.3/pytctracer/config/config.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:58:18.516657 pytctracer-0.2.3/pytctracer/config/constants/
+-rw-rw-rw-   0        0        0      904 2024-04-03 23:07:54.000000 pytctracer-0.2.3/pytctracer/config/constants/__init__.py
+-rw-rw-rw-   0        0        0      180 2024-04-03 23:05:28.000000 pytctracer-0.2.3/pytctracer/config/constants/classification_type.py
+-rw-rw-rw-   0        0        0      380 2024-04-03 23:05:47.000000 pytctracer-0.2.3/pytctracer/config/constants/event_type.py
+-rw-rw-rw-   0        0        0      216 2024-04-03 23:05:58.000000 pytctracer-0.2.3/pytctracer/config/constants/function_type.py
+-rw-rw-rw-   0        0        0      129 2024-04-03 23:06:06.000000 pytctracer-0.2.3/pytctracer/config/constants/instruction_opname.py
+-rw-rw-rw-   0        0        0       99 2024-04-03 23:07:08.000000 pytctracer-0.2.3/pytctracer/config/constants/level_type.py
+-rw-rw-rw-   0        0        0      202 2024-04-03 23:07:13.000000 pytctracer-0.2.3/pytctracer/config/constants/metric_score_type.py
+-rw-rw-rw-   0        0        0      535 2024-04-03 23:07:28.000000 pytctracer-0.2.3/pytctracer/config/constants/technique_parameter.py
+-rw-rw-rw-   0        0        0     1014 2024-04-26 02:42:32.000000 pytctracer-0.2.3/pytctracer/config/constants/technique_threshold.py
+-rw-rw-rw-   0        0        0      149 2024-04-03 23:07:44.000000 pytctracer-0.2.3/pytctracer/config/constants/testing_method_event_type.py
+-rw-rw-rw-   0        0        0      572 2024-04-03 23:07:50.000000 pytctracer-0.2.3/pytctracer/config/constants/trace_data_header.py
+-rw-rw-rw-   0        0        0      507 2024-04-03 23:07:54.000000 pytctracer-0.2.3/pytctracer/config/constants/trace_data_variable.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:58:18.523656 pytctracer-0.2.3/pytctracer/evaluation/
+-rw-rw-rw-   0        0        0      170 2024-03-26 14:14:33.000000 pytctracer-0.2.3/pytctracer/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     2350 2024-04-26 02:42:31.000000 pytctracer-0.2.3/pytctracer/evaluation/classify_predictions.py
+-rw-rw-rw-   0        0        0     2804 2024-04-26 02:42:31.000000 pytctracer-0.2.3/pytctracer/evaluation/evaluate_predictions.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:58:18.691200 pytctracer-0.2.3/pytctracer/evaluation/metrics/
+-rw-rw-rw-   0        0        0      613 2024-03-30 00:46:46.000000 pytctracer-0.2.3/pytctracer/evaluation/metrics/__init__.py
+-rw-rw-rw-   0        0        0     3048 2024-04-26 03:57:16.000000 pytctracer-0.2.3/pytctracer/evaluation/metrics/area_under_curve.py
+-rw-rw-rw-   0        0        0     4165 2024-04-26 03:55:20.000000 pytctracer-0.2.3/pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py
+-rw-rw-rw-   0        0        0     1728 2024-04-26 03:53:52.000000 pytctracer-0.2.3/pytctracer/evaluation/metrics/f1.py
+-rw-rw-rw-   0        0        0     1972 2024-04-26 03:53:31.000000 pytctracer-0.2.3/pytctracer/evaluation/metrics/false_negatives.py
+-rw-rw-rw-   0        0        0     1967 2024-04-26 03:52:33.000000 pytctracer-0.2.3/pytctracer/evaluation/metrics/false_positives.py
+-rw-rw-rw-   0        0        0     2371 2024-04-26 03:51:40.000000 pytctracer-0.2.3/pytctracer/evaluation/metrics/mean_average_precision.py
+-rw-rw-rw-   0        0        0     2688 2024-04-26 03:46:45.000000 pytctracer-0.2.3/pytctracer/evaluation/metrics/metric.py
+-rw-rw-rw-   0        0        0     1935 2024-04-26 03:51:00.000000 pytctracer-0.2.3/pytctracer/evaluation/metrics/precision.py
+-rw-rw-rw-   0        0        0     1886 2024-04-26 03:50:34.000000 pytctracer-0.2.3/pytctracer/evaluation/metrics/recall.py
+-rw-rw-rw-   0        0        0     1971 2024-04-26 03:49:36.000000 pytctracer-0.2.3/pytctracer/evaluation/metrics/true_positives.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:58:18.693201 pytctracer-0.2.3/pytctracer/io/
+-rw-rw-rw-   0        0        0        0 2024-03-30 00:46:30.000000 pytctracer-0.2.3/pytctracer/io/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:58:18.699208 pytctracer-0.2.3/pytctracer/io/input/
+-rw-rw-rw-   0        0        0      110 2024-03-30 00:46:37.000000 pytctracer-0.2.3/pytctracer/io/input/__init__.py
+-rw-rw-rw-   0        0        0     2372 2024-04-26 02:42:31.000000 pytctracer-0.2.3/pytctracer/io/input/from_file.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:58:18.707212 pytctracer-0.2.3/pytctracer/io/output/
+-rw-rw-rw-   0        0        0      367 2024-03-30 00:46:35.000000 pytctracer-0.2.3/pytctracer/io/output/__init__.py
+-rw-rw-rw-   0        0        0     3167 2024-04-24 01:02:45.000000 pytctracer-0.2.3/pytctracer/io/output/to_display.py
+-rw-rw-rw-   0        0        0     2455 2024-04-26 02:42:31.000000 pytctracer-0.2.3/pytctracer/io/output/to_file.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:58:18.723734 pytctracer-0.2.3/pytctracer/parsing/
+-rw-rw-rw-   0        0        0     1382 2024-03-30 00:46:28.000000 pytctracer-0.2.3/pytctracer/parsing/__init__.py
+-rw-rw-rw-   0        0        0     7226 2024-04-26 02:42:32.000000 pytctracer-0.2.3/pytctracer/parsing/find_class_level_calls.py
+-rw-rw-rw-   0        0        0     2120 2024-04-26 02:42:31.000000 pytctracer-0.2.3/pytctracer/parsing/find_class_level_names.py
+-rw-rw-rw-   0        0        0     6548 2024-04-26 02:42:32.000000 pytctracer-0.2.3/pytctracer/parsing/find_function_level_calls.py
+-rw-rw-rw-   0        0        0     2022 2024-04-26 02:42:31.000000 pytctracer-0.2.3/pytctracer/parsing/find_function_level_names.py
+-rw-rw-rw-   0        0        0     4273 2024-04-26 02:42:31.000000 pytctracer-0.2.3/pytctracer/parsing/functions_called_before_assert.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:58:18.770731 pytctracer-0.2.3/pytctracer/techniques/
+-rw-rw-rw-   0        0        0      883 2024-03-27 16:49:38.000000 pytctracer-0.2.3/pytctracer/techniques/__init__.py
+-rw-rw-rw-   0        0        0     4325 2024-04-26 02:42:32.000000 pytctracer-0.2.3/pytctracer/techniques/arg_name_to_technique_mapper.py
+-rw-rw-rw-   0        0        0     3479 2024-04-26 02:42:32.000000 pytctracer-0.2.3/pytctracer/techniques/combined.py
+-rw-rw-rw-   0        0        0     4021 2024-04-03 23:07:28.000000 pytctracer-0.2.3/pytctracer/techniques/last_call_before_assert.py
+-rw-rw-rw-   0        0        0     5118 2024-04-24 00:41:57.000000 pytctracer-0.2.3/pytctracer/techniques/levenshtein_distance.py
+-rw-rw-rw-   0        0        0    11089 2024-04-24 00:41:20.000000 pytctracer-0.2.3/pytctracer/techniques/longest_common_subsequence.py
+-rw-rw-rw-   0        0        0     6043 2024-04-24 00:40:03.000000 pytctracer-0.2.3/pytctracer/techniques/naming_conventions.py
+-rw-rw-rw-   0        0        0     4976 2024-04-24 00:39:20.000000 pytctracer-0.2.3/pytctracer/techniques/tarantula.py
+-rw-rw-rw-   0        0        0     6954 2024-04-26 02:42:32.000000 pytctracer-0.2.3/pytctracer/techniques/technique.py
+-rw-rw-rw-   0        0        0    11270 2024-04-24 00:36:56.000000 pytctracer-0.2.3/pytctracer/techniques/tfidf.py
+-rw-rw-rw-   0        0        0    21533 2024-04-26 02:42:32.000000 pytctracer-0.2.3/pytctracer/tracer.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:58:18.774730 pytctracer-0.2.3/pytctracer.egg-info/
+-rw-rw-rw-   0        0        0    17285 2024-04-26 03:58:18.000000 pytctracer-0.2.3/pytctracer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2464 2024-04-26 03:58:18.000000 pytctracer-0.2.3/pytctracer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 03:58:18.000000 pytctracer-0.2.3/pytctracer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-26 03:58:18.000000 pytctracer-0.2.3/pytctracer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      166 2024-04-26 03:58:18.000000 pytctracer-0.2.3/pytctracer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2024-04-26 03:58:18.000000 pytctracer-0.2.3/pytctracer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 03:58:18.794730 pytctracer-0.2.3/setup.cfg
```

### Comparing `pytctracer-0.2.2/PKG-INFO` & `pytctracer-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytctracer
-Version: 0.2.2
+Version: 0.2.3
 Summary: Research library demonstrating test-to-code traceability techniques on Python codebases that use the Pytest testing framework.
 Author: Jason Ho
 Project-URL: Repository, https://github.com/jasonho2582001/comp0138-pytctracer
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pytctracer-0.2.2/README.md` & `pytctracer-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pyproject.toml` & `pytctracer-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 authors = [
   {name = "Jason Ho"}
 ]
 description = """Research library demonstrating test-to-code traceability techniques on Python codebases that use the Pytest testing framework."""
 readme = "README.md"
 name = "pytctracer"
-version = "0.2.2"
+version = "0.2.3"
 classifiers=[
     "Natural Language :: English",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
```

### Comparing `pytctracer-0.2.2/pytctracer/analyser.py` & `pytctracer-0.2.3/pytctracer/analyser.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/cli.py` & `pytctracer-0.2.3/pytctracer/cli.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/config/config.py` & `pytctracer-0.2.3/pytctracer/config/config.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/config/constants/__init__.py` & `pytctracer-0.2.3/pytctracer/config/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/config/constants/technique_parameter.py` & `pytctracer-0.2.3/pytctracer/config/constants/technique_parameter.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/config/constants/technique_threshold.py` & `pytctracer-0.2.3/pytctracer/config/constants/technique_threshold.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/config/constants/trace_data_header.py` & `pytctracer-0.2.3/pytctracer/config/constants/trace_data_header.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/evaluation/classify_predictions.py` & `pytctracer-0.2.3/pytctracer/evaluation/classify_predictions.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/evaluation/evaluate_predictions.py` & `pytctracer-0.2.3/pytctracer/evaluation/evaluate_predictions.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/evaluation/metrics/__init__.py` & `pytctracer-0.2.3/pytctracer/evaluation/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/io/input/from_file.py` & `pytctracer-0.2.3/pytctracer/io/input/from_file.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/io/output/to_display.py` & `pytctracer-0.2.3/pytctracer/io/output/to_display.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/io/output/to_file.py` & `pytctracer-0.2.3/pytctracer/io/output/to_file.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/parsing/__init__.py` & `pytctracer-0.2.3/pytctracer/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/parsing/find_class_level_calls.py` & `pytctracer-0.2.3/pytctracer/parsing/find_class_level_calls.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/parsing/find_class_level_names.py` & `pytctracer-0.2.3/pytctracer/parsing/find_class_level_names.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/parsing/find_function_level_calls.py` & `pytctracer-0.2.3/pytctracer/parsing/find_function_level_calls.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/parsing/find_function_level_names.py` & `pytctracer-0.2.3/pytctracer/parsing/find_function_level_names.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/parsing/functions_called_before_assert.py` & `pytctracer-0.2.3/pytctracer/parsing/functions_called_before_assert.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/techniques/__init__.py` & `pytctracer-0.2.3/pytctracer/techniques/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/techniques/arg_name_to_technique_mapper.py` & `pytctracer-0.2.3/pytctracer/techniques/arg_name_to_technique_mapper.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/techniques/combined.py` & `pytctracer-0.2.3/pytctracer/techniques/combined.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/techniques/last_call_before_assert.py` & `pytctracer-0.2.3/pytctracer/techniques/last_call_before_assert.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/techniques/levenshtein_distance.py` & `pytctracer-0.2.3/pytctracer/techniques/levenshtein_distance.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/techniques/longest_common_subsequence.py` & `pytctracer-0.2.3/pytctracer/techniques/longest_common_subsequence.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/techniques/naming_conventions.py` & `pytctracer-0.2.3/pytctracer/techniques/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/techniques/tarantula.py` & `pytctracer-0.2.3/pytctracer/techniques/tarantula.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/techniques/technique.py` & `pytctracer-0.2.3/pytctracer/techniques/technique.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/techniques/tfidf.py` & `pytctracer-0.2.3/pytctracer/techniques/tfidf.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer/tracer.py` & `pytctracer-0.2.3/pytctracer/tracer.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.2/pytctracer.egg-info/PKG-INFO` & `pytctracer-0.2.3/pytctracer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytctracer
-Version: 0.2.2
+Version: 0.2.3
 Summary: Research library demonstrating test-to-code traceability techniques on Python codebases that use the Pytest testing framework.
 Author: Jason Ho
 Project-URL: Repository, https://github.com/jasonho2582001/comp0138-pytctracer
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pytctracer-0.2.2/pytctracer.egg-info/SOURCES.txt` & `pytctracer-0.2.3/pytctracer.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 README.md
 pyproject.toml
-data/t.py
-data/tes.py
-data/trace_parser_dynamic.py
-data/ground-truth-data/pyopenssl/pyopenssl_all_functions.py
-data/ground-truth-data/pyopenssl/pyopenssl_chosen_tests.py
 pytctracer/__init__.py
 pytctracer/analyser.py
 pytctracer/cli.py
 pytctracer/tracer.py
 pytctracer.egg-info/PKG-INFO
 pytctracer.egg-info/SOURCES.txt
 pytctracer.egg-info/dependency_links.txt
```

