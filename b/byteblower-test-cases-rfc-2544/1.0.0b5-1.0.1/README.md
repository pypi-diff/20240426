# Comparing `tmp/byteblower_test_cases_rfc_2544-1.0.0b5.tar.gz` & `tmp/byteblower_test_cases_rfc_2544-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byteblower_test_cases_rfc_2544-1.0.0b5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "byteblower_test_cases_rfc_2544-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `byteblower_test_cases_rfc_2544-1.0.0b5.tar` & `byteblower_test_cases_rfc_2544-1.0.1.tar`

### file list

```diff
@@ -1,46 +1,52 @@
--rw-r--r--   0        0        0     8075 2023-11-27 12:51:18.967302 byteblower_test_cases_rfc_2544-1.0.0b5/README.rst
--rw-r--r--   0        0        0       45 2023-11-06 15:33:24.135995 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/.gitignore
--rw-r--r--   0        0        0      167 2023-11-10 10:50:29.616442 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/__init__.py
--rw-r--r--   0        0        0       61 2023-11-06 15:33:24.135995 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/__main__.py
--rw-r--r--   0        0        0      162 2023-11-27 12:51:40.595403 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/_version.py
--rw-r--r--   0        0        0     3721 2023-11-22 10:43:54.607408 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/cli.py
--rw-r--r--   0        0        0     2417 2023-11-06 15:33:24.135995 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/definitions.py
--rw-r--r--   0        0        0     1815 2023-11-06 15:33:24.139996 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/exceptions.py
--rw-r--r--   0        0        0    11134 2023-11-10 15:02:17.267599 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/report_generator.py
--rw-r--r--   0        0        0     1906 2023-11-06 15:33:24.139996 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/scouting_flow.py
--rw-r--r--   0        0        0     1065 2023-11-06 15:33:24.139996 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/config_summary.html
--rw-r--r--   0        0        0  3089944 2023-11-06 15:33:24.191996 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/css/embedded-fonts.css
--rw-r--r--   0        0        0     1295 2023-11-06 15:33:24.191996 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/css/rfc2544.css
--rw-r--r--   0        0        0     7389 2023-11-06 15:33:24.191996 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/css/testframework.css
--rw-r--r--   0        0        0     2751 2023-11-10 15:02:17.267599 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/frame_results.html
--rw-r--r--   0        0        0     1957 2023-11-06 15:33:24.191996 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/pass_fail.html
--rw-r--r--   0        0        0      455 2023-11-06 15:33:24.191996 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/report.html
--rw-r--r--   0        0        0    59284 2023-11-06 15:33:24.195996 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/report_footer.html
--rw-r--r--   0        0        0      128 2023-11-06 15:33:24.195996 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/report_head_style.html
--rw-r--r--   0        0        0    11242 2023-11-06 15:33:24.195996 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/report_header.html
--rw-r--r--   0        0        0      208 2023-11-06 15:33:24.195996 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/report_main.html
--rw-r--r--   0        0        0     2069 2023-11-06 15:33:24.195996 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/results_summary.html
--rw-r--r--   0        0        0    22337 2023-11-06 15:33:24.195996 byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/throughput.py
--rw-r--r--   0        0        0        7 2023-11-06 15:33:24.195996 byteblower_test_cases_rfc_2544-1.0.0b5/docs/.gitignore
--rw-r--r--   0        0        0      638 2023-11-06 15:33:24.199996 byteblower_test_cases_rfc_2544-1.0.0b5/docs/Makefile
--rw-r--r--   0        0        0      769 2023-11-06 15:33:24.199996 byteblower_test_cases_rfc_2544-1.0.0b5/docs/make.bat
--rw-r--r--   0        0        0        0 2023-11-27 12:51:19.095303 byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/_static/.gitkeep
--rw-r--r--   0        0        0     7794 2023-11-10 10:50:29.620442 byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/conf.py
--rw-r--r--   0        0        0     6435 2023-11-22 15:11:44.202834 byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/config_file.rst
--rw-r--r--   0        0        0     6712 2023-11-22 15:11:44.206834 byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/extra/test-cases/rfc-2544/json/config-schema.json
--rw-r--r--   0        0        0      967 2023-11-06 15:33:24.199996 byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/extra/test-cases/rfc-2544/json/rfc_2544.json
--rw-r--r--   0        0        0   105816 2023-11-06 15:33:24.203996 byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/images/html_report_config.png
--rw-r--r--   0        0        0    71007 2023-11-06 15:33:24.203996 byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/images/html_report_error.png
--rw-r--r--   0        0        0    86560 2023-11-06 15:33:24.207996 byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/images/html_report_frame.png
--rw-r--r--   0        0        0   130323 2023-11-06 15:33:24.207996 byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/images/html_report_sum.png
--rw-r--r--   0        0        0    95352 2023-11-06 15:33:24.211996 byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/images/json_results.png
--rw-r--r--   0        0        0   305976 2023-11-06 15:33:24.215996 byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/images/rfc2544_overview.png
--rw-r--r--   0        0        0    10083 2023-11-06 15:33:24.219996 byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/images/rfc2544_setup.png
--rw-r--r--   0        0        0    23589 2023-11-06 15:33:24.219996 byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/images/simple_rfc2544_overview.png
--rw-r--r--   0        0        0      362 2023-11-06 15:33:24.219996 byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/index.rst
--rw-r--r--   0        0        0     6262 2023-11-27 12:51:18.967302 byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/installation.rst
--rw-r--r--   0        0        0      488 2023-11-06 15:33:24.219996 byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/master_index.rst
--rw-r--r--   0        0        0     4917 2023-11-22 15:11:44.206834 byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/overview.rst
--rw-r--r--   0        0        0     8016 2023-11-10 15:02:17.271599 byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/results_highlights.rst
--rw-r--r--   0        0        0     8462 2023-11-11 08:02:18.473354 byteblower_test_cases_rfc_2544-1.0.0b5/pyproject.toml
--rw-r--r--   0        0        0    10852 1970-01-01 00:00:00.000000 byteblower_test_cases_rfc_2544-1.0.0b5/PKG-INFO
+-rw-r--r--   0        0        0     7190 2024-04-26 06:30:25.041297 byteblower_test_cases_rfc_2544-1.0.1/README.rst
+-rw-r--r--   0        0        0       45 2024-01-19 09:38:04.528513 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/.gitignore
+-rw-r--r--   0        0        0      167 2024-01-19 09:38:04.528513 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/__init__.py
+-rw-r--r--   0        0        0       61 2024-01-19 09:38:04.528513 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/__main__.py
+-rw-r--r--   0        0        0     2924 2024-01-24 08:17:31.895841 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/_endpoint_factory.py
+-rw-r--r--   0        0        0     2356 2024-01-31 07:43:12.953194 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/_port_factory.py
+-rw-r--r--   0        0        0      160 2024-04-26 12:28:33.568635 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/_version.py
+-rw-r--r--   0        0        0     3721 2024-01-19 09:38:04.528513 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/cli.py
+-rw-r--r--   0        0        0     2718 2024-01-19 09:38:04.528513 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/definitions.py
+-rw-r--r--   0        0        0     2168 2024-01-24 08:17:31.895841 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/exceptions.py
+-rw-r--r--   0        0        0    11472 2024-04-25 15:09:04.055787 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/report_generator.py
+-rw-r--r--   0        0        0     2124 2024-01-22 15:22:57.638866 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/scouting_flow.py
+-rw-r--r--   0        0        0     1065 2024-01-19 09:38:04.532513 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/config_summary.html
+-rw-r--r--   0        0        0  3089944 2024-01-19 09:38:04.580513 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/css/embedded-fonts.css
+-rw-r--r--   0        0        0     1295 2024-01-19 09:38:04.580513 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/css/rfc2544.css
+-rw-r--r--   0        0        0     7389 2024-01-19 09:38:04.580513 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/css/testframework.css
+-rw-r--r--   0        0        0     2751 2024-01-19 09:38:04.584513 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/frame_results.html
+-rw-r--r--   0        0        0     1957 2024-01-19 09:38:04.584513 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/pass_fail.html
+-rw-r--r--   0        0        0      455 2024-01-19 09:38:04.584513 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/report.html
+-rw-r--r--   0        0        0    59284 2024-01-19 09:38:04.584513 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/report_footer.html
+-rw-r--r--   0        0        0      128 2024-01-19 09:38:04.584513 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/report_head_style.html
+-rw-r--r--   0        0        0    11242 2024-01-19 09:38:04.584513 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/report_header.html
+-rw-r--r--   0        0        0      208 2024-01-19 09:38:04.584513 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/report_main.html
+-rw-r--r--   0        0        0     2069 2024-01-19 09:38:04.584513 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/results_summary.html
+-rw-r--r--   0        0        0    23151 2024-04-25 15:09:04.059787 byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/throughput.py
+-rw-r--r--   0        0        0        7 2024-01-19 09:38:04.588513 byteblower_test_cases_rfc_2544-1.0.1/docs/.gitignore
+-rw-r--r--   0        0        0      638 2024-01-19 09:38:04.588513 byteblower_test_cases_rfc_2544-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0      769 2024-01-19 09:38:04.588513 byteblower_test_cases_rfc_2544-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0      910 2024-01-31 07:43:12.957194 byteblower_test_cases_rfc_2544-1.0.1/docs/source/_include/_example_test_scenario.rst
+-rw-r--r--   0        0        0        0 2024-04-26 12:28:13.992527 byteblower_test_cases_rfc_2544-1.0.1/docs/source/_static/.gitkeep
+-rw-r--r--   0        0        0      301 2024-02-07 15:38:37.810936 byteblower_test_cases_rfc_2544-1.0.1/docs/source/_static/excentis.css
+-rw-r--r--   0        0        0     4027 2024-04-26 06:30:25.041297 byteblower_test_cases_rfc_2544-1.0.1/docs/source/cli.rst
+-rw-r--r--   0        0        0     8672 2024-04-26 06:30:25.041297 byteblower_test_cases_rfc_2544-1.0.1/docs/source/conf.py
+-rw-r--r--   0        0        0     6539 2024-04-26 06:30:25.041297 byteblower_test_cases_rfc_2544-1.0.1/docs/source/config.rst
+-rw-r--r--   0        0        0    13880 2024-04-25 15:19:59.371926 byteblower_test_cases_rfc_2544-1.0.1/docs/source/extra/test-cases/rfc-2544/json/config-schema.json
+-rw-r--r--   0        0        0     1956 2024-04-25 15:19:59.371926 byteblower_test_cases_rfc_2544-1.0.1/docs/source/extra/test-cases/rfc-2544/json/endpoint/rfc_2544.json
+-rw-r--r--   0        0        0     1893 2024-04-25 15:19:59.375926 byteblower_test_cases_rfc_2544-1.0.1/docs/source/extra/test-cases/rfc-2544/json/port/rfc_2544.json
+-rw-r--r--   0        0        0   105816 2024-01-19 09:38:04.592513 byteblower_test_cases_rfc_2544-1.0.1/docs/source/images/html_report_config.png
+-rw-r--r--   0        0        0    71007 2024-01-19 09:38:04.592513 byteblower_test_cases_rfc_2544-1.0.1/docs/source/images/html_report_error.png
+-rw-r--r--   0        0        0    86560 2024-01-19 09:38:04.596513 byteblower_test_cases_rfc_2544-1.0.1/docs/source/images/html_report_frame.png
+-rw-r--r--   0        0        0   130323 2024-01-19 09:38:04.600513 byteblower_test_cases_rfc_2544-1.0.1/docs/source/images/html_report_sum.png
+-rw-r--r--   0        0        0    95352 2024-01-19 09:38:04.600513 byteblower_test_cases_rfc_2544-1.0.1/docs/source/images/json_results.png
+-rw-r--r--   0        0        0   305976 2024-01-19 09:38:04.608513 byteblower_test_cases_rfc_2544-1.0.1/docs/source/images/rfc2544_overview.png
+-rw-r--r--   0        0        0    10083 2024-01-19 09:38:04.608513 byteblower_test_cases_rfc_2544-1.0.1/docs/source/images/rfc2544_setup.png
+-rw-r--r--   0        0        0    23589 2024-01-19 09:38:04.608513 byteblower_test_cases_rfc_2544-1.0.1/docs/source/images/simple_rfc2544_overview.png
+-rw-r--r--   0        0        0      362 2024-01-19 09:38:04.608513 byteblower_test_cases_rfc_2544-1.0.1/docs/source/index.rst
+-rw-r--r--   0        0        0      488 2024-01-31 07:43:12.961195 byteblower_test_cases_rfc_2544-1.0.1/docs/source/master_index.rst
+-rw-r--r--   0        0        0     4583 2024-01-31 12:47:16.024406 byteblower_test_cases_rfc_2544-1.0.1/docs/source/overview.rst
+-rw-r--r--   0        0        0     6448 2024-04-26 06:30:25.041297 byteblower_test_cases_rfc_2544-1.0.1/docs/source/quick_start.rst
+-rw-r--r--   0        0        0     8008 2024-01-31 12:47:16.024406 byteblower_test_cases_rfc_2544-1.0.1/docs/source/results_highlights.rst
+-rw-r--r--   0        0        0     8545 2024-04-26 06:30:25.041297 byteblower_test_cases_rfc_2544-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     9965 1970-01-01 00:00:00.000000 byteblower_test_cases_rfc_2544-1.0.1/PKG-INFO
```

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/README.rst` & `byteblower_test_cases_rfc_2544-1.0.1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 *****************************************
 ByteBlower Test Case: RFC 2544 Throughput
 *****************************************
 
