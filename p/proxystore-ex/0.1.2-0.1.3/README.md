# Comparing `tmp/proxystore-ex-0.1.2.tar.gz` & `tmp/proxystore_ex-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxystore-ex-0.1.2.tar", last modified: Fri Dec 15 19:14:17 2023, max compression
+gzip compressed data, was "proxystore_ex-0.1.3.tar", last modified: Fri Apr 26 13:55:23 2024, max compression
```

## Comparing `proxystore-ex-0.1.2.tar` & `proxystore_ex-0.1.3.tar`

### file list

```diff
@@ -1,107 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.154243 proxystore-ex-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.142243 proxystore-ex-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.142243 proxystore-ex-0.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/.github/ISSUE_TEMPLATE/01_bug.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/.github/ISSUE_TEMPLATE/02_enhancement.yml
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/.github/ISSUE_TEMPLATE/03_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.142243 proxystore-ex-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/.github/workflows/cache.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/.github/workflows/check-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      918 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/.github/workflows/integration.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      793 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2023-12-15 19:14:17.154243 proxystore-ex-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.142243 proxystore-ex-0.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.142243 proxystore-ex-0.1.2/docs/_overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/_overrides/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.138243 proxystore-ex-0.1.2/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.138243 proxystore-ex-0.1.2/docs/_templates/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.142243 proxystore-ex-0.1.2/docs/_templates/python/material/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.142243 proxystore-ex-0.1.2/docs/_templates/python/material/docstring/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/_templates/python/material/docstring/admonition.html
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/_templates/python/material/function.html
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/_templates/python/material/module.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.142243 proxystore-ex-0.1.2/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/contributing/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/contributing/issues-pull-requests.md
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/contributing/releases.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/contributing/style-guide.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.146243 proxystore-ex-0.1.2/docs/css/
--rw-r--r--   0 runner    (1001) docker     (127)      557 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)    94526 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/css/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/css/mkdocstrings.css
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/generate_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.146243 proxystore-ex-0.1.2/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/guides/daos.md
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/guides/dask-distributed.md
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/guides/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/known-issues.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.146243 proxystore-ex-0.1.2/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)    46990 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)    45464 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/docs/static/icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.146243 proxystore-ex-0.1.2/proxystore_ex/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/proxystore_ex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.146243 proxystore-ex-0.1.2/proxystore_ex/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/proxystore_ex/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/proxystore_ex/connectors/daos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.146243 proxystore-ex-0.1.2/proxystore_ex/connectors/dim/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/proxystore_ex/connectors/dim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/proxystore_ex/connectors/dim/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19451 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/proxystore_ex/connectors/dim/margo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/proxystore_ex/connectors/dim/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    18580 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/proxystore_ex/connectors/dim/ucx.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/proxystore_ex/connectors/dim/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17506 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/proxystore_ex/connectors/dim/zmq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.150243 proxystore-ex-0.1.2/proxystore_ex/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/proxystore_ex/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19304 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/proxystore_ex/plugins/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/proxystore_ex/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.150243 proxystore-ex-0.1.2/proxystore_ex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2023-12-15 19:14:17.000000 proxystore-ex-0.1.2/proxystore_ex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2023-12-15 19:14:17.000000 proxystore-ex-0.1.2/proxystore_ex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 19:14:17.000000 proxystore-ex-0.1.2/proxystore_ex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-12-15 19:14:17.000000 proxystore-ex-0.1.2/proxystore_ex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-15 19:14:17.000000 proxystore-ex-0.1.2/proxystore_ex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-15 19:14:17.154243 proxystore-ex-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.150243 proxystore-ex-0.1.2/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/testing/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/testing/connectors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.150243 proxystore-ex-0.1.2/testing/mocked/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/testing/mocked/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/testing/mocked/pydaos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/testing/mocked/pymargo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/testing/mocked/ucp.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/testing/mocking.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.150243 proxystore-ex-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.150243 proxystore-ex-0.1.2/tests/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/tests/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/tests/connectors/connectors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/tests/connectors/daos_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.150243 proxystore-ex-0.1.2/tests/connectors/dim/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/tests/connectors/dim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7044 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/tests/connectors/dim/margo_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/tests/connectors/dim/ucx_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/tests/connectors/dim/zmq_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/tests/import_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:17.150243 proxystore-ex-0.1.2/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/tests/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/tests/plugins/distributed_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2023-12-15 19:14:07.000000 proxystore-ex-0.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.071875 proxystore_ex-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.055875 proxystore_ex-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.055875 proxystore_ex-0.1.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/.github/ISSUE_TEMPLATE/01_bug.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/.github/ISSUE_TEMPLATE/02_enhancement.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/.github/ISSUE_TEMPLATE/03_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.055875 proxystore_ex-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/.github/workflows/cache.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/.github/workflows/check-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/.github/workflows/integration.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-04-26 13:55:23.067875 proxystore_ex-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.055875 proxystore_ex-0.1.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.055875 proxystore_ex-0.1.3/docs/_overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/_overrides/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.051875 proxystore_ex-0.1.3/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.051875 proxystore_ex-0.1.3/docs/_templates/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.059875 proxystore_ex-0.1.3/docs/_templates/python/material/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.059875 proxystore_ex-0.1.3/docs/_templates/python/material/docstring/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/_templates/python/material/docstring/admonition.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/_templates/python/material/function.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/_templates/python/material/module.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.059875 proxystore_ex-0.1.3/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/contributing/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/contributing/issues-pull-requests.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/contributing/releases.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/contributing/style-guide.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.059875 proxystore_ex-0.1.3/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)    94526 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/css/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/generate_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.059875 proxystore_ex-0.1.3/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/guides/daos.md
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/guides/dask-distributed.md
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/guides/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.059875 proxystore_ex-0.1.3/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    46990 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45464 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/docs/static/icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.059875 proxystore_ex-0.1.3/proxystore_ex/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/proxystore_ex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.063875 proxystore_ex-0.1.3/proxystore_ex/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/proxystore_ex/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/proxystore_ex/connectors/daos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.063875 proxystore_ex-0.1.3/proxystore_ex/connectors/dim/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/proxystore_ex/connectors/dim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/proxystore_ex/connectors/dim/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19452 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/proxystore_ex/connectors/dim/margo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/proxystore_ex/connectors/dim/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18581 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/proxystore_ex/connectors/dim/ucx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/proxystore_ex/connectors/dim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17507 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/proxystore_ex/connectors/dim/zmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.063875 proxystore_ex-0.1.3/proxystore_ex/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/proxystore_ex/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18855 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/proxystore_ex/plugins/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/proxystore_ex/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.067875 proxystore_ex-0.1.3/proxystore_ex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-04-26 13:55:23.000000 proxystore_ex-0.1.3/proxystore_ex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-26 13:55:23.000000 proxystore_ex-0.1.3/proxystore_ex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:55:23.000000 proxystore_ex-0.1.3/proxystore_ex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-26 13:55:23.000000 proxystore_ex-0.1.3/proxystore_ex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 13:55:23.000000 proxystore_ex-0.1.3/proxystore_ex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 13:55:23.071875 proxystore_ex-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.063875 proxystore_ex-0.1.3/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/testing/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/testing/connectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.063875 proxystore_ex-0.1.3/testing/mocked/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/testing/mocked/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/testing/mocked/pydaos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/testing/mocked/pymargo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/testing/mocked/ucp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/testing/mocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.067875 proxystore_ex-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.067875 proxystore_ex-0.1.3/tests/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/tests/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/tests/connectors/connectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/tests/connectors/daos_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.067875 proxystore_ex-0.1.3/tests/connectors/dim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/tests/connectors/dim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/tests/connectors/dim/margo_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/tests/connectors/dim/ucx_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/tests/connectors/dim/zmq_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/tests/import_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:23.067875 proxystore_ex-0.1.3/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/tests/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/tests/plugins/distributed_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-26 13:55:18.000000 proxystore_ex-0.1.3/tox.ini
```

### Comparing `proxystore-ex-0.1.2/.github/ISSUE_TEMPLATE/01_bug.yml` & `proxystore_ex-0.1.3/.github/ISSUE_TEMPLATE/01_bug.yml`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/.github/ISSUE_TEMPLATE/02_enhancement.yml` & `proxystore_ex-0.1.3/.github/ISSUE_TEMPLATE/02_enhancement.yml`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/.github/pull_request_template.md` & `proxystore_ex-0.1.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/.github/release.yml` & `proxystore_ex-0.1.3/.github/release.yml`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/.github/workflows/cache.yml` & `proxystore_ex-0.1.3/.github/workflows/cache.yml`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/.github/workflows/check-docs.yml` & `proxystore_ex-0.1.3/.github/workflows/check-docs.yml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
       - name: Get pip cache dir
         id: pip-cache-dir
         run: echo "PIP_CACHE_DIR=$(pip cache dir)" >> $GITHUB_ENV
 
       - name: Use pip cache
         id: pip-cache
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           path: ${{ env.PIP_CACHE_DIR }}
           key: docs-ubuntu-latest-pip-3.11-${{ hashFiles('pyproject.toml') }}
           restore-keys: |
             docs-ubuntu-latest-pip-3.11-
 
       - name: Install Packages
