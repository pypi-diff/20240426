# Comparing `tmp/dank_mids-4.20.90.tar.gz` & `tmp/dank_mids-4.20.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dank_mids-4.20.90.tar", last modified: Wed Apr 24 17:34:06 2024, max compression
+gzip compressed data, was "dank_mids-4.20.91.tar", last modified: Fri Apr 26 20:36:27 2024, max compression
```

## Comparing `dank_mids-4.20.90.tar` & `dank_mids-4.20.91.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:34:06.931902 dank_mids-4.20.90/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:34:06.919902 dank_mids-4.20.90/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:34:06.923902 dank_mids-4.20.90/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-24 17:33:57.000000 dank_mids-4.20.90/.github/workflows/deploy-docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-24 17:33:57.000000 dank_mids-4.20.90/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-24 17:33:57.000000 dank_mids-4.20.90/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-24 17:33:57.000000 dank_mids-4.20.90/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 17:33:57.000000 dank_mids-4.20.90/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-24 17:33:57.000000 dank_mids-4.20.90/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-24 17:34:06.931902 dank_mids-4.20.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-24 17:33:57.000000 dank_mids-4.20.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:34:06.923902 dank_mids-4.20.90/dank_mids/
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/_batch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:34:06.927902 dank_mids-4.20.90/dank_mids/_debugging/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/_debugging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/_debugging/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/_debugging/failures.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/_demo_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/_envs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    41204 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/_uid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:34:06.927902 dank_mids-4.20.90/dank_mids/brownie_patch/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/brownie_patch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/brownie_patch/_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/brownie_patch/_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/brownie_patch/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/brownie_patch/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/brownie_patch/overloaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/brownie_patch/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:34:06.927902 dank_mids-4.20.90/dank_mids/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/helpers/_codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/helpers/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/helpers/_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/semaphore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/semaphores.py
--rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-04-24 17:33:57.000000 dank_mids-4.20.90/dank_mids/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:34:06.931902 dank_mids-4.20.90/dank_mids.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-24 17:34:06.000000 dank_mids-4.20.90/dank_mids.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-24 17:34:06.000000 dank_mids-4.20.90/dank_mids.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:34:06.000000 dank_mids-4.20.90/dank_mids.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-24 17:34:06.000000 dank_mids-4.20.90/dank_mids.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 17:34:06.000000 dank_mids-4.20.90/dank_mids.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:34:06.927902 dank_mids-4.20.90/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-24 17:33:57.000000 dank_mids-4.20.90/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:34:06.919902 dank_mids-4.20.90/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:34:06.919902 dank_mids-4.20.90/docs/_build/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:34:06.927902 dank_mids-4.20.90/docs/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-24 17:33:57.000000 dank_mids-4.20.90/docs/_build/html/_static/alabaster.css
--rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-04-24 17:33:57.000000 dank_mids-4.20.90/docs/_build/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 17:33:57.000000 dank_mids-4.20.90/docs/_build/html/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-24 17:33:57.000000 dank_mids-4.20.90/docs/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-24 17:33:57.000000 dank_mids-4.20.90/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-24 17:33:57.000000 dank_mids-4.20.90/docs/_build/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-24 17:33:57.000000 dank_mids-4.20.90/docs/_build/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-24 17:33:57.000000 dank_mids-4.20.90/docs/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-24 17:33:57.000000 dank_mids-4.20.90/docs/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-24 17:33:57.000000 dank_mids-4.20.90/docs/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-04-24 17:33:57.000000 dank_mids-4.20.90/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-24 17:33:57.000000 dank_mids-4.20.90/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-24 17:33:57.000000 dank_mids-4.20.90/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-24 17:33:57.000000 dank_mids-4.20.90/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-24 17:33:57.000000 dank_mids-4.20.90/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:34:06.927902 dank_mids-4.20.90/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-24 17:33:57.000000 dank_mids-4.20.90/examples/dank_brownie_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 17:33:57.000000 dank_mids-4.20.90/license
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-24 17:33:57.000000 dank_mids-4.20.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 17:33:57.000000 dank_mids-4.20.90/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-24 17:33:57.000000 dank_mids-4.20.90/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 17:34:06.931902 dank_mids-4.20.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-24 17:33:57.000000 dank_mids-4.20.90/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:34:06.931902 dank_mids-4.20.90/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:33:57.000000 dank_mids-4.20.90/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-24 17:33:57.000000 dank_mids-4.20.90/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    16155 2024-04-24 17:33:57.000000 dank_mids-4.20.90/tests/test_brownie_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-24 17:33:57.000000 dank_mids-4.20.90/tests/test_dank_mids.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-24 17:33:57.000000 dank_mids-4.20.90/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.947580 dank_mids-4.20.91/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.935580 dank_mids-4.20.91/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.939580 dank_mids-4.20.91/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-26 20:36:17.000000 dank_mids-4.20.91/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-26 20:36:17.000000 dank_mids-4.20.91/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-26 20:36:17.000000 dank_mids-4.20.91/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-26 20:36:17.000000 dank_mids-4.20.91/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-26 20:36:17.000000 dank_mids-4.20.91/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-26 20:36:17.000000 dank_mids-4.20.91/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-26 20:36:27.947580 dank_mids-4.20.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-26 20:36:17.000000 dank_mids-4.20.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.939580 dank_mids-4.20.91/dank_mids/
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.943580 dank_mids-4.20.91/dank_mids/_debugging/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_debugging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_debugging/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_debugging/failures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_demo_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_envs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41591 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_uid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.943580 dank_mids-4.20.91/dank_mids/brownie_patch/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/brownie_patch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/brownie_patch/_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/brownie_patch/_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/brownie_patch/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/brownie_patch/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/brownie_patch/overloaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/brownie_patch/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12236 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.943580 dank_mids-4.20.91/dank_mids/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/helpers/_codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/helpers/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/helpers/_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/semaphores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.947580 dank_mids-4.20.91/dank_mids.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-26 20:36:27.000000 dank_mids-4.20.91/dank_mids.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-26 20:36:27.000000 dank_mids-4.20.91/dank_mids.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:36:27.000000 dank_mids-4.20.91/dank_mids.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-26 20:36:27.000000 dank_mids-4.20.91/dank_mids.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 20:36:27.000000 dank_mids-4.20.91/dank_mids.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.943580 dank_mids-4.20.91/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.935580 dank_mids-4.20.91/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.935580 dank_mids-4.20.91/docs/_build/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.947580 dank_mids-4.20.91/docs/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.947580 dank_mids-4.20.91/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-26 20:36:17.000000 dank_mids-4.20.91/examples/dank_brownie_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 20:36:17.000000 dank_mids-4.20.91/license
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-26 20:36:17.000000 dank_mids-4.20.91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 20:36:17.000000 dank_mids-4.20.91/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-26 20:36:17.000000 dank_mids-4.20.91/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-26 20:36:27.947580 dank_mids-4.20.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-26 20:36:17.000000 dank_mids-4.20.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.947580 dank_mids-4.20.91/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:17.000000 dank_mids-4.20.91/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-26 20:36:17.000000 dank_mids-4.20.91/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16155 2024-04-26 20:36:17.000000 dank_mids-4.20.91/tests/test_brownie_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-26 20:36:17.000000 dank_mids-4.20.91/tests/test_dank_mids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-26 20:36:17.000000 dank_mids-4.20.91/tests/test_examples.py
```

### Comparing `dank_mids-4.20.90/.github/workflows/deploy-docs.yaml` & `dank_mids-4.20.91/.github/workflows/deploy-docs.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 name: Deploy Documentation
 
 on:
   push:
     branches:
       - master
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+  
 # Sets permissions of the GITHUB_TOKEN to allow deployment to GitHub Pages
 permissions:
   contents: write
   id-token: write
   pages: write
   
 jobs:
