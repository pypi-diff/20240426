# Comparing `tmp/dspeed-1.3.0a5.tar.gz` & `tmp/dspeed-1.3.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspeed-1.3.0a5.tar", last modified: Tue Feb 20 16:37:06 2024, max compression
+gzip compressed data, was "dspeed-1.3.0a6.tar", last modified: Fri Apr 26 17:53:20 2024, max compression
```

## Comparing `dspeed-1.3.0a5.tar` & `dspeed-1.3.0a6.tar`

### file list

```diff
@@ -1,97 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:37:06.618605 dspeed-1.3.0a5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-02-20 16:37:06.618605 dspeed-1.3.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-02-20 16:37:06.618605 dspeed-1.3.0a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:37:06.602604 dspeed-1.3.0a5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:37:06.606604 dspeed-1.3.0a5/src/dspeed/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-02-20 16:37:06.000000 dspeed-1.3.0a5/src/dspeed/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/build_dsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    88831 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processing_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:37:06.610605 dspeed-1.3.0a5/src/dspeed/processors/
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/bl_subtract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/dwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/energy_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/fftw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/fixed_time_pickoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/gaussian_filter1d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/get_multi_local_extrema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/get_wf_centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/linear_slope_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/log_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/min_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/moving_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/multi_a_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/multi_t_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/param_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/peak_snr_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/pole_zero.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/presum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/pulse_injector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/round_to_nearest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/saturation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/soft_pileup_corr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/svm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/time_over_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/time_point_thresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/transfer_function_convolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8479 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/trap_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/upsampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/wf_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/wiener_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/processors/windower.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:37:06.614605 dspeed-1.3.0a5/src/dspeed/vis/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/vis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23084 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/src/dspeed/vis/waveform_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:37:06.618605 dspeed-1.3.0a5/src/dspeed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-02-20 16:37:06.000000 dspeed-1.3.0a5/src/dspeed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-02-20 16:37:06.000000 dspeed-1.3.0a5/src/dspeed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 16:37:06.000000 dspeed-1.3.0a5/src/dspeed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-20 16:37:06.000000 dspeed-1.3.0a5/src/dspeed.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 16:37:06.000000 dspeed-1.3.0a5/src/dspeed.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-20 16:37:06.000000 dspeed-1.3.0a5/src/dspeed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-20 16:37:06.000000 dspeed-1.3.0a5/src/dspeed.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:37:06.614605 dspeed-1.3.0a5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:37:06.614605 dspeed-1.3.0a5/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (127)    10388 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/configs/icpc-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/configs/numpy-parsing.json
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/configs/sipm-dplms-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/configs/sipm-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:37:06.614605 dspeed-1.3.0a5/tests/processors/
--rw-r--r--   0 runner    (1001) docker     (127)    14296 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/processors/dplms_noise_mat.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/processors/test_dplms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/processors/test_dwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/processors/test_fftw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/processors/test_fixed_time_pickoff.py
--rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/processors/test_get_multi_local_extrema.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/processors/test_get_wf_centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/processors/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/processors/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/processors/test_min_max_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/processors/test_time_point_thresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/processors/test_transfer_function_convolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/processors/test_wf_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/test_build_dsp.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/test_list_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/test_numpy_constants_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/test_processing_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:37:06.618605 dspeed-1.3.0a5/tests/vis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:37:06.618605 dspeed-1.3.0a5/tests/vis/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/vis/configs/hpge-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-02-20 16:37:00.000000 dspeed-1.3.0a5/tests/vis/test_waveform_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.284431 dspeed-1.3.0a6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-26 17:53:20.284431 dspeed-1.3.0a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-26 17:53:20.284431 dspeed-1.3.0a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.264430 dspeed-1.3.0a6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.268431 dspeed-1.3.0a6/src/dspeed/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-26 17:53:20.000000 dspeed-1.3.0a6/src/dspeed/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/build_dsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91711 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processing_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.276430 dspeed-1.3.0a6/src/dspeed/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/bl_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/dwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/energy_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/fftw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/fixed_time_pickoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/gaussian_filter1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/get_multi_local_extrema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/get_wf_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/linear_slope_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/log_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/min_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/moving_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/multi_a_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/multi_t_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/param_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/peak_snr_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/pole_zero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/poly_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/presum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/pulse_injector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/rc_cr2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/round_to_nearest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/saturation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/soft_pileup_corr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/svm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/time_over_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16670 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/time_point_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/transfer_function_convolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8479 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/trap_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/wf_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/wiener_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/windower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.276430 dspeed-1.3.0a6/src/dspeed/vis/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/vis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23174 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/vis/waveform_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.284431 dspeed-1.3.0a6/src/dspeed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-26 17:53:20.000000 dspeed-1.3.0a6/src/dspeed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-26 17:53:20.000000 dspeed-1.3.0a6/src/dspeed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 17:53:20.000000 dspeed-1.3.0a6/src/dspeed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 17:53:20.000000 dspeed-1.3.0a6/src/dspeed.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 17:53:20.000000 dspeed-1.3.0a6/src/dspeed.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-26 17:53:20.000000 dspeed-1.3.0a6/src/dspeed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 17:53:20.000000 dspeed-1.3.0a6/src/dspeed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.276430 dspeed-1.3.0a6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.280431 dspeed-1.3.0a6/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)    10388 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/configs/icpc-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/configs/icpc-dsp-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/configs/numpy-parsing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/configs/sipm-dplms-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/configs/sipm-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.280431 dspeed-1.3.0a6/tests/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)    14296 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/dplms_noise_mat.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_dplms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_dwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_fftw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_fixed_time_pickoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_get_multi_local_extrema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_get_wf_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_min_max_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_pole_zero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_rc_cr2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13231 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_time_point_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_transfer_function_convolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_wf_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/test_build_dsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/test_list_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/test_numpy_constants_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/test_processing_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.280431 dspeed-1.3.0a6/tests/vis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.280431 dspeed-1.3.0a6/tests/vis/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/vis/configs/hpge-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/vis/test_waveform_browser.py
```

### Comparing `dspeed-1.3.0a5/LICENSE` & `dspeed-1.3.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/PKG-INFO` & `dspeed-1.3.0a6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspeed
-Version: 1.3.0a5
+Version: 1.3.0a6
 Summary: Fast Digital Signal Processing for particle detectors in Python
 Home-page: https://github.com/legend-exp/dspeed
 Author: Ian Guinn
 Author-email: guinnis@ornl.gov
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
@@ -52,35 +52,54 @@
 Provides-Extra: test
 Requires-Dist: pre-commit; extra == "test"
 Requires-Dist: pylegendtestdata; extra == "test"
 Requires-Dist: pytest>=6.0; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: scipy; extra == "test"
 
