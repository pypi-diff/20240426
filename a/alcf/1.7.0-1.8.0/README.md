# Comparing `tmp/alcf-1.7.0.tar.gz` & `tmp/alcf-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alcf-1.7.0.tar", last modified: Mon Apr  8 13:07:21 2024, max compression
+gzip compressed data, was "alcf-1.8.0.tar", last modified: Fri Apr 26 20:04:19 2024, max compression
```

## Comparing `alcf-1.7.0.tar` & `alcf-1.8.0.tar`

### file list

```diff
@@ -1,197 +1,203 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.983892 alcf-1.7.0/
--rw-r--r--   0 peter     (1000) peter     (1000)      239 2024-04-08 13:01:39.000000 alcf-1.7.0/.editorconfig
--rw-r--r--   0 peter     (1000) peter     (1000)     1144 2024-04-08 13:01:39.000000 alcf-1.7.0/LICENSE.md
--rw-r--r--   0 peter     (1000) peter     (1000)      181 2024-04-08 13:01:39.000000 alcf-1.7.0/MANIFEST.in
--rw-r--r--   0 peter     (1000) peter     (1000)     1275 2024-04-08 13:01:39.000000 alcf-1.7.0/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)     1002 2024-04-08 13:07:21.983892 alcf-1.7.0/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      764 2024-04-08 13:01:39.000000 alcf-1.7.0/README.md
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.963892 alcf-1.7.0/alcf/
--rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.963892 alcf-1.7.0/alcf/algorithms/
--rw-r--r--   0 peter     (1000) peter     (1000)       27 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.963892 alcf-1.7.0/alcf/algorithms/calibration/
--rw-r--r--   0 peter     (1000) peter     (1000)       62 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/calibration/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      373 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/calibration/default.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.967893 alcf-1.7.0/alcf/algorithms/cloud_base_detection/
--rw-r--r--   0 peter     (1000) peter     (1000)       71 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/cloud_base_detection/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      930 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/cloud_base_detection/default.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.967893 alcf-1.7.0/alcf/algorithms/cloud_detection/
--rw-r--r--   0 peter     (1000) peter     (1000)       66 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/cloud_detection/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1533 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/cloud_detection/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1871 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/couple.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1018 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/interp.pyx
--rw-r--r--   0 peter     (1000) peter     (1000)      781 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/lidar_ratio.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.967893 alcf-1.7.0/alcf/algorithms/noise_removal/
--rw-r--r--   0 peter     (1000) peter     (1000)       64 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/noise_removal/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1366 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/noise_removal/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1812 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/output_sample.py
--rw-r--r--   0 peter     (1000) peter     (1000)    10602 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/stats.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1196 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/tsample.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1365 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/zsample.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.967893 alcf-1.7.0/alcf/bin/
--rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/bin/__init__.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)      319 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/bin/alcf.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.967893 alcf-1.7.0/alcf/cmds/
--rw-r--r--   0 peter     (1000) peter     (1000)      408 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3658 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/auto.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.967893 alcf-1.7.0/alcf/cmds/auto_cmds/
--rw-r--r--   0 peter     (1000) peter     (1000)      141 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/auto_cmds/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      843 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/auto_cmds/compare.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1671 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/auto_cmds/lidar.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1086 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/auto_cmds/model.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2804 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/calibrate.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2148 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/compare.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4512 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/convert.py
--rw-r--r--   0 peter     (1000) peter     (1000)    12355 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/lidar.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1395 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/main.py
--rw-r--r--   0 peter     (1000) peter     (1000)     9347 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/model.py
--rw-r--r--   0 peter     (1000) peter     (1000)    18068 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/plot.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6424 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/simulate.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4939 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/stats.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.967893 alcf-1.7.0/alcf/fonts/
--rw-r--r--   0 peter     (1000) peter     (1000)     6709 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/fonts/LICENSE.md
--rw-r--r--   0 peter     (1000) peter     (1000)    56032 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/fonts/PublicSans-Bold.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    60100 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/fonts/PublicSans-BoldItalic.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    60316 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/fonts/PublicSans-Italic.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    56792 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/fonts/PublicSans-Regular.otf
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.971892 alcf-1.7.0/alcf/lidars/
--rw-r--r--   0 peter     (1000) peter     (1000)     1426 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2181 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/blview.py
--rw-r--r--   0 peter     (1000) peter     (1000)      101 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/caliop.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1742 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/chm15k.py
--rw-r--r--   0 peter     (1000) peter     (1000)      410 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/cl31.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2278 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/cl51.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1865 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/cl61.py
--rw-r--r--   0 peter     (1000) peter     (1000)      985 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3545 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/mpl.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2195 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/mpl2nc.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4659 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/misc.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.971892 alcf-1.7.0/alcf/models/
--rw-r--r--   0 peter     (1000) peter     (1000)     2235 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4179 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/amps.py
--rw-r--r--   0 peter     (1000) peter     (1000)      359 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/cmip5.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2577 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/era5.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2521 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/icon.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1783 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/icon_intake_healpix.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2559 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/jra55.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1650 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/merra2.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1854 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/nzcsm.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2939 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/nzesm.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2181 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/um.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.963892 alcf-1.7.0/alcf.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)     1002 2024-04-08 13:07:21.000000 alcf-1.7.0/alcf.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)     4562 2024-04-08 13:07:21.000000 alcf-1.7.0/alcf.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-04-08 13:07:21.000000 alcf-1.7.0/alcf.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       52 2024-04-08 13:07:21.000000 alcf-1.7.0/alcf.egg-info/entry_points.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-04-08 13:07:21.000000 alcf-1.7.0/alcf.egg-info/not-zip-safe
--rw-r--r--   0 peter     (1000) peter     (1000)      173 2024-04-08 13:07:21.000000 alcf-1.7.0/alcf.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        5 2024-04-08 13:07:21.000000 alcf-1.7.0/alcf.egg-info/top_level.txt
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1677 2024-04-08 13:01:39.000000 alcf-1.7.0/build_doc
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.975892 alcf-1.7.0/cosp/
--rw-r--r--   0 peter     (1000) peter     (1000)      260 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/.editorconfig
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.975892 alcf-1.7.0/cosp/MISR_simulator/
--rw-r--r--   0 peter     (1000) peter     (1000)    16546 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/MISR_simulator/MISR_simulator.f
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.975892 alcf-1.7.0/cosp/MODIS_simulator/
--rw-r--r--   0 peter     (1000) peter     (1000)    64835 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/MODIS_simulator/modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     7387 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/MODIS_simulator/test_modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5167 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)     7506 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/Makefile.cmor1
--rw-r--r--   0 peter     (1000) peter     (1000)     7515 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/Makefile.ibm
--rw-r--r--   0 peter     (1000) peter     (1000)      936 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/README.md
--rw-r--r--   0 peter     (1000) peter     (1000)    48320 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/README.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      467 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/README_v1.4.1.txt
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.975892 alcf-1.7.0/cosp/actsim/
--rw-r--r--   0 peter     (1000) peter     (1000)    35248 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/actsim/lidar_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    38101 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/actsim/lmd_ipsl_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11672 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/actsim/mie_backscatter_1064.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11571 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/actsim/mie_backscatter_532.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11642 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/actsim/mie_backscatter_910.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.975892 alcf-1.7.0/cosp/cfmip2/
--rw-r--r--   0 peter     (1000) peter     (1000)     2508 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     2487 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     7271 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     7400 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     3320 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     3261 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    31979 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    15220 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_constants.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     1881 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_defs.h
--rw-r--r--   0 peter     (1000) peter     (1000)     2644 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_htfrtc.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     6934 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_input_nl.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    40704 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_io.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     4292 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_isccp_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     4123 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_lidar.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     3561 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_misr_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    25019 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     3646 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_output_nl.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    26091 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_rttov.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5694 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_rttov_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     9657 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    13744 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    70109 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_types.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    13287 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_utils.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.979892 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/
--rw-r--r--   0 peter     (1000) peter     (1000)     2957 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)    59127 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/README
--rw-r--r--   0 peter     (1000) peter     (1000)      165 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/congvec.expected
--rw-r--r--   0 peter     (1000) peter     (1000)     2545 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/congvec.f
--rw-r--r--   0 peter     (1000) peter     (1000)    43978 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/icarus.f
--rw-r--r--   0 peter     (1000) peter     (1000)      869 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/input.data
--rw-r--r--   0 peter     (1000) peter     (1000)     1042 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/input.data.halved
--rw-r--r--   0 peter     (1000) peter     (1000)    13495 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f
--rw-r--r--   0 peter     (1000) peter     (1000)     1845 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/license
--rwxr-xr-x   0 peter     (1000) peter     (1000)       15 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/rcsid
--rw-r--r--   0 peter     (1000) peter     (1000)    11849 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/scops.f
--rw-r--r--   0 peter     (1000) peter     (1000)     2539 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/test_congvec.f
--rwxr-xr-x   0 peter     (1000) peter     (1000)     2660 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh
--rw-r--r--   0 peter     (1000) peter     (1000)    13385 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f
--rwxr-xr-x   0 peter     (1000) peter     (1000)     3095 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.979892 alcf-1.7.0/cosp/llnl/
--rw-r--r--   0 peter     (1000) peter     (1000)     7918 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/llnl/cosp_radar.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     6082 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/llnl/llnl_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5703 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/llnl/pf_to_mr.f
--rw-r--r--   0 peter     (1000) peter     (1000)     9585 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/llnl/prec_scops.f
--rw-r--r--   0 peter     (1000) peter     (1000)    75040 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/mac_info.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     1317 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/predict_mom07.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.979892 alcf-1.7.0/cosp/quickbeam/
--rw-r--r--   0 peter     (1000) peter     (1000)     1563 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/README
--rw-r--r--   0 peter     (1000) peter     (1000)     4166 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/array_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     5500 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/atmos_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     7260 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/calc_Re.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    10671 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/dsd.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4282 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/format_input.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     7774 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/gases.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     1665 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/load_hydrometeor_classes.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     1761 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/load_mie_table.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     9299 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/math_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    17248 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/mrgrnk.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    36058 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/optics_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4211 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/predict_psd07.f
--rw-r--r--   0 peter     (1000) peter     (1000)    18284 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/radar_simulator.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4867 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/radar_simulator_init.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     2934 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/radar_simulator_types.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4039 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/scale_LUTs_io.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4852 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/zeff.f90
--rwxr-xr-x   0 peter     (1000) peter     (1000)      143 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/replace_tabs.sh
--rwxr-xr-x   0 peter     (1000) peter     (1000)      196 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/tests.sh
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.979892 alcf-1.7.0/cosp/utils/
--rwxr-xr-x   0 peter     (1000) peter     (1000)     8682 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/utils/COSP_plots.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)     3379 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/utils/append_cf3hr_files.sh
--rwxr-xr-x   0 peter     (1000) peter     (1000)      333 2024-04-08 13:01:39.000000 alcf-1.7.0/download_cosp
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.983892 alcf-1.7.0/man/
--rw-r--r--   0 peter     (1000) peter     (1000)     4228 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf-auto.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2261 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf-calibrate.1
--rw-r--r--   0 peter     (1000) peter     (1000)      792 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf-compare.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2289 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf-convert.1
--rw-r--r--   0 peter     (1000) peter     (1000)     7003 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf-lidar.1
--rw-r--r--   0 peter     (1000) peter     (1000)     4711 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf-model.1
--rw-r--r--   0 peter     (1000) peter     (1000)     5415 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf-plot.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1962 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf-simulate.1
--rw-r--r--   0 peter     (1000) peter     (1000)     3925 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf-stats.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1390 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf.1
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2024-04-08 13:07:21.983892 alcf-1.7.0/setup.cfg
--rwxr-xr-x   0 peter     (1000) peter     (1000)     2220 2024-04-08 13:01:39.000000 alcf-1.7.0/setup.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.983892 alcf-1.7.0/src/
--rw-r--r--   0 peter     (1000) peter     (1000)    12585 2024-04-08 13:01:39.000000 alcf-1.7.0/src/cosp_run.f03
--rw-r--r--   0 peter     (1000) peter     (1000)    11128 2024-04-08 13:01:39.000000 alcf-1.7.0/src/main.f03
--rw-r--r--   0 peter     (1000) peter     (1000)     8501 2024-04-08 13:01:39.000000 alcf-1.7.0/src/nc_utils.f03
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.778815 alcf-1.8.0/
+-rw-r--r--   0 peter     (1000) peter     (1000)      239 2024-04-26 20:00:50.000000 alcf-1.8.0/.editorconfig
+-rw-r--r--   0 peter     (1000) peter     (1000)     1144 2024-04-26 20:00:50.000000 alcf-1.8.0/LICENSE.md
+-rw-r--r--   0 peter     (1000) peter     (1000)      181 2024-04-26 20:00:50.000000 alcf-1.8.0/MANIFEST.in
+-rw-r--r--   0 peter     (1000) peter     (1000)     1275 2024-04-26 20:00:50.000000 alcf-1.8.0/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)     1002 2024-04-26 20:04:19.778815 alcf-1.8.0/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)      764 2024-04-26 20:00:50.000000 alcf-1.8.0/README.md
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.754815 alcf-1.8.0/alcf/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.758815 alcf-1.8.0/alcf/algorithms/
+-rw-r--r--   0 peter     (1000) peter     (1000)       27 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/algorithms/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.758815 alcf-1.8.0/alcf/algorithms/calibration/
+-rw-r--r--   0 peter     (1000) peter     (1000)       62 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/algorithms/calibration/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      373 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/algorithms/calibration/default.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.758815 alcf-1.8.0/alcf/algorithms/cloud_base_detection/
+-rw-r--r--   0 peter     (1000) peter     (1000)       71 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/algorithms/cloud_base_detection/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      930 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/algorithms/cloud_base_detection/default.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.758815 alcf-1.8.0/alcf/algorithms/cloud_detection/
+-rw-r--r--   0 peter     (1000) peter     (1000)       66 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/algorithms/cloud_detection/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1533 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/algorithms/cloud_detection/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1871 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/algorithms/couple.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1018 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/algorithms/interp.pyx
+-rw-r--r--   0 peter     (1000) peter     (1000)      818 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/algorithms/lidar_ratio.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.758815 alcf-1.8.0/alcf/algorithms/noise_removal/
+-rw-r--r--   0 peter     (1000) peter     (1000)       64 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/algorithms/noise_removal/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1366 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/algorithms/noise_removal/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1812 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/algorithms/output_sample.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    11176 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/algorithms/stats.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1196 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/algorithms/tsample.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1365 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/algorithms/zsample.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.758815 alcf-1.8.0/alcf/bin/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/bin/__init__.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      319 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/bin/alcf.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.758815 alcf-1.8.0/alcf/cmds/
+-rw-r--r--   0 peter     (1000) peter     (1000)      458 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/cmds/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4022 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/cmds/auto.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.762815 alcf-1.8.0/alcf/cmds/auto_cmds/
+-rw-r--r--   0 peter     (1000) peter     (1000)      141 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/cmds/auto_cmds/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      843 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/cmds/auto_cmds/compare.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2639 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/cmds/auto_cmds/lidar.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1086 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/cmds/auto_cmds/model.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2804 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/cmds/calibrate.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2148 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/cmds/compare.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4512 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/cmds/convert.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6399 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/cmds/download.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    12355 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/cmds/lidar.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1430 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/cmds/main.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     7307 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/cmds/model.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    18510 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/cmds/plot.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6424 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/cmds/simulate.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4947 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/cmds/stats.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.762815 alcf-1.8.0/alcf/download/
+-rw-r--r--   0 peter     (1000) peter     (1000)       88 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/download/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2445 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/download/era5.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2444 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/download/merra2.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.762815 alcf-1.8.0/alcf/fonts/
+-rw-r--r--   0 peter     (1000) peter     (1000)     6709 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/fonts/LICENSE.md
+-rw-r--r--   0 peter     (1000) peter     (1000)    56032 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/fonts/PublicSans-Bold.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    60100 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/fonts/PublicSans-BoldItalic.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    60316 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/fonts/PublicSans-Italic.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    56792 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/fonts/PublicSans-Regular.otf
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.762815 alcf-1.8.0/alcf/lidars/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1426 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/lidars/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2181 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/lidars/blview.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      101 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/lidars/caliop.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1742 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/lidars/chm15k.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      410 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/lidars/cl31.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2278 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/lidars/cl51.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1865 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/lidars/cl61.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      985 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/lidars/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3545 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/lidars/mpl.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2195 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/lidars/mpl2nc.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6862 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/misc.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.766815 alcf-1.8.0/alcf/models/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2235 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/models/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4179 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/models/amps.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      359 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/models/cmip5.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2674 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/models/era5.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2521 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/models/icon.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1783 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/models/icon_intake_healpix.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2559 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/models/jra55.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1650 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/models/merra2.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1854 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/models/nzcsm.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2939 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/models/nzesm.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2181 2024-04-26 20:00:50.000000 alcf-1.8.0/alcf/models/um.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.754815 alcf-1.8.0/alcf.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1002 2024-04-26 20:04:19.000000 alcf-1.8.0/alcf.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     4676 2024-04-26 20:04:19.000000 alcf-1.8.0/alcf.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-04-26 20:04:19.000000 alcf-1.8.0/alcf.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       52 2024-04-26 20:04:19.000000 alcf-1.8.0/alcf.egg-info/entry_points.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-04-26 20:04:19.000000 alcf-1.8.0/alcf.egg-info/not-zip-safe
+-rw-r--r--   0 peter     (1000) peter     (1000)      204 2024-04-26 20:04:19.000000 alcf-1.8.0/alcf.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        5 2024-04-26 20:04:19.000000 alcf-1.8.0/alcf.egg-info/top_level.txt
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1677 2024-04-26 20:00:50.000000 alcf-1.8.0/build_doc
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.770815 alcf-1.8.0/cosp/
+-rw-r--r--   0 peter     (1000) peter     (1000)      260 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/.editorconfig
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.770815 alcf-1.8.0/cosp/MISR_simulator/
+-rw-r--r--   0 peter     (1000) peter     (1000)    16546 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/MISR_simulator/MISR_simulator.f
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.770815 alcf-1.8.0/cosp/MODIS_simulator/
+-rw-r--r--   0 peter     (1000) peter     (1000)    64835 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/MODIS_simulator/modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7387 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/MODIS_simulator/test_modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5167 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)     7506 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/Makefile.cmor1
+-rw-r--r--   0 peter     (1000) peter     (1000)     7515 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/Makefile.ibm
+-rw-r--r--   0 peter     (1000) peter     (1000)      936 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/README.md
+-rw-r--r--   0 peter     (1000) peter     (1000)    48320 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/README.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      467 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/README_v1.4.1.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.770815 alcf-1.8.0/cosp/actsim/
+-rw-r--r--   0 peter     (1000) peter     (1000)    35248 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/actsim/lidar_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    38101 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/actsim/lmd_ipsl_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11672 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/actsim/mie_backscatter_1064.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11571 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/actsim/mie_backscatter_532.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11642 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/actsim/mie_backscatter_910.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.770815 alcf-1.8.0/cosp/cfmip2/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2508 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     2487 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     7271 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     7400 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     3320 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     3261 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    31979 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cosp.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    15220 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cosp_constants.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1881 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cosp_defs.h
+-rw-r--r--   0 peter     (1000) peter     (1000)     2644 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cosp_htfrtc.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     6934 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cosp_input_nl.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    40704 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cosp_io.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4292 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cosp_isccp_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4123 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cosp_lidar.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     3561 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cosp_misr_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    25019 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cosp_modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     3646 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cosp_output_nl.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    26091 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cosp_rttov.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5694 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cosp_rttov_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     9657 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cosp_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    13744 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cosp_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    70109 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cosp_types.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    13287 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/cosp_utils.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.774815 alcf-1.8.0/cosp/icarus-scops-4.1-bsd/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2957 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/icarus-scops-4.1-bsd/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)    59127 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/icarus-scops-4.1-bsd/README
+-rw-r--r--   0 peter     (1000) peter     (1000)      165 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/icarus-scops-4.1-bsd/congvec.expected
+-rw-r--r--   0 peter     (1000) peter     (1000)     2545 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/icarus-scops-4.1-bsd/congvec.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    43978 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/icarus-scops-4.1-bsd/icarus.f
+-rw-r--r--   0 peter     (1000) peter     (1000)      869 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/icarus-scops-4.1-bsd/input.data
+-rw-r--r--   0 peter     (1000) peter     (1000)     1042 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/icarus-scops-4.1-bsd/input.data.halved
+-rw-r--r--   0 peter     (1000) peter     (1000)    13495 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     1845 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/icarus-scops-4.1-bsd/license
+-rwxr-xr-x   0 peter     (1000) peter     (1000)       15 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/icarus-scops-4.1-bsd/rcsid
+-rw-r--r--   0 peter     (1000) peter     (1000)    11849 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/icarus-scops-4.1-bsd/scops.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     2539 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/icarus-scops-4.1-bsd/test_congvec.f
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     2660 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh
+-rw-r--r--   0 peter     (1000) peter     (1000)    13385 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     3095 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.774815 alcf-1.8.0/cosp/llnl/
+-rw-r--r--   0 peter     (1000) peter     (1000)     7918 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/llnl/cosp_radar.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     6082 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/llnl/llnl_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5703 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/llnl/pf_to_mr.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     9585 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/llnl/prec_scops.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    75040 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/mac_info.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     1317 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/predict_mom07.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.774815 alcf-1.8.0/cosp/quickbeam/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1563 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/quickbeam/README
+-rw-r--r--   0 peter     (1000) peter     (1000)     4166 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/quickbeam/array_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5500 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/quickbeam/atmos_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7260 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/quickbeam/calc_Re.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    10671 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/quickbeam/dsd.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4282 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/quickbeam/format_input.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7774 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/quickbeam/gases.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1665 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/quickbeam/load_hydrometeor_classes.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1761 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/quickbeam/load_mie_table.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     9299 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/quickbeam/math_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    17248 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/quickbeam/mrgrnk.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    36058 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/quickbeam/optics_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4211 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/quickbeam/predict_psd07.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    18284 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/quickbeam/radar_simulator.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4867 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/quickbeam/radar_simulator_init.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     2934 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/quickbeam/radar_simulator_types.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4039 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/quickbeam/scale_LUTs_io.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4852 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/quickbeam/zeff.f90
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      143 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/replace_tabs.sh
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      196 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/tests.sh
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.774815 alcf-1.8.0/cosp/utils/
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     8682 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/utils/COSP_plots.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     3379 2023-04-22 09:28:05.000000 alcf-1.8.0/cosp/utils/append_cf3hr_files.sh
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      333 2024-04-26 20:00:50.000000 alcf-1.8.0/download_cosp
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.778815 alcf-1.8.0/man/
+-rw-r--r--   0 peter     (1000) peter     (1000)     4583 2024-04-26 20:00:50.000000 alcf-1.8.0/man/alcf-auto.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2280 2024-04-26 20:00:50.000000 alcf-1.8.0/man/alcf-calibrate.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      811 2024-04-26 20:00:50.000000 alcf-1.8.0/man/alcf-compare.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2308 2024-04-26 20:00:50.000000 alcf-1.8.0/man/alcf-convert.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     5120 2024-04-26 20:00:50.000000 alcf-1.8.0/man/alcf-download.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     7022 2024-04-26 20:00:50.000000 alcf-1.8.0/man/alcf-lidar.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     4811 2024-04-26 20:00:50.000000 alcf-1.8.0/man/alcf-model.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     5666 2024-04-26 20:00:50.000000 alcf-1.8.0/man/alcf-plot.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1981 2024-04-26 20:00:50.000000 alcf-1.8.0/man/alcf-simulate.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     3944 2024-04-26 20:00:50.000000 alcf-1.8.0/man/alcf-stats.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1450 2024-04-26 20:00:50.000000 alcf-1.8.0/man/alcf.1
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2024-04-26 20:04:19.778815 alcf-1.8.0/setup.cfg
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     2261 2024-04-26 20:00:50.000000 alcf-1.8.0/setup.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:04:19.778815 alcf-1.8.0/src/
+-rw-r--r--   0 peter     (1000) peter     (1000)    12585 2024-04-26 20:00:50.000000 alcf-1.8.0/src/cosp_run.f03
+-rw-r--r--   0 peter     (1000) peter     (1000)    11128 2024-04-26 20:00:50.000000 alcf-1.8.0/src/main.f03
+-rw-r--r--   0 peter     (1000) peter     (1000)     8501 2024-04-26 20:00:50.000000 alcf-1.8.0/src/nc_utils.f03
```

### Comparing `alcf-1.7.0/LICENSE.md` & `alcf-1.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/Makefile` & `alcf-1.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/PKG-INFO` & `alcf-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alcf
-Version: 1.7.0
+Version: 1.8.0
 Summary: Automatic Lidar and Ceilometer Framework (ALCF)
 Home-page: https://alcf.peterkuma.net
 Author: Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn
 Author-email: peter@peterkuma.net
 License: MIT
 Keywords: alc,ceilometer,lidar,atmosphere,model,simulator,nwp,gcm,cosp,actsim,vaisala,cl51,cl31,lufft,chm-15k,minimpl,amps,merra-2,um
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alcf-1.7.0/README.md` & `alcf-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/algorithms/cloud_base_detection/default.py` & `alcf-1.8.0/alcf/algorithms/cloud_base_detection/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/algorithms/cloud_detection/default.py` & `alcf-1.8.0/alcf/algorithms/cloud_detection/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/algorithms/couple.py` & `alcf-1.8.0/alcf/algorithms/couple.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/algorithms/interp.pyx` & `alcf-1.8.0/alcf/algorithms/interp.pyx`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/algorithms/lidar_ratio.py` & `alcf-1.8.0/alcf/algorithms/lidar_ratio.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 		 		bint[i,j] = np.sum(d['backscatter'][i,:,j]*dz)
 	else:
 		n, m = d['backscatter'].shape
 		bint = np.zeros(n, dtype=np.float64)
 		dims = ['time']
 		for i in range(n):
 		 	bint[i] = np.sum(d['backscatter'][i,:]*dz)
-	d['lr'] = 1./(2.*bint) # See O'Connor et al. (2004), Equation 6.
+	with np.errstate(divide='ignore'):
+		d['lr'] = 1./(2.*bint) # See O'Connor et al. (2004), Equation 6.
 	d['.']['lr'] = {
 		'.dims': dims,
 		'long_name': 'effective lidar ratio',
 		'units': 'sr',
 	}
 
 def stream(dd, state, **options):
```

