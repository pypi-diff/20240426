# Comparing `tmp/aisdc-1.1.2.tar.gz` & `tmp/aisdc-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aisdc-1.1.2.tar", last modified: Mon Oct 30 16:08:08 2023, max compression
+gzip compressed data, was "aisdc-1.1.3.tar", last modified: Fri Apr 26 17:15:41 2024, max compression
```

## Comparing `aisdc-1.1.2.tar` & `aisdc-1.1.3.tar`

### file list

```diff
@@ -1,64 +1,70 @@
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-10-30 16:08:08.925818 aisdc-1.1.2/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-12-04 22:46:52.000000 aisdc-1.1.2/LICENSE
--rw-r--r--   0 unknown   (1000) unknown   (1000)     6150 2023-10-30 16:08:08.925818 aisdc-1.1.2/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4370 2023-10-30 15:57:13.000000 aisdc-1.1.2/README.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-10-30 16:08:08.925818 aisdc-1.1.2/aisdc/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.1.2/aisdc/__init__.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-10-30 16:08:08.925818 aisdc-1.1.2/aisdc/attacks/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.1.2/aisdc/attacks/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1440 2023-10-09 10:26:16.000000 aisdc-1.1.2/aisdc/attacks/attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    22439 2023-10-30 15:57:13.000000 aisdc-1.1.2/aisdc/attacks/attack_report_formatter.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    26417 2023-10-09 10:26:16.000000 aisdc-1.1.2/aisdc/attacks/attribute_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3594 2023-10-09 10:26:16.000000 aisdc-1.1.2/aisdc/attacks/failfast.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    29545 2023-10-09 10:26:16.000000 aisdc-1.1.2/aisdc/attacks/likelihood_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6396 2023-10-09 10:26:16.000000 aisdc-1.1.2/aisdc/attacks/multiple_attacks.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    14509 2023-10-09 12:22:37.000000 aisdc-1.1.2/aisdc/attacks/report.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    19818 2023-10-19 12:12:50.000000 aisdc-1.1.2/aisdc/attacks/structural_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12493 2023-10-09 10:26:16.000000 aisdc-1.1.2/aisdc/attacks/target.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    37393 2023-10-09 12:22:37.000000 aisdc-1.1.2/aisdc/attacks/worst_case_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11794 2023-10-12 13:02:23.000000 aisdc-1.1.2/aisdc/metrics.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-10-30 16:08:08.925818 aisdc-1.1.2/aisdc/preprocessing/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.1.2/aisdc/preprocessing/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    23765 2023-10-19 12:12:50.000000 aisdc-1.1.2/aisdc/preprocessing/loaders.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-10-30 16:08:08.925818 aisdc-1.1.2/aisdc/safemodel/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       62 2023-10-09 10:26:16.000000 aisdc-1.1.2/aisdc/safemodel/__init__.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-10-30 16:08:08.925818 aisdc-1.1.2/aisdc/safemodel/classifiers/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      311 2023-10-09 10:26:16.000000 aisdc-1.1.2/aisdc/safemodel/classifiers/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7662 2023-10-09 12:22:37.000000 aisdc-1.1.2/aisdc/safemodel/classifiers/dp_svc.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7626 2023-10-09 10:26:16.000000 aisdc-1.1.2/aisdc/safemodel/classifiers/new_model_template.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7231 2023-10-12 13:02:23.000000 aisdc-1.1.2/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    20902 2023-10-09 10:26:16.000000 aisdc-1.1.2/aisdc/safemodel/classifiers/safekeras.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6351 2023-10-12 13:02:23.000000 aisdc-1.1.2/aisdc/safemodel/classifiers/saferandomforestclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1914 2023-10-09 10:26:16.000000 aisdc-1.1.2/aisdc/safemodel/classifiers/safesvc.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1214 2023-10-09 10:26:16.000000 aisdc-1.1.2/aisdc/safemodel/classifiers/safetf.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10824 2023-10-09 10:26:16.000000 aisdc-1.1.2/aisdc/safemodel/reporting.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4984 2023-04-26 12:57:02.000000 aisdc-1.1.2/aisdc/safemodel/rules.json
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    28094 2023-10-09 12:22:37.000000 aisdc-1.1.2/aisdc/safemodel/safemodel.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-10-30 16:08:08.925818 aisdc-1.1.2/aisdc.egg-info/
--rw-r--r--   0 unknown   (1000) unknown   (1000)     6150 2023-10-30 16:08:08.000000 aisdc-1.1.2/aisdc.egg-info/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1638 2023-10-30 16:08:08.000000 aisdc-1.1.2/aisdc.egg-info/SOURCES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-10-30 16:08:08.000000 aisdc-1.1.2/aisdc.egg-info/dependency_links.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      371 2023-10-30 16:08:08.000000 aisdc-1.1.2/aisdc.egg-info/requires.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        6 2023-10-30 16:08:08.000000 aisdc-1.1.2/aisdc.egg-info/top_level.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-10-30 16:08:08.925818 aisdc-1.1.2/setup.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2213 2023-10-30 15:57:28.000000 aisdc-1.1.2/setup.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-10-30 16:08:08.925818 aisdc-1.1.2/tests/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    18840 2023-10-12 13:02:23.000000 aisdc-1.1.2/tests/test_attack_report_formatter.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1648 2023-10-12 13:02:23.000000 aisdc-1.1.2/tests/test_attacks.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5424 2023-10-12 13:02:23.000000 aisdc-1.1.2/tests/test_attacks_target.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7074 2023-10-12 13:02:23.000000 aisdc-1.1.2/tests/test_attacks_via_safemodel.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5964 2023-10-12 13:02:23.000000 aisdc-1.1.2/tests/test_attribute_inference_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1446 2023-10-12 13:02:23.000000 aisdc-1.1.2/tests/test_data_interface.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6702 2023-10-12 13:02:23.000000 aisdc-1.1.2/tests/test_failfast.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9523 2023-10-12 13:02:23.000000 aisdc-1.1.2/tests/test_lira_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6191 2023-10-19 12:12:50.000000 aisdc-1.1.2/tests/test_loaders.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7475 2023-10-12 13:02:23.000000 aisdc-1.1.2/tests/test_metrics.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7361 2023-10-12 13:02:23.000000 aisdc-1.1.2/tests/test_multiple_attacks.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8681 2023-10-12 13:02:23.000000 aisdc-1.1.2/tests/test_safedecisiontreeclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    27277 2023-10-12 13:02:23.000000 aisdc-1.1.2/tests/test_safekeras2.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    17102 2023-10-12 13:02:23.000000 aisdc-1.1.2/tests/test_safemodel.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12049 2023-10-12 13:02:23.000000 aisdc-1.1.2/tests/test_saferandomforestclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4902 2023-10-12 13:02:23.000000 aisdc-1.1.2/tests/test_safesvc.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      399 2023-10-12 13:02:23.000000 aisdc-1.1.2/tests/test_safetf.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12811 2023-10-19 12:12:50.000000 aisdc-1.1.2/tests/test_structural_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    13363 2023-10-12 13:02:23.000000 aisdc-1.1.2/tests/test_worst_case_attack.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2024-04-26 17:15:41.359297 aisdc-1.1.3/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-12-04 22:46:52.000000 aisdc-1.1.3/LICENSE
+-rw-r--r--   0 unknown   (1000) unknown   (1000)     6824 2024-04-26 17:15:41.359297 aisdc-1.1.3/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4702 2024-04-24 16:31:19.000000 aisdc-1.1.3/README.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2024-04-26 17:15:41.351297 aisdc-1.1.3/aisdc/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.1.3/aisdc/__init__.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2024-04-26 17:15:41.355297 aisdc-1.1.3/aisdc/attacks/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.1.3/aisdc/attacks/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1440 2023-10-09 10:26:16.000000 aisdc-1.1.3/aisdc/attacks/attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    22451 2024-04-24 15:57:32.000000 aisdc-1.1.3/aisdc/attacks/attack_report_formatter.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    26286 2024-04-24 19:12:44.000000 aisdc-1.1.3/aisdc/attacks/attribute_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3506 2024-04-24 19:12:44.000000 aisdc-1.1.3/aisdc/attacks/failfast.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    29499 2024-04-26 17:15:16.000000 aisdc-1.1.3/aisdc/attacks/likelihood_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6233 2024-04-24 19:12:44.000000 aisdc-1.1.3/aisdc/attacks/multiple_attacks.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    14510 2024-04-24 19:12:44.000000 aisdc-1.1.3/aisdc/attacks/report.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    19866 2024-04-24 19:12:44.000000 aisdc-1.1.3/aisdc/attacks/structural_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12493 2024-04-25 19:35:07.000000 aisdc-1.1.3/aisdc/attacks/target.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    37257 2024-04-24 19:12:44.000000 aisdc-1.1.3/aisdc/attacks/worst_case_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11794 2024-04-26 17:15:16.000000 aisdc-1.1.3/aisdc/metrics.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2024-04-26 17:15:41.355297 aisdc-1.1.3/aisdc/preprocessing/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.1.3/aisdc/preprocessing/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    23123 2024-04-24 15:57:32.000000 aisdc-1.1.3/aisdc/preprocessing/loaders.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2024-04-26 17:15:41.355297 aisdc-1.1.3/aisdc/safemodel/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       63 2024-04-24 15:57:32.000000 aisdc-1.1.3/aisdc/safemodel/__init__.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2024-04-26 17:15:41.355297 aisdc-1.1.3/aisdc/safemodel/classifiers/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      312 2024-04-24 15:57:32.000000 aisdc-1.1.3/aisdc/safemodel/classifiers/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7663 2024-04-24 15:57:32.000000 aisdc-1.1.3/aisdc/safemodel/classifiers/dp_svc.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7626 2023-10-09 10:26:16.000000 aisdc-1.1.3/aisdc/safemodel/classifiers/new_model_template.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7221 2024-04-24 19:12:44.000000 aisdc-1.1.3/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    20853 2024-04-24 19:12:44.000000 aisdc-1.1.3/aisdc/safemodel/classifiers/safekeras.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6222 2024-04-24 19:12:44.000000 aisdc-1.1.3/aisdc/safemodel/classifiers/saferandomforestclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1914 2023-10-09 10:26:16.000000 aisdc-1.1.3/aisdc/safemodel/classifiers/safesvc.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1213 2024-04-24 15:57:32.000000 aisdc-1.1.3/aisdc/safemodel/classifiers/safetf.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10824 2023-10-09 10:26:16.000000 aisdc-1.1.3/aisdc/safemodel/reporting.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4984 2023-04-26 12:57:02.000000 aisdc-1.1.3/aisdc/safemodel/rules.json
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    27969 2024-04-24 19:12:44.000000 aisdc-1.1.3/aisdc/safemodel/safemodel.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2024-04-26 17:15:41.359297 aisdc-1.1.3/aisdc.egg-info/
+-rw-r--r--   0 unknown   (1000) unknown   (1000)     6824 2024-04-26 17:15:41.000000 aisdc-1.1.3/aisdc.egg-info/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1898 2024-04-26 17:15:41.000000 aisdc-1.1.3/aisdc.egg-info/SOURCES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2024-04-26 17:15:41.000000 aisdc-1.1.3/aisdc.egg-info/dependency_links.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      370 2024-04-26 17:15:41.000000 aisdc-1.1.3/aisdc.egg-info/requires.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       12 2024-04-26 17:15:41.000000 aisdc-1.1.3/aisdc.egg-info/top_level.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2024-04-26 17:15:41.359297 aisdc-1.1.3/setup.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2150 2024-04-24 15:57:32.000000 aisdc-1.1.3/setup.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2024-04-26 17:15:41.351297 aisdc-1.1.3/tests/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2024-04-26 17:15:41.359297 aisdc-1.1.3/tests/attacks/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2024-04-24 15:57:32.000000 aisdc-1.1.3/tests/attacks/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    19173 2024-04-24 15:57:32.000000 aisdc-1.1.3/tests/attacks/test_attack_report_formatter.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2912 2024-04-24 19:12:44.000000 aisdc-1.1.3/tests/attacks/test_attacks_target.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5384 2024-04-24 19:12:44.000000 aisdc-1.1.3/tests/attacks/test_attribute_inference_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1399 2024-04-24 19:12:44.000000 aisdc-1.1.3/tests/attacks/test_data_interface.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6668 2024-04-24 19:12:44.000000 aisdc-1.1.3/tests/attacks/test_failfast.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9443 2024-04-24 19:12:44.000000 aisdc-1.1.3/tests/attacks/test_lira_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7475 2024-04-24 15:57:32.000000 aisdc-1.1.3/tests/attacks/test_metrics.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7291 2024-04-24 19:12:44.000000 aisdc-1.1.3/tests/attacks/test_multiple_attacks.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12582 2024-04-24 15:57:32.000000 aisdc-1.1.3/tests/attacks/test_structural_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    13317 2024-04-24 19:12:44.000000 aisdc-1.1.3/tests/attacks/test_worst_case_attack.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2024-04-26 17:15:41.359297 aisdc-1.1.3/tests/preprocessing/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2024-04-24 15:57:32.000000 aisdc-1.1.3/tests/preprocessing/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7270 2024-04-24 15:57:32.000000 aisdc-1.1.3/tests/preprocessing/test_loaders.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2024-04-26 17:15:41.359297 aisdc-1.1.3/tests/safemodel/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2024-04-24 15:57:32.000000 aisdc-1.1.3/tests/safemodel/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1648 2024-04-24 15:57:32.000000 aisdc-1.1.3/tests/safemodel/test_attacks.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3935 2024-04-24 19:12:44.000000 aisdc-1.1.3/tests/safemodel/test_attacks_via_safemodel.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8681 2024-04-24 15:57:32.000000 aisdc-1.1.3/tests/safemodel/test_safedecisiontreeclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    27278 2024-04-24 19:12:44.000000 aisdc-1.1.3/tests/safemodel/test_safekeras2.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    17150 2024-04-24 15:57:32.000000 aisdc-1.1.3/tests/safemodel/test_safemodel.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12014 2024-04-24 15:57:32.000000 aisdc-1.1.3/tests/safemodel/test_saferandomforestclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4902 2024-04-24 15:57:32.000000 aisdc-1.1.3/tests/safemodel/test_safesvc.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      399 2024-04-24 15:57:32.000000 aisdc-1.1.3/tests/safemodel/test_safetf.py
```

### Comparing `aisdc-1.1.2/LICENSE` & `aisdc-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aisdc-1.1.2/PKG-INFO` & `aisdc-1.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,71 @@
 Metadata-Version: 2.1
 Name: aisdc
