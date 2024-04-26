# Comparing `tmp/bioimageio.core-0.6.0.tar.gz` & `tmp/bioimageio.core-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio.core-0.6.0.tar", last modified: Tue Apr 23 23:21:59 2024, max compression
+gzip compressed data, was "bioimageio.core-0.6.1.tar", last modified: Fri Apr 26 08:10:14 2024, max compression
```

## Comparing `bioimageio.core-0.6.0.tar` & `bioimageio.core-0.6.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.273630 bioimageio.core-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 23:21:21.000000 bioimageio.core-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-23 23:21:59.273630 bioimageio.core-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.257630 bioimageio.core-0.6.0/bioimageio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.265630 bioimageio.core-0.6.0/bioimageio/core/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/_magic_tensor_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/_op_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/_prediction_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/_resource_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/block_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/digest_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.265630 bioimageio.core-0.6.0/bioimageio/core/model_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/model_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/model_adapters/_keras_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/model_adapters/_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/model_adapters/_onnx_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/model_adapters/_pytorch_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/model_adapters/_tensorflow_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/model_adapters/_torchscript_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)    21626 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/proc_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/proc_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    20495 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/stat_calculators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/stat_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)    16351 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.265630 bioimageio.core-0.6.0/bioimageio/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.269630 bioimageio.core-0.6.0/bioimageio/core/weight_converter/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/weight_converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.269630 bioimageio.core-0.6.0/bioimageio/core/weight_converter/keras/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/weight_converter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/weight_converter/keras/_tensorflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.269630 bioimageio.core-0.6.0/bioimageio/core/weight_converter/torch/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/weight_converter/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/weight_converter/torch/_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/weight_converter/torch/_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/weight_converter/torch/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.261630 bioimageio.core-0.6.0/bioimageio.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-23 23:21:59.000000 bioimageio.core-0.6.0/bioimageio.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-23 23:21:59.000000 bioimageio.core-0.6.0/bioimageio.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 23:21:59.000000 bioimageio.core-0.6.0/bioimageio.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 23:21:59.000000 bioimageio.core-0.6.0/bioimageio.core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-23 23:21:59.000000 bioimageio.core-0.6.0/bioimageio.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 23:21:59.000000 bioimageio.core-0.6.0/bioimageio.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.269630 bioimageio.core-0.6.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/scripts/setup_dev_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/scripts/show_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 23:21:59.273630 bioimageio.core-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.269630 bioimageio.core-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_any_model_fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_bioimageio_spec_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_digest_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_prediction_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_prediction_pipeline_device_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_proc_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_resource_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_stat_calculators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_stat_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.269630 bioimageio.core-0.6.0/tests/weight_converter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.269630 bioimageio.core-0.6.0/tests/weight_converter/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/weight_converter/keras/test_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/weight_converter/test_add_weights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.273630 bioimageio.core-0.6.0/tests/weight_converter/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/weight_converter/torch/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/weight_converter/torch/test_torchscript.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.359664 bioimageio.core-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-26 08:10:14.359664 bioimageio.core-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-26 08:10:11.000000 bioimageio.core-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.347664 bioimageio.core-0.6.1/bioimageio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.351664 bioimageio.core-0.6.1/bioimageio/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-26 08:10:11.000000 bioimageio.core-0.6.1/bioimageio/core/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/_magic_tensor_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/_op_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/_prediction_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/_resource_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/block_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12279 2024-04-26 08:10:11.000000 bioimageio.core-0.6.1/bioimageio/core/digest_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.355664 bioimageio.core-0.6.1/bioimageio/core/model_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/model_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/model_adapters/_keras_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/model_adapters/_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/model_adapters/_onnx_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/model_adapters/_pytorch_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/model_adapters/_tensorflow_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/model_adapters/_torchscript_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21626 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/proc_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/proc_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20495 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/stat_calculators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/stat_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16351 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.355664 bioimageio.core-0.6.1/bioimageio/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.355664 bioimageio.core-0.6.1/bioimageio/core/weight_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/weight_converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.355664 bioimageio.core-0.6.1/bioimageio/core/weight_converter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/weight_converter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/weight_converter/keras/_tensorflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.355664 bioimageio.core-0.6.1/bioimageio/core/weight_converter/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/weight_converter/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/weight_converter/torch/_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/weight_converter/torch/_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/weight_converter/torch/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.351664 bioimageio.core-0.6.1/bioimageio.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-26 08:10:14.000000 bioimageio.core-0.6.1/bioimageio.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-26 08:10:14.000000 bioimageio.core-0.6.1/bioimageio.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:10:14.000000 bioimageio.core-0.6.1/bioimageio.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 08:10:14.000000 bioimageio.core-0.6.1/bioimageio.core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-26 08:10:14.000000 bioimageio.core-0.6.1/bioimageio.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-26 08:10:14.000000 bioimageio.core-0.6.1/bioimageio.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.355664 bioimageio.core-0.6.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/scripts/setup_dev_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/scripts/show_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 08:10:14.359664 bioimageio.core-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.355664 bioimageio.core-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_any_model_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_bioimageio_spec_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_digest_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_prediction_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_prediction_pipeline_device_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_proc_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_resource_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_stat_calculators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_stat_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.359664 bioimageio.core-0.6.1/tests/weight_converter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.359664 bioimageio.core-0.6.1/tests/weight_converter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/weight_converter/keras/test_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/weight_converter/test_add_weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.359664 bioimageio.core-0.6.1/tests/weight_converter/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/weight_converter/torch/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/weight_converter/torch/test_torchscript.py
```

### Comparing `bioimageio.core-0.6.0/LICENSE` & `bioimageio.core-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/PKG-INFO` & `bioimageio.core-0.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: bioimageio.core
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python functionality for the bioimage model zoo
 Home-page: https://github.com/bioimage-io/core-bioimage-io-python
 Author: Bioimage Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/core-bioimage-io-python/issues
 Project-URL: Source, https://github.com/bioimage-io/core-bioimage-io-python
 Description: # core-bioimage-io-python
         