```

### Comparing `proxystore-ex-0.1.2/.github/workflows/docs.yml` & `proxystore_ex-0.1.3/.github/workflows/docs.yml`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
       - name: Get pip cache dir
         id: pip-cache-dir
         run: echo "PIP_CACHE_DIR=$(pip cache dir)" >> $GITHUB_ENV
 
       - name: Use pip cache
         id: pip-cache
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           path: ${{ env.PIP_CACHE_DIR }}
           key: docs-ubuntu-latest-pip-3.11-${{ hashFiles('pyproject.toml') }}
           restore-keys: |
             docs-ubuntu-latest-pip-3.11-
 
       - name: Install Packages
@@ -42,8 +42,8 @@
 
       - name: Configure git
         run: |
           git config --local user.name "GitHub Actions Bot"
           git config --local user.email "41898282+github-actions[bot]@users.noreply.github.com"
       - name: Deploy docs for main:latest to gh-pages branch
         run: |
-          mike deploy --push --update-aliases main latest
+          mike deploy --push --update-aliases main
```

### Comparing `proxystore-ex-0.1.2/.github/workflows/integration.yml` & `proxystore_ex-0.1.3/.github/workflows/integration.yml`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/.github/workflows/publish.yml` & `proxystore_ex-0.1.3/.github/workflows/publish.yml`

 * *Files 6% similar despite different names*

```diff
@@ -55,8 +55,8 @@
         run: |
           git config --local user.name "GitHub Actions Bot"
           git config --local user.email "41898282+github-actions[bot]@users.noreply.github.com"
       - name: Deploy docs for release version to gh-pages branch
         if: startsWith(github.ref, 'refs/tags/')
         run: |
           pip install .[docs]
-          mike deploy --push "${{ env.PACKAGE_VERSION }}"
+          mike deploy --push --update-aliases "${{ env.PACKAGE_VERSION }}" latest
```

### Comparing `proxystore-ex-0.1.2/.github/workflows/tests.yml` & `proxystore_ex-0.1.3/.github/workflows/tests.yml`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
       - name: Get pip cache dir
         id: pip-cache-dir
         run: echo "PIP_CACHE_DIR=$(pip cache dir)" >> $GITHUB_ENV
 
       - name: Use pip cache
         id: pip-cache
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           path: ${{ env.PIP_CACHE_DIR }}
           key: tests-${{ matrix.os }}-pip-${{ matrix.python }}-${{ hashFiles('pyproject.toml') }}
           restore-keys: |
             tests-${{ matrix.os }}-pip-${{ matrix.python }}-
 
       - name: Install Packages
```

### Comparing `proxystore-ex-0.1.2/.gitignore` & `proxystore_ex-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/.pre-commit-config.yaml` & `proxystore_ex-0.1.3/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 ci:
   autofix_prs: false
 repos:
   - repo: 'https://github.com/pre-commit/pre-commit-hooks'
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: mixed-line-ending
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-added-large-files
       - id: check-docstring-first
       - id: check-json
       - id: check-yaml
       - id: check-merge-conflict
       - id: name-tests-test
   - repo: 'https://github.com/codespell-project/codespell'
     rev: v2.2.6
     hooks:
       - id: codespell
-  - repo: 'https://github.com/charliermarsh/ruff-pre-commit'
-    rev: v0.1.7
+  - repo: 'https://github.com/astral-sh/ruff-pre-commit'
+    rev: v0.4.1
     hooks:
       - id: ruff
         args:
           - '--fix'
       - id: ruff-format
   - repo: 'https://github.com/pre-commit/mirrors-mypy'
-    rev: v1.7.1
+    rev: v1.9.0
     hooks:
       - id: mypy
-        additional_dependencies: []
+        additional_dependencies:
+          - dask[distributed]
+          - proxystore >= 0.6.5
+          - pyzmq
```

### Comparing `proxystore-ex-0.1.2/LICENSE` & `proxystore_ex-0.1.3/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023-Present Globus Labs
+Copyright (c) 2023-2024 Greg Pauloski and Globus Labs
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `proxystore-ex-0.1.2/PKG-INFO` & `proxystore_ex-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,66 @@
 Metadata-Version: 2.1
 Name: proxystore-ex
-Version: 0.1.2
+Version: 0.1.3
 Summary: ProxyStore extensions.
 Author: Globus Labs
 Author-email: Greg Pauloski <jgpauloski@uchicago.edu>
 Maintainer-email: Greg Pauloski <jgpauloski@uchicago.edu>, Valerie Hayot-Sasson <vhayot@uchicago.edu>
 License: MIT
-Project-URL: homepage, https://proxystore.dev
-Project-URL: documentation, https://extensions.proxystore.dev
-Project-URL: repository, https://github.com/proxystore/extensions
+Project-URL: Homepage, https://proxystore.dev
+Project-URL: Documentation, https://extensions.proxystore.dev
+Project-URL: Source, https://github.com/proxystore/extensions
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: proxystore>=0.5.0
+Requires-Dist: proxystore>=0.6.5
 Requires-Dist: pyzmq
 Provides-Extra: dev
 Requires-Dist: covdefaults>=2.2; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: dask; extra == "dev"
 Requires-Dist: distributed; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio>=0.23.2; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
+Requires-Dist: ruff>=0.2.0; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: virtualenv; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: black; extra == "docs"
 Requires-Dist: mkdocs-gen-files; extra == "docs"
 Requires-Dist: mkdocs-literate-nav; extra == "docs"
-Requires-Dist: mkdocs-material!=9.4.0; extra == "docs"
+Requires-Dist: mkdocs-material==9.4.7; extra == "docs"
 Requires-Dist: mkdocs-section-index; extra == "docs"
-Requires-Dist: mkdocstrings[python]; extra == "docs"
+Requires-Dist: mkdocstrings==0.23.0; extra == "docs"
+Requires-Dist: mkdocstrings-python==1.8.0; extra == "docs"
 Requires-Dist: mike; extra == "docs"
 
 # ProxyStore Extensions
 
+![PyPI - Version](https://img.shields.io/pypi/v/proxystore-ex)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/proxystore-ex)
+![GitHub License](https://img.shields.io/github/license/proxystore/extensions)
+
 [![docs](https://github.com/proxystore/extensions/actions/workflows/docs.yml/badge.svg)](https://github.com/proxystore/extensions/actions)
 [![tests](https://github.com/proxystore/extensions/actions/workflows/tests.yml/badge.svg)](https://github.com/proxystore/extensions/actions)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/proxystore/extensions/main.svg)](https://results.pre-commit.ci/latest/github/proxystore/extensions/main)
 
-Extensions for the [ProxyStore](https://github.com/proxystore/proxystore/).
+Extensions for the [ProxyStore](https://github.com/proxystore/proxystore/) package.
 
 This extensions package contains experimental features, features with
 non-Python dependencies, and plugins for third-party tools.
 
 ## Installation
 
 The extensions package can be installed alongside
@@ -80,7 +89,11 @@
 `proxystore` via the [`proxystore.ex`](https://docs.proxystore.dev/latest/api/ex/)
 module. This is the recommended method for import extension features. E.g.,
 
 ```python
 from proxystore_ex.connectors.daos import DAOSConnector  # Direct
 from proxystore.ex.connectors.daos import DAOSConnector  # Recommended
 ```
+
+## Citation
+
+The preferred citations for this code are provided at https://docs.proxystore.dev/latest/publications/.
```

### Comparing `proxystore-ex-0.1.2/README.md` & `proxystore_ex-0.1.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # ProxyStore Extensions
 
