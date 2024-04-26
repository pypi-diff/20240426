# Comparing `tmp/pydash-8.0.0.tar.gz` & `tmp/pydash-8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydash-8.0.0.tar", last modified: Wed Mar 27 02:49:21 2024, max compression
+gzip compressed data, was "pydash-8.0.1.tar", last modified: Fri Apr 26 13:23:42 2024, max compression
```

## Comparing `pydash-8.0.0.tar` & `pydash-8.0.1.tar`

### file list

```diff
@@ -1,89 +1,737 @@
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-03-27 02:49:21.302256 pydash-8.0.0/
--rw-r--r--   0 dgilland   (501) staff       (20)     1396 2023-06-02 13:53:01.000000 pydash-8.0.0/AUTHORS.rst
--rw-r--r--   0 dgilland   (501) staff       (20)    42299 2024-03-27 02:22:55.000000 pydash-8.0.0/CHANGELOG.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2581 2020-10-29 15:03:50.000000 pydash-8.0.0/CONTRIBUTING.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     1072 2021-01-05 22:53:19.000000 pydash-8.0.0/LICENSE.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      283 2023-03-18 22:34:56.000000 pydash-8.0.0/MANIFEST.in
--rw-r--r--   0 dgilland   (501) staff       (20)     4468 2024-03-27 02:49:21.302050 pydash-8.0.0/PKG-INFO
--rw-r--r--   0 dgilland   (501) staff       (20)     1262 2023-10-03 02:32:14.000000 pydash-8.0.0/README.rst
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-03-27 02:49:21.289054 pydash-8.0.0/docs/
--rw-r--r--   0 dgilland   (501) staff       (20)     3937 2019-02-04 01:30:20.000000 pydash-8.0.0/docs/Makefile
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-03-27 02:49:21.289203 pydash-8.0.0/docs/_templates/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-8.0.0/docs/_templates/.gitignore
--rw-r--r--   0 dgilland   (501) staff       (20)     2885 2019-02-04 01:30:20.000000 pydash-8.0.0/docs/api.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       28 2014-07-29 03:38:06.000000 pydash-8.0.0/docs/authors.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     4065 2019-02-04 01:30:20.000000 pydash-8.0.0/docs/callbacks.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2927 2021-09-28 21:40:18.000000 pydash-8.0.0/docs/chaining.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       30 2019-02-04 01:30:20.000000 pydash-8.0.0/docs/changelog.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     5116 2024-03-02 04:24:04.000000 pydash-8.0.0/docs/conf.py
--rw-r--r--   0 dgilland   (501) staff       (20)       33 2014-07-29 03:34:57.000000 pydash-8.0.0/docs/contributing.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      760 2019-02-04 01:30:20.000000 pydash-8.0.0/docs/deeppath.rst
--rw-rw-r--   0 dgilland   (501) staff       (20)       29 2020-10-28 20:30:40.000000 pydash-8.0.0/docs/devguide.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2045 2019-02-04 01:30:20.000000 pydash-8.0.0/docs/differences.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      605 2020-10-29 19:54:30.000000 pydash-8.0.0/docs/index.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      187 2021-06-27 18:15:05.000000 pydash-8.0.0/docs/installation.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      100 2019-02-04 01:30:20.000000 pydash-8.0.0/docs/kudos.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       45 2021-01-05 22:53:19.000000 pydash-8.0.0/docs/license.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     1499 2019-02-04 01:30:20.000000 pydash-8.0.0/docs/quickstart.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      562 2019-02-04 01:30:20.000000 pydash-8.0.0/docs/templating.rst
--rw-r--r--   0 dgilland   (501) staff       (20)    10538 2019-02-04 01:30:20.000000 pydash-8.0.0/docs/upgrading.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      497 2014-08-20 02:16:49.000000 pydash-8.0.0/docs/versioning.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     3851 2024-03-27 02:28:06.000000 pydash-8.0.0/pyproject.toml
--rw-r--r--   0 dgilland   (501) staff       (20)       10 2020-10-28 20:38:46.000000 pydash-8.0.0/requirements.txt
--rw-r--r--   0 dgilland   (501) staff       (20)       38 2024-03-27 02:49:21.302298 pydash-8.0.0/setup.cfg
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-03-27 02:49:21.282973 pydash-8.0.0/src/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-03-27 02:49:21.293096 pydash-8.0.0/src/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)    11706 2024-03-27 02:23:10.000000 pydash-8.0.0/src/pydash/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)    71289 2024-03-02 04:23:13.000000 pydash-8.0.0/src/pydash/arrays.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-03-27 02:49:21.294961 pydash-8.0.0/src/pydash/chaining/
--rw-r--r--   0 dgilland   (501) staff       (20)       93 2024-03-04 02:54:39.000000 pydash-8.0.0/src/pydash/chaining/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1364 2023-03-20 14:30:38.000000 pydash-8.0.0/src/pydash/chaining/all_funcs.py
--rw-r--r--   0 dgilland   (501) staff       (20)   130387 2024-03-04 02:54:39.000000 pydash-8.0.0/src/pydash/chaining/all_funcs.pyi
--rw-r--r--   0 dgilland   (501) staff       (20)     7704 2024-03-04 02:54:39.000000 pydash-8.0.0/src/pydash/chaining/chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)    54132 2024-03-02 04:23:13.000000 pydash-8.0.0/src/pydash/collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)      431 2023-03-18 22:34:56.000000 pydash-8.0.0/src/pydash/exceptions.py
--rw-r--r--   0 dgilland   (501) staff       (20)    40643 2024-03-02 04:23:13.000000 pydash-8.0.0/src/pydash/functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     9137 2024-03-02 04:23:13.000000 pydash-8.0.0/src/pydash/helpers.py
--rw-r--r--   0 dgilland   (501) staff       (20)    26839 2024-03-02 04:23:13.000000 pydash-8.0.0/src/pydash/numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    65283 2024-03-04 02:54:39.000000 pydash-8.0.0/src/pydash/objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    33711 2024-03-02 04:23:13.000000 pydash-8.0.0/src/pydash/predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-8.0.0/src/pydash/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)    57917 2024-03-02 04:23:13.000000 pydash-8.0.0/src/pydash/strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)      550 2024-03-02 04:23:13.000000 pydash-8.0.0/src/pydash/types.py
--rw-r--r--   0 dgilland   (501) staff       (20)    38266 2024-03-02 04:23:13.000000 pydash-8.0.0/src/pydash/utilities.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-03-27 02:49:21.301307 pydash-8.0.0/src/pydash.egg-info/
--rw-r--r--   0 dgilland   (501) staff       (20)     4468 2024-03-27 02:49:21.000000 pydash-8.0.0/src/pydash.egg-info/PKG-INFO
--rw-r--r--   0 dgilland   (501) staff       (20)     1844 2024-03-27 02:49:21.000000 pydash-8.0.0/src/pydash.egg-info/SOURCES.txt
--rw-r--r--   0 dgilland   (501) staff       (20)        1 2024-03-27 02:49:21.000000 pydash-8.0.0/src/pydash.egg-info/dependency_links.txt
--rw-r--r--   0 dgilland   (501) staff       (20)      161 2024-03-27 02:49:21.000000 pydash-8.0.0/src/pydash.egg-info/requires.txt
--rw-r--r--   0 dgilland   (501) staff       (20)        7 2024-03-27 02:49:21.000000 pydash-8.0.0/src/pydash.egg-info/top_level.txt
--rw-r--r--   0 dgilland   (501) staff       (20)     5991 2024-03-04 02:54:33.000000 pydash-8.0.0/tasks.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-03-27 02:49:21.298411 pydash-8.0.0/tests/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-23 03:21:55.000000 pydash-8.0.0/tests/__init__.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-03-27 02:49:21.283215 pydash-8.0.0/tests/build/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-03-27 02:49:21.298727 pydash-8.0.0/tests/build/testresults/
--rw-r--r--   0 dgilland   (501) staff       (20)      925 2023-04-06 01:12:00.000000 pydash-8.0.0/tests/build/testresults/junit.xml
--rw-r--r--   0 dgilland   (501) staff       (20)      143 2022-09-23 13:25:56.000000 pydash-8.0.0/tests/conftest.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1870 2022-09-23 13:11:57.000000 pydash-8.0.0/tests/helpers.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-03-27 02:49:21.301086 pydash-8.0.0/tests/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-8.0.0/tests/pytest_mypy_testing/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)    17272 2024-03-02 03:18:31.000000 pydash-8.0.0/tests/pytest_mypy_testing/test_arrays.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1087 2024-03-27 02:27:27.000000 pydash-8.0.0/tests/pytest_mypy_testing/test_chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)     8725 2024-03-02 03:18:31.000000 pydash-8.0.0/tests/pytest_mypy_testing/test_collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)     9870 2024-03-02 03:18:31.000000 pydash-8.0.0/tests/pytest_mypy_testing/test_functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     5582 2024-03-02 03:18:31.000000 pydash-8.0.0/tests/pytest_mypy_testing/test_numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    14701 2024-03-27 02:27:27.000000 pydash-8.0.0/tests/pytest_mypy_testing/test_objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    10786 2024-03-02 03:18:31.000000 pydash-8.0.0/tests/pytest_mypy_testing/test_predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)    13294 2024-03-02 03:18:31.000000 pydash-8.0.0/tests/pytest_mypy_testing/test_strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)     8601 2024-03-02 03:18:31.000000 pydash-8.0.0/tests/pytest_mypy_testing/test_utilities.py
--rw-r--r--   0 dgilland   (501) staff       (20)      178 2021-06-27 18:15:05.000000 pydash-8.0.0/tests/test_annotations.py
--rw-r--r--   0 dgilland   (501) staff       (20)    24162 2024-03-02 02:45:10.000000 pydash-8.0.0/tests/test_arrays.py
--rw-r--r--   0 dgilland   (501) staff       (20)     4052 2024-03-04 02:54:39.000000 pydash-8.0.0/tests/test_chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)    29669 2022-09-23 13:19:05.000000 pydash-8.0.0/tests/test_collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)    10861 2024-01-28 02:09:23.000000 pydash-8.0.0/tests/test_functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     7725 2024-03-02 02:45:10.000000 pydash-8.0.0/tests/test_numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    29228 2024-03-04 02:54:39.000000 pydash-8.0.0/tests/test_objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    13284 2024-03-02 02:45:10.000000 pydash-8.0.0/tests/test_predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)    33384 2024-03-02 04:23:13.000000 pydash-8.0.0/tests/test_strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)    18221 2023-03-18 22:34:56.000000 pydash-8.0.0/tests/test_utilities.py
--rw-r--r--   0 dgilland   (501) staff       (20)      299 2024-01-27 22:41:43.000000 pydash-8.0.0/tox.ini
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.952438 pydash-8.0.1/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.890843 pydash-8.0.1/.tox/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.872681 pydash-8.0.1/.tox/.pkg/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.872739 pydash-8.0.1/.tox/.pkg/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.872793 pydash-8.0.1/.tox/.pkg/lib/python3.12/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.874371 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.897864 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.873821 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.898152 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.898275 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.898373 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.898470 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.898562 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.898656 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.898758 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.898862 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.898967 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.899067 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.899162 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.899262 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.899539 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.873967 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.874303 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.899641 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:03.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.874129 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/jaraco/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.899735 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/jaraco/functools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:03.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/jaraco/functools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.899831 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:03.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.899924 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:03.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.900029 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:03.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.874418 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/setuptools/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.874819 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.900141 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:03.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.900242 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/importlib_resources/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:03.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.874637 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/jaraco/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.900337 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/jaraco/functools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:03.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/jaraco/functools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.900429 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:03.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.900519 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:03.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.900613 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:21:03.000000 pydash-8.0.1/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.874937 pydash-8.0.1/.tox/py310/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.874983 pydash-8.0.1/.tox/py310/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.875032 pydash-8.0.1/.tox/py310/lib/python3.10/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.878497 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.900943 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:30.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.901064 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2024-04-25 14:22:29.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.901334 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:31.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.901436 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:29.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.901539 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:29.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.901646 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:29.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.901759 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2024-04-25 14:22:29.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.902020 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:29.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.902125 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:29.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.902215 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:29.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.902304 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:30.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.902398 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:29.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.902497 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/invoke/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:29.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/invoke/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.876084 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/jaraco/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.902589 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/jaraco/classes/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:30.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/jaraco/classes/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.902720 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/jaraco/functools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:30.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/jaraco/functools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.902829 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:30.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.902932 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:31.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.903031 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:22:30.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.903279 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:29.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.903379 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:22:29.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.903598 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:29.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.903700 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2024-04-25 14:22:30.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.903900 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/nh3/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:28.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/nh3/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.903990 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:29.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.904082 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.877521 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.904325 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:21.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.904419 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:21.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.904512 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:21.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.904606 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:21.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.904701 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:21.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.904802 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:21.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.904898 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:21.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.904994 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:21.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.905084 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:21.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.905175 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:21.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.905280 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:21.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.905391 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:22:21.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.905675 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:21.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2024-04-25 14:22:21.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.905769 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:29.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.905866 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:29.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.905965 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pluggy/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:29.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pluggy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.906067 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-26 13:07:30.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.906177 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:30.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.906267 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:30.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.906363 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2024-04-25 14:22:31.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.906660 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:30.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.906757 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:31.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.906854 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/soupsieve/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:28.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.906956 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:31.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.907050 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:31.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.907144 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:22:28.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.907405 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:30.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.907520 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:31.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.907633 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/urllib3/
+-rw-r--r--   0 dgilland   (501) staff       (20)       93 2024-04-25 14:22:28.000000 pydash-8.0.1/.tox/py310/lib/python3.10/site-packages/urllib3/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.878612 pydash-8.0.1/.tox/py311/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.878657 pydash-8.0.1/.tox/py311/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.878704 pydash-8.0.1/.tox/py311/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.883105 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.907897 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:01.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.907990 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2024-04-25 14:23:00.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.908223 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:02.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.908319 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:00.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.908414 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:00.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.908512 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:00.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.908606 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2024-04-25 14:23:00.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.908871 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:00.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.908983 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:00.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.909082 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:02.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.909180 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:00.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.909278 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/invoke/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:00.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/invoke/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.879626 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/jaraco/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.909368 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/jaraco/classes/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:02.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/jaraco/classes/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.909459 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/jaraco/functools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:02.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/jaraco/functools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.909550 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:02.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.909653 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:03.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.909761 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:23:02.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.910034 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:00.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.910138 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:23:00.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.910389 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:00.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.910491 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2024-04-25 14:23:01.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.910728 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/nh3/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:59.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/nh3/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.910822 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:00.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.910913 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.881201 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.911183 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.911291 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.911401 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.911503 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.911601 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.911693 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.911788 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.911897 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.912011 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.912122 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.912216 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.912317 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.912599 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.881314 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pkg_resources/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.881544 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pkg_resources/_vendor/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.912713 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.912821 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.912922 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.913021 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.913112 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:00.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.913202 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:00.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.913294 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pluggy/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:00.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pluggy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.913389 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-26 13:07:50.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.913484 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:01.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.913577 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:01.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.913668 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2024-04-25 14:23:03.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.913926 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:01.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.914027 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:03.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.882267 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/setuptools/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.882665 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/setuptools/_vendor/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.914135 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.914235 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.914335 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.914429 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.914520 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:22:52.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.914809 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/soupsieve/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:59.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.914909 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:03.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.915002 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:03.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.915104 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:02.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.915205 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:03.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.915315 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/urllib3/
+-rw-r--r--   0 dgilland   (501) staff       (20)       93 2024-04-25 14:22:59.000000 pydash-8.0.1/.tox/py311/lib/python3.11/site-packages/urllib3/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.883232 pydash-8.0.1/.tox/py312/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.883284 pydash-8.0.1/.tox/py312/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.883337 pydash-8.0.1/.tox/py312/lib/python3.12/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.886704 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.915579 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:43.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.915682 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2024-04-25 14:23:42.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.915935 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:44.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.916045 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:42.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.916152 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:42.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.916264 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:42.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.916372 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2024-04-25 14:23:42.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.916642 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:42.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.916752 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:42.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.916860 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:44.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.916975 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:42.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.917077 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/invoke/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:42.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/invoke/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.884247 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/jaraco/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.917173 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/jaraco/classes/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:44.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/jaraco/classes/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.917281 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/jaraco/functools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:44.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/jaraco/functools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.917390 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:44.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.917500 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:45.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.917611 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:23:44.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.917882 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:42.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.917990 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:23:42.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.918214 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:42.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.918321 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2024-04-25 14:23:43.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.918586 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/nh3/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:40.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/nh3/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.918695 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:41.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.918812 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.885758 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.919085 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:33.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.919187 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:33.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.919292 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:33.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.919396 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:33.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.919495 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:33.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.919600 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:33.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.919718 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:33.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.919835 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:33.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.919946 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:33.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.920059 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:33.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.920162 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:33.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.920272 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:23:33.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.920564 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:33.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2024-04-25 14:23:33.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.920683 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:41.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.920802 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:41.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.920916 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pluggy/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:41.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pluggy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.921021 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-26 13:08:14.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.921134 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:43.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.921247 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:43.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.921342 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2024-04-25 14:23:45.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.921609 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:43.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.921712 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:45.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.921819 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/soupsieve/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:41.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.921924 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:44.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.922031 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:45.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.922127 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:44.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.922225 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:23:45.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.922324 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/urllib3/
+-rw-r--r--   0 dgilland   (501) staff       (20)       93 2024-04-25 14:23:40.000000 pydash-8.0.1/.tox/py312/lib/python3.12/site-packages/urllib3/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.886829 pydash-8.0.1/.tox/py38/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.886878 pydash-8.0.1/.tox/py38/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.886932 pydash-8.0.1/.tox/py38/lib/python3.8/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.890775 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.922569 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.922667 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.922916 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:16.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.923021 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.923123 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.923215 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.923307 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.923530 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.923623 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.923720 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.923821 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:15.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.923917 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/importlib_resources/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:15.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/importlib_resources/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.924014 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.924374 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/invoke/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/invoke/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.888035 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/jaraco/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.924477 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/jaraco/classes/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:15.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/jaraco/classes/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.924576 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/jaraco/functools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:15.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/jaraco/functools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.924671 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:15.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.924765 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:16.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.924859 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:21:15.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.925102 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.925193 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.925401 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.925493 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2024-04-25 14:21:15.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.925732 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/nh3/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:13.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/nh3/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.925830 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.925922 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.889734 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.926151 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.926247 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.926341 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.926436 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.926533 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.926622 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.926719 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.926813 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.926908 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.927004 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.927100 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.927193 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.927507 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2024-04-25 14:21:02.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.927621 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.927728 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.927832 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pluggy/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pluggy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.927928 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-26 13:06:42.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.928022 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:15.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.928121 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.928219 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2024-04-25 14:21:16.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.928484 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:14.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.928583 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:16.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.928680 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/soupsieve/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:13.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.928775 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:15.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.928870 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:16.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.928967 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:21:13.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.929229 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:15.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.929319 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:16.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.929414 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/urllib3/
+-rw-r--r--   0 dgilland   (501) staff       (20)       93 2024-04-25 14:21:13.000000 pydash-8.0.1/.tox/py38/lib/python3.8/site-packages/urllib3/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.890894 pydash-8.0.1/.tox/py39/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.890944 pydash-8.0.1/.tox/py39/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.890996 pydash-8.0.1/.tox/py39/lib/python3.9/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.894470 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.929705 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.929795 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.930030 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:01.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.930120 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.930210 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.930308 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.930404 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.930624 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.930723 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.930814 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.930910 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:00.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.931000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.931089 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/invoke/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/invoke/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.891960 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/jaraco/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.931179 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/jaraco/classes/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:00.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/jaraco/classes/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.931274 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/jaraco/functools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:00.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/jaraco/functools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.931363 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:00.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.931472 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:01.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.931566 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:22:00.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.931820 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.931924 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.932153 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.932245 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2024-04-25 14:22:00.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.932448 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/nh3/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:58.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/nh3/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.932542 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.932646 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.893448 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.932905 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:51.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.932998 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:51.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.933091 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:51.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.933188 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:51.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.933283 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:51.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.933379 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:51.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.933480 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:51.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.933576 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:51.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.933666 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:51.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.933760 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:51.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.933849 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:51.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.933943 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:21:51.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.934197 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:51.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2024-04-25 14:21:51.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.934295 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.934389 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.934487 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pluggy/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pluggy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.934575 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-26 13:07:10.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.934674 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:00.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.934774 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:00.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.934880 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2024-04-25 14:22:01.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.935137 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:59.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.935229 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:01.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.935319 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/soupsieve/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:21:58.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.935406 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:00.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.935496 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:01.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.935591 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2024-04-25 14:21:58.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.935850 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:00.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.935953 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2024-04-25 14:22:01.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.936056 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/urllib3/
+-rw-r--r--   0 dgilland   (501) staff       (20)       93 2024-04-25 14:21:58.000000 pydash-8.0.1/.tox/py39/lib/python3.9/site-packages/urllib3/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)     1396 2023-06-02 13:53:01.000000 pydash-8.0.1/AUTHORS.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)    42713 2024-04-26 13:11:15.000000 pydash-8.0.1/CHANGELOG.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2581 2020-10-29 15:03:50.000000 pydash-8.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     1072 2021-01-05 22:53:19.000000 pydash-8.0.1/LICENSE.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      283 2023-03-18 22:34:56.000000 pydash-8.0.1/MANIFEST.in
+-rw-r--r--   0 dgilland   (501) staff       (20)     4468 2024-04-26 13:23:42.952209 pydash-8.0.1/PKG-INFO
+-rw-r--r--   0 dgilland   (501) staff       (20)     1262 2023-10-03 02:32:14.000000 pydash-8.0.1/README.rst
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.939054 pydash-8.0.1/docs/
+-rw-r--r--   0 dgilland   (501) staff       (20)     3937 2019-02-04 01:30:20.000000 pydash-8.0.1/docs/Makefile
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.939192 pydash-8.0.1/docs/_templates/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-8.0.1/docs/_templates/.gitignore
+-rw-r--r--   0 dgilland   (501) staff       (20)     2885 2019-02-04 01:30:20.000000 pydash-8.0.1/docs/api.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       28 2014-07-29 03:38:06.000000 pydash-8.0.1/docs/authors.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     4065 2019-02-04 01:30:20.000000 pydash-8.0.1/docs/callbacks.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2927 2021-09-28 21:40:18.000000 pydash-8.0.1/docs/chaining.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       30 2019-02-04 01:30:20.000000 pydash-8.0.1/docs/changelog.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     5116 2024-03-02 04:24:04.000000 pydash-8.0.1/docs/conf.py
+-rw-r--r--   0 dgilland   (501) staff       (20)       33 2014-07-29 03:34:57.000000 pydash-8.0.1/docs/contributing.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      760 2019-02-04 01:30:20.000000 pydash-8.0.1/docs/deeppath.rst
+-rw-rw-r--   0 dgilland   (501) staff       (20)       29 2020-10-28 20:30:40.000000 pydash-8.0.1/docs/devguide.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2045 2019-02-04 01:30:20.000000 pydash-8.0.1/docs/differences.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      605 2020-10-29 19:54:30.000000 pydash-8.0.1/docs/index.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      187 2021-06-27 18:15:05.000000 pydash-8.0.1/docs/installation.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      100 2019-02-04 01:30:20.000000 pydash-8.0.1/docs/kudos.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       45 2021-01-05 22:53:19.000000 pydash-8.0.1/docs/license.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     1499 2019-02-04 01:30:20.000000 pydash-8.0.1/docs/quickstart.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      562 2019-02-04 01:30:20.000000 pydash-8.0.1/docs/templating.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)    10538 2019-02-04 01:30:20.000000 pydash-8.0.1/docs/upgrading.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      497 2014-08-20 02:16:49.000000 pydash-8.0.1/docs/versioning.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     3851 2024-04-26 13:12:28.000000 pydash-8.0.1/pyproject.toml
+-rw-r--r--   0 dgilland   (501) staff       (20)       10 2020-10-28 20:38:46.000000 pydash-8.0.1/requirements.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)       38 2024-04-26 13:23:42.952485 pydash-8.0.1/setup.cfg
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.894783 pydash-8.0.1/src/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.943071 pydash-8.0.1/src/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)    11706 2024-04-26 13:11:23.000000 pydash-8.0.1/src/pydash/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    71289 2024-03-02 04:23:13.000000 pydash-8.0.1/src/pydash/arrays.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.945189 pydash-8.0.1/src/pydash/chaining/
+-rw-r--r--   0 dgilland   (501) staff       (20)       93 2024-03-04 02:54:39.000000 pydash-8.0.1/src/pydash/chaining/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1364 2023-03-20 14:30:38.000000 pydash-8.0.1/src/pydash/chaining/all_funcs.py
+-rw-r--r--   0 dgilland   (501) staff       (20)   130387 2024-03-04 02:54:39.000000 pydash-8.0.1/src/pydash/chaining/all_funcs.pyi
+-rw-r--r--   0 dgilland   (501) staff       (20)     7704 2024-03-04 02:54:39.000000 pydash-8.0.1/src/pydash/chaining/chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    54132 2024-03-02 04:23:13.000000 pydash-8.0.1/src/pydash/collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      431 2023-03-18 22:34:56.000000 pydash-8.0.1/src/pydash/exceptions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    40643 2024-03-02 04:23:13.000000 pydash-8.0.1/src/pydash/functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     9498 2024-04-25 14:27:07.000000 pydash-8.0.1/src/pydash/helpers.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    26839 2024-03-02 04:23:13.000000 pydash-8.0.1/src/pydash/numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    65283 2024-03-04 02:54:39.000000 pydash-8.0.1/src/pydash/objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    33711 2024-03-02 04:23:13.000000 pydash-8.0.1/src/pydash/predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-8.0.1/src/pydash/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)    57917 2024-03-02 04:23:13.000000 pydash-8.0.1/src/pydash/strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      550 2024-03-02 04:23:13.000000 pydash-8.0.1/src/pydash/types.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    38266 2024-03-02 04:23:13.000000 pydash-8.0.1/src/pydash/utilities.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.951296 pydash-8.0.1/src/pydash.egg-info/
+-rw-r--r--   0 dgilland   (501) staff       (20)     4468 2024-04-26 13:23:41.000000 pydash-8.0.1/src/pydash.egg-info/PKG-INFO
+-rw-r--r--   0 dgilland   (501) staff       (20)    20691 2024-04-26 13:23:42.000000 pydash-8.0.1/src/pydash.egg-info/SOURCES.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)        1 2024-04-26 13:23:41.000000 pydash-8.0.1/src/pydash.egg-info/dependency_links.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)      161 2024-04-26 13:23:41.000000 pydash-8.0.1/src/pydash.egg-info/requires.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)        7 2024-04-26 13:23:41.000000 pydash-8.0.1/src/pydash.egg-info/top_level.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)     5991 2024-03-04 02:54:33.000000 pydash-8.0.1/tasks.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.948689 pydash-8.0.1/tests/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-23 03:21:55.000000 pydash-8.0.1/tests/__init__.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.895027 pydash-8.0.1/tests/build/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.949000 pydash-8.0.1/tests/build/testresults/
+-rw-r--r--   0 dgilland   (501) staff       (20)      925 2023-04-06 01:12:00.000000 pydash-8.0.1/tests/build/testresults/junit.xml
+-rw-r--r--   0 dgilland   (501) staff       (20)      143 2022-09-23 13:25:56.000000 pydash-8.0.1/tests/conftest.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1870 2022-09-23 13:11:57.000000 pydash-8.0.1/tests/helpers.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2024-04-26 13:23:42.951115 pydash-8.0.1/tests/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-8.0.1/tests/pytest_mypy_testing/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    17272 2024-03-02 03:18:31.000000 pydash-8.0.1/tests/pytest_mypy_testing/test_arrays.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1087 2024-03-27 02:27:27.000000 pydash-8.0.1/tests/pytest_mypy_testing/test_chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8725 2024-03-02 03:18:31.000000 pydash-8.0.1/tests/pytest_mypy_testing/test_collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     9870 2024-03-02 03:18:31.000000 pydash-8.0.1/tests/pytest_mypy_testing/test_functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     5582 2024-03-02 03:18:31.000000 pydash-8.0.1/tests/pytest_mypy_testing/test_numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    14701 2024-03-27 02:27:27.000000 pydash-8.0.1/tests/pytest_mypy_testing/test_objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    10786 2024-03-02 03:18:31.000000 pydash-8.0.1/tests/pytest_mypy_testing/test_predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    13294 2024-03-02 03:18:31.000000 pydash-8.0.1/tests/pytest_mypy_testing/test_strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8601 2024-03-02 03:18:31.000000 pydash-8.0.1/tests/pytest_mypy_testing/test_utilities.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      178 2021-06-27 18:15:05.000000 pydash-8.0.1/tests/test_annotations.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    24162 2024-03-02 02:45:10.000000 pydash-8.0.1/tests/test_arrays.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     4052 2024-03-04 02:54:39.000000 pydash-8.0.1/tests/test_chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    30120 2024-04-26 13:06:28.000000 pydash-8.0.1/tests/test_collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    10861 2024-01-28 02:09:23.000000 pydash-8.0.1/tests/test_functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     7725 2024-03-02 02:45:10.000000 pydash-8.0.1/tests/test_numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    29228 2024-03-04 02:54:39.000000 pydash-8.0.1/tests/test_objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    13284 2024-03-02 02:45:10.000000 pydash-8.0.1/tests/test_predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    33384 2024-03-02 04:23:13.000000 pydash-8.0.1/tests/test_strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    18221 2023-03-18 22:34:56.000000 pydash-8.0.1/tests/test_utilities.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      299 2024-01-27 22:41:43.000000 pydash-8.0.1/tox.ini
```

### Comparing `pydash-8.0.0/AUTHORS.rst` & `pydash-8.0.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/CHANGELOG.rst` & `pydash-8.0.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. _changelog:
 
 Changelog
 =========
 