+# DSPeed
+
 ```
 _____  _________________________________________________________________
      ||                  ____  _____  ____                   __          `,_
      ||                 / __ \/ ___/ / __ \ ___   ___   ____/ /           | `-_
  []  ||  [] [] [] []   / / / /\__ \ / /_/ // _ \ / _ \ / __  /  [] [] []  '-----`-,_
  ====||===============/ /_/ /___/ // ____//  __//  __// /_/ /====================== ``--,_
      ||              /_____//____//_/     \___/ \___/ \__,_/                              ``--,
      ||    ________                                                        ________            )
 \____||___/.-.  .-.\______________________________________________________/.-.  .-.\______,,--'
 ==========='-'=='-'========================================================'-'=='-'=============
 ```
+
 [![PyPI](https://img.shields.io/pypi/v/dspeed?logo=pypi)](https://pypi.org/project/dspeed/)
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/legend-exp/dspeed?logo=git)
 [![GitHub Workflow Status](https://img.shields.io/github/checks-status/legend-exp/dspeed/main?label=main%20branch&logo=github)](https://github.com/legend-exp/dspeed/actions)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Codecov](https://img.shields.io/codecov/c/github/legend-exp/dspeed?logo=codecov)](https://app.codecov.io/gh/legend-exp/dspeed)
 ![GitHub issues](https://img.shields.io/github/issues/legend-exp/dspeed?logo=github)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/legend-exp/dspeed?logo=github)
 ![License](https://img.shields.io/github/license/legend-exp/dspeed)
 [![Read the Docs](https://img.shields.io/readthedocs/dspeed?logo=readthedocs)](https://dspeed.readthedocs.io)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10684779.svg)](https://doi.org/10.5281/zenodo.10684779)
 
-# DSPeed
-DSPeed (pronounced dee-ess-speed) is a python-based package that performs bulk, high-performance digital signal processing (DSP) of time-series data such as digitized waveforms. This package is part of the [pygama](https://github.com/legend-exp/pygama) scientific computing suite.
+DSPeed (pronounced dee-ess-speed) is a python-based package that performs bulk,
+high-performance digital signal processing (DSP) of time-series data such as
+digitized waveforms. This package is part of the
+[pygama](https://github.com/legend-exp/pygama) scientific computing suite.
+
+DSPeed enables the user to define an arbitrary chain of vectorized signal
+processing routines that can be applied in bulk to waveforms and other data
+provided using the
+[LH5-format](https://legend-exp.github.io/legend-data-format-specs). These
+routines can include [numpy
+ufuncs](https://numpy.org/doc/stable/reference/ufuncs.html), custom functions
+accelerated with [numba](https://numba.pydata.org/), or other arbitrary
+functions. DSPeed will carefully manage file I/O to optimize memory usage and
+performance. Processing chains are defined using highly portable JSON files
+that can be applied to data from multiple digitizers.
 
-DSPeed enables the user to define an arbitrary chain of vectorized signal processing routines that can be applied in bulk to waveforms and other data provided using the [LH5-format](https://legend-exp.github.io/legend-data-format-specs). These routines can include [numpy ufuncs](https://numpy.org/doc/stable/reference/ufuncs.html), custom functions accelerated with [numba](https://numba.pydata.org/), or other arbitrary functions. DSPeed will carefully manage file I/O to optimize memory usage and performance. Processing chains are defined using highly portable JSON files that can be applied to data from multiple digitizers.
+See the [online documentation](https://dspeed.readthedocs.io/en/stable/) for
+more information.
 
-See the [online documentation](https://dspeed.readthedocs.io/en/stable/) for more information!
+If you are using this software, consider
+[citing](https://doi.org/10.5281/zenodo.10684779)!
```

### Comparing `dspeed-1.3.0a5/README.md` & `dspeed-1.3.0a6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,47 @@
+# DSPeed
+
 ```
 _____  _________________________________________________________________
      ||                  ____  _____  ____                   __          `,_
      ||                 / __ \/ ___/ / __ \ ___   ___   ____/ /           | `-_
  []  ||  [] [] [] []   / / / /\__ \ / /_/ // _ \ / _ \ / __  /  [] [] []  '-----`-,_
  ====||===============/ /_/ /___/ // ____//  __//  __// /_/ /====================== ``--,_
      ||              /_____//____//_/     \___/ \___/ \__,_/                              ``--,
      ||    ________                                                        ________            )
 \____||___/.-.  .-.\______________________________________________________/.-.  .-.\______,,--'
 ==========='-'=='-'========================================================'-'=='-'=============
 ```
+
 [![PyPI](https://img.shields.io/pypi/v/dspeed?logo=pypi)](https://pypi.org/project/dspeed/)
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/legend-exp/dspeed?logo=git)
 [![GitHub Workflow Status](https://img.shields.io/github/checks-status/legend-exp/dspeed/main?label=main%20branch&logo=github)](https://github.com/legend-exp/dspeed/actions)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Codecov](https://img.shields.io/codecov/c/github/legend-exp/dspeed?logo=codecov)](https://app.codecov.io/gh/legend-exp/dspeed)
 ![GitHub issues](https://img.shields.io/github/issues/legend-exp/dspeed?logo=github)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/legend-exp/dspeed?logo=github)
 ![License](https://img.shields.io/github/license/legend-exp/dspeed)
 [![Read the Docs](https://img.shields.io/readthedocs/dspeed?logo=readthedocs)](https://dspeed.readthedocs.io)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10684779.svg)](https://doi.org/10.5281/zenodo.10684779)
 
-# DSPeed
-DSPeed (pronounced dee-ess-speed) is a python-based package that performs bulk, high-performance digital signal processing (DSP) of time-series data such as digitized waveforms. This package is part of the [pygama](https://github.com/legend-exp/pygama) scientific computing suite.
+DSPeed (pronounced dee-ess-speed) is a python-based package that performs bulk,
+high-performance digital signal processing (DSP) of time-series data such as
+digitized waveforms. This package is part of the
+[pygama](https://github.com/legend-exp/pygama) scientific computing suite.
+
+DSPeed enables the user to define an arbitrary chain of vectorized signal
+processing routines that can be applied in bulk to waveforms and other data
+provided using the
+[LH5-format](https://legend-exp.github.io/legend-data-format-specs). These
+routines can include [numpy
+ufuncs](https://numpy.org/doc/stable/reference/ufuncs.html), custom functions
+accelerated with [numba](https://numba.pydata.org/), or other arbitrary
+functions. DSPeed will carefully manage file I/O to optimize memory usage and
+performance. Processing chains are defined using highly portable JSON files
+that can be applied to data from multiple digitizers.
 
-DSPeed enables the user to define an arbitrary chain of vectorized signal processing routines that can be applied in bulk to waveforms and other data provided using the [LH5-format](https://legend-exp.github.io/legend-data-format-specs). These routines can include [numpy ufuncs](https://numpy.org/doc/stable/reference/ufuncs.html), custom functions accelerated with [numba](https://numba.pydata.org/), or other arbitrary functions. DSPeed will carefully manage file I/O to optimize memory usage and performance. Processing chains are defined using highly portable JSON files that can be applied to data from multiple digitizers.
+See the [online documentation](https://dspeed.readthedocs.io/en/stable/) for
+more information.
 
-See the [online documentation](https://dspeed.readthedocs.io/en/stable/) for more information!
+If you are using this software, consider
+[citing](https://doi.org/10.5281/zenodo.10684779)!
```

### Comparing `dspeed-1.3.0a5/setup.cfg` & `dspeed-1.3.0a6/setup.cfg`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/build_dsp.py` & `dspeed-1.3.0a6/src/dspeed/build_dsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 This module provides high-level routines for running signal processing chains
 on waveform data.
 """
+
 from __future__ import annotations
 
-import json
 import logging
 import os
 
 import h5py
 import numpy as np
 from lgdo import lh5
 from tqdm.auto import tqdm
+from yaml import safe_load
 
 from .errors import DSPFatal
 from .processing_chain import build_processing_chain
 
 log = logging.getLogger(__name__)
 
 
@@ -38,24 +39,24 @@
     Parameters
     ----------
     f_raw
         name of raw-tier LH5 file to read from.
     f_dsp
         name of dsp-tier LH5 file to write to.
     dsp_config
-        :class:`dict` or name of JSON file containing
+        :class:`dict` or name of JSON or YAML file containing
         :class:`~.processing_chain.ProcessingChain` config. See
         :func:`~.processing_chain.build_processing_chain` for details.
     lh5_tables
         list of LGDO groups to process in the input file. These table should
         include all input variables for processing or contain a subgroup
         called raw that contains such a table. If ``None``, process
         all valid groups. Note that wildcards are accepted (e.g. "ch*").
     database
-        dictionary or name of JSON file containing a parameter database. See
+        dictionary or name of JSON or YAMLfile containing a parameter database. See
         :func:`~.processing_chain.build_processing_chain` for details.
     outputs
         list of parameter names to write to the output file. If not provided,
         use list provided under ``"outputs"`` in the DSP configuration file.
     n_max
         number of waveforms to process.
     write_mode
@@ -64,15 +65,15 @@
         - `'a'` -- append to end of existing output file
         - `'u'` -- update values in existing output file
     buffer_len
         number of waveforms to read/write from/to disk at a time.
     block_width
         number of waveforms to process at a time.
     chan_config
-        contains JSON DSP configuration file names for every table in
+        contains JSON or YAML DSP configuration file names for every table in
         `lh5_tables`.
     """
 
     if chan_config is not None:
         # clear existing output files
         if write_mode == "r":
             if os.path.isfile(f_dsp):
@@ -127,22 +128,22 @@
             lh5_tables[i] = f"{tb}/raw"
         elif not lh5.ls(lh5_file, tb):
             del lh5_tables[i]
 
     if len(lh5_tables) == 0:
         raise RuntimeError(f"could not find any valid LH5 table in {f_raw}")
 
-    # get the database parameters. For now, this will just be a dict in a json
+    # get the database parameters. For now, this will just be a dict in a
     # file, but eventually we will want to interface with the metadata repo
     if isinstance(database, str):
         with open(lh5.utils.expand_path(database)) as db_file:
-            database = json.load(db_file)
+            database = safe_load(db_file)
 
     if database and not isinstance(database, dict):
-        raise ValueError("input database is not a valid JSON file or dict")
+        raise ValueError("input database is not a valid JSON or YAML file or dict")
 
     if write_mode is None and os.path.isfile(f_dsp):
         raise FileExistsError(
             f"output file {f_dsp} exists. Set the 'write_mode' keyword"
         )
 
     # clear existing output files
```

### Comparing `dspeed-1.3.0a5/src/dspeed/cli.py` & `dspeed-1.3.0a6/src/dspeed/cli.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/errors.py` & `dspeed-1.3.0a6/src/dspeed/errors.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/logging.py` & `dspeed-1.3.0a6/src/dspeed/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module implements some helpers for setting up logging."""
+
 import logging
 
 import colorlog
 
 DEBUG = logging.DEBUG
 INFO = logging.INFO
 WARNING = logging.WARNING
```

### Comparing `dspeed-1.3.0a5/src/dspeed/processing_chain.py` & `dspeed-1.3.0a6/src/dspeed/processing_chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """
 This module provides routines for setting up and running signal processing
 chains on waveform data.
 """
+
 from __future__ import annotations
 
 import ast
 import importlib
 import itertools as it
-import json
 import logging
 import re
 from abc import ABCMeta, abstractmethod
 from copy import deepcopy
 from dataclasses import dataclass
 from typing import Any
 
 import lgdo
 import numpy as np
 from lgdo import LGDO, lh5
 from numba import guvectorize, vectorize
 from pint import Quantity, Unit
+from yaml import dump, safe_load
 
 from .errors import DSPFatal, ProcessingChainError
 from .processors.round_to_nearest import round_to_nearest
 from .units import unit_registry as ureg
 from .utils import ProcChainVarBase
 from .utils import numba_defaults_kwargs as nb_kwargs
 
@@ -40,14 +41,19 @@
     ast.Mult: (np.multiply, "{}*{}"),
     ast.Div: (np.divide, "{}/{}"),
     ast.FloorDiv: (np.floor_divide, "{}//{}"),
     ast.USub: (np.negative, "-{}"),
 }
 
 
+# helper function to tell if an object is found in the unit registry
+def is_in_pint(unit):
+    return isinstance(unit, (Unit, Quantity)) or (unit and unit in ureg)
+
+
 @dataclass
 class CoordinateGrid:
     """Helper class that describes a system of units, consisting of a period
     and offset.
 
     `period` is a unitted :class:`pint.Quantity`, `offset` is a scalar in units
     of `period`, a :class:`pint.Unit` or a :class:`ProcChainVar`. In the last
@@ -55,18 +61,27 @@
     for each event.
     """
 
     period: Quantity | Unit | str
     offset: Quantity | ProcChainVar | float | int = 0
 
     def __post_init__(self) -> None:
-        # Copy constructor
+        # Copy constructor and conversions
         if isinstance(self.period, CoordinateGrid):
             self.offset = self.period.offset
             self.period = self.period.period
+        elif isinstance(self.period, ProcChainVar):
+            if self.period.grid in (None, auto):
+                raise ProcessingChainError(
+                    f"{self.period} does not have an assigned coordinate grid"
+                )
+            self.offset = self.period.offset
+            self.period = self.period.period
+        elif isinstance(self.period, tuple):
+            self.period, self.offset = self.period
 
         if isinstance(self.period, str):
             self.period = Quantity(1.0, self.period)
         elif isinstance(self.period, Unit):
             self.period *= 1  # make Quantity
 
         if isinstance(self.offset, (int, float)):
@@ -241,37 +256,36 @@
         if self._buffer is None:
             if self.shape is auto:
                 raise ProcessingChainError(f"cannot deduce shape of {self.name}")
             if self.dtype is auto:
                 raise ProcessingChainError(f"cannot deduce dtype of {self.name}")
             self._buffer = self._make_buffer()
 
+        # if no unit is given, use the native unit/coordinate grid
+        if unit is None:
+            unit = self.grid if self.is_coord else self.unit
+        if not isinstance(unit, CoordinateGrid) and is_in_pint(unit):
+            unit = CoordinateGrid(unit)
+
         if isinstance(self._buffer, np.ndarray):
             if self.is_coord is True:
                 if isinstance(self.grid, CoordinateGrid):
                     pass
                 elif unit is not None:
                     self.grid = CoordinateGrid(unit)
-                else:
-                    self.grid = CoordinateGrid(self.unit)
-                self._buffer = [(self._buffer, self.grid)]
-            elif self.unit is None or not (
-                isinstance(self.unit, (Unit, Quantity)) or self.unit in ureg
-            ):
+
+            if not (isinstance(unit, CoordinateGrid) or is_in_pint(unit)):
                 # buffer cannot be converted so return
                 return self._buffer
             else:
                 # buffer can be converted, so make it a list of buffers
-                self._buffer = [(self._buffer, CoordinateGrid(self.unit))]
+                self._buffer = [(self._buffer, unit)]
 
-        # if no unit is given, use the native unit
-        if unit is None:
-            unit = self.unit
-        if not isinstance(unit, CoordinateGrid) and unit in ureg:
-            unit = CoordinateGrid(unit)
+        if not isinstance(unit, CoordinateGrid) and not is_in_pint(unit):
+            return self._buffer[0][0]
 
         # check if coordinate conversion has been done already
         for buff, buf_u in self._buffer:
             if buf_u == unit:
                 return buff
 
         # If we get this far, add conversion processor to ProcChain and add new buffer to _buffer
@@ -472,28 +486,24 @@
         dtype
             dtype of constant
         unit
             unit of constant
         """
 
         param = self.get_variable(varname)
-        assert param.is_constant or param._buffer is None
-        param.is_constant = True
+        assert param.is_const or param._buffer is None
+        param.is_const = True
 
         if isinstance(val, Quantity):
             unit = val.unit
             val = val.magnitude
 
         val = np.array(val, dtype=dtype)
 
-        param.update_auto(
-            shape=val.shape,
-            dtype=val.dtype,
-            unit=unit,
-        )
+        param.update_auto(shape=val.shape, dtype=val.dtype, unit=unit, is_coord=False)
         np.copyto(param.get_buffer(), val, casting="unsafe")
         log.debug(f"set constant: {param.description()} = {val}")
         return param
 
     def link_input_buffer(
         self, varname: str, buff: np.ndarray | LGDO = None
     ) -> np.ndarray | LGDO:
@@ -651,30 +661,40 @@
 
         log.debug(f"added output buffer: {out_man}")
         self._output_managers.append(out_man)
 
         return buff
 
     def add_processor(
-        self, func: np.ufunc, *args, signature: str = None, types: list[str] = None
+        self,
+        func: np.ufunc,
+        *args,
+        signature: str = None,
+        types: list[str] = None,
+        coord_grid: tuple | str = None,
     ) -> None:
         """Make a list of parameters from `*args`. Replace any strings in the
         list with NumPy objects from `vars_dict`, where able.
         """
         params = []
         kw_params = {}
         for _, param in enumerate(args):
             if isinstance(param, str):
                 param = self.get_variable(param)
             if isinstance(param, dict):
                 kw_params.update(param)
             else:
                 params.append(param)
 
-        proc_man = ProcessorManager(self, func, params, kw_params, signature, types)
+        if coord_grid is not None:
+            coord_grid = CoordinateGrid(coord_grid)
+
+        proc_man = ProcessorManager(
+            self, func, params, kw_params, signature, types, coord_grid
+        )
         self._proc_managers.append(proc_man)
         log.debug(f"added processor: {proc_man}")
 
     def execute(self, start: int = 0, stop: int = None) -> None:
         """Execute the dsp chain on the entire input/output buffers."""
         if stop is None:
             stop = self._buffer_len
@@ -802,16 +822,35 @@
                     ret.u, ureg.dimensionless
                 ):
                     ret = ret.to(ureg.dimensionless).magnitude
                 return ret
 
             name = "(" + op_form.format(str(lhs), str(rhs)) + ")"
             if isinstance(lhs, ProcChainVar) and isinstance(rhs, ProcChainVar):