```

### Comparing `dank_mids-4.20.90/.github/workflows/pytest.yaml` & `dank_mids-4.20.91/.github/workflows/pytest.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -23,14 +23,20 @@
         include:
         - os: ubuntu-latest
           path: ~/.cache/pip
         - os: macos-latest
           path: ~/Library/Caches/pip
         - os: windows-latest
           path: ~\AppData\Local\pip\Cache
+        exclude:
+        # gh runner throws "Error: Version ${{ matrix.pyversion }} with arch arm64 not found"
+        - os: macos-latest
+          pyversion: "3.8"
+        - os: macos-latest
+          pyversion: "3.9"
 
     steps:
       - name: Check out repository code
         uses: actions/checkout@v2
 
       - name: Setup Python (faster than using Python container)
         uses: actions/setup-python@v2
```

### Comparing `dank_mids-4.20.90/.github/workflows/release.yaml` & `dank_mids-4.20.91/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/PKG-INFO` & `dank_mids-4.20.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dank_mids
-Version: 4.20.90
+Version: 4.20.91
 Summary: Multicall batching middleware for asynchronous scripts using web3.py
 Home-page: https://github.com/BobTheBuidler/dank_mids
 Author: BobTheBuidler
 Author-email: bobthebuidlerdefi@gmail.com
 License: MIT
 Requires-Dist: aiofiles
 Requires-Dist: eth_retry<0.2,>=0.1.15
