# Comparing `tmp/cace-2.2.2.tar.gz` & `tmp/cace-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cace-2.2.2.tar", last modified: Wed Apr 24 14:18:40 2024, max compression
+gzip compressed data, was "cace-2.2.3.tar", last modified: Fri Apr 26 06:58:56 2024, max compression
```

## Comparing `cace-2.2.2.tar` & `cace-2.2.3.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.347260 cace-2.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.331260 cace-2.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.335260 cace-2.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-24 14:18:17.000000 cace-2.2.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-24 14:18:17.000000 cace-2.2.2/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-24 14:18:17.000000 cace-2.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-24 14:18:17.000000 cace-2.2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-24 14:18:17.000000 cace-2.2.2/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-24 14:18:17.000000 cace-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-24 14:18:17.000000 cace-2.2.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-24 14:18:40.347260 cace-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-04-24 14:18:17.000000 cace-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.335260 cace-2.2.2/cace/
--rwxr-xr-x   0 runner    (1001) docker     (127)      623 2024-04-24 14:18:17.000000 cace-2.2.2/cace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-24 14:18:17.000000 cace-2.2.2/cace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-24 14:18:17.000000 cace-2.2.2/cace/__version__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5906 2024-04-24 14:18:17.000000 cace-2.2.2/cace/cace_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    45110 2024-04-24 14:18:17.000000 cace-2.2.2/cace/cace_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.339260 cace-2.2.2/cace/common/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19058 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_calculate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23616 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_collate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12819 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26024 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_evaluate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    70978 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_gensim.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14672 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_launch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20756 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_makeplot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12523 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_measure.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10797 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_read.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    46512 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_regenerate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8733 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_simulate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_unused.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    55674 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_write.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7231 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/electrical_parameter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13039 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/layout_estimate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12310 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/netlist_precheck.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2451 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/physical_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/safe_eval.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14650 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/simulation_job.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19262 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/simulation_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8949 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/spiceunits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.343260 cace-2.2.2/cace/gui/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1922 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/consoletext.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29517 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/editparam.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26903 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/failreport.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3780 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/helpwindow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24388 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/rowwidget.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7191 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16180 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/simhints.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4221 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/textreport.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2450 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/tksimpledialog.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/tooltip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.347260 cace-2.2.2/cace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-24 14:18:40.000000 cace-2.2.2/cace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-24 14:18:40.000000 cace-2.2.2/cace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:18:40.000000 cace-2.2.2/cace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 14:18:40.000000 cace-2.2.2/cace.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 14:18:40.000000 cace-2.2.2/cace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 14:18:40.000000 cace-2.2.2/cace.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.343260 cace-2.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 14:18:17.000000 cace-2.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-24 14:18:17.000000 cace-2.2.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.343260 cace-2.2.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.343260 cace-2.2.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   183493 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/_static/cace_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/characterization.md
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.347260 cace-2.2.2/docs/source/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/dev/codebase.md
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/dev/coding_style.md
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/dev/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.347260 cace-2.2.2/docs/source/formats/
--rw-r--r--   0 runner    (1001) docker     (127)    22593 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/formats/format_description.md
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/formats/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/formats/schematic_description.md
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.347260 cace-2.2.2/docs/source/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/usage/cace_cli.md
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/usage/cace_gui.md
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/usage/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/usage/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-24 14:18:17.000000 cace-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 14:18:17.000000 cace-2.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-24 14:18:17.000000 cace-2.2.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-24 14:18:17.000000 cace-2.2.2/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:18:40.347260 cace-2.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.347260 cace-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 14:18:17.000000 cace-2.2.2/tests/context.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 14:18:17.000000 cace-2.2.2/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.038775 cace-2.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.022775 cace-2.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.026775 cace-2.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-26 06:58:35.000000 cace-2.2.3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-26 06:58:35.000000 cace-2.2.3/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-26 06:58:35.000000 cace-2.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-26 06:58:35.000000 cace-2.2.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-26 06:58:35.000000 cace-2.2.3/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-26 06:58:35.000000 cace-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-26 06:58:35.000000 cace-2.2.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-26 06:58:56.038775 cace-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-04-26 06:58:35.000000 cace-2.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.026775 cace-2.2.3/cace/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      623 2024-04-26 06:58:35.000000 cace-2.2.3/cace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-26 06:58:35.000000 cace-2.2.3/cace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-26 06:58:35.000000 cace-2.2.3/cace/__version__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5906 2024-04-26 06:58:35.000000 cace-2.2.3/cace/cace_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44151 2024-04-26 06:58:35.000000 cace-2.2.3/cace/cace_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.034775 cace-2.2.3/cace/common/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19058 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_calculate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23616 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_collate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12819 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26024 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_evaluate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    70978 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_gensim.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14672 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_launch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20756 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_makeplot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12523 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_measure.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10797 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46512 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_regenerate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8733 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_simulate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_unused.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55674 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_write.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7321 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/electrical_parameter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13039 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/layout_estimate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12310 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/netlist_precheck.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2540 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/physical_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/safe_eval.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14709 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/simulation_job.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22242 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/simulation_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8949 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/spiceunits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.034775 cace-2.2.3/cace/gui/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1922 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/consoletext.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29517 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/editparam.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26903 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/failreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3780 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/helpwindow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24388 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/rowwidget.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7191 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16180 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/simhints.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4221 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/textreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2450 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/tksimpledialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/tooltip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.038775 cace-2.2.3/cace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-26 06:58:55.000000 cace-2.2.3/cace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-26 06:58:56.000000 cace-2.2.3/cace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 06:58:55.000000 cace-2.2.3/cace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-26 06:58:55.000000 cace-2.2.3/cace.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 06:58:55.000000 cace-2.2.3/cace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 06:58:55.000000 cace-2.2.3/cace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.034775 cace-2.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-26 06:58:35.000000 cace-2.2.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-26 06:58:35.000000 cace-2.2.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.034775 cace-2.2.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.034775 cace-2.2.3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   183493 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/_static/cace_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/characterization.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.038775 cace-2.2.3/docs/source/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/dev/codebase.md
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/dev/coding_style.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/dev/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.038775 cace-2.2.3/docs/source/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)    22593 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/formats/format_description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/formats/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/formats/schematic_description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.038775 cace-2.2.3/docs/source/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/usage/cace_cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/usage/cace_gui.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/usage/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/usage/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-26 06:58:35.000000 cace-2.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 06:58:35.000000 cace-2.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 06:58:35.000000 cace-2.2.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-26 06:58:35.000000 cace-2.2.3/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 06:58:56.038775 cace-2.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.038775 cace-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-26 06:58:35.000000 cace-2.2.3/tests/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 06:58:35.000000 cace-2.2.3/tests/test1.py
```

### Comparing `cace-2.2.2/.github/workflows/ci.yaml` & `cace-2.2.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/.github/workflows/pypi.yaml` & `cace-2.2.3/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/.readthedocs.yaml` & `cace-2.2.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/Changelog.md` & `cace-2.2.3/Changelog.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,28 @@
-# 2.0.1
+# 2.2.3
+
+## Common
+
+- Improve scheduling of parameters
+  - Simpler and more reliable
+- Queued parameters can now be canceled
+
+## GUI
+
+- While a simulation is running, the netlist source cannot be changed
+
+# 2.2.2
+
+## Common
+
+- Lower setuptools_scm requirement to >=7
+
+# 2.2.0
+
+# 2.2.1
 
 ## GUI
 
 - Don't crash if no datasheet is found
 
 # 2.2.0
