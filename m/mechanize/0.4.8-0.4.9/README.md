# Comparing `tmp/mechanize-0.4.8.tar.gz` & `tmp/mechanize-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mechanize-0.4.8.tar", last modified: Thu Apr 14 14:14:40 2022, max compression
+gzip compressed data, was "mechanize-0.4.9.tar", last modified: Tue Nov  7 09:31:01 2023, max compression
```

## Comparing `mechanize-0.4.8.tar` & `mechanize-0.4.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-04-14 14:14:40.155328 mechanize-0.4.8/
--rw-r--r--   0 kovid     (1000) kovid     (1000)      131 2019-06-03 11:54:11.000000 mechanize-0.4.8/COPYRIGHT
--rw-r--r--   0 kovid     (1000) kovid     (1000)    29355 2022-04-14 14:02:30.000000 mechanize-0.4.8/ChangeLog
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1504 2019-06-03 11:54:11.000000 mechanize-0.4.8/LICENSE
--rw-r--r--   0 kovid     (1000) kovid     (1000)      340 2019-06-03 11:54:11.000000 mechanize-0.4.8/MANIFEST.in
--rw-r--r--   0 kovid     (1000) kovid     (1000)     3915 2022-04-14 14:14:40.155328 mechanize-0.4.8/PKG-INFO
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2259 2020-09-18 01:22:50.000000 mechanize-0.4.8/README.rst
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-04-14 14:14:40.148661 mechanize-0.4.8/examples/
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-04-14 14:14:40.148661 mechanize-0.4.8/examples/forms/
--rw-r--r--   0 kovid     (1000) kovid     (1000)       37 2019-06-03 11:59:16.000000 mechanize-0.4.8/examples/forms/data.dat
--rw-r--r--   0 kovid     (1000) kovid     (1000)       25 2019-06-03 11:59:16.000000 mechanize-0.4.8/examples/forms/data.txt
--rwxr-xr-x   0 kovid     (1000) kovid     (1000)      578 2019-06-03 11:59:16.000000 mechanize-0.4.8/examples/forms/echo.cgi
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1417 2019-06-03 11:59:16.000000 mechanize-0.4.8/examples/forms/example.html
--rwxr-xr-x   0 kovid     (1000) kovid     (1000)     7917 2019-06-03 11:59:16.000000 mechanize-0.4.8/examples/forms/example.py
--rwxr-xr-x   0 kovid     (1000) kovid     (1000)      565 2019-06-03 11:59:16.000000 mechanize-0.4.8/examples/forms/simple.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1725 2019-06-03 11:57:53.000000 mechanize-0.4.8/examples/hack21.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)      928 2019-06-03 11:57:53.000000 mechanize-0.4.8/examples/pypi.py
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-04-14 14:14:40.151994 mechanize-0.4.8/mechanize/
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4808 2021-10-20 04:41:09.000000 mechanize-0.4.8/mechanize/__init__.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2644 2019-06-03 11:57:53.000000 mechanize-0.4.8/mechanize/_auth.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     9611 2021-06-12 02:45:11.000000 mechanize-0.4.8/mechanize/_clientcookie.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)      982 2019-06-03 11:57:53.000000 mechanize-0.4.8/mechanize/_debug.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    38776 2019-09-02 09:36:37.000000 mechanize-0.4.8/mechanize/_entities.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    10886 2019-09-02 09:36:29.000000 mechanize-0.4.8/mechanize/_equiv.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     5070 2019-06-03 11:57:53.000000 mechanize-0.4.8/mechanize/_form.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    91011 2019-06-17 04:14:48.000000 mechanize-0.4.8/mechanize/_form_controls.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     6734 2021-08-01 04:46:45.000000 mechanize-0.4.8/mechanize/_gzip.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     8841 2019-12-22 03:27:48.000000 mechanize-0.4.8/mechanize/_headersutil.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    10872 2019-06-03 11:57:53.000000 mechanize-0.4.8/mechanize/_html.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    10316 2021-12-19 16:31:57.000000 mechanize-0.4.8/mechanize/_http.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    31661 2019-12-22 03:27:48.000000 mechanize-0.4.8/mechanize/_mechanize.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    14731 2019-06-03 11:57:53.000000 mechanize-0.4.8/mechanize/_opener.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     3168 2019-06-03 11:57:53.000000 mechanize-0.4.8/mechanize/_request.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    18544 2019-12-29 02:25:48.000000 mechanize-0.4.8/mechanize/_response.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     7545 2019-06-03 11:57:53.000000 mechanize-0.4.8/mechanize/_rfc3986.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)      182 2019-06-03 11:57:53.000000 mechanize-0.4.8/mechanize/_sockettimeout.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4154 2019-06-03 11:57:53.000000 mechanize-0.4.8/mechanize/_testcase.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2067 2019-06-03 11:57:53.000000 mechanize-0.4.8/mechanize/_urllib2.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    53943 2022-03-31 01:58:18.000000 mechanize-0.4.8/mechanize/_urllib2_fork.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    16572 2021-08-01 04:53:29.000000 mechanize-0.4.8/mechanize/_useragent.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     9088 2019-06-03 11:57:53.000000 mechanize-0.4.8/mechanize/_util.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)       69 2022-04-14 14:02:58.000000 mechanize-0.4.8/mechanize/_version.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     7136 2021-12-19 16:31:00.000000 mechanize-0.4.8/mechanize/polyglot.py
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-04-14 14:14:40.151994 mechanize-0.4.8/mechanize.egg-info/
--rw-r--r--   0 kovid     (1000) kovid     (1000)     3915 2022-04-14 14:14:39.000000 mechanize-0.4.8/mechanize.egg-info/PKG-INFO
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1940 2022-04-14 14:14:40.000000 mechanize-0.4.8/mechanize.egg-info/SOURCES.txt
--rw-r--r--   0 kovid     (1000) kovid     (1000)        1 2022-04-14 14:14:39.000000 mechanize-0.4.8/mechanize.egg-info/dependency_links.txt
--rw-r--r--   0 kovid     (1000) kovid     (1000)      128 2022-04-14 14:14:40.000000 mechanize-0.4.8/mechanize.egg-info/requires.txt
--rw-r--r--   0 kovid     (1000) kovid     (1000)       10 2022-04-14 14:14:40.000000 mechanize-0.4.8/mechanize.egg-info/top_level.txt
--rw-r--r--   0 kovid     (1000) kovid     (1000)        1 2019-12-22 09:18:31.000000 mechanize-0.4.8/mechanize.egg-info/zip-safe
--rwxr-xr-x   0 kovid     (1000) kovid     (1000)     2044 2021-10-20 05:23:45.000000 mechanize-0.4.8/publish.py
--rwxr-xr-x   0 kovid     (1000) kovid     (1000)     1627 2019-06-03 11:54:11.000000 mechanize-0.4.8/run_tests.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1694 2022-04-14 14:14:40.155328 mechanize-0.4.8/setup.cfg
--rwxr-xr-x   0 kovid     (1000) kovid     (1000)      117 2021-10-20 04:32:52.000000 mechanize-0.4.8/setup.py
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-04-14 14:14:40.155328 mechanize-0.4.8/test/
--rw-r--r--   0 kovid     (1000) kovid     (1000)        0 2019-06-03 11:57:52.000000 mechanize-0.4.8/test/__init__.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)      356 2019-06-03 11:57:53.000000 mechanize-0.4.8/test/test_api.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    40557 2019-12-22 03:27:48.000000 mechanize-0.4.8/test/test_browser.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1967 2019-06-03 11:57:53.000000 mechanize-0.4.8/test/test_cookie.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    76464 2019-06-29 01:46:41.000000 mechanize-0.4.8/test/test_cookies.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     3653 2019-06-03 11:57:53.000000 mechanize-0.4.8/test/test_date.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)   125798 2019-06-03 11:57:53.000000 mechanize-0.4.8/test/test_form.py
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-04-14 14:14:40.155328 mechanize-0.4.8/test/test_form_data/
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2828 2019-06-03 11:59:16.000000 mechanize-0.4.8/test/test_form_data/Auth.html
--rw-r--r--   0 kovid     (1000) kovid     (1000)     6101 2019-06-03 11:59:16.000000 mechanize-0.4.8/test/test_form_data/FullSearch.html
--rw-r--r--   0 kovid     (1000) kovid     (1000)     8500 2019-06-03 11:59:16.000000 mechanize-0.4.8/test/test_form_data/GeneralSearch.html
--rw-r--r--   0 kovid     (1000) kovid     (1000)     7769 2019-06-03 11:59:16.000000 mechanize-0.4.8/test/test_form_data/MarkedRecords.html
--rw-r--r--   0 kovid     (1000) kovid     (1000)     9055 2019-06-03 11:59:16.000000 mechanize-0.4.8/test/test_form_data/MarkedResults.html
--rw-r--r--   0 kovid     (1000) kovid     (1000)     7648 2019-06-03 11:59:16.000000 mechanize-0.4.8/test/test_form_data/Results.html
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2017 2019-06-03 11:59:16.000000 mechanize-0.4.8/test/test_form_data/SearchType.html
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1472 2019-12-22 03:27:48.000000 mechanize-0.4.8/test/test_forms.doctest
--rw-r--r--   0 kovid     (1000) kovid     (1000)    25637 2019-06-03 11:57:53.000000 mechanize-0.4.8/test/test_functional.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     5572 2019-06-03 11:57:53.000000 mechanize-0.4.8/test/test_headers.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)      280 2019-06-03 11:57:53.000000 mechanize-0.4.8/test/test_history.doctest
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4397 2019-12-29 02:23:59.000000 mechanize-0.4.8/test/test_html.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)      443 2019-09-02 09:34:38.000000 mechanize-0.4.8/test/test_http.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)      278 2019-06-03 11:57:53.000000 mechanize-0.4.8/test/test_import.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1825 2019-06-03 11:57:53.000000 mechanize-0.4.8/test/test_opener.doctest
--rw-r--r--   0 kovid     (1000) kovid     (1000)    10204 2019-06-03 11:57:53.000000 mechanize-0.4.8/test/test_opener.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4539 2019-06-03 11:57:53.000000 mechanize-0.4.8/test/test_password_manager.special_doctest
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2660 2019-06-03 11:57:53.000000 mechanize-0.4.8/test/test_performance.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1191 2019-06-03 11:57:53.000000 mechanize-0.4.8/test/test_pickle.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2123 2019-06-03 11:57:53.000000 mechanize-0.4.8/test/test_request.doctest
--rw-r--r--   0 kovid     (1000) kovid     (1000)    12166 2019-06-03 11:57:53.000000 mechanize-0.4.8/test/test_response.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     3266 2019-06-03 11:57:53.000000 mechanize-0.4.8/test/test_rfc3986.doctest
--rw-r--r--   0 kovid     (1000) kovid     (1000)    69541 2022-04-14 14:09:18.000000 mechanize-0.4.8/test/test_urllib2.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    19123 2019-06-03 11:57:53.000000 mechanize-0.4.8/test/test_urllib2_localnet.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2831 2019-06-03 11:57:53.000000 mechanize-0.4.8/test/test_useragent.py
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-04-14 14:14:40.155328 mechanize-0.4.8/test-tools/
--rw-r--r--   0 kovid     (1000) kovid     (1000)    13970 2019-06-03 11:57:53.000000 mechanize-0.4.8/test-tools/testprogram.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2668 2019-06-03 11:57:53.000000 mechanize-0.4.8/test-tools/twisted-ftpserver.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     9117 2019-06-03 11:57:53.000000 mechanize-0.4.8/test-tools/twisted-localserver.py
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-11-07 09:31:01.584754 mechanize-0.4.9/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      131 2019-06-03 11:54:11.000000 mechanize-0.4.9/COPYRIGHT
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    29444 2023-11-07 09:28:30.000000 mechanize-0.4.9/ChangeLog
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1504 2019-06-03 11:54:11.000000 mechanize-0.4.9/LICENSE
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      340 2019-06-03 11:54:11.000000 mechanize-0.4.9/MANIFEST.in
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4262 2023-11-07 09:31:01.584754 mechanize-0.4.9/PKG-INFO
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2259 2020-09-18 01:22:50.000000 mechanize-0.4.9/README.rst
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-11-07 09:31:01.574754 mechanize-0.4.9/examples/
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-11-07 09:31:01.574754 mechanize-0.4.9/examples/forms/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       37 2019-06-03 11:59:16.000000 mechanize-0.4.9/examples/forms/data.dat
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       25 2019-06-03 11:59:16.000000 mechanize-0.4.9/examples/forms/data.txt
+-rwxr-xr-x   0 kovid     (1000) kovid     (1000)      578 2019-06-03 11:59:16.000000 mechanize-0.4.9/examples/forms/echo.cgi
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1417 2019-06-03 11:59:16.000000 mechanize-0.4.9/examples/forms/example.html
+-rwxr-xr-x   0 kovid     (1000) kovid     (1000)     7917 2019-06-03 11:59:16.000000 mechanize-0.4.9/examples/forms/example.py
+-rwxr-xr-x   0 kovid     (1000) kovid     (1000)      565 2019-06-03 11:59:16.000000 mechanize-0.4.9/examples/forms/simple.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1725 2019-06-03 11:57:53.000000 mechanize-0.4.9/examples/hack21.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      928 2019-06-03 11:57:53.000000 mechanize-0.4.9/examples/pypi.py
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-11-07 09:31:01.578087 mechanize-0.4.9/mechanize/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4808 2021-10-20 04:41:09.000000 mechanize-0.4.9/mechanize/__init__.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2644 2019-06-03 11:57:53.000000 mechanize-0.4.9/mechanize/_auth.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     9611 2021-06-12 02:45:11.000000 mechanize-0.4.9/mechanize/_clientcookie.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1016 2023-05-16 03:54:51.000000 mechanize-0.4.9/mechanize/_debug.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    38776 2019-09-02 09:36:37.000000 mechanize-0.4.9/mechanize/_entities.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    10886 2019-09-02 09:36:29.000000 mechanize-0.4.9/mechanize/_equiv.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     5070 2019-06-03 11:57:53.000000 mechanize-0.4.9/mechanize/_form.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    91011 2019-06-17 04:14:48.000000 mechanize-0.4.9/mechanize/_form_controls.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     6734 2021-08-01 04:46:45.000000 mechanize-0.4.9/mechanize/_gzip.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     8841 2019-12-22 03:27:48.000000 mechanize-0.4.9/mechanize/_headersutil.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    10872 2019-06-03 11:57:53.000000 mechanize-0.4.9/mechanize/_html.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    10316 2021-12-19 16:31:57.000000 mechanize-0.4.9/mechanize/_http.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    31661 2023-05-16 03:50:00.000000 mechanize-0.4.9/mechanize/_mechanize.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    14731 2019-06-03 11:57:53.000000 mechanize-0.4.9/mechanize/_opener.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     3168 2019-06-03 11:57:53.000000 mechanize-0.4.9/mechanize/_request.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    18659 2023-05-16 03:45:00.000000 mechanize-0.4.9/mechanize/_response.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     7545 2019-06-03 11:57:53.000000 mechanize-0.4.9/mechanize/_rfc3986.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      182 2019-06-03 11:57:53.000000 mechanize-0.4.9/mechanize/_sockettimeout.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4154 2019-06-03 11:57:53.000000 mechanize-0.4.9/mechanize/_testcase.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2067 2019-06-03 11:57:53.000000 mechanize-0.4.9/mechanize/_urllib2.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    54478 2023-10-04 00:37:42.000000 mechanize-0.4.9/mechanize/_urllib2_fork.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    16488 2023-05-16 03:52:37.000000 mechanize-0.4.9/mechanize/_useragent.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     9088 2019-06-03 11:57:53.000000 mechanize-0.4.9/mechanize/_util.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       69 2023-11-07 09:29:05.000000 mechanize-0.4.9/mechanize/_version.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     7136 2021-12-19 16:31:00.000000 mechanize-0.4.9/mechanize/polyglot.py
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-11-07 09:31:01.578087 mechanize-0.4.9/mechanize.egg-info/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4262 2023-11-07 09:31:01.000000 mechanize-0.4.9/mechanize.egg-info/PKG-INFO
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1940 2023-11-07 09:31:01.000000 mechanize-0.4.9/mechanize.egg-info/SOURCES.txt
+-rw-r--r--   0 kovid     (1000) kovid     (1000)        1 2023-11-07 09:31:01.000000 mechanize-0.4.9/mechanize.egg-info/dependency_links.txt
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      128 2023-11-07 09:31:01.000000 mechanize-0.4.9/mechanize.egg-info/requires.txt
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       10 2023-11-07 09:31:01.000000 mechanize-0.4.9/mechanize.egg-info/top_level.txt
+-rw-r--r--   0 kovid     (1000) kovid     (1000)        1 2019-12-22 09:18:31.000000 mechanize-0.4.9/mechanize.egg-info/zip-safe
+-rwxr-xr-x   0 kovid     (1000) kovid     (1000)     2044 2021-10-20 05:23:45.000000 mechanize-0.4.9/publish.py
+-rwxr-xr-x   0 kovid     (1000) kovid     (1000)     1627 2019-06-03 11:54:11.000000 mechanize-0.4.9/run_tests.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1694 2023-11-07 09:31:01.588087 mechanize-0.4.9/setup.cfg
+-rwxr-xr-x   0 kovid     (1000) kovid     (1000)      117 2021-10-20 04:32:52.000000 mechanize-0.4.9/setup.py
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-11-07 09:31:01.581420 mechanize-0.4.9/test/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)        0 2019-06-03 11:57:52.000000 mechanize-0.4.9/test/__init__.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      356 2019-06-03 11:57:53.000000 mechanize-0.4.9/test/test_api.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    40557 2019-12-22 03:27:48.000000 mechanize-0.4.9/test/test_browser.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1967 2019-06-03 11:57:53.000000 mechanize-0.4.9/test/test_cookie.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    76416 2022-05-24 12:39:07.000000 mechanize-0.4.9/test/test_cookies.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     3653 2019-06-03 11:57:53.000000 mechanize-0.4.9/test/test_date.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)   125798 2019-06-03 11:57:53.000000 mechanize-0.4.9/test/test_form.py
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-11-07 09:31:01.584754 mechanize-0.4.9/test/test_form_data/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2828 2019-06-03 11:59:16.000000 mechanize-0.4.9/test/test_form_data/Auth.html
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     6101 2019-06-03 11:59:16.000000 mechanize-0.4.9/test/test_form_data/FullSearch.html
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     8500 2019-06-03 11:59:16.000000 mechanize-0.4.9/test/test_form_data/GeneralSearch.html
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     7769 2019-06-03 11:59:16.000000 mechanize-0.4.9/test/test_form_data/MarkedRecords.html
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     9055 2019-06-03 11:59:16.000000 mechanize-0.4.9/test/test_form_data/MarkedResults.html
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     7648 2019-06-03 11:59:16.000000 mechanize-0.4.9/test/test_form_data/Results.html
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2017 2019-06-03 11:59:16.000000 mechanize-0.4.9/test/test_form_data/SearchType.html
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1472 2019-12-22 03:27:48.000000 mechanize-0.4.9/test/test_forms.doctest
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    25637 2019-06-03 11:57:53.000000 mechanize-0.4.9/test/test_functional.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     5572 2019-06-03 11:57:53.000000 mechanize-0.4.9/test/test_headers.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      280 2019-06-03 11:57:53.000000 mechanize-0.4.9/test/test_history.doctest
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4397 2019-12-29 02:23:59.000000 mechanize-0.4.9/test/test_html.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      443 2019-09-02 09:34:38.000000 mechanize-0.4.9/test/test_http.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      278 2019-06-03 11:57:53.000000 mechanize-0.4.9/test/test_import.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1825 2019-06-03 11:57:53.000000 mechanize-0.4.9/test/test_opener.doctest
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    10204 2019-06-03 11:57:53.000000 mechanize-0.4.9/test/test_opener.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4539 2019-06-03 11:57:53.000000 mechanize-0.4.9/test/test_password_manager.special_doctest
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2660 2019-06-03 11:57:53.000000 mechanize-0.4.9/test/test_performance.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1191 2019-06-03 11:57:53.000000 mechanize-0.4.9/test/test_pickle.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2123 2019-06-03 11:57:53.000000 mechanize-0.4.9/test/test_request.doctest
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    12166 2019-06-03 11:57:53.000000 mechanize-0.4.9/test/test_response.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     3266 2019-06-03 11:57:53.000000 mechanize-0.4.9/test/test_rfc3986.doctest
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    69541 2022-04-14 14:09:18.000000 mechanize-0.4.9/test/test_urllib2.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    19123 2019-06-03 11:57:53.000000 mechanize-0.4.9/test/test_urllib2_localnet.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2831 2019-06-03 11:57:53.000000 mechanize-0.4.9/test/test_useragent.py
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-11-07 09:31:01.584754 mechanize-0.4.9/test-tools/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    13970 2019-06-03 11:57:53.000000 mechanize-0.4.9/test-tools/testprogram.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2668 2019-06-03 11:57:53.000000 mechanize-0.4.9/test-tools/twisted-ftpserver.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     9117 2019-06-03 11:57:53.000000 mechanize-0.4.9/test-tools/twisted-localserver.py
```

### Comparing `mechanize-0.4.8/ChangeLog` & `mechanize-0.4.9/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 This isn't really in proper GNU ChangeLog format, it just happens to
 look that way.
 