-                # TODO: handle units/coords; for now make them match lhs
-                out = ProcChainVar(self, name, is_coord=lhs.is_coord)
+                if is_in_pint(lhs.unit) and is_in_pint(rhs.unit):
+                    unit = op(Quantity(lhs.unit), Quantity(rhs.unit)).u
+                    if unit == ureg.dimensionless:
+                        unit = None
+                elif lhs.unit is not None and rhs.unit is not None:
+                    unit = op_form.format(str(lhs.unit), str(rhs.unit))
+                elif lhs.unit is not None:
+                    unit = lhs.unit
+                else:
+                    unit = rhs.unit
+                # If both vars are coordinates, this is probably not a coord.
+                # If one var is a coord, this is probably a coord
+                out = ProcChainVar(
+                    self,
+                    name,
+                    grid=None if lhs.is_coord and rhs.is_coord else auto,
+                    is_coord=(
+                        False if lhs.is_coord is True and rhs.is_coord is True else auto
+                    ),
+                    unit=unit,
+                )
             elif isinstance(lhs, ProcChainVar):
                 out = ProcChainVar(
                     self,
                     name,
                     unit=lhs.unit,
                     is_coord=lhs.is_coord,
                 )
@@ -854,15 +893,15 @@
 
             return out
 
         elif isinstance(node, ast.Subscript):
             val = self._parse_expr(node.value, expr, dry_run, var_name_list)
             if val is None:
                 return None
-            if not isinstance(val, ProcChainVar):
+            if not isinstance(val, ProcChainVar) or not len(val.shape) > 0:
                 raise ProcessingChainError("Cannot apply subscript to", node.value)
 
             def get_index(slice_value):
                 ret = self._parse_expr(slice_value, expr, dry_run, var_name_list)
                 if ret is None:
                     return ret
                 if isinstance(ret, Quantity):
@@ -872,19 +911,19 @@
                     if abs(ret - round_ret) > 0.0001:
                         log.warning(
                             f"slice value {slice_value} is non-integer. Rounding to {round_ret}"
                         )
                     return round_ret
                 return int(ret)
 
-            if isinstance(node.slice, ast.Index):
-                index = get_index(node.slice.value)
-                out_buf = val[..., index]
-                out_name = (f"{str(val)}[{index}]",)
-                out_grid = None
+            if isinstance(node.slice, ast.Constant):
+                index = get_index(node.slice)
+                out_buf = val.buffer[..., index]
+                out_name = f"{str(val)}[{index}]"
+                out_grid = val.grid if val.is_coord else None
 
             elif isinstance(node.slice, ast.Slice):
                 sl = slice(
                     get_index(node.slice.lower),
                     get_index(node.slice.upper),
                     get_index(node.slice.step),
                 )
@@ -963,15 +1002,15 @@
                 self._parse_expr(arg, expr, dry_run, var_name_list) for arg in node.args
             ]
             kwargs = {
                 kwarg.arg: self._parse_expr(kwarg.value, expr, dry_run, var_name_list)
                 for kwarg in node.keywords
             }
             if func is not None:
-                return func(*args, **kwargs)
+                return func(*args, **kwargs) if not dry_run else None
             elif self._validate_name(node.func.id):
                 var_name = node.func.id
                 var_name_list.append(var_name)
                 if var_name in self._vars_dict:
                     var = self._vars_dict[var_name]
                     var.update_auto(*args, **kwargs)
                     return self._vars_dict[var_name]
@@ -1177,14 +1216,15 @@
         self,
         proc_chain: ProcessingChain,
         func: np.ufunc,
         params: list[str],
         kw_params: dict = None,
         signature: str = None,
         types: list[str] = None,
+        grid: CoordinateGrid = None,
     ) -> None:
         assert (
             isinstance(proc_chain, ProcessingChain)
             and callable(func)
             and isinstance(params, list)
         )
 
@@ -1233,15 +1273,14 @@
                 f"expected {len(dims_list)} arguments from signature "
                 f"{self.signature}; found "
                 f"{len(params)+len(kw_params)}: ({', '.join([str(par) for par in params])})"
             )
 
         dims_dict = {}  # map from dim name -> DimInfo
         outerdims = []  # list of DimInfo
-        grid = None  # period/offset to use for unit and coordinate conversions
 
         for ipar, (dims, param) in enumerate(
             zip(dims_list, it.chain(self.params, self.kw_params.values()))
         ):
             if not isinstance(param, (ProcChainVar, np.ndarray)):
                 continue
 
@@ -1257,31 +1296,32 @@
             # fill out dimensions from dim signature and check if it works
             if param.shape is auto:
                 continue
             fun_dims = [od for od in outerdims] + [
                 d.strip() for d in dims.split(",") if d
             ]
             arr_dims = list(param.shape)
