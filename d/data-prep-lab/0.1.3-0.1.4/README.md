# Comparing `tmp/data_prep_lab-0.1.3.tar.gz` & `tmp/data_prep_lab-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_prep_lab-0.1.3.tar", last modified: Mon Apr 22 12:49:34 2024, max compression
+gzip compressed data, was "data_prep_lab-0.1.4.tar", last modified: Fri Apr 26 06:47:03 2024, max compression
```

## Comparing `data_prep_lab-0.1.3.tar` & `data_prep_lab-0.1.4.tar`

### file list

```diff
@@ -1,101 +1,100 @@
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.189223 data_prep_lab-0.1.3/
--rw-r--r--   0 boris      (501) staff       (20)      357 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/.gitignore
--rw-r--r--   0 boris      (501) staff       (20)     2287 2024-04-22 12:48:13.000000 data_prep_lab-0.1.3/Makefile
--rw-r--r--   0 boris      (501) staff       (20)     1879 2024-04-22 12:49:34.188320 data_prep_lab-0.1.3/PKG-INFO
--rw-r--r--   0 boris      (501) staff       (20)      963 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/README.md
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.155384 data_prep_lab-0.1.3/doc/
--rw-r--r--   0 boris      (501) staff       (20)    12755 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/doc/advanced-transform-tutorial.md
--rw-r--r--   0 boris      (501) staff       (20)     7617 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/doc/architecture.md
--rw-r--r--   0 boris      (501) staff       (20)     4940 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/doc/launcher-options.md
--rw-r--r--   0 boris      (501) staff       (20)     1778 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/doc/library-config.md
--rw-r--r--   0 boris      (501) staff       (20)     1607 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/doc/overview.md
--rw-r--r--   0 boris      (501) staff       (20)   137580 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/doc/processing-architecture.jpg
--rw-r--r--   0 boris      (501) staff       (20)     8708 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/doc/simplest-transform-tutorial.md
--rw-r--r--   0 boris      (501) staff       (20)      193 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/doc/testing-e2e-transform.md
--rw-r--r--   0 boris      (501) staff       (20)     5912 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/doc/testing-transforms.md
--rw-r--r--   0 boris      (501) staff       (20)    12175 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/doc/transform-external-resources.md
--rw-r--r--   0 boris      (501) staff       (20)     3666 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/doc/transform-porting.md
--rw-r--r--   0 boris      (501) staff       (20)    10818 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/doc/transform-tutorials.md
--rw-r--r--   0 boris      (501) staff       (20)     1415 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/doc/transformer-utilities.md
--rw-r--r--   0 boris      (501) staff       (20)     3570 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/doc/using_s3_transformers.md
--rw-r--r--   0 boris      (501) staff       (20)     1327 2024-04-22 12:48:17.000000 data_prep_lab-0.1.3/pyproject.toml
--rw-r--r--   0 boris      (501) staff       (20)       38 2024-04-22 12:49:34.189543 data_prep_lab-0.1.3/setup.cfg
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.139320 data_prep_lab-0.1.3/src/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.184844 data_prep_lab-0.1.3/src/data_prep_lab.egg-info/
--rw-r--r--   0 boris      (501) staff       (20)     1879 2024-04-22 12:49:33.000000 data_prep_lab-0.1.3/src/data_prep_lab.egg-info/PKG-INFO
--rw-r--r--   0 boris      (501) staff       (20)     3063 2024-04-22 12:49:34.000000 data_prep_lab-0.1.3/src/data_prep_lab.egg-info/SOURCES.txt
--rw-r--r--   0 boris      (501) staff       (20)        1 2024-04-22 12:49:33.000000 data_prep_lab-0.1.3/src/data_prep_lab.egg-info/dependency_links.txt
--rw-r--r--   0 boris      (501) staff       (20)      249 2024-04-22 12:49:33.000000 data_prep_lab-0.1.3/src/data_prep_lab.egg-info/requires.txt
--rw-r--r--   0 boris      (501) staff       (20)       16 2024-04-22 12:49:33.000000 data_prep_lab-0.1.3/src/data_prep_lab.egg-info/top_level.txt
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.157929 data_prep_lab-0.1.3/src/data_processing/
--rw-r--r--   0 boris      (501) staff       (20)        0 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/__init__.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.161591 data_prep_lab-0.1.3/src/data_processing/data_access/
--rw-r--r--   0 boris      (501) staff       (20)      427 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/data_access/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     8830 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/data_access/arrow_s3.py
--rw-r--r--   0 boris      (501) staff       (20)     8484 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/data_access/data_access.py
--rw-r--r--   0 boris      (501) staff       (20)    11316 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/data_access/data_access_factory.py
--rw-r--r--   0 boris      (501) staff       (20)     5647 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/data_access/data_access_factory_base.py
--rw-r--r--   0 boris      (501) staff       (20)    15024 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/data_access/data_access_local.py
--rw-r--r--   0 boris      (501) staff       (20)    13499 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/data_access/data_access_s3.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.165270 data_prep_lab-0.1.3/src/data_processing/ray/
--rw-r--r--   0 boris      (501) staff       (20)      574 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/ray/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     7404 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/ray/ray_utils.py
--rw-r--r--   0 boris      (501) staff       (20)     4760 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/ray/transform_launcher.py
--rw-r--r--   0 boris      (501) staff       (20)     6380 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/ray/transform_orchestrator.py
--rw-r--r--   0 boris      (501) staff       (20)     5210 2024-04-22 07:37:39.000000 data_prep_lab-0.1.3/src/data_processing/ray/transform_orchestrator_configuration.py
--rw-r--r--   0 boris      (501) staff       (20)     7253 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/ray/transform_runtime.py
--rw-r--r--   0 boris      (501) staff       (20)     3073 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/ray/transform_statistics.py
--rw-r--r--   0 boris      (501) staff       (20)     9498 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/ray/transform_table_processor.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.166325 data_prep_lab-0.1.3/src/data_processing/test_support/
--rw-r--r--   0 boris      (501) staff       (20)       62 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/test_support/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     8234 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/test_support/abstract_test.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.167341 data_prep_lab-0.1.3/src/data_processing/test_support/ray/
--rw-r--r--   0 boris      (501) staff       (20)       58 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/test_support/ray/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     4686 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/test_support/ray/transform_test.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.168774 data_prep_lab-0.1.3/src/data_processing/test_support/transform/
--rw-r--r--   0 boris      (501) staff       (20)      120 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/test_support/transform/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     4050 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/test_support/transform/noop_transform.py
--rw-r--r--   0 boris      (501) staff       (20)     4476 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/test_support/transform/transform_test.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.169601 data_prep_lab-0.1.3/src/data_processing/transform/
--rw-r--r--   0 boris      (501) staff       (20)       77 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/transform/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     2298 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/transform/table_transform.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.172758 data_prep_lab-0.1.3/src/data_processing/utils/
--rw-r--r--   0 boris      (501) staff       (20)      354 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/utils/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     3135 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/utils/cli_utils.py
--rw-r--r--   0 boris      (501) staff       (20)     1695 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/utils/config.py
--rw-r--r--   0 boris      (501) staff       (20)     2052 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/utils/log.py
--rw-r--r--   0 boris      (501) staff       (20)     6029 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/utils/params_utils.py
--rw-r--r--   0 boris      (501) staff       (20)     6740 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/src/data_processing/utils/transform_utils.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.144341 data_prep_lab-0.1.3/test/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.145407 data_prep_lab-0.1.3/test/data_processing_tests/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.181115 data_prep_lab-0.1.3/test/data_processing_tests/data_access/
--rw-r--r--   0 boris      (501) staff       (20)    24548 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/test/data_processing_tests/data_access/data_access_local_test.py
--rw-r--r--   0 boris      (501) staff       (20)     5734 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/test/data_processing_tests/data_access/data_access_s3_test.py
--rw-r--r--   0 boris      (501) staff       (20)     1545 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/test/data_processing_tests/data_access/sample_input_data_test.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.182670 data_prep_lab-0.1.3/test/data_processing_tests/ray/
--rw-r--r--   0 boris      (501) staff       (20)     9851 2024-04-22 07:41:21.000000 data_prep_lab-0.1.3/test/data_processing_tests/ray/launcher_test.py
--rw-r--r--   0 boris      (501) staff       (20)     3282 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/test/data_processing_tests/ray/ray_util_test.py
--rw-r--r--   0 boris      (501) staff       (20)     1685 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/test/data_processing_tests/ray/test_noop_launch.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.183277 data_prep_lab-0.1.3/test/data_processing_tests/transform/
--rw-r--r--   0 boris      (501) staff       (20)     1678 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/test/data_processing_tests/transform/test_noop.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.183885 data_prep_lab-0.1.3/test/data_processing_tests/util/
--rw-r--r--   0 boris      (501) staff       (20)     1386 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/test/data_processing_tests/util/transform_utils_test.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.142084 data_prep_lab-0.1.3/test-data/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.143145 data_prep_lab-0.1.3/test-data/data_processing/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.173351 data_prep_lab-0.1.3/test-data/data_processing/input/
--rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/test-data/data_processing/input/sample1.parquet
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.175721 data_prep_lab-0.1.3/test-data/data_processing/input_multiple/
--rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/test-data/data_processing/input_multiple/sample1.parquet
--rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/test-data/data_processing/input_multiple/sample2.parquet
--rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/test-data/data_processing/input_multiple/sample3.parquet
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.143282 data_prep_lab-0.1.3/test-data/data_processing/ray/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.143799 data_prep_lab-0.1.3/test-data/data_processing/ray/noop/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.177216 data_prep_lab-0.1.3/test-data/data_processing/ray/noop/expected/
--rw-r--r--   0 boris      (501) staff       (20)     1128 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/test-data/data_processing/ray/noop/expected/metadata.json
--rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/test-data/data_processing/ray/noop/expected/sample1.parquet
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.178005 data_prep_lab-0.1.3/test-data/data_processing/ray/noop/expected/subdir/
--rw-r--r--   0 boris      (501) staff       (20)      753 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/test-data/data_processing/ray/noop/expected/subdir/test1.parquet
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.178658 data_prep_lab-0.1.3/test-data/data_processing/ray/noop/input/
--rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/test-data/data_processing/ray/noop/input/sample1.parquet
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-22 12:49:34.179337 data_prep_lab-0.1.3/test-data/data_processing/ray/noop/input/subdir/
--rw-r--r--   0 boris      (501) staff       (20)      753 2024-04-20 08:49:10.000000 data_prep_lab-0.1.3/test-data/data_processing/ray/noop/input/subdir/test1.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.392725 data_prep_lab-0.1.4/
+-rw-r--r--   0 boris      (501) staff       (20)      357 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/.gitignore
+-rw-r--r--   0 boris      (501) staff       (20)     2287 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/Makefile
+-rw-r--r--   0 boris      (501) staff       (20)     1879 2024-04-26 06:47:03.392127 data_prep_lab-0.1.4/PKG-INFO
+-rw-r--r--   0 boris      (501) staff       (20)      963 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/README.md
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.317793 data_prep_lab-0.1.4/doc/
+-rw-r--r--   0 boris      (501) staff       (20)    12742 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/doc/advanced-transform-tutorial.md
+-rw-r--r--   0 boris      (501) staff       (20)     7617 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/doc/architecture.md
+-rw-r--r--   0 boris      (501) staff       (20)     4940 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/doc/launcher-options.md
+-rw-r--r--   0 boris      (501) staff       (20)     1562 2024-04-24 17:03:36.000000 data_prep_lab-0.1.4/doc/overview.md
+-rw-r--r--   0 boris      (501) staff       (20)   137580 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/doc/processing-architecture.jpg
+-rw-r--r--   0 boris      (501) staff       (20)     8678 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/doc/simplest-transform-tutorial.md
+-rw-r--r--   0 boris      (501) staff       (20)      193 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/doc/testing-e2e-transform.md
+-rw-r--r--   0 boris      (501) staff       (20)     5912 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/doc/testing-transforms.md
+-rw-r--r--   0 boris      (501) staff       (20)    12175 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/doc/transform-external-resources.md
+-rw-r--r--   0 boris      (501) staff       (20)     3666 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/doc/transform-porting.md
+-rw-r--r--   0 boris      (501) staff       (20)    10818 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/doc/transform-tutorials.md
+-rw-r--r--   0 boris      (501) staff       (20)     1415 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/doc/transformer-utilities.md
+-rw-r--r--   0 boris      (501) staff       (20)     3562 2024-04-24 17:03:36.000000 data_prep_lab-0.1.4/doc/using_s3_transformers.md
+-rw-r--r--   0 boris      (501) staff       (20)     1327 2024-04-26 06:45:51.000000 data_prep_lab-0.1.4/pyproject.toml
+-rw-r--r--   0 boris      (501) staff       (20)       38 2024-04-26 06:47:03.392863 data_prep_lab-0.1.4/setup.cfg
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.294042 data_prep_lab-0.1.4/src/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.389375 data_prep_lab-0.1.4/src/data_prep_lab.egg-info/
+-rw-r--r--   0 boris      (501) staff       (20)     1879 2024-04-26 06:47:03.000000 data_prep_lab-0.1.4/src/data_prep_lab.egg-info/PKG-INFO
+-rw-r--r--   0 boris      (501) staff       (20)     3041 2024-04-26 06:47:03.000000 data_prep_lab-0.1.4/src/data_prep_lab.egg-info/SOURCES.txt
+-rw-r--r--   0 boris      (501) staff       (20)        1 2024-04-26 06:47:03.000000 data_prep_lab-0.1.4/src/data_prep_lab.egg-info/dependency_links.txt
+-rw-r--r--   0 boris      (501) staff       (20)      249 2024-04-26 06:47:03.000000 data_prep_lab-0.1.4/src/data_prep_lab.egg-info/requires.txt
+-rw-r--r--   0 boris      (501) staff       (20)       16 2024-04-26 06:47:03.000000 data_prep_lab-0.1.4/src/data_prep_lab.egg-info/top_level.txt
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.321200 data_prep_lab-0.1.4/src/data_processing/
+-rw-r--r--   0 boris      (501) staff       (20)        0 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/__init__.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.326662 data_prep_lab-0.1.4/src/data_processing/data_access/
+-rw-r--r--   0 boris      (501) staff       (20)      427 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/data_access/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     8830 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/data_access/arrow_s3.py
+-rw-r--r--   0 boris      (501) staff       (20)     8484 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/data_access/data_access.py
+-rw-r--r--   0 boris      (501) staff       (20)    11316 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/data_access/data_access_factory.py
+-rw-r--r--   0 boris      (501) staff       (20)     5647 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/data_access/data_access_factory_base.py
+-rw-r--r--   0 boris      (501) staff       (20)    15024 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/data_access/data_access_local.py
+-rw-r--r--   0 boris      (501) staff       (20)    13499 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/data_access/data_access_s3.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.333363 data_prep_lab-0.1.4/src/data_processing/ray/
+-rw-r--r--   0 boris      (501) staff       (20)      574 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/ray/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     7404 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/ray/ray_utils.py
+-rw-r--r--   0 boris      (501) staff       (20)     4760 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/ray/transform_launcher.py
+-rw-r--r--   0 boris      (501) staff       (20)     6388 2024-04-26 06:30:19.000000 data_prep_lab-0.1.4/src/data_processing/ray/transform_orchestrator.py
+-rw-r--r--   0 boris      (501) staff       (20)     5210 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/ray/transform_orchestrator_configuration.py
+-rw-r--r--   0 boris      (501) staff       (20)     7261 2024-04-26 06:30:19.000000 data_prep_lab-0.1.4/src/data_processing/ray/transform_runtime.py
+-rw-r--r--   0 boris      (501) staff       (20)     3073 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/ray/transform_statistics.py
+-rw-r--r--   0 boris      (501) staff       (20)     9498 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/ray/transform_table_processor.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.334899 data_prep_lab-0.1.4/src/data_processing/test_support/
+-rw-r--r--   0 boris      (501) staff       (20)       62 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/test_support/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     8234 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/test_support/abstract_test.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.336397 data_prep_lab-0.1.4/src/data_processing/test_support/ray/
+-rw-r--r--   0 boris      (501) staff       (20)       58 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/test_support/ray/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     4686 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/test_support/ray/transform_test.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.338722 data_prep_lab-0.1.4/src/data_processing/test_support/transform/
+-rw-r--r--   0 boris      (501) staff       (20)      120 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/test_support/transform/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     4050 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/test_support/transform/noop_transform.py
+-rw-r--r--   0 boris      (501) staff       (20)     4476 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/test_support/transform/transform_test.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.340268 data_prep_lab-0.1.4/src/data_processing/transform/
+-rw-r--r--   0 boris      (501) staff       (20)       77 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/transform/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     2298 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/transform/table_transform.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.344696 data_prep_lab-0.1.4/src/data_processing/utils/
+-rw-r--r--   0 boris      (501) staff       (20)      354 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/utils/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     3135 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/utils/cli_utils.py
+-rw-r--r--   0 boris      (501) staff       (20)     1695 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/utils/config.py
+-rw-r--r--   0 boris      (501) staff       (20)     2052 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/utils/log.py
+-rw-r--r--   0 boris      (501) staff       (20)     6029 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/utils/params_utils.py
+-rw-r--r--   0 boris      (501) staff       (20)     6740 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/src/data_processing/utils/transform_utils.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.298992 data_prep_lab-0.1.4/test/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.300250 data_prep_lab-0.1.4/test/data_processing_tests/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.357686 data_prep_lab-0.1.4/test/data_processing_tests/data_access/
+-rw-r--r--   0 boris      (501) staff       (20)    24548 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/test/data_processing_tests/data_access/data_access_local_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     5734 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/test/data_processing_tests/data_access/data_access_s3_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     1545 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/test/data_processing_tests/data_access/sample_input_data_test.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.384677 data_prep_lab-0.1.4/test/data_processing_tests/ray/
+-rw-r--r--   0 boris      (501) staff       (20)     9851 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/test/data_processing_tests/ray/launcher_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     3282 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/test/data_processing_tests/ray/ray_util_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     1685 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/test/data_processing_tests/ray/test_noop_launch.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.387238 data_prep_lab-0.1.4/test/data_processing_tests/transform/
+-rw-r--r--   0 boris      (501) staff       (20)     1678 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/test/data_processing_tests/transform/test_noop.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.388052 data_prep_lab-0.1.4/test/data_processing_tests/util/
+-rw-r--r--   0 boris      (501) staff       (20)     1386 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/test/data_processing_tests/util/transform_utils_test.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.296081 data_prep_lab-0.1.4/test-data/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.296817 data_prep_lab-0.1.4/test-data/data_processing/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.345411 data_prep_lab-0.1.4/test-data/data_processing/input/
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/test-data/data_processing/input/sample1.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.349832 data_prep_lab-0.1.4/test-data/data_processing/input_multiple/
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/test-data/data_processing/input_multiple/sample1.parquet
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/test-data/data_processing/input_multiple/sample2.parquet
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/test-data/data_processing/input_multiple/sample3.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.296968 data_prep_lab-0.1.4/test-data/data_processing/ray/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.297953 data_prep_lab-0.1.4/test-data/data_processing/ray/noop/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.351939 data_prep_lab-0.1.4/test-data/data_processing/ray/noop/expected/
+-rw-r--r--   0 boris      (501) staff       (20)     1128 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/test-data/data_processing/ray/noop/expected/metadata.json
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/test-data/data_processing/ray/noop/expected/sample1.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.353307 data_prep_lab-0.1.4/test-data/data_processing/ray/noop/expected/subdir/
+-rw-r--r--   0 boris      (501) staff       (20)      753 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/test-data/data_processing/ray/noop/expected/subdir/test1.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.354148 data_prep_lab-0.1.4/test-data/data_processing/ray/noop/input/
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/test-data/data_processing/ray/noop/input/sample1.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:47:03.355028 data_prep_lab-0.1.4/test-data/data_processing/ray/noop/input/subdir/
+-rw-r--r--   0 boris      (501) staff       (20)      753 2024-04-23 18:07:37.000000 data_prep_lab-0.1.4/test-data/data_processing/ray/noop/input/subdir/test1.parquet
```

### Comparing `data_prep_lab-0.1.3/Makefile` & `data_prep_lab-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/PKG-INFO` & `data_prep_lab-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_prep_lab
-Version: 0.1.3
+Version: 0.1.4
 Summary: Data Preparation Laboratory Library
 Author-email: David Wood <dawood@us.ibm.com>, Boris Lublinsky <blublinsky@ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: ray[default]==2.9.3
 Requires-Dist: pyarrow==15.0.2
