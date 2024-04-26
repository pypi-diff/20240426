# Comparing `tmp/awsfindingsmanagerlib-0.0.0.tar.gz` & `tmp/awsfindingsmanagerlib-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsfindingsmanagerlib-0.0.0.tar", last modified: Fri Apr 26 11:30:05 2024, max compression
+gzip compressed data, was "awsfindingsmanagerlib-0.1.0.tar", last modified: Fri Apr 26 11:39:25 2024, max compression
```

## Comparing `awsfindingsmanagerlib-0.0.0.tar` & `awsfindingsmanagerlib-0.1.0.tar`

### file list

```diff
@@ -1,62 +1,54 @@
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-26 11:30:05.400985 awsfindingsmanagerlib-0.0.0/
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        5 2023-11-21 09:40:26.000000 awsfindingsmanagerlib-0.0.0/.VERSION
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      187 2024-04-26 11:11:56.000000 awsfindingsmanagerlib-0.0.0/AUTHORS.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1298 2023-11-21 09:40:26.000000 awsfindingsmanagerlib-0.0.0/CONTRIBUTING.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       32 2024-04-26 11:11:56.000000 awsfindingsmanagerlib-0.0.0/HISTORY.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    10534 2023-11-21 09:40:26.000000 awsfindingsmanagerlib-0.0.0/LICENSE
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      416 2023-11-21 09:40:26.000000 awsfindingsmanagerlib-0.0.0/MANIFEST.in
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3511 2024-04-26 11:30:05.400768 awsfindingsmanagerlib-0.0.0/PKG-INFO
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      637 2024-04-08 08:41:17.000000 awsfindingsmanagerlib-0.0.0/Pipfile
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    82965 2024-04-26 11:30:04.000000 awsfindingsmanagerlib-0.0.0/Pipfile.lock
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     2495 2024-04-26 11:11:56.000000 awsfindingsmanagerlib-0.0.0/README.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      961 2023-11-21 09:40:26.000000 awsfindingsmanagerlib-0.0.0/USAGE.rst
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-26 11:30:05.375939 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        5 2024-04-26 11:30:04.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/.VERSION
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      187 2024-04-26 11:30:04.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/AUTHORS.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1298 2024-04-26 11:30:04.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/CONTRIBUTING.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       32 2024-04-26 11:30:04.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/HISTORY.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    10534 2024-04-26 11:30:04.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/LICENSE
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      637 2024-04-26 11:30:04.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/Pipfile
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    82965 2024-04-26 11:30:04.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/Pipfile.lock
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     2495 2024-04-26 11:30:04.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/README.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      961 2024-04-26 11:30:04.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/USAGE.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1669 2024-04-08 08:41:17.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/__init__.py
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-26 11:30:05.392806 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/__pycache__/
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1117 2024-04-08 09:18:29.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1312 2024-04-08 09:18:29.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/__pycache__/_version.cpython-38.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    39610 2024-04-22 15:00:24.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/__pycache__/awsfindingsmanagerlib.cpython-38.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3621 2024-04-08 09:18:30.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/__pycache__/awsfindingsmanagerlibexceptions.cpython-38.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     4135 2024-04-08 09:18:30.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/__pycache__/backends.cpython-38.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2668 2024-04-08 09:18:30.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/__pycache__/configuration.cpython-38.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     7998 2024-04-08 09:18:30.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/__pycache__/validations.cpython-38.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1967 2024-04-08 08:41:17.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/_version.py
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)    41070 2024-04-22 14:52:35.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/awsfindingsmanagerlib.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2926 2024-04-08 08:41:17.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/awsfindingsmanagerlibexceptions.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     4112 2024-04-08 08:41:17.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/backends.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3154 2024-04-08 08:41:17.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/configuration.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1172 2024-04-26 11:30:04.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/dev-requirements.txt
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      614 2024-04-26 11:30:04.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/requirements.txt
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     9161 2024-04-08 08:41:17.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/validations.py
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-26 11:30:05.388309 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib.egg-info/
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3511 2024-04-26 11:30:05.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib.egg-info/PKG-INFO
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1735 2024-04-26 11:30:05.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib.egg-info/SOURCES.txt
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)        1 2024-04-26 11:30:05.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib.egg-info/dependency_links.txt
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)        1 2024-01-04 12:22:12.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib.egg-info/not-zip-safe
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      263 2024-04-26 11:30:05.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib.egg-info/requires.txt
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)       22 2024-04-26 11:30:05.000000 awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib.egg-info/top_level.txt
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1172 2024-04-26 11:30:04.000000 awsfindingsmanagerlib-0.0.0/dev-requirements.txt
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-26 11:30:05.399522 awsfindingsmanagerlib-0.0.0/docs/
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     6822 2023-11-21 09:40:26.000000 awsfindingsmanagerlib-0.0.0/docs/Makefile
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       28 2023-11-21 09:40:26.000000 awsfindingsmanagerlib-0.0.0/docs/authors.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     9054 2023-11-21 09:40:26.000000 awsfindingsmanagerlib-0.0.0/docs/conf.py
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       33 2023-11-21 09:40:26.000000 awsfindingsmanagerlib-0.0.0/docs/contributing.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       28 2023-11-21 09:40:26.000000 awsfindingsmanagerlib-0.0.0/docs/history.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      537 2023-11-21 09:40:26.000000 awsfindingsmanagerlib-0.0.0/docs/index.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)       33 2023-11-21 09:40:26.000000 awsfindingsmanagerlib-0.0.0/docs/installation.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       27 2023-11-21 09:40:26.000000 awsfindingsmanagerlib-0.0.0/docs/readme.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       26 2023-11-21 09:40:26.000000 awsfindingsmanagerlib-0.0.0/docs/usage.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      614 2024-04-26 11:30:04.000000 awsfindingsmanagerlib-0.0.0/requirements.txt
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      161 2024-04-26 11:30:05.402122 awsfindingsmanagerlib-0.0.0/setup.cfg
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     2044 2024-04-26 11:29:11.000000 awsfindingsmanagerlib-0.0.0/setup.py
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-26 11:30:05.400110 awsfindingsmanagerlib-0.0.0/tests/
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1786 2023-11-21 09:40:26.000000 awsfindingsmanagerlib-0.0.0/tests/test_awsfindingsmanagerlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:39:25.792509 awsfindingsmanagerlib-0.1.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        5 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (127)      187 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1298 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)      416 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-26 11:39:25.792509 awsfindingsmanagerlib-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)    91914 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2495 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/USAGE.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:39:25.792509 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        5 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (127)      187 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1298 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)    91914 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2495 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/USAGE.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1669 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41070 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/awsfindingsmanagerlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/awsfindingsmanagerlibexceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:39:25.792509 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:39:25.792509 awsfindingsmanagerlib-0.1.0/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6822 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9054 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       33 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/docs/contributing.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/docs/history.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      537 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/docs/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)       27 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/docs/readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)       26 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-26 11:39:25.000000 awsfindingsmanagerlib-0.1.0/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      161 2024-04-26 11:39:25.792509 awsfindingsmanagerlib-0.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2044 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:39:25.792509 awsfindingsmanagerlib-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-26 11:38:23.000000 awsfindingsmanagerlib-0.1.0/tests/test_awsfindingsmanagerlib.py
```

### Comparing `awsfindingsmanagerlib-0.0.0/CONTRIBUTING.rst` & `awsfindingsmanagerlib-0.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/LICENSE` & `awsfindingsmanagerlib-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/PKG-INFO` & `awsfindingsmanagerlib-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsfindingsmanagerlib
-Version: 0.0.0
+Version: 0.1.0
 Summary: A library to manage findings in AWS.
 Home-page: https://github.com/schubergphilis/awsfindingsmanagerlib.git
 Author: Marwin Baumann
 Author-email: mbaumann@schubergphilis.com
 License: Apache Software License 2.0
 Keywords: awsfindingsmanagerlib securityhub findings aws
 Classifier: Development Status :: 4 - Beta
