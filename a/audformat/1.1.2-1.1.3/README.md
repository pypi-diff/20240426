# Comparing `tmp/audformat-1.1.2.tar.gz` & `tmp/audformat-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audformat-1.1.2.tar", last modified: Fri Feb  2 15:22:36 2024, max compression
+gzip compressed data, was "audformat-1.1.3.tar", last modified: Fri Apr 26 10:58:56 2024, max compression
```

## Comparing `audformat-1.1.2.tar` & `audformat-1.1.3.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:22:36.214016 audformat-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:22:36.194016 audformat-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:22:36.198016 audformat-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-02-02 15:22:27.000000 audformat-1.1.2/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-02 15:22:27.000000 audformat-1.1.2/.github/workflows/linter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-02-02 15:22:27.000000 audformat-1.1.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-02-02 15:22:27.000000 audformat-1.1.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-02 15:22:27.000000 audformat-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-02-02 15:22:27.000000 audformat-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15743 2024-02-02 15:22:27.000000 audformat-1.1.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-02-02 15:22:27.000000 audformat-1.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-02-02 15:22:27.000000 audformat-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-02-02 15:22:36.214016 audformat-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-02-02 15:22:27.000000 audformat-1.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:22:36.198016 audformat-1.1.2/audformat/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:22:36.202016 audformat-1.1.2/audformat/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/core/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/core/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/core/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/core/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    58342 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/core/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/core/define.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/core/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/core/media.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/core/rater.py
--rw-r--r--   0 runner    (1001) docker     (127)    17718 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/core/scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/core/split.py
--rw-r--r--   0 runner    (1001) docker     (127)    49501 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/core/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    13655 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/core/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    65702 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:22:36.202016 audformat-1.1.2/audformat/define/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/define/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:22:36.202016 audformat-1.1.2/audformat/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/errors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:22:36.202016 audformat-1.1.2/audformat/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:22:36.202016 audformat-1.1.2/audformat/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-02-02 15:22:27.000000 audformat-1.1.2/audformat/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:22:36.214016 audformat-1.1.2/audformat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-02-02 15:22:36.000000 audformat-1.1.2/audformat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-02-02 15:22:36.000000 audformat-1.1.2/audformat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 15:22:36.000000 audformat-1.1.2/audformat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-02 15:22:36.000000 audformat-1.1.2/audformat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-02 15:22:36.000000 audformat-1.1.2/audformat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:22:36.206016 audformat-1.1.2/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-02-02 15:22:27.000000 audformat-1.1.2/benchmarks/benchmark_union.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:22:36.210016 audformat-1.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/accessing-data.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:22:36.210016 audformat-1.1.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/api/audformat.define.rst
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/api/audformat.errors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/api/audformat.rst
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/api/audformat.testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/api/audformat.utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:22:36.210016 audformat-1.1.2/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/api-src/audformat.define.rst
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/api-src/audformat.errors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/api-src/audformat.rst
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/api-src/audformat.testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/api-src/audformat.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/combine-tables.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/create-database.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/data-conventions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/data-example.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/data-format.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/data-header.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/data-introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/data-misc-tables.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/data-tables.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/emodb-example.rst
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/map-scheme.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:22:36.210016 audformat-1.1.2/docs/pics/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/pics/audformat-database.dot
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/pics/audformat-misc-table.dot
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/pics/audformat-table.dot
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-02-02 15:22:27.000000 audformat-1.1.2/docs/update-database.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-02-02 15:22:27.000000 audformat-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-02 15:22:27.000000 audformat-1.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-02 15:22:36.214016 audformat-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:22:36.214016 audformat-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-02-02 15:22:27.000000 audformat-1.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-02 15:22:27.000000 audformat-1.1.2/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-02-02 15:22:27.000000 audformat-1.1.2/tests/test_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    23286 2024-02-02 15:22:27.000000 audformat-1.1.2/tests/test_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-02-02 15:22:27.000000 audformat-1.1.2/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    27063 2024-02-02 15:22:27.000000 audformat-1.1.2/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    43614 2024-02-02 15:22:27.000000 audformat-1.1.2/tests/test_database_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-02-02 15:22:27.000000 audformat-1.1.2/tests/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-02-02 15:22:27.000000 audformat-1.1.2/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-02-02 15:22:27.000000 audformat-1.1.2/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    46698 2024-02-02 15:22:27.000000 audformat-1.1.2/tests/test_misc_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    22998 2024-02-02 15:22:27.000000 audformat-1.1.2/tests/test_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)    55994 2024-02-02 15:22:27.000000 audformat-1.1.2/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    70025 2024-02-02 15:22:27.000000 audformat-1.1.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    54334 2024-02-02 15:22:27.000000 audformat-1.1.2/tests/test_utils_concat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.346547 audformat-1.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.326547 audformat-1.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.330547 audformat-1.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-26 10:58:48.000000 audformat-1.1.3/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-26 10:58:48.000000 audformat-1.1.3/.github/workflows/linter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-26 10:58:48.000000 audformat-1.1.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-26 10:58:48.000000 audformat-1.1.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-26 10:58:48.000000 audformat-1.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-26 10:58:48.000000 audformat-1.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15990 2024-04-26 10:58:48.000000 audformat-1.1.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-26 10:58:48.000000 audformat-1.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-26 10:58:48.000000 audformat-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-26 10:58:56.346547 audformat-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-26 10:58:48.000000 audformat-1.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.330547 audformat-1.1.3/audformat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.334547 audformat-1.1.3/audformat/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58342 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/define.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/rater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17718 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49501 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13655 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66906 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.334547 audformat-1.1.3/audformat/define/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/define/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.334547 audformat-1.1.3/audformat/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/errors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.334547 audformat-1.1.3/audformat/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.334547 audformat-1.1.3/audformat/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.346547 audformat-1.1.3/audformat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-26 10:58:56.000000 audformat-1.1.3/audformat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-26 10:58:56.000000 audformat-1.1.3/audformat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:58:56.000000 audformat-1.1.3/audformat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-26 10:58:56.000000 audformat-1.1.3/audformat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 10:58:56.000000 audformat-1.1.3/audformat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.334547 audformat-1.1.3/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-26 10:58:48.000000 audformat-1.1.3/benchmarks/benchmark_union.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.338547 audformat-1.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/accessing-data.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.338547 audformat-1.1.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api/audformat.define.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api/audformat.errors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api/audformat.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api/audformat.testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api/audformat.utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.342547 audformat-1.1.3/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api-src/audformat.define.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api-src/audformat.errors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api-src/audformat.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api-src/audformat.testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api-src/audformat.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/combine-tables.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/create-database.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/data-conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/data-example.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/data-format.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/data-header.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/data-introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/data-misc-tables.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/data-tables.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/emodb-example.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/map-scheme.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.342547 audformat-1.1.3/docs/pics/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/pics/audformat-database.dot
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/pics/audformat-misc-table.dot
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/pics/audformat-table.dot
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/update-database.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-26 10:58:48.000000 audformat-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 10:58:48.000000 audformat-1.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 10:58:56.346547 audformat-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.346547 audformat-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23286 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27063 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43614 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_database_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46698 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_misc_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22998 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55994 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71995 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54334 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_utils_concat.py
```

### Comparing `audformat-1.1.2/.github/workflows/doc.yml` & `audformat-1.1.3/.github/workflows/doc.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,24 @@
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ ubuntu-latest ]
         python-version: [ '3.10' ]
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Cache emodb
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: emodb-src
         key: emodb-ubuntu
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Ubuntu - install graphviz
       run: |
         sudo apt-get update
         sudo apt-get install --yes graphviz