```

### Comparing `data_prep_lab-0.1.3/README.md` & `data_prep_lab-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/doc/advanced-transform-tutorial.md` & `data_prep_lab-0.1.4/doc/advanced-transform-tutorial.md`

 * *Files 4% similar despite different names*

```diff
@@ -265,20 +265,18 @@
 ```
 The launcher requires only an instance of DefaultTableTransformConfiguration
 (our `EdedupTransformConfiguration` class).
 A single method `launch()` is then invoked to run the transform in a Ray cluster.
 
 ## Running
 
-Assuming the above `main()` is placed in `ededup_transform.py` we can run the transform on data
-in COS as follows:
+Assuming the above `main()` is placed in `ededup_transform.py` we can run the transform on local data as follows:
 
 ```shell
-python ededup_transform.py --hash_cpu 0.5 --num_hashes 2 --doc_column "contents" \
+python ededup_transform.py --ededup_hash_cpu 0.5 --ededup_num_hashes 2  --ededup_doc_column "contents" \
   --run_locally True  \
-  --s3_cred "{'access_key': 'KEY', 'secret_key': 'SECRET', 'cos_url': 'https://s3.us-east.cloud-object-storage.appdomain.cloud'}" \
-  --s3_config "{'input_folder': 'input_folder', 'output_folder': 'output_folder'}"
+  --data_local_config="{'input_folder': '<project location>/transforms/universal/ededup/test-data/input', 'output_folder': '<project location>/transforms/universal/ededup/output'}"
 ```
 This is a minimal set of options to run locally.
 See the [launcher options](launcher-options.md) for a complete list of
 transform-independent command line options.
```

