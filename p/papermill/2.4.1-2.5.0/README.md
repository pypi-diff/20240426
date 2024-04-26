# Comparing `tmp/papermill-2.4.1.tar.gz` & `tmp/papermill-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papermill-2.4.1.tar", last modified: Wed Nov  1 22:53:54 2023, max compression
+gzip compressed data, was "papermill-2.5.0.tar", last modified: Wed Nov  1 22:58:25 2023, max compression
```

## Comparing `papermill-2.4.1.tar` & `papermill-2.5.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:53:54.497899 papermill-2.4.1/
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      129 2023-11-01 22:53:09.000000 papermill-2.4.1/.bumpversion.cfg
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      107 2020-05-26 18:35:36.000000 papermill-2.4.1/CHANGELOG.md
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      125 2023-10-30 20:48:40.000000 papermill-2.4.1/CODE_OF_CONDUCT.md
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     5097 2023-11-01 22:22:44.000000 papermill-2.4.1/CONTRIBUTING.md
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     5794 2020-05-26 18:35:36.000000 papermill-2.4.1/DEVELOPMENT_GUIDE.md
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     1507 2020-05-26 18:35:36.000000 papermill-2.4.1/LICENSE
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      914 2023-11-01 22:22:44.000000 papermill-2.4.1/MANIFEST.in
--rw-r--r--   0 mseal     (1000) mseal     (1000)    13436 2023-11-01 22:53:54.497899 papermill-2.4.1/PKG-INFO
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     7336 2023-11-01 22:22:44.000000 papermill-2.4.1/README.md
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      464 2021-06-06 18:11:26.000000 papermill-2.4.1/RELEASING.md
-drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:53:54.473898 papermill-2.4.1/papermill/
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      192 2020-09-23 20:08:59.000000 papermill-2.4.1/papermill/__init__.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)       80 2021-06-06 18:11:26.000000 papermill-2.4.1/papermill/__main__.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     2670 2023-11-01 22:22:44.000000 papermill-2.4.1/papermill/abs.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     1893 2020-05-26 18:35:36.000000 papermill-2.4.1/papermill/adl.py
--rwxrwxr-x   0 mseal     (1000) mseal     (1000)     9198 2023-11-01 22:22:44.000000 papermill-2.4.1/papermill/cli.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     4348 2020-06-29 17:58:17.000000 papermill-2.4.1/papermill/clientwrap.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)    15489 2023-10-30 20:48:40.000000 papermill-2.4.1/papermill/engines.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     2848 2023-10-30 20:48:40.000000 papermill-2.4.1/papermill/exceptions.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     8501 2023-11-01 22:22:48.000000 papermill-2.4.1/papermill/execute.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     3738 2021-01-20 21:25:25.000000 papermill-2.4.1/papermill/inspection.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)    16097 2022-08-15 03:39:08.000000 papermill-2.4.1/papermill/iorw.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)       79 2020-05-26 18:35:36.000000 papermill-2.4.1/papermill/log.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      264 2022-01-23 00:32:21.000000 papermill-2.4.1/papermill/models.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     3909 2023-10-30 20:48:40.000000 papermill-2.4.1/papermill/parameterize.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)    13919 2022-08-15 03:39:08.000000 papermill-2.4.1/papermill/s3.py
-drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:53:54.477898 papermill-2.4.1/papermill/tests/
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      265 2021-02-27 22:53:27.000000 papermill-2.4.1/papermill/tests/__init__.py
-drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:53:54.477898 papermill-2.4.1/papermill/tests/fixtures/
--rw-rw-r--   0 mseal     (1000) mseal     (1000)        4 2020-05-26 18:35:36.000000 papermill-2.4.1/papermill/tests/fixtures/rock.txt
-drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:53:54.481898 papermill-2.4.1/papermill/tests/notebooks/
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      975 2023-10-30 20:48:40.000000 papermill-2.4.1/papermill/tests/notebooks/binder.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      471 2023-10-30 20:48:40.000000 papermill-2.4.1/papermill/tests/notebooks/blank-vscode.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     1645 2020-08-27 17:00:21.000000 papermill-2.4.1/papermill/tests/notebooks/broken.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     2677 2020-05-26 18:35:36.000000 papermill-2.4.1/papermill/tests/notebooks/broken1.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     2052 2022-08-15 03:39:08.000000 papermill-2.4.1/papermill/tests/notebooks/broken2.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     1020 2020-09-23 20:08:59.000000 papermill-2.4.1/papermill/tests/notebooks/complex_parameters.ipynb
-drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:53:54.469898 papermill-2.4.1/papermill/tests/notebooks/gcs/
-drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:53:54.481898 papermill-2.4.1/papermill/tests/notebooks/gcs/gcs_in/
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     7471 2023-10-30 20:48:40.000000 papermill-2.4.1/papermill/tests/notebooks/gcs/gcs_in/gcs-simple_notebook.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     1423 2020-05-26 18:35:36.000000 papermill-2.4.1/papermill/tests/notebooks/keyboard_interrupt.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      869 2021-01-20 21:25:25.000000 papermill-2.4.1/papermill/tests/notebooks/nb_version_4.4.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      873 2021-08-31 04:31:13.000000 papermill-2.4.1/papermill/tests/notebooks/no_parameters.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      373 2020-09-23 20:08:59.000000 papermill-2.4.1/papermill/tests/notebooks/notimplemented_translator.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      775 2020-05-26 18:35:36.000000 papermill-2.4.1/papermill/tests/notebooks/read_check.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      957 2020-05-26 18:35:36.000000 papermill-2.4.1/papermill/tests/notebooks/report_mode_test.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      917 2020-05-26 18:35:36.000000 papermill-2.4.1/papermill/tests/notebooks/result_no_exec.ipynb
-drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:53:54.469898 papermill-2.4.1/papermill/tests/notebooks/s3/
-drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:53:54.481898 papermill-2.4.1/papermill/tests/notebooks/s3/s3_in/
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      915 2020-05-26 18:35:36.000000 papermill-2.4.1/papermill/tests/notebooks/s3/s3_in/s3-simple_notebook.ipynb
-drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:53:54.481898 papermill-2.4.1/papermill/tests/notebooks/s3/s3_out/
--rw-rw-r--   0 mseal     (1000) mseal     (1000)        0 2020-05-26 18:35:36.000000 papermill-2.4.1/papermill/tests/notebooks/s3/s3_out/.keep
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      910 2022-01-22 22:45:38.000000 papermill-2.4.1/papermill/tests/notebooks/simple_execute.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      871 2020-05-26 18:35:36.000000 papermill-2.4.1/papermill/tests/notebooks/sysexit.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      872 2020-05-26 18:35:36.000000 papermill-2.4.1/papermill/tests/notebooks/sysexit0.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      872 2020-05-26 18:35:36.000000 papermill-2.4.1/papermill/tests/notebooks/sysexit1.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      877 2023-10-30 20:48:40.000000 papermill-2.4.1/papermill/tests/notebooks/systemexit.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      826 2020-05-26 18:35:36.000000 papermill-2.4.1/papermill/tests/notebooks/test_autosave.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     7415 2020-05-26 18:35:36.000000 papermill-2.4.1/papermill/tests/notebooks/test_logging.ipynb
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      272 2023-10-30 20:48:40.000000 papermill-2.4.1/papermill/tests/notebooks/test_notebooknode_io.ipynb
-drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:53:54.481898 papermill-2.4.1/papermill/tests/parameters/
--rw-rw-r--   0 mseal     (1000) mseal     (1000)       14 2020-05-26 18:35:36.000000 papermill-2.4.1/papermill/tests/parameters/example.json
--rw-rw-r--   0 mseal     (1000) mseal     (1000)       74 2023-10-30 20:48:40.000000 papermill-2.4.1/papermill/tests/parameters/example.yaml
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     4954 2023-11-01 22:22:44.000000 papermill-2.4.1/papermill/tests/test_abs.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     2636 2020-05-26 18:35:36.000000 papermill-2.4.1/papermill/tests/test_adl.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     2935 2022-08-15 03:39:08.000000 papermill-2.4.1/papermill/tests/test_autosave.py
--rwxrwxr-x   0 mseal     (1000) mseal     (1000)    19561 2022-08-15 07:32:59.000000 papermill-2.4.1/papermill/tests/test_cli.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     1567 2022-08-15 03:39:08.000000 papermill-2.4.1/papermill/tests/test_clientwrap.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)       22 2020-05-26 18:35:36.000000 papermill-2.4.1/papermill/tests/test_conf.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)    21620 2023-10-30 20:48:40.000000 papermill-2.4.1/papermill/tests/test_engines.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     1568 2023-10-30 20:48:40.000000 papermill-2.4.1/papermill/tests/test_exceptions.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)    19331 2022-10-07 01:10:46.000000 papermill-2.4.1/papermill/tests/test_execute.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     6634 2022-08-15 03:39:08.000000 papermill-2.4.1/papermill/tests/test_gcs.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     1978 2023-11-01 22:22:44.000000 papermill-2.4.1/papermill/tests/test_hdfs.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     3583 2023-10-30 20:48:40.000000 papermill-2.4.1/papermill/tests/test_inspect.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)    14372 2022-08-15 03:39:08.000000 papermill-2.4.1/papermill/tests/test_iorw.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     8267 2022-08-15 03:39:08.000000 papermill-2.4.1/papermill/tests/test_parameterize.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     5725 2022-01-23 00:32:21.000000 papermill-2.4.1/papermill/tests/test_s3.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)    23127 2023-10-30 20:48:40.000000 papermill-2.4.1/papermill/tests/test_translators.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     1644 2022-08-15 03:39:08.000000 papermill-2.4.1/papermill/tests/test_utils.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)    19095 2023-11-01 22:22:44.000000 papermill-2.4.1/papermill/translators.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     4769 2021-03-09 17:49:24.000000 papermill-2.4.1/papermill/utils.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)       18 2023-11-01 22:53:09.000000 papermill-2.4.1/papermill/version.py
-drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:53:54.477898 papermill-2.4.1/papermill.egg-info/
--rw-r--r--   0 mseal     (1000) mseal     (1000)    13436 2023-11-01 22:53:54.000000 papermill-2.4.1/papermill.egg-info/PKG-INFO
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     2703 2023-11-01 22:53:54.000000 papermill-2.4.1/papermill.egg-info/SOURCES.txt
--rw-rw-r--   0 mseal     (1000) mseal     (1000)        1 2023-11-01 22:53:54.000000 papermill-2.4.1/papermill.egg-info/dependency_links.txt
--rw-rw-r--   0 mseal     (1000) mseal     (1000)       59 2023-11-01 22:53:54.000000 papermill-2.4.1/papermill.egg-info/entry_points.txt
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     1604 2023-11-01 22:53:54.000000 papermill-2.4.1/papermill.egg-info/requires.txt
--rw-rw-r--   0 mseal     (1000) mseal     (1000)       10 2023-11-01 22:53:54.000000 papermill-2.4.1/papermill.egg-info/top_level.txt
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      611 2020-05-26 18:35:36.000000 papermill-2.4.1/pyproject.toml
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      164 2023-10-30 20:48:40.000000 papermill-2.4.1/pytest.ini
-drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:53:54.485898 papermill-2.4.1/requirements/
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      100 2023-11-01 22:22:44.000000 papermill-2.4.1/requirements/azure.txt
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      425 2022-08-15 03:39:08.000000 papermill-2.4.1/requirements/dev.txt
--rw-rw-r--   0 mseal     (1000) mseal     (1000)       13 2021-06-06 18:11:26.000000 papermill-2.4.1/requirements/gcs.txt
--rw-rw-r--   0 mseal     (1000) mseal     (1000)       17 2021-08-31 04:31:21.000000 papermill-2.4.1/requirements/github.txt
--rw-rw-r--   0 mseal     (1000) mseal     (1000)       15 2023-10-30 20:48:40.000000 papermill-2.4.1/requirements/hdfs.txt
--rw-rw-r--   0 mseal     (1000) mseal     (1000)        6 2021-06-06 18:11:26.000000 papermill-2.4.1/requirements/s3.txt
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      142 2023-11-01 22:22:44.000000 papermill-2.4.1/requirements.txt
--rw-rw-r--   0 mseal     (1000) mseal     (1000)      534 2023-11-01 22:53:54.497899 papermill-2.4.1/setup.cfg
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     3673 2023-11-01 22:22:44.000000 papermill-2.4.1/setup.py
--rw-rw-r--   0 mseal     (1000) mseal     (1000)     2354 2023-11-01 22:22:44.000000 papermill-2.4.1/tox.ini
--rwxrwxr-x   0 mseal     (1000) mseal     (1000)      155 2023-11-01 22:22:44.000000 papermill-2.4.1/tox_py_installer
+drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:58:25.059989 papermill-2.5.0/
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      129 2023-11-01 22:57:59.000000 papermill-2.5.0/.bumpversion.cfg
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      107 2020-05-26 18:35:36.000000 papermill-2.5.0/CHANGELOG.md
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      125 2023-10-30 20:48:40.000000 papermill-2.5.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     5097 2023-11-01 22:22:44.000000 papermill-2.5.0/CONTRIBUTING.md
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     5794 2020-05-26 18:35:36.000000 papermill-2.5.0/DEVELOPMENT_GUIDE.md
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     1507 2020-05-26 18:35:36.000000 papermill-2.5.0/LICENSE
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      914 2023-11-01 22:22:44.000000 papermill-2.5.0/MANIFEST.in
+-rw-r--r--   0 mseal     (1000) mseal     (1000)    13436 2023-11-01 22:58:25.059989 papermill-2.5.0/PKG-INFO
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     7336 2023-11-01 22:22:44.000000 papermill-2.5.0/README.md
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      464 2021-06-06 18:11:26.000000 papermill-2.5.0/RELEASING.md
+drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:58:25.039989 papermill-2.5.0/papermill/
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      192 2020-09-23 20:08:59.000000 papermill-2.5.0/papermill/__init__.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)       80 2021-06-06 18:11:26.000000 papermill-2.5.0/papermill/__main__.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     2670 2023-11-01 22:22:44.000000 papermill-2.5.0/papermill/abs.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     1893 2020-05-26 18:35:36.000000 papermill-2.5.0/papermill/adl.py
+-rwxrwxr-x   0 mseal     (1000) mseal     (1000)     9198 2023-11-01 22:22:44.000000 papermill-2.5.0/papermill/cli.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     4348 2020-06-29 17:58:17.000000 papermill-2.5.0/papermill/clientwrap.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)    15489 2023-10-30 20:48:40.000000 papermill-2.5.0/papermill/engines.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     2848 2023-10-30 20:48:40.000000 papermill-2.5.0/papermill/exceptions.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     8501 2023-11-01 22:22:48.000000 papermill-2.5.0/papermill/execute.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     3738 2021-01-20 21:25:25.000000 papermill-2.5.0/papermill/inspection.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)    16097 2022-08-15 03:39:08.000000 papermill-2.5.0/papermill/iorw.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)       79 2020-05-26 18:35:36.000000 papermill-2.5.0/papermill/log.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      264 2022-01-23 00:32:21.000000 papermill-2.5.0/papermill/models.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     3909 2023-10-30 20:48:40.000000 papermill-2.5.0/papermill/parameterize.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)    13919 2022-08-15 03:39:08.000000 papermill-2.5.0/papermill/s3.py
+drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:58:25.043989 papermill-2.5.0/papermill/tests/
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      265 2021-02-27 22:53:27.000000 papermill-2.5.0/papermill/tests/__init__.py
+drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:58:25.043989 papermill-2.5.0/papermill/tests/fixtures/
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)        4 2020-05-26 18:35:36.000000 papermill-2.5.0/papermill/tests/fixtures/rock.txt
+drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:58:25.047989 papermill-2.5.0/papermill/tests/notebooks/
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      975 2023-10-30 20:48:40.000000 papermill-2.5.0/papermill/tests/notebooks/binder.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      471 2023-10-30 20:48:40.000000 papermill-2.5.0/papermill/tests/notebooks/blank-vscode.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     1645 2020-08-27 17:00:21.000000 papermill-2.5.0/papermill/tests/notebooks/broken.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     2677 2020-05-26 18:35:36.000000 papermill-2.5.0/papermill/tests/notebooks/broken1.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     2052 2022-08-15 03:39:08.000000 papermill-2.5.0/papermill/tests/notebooks/broken2.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     1020 2020-09-23 20:08:59.000000 papermill-2.5.0/papermill/tests/notebooks/complex_parameters.ipynb
+drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:58:25.035989 papermill-2.5.0/papermill/tests/notebooks/gcs/
+drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:58:25.047989 papermill-2.5.0/papermill/tests/notebooks/gcs/gcs_in/
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     7471 2023-10-30 20:48:40.000000 papermill-2.5.0/papermill/tests/notebooks/gcs/gcs_in/gcs-simple_notebook.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     1423 2020-05-26 18:35:36.000000 papermill-2.5.0/papermill/tests/notebooks/keyboard_interrupt.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      869 2021-01-20 21:25:25.000000 papermill-2.5.0/papermill/tests/notebooks/nb_version_4.4.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      873 2021-08-31 04:31:13.000000 papermill-2.5.0/papermill/tests/notebooks/no_parameters.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      373 2020-09-23 20:08:59.000000 papermill-2.5.0/papermill/tests/notebooks/notimplemented_translator.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      775 2020-05-26 18:35:36.000000 papermill-2.5.0/papermill/tests/notebooks/read_check.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      957 2020-05-26 18:35:36.000000 papermill-2.5.0/papermill/tests/notebooks/report_mode_test.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      917 2020-05-26 18:35:36.000000 papermill-2.5.0/papermill/tests/notebooks/result_no_exec.ipynb
+drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:58:25.035989 papermill-2.5.0/papermill/tests/notebooks/s3/
+drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:58:25.047989 papermill-2.5.0/papermill/tests/notebooks/s3/s3_in/
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      915 2020-05-26 18:35:36.000000 papermill-2.5.0/papermill/tests/notebooks/s3/s3_in/s3-simple_notebook.ipynb
+drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:58:25.047989 papermill-2.5.0/papermill/tests/notebooks/s3/s3_out/
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)        0 2020-05-26 18:35:36.000000 papermill-2.5.0/papermill/tests/notebooks/s3/s3_out/.keep
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      910 2022-01-22 22:45:38.000000 papermill-2.5.0/papermill/tests/notebooks/simple_execute.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      871 2020-05-26 18:35:36.000000 papermill-2.5.0/papermill/tests/notebooks/sysexit.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      872 2020-05-26 18:35:36.000000 papermill-2.5.0/papermill/tests/notebooks/sysexit0.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      872 2020-05-26 18:35:36.000000 papermill-2.5.0/papermill/tests/notebooks/sysexit1.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      877 2023-10-30 20:48:40.000000 papermill-2.5.0/papermill/tests/notebooks/systemexit.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      826 2020-05-26 18:35:36.000000 papermill-2.5.0/papermill/tests/notebooks/test_autosave.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     7415 2020-05-26 18:35:36.000000 papermill-2.5.0/papermill/tests/notebooks/test_logging.ipynb
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      272 2023-10-30 20:48:40.000000 papermill-2.5.0/papermill/tests/notebooks/test_notebooknode_io.ipynb
+drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:58:25.047989 papermill-2.5.0/papermill/tests/parameters/
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)       14 2020-05-26 18:35:36.000000 papermill-2.5.0/papermill/tests/parameters/example.json
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)       74 2023-10-30 20:48:40.000000 papermill-2.5.0/papermill/tests/parameters/example.yaml
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     4954 2023-11-01 22:22:44.000000 papermill-2.5.0/papermill/tests/test_abs.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     2636 2020-05-26 18:35:36.000000 papermill-2.5.0/papermill/tests/test_adl.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     2935 2022-08-15 03:39:08.000000 papermill-2.5.0/papermill/tests/test_autosave.py
+-rwxrwxr-x   0 mseal     (1000) mseal     (1000)    19561 2022-08-15 07:32:59.000000 papermill-2.5.0/papermill/tests/test_cli.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     1567 2022-08-15 03:39:08.000000 papermill-2.5.0/papermill/tests/test_clientwrap.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)       22 2020-05-26 18:35:36.000000 papermill-2.5.0/papermill/tests/test_conf.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)    21620 2023-10-30 20:48:40.000000 papermill-2.5.0/papermill/tests/test_engines.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     1568 2023-10-30 20:48:40.000000 papermill-2.5.0/papermill/tests/test_exceptions.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)    19331 2022-10-07 01:10:46.000000 papermill-2.5.0/papermill/tests/test_execute.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     6634 2022-08-15 03:39:08.000000 papermill-2.5.0/papermill/tests/test_gcs.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     1978 2023-11-01 22:22:44.000000 papermill-2.5.0/papermill/tests/test_hdfs.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     3583 2023-10-30 20:48:40.000000 papermill-2.5.0/papermill/tests/test_inspect.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)    14372 2022-08-15 03:39:08.000000 papermill-2.5.0/papermill/tests/test_iorw.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     8267 2022-08-15 03:39:08.000000 papermill-2.5.0/papermill/tests/test_parameterize.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     5725 2022-01-23 00:32:21.000000 papermill-2.5.0/papermill/tests/test_s3.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)    23127 2023-10-30 20:48:40.000000 papermill-2.5.0/papermill/tests/test_translators.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     1644 2022-08-15 03:39:08.000000 papermill-2.5.0/papermill/tests/test_utils.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)    19095 2023-11-01 22:22:44.000000 papermill-2.5.0/papermill/translators.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     4769 2021-03-09 17:49:24.000000 papermill-2.5.0/papermill/utils.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)       18 2023-11-01 22:57:59.000000 papermill-2.5.0/papermill/version.py
+drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:58:25.043989 papermill-2.5.0/papermill.egg-info/
+-rw-r--r--   0 mseal     (1000) mseal     (1000)    13436 2023-11-01 22:58:24.000000 papermill-2.5.0/papermill.egg-info/PKG-INFO
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     2703 2023-11-01 22:58:24.000000 papermill-2.5.0/papermill.egg-info/SOURCES.txt
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)        1 2023-11-01 22:58:24.000000 papermill-2.5.0/papermill.egg-info/dependency_links.txt
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)       59 2023-11-01 22:58:24.000000 papermill-2.5.0/papermill.egg-info/entry_points.txt
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     1604 2023-11-01 22:58:24.000000 papermill-2.5.0/papermill.egg-info/requires.txt
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)       10 2023-11-01 22:58:24.000000 papermill-2.5.0/papermill.egg-info/top_level.txt
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      611 2020-05-26 18:35:36.000000 papermill-2.5.0/pyproject.toml
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      164 2023-10-30 20:48:40.000000 papermill-2.5.0/pytest.ini
+drwxrwxr-x   0 mseal     (1000) mseal     (1000)        0 2023-11-01 22:58:25.047989 papermill-2.5.0/requirements/
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      100 2023-11-01 22:22:44.000000 papermill-2.5.0/requirements/azure.txt
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      425 2022-08-15 03:39:08.000000 papermill-2.5.0/requirements/dev.txt
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)       13 2021-06-06 18:11:26.000000 papermill-2.5.0/requirements/gcs.txt
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)       17 2021-08-31 04:31:21.000000 papermill-2.5.0/requirements/github.txt
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)       15 2023-10-30 20:48:40.000000 papermill-2.5.0/requirements/hdfs.txt
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)        6 2021-06-06 18:11:26.000000 papermill-2.5.0/requirements/s3.txt
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      142 2023-11-01 22:22:44.000000 papermill-2.5.0/requirements.txt
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)      534 2023-11-01 22:58:25.059989 papermill-2.5.0/setup.cfg
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     3673 2023-11-01 22:22:44.000000 papermill-2.5.0/setup.py
+-rw-rw-r--   0 mseal     (1000) mseal     (1000)     2354 2023-11-01 22:22:44.000000 papermill-2.5.0/tox.ini
+-rwxrwxr-x   0 mseal     (1000) mseal     (1000)      155 2023-11-01 22:22:44.000000 papermill-2.5.0/tox_py_installer
```

### Comparing `papermill-2.4.1/CONTRIBUTING.md` & `papermill-2.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/DEVELOPMENT_GUIDE.md` & `papermill-2.5.0/DEVELOPMENT_GUIDE.md`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/LICENSE` & `papermill-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/MANIFEST.in` & `papermill-2.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/PKG-INFO` & `papermill-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papermill
-Version: 2.4.1
+Version: 2.5.0
 Summary: Parameterize and run Jupyter and nteract Notebooks
 Home-page: https://github.com/nteract/papermill
 Author: nteract contributors
 Author-email: nteract@googlegroups.com
 License: BSD
 Project-URL: Documentation, https://papermill.readthedocs.io
 Project-URL: Funding, https://nteract.io
```

