# Comparing `tmp/seamm_util-2024.4.22.tar.gz` & `tmp/seamm_util-2024.4.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seamm_util-2024.4.22.tar", last modified: Mon Apr 22 20:04:08 2024, max compression
+gzip compressed data, was "seamm_util-2024.4.26.tar", last modified: Fri Apr 26 15:00:39 2024, max compression
```

## Comparing `seamm_util-2024.4.22.tar` & `seamm_util-2024.4.26.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:04:08.055110 seamm_util-2024.4.22/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-22 20:04:08.055110 seamm_util-2024.4.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:04:08.043110 seamm_util-2024.4.22/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     8689 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/requirements_install.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:04:08.055110 seamm_util-2024.4.22/seamm_util/
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/seamm_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-22 20:04:08.055110 seamm_util-2024.4.22/seamm_util/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    24250 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/seamm_util/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/seamm_util/check_executable.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/seamm_util/compact_json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/seamm_util/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)    63121 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/seamm_util/elemental_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/seamm_util/include_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/seamm_util/md_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/seamm_util/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/seamm_util/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    30207 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/seamm_util/printing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/seamm_util/seamm_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/seamm_util/seamm_json.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/seamm_util/seamm_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/seamm_util/units.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/seamm_util/variable_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/seamm_util/water_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    20803 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/seamm_util/zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:04:08.055110 seamm_util-2024.4.22/seamm_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-22 20:04:08.000000 seamm_util-2024.4.22/seamm_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-22 20:04:08.000000 seamm_util-2024.4.22/seamm_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 20:04:08.000000 seamm_util-2024.4.22/seamm_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 20:04:08.000000 seamm_util-2024.4.22/seamm_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 20:04:08.000000 seamm_util-2024.4.22/seamm_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-22 20:04:08.055110 seamm_util-2024.4.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:04:08.047110 seamm_util-2024.4.22/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:04:08.051110 seamm_util-2024.4.22/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/blank_lines.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/blank_lines.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/blank_lines.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/empty_file.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/empty_file.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/empty_file.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/file1.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/file1.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/file1.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/file_#include.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/file_#include.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/file_#include.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/file_end.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/file_end.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/file_end.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/file_include1.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/file_include1.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/file_include1.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/file_middle.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/file_middle.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/file_middle.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/include_blank_lines.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/include_blank_lines.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/include_blank_lines.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/include_empty_file.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/include_empty_file.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/data/include_empty_file.txt.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:04:08.051110 seamm_util-2024.4.22/tests/results/
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/results/simple_plot.html
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/results/two_plots.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:04:08.055110 seamm_util-2024.4.22/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/templates/line.html_template
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/test_open_bzip2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/test_open_gzipped.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/test_plotting_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-04-22 20:03:47.000000 seamm_util-2024.4.22/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:00:39.625866 seamm_util-2024.4.26/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-26 15:00:39.625866 seamm_util-2024.4.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:00:39.613865 seamm_util-2024.4.26/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8689 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/requirements_install.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:00:39.625866 seamm_util-2024.4.26/seamm_util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/seamm_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-26 15:00:39.625866 seamm_util-2024.4.26/seamm_util/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24040 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/seamm_util/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/seamm_util/check_executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/seamm_util/compact_json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/seamm_util/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63121 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/seamm_util/elemental_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/seamm_util/include_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/seamm_util/md_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/seamm_util/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/seamm_util/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30207 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/seamm_util/printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/seamm_util/seamm_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/seamm_util/seamm_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/seamm_util/seamm_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/seamm_util/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/seamm_util/variable_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/seamm_util/water_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20803 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/seamm_util/zenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:00:39.625866 seamm_util-2024.4.26/seamm_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-26 15:00:39.000000 seamm_util-2024.4.26/seamm_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-26 15:00:39.000000 seamm_util-2024.4.26/seamm_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:00:39.000000 seamm_util-2024.4.26/seamm_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 15:00:39.000000 seamm_util-2024.4.26/seamm_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 15:00:39.000000 seamm_util-2024.4.26/seamm_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-26 15:00:39.625866 seamm_util-2024.4.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:00:39.617866 seamm_util-2024.4.26/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:00:39.621866 seamm_util-2024.4.26/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/blank_lines.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/blank_lines.txt.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/blank_lines.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/empty_file.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/empty_file.txt.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/empty_file.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/file1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/file1.txt.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/file1.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/file_#include.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/file_#include.txt.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/file_#include.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/file_end.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/file_end.txt.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/file_end.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/file_include1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/file_include1.txt.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/file_include1.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/file_middle.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/file_middle.txt.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/file_middle.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/include_blank_lines.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/include_blank_lines.txt.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/include_blank_lines.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/include_empty_file.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/include_empty_file.txt.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/data/include_empty_file.txt.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:00:39.621866 seamm_util-2024.4.26/tests/results/
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/results/simple_plot.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/results/two_plots.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:00:39.621866 seamm_util-2024.4.26/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/templates/line.html_template
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/test_open_bzip2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/test_open_gzipped.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/test_plotting_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-04-26 15:00:32.000000 seamm_util-2024.4.26/versioneer.py
```

### Comparing `seamm_util-2024.4.22/CONTRIBUTING.rst` & `seamm_util-2024.4.26/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/HISTORY.rst` & `seamm_util-2024.4.26/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 =======
 History
 =======
