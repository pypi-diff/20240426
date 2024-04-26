# Comparing `tmp/pytctracer-0.2.1.tar.gz` & `tmp/pytctracer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytctracer-0.2.1.tar", last modified: Fri Apr 26 01:47:12 2024, max compression
+gzip compressed data, was "pytctracer-0.2.2.tar", last modified: Fri Apr 26 02:44:59 2024, max compression
```

## Comparing `pytctracer-0.2.1.tar` & `pytctracer-0.2.2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.572296 pytctracer-0.2.1/
--rw-rw-rw-   0        0        0    17285 2024-04-26 01:47:12.570299 pytctracer-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    16291 2024-04-26 01:45:21.000000 pytctracer-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.419804 pytctracer-0.2.1/data/
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.408037 pytctracer-0.2.1/data/ground-truth-data/
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.423313 pytctracer-0.2.1/data/ground-truth-data/pyopenssl/
--rw-rw-rw-   0        0        0    14927 2023-12-12 17:26:56.000000 pytctracer-0.2.1/data/ground-truth-data/pyopenssl/pyopenssl_all_functions.py
--rw-rw-rw-   0        0        0     2737 2024-01-17 14:14:19.000000 pytctracer-0.2.1/data/ground-truth-data/pyopenssl/pyopenssl_chosen_tests.py
--rw-rw-rw-   0        0        0     2195 2024-04-09 23:53:27.000000 pytctracer-0.2.1/data/t.py
--rw-rw-rw-   0        0        0      464 2024-02-25 02:21:54.000000 pytctracer-0.2.1/data/tes.py
--rw-rw-rw-   0        0        0    81882 2024-04-10 01:44:54.000000 pytctracer-0.2.1/data/trace_parser_dynamic.py
--rw-rw-rw-   0        0        0     1045 2024-04-26 01:46:22.000000 pytctracer-0.2.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.439552 pytctracer-0.2.1/pytctracer/
--rw-rw-rw-   0        0        0      104 2024-03-31 18:38:21.000000 pytctracer-0.2.1/pytctracer/__init__.py
--rw-rw-rw-   0        0        0    22580 2024-04-26 01:41:25.000000 pytctracer-0.2.1/pytctracer/analyser.py
--rw-rw-rw-   0        0        0     9139 2024-04-26 01:35:00.000000 pytctracer-0.2.1/pytctracer/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.471716 pytctracer-0.2.1/pytctracer/config/
--rw-rw-rw-   0        0        0       49 2024-03-30 00:46:49.000000 pytctracer-0.2.1/pytctracer/config/__init__.py
--rw-rw-rw-   0        0        0     1101 2024-04-24 01:08:28.000000 pytctracer-0.2.1/pytctracer/config/config.py
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.498332 pytctracer-0.2.1/pytctracer/config/constants/
--rw-rw-rw-   0        0        0      904 2024-04-03 23:07:54.000000 pytctracer-0.2.1/pytctracer/config/constants/__init__.py
--rw-rw-rw-   0        0        0      180 2024-04-03 23:05:28.000000 pytctracer-0.2.1/pytctracer/config/constants/classification_type.py
--rw-rw-rw-   0        0        0      380 2024-04-03 23:05:47.000000 pytctracer-0.2.1/pytctracer/config/constants/event_type.py
--rw-rw-rw-   0        0        0      216 2024-04-03 23:05:58.000000 pytctracer-0.2.1/pytctracer/config/constants/function_type.py
--rw-rw-rw-   0        0        0      129 2024-04-03 23:06:06.000000 pytctracer-0.2.1/pytctracer/config/constants/instruction_opname.py
--rw-rw-rw-   0        0        0       99 2024-04-03 23:07:08.000000 pytctracer-0.2.1/pytctracer/config/constants/level_type.py
--rw-rw-rw-   0        0        0      202 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/config/constants/metric_score_type.py
--rw-rw-rw-   0        0        0      535 2024-04-03 23:07:28.000000 pytctracer-0.2.1/pytctracer/config/constants/technique_parameter.py
--rw-rw-rw-   0        0        0      915 2024-04-24 01:14:30.000000 pytctracer-0.2.1/pytctracer/config/constants/technique_threshold.py
--rw-rw-rw-   0        0        0      149 2024-04-03 23:07:44.000000 pytctracer-0.2.1/pytctracer/config/constants/testing_method_event_type.py
--rw-rw-rw-   0        0        0      572 2024-04-03 23:07:50.000000 pytctracer-0.2.1/pytctracer/config/constants/trace_data_header.py
--rw-rw-rw-   0        0        0      507 2024-04-03 23:07:54.000000 pytctracer-0.2.1/pytctracer/config/constants/trace_data_variable.py
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.505999 pytctracer-0.2.1/pytctracer/evaluation/
--rw-rw-rw-   0        0        0      170 2024-03-26 14:14:33.000000 pytctracer-0.2.1/pytctracer/evaluation/__init__.py
--rw-rw-rw-   0        0        0     2358 2024-04-24 01:05:02.000000 pytctracer-0.2.1/pytctracer/evaluation/classify_predictions.py
--rw-rw-rw-   0        0        0     2808 2024-04-24 01:06:16.000000 pytctracer-0.2.1/pytctracer/evaluation/evaluate_predictions.py
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.529089 pytctracer-0.2.1/pytctracer/evaluation/metrics/
--rw-rw-rw-   0        0        0      613 2024-03-30 00:46:46.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/__init__.py
--rw-rw-rw-   0        0        0     1581 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/area_under_curve.py
--rw-rw-rw-   0        0        0     2967 2024-03-30 00:46:45.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py
--rw-rw-rw-   0        0        0      914 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/f1.py
--rw-rw-rw-   0        0        0      989 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/false_negatives.py
--rw-rw-rw-   0        0        0      989 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/false_positives.py
--rw-rw-rw-   0        0        0     1470 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/mean_average_precision.py
--rw-rw-rw-   0        0        0      744 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/metric.py
--rw-rw-rw-   0        0        0     1084 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/precision.py
--rw-rw-rw-   0        0        0     1060 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/recall.py
--rw-rw-rw-   0        0        0      995 2024-04-03 23:07:13.000000 pytctracer-0.2.1/pytctracer/evaluation/metrics/true_positives.py
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.531101 pytctracer-0.2.1/pytctracer/io/
--rw-rw-rw-   0        0        0        0 2024-03-30 00:46:30.000000 pytctracer-0.2.1/pytctracer/io/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.535129 pytctracer-0.2.1/pytctracer/io/input/
--rw-rw-rw-   0        0        0      110 2024-03-30 00:46:37.000000 pytctracer-0.2.1/pytctracer/io/input/__init__.py
--rw-rw-rw-   0        0        0     2336 2024-04-26 01:34:44.000000 pytctracer-0.2.1/pytctracer/io/input/from_file.py
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.541140 pytctracer-0.2.1/pytctracer/io/output/
--rw-rw-rw-   0        0        0      367 2024-03-30 00:46:35.000000 pytctracer-0.2.1/pytctracer/io/output/__init__.py
--rw-rw-rw-   0        0        0     3167 2024-04-24 01:02:45.000000 pytctracer-0.2.1/pytctracer/io/output/to_display.py
--rw-rw-rw-   0        0        0     2372 2024-04-24 01:00:34.000000 pytctracer-0.2.1/pytctracer/io/output/to_file.py
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.552233 pytctracer-0.2.1/pytctracer/parsing/
--rw-rw-rw-   0        0        0     1382 2024-03-30 00:46:28.000000 pytctracer-0.2.1/pytctracer/parsing/__init__.py
--rw-rw-rw-   0        0        0     7243 2024-04-24 00:56:25.000000 pytctracer-0.2.1/pytctracer/parsing/find_class_level_calls.py
--rw-rw-rw-   0        0        0     2124 2024-04-24 00:54:18.000000 pytctracer-0.2.1/pytctracer/parsing/find_class_level_names.py
--rw-rw-rw-   0        0        0     6552 2024-04-24 00:53:40.000000 pytctracer-0.2.1/pytctracer/parsing/find_function_level_calls.py
--rw-rw-rw-   0        0        0     2032 2024-04-24 00:51:05.000000 pytctracer-0.2.1/pytctracer/parsing/find_function_level_names.py
--rw-rw-rw-   0        0        0     4285 2024-04-24 00:49:28.000000 pytctracer-0.2.1/pytctracer/parsing/functions_called_before_assert.py
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.567296 pytctracer-0.2.1/pytctracer/techniques/
--rw-rw-rw-   0        0        0      883 2024-03-27 16:49:38.000000 pytctracer-0.2.1/pytctracer/techniques/__init__.py
--rw-rw-rw-   0        0        0     4333 2024-04-24 00:24:31.000000 pytctracer-0.2.1/pytctracer/techniques/arg_name_to_technique_mapper.py
--rw-rw-rw-   0        0        0     3510 2024-04-24 00:47:26.000000 pytctracer-0.2.1/pytctracer/techniques/combined.py
--rw-rw-rw-   0        0        0     4021 2024-04-03 23:07:28.000000 pytctracer-0.2.1/pytctracer/techniques/last_call_before_assert.py
--rw-rw-rw-   0        0        0     5118 2024-04-24 00:41:57.000000 pytctracer-0.2.1/pytctracer/techniques/levenshtein_distance.py
--rw-rw-rw-   0        0        0    11089 2024-04-24 00:41:20.000000 pytctracer-0.2.1/pytctracer/techniques/longest_common_subsequence.py
--rw-rw-rw-   0        0        0     6043 2024-04-24 00:40:03.000000 pytctracer-0.2.1/pytctracer/techniques/naming_conventions.py
--rw-rw-rw-   0        0        0     4976 2024-04-24 00:39:20.000000 pytctracer-0.2.1/pytctracer/techniques/tarantula.py
--rw-rw-rw-   0        0        0     6966 2024-04-24 00:44:46.000000 pytctracer-0.2.1/pytctracer/techniques/technique.py
--rw-rw-rw-   0        0        0    11270 2024-04-24 00:36:56.000000 pytctracer-0.2.1/pytctracer/techniques/tfidf.py
--rw-rw-rw-   0        0        0    21573 2024-04-24 01:38:40.000000 pytctracer-0.2.1/pytctracer/tracer.py
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:12.568296 pytctracer-0.2.1/pytctracer.egg-info/
--rw-rw-rw-   0        0        0    17285 2024-04-26 01:47:12.000000 pytctracer-0.2.1/pytctracer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2634 2024-04-26 01:47:12.000000 pytctracer-0.2.1/pytctracer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 01:47:12.000000 pytctracer-0.2.1/pytctracer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-26 01:47:12.000000 pytctracer-0.2.1/pytctracer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      166 2024-04-26 01:47:12.000000 pytctracer-0.2.1/pytctracer.egg-info/requires.txt
--rw-rw-rw-   0        0        0      101 2024-04-26 01:47:12.000000 pytctracer-0.2.1/pytctracer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 01:47:12.572296 pytctracer-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.959673 pytctracer-0.2.2/
+-rw-rw-rw-   0        0        0    17285 2024-04-26 02:44:59.957673 pytctracer-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    16291 2024-04-26 01:45:21.000000 pytctracer-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.834769 pytctracer-0.2.2/data/
+drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.821139 pytctracer-0.2.2/data/ground-truth-data/
+drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.838776 pytctracer-0.2.2/data/ground-truth-data/pyopenssl/
+-rw-rw-rw-   0        0        0    14927 2023-12-12 17:26:56.000000 pytctracer-0.2.2/data/ground-truth-data/pyopenssl/pyopenssl_all_functions.py
+-rw-rw-rw-   0        0        0     2737 2024-01-17 14:14:19.000000 pytctracer-0.2.2/data/ground-truth-data/pyopenssl/pyopenssl_chosen_tests.py
+-rw-rw-rw-   0        0        0     2195 2024-04-09 23:53:27.000000 pytctracer-0.2.2/data/t.py
+-rw-rw-rw-   0        0        0      464 2024-02-25 02:21:54.000000 pytctracer-0.2.2/data/tes.py
+-rw-rw-rw-   0        0        0    81858 2024-04-26 02:23:42.000000 pytctracer-0.2.2/data/trace_parser_dynamic.py
+-rw-rw-rw-   0        0        0     1045 2024-04-26 02:44:32.000000 pytctracer-0.2.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.845410 pytctracer-0.2.2/pytctracer/
+-rw-rw-rw-   0        0        0      104 2024-03-31 18:38:21.000000 pytctracer-0.2.2/pytctracer/__init__.py
+-rw-rw-rw-   0        0        0    22577 2024-04-26 02:42:32.000000 pytctracer-0.2.2/pytctracer/analyser.py
+-rw-rw-rw-   0        0        0     9141 2024-04-26 02:42:31.000000 pytctracer-0.2.2/pytctracer/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.890238 pytctracer-0.2.2/pytctracer/config/
+-rw-rw-rw-   0        0        0       49 2024-03-30 00:46:49.000000 pytctracer-0.2.2/pytctracer/config/__init__.py
+-rw-rw-rw-   0        0        0     1103 2024-04-26 02:42:31.000000 pytctracer-0.2.2/pytctracer/config/config.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.904814 pytctracer-0.2.2/pytctracer/config/constants/
+-rw-rw-rw-   0        0        0      904 2024-04-03 23:07:54.000000 pytctracer-0.2.2/pytctracer/config/constants/__init__.py
+-rw-rw-rw-   0        0        0      180 2024-04-03 23:05:28.000000 pytctracer-0.2.2/pytctracer/config/constants/classification_type.py
+-rw-rw-rw-   0        0        0      380 2024-04-03 23:05:47.000000 pytctracer-0.2.2/pytctracer/config/constants/event_type.py
+-rw-rw-rw-   0        0        0      216 2024-04-03 23:05:58.000000 pytctracer-0.2.2/pytctracer/config/constants/function_type.py
+-rw-rw-rw-   0        0        0      129 2024-04-03 23:06:06.000000 pytctracer-0.2.2/pytctracer/config/constants/instruction_opname.py
+-rw-rw-rw-   0        0        0       99 2024-04-03 23:07:08.000000 pytctracer-0.2.2/pytctracer/config/constants/level_type.py
+-rw-rw-rw-   0        0        0      202 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/config/constants/metric_score_type.py
+-rw-rw-rw-   0        0        0      535 2024-04-03 23:07:28.000000 pytctracer-0.2.2/pytctracer/config/constants/technique_parameter.py
+-rw-rw-rw-   0        0        0     1014 2024-04-26 02:42:32.000000 pytctracer-0.2.2/pytctracer/config/constants/technique_threshold.py
+-rw-rw-rw-   0        0        0      149 2024-04-03 23:07:44.000000 pytctracer-0.2.2/pytctracer/config/constants/testing_method_event_type.py
+-rw-rw-rw-   0        0        0      572 2024-04-03 23:07:50.000000 pytctracer-0.2.2/pytctracer/config/constants/trace_data_header.py
+-rw-rw-rw-   0        0        0      507 2024-04-03 23:07:54.000000 pytctracer-0.2.2/pytctracer/config/constants/trace_data_variable.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.909408 pytctracer-0.2.2/pytctracer/evaluation/
+-rw-rw-rw-   0        0        0      170 2024-03-26 14:14:33.000000 pytctracer-0.2.2/pytctracer/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     2350 2024-04-26 02:42:31.000000 pytctracer-0.2.2/pytctracer/evaluation/classify_predictions.py
+-rw-rw-rw-   0        0        0     2804 2024-04-26 02:42:31.000000 pytctracer-0.2.2/pytctracer/evaluation/evaluate_predictions.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.924377 pytctracer-0.2.2/pytctracer/evaluation/metrics/
+-rw-rw-rw-   0        0        0      613 2024-03-30 00:46:46.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1581 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/area_under_curve.py
+-rw-rw-rw-   0        0        0     2967 2024-03-30 00:46:45.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py
+-rw-rw-rw-   0        0        0      914 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/f1.py
+-rw-rw-rw-   0        0        0      989 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/false_negatives.py
+-rw-rw-rw-   0        0        0      989 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/false_positives.py
+-rw-rw-rw-   0        0        0     1470 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/mean_average_precision.py
+-rw-rw-rw-   0        0        0      744 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/metric.py
+-rw-rw-rw-   0        0        0     1084 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/precision.py
+-rw-rw-rw-   0        0        0     1060 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/recall.py
+-rw-rw-rw-   0        0        0      995 2024-04-03 23:07:13.000000 pytctracer-0.2.2/pytctracer/evaluation/metrics/true_positives.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.925583 pytctracer-0.2.2/pytctracer/io/
+-rw-rw-rw-   0        0        0        0 2024-03-30 00:46:30.000000 pytctracer-0.2.2/pytctracer/io/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.928591 pytctracer-0.2.2/pytctracer/io/input/
+-rw-rw-rw-   0        0        0      110 2024-03-30 00:46:37.000000 pytctracer-0.2.2/pytctracer/io/input/__init__.py
+-rw-rw-rw-   0        0        0     2372 2024-04-26 02:42:31.000000 pytctracer-0.2.2/pytctracer/io/input/from_file.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.932591 pytctracer-0.2.2/pytctracer/io/output/
+-rw-rw-rw-   0        0        0      367 2024-03-30 00:46:35.000000 pytctracer-0.2.2/pytctracer/io/output/__init__.py
+-rw-rw-rw-   0        0        0     3167 2024-04-24 01:02:45.000000 pytctracer-0.2.2/pytctracer/io/output/to_display.py
+-rw-rw-rw-   0        0        0     2455 2024-04-26 02:42:31.000000 pytctracer-0.2.2/pytctracer/io/output/to_file.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.940619 pytctracer-0.2.2/pytctracer/parsing/
+-rw-rw-rw-   0        0        0     1382 2024-03-30 00:46:28.000000 pytctracer-0.2.2/pytctracer/parsing/__init__.py
+-rw-rw-rw-   0        0        0     7226 2024-04-26 02:42:32.000000 pytctracer-0.2.2/pytctracer/parsing/find_class_level_calls.py
+-rw-rw-rw-   0        0        0     2120 2024-04-26 02:42:31.000000 pytctracer-0.2.2/pytctracer/parsing/find_class_level_names.py
+-rw-rw-rw-   0        0        0     6548 2024-04-26 02:42:32.000000 pytctracer-0.2.2/pytctracer/parsing/find_function_level_calls.py
+-rw-rw-rw-   0        0        0     2022 2024-04-26 02:42:31.000000 pytctracer-0.2.2/pytctracer/parsing/find_function_level_names.py
+-rw-rw-rw-   0        0        0     4273 2024-04-26 02:42:31.000000 pytctracer-0.2.2/pytctracer/parsing/functions_called_before_assert.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.954652 pytctracer-0.2.2/pytctracer/techniques/
+-rw-rw-rw-   0        0        0      883 2024-03-27 16:49:38.000000 pytctracer-0.2.2/pytctracer/techniques/__init__.py
+-rw-rw-rw-   0        0        0     4325 2024-04-26 02:42:32.000000 pytctracer-0.2.2/pytctracer/techniques/arg_name_to_technique_mapper.py
+-rw-rw-rw-   0        0        0     3479 2024-04-26 02:42:32.000000 pytctracer-0.2.2/pytctracer/techniques/combined.py
+-rw-rw-rw-   0        0        0     4021 2024-04-03 23:07:28.000000 pytctracer-0.2.2/pytctracer/techniques/last_call_before_assert.py
+-rw-rw-rw-   0        0        0     5118 2024-04-24 00:41:57.000000 pytctracer-0.2.2/pytctracer/techniques/levenshtein_distance.py
+-rw-rw-rw-   0        0        0    11089 2024-04-24 00:41:20.000000 pytctracer-0.2.2/pytctracer/techniques/longest_common_subsequence.py
+-rw-rw-rw-   0        0        0     6043 2024-04-24 00:40:03.000000 pytctracer-0.2.2/pytctracer/techniques/naming_conventions.py
+-rw-rw-rw-   0        0        0     4976 2024-04-24 00:39:20.000000 pytctracer-0.2.2/pytctracer/techniques/tarantula.py
+-rw-rw-rw-   0        0        0     6954 2024-04-26 02:42:32.000000 pytctracer-0.2.2/pytctracer/techniques/technique.py
+-rw-rw-rw-   0        0        0    11270 2024-04-24 00:36:56.000000 pytctracer-0.2.2/pytctracer/techniques/tfidf.py
+-rw-rw-rw-   0        0        0    21533 2024-04-26 02:42:32.000000 pytctracer-0.2.2/pytctracer/tracer.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:44:59.956666 pytctracer-0.2.2/pytctracer.egg-info/
+-rw-rw-rw-   0        0        0    17285 2024-04-26 02:44:59.000000 pytctracer-0.2.2/pytctracer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2634 2024-04-26 02:44:59.000000 pytctracer-0.2.2/pytctracer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 02:44:59.000000 pytctracer-0.2.2/pytctracer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-26 02:44:59.000000 pytctracer-0.2.2/pytctracer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      166 2024-04-26 02:44:59.000000 pytctracer-0.2.2/pytctracer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       43 2024-04-26 02:44:59.000000 pytctracer-0.2.2/pytctracer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 02:44:59.959673 pytctracer-0.2.2/setup.cfg
```

### Comparing `pytctracer-0.2.1/PKG-INFO` & `pytctracer-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytctracer
-Version: 0.2.1
+Version: 0.2.2
 Summary: Research library demonstrating test-to-code traceability techniques on Python codebases that use the Pytest testing framework.
 Author: Jason Ho
 Project-URL: Repository, https://github.com/jasonho2582001/comp0138-pytctracer
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pytctracer-0.2.1/README.md` & `pytctracer-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/data/ground-truth-data/pyopenssl/pyopenssl_all_functions.py` & `pytctracer-0.2.2/data/ground-truth-data/pyopenssl/pyopenssl_all_functions.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/data/ground-truth-data/pyopenssl/pyopenssl_chosen_tests.py` & `pytctracer-0.2.2/data/ground-truth-data/pyopenssl/pyopenssl_chosen_tests.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/data/t.py` & `pytctracer-0.2.2/data/t.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/data/trace_parser_dynamic.py` & `pytctracer-0.2.2/data/trace_parser_dynamic.py`

 * *Files 0% similar despite different names*

```diff
@@ -668,15 +668,15 @@
     # print_dict_results(naming_convention_contains_dict, "Results for Naming Convention - Contains", 10)
     # print_dict_results(lcsb_dict, "LCS - Both", tests_to_create_links_for, 10)
     # print_dict_results(lcsu_dict, "LCS - Unit", tests_to_create_links_for, 10)
     # print_dict_results(levenshtein_dict, "Levenshtein", tests_to_create_links_for, 10)
     # print_dict_results(lcba_dict, "LCBA", tests_to_create_links_for, 10)
     # print_dict_results(tarantula_dict, "Tarauntula", tests_to_create_links_for, 10)
     # print_dict_results(tfidf_dict, "Tarauntula", tests_to_create_links_for, 10)z
