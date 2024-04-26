# Comparing `tmp/tvb-widgets-1.6.0.tar.gz` & `tmp/tvb-widgets-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-widgets-1.6.0.tar", last modified: Tue Sep 19 09:08:30 2023, max compression
+gzip compressed data, was "tvb-widgets-2.0.0.tar", last modified: Fri Apr 26 11:54:53 2024, max compression
```

## Comparing `tvb-widgets-1.6.0.tar` & `tvb-widgets-2.0.0.tar`

### file list

```diff
@@ -1,88 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:30.383947 tvb-widgets-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35796 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2023-09-19 09:08:30.383947 tvb-widgets-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-19 09:08:30.383947 tvb-widgets-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:30.375948 tvb-widgets-1.6.0/tvb_widgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2023-09-19 09:08:30.000000 tvb-widgets-1.6.0/tvb_widgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2023-09-19 09:08:30.000000 tvb-widgets-1.6.0/tvb_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-19 09:08:30.000000 tvb-widgets-1.6.0/tvb_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      281 2023-09-19 09:08:30.000000 tvb-widgets-1.6.0/tvb_widgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-19 09:08:30.000000 tvb-widgets-1.6.0/tvb_widgets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:30.375948 tvb-widgets-1.6.0/tvbwidgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:30.375948 tvb-widgets-1.6.0/tvbwidgets/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/core/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:30.375948 tvb-widgets-1.6.0/tvbwidgets/core/hpc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/core/hpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/core/hpc/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11563 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/core/hpc/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/core/ini_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:30.375948 tvb-widgets-1.6.0/tvbwidgets/core/logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/core/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/core/logger/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/core/logger/logging.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:30.375948 tvb-widgets-1.6.0/tvbwidgets/core/pse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/core/pse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13775 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/core/pse/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/core/pse/pse_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/core/pse/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/core/pse/toml_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:30.375948 tvb-widgets-1.6.0/tvbwidgets/core/simulator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/core/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/core/simulator/model_exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/core/simulator/tvb_integrators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:30.379948 tvb-widgets-1.6.0/tvbwidgets/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/tests/test_drive_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/tests/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/tests/test_head_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/tests/test_phase_plane_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/tests/test_pse_stage_in.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/tests/test_tvb_integrators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:30.379948 tvb-widgets-1.6.0/tvbwidgets/tests/ts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/tests/ts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/tests/ts/test_data_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/tests/ts/test_mne_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/tests/ts/test_plotly_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/tests/ts/ts_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:30.379948 tvb-widgets-1.6.0/tvbwidgets/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/base_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:30.379948 tvb-widgets-1.6.0/tvbwidgets/ui/connectivity_ipy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/connectivity_ipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/connectivity_ipy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9851 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/connectivity_ipy/connectivity_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/connectivity_ipy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/connectivity_ipy/global_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    13464 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/connectivity_ipy/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/connectivity_ipy/outputs_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:30.379948 tvb-widgets-1.6.0/tvbwidgets/ui/connectivity_react/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/connectivity_react/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/connectivity_react/connectivity_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/connectivity_react/connectivity_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/drive_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    12507 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/head_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    36585 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/phase_plane_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    12785 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/pse_launcher_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/pse_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/storage_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:30.383947 tvb-widgets-1.6.0/tvbwidgets/ui/ts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/ts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/ts/base_ts_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:30.383947 tvb-widgets-1.6.0/tvbwidgets/ui/ts/data_wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/ts/data_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/ts/data_wrappers/base_data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/ts/data_wrappers/numpy_data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/ts/data_wrappers/tvb_data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    14483 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/ts/mne_ts_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    13241 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/ts/plotly_ts_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/ts/ts_widget_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2023-09-19 09:08:24.000000 tvb-widgets-1.6.0/tvbwidgets/ui/widget_with_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:53.561913 tvb-widgets-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35796 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-26 11:54:53.561913 tvb-widgets-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 11:54:53.561913 tvb-widgets-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:53.549913 tvb-widgets-2.0.0/tvb_widgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-26 11:54:53.000000 tvb-widgets-2.0.0/tvb_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-26 11:54:53.000000 tvb-widgets-2.0.0/tvb_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:54:53.000000 tvb-widgets-2.0.0/tvb_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-26 11:54:53.000000 tvb-widgets-2.0.0/tvb_widgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 11:54:53.000000 tvb-widgets-2.0.0/tvb_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:53.553913 tvb-widgets-2.0.0/tvbwidgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:53.553913 tvb-widgets-2.0.0/tvbwidgets/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/core/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:53.553913 tvb-widgets-2.0.0/tvbwidgets/core/hpc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/core/hpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/core/hpc/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11605 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/core/hpc/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/core/ini_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:53.553913 tvb-widgets-2.0.0/tvbwidgets/core/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/core/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/core/logger/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/core/logger/logging.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:53.553913 tvb-widgets-2.0.0/tvbwidgets/core/pse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/core/pse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13775 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/core/pse/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/core/pse/pse_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/core/pse/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/core/pse/toml_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:53.553913 tvb-widgets-2.0.0/tvbwidgets/core/simulator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/core/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/core/simulator/model_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/core/simulator/tvb_integrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/readers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:53.553913 tvb-widgets-2.0.0/tvbwidgets/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/tests/test_drive_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/tests/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/tests/test_head_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/tests/test_phase_plane_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/tests/test_pse_stage_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/tests/test_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/tests/test_tvb_integrators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:53.557913 tvb-widgets-2.0.0/tvbwidgets/tests/ts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/tests/ts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/tests/ts/test_data_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/tests/ts/test_mne_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/tests/ts/test_plotly_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/tests/ts/ts_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:53.557913 tvb-widgets-2.0.0/tvbwidgets/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/base_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:53.557913 tvb-widgets-2.0.0/tvbwidgets/ui/connectivity_ipy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/connectivity_ipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/connectivity_ipy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/connectivity_ipy/connectivity_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/connectivity_ipy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/connectivity_ipy/global_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13468 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/connectivity_ipy/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/connectivity_ipy/outputs_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:53.557913 tvb-widgets-2.0.0/tvbwidgets/ui/connectivity_react/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/connectivity_react/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/connectivity_react/connectivity_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/connectivity_react/connectivity_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/dicom_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/drive_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12813 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/head_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36757 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/phase_plane_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/pse_launcher_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/pse_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/storage_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:53.557913 tvb-widgets-2.0.0/tvbwidgets/ui/ts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/ts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/ts/base_ts_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:53.561913 tvb-widgets-2.0.0/tvbwidgets/ui/ts/data_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/ts/data_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/ts/data_wrappers/base_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/ts/data_wrappers/numpy_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/ts/data_wrappers/tvb_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/ts/mne_ts_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/ts/plotly_ts_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/ts/ts_widget_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-26 11:54:48.000000 tvb-widgets-2.0.0/tvbwidgets/ui/widget_with_browser.py
```

### Comparing `tvb-widgets-1.6.0/LICENSE` & `tvb-widgets-2.0.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 "TheVirtualBrain - Widgets" is a package with GUI components for EBRAINS
 
-(c) 2022-2023, TVB Widgets Team
+(c) 2022-2024, TVB Widgets Team
 
 This program is free software: you can redistribute it and/or modify it under the terms
 of the GNU General Public License as published by the Free Software Foundation, either
 version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
```

### Comparing `tvb-widgets-1.6.0/PKG-INFO` & `tvb-widgets-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-widgets
-Version: 1.6.0
+Version: 2.0.0
 Summary: GUI widgets for EBRAINS showcases
 Home-page: https://github.com/the-virtual-brain/tvb-widgets
 Author: TVB Widgets Team (Juelich SDL Neuroscience, INS - Marseille, Codemart)
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb widgets jupyterlab ebrains showcases
 Platform: UNKNOWN