+2024.4.26 -- Removed debug printing
+    * Some debug printing was accidentally left in the code.
+      
 2024.4.22 -- Moving user preferences to ~/.seamm.d
     * To better support Docker, moving ~/.seammrc to ~/.seamm.d/seamrc
     * Moved seamm.ini from ~/SEAMM to ~/seamm.d since it only contains personal preferences.
 
 2023.11.12 -- Internal update
     * Versioneer needed to be updated to account for changes in configparser.
```

### Comparing `seamm_util-2024.4.22/LICENSE` & `seamm_util-2024.4.26/LICENSE`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/PKG-INFO` & `seamm_util-2024.4.26/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm_util
-Version: 2024.4.22
+Version: 2024.4.26
 Summary: seamm_util
 Home-page: https://github.com/molssi-seamm/seamm_util
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: seamm_util
 Platform: Linux
@@ -81,14 +81,17 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2024.4.26 -- Removed debug printing
+    * Some debug printing was accidentally left in the code.
+      
 2024.4.22 -- Moving user preferences to ~/.seamm.d
     * To better support Docker, moving ~/.seammrc to ~/.seamm.d/seamrc
     * Moved seamm.ini from ~/SEAMM to ~/seamm.d since it only contains personal preferences.
 
 2023.11.12 -- Internal update
     * Versioneer needed to be updated to account for changes in configparser.
```

### Comparing `seamm_util-2024.4.22/README.rst` & `seamm_util-2024.4.26/README.rst`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/docs/Makefile` & `seamm_util-2024.4.26/docs/Makefile`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/docs/conf.py` & `seamm_util-2024.4.26/docs/conf.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/docs/index.rst` & `seamm_util-2024.4.26/docs/index.rst`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/docs/installation.rst` & `seamm_util-2024.4.26/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/docs/make.bat` & `seamm_util-2024.4.26/docs/make.bat`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/seamm_util/__init__.py` & `seamm_util-2024.4.26/seamm_util/__init__.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/seamm_util/argument_parser.py` & `seamm_util-2024.4.26/seamm_util/argument_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,23 +169,16 @@
 
         # 2. Read the .ini files, if any.
 
         # Moving from ~/SEAMM/seamm.ini to ~/.seamm.d/seamm.ini
         # Make directory and move if it does not exist
         path = Path("~/.seamm.d/seamm.ini").expanduser()
         tmp = Path("~/SEAMM/seamm.ini").expanduser()
-        print(f"{path=}")
-        print(f"{path.exists()=}")
-        print(f" {tmp=}")
-        print(f"{tmp.exists()=}")
         if not path.parent.exists():
             path.parent.mkdir(parents=True)