-    # print_dict_results(average_dict, "Simple Average", tests_to_create_links_for, 10)
+    # print_dict_results(average_dict, "Combined", tests_to_create_links_for, 10)
 
     # PRODUCING PREDICTIONS
     combined_evaluation_dict = {}
     
     predicted_links_for_naming_convention = generate_predicted_links(naming_conventions_dict, 1, tests_to_create_links_for)
     predicted_links_for_naming_convention_contains = generate_predicted_links(naming_convention_contains_dict, 1, tests_to_create_links_for)
     predicted_links_for_lcsb = generate_predicted_links(lcsb_dict, THRESHOLD_FOR_LCSB, tests_to_create_links_for)
@@ -706,15 +706,15 @@
     combined_evaluation_dict["Longest Common Subsequence - Both"] = evaluation_dict_for_lcsb
     combined_evaluation_dict["Longest Common Subsequence - Unit"] = evaluation_dict_for_lcsu
     combined_evaluation_dict["Levenshtein Distance"] = evaluation_dict_for_levenshtein
     combined_evaluation_dict["Last Call Before Assert"] = evaluation_dict_for_lcba
     combined_evaluation_dict["Tarantula"] = evaluation_dict_for_tarauntula
     combined_evaluation_dict["TF-IDF"] = evaluation_dict_for_tfidf
     combined_evaluation_dict["TF-IDF (Multiset)"] = evaluation_dict_for_tfidf_count