+![PyPI - Version](https://img.shields.io/pypi/v/proxystore-ex)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/proxystore-ex)
+![GitHub License](https://img.shields.io/github/license/proxystore/extensions)
+
 [![docs](https://github.com/proxystore/extensions/actions/workflows/docs.yml/badge.svg)](https://github.com/proxystore/extensions/actions)
 [![tests](https://github.com/proxystore/extensions/actions/workflows/tests.yml/badge.svg)](https://github.com/proxystore/extensions/actions)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/proxystore/extensions/main.svg)](https://results.pre-commit.ci/latest/github/proxystore/extensions/main)
 
-Extensions for the [ProxyStore](https://github.com/proxystore/proxystore/).
+Extensions for the [ProxyStore](https://github.com/proxystore/proxystore/) package.
 
 This extensions package contains experimental features, features with
 non-Python dependencies, and plugins for third-party tools.
 
 ## Installation
 
 The extensions package can be installed alongside
@@ -37,7 +41,11 @@
 `proxystore` via the [`proxystore.ex`](https://docs.proxystore.dev/latest/api/ex/)
 module. This is the recommended method for import extension features. E.g.,
 
 ```python
 from proxystore_ex.connectors.daos import DAOSConnector  # Direct
 from proxystore.ex.connectors.daos import DAOSConnector  # Recommended
 ```
+
+## Citation
+
+The preferred citations for this code are provided at https://docs.proxystore.dev/latest/publications/.
```

### Comparing `proxystore-ex-0.1.2/docs/_templates/python/material/function.html` & `proxystore_ex-0.1.3/docs/_templates/python/material/function.html`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/docs/_templates/python/material/module.html` & `proxystore_ex-0.1.3/docs/_templates/python/material/module.html`

 * *Files 11% similar despite different names*

```diff
@@ -44,15 +44,15 @@
           hidden=True) %}
       {% endfilter %}
     {% endif %}
     {% set heading_level = heading_level - 1 %}
   {% endif %}
 
   <div class="doc doc-contents">
-      <a target="_blank" href="https://github.com/proxystore/proxystore/blob/main/{{ module.filepath }}"><code>{{ module.filepath }}</code></a>
+    <a target="_blank" href="https://github.com/proxystore/extensions/blob/main/{{ module.relative_package_filepath }}"><code>{{ module.relative_package_filepath }}</code></a>
   </div>
 
   <div class="doc doc-contents {% if root %}first{% endif %}">
     {% with docstring_sections = module.docstring.parsed %}
       {% include "docstring.html" with context %}
     {% endwith %}
```

### Comparing `proxystore-ex-0.1.2/docs/contributing/index.md` & `proxystore_ex-0.1.3/docs/contributing/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 to setup the development environment. This will create a new virtual
 environment with all of the required packages installed
 and ProxyStore installed in editable mode with the necessary extras options.
 
 ```bash
 $ git clone https://github.com/proxystore/extensions
 $ cd extensions
-$ tox --devenv venv -e py310
+$ tox --devenv venv -e py311
 $ . venv/bin/activate
 ```
 
 !!! warning
 
     Running Tox in a Conda environment is possible but it may conflict with
     Tox's ability to find the correct Python versions. E.g., if your
@@ -45,29 +45,29 @@
 
 ### Tests (tox)
 
 The entire CI workflow can be run with `#!bash $ tox`.
 This will test against multiple versions of Python and can be slow.
 
 Module-level unit-test are located in the `tests/` directory and its
-structure is intended to match that of `proxystore_extensions/`.
-E.g. the tests for `proxystore_extenions/x/y.py` are located in
+structure is intended to match that of `proxystore_ex/`.
+E.g. the tests for `proxystore_ex/x/y.py` are located in
 `tests/x/y_test.py`; however, additional test files can be added
 as needed. Tests should be narrowly focused and target a single aspect of the
 code's functionality, tests should not test internal implementation details of
 the code, and tests should not be dependent on the order in which they are run.
 
 Code that is useful for building tests but is not a test itself belongs in the
 `testing/` directory.
 
 ```bash
 # Run all tests in tests/
-$ tox -e py39
+$ tox -e py311
 # Run a specific test
-$ tox -e py39 -- tests/x/y_test.py::test_z
+$ tox -e py311 -- tests/x/y_test.py::test_z
 ```
 
 ### Tests (docker)
 
 The test suite mocks certain third-party programs that cannot be installed via
 pip (e.g., Margo, UCX, Redis). For Margo and UCX, a Docker image is provided
 at
@@ -77,15 +77,15 @@
 the un-mocked software.
 
 ```bash
 $ docker pull ghcr.io/proxystore/proxystore-dim:nightly
 # Be sure to change the path to your proxystore repo directory
 $ docker run --rm -it --network host -v /path/to/proxystore:/proxystore ghcr.io/proxystore/proxystore-dim:nightly
 # Inside container
-$ tox -e py310-dim
+$ tox -e py311-dim
 ```
 
 ## Docs
 
 If code changes require an update to the documentation (e.g., for function
 signature changes, new modules, etc.), the documentation can be built using
 MKDocs.
```

### Comparing `proxystore-ex-0.1.2/docs/contributing/issues-pull-requests.md` & `proxystore_ex-0.1.3/docs/contributing/issues-pull-requests.md`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,16 @@
         * limit subject line to 50 characters,
         * capitalize first word of subject line,
         * do not end the subject line with a period,
         * use the imperative mood for subject lines,
         * include related issue numbers at end of subject line,
         * wrap body at 72 characters, and
         * use the body to explain what/why rather than how.
-      Example: `Fix concurrency bug in Store (#42)`
+        * *Example*: `Fix concurrency bug in Store (#42)`
+
 3. Push commits to your fork.
     - Please squash commits fixing mistakes to keep the git history clean.
       For example, if commit "b" follows commit "a" and only fixes a small typo
       from "a", please squash "a" and "b" into a single, correct commit.
       This keeps the commit history readable and easier to search through when
       debugging (e.g., git blame/bisect).
 4. Open a pull request in this repository.
```

### Comparing `proxystore-ex-0.1.2/docs/contributing/releases.md` & `proxystore_ex-0.1.3/docs/contributing/releases.md`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/docs/css/extra.css` & `proxystore_ex-0.1.3/docs/css/extra.css`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/docs/css/favicon.png` & `proxystore_ex-0.1.3/docs/css/favicon.png`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/docs/css/mkdocstrings.css` & `proxystore_ex-0.1.3/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/docs/generate_api.py` & `proxystore_ex-0.1.3/docs/generate_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Generate the code reference pages and navigation."""
+
 from __future__ import annotations
 
 from pathlib import Path
 
 import mkdocs_gen_files
 
 PACKAGE = 'proxystore_ex'
```

### Comparing `proxystore-ex-0.1.2/docs/guides/daos.md` & `proxystore_ex-0.1.3/docs/guides/daos.md`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/docs/installation.md` & `proxystore_ex-0.1.3/docs/installation.md`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/docs/static/favicon.png` & `proxystore_ex-0.1.3/docs/static/favicon.png`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/docs/static/icon.png` & `proxystore_ex-0.1.3/docs/static/icon.png`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/mkdocs.yml` & `proxystore_ex-0.1.3/mkdocs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -103,29 +103,32 @@
   - pymdownx.tasklist:
       custom_checkbox: true
 
 nav:
   - Home:
       - Overview: index.md
       - Installation: installation.md
-      - Known Issues: known-issues.md
+      - Issues (GitHub): https://github.com/proxystore/issues
       - Changelog (GitHub): https://github.com/proxystore/extensions/releases
   - Guides:
       - guides/index.md
       - DAOS at ALCF: guides/daos.md
       - Dask with ProxyStore: guides/dask-distributed.md
   - API Reference:
       - ProxyStore Extensions: api/
   - Contributing:
       - contributing/index.md
       - Style Guide: contributing/style-guide.md
       - Issues and Pull Requests: contributing/issues-pull-requests.md
       - Releases: contributing/releases.md
 
 plugins:
+  - mike:
+      alias_type: symlink
+      canonical_version: latest
   - gen-files:
       scripts:
         - docs/generate_api.py
   - literate-nav:
       nav_file: SUMMARY.md
   - mkdocstrings:
       custom_templates: docs/_templates
@@ -136,19 +139,23 @@
             - import pytkdocs_tweaks
             - pytkdocs_tweaks.main()
           import:
             - https://docs.python.org/3/objects.inv
             - https://docs.proxystore.dev/main/objects.inv
             - https://distributed.dask.org/en/latest/objects.inv
           options:
+            annotations_path: brief
             docstring_section_style: list
             docstring_style: google
             inherited_members: yes
             line_length: 60
             members_order: source
             merge_init_into_class: yes
             separate_signature: yes
+            show_root_members_full_path: no
+            show_object_full_path: no
             show_root_full_path: yes
             show_signature_annotations: yes
             show_submodules: no
+            signature_crossrefs: yes
   - search
   - section-index
```

### Comparing `proxystore-ex-0.1.2/proxystore_ex/connectors/daos.py` & `proxystore_ex-0.1.3/proxystore_ex/connectors/daos.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """DAOS Container connector implementation."""
+
 from __future__ import annotations
 
 import sys
 import uuid
 from types import TracebackType
 from typing import Any
 from typing import NamedTuple
@@ -223,14 +224,33 @@
         # this method, we have to try each key individually.
         objs: list[bytes | None] = []
         for key in keys:
             self._validate_key(key)
             objs.append(self.get(key))
         return objs
 
+    def new_key(self, obj: bytes | None = None) -> DAOSKey:
+        """Create a new key.
+
+        Args:
+            obj: Optional object which the key will be associated with.
+                Ignored in this implementation.
+
+        Returns:
+            Key which can be used to retrieve an object once \
+            [`set()`][proxystore_ex.connectors.daos.DAOSConnector.set] \
+            has been called on the key.
+        """
+        return DAOSKey(
+            pool=self.pool,
+            container=self.container,
+            namespace=self.namespace,
+            dict_key=str(uuid.uuid4()),
+        )
+
     def put(self, obj: bytes) -> DAOSKey:
         """Put a serialized object in the store.
 
         Args:
             obj: Serialized object to put in the store.
 
         Returns:
@@ -262,7 +282,28 @@
                 namespace=self.namespace,
                 dict_key=str(uuid.uuid4()),
             )
             for _ in objs
         ]
         self._dict.bput({key.dict_key: obj for key, obj in zip(keys, objs)})
         return keys
+
+    def set(self, key: DAOSKey, obj: bytes) -> None:
+        """Set the object associated with a key.
+
+        Note:
+            The [`Connector`][proxystore.connectors.protocols.Connector]
+            provides write-once, read-many semantics. Thus,
+            [`set()`][proxystore.connectors.protocols.DeferrableConnector.set]
+            should only be called once per key, otherwise unexpected behavior
+            can occur.
+
+        Warning:
+            This method is not required to be atomic and could therefore
+            result in race conditions with calls to
+            [`get()`][proxystore.connectors.protocols.Connector.get].
+
+        Args:
+            key: Key that the object will be associated with.
+            obj: Object to associate with the key.
+        """
+        self._dict.put(key.dict_key, obj)
```

### Comparing `proxystore-ex-0.1.2/proxystore_ex/connectors/dim/margo.py` & `proxystore_ex-0.1.3/proxystore_ex/connectors/dim/margo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Margo RPC-based distributed in-memory connector implementation."""
+
 from __future__ import annotations
 
 import atexit
 import logging
 import multiprocessing
 import os
 import sys
```

### Comparing `proxystore-ex-0.1.2/proxystore_ex/connectors/dim/models.py` & `proxystore_ex-0.1.3/proxystore_ex/connectors/dim/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Message types for communication with DIM servers."""
+
 from __future__ import annotations
 
 import sys
 from dataclasses import dataclass
 from typing import NamedTuple
 
 if sys.version_info >= (3, 9):  # pragma: >=3.9 cover
```

### Comparing `proxystore-ex-0.1.2/proxystore_ex/connectors/dim/ucx.py` & `proxystore_ex-0.1.3/proxystore_ex/connectors/dim/ucx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """UCX-based distributed in-memory connector implementation."""
+
 from __future__ import annotations
 
 import asyncio
 import atexit
 import logging
 import multiprocessing
 import signal
```

### Comparing `proxystore-ex-0.1.2/proxystore_ex/connectors/dim/utils.py` & `proxystore_ex-0.1.3/proxystore_ex/connectors/dim/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Shared functions used by DIM stores."""
+
 from __future__ import annotations
 
 import fcntl
 import socket
 import struct
```

### Comparing `proxystore-ex-0.1.2/proxystore_ex/connectors/dim/zmq.py` & `proxystore_ex-0.1.3/proxystore_ex/connectors/dim/zmq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ZeroMQ-based distributed in-memory connector implementation."""
+
 from __future__ import annotations
 
 import asyncio
 import atexit
 import logging
 import multiprocessing
 import signal
```

### Comparing `proxystore-ex-0.1.2/proxystore_ex/plugins/distributed.py` & `proxystore_ex-0.1.3/proxystore_ex/plugins/distributed.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Custom ProxyStore client for Dask Distributed."""
+
 from __future__ import annotations
 
 import functools
 import logging
 import sys
 import warnings
 from functools import partial
@@ -26,21 +27,20 @@
 except ImportError as e:  # pragma: no cover
     raise ImportError(
         'The dask and distributed packages must both be installed to '
         'use the associated plugins.',
     ) from e
 
 from proxystore.connectors.protocols import Connector
-from proxystore.proxy import _proxy_trampoline
 from proxystore.proxy import Proxy
 from proxystore.serialize import serialize
 from proxystore.store import get_store
 from proxystore.store import Store
-from proxystore.store.factory import StoreFactory
 from proxystore.store.types import ConnectorKeyT
+from proxystore.store.utils import get_key
 from proxystore.warnings import ExperimentalWarning
 
 warnings.warn(
     'Dask plugins are an experimental feature and may exhibit unexpected '
     'behaviour or change in the future.',
     category=ExperimentalWarning,
     stacklevel=2,
@@ -49,40 +49,76 @@
 T = TypeVar('T')
 P = ParamSpec('P')
 ConnectorT = TypeVar('ConnectorT', bound=Connector[Any])
 
 logger = logging.getLogger(__name__)
 
 
-class Future(DaskDistributedFuture):
-    """Custom future which returns results as proxies as necessary.
-
-    The ProxyStore Dask [`Client`][proxystore_ex.plugins.distributed.Client]
-    can return large function results as a
-    [`StoreFactory`][proxystore.store.factory.StoreFactory] instance which
-    will return the actual function result when invoked. This custom
-    Dask [`Future`][distributed.Future] will wrap result factories in a
-    [`Proxy`][proxystore.proxy.Proxy].
-    """
-
-    def result(self, timeout: int | None = None) -> Any:
-        """Wait until computation completes, gather result to local process."""
-        result = super().result()
-        if isinstance(result, StoreFactory):
-            result = _proxy_trampoline(result)
-        return result
-
-
 class Client(DaskDistributedClient):
     """Dask Distributed Client with ProxyStore support.
 
     This is a wrapper around [`dask.distributed.Client`][distributed.Client]
     that proxies function arguments and return values using a provided
     [`Store`][proxystore.store.base.Store] and threshold size.
 
+    !!! warning
+
+        The custom Dask [`Client`][proxystore_ex.plugins.distributed.Client]
+        is an experimental feature and the API may change in the future. If you
+        encounter unexpected behavior, please
+        [open a bug report](https://github.com/proxystore/extensions/issues/new/choose){target=_blank}.
+
+    Using this custom client is as easy as changing your import and passing
+    two extra arguments to the constructor.
+
+    ```python linenums="1" title="example.py" hl_lines="3 9"
+    import tempfile
+
+    from proxystore.ex.plugins.distributed import Client  # (1)!
+    from proxystore.connectors.file import FileConnector
+    from proxystore.store import Store
+
+    with tempfile.TemporaryDirectory() as tmp_dir:
+        with Store('default', FileConnector(tmp_dir), register=True) as store:
+            client = Client(..., ps_store=store, ps_threshold=100)  # (2)!
+
+            x = list(range(100))
+            p = store.proxy(x)
+            y = client.submit(sum, p)
+
+            print(f'Result: {y.result()}')
+
+            client.close()
+    ```
+
+    1. Change the import of `Client` from `dask.distributed` to
+       `proxystore.ex.plugins.distributed`.
+    2. Pass your [`Store`][proxystore.store.base.Store] and threshold object
+       size. Serialized objects larger than the threshold size in bytes will
+       be serialized using the store you provide and pass-by-proxy.
+
+    The custom [`Client`][proxystore_ex.plugins.distributed.Client] behaves
+    exactly as a normal Dask client when `ps_store` is `None`. But when
+    ProxyStore is configured, function args, kwargs, and results from
+    passed to or from [`Client.submit()`][distributed.Client.submit] and
+    [`Client.map()`][distributed.Client.map] will be scanned and proxied as
+    necessary based on their size.
+
+    When invoking a function, you can alter this behavior by passing
+    `proxy_args=False` and/or `proxy_result=False` to disable proxying for that
+    specific function submission to the scheduler.
+
+    !!! warning
+
+        There are some edge cases to be aware of when using the automatic
+        proxying. Please read the documentation for
+        [`Client.submit()`][proxystore_ex.plugins.distributed.Client.submit]
+        and [`Client.map()`][proxystore_ex.plugins.distributed.Client.map] for
+        the most up to date details.
+
     Args:
         args: Positional arguments to pass to
             [`dask.distributed.Client`][distributed.Client].
         ps_store: Store to use when proxying objects.
         ps_threshold: Object size threshold in bytes. Objects larger than this
             threshold will be proxied.
         kwargs: Keyword arguments to pass to
@@ -138,14 +174,16 @@
         This method adds the `proxy_args` and `proxy_result` flags (default
         `True`) which can be used to disable proxying of function arguments
         or return values, respectively, for a single invocation.
 
         Note:
             Proxied arguments will be evicted from the store when the
             future containing the result of the function application is set.
+            However, proxied keyword arguments shared across all functions
+            will not be evict if they were proxied.
 
         Warning:
             Unless the function is explicitly marked as not pure, a function
             result that gets proxied will not be automatically evicted. This
             is because Dask caches results of pure functions to avoid
             duplicate computation so it is not guaranteed to be safe to evict
             the function result once consumed by the client code.
@@ -156,39 +194,33 @@
             and self._ps_store is not None
         ):
             # map() partitions the iterators if batching needs to be performed
             # and calls itself again on each of the batches in the iterators.
             # In this case, we don't want to proxy the pre-batched iterators
             # and instead want to wait to proxy until the later calls to map()
             # on each batch.
-
             key = key or funcname(func)
             iterables = list(zip(*zip(*iterables)))  # type: ignore[assignment]
             if not isinstance(key, list) and pure:  # pragma: no branch
-                # Calling tokenize() on args/kwargs containing proxies will
-                # fail because the tokenize dispatch mechanism will perform
-                # introspection on the proxy. To avoid this failure, we
-                # can create the key before proxying. Source:
-                # https://github.com/dask/distributed/blob/6d1e1333a72dd78811883271511070c70369402b/distributed/client.py#L2126
                 key = [
                     f'{key}-{tokenize(func, kwargs, *args)}-proxy'
                     for args in zip(*iterables)
                 ]
 
             iterables = tuple(
-                pseudoproxy_iterable(
+                proxy_iterable(
                     iterable,
                     store=self._ps_store,
                     threshold=self._ps_threshold if proxy_args else None,
                     evict=False,
                 )
                 for iterable in iterables
             )
 
-            kwargs = pseudoproxy_mapping(
+            kwargs = proxy_mapping(
                 kwargs,
                 store=self._ps_store,
                 threshold=self._ps_threshold if proxy_args else None,
                 evict=False,
             )
 
             func = proxy_task_wrapper(
@@ -196,15 +228,15 @@
                 store=self._ps_store,
                 threshold=self._ps_threshold if proxy_result else None,
                 # Pure function results can be cached so we don't want to
                 # evict those once the result is consumed
                 evict=not pure,
             )
 
-        base_futures = super().map(
+        futures = super().map(
             func,
             *iterables,
             key=key,
             workers=workers,
             retries=retries,
             resources=resources,
             priority=priority,
@@ -217,40 +249,35 @@
             **kwargs,
         )
 
         if (
             not (batch_size and batch_size > 1 and total_length > batch_size)
             and self._ps_store is not None
         ):
-            futures = [
-                Future(
-                    key=base_future.key,
-                    client=base_future._client,
-                    inform=base_future._inform,
-                    state=base_future._state,
-                )
-                for base_future in base_futures
-            ]
-            del base_futures
-
             for future, *args in zip(futures, *iterables):
                 proxied_args_keys = [
-                    f.key for f in args if isinstance(f, StoreFactory)
+                    get_key(x) for x in args if isinstance(x, Proxy)
                 ]
                 # TODO: how to delete kwargs?
                 callback = partial(
                     _evict_proxies_callback,
                     keys=proxied_args_keys,
                     store=self._ps_store,
                 )
                 future.add_done_callback(callback)
 
-            return futures
-        else:
-            return base_futures
+            if any(isinstance(x, Proxy) for x in kwargs.values()):
+                warnings.warn(
+                    'A keyword argument to map() was proxied, but proxied '
+                    'keyword arguments will not be automatically evicted. '
+                    'This can lead to memory leaks.',
+                    stacklevel=2,
+                )
+
+        return futures
 
     def submit(  # type: ignore[no-untyped-def]
         self,
         func,
         *args,
         key=None,
         workers=None,
@@ -287,54 +314,49 @@
             is because Dask caches results of pure functions to avoid
             duplicate computation so it is not guaranteed to be safe to evict
             the function result once consumed by the client code.
         """
         proxied_args_keys: list[ConnectorKeyT] = []
         if self._ps_store is not None:
             if key is None and pure:  # pragma: no branch
-                # Calling tokenize() on args/kwargs containing proxies will
-                # fail because the tokenize dispatch mechanism will perform
-                # introspection on the proxy. To avoid this failure, we
-                # can create the key before proxying. Source:
-                # https://github.com/dask/distributed/blob/6d1e1333a72dd78811883271511070c70369402b/distributed/client.py#L1942
                 key = f'{funcname(func)}-{tokenize(func, kwargs, *args)}-proxy'
                 pure = False
 
-            args = pseudoproxy_iterable(
+            args = proxy_iterable(
                 args,
                 store=self._ps_store,
                 threshold=self._ps_threshold if proxy_args else None,
                 # Don't evict data after proxy resolve because we will
                 # manually evict after the task future completes.
                 evict=False,
             )
             proxied_args_keys.extend(
-                f.key for f in args if isinstance(f, StoreFactory)
+                get_key(x) for x in args if isinstance(x, Proxy)
             )
 
-            kwargs = pseudoproxy_mapping(
+            kwargs = proxy_mapping(
                 kwargs,
                 store=self._ps_store,
                 threshold=self._ps_threshold if proxy_args else None,
                 evict=False,
             )
             proxied_args_keys.extend(
-                f.key for f in kwargs.values() if isinstance(f, StoreFactory)
+                get_key(x) for x in kwargs.values() if isinstance(x, Proxy)
             )
 
             func = proxy_task_wrapper(
                 func,
                 store=self._ps_store,
                 threshold=self._ps_threshold if proxy_result else None,
                 # Pure function results can be cached so we don't want to
                 # evict those once the result is consumed
                 evict=not pure,
             )
 
-        base_future = super().submit(
+        future = super().submit(
             func,
             *args,
             key=key,
             workers=workers,
             resources=resources,
             retries=retries,
             priority=priority,
@@ -343,215 +365,179 @@
             actor=actor,
             actors=actors,
             pure=pure,
             **kwargs,
         )
 
         if self._ps_store is not None:
-            future = Future(
-                key=base_future.key,
-                client=base_future._client,
-                inform=base_future._inform,
-                state=base_future._state,
-            )
-            del base_future
-
             callback = partial(
                 _evict_proxies_callback,
                 keys=proxied_args_keys,
                 store=self._ps_store,
             )
             future.add_done_callback(callback)
 
-            return future
-        else:
-            return base_future
+        return future
 
 
 def _evict_proxies_callback(
-    _future: Future,
+    _future: DaskDistributedFuture,
     keys: Iterable[ConnectorKeyT],
     store: Store[Any],
 ) -> None:
     for key in keys:
         store.evict(key)
 
 
-def pseudoproxy_by_size(
-    x: T | Proxy[T],
+def proxy_by_size(
+    x: T,
     store: Store[ConnectorT],
     threshold: int | None = None,
     evict: bool = True,
-) -> T | StoreFactory[ConnectorT, T]:
+) -> T | Proxy[T]:
     """Serialize an object and proxy it if the object is larger enough.
 
     Args:
         x: Object to possibly proxy.
         store: Store to use to proxy objects.
         threshold: Threshold size in bytes. If `None`, the object will not
             be proxied.
         evict: Evict flag value to pass to created proxies.
 
     Returns:
         The input object `x` if `x` is smaller than `threshold` otherwise \
-        a [`StoreFactory`][proxystore.store.factory.StoreFactory] which can \
-        be used to initialize a [`Proxy`][proxystore.proxy.Proxy].
+        a [`Proxy`][proxystore.proxy.Proxy] of `x`.
     """
-    if threshold is None:
+    if threshold is None or isinstance(x, Proxy):
         return x
 
-    if isinstance(x, Proxy):
-        # Shortcut to replace proxies with their factories because
-        # proxies are not compatible with Dask as function arguments.
-        return x.__factory__
-
     s = serialize(x)
 
     if len(s) >= threshold:
         proxy = store.proxy(
             s,
             evict=evict,
+            # We can't use populate_target here because we are passing
+            # the serialized object to store.proxy(), not the actual object.
+            # populate_target=True,
             serializer=lambda x: x,
             skip_nonproxiable=True,
         )
-        res = proxy.__factory__
+
+        # This is dangerous code, but is taken from the Proxy constructor
+        # to essentially mimic what populate_target=True would have done
+        # above but using the actual target object x and not the serialized s.
+        object.__setattr__(proxy, '__proxy_target__', x)
+        object.__setattr__(proxy, '__proxy_default_class__', x.__class__)
+        default_hash: Exception | int
+        try:
+            default_hash = hash(x)
+        except TypeError as e:
+            default_hash = e
+        object.__setattr__(proxy, '__proxy_default_hash__', default_hash)
+
+        return cast(Proxy[T], proxy)
     else:
         # In this case, we paid the cost of serializing x but did not use
         # that serialization of x so it will be serialized again using
         # Dask's mechanisms. This adds some overhead, but the hope is that
         # the threshold is reasonably set such that it is only small objects
         # which get serialized twice. Large objects above the threshold only
         # get serialized once by ProxyStore and the lightweight proxy is
         # serialized by Dask.
-        res = x
-
-    return res
+        return x
 
 
-def pseudoproxy_iterable(
+def proxy_iterable(
     iterable: Iterable[Any],
     store: Store[ConnectorT],
     threshold: int | None = None,
     evict: bool = True,
 ) -> tuple:  # type: ignore[type-arg]
-    """Psuedoproxy values in an iterable than the threshold size.
-
-    This function is "pseudo" because values larger than the threshold size
-    are technically proxied, but the proxies are discarded and only the
-    internal factory is returned. This is because Dask does not play nicely
-    with serializing proxy types so we pass the factories instead and
-    reconstruct the proxies later.
+    """Proxy values in an iterable larger than the threshold size.
 
     Args:
         iterable: Iterable containing possibly large values to proxy.
         store: Store to use to proxy objects.
         threshold: Threshold size in bytes. If `None`, no objects will b
             proxied.
         evict: Evict flag value to pass to created proxies.
 
     Returns:
         Tuple containing the objects yielded by the iterable with objects \
-        larger than the threshold size replaced with factories which \
-        can later be used to construct proxies.
+        larger than the threshold size replaced with proxies.
     """
     return tuple(
-        pseudoproxy_by_size(
+        proxy_by_size(
             value,
             store=store,
             threshold=threshold,
             evict=evict,
         )
         for value in iterable
     )
 
 
-def pseudoproxy_mapping(
+def proxy_mapping(
     mapping: Mapping[T, Any],
     store: Store[ConnectorT],
     threshold: int | None = None,
     evict: bool = True,
 ) -> dict[T, Any]:
-    """Psuedoproxy values in a mapping larger than the threshold size.
-
-    This function is "pseudo" because values larger than the threshold size
-    are technically proxied, but the proxies are discarded and only the
-    internal factory is returned. This is because Dask does not play nicely
-    with serializing proxy types so we pass the factories instead and
-    reconstruct the proxies later.
+    """Proxy values in a mapping larger than the threshold size.
 
     Args:
         mapping: Mapping containing possibly large values to proxy.
         store: Store to use to proxy objects.
         threshold: Threshold size in bytes. If `None`, no objects will b
             proxied.
         evict: Evict flag value to pass to created proxies.
 
     Returns:
         Mapping containing the same keys and values as the input mapping \
-        but objects larger than the threshold size are replaced with \
-        factories which can be later used to construct proxies.
+        but objects larger than the threshold size are replaced with proxies.
     """
     return {
-        key: pseudoproxy_by_size(
+        key: proxy_by_size(
             mapping[key],
             store=store,
             threshold=threshold,
             evict=evict,
         )
         for key in mapping
     }
 
 
 def proxy_task_wrapper(
     func: Callable[P, T],
     store: Store[ConnectorT],
     threshold: int | None = None,
     evict: bool = True,
-) -> Callable[P, T | StoreFactory[ConnectorT, T]]:
+) -> Callable[P, T | Proxy[T]]:
     """Proxy task wrapper.
 
-    Wraps a task function with mechanisms to translate StoreFactory types
-    to Proxy types initialized with the factory and to proxy return
-    values larger than a threshold.
+    Wraps a task function to proxy returns values larger than a threshold.
 
     Args:
         func: Function to wrap.
         store: Store to use to proxy the result.
         threshold: Threshold size in bytes.
         evict: Evict flag value to pass to the created proxy.
 
     Returns:
         Callable with the same shape as `func` but that returns either the \
         original return type or a factory of the return type which can be \
         used to construct a proxy.
     """
 
     @functools.wraps(func)
-    def _proxy_wrapper(
-        *args: P.args,
-        **kwargs: P.kwargs,
-    ) -> T | StoreFactory[ConnectorT, T]:
-        args = cast(
-            P.args,
-            tuple(
-                _proxy_trampoline(v) if isinstance(v, StoreFactory) else v
-                for v in args
-            ),
-        )
-        kwargs = cast(
-            P.kwargs,
-            {
-                k: _proxy_trampoline(v) if isinstance(v, StoreFactory) else v
-                for k, v in kwargs.items()
-            },
-        )
-
+    def _proxy_wrapper(*args: P.args, **kwargs: P.kwargs) -> T | Proxy[T]:
         result = func(*args, **kwargs)
-        factory_or_result = pseudoproxy_by_size(
+        proxy_or_result = proxy_by_size(
             result,
             store=store,
             threshold=threshold,
             evict=evict,
         )
-        return factory_or_result
+        return proxy_or_result
 
     return _proxy_wrapper
```

### Comparing `proxystore-ex-0.1.2/proxystore_ex.egg-info/PKG-INFO` & `proxystore_ex-0.1.3/proxystore_ex.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,66 @@
 Metadata-Version: 2.1
 Name: proxystore-ex
-Version: 0.1.2
+Version: 0.1.3
 Summary: ProxyStore extensions.
 Author: Globus Labs
 Author-email: Greg Pauloski <jgpauloski@uchicago.edu>
 Maintainer-email: Greg Pauloski <jgpauloski@uchicago.edu>, Valerie Hayot-Sasson <vhayot@uchicago.edu>
 License: MIT
-Project-URL: homepage, https://proxystore.dev
-Project-URL: documentation, https://extensions.proxystore.dev
-Project-URL: repository, https://github.com/proxystore/extensions
+Project-URL: Homepage, https://proxystore.dev
+Project-URL: Documentation, https://extensions.proxystore.dev
+Project-URL: Source, https://github.com/proxystore/extensions
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: proxystore>=0.5.0
+Requires-Dist: proxystore>=0.6.5
 Requires-Dist: pyzmq
 Provides-Extra: dev
 Requires-Dist: covdefaults>=2.2; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: dask; extra == "dev"
 Requires-Dist: distributed; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio>=0.23.2; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
+Requires-Dist: ruff>=0.2.0; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: virtualenv; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: black; extra == "docs"
 Requires-Dist: mkdocs-gen-files; extra == "docs"
 Requires-Dist: mkdocs-literate-nav; extra == "docs"
-Requires-Dist: mkdocs-material!=9.4.0; extra == "docs"
+Requires-Dist: mkdocs-material==9.4.7; extra == "docs"
 Requires-Dist: mkdocs-section-index; extra == "docs"
-Requires-Dist: mkdocstrings[python]; extra == "docs"
+Requires-Dist: mkdocstrings==0.23.0; extra == "docs"
+Requires-Dist: mkdocstrings-python==1.8.0; extra == "docs"
 Requires-Dist: mike; extra == "docs"
 
 # ProxyStore Extensions
 
+![PyPI - Version](https://img.shields.io/pypi/v/proxystore-ex)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/proxystore-ex)
+![GitHub License](https://img.shields.io/github/license/proxystore/extensions)
+
 [![docs](https://github.com/proxystore/extensions/actions/workflows/docs.yml/badge.svg)](https://github.com/proxystore/extensions/actions)
 [![tests](https://github.com/proxystore/extensions/actions/workflows/tests.yml/badge.svg)](https://github.com/proxystore/extensions/actions)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/proxystore/extensions/main.svg)](https://results.pre-commit.ci/latest/github/proxystore/extensions/main)
 
-Extensions for the [ProxyStore](https://github.com/proxystore/proxystore/).
+Extensions for the [ProxyStore](https://github.com/proxystore/proxystore/) package.
 
 This extensions package contains experimental features, features with
 non-Python dependencies, and plugins for third-party tools.
 
 ## Installation
 
 The extensions package can be installed alongside
@@ -80,7 +89,11 @@
 `proxystore` via the [`proxystore.ex`](https://docs.proxystore.dev/latest/api/ex/)
 module. This is the recommended method for import extension features. E.g.,
 
 ```python
 from proxystore_ex.connectors.daos import DAOSConnector  # Direct
 from proxystore.ex.connectors.daos import DAOSConnector  # Recommended
 ```
+
+## Citation
+
+The preferred citations for this code are provided at https://docs.proxystore.dev/latest/publications/.
```

### Comparing `proxystore-ex-0.1.2/proxystore_ex.egg-info/SOURCES.txt` & `proxystore_ex-0.1.3/proxystore_ex.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .gitignore
 .pre-commit-config.yaml
-CITATION.cff
 LICENSE
 README.md
 mkdocs.yml
 pyproject.toml
 tox.ini
 .github/dependabot.yml
 .github/pull_request_template.md
@@ -18,15 +17,14 @@
 .github/workflows/docs.yml
 .github/workflows/integration.yml
 .github/workflows/publish.yml
 .github/workflows/tests.yml
 docs/generate_api.py
 docs/index.md
 docs/installation.md
-docs/known-issues.md
 docs/_overrides/base.html
 docs/_templates/python/material/function.html
 docs/_templates/python/material/module.html
 docs/_templates/python/material/docstring/admonition.html
 docs/contributing/index.md
 docs/contributing/issues-pull-requests.md
 docs/contributing/releases.md
```

### Comparing `proxystore-ex-0.1.2/pyproject.toml` & `proxystore_ex-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,70 @@
 [build-system]
 requires = ["setuptools>=64.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proxystore-ex"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
-    {name = "Globus Labs"},
     {name = "Greg Pauloski", email = "jgpauloski@uchicago.edu"},
+    {name = "Globus Labs"},
 ]
 maintainers = [
     {name = "Greg Pauloski", email = "jgpauloski@uchicago.edu"},
     {name = "Valerie Hayot-Sasson", email = "vhayot@uchicago.edu"},
 ]
 description = "ProxyStore extensions."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 dependencies = [
-    "proxystore>=0.5.0",
+    "proxystore>=0.6.5",
     "pyzmq",
 ]
 
 [project.urls]
-homepage = "https://proxystore.dev"
-documentation = "https://extensions.proxystore.dev"
-repository = "https://github.com/proxystore/extensions"
+Homepage = "https://proxystore.dev"
+Documentation = "https://extensions.proxystore.dev"
+Source = "https://github.com/proxystore/extensions"
 
 [project.optional-dependencies]
 dev = [
     "covdefaults>=2.2",
     "coverage",
     "dask",
     "distributed",
     "mypy",
     "pre-commit",
     "pytest",
     "pytest-asyncio>=0.23.2",
     "pytest-cov",
     "pytest-timeout",
-    "ruff",
+    "ruff>=0.2.0",
     "tox",
     "virtualenv",
 ]
 docs = [
     "black",
     "mkdocs-gen-files",
     "mkdocs-literate-nav",
-    # mkdocs-material 9.4.0 makes mkdocs-section-index break
-    "mkdocs-material!=9.4.0",
+    "mkdocs-material==9.4.7",
     "mkdocs-section-index",
-    "mkdocstrings[python]",
+    "mkdocstrings==0.23.0",
+    "mkdocstrings-python==1.8.0",
     "mike",
 ]
 
 [tool.codespell]
 skip = """
 .git,
 .github,
@@ -77,14 +81,15 @@
     "examples",
     "testing/mocked/pydaos.py",
 ]
 parallel = true
 
 [tool.mypy]
 python_version = "3.10"
+plugins = [ "proxystore.mypy_plugin" ]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_configs = true
@@ -100,28 +105,40 @@
 allow_incomplete_defs = true
 allow_untyped_defs = true
 
 [tool.pytest]
 timeout = 30
 
 [tool.ruff]
+line-length = 79
+target-version = "py38"
+
+[tool.ruff.format]
+indent-style = "space"
+quote-style = "single"
+
+[tool.ruff.lint]
 # See all rules here: https://beta.ruff.rs/docs/rules
 select = [
     # pyflakes
     "F",
     # pycodestyle
     "E",
+    # mccabe
+    "C90",
     # isort
     "I",
     # pep8-naming
     "N",
     # pydocstyle
     "D",
     # pyupgrade
     "UP",
+    # flake8-2020
+    "YTT",
     # flake8-bugbear
     "B",
     # flake8-builtins
     "A",
     # flake8-commas
     "COM",
     # flake8-comprehensions
@@ -130,14 +147,16 @@
     "ISC",
     # flake8-pytest-style
     "PT",
     # flake8-quotes
     "Q",
     # flake8-debugger
     "T10",
+    # flake8-simplify
+    "SIM",
     # PyLint
     "PLE", "PLW",
     # ruff-specific
     "RUF",
 ]
 extend-ignore = [
     # Do not require docstrings for magic methods
@@ -149,39 +168,35 @@
     # Ruff will change all([generator]) to all(generator) because the all/any
     # generator expressions directly and the list comprehension is not needed.
     # However, coverage marks unfinished generators as not covered and
     # all/any can early exit before exhausting the generator.
     "C419",
     # Allow pytest.raises() without match
     "PT011",
+    # Allow try-except-pass and nested with statements
+    "SIM105", "SIM117",
 ]
-line-length = 79
-target-version = "py38"
 
-[tool.ruff.flake8-pytest-style]
+[tool.ruff.lint.flake8-pytest-style]
 parametrize-values-type = "tuple"
 
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 inline-quotes = "single"
 
-[tool.ruff.format]
-indent-style = "space"
-quote-style = "single"
-
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 force-single-line = true
 known-first-party = ["proxystore_ex", "test", "testing"]
 order-by-type = false
 required-imports = ["from __future__ import annotations"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "*/__init__.py" = ["F401"]
 "tests/*" = ["D10"]
 "tests/conftest.py" = ["F401"]
 "testing/*" = ["D100", "D104"]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.setuptools.packages.find]
 exclude = ["tests*", "testing*"]
 namespaces = false
```

### Comparing `proxystore-ex-0.1.2/testing/compat.py` & `proxystore_ex-0.1.3/testing/compat.py`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/testing/connectors.py` & `proxystore_ex-0.1.3/testing/connectors.py`

 * *Files 8% similar despite different names*

```diff
@@ -108,19 +108,16 @@
 
 
 @pytest.fixture(scope='session')
 def zmq_connector() -> Generator[Connector[Any], None, None]:
     """ZeroMQ store fixture."""
     port = open_port()
 
-    if platform.system() == 'Darwin':  # pragma: no cover
-        # MacOS GitHub Actions runners are slow
-        timeout = 1.0
-    else:  # pragma: no cover
-        timeout = 0.5
+    # MacOS GitHub Actions runners are slow
+    timeout = 1.0 if platform.system() == 'Darwin' else 0.5
 
     with zmq.ZeroMQConnector(
         port=port,
         timeout=timeout,
     ) as connector:
         yield connector
```

### Comparing `proxystore-ex-0.1.2/testing/mocked/pydaos.py` & `proxystore_ex-0.1.3/testing/mocked/pydaos.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 A lot of this code is either inneficient, not very pythonic, or just really
 strange, but this is because it is verbatim from the reference implementation
 where possible. There are some strange choices in it...
 
 Reference implementation:
 https://github.com/daos-stack/daos/blob/release/2.4/src/client/pydaos/pydaos_core.py
 """
+
 from __future__ import annotations
 
 from typing import Any
 from typing import cast
 from typing import Dict
 from typing import Generator
```

### Comparing `proxystore-ex-0.1.2/testing/mocked/pymargo.py` & `proxystore_ex-0.1.3/testing/mocked/pymargo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Mock PyMargo implementation."""
+
 from __future__ import annotations
 
 from typing import Any
 
 from proxystore.serialize import serialize
 
 from proxystore_ex.connectors.dim.models import DIMKey
```

### Comparing `proxystore-ex-0.1.2/testing/mocked/ucp.py` & `proxystore_ex-0.1.3/testing/mocked/ucp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Mock UCX implementation."""
+
 from __future__ import annotations
 
 from typing import Any
 
 from proxystore.serialize import deserialize
 from proxystore.serialize import serialize
```

### Comparing `proxystore-ex-0.1.2/testing/utils.py` & `proxystore_ex-0.1.3/testing/utils.py`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/tests/conftest.py` & `proxystore_ex-0.1.3/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import sys
+from typing import Generator
 
 try:
     import pydaos
 except ImportError:
     from testing.mocked import pydaos
 
     sys.modules['pydaos'] = pydaos
@@ -21,12 +22,26 @@
 try:
     import ucp
 except ImportError:
     from testing.mocked import ucp
 
     sys.modules['ucp'] = ucp
 
+import proxystore
+import pytest
+
 from testing.connectors import connectors
 from testing.connectors import daos_connector
 from testing.connectors import margo_connector
 from testing.connectors import ucx_connector
 from testing.connectors import zmq_connector
+
+
+@pytest.fixture(autouse=True)
+def _verify_no_registered_stores() -> Generator[None, None, None]:
+    yield
+
+    if len(proxystore.store._stores) > 0:  # pragma: no cover
+        raise RuntimeError(
+            'Test left at least one store registered: '
+            f'{tuple(proxystore.store._stores.keys())}.',
+        )
```

### Comparing `proxystore-ex-0.1.2/tests/connectors/connectors_test.py` & `proxystore_ex-0.1.3/tests/connectors/connectors_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from __future__ import annotations
 
 from typing import Any
 
-try:
-    from proxystore.connectors.connector import Connector
-except ImportError:  # pragma: no cover
-    # This import changed in ProxyStore v0.6.1
-    from proxystore.connectors.protocols import Connector
+from proxystore.connectors.protocols import Connector
+from proxystore.connectors.protocols import DeferrableConnector
 
 
 def test_connector_repr(connectors: Connector[Any]) -> None:
     assert isinstance(repr(connectors), str)
 
 
 def test_connector_basic_ops(connectors: Connector[Any]) -> None:
@@ -47,7 +44,19 @@
     connector = connectors
 
     config = connector.config()
     new_connector = type(connector).from_config(config)
 
     assert isinstance(new_connector, Connector)
     assert type(connector) == type(new_connector)
+
+
+def test_deferrable_connector_ops(connectors: Connector[Any]) -> None:
+    connector = connectors
+
+    if isinstance(connector, DeferrableConnector):  # pragma: no break
+        obj = b'test_value'
+        key = connector.new_key(obj)
+        assert not connector.exists(key)
+        connector.set(key, obj)
+        connector.set(key, obj)
+        assert connector.get(key) == obj
```

### Comparing `proxystore-ex-0.1.2/tests/connectors/daos_test.py` & `proxystore_ex-0.1.3/tests/connectors/daos_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/tests/connectors/dim/margo_test.py` & `proxystore_ex-0.1.3/tests/connectors/dim/margo_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/tests/connectors/dim/ucx_test.py` & `proxystore_ex-0.1.3/tests/connectors/dim/ucx_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-ex-0.1.2/tests/connectors/dim/zmq_test.py` & `proxystore_ex-0.1.3/tests/connectors/dim/zmq_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,16 @@
 from proxystore_ex.connectors.dim.models import RPCResponse
 from proxystore_ex.connectors.dim.zmq import wait_for_server
 from proxystore_ex.connectors.dim.zmq import ZeroMQConnector
 from proxystore_ex.connectors.dim.zmq import ZeroMQServer
 from testing.compat import randbytes
 from testing.utils import open_port
 
-if platform.system() == 'Darwin':  # pragma: no cover
-    # MacOS GitHub Actions runners are slow
-    TIMEOUT = 1.0
-else:  # pragma: no cover
-    TIMEOUT = 0.5
+# MacOS GitHub Actions runners are slow
+TIMEOUT = 1.0 if platform.system() == 'Darwin' else 0.5
 
 TEST_KEY = DIMKey(
     'zmq',
     obj_id='key',
     size=0,
     peer_host='localhost',
     peer_port=0,
```

### Comparing `proxystore-ex-0.1.2/tests/plugins/distributed_test.py` & `proxystore_ex-0.1.3/tests/plugins/distributed_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,24 +2,22 @@
 
 import pathlib
 
 import pytest
 from proxystore.connectors.file import FileConnector
 from proxystore.connectors.local import LocalConnector
 from proxystore.proxy import Proxy
-from proxystore.store import register_store
 from proxystore.store import Store
-from proxystore.store import unregister_store
-from proxystore.store.factory import StoreFactory
+from proxystore.store.utils import get_key
 
 from proxystore_ex.plugins.distributed import Client
+from proxystore_ex.plugins.distributed import proxy_by_size
+from proxystore_ex.plugins.distributed import proxy_iterable
+from proxystore_ex.plugins.distributed import proxy_mapping
 from proxystore_ex.plugins.distributed import proxy_task_wrapper
-from proxystore_ex.plugins.distributed import pseudoproxy_by_size
-from proxystore_ex.plugins.distributed import pseudoproxy_iterable
-from proxystore_ex.plugins.distributed import pseudoproxy_mapping
 
 
 def test_warn_unregistered_store() -> None:
     with Store('test_warn_unregistered_store', LocalConnector()) as store:
         with pytest.warns(UserWarning, match='Call register_store()'):
             client = Client(ps_store=store, ps_threshold=0)
             client.close()
@@ -45,17 +43,16 @@
     return x * x
 
 
 def test_client_proxy_everything(tmp_path: pathlib.Path) -> None:
     with Store(
         'test_client_proxy_everything',
         FileConnector(str(tmp_path / 'proxy-cache')),
+        register=True,
     ) as store:
-        register_store(store)
-
         client = Client(
             ps_store=store,
             ps_threshold=0,
             n_workers=1,
             processes=False,
         )
 
@@ -72,148 +69,184 @@
         futures = client.map(_square, [1, 2, 3], batch_size=2)
         results = [f.result() for f in futures]
         assert all([isinstance(r, Proxy) for r in results])
         assert results == [1, 4, 9]
 
         client.close()
 
-        unregister_store(store)
-
 
 def test_client_proxy_skip_result(tmp_path: pathlib.Path) -> None:
     with Store(
         'test_client_proxy_skip_result',
         FileConnector(str(tmp_path / 'proxy-cache')),
+        register=True,
     ) as store:
-        register_store(store)
-
         client = Client(
             ps_store=store,
             ps_threshold=0,
             n_workers=1,
             processes=False,
         )
 
         future = client.submit(sum, [1, 2, 3], proxy_result=False)
         result = future.result()
         assert not isinstance(result, Proxy)
         assert result == 6
 
         client.close()
 
-        unregister_store(store)
+
+def _pow(x: int, *, p: int) -> int:
+    assert isinstance(x, Proxy)
+    assert isinstance(p, Proxy)
+    return x**p
+
+
+def test_client_map_proxy_kwarg_warning(tmp_path: pathlib.Path) -> None:
+    with Store(
+        'test_client_map_proxy_kwarg_warning',
+        FileConnector(str(tmp_path / 'proxy-cache')),
+        register=True,
+    ) as store:
+        client = Client(
+            ps_store=store,
+            ps_threshold=0,
+            n_workers=1,
+            processes=False,
+        )
+
+        with pytest.warns(UserWarning):
+            futures = client.map(_pow, [1, 2, 3], p=2)
+
+        results = [f.result() for f in futures]
+        assert all([isinstance(r, Proxy) for r in results])
+        assert results == [1, 4, 9]
+
+        client.close()
 
 
 def test_client_submit_manual_proxy(tmp_path: pathlib.Path) -> None:
     with Store(
         'test_client_submit_manual_proxy',
         FileConnector(str(tmp_path / 'proxy-cache')),
+        register=True,
     ) as store:
-        register_store(store)
-
         client = Client(
             ps_store=store,
             ps_threshold=int(1e6),
             n_workers=1,
             processes=False,
         )
 
         x = store.proxy([1, 2, 3])
 
         future = client.submit(sum, x, key='test-client-submit-manual-proxy')
         assert future.result() == 6
 
         client.close()
 
-        unregister_store(store)
-
 
-def test_pseudoproxy_by_size() -> None:
+def test_proxy_by_size() -> None:
     test_obj = 'foobar'
-    with Store('test_pseudoproxy_by_size', LocalConnector()) as store:
+    with Store('test_proxy_by_size', LocalConnector(), register=True) as store:
         # threshold = None should be a no-op and return the input object
-        x = pseudoproxy_by_size(test_obj, store, None)
+        x = proxy_by_size(test_obj, store, None)
         assert x == test_obj
 
         def _factory() -> str:
             return test_obj
 
-        # Passing a proxy should return its factory
-        x = pseudoproxy_by_size(Proxy(_factory), store, 0)
-        assert x == _factory
-        assert x() == test_obj
+        # Passing a proxy should return the proxy
+        p = Proxy(_factory)
+        x = proxy_by_size(p, store, 0)
+        assert x == p
 
         # Large threshold will not proxy object
-        x = pseudoproxy_by_size(test_obj, store, int(1e6))
+        x = proxy_by_size(test_obj, store, int(1e6))
         assert x == test_obj
 
         # Object actually gets proxied here
-        x = pseudoproxy_by_size(test_obj, store, 0, evict=True)
-        assert isinstance(x, StoreFactory)
-        assert store.exists(x.key)
-        assert x() == test_obj
-        assert not store.exists(x.key)
+        x = proxy_by_size(test_obj, store, 0, evict=True)
+        assert isinstance(x, Proxy)
+        # The target is already set by default
+        del x.__proxy_target__
+        assert x == test_obj
+        assert not store.exists(get_key(x))
 
 
-def test_pseudoproxy_iterable() -> None:
-    with Store('test_pseudoproxy_iterable', LocalConnector()) as store:
-        assert pseudoproxy_iterable([], store, 0) == ()
+def test_proxy_iterable() -> None:
+    with Store(
+        'test_proxy_iterable',
+        LocalConnector(),
+        register=True,
+    ) as store:
+        assert proxy_iterable([], store, 0) == ()
 
-        assert pseudoproxy_iterable([1, 2, 3], store, None) == (1, 2, 3)
+        assert proxy_iterable([1, 2, 3], store, None) == (1, 2, 3)
 
-        x = pseudoproxy_iterable(['a', 'b', 'c'], store, 0)
-        assert all([isinstance(v, StoreFactory) for v in x])
+        x = proxy_iterable(['a', 'b', 'c'], store, 0)
+        assert all([isinstance(v, Proxy) for v in x])
 
         v = ['x' * 10, 'x']
-        x = pseudoproxy_iterable(v, store, 8)
-        assert isinstance(x[0], StoreFactory)
+        x = proxy_iterable(v, store, 8)
+        assert isinstance(x[0], Proxy)
         assert isinstance(x[1], str)
 
 
-def test_pseudoproxy_mapping() -> None:
-    with Store('test_pseudoproxy_mapping', LocalConnector()) as store:
-        assert pseudoproxy_mapping({}, store, 0) == {}
+def test_proxy_mapping() -> None:
+    with Store('test_proxy_mapping', LocalConnector(), register=True) as store:
+        assert proxy_mapping({}, store, 0) == {}
 
         m = {'a': 1, 'b': 2}
-        assert pseudoproxy_mapping(m, store, None) == m
+        assert proxy_mapping(m, store, None) == m
 
-        x = pseudoproxy_mapping({'a': 'a', 'b': 'b'}, store, 0)
-        assert all([isinstance(v, StoreFactory) for v in x.values()])
+        x = proxy_mapping({'a': 'a', 'b': 'b'}, store, 0)
+        assert all([isinstance(v, Proxy) for v in x.values()])
 
         v = {'a': 'x' * 10, 'b': 'x'}
-        x = pseudoproxy_mapping(v, store, 8)
-        assert isinstance(x['a'], StoreFactory)
+        x = proxy_mapping(v, store, 8)
+        assert isinstance(x['a'], Proxy)
         assert isinstance(x['b'], str)
 
 
 def test_proxy_task_wrapper() -> None:
-    with Store('test_proxy_task_wrapper', LocalConnector()) as store:
+    with Store(
+        'test_proxy_task_wrapper',
+        LocalConnector(),
+        register=True,
+    ) as store:
 
         def _foo(a: int, b: str, *, c: int, d: str) -> str:
             assert not isinstance(a, Proxy)
             assert isinstance(b, Proxy)
             assert not isinstance(c, Proxy)
             assert isinstance(d, Proxy)
 
             return str(a) + b + str(c) + d
 
         foo = proxy_task_wrapper(_foo, store, threshold=8, evict=True)
 
-        b = store.proxy('b' * 10, evict=True).__factory__
-        d = store.proxy('d' * 10, evict=True).__factory__
+        b = store.proxy('b' * 10, evict=True)
+        d = store.proxy('d' * 10, evict=True)
 
         result = foo(1, b, c=2, d=d)
 
-        assert isinstance(result, StoreFactory)
-        assert result() == '1bbbbbbbbbb2dddddddddd'
-        assert not store.exists(result.key)
+        assert isinstance(result, Proxy)
+        # The target is already set by default
+        del result.__proxy_target__
+        assert result == '1bbbbbbbbbb2dddddddddd'
+        assert not store.exists(get_key(result))
 
 
 def test_proxy_task_wrapper_standard() -> None:
-    with Store('test_proxy_task_wrapper_standard', LocalConnector()) as store:
+    with Store(
+        'test_proxy_task_wrapper_standard',
+        LocalConnector(),
+        register=True,
+    ) as store:
 
         def _foo(x: int, *, y: int) -> int:
             return x * y
 
         foo = proxy_task_wrapper(_foo, store)
 
         assert foo(2, y=3) == 6
```

### Comparing `proxystore-ex-0.1.2/tox.ini` & `proxystore_ex-0.1.3/tox.ini`

 * *Files identical despite different names*