+2023-11-07 Kovid Goyal
+	* 0.4.9 release
+	* Fix error on PyPy3
+	* Fix error CPython 3.12
+
 2022-04-14 Kovid Goyal
 	* 0.4.8 release
 	* Handle mal-encoded robots.txt files more gracefully
 	* Support HTTP 308 redirects
 
 2021-09-19 Kovid Goyal
 	* 0.4.7 release
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
 This isn't really in proper GNU ChangeLog format, it just happens to look that
-way. 2022-04-14 Kovid Goyal * 0.4.8 release * Handle mal-encoded robots.txt
-files more gracefully * Support HTTP 308 redirects 2021-09-19 Kovid Goyal *
-0.4.7 release * Fix the ~ character being percent escaped when sending URLs to
-servers. See RFC 3986. 2021-09-01 Kovid Goyal * 0.4.6 release * Python 3.10
-compatibility * Fix a bug in the regex used to parse www-authenticate headers
-that could lead to Denial-of-Service 2019-12-22 Kovid Goyal * 0.4.5 release *
-Add a set_html() method to the browser object 2019-11-07 Kovid Goyal * 0.4.4
-release * URLs passed into mechanize now automatically have URL unsafe
+way. 2023-11-07 Kovid Goyal * 0.4.9 release * Fix error on PyPy3 * Fix error
+CPython 3.12 2022-04-14 Kovid Goyal * 0.4.8 release * Handle mal-encoded
+robots.txt files more gracefully * Support HTTP 308 redirects 2021-09-19 Kovid
+Goyal * 0.4.7 release * Fix the ~ character being percent escaped when sending
+URLs to servers. See RFC 3986. 2021-09-01 Kovid Goyal * 0.4.6 release * Python
+3.10 compatibility * Fix a bug in the regex used to parse www-authenticate
+headers that could lead to Denial-of-Service 2019-12-22 Kovid Goyal * 0.4.5
+release * Add a set_html() method to the browser object 2019-11-07 Kovid Goyal
+* 0.4.4 release * URLs passed into mechanize now automatically have URL unsafe
 characters percent encoded. This is necessary because newer versions of python
 disallow processing of URLs with unsafe characters. Note that this means values
 return by get_full_url(), get_selector() etc will be percent encoded. 2019-08-
 18 Kovid Goyal * 0.4.3 release * When filling forms with unicode strings
 automatically encode them into the correct encoding fr the HTML page being
 viewed * Guess content type when uploading files if not specified * py3 compat
 - Have the version of simple cookies be 0 rather than None 2019-04-12 Kovid