+v8.0.1 (2024-04-26)
+-------------------
+
+- Fix issue where too many arguments were passed to stdlib's ``operator.attrgetter``, ``operator.itemgetter``, and ``operator.methodcaller`` when instances of those classes were used as callbacks to functions like ``map_``, ``filter_``, etc. due to a bug introduced in Python 3.12.3 and 3.11.9 that reported an incorrect signature for those ``operator`` class instances.
+
+
 v8.0.0 (2024-03-26)
 -------------------
 
 - Add functions (Thanks DeviousStoat_!):
 
   - ``apply`` (previously named ``thru``)
   - ``apply_catch``
```

### Comparing `pydash-8.0.0/CONTRIBUTING.rst` & `pydash-8.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/LICENSE.rst` & `pydash-8.0.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/PKG-INFO` & `pydash-8.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash
-Version: 8.0.0
+Version: 8.0.1
 Summary: The kitchen sink of Python utility libraries for doing "stuff" in a functional way. Based on the Lo-Dash Javascript library.
 Author-email: Derrick Gilland <dgilland@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Derrick Gilland
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pydash-8.0.0/README.rst` & `pydash-8.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/docs/Makefile` & `pydash-8.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/docs/api.rst` & `pydash-8.0.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/docs/callbacks.rst` & `pydash-8.0.1/docs/callbacks.rst`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/docs/chaining.rst` & `pydash-8.0.1/docs/chaining.rst`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/docs/conf.py` & `pydash-8.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/docs/deeppath.rst` & `pydash-8.0.1/docs/deeppath.rst`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/docs/differences.rst` & `pydash-8.0.1/docs/differences.rst`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/docs/index.rst` & `pydash-8.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/docs/quickstart.rst` & `pydash-8.0.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/docs/templating.rst` & `pydash-8.0.1/docs/templating.rst`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/docs/upgrading.rst` & `pydash-8.0.1/docs/upgrading.rst`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/pyproject.toml` & `pydash-8.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/src/pydash/__init__.py` & `pydash-8.0.1/src/pydash/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Python port of Lo-Dash."""
 
-__version__ = "8.0.0"
+__version__ = "8.0.1"
 
 from .arrays import (
     chunk,
     compact,
     concat,
     difference,
     difference_by,
```

### Comparing `pydash-8.0.0/src/pydash/arrays.py` & `pydash-8.0.1/src/pydash/arrays.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/src/pydash/chaining/all_funcs.py` & `pydash-8.0.1/src/pydash/chaining/all_funcs.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/src/pydash/chaining/all_funcs.pyi` & `pydash-8.0.1/src/pydash/chaining/all_funcs.pyi`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/src/pydash/chaining/chaining.py` & `pydash-8.0.1/src/pydash/chaining/chaining.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/src/pydash/collections.py` & `pydash-8.0.1/src/pydash/collections.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/src/pydash/functions.py` & `pydash-8.0.1/src/pydash/functions.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/src/pydash/helpers.py` & `pydash-8.0.1/src/pydash/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Generic utility methods not part of main API."""
 
 import builtins
 from collections.abc import Hashable, Iterable, Mapping, Sequence
 from decimal import Decimal
 from functools import wraps
 import inspect