+.. footer::
+   Copyright |copy| |year| - Excentis N.V.
+
+.. |copy| unicode:: U+00A9 .. copyright sign
+.. |year| date:: %Y
+
 Introduction
 ============
 
 This package contains an implementation of the `RFC 2544`_ Throughput
 Test using the `ByteBlower Test Framework`_.
 
 .. _RFC 2544: https://www.ietf.org/rfc/rfc2544.txt
 .. _ByteBlower Test Framework: https://pypi.org/project/byteblower-test-framework/.
 
-.. footer::
-   Copyright |copy| |year| - Excentis N.V.
-
-.. |copy| unicode:: U+00A9 .. copyright sign
-.. |year| date:: %Y
-
 A throughput test aims to measure, under given circumstances,
 the highest throughput the DUT can handle correctly without exceeding a given
 threshold of frame loss (theoretically, this threshold is 0).
 
 This ByteBlower RFC 2544 throughput test case allows you to:
 
 #. Run throughput tests based on RFC 2544
@@ -53,16 +53,16 @@
 We recommend managing the runtime environment in a Python virtual
 environment. This guarantees proper separation of the system-wide
 installed Python and pip packages.
 
 Python
 ------
 
-The ByteBlower Test Framework currently supports Python versions 3.7
-up to 3.11.
+The ByteBlower Test Framework currently supports Python versions
+3.7 up to 3.11.
 
 Important: Working directory
 ----------------------------
 
 All the following sections expect that you first moved to your working
 directory where you want to run this project. You may also want to create
 your configuration files under a sub-directory of your choice.
@@ -165,30 +165,42 @@
 For example (*to get help for the command-line arguments*):
 
 #. As a python module:
 
    .. code-block:: shell
 
       # To get help for the command-line arguments:
-      python -m byteblower.test_case.rfc_2544 --help
+      python -m byteblower.test_cases.rfc_2544 --help
 
 #. As a command-line script:
 
    .. code-block:: shell
 
       # To get help for the command-line arguments:
       byteblower-test-cases-rfc-2544-throughput --help
 
-To run the ByteBlower RFC 2544 throughput test case, you should first provide
-your test configuration, or copy this `Configuration file example`_ to
-``rfc_2544.json`` file you create in your working directory. Make sure to
-update the example configuration to your actual setup configuration
-(ByteBlower server host name or IP, source and destination ports)
+For a quick start, you can run a simple test using the JSON configuration of
+one of the example files below:
+
+* Using `ByteBlower Ports scenario <https://api.byteblower.com/test-framework/json/test-cases/rfc-2544/port/rfc_2544.json>`_
+* Using `ByteBlower Endpoint scenario <https://api.byteblower.com/test-framework/json/test-cases/rfc-2544/endpoint/rfc_2544.json>`_
+
+Save you configuration in your working directory as ``rfc_2544.json``.
+Make sure you change the ``"server"`` and ``"ports"`` configuration
+according to the setup you want to run your test on.
 
-The reports will be stored under a subdirectory ``reports/``.
+More detailed documentation is available in the `Configuration file`_ section
+of the documentation.
+
+.. _Configuration file: https://api.byteblower.com/test-framework/latest/test-cases/rfc-2544/config.html
+
+The ``rfc_2544.json`` can be used then to run the test in the
+command line interface using the following commands:
+
+**Note**: *The reports will be stored under a subdirectory* ``reports/``.
 
 #. On Unix-based systems (Linux, WSL, macOS):
 
    .. code-block:: shell
 
       # Optional: create rfc_2544.json, then copy the configuration to it
       touch rfc_2544.json
@@ -209,69 +221,16 @@
       byteblower-test-cases-rfc-2544-throughput --report-path reports
 
 Integrated
 ----------
 
 .. code-block:: python
 
-   from byteblower.test_case.rfc_2544 import run
+   from byteblower.test_cases.rfc_2544 import run
 
    # Defining test configuration, report path and report file name prefix:
    test_config = {} # Here you should provide your test setup + frame(s') configuration(s)
    report_path = 'my-output-folder' # Optional: provide the path to the output folder, defaults to the current working directory
    report_prefix = 'my-dut-feature-test' # Optional: provide prefix of the output files, defaults to 'report'
 
    # Run the RFC 2544 throughput test:
    run(test_config, report_path=report_path, report_prefix=report_prefix)
-
-
-Configuration file example
---------------------------
-
-.. code-block:: json
-
-   {
-       "server": "byteblower-server.com.",
-       "source": {
-           "name": "Source",
-           "interface": "nontrunk-1",
-           "ipv4": "192.168.5.2",
-           "netmask": "255.255.255.0",
-           "gateway": "192.168.5.254"
-       },
-       "destination": {
-           "name": "Destination",
-           "interface": "trunk-1",
-           "ipv4": "dhcp",
-           "nat": true
-       },
-       "duration": 60,
-       "max_iterations": 25,
-       "frame_configs": [
-           {
-               "size": 60,
-               "initial_bitrate": 3e8,
-               "tolerated_frame_loss": 1e-4,
-               "expected_bitrate": 1.7e8,
-               "accuracy": 1e3
-           },
-           {
-               "size": 124,
-               "initial_bitrate": 6e8,
-               "tolerated_frame_loss": 1e-3,
-               "expected_bitrate": 4.5e8,
-               "accuracy": 1e4
-           },
-           {
-               "size": 252,
-               "initial_bitrate": 7e8,
-               "tolerated_frame_loss": 1e-2,
-               "expected_bitrate": 6.5e8,
-               "accuracy": 1e5
-           }
-       ]
-   }
-
-More detailed documentation is available in the `Configuration file`_ section
-of the documentation.
-
-.. _Configuration file: https://api.byteblower.com/test-framework/latest/test-cases/rfc-2544/config_file.html
```

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/cli.py` & `byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/cli.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/definitions.py` & `byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Shared type definitions and constants."""
+from typing import Any, Dict  # for type hinting
+
 # Default maximum iterations
 MAX_ITERATIONS = 25
 
 # Default packet loss threshold
 MAX_PACKET_LOSS = 0
 
 # Defualt expected  maximum bitrate
@@ -18,74 +21,82 @@
 
 # Maximum number of retries on trial failure
 MAX_RETRY_COUNT = 5
 
 # Default duration of one trial
 DEFAULT_TRIAL_DURATION = 60
 
+# Type aliases
+PortConfig = Dict[str, Any]
+
 LOGGING_PREFIX = 'ByteBlower Test: '
 
-DEFAULT_FRAME_CONFIG = [{
-    "size": 60,
-    "initial_bitrate": 3e8,
-    "tolerated_frame_loss": TOLERATED_FRAME_LOSS,
-    "expected_bitrate": 3.7e8,
-    "accuracy": TEST_ACCURACY
-}, {
-    "size": 124,
-    "initial_bitrate": 6e8,
-    "tolerated_frame_loss": TOLERATED_FRAME_LOSS,
-    "expected_bitrate": 4.5e8,
-    "accuracy": TEST_ACCURACY
-}, {
-    "size": 252,
-    "initial_bitrate": 8e8,
-    "tolerated_frame_loss": TOLERATED_FRAME_LOSS,
-    "expected_bitrate": 5.7e8,
-    "accuracy": TEST_ACCURACY
-}, {
-    "size": 508,
-    "initial_bitrate": 8e8,
-    "tolerated_frame_loss": TOLERATED_FRAME_LOSS,
-    "expected_bitrate": 6.6e8,
-    "accuracy": TEST_ACCURACY
-}, {
-    "size": 1020,
-    "initial_bitrate": 1e9,
-    "tolerated_frame_loss": TOLERATED_FRAME_LOSS,
-    "expected_bitrate": 7.15e8,
-    "accuracy": TEST_ACCURACY
-}, {
-    "size": 1276,
-    "initial_bitrate": 1e9,
-    "tolerated_frame_loss": TOLERATED_FRAME_LOSS,
-    "expected_bitrate": 7.25e8,
-    "accuracy": TEST_ACCURACY
-}, {
-    "size": 1514,
-    "initial_bitrate": 1e9,
-    "tolerated_frame_loss": TOLERATED_FRAME_LOSS,
-    "expected_bitrate": 7.35e8,
-    "accuracy": TEST_ACCURACY
-}]
+DEFAULT_FRAME_CONFIG = [
+    {
+        "size": 60,
+        "initial_bitrate": 3e8,
+        "tolerated_frame_loss": TOLERATED_FRAME_LOSS,
+        "expected_bitrate": 3.7e8,
+        "accuracy": TEST_ACCURACY
+    }, {
+        "size": 124,
+        "initial_bitrate": 6e8,
+        "tolerated_frame_loss": TOLERATED_FRAME_LOSS,
+        "expected_bitrate": 4.5e8,
+        "accuracy": TEST_ACCURACY
+    }, {
+        "size": 252,
+        "initial_bitrate": 8e8,
+        "tolerated_frame_loss": TOLERATED_FRAME_LOSS,
+        "expected_bitrate": 5.7e8,
+        "accuracy": TEST_ACCURACY
+    }, {
+        "size": 508,
+        "initial_bitrate": 8e8,
+        "tolerated_frame_loss": TOLERATED_FRAME_LOSS,
+        "expected_bitrate": 6.6e8,
+        "accuracy": TEST_ACCURACY
+    }, {
+        "size": 1020,
+        "initial_bitrate": 1e9,
+        "tolerated_frame_loss": TOLERATED_FRAME_LOSS,
+        "expected_bitrate": 7.15e8,
+        "accuracy": TEST_ACCURACY
+    }, {
+        "size": 1276,
+        "initial_bitrate": 1e9,
+        "tolerated_frame_loss": TOLERATED_FRAME_LOSS,
+        "expected_bitrate": 7.25e8,
+        "accuracy": TEST_ACCURACY
+    }, {
+        "size": 1514,
+        "initial_bitrate": 1e9,
+        "tolerated_frame_loss": TOLERATED_FRAME_LOSS,
+        "expected_bitrate": 7.35e8,
+        "accuracy": TEST_ACCURACY
+    }
+]
 
 
 class TestProgress():
 
     def __init__(self, estimated_test_iterations):
         self.estimated_test_iterations = estimated_test_iterations
         self._current_iteration = 1
 
-    def test_progress(self, estimated_test_iterations: int,
-                      current_test_iterations: int) -> None:
-        rate = round(current_test_iterations / estimated_test_iterations * 100,
-                     2)
+    def test_progress(
+        self, estimated_test_iterations: int, current_test_iterations: int
+    ) -> None:
+        rate = round(
+            current_test_iterations / estimated_test_iterations * 100, 2
+        )
         # Clear screen before desplay progress bar?
         # run("clear")
         bar = "*" * int(rate)
         print(f"Estimated progress state {rate}%".center(100, " "))
         print(bar + "\n")
 
     def next_iteration(self):
-        self.test_progress(self.estimated_test_iterations,
-                           self._current_iteration)
+        self.test_progress(
+            self.estimated_test_iterations, self._current_iteration
+        )
         self._current_iteration += 1
```

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/exceptions.py` & `byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,21 +6,38 @@
 
 
 # Exceptions related to misconfigured parameters
 class ConfigFileError(Rfc2544Exception):
     pass
 
 