-            arr_grid = (
-                param.grid
-                if isinstance(param, ProcChainVar) and param.grid is not auto
-                else None
-            )
+            if (
+                isinstance(param, ProcChainVar)
+                and param.grid is not auto
+                and not param.is_coord
+            ):
+                arr_grid = param.grid
+            else:
+                arr_grid = None
             if not grid:
                 grid = arr_grid
 
             # check if arr_dims can be broadcast to match fun_dims
             for i in range(max(len(fun_dims), len(arr_dims))):
                 fd = fun_dims[-i - 1] if i < len(fun_dims) else None
                 ad = (
                     arr_dims[-i - 1]
                     if i < len(arr_dims)
-                    else self.proc_chain._block_width
-                    if i == len(arr_dims)
-                    else None
+                    else self.proc_chain._block_width if i == len(arr_dims) else None
                 )
 
                 if isinstance(fd, str):
                     if fd in dims_dict:
                         this_dim = dims_dict[fd]
                         if not ad or this_dim.length != ad:
                             raise ProcessingChainError(
@@ -1385,16 +1425,15 @@
                 # Deduce any automated descriptions of parameter
                 unit = None
                 is_coord = False
                 if param.is_coord is True and grid is not None:
                     unit = str(grid.period.u)
                     this_grid = grid
                 elif (
-                    isinstance(param.unit, str)
-                    and param.unit in ureg
+                    is_in_pint(param.unit)
                     and grid is not None
                     and ureg.is_compatible_with(grid.period, param.unit)
                 ):
                     is_coord = True
                     this_grid = grid
 
                 param.update_auto(
@@ -1406,15 +1445,17 @@
                 )
 
                 # reshape just in case there are some missing dimensions
                 arshape = list(param.buffer.shape)
                 for idim in range(-1, -1 - len(shape), -1):
                     if len(arshape) < -idim or arshape[idim] != shape[idim]:
                         arshape.insert(len(arshape) + idim + 1, 1)
-                param = param.get_buffer(grid).reshape(arshape)
+                param = param.get_buffer(grid if param.is_coord else None).reshape(
+                    arshape
+                )
 
             elif isinstance(param, str):
                 # Convert string into integer buffer if appropriate
                 if np.issubdtype(dtype, np.integer):
                     try:
                         param = np.frombuffer(param.encode("ascii"), dtype).reshape(
                             shape
@@ -1511,31 +1552,31 @@
         if round:
             self.processor = UnitConversionManager.convert_round
         elif issubclass(var.dtype.type, np.floating):
             self.processor = UnitConversionManager.convert
         else:
             self.processor = UnitConversionManager.convert_int
 
-        # list of parameters prior to converting to internal representation
-        self.params = [var, unit]
-        self.kw_params = {}
-
         to_offset = 0
         if isinstance(unit, CoordinateGrid):
             to_offset = unit.get_offset()
             unit = unit.period
 
         if isinstance(var._buffer, list):
             from_buffer, from_unit = var._buffer[0]
         else:
             from_buffer = var._buffer
             from_unit = var.unit
             if isinstance(from_unit, str) and from_unit in ureg:
                 from_unit = ureg.Quantity(from_unit)
 
+        # list of parameters prior to converting to internal representation
+        self.params = [var]
+        self.kw_params = {"from": from_unit, "to": unit}
+
         if isinstance(from_unit, CoordinateGrid):
             ratio = from_unit.get_period(unit)
             from_offset = from_unit.get_offset()
         elif isinstance(from_unit, (Unit, Quantity)):
             if isinstance(unit, str):
                 unit = ureg.Quantity(unit)
             ratio = float(from_unit / unit)
@@ -1693,27 +1734,36 @@
         assert isinstance(io_array, lgdo.ArrayOfEqualSizedArrays) and isinstance(
             var, ProcChainVar
         )
 
         unit = io_array.attrs.get("units", None)
         var.update_auto(dtype=io_array.dtype, shape=io_array.nda.shape[1:], unit=unit)
 
-        if isinstance(var.unit, CoordinateGrid):
+        if isinstance(var.unit, (CoordinateGrid, Quantity, Unit)):
+            if isinstance(var.unit, CoordinateGrid):
+                var_u = var.unit.period.u
+            elif isinstance(var.unit, Quantity):
+                var_u = var.unit.u
+            else:
+                var_u = var.unit
+
             if unit is None:
-                unit = var.unit.period.u
-            elif ureg.is_compatible_with(var.unit.period, unit):
+                unit = var_u
+            elif ureg.is_compatible_with(var_u, unit):
                 unit = ureg.Quantity(unit).u
             else:
                 raise ProcessingChainError(
                     f"LGDO array and variable {var} have incompatible units "
-                    f"({var.unit.period.u} and {unit})"
+                    f"({var_u} and {unit})"
                 )
+        elif isinstance(var.unit, str) and unit is None:
+            unit = var.unit
 
-        if unit is None and var.unit is not None:
-            io_array.attrs["units"] = str(var.unit)
+        if "units" not in io_array.attrs and unit is not None:
+            io_array.attrs["units"] = str(unit)
 
         self.io_array = io_array
         self.raw_buf = io_array.nda
         self.var = var
         self.raw_var = var.get_buffer(unit)
 
         if (
@@ -1753,30 +1803,37 @@
         if not np.issubdtype(var.vector_len.dtype, np.integer):
             raise ProcessingChainError(
                 f"{var.vector_len} must be an integer to act as a vector len"
             )
 
         unit = io_vov.attrs.get("units", None)
         var.update_auto(dtype=io_vov.dtype, shape=10, unit=unit)
-        if var.vector_len is None:
-            var.vector_len = (f"{var.name}_len",)
 
-        if isinstance(var.unit, CoordinateGrid):
+        if isinstance(var.unit, (CoordinateGrid, Quantity, Unit)):
+            if isinstance(var.unit, CoordinateGrid):
+                var_u = var.unit.period.u
+            elif isinstance(var.unit, Quantity):
+                var_u = var.unit.u
+            else:
+                var_u = var.unit
+
             if unit is None:
-                unit = var.unit.period.u
-            elif ureg.is_compatible_with(var.unit.period, unit):
+                unit = var_u
+            elif ureg.is_compatible_with(var_u, unit):
                 unit = ureg.Quantity(unit).u
             else:
                 raise ProcessingChainError(
                     f"LGDO array and variable {var} have incompatible units "
-                    f"({var.unit.period.u} and {unit})"
+                    f"({var_u} and {unit})"
                 )
+        elif isinstance(var.unit, str) and unit is None:
+            unit = var.unit
 
-        if unit is None and var.unit is not None:
-            io_vov.attrs["units"] = str(var.unit)
+        if "units" not in io_vov.attrs and unit is not None:
+            io_vov.attrs["units"] = str(unit)
 
         self.io_vov = io_vov
         self.raw_buf = io_vov.flattened_data
         self.cumlen_buf = io_vov.cumulative_length
         self.var = var
         self.raw_var = var.get_buffer(unit)
         self.len_var = var.vector_len.get_buffer()
@@ -1928,24 +1985,24 @@
     dsp_config: dict | str,
     db_dict: dict = None,
     outputs: list[str] = None,
     block_width: int = 16,
 ) -> tuple[ProcessingChain, list[str], lgdo.Table]:
     """Produces a :class:`ProcessingChain` object and an LH5
     :class:`~lgdo.types.table.Table` for output parameters from an input LH5
-    :class:`~lgdo.types.table.Table` and a JSON recipe.
+    :class:`~lgdo.types.table.Table` and a JSON or YAML recipe.
 
     Parameters
     ----------
     lh5_in
         HDF5 table from which raw data is read. At least one row of entries
         should be read in prior to calling this!
 
     dsp_config
-        A dictionary or JSON filename containing the recipes for computing DSP
+        A dictionary or YAML/JSON filename containing the recipes for computing DSP
         parameter from raw parameters. The format is as follows:
 
         .. code-block:: json
 
             {
                "outputs" : [ "par1", "par2" ]
                "processors" : {
@@ -2011,22 +2068,22 @@
         - `lh5_out` -- output :class:`~lgdo.table.Table` containing processed
           values
     """
     proc_chain = ProcessingChain(block_width, lh5_in.size)
 
     if isinstance(dsp_config, str):
         with open(lh5.utils.expand_path(dsp_config)) as f:
-            dsp_config = json.load(f)
+            dsp_config = safe_load(f)
     elif dsp_config is None:
         dsp_config = {"outputs": [], "processors": {}}
     elif isinstance(dsp_config, dict):
         # We don't want to modify the input!
         dsp_config = deepcopy(dsp_config)
     else:
-        raise ValueError("dsp_config must be a dict, json file, or None")
+        raise ValueError("dsp_config must be a dict, json/yaml file, or None")
 
     if outputs is None:
         outputs = dsp_config["outputs"]
 
     processors = dsp_config["processors"]
 
     # prepare the processor list
@@ -2187,30 +2244,47 @@
                     unit=fun_var.unit,
                     is_coord=fun_var.is_coord,
                 )
                 new_var._buffer = fun_var._buffer
                 log.debug(f"setting {new_var} = {fun_var}")
                 continue
 
-            module = importlib.import_module(recipe["module"])
-            func = getattr(module, recipe["function"])
+            if "module" in recipe:
+                module = importlib.import_module(recipe["module"])
+                func = getattr(module, recipe["function"])
+            else:
+                p = recipe["function"].rfind(".")
+                if p < 0:
+                    raise ProcessingChainError(
+                        f"Must provide a module for function {recipe['function']}"
+                    )
+                module = importlib.import_module(recipe["function"][:p])
+                func = getattr(module, recipe["function"][p + 1 :])
+
             args = recipe["args"]
             new_vars = [k for k in re.split(",| ", proc_par) if k != ""]
 
             # Initialize the new variables, if needed
             if "unit" in recipe:
                 for i, name in enumerate(new_vars):
                     unit = recipe.get("unit", auto)
                     if isinstance(unit, list):
                         unit = unit[i]
 
                     proc_chain.add_variable(name, unit=unit)
 
             # get this list of kwargs
             kwargs = recipe.get("kwargs", {})  # might also need db lookup here
+            kwargs.update(
+                {
+                    key: recipe[key]
+                    for key in ["signature", "types", "coord_grid"]
+                    if key in recipe
+                }
+            )
 
             # if init_args are defined, parse any strings and then call func
             # as a factory/constructor function
             try:
                 init_args_in = recipe["init_args"]
                 init_args = []
                 init_kwargs = {}
@@ -2303,16 +2377,15 @@
                         proc_chain.set_constant(var, val)
 
             else:
                 proc_chain.add_processor(func, *params, kw_params, **kwargs)
 
         except Exception as e:
             raise ProcessingChainError(
-                "Exception raised while attempting to add processor:\n"
-                + json.dumps(recipe, indent=2)
+                "Exception raised while attempting to add processor:\n" + dump(recipe)
             ) from e
 
     # build the output buffers
     lh5_out = lgdo.Table(size=proc_chain._buffer_len)
 
     # add inputs that are directly copied
     for copy_par in copy_par_list:
```

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/__init__.py` & `dspeed-1.3.0a6/src/dspeed/processors/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,22 +81,29 @@
 )
 from .multi_a_filter import multi_a_filter
 from .multi_t_filter import multi_t_filter, remove_duplicates
 from .optimize import optimize_1pz, optimize_2pz
 from .param_lookup import param_lookup
 from .peak_snr_threshold import peak_snr_threshold
 from .pole_zero import double_pole_zero, pole_zero
+from .poly_fit import poly_diff, poly_exp_rms, poly_fit
 from .presum import presum
 from .pulse_injector import inject_exp_pulse, inject_sig_pulse
+from .rc_cr2 import rc_cr2
 from .round_to_nearest import round_to_nearest
 from .saturation import saturation
 from .soft_pileup_corr import soft_pileup_corr, soft_pileup_corr_bl
 from .svm import svm_predict
 from .time_over_threshold import time_over_threshold
-from .time_point_thresh import interpolated_time_point_thresh, time_point_thresh
+from .time_point_thresh import (
+    bi_level_zero_crossing_time_points,
+    interpolated_time_point_thresh,
+    multi_time_point_thresh,
+    time_point_thresh,
+)
 from .transfer_function_convolver import transfer_function_convolver
 from .trap_filters import asym_trap_filter, trap_filter, trap_norm, trap_pickoff
 from .upsampler import interpolating_upsampler, upsampler
 from .wf_alignment import wf_alignment
 from .wiener_filter import wiener_filter
 from .windower import windower
 
@@ -114,14 +121,17 @@
     "fixed_time_pickoff",
     "gaussian_filter1d",
     "get_multi_local_extrema",
     "histogram",
     "histogram_stats",
     "linear_slope_fit",
     "linear_slope_diff",
+    "poly_diff",
+    "poly_fit",
+    "poly_exp_rms",
     "log_check",
     "min_max",
     "min_max_norm",
     "avg_current",
     "moving_window_left",
     "moving_window_multi",
     "moving_window_right",
@@ -139,14 +149,15 @@
     "saturation",
     "peak_snr_threshold",
     "soft_pileup_corr",
     "soft_pileup_corr_bl",
     "svm_predict",
     "time_point_thresh",
     "interpolated_time_point_thresh",
+    "multi_time_point_thresh",
     "asym_trap_filter",
     "trap_filter",
     "trap_norm",
     "trap_pickoff",
     "upsampler",
     "interpolating_upsampler",
     "wiener_filter",
@@ -155,8 +166,10 @@
     "dplms",
     "moving_slope",
     "step",
     "get_wf_centroid",
     "wf_alignment",
     "round_to_nearest",
     "transfer_function_convolver",
+    "rc_cr2",
+    "bi_level_zero_crossing_time_points",
 ]
```

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/bl_subtract.py` & `dspeed-1.3.0a6/src/dspeed/processors/bl_subtract.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/convolutions.py` & `dspeed-1.3.0a6/src/dspeed/processors/convolutions.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/dwt.py` & `dspeed-1.3.0a6/src/dspeed/processors/dwt.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/energy_kernels.py` & `dspeed-1.3.0a6/src/dspeed/processors/energy_kernels.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/fftw.py` & `dspeed-1.3.0a6/src/dspeed/processors/fftw.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,17 +151,19 @@
             w_out.update_auto(
                 shape=w_in.shape[:-1] + (2 * (w_in.shape[-1] - 1),),
                 dtype=np.dtype(f"f{s//2}"),
                 period=1.0 / w_in.period / w_in.shape[-1],
             )
         else:
             w_out.update_auto(
-                shape=w_in.shape
-                if w_out.dtype.kind == "c"
-                else w_in.shape[:-1] + (2 * (w_in.shape[-1] - 1),),
+                shape=(
+                    w_in.shape
+                    if w_out.dtype.kind == "c"
+                    else w_in.shape[:-1] + (2 * (w_in.shape[-1] - 1),)
+                ),
                 period=1.0 / w_in.period / w_in.shape[-1],
             )
         w_in = w_in.buffer
         w_out = w_out.buffer
 
     try:
         idft_fun = FFTW(w_in, w_out, axes=(-1,), direction="FFTW_BACKWARD")
```

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/fixed_time_pickoff.py` & `dspeed-1.3.0a6/src/dspeed/processors/fixed_time_pickoff.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/gaussian_filter1d.py` & `dspeed-1.3.0a6/src/dspeed/processors/gaussian_filter1d.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/get_multi_local_extrema.py` & `dspeed-1.3.0a6/src/dspeed/processors/get_multi_local_extrema.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/get_wf_centroid.py` & `dspeed-1.3.0a6/src/dspeed/processors/get_wf_centroid.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/histogram.py` & `dspeed-1.3.0a6/src/dspeed/processors/histogram.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/kernels.py` & `dspeed-1.3.0a6/src/dspeed/processors/kernels.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/linear_slope_fit.py` & `dspeed-1.3.0a6/src/dspeed/processors/linear_slope_fit.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/log_check.py` & `dspeed-1.3.0a6/src/dspeed/processors/log_check.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/min_max.py` & `dspeed-1.3.0a6/src/dspeed/processors/min_max.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/moving_windows.py` & `dspeed-1.3.0a6/src/dspeed/processors/moving_windows.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/multi_a_filter.py` & `dspeed-1.3.0a6/src/dspeed/processors/multi_a_filter.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/multi_t_filter.py` & `dspeed-1.3.0a6/src/dspeed/processors/multi_t_filter.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/optimize.py` & `dspeed-1.3.0a6/src/dspeed/processors/optimize.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/param_lookup.py` & `dspeed-1.3.0a6/src/dspeed/processors/param_lookup.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/peak_snr_threshold.py` & `dspeed-1.3.0a6/src/dspeed/processors/peak_snr_threshold.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/pole_zero.py` & `dspeed-1.3.0a6/src/dspeed/processors/pole_zero.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,17 +39,31 @@
     """
     w_out[:] = np.nan
 
     if np.isnan(w_in).any() or np.isnan(t_tau):
         return
 
     const = np.exp(-1 / t_tau)
+
+    # Create a buffer of float64s, because performing the recursion at float32 causes instabilities in the filter due to truncation
+    w_tmp = np.zeros(2, dtype=np.float64)
+
+    # Initialize the arrays for recursion
     w_out[0] = w_in[0]
+    w_tmp[0] = w_in[0]
+
     for i in range(1, len(w_in), 1):
-        w_out[i] = w_out[i - 1] + w_in[i] - w_in[i - 1] * const
+        w_tmp[1] = w_tmp[0] + w_in[i] - w_in[i - 1] * const
+
+        w_out[i] = w_tmp[1]  # Put the higher precision buffer into the desired output
+        w_tmp[0] = w_tmp[1]  # Shuffle the buffer for the next iteration
+
+    # Check the output
+    if np.isnan(w_out).any():
+        raise DSPFatal("Pole-zero filter produced nans in output.")
 
 
 @guvectorize(
     [
         "void(float32[:], float32, float32, float32, float32[:])",
         "void(float64[:], float64, float64, float64, float64[:])",
     ],
@@ -130,19 +144,33 @@
     b = np.exp(-1 / t_tau2)
 
     transfer_denom_1 = frac * b - frac * a - b - 1
     transfer_denom_2 = -1 * (frac * b - frac * a - b)
     transfer_num_1 = -1 * (a + b)
     transfer_num_2 = a * b
 
+    # Create a buffer of float64s, because performing the recursion at float32 causes instabilities in the filter due to truncation
+    w_tmp = np.zeros(3, dtype=np.float64)
+
+    # Initialize the arrays for recursion
+    w_tmp[0] = w_in[0]
+    w_tmp[1] = w_in[1]
+
     w_out[0] = w_in[0]
     w_out[1] = w_in[1]
-    w_out[2] = w_in[2]
 
     for i in range(2, len(w_in), 1):
-        w_out[i] = (
+        w_tmp[2] = (
             w_in[i]
             + transfer_num_1 * w_in[i - 1]
             + transfer_num_2 * w_in[i - 2]
-            - transfer_denom_1 * w_out[i - 1]
-            - transfer_denom_2 * w_out[i - 2]
+            - transfer_denom_1 * w_tmp[1]
+            - transfer_denom_2 * w_tmp[0]
         )
+
+        w_out[i] = w_tmp[2]  # Put the higher precision buffer into the desired output
+        # Shuffle the buffer for the next iteration
+        w_tmp[0] = w_tmp[1]
+        w_tmp[1] = w_tmp[2]
+    # Check the output
+    if np.isnan(w_out).any():
+        raise DSPFatal("Double-pole-zero filter produced nans in output.")
```

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/presum.py` & `dspeed-1.3.0a6/src/dspeed/processors/presum.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/pulse_injector.py` & `dspeed-1.3.0a6/src/dspeed/processors/pulse_injector.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/round_to_nearest.py` & `dspeed-1.3.0a6/src/dspeed/processors/round_to_nearest.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/saturation.py` & `dspeed-1.3.0a6/src/dspeed/processors/saturation.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/soft_pileup_corr.py` & `dspeed-1.3.0a6/src/dspeed/processors/soft_pileup_corr.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/svm.py` & `dspeed-1.3.0a6/src/dspeed/processors/svm.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,16 +37,19 @@
             "args": ["dwt_norm", "svm_label"],
             "unit": "",
             "prereqs": ["dwt_norm"],
             "init_args": ["'svm_p*_r*_T***Z.sav'"]
         }
     """
 
-    with open(svm_file, "rb") as f:
-        svm = pickle.load(f)
+    if svm_file == 0:
+        svm = None
+    else:
+        with open(svm_file, "rb") as f:
+            svm = pickle.load(f)
 
     @guvectorize(
         [
             "void(float32[:], float32[:])",
             "void(float64[:], float64[:])",
         ],
         "(n),()",
@@ -61,13 +64,19 @@
         w_in
            The input waveform (has to be a max_min normalized discrete wavelet transform)
         label_out
            The predicted label by the trained SVM for the input waveform.
         """
         label_out[0] = np.nan
 