```

### Comparing `cace-2.2.2/LICENSE` & `cace-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/Makefile` & `cace-2.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/PKG-INFO` & `cace-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cace
-Version: 2.2.2
+Version: 2.2.3
 Summary: Circuit Automatic Characterization Engine
 Author-email: Tim Edwards <tim@efabless.com>, Leo Moser <leo.moser@efabless.com>
 Project-URL: Homepage, https://github.com/efabless/cace
 Project-URL: Issues, https://github.com/efabless/cace/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cace Version: 2.2.2 Summary: Circuit Automatic
+Metadata-Version: 2.1 Name: cace Version: 2.2.3 Summary: Circuit Automatic
 Characterization Engine Author-email: Tim Edwards
 efabless.com>, Leo Moser
 efabless.com> Project-URL: Homepage, https://github.com/efabless/cace Project-
 URL: Issues, https://github.com/efabless/cace/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

### Comparing `cace-2.2.2/README.md` & `cace-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/__init__.py` & `cace-2.2.3/cace/__init__.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/__main__.py` & `cace-2.2.3/cace/__main__.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/__version__.py` & `cace-2.2.3/cace/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = '2.2.2'
+__version__ = '2.2.3'
 
 if __name__ == '__main__':
     print(__version__, end='')
```

### Comparing `cace-2.2.2/cace/cace_cli.py` & `cace-2.2.3/cace/cace_cli.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/cace_gui.py` & `cace-2.2.3/cace/cace_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,17 @@
         if not self.check_saved():
             warning = 'Warning:  Simulation results have not been saved.'
             confirm = ConfirmDialog(self, warning).result
             if not confirm == 'okay':
                 print('Quit canceled.')
                 return
 
-        # Cancel all queued and running simulations and join
+        # Cancel all queued and running parameters and join them
         print('Stopping all simulations for shutdown.')
