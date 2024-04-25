# Comparing `tmp/hdx_python_utilities-3.6.7.tar.gz` & `tmp/hdx_python_utilities-3.6.8.tar.gz`

## Comparing `hdx_python_utilities-3.6.7.tar` & `hdx_python_utilities-3.6.8.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     3974 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/requirements.txt
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/.config/coveragerc
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/.config/pytest.ini
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/documentation/.readthedocs.yaml
--rw-r--r--   0        0        0    36044 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/documentation/main.md
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/documentation/pydoc-markdown.yaml
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/_version.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/base_downloader.py
--rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/compare.py
--rwxr-xr-x   0        0        0    35024 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/dateparse.py
--rwxr-xr-x   0        0        0    15753 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/dictandlist.py
--rwxr-xr-x   0        0        0    62652 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/downloader.py
--rwxr-xr-x   0        0        0     2188 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/easy_logging.py
--rwxr-xr-x   0        0        0     8029 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/email.py
--rwxr-xr-x   0        0        0     2203 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/encoding.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/errors_onexit.py
--rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/frictionless_wrapper.py
--rwxr-xr-x   0        0        0     2968 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/html.py
--rwxr-xr-x   0        0        0     6253 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/loader.py
--rwxr-xr-x   0        0        0    17575 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/path.py
--rw-r--r--   0        0        0    19002 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/retriever.py
--rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/saver.py
--rwxr-xr-x   0        0        0     9923 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/session.py
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/state.py
--rwxr-xr-x   0        0        0    13873 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/text.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/typehint.py
--rwxr-xr-x   0        0        0     7152 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/useragent.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/src/hdx/utilities/uuid.py
--rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/test_data.csv
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/compare/test_csv_processing.csv
--rwxr-xr-x   0        0        0      127 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/compare/test_csv_processing2.csv
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/config/empty.yaml
--rwxr-xr-x   0        0        0      483 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/config/hdx_config.json
--rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/config/hdx_config.yaml
--rwxr-xr-x   0        0        0      173 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/config/hdx_email_configuration.json
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/config/hdx_email_configuration.yaml
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/config/json_csv.yaml
--rwxr-xr-x   0        0        0      883 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/config/logging_config.json
--rwxr-xr-x   0        0        0      806 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/config/logging_config.yaml
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/config/project_configuration.json
--rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/config/project_configuration.yaml
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/config/smtp_config.json
--rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/config/smtp_config.yaml
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/config/user_agent_config.yaml
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/config/user_agent_config2.yaml
--rwxr-xr-x   0        0        0       74 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/config/user_agent_config3.yaml
--rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/config/user_agent_config_wrong.yaml
--rwxr-xr-x   0        0        0       31 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/downloader/basicauth.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/downloader/bearertoken.txt
--rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/downloader/extra_params.json
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/downloader/extra_params.yaml
--rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/downloader/extra_params_tree.yaml
--rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/downloader/test_csv_processing.csv
--rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/downloader/test_csv_processing_blanks.csv
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/downloader/test_data.csv
--rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/downloader/test_data.xlsx
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/downloader/test_data2.csv
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/downloader/test_json_processing.json
--rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/downloader/test_xls_processing.xls
--rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/downloader/test_xlsx_processing.xlsx
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/downloader/test_data1.csv/empty.txt
--rwxr-xr-x   0        0        0  1622046 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/html/response.html
--rwxr-xr-x   0        0        0        3 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/loader/empty.json
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/loader/empty.yaml
--rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/retriever/retriever-test.csv
--rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/retriever/test.csv
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/retriever/test.json
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/retriever/test.txt
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/retriever/test.yaml
--rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/retriever/test_hxl.csv
--rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/retriever/fallbacks/test.csv
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/retriever/fallbacks/test.json
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/retriever/fallbacks/test.txt
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/retriever/fallbacks/test.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/saver/out.csv
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/saver/out.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/saver/out2.csv
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/saver/out2.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/saver/out5.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/saver/out6.json
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/saver/out7.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/saver/out8.csv
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/saver/out8.json
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/saver/pretty-false_sortkeys-false.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/saver/pretty-false_sortkeys-false.yaml
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/saver/pretty-false_sortkeys-true.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/saver/pretty-false_sortkeys-true.yaml
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/saver/pretty-true_sortkeys-false.json
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/saver/pretty-true_sortkeys-false.yaml
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/saver/pretty-true_sortkeys-true.json
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/saver/pretty-true_sortkeys-true.yaml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/state/analysis_dates.txt
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/fixtures/state/last_build_date.txt
--rwxr-xr-x   0        0        0     1779 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/conftest.py
--rwxr-xr-x   0        0        0      853 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/utilities/test_compare.py
--rwxr-xr-x   0        0        0     9776 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/utilities/test_dateparse.py
--rwxr-xr-x   0        0        0    13566 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/utilities/test_dictandlist.py
--rwxr-xr-x   0        0        0    50630 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/utilities/test_downloader.py
--rwxr-xr-x   0        0        0      960 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/utilities/test_easy_logging.py
--rwxr-xr-x   0        0        0     5658 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/utilities/test_email.py
--rwxr-xr-x   0        0        0      618 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/utilities/test_encoding.py
--rwxr-xr-x   0        0        0      736 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/utilities/test_errors_onexit.py
--rwxr-xr-x   0        0        0     2412 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/utilities/test_html.py
--rwxr-xr-x   0        0        0     5699 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/utilities/test_loader.py
--rwxr-xr-x   0        0        0    15297 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/utilities/test_path.py
--rwxr-xr-x   0        0        0    21711 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/utilities/test_retriever.py
--rwxr-xr-x   0        0        0    10275 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/utilities/test_saver.py
--rwxr-xr-x   0        0        0     2942 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/utilities/test_state.py
--rwxr-xr-x   0        0        0    14380 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/utilities/test_text.py
--rwxr-xr-x   0        0        0     3542 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/utilities/test_useragent.py
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/utilities/test_uuid.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/tests/hdx/utilities/utils.py
--rwxr-xr-x   0        0        0     1166 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/.gitignore
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/LICENSE
--rwxr-xr-x   0        0        0     1631 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/README.md
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/pyproject.toml
--rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.7/PKG-INFO
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     2910 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/requirements.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/.config/coveragerc
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/.config/pytest.ini
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/documentation/.readthedocs.yaml
+-rw-r--r--   0        0        0    36044 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/documentation/main.md
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/documentation/pydoc-markdown.yaml
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/_version.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/base_downloader.py
+-rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/compare.py
+-rwxr-xr-x   0        0        0    35246 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/dateparse.py
+-rwxr-xr-x   0        0        0    15753 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/dictandlist.py
+-rwxr-xr-x   0        0        0    62652 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/downloader.py
+-rwxr-xr-x   0        0        0     2188 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/easy_logging.py
+-rwxr-xr-x   0        0        0     8029 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/email.py
+-rwxr-xr-x   0        0        0     2203 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/encoding.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/errors_onexit.py
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/frictionless_wrapper.py
+-rwxr-xr-x   0        0        0     2968 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/html.py
+-rwxr-xr-x   0        0        0     6253 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/loader.py
+-rwxr-xr-x   0        0        0    17575 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/path.py
+-rw-r--r--   0        0        0    19002 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/retriever.py
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/saver.py
+-rwxr-xr-x   0        0        0     9923 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/session.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/state.py
+-rwxr-xr-x   0        0        0    13873 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/text.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/typehint.py
+-rwxr-xr-x   0        0        0     7152 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/useragent.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/src/hdx/utilities/uuid.py
+-rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/test_data.csv
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/compare/test_csv_processing.csv
+-rwxr-xr-x   0        0        0      127 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/compare/test_csv_processing2.csv
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/config/empty.yaml
+-rwxr-xr-x   0        0        0      483 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/config/hdx_config.json
+-rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/config/hdx_config.yaml
+-rwxr-xr-x   0        0        0      173 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/config/hdx_email_configuration.json
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/config/hdx_email_configuration.yaml
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/config/json_csv.yaml
+-rwxr-xr-x   0        0        0      883 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/config/logging_config.json
+-rwxr-xr-x   0        0        0      806 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/config/logging_config.yaml
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/config/project_configuration.json
+-rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/config/project_configuration.yaml
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/config/smtp_config.json
+-rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/config/smtp_config.yaml
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/config/user_agent_config.yaml
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/config/user_agent_config2.yaml
+-rwxr-xr-x   0        0        0       74 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/config/user_agent_config3.yaml
+-rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/config/user_agent_config_wrong.yaml
+-rwxr-xr-x   0        0        0       31 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/downloader/basicauth.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/downloader/bearertoken.txt
+-rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/downloader/extra_params.json
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/downloader/extra_params.yaml
+-rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/downloader/extra_params_tree.yaml
+-rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/downloader/test_csv_processing.csv
+-rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/downloader/test_csv_processing_blanks.csv
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/downloader/test_data.csv
+-rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/downloader/test_data.xlsx
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/downloader/test_data2.csv
+-rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/downloader/test_json_processing.json
+-rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/downloader/test_xls_processing.xls
+-rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/downloader/test_xlsx_processing.xlsx
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/downloader/test_data1.csv/empty.txt
+-rwxr-xr-x   0        0        0  1622046 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/html/response.html
+-rwxr-xr-x   0        0        0        3 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/loader/empty.json
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/loader/empty.yaml
+-rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/retriever/retriever-test.csv
+-rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/retriever/test.csv
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/retriever/test.json
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/retriever/test.txt
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/retriever/test.yaml
+-rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/retriever/test_hxl.csv
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/retriever/fallbacks/test.csv
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/retriever/fallbacks/test.json
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/retriever/fallbacks/test.txt
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/retriever/fallbacks/test.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/saver/out.csv
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/saver/out.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/saver/out2.csv
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/saver/out2.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/saver/out5.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/saver/out6.json
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/saver/out7.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/saver/out8.csv
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/saver/out8.json
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/saver/pretty-false_sortkeys-false.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/saver/pretty-false_sortkeys-false.yaml
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/saver/pretty-false_sortkeys-true.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/saver/pretty-false_sortkeys-true.yaml
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/saver/pretty-true_sortkeys-false.json
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/saver/pretty-true_sortkeys-false.yaml
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/saver/pretty-true_sortkeys-true.json
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/saver/pretty-true_sortkeys-true.yaml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/state/analysis_dates.txt
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/fixtures/state/last_build_date.txt
+-rwxr-xr-x   0        0        0     1779 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/conftest.py
+-rwxr-xr-x   0        0        0      853 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/utilities/test_compare.py
+-rwxr-xr-x   0        0        0     9955 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/utilities/test_dateparse.py
+-rwxr-xr-x   0        0        0    13566 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/utilities/test_dictandlist.py
+-rwxr-xr-x   0        0        0    50630 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/utilities/test_downloader.py
+-rwxr-xr-x   0        0        0      960 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/utilities/test_easy_logging.py
+-rwxr-xr-x   0        0        0     5658 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/utilities/test_email.py
+-rwxr-xr-x   0        0        0      618 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/utilities/test_encoding.py
+-rwxr-xr-x   0        0        0      736 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/utilities/test_errors_onexit.py
+-rwxr-xr-x   0        0        0     2412 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/utilities/test_html.py
+-rwxr-xr-x   0        0        0     5699 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/utilities/test_loader.py
+-rwxr-xr-x   0        0        0    15297 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/utilities/test_path.py
+-rwxr-xr-x   0        0        0    21711 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/utilities/test_retriever.py
+-rwxr-xr-x   0        0        0    10275 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/utilities/test_saver.py
+-rwxr-xr-x   0        0        0     2942 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/utilities/test_state.py
+-rwxr-xr-x   0        0        0    14380 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/utilities/test_text.py
+-rwxr-xr-x   0        0        0     3542 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/utilities/test_useragent.py
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/utilities/test_uuid.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/tests/hdx/utilities/utils.py
+-rwxr-xr-x   0        0        0     1166 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/LICENSE
+-rwxr-xr-x   0        0        0     1631 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/README.md
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/pyproject.toml
+-rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.8/PKG-INFO
```

### Comparing `hdx_python_utilities-3.6.7/CONTRIBUTING.md` & `hdx_python_utilities-3.6.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/.config/pre-commit-config.yaml` & `hdx_python_utilities-3.6.8/.config/pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,23 @@
     hooks:
       - id: trailing-whitespace
         exclude: test_loader.py
       - id: end-of-file-fixer
         exclude: (test_csv_processing_blanks.csv|test.txt)
       - id: check-ast
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.2
+    rev: v0.4.2
     hooks:
       # Run the linter.
       - id: ruff
         args: [--config, .config/ruff.toml, --fix]
       # Run the formatter.
       - id: ruff-format
         args: [--config, .config/ruff.toml]
