# Comparing `tmp/autogluon.tabular-1.1.1b20240424.tar.gz` & `tmp/autogluon.tabular-1.1.1b20240425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.tabular-1.1.1b20240424.tar", last modified: Wed Apr 24 09:04:49 2024, max compression
+gzip compressed data, was "autogluon.tabular-1.1.1b20240425.tar", last modified: Thu Apr 25 09:04:59 2024, max compression
```

## Comparing `autogluon.tabular-1.1.1b20240424.tar` & `autogluon.tabular-1.1.1b20240425.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.579177 autogluon.tabular-1.1.1b20240424/
--rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-04-24 09:04:49.579177 autogluon.tabular-1.1.1b20240424/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 09:04:49.579177 autogluon.tabular-1.1.1b20240424/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.555178 autogluon.tabular-1.1.1b20240424/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.555178 autogluon.tabular-1.1.1b20240424/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.563178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.563178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21132 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/configs/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/configs/feature_generator_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    16315 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/configs/hyperparameter_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.563178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/configs/zeroshot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/configs/zeroshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/configs/zeroshot/zeroshot_portfolio_2023.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.563178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/experimental/_scikit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/experimental/_tabular_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/experimental/_tabular_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.563178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/learner/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51771 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/learner/abstract_learner.py
--rw-r--r--   0 runner    (1001) docker     (127)    22940 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/learner/default_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.563178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.563178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/_utils/rapids_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/_utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.567178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/automm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/automm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/automm/automm_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/automm/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.567178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/catboost/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/catboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/catboost/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16575 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/catboost/catboost_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/catboost/catboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.567178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/catboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.567178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fastainn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fastainn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fastainn/callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1379 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fastainn/fastai_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.567178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fastainn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fastainn/imports_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fastainn/quantile_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27704 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.567178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fasttext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fasttext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fasttext/fasttext_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.567178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fasttext/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.567178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/image_prediction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/image_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/image_prediction/image_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.567178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/imodels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/imodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/imodels/imodels_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.571178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/knn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/knn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/knn/_knn_loo_variants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/knn/knn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/knn/knn_rapids_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/knn/knn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.571178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lgb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lgb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lgb/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.571178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lgb/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    19709 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lgb/lgb_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lgb/lgb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.571178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.571178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lr/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    14076 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lr/lr_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lr/lr_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.571178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/rf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/rf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.571178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/rf/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/rf/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/rf/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/rf/compilers/onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/rf/rf_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    36460 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/rf/rf_quantile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/rf/rf_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.575178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.575178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    22903 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/pretexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24707 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    22651 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.575178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabpfn/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabpfn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabpfn/tabpfn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.575178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.575178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.575178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.575178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.575178 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34250 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.579177 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/text_prediction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/text_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.579177 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/vowpalwabbit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/vowpalwabbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.579177 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/xgboost/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/xgboost/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.579177 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/xgboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/xgboost/xgboost_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/xgboost/xgboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.579177 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/xt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/xt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/xt/xt_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.579177 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/predictor/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/predictor/_deprecated_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/predictor/interpretable_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)   313438 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/predictor/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.579177 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.579177 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/trainer/model_presets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/trainer/model_presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17843 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/trainer/model_presets/presets.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/trainer/model_presets/presets_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/trainer/model_presets/presets_distill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.579177 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/tuning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-04-24 09:03:44.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/tuning/feature_pruner.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-24 09:04:49.000000 autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:04:49.563178 autogluon.tabular-1.1.1b20240424/src/autogluon.tabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-04-24 09:04:49.000000 autogluon.tabular-1.1.1b20240424/src/autogluon.tabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-04-24 09:04:49.000000 autogluon.tabular-1.1.1b20240424/src/autogluon.tabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:04:49.000000 autogluon.tabular-1.1.1b20240424/src/autogluon.tabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 09:04:49.000000 autogluon.tabular-1.1.1b20240424/src/autogluon.tabular.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-24 09:04:49.000000 autogluon.tabular-1.1.1b20240424/src/autogluon.tabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 09:04:49.000000 autogluon.tabular-1.1.1b20240424/src/autogluon.tabular.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:04:49.000000 autogluon.tabular-1.1.1b20240424/src/autogluon.tabular.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.753539 autogluon.tabular-1.1.1b20240425/
+-rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-04-25 09:04:59.753539 autogluon.tabular-1.1.1b20240425/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 09:04:59.753539 autogluon.tabular-1.1.1b20240425/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.729539 autogluon.tabular-1.1.1b20240425/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.729539 autogluon.tabular-1.1.1b20240425/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.733539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.733539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21132 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/configs/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/configs/feature_generator_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16315 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/configs/hyperparameter_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.733539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/configs/zeroshot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/configs/zeroshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/configs/zeroshot/zeroshot_portfolio_2023.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.737539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/experimental/_scikit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/experimental/_tabular_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/experimental/_tabular_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.737539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/learner/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51900 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/learner/abstract_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22940 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/learner/default_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.737539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.737539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/_utils/rapids_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/_utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.737539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/automm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/automm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/automm/automm_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/automm/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.737539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/catboost/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/catboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/catboost/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16575 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/catboost/catboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/catboost/catboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.737539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/catboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.737539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fastainn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fastainn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fastainn/callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1379 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fastainn/fastai_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.741539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fastainn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fastainn/imports_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fastainn/quantile_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27704 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.741539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fasttext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fasttext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fasttext/fasttext_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.741539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fasttext/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.741539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/image_prediction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/image_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/image_prediction/image_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.741539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/imodels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/imodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/imodels/imodels_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.741539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/knn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/knn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/knn/_knn_loo_variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/knn/knn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/knn/knn_rapids_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/knn/knn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.741539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lgb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lgb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lgb/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.741539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lgb/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19709 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lgb/lgb_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lgb/lgb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.741539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.741539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lr/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14076 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lr/lr_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lr/lr_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.745539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/rf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/rf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.745539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/rf/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/rf/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/rf/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/rf/compilers/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/rf/rf_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36460 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/rf/rf_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/rf/rf_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.745539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.745539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22903 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/pretexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24707 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22651 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.745539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabpfn/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabpfn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabpfn/tabpfn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.745539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.745539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.745539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.749539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.749539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34250 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.749539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/text_prediction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/text_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.749539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/vowpalwabbit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/vowpalwabbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.749539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/xgboost/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.749539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/xgboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/xgboost/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/xgboost/xgboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.749539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/xt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/xt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/xt/xt_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.749539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/predictor/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/predictor/_deprecated_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/predictor/interpretable_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)   314138 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/predictor/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.749539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.753539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/trainer/model_presets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/trainer/model_presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17843 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/trainer/model_presets/presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/trainer/model_presets/presets_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/trainer/model_presets/presets_distill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.753539 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-04-25 09:03:58.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/tuning/feature_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-25 09:04:59.000000 autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:04:59.733539 autogluon.tabular-1.1.1b20240425/src/autogluon.tabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-04-25 09:04:59.000000 autogluon.tabular-1.1.1b20240425/src/autogluon.tabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-04-25 09:04:59.000000 autogluon.tabular-1.1.1b20240425/src/autogluon.tabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:04:59.000000 autogluon.tabular-1.1.1b20240425/src/autogluon.tabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 09:04:59.000000 autogluon.tabular-1.1.1b20240425/src/autogluon.tabular.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-25 09:04:59.000000 autogluon.tabular-1.1.1b20240425/src/autogluon.tabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 09:04:59.000000 autogluon.tabular-1.1.1b20240425/src/autogluon.tabular.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:04:59.000000 autogluon.tabular-1.1.1b20240425/src/autogluon.tabular.egg-info/zip-safe
```

### Comparing `autogluon.tabular-1.1.1b20240424/PKG-INFO` & `autogluon.tabular-1.1.1b20240425/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 1.1.1b20240424
+Version: 1.1.1b20240425
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-1.1.1b20240424/setup.py` & `autogluon.tabular-1.1.1b20240425/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/configs/config_helper.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/configs/config_helper.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/configs/feature_generator_presets.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/configs/feature_generator_presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/configs/hyperparameter_configs.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/configs/hyperparameter_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/configs/presets_configs.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/configs/zeroshot/zeroshot_portfolio_2023.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/configs/zeroshot/zeroshot_portfolio_2023.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/experimental/_scikit_mixin.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/experimental/_scikit_mixin.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/experimental/_tabular_classifier.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/experimental/_tabular_classifier.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/experimental/_tabular_regressor.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/experimental/_tabular_regressor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/learner/abstract_learner.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/learner/abstract_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1038,15 +1038,16 @@
         return y_transformed
 
     def calibrate_decision_threshold(
         self,
         data: pd.DataFrame | None = None,
         metric: str | Scorer | None = None,
         model: str = "best",
-        decision_thresholds: int | List[float] = 50,
+        decision_thresholds: int | List[float] = 25,
+        secondary_decision_thresholds: int | None = 19,
         verbose: bool = True,
         **kwargs,
     ) -> float:
         # TODO: docstring
         if metric is None:
             metric = self.eval_metric
 