-        Python specific core utilities for running models in the [BioImage Model Zoo](https://bioimage.io).
+        Python specific core utilities for [bioimage.io]("https://bioimage.io") resources (in particular models).
         
         ## Installation
         
         ### Via Mamba/Conda
         
         The `bioimageio.core` package can be installed from conda-forge via
         
@@ -72,15 +72,15 @@
         
         ```console
         mamba env create -f dev/env.yaml
         mamba activate core
         pip install -e . --no-deps
         ```
         
-        There are different environment files that only install tensorflow or pytorch as dependencies available.
+        There are different environment files available that only install tensorflow or pytorch as dependencies.
         
         ## 💻 Command Line
         
         `bioimageio.core` installs a command line interface (CLI) for testing models and other functionality.
         You can list all the available commands via:
         
         ```console
@@ -111,27 +111,39 @@
         bioimagei predict-images -m <MODEL> -i <INPUT_PATTERN> - o <OUTPUT_FOLDER>
         ```
         
         `<INPUT_PATTERN>` is a `glob` pattern to select the desired images, e.g. `/path/to/my/images/*.tif`.
         
         ## From python
         
-        `bioimageio.core` is a python library that implements loading models, running prediction with them and more.
-        To get an overview of this functionality, check out the example notebooks:
+        `bioimageio.core` is a python package that implements prediction with bioimageio models
+        including standardized pre- and postprocessing operations.
+        These models are described by---and can be loaded with---the bioimageio.spec package.
         
-        * [example/model_usage](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/model_usage.ipynb) for how to load models and run prediction with them
-        * [example/model_creation](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/model_creation.ipynb) for how to create bioimage.io compatible model packages
-        * [example/dataset_statistics_demo](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/dataset_statistics_demo.ipynb) for how to use the dataset statistics for advanced pre-and-postprocessing
+        In addition bioimageio.core provides functionality to convert model weight formats.
+        
+        To get an overview of this functionality, check out these example notebooks:
+        
+        * [model creation/loading with bioimageio.spec](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example_use/load_model_and_create_your_own.ipynb)
         
         ## Model Specification
         
         The model specification and its validation tools can be found at <https://github.com/bioimage-io/spec-bioimage-io>.
         
         ## Changelog
         
+        ### 0.6.1
+        
+        * Fix [#378](https://github.com/bioimage-io/core-bioimage-io-python/pull/378) (with [#379](https://github.com/bioimage-io/core-bioimage-io-python/pull/379))*
+        
+        ### 0.6.0
+        
+        * add compatibility with new bioimageio.spec 0.5 (0.5.2post1)
+        * improve interfaces
+        
         ### 0.5.10
         
         * [Fix critical bug in predict with tiling](https://github.com/bioimage-io/core-bioimage-io-python/pull/359)
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bioimageio.core-0.6.0/README.md` & `bioimageio.core-0.6.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # core-bioimage-io-python
 
-Python specific core utilities for running models in the [BioImage Model Zoo](https://bioimage.io).
+Python specific core utilities for [bioimage.io]("https://bioimage.io") resources (in particular models).
 
 ## Installation
 
 ### Via Mamba/Conda
 
 The `bioimageio.core` package can be installed from conda-forge via
 
@@ -63,15 +63,15 @@
 
 ```console
 mamba env create -f dev/env.yaml
 mamba activate core
 pip install -e . --no-deps
 ```
 
-There are different environment files that only install tensorflow or pytorch as dependencies available.
+There are different environment files available that only install tensorflow or pytorch as dependencies.
 
 ## 💻 Command Line
 
 `bioimageio.core` installs a command line interface (CLI) for testing models and other functionality.
 You can list all the available commands via:
 
 ```console
@@ -102,23 +102,35 @@
 bioimagei predict-images -m <MODEL> -i <INPUT_PATTERN> - o <OUTPUT_FOLDER>
 ```
 
 `<INPUT_PATTERN>` is a `glob` pattern to select the desired images, e.g. `/path/to/my/images/*.tif`.
 
 ## From python
 
-`bioimageio.core` is a python library that implements loading models, running prediction with them and more.
-To get an overview of this functionality, check out the example notebooks:
+`bioimageio.core` is a python package that implements prediction with bioimageio models
+including standardized pre- and postprocessing operations.
+These models are described by---and can be loaded with---the bioimageio.spec package.
 
-* [example/model_usage](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/model_usage.ipynb) for how to load models and run prediction with them
-* [example/model_creation](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/model_creation.ipynb) for how to create bioimage.io compatible model packages
-* [example/dataset_statistics_demo](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/dataset_statistics_demo.ipynb) for how to use the dataset statistics for advanced pre-and-postprocessing
+In addition bioimageio.core provides functionality to convert model weight formats.
+
+To get an overview of this functionality, check out these example notebooks:
+
+* [model creation/loading with bioimageio.spec](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example_use/load_model_and_create_your_own.ipynb)
 
 ## Model Specification
 
 The model specification and its validation tools can be found at <https://github.com/bioimage-io/spec-bioimage-io>.
 
 ## Changelog
 
+### 0.6.1
+
+* Fix [#378](https://github.com/bioimage-io/core-bioimage-io-python/pull/378) (with [#379](https://github.com/bioimage-io/core-bioimage-io-python/pull/379))*
+
+### 0.6.0
+
+* add compatibility with new bioimageio.spec 0.5 (0.5.2post1)
+* improve interfaces
+
 ### 0.5.10
 
 * [Fix critical bug in predict with tiling](https://github.com/bioimage-io/core-bioimage-io-python/pull/359)
```

### Comparing `bioimageio.core-0.6.0/bioimageio/core/__init__.py` & `bioimageio.core-0.6.1/bioimageio/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/__main__.py` & `bioimageio.core-0.6.1/bioimageio/core/__main__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/_magic_tensor_ops.py` & `bioimageio.core-0.6.1/bioimageio/core/_magic_tensor_ops.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/_op_base.py` & `bioimageio.core-0.6.1/bioimageio/core/_op_base.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/_prediction_pipeline.py` & `bioimageio.core-0.6.1/bioimageio/core/_prediction_pipeline.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/_resource_tests.py` & `bioimageio.core-0.6.1/bioimageio/core/_resource_tests.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/axis.py` & `bioimageio.core-0.6.1/bioimageio/core/axis.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/block.py` & `bioimageio.core-0.6.1/bioimageio/core/block.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/block_meta.py` & `bioimageio.core-0.6.1/bioimageio/core/block_meta.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/common.py` & `bioimageio.core-0.6.1/bioimageio/core/common.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/digest_spec.py` & `bioimageio.core-0.6.1/bioimageio/core/digest_spec.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import importlib.util
-from functools import singledispatch
 from itertools import chain
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     List,
@@ -40,50 +39,40 @@
     SampleBlockMeta,
     sample_block_meta_generator,
 )
 from .stat_measures import Stat
 from .tensor import Tensor
 
 
-@singledispatch
-def import_callable(node: type, /) -> Callable[..., Any]:
+def import_callable(
+    node: Union[CallableFromDepencency, ArchitectureFromLibraryDescr],
+    /,
+    **kwargs: Unpack[HashKwargs],
+) -> Callable[..., Any]:
     """import a callable (e.g. a torch.nn.Module) from a spec node describing it"""
-    raise TypeError(type(node))
+    if isinstance(node, CallableFromDepencency):
+        module = importlib.import_module(node.module_name)
+        c = getattr(module, str(node.callable_name))
+    elif isinstance(node, ArchitectureFromLibraryDescr):
+        module = importlib.import_module(node.import_from)
+        c = getattr(module, str(node.callable))
+    elif isinstance(node, CallableFromFile):
+        c = _import_from_file_impl(node.source_file, str(node.callable_name), **kwargs)
+    elif isinstance(node, ArchitectureFromFileDescr):
+        c = _import_from_file_impl(node.source, str(node.callable), sha256=node.sha256)
 
+    else:
+        assert_never(node)
 
-@import_callable.register
-def _(node: CallableFromDepencency) -> Callable[..., Any]:
-    module = importlib.import_module(node.module_name)
-    c = getattr(module, str(node.callable_name))
     if not callable(c):
         raise ValueError(f"{node} (imported: {c}) is not callable")
 
     return c
 
 
-@import_callable.register
-def _(node: ArchitectureFromLibraryDescr) -> Callable[..., Any]:
-    module = importlib.import_module(node.import_from)
-    c = getattr(module, str(node.callable))
-    if not callable(c):
-        raise ValueError(f"{node} (imported: {c}) is not callable")
-
-    return c
-
-
-@import_callable.register
-def _(node: CallableFromFile, **kwargs: Unpack[HashKwargs]):
-    return _import_from_file_impl(node.source_file, str(node.callable_name), **kwargs)
-
-
-@import_callable.register
-def _(node: ArchitectureFromFileDescr, **kwargs: Unpack[HashKwargs]):
-    return _import_from_file_impl(node.source, str(node.callable), sha256=node.sha256)
-
-
 def _import_from_file_impl(
     source: FileSource, callable_name: str, **kwargs: Unpack[HashKwargs]
 ):
     local_file = download(source, **kwargs)
     module_name = local_file.path.stem
     importlib_spec = importlib.util.spec_from_file_location(
         module_name, local_file.path
```

### Comparing `bioimageio.core-0.6.0/bioimageio/core/io.py` & `bioimageio.core-0.6.1/bioimageio/core/io.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/model_adapters/_keras_model_adapter.py` & `bioimageio.core-0.6.1/bioimageio/core/model_adapters/_keras_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/model_adapters/_model_adapter.py` & `bioimageio.core-0.6.1/bioimageio/core/model_adapters/_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/model_adapters/_onnx_model_adapter.py` & `bioimageio.core-0.6.1/bioimageio/core/model_adapters/_onnx_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/model_adapters/_pytorch_model_adapter.py` & `bioimageio.core-0.6.1/bioimageio/core/model_adapters/_pytorch_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/model_adapters/_tensorflow_model_adapter.py` & `bioimageio.core-0.6.1/bioimageio/core/model_adapters/_tensorflow_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/model_adapters/_torchscript_model_adapter.py` & `bioimageio.core-0.6.1/bioimageio/core/model_adapters/_torchscript_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/proc_ops.py` & `bioimageio.core-0.6.1/bioimageio/core/proc_ops.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/proc_setup.py` & `bioimageio.core-0.6.1/bioimageio/core/proc_setup.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/sample.py` & `bioimageio.core-0.6.1/bioimageio/core/sample.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/stat_calculators.py` & `bioimageio.core-0.6.1/bioimageio/core/stat_calculators.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/stat_measures.py` & `bioimageio.core-0.6.1/bioimageio/core/stat_measures.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/tensor.py` & `bioimageio.core-0.6.1/bioimageio/core/tensor.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/utils/testing.py` & `bioimageio.core-0.6.1/bioimageio/core/utils/testing.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/weight_converter/keras/_tensorflow.py` & `bioimageio.core-0.6.1/bioimageio/core/weight_converter/keras/_tensorflow.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/weight_converter/torch/_onnx.py` & `bioimageio.core-0.6.1/bioimageio/core/weight_converter/torch/_onnx.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/weight_converter/torch/_torchscript.py` & `bioimageio.core-0.6.1/bioimageio/core/weight_converter/torch/_torchscript.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio/core/weight_converter/torch/_utils.py` & `bioimageio.core-0.6.1/bioimageio/core/weight_converter/torch/_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/bioimageio.core.egg-info/PKG-INFO` & `bioimageio.core-0.6.1/bioimageio.core.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: bioimageio.core
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python functionality for the bioimage model zoo
 Home-page: https://github.com/bioimage-io/core-bioimage-io-python
 Author: Bioimage Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/core-bioimage-io-python/issues
 Project-URL: Source, https://github.com/bioimage-io/core-bioimage-io-python
 Description: # core-bioimage-io-python
         
-        Python specific core utilities for running models in the [BioImage Model Zoo](https://bioimage.io).
+        Python specific core utilities for [bioimage.io]("https://bioimage.io") resources (in particular models).
         
         ## Installation
         
         ### Via Mamba/Conda
         
         The `bioimageio.core` package can be installed from conda-forge via
         
@@ -72,15 +72,15 @@
         
         ```console
         mamba env create -f dev/env.yaml
         mamba activate core
         pip install -e . --no-deps
         ```
         
-        There are different environment files that only install tensorflow or pytorch as dependencies available.
+        There are different environment files available that only install tensorflow or pytorch as dependencies.
         
         ## 💻 Command Line
         
         `bioimageio.core` installs a command line interface (CLI) for testing models and other functionality.
         You can list all the available commands via:
         
         ```console
@@ -111,27 +111,39 @@
         bioimagei predict-images -m <MODEL> -i <INPUT_PATTERN> - o <OUTPUT_FOLDER>
         ```
         
         `<INPUT_PATTERN>` is a `glob` pattern to select the desired images, e.g. `/path/to/my/images/*.tif`.
         
         ## From python
         
-        `bioimageio.core` is a python library that implements loading models, running prediction with them and more.
-        To get an overview of this functionality, check out the example notebooks:
+        `bioimageio.core` is a python package that implements prediction with bioimageio models
+        including standardized pre- and postprocessing operations.
+        These models are described by---and can be loaded with---the bioimageio.spec package.
         
-        * [example/model_usage](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/model_usage.ipynb) for how to load models and run prediction with them
-        * [example/model_creation](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/model_creation.ipynb) for how to create bioimage.io compatible model packages
-        * [example/dataset_statistics_demo](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/dataset_statistics_demo.ipynb) for how to use the dataset statistics for advanced pre-and-postprocessing
+        In addition bioimageio.core provides functionality to convert model weight formats.
+        
+        To get an overview of this functionality, check out these example notebooks:
+        
+        * [model creation/loading with bioimageio.spec](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example_use/load_model_and_create_your_own.ipynb)
         
         ## Model Specification
         
         The model specification and its validation tools can be found at <https://github.com/bioimage-io/spec-bioimage-io>.
         
         ## Changelog
         
+        ### 0.6.1
+        
+        * Fix [#378](https://github.com/bioimage-io/core-bioimage-io-python/pull/378) (with [#379](https://github.com/bioimage-io/core-bioimage-io-python/pull/379))*
+        
+        ### 0.6.0
+        
+        * add compatibility with new bioimageio.spec 0.5 (0.5.2post1)
+        * improve interfaces
+        
         ### 0.5.10
         
         * [Fix critical bug in predict with tiling](https://github.com/bioimage-io/core-bioimage-io-python/pull/359)
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bioimageio.core-0.6.0/bioimageio.core.egg-info/SOURCES.txt` & `bioimageio.core-0.6.1/bioimageio.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/pyproject.toml` & `bioimageio.core-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/scripts/setup_dev_env.py` & `bioimageio.core-0.6.1/scripts/setup_dev_env.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/scripts/show_diff.py` & `bioimageio.core-0.6.1/scripts/show_diff.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/setup.py` & `bioimageio.core-0.6.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             "filelock",
             "jupyter",
             "jupyter-black",
             "keras>=3.0",
             "onnxruntime",
             "packaging>=17.0",
             "pre-commit",
+            "pdoc",
             "psutil",  # parallel pytest with 'pytest -n auto'
             "pyright",
             "pytest-xdist",  # parallel pytest
             "pytest",
             "torch>=1.6",
             "torchvision",
         ],
```

### Comparing `bioimageio.core-0.6.0/tests/test_bioimageio_spec_version.py` & `bioimageio.core-0.6.1/tests/test_bioimageio_spec_version.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/tests/test_cli.py` & `bioimageio.core-0.6.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/tests/test_digest_spec.py` & `bioimageio.core-0.6.1/tests/test_digest_spec.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/tests/test_prediction.py` & `bioimageio.core-0.6.1/tests/test_prediction.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/tests/test_prediction_pipeline.py` & `bioimageio.core-0.6.1/tests/test_prediction_pipeline.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/tests/test_prediction_pipeline_device_management.py` & `bioimageio.core-0.6.1/tests/test_prediction_pipeline_device_management.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/tests/test_proc_ops.py` & `bioimageio.core-0.6.1/tests/test_proc_ops.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/tests/test_resource_tests.py` & `bioimageio.core-0.6.1/tests/test_resource_tests.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/tests/test_stat_calculators.py` & `bioimageio.core-0.6.1/tests/test_stat_calculators.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/tests/test_stat_measures.py` & `bioimageio.core-0.6.1/tests/test_stat_measures.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/tests/test_tensor.py` & `bioimageio.core-0.6.1/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/tests/weight_converter/keras/test_tensorflow.py` & `bioimageio.core-0.6.1/tests/weight_converter/keras/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/tests/weight_converter/test_add_weights.py` & `bioimageio.core-0.6.1/tests/weight_converter/test_add_weights.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/tests/weight_converter/torch/test_onnx.py` & `bioimageio.core-0.6.1/tests/weight_converter/torch/test_onnx.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.0/tests/weight_converter/torch/test_torchscript.py` & `bioimageio.core-0.6.1/tests/weight_converter/torch/test_torchscript.py`

 * *Files identical despite different names*

