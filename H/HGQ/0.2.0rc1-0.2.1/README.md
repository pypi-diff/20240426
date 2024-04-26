# Comparing `tmp/HGQ-0.2.0rc1.tar.gz` & `tmp/hgq-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HGQ-0.2.0rc1.tar", last modified: Sat Dec  2 02:51:55 2023, max compression
+gzip compressed data, was "hgq-0.2.1.tar", last modified: Fri Apr 26 21:54:05 2024, max compression
```

## Comparing `HGQ-0.2.0rc1.tar` & `hgq-0.2.1.tar`

### file list

```diff
@@ -1,76 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.214615 HGQ-0.2.0rc1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.198615 HGQ-0.2.0rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.202615 HGQ-0.2.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/.github/workflows/sphinx-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15602 2023-12-02 02:51:55.214615 HGQ-0.2.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.202615 HGQ-0.2.0rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.202615 HGQ-0.2.0rc1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8903 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/_static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    14525 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/_static/logo-icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    20384 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      973 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/install.md
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/qkeras.md
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/reference.md
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/status.md
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/tips.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.206615 HGQ-0.2.0rc1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    44996 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/examples/mnist.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/examples/qkeras.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      990 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-02 02:51:55.214615 HGQ-0.2.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.198615 HGQ-0.2.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.206615 HGQ-0.2.0rc1/src/HGQ/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-12-02 02:51:55.000000 HGQ-0.2.0rc1/src/HGQ/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.206615 HGQ-0.2.0rc1/src/HGQ/bops/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/bops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/bops/bops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.206615 HGQ-0.2.0rc1/src/HGQ/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10374 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/layers/batchnorm_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18273 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/layers/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/layers/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/layers/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/layers/passive_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.210615 HGQ-0.2.0rc1/src/HGQ/proxy/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12225 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/proxy/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/proxy/fixed_point_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.210615 HGQ-0.2.0rc1/src/HGQ/proxy/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/proxy/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/proxy/plugins/qkeras.py
--rw-r--r--   0 runner    (1001) docker     (127)    16786 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/proxy/precision_derivation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.210615 HGQ-0.2.0rc1/src/HGQ/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11916 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/quantizer/quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.210615 HGQ-0.2.0rc1/src/HGQ/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.210615 HGQ-0.2.0rc1/src/HGQ.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15602 2023-12-02 02:51:55.000000 HGQ-0.2.0rc1/src/HGQ.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2023-12-02 02:51:55.000000 HGQ-0.2.0rc1/src/HGQ.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-02 02:51:55.000000 HGQ-0.2.0rc1/src/HGQ.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-02 02:51:55.000000 HGQ-0.2.0rc1/src/HGQ.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-12-02 02:51:55.000000 HGQ-0.2.0rc1/src/HGQ.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.210615 HGQ-0.2.0rc1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/test/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/test/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/test/test_convert_manual_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/test/test_end2end_tiny.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/test/test_syn_hlayers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/test/test_syn_large.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/test/test_syn_players.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/test/test_syn_qkeras.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/test/test_syn_small.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:54:05.252783 hgq-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:54:05.240783 hgq-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:54:05.240783 hgq-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-26 21:54:00.000000 hgq-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-26 21:54:00.000000 hgq-0.2.1/.github/workflows/sphinx-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-26 21:54:00.000000 hgq-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-26 21:54:00.000000 hgq-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-04-26 21:54:00.000000 hgq-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16520 2024-04-26 21:54:05.252783 hgq-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-26 21:54:00.000000 hgq-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:54:05.244783 hgq-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-26 21:54:00.000000 hgq-0.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:54:05.244783 hgq-0.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-26 21:54:00.000000 hgq-0.2.1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8903 2024-04-26 21:54:00.000000 hgq-0.2.1/docs/_static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-26 21:54:00.000000 hgq-0.2.1/docs/_static/logo-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-26 21:54:00.000000 hgq-0.2.1/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    31855 2024-04-26 21:54:00.000000 hgq-0.2.1/docs/_static/overview.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-26 21:54:00.000000 hgq-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-26 21:54:00.000000 hgq-0.2.1/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-26 21:54:00.000000 hgq-0.2.1/docs/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-26 21:54:00.000000 hgq-0.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-26 21:54:00.000000 hgq-0.2.1/docs/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-26 21:54:00.000000 hgq-0.2.1/docs/qkeras.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-04-26 21:54:00.000000 hgq-0.2.1/docs/reference.md
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-26 21:54:00.000000 hgq-0.2.1/docs/status.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-26 21:54:00.000000 hgq-0.2.1/docs/tips.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:54:05.244783 hgq-0.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    44996 2024-04-26 21:54:00.000000 hgq-0.2.1/examples/mnist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-26 21:54:00.000000 hgq-0.2.1/examples/qkeras.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-26 21:54:00.000000 hgq-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 21:54:05.252783 hgq-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:54:05.240783 hgq-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:54:05.244783 hgq-0.2.1/src/HGQ/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 21:54:05.000000 hgq-0.2.1/src/HGQ/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:54:05.248783 hgq-0.2.1/src/HGQ/bops/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/bops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/bops/bops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:54:05.248783 hgq-0.2.1/src/HGQ/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10955 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/layers/batchnorm_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18263 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/layers/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/layers/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/layers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/layers/passive_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:54:05.248783 hgq-0.2.1/src/HGQ/proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/proxy/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/proxy/fixed_point_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:54:05.248783 hgq-0.2.1/src/HGQ/proxy/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/proxy/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/proxy/plugins/qkeras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17073 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/proxy/precision_derivation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/proxy/unary_lut.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:54:05.248783 hgq-0.2.1/src/HGQ/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12341 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/quantizer/quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:54:05.248783 hgq-0.2.1/src/HGQ/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-26 21:54:00.000000 hgq-0.2.1/src/HGQ/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:54:05.252783 hgq-0.2.1/src/HGQ.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16520 2024-04-26 21:54:05.000000 hgq-0.2.1/src/HGQ.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-26 21:54:05.000000 hgq-0.2.1/src/HGQ.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 21:54:05.000000 hgq-0.2.1/src/HGQ.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-26 21:54:05.000000 hgq-0.2.1/src/HGQ.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-26 21:54:05.000000 hgq-0.2.1/src/HGQ.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:54:05.252783 hgq-0.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-26 21:54:00.000000 hgq-0.2.1/test/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-26 21:54:00.000000 hgq-0.2.1/test/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-26 21:54:00.000000 hgq-0.2.1/test/test_convert_manual_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-26 21:54:00.000000 hgq-0.2.1/test/test_end2end_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-26 21:54:00.000000 hgq-0.2.1/test/test_syn_hlayers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-26 21:54:00.000000 hgq-0.2.1/test/test_syn_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-26 21:54:00.000000 hgq-0.2.1/test/test_syn_players.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-26 21:54:00.000000 hgq-0.2.1/test/test_syn_qkeras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-26 21:54:00.000000 hgq-0.2.1/test/test_syn_small.py
```

### Comparing `HGQ-0.2.0rc1/.github/workflows/python-publish.yml` & `hgq-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0rc1/.github/workflows/sphinx-build.yml` & `hgq-0.2.1/.github/workflows/sphinx-build.yml`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0rc1/.gitignore` & `hgq-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0rc1/.pre-commit-config.yaml` & `hgq-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0rc1/LICENSE` & `hgq-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0rc1/PKG-INFO` & `hgq-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HGQ
-Version: 0.2.0rc1
+Version: 0.2.1
 Summary: High Granularity Quantizarion
 Author-email: Chang Sun <chsun@cern.ch>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,15 +209,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tensorflow~=2.13
+Requires-Dist: tensorflow<2.16,>=2.13
 Requires-Dist: numpy>=1.23
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: qkeras; extra == "docs"
 Requires-Dist: pyparsing; extra == "docs"
@@ -236,18 +236,32 @@
 # High Granularity Quantization
 
 [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-green.svg)](LICENSE)
 [![Documentation](https://github.com/calad0i/HGQ/actions/workflows/sphinx-build.yml/badge.svg)](https://calad0i.github.io/HGQ/)
 [![PyPI version](https://badge.fury.io/py/hgq.svg)](https://badge.fury.io/py/hgq)
 
 
-HGQ is a framework for quantization aware training of neural networks to be deployed on FPGAs, which allows for per-weight and per-activation bitwidth optimization.
+HGQ is an gradient-based automatic bitwidth optimization and quantization-aware training algorithm for neural networks to be deployed on FPGAs, By laveraging gradients, it allows for bitwidth optimization at arbitrary granularity, up to per-weight and per-activation level.
 
-Depending on the specific [application](https://arxiv.org/abs/2006.10159), HGQ could achieve up to 10x resource reduction compared to the traditional `AutoQkeras` approach, while maintaining the same accuracy. For some more challenging [tasks](https://arxiv.org/abs/2202.04976), where the model is already under-fitted, HGQ could still improve the performance under the same on-board resource consumption. For more details, please refer to our paper (link coming not too soon).
+<img src="docs/_static/overview.svg" alt="HGQ-overview" width="600"/>
 
-This repository implements HGQ for `tensorflow.keras` models. It is independent of the [QKeras project](https://github.com/google/qkeras).
+Compare to the other heterogeneous quantization approach, like the QKeras counterpart, HGQ provides the following advantages:
 
-## Warning:
+- **High Granularity**: HGQ supports per-weight and per-activation bitwidth optimization, or any other lower granularity.
+- **Automatic Quantization**: By setting a resource regularization term, HGQ could automatically optimize the bitwidth of all parameters during training. Pruning is performed naturally when a bitwidth is reduced to 0.
+- **Bit-accurate conversion** to `hls4ml`: You get exactly what you get from `Keras` models from `hls4ml` models. HGQ provides a bit-accurate conversion interface, proxy models, for bit-accurate conversion to hls4ml models.
+  - still subject to machine float precision limitation.
+- **Accurate Resource Estimation**: BOPs estimated by HGQ is roughly #LUTs + 55#DSPs for actual (post place & route) FPGA resource consumption. This metric is available during training, and one can estimate the resource consumption of the final model in a very early stage.
 
-This framework requires an **unmerged** [PR](https://github.com/fastmachinelearning/hls4ml/pull/914) of hls4ml. Please install it by running `pip install "git+https://github.com/calad0i/hls4ml@HGQ-integration"`. Or, conversion will fail with unsupported layer error.
+Depending on the specific [application](https://arxiv.org/abs/2006.10159), HGQ could achieve up to 20x resource reduction compared to the `AutoQkeras` approach, while maintaining the same accuracy. For some more challenging [tasks](https://arxiv.org/abs/2202.04976), where the model is already under-fitted, HGQ could still improve the performance under the same on-board resource consumption. For more details, please refer to our paper (link coming soon).
 
-## This package is still under development. Any API might change without notice at any time!
+## Installation
+
+You will need `python>=3.10` and `tensorflow>=2.13` to run this framework. You can install it via pip:
+
+```bash
+pip install hgq
+```
+
+## Usage
+
+Please refer to the [documentation](https://calad0i.github.io/HGQ/) for more details.
```

### Comparing `HGQ-0.2.0rc1/docs/Makefile` & `hgq-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0rc1/docs/_static/icon.svg` & `hgq-0.2.1/docs/_static/icon.svg`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0rc1/docs/conf.py` & `hgq-0.2.1/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,7 +62,11 @@
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "sphinx_rtd_theme"
 html_static_path = ['_static']
 html_favicon = '_static/icon.svg'
+
+html_css_files = [
+    'custom.css',
+]
```

### Comparing `HGQ-0.2.0rc1/docs/faq.md` & `hgq-0.2.1/docs/faq.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ## What's this?
 
 HGQ is a method for quantization aware training of neural works to be deployed on FPGAs, which allows for per-weight and per-activation bitwidth optimization.
 
 ## Why is it useful?
 