```

### Comparing `mechanize-0.4.8/LICENSE` & `mechanize-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/PKG-INFO` & `mechanize-0.4.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mechanize
-Version: 0.4.8
+Version: 0.4.9
 Summary: Stateful, programmatic web browsing
 Home-page: https://github.com/python-mechanize/mechanize
 Author: Kovid Goyal
 Author-email: no@no.no
 License: BSD
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,18 +28,26 @@
 Classifier: Topic :: System :: Archiving :: Mirroring
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: XML
+License-File: LICENSE
+Requires-Dist: html5lib>=0.999999999
 Provides-Extra: fast
+Requires-Dist: html5-parser>=0.4.4; extra == "fast"
 Provides-Extra: test
+Requires-Dist: twisted; extra == "test"
+Requires-Dist: service_identity; extra == "test"
+Requires-Dist: six; extra == "test"
+Requires-Dist: html5lib; extra == "test"
 Provides-Extra: binarytest
-License-File: LICENSE
+Requires-Dist: lxml; extra == "binarytest"
+Requires-Dist: html5-parser; extra == "binarytest"
 
 mechanize - Automate interaction with HTTP web servers
 ##########################################################
 
 |pypi| |build|
 
 .. contents::
@@ -123,9 +131,7 @@
 .. |pypi| image:: https://img.shields.io/pypi/v/mechanize.svg?label=version
     :target: https://pypi.python.org/pypi/mechanize
     :alt: Latest version released on PyPi
 
 .. |build| image:: https://dev.azure.com/divok/mechanize/_apis/build/status/python-mechanize.mechanize?branchName=master
     :target: https://dev.azure.com/divok/mechanize/_build/latest?definitionId=3&branchName=master
     :alt: Build status of the master branch