-  - repo: https://github.com/jazzband/pip-tools
-    rev: 7.4.1
+  - repo: https://github.com/astral-sh/uv-pre-commit
+    rev: 0.1.38
     hooks:
+      # Run the pip compile
       - id: pip-compile
         name: pip-compile requirements.txt
         files: pyproject.toml
-        args: [pyproject.toml, --resolver=backtracking, --all-extras, --upgrade, -q, -o, requirements.txt]
+        args: [ pyproject.toml, --resolver=backtracking, --all-extras, --upgrade, -q, -o, requirements.txt ]
```

### Comparing `hdx_python_utilities-3.6.7/.github/workflows/publish.yaml` & `hdx_python_utilities-3.6.8/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/.github/workflows/run-python-tests.yaml` & `hdx_python_utilities-3.6.8/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/documentation/main.md` & `hdx_python_utilities-3.6.8/documentation/main.md`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/documentation/pydoc-markdown.yaml` & `hdx_python_utilities-3.6.8/documentation/pydoc-markdown.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     packages:
       - hdx.utilities
 renderer:
   type: mkdocs
   output_directory: docs
   mkdocs_config:
     site_name: HDX Python Utilities
-    theme: mkdocs
+    theme: material
     repo_url: "https://github.com/OCHA-DAP/hdx-python-utilities"
   markdown:
     source_linker:
       type: github
       repo: OCHA-DAP/hdx-python-utilities
   pages:
     - title: Home
```

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/base_downloader.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/base_downloader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/compare.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/compare.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/dateparse.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/dateparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -646,14 +646,23 @@
 
     Returns:
         datetime: Now with UTC timezone
     """
     return datetime.now(timezone.utc)
 
 
+def now_utc_notz() -> datetime:
+    """Return now in UTC but with timezone removed.
+
+    Returns:
+        datetime: Now in UTC but with timezone removed
+    """
+    return datetime.now(timezone.utc).replace(tzinfo=None)
+
+
 def parse_date_range(
     string: str,
     date_format: Optional[str] = None,
     timezone_handling: int = 0,
     fuzzy: Optional[Dict] = None,
     include_microseconds: bool = False,
     zero_time: bool = False,
```

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/dictandlist.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/dictandlist.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/downloader.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/downloader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/easy_logging.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/easy_logging.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/email.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/email.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/encoding.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/encoding.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/errors_onexit.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/errors_onexit.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/frictionless_wrapper.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/frictionless_wrapper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/html.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/html.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/loader.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/loader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/path.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/path.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/retriever.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/retriever.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/saver.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/saver.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/session.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/session.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/state.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/state.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/text.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/text.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/useragent.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/useragent.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/src/hdx/utilities/uuid.py` & `hdx_python_utilities-3.6.8/src/hdx/utilities/uuid.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/fixtures/test_data.csv` & `hdx_python_utilities-3.6.8/tests/fixtures/test_data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/fixtures/config/json_csv.yaml` & `hdx_python_utilities-3.6.8/tests/fixtures/config/json_csv.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/fixtures/config/logging_config.json` & `hdx_python_utilities-3.6.8/tests/fixtures/config/logging_config.json`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/fixtures/config/logging_config.yaml` & `hdx_python_utilities-3.6.8/tests/fixtures/config/logging_config.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/fixtures/downloader/test_data.xlsx` & `hdx_python_utilities-3.6.8/tests/fixtures/downloader/test_data.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/fixtures/downloader/test_xls_processing.xls` & `hdx_python_utilities-3.6.8/tests/fixtures/downloader/test_xls_processing.xls`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/fixtures/downloader/test_xlsx_processing.xlsx` & `hdx_python_utilities-3.6.8/tests/fixtures/downloader/test_xlsx_processing.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/fixtures/html/response.html` & `hdx_python_utilities-3.6.8/tests/fixtures/html/response.html`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/hdx/conftest.py` & `hdx_python_utilities-3.6.8/tests/hdx/conftest.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/hdx/utilities/test_compare.py` & `hdx_python_utilities-3.6.8/tests/hdx/utilities/test_compare.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/hdx/utilities/test_dateparse.py` & `hdx_python_utilities-3.6.8/tests/hdx/utilities/test_dateparse.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,24 +6,28 @@
 from dateutil.parser import ParserError
 
 from hdx.utilities.dateparse import (
     get_datetime_from_timestamp,
     get_timestamp_from_datetime,
     iso_string_from_datetime,
     now_utc,
+    now_utc_notz,
     parse_date,
     parse_date_range,
 )
 
 
 class TestDateParse:
     def test_now_utc(self):
         assert now_utc().replace(second=0, microsecond=0) == datetime.now(
             timezone.utc
         ).replace(second=0, microsecond=0, tzinfo=timezone.utc)
+        assert now_utc_notz().replace(second=0, microsecond=0) == datetime.now(
+            timezone.utc
+        ).replace(second=0, microsecond=0, tzinfo=None)
 
     def test_parse_date_range(self):
         result = (
             datetime(2013, 2, 10, 0, 0, tzinfo=timezone.utc),
             datetime(2013, 2, 10, 0, 0, tzinfo=timezone.utc),
         )
         assert parse_date_range("10/02/2013") == result
```

### Comparing `hdx_python_utilities-3.6.7/tests/hdx/utilities/test_dictandlist.py` & `hdx_python_utilities-3.6.8/tests/hdx/utilities/test_dictandlist.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/hdx/utilities/test_downloader.py` & `hdx_python_utilities-3.6.8/tests/hdx/utilities/test_downloader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/hdx/utilities/test_easy_logging.py` & `hdx_python_utilities-3.6.8/tests/hdx/utilities/test_easy_logging.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/hdx/utilities/test_email.py` & `hdx_python_utilities-3.6.8/tests/hdx/utilities/test_email.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/hdx/utilities/test_encoding.py` & `hdx_python_utilities-3.6.8/tests/hdx/utilities/test_encoding.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/hdx/utilities/test_errors_onexit.py` & `hdx_python_utilities-3.6.8/tests/hdx/utilities/test_errors_onexit.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/hdx/utilities/test_html.py` & `hdx_python_utilities-3.6.8/tests/hdx/utilities/test_html.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/hdx/utilities/test_loader.py` & `hdx_python_utilities-3.6.8/tests/hdx/utilities/test_loader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/hdx/utilities/test_path.py` & `hdx_python_utilities-3.6.8/tests/hdx/utilities/test_path.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/hdx/utilities/test_retriever.py` & `hdx_python_utilities-3.6.8/tests/hdx/utilities/test_retriever.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/hdx/utilities/test_saver.py` & `hdx_python_utilities-3.6.8/tests/hdx/utilities/test_saver.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/hdx/utilities/test_state.py` & `hdx_python_utilities-3.6.8/tests/hdx/utilities/test_state.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/hdx/utilities/test_text.py` & `hdx_python_utilities-3.6.8/tests/hdx/utilities/test_text.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/hdx/utilities/test_useragent.py` & `hdx_python_utilities-3.6.8/tests/hdx/utilities/test_useragent.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/tests/hdx/utilities/utils.py` & `hdx_python_utilities-3.6.8/tests/hdx/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/.gitignore` & `hdx_python_utilities-3.6.8/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/LICENSE` & `hdx_python_utilities-3.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/README.md` & `hdx_python_utilities-3.6.8/README.md`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/pyproject.toml` & `hdx_python_utilities-3.6.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.7/PKG-INFO` & `hdx_python_utilities-3.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hdx-python-utilities
-Version: 3.6.7
+Version: 3.6.8
 Summary: HDX Python Utilities for streaming tabular data, date and time handling and other helpful functions
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-utilities
 Author-email: Michael Rans <rans@email.com>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,date,datetime,dict,json,library,list,streaming,tabular data,time,timezone,utilities,yaml
 Classifier: Development Status :: 5 - Production/Stable
```