-    combined_evaluation_dict["Simple Average"] = evaluation_dict_for_average
+    combined_evaluation_dict["Combined"] = evaluation_dict_for_average
     combined_evaluation_dict["Copilot"] = evaluation_dict_for_copilot
 
     # OUTPUT
     # print_predicted_links(predicted_links_for_naming_convention, evaluation_dict_for_naming_convention, "Predicted Links for Naming Convention")
     # print_predicted_links(predicted_links_for_naming_convention, evaluation_dict_for_naming_convention_contains, "Predicted Links for Naming Convention - Contains")
     # print_predicted_links(predicted_links_for_levenshtein, evaluation_dict_for_levenshtein, "Predicted Links for Levenshtein Distance")
     
@@ -759,15 +759,15 @@
     # print_dict_results(naming_convention_contains_dict, "Results for Naming Convention - Contains", 10)
     # print_dict_results(lcsb_dict, "LCS - Both", tests_to_create_links_for, 10)
     # print_dict_results(lcsu_dict, "LCS - Unit", tests_to_create_links_for, 10)
     # print_dict_results(levenshtein_dict, "Levenshtein", tests_to_create_links_for, 10)
     # print_dict_results(lcba_dict, "LCBA", tests_to_create_links_for, 10)
     # print_dict_results(tarantula_dict, "Tarauntula", tests_to_create_links_for, 10)
     # print_dict_results(tfidf_dict, "Tarauntula", tests_to_create_links_for, 10)z
