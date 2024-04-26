# Comparing `tmp/fairret-0.1.2.tar.gz` & `tmp/fairret-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairret-0.1.2.tar", last modified: Wed Apr 24 14:48:24 2024, max compression
+gzip compressed data, was "fairret-0.1.3.tar", last modified: Fri Apr 26 16:31:42 2024, max compression
```

## Comparing `fairret-0.1.2.tar` & `fairret-0.1.3.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.010423 fairret-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:23.998423 fairret-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.002423 fairret-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-24 14:48:19.000000 fairret-0.1.2/.github/workflows/pypi_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-24 14:48:19.000000 fairret-0.1.2/.github/workflows/sphinx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-24 14:48:19.000000 fairret-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-24 14:48:19.000000 fairret-0.1.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-24 14:48:19.000000 fairret-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-24 14:48:24.010423 fairret-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-24 14:48:19.000000 fairret-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.002423 fairret-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.002423 fairret-0.1.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.006423 fairret-0.1.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    39520 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/source/_static/Overview_fairret.png
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.006423 fairret-0.1.2/docs/source/generated/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/source/generated/fairret.loss.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/source/loss.rst
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/source/metric.rst
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/source/statistic.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.006423 fairret-0.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    88620 2024-04-24 14:48:19.000000 fairret-0.1.2/examples/complex_sensitive_features.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    17921 2024-04-24 14:48:19.000000 fairret-0.1.2/examples/custom_statistic.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    28213 2024-04-24 14:48:19.000000 fairret-0.1.2/examples/simple_pipeline.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16306 2024-04-24 14:48:19.000000 fairret-0.1.2/examples/stacked_statistic.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.006423 fairret-0.1.2/fairret/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.006423 fairret-0.1.2/fairret/loss/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/loss/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17955 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/loss/projection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/loss/violation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.010423 fairret-0.1.2/fairret/statistic/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/statistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/statistic/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26353 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/statistic/linear_fractional.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.010423 fairret-0.1.2/fairret.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-24 14:48:23.000000 fairret-0.1.2/fairret.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-24 14:48:23.000000 fairret-0.1.2/fairret.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:48:23.000000 fairret-0.1.2/fairret.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 14:48:23.000000 fairret-0.1.2/fairret.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 14:48:23.000000 fairret-0.1.2/fairret.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-24 14:48:19.000000 fairret-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:48:24.010423 fairret-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.010423 fairret-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-24 14:48:19.000000 fairret-0.1.2/test/test_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-24 14:48:19.000000 fairret-0.1.2/test/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-24 14:48:19.000000 fairret-0.1.2/test/test_statistic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:31:42.070747 fairret-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:31:42.062747 fairret-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:31:42.066747 fairret-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-26 16:31:37.000000 fairret-0.1.3/.github/workflows/pypi_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-26 16:31:37.000000 fairret-0.1.3/.github/workflows/sphinx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-26 16:31:37.000000 fairret-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-26 16:31:37.000000 fairret-0.1.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-26 16:31:37.000000 fairret-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-26 16:31:42.070747 fairret-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-26 16:31:37.000000 fairret-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:31:42.066747 fairret-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-26 16:31:37.000000 fairret-0.1.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-26 16:31:37.000000 fairret-0.1.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 16:31:37.000000 fairret-0.1.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:31:42.066747 fairret-0.1.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:31:42.066747 fairret-0.1.3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    39520 2024-04-26 16:31:37.000000 fairret-0.1.3/docs/source/_static/Overview_fairret.png
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-26 16:31:37.000000 fairret-0.1.3/docs/source/_static/fairret.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-26 16:31:37.000000 fairret-0.1.3/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:31:42.066747 fairret-0.1.3/docs/source/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-26 16:31:37.000000 fairret-0.1.3/docs/source/generated/fairret.loss.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-26 16:31:37.000000 fairret-0.1.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-26 16:31:37.000000 fairret-0.1.3/docs/source/loss.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-26 16:31:37.000000 fairret-0.1.3/docs/source/metric.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-26 16:31:37.000000 fairret-0.1.3/docs/source/statistic.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:31:42.066747 fairret-0.1.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    88620 2024-04-26 16:31:37.000000 fairret-0.1.3/examples/complex_sensitive_features.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    17921 2024-04-26 16:31:37.000000 fairret-0.1.3/examples/custom_statistic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    28236 2024-04-26 16:31:37.000000 fairret-0.1.3/examples/fairness_metrics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    28213 2024-04-26 16:31:37.000000 fairret-0.1.3/examples/simple_pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16306 2024-04-26 16:31:37.000000 fairret-0.1.3/examples/stacked_statistic.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:31:42.066747 fairret-0.1.3/fairret/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:31:37.000000 fairret-0.1.3/fairret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:31:42.070747 fairret-0.1.3/fairret/loss/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-26 16:31:37.000000 fairret-0.1.3/fairret/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-26 16:31:37.000000 fairret-0.1.3/fairret/loss/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18038 2024-04-26 16:31:37.000000 fairret-0.1.3/fairret/loss/projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-26 16:31:37.000000 fairret-0.1.3/fairret/loss/violation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-26 16:31:37.000000 fairret-0.1.3/fairret/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:31:42.070747 fairret-0.1.3/fairret/statistic/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-26 16:31:37.000000 fairret-0.1.3/fairret/statistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-26 16:31:37.000000 fairret-0.1.3/fairret/statistic/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26564 2024-04-26 16:31:37.000000 fairret-0.1.3/fairret/statistic/linear_fractional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-26 16:31:37.000000 fairret-0.1.3/fairret/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:31:42.070747 fairret-0.1.3/fairret.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-26 16:31:42.000000 fairret-0.1.3/fairret.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-26 16:31:42.000000 fairret-0.1.3/fairret.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:31:42.000000 fairret-0.1.3/fairret.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 16:31:42.000000 fairret-0.1.3/fairret.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 16:31:42.000000 fairret-0.1.3/fairret.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-26 16:31:37.000000 fairret-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:31:42.070747 fairret-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:31:42.070747 fairret-0.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-26 16:31:37.000000 fairret-0.1.3/test/test_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-26 16:31:37.000000 fairret-0.1.3/test/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-26 16:31:37.000000 fairret-0.1.3/test/test_statistic.py
```

### Comparing `fairret-0.1.2/.github/workflows/pypi_release.yml` & `fairret-0.1.3/.github/workflows/pypi_release.yml`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: "3.x"
+        cache: pip
     - name: Install pypa/build
       run: >-
         python3 -m
         pip install
         build
         --user
     - name: Build a binary wheel and a source tarball
```