+class InvalidInput(Rfc2544Exception):
+    """
+    Raised when the user provided invalid input values.
+
+    .. versionchanged:: 1.0.0
+       Improved exception handling.
+    """
+
+
 class FrameSizeMissing(ConfigFileError):
 
     def __init__(self):
         message = "Frame size missing"
         super().__init__(message)
 
 
+class MissingParameter(ConfigFileError):
+    """
+    Raised when a configuration parameter is missing in the configuration file.
+
+    .. versionadded:: 1.0.0
+    """
+
+
 class DiffSubnet(ConfigFileError):
 
     def __init__(self):
         message = "IP address and gateway are not in the same subnet"
         super().__init__(message)
 
 
@@ -59,9 +76,9 @@
         message = f"Frame loss reached 100% on frame size {frame_size}. Check setup for eventual failures"
         super().__init__(message)
 
 
 class PortLayer3Mismatch(TrialException):
 
     def __init__(self):
-        message = "Source and destination ports Layer 3 different"
+        message = "Source and destination ports IP version is different"
         super().__init__(message)
```

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/report_generator.py` & `byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/report_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,19 @@
     return str(timedelta)[:-4]
 
 
 def format_datetime_iso(dt: datetime):
     return dt.isoformat()
 
 
-_JINJA2_ENV = jinja2.Environment(loader=jinja2.FileSystemLoader(
-    searchpath=join(_PACKAGE_DIRECTORY, 'templates')))
+_JINJA2_ENV = jinja2.Environment(
+    loader=jinja2.FileSystemLoader(
+        searchpath=join(_PACKAGE_DIRECTORY, 'templates')
+    )
+)
 _JINJA2_ENV.filters['total_seconds'] = timedelta_to_seconds
 _JINJA2_ENV.filters['iso_format'] = format_datetime_iso
 _JINJA2_ENV.filters['str'] = timedelta_to_str
 _TEMPLATE = _JINJA2_ENV.get_template("report.html")
 
 
 def _chart_options(x_axis: Dict, title: str, y_axis: List[Dict]) -> Dict:
@@ -84,67 +87,73 @@
         "chart": {
             "zoomType": "xy"
         },
         "title": {
             "text": title,
             "align": "center"
         },
-        "xAxis": [{
-            "title": {
-                "text": x_axis['text'],
-                "style": {
-                    "color": "black"
-                }
-            },
-            "categories": x_axis['values'],
-        }],
-        "yAxis": [{
-            "labels": {
-                "format": "{value}" + y_axis[0].get("value", "Mb/s"),
-                "style": {
-                    "color": "Highcharts.getOptions().colors[0]"
-                }
-            },
-            "title": {
-                "text": y_axis[0].get("text", "Bitrate"),
-                "style": {
-                    "color": "Highcharts.getOptions().colors[0]"
-                }
-            },
-            "min": y_axis[0].get("min", 0),
-        }]
+        "xAxis": [
+            {
+                "title": {
+                    "text": x_axis['text'],
+                    "style": {
+                        "color": "black"
+                    }
+                },
+                "categories": x_axis['values'],
+            }
+        ],
+        "yAxis": [
+            {
+                "labels": {
+                    "format": "{value}" + y_axis[0].get("value", "Mb/s"),
+                    "style": {
+                        "color": "Highcharts.getOptions().colors[0]"
+                    }
+                },
+                "title": {
+                    "text": y_axis[0].get("text", "Bitrate"),
+                    "style": {
+                        "color": "Highcharts.getOptions().colors[0]"
+                    }
+                },
+                "min": y_axis[0].get("min", 0),
+            }
+        ]
     }
     if len(y_axis) > 1:
-        options["yAxis"].append({
-            "title": {
-                "text": y_axis[1].get("text", "Frame loss"),
-                "style": {
-                    "color": "Highcharts.getOptions().colors[1]"
-                }
-            },
-            "labels": {
-                "format": "{value}" + y_axis[1].get("value", "%"),
-                "style": {
-                    "color": "Highcharts.getOptions().colors[1]"
-                }
-            },
-            "min": y_axis[1].get("min", 0),
-            "opposite": "true"
-        })
+        options["yAxis"].append(
+            {
+                "title": {
+                    "text": y_axis[1].get("text", "Frame loss"),
+                    "style": {
+                        "color": "Highcharts.getOptions().colors[1]"
+                    }
+                },
+                "labels": {
+                    "format": "{value}" + y_axis[1].get("value", "%"),
+                    "style": {
+                        "color": "Highcharts.getOptions().colors[1]"
+                    }
+                },
+                "min": y_axis[1].get("min", 0),
+                "opposite": "true"
+            }
+        )
     options['legend'] = {'align': 'center', 'verticalAlign': 'bottom'}
     return options
 
 
 def _summary_plot_generator(
     result_dict: List[Dict],
     plot_name: str,
     title: str,
     yaxis: List[Dict],
-    series=List[Dict],
-):
+    series: List[Dict],
+) -> str:
     # data preparation
     x_axis = {"values": [x['size'] for x in result_dict], 'text': 'Frame size'}
     chart = Highchart(renderTo=plot_name)
     chart.set_dict_options(_chart_options(x_axis, title, yaxis))
     for serie in series:
         if serie['data'] == 'trials':
             data = [len(x[serie['data']]) for x in result_dict]
@@ -156,71 +165,79 @@
         else:
             data = [round(x[serie['data']] / 1e6, 2) for x in result_dict]
         chart.add_data_set(
             data=data,
             series_type=serie.get('series_type', 'column'),
             name=serie['title'],
             yAxis=serie.get('yaxis', 0),
-            tooltip={'valueSuffix': serie.get('valueSuffix', '')})
+            tooltip={'valueSuffix': serie.get('valueSuffix', '')}
+        )
     chart.buildhtml()
     return chart.content
 
 
 def _final_plots_generator(results: List[Dict]):
-    plot1 = [{
-        'data': 'real_bitrate',
-        'title': 'Tested bitrate',
-        'valueSuffix': 'Mb/s'
-    }, {
-        'data': 'expected_bitrate',
-        'title': 'Expected bitrate',
-        'valueSuffix': 'Mb/s'
-    }]
-    plot2 = [{
-        'data': 'trials',
-        'title': 'Number of Trials',
-    }, {
-        'data': 'test_duration',
-        'title': 'Test duration',
-        "type": 'datetime',
-        "labels": {
-            "formatter":
-            """
+    plot1 = [
+        {
+            'data': 'real_bitrate',
+            'title': 'Tested bitrate',
+            'valueSuffix': 'Mb/s'
+        }, {
+            'data': 'expected_bitrate',
+            'title': 'Expected bitrate',
+            'valueSuffix': 'Mb/s'
+        }
+    ]
+    plot2 = [
+        {
+            'data': 'trials',
+            'title': 'Number of Trials',
+        }, {
+            'data': 'test_duration',
+            'title': 'Test duration',
+            "type": 'datetime',
+            "labels": {
+                "formatter":
+                """
                     function() {
                         var seconds = this.value % 60 ;
                         var minutes = Math.floor((this.value / 60 ) % 60);
                         var hours = Math.floor(this.value / 3600);
                         return hours + 'h ' + minutes + 'm ' + seconds + 's';
                     }
                     """
-        },
-        'yaxis': 1,
-    }]
-    yaxis = [{
-        'text': 'Trials',
-        'value': ''
-    }, {
-        'text': 'Duration',
-        'value': 's'
-    }]
+            },
+            'yaxis': 1,
+        }
+    ]
+    yaxis = [
+        {
+            'text': 'Trials',
+            'value': ''
+        }, {
+            'text': 'Duration',
+            'value': 's'
+        }
+    ]
 
     return [
         _summary_plot_generator(
             result_dict=results,
             plot_name='plot1',
             title='Real vs Expected throughputs',
             yaxis=[{}],
             series=plot1,
         ),
         _summary_plot_generator(
             result_dict=results,
             plot_name='plot2',
             title='Duration & number Trials per frame size',
             yaxis=yaxis,
-            series=plot2)
+            series=plot2
+        )
     ]
 
 
 def _frame_plot_generator(result_dict: Dict, series_type: str = 'spline'):
     # data & config preparation
     frame_loss = [
         round(1 - x['rx_packets'] / x['tx_packets'], 4) * 100
@@ -234,25 +251,31 @@
     }
     # Other configuration of the y axis
     y_axis = [{'min': 0}, {'min': 0, 'text': 'Frame loss', 'value': '%'}]
 
     # Generate the charts
     chart = Highchart(renderTo="plot_" + str(result_dict['size']))
     chart.set_dict_options(
-        _chart_options(x_axis, "Tested bitrate & Frame loss per iteration",
-                       y_axis))
-    chart.add_data_set(data=bitrates,
-                       series_type=series_type,
-                       name='Tested bitrate',
-                       tooltip={'valueSuffix': 'Mb/s'})
-    chart.add_data_set(data=frame_loss,
-                       series_type=series_type,
-                       name='Frame loss',
-                       yAxis=1,
-                       tooltip={'valueSuffix': '%'})
+        _chart_options(
+            x_axis, "Tested bitrate & Frame loss per iteration", y_axis
+        )
+    )
+    chart.add_data_set(
+        data=bitrates,
+        series_type=series_type,
+        name='Tested bitrate',
+        tooltip={'valueSuffix': 'Mb/s'}
+    )
+    chart.add_data_set(
+        data=frame_loss,
+        series_type=series_type,
+        name='Frame loss',
+        yAxis=1,
+        tooltip={'valueSuffix': '%'}
+    )
     # Building and returning the js code of the charts
     chart.buildhtml()
     return chart.content
 
 
 def html_report_generator(
     configuration: Dict,
@@ -280,24 +303,27 @@
        defaults to :const:`MAX_ITERATIONS`
     :type max_ieration: int, optional
     :param iteration_duration: duration of one iteration in seconds,
        defaults to :const:`DEFAULT_TRIAL_DURATION`
     :type iteration_duration: int, optional
     """
     #Total duration of the entire test
-    total_test_duration = sum([x["test_duration"] for x in results],
-                              timedelta())
+    total_test_duration = sum(
+        [x["test_duration"] for x in results], timedelta()
+    )
     # Generate the summary plots
     summary_plots = _final_plots_generator(results)
 
     # Detailed results + plots for each frame size
-    container = [{
-        "plot": _frame_plot_generator(frame),
-        "frame": frame
-    } for frame in results]
+    container = [
+        {
+            "plot": _frame_plot_generator(frame),
+            "frame": frame
+        } for frame in results
+    ]
 
     api_version = ByteBlower.InstanceGet().APIVersionGet()
     chart = Highchart(offline=True)
     chart.buildhtmlheader()
     js_resources = chart.htmlheader
     quote_head, quote_tagline = _QUOTES[0]
```

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/scouting_flow.py` & `byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/scouting_flow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 from time import sleep
 from typing import Any, Mapping, Optional, Sequence, Union  # for type hinting
 
 from byteblower_test_framework.endpoint import Port  # for type hinting