@@ -61,9 +61,11 @@
 To retrieve the token string, execute in https://lab.ch.ebrains.eu/:
 
     clb_oauth.get_token()
 
 #  Acknowledgments
 This project has received funding from the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 945539 (Human Brain Project SGA3).
 
+This project has received funding from the European Union’s Horizon Europe Programme under the Specific Grant Agreement No. 101147319 (EBRAINS 2.0 Project).
+
```

### Comparing `tvb-widgets-1.6.0/README.md` & `tvb-widgets-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -46,7 +46,9 @@
 To retrieve the token string, execute in https://lab.ch.ebrains.eu/:
 
     clb_oauth.get_token()
 
 #  Acknowledgments
 This project has received funding from the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 945539 (Human Brain Project SGA3).
 
+This project has received funding from the European Union’s Horizon Europe Programme under the Specific Grant Agreement No. 101147319 (EBRAINS 2.0 Project).
+
```

### Comparing `tvb-widgets-1.6.0/setup.py` & `tvb-widgets-2.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import json
 import setuptools
 import shutil
 import pkg_resources
 from pathlib import Path
```

### Comparing `tvb-widgets-1.6.0/tvb_widgets.egg-info/PKG-INFO` & `tvb-widgets-2.0.0/tvb_widgets.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-widgets
-Version: 1.6.0
+Version: 2.0.0
 Summary: GUI widgets for EBRAINS showcases
 Home-page: https://github.com/the-virtual-brain/tvb-widgets
 Author: TVB Widgets Team (Juelich SDL Neuroscience, INS - Marseille, Codemart)
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb widgets jupyterlab ebrains showcases
 Platform: UNKNOWN
@@ -61,9 +61,11 @@
 To retrieve the token string, execute in https://lab.ch.ebrains.eu/:
 
     clb_oauth.get_token()
 
 #  Acknowledgments
 This project has received funding from the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 945539 (Human Brain Project SGA3).
 
+This project has received funding from the European Union’s Horizon Europe Programme under the Specific Grant Agreement No. 101147319 (EBRAINS 2.0 Project).
+
```

### Comparing `tvb-widgets-1.6.0/tvb_widgets.egg-info/SOURCES.txt` & `tvb-widgets-2.0.0/tvb_widgets.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 tvb_widgets.egg-info/PKG-INFO
 tvb_widgets.egg-info/SOURCES.txt
 tvb_widgets.egg-info/dependency_links.txt
 tvb_widgets.egg-info/requires.txt
 tvb_widgets.egg-info/top_level.txt
 tvbwidgets/__init__.py
 tvbwidgets/api.py
+tvbwidgets/readers.py
 tvbwidgets/core/__init__.py
 tvbwidgets/core/auth.py
 tvbwidgets/core/exceptions.py
 tvbwidgets/core/ini_parser.py
 tvbwidgets/core/hpc/__init__.py
 tvbwidgets/core/hpc/config.py
 tvbwidgets/core/hpc/launcher.py
@@ -31,22 +32,24 @@
 tvbwidgets/tests/constants.py
 tvbwidgets/tests/test_base.py
 tvbwidgets/tests/test_drive_widget.py
 tvbwidgets/tests/test_exporters.py
 tvbwidgets/tests/test_head_widget.py
 tvbwidgets/tests/test_phase_plane_export.py
 tvbwidgets/tests/test_pse_stage_in.py
+tvbwidgets/tests/test_readers.py
 tvbwidgets/tests/test_tvb_integrators.py
 tvbwidgets/tests/ts/__init__.py
 tvbwidgets/tests/ts/test_data_wrappers.py
 tvbwidgets/tests/ts/test_mne_widget.py
 tvbwidgets/tests/ts/test_plotly_widget.py
 tvbwidgets/tests/ts/ts_generator.py
 tvbwidgets/ui/__init__.py
 tvbwidgets/ui/base_widget.py
+tvbwidgets/ui/dicom_widget.py
 tvbwidgets/ui/drive_widget.py
 tvbwidgets/ui/head_widget.py
 tvbwidgets/ui/phase_plane_widget.py
 tvbwidgets/ui/pse_launcher_widget.py
 tvbwidgets/ui/pse_widget.py
 tvbwidgets/ui/storage_widget.py
 tvbwidgets/ui/widget_with_browser.py
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/__init__.py` & `tvb-widgets-2.0.0/tvbwidgets/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import json
 from pathlib import Path
 from pkg_resources import get_distribution, DistributionNotFound
 from .core.logger.builder import get_logger
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/api.py` & `tvb-widgets-2.0.0/tvbwidgets/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 from .ui.connectivity_ipy.connectivity_widget import ConnectivityWidget
+from .ui.connectivity_react.connectivity_widget import ConnectivityWidgetReact
+from .ui.dicom_widget import DicomWidget
 from .ui.phase_plane_widget import PhasePlaneWidget
 from .ui.storage_widget import StorageWidget
 from .ui.head_widget import HeadBrowser, HeadWidget, HeadWidgetConfig
 from .ui.ts.mne_ts_widget import TimeSeriesWidgetMNE
 from .ui.ts.plotly_ts_widget import TimeSeriesWidgetPlotly
 from .ui.ts.ts_widget_browser import TimeSeriesBrowser
 from .ui.pse_widget import PSEWidget
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/core/auth.py` & `tvb-widgets-2.0.0/tvbwidgets/core/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import os
 from .logger.builder import get_logger
 
 CLB_AUTH = 'CLB_AUTH'
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/core/exceptions.py` & `tvb-widgets-2.0.0/tvbwidgets/core/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 class WidgetsException(Exception):
 
     def __init__(self, message):
         super().__init__(message)
         self.message = str(message)
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/core/hpc/config.py` & `tvb-widgets-2.0.0/tvbwidgets/core/hpc/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 from dataclasses import dataclass
 from pyunicore.helpers.jobs import Resources
 
 
 @dataclass
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/core/hpc/launcher.py` & `tvb-widgets-2.0.0/tvbwidgets/core/hpc/launcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import time
 import pyunicore.client
 from pathlib import Path
 from typing import Callable
 from datetime import datetime
 from urllib.error import HTTPError
-from pyunicore.helpers.jobs import Status, Description
-from pyunicore.credentials import AuthenticationFailedException
+from pyunicore.helpers.jobs import Description
+from pyunicore.client import JobStatus
+from pyunicore.credentials import AuthenticationFailedException, OIDCToken
 from pkg_resources import get_distribution, DistributionNotFound
 from tvbwidgets.core.auth import get_current_token
 from tvbwidgets.core.hpc.config import HPCConfig
 from tvbwidgets.core.logger.builder import get_logger
 from tvbwidgets.core.pse.parameters import PROGRESS_STATUS
 from tvb.simulator.simulator import Simulator
 from tvbwidgets.core.pse.storage import StoreObj
@@ -68,15 +69,15 @@
         # type: (Simulator) -> Path
         return TOMLStorage.write_pse_in_file(StoreObj(sim, self.param1, self.param2, self.param1_values,
                                                       self.param2_values, self.metrics, self.config.n_threads,
                                                       self.file_name))
 
     def connect_client(self):
         LOGGER.info(f"Connecting to {self.config.site}...")