-Version: 1.1.2
+Version: 1.1.3
 Summary: Tools for the statistical disclosure control of machine learning models
 Home-page: https://github.com/AI-SDC/AI-SDC
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,machine-learning,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.9,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dictdiffer~=0.9.0
-Requires-Dist: fpdf~=1.7.2
-Requires-Dist: joblib~=1.3
-Requires-Dist: multiprocess~=0.70.15
-Requires-Dist: numpy~=1.23.1
-Requires-Dist: pandas~=1.5.3
-Requires-Dist: scikit_learn~=1.1.3
-Requires-Dist: scipy~=1.10
-Requires-Dist: tensorflow-probability==0.15.0; python_version < "3.9"
-Requires-Dist: tensorflow~=2.10.0; python_version < "3.9"
-Requires-Dist: tensorflow~=2.12.0; python_version >= "3.9"
-Requires-Dist: tensorflow_privacy==0.7.3; python_version < "3.9"
-Requires-Dist: tensorflow_privacy==0.8.10; python_version >= "3.9"
-Requires-Dist: uuid~=1.30
-Requires-Dist: pypdf~=3.16
-Requires-Dist: xgboost~=1.7.6
-Requires-Dist: statsmodels==0.13.5
-Requires-Dist: acro==0.4.3
+Requires-Dist: acro==0.4.5
+Requires-Dist: fpdf
+Requires-Dist: pypdf
+Requires-Dist: multiprocess
+Requires-Dist: scikit-learn
+Requires-Dist: xgboost
+Provides-Extra: safemodel
+Requires-Dist: tensorflow<2.15,>=2.14; extra == "safemodel"
+Requires-Dist: tensorflow-privacy==0.9.0; extra == "safemodel"
+Requires-Dist: dictdiffer; extra == "safemodel"
+Provides-Extra: doc
+Requires-Dist: tensorflow<2.15,>=2.14; extra == "doc"
+Requires-Dist: tensorflow-privacy==0.9.0; extra == "doc"
+Requires-Dist: dictdiffer; extra == "doc"
+Requires-Dist: numpydoc; extra == "doc"
+Requires-Dist: sphinx-autopackagesummary; extra == "doc"
+Requires-Dist: sphinx-issues; extra == "doc"
+Requires-Dist: sphinx-prompt; extra == "doc"
+Requires-Dist: sphinx-rtd-theme; extra == "doc"
+Requires-Dist: sphinx; extra == "doc"
+Provides-Extra: test
+Requires-Dist: tensorflow<2.15,>=2.14; extra == "test"
+Requires-Dist: tensorflow-privacy==0.9.0; extra == "test"
+Requires-Dist: dictdiffer; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://opensource.org/licenses/MIT)
 [![Latest Version](https://img.shields.io/github/v/release/AI-SDC/AI-SDC?style=flat)](https://github.com/AI-SDC/AI-SDC/releases)
 [![DOI](https://zenodo.org/badge/518801511.svg)](https://zenodo.org/badge/latestdoi/518801511)
-[![codecov](https://codecov.io/gh/AI-SDC/AI-SDC/branch/development/graph/badge.svg?token=AXX2XCXUNU)](https://codecov.io/gh/AI-SDC/AI-SDC)
+[![codecov](https://codecov.io/gh/AI-SDC/AI-SDC/branch/main/graph/badge.svg?token=AXX2XCXUNU)](https://codecov.io/gh/AI-SDC/AI-SDC)
 [![Python versions](https://img.shields.io/pypi/pyversions/aisdc.svg)](https://pypi.org/project/aisdc)
 
 # AI-SDC
 
 A collection of tools and resources for managing the statistical disclosure control of trained machine learning models. For a brief introduction, see [Smith et al. (2022)](https://doi.org/10.48550/arXiv.2212.01233).
 
 ### User Guides
 
-A collection of user guides can be found in the 'user_stories' folder of this repository. These guides include configurable examples from the perspective of both a researcher and a TRE, with separate scripts for each. Instructions on how to use each of these scripts and which scripts to use are included in the README of the ['user_stories'](https://github.com/AI-SDC/AI-SDC/tree/user_story_visibility/user_stories) folder.
+A collection of user guides can be found in the 'user_stories' folder of this repository. These guides include configurable examples from the perspective of both a researcher and a TRE, with separate scripts for each. Instructions on how to use each of these scripts and which scripts to use are included in the README of the [`user_stories`](./user_stories) folder.
 
 ## Content
 
 * `aisdc`
     - `attacks` Contains a variety of privacy attacks on machine learning models, including membership and attribute inference.
     - `preprocessing` Contains preprocessing modules for test datasets.
     - `safemodel` The safemodel package is an open source wrapper for common machine learning models. It is designed for use by researchers in Trusted Research Environments (TREs) where disclosure control methods must be implemented. Safemodel aims to give researchers greater confidence that their models are more compliant with disclosure control.
@@ -72,63 +80,56 @@
 * `risk_examples` Contains hypothetical examples of data leakage through machine learning models as described in the [Green Paper](https://doi.org/10.5281/zenodo.6896214).
 * `tests` Contains unit tests.
 
 ## Documentation
 
 Documentation is hosted here: https://ai-sdc.github.io/AI-SDC/
 
-## Quick Start
+## Installation / End-user
 
-### Development
-
-Clone the repository and install the dependencies (safest in a virtual env):
+[![PyPI package](https://img.shields.io/pypi/v/aisdc.svg)](https://pypi.org/project/aisdc)
 
-```
-$ git clone https://github.com/AI-SDC/AI-SDC.git
-$ cd AI-SDC
-$ pip install -r requirements.txt
-```
+Install `aisdc` (safest in a virtual env) and manually copy the [`examples`](examples/) and [`example_notebooks`](example_notebooks/).
 
-Then run the tests:
+To install only the base package, which includes the attacks used for assessing privacy:
 
 ```
-$ pip install pytest
-$ pytest .
+$ pip install aisdc
 ```
 
-Or run an example:
+To install the base package and the safemodel package, which includes defensive wrappers for popular ML frameworks including [scikit-learn](https://scikit-learn.org) and [Keras](https://keras.io):
 
 ```
-$ python -m examples.lira_attack_example
+$ pip install aisdc[safemodel]
 ```
 
-### Installation / End-user
+## Running
 
-[![PyPI package](https://img.shields.io/pypi/v/aisdc.svg)](https://pypi.org/project/aisdc)
+To run an example, simply execute the desired script or start up `jupyter notebook` and run one of the notebooks.
 
-Install `aisdc` (safest in a virtual env) and manually copy the `examples` and `example_notebooks`.
+For example, to run the `lira_attack_example.py`:
 
 ```
-$ pip install aisdc
+$ python -m lira_attack_example
 ```
 
-Then to run an example:
+## Development
+
+Clone the repository and install the local package including all dependencies (safest in a virtual env):
 
 ```
-$ python attribute_inference_example.py
+$ git clone https://github.com/AI-SDC/AI-SDC.git
+$ cd AI-SDC
+$ pip install .[test]
 ```
 
-Or start up `jupyter notebook` and run an example.
-
-Alternatively, you can clone the repo and install:
+Then run the tests:
 
 ```
-$ git clone https://github.com/AI-SDC/AI-SDC.git
-$ cd AI-SDC
-$ pip install .
+$ pytest .
 ```
 
 ---
 
-This work was funded by UK Research and Innovation Grant Number MC_PC_21033 as part of Phase 1 of the DARE UK (Data and Analytics Research Environments UK) programme (https://dareuk.org.uk/), delivered in partnership with HDR UK and ADRUK. The specific project was Guidelines and Resources for AI Model Access from TrusTEd Research environments (GRAIMATTER).­ This project has also been supported by MRC and EPSRC [grant number MR/S010351/1]: PICTURES.
+This work was funded by UK Research and Innovation under Grant Numbers MC_PC_21033  and MC_PC_23006 as part of Phase 1 of the DARE UK (Data and Analytics Research Environments UK) programme (https://dareuk.org.uk/), delivered in partnership with Health Data Research UK (HDR UK) and Administrative Data Research UK (ADR UK). The specific projects were Semi-Automatic checking of Research Outputs (SACRO -MC_PC_23006) and   Guidelines and Resources for AI Model Access from TrusTEd Research environments (GRAIMATTER - MC_PC_21033).­ This project has also been supported by MRC and EPSRC [grant number MR/S010351/1]: PICTURES.
 
 <img src="docs/source/images/UK_Research_and_Innovation_logo.svg" width="20%" height="20%" padding=20/> <img src="docs/source/images/health-data-research-uk-hdr-uk-logo-vector.png" width="10%" height="10%" padding=20/> <img src="docs/source/images/logo_print.png" width="15%" height="15%" padding=20/>
```

### Comparing `aisdc-1.1.2/README.md` & `aisdc-1.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://opensource.org/licenses/MIT)
 [![Latest Version](https://img.shields.io/github/v/release/AI-SDC/AI-SDC?style=flat)](https://github.com/AI-SDC/AI-SDC/releases)
 [![DOI](https://zenodo.org/badge/518801511.svg)](https://zenodo.org/badge/latestdoi/518801511)
-[![codecov](https://codecov.io/gh/AI-SDC/AI-SDC/branch/development/graph/badge.svg?token=AXX2XCXUNU)](https://codecov.io/gh/AI-SDC/AI-SDC)
+[![codecov](https://codecov.io/gh/AI-SDC/AI-SDC/branch/main/graph/badge.svg?token=AXX2XCXUNU)](https://codecov.io/gh/AI-SDC/AI-SDC)
 [![Python versions](https://img.shields.io/pypi/pyversions/aisdc.svg)](https://pypi.org/project/aisdc)
 
 # AI-SDC
 
 A collection of tools and resources for managing the statistical disclosure control of trained machine learning models. For a brief introduction, see [Smith et al. (2022)](https://doi.org/10.48550/arXiv.2212.01233).
 
 ### User Guides
 
-A collection of user guides can be found in the 'user_stories' folder of this repository. These guides include configurable examples from the perspective of both a researcher and a TRE, with separate scripts for each. Instructions on how to use each of these scripts and which scripts to use are included in the README of the ['user_stories'](https://github.com/AI-SDC/AI-SDC/tree/user_story_visibility/user_stories) folder.
+A collection of user guides can be found in the 'user_stories' folder of this repository. These guides include configurable examples from the perspective of both a researcher and a TRE, with separate scripts for each. Instructions on how to use each of these scripts and which scripts to use are included in the README of the [`user_stories`](./user_stories) folder.
 
 ## Content
 
 * `aisdc`
     - `attacks` Contains a variety of privacy attacks on machine learning models, including membership and attribute inference.
     - `preprocessing` Contains preprocessing modules for test datasets.
     - `safemodel` The safemodel package is an open source wrapper for common machine learning models. It is designed for use by researchers in Trusted Research Environments (TREs) where disclosure control methods must be implemented. Safemodel aims to give researchers greater confidence that their models are more compliant with disclosure control.
@@ -29,63 +29,56 @@
 * `risk_examples` Contains hypothetical examples of data leakage through machine learning models as described in the [Green Paper](https://doi.org/10.5281/zenodo.6896214).
 * `tests` Contains unit tests.
 
 ## Documentation
 
 Documentation is hosted here: https://ai-sdc.github.io/AI-SDC/
 
-## Quick Start
+## Installation / End-user
 
-### Development
-
-Clone the repository and install the dependencies (safest in a virtual env):
+[![PyPI package](https://img.shields.io/pypi/v/aisdc.svg)](https://pypi.org/project/aisdc)
 
-```
-$ git clone https://github.com/AI-SDC/AI-SDC.git
-$ cd AI-SDC
-$ pip install -r requirements.txt
-```
+Install `aisdc` (safest in a virtual env) and manually copy the [`examples`](examples/) and [`example_notebooks`](example_notebooks/).
 
-Then run the tests:
+To install only the base package, which includes the attacks used for assessing privacy:
 
 ```
-$ pip install pytest
-$ pytest .
+$ pip install aisdc
 ```
 
-Or run an example:
+To install the base package and the safemodel package, which includes defensive wrappers for popular ML frameworks including [scikit-learn](https://scikit-learn.org) and [Keras](https://keras.io):
 
 ```
-$ python -m examples.lira_attack_example
+$ pip install aisdc[safemodel]
 ```
 
-### Installation / End-user
+## Running
 
-[![PyPI package](https://img.shields.io/pypi/v/aisdc.svg)](https://pypi.org/project/aisdc)
+To run an example, simply execute the desired script or start up `jupyter notebook` and run one of the notebooks.
 
-Install `aisdc` (safest in a virtual env) and manually copy the `examples` and `example_notebooks`.
+For example, to run the `lira_attack_example.py`:
 
 ```
-$ pip install aisdc
+$ python -m lira_attack_example
 ```
 
-Then to run an example:
+## Development
+
+Clone the repository and install the local package including all dependencies (safest in a virtual env):
 
 ```
-$ python attribute_inference_example.py
+$ git clone https://github.com/AI-SDC/AI-SDC.git
+$ cd AI-SDC
+$ pip install .[test]
 ```
 
-Or start up `jupyter notebook` and run an example.
-
-Alternatively, you can clone the repo and install:
+Then run the tests:
 
 ```
-$ git clone https://github.com/AI-SDC/AI-SDC.git
-$ cd AI-SDC
-$ pip install .
+$ pytest .
 ```
 
 ---
 
-This work was funded by UK Research and Innovation Grant Number MC_PC_21033 as part of Phase 1 of the DARE UK (Data and Analytics Research Environments UK) programme (https://dareuk.org.uk/), delivered in partnership with HDR UK and ADRUK. The specific project was Guidelines and Resources for AI Model Access from TrusTEd Research environments (GRAIMATTER).­ This project has also been supported by MRC and EPSRC [grant number MR/S010351/1]: PICTURES.
+This work was funded by UK Research and Innovation under Grant Numbers MC_PC_21033  and MC_PC_23006 as part of Phase 1 of the DARE UK (Data and Analytics Research Environments UK) programme (https://dareuk.org.uk/), delivered in partnership with Health Data Research UK (HDR UK) and Administrative Data Research UK (ADR UK). The specific projects were Semi-Automatic checking of Research Outputs (SACRO -MC_PC_23006) and   Guidelines and Resources for AI Model Access from TrusTEd Research environments (GRAIMATTER - MC_PC_21033).­ This project has also been supported by MRC and EPSRC [grant number MR/S010351/1]: PICTURES.
 
 <img src="docs/source/images/UK_Research_and_Innovation_logo.svg" width="20%" height="20%" padding=20/> <img src="docs/source/images/health-data-research-uk-hdr-uk-logo-vector.png" width="10%" height="10%" padding=20/> <img src="docs/source/images/logo_print.png" width="15%" height="15%" padding=20/>
```

### Comparing `aisdc-1.1.2/aisdc/attacks/attack.py` & `aisdc-1.1.3/aisdc/attacks/attack.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.1.2/aisdc/attacks/attack_report_formatter.py` & `aisdc-1.1.3/aisdc/attacks/attack_report_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,16 +257,17 @@
 
         # if model is instance based, it is automatically disclosive. Assign max score
         if self._is_instance_based_model(self.INSTANCE_MODEL_WEIGHTING_SCORE):
             summarised_score = self.INSTANCE_MODEL_WEIGHTING_SCORE
 
         output = {}
 
-        msg = "Final score (scale of 0-5, where 0 is least disclosive and 5 is recommend rejection)"
-        output[msg] = summarised_score
+        # msg = "Final score (scale of 0-5, where 0 is least disclosive and 5 is recommend
+        # rejection)"
+        # output[msg] = summarised_score
 
         return output
 
     def __str__(self):
         return "Final Recommendation"
 
 
@@ -451,25 +452,14 @@
         self.attack_json_filename = None
         self.model_name_from_target = None
 
         self.immediate_rejection = []
         self.support_rejection = []
         self.support_release = []
 
-    def _pretty_print(self, report: dict, title) -> str:
-        """Function that formats JSON code to make it more readable for TREs."""
-
-        returned_string = str(title) + "\n"
-
-        for key in report.keys():
-            returned_string = returned_string + key + "\n"
-            returned_string = returned_string + pprint.pformat(report[key]) + "\n\n"
-
-        return returned_string
-
     def _process_target_json(self):
         """Function that creates a summary of a target model JSON file."""
 
         model_params_of_interest = [
             "C",
             "kernel",
             "n_neighbors",
@@ -509,14 +499,25 @@
             filepath = os.path.split(os.path.abspath(self.target_json_filename))[0]
             self.model_name_from_target = os.path.join(
                 filepath, json_report["model_path"]
             )
 
         self.text_out.append(output_string)
 
+    def pretty_print(self, report: dict, title) -> str:
+        """Function that formats JSON code to make it more readable for TREs."""
+
+        returned_string = str(title) + "\n"
+
+        for key in report.keys():
+            returned_string = returned_string + key + "\n"
+            returned_string = returned_string + pprint.pformat(report[key]) + "\n\n"
+
+        return returned_string
+
     def process_attack_target_json(
         self, attack_filename: str, target_filename: str = None
     ):
         """Function that creates a neat summary of an attack JSON file."""
         self.attack_json_filename = attack_filename
 
         with open(attack_filename, encoding="utf-8") as f:
@@ -537,15 +538,15 @@
             output = m.process_dict()
             returned = m.get_recommendation()
 
             self.immediate_rejection += returned[0]
             self.support_rejection += returned[1]
             self.support_release += returned[2]
 
-        output_string = self._pretty_print(output, "ATTACK JSON RESULTS")
+        output_string = self.pretty_print(output, "ATTACK JSON RESULTS")
 
         self.text_out.append(output_string)
 
         bucket_text = "Immediate rejection recommended for the following reason:\n"
         if len(self.immediate_rejection) > 0:
             for reason in self.immediate_rejection:
                 bucket_text += str(reason) + "\n"
```

### Comparing `aisdc-1.1.2/aisdc/attacks/attribute_attack.py` & `aisdc-1.1.3/aisdc/attacks/attribute_attack.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,15 @@
 COLOR_A: str = "#86bf91"  # training set plot colour
 COLOR_B: str = "steelblue"  # testing set plot colour
 
 
 class AttributeAttack(Attack):
     """Class to wrap the attribute inference attack code."""
 
-    # pylint: disable=too-many-instance-attributes
-
-    def __init__(  # pylint: disable = too-many-arguments, too-many-locals
+    def __init__(  # pylint: disable = too-many-arguments
         self,
         output_dir: str = "output_attribute",
         report_name: str = "aia_report",
         n_cpu: int = max(1, mp.cpu_count() - 1),
         attack_config_json_file_name: str = None,
         target_path: str = None,
     ) -> None:
@@ -429,15 +427,15 @@
     """
     Performs a brute force attribute inference attack by computing the target
     model confidence scores for every value in the list and making an inference
     if there is a unique highest confidence score that exceeds attack_threshold.
     """
     logger.debug("Brute force attacking categorical features")
     args = [(target, feature_id, attack_threshold) for feature_id in features]
-    with mp.Pool(processes=n_cpu) as pool:  # pylint:disable=not-callable
+    with mp.Pool(processes=n_cpu) as pool:
         results = pool.starmap(_infer_categorical, args)
     return results
 
 
 def _get_bounds_risk_for_sample(  # pylint: disable=too-many-locals,too-many-arguments
     target_model: BaseEstimator,
     feat_id: int,
@@ -565,15 +563,15 @@
             target.features[feature_id]["name"],
             feature_id,
             target.x_train,
             target.x_test,
         )
         for feature_id in features
     ]
-    with mp.Pool(processes=n_cpu) as pool:  # pylint:disable=not-callable
+    with mp.Pool(processes=n_cpu) as pool:
         results = pool.starmap(_get_bounds_risk, args)
     return results
 
 
 def _attribute_inference(target: Target, n_cpu: int) -> dict:
     """Execute attribute inference attacks on a target given a trained model."""
     # brute force attack categorical attributes using dataset unique values
```

### Comparing `aisdc-1.1.2/aisdc/attacks/failfast.py` & `aisdc-1.1.3/aisdc/attacks/failfast.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """Failfast.py - class to evaluate metric for fail fast option."""
 
 from __future__ import annotations
 
 from typing import Any
 
 
-class FailFast:  # pylint: disable=too-many-instance-attributes
+class FailFast:
     """Class to check attack being successful or not for a given metric
     Note: An object of a FailFast is stateful and instance members
     (success_count and fail_count) will preserve values
     across repetitions for a test. For the new test
     a new object will require to be instantiated.
     """
 
     def __init__(self, attack_obj: Any):
         self.metric_name = attack_obj.attack_metric_success_name
         self.metric_success_thresh = attack_obj.attack_metric_success_thresh
         self.comp_type = attack_obj.attack_metric_success_comp_type
         self.success_count = 0
         self.fail_count = 0
 
-    # pylint: disable=too-many-branches
     def check_attack_success(self, metric_dict: dict) -> bool:
         """A function to check if attack was successful for a given metric.
 
         Parameters
         ----------
         metric_dict : dict
             a dictionary with all computed metric values
```

### Comparing `aisdc-1.1.2/aisdc/attacks/likelihood_attack.py` & `aisdc-1.1.3/aisdc/attacks/likelihood_attack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Likelihood testing scenario from https://arxiv.org/pdf/2112.03570.pdf."""
+
 # pylint: disable = invalid-name
 # pylint: disable = too-many-branches
 
 from __future__ import annotations
 
 import argparse
 import importlib
@@ -59,27 +60,27 @@
         logit(p)
 
     Notes
     -----
     If p is close to 0 or 1, evaluating the log will result in numerical instabilities.
     This code thresholds p at EPS and 1 - EPS where EPS defaults at 1e-16.
     """
-    if p > 1 - EPS:
+    if p > 1 - EPS:  # pylint:disable=consider-using-min-builtin
         p = 1 - EPS
     p = max(p, EPS)
     li = np.log(p / (1 - p))
     return li
 
 
 class LIRAAttack(Attack):
     """The main LIRA Attack class."""
 
     # pylint: disable=too-many-instance-attributes
 
-    def __init__(  # pylint: disable = too-many-arguments, too-many-locals
+    def __init__(  # pylint: disable = too-many-arguments
         self,
         n_shadow_models: int = 100,
         p_thresh: float = 0.05,
         output_dir: str = "outputs_lira",
         report_name: str = "report_lira",
         training_data_filename: str = None,
         test_data_filename: str = None,
@@ -187,15 +188,15 @@
         1. Replacing the values in y_train with their position in
         target.model.classes (will normally result in no change)
         2. Removing from the test set any rows corresponding to classes that
         are not in the training set.
         """
         logger = logging.getLogger("_check_and_update_dataset")
         y_train_new = []
-        classes = list(target.model.classes_)  # pylint: disable = protected-access
+        classes = list(target.model.classes_)
         for y in target.y_train:
             y_train_new.append(classes.index(y))
 
         target.y_train = np.array(y_train_new, int)
 
         logger.info(
             "new ytrain has values and counts: %s",
@@ -394,15 +395,15 @@
         mia_scores = np.array(mia_scores)
         mia_labels = np.array(mia_labels)
         y_pred_proba, y_test = metrics.get_probabilities(
             mia_clf, mia_scores, mia_labels, permute_rows=True
         )
         self.attack_metrics = [metrics.get_metrics(y_pred_proba, y_test)]
 
-    def example(self) -> None:  # pylint: disable = too-many-locals
+    def example(self) -> None:
         """Runs an example attack using data from sklearn.
 
         Generates example data, trains a classifier and tuns the attack
         """
         X, y = load_breast_cancer(return_X_y=True, as_frame=False)
         train_X, test_X, train_y, test_y = train_test_split(
             X, y, test_size=0.5, stratify=y
```

### Comparing `aisdc-1.1.2/aisdc/attacks/multiple_attacks.py` & `aisdc-1.1.3/aisdc/attacks/multiple_attacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """
 An entry point to run multiple attacks including MIA (worst-case and LIRA)
 and attribute inference attack using a single configuration file
 with multiple attack configuration.
 """
+
 from __future__ import annotations
 
 import argparse
 import json
 import logging
 import os
 import uuid
 from typing import Any
 
 from aisdc.attacks.attack import Attack
-from aisdc.attacks.attribute_attack import (
-    AttributeAttack,  # pylint: disable = import-error
-)
-from aisdc.attacks.likelihood_attack import LIRAAttack  # pylint: disable = import-error
+from aisdc.attacks.attribute_attack import AttributeAttack
+from aisdc.attacks.likelihood_attack import LIRAAttack
 from aisdc.attacks.target import Target
-from aisdc.attacks.worst_case_attack import (
-    WorstCaseAttack,  # pylint: disable = import-error
-)
+from aisdc.attacks.worst_case_attack import WorstCaseAttack
 
 
 class MultipleAttacks(Attack):
     """Class to wrap the MIA and AIA attack codes."""
 
     def __init__(
         self,
@@ -84,15 +81,15 @@
                     attack_obj.attack(target)
 
                 if attack_obj is not None:
                     _ = attack_obj.make_report()
         logger.info("Finished running attacks")
 
 
-class ConfigFile:  # pylint: disable = too-few-public-methods
+class ConfigFile:
     """Module that creates a single JSON configuration file."""
 
     def __init__(
         self,
         filename: str = None,
     ) -> None:
         self.filename = filename
```

### Comparing `aisdc-1.1.2/aisdc/attacks/report.py` & `aisdc-1.1.3/aisdc/attacks/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Code for automatic report generation."""
+
 import abc
 import json
 import os
 
 import numpy as np
 import pylab as plt
 from fpdf import FPDF
@@ -133,16 +134,16 @@
     """Create a roc_plot for a single experiment."""
     plt.figure()
     plt.plot([0, 1], [0, 1], "k--")
     plt.plot(metrics["fpr"], metrics["tpr"], "r", linewidth=2)
     plt.xscale("log")
     plt.yscale("log")
     plt.grid()
-    plt.xlabel("True Positive Rate")
-    plt.ylabel("False Positive Rate")
+    plt.ylabel("True Positive Rate")
+    plt.xlabel("False Positive Rate")
     plt.tight_layout()
     plt.savefig(save_name)
 
 
 def _roc_plot(metrics, dummy_metrics, save_name):
     """Create a roc plot for multiple repetitions."""
     plt.figure()
```

### Comparing `aisdc-1.1.2/aisdc/attacks/structural_attack.py` & `aisdc-1.1.3/aisdc/attacks/structural_attack.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,16 @@
                 and not model.bootstrap
             )
         ):
             unnecessary_risk = 1
 
     elif isinstance(model, XGBClassifier):
         n_estimators = model.n_estimators
+        if n_estimators is None:
+            n_estimators = 1000
         if (
             (
                 max_depth > 3.5
                 and 3.5 < n_estimators <= 12.5
                 and model.min_child_weight <= 1.5
             )
             or (max_depth > 3.5 and n_estimators > 12.5 and model.min_child_weight <= 3)
@@ -189,15 +191,15 @@
 
 
 class StructuralAttack(Attack):
     """Class to wrap a number of attacks based on the static structure of a model."""
 
     # pylint: disable=too-many-instance-attributes
 
-    def __init__(  # pylint: disable = too-many-arguments, too-many-locals
+    def __init__(  # pylint: disable = too-many-arguments
         self,
         attack_config_json_file_name: str = None,
         risk_appetite_config: str = "default",
         target_path: str = None,
         output_dir="outputs_structural",
         report_name="report_structural",
     ) -> None:
```

### Comparing `aisdc-1.1.2/aisdc/attacks/target.py` & `aisdc-1.1.3/aisdc/attacks/target.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.1.2/aisdc/attacks/worst_case_attack.py` & `aisdc-1.1.3/aisdc/attacks/worst_case_attack.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
         super().__init__()
         self.n_reps = n_reps
         self.reproduce_split = reproduce_split
         if isinstance(reproduce_split, int):
             reproduce_split = [reproduce_split] + [
                 x**2 for x in range(reproduce_split, reproduce_split + n_reps - 1)
-            ]  # pylint: disable = line-too-long
+            ]
         else:
             reproduce_split = list(
                 dict.fromkeys(reproduce_split)
             )  # remove potential duplicates
             if len(reproduce_split) == n_reps:
                 pass
             elif len(reproduce_split) > n_reps:
@@ -236,15 +236,15 @@
         Filenames for the saved prediction files to be specified in the arguments provided
         in the constructor
         """
         train_preds = np.loadtxt(self.training_preds_filename, delimiter=",")
         test_preds = np.loadtxt(self.test_preds_filename, delimiter=",")
         self.attack_from_preds(train_preds, test_preds)
 
-    def attack_from_preds(  # pylint: disable=too-many-locals
+    def attack_from_preds(
         self,
         train_preds: np.ndarray,
         test_preds: np.ndarray,
         train_correct: np.ndarray = None,
         test_correct: np.ndarray = None,
     ) -> None:
         """
@@ -433,17 +433,17 @@
             ]
 
             m = attack_metrics[0]
             _, auc_std = metrics.auc_p_val(
                 0.5, m["n_pos_test_examples"], m["n_neg_test_examples"]
             )
 
-            global_metrics[
-                "null_auc_3sd_range"
-            ] = f"{0.5 - 3*auc_std:.4f} -> {0.5 + 3*auc_std:.4f}"
+            global_metrics["null_auc_3sd_range"] = (
+                f"{0.5 - 3*auc_std:.4f} -> {0.5 + 3*auc_std:.4f}"
+            )
             global_metrics["n_sig_auc_p_vals"] = self._get_n_significant(
                 auc_p_vals, self.p_thresh
             )
             global_metrics["n_sig_auc_p_vals_corrected"] = self._get_n_significant(
                 auc_p_vals, self.p_thresh, bh_fdr_correction=True
             )
 
@@ -459,17 +459,15 @@
 
     def _get_n_significant(self, p_val_list, p_thresh, bh_fdr_correction=False):
         """
         Helper method to determine if values within a list of p-values are significant at
         p_thresh. Can perform multiple testing correction.
         """
         if not bh_fdr_correction:
-            return sum(
-                1 for p in p_val_list if p <= p_thresh
-            )  # pylint: disable = consider-using-generator
+            return sum(1 for p in p_val_list if p <= p_thresh)
         p_val_list = np.asarray(sorted(p_val_list))
         n_vals = len(p_val_list)
         hoch_vals = np.array([(k / n_vals) * P_THRESH for k in range(1, n_vals + 1)])
         bh_sig_list = p_val_list <= hoch_vals
         if any(bh_sig_list):
             n_sig_bh = (np.where(bh_sig_list)[0]).max() + 1
         else:
@@ -599,36 +597,36 @@
         attack_metrics_experiment = {}
         attack_metrics_instances = {}
 
         for rep, _ in enumerate(self.attack_metrics):
             attack_metrics_instances["instance_" + str(rep)] = self.attack_metrics[rep]
 
         attack_metrics_experiment["attack_instance_logger"] = attack_metrics_instances
-        attack_metrics_experiment[
-            "attack_metric_failfast_summary"
-        ] = self.attack_metric_failfast_summary.get_attack_summary()
+        attack_metrics_experiment["attack_metric_failfast_summary"] = (
+            self.attack_metric_failfast_summary.get_attack_summary()
+        )
 
         return attack_metrics_experiment
 
     def _get_dummy_attack_metrics_experiments_instances(self) -> dict:
         """Constructs the metadata object, after attacks."""
         dummy_attack_metrics_experiments = {}
 
         for exp_rep, _ in enumerate(self.dummy_attack_metrics):
             temp_dummy_attack_metrics = self.dummy_attack_metrics[exp_rep]
             dummy_attack_metric_instances = {}
             for rep, _ in enumerate(temp_dummy_attack_metrics):
-                dummy_attack_metric_instances[
-                    "instance_" + str(rep)
-                ] = temp_dummy_attack_metrics[rep]
+                dummy_attack_metric_instances["instance_" + str(rep)] = (
+                    temp_dummy_attack_metrics[rep]
+                )
             temp = {}
             temp["attack_instance_logger"] = dummy_attack_metric_instances
-            temp[
-                "attack_metric_failfast_summary"
-            ] = self.dummy_attack_metric_failfast_summary[exp_rep].get_attack_summary()
+            temp["attack_metric_failfast_summary"] = (
+                self.dummy_attack_metric_failfast_summary[exp_rep].get_attack_summary()
+            )
             dummy_attack_metrics_experiments[
                 "dummy_attack_metrics_experiment_" + str(exp_rep)
             ] = temp
 
         return dummy_attack_metrics_experiments
 
     def make_report(self) -> dict:
@@ -639,17 +637,17 @@
         output["log_id"] = str(uuid.uuid4())
         output["log_time"] = datetime.now().strftime("%d/%m/%Y %H:%M:%S")
 
         self._construct_metadata()
         output["metadata"] = self.metadata
 
         output["attack_experiment_logger"] = self._get_attack_metrics_instances()
-        output[
-            "dummy_attack_experiments_logger"
-        ] = self._get_dummy_attack_metrics_experiments_instances()
+        output["dummy_attack_experiments_logger"] = (
+            self._get_dummy_attack_metrics_experiments_instances()
+        )
 
         report_dest = os.path.join(self.output_dir, self.report_name)
         json_attack_formatter = GenerateJSONModule(report_dest + ".json")
         json_report = report.create_json_report(output)
         json_attack_formatter.add_attack_output(json_report, "WorstCaseAttack")
 
         pdf_report = report.create_mia_report(output)
```

### Comparing `aisdc-1.1.2/aisdc/metrics.py` & `aisdc-1.1.3/aisdc/metrics.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.1.2/aisdc/preprocessing/loaders.py` & `aisdc-1.1.3/aisdc/preprocessing/loaders.py`

 * *Files 18% similar despite different names*

```diff
@@ -68,15 +68,14 @@
     The following datasets are available:
     mimic2-iaccd (requires data download)
     in-hospital-mortality (requires data download)
     medical-mnist-ab-v-br-100 (requires data download)
     medical-mnist-ab-v-br-500 (requires data download)
     medical-mnist-all-100 (requires data download)
     indian liver (requires data download)
-    texas hospitals 10 (requires data download)
     synth-ae (requires data download)
     synth-ae-small (requires data download)
     nursery (downloads automatically)
     iris (available out of the box via sklearn)
 
     Datasets can be normalised by adding the following prefixes:
     standard: standardises all columns to have zero mean and unit variance.
@@ -139,18 +138,26 @@
         )
     if dataset_name == "indian liver":
         return _indian_liver(data_folder)
     if dataset_name == "synth-ae":
         return _synth_ae(data_folder)
     if dataset_name == "synth-ae-small":
         return _synth_ae(data_folder, 200)
+    if dataset_name == "synth-ae-large":
+        return _synth_ae(data_folder, 500000)
+    if dataset_name == "synth-ae-extra-large":
+        return _synth_ae(data_folder, 2000000)
+    if dataset_name == "synth-ae-XXL":
+        return _synth_ae(data_folder, 50000000)
     if dataset_name == "nursery":
         return _nursery()
     if dataset_name == "iris":
         return _iris()
+    if dataset_name == "RDMP":
+        return _RDMP(data_folder)
     raise UnknownDataset(dataset_name)
 
 
 def _iris() -> Tuple[pd.DataFrame, pd.DataFrame]:
     """Sklearn iris data - just first two classes."""
     X, y = load_iris(return_X_y=True, as_frame=True)
     X = X[y < 2]
@@ -371,14 +378,15 @@
     In-hospital mortality data from this study:
         https://datadryad.org/stash/dataset/doi:10.5061/dryad.0p2ngf1zd.
     """
     # Check the data has been downloaded. If not throw an exception with instructions on how to
     # download, and where to store
     files = ["data01.csv", "doi_10.5061_dryad.0p2ngf1zd__v5.zip"]
     file_path = [os.path.join(data_folder, f) for f in files]
+    print(file_path)
 
     if not any(  # pylint: disable=use-a-generator
         [os.path.exists(fp) for fp in file_path]
     ):  # pylint: disable=use-a-generator
         help_message = f"""
 Data file {file_path[0]} or {file_path[1]} does not exist. Please download the file from:
 https://datadryad.org/stash/dataset/doi:10.5061/dryad.0p2ngf1zd
@@ -454,192 +462,199 @@
     label_encoder = LabelEncoder()
     encoded_labels = label_encoder.fit_transform(y.values)
     y = pd.DataFrame({"censor_flag": encoded_labels})
 
     return (X, y)
 
 
-def _texas_hospitals(
+def _RDMP(  # pylint: disable=too-many-locals, too-many-statements
     data_folder: str,
-) -> Tuple[pd.DataFrame, pd.DataFrame]:  # pragma: no cover
-    # pylint: disable=too-many-statements, too-many-locals
-    """
-    Texas Hospitals Dataset
-    https://www.dshs.texas.gov/texas-health-care-information-collection/health-data-researcher-information/texas-inpatient-public-use # pylint: disable=line-too-long.
-
-    Download the tab-delimited files for each quarter from
-    2006, 2007, 2008 and 2009.
-    Note: This data is free to download.
-    """
-    file_list = [
-        "PUDF 1Q2006 tab-delimited.zip",
-        "PUDF 1Q2007 tab-delimited.zip",
-        "PUDF 1Q2009 tab-delimited.zip",
-        "PUDF 2Q2006 tab-delimited.zip",
-        "PUDF 2Q2007 tab-delimited.zip",
-        "PUDF 2Q2009 tab-delimited.zip",
-        "PUDF 3Q2006 tab-delimited.zip",
-        "PUDF 3Q2007 tab-delimited.zip",
-        "PUDF 4Q2006 tab-delimited.zip",
-        "PUDF 4Q2007 tab-delimited.zip",
-        "PUDF 4Q2009 tab-delimited.zip",
-        "PUDF1Q08_update_tab.zip",
-        "PUDF2Q08_update_tab.zip",
-        "PUDF3Q08_update_tab.zip",
-    ]
-    files_path = [os.path.join(data_folder, f) for f in file_list]
-
-    found = [os.path.exists(file_path) for file_path in files_path]
-    not_found = [file_path for file_path in files_path if not os.path.exists(file_path)]
+) -> Tuple[pd.DataFrame, pd.DataFrame]:
+    def find_age(row):
+        date_ = pd.to_datetime("01/06/2020")
+        if row.date_of_death != row.date_of_death:
+            age = np.floor((date_ - row.date_of_birth).days / 365.25)
+        else:
+            age = np.floor((row.date_of_death - row.date_of_birth).days / 365.25)
+        return age
 
-    processed_data_file = "texas_data10_rm_binary.csv"
-    if not all(found):
-        help_message = f"""
-    Some or all data files do not exist. Please accept their terms & conditions,then download the
-    tab delimited files from each quarter during 2006-2009 from:
-    https://www.dshs.texas.gov/THCIC/Hospitals/Download.shtm
-and place it in the correct folder.
+    def hospital_days(row):
+        if row.DischargeDate == row.DischargeDate:
+            t = row.DischargeDate - row.AdmissionDate
+            days = t.days + round(((t.seconds / 60) / 60) / 24)
+        else:
+            days = 0
+        return days
 
-    Missing files are:
-    {not_found}
-        """
-        raise DataNotAvailable(help_message)
+    processed_data_file = "rdmp_binary.csv"
+    os.path.join(data_folder, "RDMP")
+    if os.path.exists(os.path.join(data_folder, "RDMP", processed_data_file)):
+        logger.info("Loading processed RDMP file.")
+        # load data processed csv file
+        df = pd.read_csv(os.path.join(data_folder, "RDMP", processed_data_file))
+    else:
+        logger.info("Processing RDMP synthetic data")
+        file_list = [
+            "CarotidArteryScan.csv",
+            "Demography.csv",
+            "HospitalAdmissions.csv",
+        ]
+        files_path = [os.path.join(data_folder, "RDMP", f) for f in file_list]
+        found = [os.path.exists(file_path) for file_path in files_path]
+        not_found = [
+            file_path for file_path in files_path if not os.path.exists(file_path)
+        ]
 
-    if not os.path.exists(
-        os.path.join(data_folder, "TexasHospitals", processed_data_file)
-    ):
-        logger.info("Processing Texas Hospitals data (2006-2009)")
+        if not all(found):
+            help_message = f"""
+            Some or all data files do not exist. Please download the files from RDMP,
+        and place it in the correct folder.
+
+            Missing files are:
+            {not_found}
+            """
+            raise DataNotAvailable(help_message)
 
         # Load data
-        columns_names = [
-            "THCIC_ID",  # Provider ID. Unique identifier assigned to the provider by DSHS.
-            # Hospitals with fewer than 50 discharges have been aggregated into the
-            # Provider ID '999999'
-            "DISCHARGE_QTR",  # yyyyQm
-            "TYPE_OF_ADMISSION",
-            "SOURCE_OF_ADMISSION",
-            "PAT_ZIP",  # Patient’s five-digit ZIP code
-            "PUBLIC_HEALTH_REGION",  # Public Health Region of patient’s address
-            "PAT_STATUS",  # Code indicating patient status as of the ending date of service for
-            # the period of care reported
-            "SEX_CODE",
-            "RACE",
-            "ETHNICITY",
-            "LENGTH_OF_STAY",
-            "PAT_AGE",  # Code indicating age of patient in days or years on date of discharge.
-            "PRINC_DIAG_CODE",  # diagnosis code for the principal diagnosis
-            "E_CODE_1",  # external cause of injury
-            "PRINC_SURG_PROC_CODE",  # Code for the principal surgical or other procedure performed
-            # during the period covered by the bill
-            "RISK_MORTALITY",  # Assignment of a risk of mortality score from the All Patient
-            # Refined (APR) Diagnosis Related Group (DRG)
-            "ILLNESS_SEVERITY",  # Assignment of a severity of illness score from the All Patient
-            # Refined (APR) Diagnosis RelatedGroup (DRG
-            "RECORD_ID",
+        headers0 = [
+            "R_CC_STEN_A",
+            "R_CC_STEN_B",
+            "R_CC_STEN_C",
+            "R_CC_STEN_D",
+            "R_CC_STEN_S",  # pylint: disable=unreachable
+            "L_IC_STEN_A",
+            "L_IC_STEN_B",
+            "L_IC_STEN_C",
+            "L_IC_STEN_D",
+            "L_IC_STEN_S",
+            "R_IC_STEN_A",
+            "R_IC_STEN_B",
+            "R_IC_STEN_C",
+            "R_IC_STEN_D",
+            "R_IC_STEN_S",
+            "PatientID",
+            "L_CC_STEN_S",
+            "L_CC_STEN_D",
+            "L_CC_STEN_B",
+            "L_BD_RATIO",
+            "L_AC_RATIO",
+            "R_BD_RATIO",
+            "R_AC_RATIO",
+            "L_CC_STENOSIS",
+            "L_CC_PEAK_SYS",
+            "L_CC_END_DIA",
+            "L_IC_STENOSIS",
+            "L_IC_PEAK_SYS",
+            "L_IC_END_DIA",
+            "L_EC_STENOSIS",
+            "L_PLAQUE",
+            "L_SYMPTOMS",
+            "L_BRUIT",
+            "L_CC_STEN_A",
+            "ON_STEN_STUDY",
+            "R_VERT_ARTERY",
+            "R_BRUIT",
+            "R_SYMPTOMS",
+            "R_PLAQUE",
+            "L_CC_STEN_C",
+            "R_EC_STENOSIS",
+            "R_IC_PEAK_SYS",
+            "R_IC_STENOSIS",
+            "R_CC_END_DIA",
+            "R_CC_PEAK_SYS",
+            "R_CC_STENOSIS",
+            "L_VERT_ARTERY",
+            "R_IC_END_DIA",
+        ]
+        headers1 = [
+            "chi",
+            "sex",
+            "current_address_L2",
+            "date_of_death",
+            "date_of_birth",
+        ]
+        headers2 = [
+            "chi",
+            "AdmissionDate",
+            "DischargeDate",
+            "MainCondition",
+            "OtherCondition1",
+            "OtherCondition2",
+            "OtherCondition3",
+            "MainOperation",
+            "MainOperationB",
+            "OtherOperation1",
+            "OtherOperation1B",
+            "OtherOperation2",
+            "OtherOperation2B",
+            "OtherOperation3",
+            "OtherOperation3B",
         ]
-        # obtain the 100 most frequent procedures
-        tmp = []
-        for f in files_path:
-            df = [
-                pd.read_csv(
-                    ZipFile(f).open(i), sep="\t", usecols=["PRINC_SURG_PROC_CODE"]
-                )
-                for i in ZipFile(f).namelist()
-                if "base" in i
-            ]
-            if len(df) < 1:
-                print(f"WARNING: {f} could not be loaded.")
-            else:
-                df[0].dropna(inplace=True)
-                tmp.extend(list(df[0].PRINC_SURG_PROC_CODE))
-        princ_surg_proc_keep = [k for k, v in Counter(tmp).most_common(10)]
-        # remove unnecessary variables
-        del tmp
-
-        # Load the data
-        tx_data = pd.DataFrame()
-        for f in files_path:
-            df = [
-                pd.read_csv(ZipFile(f).open(i), sep="\t", usecols=columns_names)
-                for i in ZipFile(f).namelist()
-                if "base" in i
-            ][0]
-            # keep only those rows with one of the 10 most common principal surgical procedure
-            df = df[df["PRINC_SURG_PROC_CODE"].isin(princ_surg_proc_keep)]
-            # clean up data
-            df.dropna(inplace=True)
-            df.replace("`", pd.NA, inplace=True)
-            df.replace("*", pd.NA, inplace=True)
-            # replace sex to numeric
-            df.SEX_CODE.replace("M", 0, inplace=True)
-            df.SEX_CODE.replace("F", 1, inplace=True)
-            df.SEX_CODE.replace("U", 2, inplace=True)
-            # set to numerical variable
-            for d_code in set(list(df.DISCHARGE_QTR)):
-                df.DISCHARGE_QTR.replace(
-                    d_code, "".join(d_code.split("Q")), inplace=True
-                )
-            df.dropna(inplace=True)
-            # merge data
-            tx_data = pd.concat([tx_data, df])
-        # remove unnecessary variables
-        del df
-
-        # Risk mortality, make it binary
-        # 1 Minor
-        # 2 Moderate
-        # 3 Major
-        # 4 Extreme
-        tx_data.RISK_MORTALITY.astype(int)
-        tx_data.RISK_MORTALITY.replace(1, 0, inplace=True)
-        tx_data.RISK_MORTALITY.replace(2, 0, inplace=True)
-        tx_data.RISK_MORTALITY.replace(3, 1, inplace=True)
-        tx_data.RISK_MORTALITY.replace(4, 1, inplace=True)
-
-        # renumber non-numerical codes for cols
-        cols = ["PRINC_DIAG_CODE", "SOURCE_OF_ADMISSION", "E_CODE_1"]
-        for col in cols:
-            tmp = list(
-                {
-                    x
-                    for x in tx_data[col]
-                    if not str(x).isdigit() and not isinstance(x, float)
-                }  # pylint: disable=consider-using-set-comprehension
-            )
-            n = max(
-                list(
-                    {
-                        int(x)
-                        for x in tx_data[col]
-                        if str(x).isdigit() or isinstance(x, float)
-                    }  # pylint: disable=consider-using-set-comprehension
-                )
-            )
-            for i, x in enumerate(tmp):
-                tx_data[col].replace(x, n + i, inplace=True)
-        del tmp, n
-        # set index
-        tx_data.set_index("RECORD_ID", inplace=True)
-        # final check and drop of NAs
-        tx_data.dropna(inplace=True)
-        # convert all data to numerical
-        tx_data = tx_data.astype(int)
-        # save csv file
-        tx_data.to_csv(os.path.join(data_folder, "TexasHospitals", processed_data_file))
-    else:
-        logger.info("Loading processed Texas Hospitals data (2006-2009) csv file.")
-        # load texas data processed csv file
-        tx_data = pd.read_csv(
-            os.path.join(data_folder, "TexasHospitals", processed_data_file)
-        )
-
-    # extract target
-    var = "RISK_MORTALITY"
-    labels = tx_data[var]
-    # Drop the column that contains the labels
-    tx_data.drop([var], axis=1, inplace=True)
 
-    label_encoder = LabelEncoder()
-    encoded_labels = label_encoder.fit_transform(labels.values)
-    labels = pd.DataFrame({var: encoded_labels})
+        # Process first file
+        df = pd.read_csv(files_path[0], usecols=headers0, encoding="ISO 8859-1")
+        # Change name to be the same in all files
+        df.rename(columns={"PatientID": "chi"}, inplace=True)
+        df = df.groupby(["chi"]).max()
+
+        # Process second file
+        df_ = pd.read_csv(files_path[1], usecols=headers1)
+        df_["date_of_birth"] = pd.to_datetime(df_["date_of_birth"])
+        df_["date_of_death"] = pd.to_datetime(df_["date_of_death"])
+        df_ = df_.groupby(["chi"]).max()
+
+        # Merge first and second file
+        df = df.merge(df_, how="inner", on="chi", suffixes=(False, False))
+        del df_
+
+        # Process third file
+        df__ = pd.read_csv(files_path[2], usecols=headers2, encoding="ISO 8859-1")
+        df__["AdmissionDate"] = pd.to_datetime(df__["AdmissionDate"])
+        df__["DischargeDate"] = pd.to_datetime(df__["DischargeDate"])
+        df__["days_in_hospital"] = df__.apply(hospital_days, axis=1)
+        number_stays = df__.groupby(["chi"]).count()["AdmissionDate"]
+        dih = df__.groupby(["chi"])["days_in_hospital"].sum()
+        nc = (
+            df__.groupby(["chi"])[[x for x in df__.columns if "Condition" in x]]
+            .count()
+            .mean(axis=1)
+        )  # pylint: disable=line-too-long
+        no = (
+            df__.groupby(["chi"])[[x for x in df__.columns if "Operation" in x]]
+            .count()
+            .sum(axis=1)
+        )  # pylint: disable=line-too-long
+        df__.drop(
+            columns=[
+                x
+                for x in df__.columns
+                if "Date" in x or "Operation" in x or "Condition" in x
+            ],
+            inplace=True,
+        )  # pylint: disable=line-too-long
+        df__ = pd.DataFrame()
+        df__["days_in_hospital"] = dih
+        df__["average_number_conditions"] = nc
+        df__["total_number_operations"] = no
+        df__["number_admissions"] = number_stays
+
+        # merge the third file
+        df = df.merge(df__, how="inner", on="chi", suffixes=(False, False))
+
+        # Final processing after merging
+        df["death"] = [1 if x else 0 for x in pd.notna(df.date_of_death)]
+        df["age"] = df.apply(find_age, axis=1).astype("int64")
+        df.drop(columns=["date_of_birth", "date_of_death"], inplace=True)
+
+        # save the dataframe
+        df.to_csv(os.path.join(data_folder, "RDMP", processed_data_file))
+
+    labels = df["death"]
+    df.drop(columns=["death"], inplace=True)
+
+    # OneHotEncoder
+    for col in df.columns:
+        if df[col].dtypes in ("bool", "object"):
+            encoder = LabelEncoder()
+            df[col] = encoder.fit_transform(df[col].values)
 
-    return (tx_data, labels)
+    return (df, labels)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aisdc-1.1.2/aisdc/safemodel/classifiers/dp_svc.py` & `aisdc-1.1.3/aisdc/safemodel/classifiers/dp_svc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Differentially private SVC
 James Liley
 21/03/22.
 """
+
 import logging
 from typing import Any
 
 import numpy as np
 from sklearn.linear_model import LogisticRegression
 from sklearn.svm import SVC
```

### Comparing `aisdc-1.1.2/aisdc/safemodel/classifiers/new_model_template.py` & `aisdc-1.1.3/aisdc/safemodel/classifiers/new_model_template.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.1.2/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py` & `aisdc-1.1.3/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     # print(f' leaf ids {uniqs_counts[0]} and counts {uniqs_counts[1]}'
     #        f'the  k-anonymity of the tree is {k_anonymity}')
     return k_anonymity
 
 
 class SafeDecisionTreeClassifier(
     SafeModel, DecisionTreeClassifier
-):  # pylint: disable=too-many-instance-attributes
+):  # pylint: disable=too-many-ancestors
     """Privacy protected Decision Tree classifier."""
 
     def __init__(self, **kwargs: Any) -> None:
         """Creates model and applies constraints to params."""
         SafeModel.__init__(self)
         self.basemodel_paramnames = [
             "criterion",
```

### Comparing `aisdc-1.1.2/aisdc/safemodel/classifiers/safekeras.py` & `aisdc-1.1.3/aisdc/safemodel/classifiers/safekeras.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Safekeras.py:
  Jim Smith, Andrew McCarty and Richard Preen
  UWE 2022.
 """
+
 # general imports
 
 
 import os
 import warnings
 
 # import sys
@@ -403,15 +404,15 @@
         (iii) then calls the tensorflow fit() function.
         (iv) finally makes a saved copy of the newly fitted model.
         """
 
         # pylint can't cope that we first declared these via a dict :(
         self.num_samples = X.shape[0]  # pylint: disable=attribute-defined-outside-init
         self.epochs = epochs  # pylint: disable=attribute-defined-outside-init
-        self.batch_size = batch_size  # pylint: disable=attribute-defined-outside-init
+        self.batch_size = batch_size
         # make sure you are passing keywords through - but also checking batch size epochs
         ok, msg = self.check_epsilon(X.shape[0], batch_size, epochs)
 
         if not ok:
             print(msg)
         if refine_epsilon:
             print(
```

### Comparing `aisdc-1.1.2/aisdc/safemodel/classifiers/saferandomforestclassifier.py` & `aisdc-1.1.3/aisdc/safemodel/classifiers/saferandomforestclassifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,21 @@
 import numpy as np
 from sklearn.ensemble import RandomForestClassifier
 
 from ..reporting import get_reporting_string
 from ..safemodel import SafeModel
 from .safedecisiontreeclassifier import decision_trees_are_equal
 
-# pylint: disable=too-many-ancestors,too-many-instance-attributes, unidiomatic-typecheck
+# pylint: disable=too-many-ancestors, unidiomatic-typecheck
 
 
 class SafeRandomForestClassifier(SafeModel, RandomForestClassifier):
     """Privacy protected Random Forest classifier."""
 
-    def __init__(
-        self, **kwargs: Any
-    ) -> None:  # pylint: disable=too-many-instance-attributes
+    def __init__(self, **kwargs: Any) -> None:
         """Creates model and applies constraints to params."""
         SafeModel.__init__(self)
         self.basemodel_paramnames = [
             "n_estimators",
             "criterion",
             "max_depth",
             "min_samples_split",
@@ -50,38 +48,38 @@
                 the_kwds[key] = val
         RandomForestClassifier.__init__(self, **the_kwds)
         self.model_type: str = "RandomForestClassifier"
         super().preliminary_check(apply_constraints=False, verbose=True)
         self.ignore_items = [
             "model_save_file",
             "ignore_items",
-            "base_estimator_",  # this is an object
+            "estimator_",  # this is an object
             "timestamp",
         ]
-        self.examine_seperately_items = ["estimators_", "base_estimator"]
+        self.examine_seperately_items = ["estimators_", "estimator"]
         self.k_anonymity = 0
 
-    def additional_checks(  # pylint: disable=too-many-nested-blocks,too-many-branches
+    def additional_checks(  # pylint: disable=too-many-nested-blocks
         self, curr_separate: dict, saved_separate: dict
     ) -> tuple[str, str]:
         """Random Forest-specific checks
         would benefit from refactoring into simpler blocks perhaps.
         NOTE that this is never called if the model has not been fitted.
         """
         msg = ""
         disclosive = False
         # now the relevant random-forest specific things
         for item in self.examine_seperately_items:
             # template for class of things that make up forest
-            if item == "base_estimator":
+            if item == "estimator":
                 if type(curr_separate[item]) != type(saved_separate[item]):
                     # msg += get_reporting_string(name="basic_params_differ",length=1)
                     msg += get_reporting_string(
                         name="param_changed_from_to",
-                        key="base_estimator",
+                        key="estimator",
                         val=saved_separate[item],
                         cur_val=curr_separate[item],
                     )
                     disclosive = True
             # the forest itself
             elif item == "estimators_":
                 try:
```

### Comparing `aisdc-1.1.2/aisdc/safemodel/classifiers/safesvc.py` & `aisdc-1.1.3/aisdc/safemodel/classifiers/safesvc.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.1.2/aisdc/safemodel/classifiers/safetf.py` & `aisdc-1.1.3/aisdc/safemodel/classifiers/safetf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Work in progress to allow use of the DPModel classes
  Jim smith 2022
  When ready, linting of  the imports will be enabled.
 """
 
-
 # pylint: disable=unused-import
 from typing import Any
 
 import tensorflow as tf
 import tensorflow_privacy as tf_privacy
 from tensorflow_privacy import DPModel
```

### Comparing `aisdc-1.1.2/aisdc/safemodel/reporting.py` & `aisdc-1.1.3/aisdc/safemodel/reporting.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.1.2/aisdc/safemodel/rules.json` & `aisdc-1.1.3/aisdc/safemodel/rules.json`

 * *Files identical despite different names*

### Comparing `aisdc-1.1.2/aisdc/safemodel/safemodel.py` & `aisdc-1.1.3/aisdc/safemodel/safemodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,17 +248,15 @@
         for key, val in self.__dict__.items():
             if key in self.basemodel_paramnames:
                 the_params[key] = val
         if deep:
             pass  # not implemented yet
         return the_params
 
-    def save(
-        self, name: str = "undefined"
-    ) -> None:  # pylint: disable=too-many-branches
+    def save(self, name: str = "undefined") -> None:
         """Writes model to file in appropriate format.
 
         Note this is overloaded in SafeKerasClassifer
         to deal with tensorflow specifics.
 
         Parameters
         ----------
@@ -570,15 +568,15 @@
                 msg += get_reporting_string(name="saved_item_removed", item=item)
 
         if not disclosive:  # ok, so can call mode-specific extra checks
             msg, disclosive = self.additional_checks(curr_vals, saved_vals)
 
         return msg, disclosive
 
-    def posthoc_check(self) -> tuple[str, bool]:  # pylint: disable=too-many-branches
+    def posthoc_check(self) -> tuple[str, bool]:
         """Checks whether model has been interfered with since fit() was last run."""
 
         disclosive = False
         msg = ""
 
         current_model, saved_model = self.get_current_and_saved_models()
         if len(saved_model) == 0:
@@ -624,15 +622,15 @@
             )
             msg += extra_msg
             if extra_disclosive:
                 disclosive = True
 
         return msg, disclosive
 
-    def additional_checks(  # pylint: disable=too-many-branches
+    def additional_checks(
         self, curr_separate: dict, saved_separate: dict
     ) -> tuple[str, bool]:
         """Placeholder function for additional posthoc checks e.g. keras this
         version just checks that any lists have the same contents.
 
         Parameters
         ----------
```

### Comparing `aisdc-1.1.2/aisdc.egg-info/PKG-INFO` & `aisdc-1.1.3/aisdc.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,71 @@
 Metadata-Version: 2.1
 Name: aisdc
-Version: 1.1.2
+Version: 1.1.3
 Summary: Tools for the statistical disclosure control of machine learning models
 Home-page: https://github.com/AI-SDC/AI-SDC
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,machine-learning,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.9,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dictdiffer~=0.9.0
-Requires-Dist: fpdf~=1.7.2
-Requires-Dist: joblib~=1.3
-Requires-Dist: multiprocess~=0.70.15
-Requires-Dist: numpy~=1.23.1
-Requires-Dist: pandas~=1.5.3
-Requires-Dist: scikit_learn~=1.1.3
-Requires-Dist: scipy~=1.10
-Requires-Dist: tensorflow-probability==0.15.0; python_version < "3.9"
-Requires-Dist: tensorflow~=2.10.0; python_version < "3.9"
-Requires-Dist: tensorflow~=2.12.0; python_version >= "3.9"
-Requires-Dist: tensorflow_privacy==0.7.3; python_version < "3.9"
-Requires-Dist: tensorflow_privacy==0.8.10; python_version >= "3.9"
-Requires-Dist: uuid~=1.30
-Requires-Dist: pypdf~=3.16
-Requires-Dist: xgboost~=1.7.6
-Requires-Dist: statsmodels==0.13.5
-Requires-Dist: acro==0.4.3
+Requires-Dist: acro==0.4.5
+Requires-Dist: fpdf
+Requires-Dist: pypdf
+Requires-Dist: multiprocess
+Requires-Dist: scikit-learn
+Requires-Dist: xgboost
+Provides-Extra: safemodel
+Requires-Dist: tensorflow<2.15,>=2.14; extra == "safemodel"
+Requires-Dist: tensorflow-privacy==0.9.0; extra == "safemodel"
+Requires-Dist: dictdiffer; extra == "safemodel"
+Provides-Extra: doc
+Requires-Dist: tensorflow<2.15,>=2.14; extra == "doc"
+Requires-Dist: tensorflow-privacy==0.9.0; extra == "doc"
+Requires-Dist: dictdiffer; extra == "doc"
+Requires-Dist: numpydoc; extra == "doc"
+Requires-Dist: sphinx-autopackagesummary; extra == "doc"
+Requires-Dist: sphinx-issues; extra == "doc"
+Requires-Dist: sphinx-prompt; extra == "doc"
+Requires-Dist: sphinx-rtd-theme; extra == "doc"
+Requires-Dist: sphinx; extra == "doc"
+Provides-Extra: test
+Requires-Dist: tensorflow<2.15,>=2.14; extra == "test"
+Requires-Dist: tensorflow-privacy==0.9.0; extra == "test"
+Requires-Dist: dictdiffer; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://opensource.org/licenses/MIT)
 [![Latest Version](https://img.shields.io/github/v/release/AI-SDC/AI-SDC?style=flat)](https://github.com/AI-SDC/AI-SDC/releases)
 [![DOI](https://zenodo.org/badge/518801511.svg)](https://zenodo.org/badge/latestdoi/518801511)
-[![codecov](https://codecov.io/gh/AI-SDC/AI-SDC/branch/development/graph/badge.svg?token=AXX2XCXUNU)](https://codecov.io/gh/AI-SDC/AI-SDC)
+[![codecov](https://codecov.io/gh/AI-SDC/AI-SDC/branch/main/graph/badge.svg?token=AXX2XCXUNU)](https://codecov.io/gh/AI-SDC/AI-SDC)
 [![Python versions](https://img.shields.io/pypi/pyversions/aisdc.svg)](https://pypi.org/project/aisdc)
 
 # AI-SDC
 
 A collection of tools and resources for managing the statistical disclosure control of trained machine learning models. For a brief introduction, see [Smith et al. (2022)](https://doi.org/10.48550/arXiv.2212.01233).
 
 ### User Guides
 
-A collection of user guides can be found in the 'user_stories' folder of this repository. These guides include configurable examples from the perspective of both a researcher and a TRE, with separate scripts for each. Instructions on how to use each of these scripts and which scripts to use are included in the README of the ['user_stories'](https://github.com/AI-SDC/AI-SDC/tree/user_story_visibility/user_stories) folder.
+A collection of user guides can be found in the 'user_stories' folder of this repository. These guides include configurable examples from the perspective of both a researcher and a TRE, with separate scripts for each. Instructions on how to use each of these scripts and which scripts to use are included in the README of the [`user_stories`](./user_stories) folder.
 
 ## Content
 
 * `aisdc`
     - `attacks` Contains a variety of privacy attacks on machine learning models, including membership and attribute inference.
     - `preprocessing` Contains preprocessing modules for test datasets.
     - `safemodel` The safemodel package is an open source wrapper for common machine learning models. It is designed for use by researchers in Trusted Research Environments (TREs) where disclosure control methods must be implemented. Safemodel aims to give researchers greater confidence that their models are more compliant with disclosure control.
@@ -72,63 +80,56 @@
 * `risk_examples` Contains hypothetical examples of data leakage through machine learning models as described in the [Green Paper](https://doi.org/10.5281/zenodo.6896214).
 * `tests` Contains unit tests.
 
 ## Documentation
 
 Documentation is hosted here: https://ai-sdc.github.io/AI-SDC/
 
-## Quick Start
+## Installation / End-user
 
-### Development
-
-Clone the repository and install the dependencies (safest in a virtual env):
+[![PyPI package](https://img.shields.io/pypi/v/aisdc.svg)](https://pypi.org/project/aisdc)
 
-```
-$ git clone https://github.com/AI-SDC/AI-SDC.git
-$ cd AI-SDC
-$ pip install -r requirements.txt
-```
+Install `aisdc` (safest in a virtual env) and manually copy the [`examples`](examples/) and [`example_notebooks`](example_notebooks/).
 
-Then run the tests:
+To install only the base package, which includes the attacks used for assessing privacy:
 
 ```
-$ pip install pytest
-$ pytest .
+$ pip install aisdc
 ```
 
-Or run an example:
+To install the base package and the safemodel package, which includes defensive wrappers for popular ML frameworks including [scikit-learn](https://scikit-learn.org) and [Keras](https://keras.io):
 
 ```
-$ python -m examples.lira_attack_example
+$ pip install aisdc[safemodel]
 ```
 
-### Installation / End-user
+## Running
 
-[![PyPI package](https://img.shields.io/pypi/v/aisdc.svg)](https://pypi.org/project/aisdc)
+To run an example, simply execute the desired script or start up `jupyter notebook` and run one of the notebooks.
 
-Install `aisdc` (safest in a virtual env) and manually copy the `examples` and `example_notebooks`.
+For example, to run the `lira_attack_example.py`:
 
 ```
-$ pip install aisdc
+$ python -m lira_attack_example
 ```
 
-Then to run an example:
+## Development
+
+Clone the repository and install the local package including all dependencies (safest in a virtual env):
 
 ```
-$ python attribute_inference_example.py
+$ git clone https://github.com/AI-SDC/AI-SDC.git
+$ cd AI-SDC
+$ pip install .[test]
 ```
 
-Or start up `jupyter notebook` and run an example.
-
-Alternatively, you can clone the repo and install:
+Then run the tests:
 
 ```
-$ git clone https://github.com/AI-SDC/AI-SDC.git
-$ cd AI-SDC
-$ pip install .
+$ pytest .
 ```
 
 ---
 
-This work was funded by UK Research and Innovation Grant Number MC_PC_21033 as part of Phase 1 of the DARE UK (Data and Analytics Research Environments UK) programme (https://dareuk.org.uk/), delivered in partnership with HDR UK and ADRUK. The specific project was Guidelines and Resources for AI Model Access from TrusTEd Research environments (GRAIMATTER).­ This project has also been supported by MRC and EPSRC [grant number MR/S010351/1]: PICTURES.
+This work was funded by UK Research and Innovation under Grant Numbers MC_PC_21033  and MC_PC_23006 as part of Phase 1 of the DARE UK (Data and Analytics Research Environments UK) programme (https://dareuk.org.uk/), delivered in partnership with Health Data Research UK (HDR UK) and Administrative Data Research UK (ADR UK). The specific projects were Semi-Automatic checking of Research Outputs (SACRO -MC_PC_23006) and   Guidelines and Resources for AI Model Access from TrusTEd Research environments (GRAIMATTER - MC_PC_21033).­ This project has also been supported by MRC and EPSRC [grant number MR/S010351/1]: PICTURES.
 
 <img src="docs/source/images/UK_Research_and_Innovation_logo.svg" width="20%" height="20%" padding=20/> <img src="docs/source/images/health-data-research-uk-hdr-uk-logo-vector.png" width="10%" height="10%" padding=20/> <img src="docs/source/images/logo_print.png" width="15%" height="15%" padding=20/>
```

### Comparing `aisdc-1.1.2/aisdc.egg-info/SOURCES.txt` & `aisdc-1.1.3/aisdc.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -29,26 +29,29 @@
 aisdc/safemodel/classifiers/dp_svc.py
 aisdc/safemodel/classifiers/new_model_template.py
 aisdc/safemodel/classifiers/safedecisiontreeclassifier.py
 aisdc/safemodel/classifiers/safekeras.py
 aisdc/safemodel/classifiers/saferandomforestclassifier.py
 aisdc/safemodel/classifiers/safesvc.py
 aisdc/safemodel/classifiers/safetf.py
-tests/test_attack_report_formatter.py
-tests/test_attacks.py
-tests/test_attacks_target.py
-tests/test_attacks_via_safemodel.py
-tests/test_attribute_inference_attack.py
-tests/test_data_interface.py
-tests/test_failfast.py
-tests/test_lira_attack.py
-tests/test_loaders.py
-tests/test_metrics.py
-tests/test_multiple_attacks.py
-tests/test_safedecisiontreeclassifier.py
-tests/test_safekeras2.py
-tests/test_safemodel.py
-tests/test_saferandomforestclassifier.py
-tests/test_safesvc.py
-tests/test_safetf.py
-tests/test_structural_attack.py
-tests/test_worst_case_attack.py
+tests/attacks/__init__.py
+tests/attacks/test_attack_report_formatter.py
+tests/attacks/test_attacks_target.py
+tests/attacks/test_attribute_inference_attack.py
+tests/attacks/test_data_interface.py
+tests/attacks/test_failfast.py
+tests/attacks/test_lira_attack.py
+tests/attacks/test_metrics.py
+tests/attacks/test_multiple_attacks.py
+tests/attacks/test_structural_attack.py
+tests/attacks/test_worst_case_attack.py
+tests/preprocessing/__init__.py
+tests/preprocessing/test_loaders.py
+tests/safemodel/__init__.py
+tests/safemodel/test_attacks.py
+tests/safemodel/test_attacks_via_safemodel.py
+tests/safemodel/test_safedecisiontreeclassifier.py
+tests/safemodel/test_safekeras2.py
+tests/safemodel/test_safemodel.py
+tests/safemodel/test_saferandomforestclassifier.py
+tests/safemodel/test_safesvc.py
+tests/safemodel/test_safetf.py
```

### Comparing `aisdc-1.1.2/tests/test_attack_report_formatter.py` & `aisdc-1.1.3/tests/attacks/test_attack_report_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,24 @@
             file_contents = json.loads(f.read())
 
         self.assertIn(msg_1, file_contents["FirstTestAttack"]["test_output"])
         self.assertIn(msg_2, file_contents["SecondTestAttack"]["test_output"])
 
         clean_up(test_filename)
 
+    def test_pretty_print(self):
+        """Test which tests the pretty_print function with nested dictionaries."""
+        example_report = {
+            "example_a": "example_value",
+            "example_b": {"A": 1.0, "B": 1.0},
+        }
+
+        g = GenerateTextReport()
+        g.pretty_print(example_report, "Example Title")
+
     def test_process_attack_target_json(self):
         """Test which tests the process_attack_target_json function."""
         target_report = get_target_report()
         target_json = "target.json"
 
         with open(target_json, "w", encoding="utf-8") as f:
             json.dump(target_report, f)
```

### Comparing `aisdc-1.1.2/tests/test_attacks.py` & `aisdc-1.1.3/tests/safemodel/test_attacks.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.1.2/tests/test_attribute_inference_attack.py` & `aisdc-1.1.3/tests/attacks/test_attribute_inference_attack.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,47 +8,34 @@
 python -m examples.attribute_inference_example
 """
 
 from __future__ import annotations
 
 import json
 import os
-import shutil
 import sys
 import unittest
 
-# ignore unused imports because it depends on whether data file is present
-from sklearn.datasets import fetch_openml  # pylint:disable=unused-import
 from sklearn.ensemble import RandomForestClassifier
-from sklearn.preprocessing import (  # pylint:disable=unused-import
-    LabelEncoder,
-    OneHotEncoder,
-)
 
-from aisdc.attacks import attribute_attack  # pylint: disable = import-error
+from aisdc.attacks import attribute_attack
 from aisdc.attacks.attribute_attack import (
     _get_bounds_risk,
     _infer_categorical,
     _unique_max,
 )
-from tests.test_attacks_via_safemodel import get_target
+
+from ..common import clean, get_target
 
 # pylint: disable = duplicate-code
 
 
 class TestAttributeInferenceAttack(unittest.TestCase):
     """Class which tests the AttributeInferenceAttack module."""
 
-    def _cleanup_file(self, name: str):
-        """Removes unwanted files or directory."""
-        if os.path.exists(name) and os.path.isfile(name):  # h5
-            os.remove(name)
-        elif os.path.exists(name) and os.path.isdir(name):  # tf
-            shutil.rmtree(name)
-
     def _common_setup(self):
         """Basic commands to get ready to test some code."""
         model = RandomForestClassifier(bootstrap=False)
         target = get_target(model)
         model.fit(target.x_train, target.y_train)
         attack_obj = attribute_attack.AttributeAttack(n_cpu=7, report_name="aia_report")
         return target, attack_obj
@@ -110,14 +97,15 @@
 
         # Check the number of parameters returned
         self.assertEqual(3, len(returned.keys()))
 
         # Check the value of the returned parameters
         self.assertEqual(0.0, returned["train"])
         self.assertEqual(0.0, returned["test"])
+        clean("output_attribute")
 
     # test below covers a lot of the plotting etc.
     def test_AIA_on_nursery(self):
         """Tests running AIA on the nursery data
         with an added continuous feature.
         """
         target, attack_obj = self._common_setup()
@@ -168,8 +156,8 @@
             "aia_attack_from_configfile.json",
             "test_attribute_attack.json",
             os.path.join("tests", "test_config_aia_cmd.json"),
             os.path.join("tests", "test_aia_target/"),
             "output_attribute",
         )
         for fname in files_made:
-            self._cleanup_file(fname)
+            clean(fname)
```

### Comparing `aisdc-1.1.2/tests/test_data_interface.py` & `aisdc-1.1.3/tests/attacks/test_data_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 
 from __future__ import annotations
 
 import unittest
 
 import pandas as pd
 
-from aisdc.preprocessing.loaders import (  # pylint: disable = import-error
-    UnknownDataset,
-    get_data_sklearn,
-)
+from aisdc.preprocessing.loaders import UnknownDataset, get_data_sklearn
 
 
 class TestLoaders(unittest.TestCase):
     """Test the data loaders."""
 
     def test_iris(self):
         """Nursery data."""
```

### Comparing `aisdc-1.1.2/tests/test_failfast.py` & `aisdc-1.1.3/tests/attacks/test_failfast.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from __future__ import annotations
 
 import shutil
 import unittest
 
-from aisdc.attacks import failfast, worst_case_attack  # pylint: disable = import-error
+from aisdc.attacks import failfast, worst_case_attack
 
 
 class TestFailFast(unittest.TestCase):
     """Class which tests the fail fast functionality of the WortCaseAttack module."""
 
     def test_parse_boolean_argument(self):
         """Test all comparison operators and both options for attack
```

### Comparing `aisdc-1.1.2/tests/test_lira_attack.py` & `aisdc-1.1.3/tests/attacks/test_lira_attack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Test_lira_attack.py
 Copyright (C) Jim Smith2022  <james.smith@uwe.ac.uk>.
 """
+
 # pylint: disable = duplicate-code
 
 from __future__ import annotations
 
 import logging
 import os
 import shutil
@@ -16,19 +17,16 @@
 
 import numpy as np
 from sklearn.datasets import load_breast_cancer
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import train_test_split
 
 from aisdc.attacks import likelihood_attack
-from aisdc.attacks.likelihood_attack import (  # pylint: disable = import-error
-    DummyClassifier,
-    LIRAAttack,
-)
-from aisdc.attacks.target import Target  # pylint: disable = import-error
+from aisdc.attacks.likelihood_attack import DummyClassifier, LIRAAttack
+from aisdc.attacks.target import Target
 
 N_SHADOW_MODELS = 20
 
 logger = logging.getLogger(__file__)
 
 
 def clean_up(name):
```

### Comparing `aisdc-1.1.2/tests/test_loaders.py` & `aisdc-1.1.3/tests/preprocessing/test_loaders.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,25 +13,29 @@
 
 import pytest
 
 from aisdc.preprocessing import loaders
 from aisdc.preprocessing.loaders import DataNotAvailable, UnknownDataset
 
 PROJECT_ROOT_FOLDER = os.path.dirname(os.path.dirname(__file__))
-DATA_FOLDER = os.path.join(PROJECT_ROOT_FOLDER, "tests", "datasets")
+DATA_FOLDER = os.path.join(PROJECT_ROOT_FOLDER, "datasets")
 
 datasets = (
     "mimic2-iaccd",
     "in-hospital-mortality",
     "medical-mnist-ab-v-br-100",
     "medical-mnist-ab-v-br-500",
     "medical-mnist-all-100",
     "indian liver",
     "synth-ae",
     "synth-ae-small",
+    "synth-ae-large",
+    "synth-ae-extra-large",
+    "synth-ae-XXL-large",
+    "RDMP",
     "nursery",
     "iris",
 )
 
 preprocessing = ("standard", "minmax", "round")
 
 
@@ -87,14 +91,30 @@
     with pytest.raises(DataNotAvailable):
         _, _ = loaders.get_data_sklearn("synth-ae")
 
     # synthae-small
     with pytest.raises(DataNotAvailable):
         _, _ = loaders.get_data_sklearn("synth-ae-small")
 
+    # synthae-large
+    with pytest.raises(DataNotAvailable):
+        _, _ = loaders.get_data_sklearn("synth-ae-large")
+
+    # synthae-large
+    with pytest.raises(DataNotAvailable):
+        _, _ = loaders.get_data_sklearn("synth-ae-extra-large")
+
+    # synthae-large
+    with pytest.raises(DataNotAvailable):
+        _, _ = loaders.get_data_sklearn("synth-ae-XXL")
+
+    # RDMP
+    with pytest.raises(DataNotAvailable):
+        _, _ = loaders.get_data_sklearn("RDMP")
+
     # unknown
     with pytest.raises(UnknownDataset):
         _, _ = loaders.get_data_sklearn("no such dataset")
 
 
 def test_mimic():
     """Load the mimic2 dataset."""
@@ -165,23 +185,38 @@
 def test_indian_liver():
     """The indian liver dataloader."""
     x_df, y_df = loaders.get_data_sklearn("indian liver", DATA_FOLDER)
     assert x_df.shape == (11, 10), f"x_df shape is {x_df.shape}"
     assert y_df.shape == (11, 1)
 
 
-def test_texas():
-    """The texas dataset has quite restrictive licenses arounbd copying.
-    Therefore it is omitted from the CI testing.
-    This code was fully tested during the GRAIMatter project.
-    """
-
-
 def test_synth_ae():
     """Tests different versions of the  synthetic A&E dataset."""
     x_df, y_df = loaders.get_data_sklearn("synth-ae", DATA_FOLDER)
     assert x_df.shape == (8, 16), f"x_df shape is {x_df.shape}"
     assert y_df.shape == (8, 1)
 
     x_df, y_df = loaders.get_data_sklearn("synth-ae-small", DATA_FOLDER)
     assert x_df.shape == (8, 16), f"x_df shape is {x_df.shape}"
     assert y_df.shape == (8, 1)
+
+    x_df, y_df = loaders.get_data_sklearn("synth-ae-large", DATA_FOLDER)
+    assert x_df.shape == (8, 16), f"x_df shape is {x_df.shape}"
+    assert y_df.shape == (8, 1)
+
+    x_df, y_df = loaders.get_data_sklearn("synth-ae-extra-large", DATA_FOLDER)
+    assert x_df.shape == (8, 16), f"x_df shape is {x_df.shape}"
+    assert y_df.shape == (8, 1)
+
+    x_df, y_df = loaders.get_data_sklearn("synth-ae-XXL", DATA_FOLDER)
+    assert x_df.shape == (8, 16), f"x_df shape is {x_df.shape}"
+    assert y_df.shape == (8, 1)
+
+
+# def test_rdmp():
+#     """The RDMP dataloader."""
+#     x_df, y_df = loaders.get_data_sklearn("RDMP", DATA_FOLDER)
+
+#     assert 'death' not in x_df.columns
+#     assert 'age' in x_df.columns
+
+#     assert y_df.shape[1] == 1
```

### Comparing `aisdc-1.1.2/tests/test_metrics.py` & `aisdc-1.1.3/tests/attacks/test_metrics.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.1.2/tests/test_multiple_attacks.py` & `aisdc-1.1.3/tests/attacks/test_multiple_attacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,19 +22,17 @@
 from sklearn.datasets import fetch_openml  # pylint:disable=unused-import
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.preprocessing import (  # pylint:disable=unused-import
     LabelEncoder,
     OneHotEncoder,
 )
 
-from aisdc.attacks.multiple_attacks import (  # pylint: disable = import-error
-    ConfigFile,
-    MultipleAttacks,
-)
-from tests.test_attacks_via_safemodel import get_target
+from aisdc.attacks.multiple_attacks import ConfigFile, MultipleAttacks
+
+from ..common import get_target
 
 # pylint: disable = duplicate-code
 
 
 def cleanup_file(name: str):
     """Removes unwanted files or directory."""
     if os.path.exists(name):
```

### Comparing `aisdc-1.1.2/tests/test_safedecisiontreeclassifier.py` & `aisdc-1.1.3/tests/safemodel/test_safedecisiontreeclassifier.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.1.2/tests/test_safekeras2.py` & `aisdc-1.1.3/tests/safemodel/test_safekeras2.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,19 @@
 from __future__ import annotations
 
 import os
 import shutil
 import warnings
 
 import numpy as np
+import pytest
 import tensorflow as tf
 from sklearn import datasets
 from sklearn.model_selection import train_test_split
-from tensorflow.keras.layers import (  # pylint: disable = import-error, no-name-in-module
-    Dense,
-    Input,
-)
+from tensorflow.keras.layers import Dense, Input  # pylint: disable = import-error
 
 from aisdc.safemodel.classifiers import SafeKerasModel, safekeras
 from aisdc.safemodel.reporting import get_reporting_string
 
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 warnings.filterwarnings("ignore", category=FutureWarning)
 
@@ -420,16 +418,16 @@
     )
     model.compile(loss=loss, optimizer=None)
     isDP, _ = safekeras.check_optimizer_is_DP(model.optimizer)
     assert isDP, "failed check that optimizer is dP"
 
     right_epsilon = 20.363059561511612
     model.check_epsilon(X.shape[0], 20, 10)
-    assert (
-        model.current_epsilon == right_epsilon
+    assert model.current_epsilon == pytest.approx(
+        right_epsilon, 0.01
     ), "failed check for epsilon after compilation"
 
     # check this works
     ok, msg = model.check_epsilon(X.shape[0], 0, 10)
     assert ok, "should be ok after resetting batch size =1"
     correct_msg = get_reporting_string(name="division_by_zero")
     assert msg == correct_msg, msg
```

### Comparing `aisdc-1.1.2/tests/test_safemodel.py` & `aisdc-1.1.3/tests/safemodel/test_safemodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import joblib
 import numpy as np
 from sklearn import datasets
 
 from aisdc.safemodel.reporting import get_reporting_string
 from aisdc.safemodel.safemodel import SafeModel
 
+from ..common import clean
+
 notok_start = get_reporting_string(name="warn_possible_disclosure_risk")
 ok_start = get_reporting_string(name="within_recommended_ranges")
 
 
 class DummyClassifier:
     """Dummy Classifier that always returns predictions of zero."""
 
@@ -550,7 +552,9 @@
             "model_type": model.model_type,
             "details": details,
             "k_anonymity": k_anonymity,
             "recommendation": recommendation,
             "reason": reason,
             "timestamp": model.timestamp,
         } in json_data["safemodel"]
+
+    clean(RES_DIR)
```

### Comparing `aisdc-1.1.2/tests/test_saferandomforestclassifier.py` & `aisdc-1.1.3/tests/safemodel/test_saferandomforestclassifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
     msg2, disclosive2 = model.posthoc_check()
     part1 = get_reporting_string(name="basic_params_differ", length=1)
     part2 = get_reporting_string(
         name="param_changed_from_to", key="bootstrap", val=False, cur_val=True
     )
     part3 = ""  # get_reporting_string(
     #        name="param_changed_from_to",
-    #        key="base_estimator",
+    #        key="estimator",
     #        val="DecisionTreeClassifier()",
     #        cur_val="DecisionTreeClassifier()",
     #    )
     correct_msg2 = part1 + part2 + part3
     # print(f'Correct: {correct_msg2}\n Actual: {msg2}')
 
     assert msg2 == correct_msg2, f"{msg2}\n should be {correct_msg2}"
@@ -192,32 +192,32 @@
 def test_randomforest_modeltype_changed():
     """Model type has been changed after fit()
     in this this case to hide some data.
     """
     x, y = get_data()
     model = SafeRandomForestClassifier(random_state=1, n_estimators=5)
     correct_msg = ""
-    # check code that tests base_estimator_
+    # check code that tests estimator_
     model.fit(x, y)
-    model.base_estimator = "DummyClassifier()"
+    model.estimator = "DummyClassifier()"
 
     # hide some data
     for i in range(5):  # changed lengths get picked up in different test
         model.estimators_[i] = x[i, :]
 
     msg, disclosive = model.posthoc_check()
     # correct_msg += get_reporting_string(name="basic_params_differ",length=1)
     correct_msg = get_reporting_string(name="forest_estimators_differ", idx=5)
     correct_msg += get_reporting_string(
         name="param_changed_from_to",
-        key="base_estimator",
+        key="estimator",
         val="DecisionTreeClassifier()",
         cur_val="DummyClassifier()",
     )
-    #    correct_msg += ("structure base_estimator has 1 differences: [('change', '', "
+    #    correct_msg += ("structure estimator has 1 differences: [('change', '', "
     #                    "(DecisionTreeClassifier(), DecisionTreeClassifier()))]"
     #                   )
     print(f"Correct: {correct_msg} Actual: {msg}")
 
     assert msg == correct_msg, f"{msg}\n should be {correct_msg}"
     assert disclosive is True, "should have been flagged as disclosive"
 
@@ -276,15 +276,15 @@
     part1 = get_reporting_string(name="basic_params_differ", length=1)
     part2 = get_reporting_string(
         name="param_changed_from_to", key="max_depth", val="None", cur_val="2"
     )
     part3 = get_reporting_string(name="forest_estimators_differ", idx=5)
     part4 = ""  # get_reporting_string(
     #        name="param_changed_from_to",
-    #        key="base_estimator",
+    #        key="estimator",
     #        val="DecisionTreeClassifier()",
     #        cur_val="DecisionTreeClassifier()",
     #    )
     correct_msg = part1 + part2 + part3 + part4
     # print(f'Correct:\n{correct_msg} Actual:\n{msg}')
     assert msg == correct_msg, f"{msg}\n should be {correct_msg}"
     assert disclosive, "should be flagged as disclosive"
@@ -307,15 +307,15 @@
     part1 = get_reporting_string(name="basic_params_differ", length=1)
     part2 = get_reporting_string(
         name="param_changed_from_to", key="n_estimators", val="5", cur_val="10"
     )
     part3 = get_reporting_string(name="different_num_estimators", num1=10, num2=5)
     part4 = ""  # get_reporting_string(
     #        name="param_changed_from_to",
-    #        key="base_estimator",
+    #        key="estimator",
     #        val="DecisionTreeClassifier()",
     #        cur_val="DecisionTreeClassifier()",
     #    )
     correct_msg = part1 + part2 + part3 + part4
     # print(f'Correct:\n{correct_msg} Actual:\n{msg}')
     assert msg == correct_msg, f"{msg}\n should be {correct_msg}"
     assert disclosive, "should be flagged as disclosive"
```

### Comparing `aisdc-1.1.2/tests/test_safesvc.py` & `aisdc-1.1.3/tests/safemodel/test_safesvc.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.1.2/tests/test_structural_attack.py` & `aisdc-1.1.3/tests/attacks/test_structural_attack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,29 @@
 """Test_worst_case_attack.py
 Copyright (C) Jim Smith 2023 <james.smith@uwe.ac.uk>.
 """
 
 from __future__ import annotations
 
 import json
-import os
-import shutil
 import sys
 from unittest.mock import patch
 
-# import numpy as np
 import pytest
 from sklearn.datasets import load_breast_cancer
 from sklearn.ensemble import AdaBoostClassifier, RandomForestClassifier
 from sklearn.model_selection import train_test_split
 from sklearn.svm import SVC
 from sklearn.tree import DecisionTreeClassifier
 from xgboost.sklearn import XGBClassifier
 
 import aisdc.attacks.structural_attack as sa
 from aisdc.attacks.target import Target
 
-
-def clean_up(name):
-    """Removes unwanted files or directory."""
-    if os.path.exists(name):
-        if os.path.isfile(name):
-            os.remove(name)
-        elif os.path.isdir(name):
-            shutil.rmtree(name)
+from ..common import clean
 
 
 def get_target(modeltype: str, **kwparams: dict) -> Target:
     """Loads dataset and creates target of the desired type."""
 
     X, y = load_breast_cancer(return_X_y=True, as_frame=False)
     train_X, test_X, train_y, test_y = train_test_split(X, y, test_size=0.3)
@@ -214,30 +204,30 @@
 
 def test_adaboost():
     """Test for adaboost classifier."""
 
     # 'non' disclosive'
     # - base estimator =None => DecisionTreeClassifier with max_depth 1
     # also set THRESHOLD to 4
-    param_dict = {"n_estimators": 2, "base_estimator": None}
+    param_dict = {"n_estimators": 2, "estimator": None}
     target = get_target("adaboost", **param_dict)
     myattack = sa.StructuralAttack()
     myattack.THRESHOLD = 2
     myattack.attack(target)
     assert myattack.DoF_risk == 0, "should be no DoF risk with just 2 decision stumps"
     assert (
         myattack.k_anonymity_risk == 0
     ), "should be no k-anonymity risk with only 2 stumps"
     assert myattack.class_disclosure_risk == 0, "no class disclosure risk for 2 stumps"
     assert myattack.unnecessary_risk == 0, " unnecessary risk not defined for adaboost"
 
     # highly disclosive
     kwargs = {"max_depth": None, "min_samples_leaf": 2}
     param_dict2 = {
-        "base_estimator": DecisionTreeClassifier(**kwargs),
+        "estimator": DecisionTreeClassifier(**kwargs),
         "n_estimators": 1000,
     }
     target = get_target("adaboost", **param_dict2)
     myattack2 = sa.StructuralAttack()
     myattack2.attack(target)
     assert myattack2.DoF_risk == 1, "should be  DoF risk with adaboost of deep trees"
     assert (
@@ -363,10 +353,11 @@
         "config_structural_test.json",
         "--attack-target-folder-path",
         "dt.sav",
     ]
     with patch.object(sys, "argv", testargs):
         sa.main()
 
-    clean_up("dt.sav")
-    clean_up("test_output_sa")
-    clean_up("config_structural_test.json")
+    clean("dt.sav")
+    clean("test_output_sa")
+    clean("config_structural_test.json")
+    clean("outputs_structural")
```

### Comparing `aisdc-1.1.2/tests/test_worst_case_attack.py` & `aisdc-1.1.3/tests/attacks/test_worst_case_attack.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import numpy as np
 import pytest
 from sklearn.datasets import load_breast_cancer
 from sklearn.model_selection import train_test_split
 from sklearn.svm import SVC
 
-from aisdc.attacks import worst_case_attack  # pylint: disable = import-error
+from aisdc.attacks import worst_case_attack
 from aisdc.attacks.target import Target
 
 
 def clean_up(name):
     """Removes unwanted files or directory."""
     if os.path.exists(name):
         if os.path.isfile(name):
@@ -265,23 +265,23 @@
     attack_obj = worst_case_attack.WorstCaseAttack()
     train_preds = np.array([[1, 0], [0, 1]], int)
     test_preds = np.array([[2, 0], [0, 2]], int)
 
     mi_x, mi_y = attack_obj._prepare_attack_data(  # pylint: disable=protected-access
         train_preds, test_preds
     )
-    np.testing.assert_array_equal(mi_y, np.array([1, 1, 0, 0], np.int))
+    np.testing.assert_array_equal(mi_y, np.array([1, 1, 0, 0], int))
     # Test the x data produced. Each row should be sorted in descending order
     np.testing.assert_array_equal(mi_x, np.array([[1, 0], [1, 0], [2, 0], [2, 0]]))
     # With sort_probs = False, the rows of x should not be sorted
     attack_obj = worst_case_attack.WorstCaseAttack(sort_probs=False)
     mi_x, mi_y = attack_obj._prepare_attack_data(  # pylint: disable=protected-access
         train_preds, test_preds
     )
-    np.testing.assert_array_equal(mi_y, np.array([1, 1, 0, 0], np.int))
+    np.testing.assert_array_equal(mi_y, np.array([1, 1, 0, 0], int))
     np.testing.assert_array_equal(mi_x, np.array([[1, 0], [0, 1], [2, 0], [0, 2]]))
 
 
 def test_attack_data_prep_with_correct_feature():
     """Test the method that prepares the attack data.
     This time, testing that the model correctness values are added, are always
     the final feature, and are not included in the sorting.
@@ -291,28 +291,28 @@
     test_preds = np.array([[2, 0], [0, 2]], int)
     train_correct = np.array([1, 0], int)
     test_correct = np.array([0, 1], int)
 
     mi_x, mi_y = attack_obj._prepare_attack_data(  # pylint: disable=protected-access
         train_preds, test_preds, train_correct=train_correct, test_correct=test_correct
     )
-    np.testing.assert_array_equal(mi_y, np.array([1, 1, 0, 0], np.int))
+    np.testing.assert_array_equal(mi_y, np.array([1, 1, 0, 0], int))
     # Test the x data produced. Each row should be sorted in descending order
     np.testing.assert_array_equal(
         mi_x, np.array([[1, 0, 1], [1, 0, 0], [2, 0, 0], [2, 0, 1]])
     )
 
     # With sort_probs = False, the rows of x should not be sorted
     attack_obj = worst_case_attack.WorstCaseAttack(
         sort_probs=False, include_model_correct_feature=True
     )
     mi_x, mi_y = attack_obj._prepare_attack_data(  # pylint: disable=protected-access
         train_preds, test_preds, train_correct=train_correct, test_correct=test_correct
     )
-    np.testing.assert_array_equal(mi_y, np.array([1, 1, 0, 0], np.int))
+    np.testing.assert_array_equal(mi_y, np.array([1, 1, 0, 0], int))
     np.testing.assert_array_equal(
         mi_x, np.array([[1, 0, 1], [0, 1, 0], [2, 0, 0], [0, 2, 1]])
     )
 
 
 def test_non_rf_mia():
     """Tests that it is possible to set the attack model via the args
```