-            print("made directory")
-        else:
-            print("directory existed")
 
         if tmp.exists() and not path.exists():
             print("/ntext:")
             print(tmp.read_text())
             print()
             path.write_text(tmp.read_text())
             tmp.unlink()
```

### Comparing `seamm_util-2024.4.22/seamm_util/check_executable.py` & `seamm_util-2024.4.26/seamm_util/check_executable.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/seamm_util/compact_json_encoder.py` & `seamm_util-2024.4.26/seamm_util/compact_json_encoder.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/seamm_util/dictionary.py` & `seamm_util-2024.4.26/seamm_util/dictionary.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/seamm_util/elemental_data.py` & `seamm_util-2024.4.26/seamm_util/elemental_data.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/seamm_util/include_open.py` & `seamm_util-2024.4.26/seamm_util/include_open.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/seamm_util/md_statistics.py` & `seamm_util-2024.4.26/seamm_util/md_statistics.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/seamm_util/output.py` & `seamm_util-2024.4.26/seamm_util/output.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/seamm_util/plotting.py` & `seamm_util-2024.4.26/seamm_util/plotting.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/seamm_util/printing.py` & `seamm_util-2024.4.26/seamm_util/printing.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/seamm_util/seamm_file.py` & `seamm_util-2024.4.26/seamm_util/seamm_file.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/seamm_util/seamm_json.py` & `seamm_util-2024.4.26/seamm_util/seamm_json.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/seamm_util/units.py` & `seamm_util-2024.4.26/seamm_util/units.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/seamm_util/variable_names.py` & `seamm_util-2024.4.26/seamm_util/variable_names.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/seamm_util/water_models.py` & `seamm_util-2024.4.26/seamm_util/water_models.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/seamm_util/zenodo.py` & `seamm_util-2024.4.26/seamm_util/zenodo.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/seamm_util.egg-info/PKG-INFO` & `seamm_util-2024.4.26/seamm_util.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm_util
-Version: 2024.4.22
+Version: 2024.4.26
 Summary: seamm_util
 Home-page: https://github.com/molssi-seamm/seamm_util
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: seamm_util
 Platform: Linux
@@ -81,14 +81,17 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2024.4.26 -- Removed debug printing
+    * Some debug printing was accidentally left in the code.
+      
 2024.4.22 -- Moving user preferences to ~/.seamm.d
     * To better support Docker, moving ~/.seammrc to ~/.seamm.d/seamrc
     * Moved seamm.ini from ~/SEAMM to ~/seamm.d since it only contains personal preferences.
 
 2023.11.12 -- Internal update
     * Versioneer needed to be updated to account for changes in configparser.
```

### Comparing `seamm_util-2024.4.22/seamm_util.egg-info/SOURCES.txt` & `seamm_util-2024.4.26/seamm_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/setup.py` & `seamm_util-2024.4.26/setup.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/tests/results/simple_plot.html` & `seamm_util-2024.4.26/tests/results/simple_plot.html`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/tests/results/two_plots.html` & `seamm_util-2024.4.26/tests/results/two_plots.html`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/tests/templates/line.html_template` & `seamm_util-2024.4.26/tests/templates/line.html_template`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/tests/test_dictionary.py` & `seamm_util-2024.4.26/tests/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/tests/test_open.py` & `seamm_util-2024.4.26/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/tests/test_open_bzip2.py` & `seamm_util-2024.4.26/tests/test_open_bzip2.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/tests/test_open_gzipped.py` & `seamm_util-2024.4.26/tests/test_open_gzipped.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/tests/test_plotting.py` & `seamm_util-2024.4.26/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/tests/test_plotting_figure.py` & `seamm_util-2024.4.26/tests/test_plotting_figure.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/tests/test_units.py` & `seamm_util-2024.4.26/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2024.4.22/versioneer.py` & `seamm_util-2024.4.26/versioneer.py`

 * *Files identical despite different names*