```

### Comparing `audformat-1.1.2/.github/workflows/publish.yml` & `audformat-1.1.3/.github/workflows/publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -12,26 +12,26 @@
     permissions:
       contents: write
       id-token: write
     concurrency:
       group: ${{ github.workflow }}-${{ github.ref }}
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         fetch-depth: 2
 
     - name: Cache emodb
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: emodb-src
         key: emodb-ubuntu
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.10'
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build virtualenv
@@ -77,14 +77,14 @@
           echo 'body<<EOF'
           echo "$CHANGELOG"
           echo EOF
         } >> "$GITHUB_OUTPUT"
 
     - name: Create release on Github
       id: create_release
-      uses: softprops/action-gh-release@v1
+      uses: softprops/action-gh-release@v2
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       with:
         tag_name: ${{ github.ref }}
         name: Release ${{ github.ref_name }}
         body: ${{ steps.changelog.outputs.body }}
```

### Comparing `audformat-1.1.2/.github/workflows/test.yml` & `audformat-1.1.3/.github/workflows/test.yml`

 * *Files 9% similar despite different names*

```diff
@@ -19,25 +19,25 @@
             python-version: '3.8'
           - os: ubuntu-latest
             python-version: '3.9'
           - os: ubuntu-latest
             python-version: '3.11'
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Cache emodb
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: emodb-src
         key: emodb-ubuntu
       if: matrix.os == 'ubuntu-20.04'
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Prepare Ubuntu
       run: |
         sudo apt-get update
         sudo apt-get install --no-install-recommends --yes libsndfile1