### Comparing `alcf-1.7.0/alcf/algorithms/noise_removal/default.py` & `alcf-1.8.0/alcf/algorithms/noise_removal/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/algorithms/output_sample.py` & `alcf-1.8.0/alcf/algorithms/output_sample.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/algorithms/stats.py` & `alcf-1.8.0/alcf/algorithms/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,18 @@
 		'backscatter_mol_avg',
 		np.zeros(dims2, dtype=np.float64)
 	)
 	state['cl'] = state.get(
 		'cl',
 		np.zeros(dims2, dtype=np.float64)
 	)
+	state['cbh'] = state.get(
+		'cbh',
+		np.zeros(dims2, dtype=np.float64)
+	)
 	state['clt'] = state.get(
 		'clt',
 		np.zeros(l, dtype=np.float64) if l > 0 else 0
 	)
 	state['backscatter_hist'] = state.get(
 		'backscatter_hist',
 		np.zeros(hist_dims2, dtype=np.float64)
@@ -186,25 +190,31 @@
 		if not mask[i]:
 			continue
 		if l > 0:
 			for k in range(l):
 				if not filter_mask[i,k]:
 					continue
 				cl_tmp[:,k] += d['cloud_mask'][i,:,k]
+				if np.isfinite(d['cbh'][i,k]):
+					j = np.argmin(np.abs(state['zfull2'] - d['cbh'][i,k]))
+					state['cbh'][j,k] += 1
 				backscatter_avg_tmp[:,k] += d['backscatter'][i,:,k]
 				if 'backscatter_mol' in d:
 					backscatter_mol_avg_tmp[:,k] += d['backscatter_mol'][i,:]
 				state['n'][k] += 1
 				state['time_total'][k] += \
 					24*60*60*(d['time_bnds'][i,1] - d['time_bnds'][i,0])
 				state['clt'][k] += np.any(d['cloud_mask'][i,:,k])
 		else:
 			if not filter_mask[i]:
 				continue
 			cl_tmp[:] += d['cloud_mask'][i,:]
+			if np.isfinite(d['cbh'][i]):
+				j = np.argmin(np.abs(state['zfull2'] - d['cbh'][i]))
+				state['cbh'][j] += 1
 			backscatter_avg_tmp[:] += d['backscatter'][i,:]
 			if 'backscatter_mol' in d:
 				backscatter_mol_avg_tmp[:] += d['backscatter_mol'][i,:]
 			state['n'] += 1
 			state['time_total'] += \
 				24*60*60*(d['time_bnds'][i,1] - d['time_bnds'][i,0])
 			state['clt'] += np.any(d['cloud_mask'][i,:])
@@ -244,27 +254,30 @@
 
 def stats_reduce(state, bsd_z=None, **kwargs):
 	if len(state['cl'].shape) == 2:
 		for k in range(len(state['n'])):
 			if state['n'][k] > 0:
 				state['backscatter_hist'][:,:,k] /= state['n'][k]
 				state['cl'][:,k] /= state['n'][k]
+				state['cbh'][:,k] /= state['clt'][k]
 				state['clt'][k] /= state['n'][k]
 				state['backscatter_avg'][:,k] /= state['n'][k]
 				state['backscatter_mol_avg'][:,k] /= state['n'][k]
 	else:
 		if state['n'] != 0:
 			state['backscatter_hist'] /= state['n']
 			state['cl'] /= state['n']
+			state['cbh'] /= state['clt']
 			state['clt'] /= state['n']
 			state['backscatter_avg'] /= state['n']
 			state['backscatter_mol_avg'] /= state['n']
 	state['backscatter_sd_hist'] /= state['n']
 	do = {
 		'cl': 100.*state['cl'],
+		'cbh': 100.*state['cbh'],
 		'clt': 100.*state['clt'],
 		'zfull': state['zfull2'],
 		'n': state['n'],
 		'time_total': state['time_total'],
 		'backscatter_avg': state['backscatter_avg'],
 		'backscatter_mol_avg': state['backscatter_mol_avg'],
 		'backscatter_full': state['backscatter_full'],
@@ -284,14 +297,21 @@
 			'.dims': ['zfull', 'column'] \
 				if len(state['cl'].shape) == 2 \
 				else ['zfull'],
 			'long_name': 'cloud area fraction',
 			'standard_name': 'cloud_area_fraction_in_atmosphere_layer',
 			'units': '%',
 		},
+		'cbh': {
+			'.dims': ['zfull', 'column'] \
+				if len(state['cl'].shape) == 2 \
+				else ['zfull'],
+			'long_name': 'cloud base height',
+			'units': '%',
+		},
 		'clt': {
 			'.dims': ['column'] \
 				if isinstance(state['clt'], np.ndarray) \
 				else [],
 			'long_name': 'total cloud fraction',
 			'standard_name': 'cloud_area_fraction',
 			'units': '%',
```

### Comparing `alcf-1.7.0/alcf/algorithms/tsample.py` & `alcf-1.8.0/alcf/algorithms/tsample.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/algorithms/zsample.py` & `alcf-1.8.0/alcf/algorithms/zsample.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/cmds/auto.py` & `alcf-1.8.0/alcf/cmds/auto.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,25 +21,35 @@
 
 `alcf auto model` is equivalent to the sequence of commands:
 
     alcf model
     alcf simulate
     alcf lidar
     alcf stats
+    alcf stats (fine-scale)
+    alcf stats (clear-sky fine-scale)
     alcf plot backscatter
     alcf plot backscatter_hist
+    alcf plot backscatter_hist (fine-scale)
+    alcf plot backscatter_hist (clear-sky fine-scale)
     alcf plot cloud_occurrence
+    alcf plot cbh
 
 `alcf auto lidar` is equivalent to the sequence of commands:
 
     alcf lidar
     alcf stats
+    alcf stats (fine-scale)
+    alcf stats (clear-sky fine-scale)
     alcf plot backscatter
     alcf plot backscatter_hist
+    alcf plot backscatter_hist (fine-scale)
+    alcf plot backscatter_hist (clear-sky fine-scale)
     alcf plot cloud_occurrence
+    alcf plot cbh
 
 Arguments following `--` are treated as literal strings. Use this delimiter if the input or output file names might otherwise be interpreted as non-strings, e.g. purely numerical file names.
 
 Arguments
 ---------
 
 - `end`: End time (see Time format below).
```

### Comparing `alcf-1.7.0/alcf/cmds/auto_cmds/compare.py` & `alcf-1.8.0/alcf/cmds/auto_cmds/compare.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/cmds/auto_cmds/lidar.py` & `alcf-1.8.0/alcf/cmds/auto_cmds/lidar.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,18 +3,23 @@
 
 STEPS = ['lidar', 'stats', 'plot']
 
 def run(type_, input_, output, *args, skip=None, **kwargs):
 	lidar_dir = os.path.join(output, 'lidar')
 	stats_dir = os.path.join(output, 'stats')
 	stats_filename = os.path.join(stats_dir, 'all.nc')
+	stats_fine_filename = os.path.join(stats_dir, 'all_fine.nc')
+	stats_clear_fine_filename = os.path.join(stats_dir, 'clear_fine.nc')
 	plot_dir = os.path.join(output, 'plot')
 	backscatter_dir = os.path.join(plot_dir, 'backscatter')
 	cloud_occurrence_filename = os.path.join(plot_dir, 'cloud_occurrence.png')
+	cbh_filename = os.path.join(plot_dir, 'cbh.png')
 	backscatter_hist_filename = os.path.join(plot_dir, 'backscatter_hist.png')
+	backscatter_hist_fine_filename = os.path.join(plot_dir, 'backscatter_hist_all_fine.png')
+	backscatter_hist_clear_fine_filename = os.path.join(plot_dir, 'backscatter_hist_clear_fine.png')
 
 	if skip is not None:
 		try: i = STEPS.index(skip)
 		except ValueError:
 			raise ValueError('Invalid step "%s"' % skip)
 	else:
 		i = -1
@@ -31,24 +36,55 @@
 		lidar.run(type_, input_, lidar_dir, *args, **kwargs)
 	if i < STEPS.index('stats'):
 		print('-> %s' % stats_dir)
 		try: os.mkdir(stats_dir)
 		except OSError: pass
 		print('! alcf stats')
 		stats.run(lidar_dir, stats_filename, **kwargs)
+		stats.run(lidar_dir, stats_fine_filename,
+			blim=[-1, 1],
+			bres=0.005,
+			**kwargs
+		)
+		stats.run(lidar_dir, stats_clear_fine_filename,
+			filter='clear',
+			blim=[-1, 1],
+			bres=0.005,
+			**kwargs
+		)
 	if i < STEPS.index('plot'):
 		print('-> %s' % plot_dir)
 		try: os.mkdir(plot_dir)
 		except OSError: pass
 		print('-> %s' % backscatter_dir)
 		try: os.mkdir(backscatter_dir)
 		except OSError: pass
 		print('! alcf plot backscatter')
 		plot.run('backscatter', lidar_dir, backscatter_dir, **kwargs)
 		print('! alcf plot cloud_occurrence')
 		plot.run('cloud_occurrence', stats_filename, cloud_occurrence_filename,
 			**kwargs
 		)
+		print('! alcf plot cbh')
+		plot.run('cbh', stats_filename, cbh_filename,
+			**kwargs
+		)
 		print('! alcf plot backscatter_hist')
 		plot.run('backscatter_hist', stats_filename, backscatter_hist_filename,
 			**kwargs
 		)
+		plot.run(
+			'backscatter_hist',
+			stats_fine_filename,
+			backscatter_hist_fine_filename,
+			vlog=True,
+			vlim=[1e-3, 5],
+			**kwargs
+		)
+		plot.run(
+			'backscatter_hist',
+			stats_clear_fine_filename,
+			backscatter_hist_clear_fine_filename,
+			vlog=True,
+			vlim=[1e-3, 5],
+			**kwargs
+		)
```

### Comparing `alcf-1.7.0/alcf/cmds/auto_cmds/model.py` & `alcf-1.8.0/alcf/cmds/auto_cmds/model.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/cmds/calibrate.py` & `alcf-1.8.0/alcf/cmds/calibrate.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/cmds/compare.py` & `alcf-1.8.0/alcf/cmds/compare.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/cmds/convert.py` & `alcf-1.8.0/alcf/cmds/convert.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/cmds/lidar.py` & `alcf-1.8.0/alcf/cmds/lidar.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/cmds/main.py` & `alcf-1.8.0/alcf/cmds/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 Commands
 --------
 
 - `auto`: Peform automatic processing of model or lidar data.
 - `calibrate`: Calibrate lidar backscatter.
 - `convert`: Convert input instrument or model data to the ALCF standard NetCDF.
+- `download`: Download model data.
 - `lidar`: Process lidar data.
 - `model`: Extract model data at a point or along a track.
 - `plot`: Plot lidar data.
 - `simulate`: Simulate lidar measurements from model data using COSP.
 - `stats`: Calculate cloud occurrence statistics.
 
 Options
```

### Comparing `alcf-1.7.0/alcf/cmds/model.py` & `alcf-1.8.0/alcf/cmds/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,65 +4,14 @@
 from concurrent.futures import ProcessPoolExecutor, as_completed
 import numpy as np
 import aquarius_time as aq
 import ds_format as ds
 from alcf.models import MODELS, META
 from alcf import misc
 
-def point_to_track(point, time):
-	time_mid = 0.5*(time[0] + time[1])
-	return {
-		'lon': np.array([point[0], point[0]], dtype=np.float64),
-		'lat': np.array([point[1], point[1]], dtype=np.float64),
-		'time': np.array([time[0], time[1]], dtype=np.float64),
-		'time_bnds': np.array([[time[0], time_mid], [time_mid, time[1]]],
-			dtype=np.float64),
-	}
-
-def track_auto_time_bnds(time, track_gap=0):
-	n = len(time)
-	time_bnds = np.full((n, 2), np.nan, np.float64)
-	time_bnds[0,0] = time[0]
-	time_bnds[-1,1] = time[-1]
-	time_avg = 0.5*(time[:-1] + time[1:])
-	time_bnds[1:,0] = time_avg
-	time_bnds[:-1,1] = time_avg
-	if track_gap != 0:
-		time_diff = time[1:] - time[:-1]
-		mask1 = np.full(n, False, bool)
-		mask2 = np.full(n, False, bool)
-		mask1[:-1] = time_diff > track_gap
-		mask2[1:] = time_diff > track_gap
-		time_bnds[mask1,1] = time[mask1]
-		time_bnds[mask2,0] = time[mask2]
-	return time_bnds
-
-def read_track(filenames, lon_180=False, track_gap=0):
-	if type(filenames) not in [list, tuple]:
-		filenames = [filenames]
-	dd = []
-	for filename in filenames:
-		d = ds.read(filename, jd=True)
-		if len(d['time']) < 2:
-			raise ValueError('%s: Track must contain at least two records', filename)
-		if 'time_bnds' not in d:
-			d['time_bnds'] = track_auto_time_bnds(d['time'], track_gap)
-			d['.']['time_bnds'] = {
-				'.dims': ['time', 'bnds'],
-				'long_name': 'time bounds',
-				'standard_name': 'time',
-				'units': 'days since -4713-11-24 12:00 UTC',
-				'calendar': 'proleptic_gregorian',
-			}
-		dd += [d]
-	d = ds.merge(dd, 'time')
-	if lon_180:
-		d['lon'] = np.where(d['lon'] > 0, d['lon'], 360. + d['lon'])
-	return d
-
 def override_year_in_time(time, year):
 	try: len(time)
 	except:	return override_year_in_time(np.array([time]), year)[0]
 	date = aq.to_date(time)
 	y = date[1]
 	n = len(y)
 	if np.all(y == year):
@@ -74,18 +23,14 @@
 	start_new = np.full(n, start_new_1)
 	dt = time - start_old
 	time_new = start_new + dt
 	# Do this again in case the day overflows because of the old year is a leap
 	# year while the new is not, and the time as near the end of the year.
 	return override_year_in_time(time_new, year)
 
-def track_has_seg(track, t1, t2):
-	mask = (track['time_bnds'][:,0] < t2) & (track['time_bnds'][:,1] >= t1)
-	return np.any(mask)
-
 def worker(type_, input_, index, output, track, start, debug, r,
 	override_year=None):
 	try:
 		if override_year is not None:
 			t1 = override_year_in_time(start, override_year)
 		else:
 			t1 = start
@@ -141,15 +86,15 @@
 ==========
 
 Synopsis
 --------
 
     alcf model <type> point: { <lon> <lat> } time: { <start> <end> } [options] [--] <input> <output>
 
-    alcf model <type> track: <track> [--] <input> <output>
+    alcf model <type> track: <track> [options] [--] <input> <output>
 
 Description
 -----------
 
 Arguments following `--` are treated as literal strings. Use this delimiter if the input or output file names might otherwise be interpreted as non-strings, e.g. purely numerical file names.
 
 Arguments
@@ -159,24 +104,24 @@
 - `input`: Input directory.
 - `output`: Output directory.
 - `lon`: Point longitude (degrees East).
 - `lat`: Point latitutde (degrees North).
 - `start`: Start time (see Time format below).
 - `end`: End time (see Time format below).
 - `track: <file>`, `track: { <file>... }`: One or more track NetCDF files (see Files below). If multiple files are supplied and `time_bnds` is not present in the files, they are assumed to be multiple segments of a discontinous track unless the last and first time of adjacent tracks are the same.
-- `track_gap: <interval>`: If the interval is not 0, a track file is supplied, the `time_bnds` variable is not defined in the file and any two adjacent points are separated by more than the specified time interval (seconds), then a gap is assumed to be present between the two data points, instead of interpolating location between the two points. Default: `21600` (6 hours).
 - `options`: See Options below.
 
 Options
 -------
 
 - `njobs: <n>`: Number of parallel jobs. Default: number of CPU cores.
 - `-r`: Process the input directory recursively.
-- `--track_lon_180`: Expect track longitude between -180 and 180 degrees.
+- `--track_lon_180`: Expect track longitude between -180 and 180 degrees. This option is no longer needed as the conversion is automatically. [deprecated]
 - `override_year: <year>`: Override year in the track. Use if comparing observations with a model statistically and the model output does not have a corresponding year available. The observation time is converted to the same time relative to the start of the year in the specified year. Note that if the original year is a leap year and the override year is not, as a consequence of the above 31 December is mapped to 1 January. The output retains the original year as in the track, even though the model data come from the override year. Default: `none`.
+- `track_gap: <interval>`: If the interval is not 0, a track file is supplied, the `time_bnds` variable is not defined in the file and any two adjacent points are separated by more than the specified time interval (seconds), then a gap is assumed to be present between the two data points, instead of interpolating location between the two points. Default: `21600` (6 hours).
 
 Types
 -----
 
 - `amps`: Antarctic Mesoscale Prediction System (AMPS).
 - `era5`: ERA5.
 - `icon`: ICON.
@@ -200,34 +145,20 @@
 Examples
 --------
 
 Extract MERRA-2 model data in `M2I3NVASM.5.12.4` at 45 S, 170 E between 1 and 2 January 2020 and store the output in the directory `alcf_merra2_model`.
 
     alcf model merra2 point: { -45.0 170.0 } time: { 2020-01-01 2020-01-02 } M2I3NVASM.5.12.4 alcf_merra2_model
 	'''
-	time_lim = [-np.inf, np.inf]
-	if time is not None:
-		for i in [0, 1]:
-			time_lim[i] = aq.from_iso(time[i])
-			if time_lim[i] is None:
-				raise ValueError('Invalid time format: %s' % time[i])
-
-	d_track = None
-	if track is not None:
-		d_track = read_track(track, track_lon_180, track_gap/86400.)
-	elif point is not None and time is not None:
-		d_track = point_to_track(point, time_lim)
-	else:
-		raise ValueError('Point and time or track is required')
-
+	d_track, time_lim = misc.cmd_point_or_track(point, time, track,
+		track_gap=track_gap,
+	)
 	time_start = max(d_track['time_bnds'][0,0], time_lim[0])
 	time_end = min(d_track['time_bnds'][-1,1], time_lim[1])
 
-	# if os.path.isdir(output):
-
 	model = MODELS.get(type_)
 	if model is None:
 		raise ValueError('Invalid type: %s' % type_)
 
 	if njobs is None: njobs = os.cpu_count()
 
 	warnings = []
@@ -235,15 +166,15 @@
 	if hasattr(model, 'index'):
 		index = model.index(input_, warnings=warnings, recursive=r, njobs=njobs)
 
 	with ProcessPoolExecutor(max_workers=njobs) as ex:
 		fs = []
 		tt = np.arange(np.floor(time_start - 0.5), np.ceil(time_end - 0.5)) + 0.5
 		for t in tt:
-			if not track_has_seg(d_track, t, t + 1):
+			if not misc.track_has_seg(d_track, t, t + 1):
 				continue
 			f = ex.submit(worker, type_, input_, index, output, d_track, t,
 				debug, r, override_year)
 			fs += [f]
 	for w in warnings:
 		if len(w) == 2:
 			print('Warning: %s' % w[0], file=sys.stderr)
```

### Comparing `alcf-1.7.0/alcf/cmds/plot.py` & `alcf-1.8.0/alcf/cmds/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 	'backscatter',
 	'backscatter_sd',
 	'backscatter_mol',
 	'backscatter_sd_full',
 	'backscatter_sd_hist',
 	'zfull',
 	'lr',
+	'cbh',
 	'cl',
 	'clt',
 	'n',
 	'cloud_mask',
 	'backscatter_hist',
 	'backscatter_full',
 	'altitude',
@@ -243,44 +244,51 @@
 	formatter = plt.FuncFormatter(f)
 	plt.gca().xaxis.set_major_formatter(formatter)
 	plt.xlim(np.min(d['time']), np.max(d['time']))
 	plt.ylim(0, 50)
 	plt.ylabel('Eff. lidar ratio (sr)')
 	plt.xlabel('Time (UTC)')
 
-def plot_cloud_occurrence(dd,
+def plot_cloud_dist(plot_type, dd,
 	colors=COLORS,
 	linestyle=LINESTYLE,
 	lw=None,
 	labels=None,
 	subcolumn=0,
 	xlim=[0., 100.],
 	zlim=[0., 15000],
 	**kwargs
 ):
+	var = {
+		'cbh': 'cbh',
+		'cloud_occurrence': 'cl',
+	}[plot_type]
 	for i, d in enumerate(dd):
 		zfull = d['zfull']
-		cl = d['cl'][:,subcolumn] \
-			if len(d['cl'].shape) == 2 \
-			else d['cl']
-		clt = d['clt'][subcolumn] \
-			if len(d['clt'].shape) == 1 \
-			else d['clt']
-		n = d['n']
+		x = d[var][:,subcolumn] \
+			if len(d[var].shape) == 2 \
+			else d[var]
 		label = (labels[i] if labels is not None else '')
-		label += ' | CF: %d%%' % clt
-		plt.plot(cl, 1e-3*zfull,
+		if plot_type == 'cloud_occurrence':
+			clt = d['clt'][subcolumn] \
+				if len(d['clt'].shape) == 1 \
+				else d['clt']
+			label += ' | CF: %d%%' % clt
+		plt.plot(x, 1e-3*zfull,
 			color=colors[i],
 			linestyle=(linestyle[i] if type(linestyle) is list else linestyle),
 			lw=lw,
 			label=label,
 		)
 	plt.xlim(xlim[0], xlim[1])
 	plt.ylim(zlim[0]*1e-3, zlim[1]*1e-3)
-	plt.xlabel('Cloud occurrence (%)')
+	plt.xlabel({
+		'cbh': 'Cloud base height distribution (%)',
+		'cloud_occurrence': 'Cloud occurrence (%)',
+	}[plot_type])
 	plt.ylabel('Height (km)')
 
 	if labels is not None:
 		plot_legend()
 
 def plot_backscatter_hist(d,
 	subcolumn=0,
@@ -428,16 +436,16 @@
 			figure=plt.gcf(),
 		)
 		cax1 = plt.subplot(gs[1])
 		cax2 = plt.subplot(gs[3])
 		ax = plt.subplot(gs[0])
 		plot_profile('clw', d, cax1, alpha=0.5, **kwargs)
 		plot_profile('cli', d, cax2, alpha=0.5, **kwargs)
-	elif plot_type == 'cloud_occurrence':
-		plot_cloud_occurrence(d, **kwargs)
+	elif plot_type in ('cbh', 'cloud_occurrence'):
+		plot_cloud_dist(plot_type, d, **kwargs)
 	elif plot_type == 'backscatter_hist':
 		plot_backscatter_hist(d, **kwargs)
 	elif plot_type == 'backscatter_sd_hist':
 		plot_backscatter_sd_hist(d, **kwargs)
 	else:
 		raise ValueError('Invalid plot type "%s"' % plot_type)
 
@@ -494,22 +502,23 @@
 - `output`: Output filename or directory.
 - `options`: See Options below.
 - `plot_options`: Plot type specific options. See Plot options below.
 
 Plot types
 ----------
 
-- `backscatter`: Plot backscatter from `alcf lidar` output.
-- `backscatter_hist`: Plot backscatter histogram from `alcf stats` output.
+- `backscatter`: Plot backscatter from `alcf lidar` output on time-height axes.
+- `backscatter_hist`: Plot backscatter histogram from `alcf stats` output on backscatter-height axes.
 - `backscatter_sd_hist`: Plot backscatter standard deviation histogram from `alcf stats` output.
-- `cl`: Plot model cloud area fraction from `alcf lidar` output.
-- `cli`: Plot model mass fraction of cloud ice from `alcf lidar` output.
-- `cloud_occurrence`: Plot cloud occurrence from `alcf stats` output.
-- `clw`: Plot model mass fraction of cloud liquid water from `alcf lidar` output.
-- `clw+cli`: Plot model mass fraction of cloud liquid water and ice from `alcf lidar` output.
+- `cbh`: Plot cloud base height distribution from `alcf stats` output.
+- `cl`: Plot model cloud area fraction from `alcf lidar` output on time-height axes.
+- `cli`: Plot model mass fraction of cloud ice from `alcf lidar` output on time-height axes.
+- `cloud_occurrence`: Plot cloud occurrence by height from `alcf stats` output.
+- `clw`: Plot model mass fraction of cloud liquid water from `alcf lidar` output on time-height axes.
+- `clw+cli`: Plot model mass fraction of cloud liquid water and ice from `alcf lidar` output on time-height axes.
 
 General options
 ---------------
 
 - `dpi: <value>`: Resolution in dots per inch (DPI). Default: `300`.
 - `--grid`: Plot grid.
 - `height: <value>`: Plot height (inches). Default: `5` if `plot_type` is `cloud_occurrence` or `backscatter_hist` else `4`.
@@ -552,16 +561,16 @@
 cli, clw, and clw+cli options
 -----------------------------
 
 - `vlim: { <min> <max> }`: Value limits (g/kg). Default: `{ 1e-3 1 }`.
 - `vlog: <value>`: Plot values on logarithmic scale: `true` of `false`. Default: `true`.
 - `zres: <zres>`: Height resolution (m). Default: `50`.
 
-cloud_occurrence options
-------------------------
+cbh and cloud_occurrence options
+--------------------------------
 
 - `colors: { <value>... }`: Line colors. Default: `{ #0084c8 #dc0000 #009100 #ffc022 #ba00ff }`
 - `linestyle: { <value> ... }`: Line style (`solid`, `dashed`, `dotted`). Default: `solid`.
 - `labels: { <value>... }`: Line labels. Default: `none`.
 - `lw: <value>`: Line width. Default: `1`.
 - `xlim: { <min> <max> }`: x axis limits (%). Default: `{ 0 100 }`.
 - `zlim: { <min> <max> }`: z axis limits (m). Default: `{ 0 15 }`.
@@ -572,15 +581,15 @@
 Plot backscatter from processed Vaisala CL51 data in `alcf_cl51_lidar` and store the output in the directory `alcf_cl51_backscatter`.
 
     alcf plot backscatter alcf_cl51_lidar alcf_cl51_backscatter
 	'''
 	input_ = args[:-1]
 	output = args[-1]
 
-	if plot_type in ('backscatter_hist', 'backscatter_sd_hist', 'cloud_occurrence'):
+	if plot_type in ('backscatter_hist', 'backscatter_sd_hist', 'cbh', 'cloud_occurrence'):
 		width = width if width is not None else 5
 		height = height if height is not None else 5
 	else:
 		width = width if width is not None else 10
 		height = height if height is not None else 6
 
 	opts = {
@@ -603,15 +612,15 @@
 	if xlim is not None: opts['xlim'] = xlim
 	if zlim is not None: opts['zlim'] = zlim
 	if vlim is not None: opts['vlim'] = vlim
 	if vlog is not None: opts['vlog'] = vlog
 	if zres is not None: opts['zres'] = zres
 
 	state = {}
-	if plot_type in ('cloud_occurrence', 'backscatter_sd_hist'):
+	if plot_type in ('cbh', 'cloud_occurrence', 'backscatter_sd_hist'):
 		dd = []
 		for file in input_:
 			print('<- %s' % file)
 			dd += [ds.read(file, VARIABLES)]
 		plot(plot_type, dd, output, **opts)
 		print('-> %s' % output)
 	elif plot_type == 'backscatter_hist':
```

### Comparing `alcf-1.7.0/alcf/cmds/simulate.py` & `alcf-1.8.0/alcf/cmds/simulate.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/cmds/stats.py` & `alcf-1.8.0/alcf/cmds/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import ds_format as ds
 from alcf.algorithms import interp
 from alcf.algorithms import stats
 from alcf.misc import parse_time
 
 VARIABLES = [
 	'cloud_mask',
+	'cbh',
 	'zfull',
 	'time',
 	'time_bnds',
 	'backscatter',
 	'backscatter_sd',
 	'backscatter_mol',
 	'lon',
```

### Comparing `alcf-1.7.0/alcf/fonts/LICENSE.md` & `alcf-1.8.0/alcf/fonts/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/fonts/PublicSans-Bold.otf` & `alcf-1.8.0/alcf/fonts/PublicSans-Bold.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/fonts/PublicSans-BoldItalic.otf` & `alcf-1.8.0/alcf/fonts/PublicSans-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/fonts/PublicSans-Italic.otf` & `alcf-1.8.0/alcf/fonts/PublicSans-Italic.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/fonts/PublicSans-Regular.otf` & `alcf-1.8.0/alcf/fonts/PublicSans-Regular.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/lidars/__init__.py` & `alcf-1.8.0/alcf/lidars/__init__.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/lidars/blview.py` & `alcf-1.8.0/alcf/lidars/blview.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/lidars/chm15k.py` & `alcf-1.8.0/alcf/lidars/chm15k.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/lidars/cl51.py` & `alcf-1.8.0/alcf/lidars/cl51.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/lidars/cl61.py` & `alcf-1.8.0/alcf/lidars/cl61.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/lidars/default.py` & `alcf-1.8.0/alcf/lidars/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/lidars/mpl.py` & `alcf-1.8.0/alcf/lidars/mpl.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/lidars/mpl2nc.py` & `alcf-1.8.0/alcf/lidars/mpl2nc.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/models/__init__.py` & `alcf-1.8.0/alcf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/models/amps.py` & `alcf-1.8.0/alcf/models/amps.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/models/era5.py` & `alcf-1.8.0/alcf/models/era5.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 	}[type_]
 
 	dd = []
 	for d_idx in dd_idx:
 		time = d_idx['time']
 		lat = d_idx['latitude']
 		lon = d_idx['longitude']
+		lon = lon % 360
 		filename = d_idx['filename']
 
 		ii = np.nonzero(
 			(time >= t1 - step*0.5) &
 			(time < t2 + step*0.5)
 		)[0]
 		for i in ii:
@@ -90,14 +91,15 @@
 				jd=True,
 			)
 			for a, b in trans.items():
 				if a in d.keys():
 					ds.rename(d, a, b)
 			d['lat'] = np.array([d['lat']])
 			d['lon'] = np.array([d['lon']])
+			d['lon'] = d['lon'] % 360
 			d['.']['lat']['.dims'] = ['time']
 			d['.']['lon']['.dims'] = ['time']
 			if type_ == 'plev':
 				d['pfull'] = d['pfull'].reshape([1, len(d['pfull'])])
 				d['.']['pfull']['.dims'] = ['time', 'level']
 				d['cl'] = d['cl'][:,::-1]
 				d['clw'] = d['clw'][:,::-1]
@@ -110,14 +112,15 @@
 	if 'pfull' in d:
 		d['pfull'] = 1e2*d['pfull']
 	if 'zfull' in d:
 		d['zfull'] /= 9.80665
 	if 'orog' in d:
 		d['orog'] /= 9.80665
 	if 'cl' in d:
+		d['cl'] = np.minimum(1, np.maximum(0, d['cl']))
 		d['cl'] *= 100.
 	return d
 
 def read(dirname, index, track, t1, t2,
 	warnings=[], step=STEP, recursive=False):
 
 	d_surf = read0('surf', os.path.join(dirname, 'surf'), track, t1, t2,
```

### Comparing `alcf-1.7.0/alcf/models/icon.py` & `alcf-1.8.0/alcf/models/icon.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/models/icon_intake_healpix.py` & `alcf-1.8.0/alcf/models/icon_intake_healpix.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/models/jra55.py` & `alcf-1.8.0/alcf/models/jra55.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/models/merra2.py` & `alcf-1.8.0/alcf/models/merra2.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/models/nzcsm.py` & `alcf-1.8.0/alcf/models/nzcsm.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/models/nzesm.py` & `alcf-1.8.0/alcf/models/nzesm.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf/models/um.py` & `alcf-1.8.0/alcf/models/um.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/alcf.egg-info/PKG-INFO` & `alcf-1.8.0/alcf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alcf
-Version: 1.7.0
+Version: 1.8.0
 Summary: Automatic Lidar and Ceilometer Framework (ALCF)
 Home-page: https://alcf.peterkuma.net
 Author: Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn
 Author-email: peter@peterkuma.net
 License: MIT
 Keywords: alc,ceilometer,lidar,atmosphere,model,simulator,nwp,gcm,cosp,actsim,vaisala,cl51,cl31,lufft,chm-15k,minimpl,amps,merra-2,um
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alcf-1.7.0/alcf.egg-info/SOURCES.txt` & `alcf-1.8.0/alcf.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -34,24 +34,28 @@
 alcf/bin/__init__.py
 alcf/bin/alcf.py
 alcf/cmds/__init__.py
 alcf/cmds/auto.py
 alcf/cmds/calibrate.py
 alcf/cmds/compare.py
 alcf/cmds/convert.py
+alcf/cmds/download.py
 alcf/cmds/lidar.py
 alcf/cmds/main.py
 alcf/cmds/model.py
 alcf/cmds/plot.py
 alcf/cmds/simulate.py
 alcf/cmds/stats.py
 alcf/cmds/auto_cmds/__init__.py
 alcf/cmds/auto_cmds/compare.py
 alcf/cmds/auto_cmds/lidar.py
 alcf/cmds/auto_cmds/model.py
+alcf/download/__init__.py
+alcf/download/era5.py
+alcf/download/merra2.py
 alcf/fonts/LICENSE.md
 alcf/fonts/PublicSans-Bold.otf
 alcf/fonts/PublicSans-BoldItalic.otf
 alcf/fonts/PublicSans-Italic.otf
 alcf/fonts/PublicSans-Regular.otf
 alcf/lidars/__init__.py
 alcf/lidars/blview.py
@@ -155,14 +159,15 @@
 cosp/quickbeam/zeff.f90
 cosp/utils/COSP_plots.py
 cosp/utils/append_cf3hr_files.sh
 man/alcf-auto.1
 man/alcf-calibrate.1
 man/alcf-compare.1
 man/alcf-convert.1
+man/alcf-download.1
 man/alcf-lidar.1
 man/alcf-model.1
 man/alcf-plot.1
 man/alcf-simulate.1
 man/alcf-stats.1
 man/alcf.1
 src/cosp_run.f03
```

### Comparing `alcf-1.7.0/build_doc` & `alcf-1.8.0/build_doc`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import subprocess
 from alcf.cmds import CMDS
 from alcf.cmds import main
 
 MAN_FOOTER = '''
 ## COPYRIGHT
 
-Copyright © 2019–2021 Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard
+Copyright © 2019–2024 Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard
 Querel, Israel Silber and Connor J. Flynn.
 
 ## BUG REPORTING
 
 Report bugs to Peter Kuma (<peter@peterkuma.net>).
 
 ## SEE ALSO
```

### Comparing `alcf-1.7.0/cosp/MISR_simulator/MISR_simulator.f` & `alcf-1.8.0/cosp/MISR_simulator/MISR_simulator.f`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/MODIS_simulator/modis_simulator.F90` & `alcf-1.8.0/cosp/MODIS_simulator/modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/MODIS_simulator/test_modis_simulator.F90` & `alcf-1.8.0/cosp/MODIS_simulator/test_modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/Makefile` & `alcf-1.8.0/cosp/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/Makefile.cmor1` & `alcf-1.8.0/cosp/Makefile.cmor1`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/Makefile.ibm` & `alcf-1.8.0/cosp/Makefile.ibm`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/README.md` & `alcf-1.8.0/cosp/README.md`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/README.txt` & `alcf-1.8.0/cosp/README.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/actsim/lidar_simulator.F90` & `alcf-1.8.0/cosp/actsim/lidar_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/actsim/lmd_ipsl_stats.F90` & `alcf-1.8.0/cosp/actsim/lmd_ipsl_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/actsim/mie_backscatter_1064.F90` & `alcf-1.8.0/cosp/actsim/mie_backscatter_1064.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/actsim/mie_backscatter_532.F90` & `alcf-1.8.0/cosp/actsim/mie_backscatter_532.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/actsim/mie_backscatter_910.F90` & `alcf-1.8.0/cosp/actsim/mie_backscatter_910.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt` & `alcf-1.8.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt` & `alcf-1.8.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt` & `alcf-1.8.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt` & `alcf-1.8.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt` & `alcf-1.8.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt` & `alcf-1.8.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cosp.F90` & `alcf-1.8.0/cosp/cosp.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cosp_constants.F90` & `alcf-1.8.0/cosp/cosp_constants.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cosp_defs.h` & `alcf-1.8.0/cosp/cosp_defs.h`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cosp_htfrtc.F90` & `alcf-1.8.0/cosp/cosp_htfrtc.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cosp_input_nl.txt` & `alcf-1.8.0/cosp/cosp_input_nl.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cosp_io.F90` & `alcf-1.8.0/cosp/cosp_io.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cosp_isccp_simulator.F90` & `alcf-1.8.0/cosp/cosp_isccp_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cosp_lidar.F90` & `alcf-1.8.0/cosp/cosp_lidar.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cosp_misr_simulator.F90` & `alcf-1.8.0/cosp/cosp_misr_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cosp_modis_simulator.F90` & `alcf-1.8.0/cosp/cosp_modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cosp_output_nl.txt` & `alcf-1.8.0/cosp/cosp_output_nl.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cosp_rttov.F90` & `alcf-1.8.0/cosp/cosp_rttov.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cosp_rttov_simulator.F90` & `alcf-1.8.0/cosp/cosp_rttov_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cosp_simulator.F90` & `alcf-1.8.0/cosp/cosp_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cosp_stats.F90` & `alcf-1.8.0/cosp/cosp_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cosp_types.F90` & `alcf-1.8.0/cosp/cosp_types.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/cosp_utils.F90` & `alcf-1.8.0/cosp/cosp_utils.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/Makefile` & `alcf-1.8.0/cosp/icarus-scops-4.1-bsd/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/README` & `alcf-1.8.0/cosp/icarus-scops-4.1-bsd/README`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/congvec.f` & `alcf-1.8.0/cosp/icarus-scops-4.1-bsd/congvec.f`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/icarus.f` & `alcf-1.8.0/cosp/icarus-scops-4.1-bsd/icarus.f`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/input.data` & `alcf-1.8.0/cosp/icarus-scops-4.1-bsd/input.data`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/input.data.halved` & `alcf-1.8.0/cosp/icarus-scops-4.1-bsd/input.data.halved`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f` & `alcf-1.8.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/license` & `alcf-1.8.0/cosp/icarus-scops-4.1-bsd/license`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/scops.f` & `alcf-1.8.0/cosp/icarus-scops-4.1-bsd/scops.f`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/test_congvec.f` & `alcf-1.8.0/cosp/icarus-scops-4.1-bsd/test_congvec.f`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh` & `alcf-1.8.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f` & `alcf-1.8.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh` & `alcf-1.8.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/llnl/cosp_radar.F90` & `alcf-1.8.0/cosp/llnl/cosp_radar.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/llnl/llnl_stats.F90` & `alcf-1.8.0/cosp/llnl/llnl_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/llnl/pf_to_mr.f` & `alcf-1.8.0/cosp/llnl/pf_to_mr.f`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/llnl/prec_scops.f` & `alcf-1.8.0/cosp/llnl/prec_scops.f`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/mac_info.txt` & `alcf-1.8.0/cosp/mac_info.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/predict_mom07.F90` & `alcf-1.8.0/cosp/predict_mom07.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/quickbeam/README` & `alcf-1.8.0/cosp/quickbeam/README`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/quickbeam/array_lib.f90` & `alcf-1.8.0/cosp/quickbeam/array_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/quickbeam/atmos_lib.f90` & `alcf-1.8.0/cosp/quickbeam/atmos_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/quickbeam/calc_Re.f90` & `alcf-1.8.0/cosp/quickbeam/calc_Re.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/quickbeam/dsd.f90` & `alcf-1.8.0/cosp/quickbeam/dsd.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/quickbeam/format_input.f90` & `alcf-1.8.0/cosp/quickbeam/format_input.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/quickbeam/gases.f90` & `alcf-1.8.0/cosp/quickbeam/gases.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/quickbeam/load_hydrometeor_classes.f90` & `alcf-1.8.0/cosp/quickbeam/load_hydrometeor_classes.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/quickbeam/load_mie_table.f90` & `alcf-1.8.0/cosp/quickbeam/load_mie_table.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/quickbeam/math_lib.f90` & `alcf-1.8.0/cosp/quickbeam/math_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/quickbeam/mrgrnk.f90` & `alcf-1.8.0/cosp/quickbeam/mrgrnk.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/quickbeam/optics_lib.f90` & `alcf-1.8.0/cosp/quickbeam/optics_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/quickbeam/predict_psd07.f` & `alcf-1.8.0/cosp/quickbeam/predict_psd07.f`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/quickbeam/radar_simulator.f90` & `alcf-1.8.0/cosp/quickbeam/radar_simulator.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/quickbeam/radar_simulator_init.f90` & `alcf-1.8.0/cosp/quickbeam/radar_simulator_init.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/quickbeam/radar_simulator_types.f90` & `alcf-1.8.0/cosp/quickbeam/radar_simulator_types.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/quickbeam/scale_LUTs_io.f90` & `alcf-1.8.0/cosp/quickbeam/scale_LUTs_io.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/quickbeam/zeff.f90` & `alcf-1.8.0/cosp/quickbeam/zeff.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/utils/COSP_plots.py` & `alcf-1.8.0/cosp/utils/COSP_plots.py`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/cosp/utils/append_cf3hr_files.sh` & `alcf-1.8.0/cosp/utils/append_cf3hr_files.sh`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/man/alcf-auto.1` & `alcf-1.8.0/man/alcf-auto.1`

 * *Files 12% similar despite different names*

```diff
@@ -15,28 +15,38 @@
 \fBalcf auto model\fR is equivalent to the sequence of commands:
 .IP "" 4
 .nf
 alcf model
 alcf simulate
 alcf lidar
 alcf stats
+alcf stats (fine\-scale)
+alcf stats (clear\-sky fine\-scale)
 alcf plot backscatter
 alcf plot backscatter_hist
+alcf plot backscatter_hist (fine\-scale)
+alcf plot backscatter_hist (clear\-sky fine\-scale)
 alcf plot cloud_occurrence
+alcf plot cbh
 .fi
 .IP "" 0
 .P
 \fBalcf auto lidar\fR is equivalent to the sequence of commands:
 .IP "" 4
 .nf
 alcf lidar
 alcf stats
+alcf stats (fine\-scale)
+alcf stats (clear\-sky fine\-scale)
 alcf plot backscatter
 alcf plot backscatter_hist
+alcf plot backscatter_hist (fine\-scale)
+alcf plot backscatter_hist (clear\-sky fine\-scale)
 alcf plot cloud_occurrence
+alcf plot cbh
 .fi
 .IP "" 0
 .P
 Arguments following \fB\-\-\fR are treated as literal strings\. Use this delimiter if the input or output file names might otherwise be interpreted as non\-strings, e\.g\. purely numerical file names\.
 .SH "ARGUMENTS"
 .TP
 \fBend\fR
@@ -150,12 +160,12 @@
 Process Lufft CHM 15k data in \fBchm15k\fR and store the output in \fBalcf_chm15k\fR\.
 .IP "" 4
 .nf
 alcf auto lidar chm15k chm15k_data alcf_chm15k
 .fi
 .IP "" 0
 .SH "COPYRIGHT"
-Copyright \(co 2019–2021 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
+Copyright \(co 2019–2024 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
 .SH "BUG REPORTING"
 Report bugs to Peter Kuma (\fIpeter@peterkuma\.net\fR)\.
 .SH "SEE ALSO"
-alcf(1), alcf\-calibrate(1), alcf\-compare(1), alcf\-convert(1), alcf\-lidar(1), alcf\-model(1), alcf\-plot(1), alcf\-simulate(1), alcf\-stats(1)
+alcf(1), alcf\-calibrate(1), alcf\-compare(1), alcf\-convert(1), alcf\-download(1), alcf\-lidar(1), alcf\-model(1), alcf\-plot(1), alcf\-simulate(1), alcf\-stats(1)
```

### Comparing `alcf-1.7.0/man/alcf-calibrate.1` & `alcf-1.8.0/man/alcf-calibrate.1`

 * *Files 5% similar despite different names*

```diff
@@ -52,12 +52,12 @@
 Read time periods from \fBtime_periods\.txt\fR, lidar profiles from the directory \fBlidar\fR and write the calibration coefficient to \fBcalibration\.txt\fR\.
 .IP "" 4
 .nf
 alcf calibrate time_periods\.txt lidar calibration\.txt
 .fi
 .IP "" 0
 .SH "COPYRIGHT"
-Copyright \(co 2019–2021 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
+Copyright \(co 2019–2024 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
 .SH "BUG REPORTING"
 Report bugs to Peter Kuma (\fIpeter@peterkuma\.net\fR)\.
 .SH "SEE ALSO"
-alcf(1), alcf\-auto(1), alcf\-compare(1), alcf\-convert(1), alcf\-lidar(1), alcf\-model(1), alcf\-plot(1), alcf\-simulate(1), alcf\-stats(1)
+alcf(1), alcf\-auto(1), alcf\-compare(1), alcf\-convert(1), alcf\-download(1), alcf\-lidar(1), alcf\-model(1), alcf\-plot(1), alcf\-simulate(1), alcf\-stats(1)
```

### Comparing `alcf-1.7.0/man/alcf-compare.1` & `alcf-1.8.0/man/alcf-compare.1`

 * *Files 8% similar despite different names*

```diff
@@ -11,12 +11,12 @@
 .TP
 \fBinput_*\fR
 Input lidar data directory\.
 .TP
 \fBoutput\fR
 Output filename\.
 .SH "COPYRIGHT"
-Copyright \(co 2019–2021 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
+Copyright \(co 2019–2024 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
 .SH "BUG REPORTING"
 Report bugs to Peter Kuma (\fIpeter@peterkuma\.net\fR)\.
 .SH "SEE ALSO"
-alcf(1), alcf\-auto(1), alcf\-calibrate(1), alcf\-convert(1), alcf\-lidar(1), alcf\-model(1), alcf\-plot(1), alcf\-simulate(1), alcf\-stats(1)
+alcf(1), alcf\-auto(1), alcf\-calibrate(1), alcf\-convert(1), alcf\-download(1), alcf\-lidar(1), alcf\-model(1), alcf\-plot(1), alcf\-simulate(1), alcf\-stats(1)
```

### Comparing `alcf-1.7.0/man/alcf-convert.1` & `alcf-1.8.0/man/alcf-convert.1`

 * *Files 1% similar despite different names*

```diff
@@ -50,12 +50,12 @@
 Convert JRA\-55 data in \fBjra55_grib\fR to NetCDF and store the output in the directory \fBjra55_nc\fR\.
 .IP "" 4
 .nf
 alcf convert jra55 jra55_grib jra55_nc
 .fi
 .IP "" 0
 .SH "COPYRIGHT"
-Copyright \(co 2019–2021 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
+Copyright \(co 2019–2024 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
 .SH "BUG REPORTING"
 Report bugs to Peter Kuma (\fIpeter@peterkuma\.net\fR)\.
 .SH "SEE ALSO"
-alcf(1), alcf\-auto(1), alcf\-calibrate(1), alcf\-compare(1), alcf\-lidar(1), alcf\-model(1), alcf\-plot(1), alcf\-simulate(1), alcf\-stats(1)
+alcf(1), alcf\-auto(1), alcf\-calibrate(1), alcf\-compare(1), alcf\-download(1), alcf\-lidar(1), alcf\-model(1), alcf\-plot(1), alcf\-simulate(1), alcf\-stats(1)
```

### Comparing `alcf-1.7.0/man/alcf-lidar.1` & `alcf-1.8.0/man/alcf-lidar.1`

 * *Files 1% similar despite different names*

```diff
@@ -189,12 +189,12 @@
 Process Vaisala CL51 data in \fBcl51_nc\fR and store the output in \fBcl51_alcf_lidar\fR, assuming instrument altitude of 100 m above sea level\.
 .IP "" 4
 .nf
 alcf lidar cl51 cl51_nc cl51_alcf_lidar altitude: 100
 .fi
 .IP "" 0
 .SH "COPYRIGHT"
-Copyright \(co 2019–2021 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
+Copyright \(co 2019–2024 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
 .SH "BUG REPORTING"
 Report bugs to Peter Kuma (\fIpeter@peterkuma\.net\fR)\.
 .SH "SEE ALSO"
-alcf(1), alcf\-auto(1), alcf\-calibrate(1), alcf\-compare(1), alcf\-convert(1), alcf\-model(1), alcf\-plot(1), alcf\-simulate(1), alcf\-stats(1)
+alcf(1), alcf\-auto(1), alcf\-calibrate(1), alcf\-compare(1), alcf\-convert(1), alcf\-download(1), alcf\-model(1), alcf\-plot(1), alcf\-simulate(1), alcf\-stats(1)
```

### Comparing `alcf-1.7.0/man/alcf-model.1` & `alcf-1.8.0/man/alcf-model.1`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 .TH "ALCF\-MODEL" "1" "April 2024" ""
 .SH "NAME"
 \fBalcf\-model\fR \- Extract model data at a point or along a track\.
 .SH "SYNOPSIS"
 .nf
 alcf model <type> point: { <lon> <lat> } time: { <start> <end> } [options] [\-\-] <input> <output>
 
-alcf model <type> track: <track> [\-\-] <input> <output>
+alcf model <type> track: <track> [options] [\-\-] <input> <output>
 .fi
 .SH "DESCRIPTION"
 Arguments following \fB\-\-\fR are treated as literal strings\. Use this delimiter if the input or output file names might otherwise be interpreted as non\-strings, e\.g\. purely numerical file names\.
 .SH "ARGUMENTS"
 .IP "\[ci]" 4
 \fBtype\fR: Input data type (see Types below)\.
 .IP "\[ci]" 4
@@ -25,31 +25,32 @@
 .IP "\[ci]" 4
 \fBstart\fR: Start time (see Time format below)\.
 .IP "\[ci]" 4
 \fBend\fR: End time (see Time format below)\.
 .IP "\[ci]" 4
 \fBtrack: <file>\fR, \fBtrack: { <file>\|\.\|\.\|\. }\fR: One or more track NetCDF files (see Files below)\. If multiple files are supplied and \fBtime_bnds\fR is not present in the files, they are assumed to be multiple segments of a discontinous track unless the last and first time of adjacent tracks are the same\.
 .IP "\[ci]" 4
-\fBtrack_gap: <interval>\fR: If the interval is not 0, a track file is supplied, the \fBtime_bnds\fR variable is not defined in the file and any two adjacent points are separated by more than the specified time interval (seconds), then a gap is assumed to be present between the two data points, instead of interpolating location between the two points\. Default: \fB21600\fR (6 hours)\.
-.IP "\[ci]" 4
 \fBoptions\fR: See Options below\.
 .IP "" 0
 .SH "OPTIONS"
 .TP
 \fBnjobs: <n>\fR
 Number of parallel jobs\. Default: number of CPU cores\.
 .TP
 \fB\-r\fR
 Process the input directory recursively\.
 .TP
 \fB\-\-track_lon_180\fR
-Expect track longitude between \-180 and 180 degrees\.
+Expect track longitude between \-180 and 180 degrees\. This option is no longer needed as the conversion is automatically\. [deprecated]
 .TP
 \fBoverride_year: <year>\fR
 Override year in the track\. Use if comparing observations with a model statistically and the model output does not have a corresponding year available\. The observation time is converted to the same time relative to the start of the year in the specified year\. Note that if the original year is a leap year and the override year is not, as a consequence of the above 31 December is mapped to 1 January\. The output retains the original year as in the track, even though the model data come from the override year\. Default: \fBnone\fR\.
+.TP
+\fBtrack_gap: <interval>\fR
+If the interval is not 0, a track file is supplied, the \fBtime_bnds\fR variable is not defined in the file and any two adjacent points are separated by more than the specified time interval (seconds), then a gap is assumed to be present between the two data points, instead of interpolating location between the two points\. Default: \fB21600\fR (6 hours)\.
 .SH "TYPES"
 .TP
 \fBamps\fR
 Antarctic Mesoscale Prediction System (AMPS)\.
 .TP
 \fBera5\fR
 ERA5\.
@@ -82,12 +83,12 @@
 Extract MERRA\-2 model data in \fBM2I3NVASM\.5\.12\.4\fR at 45 S, 170 E between 1 and 2 January 2020 and store the output in the directory \fBalcf_merra2_model\fR\.
 .IP "" 4
 .nf
 alcf model merra2 point: { \-45\.0 170\.0 } time: { 2020\-01\-01 2020\-01\-02 } M2I3NVASM\.5\.12\.4 alcf_merra2_model
 .fi
 .IP "" 0
 .SH "COPYRIGHT"
-Copyright \(co 2019–2021 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
+Copyright \(co 2019–2024 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
 .SH "BUG REPORTING"
 Report bugs to Peter Kuma (\fIpeter@peterkuma\.net\fR)\.
 .SH "SEE ALSO"
-alcf(1), alcf\-auto(1), alcf\-calibrate(1), alcf\-compare(1), alcf\-convert(1), alcf\-lidar(1), alcf\-plot(1), alcf\-simulate(1), alcf\-stats(1)
+alcf(1), alcf\-auto(1), alcf\-calibrate(1), alcf\-compare(1), alcf\-convert(1), alcf\-download(1), alcf\-lidar(1), alcf\-plot(1), alcf\-simulate(1), alcf\-stats(1)
```

### Comparing `alcf-1.7.0/man/alcf-plot.1` & `alcf-1.8.0/man/alcf-plot.1`

 * *Files 4% similar despite different names*

```diff
@@ -24,36 +24,39 @@
 See Options below\.
 .TP
 \fBplot_options\fR
 Plot type specific options\. See Plot options below\.
 .SH "PLOT TYPES"
 .TP
 \fBbackscatter\fR
-Plot backscatter from \fBalcf lidar\fR output\.
+Plot backscatter from \fBalcf lidar\fR output on time\-height axes\.
 .TP
 \fBbackscatter_hist\fR
-Plot backscatter histogram from \fBalcf stats\fR output\.
+Plot backscatter histogram from \fBalcf stats\fR output on backscatter\-height axes\.
 .TP
 \fBbackscatter_sd_hist\fR
 Plot backscatter standard deviation histogram from \fBalcf stats\fR output\.
 .TP
+\fBcbh\fR
+Plot cloud base height distribution from \fBalcf stats\fR output\.
+.TP
 \fBcl\fR
-Plot model cloud area fraction from \fBalcf lidar\fR output\.
+Plot model cloud area fraction from \fBalcf lidar\fR output on time\-height axes\.
 .TP
 \fBcli\fR
-Plot model mass fraction of cloud ice from \fBalcf lidar\fR output\.
+Plot model mass fraction of cloud ice from \fBalcf lidar\fR output on time\-height axes\.
 .TP
 \fBcloud_occurrence\fR
-Plot cloud occurrence from \fBalcf stats\fR output\.
+Plot cloud occurrence by height from \fBalcf stats\fR output\.
 .TP
 \fBclw\fR
-Plot model mass fraction of cloud liquid water from \fBalcf lidar\fR output\.
+Plot model mass fraction of cloud liquid water from \fBalcf lidar\fR output on time\-height axes\.
 .TP
 \fBclw+cli\fR
-Plot model mass fraction of cloud liquid water and ice from \fBalcf lidar\fR output\.
+Plot model mass fraction of cloud liquid water and ice from \fBalcf lidar\fR output on time\-height axes\.
 .SH "GENERAL OPTIONS"
 .TP
 \fBdpi: <value>\fR
 Resolution in dots per inch (DPI)\. Default: \fB300\fR\.
 .TP
 \fB\-\-grid\fR
 Plot grid\.
@@ -127,15 +130,15 @@
 Value limits (g/kg)\. Default: \fB{ 1e\-3 1 }\fR\.
 .TP
 \fBvlog: <value>\fR
 Plot values on logarithmic scale: \fBtrue\fR of \fBfalse\fR\. Default: \fBtrue\fR\.
 .TP
 \fBzres: <zres>\fR
 Height resolution (m)\. Default: \fB50\fR\.
-.SH "CLOUD_OCCURRENCE OPTIONS"
+.SH "CBH AND CLOUD_OCCURRENCE OPTIONS"
 .TP
 \fBcolors: { <value>\|\.\|\.\|\. }\fR
 Line colors\. Default: \fB{ #0084c8 #dc0000 #009100 #ffc022 #ba00ff }\fR
 .TP
 \fBlinestyle: { <value> \|\.\|\.\|\. }\fR
 Line style (\fBsolid\fR, \fBdashed\fR, \fBdotted\fR)\. Default: \fBsolid\fR\.
 .TP
@@ -154,12 +157,12 @@
 Plot backscatter from processed Vaisala CL51 data in \fBalcf_cl51_lidar\fR and store the output in the directory \fBalcf_cl51_backscatter\fR\.
 .IP "" 4
 .nf
 alcf plot backscatter alcf_cl51_lidar alcf_cl51_backscatter
 .fi
 .IP "" 0
 .SH "COPYRIGHT"
-Copyright \(co 2019–2021 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
+Copyright \(co 2019–2024 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
 .SH "BUG REPORTING"
 Report bugs to Peter Kuma (\fIpeter@peterkuma\.net\fR)\.
 .SH "SEE ALSO"
-alcf(1), alcf\-auto(1), alcf\-calibrate(1), alcf\-compare(1), alcf\-convert(1), alcf\-lidar(1), alcf\-model(1), alcf\-simulate(1), alcf\-stats(1)
+alcf(1), alcf\-auto(1), alcf\-calibrate(1), alcf\-compare(1), alcf\-convert(1), alcf\-download(1), alcf\-lidar(1), alcf\-model(1), alcf\-simulate(1), alcf\-stats(1)
```

### Comparing `alcf-1.7.0/man/alcf-simulate.1` & `alcf-1.8.0/man/alcf-simulate.1`

 * *Files 10% similar despite different names*

```diff
@@ -52,12 +52,12 @@
 Simulate a Vaisala CL51 instrument from model data in \fBalcf_merra2_model\fR previously extracted using \fBalcf model\fR and store the output in the direcctory \fBalcf_merra2_simulate\fR\.
 .IP "" 4
 .nf
 alcf simulate cl51 alcf_merra2_model alcf_merra2_simulate
 .fi
 .IP "" 0
 .SH "COPYRIGHT"
-Copyright \(co 2019–2021 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
+Copyright \(co 2019–2024 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
 .SH "BUG REPORTING"
 Report bugs to Peter Kuma (\fIpeter@peterkuma\.net\fR)\.
 .SH "SEE ALSO"
-alcf(1), alcf\-auto(1), alcf\-calibrate(1), alcf\-compare(1), alcf\-convert(1), alcf\-lidar(1), alcf\-model(1), alcf\-plot(1), alcf\-stats(1)
+alcf(1), alcf\-auto(1), alcf\-calibrate(1), alcf\-compare(1), alcf\-convert(1), alcf\-download(1), alcf\-lidar(1), alcf\-model(1), alcf\-plot(1), alcf\-stats(1)
```

### Comparing `alcf-1.7.0/man/alcf-stats.1` & `alcf-1.8.0/man/alcf-stats.1`

 * *Files 2% similar despite different names*

```diff
@@ -61,12 +61,12 @@
 Calculate statistics from processed lidar data in \fBalcf_cl51_lidar\fR and store the output in \fBalcf_cl51_stats\.nc\fR\.
 .IP "" 4
 .nf
 alcf stats alcf_cl51_lidar alcf_cl51_stats\.nc
 .fi
 .IP "" 0
 .SH "COPYRIGHT"
-Copyright \(co 2019–2021 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
+Copyright \(co 2019–2024 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
 .SH "BUG REPORTING"
 Report bugs to Peter Kuma (\fIpeter@peterkuma\.net\fR)\.
 .SH "SEE ALSO"
-alcf(1), alcf\-auto(1), alcf\-calibrate(1), alcf\-compare(1), alcf\-convert(1), alcf\-lidar(1), alcf\-model(1), alcf\-plot(1), alcf\-simulate(1)
+alcf(1), alcf\-auto(1), alcf\-calibrate(1), alcf\-compare(1), alcf\-convert(1), alcf\-download(1), alcf\-lidar(1), alcf\-model(1), alcf\-plot(1), alcf\-simulate(1)
```

### Comparing `alcf-1.7.0/man/alcf.1` & `alcf-1.8.0/man/alcf.1`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 .TP
 \fBcalibrate\fR
 Calibrate lidar backscatter\.
 .TP
 \fBconvert\fR
 Convert input instrument or model data to the ALCF standard NetCDF\.
 .TP
+\fBdownload\fR
+Download model data\.
+.TP
 \fBlidar\fR
 Process lidar data\.
 .TP
 \fBmodel\fR
 Extract model data at a point or along a track\.
 .TP
 \fBplot\fR
@@ -44,12 +47,12 @@
 .TP
 \fB\-\-help\fR
 Print help for command\.
 .TP
 \fB\-\-debug\fR
 Enable debugging information\.
 .SH "COPYRIGHT"
-Copyright \(co 2019–2021 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
+Copyright \(co 2019–2024 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
 .SH "BUG REPORTING"
 Report bugs to Peter Kuma (\fIpeter@peterkuma\.net\fR)\.
 .SH "SEE ALSO"
-alcf\-auto(1), alcf\-calibrate(1), alcf\-compare(1), alcf\-convert(1), alcf\-lidar(1), alcf\-model(1), alcf\-plot(1), alcf\-simulate(1), alcf\-stats(1)
+alcf\-auto(1), alcf\-calibrate(1), alcf\-compare(1), alcf\-convert(1), alcf\-download(1), alcf\-lidar(1), alcf\-model(1), alcf\-plot(1), alcf\-simulate(1), alcf\-stats(1)
```

### Comparing `alcf-1.7.0/setup.py` & `alcf-1.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 	def run(self):
 		subprocess.run('make', cwd='cosp', check=True)
 		subprocess.run('make', check=True)
 		build_py.run(self)
 
 setup(
 	name='alcf',
-	version='1.7.0',
+	version='1.8.0',
 	description='Automatic Lidar and Ceilometer Framework (ALCF)',
 	author='Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn',
 	author_email='peter@peterkuma.net',
 	license='MIT',
 	entry_points={
 		'console_scripts': 'alcf = alcf.bin.alcf:main_wrapper',
 	},
@@ -53,14 +53,16 @@
 		'cl2nc>=3.4.0',
 		'mpl2nc>=1.3.6',
 		'aquarius-time>=0.4.0',
 		'ds-format>=4.1.0',
 		'pst-format>=2.0.0',
 		'astropy>=5.3.2',
 		'cftime>=1.6.2',
+		'requests>=2.31.0',
+		'cdsapi>=0.7.0',
 	],
 	keywords=['alc', 'ceilometer', 'lidar', 'atmosphere', 'model', 'simulator', 'nwp', 'gcm', 'cosp', 'actsim', 'vaisala', 'cl51', 'cl31', 'lufft', 'chm-15k', 'minimpl', 'amps', 'merra-2', 'um'],
 	url='https://alcf.peterkuma.net',
 	classifiers=[
 		'Development Status :: 5 - Production/Stable',
 		'Environment :: Console',
 		'Intended Audience :: Science/Research',
```

### Comparing `alcf-1.7.0/src/cosp_run.f03` & `alcf-1.8.0/src/cosp_run.f03`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/src/main.f03` & `alcf-1.8.0/src/main.f03`

 * *Files identical despite different names*

### Comparing `alcf-1.7.0/src/nc_utils.f03` & `alcf-1.8.0/src/nc_utils.f03`

 * *Files identical despite different names*