-        token = get_current_token()
+        token = OIDCToken(get_current_token())
         transport = pyunicore.client.Transport(token)
         registry = pyunicore.client.Registry(transport, pyunicore.client._HBP_REGISTRY_URL)
 
         try:
             sites = registry.site_urls
         except Exception:
             LOGGER.error("Unicore seems to be down at the moment. "
@@ -178,15 +179,15 @@
                 self.JOB_TYPE_KEY: self.INTERACTIVE_KEY}
             job_env_prep = client.new_job(job_description, inputs=[])
             LOGGER.info(f"Job is running at {self.config.site}: {job_env_prep.working_dir.properties['mountPoint']}. "
                         f"Submission time is: {self._format_date_for_job(job_env_prep)}. "
                         f"Waiting for job to finish..."
                         f'It can also be monitored with the "PyUnicore tasks stream" tool on the right-side bar.')
             job_env_prep.poll()
-            if job_env_prep.properties['status'] == Status.FAILED:
+            if job_env_prep.properties['status'] == JobStatus.FAILED:
                 LOGGER.error("Encountered an error during environment setup, stopping execution.")
                 return
             LOGGER.info("Successfully finished the environment setup.")
 
         command = f"{self._module_load_command} && {self._activate_command} && " \
                   f"python -m {executable} {path_input}"
         LOGGER.info(f"Launching workflow for command: \n {command}")
@@ -220,24 +221,24 @@
 
     def monitor_job(self, job):
         LOGGER.info('Waiting for job to finish...'
                     'It can also be monitored interactively with the "PyUnicore Tasks Stream" tool.')
 
         start_time = int(time.time())
         # we replaced job.poll to our custom while, to update the progress bar as well
-        while job.status.ordinal() < pyunicore.client.JobStatus.SUCCESSFUL.ordinal():
+        while job.status.ordinal() < JobStatus.SUCCESSFUL.ordinal():
             completed_count = int(self.read_file_from_hpc(job, PROGRESS_STATUS))
             self.update_progress(completed_count)
             time.sleep(2)
             if self.config.timeout > 0 and int(time.time()) > start_time + self.config.timeout:
                 # signalize a problem in the front-end
                 self.update_progress(error_msg="Connection Timeout")
                 raise TimeoutError(f"Timeout waiting for job to complete. Already completed {completed_count}")
 