@@ -51,12 +51,12 @@
         pip install -r tests/requirements.txt
 
     - name: Test with pytest
       run: |
         python -m pytest
 
     - name: Upload coverage to Codecov
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         file: ./coverage.xml
       if: matrix.os == 'ubuntu-20.04'
```

### Comparing `audformat-1.1.2/.pre-commit-config.yaml` & `audformat-1.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/CHANGELOG.rst` & `audformat-1.1.3/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,25 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.1.3 (2024-04-26)
+--------------------------
+
+* Added: ``as_dataframe`` argument
+  to ``audformat.utils.read_csv()``
+* Fixed: ``audformat.utils.read_csv()``
+  now treats float/integer values
+  in ``start``, ``end`` columns
+  as seconds
+
+
 Version 1.1.2 (2024-02-02)
 --------------------------
 
 * Fixed: ``audformat.Database.load()``
   when loading databases
   with a misc table
   that has an assigned split
```

### Comparing `audformat-1.1.2/CONTRIBUTING.rst` & `audformat-1.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/LICENSE` & `audformat-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/PKG-INFO` & `audformat-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audformat
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python implementation of audformat
 Author: BahaEddine Abrougui
 Author-email: Hagen Wierstorf <hwierstorf@audeering.com>, Johannes Wagner <jwagner@audeering.com>
 License: MIT License
         
         Copyright (c) 2018-present audEERING GmbH and Contributors