### Comparing `papermill-2.4.1/README.md` & `papermill-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/abs.py` & `papermill-2.5.0/papermill/abs.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/adl.py` & `papermill-2.5.0/papermill/adl.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/cli.py` & `papermill-2.5.0/papermill/cli.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/clientwrap.py` & `papermill-2.5.0/papermill/clientwrap.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/engines.py` & `papermill-2.5.0/papermill/engines.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/exceptions.py` & `papermill-2.5.0/papermill/exceptions.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/execute.py` & `papermill-2.5.0/papermill/execute.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/inspection.py` & `papermill-2.5.0/papermill/inspection.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/iorw.py` & `papermill-2.5.0/papermill/iorw.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/parameterize.py` & `papermill-2.5.0/papermill/parameterize.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/s3.py` & `papermill-2.5.0/papermill/s3.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/binder.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/binder.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/broken.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/broken.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/broken1.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/broken1.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/broken2.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/broken2.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/complex_parameters.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/complex_parameters.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/gcs/gcs_in/gcs-simple_notebook.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/gcs/gcs_in/gcs-simple_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/keyboard_interrupt.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/keyboard_interrupt.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/nb_version_4.4.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/nb_version_4.4.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/no_parameters.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/no_parameters.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/read_check.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/read_check.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/report_mode_test.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/report_mode_test.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/result_no_exec.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/result_no_exec.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/s3/s3_in/s3-simple_notebook.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/s3/s3_in/s3-simple_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/simple_execute.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/simple_execute.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/sysexit.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/sysexit.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/sysexit0.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/sysexit0.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/sysexit1.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/sysexit1.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/systemexit.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/systemexit.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/test_autosave.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/test_autosave.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/notebooks/test_logging.ipynb` & `papermill-2.5.0/papermill/tests/notebooks/test_logging.ipynb`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/test_abs.py` & `papermill-2.5.0/papermill/tests/test_abs.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/test_adl.py` & `papermill-2.5.0/papermill/tests/test_adl.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/test_autosave.py` & `papermill-2.5.0/papermill/tests/test_autosave.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/test_cli.py` & `papermill-2.5.0/papermill/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/test_clientwrap.py` & `papermill-2.5.0/papermill/tests/test_clientwrap.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/test_engines.py` & `papermill-2.5.0/papermill/tests/test_engines.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/test_exceptions.py` & `papermill-2.5.0/papermill/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/test_execute.py` & `papermill-2.5.0/papermill/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/test_gcs.py` & `papermill-2.5.0/papermill/tests/test_gcs.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/test_hdfs.py` & `papermill-2.5.0/papermill/tests/test_hdfs.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/test_inspect.py` & `papermill-2.5.0/papermill/tests/test_inspect.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/test_iorw.py` & `papermill-2.5.0/papermill/tests/test_iorw.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/test_parameterize.py` & `papermill-2.5.0/papermill/tests/test_parameterize.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/test_s3.py` & `papermill-2.5.0/papermill/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/test_translators.py` & `papermill-2.5.0/papermill/tests/test_translators.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/tests/test_utils.py` & `papermill-2.5.0/papermill/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/translators.py` & `papermill-2.5.0/papermill/translators.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill/utils.py` & `papermill-2.5.0/papermill/utils.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill.egg-info/PKG-INFO` & `papermill-2.5.0/papermill.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papermill
-Version: 2.4.1
+Version: 2.5.0
 Summary: Parameterize and run Jupyter and nteract Notebooks
 Home-page: https://github.com/nteract/papermill
 Author: nteract contributors
 Author-email: nteract@googlegroups.com
 License: BSD
 Project-URL: Documentation, https://papermill.readthedocs.io
 Project-URL: Funding, https://nteract.io
```

### Comparing `papermill-2.4.1/papermill.egg-info/SOURCES.txt` & `papermill-2.5.0/papermill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/papermill.egg-info/requires.txt` & `papermill-2.5.0/papermill.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/pyproject.toml` & `papermill-2.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/setup.cfg` & `papermill-2.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/setup.py` & `papermill-2.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `papermill-2.4.1/tox.ini` & `papermill-2.5.0/tox.ini`

 * *Files identical despite different names*