```

### Comparing `dank_mids-4.20.90/README.md` & `dank_mids-4.20.91/README.md`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/ENVIRONMENT_VARIABLES.py` & `dank_mids-4.20.91/dank_mids/ENVIRONMENT_VARIABLES.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/__init__.py` & `dank_mids-4.20.91/dank_mids/__init__.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/_batch.py` & `dank_mids-4.20.91/dank_mids/_batch.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/_debugging/_base.py` & `dank_mids-4.20.91/dank_mids/_debugging/_base.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/_debugging/failures.py` & `dank_mids-4.20.91/dank_mids/_debugging/failures.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/_exceptions.py` & `dank_mids-4.20.91/dank_mids/_exceptions.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/_mode.py` & `dank_mids-4.20.91/dank_mids/_mode.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/_requests.py` & `dank_mids-4.20.91/dank_mids/_requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 
 import abc
 import asyncio
 import logging
 import time
+import weakref
 from collections import defaultdict
 from concurrent.futures.process import BrokenProcessPool
 from contextlib import suppress
-from functools import cached_property, lru_cache
+from functools import cached_property, lru_cache, partial
 from typing import (TYPE_CHECKING, Any, DefaultDict, Dict, Generator, Generic,
                     Iterable, Iterator, List, NoReturn, Optional, Tuple,
                     TypeVar, Union)
 
 import a_sync
 import eth_retry
 import msgspec
@@ -45,26 +46,26 @@
 logger = logging.getLogger(__name__)
 
 _Response = TypeVar("_Response", Response, List[Response], RPCResponse, List[RPCResponse])
 
 class _RequestEvent(a_sync.Event):
     def __init__(self, owner: "_RequestMeta") -> None:
         super().__init__(debug_daemon_interval=300)
-        self._owner = owner
+        self._owner = weakref.proxy(owner)
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} object at {hex(id(self))} [{'set' if self.is_set() else 'unset'}, waiter:{self._owner}>"
     def set(self):
         # Make sure we wake up the _RequestEvent's event loop if its in another thread
         if asyncio.get_running_loop() == self._loop:
             super().set()
         else:
             self._loop.call_soon_threadsafe(super().set)
 
 class _RequestMeta(Generic[_Response], metaclass=abc.ABCMeta):
-    __slots__ = 'controller', 'uid', '_response', '_done', '_start', '_batch'
+    __slots__ = 'controller', 'uid', '_response', '_done', '_start', '_batch', '__weakref__'
     controller: "DankMiddlewareController"
     def __init__(self) -> None:
         self.uid = self.controller.call_uid.next
         self._response: Optional[_Response] = None
         self._done = _RequestEvent(self)
         self._start = time.time()
     
@@ -104,15 +105,15 @@
     __slots__ = 'method', 'params', 'should_batch', '_started', '_retry', '_daemon'
     dict_responses = set()
     str_responses = set()
 
     _types = set()
 
     def __init__(self, controller: "DankMiddlewareController", method: RPCEndpoint, params: Any, retry: bool = False):
-        self.controller = controller
+        self.controller = weakref.proxy(controller)
         self.method = method
         self.params = params
         self.should_batch = _should_batch_method(method)
         self._started = False
         self._retry = retry
         super().__init__()
 
@@ -346,23 +347,22 @@
     
 
 ### Batch requests:
 
 _Request = TypeVar("_Request")
 
 class _Batch(_RequestMeta[List[RPCResponse]], Iterable[_Request]):
-    __slots__ = 'calls', '_fut', '_lock', '_daemon'
+    _fut = None
+    __slots__ = 'calls', '_lock', '_daemon'
     calls: List[_Request]
 
     def __init__(self, controller: "DankMiddlewareController", calls: Iterable[_Request]):
-        self.controller = controller
-        self.calls = list(calls)  # type: ignore
-        self._fut = None
+        self.controller = weakref.proxy(controller)
+        self.calls = [weakref.proxy(call, callback=self._remove) for call in calls]
         self._lock = _AlertingRLock(name=self.__class__.__name__)
-        #self._len = 0
         super().__init__()
     
     def __bool__(self) -> bool:
         return bool(self.calls)
     
     def __getitem__(self, ix: int) -> _Request:
         return self.calls[ix]
@@ -428,14 +428,20 @@
             # TODO: use these exceptions to optimize for the user's node
             logger.debug('Dank too loud. Bisecting batch and retrying.')
         elif isinstance(e, BadResponse) and (_needs_full_request_spec(e) or _is_call_revert(e)):
             pass
         elif "429" not in f"{e}":
             logger.warning(f"unexpected {e.__class__.__name__}: {e}")
         return len(self) > 1
+      
+    def _remove(self, proxy: weakref.CallableProxyType) -> None:
+        try:
+            self.calls.remove(proxy)
+        except ValueError:
+            pass
 
 mcall_encoder = abi.default_codec._registry.get_encoder("(bool,(address,bytes)[])")
 mcall_decoder = abi.default_codec._registry.get_decoder("(uint256,uint256,(bool,bytes)[])")
 
 def mcall_encode(data: List[Tuple[bool, bytes]]) -> bytes:
     return mcall_encoder([False, data])
 
@@ -824,15 +830,17 @@
             self.controller.reduce_batch_size(len(self))
             stats.logger.devhint(
                 "We still need some better logic for catching these errors and using them to better optimize the batching process"
             )
 
     def _post_future_cleanup(self) -> None:
         with self.controller.pools_closed_lock:
-            self.controller.pending_rpc_calls = JSONRPCBatch(self.controller)
+            # a hacky way to get the real controller obj from the weak reference proxy
+            controller = self.controller.__repr__.__self__
+            self.controller.pending_rpc_calls = JSONRPCBatch(controller)
 
 def _log_exception(e: Exception) -> bool:
     # NOTE: These errors are expected during normal use and are not indicative of any problem(s). No need to log them.
     # TODO: Better filter what we choose to log here
     dont_need_to_see_errs = constants.RETRY_ERRS + ['out of gas', 'non_empty_data', 'exceeding --rpc.returndata.limit', "'code': 429", 'payload too large']
     
     dont_need_to_see_errs += [
@@ -845,8 +853,8 @@
     
     
     stre = str(e).lower()
     if any(err in stre for err in dont_need_to_see_errs):
         return ENVS.DEBUG  # type: ignore [attr-defined]
     logger.warning("The following exception is being logged for informational purposes and does not indicate failure:")
     logger.warning(e, exc_info=True)
-    return ENVS.DEBUG  # type: ignore [attr-defined]
+    return ENVS.DEBUG  # type: ignore [attr-defined]
```