+        if svm is None:
+            return
+
+        if np.isnan(w_in).any():
+            return
+
         if w_in.ndim == 1:
             label_out[0] = svm.predict(w_in.reshape(1, -1))
         else:
             label_out[0] = svm.predict(w_in)
 
     return svm_out
```

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/time_over_threshold.py` & `dspeed-1.3.0a6/src/dspeed/processors/time_over_threshold.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/transfer_function_convolver.py` & `dspeed-1.3.0a6/src/dspeed/processors/transfer_function_convolver.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/trap_filters.py` & `dspeed-1.3.0a6/src/dspeed/processors/trap_filters.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/upsampler.py` & `dspeed-1.3.0a6/src/dspeed/processors/upsampler.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/wf_alignment.py` & `dspeed-1.3.0a6/src/dspeed/processors/wf_alignment.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/wiener_filter.py` & `dspeed-1.3.0a6/src/dspeed/processors/wiener_filter.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/processors/windower.py` & `dspeed-1.3.0a6/src/dspeed/processors/windower.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/src/dspeed/utils.py` & `dspeed-1.3.0a6/src/dspeed/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,8 +82,9 @@
 
 class ProcChainVarBase(metaclass=ABCMeta):
     r"""Base class.
 
     :class:`ProcChainVar` implements this class. This base class is used
     by processors that use ProcChainVar in their constructors.
     """
+
     pass
```