### Comparing `data_prep_lab-0.1.3/doc/architecture.md` & `data_prep_lab-0.1.4/doc/architecture.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/doc/launcher-options.md` & `data_prep_lab-0.1.4/doc/launcher-options.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/doc/overview.md` & `data_prep_lab-0.1.4/doc/overview.md`

 * *Files 18% similar despite different names*

```diff
@@ -16,11 +16,10 @@
 command line arguments specific to transform, and the short name for the transform.
 * [Transformation Runtime](../src/data_processing/ray/transform_runtime.py) - allows for customization of the Ray environment for the transformer.
 This might include provisioning of shared memory objects or creation of additional actors.
 
 To learn more consider the following:
 * [Transform Tutorials](transform-tutorials.md)
 * [Testing transformers with S3](using_s3_transformers.md)
-* [Library Configuration](library-config.md)
 * [Architecture Deep Dive](architecture.md)
 * [Transform project root readme](../../transforms/README.md)
```

### Comparing `data_prep_lab-0.1.3/doc/processing-architecture.jpg` & `data_prep_lab-0.1.4/doc/processing-architecture.jpg`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/doc/simplest-transform-tutorial.md` & `data_prep_lab-0.1.4/doc/simplest-transform-tutorial.md`

 * *Files 4% similar despite different names*

