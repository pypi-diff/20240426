# Comparing `tmp/data-validation-framework-0.7.4.tar.gz` & `tmp/data_validation_framework-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-validation-framework-0.7.4.tar", last modified: Mon Feb 26 18:03:00 2024, max compression
+gzip compressed data, was "data_validation_framework-0.8.0.tar", last modified: Fri Apr 26 13:32:24 2024, max compression
```

## Comparing `data-validation-framework-0.7.4.tar` & `data_validation_framework-0.8.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:03:00.403126 data-validation-framework-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.auto-changelog
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.auto-changelog-template.hbs
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.codespellignorelines
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:03:00.395126 data-validation-framework-0.7.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:03:00.395126 data-validation-framework-0.7.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.github/ISSUE_TEMPLATE/how_to_use.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:03:00.395126 data-validation-framework-0.7.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.github/workflows/commitlint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-02-26 18:03:00.403126 data-validation-framework-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:03:00.395126 data-validation-framework-0.7.4/data_validation_framework/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/data_validation_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/data_validation_framework/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/data_validation_framework/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/data_validation_framework/rst_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/data_validation_framework/target.py
--rw-r--r--   0 runner    (1001) docker     (127)    29859 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/data_validation_framework/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/data_validation_framework/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:03:00.403126 data-validation-framework-0.7.4/data_validation_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-02-26 18:03:00.000000 data-validation-framework-0.7.4/data_validation_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-02-26 18:03:00.000000 data-validation-framework-0.7.4/data_validation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 18:03:00.000000 data-validation-framework-0.7.4/data_validation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-26 18:03:00.000000 data-validation-framework-0.7.4/data_validation_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-26 18:03:00.000000 data-validation-framework-0.7.4/data_validation_framework.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:03:00.395126 data-validation-framework-0.7.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:03:00.399126 data-validation-framework-0.7.4/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/docs/source/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/docs/source/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 18:03:00.403126 data-validation-framework-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:03:00.399126 data-validation-framework-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:03:00.387126 data-validation-framework-0.7.4/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:03:00.399126 data-validation-framework-0.7.4/tests/data/test_report/
--rw-r--r--   0 runner    (1001) docker     (127)    54609 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tests/data/test_report/report_latexpdf.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    16224 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tests/data/test_report/report_no_exception_rst2pdf.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    17614 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tests/data/test_report/report_rst2pdf.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    15033 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tests/data/test_report/report_rst2pdf_all_fail.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tests/data/test_report/report_rst2pdf_all_success.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    15064 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tests/data/test_report/report_rst2pdf_warnings.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:03:00.403126 data-validation-framework-0.7.4/tests/data/test_report_before_run/
--rw-r--r--   0 runner    (1001) docker     (127)    34465 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tests/data/test_report_before_run/report_latexpdf.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    34807 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tests/data/test_report_before_run/report_latexpdf_with_config.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     9927 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tests/data/test_report_before_run/report_rst2pdf.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    12110 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tests/data/test_report_before_run/report_rst2pdf_nested.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tests/data/test_report_before_run/report_rst2pdf_with_config.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tests/test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tests/test_rst_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tests/test_target.py
--rw-r--r--   0 runner    (1001) docker     (127)   101455 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-02-26 18:02:52.000000 data-validation-framework-0.7.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:32:24.711136 data_validation_framework-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.auto-changelog
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.auto-changelog-template.hbs
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.codespellignorelines
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:32:24.703136 data_validation_framework-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:32:24.703136 data_validation_framework-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.github/ISSUE_TEMPLATE/how_to_use.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:32:24.703136 data_validation_framework-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.github/workflows/commitlint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11686 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-04-26 13:32:24.711136 data_validation_framework-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:32:24.703136 data_validation_framework-0.8.0/data_validation_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/data_validation_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/data_validation_framework/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/data_validation_framework/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/data_validation_framework/rst_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/data_validation_framework/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29916 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/data_validation_framework/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/data_validation_framework/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:32:24.711136 data_validation_framework-0.8.0/data_validation_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-04-26 13:32:24.000000 data_validation_framework-0.8.0/data_validation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-26 13:32:24.000000 data_validation_framework-0.8.0/data_validation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:32:24.000000 data_validation_framework-0.8.0/data_validation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-26 13:32:24.000000 data_validation_framework-0.8.0/data_validation_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 13:32:24.000000 data_validation_framework-0.8.0/data_validation_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:32:24.707136 data_validation_framework-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:32:24.707136 data_validation_framework-0.8.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/docs/source/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/docs/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 13:32:24.711136 data_validation_framework-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:32:24.707136 data_validation_framework-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:32:24.699136 data_validation_framework-0.8.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:32:24.707136 data_validation_framework-0.8.0/tests/data/test_report/
+-rw-r--r--   0 runner    (1001) docker     (127)    54609 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tests/data/test_report/report_latexpdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    16224 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tests/data/test_report/report_no_exception_rst2pdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    17614 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tests/data/test_report/report_rst2pdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    15033 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tests/data/test_report/report_rst2pdf_all_fail.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tests/data/test_report/report_rst2pdf_all_success.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    15064 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tests/data/test_report/report_rst2pdf_warnings.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:32:24.711136 data_validation_framework-0.8.0/tests/data/test_report_before_run/
+-rw-r--r--   0 runner    (1001) docker     (127)    34465 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tests/data/test_report_before_run/report_latexpdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    34807 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tests/data/test_report_before_run/report_latexpdf_with_config.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     9927 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tests/data/test_report_before_run/report_rst2pdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    12110 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tests/data/test_report_before_run/report_rst2pdf_nested.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tests/data/test_report_before_run/report_rst2pdf_with_config.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tests/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tests/test_rst_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tests/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102414 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-26 13:32:20.000000 data_validation_framework-0.8.0/tox.ini
```

### Comparing `data-validation-framework-0.7.4/.auto-changelog` & `data_validation_framework-0.8.0/.auto-changelog`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/.auto-changelog-template.hbs` & `data_validation_framework-0.8.0/.auto-changelog-template.hbs`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/.copier-answers.yml` & `data_validation_framework-0.8.0/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/.github/ISSUE_TEMPLATE/bug_report.yaml` & `data_validation_framework-0.8.0/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/.github/ISSUE_TEMPLATE/feature_request.yaml` & `data_validation_framework-0.8.0/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/.github/ISSUE_TEMPLATE/how_to_use.yaml` & `data_validation_framework-0.8.0/.github/ISSUE_TEMPLATE/how_to_use.yaml`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/.github/dependabot.yml` & `data_validation_framework-0.8.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/.github/pull_request_template.md` & `data_validation_framework-0.8.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/.github/workflows/commitlint.yml` & `data_validation_framework-0.8.0/.github/workflows/commitlint.yml`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/.github/workflows/publish-sdist.yml` & `data_validation_framework-0.8.0/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/.github/workflows/run-tox.yml` & `data_validation_framework-0.8.0/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/.pre-commit-config.yaml` & `data_validation_framework-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/.pylintrc` & `data_validation_framework-0.8.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/CHANGELOG.md` & `data_validation_framework-0.8.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## [0.8.0](https://github.com/BlueBrain/data-validation-framework/compare/0.7.4..0.8.0)
+
+> 26 April 2024
+
+### Fixes
+
+- Add an auto_format parameter to the ValidationResultSet constructor (Adrien Berchet - [#62](https://github.com/BlueBrain/data-validation-framework/pull/62))
+
 ## [0.7.4](https://github.com/BlueBrain/data-validation-framework/compare/0.7.3..0.7.4)
 
 > 26 February 2024
 
 ### Chores And Housekeeping
 
 - Remove warning when creating chunks (Adrien Berchet - [#60](https://github.com/BlueBrain/data-validation-framework/pull/60))
```

### Comparing `data-validation-framework-0.7.4/CONTRIBUTING.md` & `data_validation_framework-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/LICENSE.txt` & `data_validation_framework-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/PKG-INFO` & `data_validation_framework-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-validation-framework
-Version: 0.7.4
+Version: 0.8.0
 Summary: Simple framework to create data validation workflows.
 Home-page: https://data-validation-framework.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: Apache License 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/data-validation-framework/issues
 Project-URL: Source, https://github.com/BlueBrain/data-validation-framework
 Classifier: Development Status :: 4 - Beta
@@ -27,14 +27,15 @@
 Requires-Dist: luigi-tools>=0.0.18
 Requires-Dist: numpy>=1.21
 Requires-Dist: pandas>=1.3
 Requires-Dist: rst2pdf>=0.99
 Requires-Dist: sphinx<8,>=4
 Requires-Dist: tqdm>=4.40
 Provides-Extra: docs
+Requires-Dist: docutils<0.21; extra == "docs"
 Requires-Dist: m2r2; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-bluebrain-theme; extra == "docs"
 Provides-Extra: test
 Requires-Dist: diff_pdf_visually>=1.6.2; extra == "test"
 Requires-Dist: pause>=0.2; extra == "test"
 Requires-Dist: pytest>=7; extra == "test"
```

### Comparing `data-validation-framework-0.7.4/README.md` & `data_validation_framework-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/commitlint.config.js` & `data_validation_framework-0.8.0/commitlint.config.js`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/data_validation_framework/report.py` & `data_validation_framework-0.8.0/data_validation_framework/report.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/data_validation_framework/result.py` & `data_validation_framework-0.8.0/data_validation_framework/result.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,22 +57,17 @@
     out_cols = {
         "is_valid": True,  # if we don't yet have an is_valid, we consider them all
         "ret_code": None,
         "comment": None,
         "exception": None,
     }
 
-    def __init__(self, *args, output_columns=None, **kwargs):
+    def __init__(self, *args, output_columns=None, auto_format=False, **kwargs):
         super().__init__(*args, **kwargs)
-
-        # Skip weird states due to Pandas and tqdm interactions
-        data = kwargs.get("data", args[0] if len(args) > 0 else None)
-        if not isinstance(
-            data, (ValidationResultSet, pd.core.internals.managers.BlockManager)
-        ) and not set(self.index).intersection(set(ValidationResultSet.out_cols.keys())):
+        if auto_format:
             self.format_data(output_columns)
 
     @property
     def _constructor(self):
         """Pandas internal constructor property.
 
         See details here:
```

### Comparing `data-validation-framework-0.7.4/data_validation_framework/rst_tools.py` & `data_validation_framework-0.8.0/data_validation_framework/rst_tools.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/data_validation_framework/target.py` & `data_validation_framework-0.8.0/data_validation_framework/target.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/data_validation_framework/task.py` & `data_validation_framework-0.8.0/data_validation_framework/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -569,15 +569,15 @@
         # Add output columns
         if self.output_columns:
             self._report_cols.extend(
                 [col for col in self.output_columns if col not in self._report_cols]
             )
 
         # Format the DataFrame
-        df = ValidationResultSet(new_df, output_columns=self.output_columns)
+        df = ValidationResultSet(new_df, output_columns=self.output_columns, auto_format=True)
 
         # Copy current index
         index = df.index.copy()
 
         # Apply pre process
         self.pre_process(df, args, kwargs)
 
@@ -699,15 +699,15 @@
         df.loc[(df["is_valid"]) & (df["ret_code"].isnull()), "ret_code"] = 0
         df.loc[(~df["is_valid"]) & (df["ret_code"].isnull()), "ret_code"] = 1
 
         # Fix missing comment and exception values
         df.loc[df["comment"].isnull(), "comment"] = ""
         df.loc[df["exception"].isnull(), "exception"] = ""
 
-        return df
+        return ValidationResultSet(df, auto_format=True)
 
 
 class ValidationWorkflow(SetValidationTask, luigi.WrapperTask):
     """Class to define and process a validation workflow."""
 
     report_path = OptionalStrParameter(
         default=None, description=":str: Path to the workflow report."
```

### Comparing `data-validation-framework-0.7.4/data_validation_framework/util.py` & `data_validation_framework-0.8.0/data_validation_framework/util.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/data_validation_framework.egg-info/PKG-INFO` & `data_validation_framework-0.8.0/data_validation_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-validation-framework
-Version: 0.7.4
+Version: 0.8.0
 Summary: Simple framework to create data validation workflows.
 Home-page: https://data-validation-framework.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: Apache License 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/data-validation-framework/issues
 Project-URL: Source, https://github.com/BlueBrain/data-validation-framework
 Classifier: Development Status :: 4 - Beta
@@ -27,14 +27,15 @@
 Requires-Dist: luigi-tools>=0.0.18
 Requires-Dist: numpy>=1.21
 Requires-Dist: pandas>=1.3
 Requires-Dist: rst2pdf>=0.99
 Requires-Dist: sphinx<8,>=4
 Requires-Dist: tqdm>=4.40
 Provides-Extra: docs
+Requires-Dist: docutils<0.21; extra == "docs"
 Requires-Dist: m2r2; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-bluebrain-theme; extra == "docs"
 Provides-Extra: test
 Requires-Dist: diff_pdf_visually>=1.6.2; extra == "test"
 Requires-Dist: pause>=0.2; extra == "test"
 Requires-Dist: pytest>=7; extra == "test"
```

### Comparing `data-validation-framework-0.7.4/data_validation_framework.egg-info/SOURCES.txt` & `data_validation_framework-0.8.0/data_validation_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/docs/Makefile` & `data_validation_framework-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/docs/source/conf.py` & `data_validation_framework-0.8.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/package.json` & `data_validation_framework-0.8.0/package.json`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/pyproject.toml` & `data_validation_framework-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/setup.py` & `data_validation_framework-0.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "numpy>=1.21",
     "pandas>=1.3",
     "rst2pdf>=0.99",
     "sphinx>=4,<8",
     "tqdm>=4.40",
 ]
 doc_reqs = [
+    "docutils<0.21",  # Temporary fix for m2r2
     "m2r2",
     "sphinx",
     "sphinx-bluebrain-theme",
 ]
 test_reqs = [
     "diff_pdf_visually>=1.6.2",
     "pause>=0.2",
```

### Comparing `data-validation-framework-0.7.4/tests/__init__.py` & `data_validation_framework-0.8.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/tests/conftest.py` & `data_validation_framework-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/tests/data/test_report/report_latexpdf.pdf` & `data_validation_framework-0.8.0/tests/data/test_report/report_latexpdf.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/tests/data/test_report/report_no_exception_rst2pdf.pdf` & `data_validation_framework-0.8.0/tests/data/test_report/report_no_exception_rst2pdf.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/tests/data/test_report/report_rst2pdf.pdf` & `data_validation_framework-0.8.0/tests/data/test_report/report_rst2pdf.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/tests/data/test_report/report_rst2pdf_all_fail.pdf` & `data_validation_framework-0.8.0/tests/data/test_report/report_rst2pdf_all_fail.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/tests/data/test_report/report_rst2pdf_all_success.pdf` & `data_validation_framework-0.8.0/tests/data/test_report/report_rst2pdf_all_success.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/tests/data/test_report/report_rst2pdf_warnings.pdf` & `data_validation_framework-0.8.0/tests/data/test_report/report_rst2pdf_warnings.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/tests/data/test_report_before_run/report_latexpdf.pdf` & `data_validation_framework-0.8.0/tests/data/test_report_before_run/report_latexpdf.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/tests/data/test_report_before_run/report_latexpdf_with_config.pdf` & `data_validation_framework-0.8.0/tests/data/test_report_before_run/report_latexpdf_with_config.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/tests/data/test_report_before_run/report_rst2pdf.pdf` & `data_validation_framework-0.8.0/tests/data/test_report_before_run/report_rst2pdf.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/tests/data/test_report_before_run/report_rst2pdf_nested.pdf` & `data_validation_framework-0.8.0/tests/data/test_report_before_run/report_rst2pdf_nested.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/tests/data/test_report_before_run/report_rst2pdf_with_config.pdf` & `data_validation_framework-0.8.0/tests/data/test_report_before_run/report_rst2pdf_with_config.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/tests/test_result.py` & `data_validation_framework-0.8.0/tests/test_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,48 +30,50 @@
 
 
 class TestValidationResultSet:
     """Test the ValidationResultSet class."""
 
     def test_defaults(self):
         """Check defaults."""
-        df = result.ValidationResultSet(index=["a", "b"])
+        df = result.ValidationResultSet(index=["a", "b"], auto_format=True)
         assert df.to_dict() == {
             "is_valid": {"a": True, "b": True},
             "ret_code": {"a": 0, "b": 0},
             "comment": {"a": None, "b": None},
             "exception": {"a": None, "b": None},
         }
 
     def test_defaults_with_extra_data(self):
         """Check defaults with extra data."""
-        df = result.ValidationResultSet({"a": [1, 2], "b": [3, 4]})
+        df = result.ValidationResultSet({"a": [1, 2], "b": [3, 4]}, auto_format=True)
         assert df.to_dict() == {
             "is_valid": {0: True, 1: True},
             "ret_code": {0: 0, 1: 0},
             "comment": {0: None, 1: None},
             "exception": {0: None, 1: None},
             "a": {0: 1, 1: 2},
             "b": {0: 3, 1: 4},
         }
 
     def test_default_ret_code(self):
         """Check default return code."""
-        df = result.ValidationResultSet({"is_valid": [True, False, True, False]})
+        df = result.ValidationResultSet({"is_valid": [True, False, True, False]}, auto_format=True)
         assert df.to_dict() == {
             "is_valid": {0: True, 1: False, 2: True, 3: False},
             "ret_code": {0: 0, 1: 1, 2: 0, 3: 1},
             "comment": {0: None, 1: None, 2: None, 3: None},
             "exception": {0: None, 1: None, 2: None, 3: None},
         }
 
     def test_output_columns(self):
         """Check output_columns argument."""
         df = result.ValidationResultSet(
-            index=["a", "b"], output_columns={"col1": "val1", "col2": "val2"}
+            index=["a", "b"],
+            output_columns={"col1": "val1", "col2": "val2"},
+            auto_format=True,
         )
         assert df.to_dict() == {
             "is_valid": {"a": True, "b": True},
             "ret_code": {"a": 0, "b": 0},
             "comment": {"a": None, "b": None},
             "exception": {"a": None, "b": None},
             "col1": {"a": "val1", "b": "val1"},
@@ -80,14 +82,15 @@
 
     def test_output_columns_with_existing_columns(self):
         """Check output_columns argument with existing columns."""
         df = result.ValidationResultSet(
             {"is_valid": [True, False], "col1": ["test1", "test2"]},
             index=["a", "b"],
             output_columns={"col1": "val1", "col2": "val2"},
+            auto_format=True,
         )
         assert df.to_dict() == {
             "is_valid": {"a": True, "b": False},
             "ret_code": {"a": 0, "b": 1},
             "comment": {"a": None, "b": None},
             "exception": {"a": None, "b": None},
             "col1": {"a": "test1", "b": "test2"},
@@ -122,17 +125,19 @@
     @pytest.mark.filterwarnings("ignore::numpy.VisibleDeprecationWarning")
     def test_column_order(self):
         """Check column order."""
         df = result.ValidationResultSet(
             {"is_valid": [True, False], "col1": ["test1", "test2"]},
             index=["a", "b"],
             output_columns={"col1": "val1", "col2": "val2"},
+            auto_format=True,
         )
         df_order = result.ValidationResultSet(
-            pd.DataFrame(df[["col2", "comment", "is_valid", "col1", "exception", "ret_code"]])
+            pd.DataFrame(df[["col2", "comment", "is_valid", "col1", "exception", "ret_code"]]),
+            auto_format=True,
         )
         assert df_order.columns.tolist() == [
             "is_valid",
             "ret_code",
             "comment",
             "exception",
             "col1",
@@ -149,15 +154,16 @@
                         "is_valid",
                         "col1",
                         ("tuple", "in", "col"),
                         "exception",
                         "ret_code",
                     ]
                 ]
-            )
+            ),
+            auto_format=True,
         )
         assert df_order.columns.tolist() == [
             "is_valid",
             "ret_code",
             "comment",
             "exception",
             "col1",
@@ -167,12 +173,13 @@
 
     def test_pandas_method(self):
         """Check using as a pandas.DataFrame."""
         df = result.ValidationResultSet(
             {"is_valid": [True, False], "col1": ["test1", "test2"]},
             index=["a", "b"],
             output_columns={"col1": "val1", "col2": "val2"},
+            auto_format=True,
         )
         new_df = result.ValidationResultSet(df)
         assert new_df.apply(lambda x: x.ret_code * 5, axis=1).to_dict() == {"a": 0, "b": 5}
         assert new_df["is_valid"].sum() == 1
         assert new_df["ret_code"].sum() == 1
```

### Comparing `data-validation-framework-0.7.4/tests/test_rst_tools.py` & `data_validation_framework-0.8.0/tests/test_rst_tools.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/tests/test_target.py` & `data_validation_framework-0.8.0/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.4/tests/test_task.py` & `data_validation_framework-0.8.0/tests/test_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1971,14 +1971,41 @@
         assert luigi.build(
             [TestWorkflow(dataset_df=dataset_df_path, result_path=str(tmpdir))],
             local_scheduler=True,
         )
         assert (tmpdir / "TestWorkflow" / "report.csv").exists()
         assert not (tmpdir / "report.pdf").exists()
 
+    def test_recursive_error(self, tmpdir, dataset_df_path):
+        """Check using as a pandas.DataFrame."""
+
+        class TestTask(task.ElementValidationTask):
+            output_columns = {"transformed_morph_path": None}
+
+            @staticmethod
+            def validation_function(row, data_dir):
+                return result.ValidationResult(
+                    is_valid=True, transformed_morph_path="/tmp/test_path"
+                )
+
+        class TestWorkflow(task.ValidationWorkflow):
+            args = ["transformed_dataset.csv", 2]
+
+            @staticmethod
+            def validation_function(df, data_dir, df_path="reduced_df.csv", parents=None):
+                print(df)  # The recursive error was happening here
+
+            def inputs(self):
+                return {TestTask: {}}
+
+        assert luigi.build(
+            [TestWorkflow(dataset_df=dataset_df_path, result_path=str(tmpdir))],
+            local_scheduler=True,
+        )
+
     class TestReport:
         """Test the report generation after workflow run."""
 
         @pytest.fixture
         def TestTask(self, comment, exception):  # noqa: D102
             class TestTask(task.SetValidationTask):
                 """A test validation task."""
```

### Comparing `data-validation-framework-0.7.4/tests/test_util.py` & `data_validation_framework-0.8.0/tests/test_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
                 "is_valid": [True, False, True, True],
                 "a": [1, 2, 3, 4],
                 "b": [4, 5, 6, 7],
                 ("c", "d"): [7, 8, 9, 10],
             }
         ),
         output_columns={"new_data": None, "pid": None},
+        auto_format=True,
     )
 
     res = util.apply_to_df(
         df,
         _tested_func,
         "val1",
         "val2",
```

### Comparing `data-validation-framework-0.7.4/tox.ini` & `data_validation_framework-0.8.0/tox.ini`

 * *Files identical despite different names*