### Comparing `dank_mids-4.20.90/dank_mids/_uid.py` & `dank_mids-4.20.91/dank_mids/_uid.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/brownie_patch/__init__.py` & `dank_mids-4.20.91/dank_mids/brownie_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/brownie_patch/_method.py` & `dank_mids-4.20.91/dank_mids/brownie_patch/_method.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/brownie_patch/call.py` & `dank_mids-4.20.91/dank_mids/brownie_patch/call.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/brownie_patch/contract.py` & `dank_mids-4.20.91/dank_mids/brownie_patch/contract.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/brownie_patch/overloaded.py` & `dank_mids-4.20.91/dank_mids/brownie_patch/overloaded.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/brownie_patch/types.py` & `dank_mids-4.20.91/dank_mids/brownie_patch/types.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/constants.py` & `dank_mids-4.20.91/dank_mids/constants.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/controller.py` & `dank_mids-4.20.91/dank_mids/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         if multicall:
             self.no_multicall.add(to_checksum_address(multicall))
         if self.mc2:
             self.no_multicall.add(self.mc2.address)
         if self.mc3:
             self.no_multicall.add(self.mc3.address)
         
-        self.method_semaphores = _MethodSemaphores(self)
+        self.eth_call_semaphores = _MethodSemaphores(self)["eth_call"]  # TODO: refactor this out
         # semaphores soon to be deprecated for smart queue
         self.method_queues = _MethodQueues(self)
         self.batcher = NotSoBrightBatcher()
         self.batcher.step = ENVS.MAX_MULTICALL_SIZE
 
         self.call_uid = UIDGenerator()
         self.multicall_uid: UIDGenerator = UIDGenerator()