-        self.simulation_manager.clear_queued_parameters(cancel_cb=True)
-        self.simulation_manager.cancel_running_parameters(cancel_cb=True)
+        self.simulation_manager.cancel_parameters(cancel_cb=True)
         self.simulation_manager.join_parameters()
 
         if self.logfile:
             self.logfile.close()
 
         self.quit()
 
@@ -194,15 +193,16 @@
             text='Netlist from:',
             style='normal.TLabel',
         )
         self.toppane.title_frame.origin_label.grid(
             column=4, row=0, ipadx=5, padx=10
         )
 
-        self.origin.set('Schematic Capture')
+        self.netlist_text = 'Schematic Capture'
+        self.origin.set(self.netlist_text)
         self.toppane.title_frame.origin_select = ttk.OptionMenu(
             self.toppane.title_frame,
             self.origin,
             'Schematic Capture',
             'Schematic Capture',
             'Layout Extracted',
             'C Extracted',
@@ -416,17 +416,14 @@
 
         self.update_simulate_all_button(from_callback=True)
 
     def simulate_param(self, pname, process=True):
         """Simulate a single parameter"""
 
         self.simulation_manager.set_runtime_options(
-            'netlist_source', self.get_netlist_source()
-        )
-        self.simulation_manager.set_runtime_options(
             'force', self.settings.get_force()
         )
         self.simulation_manager.set_runtime_options(
             'keep', self.settings.get_keep()
         )
         self.simulation_manager.set_runtime_options(
             'sequential', self.settings.get_sequential()
@@ -630,27 +627,20 @@
                 errors += 1
             if ematch or wmatch:
                 print(line)
         return errors
 
     def sim_all(self):
         # Make sure no simulation is running
-        if (
-            self.simulation_manager.num_queued_parameters()
-            + self.simulation_manager.num_running_parameters()
-            > 0
-        ):
+        if self.simulation_manager.num_parameters() > 0:
             print('Simulation in progress must finish first.')
             return
 
         # TODO set at startup and only change directly if necessary
         self.simulation_manager.set_runtime_options(
-            'netlist_source', self.get_netlist_source()
-        )
-        self.simulation_manager.set_runtime_options(
             'force', self.settings.get_force()
         )
         self.simulation_manager.set_runtime_options(
             'keep', self.settings.get_keep()
         )
         self.simulation_manager.set_runtime_options(
             'sequential', self.settings.get_sequential()
@@ -672,50 +662,27 @@
         # Now simulate all parameters
         self.simulation_manager.run_parameters_async()
 
         self.update_simulate_all_button()
 
     def stop_sims(self):
         # Check whether simulations are running
-        if (
-            self.simulation_manager.num_queued_parameters()
-            + self.simulation_manager.num_running_parameters()
-            == 0
-        ):
+        if self.simulation_manager.num_parameters() == 0:
             print('No simulation running.')
         else:
-            # Cancel all queued and running simulations
-            self.simulation_manager.clear_queued_parameters()
-            self.simulation_manager.cancel_running_parameters()
-            # self.simulation_manager.join_parameters() # TODO deadlock because of GUI cb
-
-            if (
-                self.simulation_manager.num_queued_parameters()
-                + self.simulation_manager.num_running_parameters()
-                == 0
-            ):
-                print('All simulations have stopped.')
-            else:
-                print('Not all simulations have stopped yet.')
+            # Cancel all queued and running parameters
+            self.simulation_manager.cancel_parameters()
 
         self.update_simulate_all_button()
 
     def update_simulate_all_button(self, from_callback=False):
         # Check whether no simulations are running, or
         # if the function call comes from a callback,
         # only one simulation is running
-        if (
-            self.simulation_manager.num_queued_parameters()
-            + self.simulation_manager.num_running_parameters()
-            == 0
-            or from_callback
-            and self.simulation_manager.num_queued_parameters()
-            + self.simulation_manager.num_running_parameters()
-            == 1
-        ):
+        if self.simulation_manager.num_parameters() == 0:
             self.allsimbutton.configure(
                 style='bluetitle.TButton',
                 text='Simulate All',
                 command=self.sim_all,
             )
         else:
             # Button now stops the simulations
@@ -753,30 +720,14 @@
 
     def add_hints(self, param, simbutton):
         # Raise hints window and configure appropriately for the parameter.
         # Fill in any existing hints.
         self.simhints.populate(param, simbutton)
         self.simhints.open()
 
-    # Get the value for runtime options['netlist_source']
-    def get_netlist_source(self):
-        netlist_text = self.origin.get()
-        if netlist_text == 'Schematic Capture':
-            return 'schematic'
-        elif netlist_text == 'Layout Extracted':
-            return 'layout'
-        elif netlist_text == 'C Extracted':
-            return 'pex'
-        elif netlist_text == 'R-C Extracted':
-            return 'rcx'
-        else:
-            print('Unhandled netlist source ' + netlist_text)
-            print('Reverting to schematic.')
-            return 'schematic'
-
     def clear_results(self, dsheet):
         # TODO do in SimulationManager
 
         # Remove results from the window by clearing parameter results
         paramstodo = []
         if 'electrical_parameters' in dsheet:
             paramstodo.extend(dsheet['electrical_parameters'])
@@ -965,14 +916,44 @@
 
             self.create_datasheet_view()
 
     def generate_html(self):
         self.simulation_manager.generate_html()
 
     def swap_results(self, value={}):
+        """Triggered when a new netlist source is selected"""
+
+        # Make sure no parameters are currently scheduled
+        if self.simulation_manager.num_parameters() > 0:
+            print('Cannot change the netlist source: Parameters are running.')
+            self.origin.set(self.netlist_text)
+            return
+
+        netlist_source = None
+
+        # Get the netlist source from the text
+        self.netlist_text = self.origin.get()
+        if self.netlist_text == 'Schematic Capture':
+            netlist_source = 'schematic'
+        elif self.netlist_text == 'Layout Extracted':
+            netlist_source = 'layout'
+        elif self.netlist_text == 'C Extracted':
+            netlist_source = 'pex'
+        elif self.netlist_text == 'R-C Extracted':
+            netlist_source = 'rcx'
+        else:
+            print(f'Unhandled netlist source {netlist_text}')
+            print('Reverting to schematic.')
+            netlist_source = 'schematic'
+
+        # Update netlist source
+        self.simulation_manager.set_runtime_options(
+            'netlist_source', netlist_source
+        )
+
         # This routine just calls self.create_datasheet_view(), but the
         # button callback has an argument that needs to be handled even
         # if it is just discarded.
         self.create_datasheet_view()
 
     def load_results(self, value={}):
 
@@ -1006,14 +987,15 @@
         if not os.path.exists(dsdir):
             # Try 'spice' as a subdirectory of the datasheet directory as a
             # fallback.
             dsdir = dspath + '/spice'
             if not os.path.exists(dsdir):
                 print('Error:  Cannot find directory spice/ in path ' + dspath)
 
+        # TODO rework
         if self.origin.get() == 'Layout Extracted':
             spifile = dsdir + '/layout/' + dsroot + '.spice'
         if self.origin.get() == 'C Extracted':
             spifile = dsdir + '/pex/' + dsroot + '.spice'
         elif self.origin.get() == 'R-C Extracted':
             spifile = dsdir + '/rcx/' + dsroot + '.spice'
         else:
@@ -1072,19 +1054,14 @@
         for widget in dframe.winfo_children():
             widget.destroy()
 
         self.parameter_widgets = {}
 
         dsheet = self.simulation_manager.get_datasheet()
 
-        # Update netlist source
-        self.simulation_manager.set_runtime_options(
-            'netlist_source', self.get_netlist_source()
-        )
-
         # Add basic information at the top
 
         n = 0
         dframe.cframe = ttk.Frame(dframe)
         dframe.cframe.grid(column=0, row=n, sticky='ewns', columnspan=10)
 
         dframe.cframe.plabel = ttk.Label(
@@ -1136,19 +1113,15 @@
         dframe.max_title.grid(column=6, row=n, sticky='ewns', columnspan=2)
         dframe.stat_title = ttk.Label(
             dframe, text='Status', style='title.TLabel'
         )
         dframe.stat_title.grid(column=8, row=n, sticky='ewns')
 
         # Check whether simulations are running
-        if (
-            self.simulation_manager.num_queued_parameters()
-            + self.simulation_manager.num_running_parameters()
-            > 0
-        ):
+        if self.simulation_manager.num_parameters() > 0:
             self.allsimbutton = ttk.Button(
                 dframe,
                 text='Stop Simulations',
                 style='redtitle.TButton',
                 command=self.stop_sims,
             )
         else:
@@ -1201,15 +1174,15 @@
             n,
             self.simulation_manager,
         )
 
         # Set functions
         self.parameter_widgets[pname].set_functions(
             self.simulate_param,
-            self.simulation_manager.cancel_running_parameter,
+            self.simulation_manager.cancel_parameter,
             self.edit_param,
             self.copy_param,
             self.delete_param,
             self.failreport.display,
             self.textreport.display,
         )
```

### Comparing `cace-2.2.2/cace/common/cace_calculate.py` & `cace-2.2.3/cace/common/cace_calculate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/common/cace_collate.py` & `cace-2.2.3/cace/common/cace_collate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/common/cace_compat.py` & `cace-2.2.3/cace/common/cace_compat.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/common/cace_evaluate.py` & `cace-2.2.3/cace/common/cace_evaluate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/common/cace_gensim.py` & `cace-2.2.3/cace/common/cace_gensim.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/common/cace_launch.py` & `cace-2.2.3/cace/common/cace_launch.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/common/cace_makeplot.py` & `cace-2.2.3/cace/common/cace_makeplot.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/common/cace_measure.py` & `cace-2.2.3/cace/common/cace_measure.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/common/cace_read.py` & `cace-2.2.3/cace/common/cace_read.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/common/cace_regenerate.py` & `cace-2.2.3/cace/common/cace_regenerate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/common/cace_simulate.py` & `cace-2.2.3/cace/common/cace_simulate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/common/cace_unused.txt` & `cace-2.2.3/cace/common/cace_unused.txt`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/common/cace_write.py` & `cace-2.2.3/cace/common/cace_write.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/common/electrical_parameter.py` & `cace-2.2.3/cace/common/electrical_parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,17 @@
         self.cb_sims = cb_sims
         self.pdk = pdk
         self.paths = paths
         self.runtime_options = runtime_options
 
         self.queued_jobs = []
         self.new_testbenches = []
+
         self.canceled = False
+        self.done = False
 
         super().__init__(*args, **kwargs)
 
     def cancel(self, cancel_cb):
         print(f'Cancel electrical parameter: {self.param["name"]}')
         self.canceled = True
 
@@ -130,14 +132,17 @@
 
         # Assign the new testbenches to the parameter
         # (cancel is not possible anymore)
         self.param['testbenches'] = self.new_testbenches
 
         self.postprocess()
 
+        # Set done before calling cb
+        self.done = True
+
         if self.cb:
             self.cb(self.param['name'])
 
         print(f'{self.param["name"]}: Completed')
 
     def add_simulation_job(self, job):
         self.queued_jobs.append(job)
```

### Comparing `cace-2.2.2/cace/common/layout_estimate.py` & `cace-2.2.3/cace/common/layout_estimate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/common/netlist_precheck.py` & `cace-2.2.3/cace/common/netlist_precheck.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/common/physical_parameter.py` & `cace-2.2.3/cace/common/physical_parameter.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         self.cb = cb
         self.cb_sims = cb_sims
         self.pdk = pdk
         self.paths = paths
         self.runtime_options = runtime_options
 
         self.canceled = False
+        self.done = False
 
         super().__init__(*args, **kwargs)
 
     def run(self):
 
         self.cancel_point()
 
@@ -67,14 +68,17 @@
             return 1
 
         self.cancel_point()
 
         print(f'{self.param["name"]}: Evaluating physical parameter')
         cace_evaluate(self.datasheet, self.param)
 
+        # Set done before calling cb
+        self.done = True
+
         if self.cb:
             self.cb(self.param['name'])
 
     def cancel(self, cancel_cb):
         print(f'{self.param["name"]}: Cancel physical parameter')
         self.canceled = True
```

### Comparing `cace-2.2.2/cace/common/safe_eval.py` & `cace-2.2.3/cace/common/safe_eval.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/common/simulation_job.py` & `cace-2.2.3/cace/common/simulation_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,43 +29,49 @@
     ):
         self.param = param
         self.testbenchlist = testbenchlist
         self.pdk = pdk
         self.paths = paths
         self.runtime_options = runtime_options
 
-        self.sim_complete_callback = None
+        self.cb = None
 
         self.canceled = False
         self.spiceproc = None
 
         super().__init__(*args, **kwargs)
 
     def cancel(self, cancel_cb):
-        print(f'{self.param["name"]}: Cancel simulation: {self.testbenchlist}')
+        # print(f'{self.param["name"]}: Cancel simulation: {self.testbenchlist}')
         self.canceled = True
 
         if cancel_cb:
-            self.sim_complete_callback = None
+            self.cb = None
 
         if self.spiceproc:
             self.spiceproc.kill()
 
+    def cancel_point(self):
+        """If canceled, call the cb and exit the thread"""
+
+        if self.canceled:
+            if self.cb:
+                self.cb(self.param['name'], self.testbenchlist, True)
+            sys.exit()
+
     def run(self):
         paramname = self.param['name']
         simresult = 0
 
-        if self.canceled:
-            return None
+        self.cancel_point()
 
         for testbench in self.testbenchlist:
             simresult += self.simulate(testbench)
 
-            if self.canceled:
-                return None
+            self.cancel_point()
 
         debug = (
             self.runtime_options['debug']
             if 'debug' in self.runtime_options
             else False
         )
 
@@ -307,24 +313,19 @@
                         print('Copying ngspice configuration file from PDK.')
                         shutil.copy(spinitfile, '.spiceinit')
 
             # Capture all output from stdout and stderr.  Print each line in
             # real-time, and flush the output buffer.  All output is ignored.
             # Note:  bufsize = 1 and universal_newlines = True sets line-buffered output
 
-            print(
-                'Running: '
-                + simulator
-                + ' '
-                + ' '.join(simargs)
-                + ' '
-                + filename
-            )
+            print(f'Running: {simulator} {" ".join(simargs)} {filename}')
             print('Current working directory is: ' + os.getcwd())
 
+            self.cancel_point()
+
             self.spiceproc = subprocess.Popen(
                 [simulator, *simargs, filename],
                 stdin=None,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.STDOUT,
                 bufsize=1,
                 text=True,
```

### Comparing `cace-2.2.2/cace/common/simulation_manager.py` & `cace-2.2.3/cace/common/simulation_manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 import re
 import sys
 import time
 import shutil
 import signal
 import threading
 
-from queue import Queue
-
 from .cace_read import cace_read
 from .cace_compat import cace_compat
 from .cace_write import cace_write, cace_summary, cace_generate_html
 from .physical_parameter import PhysicalParameter
 from .electrical_parameter import ElectricalParameter
 
 
@@ -36,18 +34,22 @@
     It also holds the datasheet and provides functions to
     manipulate it.
     """
 
     def __init__(self, datasheet={}):
         """Initialize the object with a datasheet"""
         self.datasheet = datasheet
-        self.threads = []
-        self.queue = Queue()
-        self.thread = None
-        self.threads = []
+
+        self.worker_thread = None
+
+        self.queued_threads = []
+        self.queued_lock = threading.Lock()
+
+        self.running_threads = []
+        self.running_lock = threading.Lock()
 
         self.default_options = {
             'netlist_source': 'schematic',
             'force': False,
             'keep': False,
             'nosim': False,
             'json': False,
@@ -283,15 +285,15 @@
             self.datasheet['paths'][key] = key
 
         return self.datasheet['paths'][key]
 
     def validate_runtime_options(self):
         """Make sure the runtime options contain valid values"""
 
-        valid_sources = ['schematic', 'layout', 'pex', 'rcx']
+        valid_sources = ['schematic', 'layout', 'pex', 'rcx', 'best']
 
         if (
             not self.datasheet['runtime_options']['netlist_source']
             in valid_sources
         ):
             print(
                 f'Error: Invalid netlist source: {self.datasheet["runtime_options"]["netlist_source"]}'
@@ -392,15 +394,17 @@
                     new_sim_param = ElectricalParameter(
                         param, self.datasheet, pdk, paths, runtime_options, cb
                     )
 
                     print(
                         f'Inserting electrical parameter {param["name"]} into queue'
                     )
-                    self.queue.put(new_sim_param)
+
+                    with self.queued_lock:
+                        self.queued_threads.insert(0, new_sim_param)
 
                     # TODO return number of simulations for this parameter
                     #      needed for progress bars etc.
                     return 1
 
         if 'physical_parameters' in self.datasheet:
             for param in self.datasheet['physical_parameters']:
@@ -422,15 +426,17 @@
                     new_sim_param = PhysicalParameter(
                         param, self.datasheet, pdk, paths, runtime_options, cb
                     )
 
                     print(
                         f'Inserting physical parameter {param["name"]} into queue'
                     )
-                    self.queue.put(new_sim_param)
+
+                    with self.queued_lock:
+                        self.queued_threads.insert(0, new_sim_param)
 
                     # TODO return number of simulations for this parameter
                     #      needed for progress bars etc.
                     return 1
 
         print(f'Unknown parameter {pname}')
         if 'electrical_parameters' in self.datasheet:
@@ -440,106 +446,183 @@
         if 'physical_parameters' in self.datasheet:
             print('Known physical parameters are:')
             for pparam in self.datasheet['physical_parameters']:
                 print(pparam['name'])
 
         return None
 
+    def prune_running_threads(self):
+        """Remove threads that are either marked as done or have been canceled"""
+
+        needs_unlock = False
+        if not self.running_lock.locked():
+            self.running_lock.lock()
+            needs_unlock = True
+
+        # Remove completed threads
+        self.running_threads = [
+            t
+            for t in self.running_threads
+            if t.is_alive() or (not t.done and not t.canceled)
+        ]
+
+        if needs_unlock:
+            self.running_lock.unlock()
+
+    def num_parameters(self):
+        """Get the number of queued or running parameters"""
+
+        return self.num_queued_parameters() + self.num_running_parameters()
+
     def num_queued_parameters(self):
         """Get the number of queued parameters"""
 
-        return self.queue.qsize()
+        return len(self.queued_threads)
 
     def num_running_parameters(self):
         """Get the number of running parameters"""
 
-        # Remove completed threads
-        self.threads = [t for t in self.threads if t.is_alive()]
+        with self.running_lock:
+            self.prune_running_threads()
+
+            # Count the parameter threads that are not yet done
+            num_running = sum(
+                1
+                for t in self.running_threads
+                if not t.done and not t.canceled
+            )
 
-        return len(self.threads)
+        return num_running
 
     def run_parameters_async(self):
-        """Start a thread to start parameter threads"""
+        """Start a worker thread to start parameter threads"""
 
-        # Wait until previous run completed
-        if self.thread:
-            self.thread.join()
-        self.thread = None
-
-        # Start new thread to start parameter threads
-        self.thread = threading.Thread(target=self.run_parameters_thread)
-        self.thread.start()
+        # Only start a new worker thread, if
+        # the previous one hasn't completed yet
+        if not self.worker_thread or not self.worker_thread.is_alive():
+            # Start new worker thread to start parameter threads
+            self.worker_thread = threading.Thread(
+                target=self.run_parameters_thread
+            )
+            self.worker_thread.start()
 
     def run_parameters_thread(self):
-        """A thread starts the thread of queued parameters"""
+        """Called as a thread, starts the threads of queued parameters"""
+
+        while self.queued_threads:
 
-        while not self.queue.empty():
             # Check whether we can start another parameter in parallel
             if (
                 self.num_running_parameters()
                 < self.datasheet['runtime_options']['parallel_parameters']
             ):
+                param_thread = None
 
-                sim_param = self.queue.get()
-                print(f'Running parameter {sim_param.param["name"]}')
-                # sim_param.setDaemon(True) # TODO correct?
-                sim_param.start()
+                # Holding both locks, move a parameter
+                # from queued to running
+                with self.running_lock:
+                    with self.queued_lock:
+                        # Could have been cancelled meanhwile
+                        if self.queued_threads:
+                            param_thread = self.queued_threads.pop()
+                            self.running_threads.append(param_thread)
+
+                if param_thread and not param_thread.canceled:
+                    print(f'Running parameter {param_thread.param["name"]}')
+                    param_thread.start()
 
-                self.threads.append(sim_param)
             # Else wait until another parameter has completed
             else:
                 time.sleep(0.1)
 
     def join_parameters(self):
         """Join all running parameter threads"""
 
-        # Wait until previous run completed
-        if self.thread:
-            self.thread.join()
-        self.thread = None
-
-        # Wait until thread is complete
-        for thread in self.threads:
-            thread.join()
+        # Wait until all parameters are running
+        if self.worker_thread:
+            self.worker_thread.join()
+        self.worker_thread = None
+
+        # Wait until all parameters are complete
+        with self.running_lock:
+            for param_thread in self.running_threads:
+                param_thread.join()
 
-        # Remove completed threads
-        self.threads = [t for t in self.threads if t.is_alive()]
+            # Remove completed threads
+            self.prune_running_threads()
 
     def run_parameters(self):
         """Run parameters sequentially, note that simulations can still be parallelized"""
 
-        while not self.queue.empty():
-            sim_param = self.queue.get()
-            sim_param.run()
+        with self.queued_lock:
+            while self.queued_threads:
+                param_thread = self.queued_threads.pop()
+                param_thread.run()
+
+    def cancel_parameters(self, cancel_cb=False):
+        """Cancel all parameters"""
+
+        self.cancel_queued_parameters(cancel_cb)
+        self.cancel_running_parameters(cancel_cb)
+
+    def cancel_queued_parameters(self, cancel_cb=False):
+        """Cancel all queued parameters"""
+
+        with self.queued_lock:
+            while self.queued_threads:
+                param_thread = self.queued_threads.pop()
+
+                # Cancel the thread and start it
+                # so that it directly calls its callback
+                param_thread.cancel(cancel_cb)
+                param_thread.start()
+
+    def cancel_running_parameters(self, cancel_cb=False):
+        """Cancel all running parameters"""
 
-    def clear_queued_parameters(self, cancel_cb=False):
-        """Clear all queued parameters"""
+        with self.running_lock:
 
-        while not self.queue.empty():
-            sim_param = self.queue.get()
+            # Remove completed threads
+            self.prune_running_threads()
 
-            if not cancel_cb and sim_param.cb:
-                sim_param.cb(sim_param.param['name'])
+            for param_thread in self.running_threads:
+                param_thread.cancel(cancel_cb)
 
-    def cancel_running_parameters(self, cancel_cb=False):
-        """Cancel all running parameters"""
+    def cancel_parameter(self, pname, cancel_cb=False):
+        """Cancel a single parameter"""
 
-        # Remove completed threads
-        self.threads = [t for t in self.threads if t.is_alive()]
+        self.cancel_queued_parameter(pname, cancel_cb)
+        self.cancel_running_parameter(pname, cancel_cb)
 
-        for thread in self.threads:
-            thread.cancel(cancel_cb)
+    def cancel_queued_parameter(self, pname, cancel_cb=False):
+        """Cancel a single running parameter"""
+
+        with self.queued_lock:
+
+            # Get all threads that should be canceled
+            # Maybe there are multiple threads with the same name
+            cancel_threads = [
+                t for t in self.queued_threads if t.param['name'] == pname
+            ]
+
+            for param_thread in cancel_threads:
+
+                # Remove the thread from the queued list
+                self.queued_threads.remove(param_thread)
+
+                # Cancel the thread and start it
+                # so that it directly calls its callback
+                param_thread.cancel(cancel_cb)
+                param_thread.start()
 
     def cancel_running_parameter(self, pname, cancel_cb=False):
         """Cancel a single running parameter"""
 
-        # Remove completed threads
-        self.threads = [t for t in self.threads if t.is_alive()]
+        with self.running_lock:
 
-        found = False
-        for thread in self.threads:
-            if thread.param['name'] == pname:
-                found = True
-                thread.cancel(cancel_cb)
+            # Remove completed threads
+            self.prune_running_threads()
 
-        if not found:
-            print(f'Error: Could not cancel parameter: {pname} not found')
+            for param_thread in self.running_threads:
+                # TODO also check source
+                if param_thread.param['name'] == pname:
+                    param_thread.cancel(cancel_cb)
```

### Comparing `cace-2.2.2/cace/common/spiceunits.py` & `cace-2.2.3/cace/common/spiceunits.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/gui/consoletext.py` & `cace-2.2.3/cace/gui/consoletext.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/gui/editparam.py` & `cace-2.2.3/cace/gui/editparam.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/gui/failreport.py` & `cace-2.2.3/cace/gui/failreport.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/gui/helpwindow.py` & `cace-2.2.3/cace/gui/helpwindow.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/gui/rowwidget.py` & `cace-2.2.3/cace/gui/rowwidget.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/gui/settings.py` & `cace-2.2.3/cace/gui/settings.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/gui/simhints.py` & `cace-2.2.3/cace/gui/simhints.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/gui/style.py` & `cace-2.2.3/cace/gui/style.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/gui/textreport.py` & `cace-2.2.3/cace/gui/textreport.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/gui/tksimpledialog.py` & `cace-2.2.3/cace/gui/tksimpledialog.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace/gui/tooltip.py` & `cace-2.2.3/cace/gui/tooltip.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/cace.egg-info/PKG-INFO` & `cace-2.2.3/cace.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cace
-Version: 2.2.2
+Version: 2.2.3
 Summary: Circuit Automatic Characterization Engine
 Author-email: Tim Edwards <tim@efabless.com>, Leo Moser <leo.moser@efabless.com>
 Project-URL: Homepage, https://github.com/efabless/cace
 Project-URL: Issues, https://github.com/efabless/cace/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cace Version: 2.2.2 Summary: Circuit Automatic
+Metadata-Version: 2.1 Name: cace Version: 2.2.3 Summary: Circuit Automatic
 Characterization Engine Author-email: Tim Edwards
 efabless.com>, Leo Moser
 efabless.com> Project-URL: Homepage, https://github.com/efabless/cace Project-
 URL: Issues, https://github.com/efabless/cace/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

### Comparing `cace-2.2.2/cace.egg-info/SOURCES.txt` & `cace-2.2.3/cace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/docs/Makefile` & `cace-2.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/docs/make.bat` & `cace-2.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/docs/source/_static/cace_screenshot.png` & `cace-2.2.3/docs/source/_static/cace_screenshot.png`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/docs/source/characterization.md` & `cace-2.2.3/docs/source/characterization.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/docs/source/conf.py` & `cace-2.2.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/docs/source/formats/format_description.md` & `cace-2.2.3/docs/source/formats/format_description.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/docs/source/formats/schematic_description.md` & `cace-2.2.3/docs/source/formats/schematic_description.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/docs/source/index.md` & `cace-2.2.3/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/docs/source/usage/cace_cli.md` & `cace-2.2.3/docs/source/usage/cace_cli.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/docs/source/usage/cace_gui.md` & `cace-2.2.3/docs/source/usage/cace_gui.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/docs/source/usage/getting_started.md` & `cace-2.2.3/docs/source/usage/getting_started.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.2/pyproject.toml` & `cace-2.2.3/pyproject.toml`

 * *Files identical despite different names*