-
-
```

### Comparing `mechanize-0.4.8/README.rst` & `mechanize-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/examples/forms/echo.cgi` & `mechanize-0.4.9/examples/forms/echo.cgi`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/examples/forms/example.html` & `mechanize-0.4.9/examples/forms/example.html`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/examples/forms/example.py` & `mechanize-0.4.9/examples/forms/example.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/examples/forms/simple.py` & `mechanize-0.4.9/examples/forms/simple.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/examples/hack21.py` & `mechanize-0.4.9/examples/hack21.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/examples/pypi.py` & `mechanize-0.4.9/examples/pypi.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/__init__.py` & `mechanize-0.4.9/mechanize/__init__.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/_auth.py` & `mechanize-0.4.9/mechanize/_auth.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/_clientcookie.py` & `mechanize-0.4.9/mechanize/_clientcookie.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/_debug.py` & `mechanize-0.4.9/mechanize/_debug.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,7 +26,9 @@
 class HTTPRedirectDebugProcessor(BaseHandler):
 
     def http_request(self, request):
         if hasattr(request, "redirect_dict"):
             info = logging.getLogger("mechanize.http_redirects").info
             info("redirecting to %s", request.get_full_url())
         return request
+
+    https_request = http_request
```

### Comparing `mechanize-0.4.8/mechanize/_entities.py` & `mechanize-0.4.9/mechanize/_entities.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/_equiv.py` & `mechanize-0.4.9/mechanize/_equiv.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/_form.py` & `mechanize-0.4.9/mechanize/_form.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/_form_controls.py` & `mechanize-0.4.9/mechanize/_form_controls.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/_gzip.py` & `mechanize-0.4.9/mechanize/_gzip.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/_headersutil.py` & `mechanize-0.4.9/mechanize/_headersutil.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/_html.py` & `mechanize-0.4.9/mechanize/_html.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/_http.py` & `mechanize-0.4.9/mechanize/_http.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/_mechanize.py` & `mechanize-0.4.9/mechanize/_mechanize.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/_opener.py` & `mechanize-0.4.9/mechanize/_opener.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/_request.py` & `mechanize-0.4.9/mechanize/_request.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/_response.py` & `mechanize-0.4.9/mechanize/_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,14 +285,18 @@
     # than by seek_wrapper's __getattr__ delegation) so that the nasty
     # dynamically-created HTTPError classes in get_seek_wrapper_class() get the
     # wrapped object's implementation, and not HTTPError's.
 
     def info(self):
         return self._headers
 