```

### Comparing `audformat-1.1.2/README.rst` & `audformat-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/audformat/__init__.py` & `audformat-1.1.3/audformat/__init__.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/audformat/core/attachment.py` & `audformat-1.1.3/audformat/core/attachment.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/audformat/core/column.py` & `audformat-1.1.3/audformat/core/column.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/audformat/core/common.py` & `audformat-1.1.3/audformat/core/common.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/audformat/core/conftest.py` & `audformat-1.1.3/audformat/core/conftest.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/audformat/core/database.py` & `audformat-1.1.3/audformat/core/database.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/audformat/core/define.py` & `audformat-1.1.3/audformat/core/define.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/audformat/core/errors.py` & `audformat-1.1.3/audformat/core/errors.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/audformat/core/index.py` & `audformat-1.1.3/audformat/core/index.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/audformat/core/media.py` & `audformat-1.1.3/audformat/core/media.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/audformat/core/rater.py` & `audformat-1.1.3/audformat/core/rater.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/audformat/core/scheme.py` & `audformat-1.1.3/audformat/core/scheme.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/audformat/core/split.py` & `audformat-1.1.3/audformat/core/split.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/audformat/core/table.py` & `audformat-1.1.3/audformat/core/table.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/audformat/core/testing.py` & `audformat-1.1.3/audformat/core/testing.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/audformat/core/utils.py` & `audformat-1.1.3/audformat/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1257,80 +1257,105 @@
         raise ValueError(f"'{language}' is not supported by ISO 639-3.")
 
     return result
 
 
 def read_csv(
     *args,
+    as_dataframe: bool = False,
     **kwargs,
 ) -> typing.Union[pd.Index, pd.Series, pd.DataFrame]:
     r"""Read object from CSV file.
 
     Automatically detects the index type and returns an object that is
     conform to :ref:`table specifications <data-tables:Tables>`.
     If conversion is not possible, an error is raised.
 
-    See :meth:`pandas.read_csv` for supported arguments.
+    Time values for the ``start`` and ``end`` column
+    are converted using :func:`pandas.to_timedelta`,
+    whereby float and integers are treated as seconds.
+
 
     Args:
-        *args: arguments
-        **kwargs: keyword arguments
+        *args: arguments passed on to :func:`pandas.read_csv`
+        as_dataframe: if ``False``,
+            a dataframe is only returned for data with two or more columns,
+            a series for data with one column,
+            an index for data with zero columns
+        **kwargs: keyword arguments passed on to :func:`pandas.read_csv`
 
     Returns:
         object conform to :ref:`table specifications <data-tables:Tables>`
 
     Raises:
         ValueError: if CSV file is not conform to
             :ref:`table specifications <data-tables:Tables>`
 
     Examples:
-        >>> from io import StringIO
-        >>> string = StringIO(
-        ...     '''file,start,end,value
+        >>> string = '''file,start,end,value
         ... f1,00:00:00,00:00:01,0.0
         ... f1,00:00:01,00:00:02,1.0
         ... f2,00:00:02,00:00:03,2.0'''
-        ... )
-        >>> read_csv(string)
+        >>> with open("file.csv", "w") as file:
+        ...     _ = file.write(string)
+        >>> read_csv("file.csv")
+        file  start            end
+        f1    0 days 00:00:00  0 days 00:00:01    0.0
+              0 days 00:00:01  0 days 00:00:02    1.0
+        f2    0 days 00:00:02  0 days 00:00:03    2.0
+        Name: value, dtype: float64
+        >>> string = '''file,start,end,value
+        ... f1,0,1,0.0
+        ... f1,1,2,1.0
+        ... f2,2,3,2.0'''
+        >>> with open("file.csv", "w") as file:
+        ...     _ = file.write(string)
+        >>> read_csv("file.csv")
         file  start            end
         f1    0 days 00:00:00  0 days 00:00:01    0.0
               0 days 00:00:01  0 days 00:00:02    1.0
         f2    0 days 00:00:02  0 days 00:00:03    2.0
         Name: value, dtype: float64
+        >>> read_csv("file.csv", as_dataframe=True)
+                                              value
+        file start           end
+        f1   0 days 00:00:00 0 days 00:00:01    0.0
+             0 days 00:00:01 0 days 00:00:02    1.0
+        f2   0 days 00:00:02 0 days 00:00:03    2.0
 
     """
     frame = pd.read_csv(*args, **kwargs)
 
     drop = [define.IndexField.FILE]
     if define.IndexField.FILE in frame.columns:
         files = frame[define.IndexField.FILE].astype("string")
     else:
         raise ValueError("Index not conform to audformat.")
 
     starts = None
     if define.IndexField.START in frame.columns:
-        starts = pd.to_timedelta(frame[define.IndexField.START])
+        starts = frame[define.IndexField.START]
         drop.append(define.IndexField.START)
 
     ends = None
     if define.IndexField.END in frame.columns:
-        ends = pd.to_timedelta(frame[define.IndexField.END])
+        ends = frame[define.IndexField.END]
         drop.append(define.IndexField.END)
 
     if starts is None and ends is None:
         index = filewise_index(files)
     else:
         index = segmented_index(files, starts=starts, ends=ends)
     frame.drop(drop, axis="columns", inplace=True)
 