### Comparing `fairret-0.1.2/.github/workflows/sphinx.yml` & `fairret-0.1.3/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `fairret-0.1.2/.gitignore` & `fairret-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `fairret-0.1.2/CITATION.cff` & `fairret-0.1.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `fairret-0.1.2/LICENSE` & `fairret-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fairret-0.1.2/PKG-INFO` & `fairret-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairret
-Version: 0.1.2
+Version: 0.1.3
 Summary: A fairness library in PyTorch.
 Author-email: Maarten Buyl <maarten.buyl@ugent.be>, MaryBeth Defrance <marybeth.defrance@ugent.be>
 License: MIT License
         
         Copyright (c) 2024 Ghent University Artificial Intelligence & Data Analytics Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,39 +34,32 @@
 
 # fairret - a fairness library in PyTorch
 
 [![Licence](https://img.shields.io/github/license/aida-ugent/fairret)](https://github.com/aida-ugent/fairret/blob/main/LICENSE)
 [![PyPI - Version](https://img.shields.io/pypi/v/fairret)](https://pypi.org/project/fairret/)
 ![Static Badge](https://img.shields.io/badge/PyTorch-ee4c2c)
 [![Static Badge](https://img.shields.io/badge/Original%20Paper-00a0ff)](https://openreview.net/pdf?id=NnyD0Rjx2B)
+<img src="./docs/source/_static/fairret.png" height="300" align="right">
 
-## Description
+The goal of fairret is to serve as an open-source library for measuring and mitigating statistical fairness in PyTorch models. 
 
-The goal of fairret is to serve as an open-source Python library for measuring and mitigating statistical fairness in PyTorch models. The library is designed to be 
+The library is designed to be 
 1. *flexible* in how fairness is defined and pursued.
 2. *easy* to integrate into existing PyTorch pipelines.
 3. *clear* in what its tools can and cannot do.
 
-The central to the library is the paradigm of the _fairness regularization term_ (fairrets) that quantify unfairness as differentiable PyTorch loss functions. 
-These can then be optimized together with e.g. the binary cross-entropy error such that the classifier improves both its accuracy and fairness.
+Central to the library is the paradigm of the _fairness regularization term_ (fairrets) that quantify unfairness as differentiable PyTorch loss functions. 
 
-## Installation
-The fairret library can be installed via PyPi:
-
-```
-pip install fairret
-```
-
-A minimal list of dependencies is provided in [pyproject.toml](https://github.com/aida-ugent/fairret/blob/main/pyproject.toml). 
-
-If the library is installed locally, the required packages can be installed via `pip install .`
+These can be minimized jointly with other losses, like the binary cross-entropy error, by just adding them together!
 
 ## Quickstart
 
-It suffices to simply choose a statistic that should be equalized across groups and a fairret that quantifies the gap. The model can then be trained as follows:
+It suffices to simply choose a _statistic_ that should be equalized across groups and a _fairret_ that quantifies the gap. 
+
+The model can then be trained as follows:
 
 ```python
 import torch.nn.functional as F
 from fairret.statistic import PositiveRate
 from fairret.loss import NormLoss
 
 statistic = PositiveRate()
@@ -81,18 +74,31 @@
             fairret_loss = norm_fairret(logit, sens)
             loss = bce_loss + fairret_loss
             loss.backward()
             
             optimizer.step()
 ```
 
-No special data structure is required for the sensitive features. If the training batch contains N elements, then `sens` should be a tensor of floats with shape (N, d_s), with d_s the number of sensitive features. **Like any categorical feature, it is expected that categorical sensitive features are one-hot encoded.**
+No special data structure is required for the sensitive features. If the training batch contains $N$ elements, then `sens` should be a tensor of floats with shape $(N, d_s)$, with $d_s$ the number of sensitive features. **Like any categorical feature, it is expected that categorical sensitive features are one-hot encoded.**
 
 A notebook with a full example pipeline is provided here: [simple_pipeline.ipynb](/examples/simple_pipeline.ipynb).
 
+We also host [documentation](https://aida-ugent.github.io/fairret/).
+
+## Installation
+The fairret library can be installed via PyPi:
+
+```
+pip install fairret
+```
+
+A minimal list of dependencies is provided in [pyproject.toml](https://github.com/aida-ugent/fairret/blob/main/pyproject.toml). 
+
+If the library is installed locally, the required packages can be installed via `pip install .`
+
 ## Warning: AI fairness != fairness
 There are many ways in which technical approaches to AI fairness, such as this library, are simplistic and limited in actually achieving fairness in real-world decision processes.
 
 More information on these limitations can be found [here](https://dl.acm.org/doi/full/10.1145/3624700) or [here](https://ojs.aaai.org/index.php/AAAI/article/view/26798).
 
 ## Future plans
 The library maintains a core focus on only fairrets for now, yet we plan to add more fairness tools that align with the design principles in the future. These may involve breaking changes. At the same time, we'll keep reviewing the role of this library within the wider ecosystem of fairness toolkits.
```

### Comparing `fairret-0.1.2/README.md` & `fairret-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 # fairret - a fairness library in PyTorch
 
 [![Licence](https://img.shields.io/github/license/aida-ugent/fairret)](https://github.com/aida-ugent/fairret/blob/main/LICENSE)
 [![PyPI - Version](https://img.shields.io/pypi/v/fairret)](https://pypi.org/project/fairret/)
 ![Static Badge](https://img.shields.io/badge/PyTorch-ee4c2c)
 [![Static Badge](https://img.shields.io/badge/Original%20Paper-00a0ff)](https://openreview.net/pdf?id=NnyD0Rjx2B)
+<img src="./docs/source/_static/fairret.png" height="300" align="right">
 
-## Description
+The goal of fairret is to serve as an open-source library for measuring and mitigating statistical fairness in PyTorch models. 
 
-The goal of fairret is to serve as an open-source Python library for measuring and mitigating statistical fairness in PyTorch models. The library is designed to be 
+The library is designed to be 
 1. *flexible* in how fairness is defined and pursued.
 2. *easy* to integrate into existing PyTorch pipelines.
 3. *clear* in what its tools can and cannot do.
 
-The central to the library is the paradigm of the _fairness regularization term_ (fairrets) that quantify unfairness as differentiable PyTorch loss functions. 
-These can then be optimized together with e.g. the binary cross-entropy error such that the classifier improves both its accuracy and fairness.
+Central to the library is the paradigm of the _fairness regularization term_ (fairrets) that quantify unfairness as differentiable PyTorch loss functions. 
 
-## Installation
-The fairret library can be installed via PyPi:
-
-```
-pip install fairret
-```
-
-A minimal list of dependencies is provided in [pyproject.toml](https://github.com/aida-ugent/fairret/blob/main/pyproject.toml). 
-
-If the library is installed locally, the required packages can be installed via `pip install .`
+These can be minimized jointly with other losses, like the binary cross-entropy error, by just adding them together!
 
 ## Quickstart
 
-It suffices to simply choose a statistic that should be equalized across groups and a fairret that quantifies the gap. The model can then be trained as follows:
+It suffices to simply choose a _statistic_ that should be equalized across groups and a _fairret_ that quantifies the gap. 
+
+The model can then be trained as follows:
 
 ```python
 import torch.nn.functional as F
 from fairret.statistic import PositiveRate
 from fairret.loss import NormLoss
 
 statistic = PositiveRate()
@@ -47,18 +40,31 @@
             fairret_loss = norm_fairret(logit, sens)
             loss = bce_loss + fairret_loss
             loss.backward()
             
             optimizer.step()
 ```
 
-No special data structure is required for the sensitive features. If the training batch contains N elements, then `sens` should be a tensor of floats with shape (N, d_s), with d_s the number of sensitive features. **Like any categorical feature, it is expected that categorical sensitive features are one-hot encoded.**
+No special data structure is required for the sensitive features. If the training batch contains $N$ elements, then `sens` should be a tensor of floats with shape $(N, d_s)$, with $d_s$ the number of sensitive features. **Like any categorical feature, it is expected that categorical sensitive features are one-hot encoded.**
 
 A notebook with a full example pipeline is provided here: [simple_pipeline.ipynb](/examples/simple_pipeline.ipynb).
 
+We also host [documentation](https://aida-ugent.github.io/fairret/).
+
+## Installation
+The fairret library can be installed via PyPi:
+
+```
+pip install fairret
+```
+
+A minimal list of dependencies is provided in [pyproject.toml](https://github.com/aida-ugent/fairret/blob/main/pyproject.toml). 
+
+If the library is installed locally, the required packages can be installed via `pip install .`
+
 ## Warning: AI fairness != fairness
 There are many ways in which technical approaches to AI fairness, such as this library, are simplistic and limited in actually achieving fairness in real-world decision processes.
 
 More information on these limitations can be found [here](https://dl.acm.org/doi/full/10.1145/3624700) or [here](https://ojs.aaai.org/index.php/AAAI/article/view/26798).
 
 ## Future plans
 The library maintains a core focus on only fairrets for now, yet we plan to add more fairness tools that align with the design principles in the future. These may involve breaking changes. At the same time, we'll keep reviewing the role of this library within the wider ecosystem of fairness toolkits.
```

### Comparing `fairret-0.1.2/docs/Makefile` & `fairret-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fairret-0.1.2/docs/make.bat` & `fairret-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fairret-0.1.2/docs/source/_static/Overview_fairret.png` & `fairret-0.1.3/docs/source/_static/Overview_fairret.png`

 * *Files identical despite different names*

### Comparing `fairret-0.1.2/docs/source/conf.py` & `fairret-0.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fairret-0.1.2/docs/source/index.rst` & `fairret-0.1.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fairret-0.1.2/examples/complex_sensitive_features.ipynb` & `fairret-0.1.3/examples/complex_sensitive_features.ipynb`

 * *Files identical despite different names*

### Comparing `fairret-0.1.2/examples/custom_statistic.ipynb` & `fairret-0.1.3/examples/custom_statistic.ipynb`

 * *Files identical despite different names*

### Comparing `fairret-0.1.2/examples/simple_pipeline.ipynb` & `fairret-0.1.3/examples/simple_pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `fairret-0.1.2/examples/stacked_statistic.ipynb` & `fairret-0.1.3/examples/stacked_statistic.ipynb`

 * *Files identical despite different names*

### Comparing `fairret-0.1.2/fairret/loss/base.py` & `fairret-0.1.3/fairret/loss/base.py`

 * *Files identical despite different names*

### Comparing `fairret-0.1.2/fairret/loss/projection.py` & `fairret-0.1.3/fairret/loss/projection.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,21 +23,21 @@
     """
     Abstract base class for fairness losses that penalize the statistical distance between a set of predictions and
     the fair projection of those predictions. The fair projection satisfies the linear fairness constraint
     corresponding to a LinearFractionalStatistic that is fixed to a target value (such as the overall statistic).
 
     The projections are computed using cvxpy. Hence, any subclass is expected to implement the statistical distance
     between distributions in both cvxpy and PyTorch by implementing the
-    :func:`~projection.ProjectionLoss.cvxpy_distance` method and the
-    :func:`~projection.ProjectionLoss.torch_distance` method respectively.
+    :py:meth:`~fairret.loss.projection.ProjectionLoss.cvxpy_distance` method and the
+    :py:meth:`~fairret.loss.projection.ProjectionLoss.torch_distance` method respectively.
 
-    Optionally, the :func:`~projection.ProjectionLoss.torch_distance_with_logits` method can be overwritten to
-    provide a more numerically stable handling of predictions that are provided as logits. If left unimplemented,
-    :func:`~projection.ProjectionLoss.torch_distance` will be called instead, after applying the sigmoid function to
-    the predictions.
+    Optionally, the :py:meth:`~fairret.loss.projection.ProjectionLoss.torch_distance_with_logits` method can be
+    overwritten to provide a more numerically stable handling of predictions that are provided as logits. If left
+    unimplemented, :py:meth:`~fairret.loss.projection.ProjectionLoss.torch_distance` will be called instead,
+    after applying the sigmoid function to the predictions.
 
     Note:
         We use 'statistical distance' in a broad sense here, and do not require that the distance is a metric. See
         https://en.wikipedia.org/wiki/Statistical_distance for more information.
     """
 
     def __init__(self, statistic: LinearFractionalStatistic, force_proj_normalized=True, proj_eps=0.,
@@ -127,16 +127,16 @@
             torch.Tensor: The statistical distance as a scalar tensor.
         """
 
         raise NotImplementedError
 
     def torch_distance_with_logits(self, pred, proj):
         """
-        A more numerically stable alternative method to :func:`~projection.ProjectionLoss.torch_distance`, where `pred`
-        is assumed to be logits.
+        A more numerically stable alternative method to
+        :py:meth:`~fairret.loss.projection.ProjectionLoss.torch_distance`, where `pred` is assumed to be logits.
 
         Args:
             pred (torch.Tensor): The predicted distribution as logits, in shape (N,1). As we assume binary
                 classification, this is the logit of the probability of the positive class.
             proj (torch.Tensor): The projected distribution in shape (N,2) as probabilities. As we assume binary
                 classification, the first column is the probability of the negative class and the second column is the
                 probability of the positive class.
@@ -259,15 +259,15 @@
             self._problem = problem
 
         # If the received batch is smaller than we expected (e.g. because it is the last batch in an epoch), then pad
         # the batch with zeros to match the batch size of the first batch
         batch_size = pred.shape[0]
         if batch_size < self._batch_size:
             gap = self._batch_size - batch_size
-            pred = torch.cat([pred, torch.zeros(gap)])
+            pred = torch.cat([pred, torch.zeros(gap, 1)])
             slope = torch.cat([slope, torch.zeros((gap, slope.shape[1]))])
         elif batch_size > self._batch_size:
             raise ValueError(f"For {self.__class__.__name__} with reuse_definition=True, the batch size must never "
                              f"exceed the batch size of the first batch. Got {batch_size}, yet we initialized with "
                              f"{self._batch_size}!")
 
         # Expand the prediction to its Bernoulli distribution and fill in the parameters of the cvxpy problem.
```

### Comparing `fairret-0.1.2/fairret/loss/violation.py` & `fairret-0.1.3/fairret/loss/violation.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         """
         raise NotImplementedError
 
     def forward(self, pred: torch.Tensor, sens: torch.Tensor, *stat_args, pred_as_logit=True,
                 target_statistic: Optional[torch.Tensor] = None, **stat_kwargs: Any) -> torch.Tensor:
         """
         Calculate the violation vector in relation to the `target_statistic` and penalize this violation using the
-        :func:`~violation.ViolationLoss.penalize_violation` method implemented by the subclass.
+        :py:meth:`~fairret.loss.violation.ViolationLoss.penalize_violation` method implemented by the subclass.
 
         Args:
             pred (torch.Tensor): Predictions of shape :math:`(N, 1)`, as we assume to be performing binary
                 classification or regression.
             sens (torch.Tensor): Sensitive features of shape :math:`(N, S)` with `S` the number of sensitive features.
             *stat_args: All arguments used by the statistic that this loss minimizes.
             pred_as_logit (bool): Whether the `pred` tensor should be interpreted as logits. Though most losses are
```

### Comparing `fairret-0.1.2/fairret/metric.py` & `fairret-0.1.3/fairret/metric.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,29 +41,32 @@
     """
     return torch.amax(torch.abs(vals / target_val - 1), dim=-1)
 
 
 class LinearFractionalParity(torchmetrics.Metric):
     """
     Metric that assesses the fairness of a model's predictions by comparing the gaps between the provided
-    LinearFractionalStatistic for every sensitive feature.
+    :py:class:`~fairret.statistic.linear_fractional.LinearFractionalStatistic` for every sensitive feature.
 
     The metric maintains two pairs of running sums: one for the statistic for every sensitive feature, and one for the
     overall statistic. Each pair of running sums consists of the numerator and the denominator for those statistics.
-    Observations are added to these sums by calling the `update` method. The final fairness gap is computed by calling
-    the `compute` method, which also resets the internal state of the metric.
+    Observations are added to these sums by calling the :py:meth:`~fairret.metric.LinearFractionalParity.update` method.
+    The final fairness gap is computed by calling the :py:meth:`~fairret.metric.LinearFractionalParity.compute` method.
 
-    The class is implemented as a subclass of torchmetrics.Metric, so the `torchmetrics` package is required.
+    The class is implemented as a subclass of :py:class:`torchmetrics.Metric`, so the :py:mod:`torchmetrics` package is
+    required.
 
     Warning:
-        It is advised not to mix LinearFractionalParity metrics with different statistics in a single
-        torchmetrics.MetricCollection with `compute_groups=True`, as this can lead to hard-to-debug errors.
+        A separate :py:meth:`~torchmetrics.Metric.reset()` call is required to reset the internal state of the metric
+        between epochs.
+    Warning:
+        It is advised not to mix metrics of this class with different statistics in a single
+        :py:class:`torchmetrics.MetricCollection` with `compute_groups=True`, as this can lead to hard-to-debug errors.
     """
 
-    # TODO: warn about compute groups.
     is_differentiable = True
     higher_is_better = False
     full_state_update = False
 
     def __init__(self,
                  statistic: LinearFractionalStatistic,
                  stat_shape: Union[int, Tuple[int]],
@@ -116,15 +119,16 @@
         self.overall_denom += self.stat.denom(pred, None, *stat_args, **stat_kwargs)
 
     def compute(self) -> float:
         """
         Divide the running sums of the numerator and denominator of the groupwise and overall statistics and compute the
         final gaps between the groupwise and overall statistics, according to the `gap_fn`.
 
-        The internal state of the metric is reset after calling this method.
+        Warning:
+            This does NOT reset the internal state of the metric. A separate `.reset()` call is required to do so.
 
         Returns:
             float: The final fairness gap.
         """
 
         stats = safe_div(self.num, self.denom)
         overall_stat = safe_div(self.overall_num, self.overall_denom)
```

### Comparing `fairret-0.1.2/fairret/statistic/base.py` & `fairret-0.1.3/fairret/statistic/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class Statistic(abc.ABC, torch.nn.Module):
     """
     Abstract base class for a statistic.
 
     As a subclass of torch.nn.Module, it should implement the :func:`~base.Statistic.forward` method with the
-    :func:`~base.Statistic.forward(self, pred, sens, \*stat_args, \*\*stat_kwargs)' signature.
+    :func:`~base.Statistic.forward(self, pred, sens, \*stat_args, \*\*stat_kwargs)` signature.
     """
 
     @abc.abstractmethod
     def forward(self, pred: torch.Tensor, sens: torch.Tensor, *stat_args: Any, **stat_kwargs: Any) -> torch.Tensor:
         """
         Compute the statistic for a batch of `N` samples for each sensitive feature.
```

### Comparing `fairret-0.1.2/fairret/statistic/linear_fractional.py` & `fairret-0.1.3/fairret/statistic/linear_fractional.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 class LinearFractionalStatistic(Statistic):
     """
     Absract base class for a linear-fractional Statistic. This is a Statistic that is computed as the ratio between two
     linear functions over the predictions.
 
     A LinearFractionalStatistic is constructed in a canonical form by defining the intercept and slope of the
     numerator and denominator linear functions, i.e. the functions
-    :func:`~linear_fractional.LinearFractionalStatistic.num_intercept`,
-    :func:`~linear_fractional.LinearFractionalStatistic.num_slope`,
-    :func:`~linear_fractional.LinearFractionalStatistic.denom_intercept`,
-    and :func:`~linear_fractional.LinearFractionalStatistic.denom_slope`. Each subclass must implement these
-    functions (using any signature).
+    :py:meth:`~fairret.statistic.linear_fractional.LinearFractionalStatistic.num_intercept`,
+    :py:meth:`~fairret.statistic.linear_fractional.LinearFractionalStatistic.num_slope`,
+    :py:meth:`~fairret.statistic.linear_fractional.LinearFractionalStatistic.denom_intercept`,
+    and :py:meth:`~fairret.statistic.linear_fractional.LinearFractionalStatistic.denom_slope`. Each subclass must
+    implement these functions (using any signature).
 
     The statistic is then computed as :math:`\\frac{num\\_intercept + num\\_slope * pred}{denom\\_intercept +
     denom\\_slope * pred}`.
     """
 
     # The following methods violate the Liskov Substitution Principle (LSP) because they are implemented more generally
     # in this base class than is expected in the subclasses. However, it is kept for practical reasons. See 
@@ -112,16 +112,19 @@
             raise TypeError(f"All {abstract_methods} methods should share the same signature.\n"
                             f"The signatures are:\n{pprint.pformat(signatures)}")
         cls.expected_signature = expected_signature
 
     def __check_stat_args(self, *stat_args: Any, **stat_kwargs: Any) -> None:
         """
         Check whether the arguments and keyword arguments passed to the statistic are valid. This is done by checking
-        whether all arguments and keyword arguments together match the signature of  `num_intercept`, `num_slope`,
-        `denom_intercept`, and `denom_slope` methods.
+        whether all arguments and keyword arguments together match the signature of
+        :py:meth:`~fairret.statistic.linear_fractional.LinearFractionalStatistic.num_intercept`,
+        :py:meth:`~fairret.statistic.linear_fractional.LinearFractionalStatistic.num_slope`,
+        :py:meth:`~fairret.statistic.linear_fractional.LinearFractionalStatistic.denom_intercept`,
+        and :py:meth:`~fairret.statistic.linear_fractional.LinearFractionalStatistic.denom_slope` methods.
 
         Args:
             *stat_args: Any arguments.
             **stat_kwargs: Any keyword arguments.
         """
         try:
             self.expected_signature.bind(self, *stat_args, **stat_kwargs)
@@ -235,15 +238,15 @@
             torch.Tensor: The overall statistic as a scalar tensor.
         """
         return self.forward(pred, None, *stat_args, **stat_kwargs)
 
     def fixed_constraint(self, fix_value: torch.Tensor, sens: torch.Tensor, *stat_args: Any, **stat_kwargs: Any
                          ) -> Tuple[torch.Tensor, torch.Tensor]:
         """
-        Reformulate the fairness definition for this LinearFractionalStatistic as a linear constraint.
+        Reformulate the fairness definition for this linear-fractional statistic as a linear constraint.
 
         This is done by fixing the intended values of the statistic for every sensitive feature to a given value
         `fix_value`. The linear expressions that make up the numerator and denominator are then combined into a single
         linear constraint.
 
         Args:
             fix_value (torch.Tensor): The intended value of the statistic for every sensitive feature. Typically, this
@@ -281,15 +284,15 @@
         else:
             slope = torch.einsum('n...y,ns->n...s', slope, sens).flatten(start_dim=1)
         return intercept, slope
 
 
 class PositiveRate(LinearFractionalStatistic):
     """
-    PositiveRate is a LinearFractionalStatistic that computes the average rate at which positive predictions are made in
+    PositiveRate computes the average rate at which positive predictions are made in
     binary classification.
 
     Formulated as a probability, it computes :math:`P(\\hat{Y} = 1 | S)` for categorical sensitive features :math:`S`,
     with the predicted label :math:`\\hat{Y}` sampled according to the model's (probabilistic) prediction.
 
     The functions of its canonical form take no arguments.
     """
@@ -317,15 +320,15 @@
         :math:`= 0`
         """
         return 0.
 
 
 class TruePositiveRate(LinearFractionalStatistic):
     """
-    TruePositiveRate is a LinearFractionalStatistic that computes the average rate at which positives are actually
+    TruePositiveRate computes the average rate at which positives are actually
     predicted as positives, also known as the recall.
 
     Formulated as a probability, it computes :math:`P(\\hat{Y} = 1 | Y = 1, S)` for categorical sensitive features
     :math:`S` and only for samples where the target label :math:`Y` is positive, with the predicted label
     :math:`\\hat{Y}` sampled according to the model's (probabilistic) prediction.
 
     The functions of its canonical form require that the tensor of target labels is provided with the same shape as the
@@ -355,15 +358,15 @@
         :math:`= 0`
         """
         return 0.
 
 
 class FalsePositiveRate(LinearFractionalStatistic):
     """
-    FalsePositiveRate is a LinearFractionalStatistic that computes the average rate at which negatives are actually
+    FalsePositiveRate computes the average rate at which negatives are actually
     predicted as positives.
 
     Formulated as a probability, it computes :math:`P(\\hat{Y} = 1 | Y = 0, S)` for categorical sensitive features
     :math:`S` and only for samples where the target label :math:`Y` is negative, with the predicted label
     :math:`\\hat{Y}` sampled according to the model's (probabilistic) prediction.
 
     The functions of its canonical form require that the tensor of target labels is provided with the same shape as the
@@ -393,15 +396,15 @@
         :math:`= 0`
         """
         return 0.
 
 
 class PositivePredictiveValue(LinearFractionalStatistic):
     """
-    PositivePredictiveValue is a LinearFractionalStatistic that computes the average rate at which the predicted
+    PositivePredictiveValue computes the average rate at which the predicted
     positives were actually labeled positive, also known as the precision.
 
     Formulated as a probability, it computes :math:`P(Y = 1 | \\hat{Y} = 1, S)` for categorical sensitive features
     :math:`S` and only for samples where the predicted label (sampled according to the model's (probabilistic)
     prediction) is positive, with :math:`Y` the target label.
 
     The functions of its canonical form require that the tensor of target labels is provided with the same shape as the
@@ -431,15 +434,15 @@
         :math:`= 1`
         """
         return 1.
 
 
 class FalseOmissionRate(LinearFractionalStatistic):
     """
-    FalseOmissionRate is a LinearFractionalStatistic that computes the average rate at which the predicted
+    FalseOmissionRate computes the average rate at which the predicted
     negatives were actually labeled positive, also known as the precision.
 
     Formulated as a probability, it computes :math:`P(Y = 1 | \\hat{Y} = 0, S)` for categorical sensitive features
     :math:`S` and only for samples where the predicted label (sampled according to the model's (probabilistic)
     prediction) is negative, with :math:`Y` the target label.
 
     The functions of its canonical form require that the tensor of target labels is provided with the same shape as the
@@ -469,15 +472,15 @@
         :math:`= -1`
         """
         return -1.
 
 
 class Accuracy(LinearFractionalStatistic):
     """
-    Accuracy is a LinearFractionalStatistic that computes the average rate at which predictions match the actual target
+    Accuracy computes the average rate at which predictions match the actual target
     labels.
 
     Formulated as a probability, it computes :math:`P(\\hat{Y} = Y | S)` for categorical sensitive features :math:`S`,
     with the predicted label :math:`\\hat{Y}` sampled according to the model's (probabilistic) prediction and with
     :math:`Y` the target label.
 
     The functions of its canonical form require that the tensor of target labels is provided with the same shape as the
@@ -507,15 +510,15 @@
         :math:`= 0`
         """
         return 0.
 
 
 class FalseNegativeFalsePositiveFraction(LinearFractionalStatistic):
     """
-    FalseNegativeFalsePositiveFraction is a LinearFractionalStatistic that computes the ratio between false negatives
+    FalseNegativeFalsePositiveFraction computes the ratio between false negatives
     and false positives.
 
     The statistic cannot be formulated as a single probability.
 
     The functions of its canonical form require that the tensor of target labels is provided with the same shape as the
     predictions.
     """
@@ -543,16 +546,16 @@
         :math:`= 1 - Y`
         """
         return 1 - label
 
 
 class FScore(LinearFractionalStatistic):
     """
-    FScore is a LinearFractionalStatistic that computes the :math:`F_β`-score, the weighted mean of precision and
-    recall. The :math:`F_1`-score is the harmonic mean of precision and recall.
+    FScore computes the :math:`F_β`-score, the weighted mean of precision and recall. The :math:`F_1`-score is the
+    harmonic mean of precision and recall.
 
     The statistic cannot be formulated as a single probability.
 
     The functions of its canonical form require that the tensor of target labels is provided with the same shape as the
     predictions.
     """
 
@@ -587,22 +590,24 @@
         :math:`= 1`
         """
         return 1.
 
 
 class StackedLinearFractionalStatistic(LinearFractionalStatistic):
     """
-    A vector-valued LinearFractionalStatistic that combines the outputs of K LinearFractionalStatistics into a single
-    statistic with output (K, S) by stacking all outputs in the second-to-last dimension (`dim=-2`).
+    A vector-valued statistic that combines the outputs of K
+    :py:class:`~fairret.statistic.linear_fractional.LinearFractionalStatistic` 's into a single statistic with output
+    (K, S) by stacking all outputs in the second-to-last dimension (`dim=-2`).
     """
 
     def __init__(self, *statistics: LinearFractionalStatistic):
         """
         Args:
-            *statistics: The LinearFractionalStatistics to be stacked.
+            *statistics: The :py:class:`~fairret.statistic.linear_fractional.LinearFractionalStatistic` 's to be
+            stacked.
         """
 
         super().__init__()
 
         if len(statistics) == 0:
             raise ValueError("At least one statistic should be provided.")
         if any(not isinstance(stat, LinearFractionalStatistic) for stat in statistics):
```

### Comparing `fairret-0.1.2/fairret/utils.py` & `fairret-0.1.3/fairret/utils.py`

 * *Files identical despite different names*

### Comparing `fairret-0.1.2/fairret.egg-info/PKG-INFO` & `fairret-0.1.3/fairret.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairret
-Version: 0.1.2
+Version: 0.1.3
 Summary: A fairness library in PyTorch.
 Author-email: Maarten Buyl <maarten.buyl@ugent.be>, MaryBeth Defrance <marybeth.defrance@ugent.be>
 License: MIT License
         
         Copyright (c) 2024 Ghent University Artificial Intelligence & Data Analytics Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,39 +34,32 @@
 
 # fairret - a fairness library in PyTorch
 
 [![Licence](https://img.shields.io/github/license/aida-ugent/fairret)](https://github.com/aida-ugent/fairret/blob/main/LICENSE)
 [![PyPI - Version](https://img.shields.io/pypi/v/fairret)](https://pypi.org/project/fairret/)
 ![Static Badge](https://img.shields.io/badge/PyTorch-ee4c2c)
 [![Static Badge](https://img.shields.io/badge/Original%20Paper-00a0ff)](https://openreview.net/pdf?id=NnyD0Rjx2B)
+<img src="./docs/source/_static/fairret.png" height="300" align="right">
 
-## Description
+The goal of fairret is to serve as an open-source library for measuring and mitigating statistical fairness in PyTorch models. 
 
-The goal of fairret is to serve as an open-source Python library for measuring and mitigating statistical fairness in PyTorch models. The library is designed to be 
+The library is designed to be 
 1. *flexible* in how fairness is defined and pursued.
 2. *easy* to integrate into existing PyTorch pipelines.
 3. *clear* in what its tools can and cannot do.
 
-The central to the library is the paradigm of the _fairness regularization term_ (fairrets) that quantify unfairness as differentiable PyTorch loss functions. 
-These can then be optimized together with e.g. the binary cross-entropy error such that the classifier improves both its accuracy and fairness.
+Central to the library is the paradigm of the _fairness regularization term_ (fairrets) that quantify unfairness as differentiable PyTorch loss functions. 
 
-## Installation
-The fairret library can be installed via PyPi:
-
-```
-pip install fairret
-```
-
-A minimal list of dependencies is provided in [pyproject.toml](https://github.com/aida-ugent/fairret/blob/main/pyproject.toml). 
-
-If the library is installed locally, the required packages can be installed via `pip install .`
+These can be minimized jointly with other losses, like the binary cross-entropy error, by just adding them together!
 
 ## Quickstart
 
-It suffices to simply choose a statistic that should be equalized across groups and a fairret that quantifies the gap. The model can then be trained as follows:
+It suffices to simply choose a _statistic_ that should be equalized across groups and a _fairret_ that quantifies the gap. 
+
+The model can then be trained as follows:
 
 ```python
 import torch.nn.functional as F
 from fairret.statistic import PositiveRate
 from fairret.loss import NormLoss
 
 statistic = PositiveRate()
@@ -81,18 +74,31 @@
             fairret_loss = norm_fairret(logit, sens)
             loss = bce_loss + fairret_loss
             loss.backward()
             
             optimizer.step()
 ```
 
-No special data structure is required for the sensitive features. If the training batch contains N elements, then `sens` should be a tensor of floats with shape (N, d_s), with d_s the number of sensitive features. **Like any categorical feature, it is expected that categorical sensitive features are one-hot encoded.**
+No special data structure is required for the sensitive features. If the training batch contains $N$ elements, then `sens` should be a tensor of floats with shape $(N, d_s)$, with $d_s$ the number of sensitive features. **Like any categorical feature, it is expected that categorical sensitive features are one-hot encoded.**
 
 A notebook with a full example pipeline is provided here: [simple_pipeline.ipynb](/examples/simple_pipeline.ipynb).
 
+We also host [documentation](https://aida-ugent.github.io/fairret/).
+
+## Installation
+The fairret library can be installed via PyPi:
+
+```
+pip install fairret
+```
+
+A minimal list of dependencies is provided in [pyproject.toml](https://github.com/aida-ugent/fairret/blob/main/pyproject.toml). 
+
+If the library is installed locally, the required packages can be installed via `pip install .`
+
 ## Warning: AI fairness != fairness
 There are many ways in which technical approaches to AI fairness, such as this library, are simplistic and limited in actually achieving fairness in real-world decision processes.
 
 More information on these limitations can be found [here](https://dl.acm.org/doi/full/10.1145/3624700) or [here](https://ojs.aaai.org/index.php/AAAI/article/view/26798).
 
 ## Future plans
 The library maintains a core focus on only fairrets for now, yet we plan to add more fairness tools that align with the design principles in the future. These may involve breaking changes. At the same time, we'll keep reviewing the role of this library within the wider ecosystem of fairness toolkits.
```

### Comparing `fairret-0.1.2/fairret.egg-info/SOURCES.txt` & `fairret-0.1.3/fairret.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 docs/requirements.txt
 docs/source/conf.py
 docs/source/index.rst
 docs/source/loss.rst
 docs/source/metric.rst
 docs/source/statistic.rst
 docs/source/_static/Overview_fairret.png
+docs/source/_static/fairret.png
 docs/source/generated/fairret.loss.rst
 examples/complex_sensitive_features.ipynb
 examples/custom_statistic.ipynb
+examples/fairness_metrics.ipynb
 examples/simple_pipeline.ipynb
 examples/stacked_statistic.ipynb
 fairret/__init__.py
 fairret/metric.py
 fairret/utils.py
 fairret.egg-info/PKG-INFO
 fairret.egg-info/SOURCES.txt
```

### Comparing `fairret-0.1.2/pyproject.toml` & `fairret-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fairret-0.1.2/test/test_loss.py` & `fairret-0.1.3/test/test_loss.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,17 +33,25 @@
     feat_backup = feat.clone()
     sens_backup = sens.clone()
 
     fairret = loss_cls(PositiveRate())
     nb_tries = 5
 
     # Calculate loss multiple times as some losses are stateful
-    for _ in range(nb_tries):
-        logit = net(feat)
-        loss = fairret(logit, sens)
+    for attempt in range(nb_tries):
+        if attempt % 2 == 1:
+            # Vary the amount of data to check if the loss can handle it
+            batch_feat = feat[:2]
+            batch_sens = sens[:2]
+        else:
+            batch_feat = feat
+            batch_sens = sens
+
+        logit = net(batch_feat)
+        loss = fairret(logit, batch_sens)
         assert loss.item() >= 0  # fairret should be nonnegative
         loss.backward()
         for p in net.parameters():
             assert p.grad is not None
             assert torch.all(torch.isfinite(p.grad))
             p.grad.zero_()
 
@@ -60,17 +68,26 @@
     sens_backup = sens.clone()
     label_backup = label.clone()
 
     fairret = loss_cls(Accuracy())
     nb_tries = 5
 
     # Calculate loss multiple times as some losses are stateful
-    for _ in range(nb_tries):
-        logit = net(feat)
-        loss = fairret(logit, sens, label)
+    for attempt in range(nb_tries):
+        if attempt % 2 == 1:
+            # Vary the amount of data to check if the loss can handle it
+            batch_feat = feat[:2]
+            batch_sens = sens[:2]
+            batch_label = label[:2]
+        else:
+            batch_feat = feat
+            batch_sens = sens
+            batch_label = label
+        logit = net(batch_feat)
+        loss = fairret(logit, batch_sens, batch_label)
         assert loss.item() >= 0  # fairret should be nonnegative
         loss.backward()
         for p in net.parameters():
             assert p.grad is not None
             assert torch.all(torch.isfinite(p.grad))
             p.grad.zero_()
```

### Comparing `fairret-0.1.2/test/test_metric.py` & `fairret-0.1.3/test/test_metric.py`

 * *Files identical despite different names*

### Comparing `fairret-0.1.2/test/test_statistic.py` & `fairret-0.1.3/test/test_statistic.py`

 * *Files identical despite different names*