+    @property
+    def headers(self):
+        return self._headers
+
     def geturl(self):
         return self.wrapped.geturl()
 
     def set_data(self, data):
         self.seek(0)
         self.read()
         self.close()
@@ -330,14 +334,18 @@
 
     def geturl(self):
         return self._url
 
     def info(self):
         return self._headers
 
+    @property
+    def headers(self):
+        return self._headers
+
 
 class closeable_response:
     """Avoids unnecessarily clobbering urllib.addinfourl methods on .close().
 
     Only supports responses returned by mechanize.HTTPHandler.
 
     After .close(), the following methods are supported:
@@ -388,27 +396,28 @@
     def __repr__(self):
         return '<%s at %s whose fp = %r>' % (self.__class__.__name__,
                                              hex(abs(id(self))), self.fp)
 
     def info(self):
         return self._headers
 
+    @property
+    def headers(self):
+        return self._headers
+
     def getcode(self):
         return self.code
 
     def get_header_values(self, name):
-        return self._headers.getheaders(name)
+        return self._headers.get_all(name)
 
     def get_all_header_names(self, normalize=True):
-        ans = []
-        for line in self._headers.headers:
-            h = line.partition(':')[0]
-            if normalize:
-                h = normalize_header_name(h)
-            ans.append(h)
+        ans = self._headers.keys()
+        if normalize:
+            ans = list(map(normalize_header_name, ans))
         return ans
 
     def __getitem__(self, name):
         return self._headers[name]
 
     def get(self, name, default):
         return self._headers.get(name)
```

### Comparing `mechanize-0.4.8/mechanize/_rfc3986.py` & `mechanize-0.4.9/mechanize/_rfc3986.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/_testcase.py` & `mechanize-0.4.9/mechanize/_testcase.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/_urllib2.py` & `mechanize-0.4.9/mechanize/_urllib2.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/_urllib2_fork.py` & `mechanize-0.4.9/mechanize/_urllib2_fork.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,18 +71,24 @@
         data = data.encode('utf-8')
     return hashlib.md5(data).hexdigest()
 
 
 if platform.python_implementation() == 'PyPy':
     def create_readline_wrapper(fh):
         fh.recv = fh.read
-        if not hasattr(fh, '_drop'):
-            fh._drop = lambda: None
-            fh._reuse = lambda: None
-        return socket._fileobject(fh, close=True)
+        if is_py2:
+            if not hasattr(fh, '_drop'):
+                fh._drop = lambda: None
+                fh._reuse = lambda: None
+            ans = socket._fileobject(fh, close=True)
+        else:
+            fh.recv_into = fh.readinto
+            fh._decref_socketios = lambda: None
+            ans = BufferedReader(socket.SocketIO(fh, 'r'))
+        return ans
 else:
     def create_readline_wrapper(fh):
         fh.recv = fh.read
         if is_py2:
             ans = socket._fileobject(fh, close=True)
         else:
             fh.recv_into = fh.readinto
@@ -1268,22 +1274,29 @@
         self.ssl_context = None
 
     def https_open(self, req):
         key_file = cert_file = None
         if self.client_cert_manager is not None:
             key_file, cert_file = self.client_cert_manager.find_key_cert(
                 req.get_full_url())
-        if self.ssl_context is None:
-            conn_factory = partial(
-                HTTPSConnection, key_file=key_file,
-                cert_file=cert_file)
+        if sys.version_info > (3, 5):
+            import ssl
+            ctx = self.ssl_context or ssl.create_default_context()
+            if cert_file:
+                ctx.load_cert_chain(cert_file, key_file)
+            conn_factory = partial(HTTPSConnection, context=ctx)
         else:
-            conn_factory = partial(
-                HTTPSConnection, key_file=key_file,
-                cert_file=cert_file, context=self.ssl_context)
+            if self.ssl_context is None:
+                conn_factory = partial(
+                    HTTPSConnection, key_file=key_file,
+                    cert_file=cert_file)
+            else:
+                conn_factory = partial(
+                    HTTPSConnection, key_file=key_file,
+                    cert_file=cert_file, context=self.ssl_context)
         return self.do_open(conn_factory, req)
 
     https_request = AbstractHTTPHandler.do_request_
 
     def __copy__(self):
         ans = self.__class__(self.client_cert_manager)
         ans._debuglevel = self._debuglevel
```

### Comparing `mechanize-0.4.8/mechanize/_useragent.py` & `mechanize-0.4.9/mechanize/_useragent.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,19 +247,19 @@
         self._client_cert_manager = handler.client_cert_manager = cert_manager
 
     def set_ca_data(self, cafile=None, capath=None, cadata=None, context=None):
         '''
         Set the SSL Context used for connecting to SSL servers.
 
         This method accepts the same arguments as the
-        :py:meth:`ssl.SSLContext.load_verify_locations()` method from the
-        python standard library. You can also pass a pre-built context via the
-        `context` keyword argument. Note that to use this feature, you must be
-        using python >= 2.7.9. In addition you can directly pass in
-        a pre-built :class:`ssl.SSLContext` as the `context` argument.
+        :py:meth:`ssl.SSLContext.load_verify_locations()` method from
+        the Python standard library. You can also pass a pre-built
+        :class:`ssl.SSLContext` via the `context` keyword argument.
+        Note that to use this feature, you must be using Python >=
+        2.7.9.
 
         '''
         import ssl
         if context is None:
             try:
                 context = ssl.create_default_context(
                     cafile=cafile, capath=capath, cadata=cadata)
```

### Comparing `mechanize-0.4.8/mechanize/_util.py` & `mechanize-0.4.9/mechanize/_util.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize/polyglot.py` & `mechanize-0.4.9/mechanize/polyglot.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/mechanize.egg-info/PKG-INFO` & `mechanize-0.4.9/mechanize.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mechanize
-Version: 0.4.8
+Version: 0.4.9
 Summary: Stateful, programmatic web browsing
 Home-page: https://github.com/python-mechanize/mechanize
 Author: Kovid Goyal
 Author-email: no@no.no
 License: BSD
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,18 +28,26 @@
 Classifier: Topic :: System :: Archiving :: Mirroring
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: XML
+License-File: LICENSE
+Requires-Dist: html5lib>=0.999999999
 Provides-Extra: fast
+Requires-Dist: html5-parser>=0.4.4; extra == "fast"
 Provides-Extra: test
+Requires-Dist: twisted; extra == "test"
+Requires-Dist: service_identity; extra == "test"
+Requires-Dist: six; extra == "test"
+Requires-Dist: html5lib; extra == "test"
 Provides-Extra: binarytest
-License-File: LICENSE
+Requires-Dist: lxml; extra == "binarytest"
+Requires-Dist: html5-parser; extra == "binarytest"
 
 mechanize - Automate interaction with HTTP web servers
 ##########################################################
 
 |pypi| |build|
 
 .. contents::
@@ -123,9 +131,7 @@
 .. |pypi| image:: https://img.shields.io/pypi/v/mechanize.svg?label=version
     :target: https://pypi.python.org/pypi/mechanize
     :alt: Latest version released on PyPi
 
 .. |build| image:: https://dev.azure.com/divok/mechanize/_apis/build/status/python-mechanize.mechanize?branchName=master
     :target: https://dev.azure.com/divok/mechanize/_build/latest?definitionId=3&branchName=master
     :alt: Build status of the master branch
-
-
```

### Comparing `mechanize-0.4.8/mechanize.egg-info/SOURCES.txt` & `mechanize-0.4.9/mechanize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/publish.py` & `mechanize-0.4.9/publish.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/run_tests.py` & `mechanize-0.4.9/run_tests.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/setup.cfg` & `mechanize-0.4.9/setup.cfg`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 author = Kovid Goyal
 platforms = any
 author_email = no@no.no
 license = BSD
 description = Stateful, programmatic web browsing
 long_description = file: README.rst
 url = https://github.com/python-mechanize/mechanize
-packages = mechanize
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Operating System :: OS Independent
@@ -33,14 +32,15 @@
 	Topic :: System :: Systems Administration
 	Topic :: Text Processing
 	Topic :: Text Processing :: Markup
 	Topic :: Text Processing :: Markup :: HTML
 	Topic :: Text Processing :: Markup :: XML
 
 [options]
+packages = mechanize
 zip_safe = True
 install_requires = html5lib>=0.999999999
 
 [options.extras_require]
 fast = html5-parser>=0.4.4
 test = 
 	twisted
```

### Comparing `mechanize-0.4.8/test/test_browser.py` & `mechanize-0.4.9/test/test_browser.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_cookie.py` & `mechanize-0.4.9/test/test_cookie.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_cookies.py` & `mechanize-0.4.9/test/test_cookies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1018,26 +1018,20 @@
         versions = [1, 1, 1, 0, 1]
         names = ["bang", "foo", "foo", "spam", "foo"]
         domains = [
             ".sol.no", "blah.spam.org", "www.acme.com", "www.acme.com",
             "www.acme.com"
         ]
         paths = ["/", "/", "/", "/blah", "/blah/"]
-
+        expected = set(zip(versions, names, domains, paths))
         # sequential iteration
-        for i in range(4):
-            i = 0
-            for c in cs:
-                # assert isinstance(c, Cookie)
-                assert c.version == versions[i]
-                assert c.name == names[i]
-                assert c.domain == domains[i]
-                assert c.path == paths[i]
-                i = i + 1
-
+        # python 3.11 iterates in add order, earlier pythons iterate in domain
+        # sorted order
+        actual = {(c.version, c.name, c.domain, c.path) for c in cs}
+        self.assertEqual(expected, actual)
         self.assertRaises(IndexError, lambda cs=cs: cs[5])
 
     def test_parse_ns_headers(self):
         from mechanize._headersutil import parse_ns_headers
 
         # missing domain value (invalid cookie)
         assert parse_ns_headers(
```

### Comparing `mechanize-0.4.8/test/test_date.py` & `mechanize-0.4.9/test/test_date.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_form.py` & `mechanize-0.4.9/test/test_form.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_form_data/Auth.html` & `mechanize-0.4.9/test/test_form_data/Auth.html`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_form_data/FullSearch.html` & `mechanize-0.4.9/test/test_form_data/FullSearch.html`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_form_data/GeneralSearch.html` & `mechanize-0.4.9/test/test_form_data/GeneralSearch.html`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_form_data/MarkedRecords.html` & `mechanize-0.4.9/test/test_form_data/MarkedRecords.html`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_form_data/MarkedResults.html` & `mechanize-0.4.9/test/test_form_data/MarkedResults.html`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_form_data/Results.html` & `mechanize-0.4.9/test/test_form_data/Results.html`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_form_data/SearchType.html` & `mechanize-0.4.9/test/test_form_data/SearchType.html`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_forms.doctest` & `mechanize-0.4.9/test/test_forms.doctest`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_functional.py` & `mechanize-0.4.9/test/test_functional.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_headers.py` & `mechanize-0.4.9/test/test_headers.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_html.py` & `mechanize-0.4.9/test/test_html.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_opener.doctest` & `mechanize-0.4.9/test/test_opener.doctest`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_opener.py` & `mechanize-0.4.9/test/test_opener.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_password_manager.special_doctest` & `mechanize-0.4.9/test/test_password_manager.special_doctest`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_performance.py` & `mechanize-0.4.9/test/test_performance.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_pickle.py` & `mechanize-0.4.9/test/test_pickle.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_request.doctest` & `mechanize-0.4.9/test/test_request.doctest`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_response.py` & `mechanize-0.4.9/test/test_response.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_rfc3986.doctest` & `mechanize-0.4.9/test/test_rfc3986.doctest`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_urllib2.py` & `mechanize-0.4.9/test/test_urllib2.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_urllib2_localnet.py` & `mechanize-0.4.9/test/test_urllib2_localnet.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test/test_useragent.py` & `mechanize-0.4.9/test/test_useragent.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test-tools/testprogram.py` & `mechanize-0.4.9/test-tools/testprogram.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test-tools/twisted-ftpserver.py` & `mechanize-0.4.9/test-tools/twisted-ftpserver.py`

 * *Files identical despite different names*

### Comparing `mechanize-0.4.8/test-tools/twisted-localserver.py` & `mechanize-0.4.9/test-tools/twisted-localserver.py`

 * *Files identical despite different names*