-    if len(frame.columns) == 0:
+    if len(frame.columns) == 0 and not as_dataframe:
         return index
 
     frame = frame.set_index(index)
-    if len(frame.columns) == 1:
+    if len(frame.columns) == 1 and not as_dataframe:
         return frame[frame.columns[0]]
     else:
         return frame
 
 
 def replace_file_extension(
     index: pd.Index,
```

### Comparing `audformat-1.1.2/audformat/utils/__init__.py` & `audformat-1.1.3/audformat/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/audformat.egg-info/PKG-INFO` & `audformat-1.1.3/audformat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audformat
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python implementation of audformat
 Author: BahaEddine Abrougui
 Author-email: Hagen Wierstorf <hwierstorf@audeering.com>, Johannes Wagner <jwagner@audeering.com>
 License: MIT License
         
         Copyright (c) 2018-present audEERING GmbH and Contributors
```

### Comparing `audformat-1.1.2/audformat.egg-info/SOURCES.txt` & `audformat-1.1.3/audformat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/benchmarks/benchmark_union.py` & `audformat-1.1.3/benchmarks/benchmark_union.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/accessing-data.rst` & `audformat-1.1.3/docs/accessing-data.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/api/audformat.define.rst` & `audformat-1.1.3/docs/api/audformat.define.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/api/audformat.testing.rst` & `audformat-1.1.3/docs/api/audformat.testing.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/api-src/audformat.define.rst` & `audformat-1.1.3/docs/api-src/audformat.define.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/api-src/audformat.testing.rst` & `audformat-1.1.3/docs/api-src/audformat.testing.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/combine-tables.rst` & `audformat-1.1.3/docs/combine-tables.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/conf.py` & `audformat-1.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/create-database.rst` & `audformat-1.1.3/docs/create-database.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/data-conventions.rst` & `audformat-1.1.3/docs/data-conventions.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/data-example.rst` & `audformat-1.1.3/docs/data-example.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/data-format.rst` & `audformat-1.1.3/docs/data-format.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/data-header.rst` & `audformat-1.1.3/docs/data-header.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/data-introduction.rst` & `audformat-1.1.3/docs/data-introduction.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/data-misc-tables.rst` & `audformat-1.1.3/docs/data-misc-tables.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/data-tables.rst` & `audformat-1.1.3/docs/data-tables.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/emodb-example.rst` & `audformat-1.1.3/docs/emodb-example.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/index.rst` & `audformat-1.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/map-scheme.rst` & `audformat-1.1.3/docs/map-scheme.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/pics/audformat-database.dot` & `audformat-1.1.3/docs/pics/audformat-database.dot`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/docs/update-database.rst` & `audformat-1.1.3/docs/update-database.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/pyproject.toml` & `audformat-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/tests/conftest.py` & `audformat-1.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/tests/test_attachment.py` & `audformat-1.1.3/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/tests/test_column.py` & `audformat-1.1.3/tests/test_column.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/tests/test_common.py` & `audformat-1.1.3/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/tests/test_database.py` & `audformat-1.1.3/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/tests/test_database_get.py` & `audformat-1.1.3/tests/test_database_get.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/tests/test_eq.py` & `audformat-1.1.3/tests/test_eq.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/tests/test_errors.py` & `audformat-1.1.3/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/tests/test_index.py` & `audformat-1.1.3/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/tests/test_misc_table.py` & `audformat-1.1.3/tests/test_misc_table.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/tests/test_scheme.py` & `audformat-1.1.3/tests/test_scheme.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/tests/test_table.py` & `audformat-1.1.3/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.2/tests/test_utils.py` & `audformat-1.1.3/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1459,14 +1459,31 @@
                     ends=pd.to_timedelta([pd.NaT, pd.NaT, pd.NaT]),
                 ),
                 name="value",
             ),
         ),
         (
             StringIO(
+                """file,start,value
+f1,0,0.0
+f1,1,1.0
+f2,2,2.0"""
+            ),
+            pd.Series(
+                [0.0, 1.0, 2.0],
+                index=audformat.segmented_index(
+                    ["f1", "f1", "f2"],
+                    starts=["0s", "1s", "2s"],
+                    ends=pd.to_timedelta([pd.NaT, pd.NaT, pd.NaT]),
+                ),
+                name="value",
+            ),
+        ),
+        (
+            StringIO(
                 """file,end,value
 f1,00:00:01,0.0
 f1,00:00:02,1.0
 f2,00:00:03,2.0"""
             ),
             pd.Series(
                 [0.0, 1.0, 2.0],
@@ -1489,14 +1506,27 @@
                 ["f1", "f1", "f2"],
                 ["0s", "1s", "2s"],
                 ["1s", "2s", "3s"],
             ),
         ),
         (
             StringIO(
+                """file,start,end
+f1,0,1
+f1,1,2
+f2,2,3"""
+            ),
+            audformat.segmented_index(
+                ["f1", "f1", "f2"],
+                ["0s", "1s", "2s"],
+                ["1s", "2s", "3s"],
+            ),
+        ),
+        (
+            StringIO(
                 """file,start,end,value
 f1,00:00:00,00:00:01,0.0
 f1,00:00:01,00:00:02,1.0
 f2,00:00:02,00:00:03,2.0"""
             ),
             pd.Series(
                 [0.0, 1.0, 2.0],
@@ -1506,14 +1536,48 @@
                     ends=["1s", "2s", "3s"],
                 ),
                 name="value",
             ),
         ),
         (
             StringIO(
+                """file,start,end,value
+f1,0,1,0.0
+f1,1,2,1.0
+f2,2,3,2.0"""
+            ),
+            pd.Series(
+                [0.0, 1.0, 2.0],
+                index=audformat.segmented_index(
+                    ["f1", "f1", "f2"],
+                    starts=["0s", "1s", "2s"],
+                    ends=["1s", "2s", "3s"],
+                ),
+                name="value",
+            ),
+        ),
+        (
+            StringIO(
+                """file,start,end,value
+f1,0.0,1.0,0.0
+f1,1.0,2.0,1.0
+f2,2.0,3.0,2.0"""
+            ),
+            pd.Series(
+                [0.0, 1.0, 2.0],
+                index=audformat.segmented_index(
+                    ["f1", "f1", "f2"],
+                    starts=["0s", "1s", "2s"],
+                    ends=["1s", "2s", "3s"],
+                ),
+                name="value",
+            ),
+        ),
+        (
+            StringIO(
                 """file,start,end,value1,value2
 f1,00:00:00,00:00:01,0.0,a
 f1,00:00:01,00:00:02,1.0,b
 f2,00:00:02,00:00:03,2.0,c"""
             ),
             pd.DataFrame(
                 {
@@ -1544,14 +1608,22 @@
     obj = audformat.utils.read_csv(csv)
     if isinstance(result, pd.Index):
         pd.testing.assert_index_equal(obj, result)
     elif isinstance(result, pd.Series):
         pd.testing.assert_series_equal(obj, result)
     else:
         pd.testing.assert_frame_equal(obj, result)
+    # Request dataframe as return type
+    csv.seek(0)  # rewind string file object
+    obj = audformat.utils.read_csv(csv, as_dataframe=True)
+    if isinstance(result, pd.Index):
+        result = pd.DataFrame([], columns=[], index=result)
+    elif isinstance(result, pd.Series):
+        result = result.to_frame()
+    pd.testing.assert_frame_equal(obj, result)
 
 
 @pytest.mark.parametrize(
     "index, extension, pattern, expected_index",
     [
         (
             audformat.filewise_index(),
```

### Comparing `audformat-1.1.2/tests/test_utils_concat.py` & `audformat-1.1.3/tests/test_utils_concat.py`

 * *Files identical despite different names*