```diff
@@ -176,20 +176,19 @@
 ```
 The launcher requires only an instance of DefaultTableTransformConfiguration 
 (our `NOOPTransformConfiguration` class).
 A single method `launch()` is then invoked to run the transform in a Ray cluster.
 
 ## Running
 
-Assuming the above `main()` is placed in `noop_main.py` we can run the transform on data 
-in COS as follows:
+Assuming the above `main()` is placed in `noop_main.py` we can run the transform on local data as follows:
 
 ```shell
-python noop_main.py --noop_sleep_msec 2 \
-  --run_locally True  \
-  --s3_cred "{'access_key': 'access', 'secret_key': 'secret', 'url': 'https://s3.us-east.cloud-object-storage.appdomain.cloud'}" \
-  --s3_config "{'input_folder': 'input_folder', 'output_folder': 'output_folder'}"
+python noop_transform.py \
+  --noop_sleep_sec 2  \
+  --run_locally=True  \
+  --data_local_config="{'input_folder': '<project location>/transforms/universal/noop/test-data/input', 'output_folder': '<project location>/transforms/universal/noop/output'}"
 ```
 This is a minimal set of options to run locally.
 See the [launcher options](launcher-options.md) for a complete list of
 transform-independent command line options.
```

### Comparing `data_prep_lab-0.1.3/doc/testing-transforms.md` & `data_prep_lab-0.1.4/doc/testing-transforms.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/doc/transform-external-resources.md` & `data_prep_lab-0.1.4/doc/transform-external-resources.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/doc/transform-porting.md` & `data_prep_lab-0.1.4/doc/transform-porting.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/doc/transform-tutorials.md` & `data_prep_lab-0.1.4/doc/transform-tutorials.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/doc/transformer-utilities.md` & `data_prep_lab-0.1.4/doc/transformer-utilities.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/doc/using_s3_transformers.md` & `data_prep_lab-0.1.4/doc/using_s3_transformers.md`

 * *Files 4% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 ```
 
 Once the bucket is created, you can copy files (assuming you are in the transforms directory), using:
 
 ```shell
 mc cp --recursive tools/ingest2parquet/test-data/input/ local/test/ingest2parquet/input
 mc cp --recursive code/code_quality/test-data/input/ local/test/code_quality/input
-mc cp --recursive code/language_annotator/test-data/input/ local/test/language_annotator/input
-mc cp --recursive code/language_annotator/test-data/languages/ local/test/lang_annotator/languages
+mc cp --recursive code/proglang_select/test-data/input/ local/test/proglang_select/input
+mc cp --recursive code/proglang_select/test-data/languages/ local/test/proglang_select/languages
 mc cp --recursive code/malware/test-data/input/ local/test/malware/input
 
 mc cp --recursive language/doc_quality/test-data/input/ local/test/doc_quality/input
 mc cp --recursive language/language_id/test-data/input/ local/test/language_id/input
 
 mc cp --recursive universal/blocklist/test-data/input/ local/test/blocklist/input
 mc cp --recursive universal/blocklist/test-data/domains/ local/test/blocklist/domains
```