@@ -1063,14 +1064,15 @@
         return self.load_trainer().calibrate_decision_threshold(
             X=X,
             y=y,
             metric=metric,
             model=model,
             weights=weights,
             decision_thresholds=decision_thresholds,
+            secondary_decision_thresholds=secondary_decision_thresholds,
             verbose=verbose,
             **kwargs,
         )
 
     # TODO: Add data info gathering at beginning of .fit() that is used by all learners to add to get_info output
     # TODO: Add feature inference / feature engineering info to get_info output
     def get_info(self, **kwargs):
```

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/learner/default_learner.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/learner/default_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/__init__.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/_utils/rapids_utils.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/_utils/rapids_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/_utils/torch_utils.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/automm/automm_model.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/automm/automm_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/automm/ft_transformer.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/automm/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/catboost/callbacks.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/catboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/catboost/catboost_model.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/catboost/catboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/catboost/catboost_utils.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/catboost/catboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fastainn/callbacks.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fastainn/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fastainn/fastai_helpers.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fastainn/fastai_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fastainn/quantile_helpers.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fastainn/quantile_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fasttext/fasttext_model.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fasttext/fasttext_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/image_prediction/image_predictor.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/image_prediction/image_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/imodels/imodels_models.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/imodels/imodels_models.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/knn/_knn_loo_variants.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/knn/_knn_loo_variants.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/knn/knn_model.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/knn/knn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/knn/knn_rapids_model.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/knn/knn_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/knn/knn_utils.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/knn/knn_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lgb/callbacks.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lgb/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lgb/lgb_model.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lgb/lgb_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lgb/lgb_utils.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lgb/lgb_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lr/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lr/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lr/lr_model.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lr/lr_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/lr/lr_rapids_model.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/lr/lr_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/rf/compilers/native.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/rf/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/rf/compilers/onnx.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/rf/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/rf/rf_model.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/rf/rf_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/rf/rf_quantile.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/rf/rf_quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/rf/rf_rapids_model.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/rf/rf_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/modified_transformer.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/modified_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/pretexts.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/pretexts.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/tab_model_base.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/tab_model_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/tab_transformer.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tab_transformer/utils.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tab_transformer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabpfn/tabpfn_model.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabpfn/tabpfn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/compilers/native.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/xgboost/callbacks.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/xgboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/xgboost/xgboost_model.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/xgboost/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/xgboost/xgboost_utils.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/xgboost/xgboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/models/xt/xt_model.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/models/xt/xt_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/predictor/_deprecated_methods.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/predictor/_deprecated_methods.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/predictor/interpretable_predictor.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/predictor/interpretable_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/predictor/predictor.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/predictor/predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -3366,15 +3366,16 @@
         return models
 
     def calibrate_decision_threshold(
         self,
         data: str | TabularDataset | pd.DataFrame | None = None,
         metric: str | Scorer | None = None,
         model: str = "best",
-        decision_thresholds: int | List[float] = 50,
+        decision_thresholds: int | List[float] = 25,
+        secondary_decision_thresholds: int | None = 19,
         subsample_size: int | None = 1000000,
         verbose: bool = True,
     ) -> float:
         """
         Calibrate the decision threshold in binary classification to optimize a given metric.
         You can pass the output of this method as input to `predictor.set_decision_threshold` to update the predictor.
         Will raise an AssertionError if `predictor.problem_type != 'binary'`.
@@ -3392,18 +3393,24 @@
             If None, will use internal data such as the holdout validation data or out-of-fold predictions.
         metric : autogluon.core.metrics.Scorer or str, default = None
             The metric to optimize during calibration.
             If None, uses `predictor.eval_metric`.
         model : str, default = 'best'
             The model to use prediction probabilities of when calibrating the threshold.
             If 'best', will use `predictor.model_best`.
-        decision_thresholds : Union[int, List[float]], default = 50
+        decision_thresholds : int | List[float], default = 25
             The number of decision thresholds on either side of `0.5` to search.
-            The default of 50 will result in 101 searched thresholds: [0.00, 0.01, 0.02, ..., 0.49, 0.50, 0.51, ..., 0.98, 0.99, 1.00]
+            The default of 25 will result in 51 searched thresholds: [0.00, 0.02, 0.04, ..., 0.48, 0.50, 0.52, ..., 0.96, 0.98, 1.00]
             Alternatively, a list of decision thresholds can be passed and only the thresholds in the list will be searched.
+        secondary_decision_thresholds : int | None, default = 19
+            The number of secondary decision thresholds to check on either side of the threshold identified in the first phase.
+            Skipped if None.
+            For example, if decision_thresholds=50 and 0.14 was identified as the optimal threshold, while secondary_decision_threshold=9,
+                Then the following additional thresholds are checked:
+                    [0.131, 0.132, 0.133, 0.134, 0.135, 0.136, 0.137, 0.138, 0.139, 0.141, 0.142, 0.143, 0.144, 0.145, 0.146, 0.147, 0.148, 0.149]
         subsample_size : int | None, default = 1000000
             When `subsample_size` is not None and `data` contains more rows than `subsample_size`, samples to `subsample_size` rows to speed up calibration.
             Usually it is not necessary to use more than 1 million rows for calibration.
         verbose : bool, default = True
             If True, will log information about the calibration process.
 
         Returns
@@ -3433,14 +3440,15 @@
             model = self.model_best
 
         return self._learner.calibrate_decision_threshold(
             data=data,
             metric=metric,
             model=model,
             decision_thresholds=decision_thresholds,
+            secondary_decision_thresholds=secondary_decision_thresholds,
             subsample_size=subsample_size,
             verbose=verbose,
         )
 
     def predict_oof(self, model: str = None, *, transformed=False, train_data=None, internal_oof=False, decision_threshold=None, can_infer=None) -> pd.Series:
         """
         Note: This is advanced functionality not intended for normal usage.
```

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/trainer/auto_trainer.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/trainer/model_presets/presets.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/trainer/model_presets/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/trainer/model_presets/presets_custom.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/trainer/model_presets/presets_custom.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/trainer/model_presets/presets_distill.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/trainer/model_presets/presets_distill.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon/tabular/tuning/feature_pruner.py` & `autogluon.tabular-1.1.1b20240425/src/autogluon/tabular/tuning/feature_pruner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon.tabular.egg-info/PKG-INFO` & `autogluon.tabular-1.1.1b20240425/src/autogluon.tabular.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 1.1.1b20240424
+Version: 1.1.1b20240425
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon.tabular.egg-info/SOURCES.txt` & `autogluon.tabular-1.1.1b20240425/src/autogluon.tabular.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240424/src/autogluon.tabular.egg-info/requires.txt` & `autogluon.tabular-1.1.1b20240425/src/autogluon.tabular.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 numpy<1.29,>=1.21
 scipy<1.13,>=1.5.4
 pandas<2.3.0,>=2.0.0
 scikit-learn<1.4.1,>=1.3.0
 networkx<4,>=3.0
-autogluon.core==1.1.1b20240424
-autogluon.features==1.1.1b20240424
+autogluon.core==1.1.1b20240425
+autogluon.features==1.1.1b20240425
 
 [all]
-autogluon.core[all]==1.1.1b20240424
-torch<2.2,>=2.1
-fastai<2.8,>=2.3.1
 xgboost<2.1,>=1.6
 lightgbm<4.4,>=3.3
+fastai<2.8,>=2.3.1
+torch<2.2,>=2.1
+autogluon.core[all]==1.1.1b20240425
 
 [all:sys_platform != "darwin"]
 catboost<1.3,>=1.1
 
 [all:sys_platform == "darwin" and python_version < "3.11"]
 catboost<1.2,>=1.1
 
@@ -34,15 +34,15 @@
 [imodels]
 imodels<1.4.0,>=1.3.10
 
 [lightgbm]
 lightgbm<4.4,>=3.3
 
 [ray]
-autogluon.core[all]==1.1.1b20240424
+autogluon.core[all]==1.1.1b20240425
 
 [skex]
 scikit-learn-intelex<2024.3,>=2023.0
 
 [skl2onnx]
 skl2onnx<1.17.0,>=1.15.0
 onnxruntime-gpu<1.18.0,>=1.15.0
```