-    # print_dict_results(average_dict, "Simple Average", tests_to_create_links_for, 10)
+    # print_dict_results(average_dict, "Combined", tests_to_create_links_for, 10)
 
     # PRODUCING PREDICTIONS
     combined_evaluation_dict = {}
     
     predicted_links_for_naming_convention = generate_predicted_links(naming_conventions_dict, 1, tests_to_create_links_for)
     predicted_links_for_naming_convention_contains = generate_predicted_links(naming_convention_contains_dict, 1, tests_to_create_links_for)
     predicted_links_for_lcsb = generate_predicted_links(lcsb_dict, THRESHOLD_FOR_LCSB, tests_to_create_links_for)
@@ -796,15 +796,15 @@
     combined_evaluation_dict["Longest Common Subsequence - Both"] = evaluation_dict_for_lcsb
     combined_evaluation_dict["Longest Common Subsequence - Unit"] = evaluation_dict_for_lcsu
     combined_evaluation_dict["Levenshtein Distance"] = evaluation_dict_for_levenshtein
     combined_evaluation_dict["Last Call Before Assert"] = evaluation_dict_for_lcba
     combined_evaluation_dict["Tarantula"] = evaluation_dict_for_tarauntula
     combined_evaluation_dict["TF-IDF"] = evaluation_dict_for_tfidf
     combined_evaluation_dict["TF-IDF (Multiset)"] = evaluation_dict_for_tfidf_count
-    combined_evaluation_dict["Simple Average"] = evaluation_dict_for_average
+    combined_evaluation_dict["Combined"] = evaluation_dict_for_average
     combined_evaluation_dict["Copilot"] = evaluation_dict_for_copilot
 
     # OUTPUT
     # print_predicted_links(predicted_links_for_naming_convention, evaluation_dict_for_naming_convention, "Predicted Links for Naming Convention")
     # print_predicted_links(predicted_links_for_naming_convention, evaluation_dict_for_naming_convention_contains, "Predicted Links for Naming Convention - Contains")
     # print_predicted_links(predicted_links_for_levenshtein, evaluation_dict_for_levenshtein, "Predicted Links for Levenshtein Distance")
```

### Comparing `pytctracer-0.2.1/pyproject.toml` & `pytctracer-0.2.2/pyproject.toml`

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
-version = "0.2.1"
+version = "0.2.2"
 classifiers=[
     "Natural Language :: English",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
```

### Comparing `pytctracer-0.2.1/pytctracer/analyser.py` & `pytctracer-0.2.2/pytctracer/analyser.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 
 class Analyser:
     """
     Class which handles the the generation, evaluation and comparison
     of test-to-code traceability links.
     """