-from byteblower_test_framework.traffic import UDP_DYNAMIC_PORT_START, IPv4Frame
+from byteblower_test_framework.factory import create_frame
+from byteblower_test_framework.traffic import UDP_DYNAMIC_PORT_START
 from byteblowerll.byteblower import Stream  # for type hinting
 
 from .exceptions import PortLayer3Mismatch
 
 # Type aliases
 _FrameConfig = Mapping[str, Any]
 _ImixFrameConfig = Mapping[str, int]
 _ImixFrameConfigCollection = Sequence[_ImixFrameConfig]
 _ImixConfig = Mapping[str, Union[int, _ImixFrameConfigCollection]]
 
 
 class ScoutingFlow:
+    """Prepares the network for the actual traffic defined in the test."""
 
     @staticmethod
     def run_udp_flow(
         source: Port,
         destination: Port,
         frame_config: Optional[_FrameConfig] = None,
     ) -> None:
         if source.layer3.__class__ != destination.layer3.__class__:
             raise PortLayer3Mismatch()
 
+        # Create frame
+        frame = create_frame(source, **(frame_config or {}))
+        frame_content = frame.build_frame_content(source, destination)
+
         # Configure stream
         stream: Stream = source.bb_port.TxStreamAdd()
         stream.InterFrameGapSet(100 * 1000 * 1000)  # 100ms
         stream.NumberOfFramesSet(10)
 
         # Add frame to the stream
-        frame = IPv4Frame(**(frame_config or dict()))
-        frame._add(source, destination, stream)
+        frame.add(frame_content, stream)
 
         # Start resolution process
         stream.Start()
 
         sleep(1)
 
         # Stop stream (should have stopped by itself already)
```

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/config_summary.html` & `byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/config_summary.html`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/css/embedded-fonts.css` & `byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/css/embedded-fonts.css`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/css/rfc2544.css` & `byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/css/rfc2544.css`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/css/testframework.css` & `byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/css/testframework.css`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/frame_results.html` & `byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/frame_results.html`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/pass_fail.html` & `byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/pass_fail.html`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/report_footer.html` & `byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/report_footer.html`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/report_header.html` & `byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/report_header.html`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/templates/results_summary.html` & `byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/templates/results_summary.html`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/byteblower/test_cases/rfc_2544/throughput.py` & `byteblower_test_cases_rfc_2544-1.0.1/byteblower/test_cases/rfc_2544/throughput.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,69 @@
+"""Main test execution with given test configuration (from JSON file)."""
 import logging
 from collections import defaultdict
 # import webbrowser
 from datetime import datetime, timedelta
 from enum import Enum
 from ipaddress import IPv4Network, IPv6Network
 from os import getcwd
 from os.path import join
 from time import sleep
-from typing import Optional  # for type hinting
-from typing import Any, Dict, List, Mapping, Sequence, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union  # for type hinting
 
 from byteblower_test_framework.analysis import FrameLossAnalyser
-from byteblower_test_framework.endpoint import Port  # for type hinting
-from byteblower_test_framework.endpoint import IPv4Port, IPv6Port, NattedPort
+from byteblower_test_framework.endpoint import (  # for type hinting
+    Endpoint,
+    IPv4Port,
+    IPv6Port,
+    NatDiscoveryIPv4Port,
+    Port,
+)
 from byteblower_test_framework.exceptions import log_api_error
-from byteblower_test_framework.host import Server
+from byteblower_test_framework.host import MeetingPoint, Server
 from byteblower_test_framework.run import Scenario
-from byteblower_test_framework.traffic import (FrameBlastingFlow, IPv4Frame,
-                                               IPv6Frame)
-
-from .definitions import (DEFAULT_FRAME_CONFIG, DEFAULT_TRIAL_DURATION,
-                          INITIAL_BITRATE, LOGGING_PREFIX, MAX_ITERATIONS,
-                          MAX_RETRY_COUNT, SLEEP_TIME, TEST_ACCURACY,
-                          TOLERATED_FRAME_LOSS, TestProgress)
-from .exceptions import (AllFramesLost, ConfigFileError, DiffSubnet,
-                         DuplicateFrames, FrameSizeMissing, MaxRetriesReached,
-                         OtherTrialException, PortLayer3Mismatch,
-                         TrialException)
+from byteblower_test_framework.traffic import (
+    FrameBlastingFlow,
+    IPv4Frame,
+    IPv6Frame,
+)
+from byteblowerll.byteblower import ByteBlowerAPIException
+
+from ._endpoint_factory import initialize_endpoint
+from ._port_factory import initialize_port
+from .definitions import (
+    DEFAULT_FRAME_CONFIG,
+    DEFAULT_TRIAL_DURATION,
+    INITIAL_BITRATE,
+    LOGGING_PREFIX,
+    MAX_ITERATIONS,
+    MAX_RETRY_COUNT,
+    SLEEP_TIME,
+    TEST_ACCURACY,
+    TOLERATED_FRAME_LOSS,
+    PortConfig,
+    TestProgress,
+)
+from .exceptions import (
+    AllFramesLost,
+    ConfigFileError,
+    DiffSubnet,
+    DuplicateFrames,
+    FrameSizeMissing,
+    InvalidInput,
+    MaxRetriesReached,
+    OtherTrialException,
+    PortLayer3Mismatch,
+    TrialException,
+)
 from .report_generator import html_report_generator, json_report_generator
 from .scouting_flow import ScoutingFlow
 
 __all__ = ('run', )
 
-# Type aliases
-_PortConfig = Mapping[str, Any]
-_FlowConfig = Mapping[str, Any]
-
 
 def run(test_config: dict, report_path: str, report_prefix: str) -> None:
     """RFC 2544 throughput test for a set of frame configurations.
 
     The frame configurations consist of frame size without CRC,
     expected bitrate, ...
 
@@ -48,36 +72,43 @@
     :type test_config: dict
     :param report_path: Path where to store the report files
     :type report_path: str
     :param report_prefix: Prefix of the report files
     :type report_prefix: str
     :raises MaxRetriesReached: Occurs when number of trial retries exceeds
        the allowed :const:`MAX_RETRY_COUNT`
+
+    .. versionchanged:: 1.0.0
+       Add support for ByteBlower Endpoint.
     """
     try:
         (
             frame_configs,
             max_iteration,
             duration,
             server_name,
-            source_port_configs,
-            destination_port_configs,
+            meeting_point,
+            source_port_config,
+            destination_port_config,
             test_progress,
         ) = _rfc2544_test_initialization(test_config)
         error_logs = defaultdict(list)
         rfc_test_results = {
             "configuration": {
                 'server': server_name,
-                'source': source_port_configs,
-                'destination': destination_port_configs
+                'source': source_port_config,
+                'destination': destination_port_config
             },
             "frame": [],
             "status": False,
             "error_logs": error_logs,
         }
+        if meeting_point is not None:
+            rfc_test_results['configuration']['meeting_point'] = meeting_point
+
         _rfc2544_all_frames(
             frame_configs,
             rfc_test_results,
             duration,
             max_iteration,
             test_progress,
         )
