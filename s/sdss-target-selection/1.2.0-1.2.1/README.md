# Comparing `tmp/sdss_target_selection-1.2.0.tar.gz` & `tmp/sdss_target_selection-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_target_selection-1.2.0.tar", last modified: Wed Apr 24 00:03:19 2024, max compression
+gzip compressed data, was "sdss_target_selection-1.2.1.tar", last modified: Thu Apr 25 23:06:37 2024, max compression
```

## Comparing `sdss_target_selection-1.2.0.tar` & `sdss_target_selection-1.2.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-24 00:03:19.799222 sdss_target_selection-1.2.0/
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     1504 2021-05-24 23:45:26.000000 sdss_target_selection-1.2.0/LICENSE.md
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)       79 2021-05-24 23:45:26.000000 sdss_target_selection-1.2.0/MANIFEST.in
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     3968 2024-04-24 00:03:19.799222 sdss_target_selection-1.2.0/PKG-INFO
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     1484 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/README.md
-drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-24 00:03:19.787222 sdss_target_selection-1.2.0/bin/
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)      302 2021-05-24 23:45:26.000000 sdss_target_selection-1.2.0/bin/target_selection
--rwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)     6590 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/bin/yanny_scraper
-drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-24 00:03:19.787222 sdss_target_selection-1.2.0/python/
-drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-24 00:03:19.795222 sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     3968 2024-04-24 00:03:19.000000 sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/PKG-INFO
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     3296 2024-04-24 00:03:19.000000 sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/SOURCES.txt
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)        1 2024-04-24 00:03:19.000000 sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/dependency_links.txt
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)        1 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/not-zip-safe
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)      624 2024-04-24 00:03:19.000000 sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/requires.txt
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)       17 2024-04-24 00:03:19.000000 sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/top_level.txt
-drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-24 00:03:19.787222 sdss_target_selection-1.2.0/python/target_selection/
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)      718 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/__init__.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    11216 2023-05-17 22:25:33.000000 sdss_target_selection-1.2.0/python/target_selection/__main__.py
-drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-24 00:03:19.791222 sdss_target_selection-1.2.0/python/target_selection/cartons/
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     1079 2023-06-01 13:48:09.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/__init__.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    50847 2024-04-23 23:42:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/base.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    11674 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_aqmes.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    13826 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_csc.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    11105 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_galaxies.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    10763 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_gua.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    14152 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_rm.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    52812 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_spiders_agn.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    16838 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_spiders_clusters.py
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     2654 2021-05-24 23:45:26.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/guide.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    12336 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_bin_gaia.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     5621 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_bin_vis.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    45489 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_cb.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     3361 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_cb_cvcandidates.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    13869 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_dust.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    13013 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_erosita.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    10863 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_galactic.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     8713 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_halo.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    50754 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_halo_gaia_dr3.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     5476 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_legacy_ir2opt.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     7694 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_magcloud_agb.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     7060 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_magcloud_rgb.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    14468 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_monitor_apogee.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     9872 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_ob.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     4055 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_planet.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    25410 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_rv.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    17466 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_snc.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     4079 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_tess_ob.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     6738 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_tess_rgb.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     4882 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_wd.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    71200 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_yso.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     7568 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/ops_apogee_stds.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    59366 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/ops_boss_stds.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    12519 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/ops_bright_stars.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    15848 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/ops_skies.py
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     5789 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/skymask.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     2161 2024-04-23 23:42:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/too.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    21933 2023-05-18 08:21:33.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/tools.py
-drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-24 00:03:19.795222 sdss_target_selection-1.2.0/python/target_selection/config/
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)   147249 2024-04-23 23:42:23.000000 sdss_target_selection-1.2.0/python/target_selection/config/target_selection.yml
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     9866 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/config/target_selection_v0.yml
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     8761 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/config/xmatch_v0.yml
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     6480 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/config/xmatch_v0p5.yml
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    32525 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/config/xmatch_v1.yml
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     1383 2023-06-01 20:51:59.000000 sdss_target_selection-1.2.0/python/target_selection/exceptions.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     3148 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/mag_flux.py
-drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-24 00:03:19.795222 sdss_target_selection-1.2.0/python/target_selection/masks/
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     4171 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.0/python/target_selection/masks/AQMES_wboss_imaging_NGC_proc.ply
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     8640 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.2.1.fits
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     8640 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.3.1.fits
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)    40320 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.2.1.fits
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    40320 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.3.1.fits
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     8640 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_rm_v0.2.1.fits
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)   348269 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.0/python/target_selection/masks/rsFields-annotated-lco-deep_proc.ply
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)   135360 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.0/python/target_selection/masks/rsFields_boss_survey.fits
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)    40320 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.0/python/target_selection/masks/rsFields_boss_survey_sgc.fits
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    37638 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/skies.py
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)    10703 2021-05-24 23:45:26.000000 sdss_target_selection-1.2.0/python/target_selection/utils.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    86433 2024-04-23 23:42:23.000000 sdss_target_selection-1.2.0/python/target_selection/xmatch.py
--rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     2541 2024-04-24 00:03:19.799222 sdss_target_selection-1.2.0/setup.cfg
--rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)       73 2021-05-24 23:45:26.000000 sdss_target_selection-1.2.0/setup.py
+drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-04-25 23:06:37.745427 sdss_target_selection-1.2.1/
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1504 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/LICENSE.md
+-rw-r--r--   0 gallegoj   (501) staff       (20)       79 2024-02-07 23:03:33.000000 sdss_target_selection-1.2.1/MANIFEST.in
+-rw-r--r--   0 gallegoj   (501) staff       (20)     3969 2024-04-25 23:06:37.744903 sdss_target_selection-1.2.1/PKG-INFO
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1485 2024-04-25 14:27:13.000000 sdss_target_selection-1.2.1/README.md
+drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-04-25 23:06:37.652361 sdss_target_selection-1.2.1/bin/
+-rw-r--r--   0 gallegoj   (501) staff       (20)      302 2024-02-07 23:03:33.000000 sdss_target_selection-1.2.1/bin/target_selection
+-rwxr-xr-x   0 gallegoj   (501) staff       (20)     6590 2023-02-07 16:26:59.000000 sdss_target_selection-1.2.1/bin/yanny_scraper
+drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-04-25 23:06:37.644012 sdss_target_selection-1.2.1/python/
+drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-04-25 23:06:37.735895 sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/
+-rw-r--r--   0 gallegoj   (501) staff       (20)     3969 2024-04-25 23:06:37.000000 sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/PKG-INFO
+-rw-r--r--   0 gallegoj   (501) staff       (20)     3296 2024-04-25 23:06:37.000000 sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/SOURCES.txt
+-rw-r--r--   0 gallegoj   (501) staff       (20)        1 2024-04-25 23:06:37.000000 sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/dependency_links.txt
+-rw-r--r--   0 gallegoj   (501) staff       (20)        1 2024-02-07 23:06:15.000000 sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/not-zip-safe
+-rw-r--r--   0 gallegoj   (501) staff       (20)      624 2024-04-25 23:06:37.000000 sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/requires.txt
+-rw-r--r--   0 gallegoj   (501) staff       (20)       17 2024-04-25 23:06:37.000000 sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/top_level.txt
+drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-04-25 23:06:37.663612 sdss_target_selection-1.2.1/python/target_selection/
+-rw-r--r--   0 gallegoj   (501) staff       (20)      718 2024-02-14 03:30:22.000000 sdss_target_selection-1.2.1/python/target_selection/__init__.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    11216 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/__main__.py
+drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-04-25 23:06:37.714995 sdss_target_selection-1.2.1/python/target_selection/cartons/
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1079 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/__init__.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    50847 2024-04-25 14:27:13.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/base.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    11674 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_aqmes.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    13826 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_csc.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    11105 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_galaxies.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    10763 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_gua.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    14152 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_rm.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    52812 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_spiders_agn.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    16838 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_spiders_clusters.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     2654 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/guide.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    12336 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_bin_gaia.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5621 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_bin_vis.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    45489 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_cb.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     3361 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_cb_cvcandidates.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    13869 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_dust.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    13013 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_erosita.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    10863 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_galactic.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8713 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_halo.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    50754 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_halo_gaia_dr3.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5476 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_legacy_ir2opt.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7694 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_magcloud_agb.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7060 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_magcloud_rgb.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    14468 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_monitor_apogee.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     9872 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_ob.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     4055 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_planet.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    25410 2024-04-23 18:31:40.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_rv.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    17466 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_snc.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     4079 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_tess_ob.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6738 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_tess_rgb.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     4882 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_wd.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    71200 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_yso.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7568 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/ops_apogee_stds.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    59366 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/ops_boss_stds.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    12519 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/ops_bright_stars.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    15848 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/ops_skies.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5789 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/skymask.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     2161 2024-04-25 14:27:13.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/too.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    21933 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/tools.py
+drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-04-25 23:06:37.721035 sdss_target_selection-1.2.1/python/target_selection/config/
+-rw-r--r--   0 gallegoj   (501) staff       (20)   147249 2024-04-25 14:27:13.000000 sdss_target_selection-1.2.1/python/target_selection/config/target_selection.yml
+-rw-r--r--   0 gallegoj   (501) staff       (20)     9866 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/python/target_selection/config/target_selection_v0.yml
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8761 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/python/target_selection/config/xmatch_v0.yml
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6480 2023-04-19 16:37:23.000000 sdss_target_selection-1.2.1/python/target_selection/config/xmatch_v0p5.yml
+-rw-r--r--   0 gallegoj   (501) staff       (20)    33349 2024-04-25 21:48:29.000000 sdss_target_selection-1.2.1/python/target_selection/config/xmatch_v1.yml
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1383 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/exceptions.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     3148 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/mag_flux.py
+drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-04-25 23:06:37.734762 sdss_target_selection-1.2.1/python/target_selection/masks/
+-rw-r--r--   0 gallegoj   (501) staff       (20)     4171 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/python/target_selection/masks/AQMES_wboss_imaging_NGC_proc.ply
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8640 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.2.1.fits
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8640 2023-02-07 16:26:59.000000 sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.3.1.fits
+-rw-r--r--   0 gallegoj   (501) staff       (20)    40320 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.2.1.fits
+-rw-r--r--   0 gallegoj   (501) staff       (20)    40320 2023-02-07 16:26:59.000000 sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.3.1.fits
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8640 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_rm_v0.2.1.fits
+-rw-r--r--   0 gallegoj   (501) staff       (20)   348269 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/python/target_selection/masks/rsFields-annotated-lco-deep_proc.ply
+-rw-r--r--   0 gallegoj   (501) staff       (20)   135360 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/python/target_selection/masks/rsFields_boss_survey.fits
+-rw-r--r--   0 gallegoj   (501) staff       (20)    40320 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/python/target_selection/masks/rsFields_boss_survey_sgc.fits
+-rw-r--r--   0 gallegoj   (501) staff       (20)    37638 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/skies.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    10703 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/utils.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    86826 2024-04-25 22:20:34.000000 sdss_target_selection-1.2.1/python/target_selection/xmatch.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     2541 2024-04-25 23:06:37.748657 sdss_target_selection-1.2.1/setup.cfg
+-rw-r--r--   0 gallegoj   (501) staff       (20)       73 2024-02-07 23:03:33.000000 sdss_target_selection-1.2.1/setup.py
```

### Comparing `sdss_target_selection-1.2.0/LICENSE.md` & `sdss_target_selection-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/PKG-INFO` & `sdss_target_selection-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-target-selection
-Version: 1.2.0
+Version: 1.2.1
 Summary: Code to perform target selection for BHM/MWM using catalogdb
 Home-page: https://github.com/sdss/target_selection
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/target_selection
 Project-URL: Documentation, https://sdss-target-selection.readthedocs.org