@@ -137,15 +137,15 @@
                     return await queue(self, method, _helpers._make_hashable(params))
                 raise e
             
         # eth_call go thru a specialized Semaphore and other methods pass thru unblocked
         logger.debug(f'making {self.request_type.__name__} {method} with params {params}')
         if method != "eth_call":
             return await RPCRequest(self, method, params)
-        async with self.method_semaphores[method][params[1]]:
+        async with self.eth_call_semaphores[params[1]]:
             if params[0]["to"] not in self.no_multicall:
                 return await eth_call(self, params)
             return await RPCRequest(self, method, params)
     
     @eth_retry.auto_retry
     async def make_request(self, method: str, params: List[Any], request_id: Optional[int] = None) -> RawResponse:
         request = self.request_type(method=method, params=params, id=request_id or self.call_uid.next)
@@ -245,8 +245,8 @@
         if self.deploy_block is None:
             return True
         if isinstance(block, str):
             block = int(block, 16)
         return block < self.deploy_block
     
     def __hash__(self) -> int:
-        return hash(self.address)
+        return hash(self.address)
```

### Comparing `dank_mids-4.20.90/dank_mids/helpers/_codec.py` & `dank_mids-4.20.91/dank_mids/helpers/_codec.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/helpers/_helpers.py` & `dank_mids-4.20.91/dank_mids/helpers/_helpers.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/helpers/_session.py` & `dank_mids-4.20.91/dank_mids/helpers/_session.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/middleware.py` & `dank_mids-4.20.91/dank_mids/middleware.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/semaphores.py` & `dank_mids-4.20.91/dank_mids/semaphores.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/stats.py` & `dank_mids-4.20.91/dank_mids/stats.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids/types.py` & `dank_mids-4.20.91/dank_mids/types.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/dank_mids.egg-info/PKG-INFO` & `dank_mids-4.20.91/dank_mids.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dank_mids
-Version: 4.20.90
+Version: 4.20.91
 Summary: Multicall batching middleware for asynchronous scripts using web3.py
 Home-page: https://github.com/BobTheBuidler/dank_mids
 Author: BobTheBuidler
 Author-email: bobthebuidlerdefi@gmail.com
 License: MIT
 Requires-Dist: aiofiles
 Requires-Dist: eth_retry<0.2,>=0.1.15
```

### Comparing `dank_mids-4.20.90/dank_mids.egg-info/SOURCES.txt` & `dank_mids-4.20.91/dank_mids.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/docs/Makefile` & `dank_mids-4.20.91/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/docs/_build/html/_static/alabaster.css` & `dank_mids-4.20.91/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/docs/_build/html/_static/basic.css` & `dank_mids-4.20.91/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/docs/_build/html/_static/doctools.js` & `dank_mids-4.20.91/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/docs/_build/html/_static/language_data.js` & `dank_mids-4.20.91/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/docs/_build/html/_static/pygments.css` & `dank_mids-4.20.91/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/docs/_build/html/_static/searchtools.js` & `dank_mids-4.20.91/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/docs/_build/html/_static/sphinx_highlight.js` & `dank_mids-4.20.91/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/docs/conf.py` & `dank_mids-4.20.91/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/docs/make.bat` & `dank_mids-4.20.91/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/examples/dank_brownie_example.py` & `dank_mids-4.20.91/examples/dank_brownie_example.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/license` & `dank_mids-4.20.91/license`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/setup.py` & `dank_mids-4.20.91/setup.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/tests/test_brownie_patch.py` & `dank_mids-4.20.91/tests/test_brownie_patch.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.90/tests/test_dank_mids.py` & `dank_mids-4.20.91/tests/test_dank_mids.py`

 * *Files identical despite different names*