@@ -87,52 +118,70 @@
     else:
         # Check if at least one result is recorded
         if rfc_test_results['frame']:
             logging.info("RFC 2544 throughput test has finished")
             rfc_test_results["status"] = not error_logs
             path_and_prefix = join(
                 report_path or getcwd(),
-                report_prefix + "_" + datetime.now().strftime('%Y%m%d_%H%M%S'))
+                report_prefix + "_" + datetime.now().strftime('%Y%m%d_%H%M%S')
+            )
 
             # Export results into  JSON file
             json_report_generator(rfc_test_results, path_and_prefix + ".json")
 
             # Gererate HTML report
             html_report_generator(
                 rfc_test_results["configuration"],
                 rfc_test_results["frame"],
                 dict(error_logs),
                 path_and_prefix + ".html",
                 status=rfc_test_results["status"],
             )
 
 
-def _rfc2544_all_frames(frame_configs, rfc_test_results, duration,
-                        max_iteration, test_progress):
+def _rfc2544_all_frames(
+    frame_configs,
+    rfc_test_results,
+    duration,
+    max_iteration,
+    test_progress,
+):
     error_logs = rfc_test_results['error_logs']
     server_name = rfc_test_results['configuration']['server']
-    source_port_configs = rfc_test_results['configuration']['source']
-    destination_port_configs = rfc_test_results['configuration']['destination']
+    meeting_point_name = rfc_test_results['configuration'].get('meeting_point')
+    source_port_config = rfc_test_results['configuration']['source']
+    destination_port_config = rfc_test_results['configuration']['destination']
     previous_max_bitrate = INITIAL_BITRATE
     last_index = len(frame_configs) - 1
     #overall_test_status: True  if all tests finished correctly, else is false
     overall_test_status = True
     for frame_conf_index, frame_conf in enumerate(frame_configs):
         try:
             frame_size = frame_conf['size']
-            initial_bitrate = frame_conf.get("initial_bitrate",
-                                             previous_max_bitrate)
+            initial_bitrate = frame_conf.get(
+                "initial_bitrate", previous_max_bitrate
+            )
             # Create new test scenario
             scenario = Scenario()
             # Connect to the ByteBlower Server
             server = Server(server_name)
 
+            # Connect to the Meeting Point if provided
+            meeting_point = MeetingPoint(
+                meeting_point_name
+            ) if meeting_point_name else None
+
             # initialize the ports
             source_port, destination_port = _initialize_ports(
-                server, source_port_configs, destination_port_configs)
+                server,
+                meeting_point,
+                source_port_config,
+                destination_port_config,
+            )
+
             # Initialize traffic flows
             udp_flow: FrameBlastingFlow
             udp_flow_analyzer: FrameLossAnalyser
             udp_flow, udp_flow_analyzer = _initialize_frameblasting_flows(
                 scenario,
                 source_port,
                 destination_port,
@@ -198,16 +247,17 @@
     frame_conf_index,
     last_index,
 ):
     # Limit number of iterations/framesize : 25 iteration/frame_size
     frame_size = frame_conf["size"]
     test_accuracy = frame_conf.get("accuracy", TEST_ACCURACY)
     test_bitrate = initial_bitrate
-    tolerated_packet_loss = frame_conf.get("tolerated_frame_loss",
-                                           TOLERATED_FRAME_LOSS)
+    tolerated_packet_loss = frame_conf.get(
+        "tolerated_frame_loss", TOLERATED_FRAME_LOSS
+    )
     trials = []
     frame_results = {
         "size": frame_size,
         "tolerated_frame_loss": tolerated_packet_loss,
         "expected_bitrate": frame_conf["expected_bitrate"],
         "trials": trials,
         "real_bitrate": None,
@@ -223,15 +273,15 @@
         # Limit number of iterations/framesize : 25 iteration/frame_size
         while True:
             if restart_count >= MAX_RETRY_COUNT:
                 raise MaxRetriesReached(frame_size, MAX_RETRY_COUNT)
             try:
 
                 # Initialize scouting flows
-                _send_scouting_flows(source_port, destination_port)
+                _run_scouting_flows(source_port, destination_port)
                 trial_duration, sent, received = _run_trial(
                     scenario,
                     duration,
                     udp_flow_analyzer,
                     frame_size,
                 )
                 test_progress.next_iteration()
@@ -241,44 +291,61 @@
                 _exception_handler(
                     frame_size,
                     error,
                     error_logs,
                     restart_count=restart_count,
                 )
                 continue
+            except ByteBlowerAPIException as error:
+                restart_count += 1
+                _exception_handler(
+                    frame_size,
+                    error,
+                    error_logs,
+                    restart_count=restart_count,
+                    hint=(
+                        f"ByteBlower API exception !!  Check ==> {error.getMessage()}"
+                    )
+                )
+                continue
             except Exception as error:
                 restart_count += 1
                 _exception_handler(
                     frame_size,
                     error,
                     error_logs,
                     restart_count=restart_count,
                     hint=(
                         f"Unexpected exception occurred !!  Check ==> {error}"
-                    ))
+                    )
+                )
                 continue
             # Save trial results
             test_status = (1 - (received / sent)) <= tolerated_packet_loss
 
             # trial_duration
             trials.append(
-                _results_dict_generator(test_status, test_bitrate,
-                                        received, sent, trial_duration,
-                                        datetime.utcnow()))
+                _results_dict_generator(
+                    test_status, test_bitrate, received, sent, trial_duration,
+                    datetime.utcnow()
+                )
+            )
             diff = (max_bitrate - min_bitrate) / 2
             if (test_status
                     and diff < test_accuracy) or trial_count > max_iteration:
                 logging.info(
                     "Throughput test for frame size %d is done successfully",
-                    frame_size)
+                    frame_size
+                )
                 break
             else:
                 # Calculate next biterate
                 min_bitrate, max_bitrate, test_bitrate = _rfc2544_throughput(
-                    test_status, test_bitrate, min_bitrate, max_bitrate, diff)
+                    test_status, test_bitrate, min_bitrate, max_bitrate, diff
+                )
                 # ! TODO: Move this functionality to the byteblower-test-framework
                 # Update flow parameters
                 frame_rate = test_bitrate / (frame_size * 8)
                 udp_flow._frame_rate = frame_rate
                 udp_flow._number_of_frames = int(frame_rate * duration)
                 trial_count += 1
                 # ! **************************************************************
@@ -308,16 +375,16 @@
     frame_test_duration = datetime.utcnow() - frame_test_start
     frame_results["real_bitrate"] = test_bitrate
     return test_bitrate, frame_test_duration, frame_results, frame_status
 
 
 def _run_trial(
     scenario: Scenario,
-    duration: int,
-    udp_flow_analyzer,
+    duration: float,
+    udp_flow_analyzer: FrameLossAnalyser,
     frame_size: int,
 ) -> Tuple[timedelta, int, int]:
     logging.info('%sStarting', LOGGING_PREFIX)
     scenario.run(maximum_run_time=timedelta(seconds=duration))
     trial_duration = scenario.duration
     # display progresss bar
 
@@ -327,16 +394,21 @@
     if received == 0:
         raise AllFramesLost(frame_size)
     if received > sent:
         raise DuplicateFrames(frame_size, received - sent)
     return trial_duration, sent, received
 
 
-def _rfc2544_throughput(test_status: bool, test_bitrate: float, min_bitrate,
-                        max_bitrate, diff) -> Tuple[float, float, float]:
+def _rfc2544_throughput(
+    test_status: bool,
+    test_bitrate: float,
+    min_bitrate,
+    max_bitrate,
+    diff,
+) -> Tuple[float, float, float]:
     if min_bitrate > max_bitrate:
         max_bitrate = min_bitrate
         min_bitrate = 0
     if diff == 0:  # min_bitrate == max_bitrate
         min_bitrate = 0.5 * min_bitrate
     if test_bitrate > max_bitrate:
         max_bitrate = test_bitrate
@@ -353,72 +425,82 @@
             test_bitrate += diff
         max_bitrate = test_bitrate
 
     return min_bitrate, max_bitrate, test_bitrate
 
 
 def _rfc2544_test_initialization(test_config):
-    frame_configs: List(Dict) = test_config.get('frame_configs',
-                                                DEFAULT_FRAME_CONFIG)
+    frame_configs: List[Dict] = test_config.get(
+        'frame_configs', DEFAULT_FRAME_CONFIG
+    )
     _frame_config_check(frame_configs)
     max_iteration = test_config.get('max_iterations', MAX_ITERATIONS)
-    # Read server/ports configuration
+    # Read server and meeting point
     server_name = test_config['server']
-    source_port_configs = test_config['source']
-    destination_port_configs = test_config['destination']
-    _port_config_check(source_port_configs)
-    _port_config_check(destination_port_configs)
+    meeting_point_name = test_config.get('meeting_point', None)
+    # ports configuration parameters
+    source_port_config = test_config['source']
+    destination_port_config = test_config['destination']
+    _port_config_check(source_port_config)
+    _port_config_check(destination_port_config)
     # Trial duration
+
     duration = test_config.get('maximum_run_time', DEFAULT_TRIAL_DURATION)
     # Approximately 19 iteration / frame size => To be used only for progress bar
     estimated_test_iterations = len(frame_configs) * 19
     test_progress = TestProgress(estimated_test_iterations)
     return (
         frame_configs,
         max_iteration,
         duration,
         server_name,
-        source_port_configs,
-        destination_port_configs,
+        meeting_point_name,
+        source_port_config,
+        destination_port_config,
         test_progress,
     )
 
 
-def _error_dict_generator(exception: str,
-                          error_msg: str,
-                          timestamp: str,
-                          hint: Optional[str] = None) -> dict:
+def _error_dict_generator(
+    exception: str,
+    error_msg: str,
+    timestamp: str,
+    hint: Optional[str] = None,
+) -> dict:
 
     results_dict = {
         "exception": exception,
         "error_msg": error_msg,
         "timestamp": timestamp,
     }
     if hint:
         results_dict["hint"] = hint
     return results_dict
 
 
 def _exception_handler(
     frame_size: int,
-    execption: Exception,
+    exception: Exception,
     error_logs,
     restart_count: Optional[int] = None,
     hint: Optional[str] = None,
 ) -> None:
     if hint:
         logging.exception(hint)
     else:
-        logging.error("%s: %s", type(execption).__name__, execption)
+        logging.error("%s: %s", type(exception).__name__, exception)
     error_logs[frame_size].append(
         _error_dict_generator(
-            type(execption).__name__, execption, datetime.utcnow(), hint))
+            type(exception).__name__, exception, datetime.utcnow(), hint
+        )
+    )
     if restart_count is not None:
-        logging.info("Attempt to restart test (%d) in %ds", restart_count,
-                     SLEEP_TIME)
+        logging.info(
+            "Attempt to restart test (%d) in %ds", restart_count, SLEEP_TIME
+        )
         sleep(SLEEP_TIME)
 
 
 def _frame_config_check(frame_configs) -> None:
     for config in frame_configs:
         if config.get('size') is None:
             raise FrameSizeMissing()
@@ -440,167 +522,181 @@
                     strict=False) != IPv6Network(
                         f"{port_config['gateway']}/{port_config['netmask']}",
                         strict=False):
                 raise DiffSubnet()
     return True
 
 
-def _results_dict_generator(status: bool, tested_Th: float, rx_packets: int,
-                            tx_packets: int, duration: float,
-                            timestamp: str) -> dict:
+def _results_dict_generator(
+    status: bool,
+    tested_Th: float,
+    rx_packets: int,
+    tx_packets: int,
+    duration: float,
+    timestamp: str,
+) -> dict:
 
     results_dict = {
         "bitrate": tested_Th,
         "passed": status,
         "tx_packets": tx_packets,
         "rx_packets": rx_packets,
         "timestamp": timestamp,
         "duration": duration
     }
     return results_dict
 
 
-class PortFactory:
-
-    @staticmethod
-    def build_port(server: Server, **port_config) -> Port:
-        if 'ipv4' in port_config:
-            nat = port_config.pop('nat', False)
-            if nat:
-                port_class = NattedPort
+def _initialize_ports(
+    server: Server,
+    meeting_point: Optional[MeetingPoint],
+    source_port_config: PortConfig,
+    destination_port_config: PortConfig,
+) -> List[Port]:
+    """Initialize source and destination ports.
+
+    :param server: Server instance to create the ports on.
+    :type server: Server
+    :param meeting_point: MeetingPoint instance to create the endpoint on.
+    :type meeting_point: Optional[MeetingPoint]
+    :param source_port_config: Configuration parameters for the source port.
+    :type source_port_config: PortConfig
+    :param destination_port_config: Configuration parameters for the
+    destination port.
+    :type destination_port_config: PortConfig
+    :return: list of source Port and destination Port.
+    :rtype: List[Port]
+    """
+    ports = []
+    for port_config in (source_port_config, destination_port_config):
+        # Build destination port
+        if 'interface' in port_config:
+            port = initialize_port(server, port_config)
+        elif 'uuid' in port_config:
+            if meeting_point is not None:
+                port = initialize_endpoint(meeting_point, port_config)
             else:
-                port_class = IPv4Port
-        elif 'ipv6' in port_config:
-            port_class = IPv6Port
-        name = port_config.pop('name', None)
-        port = port_class(server, name=name, **port_config)
-        return port
+                raise InvalidInput(
+                    "Please provide meeting point address"
+                    " to initialize endpoint"
+                )
+        else:
+            raise InvalidInput(
+                "Please provide either Port or Endpoint configuration"
+            )
 
+        ports.append(port)
 
-def _initialize_ports(
-    server, source_port_configs: Union[Sequence[_PortConfig], _PortConfig],
-    destination_port_configs: Union[Sequence[_PortConfig], _PortConfig]
-) -> Tuple[Port, Port]:
-
-    # Build source port
-    logging.info('%sInitializing Source port', LOGGING_PREFIX)
-    source_port: Port = PortFactory.build_port(server, **source_port_configs)
-    logging.info(
-        '%sInitialized Source port %r'
-        ' with IP address %r, network %r', LOGGING_PREFIX, source_port.name,
-        source_port.ip, source_port.network)
-
-    # Build destination port
-    destination_port: Port = PortFactory.build_port(server,
-                                                    **destination_port_configs)
-    logging.info(
-        '%sInitialized Destination port %r'
-        ' with IP address %r, network %r', LOGGING_PREFIX,
-        destination_port.name, destination_port.ip, destination_port.network)
-
-    return source_port, destination_port
-
-
-def _send_scouting_flows(
-    source_port: Port,
-    destination_port: Port,
-    udp_flow_config: Optional[_FlowConfig] = None,
-    frame_size: Optional[int] = None,
-) -> None:
-    # UDP (Frame Blasting) flows
-    if udp_flow_config is not None:
-        _frameblasting_scouting_flows(source_port,
-                                      destination_port,
-                                      frame_size=frame_size)
+    return ports
 
 
 class FlowType(Enum):
     ipv4 = 'IPv4'
     ipv6 = 'IPv6'
 
 
-def _frameblasting_scouting_flows(source_port: Port,
-                                  destination_port: Port,
-                                  frame_size: Optional[int] = None) -> None:
-
-    #! NOTE - **WORKAROUND** !
-    #        * First sending upstream scouting frames to freshen NAT
-    #        * entries avoiding unexpected traffic loss in either
-    #        * direction, likely caused by *new NAT entries*.
-    if isinstance(destination_port, NattedPort):
-        _send_udp_scounting_flow(destination_port, source_port, frame_size)
-    else:
-        _send_udp_scounting_flow(source_port, destination_port, frame_size)
+def _run_scouting_flows(
+    source_port: Union[Port, Endpoint],
+    destination_port: Union[Port, Endpoint],
+    frame_size: Optional[int] = None,
+) -> None:
+    # Scouting flows are only needed for BB Ports,
+    # for BB endpoint it is handled because we do address (NAT) resolution.
+    if isinstance(source_port, Port) and isinstance(destination_port, Port):
+        if isinstance(destination_port, NatDiscoveryIPv4Port):
+            #! NOTE - **WORKAROUND** !
+            #        * First sending upstream scouting frames to freshen NAT
+            #        * entries avoiding unexpected traffic loss in either
+            #        * direction, likely caused by *new NAT entries*.
+            _run_frameblasting_scouting_flow(
+                destination_port, source_port, frame_size
+            )
+        else:
+            _run_frameblasting_scouting_flow(
+                source_port, destination_port, frame_size
+            )
 
 
-def _send_udp_scounting_flow(cpe_port: Port, nsi_port: Port,
-                             frame_size: int) -> None:
+def _run_frameblasting_scouting_flow(
+    cpe_port: Port,
+    nsi_port: Port,
+    frame_size: int,
+) -> None:
     try:
         # First, send "upstream" traffic
-        ScoutingFlow.run_udp_flow(cpe_port,
-                                  nsi_port,
-                                  frame_config={"length": frame_size})
+        ScoutingFlow.run_udp_flow(
+            cpe_port, nsi_port, frame_config={"length": frame_size}
+        )
         # Secondly, send "downstream" traffic
-        ScoutingFlow.run_udp_flow(nsi_port,
-                                  cpe_port,
-                                  frame_config={"length": frame_size})
+        ScoutingFlow.run_udp_flow(
+            nsi_port, cpe_port, frame_config={"length": frame_size}
+        )
     except PortLayer3Mismatch as error:
-        logging.warning("%s: Skipping upstream/downstream scouting flow",
-                        error)
+        logging.warning(
+            "%s: Skipping upstream/downstream scouting flow", error
+        )
 
 
 class FlowFactory:
 
     @staticmethod
     def create_udp_flow(
-            source: Port,
-            destination: Port,
-            bitrate: float,
-            frame_size: Optional[int] = None,
-            flow_name_suffix: str = 'UDP traffic') -> FrameBlastingFlow:
+        source: Union[Port, Endpoint],
+        destination: Union[Port, Endpoint],
+        bitrate: float,
+        frame_size: Optional[int] = None,
+        flow_name_suffix: str = 'UDP traffic',
+    ) -> FrameBlastingFlow:
         # Parse arguments
         # NOTE - Create a copy before altering.
         # Determine flow type and create frame
         if isinstance(source, IPv4Port):
             # Using default configuration if no frame_config given:
             frame = IPv4Frame(length=frame_size)
             flow_type = FlowType.ipv4
         elif isinstance(source, IPv6Port):
             # Using default configuration if no frame_config given:
             frame = IPv6Frame(length=frame_size)
             flow_type = FlowType.ipv6
         else:
             raise ValueError(
-                f'Unsupported Port type: {type(source).__name__!r}')
+                f'Unsupported Port type: {type(source).__name__!r}'
+            )
 
         # Configure frame blasting flow
         destination_port = destination
-        flow_name = '{} - {} {}'.format(destination_port.name, flow_type.value,
-                                        flow_name_suffix)
+        flow_name = '{} - {} {}'.format(
+            destination_port.name, flow_type.value, flow_name_suffix
+        )
         try:
-            flow = FrameBlastingFlow(source,
-                                     destination,
-                                     name=flow_name,
-                                     bitrate=bitrate,
-                                     frame_list=[frame])
+            flow = FrameBlastingFlow(
+                source,
+                destination,
+                name=flow_name,
+                bitrate=bitrate,
+                frame_list=[frame],
+            )
             return flow
         except Exception as error:
             logging.error(error)
 
 
 @log_api_error
 def _initialize_frameblasting_flows(
-        scenario: Scenario,
-        source_port: Port,
-        destination_port: Port,
-        bitrate: float,
-        frame_size: int = None) -> Tuple[FrameBlastingFlow, FrameLossAnalyser]:
+    scenario: Scenario,
+    source_port: Union[Port, Endpoint],
+    destination_port: Union[Port, Endpoint],
+    bitrate: float,
+    frame_size: int = None,
+) -> Tuple[FrameBlastingFlow, FrameLossAnalyser]:
     # Create frame blasting flow & Add analyzer
-    udp_flow = FlowFactory.create_udp_flow(source_port,
-                                           destination_port,
-                                           bitrate,
-                                           frame_size=frame_size)
+    udp_flow = FlowFactory.create_udp_flow(
+        source_port,
+        destination_port,
+        bitrate,
+        frame_size=frame_size,
+    )
     udp_flow_analyser = FrameLossAnalyser()
     udp_flow.add_analyser(udp_flow_analyser)
     # Add frame blasting flow to the scenario
     scenario.add_flow(udp_flow)
     return udp_flow, udp_flow_analyser