+
     def __init__(self) -> None:
         self.arg_name_to_technique_map = ArgNameToTechniqueMapper()
         self.arg_name_to_metric_map = ArgNameToMetricMapper()
         self.default_technique_names = Config.DEFAULT_CHOSEN_TECHNIQUE_NAMES
         self.default_metric_names = Config.DEFAULT_CHOSEN_METRIC_NAMES
 
     def produce_traceability_links_for_trace(
@@ -93,18 +94,18 @@
         classifications_output_directory_path: Optional[str] = None,
         evaluation_metrics_output_path: Optional[str] = None,
         display_classifications_to_stdout: bool = False,
         metric_as_percentage: bool = False,
     ) -> None:
         """
         Produces traceability links for a given dynamic trace log, and then
-        evaluates them against a specified ground truth. Allows for choosing 
+        evaluates them against a specified ground truth. Allows for choosing
         the technique names to evaluate predictions for, the metric names to
-        compute, and whether to add a combined technique as well as output 
-        paths for the classifications and metrics. 
+        compute, and whether to add a combined technique as well as output
+        paths for the classifications and metrics.
 
         Args:
             trace_csv_log_path (str): The path to the dynamic trace log CSV file.
             ground_truth_path (str): The path to the ground truth JSON file.
             traceability_level (LevelType): The level of traceability to produce links for.
             add_combined_technique (bool): Whether to produce links with the combined technique.
             chosen_technique_names (Optional[List[str]]): The arg names of the techniques to use.
@@ -245,15 +246,14 @@
         tests_in_predicted_links = set(predicted_links.keys())
         for test in ground_truth_links:
             if test not in tests_in_predicted_links:
                 raise ValueError(
                     f"Test '{test}' in ground truth but not in predicted links"
                 )
 
-
     def _write_classifications_for_techniques(
         self,
         classifications_for_techniques: Dict[str, Dict[str, List[str]]],
         classifications_output_directory_path: str,
         traceability_level: LevelType,
     ) -> None:
         for (
```

### Comparing `pytctracer-0.2.1/pytctracer/cli.py` & `pytctracer-0.2.2/pytctracer/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
     is_flag=True,
     default=False,
     help="""Report continous metrics as percentages. If omitted,
               metrics are reported as raw values by default.""",
 )
 @click.option(
     "--classifications-output-path",
-    type=click.Path(exists=True),
+    type=click.Path(exists=False),
     help="""Path to write the JSON containing the classifications to.""",
 )
 @click.option(
     "--metrics-output-path",
     type=click.Path(exists=False),
     help="""Path to write the CSV containing the evaluation metric results to.""",
 )
@@ -238,9 +238,10 @@
             metric_as_percentage=as_percentage,
             classifications_output_path=classifications_output_path,
             evaluation_metrics_output_path=metrics_output_path,
         )
     except Exception as e:
         raise click.ClickException(str(e))
 
+
 if __name__ == "__main__":
     cli()
```

### Comparing `pytctracer-0.2.1/pytctracer/config/config.py` & `pytctracer-0.2.2/pytctracer/config/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 class Config:
     """
     Class storing configuration variables for the package.
     """
+
     SELECTABLE_TECHNIQUE_NAMES = [
         "nc",
         "ncc",
         "lcsb",
         "lcsu",
         "leven",
         "lcba",
@@ -51,8 +52,9 @@
         "leven": 0.95,
         "tarantula": 0.95,
         "tfidf": 0.9,
         "tfidf_multiset": 0.9,
         "combined": 0.85,
     }
 
+
 __all__ = ["Config"]
```

### Comparing `pytctracer-0.2.1/pytctracer/config/constants/__init__.py` & `pytctracer-0.2.2/pytctracer/config/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/config/constants/technique_parameter.py` & `pytctracer-0.2.2/pytctracer/config/constants/technique_parameter.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/config/constants/technique_threshold.py` & `pytctracer-0.2.2/pytctracer/config/constants/technique_threshold.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,30 @@
 from dotenv import load_dotenv
 from pytctracer.config.config import Config
 
 DEFAULT_THRESHOLDS = Config.DEFAULT_THRESHOLDS
 
 load_dotenv()
 
+
 class TechniqueThreshold(float, Enum):
-    THRESHOLD_FOR_LCSU = os.environ.get("THRESHOLD_FOR_LCSU", DEFAULT_THRESHOLDS["lcsu"])
-    THRESHOLD_FOR_LCSB = os.environ.get("THRESHOLD_FOR_LCSB", DEFAULT_THRESHOLDS["lcsb"])
-    THRESHOLD_FOR_LEVENSHTEIN = os.environ.get("THRESHOLD_FOR_LEVENSHTEIN", DEFAULT_THRESHOLDS["leven"])
-    THRESHOLD_FOR_TARANTULA = os.environ.get("THRESHOLD_FOR_TARANTULA", DEFAULT_THRESHOLDS["tarantula"])
-    THRESHOLD_FOR_TFIDF = os.environ.get("THRESHOLD_FOR_TFIDF", DEFAULT_THRESHOLDS["tfidf"])
-    THRESHOLD_FOR_TFIDF_MULTISET = os.environ.get("THRESHOLD_FOR_TFIDF_MULTISET", DEFAULT_THRESHOLDS["tfidf_multiset"])
-    THRESHOLD_FOR_COMBINED = os.environ.get("THRESHOLD_FOR_COMBINED", DEFAULT_THRESHOLDS["combined"])
+    THRESHOLD_FOR_LCSU = os.environ.get(
+        "THRESHOLD_FOR_LCSU", DEFAULT_THRESHOLDS["lcsu"]
+    )
+    THRESHOLD_FOR_LCSB = os.environ.get(
+        "THRESHOLD_FOR_LCSB", DEFAULT_THRESHOLDS["lcsb"]
+    )
+    THRESHOLD_FOR_LEVENSHTEIN = os.environ.get(
+        "THRESHOLD_FOR_LEVENSHTEIN", DEFAULT_THRESHOLDS["leven"]
+    )
+    THRESHOLD_FOR_TARANTULA = os.environ.get(
+        "THRESHOLD_FOR_TARANTULA", DEFAULT_THRESHOLDS["tarantula"]
+    )
+    THRESHOLD_FOR_TFIDF = os.environ.get(
+        "THRESHOLD_FOR_TFIDF", DEFAULT_THRESHOLDS["tfidf"]
+    )
+    THRESHOLD_FOR_TFIDF_MULTISET = os.environ.get(
+        "THRESHOLD_FOR_TFIDF_MULTISET", DEFAULT_THRESHOLDS["tfidf_multiset"]
+    )
+    THRESHOLD_FOR_COMBINED = os.environ.get(
+        "THRESHOLD_FOR_COMBINED", DEFAULT_THRESHOLDS["combined"]
+    )
```

### Comparing `pytctracer-0.2.1/pytctracer/config/constants/trace_data_header.py` & `pytctracer-0.2.2/pytctracer/config/constants/trace_data_header.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/evaluation/classify_predictions.py` & `pytctracer-0.2.2/pytctracer/evaluation/classify_predictions.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             the fully qualified names of the unit tests, and the values are lists
             of fully qualified names of the functions predicted to be linked to
             the unit test.
         ground_truth_links (Dict[str, List[str]]): A dictionary where the keys are
             the fully qualified names of the unit tests, and the values are lists
             of fully qualified names of the functions that are actually linked
             to the unit test.
-        
+
     Returns:
         Dict[str, Dict[str, List[str]]]: A dictionary where the keys are the fully
         qualified names of the unit tests, and the values are dictionaries
         containing the true positives, false positives, and false negatives for
         each unit test.
     """
     classification_dict = defaultdict(dict)
```

### Comparing `pytctracer-0.2.1/pytctracer/evaluation/evaluate_predictions.py` & `pytctracer-0.2.2/pytctracer/evaluation/evaluate_predictions.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             of traceability scores for each test and source code pair. Defaults to None.
         metric_as_percentage (bool, optional): Whether to report continous metrics as
             percentages. If omitted, metrics are reported as raw values by default.
             Defaults to False.
         uses_threshold (bool, optional): Whether the technique uses a threshold value
             to generate predicted links (Used if an evaluation is for predictions generated
             from a technique class). Defaults to True.
-    
+
     Returns:
         Dict[str, float]: A dictionary where the keys are the argument names of the
             selected metrics, and the values are the scores for the metrics.
     """
     evaluation_dict = {}
     for metric in selected_metrics:
         if metric.metric_type == MetricScoreType.THRESHOLD_INDEPENDENT and (
```

### Comparing `pytctracer-0.2.1/pytctracer/evaluation/metrics/__init__.py` & `pytctracer-0.2.2/pytctracer/evaluation/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/evaluation/metrics/area_under_curve.py` & `pytctracer-0.2.2/pytctracer/evaluation/metrics/area_under_curve.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py` & `pytctracer-0.2.2/pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/evaluation/metrics/f1.py` & `pytctracer-0.2.2/pytctracer/evaluation/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/evaluation/metrics/false_negatives.py` & `pytctracer-0.2.2/pytctracer/evaluation/metrics/false_negatives.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/evaluation/metrics/false_positives.py` & `pytctracer-0.2.2/pytctracer/evaluation/metrics/false_positives.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/evaluation/metrics/mean_average_precision.py` & `pytctracer-0.2.2/pytctracer/evaluation/metrics/mean_average_precision.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/evaluation/metrics/metric.py` & `pytctracer-0.2.2/pytctracer/evaluation/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/evaluation/metrics/precision.py` & `pytctracer-0.2.2/pytctracer/evaluation/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/evaluation/metrics/recall.py` & `pytctracer-0.2.2/pytctracer/evaluation/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/evaluation/metrics/true_positives.py` & `pytctracer-0.2.2/pytctracer/evaluation/metrics/true_positives.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/io/input/from_file.py` & `pytctracer-0.2.2/pytctracer/io/input/from_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 def read_trace_csv_log(file_path: str) -> List[Dict[str, str]]:
     """
     Read a CSV file containing trace data and return it as a list of dictionaries.
 
     Args:
         file_path (str): The path to the CSV file.