@@ -58,15 +58,15 @@
 Requires-Dist: furo>=2021.6.18-beta.36; extra == "docs"
 Requires-Dist: sphinx-autobuild>=2021.3.14; extra == "docs"
 Requires-Dist: sphinx-copybutton>=0.3.3; extra == "docs"
 Requires-Dist: myst-parser>=0.15; extra == "docs"
 
 # target_selection
 
-![Versions](https://img.shields.io/badge/python->3.7-blue)
+![Versions](https://img.shields.io/badge/python->=3.8-blue)
 [![Documentation Status](https://readthedocs.org/projects/sdss-target-selection/badge/?version=latest)](https://sdss-target-selection.readthedocs.io/en/latest/?badge=latest)
 <!-- [![Travis (.org)](https://img.shields.io/travis/sdss/target_selection)](https://travis-ci.org/sdss/target_selection)
 [![codecov](https://codecov.io/gh/sdss/target_selection/branch/main/graph/badge.svg)](https://codecov.io/gh/sdss/target_selection) -->
 
 Code to perform target selection for BHM/MWM using catalogdb.
 
 ## Installation
```

### Comparing `sdss_target_selection-1.2.0/README.md` & `sdss_target_selection-1.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # target_selection
 
-![Versions](https://img.shields.io/badge/python->3.7-blue)
+![Versions](https://img.shields.io/badge/python->=3.8-blue)
 [![Documentation Status](https://readthedocs.org/projects/sdss-target-selection/badge/?version=latest)](https://sdss-target-selection.readthedocs.io/en/latest/?badge=latest)
 <!-- [![Travis (.org)](https://img.shields.io/travis/sdss/target_selection)](https://travis-ci.org/sdss/target_selection)
 [![codecov](https://codecov.io/gh/sdss/target_selection/branch/main/graph/badge.svg)](https://codecov.io/gh/sdss/target_selection) -->
 
 Code to perform target selection for BHM/MWM using catalogdb.
 
 ## Installation
```

### Comparing `sdss_target_selection-1.2.0/bin/yanny_scraper` & `sdss_target_selection-1.2.1/bin/yanny_scraper`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/PKG-INFO` & `sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-target-selection
-Version: 1.2.0
+Version: 1.2.1
 Summary: Code to perform target selection for BHM/MWM using catalogdb
 Home-page: https://github.com/sdss/target_selection
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/target_selection
 Project-URL: Documentation, https://sdss-target-selection.readthedocs.org
@@ -58,15 +58,15 @@
 Requires-Dist: furo>=2021.6.18-beta.36; extra == "docs"
 Requires-Dist: sphinx-autobuild>=2021.3.14; extra == "docs"
 Requires-Dist: sphinx-copybutton>=0.3.3; extra == "docs"
 Requires-Dist: myst-parser>=0.15; extra == "docs"
 
 # target_selection
 
-![Versions](https://img.shields.io/badge/python->3.7-blue)
+![Versions](https://img.shields.io/badge/python->=3.8-blue)
 [![Documentation Status](https://readthedocs.org/projects/sdss-target-selection/badge/?version=latest)](https://sdss-target-selection.readthedocs.io/en/latest/?badge=latest)
 <!-- [![Travis (.org)](https://img.shields.io/travis/sdss/target_selection)](https://travis-ci.org/sdss/target_selection)
 [![codecov](https://codecov.io/gh/sdss/target_selection/branch/main/graph/badge.svg)](https://codecov.io/gh/sdss/target_selection) -->
 
 Code to perform target selection for BHM/MWM using catalogdb.
 
 ## Installation
```

### Comparing `sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/SOURCES.txt` & `sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/requires.txt` & `sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/__init__.py` & `sdss_target_selection-1.2.1/python/target_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/__main__.py` & `sdss_target_selection-1.2.1/python/target_selection/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/__init__.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/base.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/base.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_aqmes.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_aqmes.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_csc.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_csc.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_galaxies.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_galaxies.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_gua.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_gua.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_rm.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_rm.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_spiders_agn.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_spiders_agn.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_spiders_clusters.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_spiders_clusters.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/guide.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/guide.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_bin_gaia.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_bin_gaia.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_bin_vis.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_bin_vis.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_cb.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_cb.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_cb_cvcandidates.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_cb_cvcandidates.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_dust.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_dust.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_erosita.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_erosita.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_galactic.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_galactic.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_halo.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_halo.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_halo_gaia_dr3.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_halo_gaia_dr3.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_legacy_ir2opt.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_legacy_ir2opt.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_magcloud_agb.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_magcloud_agb.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_magcloud_rgb.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_magcloud_rgb.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_monitor_apogee.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_monitor_apogee.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_ob.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_ob.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_planet.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_planet.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_rv.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_rv.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_snc.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_snc.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_tess_ob.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_tess_ob.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_tess_rgb.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_tess_rgb.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_wd.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_wd.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_yso.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_yso.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/ops_apogee_stds.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/ops_apogee_stds.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/ops_boss_stds.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/ops_boss_stds.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/ops_bright_stars.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/ops_bright_stars.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/ops_skies.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/ops_skies.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/skymask.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/skymask.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/too.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/too.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/cartons/tools.py` & `sdss_target_selection-1.2.1/python/target_selection/cartons/tools.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/config/target_selection.yml` & `sdss_target_selection-1.2.1/python/target_selection/config/target_selection.yml`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/config/target_selection_v0.yml` & `sdss_target_selection-1.2.1/python/target_selection/config/target_selection_v0.yml`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/config/xmatch_v0.yml` & `sdss_target_selection-1.2.1/python/target_selection/config/xmatch_v0.yml`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/config/xmatch_v0p5.yml` & `sdss_target_selection-1.2.1/python/target_selection/config/xmatch_v0p5.yml`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/config/xmatch_v1.yml` & `sdss_target_selection-1.2.1/python/target_selection/config/xmatch_v1.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,38 @@
+'1.1.1':
+    run_id: 9
+    query_radius: 1.0
+    show_sql: True
+    schema: catalogdb
+    output_table: catalog
+    start_node: gaia_dr3_source
+    debug: true
+    log_path: xmatch_{plan}.log
+    path_mode: config_list
+    extra_nodes:
+        - 'tycho2'
+        - 'catalog_to_tycho2'
+        - 'twomass_psc'
+        - 'catalog_to_twomass_psc'
+    version_id: 31
+    order:
+        - marvels_dr11_star
+    tables:
+        marvels_dr11_star:
+            ra_column: ra_final
+            dec_column: dec_final
+    join_paths:
+        - ['marvels_dr11_star', 'tycho2', 'catalog_to_tycho2', 'catalog']
+        - ['marvels_dr11_star', 'twomass_psc', 'catalog_to_twomass_psc', 'catalog']
+    database_options:
+        work_mem: '10GB'
+        temp_buffers: '5GB'
+        maintenance_work_mem: '5GB'
+        enable_hashjoin: false
+
 '1.1.0':
     run_id: 8
     query_radius: 1.0
     show_sql: True
     schema: catalogdb
     output_table: catalog
     start_node: gaia_dr3_source
```

### Comparing `sdss_target_selection-1.2.0/python/target_selection/exceptions.py` & `sdss_target_selection-1.2.1/python/target_selection/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/mag_flux.py` & `sdss_target_selection-1.2.1/python/target_selection/mag_flux.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/masks/AQMES_wboss_imaging_NGC_proc.ply` & `sdss_target_selection-1.2.1/python/target_selection/masks/AQMES_wboss_imaging_NGC_proc.ply`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.2.1.fits` & `sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.2.1.fits`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.3.1.fits` & `sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.3.1.fits`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.2.1.fits` & `sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.2.1.fits`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.3.1.fits` & `sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.3.1.fits`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_rm_v0.2.1.fits` & `sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_rm_v0.2.1.fits`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/masks/rsFields-annotated-lco-deep_proc.ply` & `sdss_target_selection-1.2.1/python/target_selection/masks/rsFields-annotated-lco-deep_proc.ply`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/masks/rsFields_boss_survey.fits` & `sdss_target_selection-1.2.1/python/target_selection/masks/rsFields_boss_survey.fits`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/masks/rsFields_boss_survey_sgc.fits` & `sdss_target_selection-1.2.1/python/target_selection/masks/rsFields_boss_survey_sgc.fits`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/skies.py` & `sdss_target_selection-1.2.1/python/target_selection/skies.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/utils.py` & `sdss_target_selection-1.2.1/python/target_selection/utils.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.0/python/target_selection/xmatch.py` & `sdss_target_selection-1.2.1/python/target_selection/xmatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -568,14 +568,19 @@
             The path to the configuration file to use. Defaults to
             ``config/xmatch.yml``. The file must contain a hash with the
             cross-match plan.
         kwargs : dict
             User arguments that will override the configuration file values.
 
         """
+
+        # HACK: this ensures that the catalogdb.models are populated. In principle thos would not
+        # work if schema != catalogdb but anyway many other things would fail in that case.
+        from sdssdb.peewee.sdss5db import catalogdb  # noqa
+
         if isinstance(in_models, (list, tuple)):
             models = in_models
         elif inspect.isclass(in_models) and issubclass(in_models, Model):
             database = in_models._meta.database
             models = set(in_models.__subclasses__())
             while True:
                 old_models = models.copy()
@@ -979,20 +984,21 @@
 
         Version._meta.schema = self.schema
         Version._meta.set_database(self.database)
 
     def _check_version(self, model, force=False):
         """Checks if a model contains a plan version."""
 
-        vexists = (peewee.Select(
-            columns=[fn.EXISTS(model
-                               .select(SQL('1'))
-                               .where(model.version_id == self.version_id))])
-                   .tuples()
-                   .execute(self.database))[0][0]
+        with self.database.atomic():
+            self.database.execute_sql('SET LOCAL enable_seqscan = off;')
+            vexists = (peewee.Select(
+                columns=[fn.EXISTS(model
+                                   .select(SQL('1'))
+                                   .where(model.version_id == self.version_id))]).tuples()
+                       .execute(self.database))[0][0]
 
         if vexists:
 
             msg = (f'{model._meta.table_name!r} contains records for this '
                    f'cross-matching plan ({self.plan}).')
 
             if force:
@@ -1912,16 +1918,17 @@
 
         self.log.debug(f'Inserted {n_rows:,} rows in {timer.elapsed:.3f} s.')
 
         if not keep_temp:
             self.database.drop_tables([from_model])
             self.log.info(f'Dropped temporary table {from_table}.')
 
-        self.log.debug(f'Running VACUUM ANALYZE on {to_table}.')
-        vacuum_table(self.database, to_table, vacuum=True, analyze=True)
+        if n_rows > 0:
+            self.log.debug(f'Running VACUUM ANALYZE on {to_table}.')
+            vacuum_table(self.database, to_table, vacuum=True, analyze=True)
 
     def _get_sql(self, query, return_string=False):
         """Returns colourised SQL text for logging."""
 
         query_str, query_params = query.sql()
 
         if query_params:
```

### Comparing `sdss_target_selection-1.2.0/setup.cfg` & `sdss_target_selection-1.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sdss-target-selection
-version = 1.2.0
+version = 1.2.1
 author = José Sánchez-Gallego
 author_email = gallegoj@uw.edu
 description = Code to perform target selection for BHM/MWM using catalogdb
 url = https://github.com/sdss/target_selection
 project_urls = 
 	Repository = https://github.com/sdss/target_selection
 	Documentation = https://sdss-target-selection.readthedocs.org
```