```

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/docs/Makefile` & `byteblower_test_cases_rfc_2544-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/docs/make.bat` & `byteblower_test_cases_rfc_2544-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/conf.py` & `byteblower_test_cases_rfc_2544-1.0.1/docs/source/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Configuration file for the Sphinx documentation builder.
 #
-# For the full list of built-in configuration values, see the documentation:
+# This file only contains a selection of the most common options. For the full
+# list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
@@ -48,20 +49,29 @@
     'sphinx_tabs.tabs',
     'sphinx-jsonschema',
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
+# The language for content autogenerated by Sphinx. Refer to documentation
+# for a list of supported languages.
+#
+# This is also used if you do content translation via gettext catalogs.
+# Usually you set "language" from the command line for these cases.
+# language = 'en'  # default
+# XXX - By default, build using default English
+# language = 'nl'
+
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = []
-
-language = 'en'
+exclude_patterns = [
+    '_include/*.rst',
+]
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
@@ -78,14 +88,22 @@
 pygments_style = 'sphinx'
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
+# A list of CSS files. The entry must be a filename string or a tuple
+# containing the filename string and the attributes dictionary.
+# The filename must be relative to the html_static_path, or a full URI
+# with scheme like https://example.org/style.css.
+# The attributes is used for attributes of <link> tag.
+# It defaults to an empty list.
+html_css_files = ['excentis.css']
+
 # If true, “Created using Sphinx” is shown in the HTML footer.
 # Default is True.
 html_show_sphinx = False
 
 # If true, the reST sources are included in the HTML build as _sources/name.
 # The default is True.
 html_copy_source = False
@@ -175,14 +193,15 @@
 # See:
 #   https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#confval-autodoc_inherit_docstrings
 # autodoc_inherit_docstrings = True  # default
 
 # -- Options for intersphinx extension ---------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/extensions/intersphinx.html#configuration
 
+# Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
 }
 
 # -- Options for todo extension ----------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/extensions/todo.html#configuration
```

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/extra/test-cases/rfc-2544/json/rfc_2544.json` & `byteblower_test_cases_rfc_2544-1.0.1/docs/source/extra/test-cases/rfc-2544/json/endpoint/rfc_2544.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6008928571428572%*

 * *Differences: {"'$schema'": "'https://api.byteblower.com/test-framework/json/test-cases/rfc-2544/config-schema.json'",*

 * * "'destination'": "{'ipv4': True, 'uuid': '4d9a5fdb-32b4-4523-ace9-5972518de13b', delete: "*

 * *                  "['interface', 'nat']}",*

 * * "'frame_configs'": "{0: {'initial_bitrate': 3000000.0, 'tolerated_frame_loss': 0.001, 'accuracy': "*

 * *                    "10000.0}, 1: {'initial_bitrate': 6000000.0}, 2: {'initial_bitrate': "*

 * *                    "8000000.0, 'tolerated_frame_loss': 0.001, 'expected_bitrate […]*

```diff
@@ -1,40 +1,69 @@
 {
+    "$schema": "https://api.byteblower.com/test-framework/json/test-cases/rfc-2544/config-schema.json",
     "destination": {
-        "interface": "trunk-1",
-        "ipv4": "dhcp",
+        "ipv4": true,
         "name": "Destination",
-        "nat": true
+        "uuid": "4d9a5fdb-32b4-4523-ace9-5972518de13b"
     },
     "duration": 60,
     "frame_configs": [
         {
-            "accuracy": 1000.0,
+            "accuracy": 10000.0,
             "expected_bitrate": 170000000.0,
-            "initial_bitrate": 300000000.0,
+            "initial_bitrate": 3000000.0,
             "size": 60,
-            "tolerated_frame_loss": 0.0001
+            "tolerated_frame_loss": 0.001
         },
         {
             "accuracy": 10000.0,
             "expected_bitrate": 450000000.0,
-            "initial_bitrate": 600000000.0,
+            "initial_bitrate": 6000000.0,
             "size": 124,
             "tolerated_frame_loss": 0.001
         },
         {
-            "accuracy": 100000.0,
-            "expected_bitrate": 650000000.0,
-            "initial_bitrate": 700000000.0,
+            "accuracy": 1000.0,
+            "expected_bitrate": 570000000.0,
+            "initial_bitrate": 8000000.0,
             "size": 252,
-            "tolerated_frame_loss": 0.01
+            "tolerated_frame_loss": 0.001
+        },
+        {
+            "accuracy": 1000.0,
+            "expected_bitrate": 660000000.0,
+            "initial_bitrate": 800000000.0,
+            "size": 508,
+            "tolerated_frame_loss": 0.001
+        },
+        {
+            "accuracy": 100.0,
+            "expected_bitrate": 715000000.0,
+            "initial_bitrate": 1000000000.0,
+            "size": 1020,
+            "tolerated_frame_loss": 0.001
+        },
+        {
+            "accuracy": 100.0,
+            "expected_bitrate": 725000000.0,
+            "initial_bitrate": 1000000000.0,
+            "size": 1276,
+            "tolerated_frame_loss": 0.001
+        },
+        {
+            "accuracy": 100.0,
+            "expected_bitrate": 735000000.0,
+            "initial_bitrate": 1000000000.0,
+            "size": 1514,
+            "tolerated_frame_loss": 0.001
         }
     ],
     "max_iterations": 25,
-    "server": "byteblower-server.com.",
+    "meeting_point": "byteblower-meeting-point.example.com.",
+    "server": "byteblower-server.example.com.",
     "source": {
         "gateway": "192.168.5.254",
         "interface": "nontrunk-1",
         "ipv4": "192.168.5.2",
         "name": "Source",
         "netmask": "255.255.255.0"
     }
```

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/images/html_report_config.png` & `byteblower_test_cases_rfc_2544-1.0.1/docs/source/images/html_report_config.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/images/html_report_error.png` & `byteblower_test_cases_rfc_2544-1.0.1/docs/source/images/html_report_error.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/images/html_report_frame.png` & `byteblower_test_cases_rfc_2544-1.0.1/docs/source/images/html_report_frame.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/images/html_report_sum.png` & `byteblower_test_cases_rfc_2544-1.0.1/docs/source/images/html_report_sum.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/images/json_results.png` & `byteblower_test_cases_rfc_2544-1.0.1/docs/source/images/json_results.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/images/rfc2544_overview.png` & `byteblower_test_cases_rfc_2544-1.0.1/docs/source/images/rfc2544_overview.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/images/rfc2544_setup.png` & `byteblower_test_cases_rfc_2544-1.0.1/docs/source/images/rfc2544_setup.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/images/simple_rfc2544_overview.png` & `byteblower_test_cases_rfc_2544-1.0.1/docs/source/images/simple_rfc2544_overview.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/installation.rst` & `byteblower_test_cases_rfc_2544-1.0.1/docs/source/quick_start.rst`

 * *Files 18% similar despite different names*

```diff
@@ -87,17 +87,18 @@
 
 .. tabs::
 
    .. group-tab:: Windows
 
       On Windows systems using PowerShell:
 
-         **Note**: On Microsoft Windows, it may be required to enable the
-         Activate.ps1 script by setting the execution policy for the user.
-         You can do this by issuing the following PowerShell command:
+         .. note::
+            On Microsoft Windows, it may be required to enable the
+            Activate.ps1 script by setting the execution policy for the user.
+            You can do this by issuing the following PowerShell command:
 
          .. code-block:: shell
 
             PS C:> Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
 
          See `About Execution Policies`_ for more information.
 
@@ -112,27 +113,28 @@
          & ".\env\Scripts\activate.ps1"
          python -m pip install -U pip build
 
    .. group-tab:: Linux and macOS
 
       On Unix-based systems (Linux, WSL, macOS):
 
-      **Note**: *Mind the leading* ``.`` *which means* **sourcing**
-      ``./env/bin/activate``.
+      .. note::
+         *Mind the leading* ``.`` *which means* **sourcing**
+         ``./env/bin/activate``.
 
       .. code-block:: shell
 
          python3 -m venv --clear env
          . ./env/bin/activate
          pip install -U pip build
 
 Install the ByteBlower RFC 2544 throughput Test Case
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+----------------------------------------------------
 
-First make sure that you *activated* your virtual environment:
+First make sure that you have *activated* your virtual environment:
 
 .. tabs::
 
    .. group-tab:: Windows
 
       On Windows systems using PowerShell:
 
@@ -151,84 +153,97 @@
 Then install (or update) the RFC 2544 throughput test case
 and its dependencies:
 
 .. code-block:: shell
 
    pip install -U byteblower-test-cases-rfc-2544
 
-Quick start
-===========
+The RFC 2544 throughput test case and its dependencies will now be installed
+from `PyPI`_.
 
-Command-line interface
-----------------------
+.. _PyPI: https://pypi.org/project/byteblower-test-cases-rfc-2544/
 
-After providing the appropriate test setup and frame configurations,
-the test script can be run either as Python module or as a command-line script.
+Example test scenario
+=====================
 
-Show help
-^^^^^^^^^
+To run your test using the command-line interface, define your test scenario
+in a file in ``JSON`` format.
 
-To get help for the command-line arguments:
+Use one of these example scenarios to get started.
+Copy it to your working directory as ``rfc_2544.json``:
 
-#. As a Python module:
+- Using `ByteBlower Ports <json/port/rfc_2544.json>`_
+- Using `ByteBlower Endpoint <json/endpoint/rfc_2544.json>`_
 
-   .. code-block:: shell
+.. include:: _include/_example_test_scenario.rst
 
-      # To get help for the command-line arguments:
-      python -m byteblower.test_cases.rfc_2544 --help
+Run a test
+==========
 
-#. As a command-line script:
+The traffic test scenario can be run via command-line interface (either as
+a script or Python module), or integrated in your own Python script.
 
-   .. code-block:: shell
+Command-line interface
+----------------------
 
-      # To get help for the command-line arguments:
-      byteblower-test-cases-rfc-2544-throughput --help
+Run a test with default input/output parameters
 
-Run a test
-^^^^^^^^^^
-
-To run the ByteBlower RFC 2544 throughput test case, you should first provide
-your test configuration, or use this `configuration file example
-<json/rfc_2544.json>`_ (copy it to your working directory),
-after you make sure to update the example configuration to your actual setup
-configuration (ByteBlower server host name or IP, source and destination ports)
+.. tabs::
 
-The reports will be stored under a subdirectory ``reports/``.
+   .. group-tab:: As a command-line script
 
-.. tabs::
+      .. code-block:: shell
 
-   .. group-tab:: Windows
+         byteblower-test-cases-rfc-2544-throughput
 
-      On Windows systems using PowerShell:
+   .. group-tab:: As a Python module
 
       .. code-block:: shell
 
-         # Create reports folder to store HTML/JSON files
-         md reports
-         # Run test
-         byteblower-test-cases-rfc-2544-throughput --report-path reports
+         python -m byteblower.test_cases.rfc_2544
 
-   .. group-tab:: Linux and macOS
+By default:
 
-      On Unix-based systems (Linux, WSL, macOS):
+- The *configuration file* (``rfc_2544.json``) will be loaded
+  from the *current directory*.
+- The resulting reports will also be saved into the *current directory*.
 
-      .. code-block:: shell
+Take a look here for more details on using the :doc:`cli`.
 
-         # Create reports folder to store HTML/JSON files
-         mkdir reports
-         # Run test
-         byteblower-test-cases-rfc-2544-throughput --report-path  reports
+From Python
+-----------
 
-Integrated
-^^^^^^^^^^
+The RFC 2544 throughput test case can also be imported and used in Python
+as follows:
 
 .. code-block:: python
 
    from byteblower.test_cases.rfc_2544 import run
 
+   # Show documentation
+   help(run)
+
    # Defining test configuration, report path and report file name prefix:
-   test_config = {} # Here you should provide your test setup + frame(s') configuration(s)
-   report_path = 'my-output-folder' # Optional: provide the path to the output folder, defaults to the current working directory
-   report_prefix = 'my-dut-feature-test' # Optional: provide prefix of the output files, defaults to 'report'
+
+   # Here you provide your test setup (ByteBlower server, ports, flows, ...),
+   # or load it from a JSON file
+   test_config = {}
+
+   # Optional: provide the path to the output folder, defaults to the current
+   # working directory
+   report_path = 'my-output-folder'
+
+   # Optional: provide prefix of the output files, defaults to 'report'
+   report_prefix = 'my-dut-feature-test'
 
    # Run the RFC 2544 throughput test:
    run(test_config, report_path=report_path, report_prefix=report_prefix)
+
+Define your own test scenario
+=============================
+
+Congratulations! You just ran your first traffic tests.
+
+You want to define your own test scenarios? Great!
+
+Have a look at :doc:`config` for a complete overview of the
+configuration format.
```

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/overview.rst` & `byteblower_test_cases_rfc_2544-1.0.1/docs/source/overview.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-*****************************************
-ByteBlower Test Case: RFC 2544 Throughput
-*****************************************
+********
+Overview
+********
 
 Introduction
 ============
 
 This test case is an implementation of the `RFC 2544`_ Throughput test using
 the `ByteBlower Test Framework`_.
 
@@ -20,15 +20,15 @@
 This ByteBlower RFC 2544 throughput test case allows you to:
 
 #. Run throughput tests based on RFC 2544
 #. Collect & Analyse statistics
 #. Generate HTML & JSON reports
 
 You know about RFC 2544 and you are thrilled to run the test?
-Then you can immediately jump to our :doc:`installation`.
+Then you can immediately jump to our :doc:`quick_start`.
 
 RFC 2544 introduction
 =====================
 
 `RFC 2544`_ specifies a test suite designed to analyze and report on the
 capabilities of network equipment (also referred to as Device Under Test DUT).
 
@@ -124,22 +124,13 @@
    These files include:
 
    * The used setup configuration
    * Test results of each frame size
      (trials results, final real throughput, duration of the test, ...)
    * All error logs
 
-Test configuration
-==================
-
-In the current release, it is possible to supply a configuration file
-in ``JSON`` format for running your tests.
-
-Have a look at ':doc:`config_file`' for a complete overview
-of the file format.
-
 Detailed implementation flow chart
 ==================================
 
 .. figure::  images/rfc2544_overview.png
    :width: 100%
```

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/docs/source/results_highlights.rst` & `byteblower_test_cases_rfc_2544-1.0.1/docs/source/results_highlights.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-******************
-Results highlights
-******************
+*****************
+Result highlights
+*****************
 
 HTML report
 ===========
 
 Summary and configuration
 -------------------------
 
@@ -72,15 +72,15 @@
 
 Ths JSON file consists of 3 main parts in addition to the *"status"* field,
 which indicates if the execution completed correctly.
 
 Configuration
 -------------
 This part contain the ByteBlower server host name and both used endpoints for
-the test (as detailed in :doc:`config_file`)
+the test (as detailed in :doc:`config`)
 
 .. code-block:: json
 
    {
        "configuration": {
            "server": "byteblower-integration-3100-1.lab.byteblower.excentis.com.",
            "source": {
```

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/pyproject.toml` & `byteblower_test_cases_rfc_2544-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,16 @@
     "traffic test",
     "test case",
     "throughput",
     "RFC 2544",
 ]
 classifiers = [
     # See also https://pypi.org/classifiers/
-    "Development Status :: 5 - Production/Stable",
+    # "Development Status :: 4 - Beta",  # For beta releases!
+    "Development Status :: 5 - Production/Stable",  # Only for release!
     "Intended Audience :: Developers",
     "Intended Audience :: Telecommunications Industry",
     #
     # ! XXX - Also keep ``project.license`` in sync!
     #
     'License :: Other/Proprietary License',
     "Operating System :: OS Independent",
```

### Comparing `byteblower_test_cases_rfc_2544-1.0.0b5/PKG-INFO` & `byteblower_test_cases_rfc_2544-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byteblower-test-cases-rfc-2544
-Version: 1.0.0b5
+Version: 1.0.1
 Summary: Perform throughput test based on RFC 2544 using ByteBlower.
 Keywords: ByteBlower,network test,traffic test,test case,throughput,RFC 2544
 Author-email: ByteBlower Development Team <support.byteblower@excentis.com>
 Maintainer-email: Abdennour Rachedi <abdennour.rachedi@excentis.com>, Tom Ghyselinck <tom.ghyselinck@excentis.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -54,29 +54,29 @@
 Provides-Extra: docs-dev
 Provides-Extra: test
 
 *****************************************
 ByteBlower Test Case: RFC 2544 Throughput
 *****************************************
 
+.. footer::
+   Copyright |copy| |year| - Excentis N.V.
+
+.. |copy| unicode:: U+00A9 .. copyright sign
+.. |year| date:: %Y
+
 Introduction
 ============
 
 This package contains an implementation of the `RFC 2544`_ Throughput
 Test using the `ByteBlower Test Framework`_.
 
 .. _RFC 2544: https://www.ietf.org/rfc/rfc2544.txt
 .. _ByteBlower Test Framework: https://pypi.org/project/byteblower-test-framework/.
 
-.. footer::
-   Copyright |copy| |year| - Excentis N.V.
-
-.. |copy| unicode:: U+00A9 .. copyright sign
-.. |year| date:: %Y
-
 A throughput test aims to measure, under given circumstances,
 the highest throughput the DUT can handle correctly without exceeding a given
 threshold of frame loss (theoretically, this threshold is 0).
 
 This ByteBlower RFC 2544 throughput test case allows you to:
 
 #. Run throughput tests based on RFC 2544
@@ -109,16 +109,16 @@
 We recommend managing the runtime environment in a Python virtual
 environment. This guarantees proper separation of the system-wide
 installed Python and pip packages.
 
 Python
 ------
 
-The ByteBlower Test Framework currently supports Python versions 3.7
-up to 3.11.
+The ByteBlower Test Framework currently supports Python versions
+3.7 up to 3.11.
 
 Important: Working directory
 ----------------------------
 
 All the following sections expect that you first moved to your working
 directory where you want to run this project. You may also want to create
 your configuration files under a sub-directory of your choice.
@@ -221,30 +221,42 @@
 For example (*to get help for the command-line arguments*):
 
 #. As a python module:
 
    .. code-block:: shell
 
       # To get help for the command-line arguments:
-      python -m byteblower.test_case.rfc_2544 --help
+      python -m byteblower.test_cases.rfc_2544 --help
 
 #. As a command-line script:
 
    .. code-block:: shell
 
       # To get help for the command-line arguments:
       byteblower-test-cases-rfc-2544-throughput --help
 
-To run the ByteBlower RFC 2544 throughput test case, you should first provide
-your test configuration, or copy this `Configuration file example`_ to
-``rfc_2544.json`` file you create in your working directory. Make sure to
-update the example configuration to your actual setup configuration
-(ByteBlower server host name or IP, source and destination ports)
+For a quick start, you can run a simple test using the JSON configuration of
+one of the example files below:
+
+* Using `ByteBlower Ports scenario <https://api.byteblower.com/test-framework/json/test-cases/rfc-2544/port/rfc_2544.json>`_
+* Using `ByteBlower Endpoint scenario <https://api.byteblower.com/test-framework/json/test-cases/rfc-2544/endpoint/rfc_2544.json>`_
+
+Save you configuration in your working directory as ``rfc_2544.json``.
+Make sure you change the ``"server"`` and ``"ports"`` configuration
+according to the setup you want to run your test on.
 
-The reports will be stored under a subdirectory ``reports/``.
+More detailed documentation is available in the `Configuration file`_ section
+of the documentation.
+
+.. _Configuration file: https://api.byteblower.com/test-framework/latest/test-cases/rfc-2544/config.html
+
+The ``rfc_2544.json`` can be used then to run the test in the
+command line interface using the following commands:
+
+**Note**: *The reports will be stored under a subdirectory* ``reports/``.
 
 #. On Unix-based systems (Linux, WSL, macOS):
 
    .. code-block:: shell
 
       # Optional: create rfc_2544.json, then copy the configuration to it
       touch rfc_2544.json
@@ -265,70 +277,17 @@
       byteblower-test-cases-rfc-2544-throughput --report-path reports
 
 Integrated
 ----------
 
 .. code-block:: python
 
-   from byteblower.test_case.rfc_2544 import run
+   from byteblower.test_cases.rfc_2544 import run
 
    # Defining test configuration, report path and report file name prefix:
    test_config = {} # Here you should provide your test setup + frame(s') configuration(s)
    report_path = 'my-output-folder' # Optional: provide the path to the output folder, defaults to the current working directory
    report_prefix = 'my-dut-feature-test' # Optional: provide prefix of the output files, defaults to 'report'
 
    # Run the RFC 2544 throughput test:
    run(test_config, report_path=report_path, report_prefix=report_prefix)
 
-
-Configuration file example
---------------------------
-
-.. code-block:: json
-
-   {
-       "server": "byteblower-server.com.",
-       "source": {
-           "name": "Source",
-           "interface": "nontrunk-1",
-           "ipv4": "192.168.5.2",
-           "netmask": "255.255.255.0",
-           "gateway": "192.168.5.254"
-       },
-       "destination": {
-           "name": "Destination",
-           "interface": "trunk-1",
-           "ipv4": "dhcp",
-           "nat": true
-       },
-       "duration": 60,
-       "max_iterations": 25,
-       "frame_configs": [
-           {
-               "size": 60,
-               "initial_bitrate": 3e8,
-               "tolerated_frame_loss": 1e-4,
-               "expected_bitrate": 1.7e8,
-               "accuracy": 1e3
-           },
-           {
-               "size": 124,
-               "initial_bitrate": 6e8,
-               "tolerated_frame_loss": 1e-3,
-               "expected_bitrate": 4.5e8,
-               "accuracy": 1e4
-           },
-           {
-               "size": 252,
-               "initial_bitrate": 7e8,
-               "tolerated_frame_loss": 1e-2,
-               "expected_bitrate": 6.5e8,
-               "accuracy": 1e5
-           }
-       ]
-   }
-
-More detailed documentation is available in the `Configuration file`_ section
-of the documentation.
-
-.. _Configuration file: https://api.byteblower.com/test-framework/latest/test-cases/rfc-2544/config_file.html
-
```