-    
+
     Returns:
         List[Dict[str, str]]: A list of dictionaries where each dictionary represents
         a row in the CSV file, with the keys being the column names and the values
         being the corresponding values in the row.
     """
     data = []
     try:
@@ -37,36 +37,40 @@
 
         return data
 
     except FileNotFoundError:
         raise FileNotFoundError(f"Trace log not found at path: {file_path}")
 
     except:
-        raise ValueError(f"An error occurred while reading the trace log at path: {file_path}.")
+        raise ValueError(
+            f"An error occurred while reading the trace log at path: {file_path}."
+        )
 
 
 def load_link_json(link_path: str) -> Dict[str, List[str]]:
     """
     Loads a JSON file containing test-to-code links as a dictionary.
 
     Args:
         link_path (str): The path to the JSON file containing test-to-code links.
-    
+
     Returns:
         Dict[str, List[str]]: A dictionary where the keys are the fully qualified names
         of the test or test classes, and the values are lists containing the fully
         qualified names of the function or function classes that the test invokes.
     """
     try:
         with open(link_path, encoding="utf8") as file:
             link_dict = json.load(file)
 
     except FileNotFoundError:
         raise FileNotFoundError(f"Link file not found at path: {link_path}")
 
     except:
-        raise ValueError(f"An error occurred while reading the link file at path: {link_path}.")
+        raise ValueError(
+            f"An error occurred while reading the link file at path: {link_path}."
+        )
 
     return link_dict
 
 
 __all__ = ["read_trace_csv_log", "load_link_json"]
```

### Comparing `pytctracer-0.2.1/pytctracer/io/output/to_display.py` & `pytctracer-0.2.2/pytctracer/io/output/to_display.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/io/output/to_file.py` & `pytctracer-0.2.2/pytctracer/io/output/to_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,21 +17,22 @@
         dict_to_write (Dict[str, Dict[str, str]): The dictionary to write to the JSON file.
         file_path (str): The path to the JSON file to write to.
         sort_keys (bool, optional): Whether to sort the keys in the JSON file. Defaults to True.
     """
     try:
         with open(file_path, "w", encoding="utf8") as file:
             json.dump(dict_to_write, file, indent=4, sort_keys=sort_keys)
-    
+
     except FileNotFoundError:
         raise FileNotFoundError(f"File not found at path: {file_path}")
-    
-    except:
-        raise ValueError(f"An error occurred while writing to the JSON file with path: {file_path}.")
 
+    except:
+        raise ValueError(
+            f"An error occurred while writing to the JSON file with path: {file_path}."
+        )
 
 
 def write_evaluation_metrics_to_csv(
     combined_evaluation_dict: Dict[str, Dict[str, float]], csv_name: str
 ) -> None:
     """
     Write the evaluation metrics for the traceability predictions to a CSV file.
@@ -47,18 +48,22 @@
     try:
         with open(csv_name, "w", newline="", encoding="utf8") as csv_file:
             csv_writer = csv.DictWriter(csv_file, fieldnames=csv_headers)
             csv_writer.writeheader()
             for technique, evaluation_dict in combined_evaluation_dict.items():
                 row = {TECHNIQUE: technique}
                 for metric, score in evaluation_dict.items():
-                    row[metric] = score if not isinstance(score, float) else round(score, 1)
+                    row[metric] = (
+                        score if not isinstance(score, float) else round(score, 1)
+                    )
                 csv_writer.writerow(row)
 
     except FileNotFoundError:
         raise FileNotFoundError(f"File not found at path: {csv_name}")
 
     except:
-        raise ValueError(f"An error occurred while writing to the CSV file with path: {csv_name}.")
+        raise ValueError(
+            f"An error occurred while writing to the CSV file with path: {csv_name}."
+        )
 
 
 __all__ = ["write_classifications_to_json", "write_evaluation_metrics_to_csv"]
```

### Comparing `pytctracer-0.2.1/pytctracer/parsing/__init__.py` & `pytctracer-0.2.2/pytctracer/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/parsing/find_class_level_calls.py` & `pytctracer-0.2.2/pytctracer/parsing/find_class_level_calls.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     trace_data: List[Dict[str, str]]
 ) -> Dict[str, Set[str]]:
     """
     Find the function classes called by each test in the trace data.
 
     Args:
         trace_data (List[Dict[str, str]]): The tracing CSV log as a dictionary.
-    
+
     Returns:
         Dict[str, Set[str]]: A dictionary where the keys are the fully qualified
         names of the unit test, and the values are sets containing the
         fully qualified names of each function class invoked.
     """
     function_classes_called_by_test_dict = defaultdict(set)
     current_test = None
@@ -50,15 +50,15 @@
 ) -> Dict[str, Dict[str, int]]:
     """
     Find the function classes called by each test in the trace data, along with the
     number of times each function class was called.
 
     Args:
         trace_data (List[Dict[str, str]]): The tracing CSV log as a dictionary.
-    
+
     Returns:
         Dict[str, Dict[str, int]]: A dictionary where the keys are the fully
         qualified names of the unit test, and the values are dictionaries
         containing the fully qualified names of each function class invoked, along
         with the number of times each function class was called.
     """
     function_classes_called_by_test_count_dict = defaultdict(lambda: defaultdict(int))
@@ -89,15 +89,15 @@
     trace_data: List[Dict[str, str]],
 ) -> Dict[str, Set[str]]:
     """
     Find the tests that call each function class in the trace data.
 
     Args:
         trace_data (List[Dict[str, str]]): The tracing CSV log as a dictionary.
-    
+
     Returns:
         Dict[str, Set[str]]: A dictionary where the keys are the fully qualified
         names of the function class, and the values are sets containing the
         fully qualified names of each test that calls the function class.
     """
     tests_that_call_function_classes_dict = defaultdict(set)
     current_test = None
@@ -123,20 +123,20 @@
 
 
 def find_function_classes_called_by_test_depth(
     trace_data: List[Dict[str, str]],
 ) -> Dict[str, Dict[str, int]]:
     """
     Find the function classes called by each test in the trace data, along with the
-    depth at which each function class was called. If a function class is called 
+    depth at which each function class was called. If a function class is called
     multiple times by a test class, the lowest depth is recorded.
 
     Args:
         trace_data (List[Dict[str, str]]): The tracing CSV log as a dictionary.
-    
+
     Returns:
         Dict[str, Dict[str, int]]: A dictionary where the keys are the fully
         qualified names of the unit test, and the values are dictionaries
         containing the fully qualified names of each function class invoked, along
         with the depth at which each function class was called.
     """
     # Each function appears once for a test, at the highest depth
```

### Comparing `pytctracer-0.2.1/pytctracer/parsing/find_class_level_names.py` & `pytctracer-0.2.2/pytctracer/parsing/find_class_level_names.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ) -> Set[Tuple[str, str]]:
     """
     Find the function and fully qualified names of the function classes found in the
     trace data.
 
     Args:
         trace_data (List[Dict[str, str]]): The tracing CSV log as a dictionary.