-Depending on the specific [application](https://arxiv.org/abs/2006.10159), HGQ could achieve up to 10x resource reduction compared to the traditional `AutoQkeras` approach, while maintaining the same accuracy. For some more challenging [tasks](https://arxiv.org/abs/2202.04976), where the model is already under-fitted, HGQ could still improve the performance under the same on-board resource consumption. For more details, please refer to our paper (link coming not too soon).
+Depending on the specific [application](https://arxiv.org/abs/2006.10159), HGQ could achieve up to 20x resource reduction compared to the traditional `AutoQkeras` approach, while maintaining the same accuracy. For some more challenging [tasks](https://arxiv.org/abs/2202.04976), where the model is already under-fitted, HGQ could still improve the performance under the same on-board resource consumption. For more details, please refer to our paper (link coming not too soon).
 
 ## Can I use it?
 
 The following conditions must be met:
 
 1. Your model is competible with `hls4ml` (i.e. it can be converted to HLS C++ code).
 2. You are using `Vivado` as your FPGA backend.
```

### Comparing `HGQ-0.2.0rc1/docs/getting_started.md` & `hgq-0.2.1/docs/getting_started.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Quick Start
 
-```{warning}
-This guide is only for models with fully heterogeneous quantized weights. For models with partially-heterogeneous quantized weights, please refer to the [Full Usage](#Full Usage) guide.
+```{note}
+This guide is only for models with fully heterogeneous quantized weights (per-weight bitwidth).
 ```
 
 ## Model definition & training
 
 Let's consider the following model for MNIST classification:
 
 ```python
```

### Comparing `HGQ-0.2.0rc1/docs/qkeras.md` & `hgq-0.2.1/docs/qkeras.md`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0rc1/docs/reference.md` & `hgq-0.2.1/docs/reference.md`

 * *Files 14% similar despite different names*

```diff
@@ -46,28 +46,47 @@
   - Param `parallel_factor`: how many kernel operations are performed in parallel. Defaults to 1. This parameter will be passed to hls4ml.
 - `HActivation`: Similar to the `Activation` layer, but with (heterogeneous) activations.
   - Supports any built-in keras activations, but may or may not be supported by hls4ml, or bit-accurate in general.
   - The tested activations are: `linear`, `relu`, `sigmoid`, `tanh`, `softmax`. `softmax` is never bit-accurate, and `tanh` and `sigmoid` are only bit-accurate when certain conditions are met.
 - `HAdd`: Element-wise addition.
 - `HDenseBatchNorm`: `HDense` with fused batch normalization. No resource overhead when converting to hls4ml.
 - `HConv*DBatchNorm`: `HConv*D` with fused batch normalization. No resource overhead when converting to hls4ml.
+- (New in 0.2) `HActivation` with **arbitrary unary function**. (See note below.)
+
+```{note}
+`HActivation` will be converted to a general `unaryLUT` in `to_proxy_model` when
+ - the required table size is smaller or equal to `unary_lut_max_table_size`.
+ - the corresponding function is not `relu`.
+
+Here, table size is determined by $2^{bw_{in}}$, where $bw_{in}$ is the bitwidth of the input.
+
+If the condition is not met, already supported activations like `tanh` or `sigmoid` will be done in the traditional way. However, if a arbitrary unary function is used, the conversion will fail. Thus, when using arbitrary unary functions, make sure that the table size is small enough.
+```
 
 ```{note}
 `H*BatchNorm` layers require both scaling and shifting parameters to be fused into the layer. Thus, when bias is set to `False`, shifting will not be available.
 ```
 
 Passive layers (`P-` prefix):
 
 - `PMaxPooling*D`: Max pooling layers.
 - `PAveragePooling*D`: Average pooling layers.
 - `PConcatenate`: Concatenate layer.
 - `PReshape`: Reshape layer.
 - `PFlatten`: Flatten layer.
 - `Signature`: Does nothing, but marks the input to the next layer as already quantized to specified bitwidth.
 
+```{note}
+Average pooling layers are now bit-accurate, with the requirement that **all** individual pool size is a power of 2. This include all padded pools, with are with smaller sizes, if any.
+```
+
+```{warning}
+As of hls4ml v0.9.1, padding in pooling layers with `io_stream` is not supported. If you are using `io_stream`, please make sure that the padding is set to `valid`. For more details, merely setting `padding='same'` is fine, but no actual padding may be performed, or the generated firmware will fail at an assertion.
+```
+
 ## Commonly used functions
 
 - `trace_minmax`: Trace the min/max values of the model against a dataset, print computed `BOPs` per-layer, and return the accumulated `BOPs` of the model.
 - `to_proxy_model`: Convert a HGQ model to a hls4ml-compatible proxy model. The proxy model will contain all necessary information for HLS synthesis.
   - Param `aggressive`: If `True`, the proxy model will use `WRAP` for as overflow mode for all layers in seek of latency. If `False`, the overflow mode will be set to `SAT`.
 
 ## Callbacks
@@ -92,7 +111,11 @@
 1. Some intermediate values cannot be represented by the floating point format used by tensorflow, which is usually `float32` (23 bits mantissa) or `TF32` (10 bits mantissa).
 2. For activations, bit-accuracy cannot be guaranteed. A great example of this is `softmax`. Also, unary nonlinear activations may or may not be bit-accurate with the current hls4ml implementation. Currently, if the bitwidth is very high and the input value's range is greater than a certain value, bit-accuracy will be lost due to some hardcoded LUT size in hls4ml.
 ```
 
 ```{tip}
 The proxy model can also be used to convert a `QKeras` model to a bit-accurate hls4ml-ready proxy model. See more details in the [Regarding QKeras](qkeras.md) section.
 ```
+
+```{warning}
+Experimental: Nested layer structure is now supported by `to_keras_model` in v0.2.0. If you pass a model with nested layers, the function will flatten the model. However, be careful that some information in the inner models (e.g., `parallelization_factor`) may be lost during the conversion.
+```
```

### Comparing `HGQ-0.2.0rc1/docs/status.md` & `hgq-0.2.1/docs/status.md`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0rc1/docs/tips.md` & `hgq-0.2.1/docs/tips.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,30 +4,32 @@
 
 The BOPs generated by this framework can be use as a good estimator for the on-chip resource consumption, when the following conditions are met:
 
 - `latency` strategy is used.
 - `reuse_factor` is set to 1.
 - `parallel_factor` is set to match the number of convolution kernel application count (Everything done in parallel).
 
-If `io_parallel` is used, resource consumption in terms of LUTs, can be estimated by: $$\#\mathrm{LUTs}\sim\#\mathrm{BOPs}$$
+If `io_parallel` is used, resource consumption can be estimated in terms of a linear combination of LUTs and DSPs: $$\mathrm{LUTs}+55\cdot\mathrm{LUTs}\sim\mathrm{BOPs}$$
+
+The factor in front of DSPs is rough, but the final order-of-magnitude estimation is still useful.
 
 If `io_stream` is used, you will need to add resources used for FIFOs, which cannot be directly estimated from BOPs, and depends on the specific implementation (i.e. ShiftRegister vs. BRAM).
 
-## Regarding `#pragma HLS DATAFLOW`
+## Regarding `#pragma HLS DATAFLOW` in `vivado/vitis`
 
 If you are using `io_parallel` AND met the above conditions AND and has a colvolution layer in your network, you may get a much larger resource consumption than expected together with terrible latency. In this case, please try changing the `#pragma HLS DATAFLOW` to `#pragma HLS PIPELINE` or simply removing it and re-synthesize the code.
 
-## Regarding `#pragma HLS INLINE RECURSIVE`
+## Regarding `#pragma HLS INLINE RECURSIVE` in `vivado`
 
-If you are using `io_parallel` with `latency` strategy, you may try adding `#pragma HLS INLINE RECURSIVE` to your top function. This **may** reduce the resource consumption for some networks. In many cases, resource consumption can be reduced by $\sim10$%, and latency may or may not be improved.
+If you are using `io_parallel` with `latency` strategy with `vivado_hls`, you may try adding `#pragma HLS INLINE RECURSIVE` to your top function. This **may** reduce the resource consumption for some networks. In many cases, resource consumption can be reduced by $\sim10$%, and latency may or may not be improved.
 
 ## When use intra-layer heterogeneous quantization
 
 If using `latency` strategy, it is **recommended** to use intra-layer heterogeneous weight quantization.
 
 For intra-later heterogeneous activation quantization, if you are using `io_parallel` with `latency` strategy, one **may** enable it. For some networks, this may lead to a huge overfitting, and the resource reduction is not as significant as the weight counterpart.
 
 ## When using only inter-layer heterogeneous quantization
 
-It is **recommended** one should use inter-layer heterogeneous quantization **if and only if** the model is planned to be deployed with the `resource` strategy in `hls4ml`. This is equivalent to optimizing bitwidths with approximated gradient, and the obtained resource may be better or worse than the `AutoQKeras` counterpart.
+One is **recommended** to disable intra-layer heterogeneous weight quantization **if and only if** the model is planned to be deployed with the `resource` strategy in `hls4ml`. When intra-layer heterogeneous quantization is not enabled, this is equivalent to optimizing bitwidths with approximated gradients. The obtained resource may be better or worse than the `AutoQKeras` counterpart.
 
 When doing this, it is **strongly recommended** to use only `L1` and/or `L2` regulation on weights and activations (i.e., set `beta=0`), as the training time BOPs estimated is **not accurate at all and not relevant**.
```

### Comparing `HGQ-0.2.0rc1/examples/mnist.ipynb` & `hgq-0.2.1/examples/mnist.ipynb`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0rc1/examples/qkeras.ipynb` & `hgq-0.2.1/examples/qkeras.ipynb`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0rc1/pyproject.toml` & `hgq-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools_scm>=8"]
 
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HGQ"
-version = "0.2.0rc1"
+version = "0.2.1"
 authors = [{ name = "Chang Sun", email = "chsun@cern.ch" }]
 description = "High Granularity Quantizarion"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
 
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
   "License :: OSI Approved :: Apache Software License",
   "Development Status :: 4 - Beta",
 ]
 
-dependencies = ['tensorflow~=2.13', 'numpy>=1.23']
+dependencies = ['tensorflow>=2.13,<2.16', 'numpy>=1.23']
 
 [project.urls]
 repository = "https://github.com/calad0i/HGQ"
 
 [tool.setuptools_scm]
 write_to = "src/HGQ/_version.py"
```

### Comparing `HGQ-0.2.0rc1/src/HGQ/__init__.py` & `hgq-0.2.1/src/HGQ/__init__.py`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0rc1/src/HGQ/_patch.py` & `hgq-0.2.1/src/HGQ/_patch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 def patch_singledispatch():
     "Patch functools.singledispatch to support Union types. Invoked only for python<=3.10"
     import sys
     if sys.version_info >= (3, 11):
-        print("singledispatch patch not needed for python>=3.11")
         return
     import functools
     from functools import singledispatch as _singledispatch
     from types import UnionType
 
     def singledispatch(func):
         func = _singledispatch(func)
```

### Comparing `HGQ-0.2.0rc1/src/HGQ/bops/bops.py` & `hgq-0.2.1/src/HGQ/bops/bops.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,21 +64,21 @@
             warn(f'cover_factor<1.0 will likely to result in overflows.')
         for layer in model.layers:
             if not isinstance(layer, HLayerBase):
                 continue
 
             aq = layer.paq
             _min, _max = aq._min.numpy(), aq._max.numpy()  # type: ignore
-            cover_factor_min = np.full_like(_min, cover_factor)
-            cover_factor_min[_min > 0] = 1. / cover_factor
-            cover_factor_max = np.full_like(_max, cover_factor)
-            cover_factor_max[_max < 0] = 1. / cover_factor
+            mean = (_min + _max) / 2
+            diff = (_max - _min) / 2
+            _min = mean - diff * cover_factor
+            _max = mean + diff * cover_factor
 
-            aq._min.assign(aq(aq._min * cover_factor_min))  # type: ignore
-            aq._max.assign(aq(aq._max * cover_factor_max))  # type: ignore
+            aq._min.assign(aq(tf.constant(_min)))  # type: ignore
+            aq._max.assign(aq(tf.constant(_max)))  # type: ignore
 
     for layer in model.layers:
         if not hasattr(layer, 'activation'):
             continue
         if not isinstance(layer, HLayerBase):
             continue
         aq = layer.paq
```

### Comparing `HGQ-0.2.0rc1/src/HGQ/layers/base.py` & `hgq-0.2.1/src/HGQ/layers/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,27 +27,32 @@
     def input_bw(self):
         assert len(self._inbound_nodes) <= 1, f"Layer {self.name} is reused {len(self._inbound_nodes)} times. This is not allowed."
         try:
             return self.last_layer.act_bw
         except AssertionError:
             return None
 
+    @property
+    def input_bw_exact(self):
+        assert len(self._inbound_nodes) <= 1, f"Layer {self.name} is reused {len(self._inbound_nodes)} times. This is not allowed."
+        return self.last_layer.act_bw_exact.astype(np.float32)
+
 
 class HLayerBase(ABSBaseLayer):
     """Abstract base class for all layers in the library. Child classes should call post_build() after calling their build() method.
     """
 
     def __init__(self, kq_conf=None, paq_conf=None, beta=0., **kwargs):
         self._has_kernel = None
         self._has_bias = None
         self.kq_config = kq_conf or get_default_kq_conf()
         "kernel quantizer config"
         self.paq_config = paq_conf or get_default_paq_conf()
         "pre-activation quantizer config"
-        self.beta = tf.constant(beta, dtype=tf.float32, name='beta')
+        self.beta = tf.Variable(beta, dtype=tf.float32, name='beta', trainable=False)
         "BOPs-regularization strength"
         self.record_minmax = False
         self._has_last_layer = False
         self._do_adapt_kernel_bits = kwargs.pop('do_adapt_kernel_bits', True)
         self._delayed_kernel_bits_adaption = False
 
         activation = kwargs.get('activation', None)
@@ -77,23 +82,26 @@
             return True
         if self.channel_loc == -1:
             return np.prod(quantizer_shape[:-1]) == 1 and bias_shape == quantizer_shape[-1:]
         elif self.channel_loc == 1:
             return np.prod(quantizer_shape[1:]) == 1 and bias_shape == quantizer_shape[0:1]
         return False
 
+    @property
+    def _relu_act(self):
+        return hasattr(self, 'activation') and self.activation is tf.keras.activations.relu
+
     def post_build(self, input_shape):
         """This method should be called after calling build() method of the child class. It initializes the quantizers and sets the bops variable, and set a few flags (_has_kernel, _has_bias, _relu_act) for convenience.)"""
         self._has_kernel = False
         self._has_bias = False
         if hasattr(self, 'kernel') and self.kernel is not None:
             self._has_kernel = True
         if hasattr(self, 'bias') and self.bias is not None:
             self._has_bias = True
-        self._relu_act = hasattr(self, 'activation') and self.activation is tf.keras.activations.relu
 
         self.init_quantizers(input_shape)
         if not hasattr(self, 'channel_loc'):
             self.channel_loc = -1
         if self.paq_config['rnd_strategy'] == 'auto':
             self.paq.rnd_strategy = 0 if self.can_bias_cover_rnd else 3
 
@@ -165,29 +173,36 @@
         k_bw = tf.nn.relu(int_bits + fp_bits)  # negative sign not considered for kernel
         k_bw = scale_grad(k_bw, tf.sqrt(1. / self.kq.degeneracy))  # type: ignore
         return tf.broadcast_to(k_bw, qk.shape)
 
     @property
     def kernel_bw_exact(self):
         """Returns exact bitwidth of the kernel. Non-differentiable. For post-training use."""
-        int_bits, fb, kn = self.kq.get_bits_exact(self.fused_kernel)
+        kn, int_bits, fb = self.kq.get_bits_exact(self.fused_kernel)
         return int_bits + fb  # sign not considered for kernel
 
     @property
     def act_bw(self):
         """Returns the bitwidth of the pre-activation values. Differentiable."""
         int_bits, fp_bits, kn = self.paq.get_bits(pos_only=self._relu_act)  # type: ignore
         bw = int_bits + fp_bits
         if not self._relu_act:
             bw = bw + kn
         bw = tf.nn.relu(bw)
         bw = scale_grad(bw, tf.sqrt(1. / self.paq.degeneracy))  # type: ignore
         return tf.broadcast_to(bw, (1,) + self.output_shape[1:])
 
     @property
+    def act_bw_exact(self) -> np.ndarray:
+        """Returns the exact bitwidth of the pre-activation values. Non-differentiable. For post-training use."""
+        kn, int_bits, fb = self.paq.get_bits_exact(pos_only=self._relu_act)
+        bw = int_bits + fb + kn
+        return np.broadcast_to(bw, (1,) + self.output_shape[1:])
+
+    @property
     def fused_bias(self):
         return self.bias
 
     @property
     def fused_kernel(self):
         return self.kernel
 
@@ -199,17 +214,14 @@
 
     @property
     @tf.function(jit_compile=True)
     def fused_qbias(self):
         """Returns the final, quantized bias for deployment. non-differentiable, should not be used for training. When using rounding to nearest and the bias can cover the rounding error, bias is pre-biased to cover the rounding shift 2^-fbw, and then TRN can be used instead RND without any loss of accuracy."""
         bias = self.paq.bias_forward(self.fused_bias, False, self.channel_loc)  # type: ignore
 
-        if bias is None:
-            return None
-
         fbw = self.paq.fbw
         if self.channel_loc == -1:
             dims = list(range(len(fbw.shape) - 1))
         elif self.channel_loc == 1:
             dims = [0] + list(range(2, len(fbw.shape)))
         else:
             raise ValueError('channel_loc must be -1 or 1')
```

### Comparing `HGQ-0.2.0rc1/src/HGQ/layers/batchnorm_base.py` & `hgq-0.2.1/src/HGQ/layers/batchnorm_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import tensorflow as tf
 from keras.src.utils import tf_utils
 from tensorflow import keras
 
+from ..utils import warn
 from .base import HLayerBase
 
 
 class HBatchNormBase(HLayerBase):
     def __init__(
         self,
         axis=-1,
@@ -19,14 +20,15 @@
         moving_variance_initializer="ones",
         beta_regularizer=None,
         gamma_regularizer=None,
         beta_constraint=None,
         gamma_constraint=None,
         **kwargs,
     ):
+
         super().__init__(**kwargs)
         self.axis = [axis] if not isinstance(axis, (list, tuple)) else list(axis)
         self.momentum = tf.constant(momentum, dtype=self.dtype)
         self.epsilon = tf.constant(epsilon, dtype=self.dtype)
         self.center = center
         self.scale = scale
         self.beta_initializer = tf.keras.initializers.get(beta_initializer)
@@ -47,14 +49,19 @@
         self.axis: list = tf_utils.validate_axis(self.axis, input_shape)
         self._post_build(input_shape)  # type: ignore
 
     def _post_build(self, input_shape):
         self._reduction_axis = tuple([i for i in range(len(input_shape)) if i not in self.axis])
         output_shape = self.compute_output_shape(input_shape)
         shape = tuple([output_shape[i] for i in self.axis])
+
+        if self.center and not getattr(self, "use_bias", False):
+            warn(f'`center` in fused BatchNorm can only be used if `use_bias` is True. Setting center to False.', stacklevel=3)
+            self.center = False
+
         if self.center:
             self.bn_beta: tf.Variable = self.add_weight(
                 name="bn_beta",
                 shape=shape,
                 initializer=self.beta_initializer,
                 regularizer=self.beta_regularizer,
                 constraint=self.beta_constraint,
@@ -94,15 +101,15 @@
 
     @property
     @tf.function(jit_compile=True)
     def fused_bias(self):
         if not self.center:
             return self.bias
         scale = self.bn_gamma * tf.math.rsqrt(self.moving_variance + self.epsilon)
-        return self.bias - self.moving_mean * scale
+        return self.bias - self.moving_mean * scale + self.bn_beta
 
     def adapt_fused_bn_kernel_bw_bits(self, x: tf.Tensor):
         """Adapt the bitwidth of the kernel quantizer to the input tensor, such that each input is represented with approximately the same number of bits after fused batchnormalization."""
         if not self.scale:
             self.kq.adapt_bw_bits(self.kernel)
             return
```

### Comparing `HGQ-0.2.0rc1/src/HGQ/layers/conv.py` & `hgq-0.2.1/src/HGQ/layers/conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         a = self.activation(z)  # type: ignore
 
         return a, kq
 
     @property
     def compute_exact_bops(self):
         kernel_bw = tf.constant(self.kernel_bw_exact, dtype=tf.float32)
-        input_bw = self.input_bw  # type: ignore
+        input_bw = self.input_bw_exact
         bops = int(tf.reduce_sum(self.convolution_op(input_bw, kernel_bw)).numpy()) * int(self.parallel_factor.numpy()) / int(self.total_channels.numpy())  # type: ignore
         self.bops.assign(tf.constant(bops, dtype=tf.float32))
         return bops
 
 
 @register_keras_serializable(package="HGQ")
 class HConv2D(HConv):
```

### Comparing `HGQ-0.2.0rc1/src/HGQ/layers/dense.py` & `hgq-0.2.1/src/HGQ/layers/dense.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         a, kq = self.jit_forward(x, training=training, record_minmax=record_minmax)  # type: ignore
 
         input_bw = self.input_bw
         if input_bw is not None:
             kernel_bw = self._kernel_bw(kq)  # type: ignore
             bops = tf.reduce_sum(tf.matmul(input_bw, kernel_bw))
             self.bops.assign(bops)
-            bops = tf.cast(bops, tf.float32) * self.beta
+            bops = tf.cast(bops, tf.float32) * self.beta  # type: ignore
             self.add_loss(tf.convert_to_tensor(bops))
         return a
 
     @tf.function(jit_compile=True)
     def jit_forward(self, x, training=None, record_minmax=None):
 
         kq = self.kq(self.fused_kernel, training, False)  # type: ignore
@@ -67,16 +67,16 @@
         a = self.activation(z)  # type: ignore
 
         return a, kq
 
     @property
     def compute_exact_bops(self):
         kernel_bw = self.kernel_bw_exact
-        input_bw = self.input_bw.numpy()  # type: ignore
-        bops = np.sum(np.matmul(input_bw, kernel_bw))
+        input_bw = self.input_bw_exact
+        bops = np.sum(np.matmul(input_bw, kernel_bw))  # type: ignore
         self.bops.assign(tf.constant(bops, dtype=tf.float32))
         return bops
 
 
 @register_keras_serializable(package="HGQ")
 class HDenseBatchNorm(HDense, HBatchNormBase):
 
@@ -152,15 +152,15 @@
             a, kq = self.jit_forward(x, False, record_minmax=record_minmax)  # type: ignore
 
         input_bw = self.input_bw
         if input_bw is not None:
             kernel_bw = self._kernel_bw(kq)  # type: ignore
             bops = tf.reduce_sum(tf.matmul(input_bw, kernel_bw))
             self.bops.assign(bops)
-            bops = tf.cast(bops, tf.float32) * self.beta
+            bops = tf.cast(bops, tf.float32) * self.beta  # type: ignore
             self.add_loss(tf.convert_to_tensor(bops))
         return a
 
     @tf.function(jit_compile=True)
     def bn_train_jit_forward(self, x, training, record_minmax=None):
 
         if self.scale:
```

### Comparing `HGQ-0.2.0rc1/src/HGQ/layers/misc.py` & `hgq-0.2.1/src/HGQ/layers/misc.py`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0rc1/src/HGQ/layers/passive_layers.py` & `hgq-0.2.1/src/HGQ/layers/passive_layers.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,14 +19,20 @@
     @property
     def act_bw(self):
         """Returns the bitwidth of the pre-activation values. Differentiable."""
         shape = (1,) + self.output_shape[1:]
         input_bw = tf.reshape(self.input_bw, shape)
         return tf.ensure_shape(input_bw, shape)
 
+    @property
+    def act_bw_exact(self) -> np.ndarray:
+        """Returns the bitwidth of the pre-activation values. Differentiable."""
+        shape = (1,) + self.output_shape[1:]
+        return self.input_bw_exact.reshape(shape)
+
 
 @register_keras_serializable(package="HGQ")
 class Signature(PLayerBase):
 
     def __init__(self, keep_negative, bits, int_bits, **kwargs):
         super().__init__(**kwargs)
         if not hasattr(keep_negative, 'shape'):
@@ -52,14 +58,18 @@
 
     @property
     @tf.function(jit_compile=True)
     def act_bw(self):
         return tf.keras.backend.cast_to_floatx(self.bits)
 
     @property
+    def act_bw_exact(self) -> np.ndarray:
+        return self.bits.numpy()  # type: ignore
+
+    @property
     def input_bw(self):
         raise ValueError('Signature layer does not have input_bw')
 
     def get_config(self):
         return {
             'name': self.name,
             'keep_negative': self.keep_negative.numpy().tolist(),  # type: ignore
@@ -91,40 +101,54 @@
     @property
     def input_bw(self):
         assert len(self._inbound_nodes) <= 1, f"Layer {self.name} is reused {len(self._inbound_nodes)} times. This is not allowed."
         assert len(self._inbound_nodes[0].inbound_layers) > 1, "Concatenate layer should have at least two inputs"
         input_bws = [l.act_bw for l in self._inbound_nodes[0].inbound_layers]
         return tf.concat(input_bws, axis=self.axis)
 
+    @property
+    def act_bw_exact(self) -> np.ndarray:
+        return np.concatenate([l.act_bw_exact for l in self._inbound_nodes[0].inbound_layers], axis=self.axis)
+
 
 @register_keras_serializable(package="HGQ")
 class PPool2D(PLayerBase, Pooling2D):
 
     def build(self, input_shape):
         super().build(input_shape)
         self._tf_data_format = conv_utils.convert_data_format(self.data_format, 4)
 
     @property
     def act_bw(self):
         act_bw = super().input_bw
         return tf.nn.max_pool2d(act_bw, ksize=self.pool_size, strides=self.strides, padding=self.padding.upper(), data_format=self._tf_data_format)
 
+    @property
+    def act_bw_exact(self) -> np.ndarray:
+        act_bw = super().input_bw_exact
+        return tf.nn.max_pool2d(act_bw, ksize=self.pool_size, strides=self.strides, padding=self.padding.upper(), data_format=self._tf_data_format).numpy()
+
 
 @register_keras_serializable(package="HGQ")
 class PPool1D(PLayerBase, Pooling1D):
 
     def build(self, input_shape):
         super().build(input_shape)
         self._tf_data_format = conv_utils.convert_data_format(self.data_format, 3)
 
     @property
     def act_bw(self):
         act_bw = super().input_bw
         return tf.nn.max_pool1d(act_bw, ksize=self.pool_size, strides=self.strides, padding=self.padding.upper(), data_format=self._tf_data_format)
 
+    @property
+    def act_bw_exact(self) -> np.ndarray:
+        act_bw = super().input_bw_exact
+        return tf.nn.max_pool1d(act_bw, ksize=self.pool_size, strides=self.strides, padding=self.padding.upper(), data_format=self._tf_data_format).numpy()
+
 
 @register_keras_serializable(package="HGQ")
 class PMaxPooling2D(PPool2D, tf.keras.layers.MaxPool2D):
     pass
 
 
 @register_keras_serializable(package="HGQ")
```

### Comparing `HGQ-0.2.0rc1/src/HGQ/proxy/convert.py` & `hgq-0.2.1/src/HGQ/proxy/convert.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,61 @@
-from functools import singledispatch
+from collections.abc import Callable
+from copy import copy, deepcopy
+from functools import partial, singledispatch, singledispatchmethod
+from typing import Any
 
 import numpy as np
 import tensorflow as tf
 from keras.src.engine.keras_tensor import KerasTensor
 from keras.src.engine.node import Node
 from tensorflow import keras
 
 from ..layers import HLayerBase, HQuantize, PDropout, PLayerBase, Signature
 from ..layers.base import ABSBaseLayer
 from ..utils import warn
 from .fixed_point_quantizer import FixedPointQuantizer
 from .precision_derivation import register_qconf
+from .unary_lut import xfr_to_unary_lut
 
 
 def get_all_nodes(model: keras.Model) -> set[Node]:
     """Get all nodes in the model as a set."""
     nodes = set()
+    layers = set(model.layers)
     for layer in model.layers:
         for node in layer._inbound_nodes:
-            nodes.add(node)
+            if node.layer in layers:
+                nodes.add(node)
         for node in layer._outbound_nodes:
-            nodes.add(node)
+            if node.layer in layers:
+                nodes.add(node)
     return nodes
 
 
 def solve_dependencies(model: keras.Model):
     """Given a keras model, return the input nodes, output nodes and a list of (layer, requires, provides) tuples. Requires is a list of nodes that are parents of the layer, provides is the node that is the output of the layer."""
     inp_tensors: list[KerasTensor] = model.inputs  # type:ignore
     out_tensors: list[KerasTensor] = model.outputs  # type:ignore
 
     input_nodes: list[Node] = [t.node for t in inp_tensors]  # type:ignore
     output_nodes: list[Node] = [t.node for t in out_tensors]  # type:ignore
 
     nodes = get_all_nodes(model)
 
-    dependencies_list: list[tuple[keras.layers.Layer, list[Node], Node]] = []
+    dependencies_dict: dict[Node, tuple[keras.layers.Layer, list[Node]]] = {}
     "List of (layer, requires, provides) tuples; requires is a list of nodes, provides is a single node."
 
     for node in nodes:
         if node.is_input:
             continue
-        layer = node.layer
-        if layer not in model.layers:
-            continue
+        layer = node.layer  # layer that is called on the node
         requires = list(node.parent_nodes)
         provides = node
-        dependencies_list.append((layer, requires, provides))
-    return input_nodes, output_nodes, dependencies_list
+        dependencies_dict[provides] = (layer, requires)
+    return input_nodes, output_nodes, dependencies_dict
 
 
 def get_weight(layer: keras.layers.Layer, name: str):
     """Given a layer and a weight name, return the weight. The weight name may or may not contain the layer name. If the number index is missing, it is assumed to be 0."""
     if '/' in name:
         name = name.split('/')[-1]
     if ':' not in name:
@@ -95,203 +100,274 @@
             while f'{name}_{i}' in self.used_names:
                 i += 1
             name = f'{name}_{i}'
         self.used_names.add(name)
         return name
 
 
-def extract_keras_layers(layer: HLayerBase | PLayerBase, name: str) -> tuple[keras.layers.Layer, ...]:
-    """Given a HGQ layer, return a tuple of keras layers in corresponding order. The tuple may be empty if the layer is a quantizer, or containing only the corresponding layer if the layer is an activation or does not have a non-linear activation, or containing the corresponding layer and the activation layer otherwise.
+def _get_out_tensor(
+    dependencies_dict: dict[Node, tuple[keras.layers.Layer, list[Node]]],
+    satisfied: dict[Node, Any],
+    node: Node,
+    namer: Namer | None = None,
+    layer_xformer: Callable[[keras.layers.Layer], keras.layers.Layer] = lambda x: x,
+):
+    """Given a node, get the output tensor provided generated by the node."""
+
+    assert node not in satisfied, f'Node {node} already satisfied.'
+
+    namer = namer or Namer()
+    layer, requires = dependencies_dict[node]
+    inps = []
+    for req in requires:
+        if req in satisfied:
+            inps.append(satisfied[req])
+        else:
+            inp = _get_out_tensor(dependencies_dict, satisfied, req, namer, layer_xformer)
+            inps.append(inp)
+    if len(inps) == 1:
+        inps = inps[0]
+
+    satisfied[node] = apply_layer(layer, inps, namer=namer, layer_xformer=layer_xformer)
+    return satisfied[node]
+
+
+@singledispatch
+def apply_layer(
+    layer: keras.layers.Layer | None,
+    inp_tensors: list[tf.Tensor] | tf.Tensor,
+    namer: None | Namer = None,
+    # satisfied: dict[Node, Any] | None = None,
+    layer_xformer: Callable[[keras.layers.Layer], keras.layers.Layer] = lambda x: x,
+):
+    """
+    Apply a layer to the input tensors:
+      - if the layer is a model, apply the model recursively in a flattened manner.
+      - if the layer is a keras layer, transform it by layer_transformer, until the exactly same reference is returned.
+    """
+
+    layer_xf = layer_xformer(layer)
+    n = 0
+    namer = namer or Namer()
+    while layer_xf is not layer:
+        if isinstance(layer_xf, keras.Model):
+            # layer_transformer may return a keras.Model from a layer.
+            return apply_layer(layer_xf, inp_tensors, namer=namer, layer_xformer=layer_xformer)
+        assert n < 1024, f'layer_transformer does not converge for layer (name: {layer.name if layer is not None else None}).'
+        layer = layer_xf
+        layer_xf = layer_xformer(layer)
+        n += 1
+
+    if layer_xf is not None:
+        name = namer.next_name(layer_xf.name)
+        layer_xf._name = name
+        # Remove all inbound and outbound nodes to clean up the graph.
+        layer_xf = copy(layer_xf)
+        layer_xf._inbound_nodes = []
+        layer_xf._outbound_nodes = []
+        return layer_xf(inp_tensors)
+    else:
+        return inp_tensors
+
+
+@apply_layer.register
+def _(
+    layer: keras.Model,
+    inp_tensors: list[tf.Tensor] | tf.Tensor,
+    namer: None | Namer = None,
+    # satisfied: dict[Node, Any] | None = None,
+    layer_xformer: Callable[[keras.layers.Layer], keras.layers.Layer] = lambda x: x,
+):
+    model = layer
+    if not model.built:
+        if isinstance(inp_tensors, (list, tuple)):
+            model.build([t.shape for t in inp_tensors])
+        else:
+            model.build(inp_tensors.shape)
+
+    namer = namer or Namer()
+    inp_tensors = [inp_tensors] if not isinstance(inp_tensors, (list, tuple)) else inp_tensors
+    input_nodes, output_nodes, dependencies_dict = solve_dependencies(model)
+    satisfied = {node: tensor for node, tensor in zip(input_nodes, inp_tensors)}
+    get_out_tensor = partial(_get_out_tensor, dependencies_dict, satisfied, namer=namer, layer_xformer=layer_xformer)
+    outs = [get_out_tensor(output_node) for output_node in output_nodes]
+    return outs[0] if len(outs) == 1 else outs
+
+
+def convert_model(model: keras.Model, layer_xformer: Callable[[keras.layers.Layer], keras.layers.Layer] = lambda x: x):
+    """For a keras model, convert each layer with layer_transformer, flatten all layers (remove all keras.Model as layers), and return a new model.
+
+    Args:
+        model (keras.Model): Input keras model.
+        layer_transformer: A function that takes a keras layer and returns a keras layer (can be a keras.Model). For the final set of layer, it must return the same reference, rather than a copy, or the conversion will never end.
+
+    Returns:
+        keras.Model: A new keras model.
+
+    Examples:
+        Simply flatten a keras model: `convert_model(model)`
+        Flatten a keras model, return a new model with all
+    """
+
+    inputs: list[tf.Tensor] = [keras.layers.Input(shape=t.shape[1:]) for t in model.inputs]  # type: ignore
+    if len(inputs) == 1:
+        inputs = inputs[0]
+    outs = apply_layer(model, inputs, layer_xformer=layer_xformer)
+    return keras.Model(inputs, outs)
+
+
+@singledispatch
+def to_keras_layer(layer):
+    raise TypeError(f'No matching overload for layer type {type(layer)}. Signatures available: {to_keras_layer.registry.keys()}')
+
+
+@to_keras_layer.register
+def _(layer: ABSBaseLayer):
+    """Given a HGQ layer, return the corresponding keras layer.
 
     Example:
-        HQuantize -> ()
-        HDense[linaer] -> (Dense,)
-        HDense[relu] -> (Dense, Activation)
+        HDense -> Dense
+        HQuantize -> Raise TypeError
     """
 
-    if isinstance(layer, (HQuantize, Signature)):
-        return tuple()
+    assert not isinstance(layer, (HQuantize, Signature)), 'to_keras_layers should not be called on HQuantize or Signature layers.'
 
     if hasattr(layer, 'get_keras_config'):
         conf = layer.get_keras_config()
     else:
         conf = layer.get_config()
-    conf['name'] = name
-    activation_layer = None
 
     if not isinstance(layer, keras.layers.Activation):
         if 'activation' in conf and conf['activation'] != 'linear':
-            activation = conf['activation']
-            if isinstance(activation, str):
-                activation_name = activation
-            else:
-                activation_name = activation.__name__
-            activation_layer = keras.layers.Activation(activation, name=f'{name}_{activation_name}')
+            # Activation will be processed separately for non-activation layers.
             conf['activation'] = 'linear'
+    else:
+        # Prevent custom activation crashing conversion.
+        conf['activation'] = layer.activation
+
     cls_name = layer.__class__.__name__[1:]
     if hasattr(keras.layers, cls_name):
         layer_cls = getattr(keras.layers, cls_name)
     elif hasattr(keras.layers, cls_name.replace('BatchNorm', '')):
         layer_cls = getattr(keras.layers, cls_name.replace('BatchNorm', ''))
     else:
         raise RuntimeError(f'Unknown layer type {layer.__class__.__name__}: no corresponding keras layer found.')
     klayer = layer_cls.from_config(conf)
     klayer.build(layer.input_shape)
     copy_fused_weights(layer, klayer)
-    if activation_layer is not None:
-        return klayer, activation_layer
-    else:
-        return klayer,
-
-
-def extract_quantizers(layer: HLayerBase | Signature, name: str, SAT='WRAP') -> tuple[FixedPointQuantizer, ...]:
-    """Given a HGQ layer, return a tuple of quantizers that are used in the layer."""
-    if isinstance(layer, Signature):
-        return FixedPointQuantizer(layer.keep_negative, layer.bits, layer.int_bits, 'TRN', SAT),
-
-    quantizer = layer.paq
-    if quantizer.rnd_strategy != 3 and not layer.can_bias_cover_rnd:
-        RND = 'RND'
-    else:
-        RND = 'TRN'
-
-    relu_act = layer._relu_act
-    overriddes = None
-    if layer._has_kernel:
-        if hasattr(layer, 'parallel_factor'):
-            parallel_factor = int(layer.parallel_factor)
-            overriddes = {'layers': {name: {'parallelization_factor': parallel_factor}}}
-
-    int_bits, fp_bits, kn = quantizer.get_bits_exact(pos_only=False)  # type: ignore
-
-    if not relu_act:
-        k, b, i = kn, kn + int_bits + fp_bits, kn + int_bits
-        return FixedPointQuantizer(k, b, i, RND, SAT, name=f'{name}_quantizer', overrides=overriddes),
-
-    mask = int_bits + fp_bits + kn > 0
-
-    r_int_bits, r_fp_bits, rk = quantizer.get_bits_exact(pos_only=True)
-    rk, rb, ri = rk, r_int_bits + r_fp_bits, r_int_bits
-    relu_quantizer = FixedPointQuantizer(rk, rb, ri, RND, SAT, name=f'{name}_relu_quantizer')
+    return klayer
 
-    if isinstance(layer, keras.layers.Activation):
-        return relu_quantizer,
 
-    k = tf.reduce_max(kn[mask], keepdims=True)
-    i = tf.reduce_max(int_bits[mask], keepdims=True)
-    f = tf.reduce_max(fp_bits[mask], keepdims=True)
-    k, b, i = k, k + i + f, k + i
+class ProxyLayerXFormer:
+    def __init__(self, SAT='WRAP', use_uniary_lut=False):
+        self.SAT = SAT
+        self.use_uniary_lut = use_uniary_lut
+
+    @singledispatchmethod
+    def get_kbiRS(self, layer: HLayerBase, **kwargs):
+        q = layer.paq
+        pos_only = kwargs.get('pos_only', False)
+        k, i, f = q.get_bits_exact(pos_only=pos_only)
+        k, b, i = k, k + i + f, k + i
+        if q.rnd_strategy != 3 and not layer.can_bias_cover_rnd:
+            RND = 'RND'
+        else:
+            RND = 'TRN'
+        return k, b, i, RND, self.SAT
 
-    # If there is a rounding following the layer, keep one or two extra bit and do NOT round perserve bit accuracy.
-    if RND == 'RND':
-        b += 1
-    elif RND != 'TRN':
-        b += 2
+    @singledispatchmethod
+    def __call__(self, layer: keras.layers.Layer | None) -> keras.layers.Layer | None:
+        if layer is None:
+            return None
+        try:
+            from hls4ml.converters.keras_to_hls import layer_handlers
+        except ImportError:
+            return layer
+        cls_name = layer.__class__.__name__
+        assert cls_name in layer_handlers, f'Layer {layer.name}: {cls_name} is not supported by hls4ml.'
+        return layer
+
+    @__call__.register
+    def _(self, layer: HQuantize):
+        kbiRS = self.get_kbiRS(layer)
+        return FixedPointQuantizer(*kbiRS, name=layer.name)
+
+    @__call__.register
+    def _(self, layer: Signature):
+        return FixedPointQuantizer(layer.keep_negative, layer.bits, layer.int_bits, 'TRN', self.SAT, name=layer.name)
+
+    @__call__.register
+    def _(self, layer: HLayerBase):
+        # HLayer = Layer + Quantizer, or Layer + Quantizer1 + ReLU + Quantizer2
 
-    layer_quantizer = FixedPointQuantizer(k, b, i, 'TRN', SAT, name=f'{name}_quantizer', overrides=overriddes)
+        name = layer.name
+        klayer = to_keras_layer(layer)
 
-    return layer_quantizer, relu_quantizer
+        input_shape = layer.input_shape
+        if isinstance(input_shape, tuple):
+            inputs = keras.layers.Input(shape=input_shape[1:])
+        else:
+            inputs = [keras.layers.Input(shape=shape[1:]) for shape in input_shape]
 
+        overrides = {'layers': {}}
+        if hasattr(layer, 'parallel_factor'):
+            parallel_factor = layer.parallel_factor
+            overrides = {'layers': {name: {'parallelization_factor': int(parallel_factor)}}}
 
-@singledispatch
-def to_proxy_layers(layer, name, SAT: str) -> tuple[keras.layers.Layer, ...]:
-    """Given a layer, return a tuple of keras layers and quantizers that are equivalent to the layer when applied in order. (When it doesn't overflow, and up to fp precision)"""
-    if hasattr(keras.layers, layer.__class__.__name__):
-        # Is already vanilla keras layer
-        new_layer = layer.__class__.from_config(layer.get_config())
-        new_layer.build(layer.input_shape)
-        for w1, w2 in zip(new_layer.weights, layer.weights):
-            w1.assign(w2)
-        return new_layer,
-
-    raise TypeError(f'No matching overload for layer type {type(layer)}. Signatures available: {to_proxy_layers.registry.keys()}')
-
-
-@to_proxy_layers.register
-def _(layer: ABSBaseLayer, name: str, SAT: str):
-    proxy_quantizer_layers = ()
-    layers = []
-    proxy_layers = list(extract_keras_layers(layer, name))
-
-    if hasattr(layer, 'paq') or isinstance(layer, Signature):
-        proxy_quantizer_layers = list(extract_quantizers(layer, name, SAT))
-    if len(proxy_layers) > len(proxy_quantizer_layers) and isinstance(layer, HLayerBase):
-        warn(f'Layer {layer.name} does not have a quantizer attached!')
-
-    while proxy_layers or proxy_quantizer_layers:
-        if proxy_layers:
-            layers.append(proxy_layers.pop(0))
-        if proxy_quantizer_layers:
-            layers.append(proxy_quantizer_layers.pop(0))
-
-    assert layers, f'Failed to convert layer {layer.name}: layer not mapped to anything.'
-    return tuple(layers)
-
-
-SKIP_LAYERS = (PDropout,)
-
-
-def apply_proxy_layers(layer: keras.layers.Layer, tensor, namer: Namer | None = None, SAT='WRAP'):
-    """Given a HGQ-competible layer and a tensor, return the output of the layer when applied to the tensor. Used in builing the proxy model."""
-    if isinstance(layer, SKIP_LAYERS):
-        return tensor
-    if namer is not None:
-        name = namer.next_name(layer.name)
-    else:
-        name = layer.name
-    for l in to_proxy_layers(layer, name, SAT):
-        tensor = l(tensor)
-    return tensor
+        if not isinstance(klayer, keras.layers.Activation):
+            if layer._relu_act:  # a non-activation layer can only have relu or liner as activation
+                k, i, f = layer.paq.get_bits_exact(pos_only=False)
+                k, i, f = tf.reduce_max(k), tf.reduce_max(i), tf.reduce_max(f)
+                k, b, i = k, k + i + f, k + i
+                rk, rb, ri, R, S = self.get_kbiRS(layer, pos_only=True)
+
+                f_add_bits = 0 if R == 'TRN' else 1 if R == 'RND' else 2
+                fq1 = FixedPointQuantizer(k, b + f_add_bits, i, SAT=S, RND='TRN', name=f'{name}_quantizer')
+                fq2 = FixedPointQuantizer(rk, rb, ri, SAT=S, RND=R, name=f'{name}_relu_quantizer', overrides=overrides)
+                return keras.Model(inputs, fq2(keras.layers.ReLU()(fq1(klayer(inputs)))))
+
+        k, b, i, R, S = self.get_kbiRS(layer)
+        q = FixedPointQuantizer(k, b, i, R, SAT=S, name=f'{name}_quantizer', overrides=overrides)
+        return keras.Model(inputs, q(klayer(inputs)))
+
+    @__call__.register
+    def _(self, layer: PLayerBase):
+        klayer = to_keras_layer(layer)
+        return klayer
+
+    @__call__.register
+    def _(self, layer: keras.layers.Dropout):
+        # Dropout does nothing at inference time
+        return None
+
+    @__call__.register
+    def _(self, layer: keras.layers.Activation):
+        # Purge linear activation on sight
+        if layer.activation is keras.activations.linear:
+            return None
+        return layer
 
 
-def to_proxy_model(model: keras.Model, aggressive: bool = True, accum_fp_max_offset: int | None = None):
+def to_proxy_model(model: keras.Model, aggressive: bool = True, accum_fp_max_offset: int | None = None, unary_lut_max_table_size=-1):
     """Given a HGQ model, return a hls4ml-ready keras model.
 
     Args:
         model: The HGQ model to be converted.
 
-        aggressive (default: True): If True, use WRAP overflow mode. Sigificant performance degradation may occur if overflow occurs, but latency may be reduced. If False, use SAT overflow mode. Performance is more stable when it overflows, but latency may be increased.
+        aggressive (default: True): If True, use WRAP overflow mode. Significant performance degradation may occur if overflow occurs, but latency may be reduced. If False, use SAT overflow mode. Performance is more stable when it overflows, but latency may be increased.
 
-        accum_fp_max_offset (default: None): If not None, autoset accumlator such that the model is bit accurate (when no overflow occurs and up to fp precision). If set, use the specified number of floating bits plus result float bits as accumlator float bits. May improve latency in some rare cases, not recommended in general.
+        accum_fp_max_offset (default: None): If not None, autoset accumulator such that the model is bit accurate (when no overflow occurs and up to fp precision). If set, use the specified number of floating bits plus result float bits as accumulator float bits. May improve latency in some rare cases, not recommended in general.
+
+        unary_lut_max_table_size (default: -1): If greater than 0, use unary LUT for `HActivation` layers, when the required table size is less than or equal to the specified value. If set to -1, do not use unary LUT.
 
     """
-    input_nodes, output_nodes, dependencies_list = solve_dependencies(model)
 
     if accum_fp_max_offset is not None and not aggressive:
         warn('You are using bitgrowth (aggressive=False) together with bias_accum_bits set. This is not recommended. If you are sure what you are doing, ignore this warning.')
     if accum_fp_max_offset is not None and accum_fp_max_offset < 0:
         warn('You are using a negative value for bias_accum_bits. Please make sure you know what you are doing.')
-
-    nof_output = len(output_nodes)
-    inputs = [keras.layers.Input(shape=node.input_shapes[0][1:]) for node in input_nodes]
-    satisfied = {node: tensor for node, tensor in zip(input_nodes, inputs)}
-    outputs = []
-    namer = Namer()
-    i = 0
-    if aggressive:
-        SAT = 'WRAP'
-    else:
-        SAT = 'SAT'
-    while dependencies_list and not len(outputs) == nof_output:
-        layer, requires, provides = dependencies_list.pop(0)
-        if set(requires).issubset(satisfied):
-            inps = [satisfied[node] for node in requires]
-            if len(inps) == 1:
-                inps = inps[0]
-            out = apply_proxy_layers(layer, inps, namer=namer, SAT=SAT)
-            satisfied[provides] = out
-            if provides in output_nodes:
-                outputs.append(out)
-        else:
-            i += 1
-            if i == 65535:
-                raise RuntimeError('Infinite loop detected.')
-            dependencies_list.append((layer, requires, provides))
-
-    if len(outputs) == 1:
-        outputs = outputs[0]
-    if len(inputs) == 1:
-        inputs = inputs[0]
-    proxy = keras.Model(inputs=inputs, outputs=outputs)
+    proxy = convert_model(model, layer_xformer=ProxyLayerXFormer('WRAP' if aggressive else 'SAT').__call__)
+    if unary_lut_max_table_size > 0:
+        proxy = convert_model(proxy, layer_xformer=partial(xfr_to_unary_lut, max_table_size=unary_lut_max_table_size))
     for layer in proxy.layers:
         register_qconf(layer, accum_fp_max_offset=accum_fp_max_offset)
     return proxy
```

### Comparing `HGQ-0.2.0rc1/src/HGQ/proxy/fixed_point_quantizer.py` & `hgq-0.2.1/src/HGQ/proxy/fixed_point_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,15 @@
     return gfixed(0, bits, integer_bits, RND, SAT)
 
 
 def fixed(bits, integer_bits, RND='TRN', SAT='WRAP') -> Callable:
     return gfixed(1, bits, integer_bits, RND, SAT)
 
 
+@keras.utils.register_keras_serializable(package='HGQ')
 class FixedPointQuantizer(keras.layers.Layer, metaclass=abc.ABCMeta):
 
     def __init__(self, keep_negative, bits, integers, RND: str = 'TRN', SAT: str = 'WRAP', overrides: dict | None = None, **kwargs):
 
         zeros = bits == 0
 
         if not hasattr(keep_negative, 'shape'):
@@ -170,15 +171,15 @@
         self.SAT = SAT
         self.overrides = overrides or {'layers': {}}
         kwargs.pop('trainable', None)
         self._quantizer_created = False
 
         super().__init__(trainable=False, **kwargs)
 
-    def call(self, x, training=None):
+    def call(self, x, training=None):  # type:ignore
         assert not training, "Proxy model shall can not be trained!"
         if not self.built:
             self.build(x.shape)
         return gfixed_quantizer(x, self.keep_negative, self.bits, self.integers, self.RND, self.SAT)  # type:ignore
 
     @property
     def result_t_kif(self):
@@ -205,15 +206,17 @@
             return True
         if not tf.reduce_all(self.integers == i0):
             return True
         return False
 
     def get_config(self):
         assert tf.reduce_all((self.keep_negative == 0) | (self.keep_negative == 1)), 'Illegal bitwidth config: keep_negative must be 0 or 1.'
-        assert tf.reduce_all(self.bits >= 0), 'Illegal bitwidth config: bits must be non-negative.'  # type:ignore
+        if not tf.reduce_all(self.bits >= 0):  # type:ignore
+            warn('Illegal bitwidth config: bits must be non-negative.')
+            self.bits.assign(tf.maximum(self.bits, 0))
         conf = super().get_config()
         conf['RND'] = self.RND
         conf['SAT'] = self.SAT
         conf['shape'] = tuple(self.bits.shape)
         overrides = self.overrides
 
         conf['overrides'] = overrides
```

### Comparing `HGQ-0.2.0rc1/src/HGQ/proxy/plugins/qkeras.py` & `hgq-0.2.1/src/HGQ/proxy/plugins/qkeras.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from qkeras.quantizers import BaseQuantizer
 from qkeras.utils import _add_supported_quantized_objects
 from tensorflow import keras
 
 from HGQ.proxy.fixed_point_quantizer import FixedPointQuantizer
 from HGQ.utils import warn
 
-from ..convert import to_proxy_layers
+from ..convert import ProxyLayerXFormer
 from ..precision_derivation import get_produced_kif
 
 qkeras_objects = {}
 _add_supported_quantized_objects(qkeras_objects)
 
 qkeras_layers = {v for v in qkeras_objects.values() if issubclass(v, keras.layers.Layer)}
 qkeras_quantizers = {v for v in qkeras_objects.values() if issubclass(v, BaseQuantizer)}
@@ -32,14 +32,19 @@
 }
 
 from functools import singledispatch
 
 
 @singledispatch
 def qkeras_quantizer_to_layers(quantizer, SAT) -> tuple[keras.layers.Layer, ...]:
+    """
+    Map qkeras quantizer to a tuple of equivalent proxy layers.
+        e.g.: quantized_bits -> (fixed,)
+              quantized_relu -> (fixed, relu, fixed)
+    """
     raise TypeError(f"Unknown quantizer type {type(quantizer)}")
 
 
 @qkeras_quantizer_to_layers.register
 def _(quantizer: quantizers.quantized_bits, SAT):
     assert quantizer.alpha == 1, f"alpha != 1 is not currently supported, got {quantizer.alpha}."
     k = quantizer.keep_negative
@@ -83,15 +88,15 @@
 
 
 @qkeras_quantizer_to_layers.register
 def _(quantizer: quantizers.quantized_po2 | quantizers.quantized_relu_po2):
     raise ValueError("quantized_po2 family cannot be implemented in hls4ml as activation.")
 
 
-def qlayer_to_keras_layer(layer: keras.layers.Layer, name) -> keras.layers.Layer | None:
+def qlayer_to_keras_layer(layer: keras.layers.Layer) -> keras.layers.Layer | None:
     base_cls_name = layer.__class__.__name__[1:]
     if not hasattr(keras.layers, base_cls_name):
         raise ValueError(f"Cannot find corresponding keras layer for {layer.__class__.__name__}")
     base_cls = getattr(keras.layers, base_cls_name)
     conf = layer.get_config()
 
     # For some ridiculous reason, QAactivation's activation is called quantizer
@@ -104,45 +109,55 @@
     blacklist = ('quantize', 'kernel_range', 'bias_range', 'constraint', 'activation', 'initializer')
     for k in list(conf.keys()):
         for k_rm in blacklist:
             if k_rm in k:
                 del conf[k]
                 continue
 
-    conf['name'] = name
     klayer = base_cls(**conf)
     klayer.trainable = False
     klayer.build(layer.input_shape)
     if hasattr(layer, 'kernel'):
         q = layer.kernel_quantizer_internal or (lambda x: x)
         klayer.kernel.assign(q(layer.kernel))
     if hasattr(layer, 'bias'):
         q = layer.bias_quantizer_internal or (lambda x: x)
         klayer.bias.assign(q(layer.bias))
     return klayer
 
 
-def qlayer_to_proxy_layers(layer: keras.layers.Layer, name: str, SAT: str) -> tuple[keras.layers.Layer, ...]:
-    klayer = qlayer_to_keras_layer(layer, name)
+def qlayer_to_proxy_layer(self: ProxyLayerXFormer, layer: keras.layers.Layer) -> tuple[keras.layers.Layer, ...]:
+
+    SAT = self.SAT
+    klayer = qlayer_to_keras_layer(layer)
     if not hasattr(layer, 'activation'):
         assert klayer is not None
-        return klayer,
+        return klayer
 
     activation = layer.quantizer if hasattr(layer, 'quantizer') else layer.activation
     act_layers = qkeras_quantizer_to_layers(activation, SAT)
-    if klayer is not None:
-        return klayer, *act_layers
+
+    input_shape = layer.input_shape
+    if isinstance(input_shape, tuple):
+        inputs = keras.layers.Input(shape=input_shape[1:])
     else:
-        return *act_layers,
+        inputs = [keras.layers.Input(shape=shape[1:]) for shape in input_shape]
+
+    out = inputs
+    if klayer is not None:
+        out = klayer(out)
+    for layer in act_layers:
+        out = layer(out)
+    return keras.Model(inputs, out)
 
 
 class QKerasBaseLayer(metaclass=abc.ABCMeta):
     pass
 
 
 for layer_cls in qkeras_layers:
     QKerasBaseLayer.register(layer_cls)
 
 
 def init():
-    to_proxy_layers.register(QKerasBaseLayer, qlayer_to_proxy_layers)
+    ProxyLayerXFormer.__call__.register(QKerasBaseLayer, qlayer_to_proxy_layer)
     get_produced_kif.register(qkeras.QActivation, get_produced_kif.registry[keras.layers.Activation])
```

### Comparing `HGQ-0.2.0rc1/src/HGQ/proxy/precision_derivation.py` & `hgq-0.2.1/src/HGQ/proxy/precision_derivation.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,18 +98,21 @@
         layer.integers.assign(tf.minimum(layer.integers, k + i))
         layer.bits.assign(tf.minimum(layer.bits, k + i + f))
 
     return k, i, f
 
 
 @get_produced_kif.register
-def _(layer: keras.layers.Activation):
+def _(layer: keras.layers.Activation | keras.layers.ReLU | keras.layers.LeakyReLU | keras.layers.Softmax):
     kifs = get_input_kifs(layer)
     assert len(kifs) == 1, f'Activation layer {layer.name} has more than one input. This is not supported.'
-    if layer.activation is tf.keras.activations.softmax:
+    if isinstance(layer, keras.layers.Activation):
+        if layer.activation is tf.keras.activations.softmax:
+            return 0, 1, 65535
+    if isinstance(layer, keras.layers.Softmax):
         return 0, 1, 65535
     k, i, f = activation_kif_forward(layer, *np.max(kifs, axis=0))
     return k, i, f
 
 
 @get_produced_kif.register
 def _(layer: AvgPool1D | AvgPool2D | AvgPool3D):
@@ -139,15 +142,16 @@
 
 @get_produced_kif.register
 def _(layer: keras.layers.Dense | Conv):
     kifs = get_input_kifs(layer)
     assert len(kifs) == 1, f'Dense layer {layer.name} has more than one input. This is not supported.'
     k, i, f = kifs[0]
     w_k, w_i, w_f = get_arr_container(layer.kernel.numpy())
-    k, i, f = int(k or w_k), i + w_i, f + w_f
+    k = int(k or w_k or np.any(layer.use_bias and layer.bias < 0))  # type: ignore
+    i, f = i + w_i, f + w_f
     if isinstance(layer, Conv):
         div = layer.filters
     else:
         div = layer.units
 
     multiplicity = np.prod(layer.kernel.shape) / div
     i += int(np.ceil(np.log2(multiplicity)))
@@ -186,15 +190,15 @@
 # Given a layer, get the bitwidth it requests (maximum bitwidth it can make use of), as a tuple of (k, i, f).
 # ===================================================================================================
 
 
 @singledispatch
 def get_request_kif(layer: keras.layers.Layer) -> tuple[int, int, int]:
     """Get the requested bitwidth of a layer, as a tuple of (k, i, f)"""
-    if isinstance(layer, (Pooling1D, Pooling2D, Pooling3D, Concatenate, Reshape, Flatten)):
+    if isinstance(layer, (Concatenate, Reshape, Flatten)):
         out_layers: list[keras.layers.Layer] = [node.outbound_layer for node in layer._outbound_nodes]
         if out_layers:
             # Layers that does nothing. Pass through.
             requested_kifs = [get_request_kif(out_layer) for out_layer in out_layers]
             k, i, f = np.max(requested_kifs, axis=0)
             return k, i, f
     return 1, 65535, 65535
@@ -378,11 +382,13 @@
     q = _get_next_quantizer(layer) or _get_last_quantizer(layer)
     assert q is not None, f'Layer {layer.name} has no quantizer before or after it. Did you create a valid proxy model?'
     return q
 
 
 def register_qconf(layer: keras.layers.Layer, accum_fp_max_offset: None | int = None):
     """Get and register quantization configuration for a layer in the proxy model."""
+    if hasattr(layer, 'proxy_ready'):
+        return
     q = get_whatever_quantizer(layer)
     conf = get_config(layer, accum_fp_max_offset=accum_fp_max_offset)
     overrides = q.overrides or {}
     overrides['layers'].setdefault(layer.name, {}).update(conf)
```

### Comparing `HGQ-0.2.0rc1/src/HGQ/quantizer/quantizer.py` & `hgq-0.2.1/src/HGQ/quantizer/quantizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,14 +45,17 @@
     n = int(np.ceil(np.max(np.log2(arr + 1))))  # type: ignore
     divisor = 2**np.arange(1, n)[None, ...]  # type: ignore
     low_pos = np.sum(arr % divisor == 0, axis=-1) + (arr[..., 0] == 1)
     with np.errstate(divide='ignore'):
         high_pos = np.where(arr[..., 0] != 0, np.floor(np.log2(arr[..., 0]) + 1), low_pos).astype(np.int8)
     fb = 32 - low_pos
     int_bits = high_pos - low_pos - fb
+    zero_mask = int_bits + fb == 0
+    int_bits[zero_mask] = 0
+    fb[zero_mask] = 0
     return kn.astype(np.int8), int_bits.astype(np.int8), fb.astype(np.int8)
 
 
 class HGQ:
     """Heterogenous quantizer."""
 
     def __init__(self, init_bw: float, skip_dims, rnd_strategy: str | int = 'floor', exact_q_value=True, dtype=None, bw_clip=(-23, 23), trainable=True, regularizer: Callable | None = None, minmax_record=False):
@@ -241,30 +244,36 @@
         """Get exact int/frac/keep_negative bits of the equivalent fixed-point quantizer.
         Args:
             ref: Input tensor to compute the bits. If None, use the min/max record.
             pos_only: If True, only compute the bits for positive values. Useful if have a ReLU layer after.
         """
 
         if ref is None and self.minmax_record:
-            fp_bits = tf.round(self.fbw).numpy()  # type: ignore
+            assert tf.reduce_all(self._min <= self._max), "Some min values are larger than max values. Did you forget to run trace_minmax?"  # type: ignore
+            f = tf.round(self.fbw).numpy()  # type: ignore
             with np.errstate(divide='ignore'):
                 if pos_only:
                     _ref = np.maximum(self._max, 0.)  # type:ignore
-                    int_bits = np.floor(np.log2(_ref)) + 1
-                    kn = np.zeros_like(self._max)
+                    i = np.floor(np.log2(_ref)) + 1
+                    k = np.zeros_like(self._max)
                 else:
-                    int_bits = np.floor(np.log2(np.maximum(np.abs(self._max), np.abs(self._min)))) + 1  # type:ignore
-                    kn = (self._min.numpy() < 0)  # type:ignore
-            int_bits = np.clip(int_bits, -fp_bits - kn, 32)
-            return int_bits.astype(np.int8), fp_bits.astype(np.int8), kn.astype(np.int8)
+                    i_neg = np.ceil(np.log2(np.abs(self._min)))  # type:ignore
+                    i_pos = np.ceil(np.log2(np.abs(self._max + 2.**-f)))  # type:ignore
+                    i = np.maximum(i_neg, i_pos)
+                    k = (self._min.numpy() < 0)  # type:ignore
+            i = np.clip(i, -f - k, 32)
+            k, i, f = k.astype(np.int8), i.astype(np.int8), f.astype(np.int8)
+            mask = k + i + f != 0
+            return k * mask, i * mask, f * mask
 
         assert ref is not None
         w = self.forward(ref).numpy()  # type: ignore
         k, i, f = get_arr_bits(w)
-        return i, f, k
+        mask = k + i + f != 0
+        return k * mask, i * mask, f * mask
 
     def adapt_bw_bits(self, ref: tf.Tensor):
         """Adapt the bitwidth of the quantizer to the input tensor, such that each input is represented with approximately the same number of bits. (i.e., 1.5 with be represented by ap_fixed<2,1> and 0.375 will be represented by ap_fixed<2,-2>)."""
         if not self.built:
             self.build(tuple(ref.shape), name=None)
         new_fbw = self.fbw - (tf.math.log(tf.abs(ref)) / log2)
         if self.skip_dims:
```

### Comparing `HGQ-0.2.0rc1/src/HGQ/utils/utils.py` & `hgq-0.2.1/src/HGQ/utils/utils.py`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0rc1/src/HGQ.egg-info/PKG-INFO` & `hgq-0.2.1/src/HGQ.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HGQ
-Version: 0.2.0rc1
+Version: 0.2.1
 Summary: High Granularity Quantizarion
 Author-email: Chang Sun <chsun@cern.ch>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,15 +209,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tensorflow~=2.13
+Requires-Dist: tensorflow<2.16,>=2.13
 Requires-Dist: numpy>=1.23
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: qkeras; extra == "docs"
 Requires-Dist: pyparsing; extra == "docs"
@@ -236,18 +236,32 @@
 # High Granularity Quantization
 
 [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-green.svg)](LICENSE)
 [![Documentation](https://github.com/calad0i/HGQ/actions/workflows/sphinx-build.yml/badge.svg)](https://calad0i.github.io/HGQ/)
 [![PyPI version](https://badge.fury.io/py/hgq.svg)](https://badge.fury.io/py/hgq)
 
 
-HGQ is a framework for quantization aware training of neural networks to be deployed on FPGAs, which allows for per-weight and per-activation bitwidth optimization.
+HGQ is an gradient-based automatic bitwidth optimization and quantization-aware training algorithm for neural networks to be deployed on FPGAs, By laveraging gradients, it allows for bitwidth optimization at arbitrary granularity, up to per-weight and per-activation level.
 
-Depending on the specific [application](https://arxiv.org/abs/2006.10159), HGQ could achieve up to 10x resource reduction compared to the traditional `AutoQkeras` approach, while maintaining the same accuracy. For some more challenging [tasks](https://arxiv.org/abs/2202.04976), where the model is already under-fitted, HGQ could still improve the performance under the same on-board resource consumption. For more details, please refer to our paper (link coming not too soon).
+<img src="docs/_static/overview.svg" alt="HGQ-overview" width="600"/>
 
-This repository implements HGQ for `tensorflow.keras` models. It is independent of the [QKeras project](https://github.com/google/qkeras).
+Compare to the other heterogeneous quantization approach, like the QKeras counterpart, HGQ provides the following advantages:
 
-## Warning:
+- **High Granularity**: HGQ supports per-weight and per-activation bitwidth optimization, or any other lower granularity.
+- **Automatic Quantization**: By setting a resource regularization term, HGQ could automatically optimize the bitwidth of all parameters during training. Pruning is performed naturally when a bitwidth is reduced to 0.
+- **Bit-accurate conversion** to `hls4ml`: You get exactly what you get from `Keras` models from `hls4ml` models. HGQ provides a bit-accurate conversion interface, proxy models, for bit-accurate conversion to hls4ml models.
+  - still subject to machine float precision limitation.
+- **Accurate Resource Estimation**: BOPs estimated by HGQ is roughly #LUTs + 55#DSPs for actual (post place & route) FPGA resource consumption. This metric is available during training, and one can estimate the resource consumption of the final model in a very early stage.
 
-This framework requires an **unmerged** [PR](https://github.com/fastmachinelearning/hls4ml/pull/914) of hls4ml. Please install it by running `pip install "git+https://github.com/calad0i/hls4ml@HGQ-integration"`. Or, conversion will fail with unsupported layer error.
+Depending on the specific [application](https://arxiv.org/abs/2006.10159), HGQ could achieve up to 20x resource reduction compared to the `AutoQkeras` approach, while maintaining the same accuracy. For some more challenging [tasks](https://arxiv.org/abs/2202.04976), where the model is already under-fitted, HGQ could still improve the performance under the same on-board resource consumption. For more details, please refer to our paper (link coming soon).
 
-## This package is still under development. Any API might change without notice at any time!
+## Installation
+
+You will need `python>=3.10` and `tensorflow>=2.13` to run this framework. You can install it via pip:
+
+```bash
+pip install hgq
+```
+
+## Usage
+
+Please refer to the [documentation](https://calad0i.github.io/HGQ/) for more details.
```

### Comparing `HGQ-0.2.0rc1/src/HGQ.egg-info/SOURCES.txt` & `hgq-0.2.1/src/HGQ.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 docs/getting_started.md
 docs/index.rst
 docs/install.md
 docs/qkeras.md
 docs/reference.md
 docs/status.md
 docs/tips.md
+docs/_static/custom.css
 docs/_static/icon.svg
 docs/_static/logo-icon.svg
 docs/_static/logo.svg
+docs/_static/overview.svg
 examples/mnist.ipynb
 examples/qkeras.ipynb
 src/HGQ/__init__.py
 src/HGQ/_patch.py
 src/HGQ/_version.py
 src/HGQ.egg-info/PKG-INFO
 src/HGQ.egg-info/SOURCES.txt
@@ -37,14 +39,15 @@
 src/HGQ/layers/dense.py
 src/HGQ/layers/misc.py
 src/HGQ/layers/passive_layers.py
 src/HGQ/proxy/__init__.py
 src/HGQ/proxy/convert.py
 src/HGQ/proxy/fixed_point_quantizer.py
 src/HGQ/proxy/precision_derivation.py
+src/HGQ/proxy/unary_lut.py
 src/HGQ/proxy/plugins/__init__.py
 src/HGQ/proxy/plugins/qkeras.py
 src/HGQ/quantizer/__init__.py
 src/HGQ/quantizer/quantizer.py
 src/HGQ/utils/__init__.py
 src/HGQ/utils/utils.py
 test/helpers.py
```

### Comparing `HGQ-0.2.0rc1/test/helpers.py` & `hgq-0.2.1/test/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,15 @@
 
 
 def _run_model_sl_test(model: keras.Model, proxy: keras.Model, data, output_dir: str):
     model.save(output_dir + '/keras.h5')
     model_loaded: keras.Model = keras.models.load_model(output_dir + '/keras.h5')  # type: ignore
 
     proxy.save(output_dir + '/proxy.h5')
-    proxy_loaded: keras.Model = keras.models.load_model(output_dir + '/proxy.h5', custom_objects={'FixedPointQuantizer': FixedPointQuantizer})  # type: ignore
-
+    proxy_loaded: keras.Model = keras.models.load_model(output_dir + '/proxy.h5')  # type: ignore
     for l1, l2 in zip(proxy.layers, proxy_loaded.layers):
         if not isinstance(l1, FixedPointQuantizer):
             continue
         assert l1.overrides == l2.overrides, f"Overrides mismatch for layer {l1.name}"
 
     assert tf.reduce_all(model(data) == model_loaded(data)), f"Model premdiction mismatch"
     assert tf.reduce_all(proxy(data) == proxy_loaded(data)), f"Proxy prediction mismatch"
@@ -129,15 +128,15 @@
 
 def run_model_test(model: keras.Model, cover_factor: float | None, data, io_type: str, backend: str, dir: str, aggressive: bool, cond=None, skip_sl_test=False, test_gard=False):
     data_len = data.shape[0] if isinstance(data, np.ndarray) else data[0].shape[0]
     if test_gard:
         _run_gradient_test(model, data)
     if cover_factor is not None:
         trace_minmax(model, data, cover_factor=cover_factor, bsz=data_len)
-    proxy = to_proxy_model(model, aggressive=aggressive)
+    proxy = to_proxy_model(model, aggressive=aggressive, unary_lut_max_table_size=4096)
     try:
         if not skip_sl_test:
             _run_model_sl_test(model, proxy, data, dir)
         _run_model_proxy_match_test(model, proxy, data, cover_factor)
         _run_synth_match_test(proxy, data, io_type, backend, dir, cond=cond)
     except AssertionError as e:
         raise e
```

### Comparing `HGQ-0.2.0rc1/test/pytest.ini` & `hgq-0.2.1/test/pytest.ini`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0rc1/test/test_convert_manual_proxy.py` & `hgq-0.2.1/test/test_convert_manual_proxy.py`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0rc1/test/test_end2end_tiny.py` & `hgq-0.2.1/test/test_end2end_tiny.py`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0rc1/test/test_syn_hlayers.py` & `hgq-0.2.1/test/test_syn_hlayers.py`

 * *Files 13% similar despite different names*

```diff
@@ -53,15 +53,19 @@
     a1 = rng.normal(0, sigma, (N, 16)).astype(np.float32)
     a2 = rng.uniform(0, max_scale, (1, 16)).astype(np.float32)
     return (a1 * a2).astype(np.float32)
 
 
 def softmax_cond(proxy, hls):
     match_precent = np.mean(np.argmax(proxy, axis=1) == np.argmax(hls, axis=1))
-    assert match_precent > 0.90, f"Keras-Proxy mismatch: {(1-match_precent) * 100}% of samples are different. Sample: {proxy[:5]} vs {hls[:5]}"
+    assert match_precent > 0.90, f"Proxy-HLS4ML mismatch: {(1-match_precent) * 100}% of samples are different. Sample: {proxy[:5]} vs {hls[:5]}"
+
+
+def custom_fn(x):
+    return tf.sin(x)**2. - x  # type: ignore
 
 
 @pytest.mark.parametrize('layer',
                          ["HDense(10)",
                           "HDense(10, use_bias=False)",
                           "HDenseBatchNorm(10)",
                           "HConv1D(2, 3, padding='same')",
@@ -75,41 +79,47 @@
                           "HConv2D(2, (3,3), padding='valid', use_bias=False)",
                           "HConv2D(2, (3,3), padding='valid', strides=2)",
                           "HConv2D(2, (3,3), padding='same', strides=2)",
                           "HConv2DBatchNorm(2, (3,3), padding='valid')",
                           "HAdd()",
                           "HActivation('relu')",
                           #   "HActivation('leaky_relu')",
-                          "HActivation('relu6')",
                           "HActivation('tanh')",
                           "HActivation('sigmoid')",
                           "HActivation('softmax')",
+                          "HActivation(custom_fn)",
                           ]
                          )
 @pytest.mark.parametrize("N", [1000])
 @pytest.mark.parametrize("rnd_strategy", ['auto', 'standard_round', 'floor'])
 @pytest.mark.parametrize("io_type", ['io_parallel', 'io_stream'])
-@pytest.mark.parametrize("cover_factor", [0.5, 1.0])
+@pytest.mark.parametrize("cover_factor", [0.25, 1.0])
 @pytest.mark.parametrize("aggressive", [True, False])
-@pytest.mark.parametrize("backend", ['vivado'])
+@pytest.mark.parametrize("backend", ['vivado', 'vitis'])
 @pytest.mark.parametrize("seed", [42])
 def test_syn_hlayers(layer, N: int, rnd_strategy: str, io_type: str, cover_factor: float, aggressive: bool, backend: str, seed: int):
     dir = get_test_dir()
     set_seed(seed)
     model = create_model(layer=layer, rnd_strategy=rnd_strategy, io_type=io_type)
     data = get_data(N, 1, 1, seed)
 
     test_grad = N > 100
-    cond = None if 'softmax' not in layer else softmax_cond
+    cond = None
+    if 'softmax' in layer:
+        cond = softmax_cond
+        cover_factor = max(cover_factor, 0.5)  # Softmax table size is sensitive to range
+
+    skip_sl_test = 'custom' in layer
     run_model_test(model,
                    cover_factor, data,
                    io_type,
                    backend,
                    dir,
                    aggressive,
                    test_gard=test_grad,
-                   cond=cond
+                   cond=cond,
+                   skip_sl_test=skip_sl_test,
                    )
 
 
 if __name__ == '__main__':
     test_syn_hlayers('HActivation("tanh")', 10, 'floor', 'io_parallel', 0.5, True, 'vivado', 42)
```

### Comparing `HGQ-0.2.0rc1/test/test_syn_large.py` & `hgq-0.2.1/test/test_syn_large.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,17 +64,17 @@
     a2 = rng.uniform(0, max_scale, (1, 10, 10, 1)).astype(np.float32)
     return (a1 * a2).astype(np.float32)
 
 
 @pytest.mark.parametrize("N", [50000, 10])
 @pytest.mark.parametrize("rnd_strategy", ['auto'])
 @pytest.mark.parametrize("io_type", ['io_parallel', 'io_stream'])
-@pytest.mark.parametrize("cover_factor", [0.49, 1.0])
+@pytest.mark.parametrize("cover_factor", [0.25, 1.0])
 @pytest.mark.parametrize("aggressive", [True, False])
-@pytest.mark.parametrize("backend", ['vivado'])  # , 'vitis'])
+@pytest.mark.parametrize("backend", ['vivado', 'vitis'])
 @pytest.mark.parametrize("seed", [42])
 def test_syn_large(N: int, rnd_strategy: str, io_type: str, cover_factor: float, aggressive: bool, backend: str, seed: int):
     dir = get_test_dir()
     set_seed(seed)
     model = create_model(rnd_strategy=rnd_strategy, io_type=io_type)
     data = get_data(N, 8, 1, seed)
```

### Comparing `HGQ-0.2.0rc1/test/test_syn_players.py` & `hgq-0.2.1/test/test_syn_players.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,105 +12,97 @@
 
 def create_model(layer: str, rnd_strategy: str, io_type: str):
     pa_config = get_default_paq_conf()
     pa_config['rnd_strategy'] = rnd_strategy
     pa_config['skip_dims'] = 'all' if io_type == 'io_stream' else 'batch'
     set_default_paq_conf(pa_config)
 
-    inp = keras.Input(shape=(16))
+    inp = keras.Input(shape=(15))
     if 'PConcatenate' in layer:
         _inp = [HQuantize()(inp)] * 2
         out = eval(layer)(_inp)
-        out = HDense(16)(out)
+        out = HDense(15)(out)
         return keras.Model(inp, out)
     elif 'Signature' in layer:
         _inp = eval(layer)(inp)
-        out = HDense(16)(_inp)
+        out = HDense(15)(_inp)
         return keras.Model(inp, out)
     elif 'Pool2D' in layer:
-        _inp = PReshape((4, 4, 1))(HQuantize()(inp))
+        _inp = PReshape((3, 5, 1))(HQuantize()(inp))
     elif 'Pool1D' in layer:
-        _inp = PReshape((16, 1))(HQuantize()(inp))
+        _inp = PReshape((5, 3))(HQuantize()(inp))
     elif 'Dense' in layer or 'Activation' in layer:
         _inp = HQuantize()(inp)
     elif 'Flatten' in layer:
         out = HQuantize()(inp)
-        out = PReshape((4, 4))(out)
+        out = PReshape((3, 5))(out)
         out = HConv1D(2, 2)(out)
         out = eval(layer)(out)
-        out = HDense(16)(out)
+        out = HDense(15)(out)
         return keras.Model(inp, out)
     else:
         raise Exception(f'Please add test for {layer}')
 
     out = eval(layer)(_inp)
+    if 'maxpool' in layer.lower():
+        out = HQuantize()(out)
     model = keras.Model(inp, out)
 
     for layer in model.layers:
         # No weight bitwidths to randomize
         # And activation bitwidths
         if hasattr(layer, 'paq'):
             fbw: tf.Variable = layer.paq.fbw
             fbw.assign(tf.constant(np.random.uniform(4, 8, fbw.shape).astype(np.float32)))
 
     return model
 
 
 def get_data(N: int, sigma: float, max_scale: float, seed):
     rng = np.random.default_rng(seed)
-    a1 = rng.normal(0, sigma, (N, 16)).astype(np.float32)
-    a2 = rng.uniform(0, max_scale, (1, 16)).astype(np.float32)
+    a1 = rng.normal(0, sigma, (N, 15)).astype(np.float32)
+    a2 = rng.uniform(0, max_scale, (1, 15)).astype(np.float32)
     return (a1 * a2).astype(np.float32)
 
 
-def parallel_avg_pool_cond(a, b):
-    close: np.ndarray = np.abs(a - b) < 1e-2
-
-    assert np.all(close), f"Keras-Proxy mismatch for approx avg pool: {np.sum(np.any(~close, axis=tuple(range(1,close.ndim))))} out of {a.shape[0]} samples are very different. Sample: {a[~close].ravel()[:5]} vs {b[~close].ravel()[:5]}"
-
-
 @pytest.mark.parametrize('layer',
                          [
                              "PConcatenate()",
                              "PMaxPool1D(2, padding='same')",
-                             "PMaxPool2D((2,2), padding='same')",
+                             "PMaxPool1D(4, padding='same')",
+                             "PMaxPool2D((5,3), padding='same')",
                              "PMaxPool1D(2, padding='valid')",
-                             "PMaxPool2D((2,2), padding='valid')",
+                             "PMaxPool2D((2,3), padding='valid')",
                              "Signature(1,6,3)",
                              "PAvgPool1D(2, padding='same')",
                              "PAvgPool2D((1,2), padding='same')",
                              "PAvgPool2D((2,2), padding='same')",
                              "PAvgPool1D(2, padding='valid')",
                              "PAvgPool2D((1,2), padding='valid')",
                              "PAvgPool2D((2,2), padding='valid')",
                              "PFlatten()",
                          ]
                          )
 @pytest.mark.parametrize("N", [1000])
 @pytest.mark.parametrize("rnd_strategy", ['auto', 'standard_round', 'floor'])
 @pytest.mark.parametrize("io_type", ['io_parallel', 'io_stream'])
-@pytest.mark.parametrize("cover_factor", [0.5, 1.0])
+@pytest.mark.parametrize("cover_factor", [0.25, 1.0])
 @pytest.mark.parametrize("aggressive", [True, False])
-@pytest.mark.parametrize("backend", ['vivado'])
+@pytest.mark.parametrize("backend", ['vivado', 'vitis'])
 @pytest.mark.parametrize("seed", [42])
 def test_syn_players(layer, N: int, rnd_strategy: str, io_type: str, cover_factor: float, aggressive: bool, backend: str, seed: int):
     dir = get_test_dir()
     set_seed(seed)
     model = create_model(layer=layer, rnd_strategy=rnd_strategy, io_type=io_type)
     data = get_data(N, 1, 1, seed)
 
     if 'Signature' in layer:
         q = gfixed(1, 6, 3)
         data = q(data).numpy()
+    if "padding='same'" in layer and io_type == 'io_stream':
+        pytest.skip("io_stream does not support padding='same' for pools at the moment")
 
-    cond = None
-    if 'AvgPool' in layer and io_type == 'io_parallel':
-        if cover_factor < 1.0:
-            # pass
-            pytest.skip('AvgPool\'s accum is not configurable for io_parallel, and cover_factor < 1.0 leads to overflow cannot be emulated')
-        cond = parallel_avg_pool_cond
-        # mark as xfail if io_parallel and cover_factor < 1.0
-    run_model_test(model, cover_factor, data, io_type, backend, dir, aggressive, cond=cond)
+    run_model_test(model, cover_factor, data, io_type, backend, dir, aggressive)
 
 
 if __name__ == '__main__':
     test_syn_players('PFlatten()', 10, 'floor', 'io_parallel', 0.5, True, 'vivado', 42)
```

### Comparing `HGQ-0.2.0rc1/test/test_syn_qkeras.py` & `hgq-0.2.1/test/test_syn_qkeras.py`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0rc1/test/test_syn_small.py` & `hgq-0.2.1/test/test_syn_small.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     a2 = rng.uniform(0, max_scale, (1, 6, 6, 1)).astype(np.float32)
     return (a1 * a2).astype(np.float32)
 
 
 @pytest.mark.parametrize("N", [50000, 10])
 @pytest.mark.parametrize("rnd_strategy", ['auto', 'standard_round', 'floor'])
 @pytest.mark.parametrize("io_type", ['io_parallel', 'io_stream'])
-@pytest.mark.parametrize("cover_factor", [0.49, 1.0])
+@pytest.mark.parametrize("cover_factor", [0.25, 1.0])
 @pytest.mark.parametrize("aggressive", [True, False])
 @pytest.mark.parametrize("backend", ['vivado', 'vitis'])
 @pytest.mark.parametrize("seed", [114514, 42, 1919810])
 def test_syn_small(N: int, rnd_strategy: str, io_type: str, cover_factor: float, aggressive: bool, backend: str, seed: int):
     dir = get_test_dir()
     set_seed(seed)
     model = create_model(rnd_strategy=rnd_strategy, io_type=io_type)
```