@@ -98,7 +98,13 @@
 While the project is released under the Apache 2 license, scripts under _CI/scripts are released under an MIT license as stated on their header.
 
 
 
 
 History
 -------
+
+
+0.1.0 (26-04-2024)
+------------------
+
+* Initial release.
```

### Comparing `awsfindingsmanagerlib-0.0.0/Pipfile` & `awsfindingsmanagerlib-0.1.0/Pipfile`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/Pipfile.lock` & `awsfindingsmanagerlib-0.1.0/Pipfile.lock`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9911225658648339%*

 * *Differences: {"'develop'": '{\'importlib-metadata\': {\'markers\': "python_version >= \'3.8\'"}, \'sh\': '*

 * *              '{\'markers\': "sys_platform != \'win32\'"}, \'cffi\': OrderedDict([(\'hashes\', '*

 * *              "['sha256:0c9ef6ff37e974b73c25eecc13952c55bceed9112be2d9d938ded8e856138bcc', "*

 * *              "'sha256:131fd094d1065b19540c3d72594260f118b231090295d8c34e19a7bbcf2e860a', "*

 * *              "'sha256:1b8ebc27c014c59692bb2664c7d13ce7a6e9a629be20e54e7271fa696ff2b417', "*

 * *              "'sha256:2c56b361916f390cd758a […]*

```diff
@@ -347,14 +347,72 @@
             "hashes": [
                 "sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f",
                 "sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2024.2.2"
         },
+        "cffi": {
+            "hashes": [
+                "sha256:0c9ef6ff37e974b73c25eecc13952c55bceed9112be2d9d938ded8e856138bcc",
+                "sha256:131fd094d1065b19540c3d72594260f118b231090295d8c34e19a7bbcf2e860a",
+                "sha256:1b8ebc27c014c59692bb2664c7d13ce7a6e9a629be20e54e7271fa696ff2b417",
+                "sha256:2c56b361916f390cd758a57f2e16233eb4f64bcbeee88a4881ea90fca14dc6ab",
+                "sha256:2d92b25dbf6cae33f65005baf472d2c245c050b1ce709cc4588cdcdd5495b520",
+                "sha256:31d13b0f99e0836b7ff893d37af07366ebc90b678b6664c955b54561fc36ef36",
+                "sha256:32c68ef735dbe5857c810328cb2481e24722a59a2003018885514d4c09af9743",
+                "sha256:3686dffb02459559c74dd3d81748269ffb0eb027c39a6fc99502de37d501faa8",
+                "sha256:582215a0e9adbe0e379761260553ba11c58943e4bbe9c36430c4ca6ac74b15ed",
+                "sha256:5b50bf3f55561dac5438f8e70bfcdfd74543fd60df5fa5f62d94e5867deca684",
+                "sha256:5bf44d66cdf9e893637896c7faa22298baebcd18d1ddb6d2626a6e39793a1d56",
+                "sha256:6602bc8dc6f3a9e02b6c22c4fc1e47aa50f8f8e6d3f78a5e16ac33ef5fefa324",
+                "sha256:673739cb539f8cdaa07d92d02efa93c9ccf87e345b9a0b556e3ecc666718468d",
+                "sha256:68678abf380b42ce21a5f2abde8efee05c114c2fdb2e9eef2efdb0257fba1235",
+                "sha256:68e7c44931cc171c54ccb702482e9fc723192e88d25a0e133edd7aff8fcd1f6e",
+                "sha256:6b3d6606d369fc1da4fd8c357d026317fbb9c9b75d36dc16e90e84c26854b088",
+                "sha256:748dcd1e3d3d7cd5443ef03ce8685043294ad6bd7c02a38d1bd367cfd968e000",
+                "sha256:7651c50c8c5ef7bdb41108b7b8c5a83013bfaa8a935590c5d74627c047a583c7",
+                "sha256:7b78010e7b97fef4bee1e896df8a4bbb6712b7f05b7ef630f9d1da00f6444d2e",
+                "sha256:7e61e3e4fa664a8588aa25c883eab612a188c725755afff6289454d6362b9673",
+                "sha256:80876338e19c951fdfed6198e70bc88f1c9758b94578d5a7c4c91a87af3cf31c",
+                "sha256:8895613bcc094d4a1b2dbe179d88d7fb4a15cee43c052e8885783fac397d91fe",
+                "sha256:88e2b3c14bdb32e440be531ade29d3c50a1a59cd4e51b1dd8b0865c54ea5d2e2",
+                "sha256:8f8e709127c6c77446a8c0a8c8bf3c8ee706a06cd44b1e827c3e6a2ee6b8c098",
+                "sha256:9cb4a35b3642fc5c005a6755a5d17c6c8b6bcb6981baf81cea8bfbc8903e8ba8",
+                "sha256:9f90389693731ff1f659e55c7d1640e2ec43ff725cc61b04b2f9c6d8d017df6a",
+                "sha256:a09582f178759ee8128d9270cd1344154fd473bb77d94ce0aeb2a93ebf0feaf0",
+                "sha256:a6a14b17d7e17fa0d207ac08642c8820f84f25ce17a442fd15e27ea18d67c59b",
+                "sha256:a72e8961a86d19bdb45851d8f1f08b041ea37d2bd8d4fd19903bc3083d80c896",
+                "sha256:abd808f9c129ba2beda4cfc53bde801e5bcf9d6e0f22f095e45327c038bfe68e",
+                "sha256:ac0f5edd2360eea2f1daa9e26a41db02dd4b0451b48f7c318e217ee092a213e9",
+                "sha256:b29ebffcf550f9da55bec9e02ad430c992a87e5f512cd63388abb76f1036d8d2",
+                "sha256:b2ca4e77f9f47c55c194982e10f058db063937845bb2b7a86c84a6cfe0aefa8b",
+                "sha256:b7be2d771cdba2942e13215c4e340bfd76398e9227ad10402a8767ab1865d2e6",
+                "sha256:b84834d0cf97e7d27dd5b7f3aca7b6e9263c56308ab9dc8aae9784abb774d404",
+                "sha256:b86851a328eedc692acf81fb05444bdf1891747c25af7529e39ddafaf68a4f3f",
+                "sha256:bcb3ef43e58665bbda2fb198698fcae6776483e0c4a631aa5647806c25e02cc0",
+                "sha256:c0f31130ebc2d37cdd8e44605fb5fa7ad59049298b3f745c74fa74c62fbfcfc4",
+                "sha256:c6a164aa47843fb1b01e941d385aab7215563bb8816d80ff3a363a9f8448a8dc",
+                "sha256:d8a9d3ebe49f084ad71f9269834ceccbf398253c9fac910c4fd7053ff1386936",
+                "sha256:db8e577c19c0fda0beb7e0d4e09e0ba74b1e4c092e0e40bfa12fe05b6f6d75ba",
+                "sha256:dc9b18bf40cc75f66f40a7379f6a9513244fe33c0e8aa72e2d56b0196a7ef872",
+                "sha256:e09f3ff613345df5e8c3667da1d918f9149bd623cd9070c983c013792a9a62eb",
+                "sha256:e4108df7fe9b707191e55f33efbcb2d81928e10cea45527879a4749cbe472614",
+                "sha256:e6024675e67af929088fda399b2094574609396b1decb609c55fa58b028a32a1",
+                "sha256:e70f54f1796669ef691ca07d046cd81a29cb4deb1e5f942003f401c0c4a2695d",
+                "sha256:e715596e683d2ce000574bae5d07bd522c781a822866c20495e52520564f0969",
+                "sha256:e760191dd42581e023a68b758769e2da259b5d52e3103c6060ddc02c9edb8d7b",
+                "sha256:ed86a35631f7bfbb28e108dd96773b9d5a6ce4811cf6ea468bb6a359b256b1e4",
+                "sha256:ee07e47c12890ef248766a6e55bd38ebfb2bb8edd4142d56db91b21ea68b7627",
+                "sha256:fa3a0128b152627161ce47201262d3140edb5a5c3da88d73a1b790a959126956",
+                "sha256:fcc8eb6d5902bb1cf6dc4f187ee3ea80a1eba0a89aba40a5cb20a5087d961357"
+            ],
+            "markers": "platform_python_implementation != 'PyPy'",
+            "version": "==1.16.0"
+        },
         "chardet": {
             "hashes": [
                 "sha256:1b3b6ff479a8c414bc3fa2c0852995695c4a026dcd6d0633b2dd092ca39c1cf7",
                 "sha256:e1cf59446890a00105fe7b7912492ea04b6e6f06d4b742b2c788469e34c82970"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==5.2.0"
@@ -527,14 +585,52 @@
                 "sha256:fea9d3ca80bcf17edb2c08a4704259dadac196fe5e9274067e7a20511fad1743",
                 "sha256:fed7a72d54bd52f4aeb6c6e951f363903bd7d70bc1cad64dd1f087980d309ab9"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
             "version": "==7.5.0"
         },
+        "cryptography": {
+            "hashes": [
+                "sha256:0270572b8bd2c833c3981724b8ee9747b3ec96f699a9665470018594301439ee",
+                "sha256:111a0d8553afcf8eb02a4fea6ca4f59d48ddb34497aa8706a6cf536f1a5ec576",
+                "sha256:16a48c23a62a2f4a285699dba2e4ff2d1cff3115b9df052cdd976a18856d8e3d",
+                "sha256:1b95b98b0d2af784078fa69f637135e3c317091b615cd0905f8b8a087e86fa30",
+                "sha256:1f71c10d1e88467126f0efd484bd44bca5e14c664ec2ede64c32f20875c0d413",
+                "sha256:2424ff4c4ac7f6b8177b53c17ed5d8fa74ae5955656867f5a8affaca36a27abb",
+                "sha256:2bce03af1ce5a5567ab89bd90d11e7bbdff56b8af3acbbec1faded8f44cb06da",
+                "sha256:329906dcc7b20ff3cad13c069a78124ed8247adcac44b10bea1130e36caae0b4",
+                "sha256:37dd623507659e08be98eec89323469e8c7b4c1407c85112634ae3dbdb926fdd",
+                "sha256:3eaafe47ec0d0ffcc9349e1708be2aaea4c6dd4978d76bf6eb0cb2c13636c6fc",
+                "sha256:5e6275c09d2badf57aea3afa80d975444f4be8d3bc58f7f80d2a484c6f9485c8",
+                "sha256:6fe07eec95dfd477eb9530aef5bead34fec819b3aaf6c5bd6d20565da607bfe1",
+                "sha256:7367d7b2eca6513681127ebad53b2582911d1736dc2ffc19f2c3ae49997496bc",
+                "sha256:7cde5f38e614f55e28d831754e8a3bacf9ace5d1566235e39d91b35502d6936e",
+                "sha256:9481ffe3cf013b71b2428b905c4f7a9a4f76ec03065b05ff499bb5682a8d9ad8",
+                "sha256:98d8dc6d012b82287f2c3d26ce1d2dd130ec200c8679b6213b3c73c08b2b7940",
+                "sha256:a011a644f6d7d03736214d38832e030d8268bcff4a41f728e6030325fea3e400",
+                "sha256:a2913c5375154b6ef2e91c10b5720ea6e21007412f6437504ffea2109b5a33d7",
+                "sha256:a30596bae9403a342c978fb47d9b0ee277699fa53bbafad14706af51fe543d16",
+                "sha256:b03c2ae5d2f0fc05f9a2c0c997e1bc18c8229f392234e8a0194f202169ccd278",
+                "sha256:b6cd2203306b63e41acdf39aa93b86fb566049aeb6dc489b70e34bcd07adca74",
+                "sha256:b7ffe927ee6531c78f81aa17e684e2ff617daeba7f189f911065b2ea2d526dec",
+                "sha256:b8cac287fafc4ad485b8a9b67d0ee80c66bf3574f655d3b97ef2e1082360faf1",
+                "sha256:ba334e6e4b1d92442b75ddacc615c5476d4ad55cc29b15d590cc6b86efa487e2",
+                "sha256:ba3e4a42397c25b7ff88cdec6e2a16c2be18720f317506ee25210f6d31925f9c",
+                "sha256:c41fb5e6a5fe9ebcd58ca3abfeb51dffb5d83d6775405305bfa8715b76521922",
+                "sha256:cd2030f6650c089aeb304cf093f3244d34745ce0cfcc39f20c6fbfe030102e2a",
+                "sha256:cd65d75953847815962c84a4654a84850b2bb4aed3f26fadcc1c13892e1e29f6",
+                "sha256:e4985a790f921508f36f81831817cbc03b102d643b5fcb81cd33df3fa291a1a1",
+                "sha256:e807b3188f9eb0eaa7bbb579b462c5ace579f1cedb28107ce8b48a9f7ad3679e",
+                "sha256:f12764b8fffc7a123f641d7d049d382b73f96a34117e0b637b80643169cec8ac",
+                "sha256:f8837fe1d6ac4a8052a9a8ddab256bc006242696f03368a4009be7ee3075cdb7"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==42.0.5"
+        },
         "dill": {
             "hashes": [
                 "sha256:3ebe3c479ad625c4553aca177444d89b486b1d84982eeacded644afc0cf797ca",
                 "sha256:c36ca9ffb54365bdd2f8eb3eff7d2a21237f8452b57ace88b1ac615b7e815bd7"
             ],
             "markers": "python_version < '3.11'",
             "version": "==0.3.8"
@@ -641,15 +737,15 @@
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
                 "sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570",
                 "sha256:b78938b926ee8d5f020fc4772d487045805a55ddbad2ecf21c6d60938dc7fcd2"
             ],
-            "markers": "python_version < '3.10'",
+            "markers": "python_version >= '3.8'",
             "version": "==7.1.0"
         },
         "importlib-resources": {
             "hashes": [
                 "sha256:50d10f043df931902d4194ea07ec57960f66a80449ff867bfe782b4c486ba78c",
                 "sha256:cdb2b453b8046ca4e3798eb1d84f3cce1446a0e8e7b5ef4efb600f19fc398145"
             ],
@@ -684,14 +780,22 @@
             "hashes": [
                 "sha256:3b24ccb921d6b593bdceb56ce14799204f473976e2a9d4b15b04d0f2c2326664",
                 "sha256:d33fa765374c0611b52f8b3a795f8900869aa88c84769d4d1746cd68fb28c3e8"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==4.0.1"
         },
+        "jeepney": {
+            "hashes": [
+                "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
+                "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
+            ],
+            "markers": "sys_platform == 'linux'",
+            "version": "==0.8.0"
+        },
         "jinja2": {
             "hashes": [
                 "sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa",
                 "sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.3"
@@ -935,14 +1039,22 @@
             "hashes": [
                 "sha256:2c9607871d58c76354b697b42f5d57e1ada7d261c261efac224b664affdc5785",
                 "sha256:d1735fc58b418fd7c5f658d28d943854f8a849b01a5d0a1e6f3f3fdd0166804b"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.9.1"
         },
+        "pycparser": {
+            "hashes": [
+                "sha256:491c8be9c040f5390f5bf44a5b07752bd07f56edf992381b05c701439eec10f6",
+                "sha256:c3702b6d3dd8c7abc1afa565d7e63d53a1d0bd86cdc24edd75470f4de499cfcc"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==2.22"
+        },
         "pydocstyle": {
             "hashes": [
                 "sha256:118762d452a49d6b05e194ef344a55822987a462831ade91ec5c06fd2169d019",
                 "sha256:7ce43f0c0ac87b07494eb9c0b462c0b73e6ff276807f204d6b53edc72b7e44e1"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.3.0"
@@ -1117,14 +1229,22 @@
             "hashes": [
                 "sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222",
                 "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==13.7.1"
         },
+        "secretstorage": {
+            "hashes": [
+                "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
+                "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
+            ],
+            "markers": "sys_platform == 'linux'",
+            "version": "==3.3.3"
+        },
         "semver": {
             "hashes": [
                 "sha256:6253adb39c70f6e51afed2fa7152bcd414c411286088fb4b9effb133885ab4cc",
                 "sha256:b1ea4686fe70b981f85359eda33199d60c53964284e0cfb4977d243e37cf4bf4"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.7'",
@@ -1138,15 +1258,15 @@
             "version": "==0.3.1"
         },
         "sh": {
             "hashes": [
                 "sha256:9b2998f313f201c777e2c0061f0b1367497097ef13388595be147e2a00bf7ba1",
                 "sha256:ced8f2e081a858b66a46ace3703dec243779abbd5a1887ba7e3c34f34da70cd2"
             ],
-            "markers": "python_version < '4.0' and python_full_version >= '3.8.1'",
+            "markers": "sys_platform != 'win32'",
             "version": "==2.0.6"
         },
         "smmap": {
             "hashes": [
                 "sha256:dceeb6c0028fdb6734471eb07c0cd2aae706ccaecab45965ee83f11c8d3b1f62",
                 "sha256:e6d8668fa5f93e706934a62d7b4db19c8d9eb8cf2adbb75ef1b675aa332b69da"
             ],
```

### Comparing `awsfindingsmanagerlib-0.0.0/README.rst` & `awsfindingsmanagerlib-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/USAGE.rst` & `awsfindingsmanagerlib-0.1.0/USAGE.rst`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/CONTRIBUTING.rst` & `awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/LICENSE` & `awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/LICENSE`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/Pipfile` & `awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/Pipfile`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/Pipfile.lock` & `awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/Pipfile.lock`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9911225658648339%*

 * *Differences: {"'develop'": '{\'importlib-metadata\': {\'markers\': "python_version >= \'3.8\'"}, \'sh\': '*

 * *              '{\'markers\': "sys_platform != \'win32\'"}, \'cffi\': OrderedDict([(\'hashes\', '*

 * *              "['sha256:0c9ef6ff37e974b73c25eecc13952c55bceed9112be2d9d938ded8e856138bcc', "*

 * *              "'sha256:131fd094d1065b19540c3d72594260f118b231090295d8c34e19a7bbcf2e860a', "*

 * *              "'sha256:1b8ebc27c014c59692bb2664c7d13ce7a6e9a629be20e54e7271fa696ff2b417', "*

 * *              "'sha256:2c56b361916f390cd758a […]*

```diff
@@ -347,14 +347,72 @@
             "hashes": [
                 "sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f",
                 "sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2024.2.2"
         },
+        "cffi": {
+            "hashes": [
+                "sha256:0c9ef6ff37e974b73c25eecc13952c55bceed9112be2d9d938ded8e856138bcc",
+                "sha256:131fd094d1065b19540c3d72594260f118b231090295d8c34e19a7bbcf2e860a",
+                "sha256:1b8ebc27c014c59692bb2664c7d13ce7a6e9a629be20e54e7271fa696ff2b417",
+                "sha256:2c56b361916f390cd758a57f2e16233eb4f64bcbeee88a4881ea90fca14dc6ab",
+                "sha256:2d92b25dbf6cae33f65005baf472d2c245c050b1ce709cc4588cdcdd5495b520",
+                "sha256:31d13b0f99e0836b7ff893d37af07366ebc90b678b6664c955b54561fc36ef36",
+                "sha256:32c68ef735dbe5857c810328cb2481e24722a59a2003018885514d4c09af9743",
+                "sha256:3686dffb02459559c74dd3d81748269ffb0eb027c39a6fc99502de37d501faa8",
+                "sha256:582215a0e9adbe0e379761260553ba11c58943e4bbe9c36430c4ca6ac74b15ed",
+                "sha256:5b50bf3f55561dac5438f8e70bfcdfd74543fd60df5fa5f62d94e5867deca684",
+                "sha256:5bf44d66cdf9e893637896c7faa22298baebcd18d1ddb6d2626a6e39793a1d56",
+                "sha256:6602bc8dc6f3a9e02b6c22c4fc1e47aa50f8f8e6d3f78a5e16ac33ef5fefa324",
+                "sha256:673739cb539f8cdaa07d92d02efa93c9ccf87e345b9a0b556e3ecc666718468d",
+                "sha256:68678abf380b42ce21a5f2abde8efee05c114c2fdb2e9eef2efdb0257fba1235",
+                "sha256:68e7c44931cc171c54ccb702482e9fc723192e88d25a0e133edd7aff8fcd1f6e",
+                "sha256:6b3d6606d369fc1da4fd8c357d026317fbb9c9b75d36dc16e90e84c26854b088",
+                "sha256:748dcd1e3d3d7cd5443ef03ce8685043294ad6bd7c02a38d1bd367cfd968e000",
+                "sha256:7651c50c8c5ef7bdb41108b7b8c5a83013bfaa8a935590c5d74627c047a583c7",
+                "sha256:7b78010e7b97fef4bee1e896df8a4bbb6712b7f05b7ef630f9d1da00f6444d2e",
+                "sha256:7e61e3e4fa664a8588aa25c883eab612a188c725755afff6289454d6362b9673",
+                "sha256:80876338e19c951fdfed6198e70bc88f1c9758b94578d5a7c4c91a87af3cf31c",
+                "sha256:8895613bcc094d4a1b2dbe179d88d7fb4a15cee43c052e8885783fac397d91fe",
+                "sha256:88e2b3c14bdb32e440be531ade29d3c50a1a59cd4e51b1dd8b0865c54ea5d2e2",
+                "sha256:8f8e709127c6c77446a8c0a8c8bf3c8ee706a06cd44b1e827c3e6a2ee6b8c098",
+                "sha256:9cb4a35b3642fc5c005a6755a5d17c6c8b6bcb6981baf81cea8bfbc8903e8ba8",
+                "sha256:9f90389693731ff1f659e55c7d1640e2ec43ff725cc61b04b2f9c6d8d017df6a",
+                "sha256:a09582f178759ee8128d9270cd1344154fd473bb77d94ce0aeb2a93ebf0feaf0",
+                "sha256:a6a14b17d7e17fa0d207ac08642c8820f84f25ce17a442fd15e27ea18d67c59b",
+                "sha256:a72e8961a86d19bdb45851d8f1f08b041ea37d2bd8d4fd19903bc3083d80c896",
+                "sha256:abd808f9c129ba2beda4cfc53bde801e5bcf9d6e0f22f095e45327c038bfe68e",
+                "sha256:ac0f5edd2360eea2f1daa9e26a41db02dd4b0451b48f7c318e217ee092a213e9",
+                "sha256:b29ebffcf550f9da55bec9e02ad430c992a87e5f512cd63388abb76f1036d8d2",
+                "sha256:b2ca4e77f9f47c55c194982e10f058db063937845bb2b7a86c84a6cfe0aefa8b",
+                "sha256:b7be2d771cdba2942e13215c4e340bfd76398e9227ad10402a8767ab1865d2e6",
+                "sha256:b84834d0cf97e7d27dd5b7f3aca7b6e9263c56308ab9dc8aae9784abb774d404",
+                "sha256:b86851a328eedc692acf81fb05444bdf1891747c25af7529e39ddafaf68a4f3f",
+                "sha256:bcb3ef43e58665bbda2fb198698fcae6776483e0c4a631aa5647806c25e02cc0",
+                "sha256:c0f31130ebc2d37cdd8e44605fb5fa7ad59049298b3f745c74fa74c62fbfcfc4",
+                "sha256:c6a164aa47843fb1b01e941d385aab7215563bb8816d80ff3a363a9f8448a8dc",
+                "sha256:d8a9d3ebe49f084ad71f9269834ceccbf398253c9fac910c4fd7053ff1386936",
+                "sha256:db8e577c19c0fda0beb7e0d4e09e0ba74b1e4c092e0e40bfa12fe05b6f6d75ba",
+                "sha256:dc9b18bf40cc75f66f40a7379f6a9513244fe33c0e8aa72e2d56b0196a7ef872",
+                "sha256:e09f3ff613345df5e8c3667da1d918f9149bd623cd9070c983c013792a9a62eb",
+                "sha256:e4108df7fe9b707191e55f33efbcb2d81928e10cea45527879a4749cbe472614",
+                "sha256:e6024675e67af929088fda399b2094574609396b1decb609c55fa58b028a32a1",
+                "sha256:e70f54f1796669ef691ca07d046cd81a29cb4deb1e5f942003f401c0c4a2695d",
+                "sha256:e715596e683d2ce000574bae5d07bd522c781a822866c20495e52520564f0969",
+                "sha256:e760191dd42581e023a68b758769e2da259b5d52e3103c6060ddc02c9edb8d7b",
+                "sha256:ed86a35631f7bfbb28e108dd96773b9d5a6ce4811cf6ea468bb6a359b256b1e4",
+                "sha256:ee07e47c12890ef248766a6e55bd38ebfb2bb8edd4142d56db91b21ea68b7627",
+                "sha256:fa3a0128b152627161ce47201262d3140edb5a5c3da88d73a1b790a959126956",
+                "sha256:fcc8eb6d5902bb1cf6dc4f187ee3ea80a1eba0a89aba40a5cb20a5087d961357"
+            ],
+            "markers": "platform_python_implementation != 'PyPy'",
+            "version": "==1.16.0"
+        },
         "chardet": {
             "hashes": [
                 "sha256:1b3b6ff479a8c414bc3fa2c0852995695c4a026dcd6d0633b2dd092ca39c1cf7",
                 "sha256:e1cf59446890a00105fe7b7912492ea04b6e6f06d4b742b2c788469e34c82970"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==5.2.0"
@@ -527,14 +585,52 @@
                 "sha256:fea9d3ca80bcf17edb2c08a4704259dadac196fe5e9274067e7a20511fad1743",
                 "sha256:fed7a72d54bd52f4aeb6c6e951f363903bd7d70bc1cad64dd1f087980d309ab9"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
             "version": "==7.5.0"
         },
+        "cryptography": {
+            "hashes": [
+                "sha256:0270572b8bd2c833c3981724b8ee9747b3ec96f699a9665470018594301439ee",
+                "sha256:111a0d8553afcf8eb02a4fea6ca4f59d48ddb34497aa8706a6cf536f1a5ec576",
+                "sha256:16a48c23a62a2f4a285699dba2e4ff2d1cff3115b9df052cdd976a18856d8e3d",
+                "sha256:1b95b98b0d2af784078fa69f637135e3c317091b615cd0905f8b8a087e86fa30",
+                "sha256:1f71c10d1e88467126f0efd484bd44bca5e14c664ec2ede64c32f20875c0d413",
+                "sha256:2424ff4c4ac7f6b8177b53c17ed5d8fa74ae5955656867f5a8affaca36a27abb",
+                "sha256:2bce03af1ce5a5567ab89bd90d11e7bbdff56b8af3acbbec1faded8f44cb06da",
+                "sha256:329906dcc7b20ff3cad13c069a78124ed8247adcac44b10bea1130e36caae0b4",
+                "sha256:37dd623507659e08be98eec89323469e8c7b4c1407c85112634ae3dbdb926fdd",
+                "sha256:3eaafe47ec0d0ffcc9349e1708be2aaea4c6dd4978d76bf6eb0cb2c13636c6fc",
+                "sha256:5e6275c09d2badf57aea3afa80d975444f4be8d3bc58f7f80d2a484c6f9485c8",
+                "sha256:6fe07eec95dfd477eb9530aef5bead34fec819b3aaf6c5bd6d20565da607bfe1",
+                "sha256:7367d7b2eca6513681127ebad53b2582911d1736dc2ffc19f2c3ae49997496bc",
+                "sha256:7cde5f38e614f55e28d831754e8a3bacf9ace5d1566235e39d91b35502d6936e",
+                "sha256:9481ffe3cf013b71b2428b905c4f7a9a4f76ec03065b05ff499bb5682a8d9ad8",
+                "sha256:98d8dc6d012b82287f2c3d26ce1d2dd130ec200c8679b6213b3c73c08b2b7940",
+                "sha256:a011a644f6d7d03736214d38832e030d8268bcff4a41f728e6030325fea3e400",
+                "sha256:a2913c5375154b6ef2e91c10b5720ea6e21007412f6437504ffea2109b5a33d7",
+                "sha256:a30596bae9403a342c978fb47d9b0ee277699fa53bbafad14706af51fe543d16",
+                "sha256:b03c2ae5d2f0fc05f9a2c0c997e1bc18c8229f392234e8a0194f202169ccd278",
+                "sha256:b6cd2203306b63e41acdf39aa93b86fb566049aeb6dc489b70e34bcd07adca74",
+                "sha256:b7ffe927ee6531c78f81aa17e684e2ff617daeba7f189f911065b2ea2d526dec",
+                "sha256:b8cac287fafc4ad485b8a9b67d0ee80c66bf3574f655d3b97ef2e1082360faf1",
+                "sha256:ba334e6e4b1d92442b75ddacc615c5476d4ad55cc29b15d590cc6b86efa487e2",
+                "sha256:ba3e4a42397c25b7ff88cdec6e2a16c2be18720f317506ee25210f6d31925f9c",
+                "sha256:c41fb5e6a5fe9ebcd58ca3abfeb51dffb5d83d6775405305bfa8715b76521922",
+                "sha256:cd2030f6650c089aeb304cf093f3244d34745ce0cfcc39f20c6fbfe030102e2a",
+                "sha256:cd65d75953847815962c84a4654a84850b2bb4aed3f26fadcc1c13892e1e29f6",
+                "sha256:e4985a790f921508f36f81831817cbc03b102d643b5fcb81cd33df3fa291a1a1",
+                "sha256:e807b3188f9eb0eaa7bbb579b462c5ace579f1cedb28107ce8b48a9f7ad3679e",
+                "sha256:f12764b8fffc7a123f641d7d049d382b73f96a34117e0b637b80643169cec8ac",
+                "sha256:f8837fe1d6ac4a8052a9a8ddab256bc006242696f03368a4009be7ee3075cdb7"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==42.0.5"
+        },
         "dill": {
             "hashes": [
                 "sha256:3ebe3c479ad625c4553aca177444d89b486b1d84982eeacded644afc0cf797ca",
                 "sha256:c36ca9ffb54365bdd2f8eb3eff7d2a21237f8452b57ace88b1ac615b7e815bd7"
             ],
             "markers": "python_version < '3.11'",
             "version": "==0.3.8"
@@ -641,15 +737,15 @@
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
                 "sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570",
                 "sha256:b78938b926ee8d5f020fc4772d487045805a55ddbad2ecf21c6d60938dc7fcd2"
             ],
-            "markers": "python_version < '3.10'",
+            "markers": "python_version >= '3.8'",
             "version": "==7.1.0"
         },
         "importlib-resources": {
             "hashes": [
                 "sha256:50d10f043df931902d4194ea07ec57960f66a80449ff867bfe782b4c486ba78c",
                 "sha256:cdb2b453b8046ca4e3798eb1d84f3cce1446a0e8e7b5ef4efb600f19fc398145"
             ],
@@ -684,14 +780,22 @@
             "hashes": [
                 "sha256:3b24ccb921d6b593bdceb56ce14799204f473976e2a9d4b15b04d0f2c2326664",
                 "sha256:d33fa765374c0611b52f8b3a795f8900869aa88c84769d4d1746cd68fb28c3e8"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==4.0.1"
         },
+        "jeepney": {
+            "hashes": [
+                "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
+                "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
+            ],
+            "markers": "sys_platform == 'linux'",
+            "version": "==0.8.0"
+        },
         "jinja2": {
             "hashes": [
                 "sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa",
                 "sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.3"
@@ -935,14 +1039,22 @@
             "hashes": [
                 "sha256:2c9607871d58c76354b697b42f5d57e1ada7d261c261efac224b664affdc5785",
                 "sha256:d1735fc58b418fd7c5f658d28d943854f8a849b01a5d0a1e6f3f3fdd0166804b"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.9.1"
         },
+        "pycparser": {
+            "hashes": [
+                "sha256:491c8be9c040f5390f5bf44a5b07752bd07f56edf992381b05c701439eec10f6",
+                "sha256:c3702b6d3dd8c7abc1afa565d7e63d53a1d0bd86cdc24edd75470f4de499cfcc"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==2.22"
+        },
         "pydocstyle": {
             "hashes": [
                 "sha256:118762d452a49d6b05e194ef344a55822987a462831ade91ec5c06fd2169d019",
                 "sha256:7ce43f0c0ac87b07494eb9c0b462c0b73e6ff276807f204d6b53edc72b7e44e1"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.3.0"
@@ -1117,14 +1229,22 @@
             "hashes": [
                 "sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222",
                 "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==13.7.1"
         },
+        "secretstorage": {
+            "hashes": [
+                "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
+                "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
+            ],
+            "markers": "sys_platform == 'linux'",
+            "version": "==3.3.3"
+        },
         "semver": {
             "hashes": [
                 "sha256:6253adb39c70f6e51afed2fa7152bcd414c411286088fb4b9effb133885ab4cc",
                 "sha256:b1ea4686fe70b981f85359eda33199d60c53964284e0cfb4977d243e37cf4bf4"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.7'",
@@ -1138,15 +1258,15 @@
             "version": "==0.3.1"
         },
         "sh": {
             "hashes": [
                 "sha256:9b2998f313f201c777e2c0061f0b1367497097ef13388595be147e2a00bf7ba1",
                 "sha256:ced8f2e081a858b66a46ace3703dec243779abbd5a1887ba7e3c34f34da70cd2"
             ],
-            "markers": "python_version < '4.0' and python_full_version >= '3.8.1'",
+            "markers": "sys_platform != 'win32'",
             "version": "==2.0.6"
         },
         "smmap": {
             "hashes": [
                 "sha256:dceeb6c0028fdb6734471eb07c0cd2aae706ccaecab45965ee83f11c8d3b1f62",
                 "sha256:e6d8668fa5f93e706934a62d7b4db19c8d9eb8cf2adbb75ef1b675aa332b69da"
             ],
```

### Comparing `awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/README.rst` & `awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/README.rst`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/USAGE.rst` & `awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/USAGE.rst`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/__init__.py` & `awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/__init__.py`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/_version.py` & `awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/_version.py`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/awsfindingsmanagerlib.py` & `awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/awsfindingsmanagerlib.py`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/awsfindingsmanagerlibexceptions.py` & `awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/awsfindingsmanagerlibexceptions.py`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/backends.py` & `awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/backends.py`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/configuration.py` & `awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/configuration.py`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/dev-requirements.txt` & `awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/requirements.txt` & `awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/requirements.txt`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib/validations.py` & `awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib/validations.py`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib.egg-info/PKG-INFO` & `awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsfindingsmanagerlib
-Version: 0.0.0
+Version: 0.1.0
 Summary: A library to manage findings in AWS.
 Home-page: https://github.com/schubergphilis/awsfindingsmanagerlib.git
 Author: Marwin Baumann
 Author-email: mbaumann@schubergphilis.com
 License: Apache Software License 2.0
 Keywords: awsfindingsmanagerlib securityhub findings aws
 Classifier: Development Status :: 4 - Beta
@@ -98,7 +98,13 @@
 While the project is released under the Apache 2 license, scripts under _CI/scripts are released under an MIT license as stated on their header.
 
 
 
 
 History
 -------
+
+
+0.1.0 (26-04-2024)
+------------------
+
+* Initial release.
```

### Comparing `awsfindingsmanagerlib-0.0.0/awsfindingsmanagerlib.egg-info/SOURCES.txt` & `awsfindingsmanagerlib-0.1.0/awsfindingsmanagerlib.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -32,21 +32,14 @@
 awsfindingsmanagerlib/validations.py
 awsfindingsmanagerlib.egg-info/PKG-INFO
 awsfindingsmanagerlib.egg-info/SOURCES.txt
 awsfindingsmanagerlib.egg-info/dependency_links.txt
 awsfindingsmanagerlib.egg-info/not-zip-safe
 awsfindingsmanagerlib.egg-info/requires.txt
 awsfindingsmanagerlib.egg-info/top_level.txt
-awsfindingsmanagerlib/__pycache__/__init__.cpython-38.pyc
-awsfindingsmanagerlib/__pycache__/_version.cpython-38.pyc
-awsfindingsmanagerlib/__pycache__/awsfindingsmanagerlib.cpython-38.pyc
-awsfindingsmanagerlib/__pycache__/awsfindingsmanagerlibexceptions.cpython-38.pyc
-awsfindingsmanagerlib/__pycache__/backends.cpython-38.pyc
-awsfindingsmanagerlib/__pycache__/configuration.cpython-38.pyc
-awsfindingsmanagerlib/__pycache__/validations.cpython-38.pyc
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
```

### Comparing `awsfindingsmanagerlib-0.0.0/dev-requirements.txt` & `awsfindingsmanagerlib-0.1.0/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/docs/Makefile` & `awsfindingsmanagerlib-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/docs/conf.py` & `awsfindingsmanagerlib-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/docs/index.rst` & `awsfindingsmanagerlib-0.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/requirements.txt` & `awsfindingsmanagerlib-0.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/setup.py` & `awsfindingsmanagerlib-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `awsfindingsmanagerlib-0.0.0/tests/test_awsfindingsmanagerlib.py` & `awsfindingsmanagerlib-0.1.0/tests/test_awsfindingsmanagerlib.py`

 * *Files identical despite different names*