-    
+
     Returns:
         Set[Tuple[str, str]]: A set of tuples where the first element of each
         tuple is the fully qualified (full path) name of a function class, and the second
         element is the short name of the function class.
     """
     function_class_names_tuple = set()
     for record in trace_data:
```

### Comparing `pytctracer-0.2.1/pytctracer/parsing/find_function_level_calls.py` & `pytctracer-0.2.2/pytctracer/parsing/find_function_level_calls.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,23 @@
     TraceDataHeader,
     TestingMethodType,
     EventType,
     FunctionType,
 )
 
 
-def find_functions_called_by_test(trace_data: List[Dict[str, str]]) -> Dict[str, Set[str]]:
+def find_functions_called_by_test(
+    trace_data: List[Dict[str, str]]
+) -> Dict[str, Set[str]]:
     """
     Find the functions called by each test in the trace data.
 
     Args:
         trace_data (List[Dict[str, str]]): The tracing CSV log as a dictionary.
-    
+
     Returns:
         Dict[str, Set[str]]: A dictionary where the keys are the fully qualified
         names of the unit test, and the values are sets containing the
         fully qualified names of each function invoked.
     """
     functions_called_by_test_dict = defaultdict(set)
     current_test = None
@@ -47,15 +49,15 @@
 ) -> Dict[str, Dict[str, int]]:
     """
     Find the functions called by each test in the trace data, along with the
     number of times each function was called.
 
     Args:
         trace_data (List[Dict[str, str]]): The tracing CSV log as a dictionary.
-    
+
     Returns:
         Dict[str, Dict[str, int]]: A dictionary where the keys are the fully
         qualified names of the unit test, and the values are dictionaries
         containing the fully qualified names of each function invoked, along
         with the number of times each function was called.
     """
     functions_called_by_test_count_dict = defaultdict(lambda: defaultdict(int))
@@ -77,21 +79,23 @@
             functions_called_by_test_count_dict[current_test][
                 record[TraceDataHeader.FULLY_QUALIFIED_FUNCTION_NAME]
             ] += 1
 
     return functions_called_by_test_count_dict
 
 
-def find_tests_that_call_function(trace_data: List[Dict[str, str]]) -> Dict[str, Set[str]]:
+def find_tests_that_call_function(
+    trace_data: List[Dict[str, str]]
+) -> Dict[str, Set[str]]:
     """
     Find the tests that call each function in the trace data.
 
     Args:
         trace_data (List[Dict[str, str]]): The tracing CSV log as a dictionary.
-    
+
     Returns:
         Dict[str, Set[str]]: A dictionary where the keys are the fully qualified
         names of the function, and the values are sets containing the fully
         qualified names of each test that calls the function.
     """
     tests_that_call_function_dict = defaultdict(set)
     current_test = None
@@ -121,15 +125,15 @@
     """
     Find the functions called by each test in the trace data, along with the
     depth of each call. If a function is called multiple times by a test, the
     lowest depth is recorded.
 
     Args:
         trace_data (List[Dict[str, str]]): The tracing CSV log as a dictionary.
-    
+
     Returns:
         Dict[str, Dict[str, int]]: A dictionary where the keys are the fully
         qualified names of the unit test, and the values are dictionaries
         containing the fully qualified names of each function invoked, along
         with the call depth of each function.
     """
     # Each function appears once for a test, at the highest depth
```

### Comparing `pytctracer-0.2.1/pytctracer/parsing/find_function_level_names.py` & `pytctracer-0.2.2/pytctracer/parsing/find_function_level_names.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
     FunctionType,
     TestingMethodType,
 )
 
 
 def find_function_names_tuple(trace_data: List[Dict[str, str]]) -> Set[Tuple[str, str]]:
     """
-    Find the function and fully qualified names of the functions found in the 
+    Find the function and fully qualified names of the functions found in the
     trace data.
 
     Args:
         trace_data (List[Dict[str, str]]): The tracing CSV log as a dictionary.
-    
+
     Returns:
         Set[Tuple[str, str]]: A set of tuples where the first element of each
-        tuple is the fully qualified (full path) name of a function, and the second 
+        tuple is the fully qualified (full path) name of a function, and the second
         element is the short name of the function.
     """
     function_names_tuple = set()
     for record in trace_data:
         if record[TraceDataHeader.FUNCTION_TYPE] == FunctionType.SOURCE:
             function_names_tuple.add(
                 (
@@ -35,15 +35,15 @@
 def find_test_names_tuple(trace_data: List[Dict[str, str]]) -> Set[Tuple[str, str]]:
     """
     Find the function and fully qualified names of the tests found in the
     trace data.
 
     Args:
         trace_data (List[Dict[str, str]]): The tracing CSV log as a dictionary.
-    
+
     Returns:
         Set[Tuple[str, str]]: A set of tuples where the first element of each
         tuple is the fully qualified (full path) name of a test, and the second
         element is the short name of the test.
     """
     test_names_tuple = set()
     for record in trace_data:
```

### Comparing `pytctracer-0.2.1/pytctracer/parsing/functions_called_before_assert.py` & `pytctracer-0.2.2/pytctracer/parsing/functions_called_before_assert.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ) -> Dict[str, Set[str]]:
     """
     Finds the fully qualified names of the functions called before an
     assert statement for each test.
 
     Args:
         trace_data (List[Dict[str, str]]): The tracing CSV log as a dictionary.
-    
+
     Returns:
         Dict[str, Set[str]]: A dictionary where the keys are the fully qualified
         names of the unit test, and the values are sets containing the
         fully qualified names of each function invoked before
         an assert statement.
     """
     functions_called_before_assert_for_each_test = defaultdict(set)
@@ -61,18 +61,18 @@
 
 def find_classes_called_before_assert_for_each_test(
     trace_data: List[Dict[str, str]]
 ) -> Dict[str, Set[str]]:
     """
     Finds the fully qualified names of the classes called before an assert
     statement for each test class.
-    
+
     Args:
         trace_data (List[Dict[str, str]]): The tracing CSV log as a dictionary.
-    
+
     Returns:
         Dict[str, Set[str]]: A dictionary where the keys are the fully qualified
         names of thetest class, and the values are sets containing the
         fully qualified names function class invoked before
         an assert statement.
     """
     function_classes_called_before_assert_for_each_test = defaultdict(set)
```

### Comparing `pytctracer-0.2.1/pytctracer/techniques/__init__.py` & `pytctracer-0.2.2/pytctracer/techniques/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/techniques/arg_name_to_technique_mapper.py` & `pytctracer-0.2.2/pytctracer/techniques/arg_name_to_technique_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 from .tfidf import TFIDF, TFIDFMultiset
 from .technique import Technique
 from .combined import Combined
 
 
 class ArgNameToTechniqueMapper:
     """
-    Class providing mappings between the argument name of each technique to 
+    Class providing mappings between the argument name of each technique to
     some relevant properties, including the technique's class, full name and
     short name.
     """
+
     def __init__(self):
         self._arg_name_to_technique = {
             LevenshteinDistance.arg_name: LevenshteinDistance,
             NamingConventions.arg_name: NamingConventions,
             NamingConventionsContains.arg_name: NamingConventionsContains,
             LastCallBeforeAssert.arg_name: LastCallBeforeAssert,
             LongestCommonSubsequenceBoth.arg_name: LongestCommonSubsequenceBoth,
@@ -56,15 +57,15 @@
             Combined.arg_name: Combined.short_name,
         }
         self._arg_names = list(self._arg_name_to_technique.keys())
 
     def get_arg_names(self) -> List[str]:
         """
         Return the list of valid technique argument names.
-        
+
         Returns:
             List[str]: List of valid technique argument names.
         """
         return self._arg_names
 
     def get_technique(self, arg_name: str) -> Technique:
         """
```

### Comparing `pytctracer-0.2.1/pytctracer/techniques/combined.py` & `pytctracer-0.2.2/pytctracer/techniques/combined.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 
     Attributes:
         full_name (str): The full name of the technique.
         short_name (str): The short name of the technique.
         arg_name (str): The argument name of the technique
         (the string used to invoke the technique through the CLI).
         description (str): A description of the technique.