-from inspect import getfullargspec
+import operator
 import warnings
 
 import pydash as pyd
 
 
 #: Singleton object that differentiates between an explicit ``None`` value and an unset value.
 #: As a class so it has its own type
@@ -68,27 +68,33 @@
 
     try:
         # PY2: inspect.signature was added in Python 3.
         # Try to use inspect.signature when possible since it works better for our purpose of
         # getting the iteratee argcount since it takes into account the "self" argument in callable
         # classes.
         sig = inspect.signature(iteratee)
-    except (TypeError, ValueError, AttributeError):
+    except (TypeError, ValueError, AttributeError):  # pragma: no cover
         pass
-    else:  # pragma: no cover
+    else:
         if not any(
             param.kind == inspect.Parameter.VAR_POSITIONAL for param in sig.parameters.values()
         ):
             argcount = len(sig.parameters)
 
     if argcount is None:
-        argspec = getfullargspec(iteratee)
-        if argspec and not argspec.varargs:  # pragma: no cover
-            # Use inspected arg count.
-            argcount = len(argspec.args)
+        # Signatures were added these operator methods in Python 3.12.3 and 3.11.9 but their
+        # instance objects are incorrectly reported as accepting varargs when they only accept a
+        # single argument.
+        if isinstance(iteratee, (operator.itemgetter, operator.attrgetter, operator.methodcaller)):
+            argcount = 1
+        else:
+            argspec = inspect.getfullargspec(iteratee)
+            if argspec and not argspec.varargs:  # pragma: no cover
+                # Use inspected arg count.
+                argcount = len(argspec.args)
 
     if argcount is None:
         # Assume all args are handleable.
         argcount = maxargs
 
     return argcount
