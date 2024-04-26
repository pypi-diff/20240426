# Comparing `tmp/psyaitools-0.1.0.tar.gz` & `tmp/psyaitools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyaitools-0.1.0.tar", max compression
+gzip compressed data, was "psyaitools-0.1.1.tar", max compression
```

## Comparing `psyaitools-0.1.0.tar` & `psyaitools-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,13 @@
--rw-r--r--   0        0        0    35149 2024-04-19 18:30:19.184238 psyaitools-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2024-04-20 08:26:47.733194 psyaitools-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-20 08:26:47.733116 psyaitools-0.1.0/psyaitools/__init__.py
--rw-r--r--   0        0        0      141 2024-04-20 08:30:23.086419 psyaitools-0.1.0/psyaitools/main.py
--rw-r--r--   0        0        0       23 2024-04-19 18:36:31.305642 psyaitools-0.1.0/psyaitools/res/res.py
--rw-r--r--   0        0        0       23 2024-04-19 18:36:31.719927 psyaitools-0.1.0/psyaitools/src/module.py
--rw-r--r--   0        0        0      294 2024-04-20 08:26:47.736637 psyaitools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      414 1970-01-01 00:00:00.000000 psyaitools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-19 18:30:19.184238 psyaitools-0.1.1/LICENSE
+-rw-r--r--   0        0        0      928 2024-04-26 16:26:27.686146 psyaitools-0.1.1/README.md
+-rw-r--r--   0        0        0     6148 2024-04-26 16:27:46.412536 psyaitools-0.1.1/psyaitools/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-26 09:29:19.590033 psyaitools-0.1.1/psyaitools/functional/IOs/__init__.py
+-rw-r--r--   0        0        0     1680 2024-04-26 14:53:49.167989 psyaitools-0.1.1/psyaitools/functional/IOs/base64_wav.py
+-rw-r--r--   0        0        0      475 2024-04-26 15:59:29.048879 psyaitools-0.1.1/psyaitools/functional/IOs/base64_xfccs.py
+-rw-r--r--   0        0        0      186 2024-04-26 12:45:48.683065 psyaitools-0.1.1/psyaitools/functional/IOs/readFiles.py
+-rw-r--r--   0        0        0      997 2024-04-26 15:06:50.275222 psyaitools-0.1.1/psyaitools/functional/ext/shInst.py
+-rw-r--r--   0        0        0     1527 2024-04-26 16:28:20.020756 psyaitools-0.1.1/psyaitools/functional/representation/factDecomMachine.py
+-rw-r--r--   0        0        0     1075 2024-04-26 15:12:30.918442 psyaitools-0.1.1/psyaitools/functional/representation/xfccs.py
+-rw-r--r--   0        0        0       23 2024-04-19 18:36:31.305642 psyaitools-0.1.1/psyaitools/res/res.py
+-rw-r--r--   0        0        0      414 2024-04-26 16:26:40.031812 psyaitools-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 psyaitools-0.1.1/PKG-INFO
```

### Comparing `psyaitools-0.1.0/LICENSE` & `psyaitools-0.1.1/LICENSE`

 * *Files identical despite different names*