-        required_parameters (Dict[str, str]): A dictionary of 
+        required_parameters (Dict[str, str]): A dictionary of
         required parameters for the technique.
-        uses_threshold (bool): A boolean indicating whether the technique 
+        uses_threshold (bool): A boolean indicating whether the technique
         uses a threshold.
         threshold (int): The threshold value for the technique.
         normalise (bool): A boolean indicating whether the technique normalises scores.
-        call_depth_discount (bool): A boolean indicating whether the technique 
+        call_depth_discount (bool): A boolean indicating whether the technique
         discounts scores based on call depth.
     """
 
-    full_name = "Combined (Simple Average)"
+    full_name = "Combined"
     short_name = "Combined"
     arg_name = "combined"
     description = "TBC"
     required_parameters = {}
     uses_threshold = True
     threshold = TechniqueThreshold.THRESHOLD_FOR_COMBINED
     normalise = True
@@ -42,20 +42,20 @@
         """
         Invokes the Combined traceability technique to produce traceability scores
         for each test-to-code pair given. This simply takes the traceability scores
         for each test-to-code pair from each technique, and produces the simple mean of
         them.
 
         Args:
-            traceability_scores_for_techniques (Dict[str, Dict[str, Dict[str, float]]]): 
-            A dictionary where the keys are the names of the techniques, and the values 
-            are dictionaries where thekeys are the fully qualified names of the test or 
+            traceability_scores_for_techniques (Dict[str, Dict[str, Dict[str, float]]]):
+            A dictionary where the keys are the names of the techniques, and the values
+            are dictionaries where thekeys are the fully qualified names of the test or
             test classes, and the values are dictionaries containing the traceability scores
             for each function or function class.
-        
+
         Returns:
             Dict[str, Dict[str, float]]: A dictionary where the keys are the fully qualified
             names of the testor test classes, and the values are dictionaries containing the
             traceability scores for each function or function class.
         """
         number_of_techniques_to_combine = len(traceability_scores_for_techniques)
         combined_scores = None
```

### Comparing `pytctracer-0.2.1/pytctracer/techniques/last_call_before_assert.py` & `pytctracer-0.2.2/pytctracer/techniques/last_call_before_assert.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/techniques/levenshtein_distance.py` & `pytctracer-0.2.2/pytctracer/techniques/levenshtein_distance.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/techniques/longest_common_subsequence.py` & `pytctracer-0.2.2/pytctracer/techniques/longest_common_subsequence.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/techniques/naming_conventions.py` & `pytctracer-0.2.2/pytctracer/techniques/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/techniques/tarantula.py` & `pytctracer-0.2.2/pytctracer/techniques/tarantula.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/techniques/technique.py` & `pytctracer-0.2.2/pytctracer/techniques/technique.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         depending on the technique.
 
         Args:
             traceability_score_dict (Dict[str, Dict[str, float]]): A dictionary of traceability
                 scores for each test and source code pair.
             tests_to_create_links_for (Optional[Set[str]], optional): A set of test names to
                 generate links for. If None, links will be generated for all tests. Defaults to None.
-            
+
         Returns:
             Dict[str, Set[str]]: A dictionary of predicted links for each test.
         """
         if not tests_to_create_links_for:
             tests_to_create_links_for = set(traceability_score_dict.keys())
 
         predicted_links_dict = defaultdict(list)
```

### Comparing `pytctracer-0.2.1/pytctracer/techniques/tfidf.py` & `pytctracer-0.2.2/pytctracer/techniques/tfidf.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.2.1/pytctracer/tracer.py` & `pytctracer-0.2.2/pytctracer/tracer.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 class PytestTracer:
     """
     Class which allows for the tracing of a Pytest test suite invocation,
     capturing and storing dynamic information, and writing of the information
     to a CSV format.
     """
+
     def __init__(
         self,
         project_root: str,
         test_folders: List[str],
         source_folders: List[str],
         output_csv_file_name: str,
     ) -> None:
@@ -70,24 +71,26 @@
         self._line_of_last_assert = None
         self._csv_data = []
         self._in_line_functions_left_list = []
         self._assert_line_values = []
         self._handle_in_line_functions = False
         self._in_line_function_calls = 0
 
-    def trace(self, frame: FrameType, event: str, arg: Optional[Any]=None) -> Callable:
+    def trace(
+        self, frame: FrameType, event: str, arg: Optional[Any] = None
+    ) -> Callable:
         """
         Trace function to be used by `sys.settrace` to capture the tracing of Python code
         during a Pytest test suite invocation.
 
         Args:
             frame (FrameType): The current frame.
             event (str): The event type.
             arg (Optional[Any]): The argument associated with the event.
-        
+
         Returns:
             Callable: The trace function.
         """
         if not self.our_frame(frame):
             code_of_current_frame = frame.f_code
             file_name = os.path.normcase(code_of_current_frame.co_filename)
             function_name = code_of_current_frame.co_name
@@ -179,15 +182,15 @@
 
                     self._current_depth += 1
 
                 elif event == SetTraceEventType.RETURN:
                     # Keep track of the last function that was last returned
                     self._current_depth -= 1
                     self._function_stack.pop()
-                    
+
                     if (
                         function_type.startswith(TEST_PREFIX.upper())
                         or function_type == FunctionType.ASSERT
                     ):
                         self._test_function_stack.pop()
 
                     if function_type == FunctionType.ASSERT:
@@ -226,15 +229,15 @@
                         testing_method=testing_method,
                         thread_id=current_thread_id,
                     )
                     self._check_remaining_in_line_functions(self._current_depth)
 
                 elif event == SetTraceEventType.EXCEPTION:
                     exc_type, exc_value, exc_traceback = arg
-            
+
                     self._add_csv_row_data(
                         depth=self._current_depth,
                         function_type=function_type,
                         function_name=function_name,
                         fully_qualified_function_name=fully_qualified_function_name,
                         class_name=class_name,
                         fully_qualified_class_name=fully_qualified_class_name,
@@ -273,18 +276,18 @@
             csv_writer.writeheader()
             for data_row in self._csv_data:
                 csv_writer.writerow(data_row)
 
     def our_frame(self, frame: FrameType) -> bool:
         """
         Checks whether the current code being traced is the PytestTracer class itself.
-        
+
         Args:
             frame (FrameType): The current frame.
-        
+
         Returns:
             bool: True if the current code being traced is the PytestTracer class itself,
             False otherwise.
         """
         return frame.f_code.co_qualname == TRACE_QUALIFIED_NAME
 
     def _add_csv_row_data(
@@ -332,15 +335,15 @@
             LOCALS
         ):
             class_name_list = code_qualified_name.split(".")
 
             # Remove last element, which should be the function name
             class_name_list.pop()
 
-            # Check current last element is not <locals>. If it is, we need to remove it, 
+            # Check current last element is not <locals>. If it is, we need to remove it,
             # and the previous element.
             # This represents an inner function, so we need to remove it as well to get the actual class
             while class_name_list and class_name_list[-1] == LOCALS:
                 class_name_list.pop()
                 class_name_list.pop()
 
             if class_name_list:
```

### Comparing `pytctracer-0.2.1/pytctracer.egg-info/PKG-INFO` & `pytctracer-0.2.2/pytctracer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytctracer
-Version: 0.2.1
+Version: 0.2.2
 Summary: Research library demonstrating test-to-code traceability techniques on Python codebases that use the Pytest testing framework.
 Author: Jason Ho
 Project-URL: Repository, https://github.com/jasonho2582001/comp0138-pytctracer
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pytctracer-0.2.1/pytctracer.egg-info/SOURCES.txt` & `pytctracer-0.2.2/pytctracer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