### Comparing `dspeed-1.3.0a5/src/dspeed/vis/waveform_browser.py` & `dspeed-1.3.0a6/src/dspeed/vis/waveform_browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,18 +418,20 @@
                 x = np.linspace(t0, t0 + dt * (data.wf_len - 1), data.wf_len)
                 lines.append(Line2D(x, y))
                 self._update_auto_limit(x, y)
 
             elif isinstance(
                 data, (lgdo.Array, lgdo.ArrayOfEqualSizedArrays, lgdo.VectorOfVectors)
             ):
-                if isinstance(data, lgdo.Array):
-                    vals = [data.nda[i_tb]]
+                if isinstance(
+                    data, (lgdo.ArrayOfEqualSizedArrays, lgdo.VectorOfVectors)
+                ):
+                    vals = list(data.nda[i_tb])
                 else:
-                    vals = data[i_tb]
+                    vals = [data.nda[i_tb]]
 
                 unit = data.attrs.get("units", None)
                 if unit and unit in ureg and ureg.is_compatible_with(unit, self.x_unit):
                     # Vertical line
                     for val in vals:
                         val = np.array(
                             [val * float(ureg(unit) / self.x_unit) - ref_time]
```

### Comparing `dspeed-1.3.0a5/src/dspeed.egg-info/PKG-INFO` & `dspeed-1.3.0a6/src/dspeed.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspeed
-Version: 1.3.0a5
+Version: 1.3.0a6
 Summary: Fast Digital Signal Processing for particle detectors in Python
 Home-page: https://github.com/legend-exp/dspeed
 Author: Ian Guinn
 Author-email: guinnis@ornl.gov
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
@@ -52,35 +52,54 @@
 Provides-Extra: test
 Requires-Dist: pre-commit; extra == "test"
 Requires-Dist: pylegendtestdata; extra == "test"
 Requires-Dist: pytest>=6.0; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: scipy; extra == "test"
 
+# DSPeed
+
 ```
 _____  _________________________________________________________________
      ||                  ____  _____  ____                   __          `,_
      ||                 / __ \/ ___/ / __ \ ___   ___   ____/ /           | `-_
  []  ||  [] [] [] []   / / / /\__ \ / /_/ // _ \ / _ \ / __  /  [] [] []  '-----`-,_
  ====||===============/ /_/ /___/ // ____//  __//  __// /_/ /====================== ``--,_
      ||              /_____//____//_/     \___/ \___/ \__,_/                              ``--,
      ||    ________                                                        ________            )
 \____||___/.-.  .-.\______________________________________________________/.-.  .-.\______,,--'
 ==========='-'=='-'========================================================'-'=='-'=============
 ```
+
 [![PyPI](https://img.shields.io/pypi/v/dspeed?logo=pypi)](https://pypi.org/project/dspeed/)
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/legend-exp/dspeed?logo=git)
 [![GitHub Workflow Status](https://img.shields.io/github/checks-status/legend-exp/dspeed/main?label=main%20branch&logo=github)](https://github.com/legend-exp/dspeed/actions)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Codecov](https://img.shields.io/codecov/c/github/legend-exp/dspeed?logo=codecov)](https://app.codecov.io/gh/legend-exp/dspeed)
 ![GitHub issues](https://img.shields.io/github/issues/legend-exp/dspeed?logo=github)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/legend-exp/dspeed?logo=github)
 ![License](https://img.shields.io/github/license/legend-exp/dspeed)
 [![Read the Docs](https://img.shields.io/readthedocs/dspeed?logo=readthedocs)](https://dspeed.readthedocs.io)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10684779.svg)](https://doi.org/10.5281/zenodo.10684779)
 
-# DSPeed
-DSPeed (pronounced dee-ess-speed) is a python-based package that performs bulk, high-performance digital signal processing (DSP) of time-series data such as digitized waveforms. This package is part of the [pygama](https://github.com/legend-exp/pygama) scientific computing suite.
+DSPeed (pronounced dee-ess-speed) is a python-based package that performs bulk,
+high-performance digital signal processing (DSP) of time-series data such as
+digitized waveforms. This package is part of the
+[pygama](https://github.com/legend-exp/pygama) scientific computing suite.
+
+DSPeed enables the user to define an arbitrary chain of vectorized signal
+processing routines that can be applied in bulk to waveforms and other data
+provided using the
+[LH5-format](https://legend-exp.github.io/legend-data-format-specs). These
+routines can include [numpy
+ufuncs](https://numpy.org/doc/stable/reference/ufuncs.html), custom functions
+accelerated with [numba](https://numba.pydata.org/), or other arbitrary
+functions. DSPeed will carefully manage file I/O to optimize memory usage and
+performance. Processing chains are defined using highly portable JSON files
+that can be applied to data from multiple digitizers.
 
-DSPeed enables the user to define an arbitrary chain of vectorized signal processing routines that can be applied in bulk to waveforms and other data provided using the [LH5-format](https://legend-exp.github.io/legend-data-format-specs). These routines can include [numpy ufuncs](https://numpy.org/doc/stable/reference/ufuncs.html), custom functions accelerated with [numba](https://numba.pydata.org/), or other arbitrary functions. DSPeed will carefully manage file I/O to optimize memory usage and performance. Processing chains are defined using highly portable JSON files that can be applied to data from multiple digitizers.
+See the [online documentation](https://dspeed.readthedocs.io/en/stable/) for
+more information.
 
-See the [online documentation](https://dspeed.readthedocs.io/en/stable/) for more information!
+If you are using this software, consider
+[citing](https://doi.org/10.5281/zenodo.10684779)!
```

### Comparing `dspeed-1.3.0a5/src/dspeed.egg-info/SOURCES.txt` & `dspeed-1.3.0a6/src/dspeed.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -37,16 +37,18 @@
 src/dspeed/processors/moving_windows.py
 src/dspeed/processors/multi_a_filter.py
 src/dspeed/processors/multi_t_filter.py
 src/dspeed/processors/optimize.py
 src/dspeed/processors/param_lookup.py
 src/dspeed/processors/peak_snr_threshold.py
 src/dspeed/processors/pole_zero.py
+src/dspeed/processors/poly_fit.py
 src/dspeed/processors/presum.py
 src/dspeed/processors/pulse_injector.py
+src/dspeed/processors/rc_cr2.py
 src/dspeed/processors/round_to_nearest.py
 src/dspeed/processors/saturation.py
 src/dspeed/processors/soft_pileup_corr.py
 src/dspeed/processors/svm.py
 src/dspeed/processors/time_over_threshold.py
 src/dspeed/processors/time_point_thresh.py
 src/dspeed/processors/transfer_function_convolver.py