```

### Comparing `pydash-8.0.0/src/pydash/numerical.py` & `pydash-8.0.1/src/pydash/numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/src/pydash/objects.py` & `pydash-8.0.1/src/pydash/objects.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/src/pydash/predicates.py` & `pydash-8.0.1/src/pydash/predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/src/pydash/strings.py` & `pydash-8.0.1/src/pydash/strings.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/src/pydash/types.py` & `pydash-8.0.1/src/pydash/types.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/src/pydash/utilities.py` & `pydash-8.0.1/src/pydash/utilities.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/src/pydash.egg-info/PKG-INFO` & `pydash-8.0.1/src/pydash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash
-Version: 8.0.0
+Version: 8.0.1
 Summary: The kitchen sink of Python utility libraries for doing "stuff" in a functional way. Based on the Lo-Dash Javascript library.
 Author-email: Derrick Gilland <dgilland@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Derrick Gilland
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pydash-8.0.0/tasks.py` & `pydash-8.0.1/tasks.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/build/testresults/junit.xml` & `pydash-8.0.1/tests/build/testresults/junit.xml`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/helpers.py` & `pydash-8.0.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/pytest_mypy_testing/test_arrays.py` & `pydash-8.0.1/tests/pytest_mypy_testing/test_arrays.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/pytest_mypy_testing/test_chaining.py` & `pydash-8.0.1/tests/pytest_mypy_testing/test_chaining.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/pytest_mypy_testing/test_collections.py` & `pydash-8.0.1/tests/pytest_mypy_testing/test_collections.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/pytest_mypy_testing/test_functions.py` & `pydash-8.0.1/tests/pytest_mypy_testing/test_functions.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/pytest_mypy_testing/test_numerical.py` & `pydash-8.0.1/tests/pytest_mypy_testing/test_numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/pytest_mypy_testing/test_objects.py` & `pydash-8.0.1/tests/pytest_mypy_testing/test_objects.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/pytest_mypy_testing/test_predicates.py` & `pydash-8.0.1/tests/pytest_mypy_testing/test_predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/pytest_mypy_testing/test_strings.py` & `pydash-8.0.1/tests/pytest_mypy_testing/test_strings.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/pytest_mypy_testing/test_utilities.py` & `pydash-8.0.1/tests/pytest_mypy_testing/test_utilities.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/test_arrays.py` & `pydash-8.0.1/tests/test_arrays.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/test_chaining.py` & `pydash-8.0.1/tests/test_chaining.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/test_collections.py` & `pydash-8.0.1/tests/test_collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import namedtuple
 import math
-from operator import itemgetter
+from operator import attrgetter, itemgetter, methodcaller
 
 import pytest
 
 import pydash as _
 
 from . import helpers
 
@@ -319,14 +319,30 @@
             (
                 [{"a": 1, "b": 2, "c": -1}, {"a": 3, "b": 4, "c": -1}, {"a": 5, "b": 6, "c": -1}],
                 itemgetter("a", "b"),
             ),
             [(1, 2), (3, 4), (5, 6)],
             False,
         ),
+        (
+            (
+                [helpers.Object(a=1, b=2, c=-1), helpers.Object(a=3, b=4, c=-1)],
+                attrgetter("a", "b"),
+            ),
+            [(1, 2), (3, 4)],
+            False,
+        ),
+        (
+            (
+                [{"a": 1, "b": 2, "c": -1}, {"a": 3, "b": 4}, {"a": 5}],
+                methodcaller("__len__"),
+            ),
+            [3, 2, 1],
+            False,
+        ),
     ],
 )
 def test_map_(case, expected, sort_results):
     actual = _.map_(*case)
 
     if sort_results:
         actual = sorted(actual)
```

### Comparing `pydash-8.0.0/tests/test_functions.py` & `pydash-8.0.1/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/test_numerical.py` & `pydash-8.0.1/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/test_objects.py` & `pydash-8.0.1/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/test_predicates.py` & `pydash-8.0.1/tests/test_predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/test_strings.py` & `pydash-8.0.1/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `pydash-8.0.0/tests/test_utilities.py` & `pydash-8.0.1/tests/test_utilities.py`

 * *Files identical despite different names*