### Comparing `data_prep_lab-0.1.3/pyproject.toml` & `data_prep_lab-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "data_prep_lab"
-version = "0.1.3"
+version = "0.1.4"
 requires-python = ">=3.10"
 description = "Data Preparation Laboratory Library"
 license = {text = "Apache-2.0"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     { name = "David Wood", email = "dawood@us.ibm.com" },
     { name = "Boris Lublinsky", email = "blublinsky@ibm.com" },
```

### Comparing `data_prep_lab-0.1.3/src/data_prep_lab.egg-info/PKG-INFO` & `data_prep_lab-0.1.4/src/data_prep_lab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_prep_lab
-Version: 0.1.3
+Version: 0.1.4
 Summary: Data Preparation Laboratory Library
 Author-email: David Wood <dawood@us.ibm.com>, Boris Lublinsky <blublinsky@ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: ray[default]==2.9.3
 Requires-Dist: pyarrow==15.0.2
```

### Comparing `data_prep_lab-0.1.3/src/data_prep_lab.egg-info/SOURCES.txt` & `data_prep_lab-0.1.4/src/data_prep_lab.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .gitignore
 Makefile
 README.md
 pyproject.toml
 doc/advanced-transform-tutorial.md
 doc/architecture.md
 doc/launcher-options.md
-doc/library-config.md
 doc/overview.md
 doc/processing-architecture.jpg
 doc/simplest-transform-tutorial.md
 doc/testing-e2e-transform.md
 doc/testing-transforms.md
 doc/transform-external-resources.md
 doc/transform-porting.md
```

### Comparing `data_prep_lab-0.1.3/src/data_processing/data_access/arrow_s3.py` & `data_prep_lab-0.1.4/src/data_processing/data_access/arrow_s3.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/data_access/data_access.py` & `data_prep_lab-0.1.4/src/data_processing/data_access/data_access.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/data_access/data_access_factory.py` & `data_prep_lab-0.1.4/src/data_processing/data_access/data_access_factory.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/data_access/data_access_factory_base.py` & `data_prep_lab-0.1.4/src/data_processing/data_access/data_access_factory_base.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/data_access/data_access_local.py` & `data_prep_lab-0.1.4/src/data_processing/data_access/data_access_local.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/data_access/data_access_s3.py` & `data_prep_lab-0.1.4/src/data_processing/data_access/data_access_s3.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/ray/__init__.py` & `data_prep_lab-0.1.4/src/data_processing/ray/__init__.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/ray/ray_utils.py` & `data_prep_lab-0.1.4/src/data_processing/ray/ray_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/ray/transform_launcher.py` & `data_prep_lab-0.1.4/src/data_processing/ray/transform_launcher.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/ray/transform_orchestrator.py` & `data_prep_lab-0.1.4/src/data_processing/ray/transform_orchestrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ################################################################################
 
 import time
 import traceback
 from datetime import datetime
 
 import ray
-from data_processing.data_access import DataAccessFactory
+from data_processing.data_access import DataAccessFactoryBase
 from data_processing.ray import (
     DefaultTableTransformConfiguration,
     RayUtils,
     TransformOrchestratorConfiguration,
     TransformStatistics,
     TransformTableProcessor,
 )
@@ -30,15 +30,15 @@
 
 logger = get_logger(__name__)
 
 
 @ray.remote(num_cpus=1, scheduling_strategy="SPREAD")
 def orchestrate(
     preprocessing_params: TransformOrchestratorConfiguration,
-    data_access_factory: DataAccessFactory,
+    data_access_factory: DataAccessFactoryBase,
     transform_runtime_config: DefaultTableTransformConfiguration,
 ) -> int:
     """
     orchestrator for transformer execution
     :param preprocessing_params: orchestrator configuration
     :param data_access_factory: data access factory
     :param transform_runtime_config: transformer runtime configuration
```

### Comparing `data_prep_lab-0.1.3/src/data_processing/ray/transform_orchestrator_configuration.py` & `data_prep_lab-0.1.4/src/data_processing/ray/transform_orchestrator_configuration.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/ray/transform_runtime.py` & `data_prep_lab-0.1.4/src/data_processing/ray/transform_runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 import argparse
 from typing import Any
 
-from data_processing.data_access import DataAccessFactory
+from data_processing.data_access import DataAccessFactoryBase
 from data_processing.transform import AbstractTableTransform
 from data_processing.utils import CLIArgumentProvider
 from ray.actor import ActorHandle
 
 
 class DefaultTableTransformRuntime:
     """
@@ -28,15 +28,15 @@
         """
         Create/config this runtime.
         :param params: parameters, often provided by the CLI arguments as defined by a TableTansformConfiguration.
         """
         self.params = params
 
     def get_transform_config(
-        self, data_access_factory: DataAccessFactory, statistics: ActorHandle, files: list[str]
+        self, data_access_factory: DataAccessFactoryBase, statistics: ActorHandle, files: list[str]
     ) -> dict[str, Any]:
         """
         Get the dictionary of configuration that will be provided to the transform's initializer.
         This is the opportunity for this runtime to create a new set of configuration based on the
         config/params provided to this instance's initializer.  This may include the addition
         of new configuration data such as ray shared memory, new actors, etc, that might be needed and
         expected by the transform in its initializer and/or transform() methods.
```

### Comparing `data_prep_lab-0.1.3/src/data_processing/ray/transform_statistics.py` & `data_prep_lab-0.1.4/src/data_processing/ray/transform_statistics.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/ray/transform_table_processor.py` & `data_prep_lab-0.1.4/src/data_processing/ray/transform_table_processor.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/test_support/abstract_test.py` & `data_prep_lab-0.1.4/src/data_processing/test_support/abstract_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/test_support/ray/transform_test.py` & `data_prep_lab-0.1.4/src/data_processing/test_support/ray/transform_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/test_support/transform/noop_transform.py` & `data_prep_lab-0.1.4/src/data_processing/test_support/transform/noop_transform.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/test_support/transform/transform_test.py` & `data_prep_lab-0.1.4/src/data_processing/test_support/transform/transform_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/transform/table_transform.py` & `data_prep_lab-0.1.4/src/data_processing/transform/table_transform.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/utils/cli_utils.py` & `data_prep_lab-0.1.4/src/data_processing/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/utils/config.py` & `data_prep_lab-0.1.4/src/data_processing/utils/config.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/utils/log.py` & `data_prep_lab-0.1.4/src/data_processing/utils/log.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/utils/params_utils.py` & `data_prep_lab-0.1.4/src/data_processing/utils/params_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/src/data_processing/utils/transform_utils.py` & `data_prep_lab-0.1.4/src/data_processing/utils/transform_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/test/data_processing_tests/data_access/data_access_local_test.py` & `data_prep_lab-0.1.4/test/data_processing_tests/data_access/data_access_local_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/test/data_processing_tests/data_access/data_access_s3_test.py` & `data_prep_lab-0.1.4/test/data_processing_tests/data_access/data_access_s3_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/test/data_processing_tests/data_access/sample_input_data_test.py` & `data_prep_lab-0.1.4/test/data_processing_tests/data_access/sample_input_data_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/test/data_processing_tests/ray/launcher_test.py` & `data_prep_lab-0.1.4/test/data_processing_tests/ray/launcher_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/test/data_processing_tests/ray/ray_util_test.py` & `data_prep_lab-0.1.4/test/data_processing_tests/ray/ray_util_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/test/data_processing_tests/ray/test_noop_launch.py` & `data_prep_lab-0.1.4/test/data_processing_tests/ray/test_noop_launch.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/test/data_processing_tests/transform/test_noop.py` & `data_prep_lab-0.1.4/test/data_processing_tests/transform/test_noop.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/test/data_processing_tests/util/transform_utils_test.py` & `data_prep_lab-0.1.4/test/data_processing_tests/util/transform_utils_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/test-data/data_processing/input/sample1.parquet` & `data_prep_lab-0.1.4/test-data/data_processing/input/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/test-data/data_processing/input_multiple/sample1.parquet` & `data_prep_lab-0.1.4/test-data/data_processing/input_multiple/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/test-data/data_processing/input_multiple/sample2.parquet` & `data_prep_lab-0.1.4/test-data/data_processing/input_multiple/sample2.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/test-data/data_processing/input_multiple/sample3.parquet` & `data_prep_lab-0.1.4/test-data/data_processing/input_multiple/sample3.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/test-data/data_processing/ray/noop/expected/metadata.json` & `data_prep_lab-0.1.4/test-data/data_processing/ray/noop/expected/metadata.json`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/test-data/data_processing/ray/noop/expected/sample1.parquet` & `data_prep_lab-0.1.4/test-data/data_processing/ray/noop/expected/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/test-data/data_processing/ray/noop/expected/subdir/test1.parquet` & `data_prep_lab-0.1.4/test-data/data_processing/ray/noop/expected/subdir/test1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/test-data/data_processing/ray/noop/input/sample1.parquet` & `data_prep_lab-0.1.4/test-data/data_processing/ray/noop/input/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.3/test-data/data_processing/ray/noop/input/subdir/test1.parquet` & `data_prep_lab-0.1.4/test-data/data_processing/ray/noop/input/subdir/test1.parquet`

 * *Files identical despite different names*