@@ -61,25 +63,28 @@
 tests/test_build_dsp.py
 tests/test_cli.py
 tests/test_list_parsing.py
 tests/test_numpy_constants_parsing.py
 tests/test_processing_chain.py
 tests/test_utils.py
 tests/configs/icpc-dsp-config.json
+tests/configs/icpc-dsp-config.yaml
 tests/configs/numpy-parsing.json
 tests/configs/sipm-dplms-config.json
 tests/configs/sipm-dsp-config.json
 tests/processors/dplms_noise_mat.dat
 tests/processors/test_dplms.py
 tests/processors/test_dwt.py
 tests/processors/test_fftw.py
 tests/processors/test_fixed_time_pickoff.py
 tests/processors/test_get_multi_local_extrema.py
 tests/processors/test_get_wf_centroid.py
 tests/processors/test_histogram.py
 tests/processors/test_import.py
 tests/processors/test_min_max_norm.py
+tests/processors/test_pole_zero.py
+tests/processors/test_rc_cr2.py
 tests/processors/test_time_point_thresh.py
 tests/processors/test_transfer_function_convolver.py
 tests/processors/test_wf_alignment.py
 tests/vis/test_waveform_browser.py
 tests/vis/configs/hpge-dsp-config.json
```

### Comparing `dspeed-1.3.0a5/tests/configs/icpc-dsp-config.json` & `dspeed-1.3.0a6/tests/configs/icpc-dsp-config.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/configs/numpy-parsing.json` & `dspeed-1.3.0a6/tests/configs/numpy-parsing.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/configs/sipm-dplms-config.json` & `dspeed-1.3.0a6/tests/configs/sipm-dplms-config.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/configs/sipm-dsp-config.json` & `dspeed-1.3.0a6/tests/configs/sipm-dsp-config.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/conftest.py` & `dspeed-1.3.0a6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/processors/dplms_noise_mat.dat` & `dspeed-1.3.0a6/tests/processors/dplms_noise_mat.dat`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/processors/test_dplms.py` & `dspeed-1.3.0a6/tests/processors/test_dplms.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/processors/test_dwt.py` & `dspeed-1.3.0a6/tests/processors/test_dwt.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/processors/test_fftw.py` & `dspeed-1.3.0a6/tests/processors/test_fftw.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/processors/test_fixed_time_pickoff.py` & `dspeed-1.3.0a6/tests/processors/test_fixed_time_pickoff.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/processors/test_get_multi_local_extrema.py` & `dspeed-1.3.0a6/tests/processors/test_get_multi_local_extrema.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/processors/test_get_wf_centroid.py` & `dspeed-1.3.0a6/tests/processors/test_get_wf_centroid.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/processors/test_histogram.py` & `dspeed-1.3.0a6/tests/processors/test_histogram.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/processors/test_min_max_norm.py` & `dspeed-1.3.0a6/tests/processors/test_min_max_norm.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/processors/test_transfer_function_convolver.py` & `dspeed-1.3.0a6/tests/processors/test_transfer_function_convolver.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/processors/test_wf_alignment.py` & `dspeed-1.3.0a6/tests/processors/test_wf_alignment.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/test_build_dsp.py` & `dspeed-1.3.0a6/tests/test_build_dsp.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,26 +6,38 @@
 from lgdo.lh5 import LH5Store, ls
 
 from dspeed import build_dsp
 
 config_dir = Path(__file__).parent / "configs"
 
 
-def test_build_dsp_basics(lgnd_test_data, tmptestdir):
+def test_build_dsp_json(lgnd_test_data, tmptestdir):
     out_name = f"{tmptestdir}/LDQTA_r117_20200110T105115Z_cal_geds_dsp.lh5"
     build_dsp(
         lgnd_test_data.get_path("lh5/LDQTA_r117_20200110T105115Z_cal_geds_raw.lh5"),
         out_name,
         dsp_config=f"{config_dir}/icpc-dsp-config.json",
         database={"pz": {"tau": 27460.5}},
         write_mode="r",
     )
     assert os.path.exists(out_name)
 
 
+def test_build_dsp_yaml(lgnd_test_data, tmptestdir):
+    out_name = f"{tmptestdir}/LDQTA_r117_20200110T105115Z_cal_geds_dsp.lh5"
+    build_dsp(
+        lgnd_test_data.get_path("lh5/LDQTA_r117_20200110T105115Z_cal_geds_raw.lh5"),
+        out_name,
+        dsp_config=f"{config_dir}/icpc-dsp-config.yaml",
+        database={"pz": {"tau": 27460.5}},
+        write_mode="r",
+    )
+    assert os.path.exists(out_name)
+
+
 def test_build_dsp_errors(lgnd_test_data, tmptestdir):
     with pytest.raises(FileExistsError):
         build_dsp(
             lgnd_test_data.get_path("lh5/LDQTA_r117_20200110T105115Z_cal_geds_raw.lh5"),
             f"{tmptestdir}/LDQTA_r117_20200110T105115Z_cal_geds_dsp.lh5",
             dsp_config=f"{config_dir}/icpc-dsp-config.json",
         )
```

### Comparing `dspeed-1.3.0a5/tests/test_cli.py` & `dspeed-1.3.0a6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/test_list_parsing.py` & `dspeed-1.3.0a6/tests/test_list_parsing.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/test_numpy_constants_parsing.py` & `dspeed-1.3.0a6/tests/test_numpy_constants_parsing.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/test_processing_chain.py` & `dspeed-1.3.0a6/tests/test_processing_chain.py`

 * *Files 11% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
 
 # Test that timing variables can be converted between multiple coordinate
 # grids correctly. Also tests slicing with a stride. Pickoff a time from
 # a windowed wf and a down-sampled waveform; they should be the same
 def test_proc_chain_coordinate_grid(spms_raw_tbl):
     dsp_config = {
-        "outputs": ["a_window", "a_downsample"],
+        "outputs": ["a_window", "a_downsample", "tp", "tp_window", "tp_downsample"],
         "processors": {
             "a_window": {
                 "function": "fixed_time_pickoff",
                 "module": "dspeed.processors",
                 "args": [
                     "waveform[2625:4025]",
                     "51.2*us + waveform.offset",
@@ -177,20 +177,52 @@
                     "waveform[0:8000:8]",
                     "51.2*us + waveform.offset",
                     "'i'",
                     "a_downsample",
                 ],
                 "unit": ["ADC"],
             },
+            "tp": {
+                "function": "time_point_thresh",
+                "module": "dspeed.processors",
+                "args": ["waveform", "a_window", "52.48*us+waveform.offset", 0, "tp"],
+                "unit": "ns",
+            },
+            "tp_window": {
+                "function": "time_point_thresh",
+                "module": "dspeed.processors",
+                "args": [
+                    "waveform[2625:4025]",
+                    "a_window",
+                    "52.48*us+waveform.offset",
+                    0,
+                    "tp_window",
+                ],
+                "unit": "ns",
+            },
+            "tp_downsample": {
+                "function": "time_point_thresh",
+                "module": "dspeed.processors",
+                "args": [
+                    "waveform[0:8000:8]",
+                    "a_window",
+                    "52.48*us+waveform.offset",
+                    0,
+                    "tp_downsample",
+                ],
+                "unit": "ns",
+            },
         },
     }
 
     proc_chain, _, lh5_out = build_processing_chain(spms_raw_tbl, dsp_config)
     proc_chain.execute(0, 1)
     assert lh5_out["a_window"][0] == lh5_out["a_downsample"][0]
+    assert lh5_out["tp_window"][0] == lh5_out["tp"][0]
+    assert -128 < lh5_out["tp_downsample"][0] - lh5_out["tp"][0] < 128
 
 
 def test_proc_chain_round(spms_raw_tbl):
     dsp_config = {
         "outputs": ["waveform_round"],
         "processors": {"waveform_round": "round(waveform, 4)"},
     }
```

### Comparing `dspeed-1.3.0a5/tests/vis/configs/hpge-dsp-config.json` & `dspeed-1.3.0a6/tests/vis/configs/hpge-dsp-config.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a5/tests/vis/test_waveform_browser.py` & `dspeed-1.3.0a6/tests/vis/test_waveform_browser.py`

 * *Files identical despite different names*