-        if job.properties['status'] == Status.FAILED:
+        if job.properties['status'] == JobStatus.FAILED:
             LOGGER.error("Job finished with errors.")
             return
         LOGGER.info("Job finished with success. Staging out the results...")
         self.stage_out_results(job)
         LOGGER.info("Finished execution.")
 
     def stage_out_results(self, job):
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/core/ini_parser.py` & `tvb-widgets-2.0.0/tvbwidgets/core/ini_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import configparser
 from collections import OrderedDict
 
 
 def parse_ini_file(ini_file):
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/core/logger/builder.py` & `tvb-widgets-2.0.0/tvbwidgets/core/logger/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import os
 import inspect
 import weakref
 import logging
 import logging.config
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/core/logger/logging.conf` & `tvb-widgets-2.0.0/tvbwidgets/core/logger/logging.conf`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.6.0/tvbwidgets/core/pse/parameters.py` & `tvb-widgets-2.0.0/tvbwidgets/core/pse/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 """
 A collection of parameter related classes and functions.
 - Temporary copy from tvb-inversion package
 
 .. moduleauthor: Fousek Jan <jan.fousek@univ-amu.fr>
 .. moduleauthor: Teodora Misan <teodora.misan@codemart.ro>
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/core/pse/pse_data.py` & `tvb-widgets-2.0.0/tvbwidgets/core/pse/pse_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 from tvb.basic.neotraits.api import NArray, HasTraits, Attr
 from tvb.core.neotraits.h5 import H5File, DataSet, Scalar, Json
 
 
 class PSEData(HasTraits):
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/core/pse/toml_storage.py` & `tvb-widgets-2.0.0/tvbwidgets/core/pse/toml_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import toml
 import importlib
 import numpy as np
 from pathlib import Path
 from datetime import datetime
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/core/simulator/model_exporters.py` & `tvb-widgets-2.0.0/tvbwidgets/core/simulator/model_exporters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import abc
 import json
 import numpy
 import os
 import re
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/core/simulator/tvb_integrators.py` & `tvb-widgets-2.0.0/tvbwidgets/core/simulator/tvb_integrators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import inspect
 from enum import Enum
 from tvb.simulator import integrators
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/tests/test_base.py` & `tvb-widgets-2.0.0/tvbwidgets/tests/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import os
 import pytest
 import tvbwidgets.api as api
 from tvbwidgets.core.auth import get_current_token, CLB_AUTH
 from tvbwidgets.ui.base_widget import TVBWidget
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/tests/test_drive_widget.py` & `tvb-widgets-2.0.0/tvbwidgets/tests/test_drive_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import os
 
 import pytest
 from ebrains_drive.files import SeafFile, SeafDir
 from ebrains_drive.repo import Repo
@@ -100,15 +100,15 @@
     # this triggers the observe events on select widget
     widget.files_list.value = widget.files_list.options[2]
     assert widget._parent_dir.path == '/'
     assert widget.get_selected_file_path() is None
     assert len(widget.files_list.options) == 1
 
     with pytest.raises(AttributeError):
-        assert widget.get_selected_file_content()
+        widget.get_selected_file_content()
 
 
 def test_storage_widget(mocker):
     def mockk(token):
         return MockDriveClient()
 
     mocker.patch('ebrains_drive.connect', mockk)
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/tests/test_exporters.py` & `tvb-widgets-2.0.0/tvbwidgets/tests/test_exporters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import json
 import os
 import numpy
 import pytest
 import shutil
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/tests/test_head_widget.py` & `tvb-widgets-2.0.0/tvbwidgets/tests/test_head_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import logging
 import os
 import numpy
 import pytest
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/tests/test_phase_plane_export.py` & `tvb-widgets-2.0.0/tvbwidgets/tests/test_phase_plane_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 import json
 import os
 
 import numpy
 import pytest
 import shutil
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/tests/test_pse_stage_in.py` & `tvb-widgets-2.0.0/tvbwidgets/tests/test_pse_stage_in.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import os
 import pytest
 import numpy as np
 from tvb.datatypes import connectivity
 from tvb.simulator.coupling import Kuramoto
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/tests/ts/test_data_wrappers.py` & `tvb-widgets-2.0.0/tvbwidgets/tests/ts/test_data_wrappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
+import math
 import numpy as np
 import pytest
 
 from tvbwidgets.tests.ts.ts_generator import generate_ts_with_mode_and_sv
 from tvbwidgets.ui.ts.data_wrappers.numpy_data_wrapper import WrapperNumpy
 from tvbwidgets.ui.ts.data_wrappers.tvb_data_wrapper import WrapperTVB
 
 
 # =========================================== TEST WRAPPER NUMPY =======================================================
 @pytest.fixture
 def wrapper_np():
     """ Returns an initialized Numpy wrapper with 3 dimensions """
-    numpy_array = np.random.rand(30000, 4, 50)
+    rng = np.random.default_rng(50)
+    numpy_array = rng.random(size=(30000, 4, 50))
     wrapper_np = WrapperNumpy(numpy_array, 0.01, ch_idx=2)
     return wrapper_np
 
 
 def test_data_shape_np(wrapper_np):
     assert wrapper_np.data_shape == (30000, 4, 50)
 
@@ -33,15 +35,15 @@
 
 
 def test_get_ts_period_np(wrapper_np):
     assert wrapper_np.get_ts_period() == 300000
 
 
 def test_get_sample_rate_np(wrapper_np):
-    assert wrapper_np.get_ts_sample_rate() == 0.01
+    assert math.isclose(wrapper_np.get_ts_sample_rate(), 0.01)
 
 
 def test_build_raw_np(wrapper_np):
     wrapper_np.get_channels_info()  # need to init ch_names for wrapper
 
     raw = wrapper_np.build_raw()
     data = wrapper_np.data[:, 0, :].squeeze()
@@ -88,15 +90,15 @@
 def test_build_wrapper_tvb(wrapper_tvb):
     assert wrapper_tvb.data_shape == (4000, 4, 76, 1)
 
     ch_names, ch_order, ch_type = wrapper_tvb.get_channels_info()
     assert len(ch_names) == len(ch_order) == len(ch_type) == 76
 
     assert wrapper_tvb.displayed_time_points == 3000
-    assert wrapper_tvb.get_ts_period() == 0.75
+    assert math.isclose(wrapper_tvb.get_ts_period(), 0.75)
     assert wrapper_tvb.get_ts_sample_rate() == 4000
 
     raw = wrapper_tvb.build_raw()
     data = wrapper_tvb.data.data[:, 0, :, 0].squeeze()
     data = np.swapaxes(data, 0, 1)
 
     assert np.array_equal(raw.get_data(), data)
@@ -116,15 +118,15 @@
     new_data = wrapper_tvb.data.data[:, sel1, :, sel2]
 
     assert np.array_equal(data_with_slice, new_data)
 
 
 def test_get_ts_period_tvb(wrapper_tvb):
     ts_period = wrapper_tvb.get_ts_period()
-    assert ts_period == 0.75
+    assert math.isclose(ts_period, 0.75)
 
 
 def test_get_ts_sample_rate_tvb(wrapper_tvb):
     sample_rate = wrapper_tvb.get_ts_sample_rate()
     assert sample_rate == 4000
 
 
@@ -166,7 +168,9 @@
     sel1 = 0
     sel2 = 0
 
     ch_value = wrapper_tvb.get_hover_channel_value(x, ch_index, sel1, sel2)
     val = wrapper_tvb.data.data[x_int, sel1, ch_index, sel2]
     val = round(val, 4)
     assert ch_value == val
+
+
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/tests/ts/test_mne_widget.py` & `tvb-widgets-2.0.0/tvbwidgets/tests/ts/test_mne_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
+import math
 import numpy as np
 import pytest
 import logging
 from ipywidgets import Checkbox
 from tvbwidgets.tests.ts.ts_generator import generate_ts_with_mode_and_sv
 from tvbwidgets.ui.ts.data_wrappers.tvb_data_wrapper import WrapperTVB
 from tvbwidgets.ui.ts.mne_ts_widget import TimeSeriesWidgetMNE
@@ -39,15 +40,15 @@
     tsw_tvb_data.add_datatype(tsr_4d)
     return tsw_tvb_data
 
 
 # =========================================== WIDGET CREATION ==========================================================
 def test_get_widget(tsw_tvb_data):
     tsw_tvb_data.get_widget()
-    assert type(tsw_tvb_data) == TimeSeriesWidgetMNE
+    assert isinstance(tsw_tvb_data, TimeSeriesWidgetMNE)
 
 
 def test_create_ts_widget(tsw):
     assert tsw.ch_names == []
     assert tsw.ch_order == []
     assert tsw.ch_types == []
     assert tsw.displayed_period == 0
@@ -63,15 +64,15 @@
 
 
 def test_populate_from_data_wrapper_tvb(tsw, wrapper_tvb):
     tsw._populate_from_data_wrapper(wrapper_tvb)
 
     assert tsw.data == wrapper_tvb
     assert tsw.sample_freq == 4000
-    assert tsw.displayed_period == 0.75
+    assert math.isclose(tsw.displayed_period, 0.75)
     assert len(tsw.ch_names) == len(tsw.ch_order) == len(tsw.ch_types) == 76
     assert tsw.raw.get_data().shape == (76, 4000)
 
 
 # ======================================== CHANNEL VALUE AREA ======================================================
 def test_create_annotation_area(tsw_tvb_data):
     ann_area = tsw_tvb_data._create_annotation_area()
@@ -100,15 +101,16 @@
     assert len(tsw_tvb_data.checkboxes) == 76
     assert len(tsw_tvb_data.radio_buttons) == 2
     assert channels_area.get_title(0) == 'Channels'
 
 
 def test_dimensions_selection_update(tsw_tvb_data):
     # simulate unchecking of some checkboxes
-    false_cb_idx = list(np.random.choice(76, size=3, replace=False))
+    rng = np.random.default_rng(50)
+    false_cb_idx = list(rng.choice(76, size=3, replace=False))
     false_cb_names = [f'sig {x}' for x in false_cb_idx]
     for cb_name in false_cb_names:
         tsw_tvb_data.checkboxes[cb_name].value = False
 
     no_false_cb = len([x for x in tsw_tvb_data.checkboxes if tsw_tvb_data.checkboxes[x].value == False])
     assert no_false_cb == 3
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/tests/ts/test_plotly_widget.py` & `tvb-widgets-2.0.0/tvbwidgets/tests/ts/test_plotly_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
+import math
 import pytest
 
 import ipywidgets as widgets
 from plotly_resampler import FigureWidgetResampler
 
 from tvbwidgets.tests.ts.ts_generator import generate_ts_with_mode_and_sv
 from tvbwidgets.ui.ts.data_wrappers.tvb_data_wrapper import WrapperTVB
@@ -40,15 +41,15 @@
     tsw_tvb_data.add_datatype(tsr_4d)
     return tsw_tvb_data
 
 
 # =========================================== WIDGET CREATION ==========================================================
 def test_get_widget(tsw_tvb_data):
     tsw_tvb_data.get_widget()
-    assert type(tsw_tvb_data) == TimeSeriesWidgetPlotly
+    assert isinstance(tsw_tvb_data, TimeSeriesWidgetPlotly)
 
 
 def test_create_ts_widget(tsw):
     assert tsw.ch_names == []
     assert not hasattr(tsw, 'ch_order')
     assert not hasattr(tsw, 'ch_types')
     assert tsw.start_time == 0
@@ -60,15 +61,15 @@
 
 # =============================================== SETUP ================================================================
 def test_populate_from_data_wrapper_tvb(tsw, wrapper_tvb):
     tsw._populate_from_data_wrapper(wrapper_tvb)
 
     assert tsw.data == wrapper_tvb
     assert tsw.sample_freq == 4000
-    assert tsw.displayed_period == 0.75
+    assert math.isclose(tsw.displayed_period, 0.75)
     assert len(tsw.ch_names) == 76
     assert tsw.raw.get_data().shape == (76, 4000)
 
 
 # ============================================== PLOT ==================================================================
 def test_add_traces_to_plot(tsw_tvb_data):
     data = tsw_tvb_data.raw[:, :][0]
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/tests/ts/ts_generator.py` & `tvb-widgets-2.0.0/tvbwidgets/tests/ts/ts_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 from tvb.simulator.lab import *
 from tvb.datatypes import time_series
 import tvb.datatypes.time_series
 import numpy as np
 import math
@@ -93,12 +93,13 @@
 
     tsr.configure()
     return tsr
 
 
 def _generate_connectivity(no_of_regions):
     labels = np.array(['sig ' + str(i) for i in range(no_of_regions)])
-    conn = connectivity.Connectivity(centres=np.random.rand(no_of_regions, 3),
+    rng = np.random.default_rng(50)
+    conn = connectivity.Connectivity(centres=rng.random(size=(no_of_regions, 3)),
                                      region_labels=labels,
-                                     weights=np.random.rand(no_of_regions, no_of_regions),
-                                     tract_lengths=np.random.rand(no_of_regions, no_of_regions))
+                                     weights=rng.random(size=(no_of_regions, no_of_regions)),
+                                     tract_lengths=rng.random(size=(no_of_regions, no_of_regions)))
     return conn
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/base_widget.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/base_widget.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 from ipywidgets import DOMWidget
 from tvb.basic.neotraits.api import HasTraits
 from tvbwidgets.core.logger.builder import get_logger
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/connectivity_ipy/connectivity_widget.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/connectivity_ipy/connectivity_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import ipywidgets
 import matplotlib
 import numpy
-import pyvista as pv
+import pyvista
 import numpy as np
 from numpy import ndarray
 from tvb.basic.neotraits.api import HasTraits
 from tvb.datatypes.connectivity import Connectivity
 from tvbwidgets.ui.base_widget import TVBWidget
 from tvbwidgets.ui.connectivity_ipy.outputs_3d import PyVistaOutput
 from tvbwidgets.ui.connectivity_ipy.operations import ConnectivityOperations
 from tvbwidgets.ui.connectivity_ipy.config import ConnectivityConfig
 from tvbwidgets.ui.connectivity_ipy.global_context import CONTEXT, ObservableAttrs
 
 DROPDOWN_KEY = 'dropdown'
 
+pyvista.set_jupyter_backend('trame')
 
 class CustomOutput(ipywidgets.Output):
     CONFIG = ConnectivityConfig()
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.plotter = matplotlib.pyplot
@@ -105,26 +106,28 @@
         CONTEXT.observe(on_ctx_change, ObservableAttrs.MATRIX)
         self.widgets_map[DROPDOWN_KEY] = dropdown
         self.children = (dropdown, *self.children)
 
 
 class Connectivity3DViewer(ipywidgets.VBox):
 
-    def __init__(self, **kwargs):
+    def __init__(self, width, height, **kwargs):
         self.output = PyVistaOutput()
+        self.output.plotter.window_size = [width, height]
+        self.output.plotter.set_background("darkgrey")
 
         super(Connectivity3DViewer, self).__init__([self.output], *kwargs)
 
         self.__init_view_connectivity()
         CONTEXT.observe(lambda *args: self.__init_view_connectivity(), ObservableAttrs.CONNECTIVITY)
 
     def __init_view_connectivity(self):
         self.output.plotter.clear()
         points, edges = self.__add_actors()
-        points_toggle, edges_toggle, labels_toggle = self.__init_controls()
+        points_toggle, edges_toggle = self.__init_controls()
 
         def on_change_points(change):
             if change['new']:
                 self.output.display_actor(points)
             else:
                 self.output.hide_actor(points)
             self.output.update_plot()
@@ -136,42 +139,38 @@
                 self.output.display_actor(edges)
             else:
                 self.output.hide_actor(edges)
             self.output.update_plot()
 
         edges_toggle.observe(on_change_edges, 'value')
 
-        window_controls = self.output.get_window_controls()
 
         self.children = [
             ipywidgets.HBox(children=(
-                points_toggle, edges_toggle, labels_toggle)),
-            window_controls,
+                points_toggle, edges_toggle)),
             self.output]
         self.output.display_actor(points)
         self.output.display_actor(edges)
         self.output.update_plot()
 
     def __init_controls(self):
         points_toggle = ipywidgets.ToggleButton(value=True,
                                                 description='Points'
                                                 )
         edges_toggle = ipywidgets.ToggleButton(value=True,
                                                description='Edges',
                                                )
 
-        labels_toggle = ipywidgets.ToggleButton(value=False,
-                                                description='Labels')
-        return points_toggle, edges_toggle, labels_toggle
+        return points_toggle, edges_toggle
 
     def __add_actors(self):
         plotter = self.output.plotter
         points = CONTEXT.connectivity.centres
 
-        mesh_points = pv.PolyData(points)
+        mesh_points = pyvista.PolyData(points)
 
         points_color = self.output.CONFIG.points_color
         points_size = self.output.CONFIG.point_size
         edge_color = self.output.CONFIG.edge_color
 
         points_actor = plotter.add_points(mesh_points, color=points_color, point_size=points_size)
 
@@ -193,19 +192,19 @@
             edges_coords.append(points[i])
             edges_coords.append(points[j])
 
         return numpy.array(edges_coords)
 
 
 class ConnectivityViewers(ipywidgets.Accordion):
-    def __init__(self, **kwargs):
+    def __init__(self, width, height, **kwargs):
         super().__init__(**kwargs)
         self.children = [
             Connectivity2DViewer(),
-            Connectivity3DViewer()
+            Connectivity3DViewer(width, height)
         ]
         self.set_title(0, '2D Connectivity Matrix viewer')
         self.set_title(1, '3D Connectivity viewer')
 
 
 class ConnectivityWidget(ipywidgets.VBox, TVBWidget):
     """
@@ -231,26 +230,26 @@
         if gid is None:
             return CONTEXT.connectivity
         conn = list(filter(lambda c: c.gid.hex == gid, CONTEXT.connectivities_history))
         if not len(conn):
             return None
         return conn[0]
 
-    def __init__(self, connectivity, default_active_tab='both', **kwargs):
+    def __init__(self, connectivity, default_active_tab='both', width=500, height=500, **kwargs):
 
         style = self.DEFAULT_BORDER
         super().__init__(**kwargs, layout=style)
 
         config = ConnectivityConfig(name=f'Connectivity - {str(connectivity.number_of_regions)}')
         CONTEXT.connectivity = connectivity
 
         viewers_visible = default_active_tab in ['both', 'viewers']
         operations_visible = default_active_tab in ['both', 'operations']
 
-        self.viewers_tab = ConnectivityViewers()
+        self.viewers_tab = ConnectivityViewers(width, height)
         self.viewers_tab.layout.display = viewers_visible and 'inline-block' or 'none'
         self.operations_tab = ConnectivityOperations()
         self.operations_tab.layout.display = operations_visible and 'inline-block' or 'none'
         tabs = (self.viewers_tab, self.operations_tab)
 
         viewers_checkbox = ipywidgets.Checkbox(value=viewers_visible or default_active_tab == 'viewers',
                                                description='Viewers')
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/connectivity_ipy/global_context.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/connectivity_ipy/global_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 import enum
 from typing import Callable
 from tvb.datatypes.connectivity import Connectivity
 
 
 class ObservableAttrs(str, enum.Enum):
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/connectivity_ipy/operations.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/connectivity_ipy/operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 import ipywidgets
 import numpy
 from tvb.datatypes.connectivity import Connectivity
 
 from tvbwidgets.ui.base_widget import TVBWidget
 from tvbwidgets.ui.connectivity_ipy.global_context import CONTEXT
@@ -146,21 +146,21 @@
                                          edge_operations])
 
     def __cut_nodes(self, selected=True):
         """
         Create a new connectivity using only the selected nodes
         """
         regions = CONTEXT.connectivity.region_labels
-        selected_regions = [numpy.where(regions == label)[0][0] for label in self.selected_regions]
+        selected_regions = [numpy.nonzero(regions == label)[0][0] for label in self.selected_regions]
         new_conn = self.__cut_connectivity_nodes(selected_regions, selected)
         CONTEXT.connectivity = new_conn
 
     def __cut_edges(self, selected=False):
         regions = CONTEXT.connectivity.region_labels
-        selected_regions = numpy.array([numpy.where(regions == label)[0][0] for label in self.selected_regions])
+        selected_regions = numpy.array([numpy.nonzero(regions == label)[0][0] for label in self.selected_regions])
         new_conn = self.__cut_connectivity_edges(selected_regions, selected)
         CONTEXT.connectivity = new_conn
 
     def __reorder_arrays(self, original_conn, new_weights, interest_areas, new_tracts=None):
         """
         Returns ordered versions of the parameters according to the hemisphere permutation.
         """
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/connectivity_react/connectivity_model.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/connectivity_react/connectivity_model.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/connectivity_react/connectivity_widget.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/connectivity_react/connectivity_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import pathlib
 
 import ipyreact
 import traitlets
 from IPython.display import HTML
 
 from .connectivity_model import ConnectivityDTO
 
 
-class ConnectivityWidgetReact(ipyreact.ReactWidget):
+class ConnectivityWidgetReact(ipyreact.Widget):
     _esm = pathlib.Path(__file__).resolve().parent / 'Connectivity.tsx'
     css_rules = (pathlib.Path(__file__).resolve().parent / 'Connectivity.css').read_text()
     HTML("<style>" + css_rules + "</style>")
     connectivity = traitlets.Any().tag(sync=True)
 
     def __init__(self, connectivity=None, **kwargs):
         self.connectivity = ConnectivityDTO(
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/drive_widget.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/drive_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import os
 import ipywidgets
 import ebrains_drive
 from ebrains_drive.exceptions import DoesNotExist
 from tvbwidgets.core.auth import get_current_token
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/head_widget.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/head_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import ipywidgets
 import numpy
 import pyvista
-
-from pyvista import PolyData
-
 from tvb.basic.neotraits.api import HasTraits
 from tvb.datatypes.connectivity import Connectivity
 from tvb.datatypes.region_mapping import RegionMapping
 from tvb.datatypes.sensors import Sensors
 from tvb.datatypes.surfaces import Surface
 
 from tvbwidgets.ui.base_widget import TVBWidget
 from tvbwidgets.ui.widget_with_browser import TVBWidgetWithBrowser
 
-pyvista.set_jupyter_backend('pythreejs')
+pyvista.set_jupyter_backend('trame')
 
 
 class HeadWidgetConfig:
 
-    def __init__(self, name='Actor', style='Surface', color='White', light=True, size=1500, cmap=None, scalars=None):
+    def __init__(self, name='Actor', style='Surface', color='White', light=True, size=15, cmap=None, scalars=None):
         self.name = name
         self.style = style
         self.color = color
         self.light = light
         self.size = size
         self.cmap = cmap
         self.scalars = scalars
@@ -52,14 +49,16 @@
 class CustomOutput(ipywidgets.Output):
     CONFIG = HeadWidgetConfig()
     MAX_ACTORS = 10
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.plotter = pyvista.Plotter()
+        self.plotter.window_size = [600, 600]
+        self.plotter.set_background('darkgrey')
         self.total_actors = 0
 
     @property
     def can_draw(self):
         return self.total_actors < self.MAX_ACTORS
 
     def add_mesh(self, mesh, config=CONFIG):
@@ -100,14 +99,15 @@
                        - default is set to False because Ebrains Lab does not support surfaces with incompatible coloring
                         (kills the kernel)
                        - locally this issue does not appear
         """
         self.output_plot = CustomOutput()
         self.plot_controls = ipywidgets.Accordion(layout=ipywidgets.Layout(width='380px'))
         self.existent_configs = []
+        self.title_suffix = " Controls"
         self.ignore = ignore
 
         super().__init__([self.plot_controls, self.output_plot], layout=self.DEFAULT_BORDER)
 
         if datatypes is not None:
             if not isinstance(datatypes, list):
                 self.logger.warning("Input not supported. Please provide a list of datatypes.")
@@ -133,19 +133,18 @@
             self.__draw_sensors_actor(datatype, config)
         elif isinstance(datatype, RegionMapping):
             self.logger.info("RegionMapping should be given as cmap in the config parameter!")
         else:
             self.logger.warning(f"Datatype {type(datatype)} not supported by this widget!")
 
     def __prepare_mesh(self, surface):
-        # type: (Surface) -> PolyData
+        # type: (Surface) -> pyvista.PolyData
         dim_4th = numpy.full((surface.triangles.shape[0], 1), 3, dtype=int)
         faces = numpy.hstack((dim_4th, surface.triangles))
-
-        mesh = PolyData(surface.vertices, faces)
+        mesh = pyvista.PolyData(surface.vertices, faces)
         return mesh
 
     def __toggle_actor(self, change, actor):
         if change.type == 'change':
             if change.new is True:
                 self.output_plot.display_actor(actor)
             else:
@@ -170,60 +169,59 @@
 
         controls_vbox = self._prepare_generic_controls(mesh_actor, config)
 
         extra_controls = self.__prepare_surface_controls(mesh_actor)
         controls_vbox.children += extra_controls
 
         self.plot_controls.children += controls_vbox,
+        self.plot_controls.set_title(self.output_plot.total_actors - 1, config.name + self.title_suffix)
         self.output_plot.update_plot()
 
     def __draw_connectivity_actor(self, connectivity, config):
         # type: (Connectivity, HeadWidgetConfig) -> None
         if config is None:
             config = HeadWidgetConfig(name='Connectivity-' + str(connectivity.number_of_regions), color='Green')
 
         conn_actor = self.output_plot.add_points(connectivity.centres, config)
         controls_vbox = self._prepare_generic_controls(conn_actor, config)
         extra_controls = self.__prepare_points_controls(conn_actor, config)
         controls_vbox.children += extra_controls
 
         self.plot_controls.children += controls_vbox,
+        self.plot_controls.set_title(self.output_plot.total_actors - 1, config.name + self.title_suffix)
         self.output_plot.update_plot()
 
     def __draw_sensors_actor(self, sensors, config):
         # type: (Sensors, HeadWidgetConfig) -> None
         if config is None:
-            config = HeadWidgetConfig(name='Sensors-' + str(sensors.number_of_sensors), color='Pink', size=1000)
+            config = HeadWidgetConfig(name='Sensors-' + str(sensors.number_of_sensors), color='Pink', size=10)
 
         sensors_actor = self.output_plot.add_points(sensors.locations, config)
         controls_vbox = self._prepare_generic_controls(sensors_actor, config)
         extra_controls = self.__prepare_points_controls(sensors_actor, config)
         controls_vbox.children += extra_controls
 
         self.plot_controls.children += controls_vbox,
+        self.plot_controls.set_title(self.output_plot.total_actors - 1, config.name + self.title_suffix)
         self.output_plot.update_plot()
 
     def _prepare_generic_controls(self, actor, config):
         toggle_prefix = "Toggle "
-        title_suffix = " Controls"
-
-        idx = self.output_plot.total_actors - 1
-        self.plot_controls.set_title(idx, config.name + title_suffix)
 
         def toggle_actor(change):
             self.__toggle_actor(change, actor)
 
         toggle_input = ipywidgets.Checkbox(description=toggle_prefix + config.name, value=True)
         toggle_input.observe(toggle_actor, names=['value'])
 
         def on_name_change(change):
             value = change['new']
             config.name = value
             toggle_input.description = toggle_prefix + config.name
-            self.plot_controls.set_title(idx, config.name + title_suffix)
+            self.plot_controls.set_title(self.output_plot.total_actors - 1, config.name + self.title_suffix)
 
         name_input = ipywidgets.Text(value=config.name, description='Name: ', disabled=False,
                                      layout=ipywidgets.Layout(width='250px'))
         name_input.observe(on_name_change, names='value')
 
         def on_color_change(change):
             value = change['new']
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/phase_plane_widget.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/phase_plane_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import colorsys
 import ipywidgets as widgets
 import matplotlib.pyplot as plt
 import numpy as np
 import tvb.simulator.integrators as integrators_module
@@ -70,14 +70,18 @@
         self.export_filename = None
         self.disable_model_dropdown = False
         self.disable_export_dropdown = False
         self.plot_size = 4, 5
         self.plot_main_axes = None
         self.plot_bellow = None
         self.noise_sliders = []
+        if hasattr(self.integrator, 'noise'):
+            self.noise_slider_valinit = self.integrator.noise.nsig[0]
+        else:
+            self.noise_slider_valinit = 0
         self.trajectories = []
         # Parameters to be passed to plotter when their change affects the drawing
         self.params = dict()
 
         # Prepare the initial state
         self.svx = self.model.state_variables[0]  # x-axis: 1st state variable
         self.svy = self.model.state_variables[1]  # y-axis: 2nd state variable
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/pse_launcher_widget.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/pse_launcher_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import threading
 import numpy as np
 import ipywidgets as widgets
 from tvb.basic.neotraits.api import NArray
 from tvb.simulator.simulator import Simulator
@@ -74,15 +74,15 @@
 
         if self.connectivity_list is not None:
             self.params_dict["connectivity"] = [0, 0, 0]
 
     def file_options(self):
         self.file_name = widgets.Text(
             placeholder='Type here',
-            description="<b>Name of file</b>",
+            description="Name of file",
             disabled=False
         )
 
     def _prepare_launch(self, where="Local"):
         self._update_info_message(f"{where} launch in progress ...")
         x_values = self.compute_params_values(self.param_1.value)
         y_values = self.compute_params_values(self.param_2.value)
@@ -151,15 +151,15 @@
                 self.progress.value += 1
             elif jobs_completed >= 0:
                 self.progress.value = jobs_completed + 1
 
     def create_metrics(self):
         self.metrics_sm = widgets.SelectMultiple(
             options=self.metrics,
-            description="<b>Metrics</b>",
+            description="Metrics",
             value=[self.metrics[0]],
             disabled=False, layout=widgets.Layout(margin="0px 20px 10px 25px", height="115px", width="340px"))
 
     def _create_infos(self):
         self.title = widgets.HTML(value="<font color='navyblue' size='4'>PSE Launcher</font>",
                                   layout=widgets.Layout(margin="0px 0px 0px 20px"))
         self.message_area = widgets.HTML(value="<p></p>", layout=widgets.Layout(margin="0px 0px 0px 20px"))
@@ -175,21 +175,21 @@
         for elem in np.arange(min_value, max_value, step):
             values.append(elem)
         return values
 
     def create_params(self):
         self.param_1 = widgets.Dropdown(
             options=sorted(self.params_dict.keys()),
-            description="<b>Param 1</b>",
+            description="Param 1",
             value=list(sorted(self.params_dict.keys()))[0],
             disabled=False
         )
         self.param_2 = widgets.Dropdown(
             options=sorted(self.params_dict.keys()),
-            description="<b>Param 2</b>",
+            description="Param 2",
             value=list(sorted(self.params_dict.keys()))[2],
             disabled=False
         )
 
         def param_changed(change):
             if change['type'] != 'change' or change['name'] != 'value':
                 return
@@ -264,27 +264,27 @@
                                            layout=widgets.Layout(margin="20px 0px 0px 0px"))
         return widgets.VBox(children=[self.title, self.message_area, param_box1, param_box2, metrics_buttons_box],
                             layout=self.DEFAULT_BORDER)
 
     def _build_for_param(self, param_current):
         min_input = widgets.FloatText(
             value=self.params_dict[param_current.value][0],
-            description="<b><font color='gray'>Min range</b>",
+            description="Min range",
             disable=False
         )
 
         max_input = widgets.FloatText(
             value=self.params_dict[param_current.value][1],
-            description="<b><font color='gray'>Max range</b>",
+            description="Max range",
             disable=False
         )
 
         step_input = widgets.FloatText(
             value=self.params_dict[param_current.value][2],
-            description="<b><font color='gray'>Step</b>",
+            description="Step",
             disable=False
         )
 
         range_box = widgets.VBox(children=[min_input, max_input, step_input],
                                  layout=widgets.Layout(margin="0px 0px 0px 40px"))
 
         param_box = widgets.HBox(children=[param_current, range_box],
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/pse_widget.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/pse_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import os.path
 import plotly.graph_objects as go
 import ipywidgets as widgets
 from IPython.core.display_functions import display
 from tvbwidgets.core.exceptions import InvalidInputException
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/storage_widget.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/storage_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 import ipywidgets
 
 from tvbwidgets.ui.base_widget import TVBWidget
 from tvbwidgets.ui.drive_widget import DriveWidget
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/ts/base_ts_widget.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/ts/base_ts_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import math
 import numpy as np
 import ipywidgets as widgets
 from tvb.datatypes.time_series import TimeSeries
 
 from tvbwidgets.core.exceptions import InvalidInputException
 from tvbwidgets.ui.base_widget import TVBWidget
 from tvbwidgets.ui.ts.data_wrappers.tvb_data_wrapper import WrapperTVB
 from tvbwidgets.ui.ts.data_wrappers.numpy_data_wrapper import WrapperNumpy
 
+
 class TimeSeriesWidgetBase(widgets.VBox, TVBWidget):
     # =========================================== SETUP ================================================================
     def add_datatype(self, ts_tvb):
         # type: (TimeSeries) -> None
         data_wrapper = WrapperTVB(ts_tvb)
         self.logger.debug("Adding TVB TS for display...")
         self._populate_from_data_wrapper(data_wrapper)
@@ -108,8 +109,8 @@
         accordion.set_title(0, title)
         return accordion, sel_radio_btn
 
     def _dimensions_selection_update(self, _):
         # update self.raw
         sel1, sel2 = self._get_selection_values()
         new_slice = self.data.get_update_slice(sel1, sel2)
-        self.raw = self.data.build_raw(new_slice)
+        self.raw = self.data.build_raw(new_slice)
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/ts/data_wrappers/base_data_wrapper.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/ts/data_wrappers/base_data_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 from abc import ABC, abstractmethod
 
 
 class ABCDataWrapper(ABC):
     """ Wrap any TimeSeries for TSWidget to read/parse uniformly"""
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/ts/data_wrappers/numpy_data_wrapper.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/ts/data_wrappers/numpy_data_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import mne
 import numpy as np
 from tvbwidgets.core.exceptions import InvalidInputException
 from tvbwidgets.ui.ts.data_wrappers.base_data_wrapper import ABCDataWrapper
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/ts/data_wrappers/tvb_data_wrapper.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/ts/data_wrappers/tvb_data_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import mne
 import numpy as np
 from tvb.datatypes.time_series import TimeSeries
 from tvbwidgets.core.exceptions import InvalidInputException
 from tvbwidgets.ui.ts.data_wrappers.base_data_wrapper import ABCDataWrapper
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/ts/mne_ts_widget.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/ts/mne_ts_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import os
 import mne
 import numpy as np
 import ipywidgets as widgets
 import matplotlib.pyplot as plt
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/ts/plotly_ts_widget.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/ts/plotly_ts_widget.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,69 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import numpy as np
 import ipywidgets as widgets
+import matplotlib.pyplot as plt
+import matplotlib.colors as mlt
 from IPython.core.display_functions import display
 from plotly_resampler import register_plotly_resampler, FigureWidgetResampler
 from tvbwidgets.ui.ts.base_ts_widget import TimeSeriesWidgetBase
 
 
 class TimeSeriesWidgetPlotly(TimeSeriesWidgetBase):
     """ TimeSeries Widget drawn using plotly"""
 
     def __init__(self, **kwargs):
         # data
         self.fig = None
         self.data = None
         self.ch_names = []
+        self.ch_picked = []
         self.raw = None
         self.sample_freq = 0
         self.start_time = 0
         self.end_time = 0
         self.std_step = 0
         self.amplitude = 1
+        self.colormap = None
 
         # plot & UI
         self.checkboxes = dict()
         self.plot_area = widgets.HBox()
         self.output = widgets.Output()
         self.channel_selection_area = widgets.HBox(layout=widgets.Layout(width='90%'))
         self.info_and_channels_area = widgets.HBox(layout=widgets.Layout(margin='0px 0px 0px 80px'))
         self.plot_area.children += (self.output,)
-        self.scaling_title = widgets.Label(value='Increase/Decrease signal scaling (current scaling value to the right)')
+        self.scaling_title = widgets.Label(
+            value='Increase/Decrease signal scaling (current scaling value to the right)')
         self.scaling_slider = widgets.IntSlider(value=1, layout=widgets.Layout(width='30%'))
-
-        super().__init__([self.plot_area, widgets.VBox([self.scaling_title, self.scaling_slider],
-                                                       layout=widgets.Layout(margin='0px 0px 0px 80px')),
-                          self.info_and_channels_area],
-                         layout=self.DEFAULT_BORDER)
+        self.colormaps = ['turbo', 'brg', 'gist_stern_r', 'nipy_spectral_r', 'coolwarm', 'plasma', 'magma', 'viridis', \
+                          'cividis', 'twilight', 'twilight_shifted', 'CMRmap_r', 'Blues', \
+                          'BuGn', 'BuPu', 'Greens', 'PuRd', 'RdPu', 'Spectral', 'YlGnBu', \
+                          'YlOrBr', 'YlOrRd', 'cubehelix_r', 'gist_earth_r', 'terrain_r', \
+                          'rainbow_r', 'pink_r', 'gist_ncar_r', 'uni-color(black)']
+        self.colormap_dropdown = widgets.Dropdown(options=self.colormaps, description='Colormap:', disabled=False)
+        self.colormap_dropdown.observe(self.update_colormap, names='value')
+
+        super().__init__(
+            [self.plot_area, widgets.VBox([self.colormap_dropdown, self.scaling_title, self.scaling_slider],
+                                          layout=widgets.Layout(margin='0px 0px 0px 80px')),
+             self.info_and_channels_area],
+            layout=self.DEFAULT_BORDER)
         self.logger.info("TimeSeries Widget with Plotly initialized")
 
     # =========================================== SETUP ================================================================
     def _populate_from_data_wrapper(self, data_wrapper):
         super()._populate_from_data_wrapper(data_wrapper=data_wrapper)
+        self.ch_picked = list(range(len(self.ch_names)))
         del self.ch_order, self.ch_types  # delete these as we don't use them in plotly
         # populate channel selection area
         self.channels_area = self._create_channel_selection_area(array_wrapper=data_wrapper)
         self._setup_scaling_slider()
         self.channel_selection_area.children += (self.channels_area,)
         # populate info area
         info = self._create_info_area()
@@ -58,17 +72,25 @@
 
     # =========================================== PLOT =================================================================
     def add_traces_to_plot(self, data, ch_names):
         """ Draw the traces """
         # traces will be added from bottom to top, so reverse the lists to put the first channel on top
         data = data[::-1]
         ch_names = ch_names[::-1]
+        if self.colormap == "uni-color(black)":
+            colormap = plt.get_cmap('gray')
+            colors = colormap(np.linspace(0, 0, len(ch_names)))
+        else:
+            colormap = plt.get_cmap(self.colormap)
+            colors = colormap(np.linspace(0.3, 1, len(ch_names)))
+        colors = [mlt.to_hex(color, keep_alpha=False) for color in colors]
 
         self.fig.add_traces(
-            [dict(y=ts * self.amplitude + i * self.std_step, name=ch_name, customdata=ts, hovertemplate='%{customdata}')
+            [dict(y=ts * self.amplitude + i * self.std_step, name=ch_name, customdata=ts, hovertemplate='%{customdata}',
+                  line_color=colors[i])
              for i, (ch_name, ts) in enumerate(zip(ch_names, data))]
         )
 
     def _populate_plot(self, data=None, ch_names=None):
         # create traces for each signal
         data_from_raw = self.raw[:, :][0]
         data = data if data is not None else data_from_raw
@@ -133,14 +155,22 @@
 
     def plot_ts_with_plotly(self, data=None, ch_names=None):
         self.create_plot(data, ch_names)
         with self.output:
             self.output.clear_output(wait=True)
             display(self.fig)
 
+    def update_colormap(self, change):
+        self.colormap = change['new']
+        self.fig.data = []
+        data = self.raw[:, :][0]
+        data = data[self.ch_picked, :]
+        ch_names = [self.ch_names[i] for i in self.ch_picked]
+        self.add_traces_to_plot(data, ch_names)
+
     # ================================================= SCALING ========================================================
     def _setup_scaling_slider(self):
         # set min and max scaling values
         self.scaling_slider.min = 1
         self.scaling_slider.max = 10
         self.scaling_slider.observe(self.update_scaling, names='value', type='change')
 
@@ -148,16 +178,17 @@
         """ Update the amplitude of traces based on slider value """
         new_val = val['new']
         self.amplitude = new_val
 
         # delete old traces
         self.fig.data = []
         data = self.raw[:, :][0]
-
-        self.add_traces_to_plot(data, self.ch_names)
+        data = data[self.ch_picked, :]
+        ch_names = [self.ch_names[i] for i in self.ch_picked]
+        self.add_traces_to_plot(data, ch_names)
 
     # =========================================== CHANNELS SELECTION ===================================================
     def _create_channel_selection_area(self, array_wrapper, no_checkbox_columns=5):
         # type: (ABCDataWrapper) -> widgets.Accordion
         """ Create the whole channel selection area: Submit button to update plot, Select/Uselect all buttons,
             State var. & Mode selection and Channel checkboxes
         """
@@ -191,32 +222,32 @@
         return channels_area
 
     def _update_ts(self, btn):
         self.logger.debug('Updating TS')
         ch_names = list(self.ch_names)
 
         # save selected channels using their index in the ch_names list
-        picks = []
+        self.ch_picked = []
         for cb in list(self.checkboxes.values()):
             ch_index = ch_names.index(cb.description)  # get the channel index
             if cb.value:
-                picks.append(ch_index)  # list with number representation of channels
+                self.ch_picked.append(ch_index)  # list with number representation of channels
 
         # if unselect all
         # TODO: should we remove just the traces and leave the channel names and the ticks??
-        if not picks:
+        if not self.ch_picked:
             self.fig.data = []  # remove traces
             self.fig.layout.annotations = []  # remove channel names
             self.fig.layout.yaxis.tickvals = []  # remove ticks between channel names and traces
             return
 
         # get data and names for selected channels; self.raw is updated before redrawing starts
         data, _ = self.raw[:, :]
-        data = data[picks, :]
-        ch_names = [ch_names[i] for i in picks]
+        data = data[self.ch_picked, :]
+        ch_names = [ch_names[i] for i in self.ch_picked]
 
         # redraw the entire plot
         self.plot_ts_with_plotly(data, ch_names)
 
     # ================================================ INFO AREA =======================================================
     def _create_info_area(self):
         # navigate through timeline
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/ts/ts_widget_browser.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/ts/ts_widget_browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import ipywidgets as widgets
 from tvb.datatypes.time_series import TimeSeries
 from tvbwidgets.ui.ts.mne_ts_widget import TimeSeriesWidgetMNE
 from tvbwidgets.ui.ts.plotly_ts_widget import TimeSeriesWidgetPlotly
 from tvbwidgets.ui.widget_with_browser import TVBWidgetWithBrowser
```

### Comparing `tvb-widgets-1.6.0/tvbwidgets/ui/widget_with_browser.py` & `tvb-widgets-2.0.0/tvbwidgets/ui/widget_with_browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import bz2
 import ipywidgets
 from tvb.basic.readers import ReaderException
 
 from tvbwidgets.core.exceptions import InvalidFileException
```

