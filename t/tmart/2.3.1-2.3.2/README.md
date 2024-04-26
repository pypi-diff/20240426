# Comparing `tmp/tmart-2.3.1.tar.gz` & `tmp/tmart-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmart-2.3.1.tar", last modified: Thu Apr 11 14:40:23 2024, max compression
+gzip compressed data, was "tmart-2.3.2.tar", last modified: Fri Apr 26 02:50:50 2024, max compression
```

## Comparing `tmart-2.3.1.tar` & `tmart-2.3.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-11 14:40:23.802264 tmart-2.3.1/
--rw-r--r--   0 yw         (501) staff       (20)       51 2023-10-19 15:57:58.000000 tmart-2.3.1/MANIFEST.in
--rw-r--r--   0 yw         (501) staff       (20)     5204 2024-04-11 14:40:23.802050 tmart-2.3.1/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)     4357 2024-03-17 13:59:52.000000 tmart-2.3.1/README.md
--rw-r--r--   0 yw         (501) staff       (20)       38 2024-04-11 14:40:23.802315 tmart-2.3.1/setup.cfg
--rw-r--r--   0 yw         (501) staff       (20)     2045 2024-04-11 14:27:23.000000 tmart-2.3.1/setup.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-11 14:40:23.779645 tmart-2.3.1/tests/
--rwxrwxrwx   0 yw         (501) staff       (20)      413 2023-10-19 16:51:10.000000 tmart-2.3.1/tests/test_AEC.py
--rw-r--r--   0 yw         (501) staff       (20)     2960 2023-05-23 22:19:27.000000 tmart-2.3.1/tests/test_AE_modelling.py
--rw-r--r--   0 yw         (501) staff       (20)     3048 2023-01-03 02:43:30.000000 tmart-2.3.1/tests/test_E_diffuse.py
--rw-r--r--   0 yw         (501) staff       (20)     2310 2023-01-03 03:48:03.000000 tmart-2.3.1/tests/test_L_sky.py
--rw-r--r--   0 yw         (501) staff       (20)     2569 2024-01-30 23:00:00.000000 tmart-2.3.1/tests/test_basic.py
--rw-r--r--   0 yw         (501) staff       (20)     1327 2022-09-21 16:59:26.000000 tmart-2.3.1/tests/test_basic_import.py
--rw-r--r--   0 yw         (501) staff       (20)      824 2023-05-26 03:52:15.000000 tmart-2.3.1/tests/test_calc_rho.py
--rw-r--r--   0 yw         (501) staff       (20)     3197 2022-09-17 14:43:02.000000 tmart-2.3.1/tests/test_calcref.py
--rw-r--r--   0 yw         (501) staff       (20)     1172 2023-05-26 22:25:30.000000 tmart-2.3.1/tests/test_fresnel.py
--rwxrwxrwx   0 yw         (501) staff       (20)     1489 2023-10-19 16:51:11.000000 tmart-2.3.1/tests/test_modelling.py
--rw-r--r--   0 yw         (501) staff       (20)     2047 2024-04-11 14:38:23.000000 tmart-2.3.1/tests/test_plot.py
--rw-r--r--   0 yw         (501) staff       (20)     2993 2023-03-25 22:34:08.000000 tmart-2.3.1/tests/test_quickstart.py
--rw-r--r--   0 yw         (501) staff       (20)     3113 2022-09-26 04:25:24.000000 tmart-2.3.1/tests/test_specular_contribution.py
--rw-r--r--   0 yw         (501) staff       (20)     3228 2022-09-27 15:07:16.000000 tmart-2.3.1/tests/test_typical_ocean.py
--rw-r--r--   0 yw         (501) staff       (20)     3021 2022-10-03 05:42:50.000000 tmart-2.3.1/tests/test_whales_SR.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-11 14:40:23.782755 tmart-2.3.1/tmart/
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-11 14:40:23.790061 tmart-2.3.1/tmart/AEC/
--rw-r--r--   0 yw         (501) staff       (20)     9444 2024-03-28 18:17:03.000000 tmart-2.3.1/tmart/AEC/AEC.py
--rw-r--r--   0 yw         (501) staff       (20)     1016 2024-03-28 20:07:38.000000 tmart-2.3.1/tmart/AEC/__init__.py
--rw-r--r--   0 yw         (501) staff       (20)     1758 2023-10-20 19:50:31.000000 tmart-2.3.1/tmart/AEC/anci_download.py
--rw-r--r--   0 yw         (501) staff       (20)     3546 2024-03-10 16:18:02.000000 tmart-2.3.1/tmart/AEC/anci_get_AER.py
--rw-r--r--   0 yw         (501) staff       (20)     2383 2024-03-10 16:16:52.000000 tmart-2.3.1/tmart/AEC/anci_get_OWV.py
--rw-r--r--   0 yw         (501) staff       (20)     1788 2024-03-10 16:16:09.000000 tmart-2.3.1/tmart/AEC/anci_list_files.py
--rw-r--r--   0 yw         (501) staff       (20)     1628 2024-03-10 16:14:25.000000 tmart-2.3.1/tmart/AEC/compute_gas_transmittance.py
--rw-r--r--   0 yw         (501) staff       (20)     9844 2024-03-28 18:15:37.000000 tmart-2.3.1/tmart/AEC/compute_masks.py
--rw-r--r--   0 yw         (501) staff       (20)      648 2023-10-18 00:57:41.000000 tmart-2.3.1/tmart/AEC/fillnan.py
--rw-r--r--   0 yw         (501) staff       (20)     9982 2024-03-10 16:15:20.000000 tmart-2.3.1/tmart/AEC/get_AOT.py
--rw-r--r--   0 yw         (501) staff       (20)     1579 2023-12-14 02:45:52.000000 tmart-2.3.1/tmart/AEC/get_ancillary.py
--rw-r--r--   0 yw         (501) staff       (20)     6588 2024-03-10 16:17:43.000000 tmart-2.3.1/tmart/AEC/get_parameters.py
--rw-r--r--   0 yw         (501) staff       (20)      995 2024-03-10 16:16:22.000000 tmart-2.3.1/tmart/AEC/identify_sensor.py
--rw-r--r--   0 yw         (501) staff       (20)     4553 2024-03-10 16:14:57.000000 tmart-2.3.1/tmart/AEC/irradiance_correction.py
--rw-r--r--   0 yw         (501) staff       (20)     1184 2024-01-11 18:18:13.000000 tmart-2.3.1/tmart/AEC/read_PRISMA_north.py
--rw-r--r--   0 yw         (501) staff       (20)     2886 2023-10-18 01:13:05.000000 tmart-2.3.1/tmart/AEC/read_PRISMA_vaa.py
--rw-r--r--   0 yw         (501) staff       (20)     1060 2024-03-10 16:17:04.000000 tmart-2.3.1/tmart/AEC/read_config.py
--rw-r--r--   0 yw         (501) staff       (20)    11907 2024-03-28 21:59:35.000000 tmart-2.3.1/tmart/AEC/read_metadata_Landsat.py
--rw-r--r--   0 yw         (501) staff       (20)     6684 2024-03-10 16:17:00.000000 tmart-2.3.1/tmart/AEC/read_metadata_S2.py
--rw-r--r--   0 yw         (501) staff       (20)     2036 2023-10-18 01:15:47.000000 tmart-2.3.1/tmart/AEC/read_xml_S2.py
--rw-r--r--   0 yw         (501) staff       (20)     1331 2023-10-18 01:14:23.000000 tmart-2.3.1/tmart/AEC/read_xml_S2_scene.py
--rw-r--r--   0 yw         (501) staff       (20)     4798 2024-03-28 17:56:28.000000 tmart-2.3.1/tmart/AEC/run.py
--rw-r--r--   0 yw         (501) staff       (20)    12038 2024-01-14 03:26:49.000000 tmart-2.3.1/tmart/AEC/run_acoliteL1R.py
--rw-r--r--   0 yw         (501) staff       (20)     2743 2024-03-28 20:00:23.000000 tmart-2.3.1/tmart/AEC/run_regular.py
--rw-r--r--   0 yw         (501) staff       (20)     1144 2024-01-11 21:20:16.000000 tmart-2.3.1/tmart/AEC/write_atm_info.py
--rw-r--r--   0 yw         (501) staff       (20)     1811 2024-01-18 16:28:44.000000 tmart-2.3.1/tmart/Aerosol.py
--rw-r--r--   0 yw         (501) staff       (20)    11377 2024-03-10 16:08:40.000000 tmart-2.3.1/tmart/Atmosphere.py
--rw-r--r--   0 yw         (501) staff       (20)     9961 2024-01-18 16:27:41.000000 tmart-2.3.1/tmart/Surface.py
--rw-r--r--   0 yw         (501) staff       (20)    13680 2024-01-18 16:35:11.000000 tmart-2.3.1/tmart/Tmart.py
--rw-r--r--   0 yw         (501) staff       (20)    38594 2024-04-11 14:37:47.000000 tmart-2.3.1/tmart/Tmart2.py
--rw-r--r--   0 yw         (501) staff       (20)      550 2023-12-28 20:42:03.000000 tmart-2.3.1/tmart/__init__.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-11 14:40:23.792044 tmart-2.3.1/tmart/ancillary/
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-11 14:40:23.800608 tmart-2.3.1/tmart/ancillary/aerosolSPF/
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:20:25.000000 tmart-2.3.1/tmart/ancillary/aerosolSPF/BiomassBurning.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:49:56.000000 tmart-2.3.1/tmart/ancillary/aerosolSPF/Continental.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:55:10.000000 tmart-2.3.1/tmart/ancillary/aerosolSPF/Desert.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 16:59:28.000000 tmart-2.3.1/tmart/ancillary/aerosolSPF/Maritime.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:21:44.000000 tmart-2.3.1/tmart/ancillary/aerosolSPF/Stratospheric.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:53:59.000000 tmart-2.3.1/tmart/ancillary/aerosolSPF/Urban.csv
--rw-r--r--   0 yw         (501) staff       (20)     1763 2022-12-14 22:44:42.000000 tmart-2.3.1/tmart/ancillary/conifer_forest.csv
--rw-r--r--   0 yw         (501) staff       (20)      838 2022-12-14 22:45:12.000000 tmart-2.3.1/tmart/ancillary/dry_beach_sand.csv
--rw-r--r--   0 yw         (501) staff       (20)     1618 2022-12-14 22:45:48.000000 tmart-2.3.1/tmart/ancillary/lawn_grass.csv
--rw-r--r--   0 yw         (501) staff       (20)      794 2021-08-03 20:21:41.000000 tmart-2.3.1/tmart/ancillary/soil.csv
--rw-r--r--   0 yw         (501) staff       (20)     1190 2021-08-03 20:22:22.000000 tmart-2.3.1/tmart/ancillary/vegetation.csv
--rw-r--r--   0 yw         (501) staff       (20)      284 2021-08-03 20:21:58.000000 tmart-2.3.1/tmart/ancillary/water.csv
--rw-r--r--   0 yw         (501) staff       (20)      707 2022-02-08 17:04:47.000000 tmart-2.3.1/tmart/ancillary/water_chl1.csv
--rw-r--r--   0 yw         (501) staff       (20)     1015 2022-12-14 22:46:19.000000 tmart-2.3.1/tmart/ancillary/wet_beach_sand.csv
--rw-r--r--   0 yw         (501) staff       (20)      181 2023-03-31 22:46:09.000000 tmart-2.3.1/tmart/ancillary/whitecap_factor.csv
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-11 14:40:23.801120 tmart-2.3.1/tmart/config/
--rw-r--r--   0 yw         (501) staff       (20)     1303 2024-03-28 18:02:22.000000 tmart-2.3.1/tmart/config/config.txt
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-11 14:40:23.801630 tmart-2.3.1/tmart/surface_rho/
--rw-r--r--   0 yw         (501) staff       (20)      341 2023-05-23 22:27:30.000000 tmart-2.3.1/tmart/surface_rho/__init__.py
--rw-r--r--   0 yw         (501) staff       (20)     5038 2023-05-26 07:42:38.000000 tmart-2.3.1/tmart/surface_rho/calculate.py
--rw-r--r--   0 yw         (501) staff       (20)     2003 2024-03-10 16:10:22.000000 tmart-2.3.1/tmart/tm_OT.py
--rw-r--r--   0 yw         (501) staff       (20)     3195 2024-01-18 16:28:32.000000 tmart-2.3.1/tmart/tm_calcref.py
--rw-r--r--   0 yw         (501) staff       (20)     3976 2024-03-10 16:09:31.000000 tmart-2.3.1/tmart/tm_geometry.py
--rw-r--r--   0 yw         (501) staff       (20)    12883 2024-03-10 16:09:57.000000 tmart-2.3.1/tmart/tm_intersect.py
--rw-r--r--   0 yw         (501) staff       (20)    11243 2024-03-10 16:10:06.000000 tmart-2.3.1/tmart/tm_move.py
--rw-r--r--   0 yw         (501) staff       (20)     6748 2024-01-18 16:33:59.000000 tmart-2.3.1/tmart/tm_sampling.py
--rw-r--r--   0 yw         (501) staff       (20)    12104 2024-04-11 14:31:53.000000 tmart-2.3.1/tmart/tm_water.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-11 14:40:23.783362 tmart-2.3.1/tmart.egg-info/
--rw-r--r--   0 yw         (501) staff       (20)     5204 2024-04-11 14:40:23.000000 tmart-2.3.1/tmart.egg-info/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)     2067 2024-04-11 14:40:23.000000 tmart-2.3.1/tmart.egg-info/SOURCES.txt
--rw-r--r--   0 yw         (501) staff       (20)        1 2024-04-11 14:40:23.000000 tmart-2.3.1/tmart.egg-info/dependency_links.txt
--rw-r--r--   0 yw         (501) staff       (20)       70 2024-04-11 14:40:23.000000 tmart-2.3.1/tmart.egg-info/requires.txt
--rw-r--r--   0 yw         (501) staff       (20)        6 2024-04-11 14:40:23.000000 tmart-2.3.1/tmart.egg-info/top_level.txt
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 02:50:50.427745 tmart-2.3.2/
+-rw-r--r--   0 yw         (501) staff       (20)       51 2023-10-19 15:57:58.000000 tmart-2.3.2/MANIFEST.in
+-rw-r--r--   0 yw         (501) staff       (20)     5181 2024-04-26 02:50:50.427512 tmart-2.3.2/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)     4334 2024-04-11 20:04:30.000000 tmart-2.3.2/README.md
+-rw-r--r--   0 yw         (501) staff       (20)       38 2024-04-26 02:50:50.427799 tmart-2.3.2/setup.cfg
+-rw-r--r--   0 yw         (501) staff       (20)     2045 2024-04-26 02:49:16.000000 tmart-2.3.2/setup.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 02:50:50.408933 tmart-2.3.2/tests/
+-rwxrwxrwx   0 yw         (501) staff       (20)      413 2023-10-19 16:51:10.000000 tmart-2.3.2/tests/test_AEC.py
+-rw-r--r--   0 yw         (501) staff       (20)     2960 2023-05-23 22:19:27.000000 tmart-2.3.2/tests/test_AE_modelling.py
+-rw-r--r--   0 yw         (501) staff       (20)     3048 2023-01-03 02:43:30.000000 tmart-2.3.2/tests/test_E_diffuse.py
+-rw-r--r--   0 yw         (501) staff       (20)     2310 2023-01-03 03:48:03.000000 tmart-2.3.2/tests/test_L_sky.py
+-rw-r--r--   0 yw         (501) staff       (20)     2569 2024-01-30 23:00:00.000000 tmart-2.3.2/tests/test_basic.py
+-rw-r--r--   0 yw         (501) staff       (20)     1327 2022-09-21 16:59:26.000000 tmart-2.3.2/tests/test_basic_import.py
+-rw-r--r--   0 yw         (501) staff       (20)      824 2023-05-26 03:52:15.000000 tmart-2.3.2/tests/test_calc_rho.py
+-rw-r--r--   0 yw         (501) staff       (20)     3197 2022-09-17 14:43:02.000000 tmart-2.3.2/tests/test_calcref.py
+-rw-r--r--   0 yw         (501) staff       (20)     1172 2023-05-26 22:25:30.000000 tmart-2.3.2/tests/test_fresnel.py
+-rwxrwxrwx   0 yw         (501) staff       (20)     1489 2023-10-19 16:51:11.000000 tmart-2.3.2/tests/test_modelling.py
+-rw-r--r--   0 yw         (501) staff       (20)     2047 2024-04-11 14:38:23.000000 tmart-2.3.2/tests/test_plot.py
+-rw-r--r--   0 yw         (501) staff       (20)     2993 2023-03-25 22:34:08.000000 tmart-2.3.2/tests/test_quickstart.py
+-rw-r--r--   0 yw         (501) staff       (20)     3113 2022-09-26 04:25:24.000000 tmart-2.3.2/tests/test_specular_contribution.py
+-rw-r--r--   0 yw         (501) staff       (20)     3228 2022-09-27 15:07:16.000000 tmart-2.3.2/tests/test_typical_ocean.py
+-rw-r--r--   0 yw         (501) staff       (20)     3021 2022-10-03 05:42:50.000000 tmart-2.3.2/tests/test_whales_SR.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 02:50:50.411898 tmart-2.3.2/tmart/
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 02:50:50.418206 tmart-2.3.2/tmart/AEC/
+-rw-r--r--   0 yw         (501) staff       (20)     9444 2024-03-28 18:17:03.000000 tmart-2.3.2/tmart/AEC/AEC.py
+-rw-r--r--   0 yw         (501) staff       (20)     1016 2024-03-28 20:07:38.000000 tmart-2.3.2/tmart/AEC/__init__.py
+-rw-r--r--   0 yw         (501) staff       (20)     1758 2023-10-20 19:50:31.000000 tmart-2.3.2/tmart/AEC/anci_download.py
+-rw-r--r--   0 yw         (501) staff       (20)     3546 2024-03-10 16:18:02.000000 tmart-2.3.2/tmart/AEC/anci_get_AER.py
+-rw-r--r--   0 yw         (501) staff       (20)     2383 2024-03-10 16:16:52.000000 tmart-2.3.2/tmart/AEC/anci_get_OWV.py
+-rw-r--r--   0 yw         (501) staff       (20)     1788 2024-03-10 16:16:09.000000 tmart-2.3.2/tmart/AEC/anci_list_files.py
+-rw-r--r--   0 yw         (501) staff       (20)     1628 2024-03-10 16:14:25.000000 tmart-2.3.2/tmart/AEC/compute_gas_transmittance.py
+-rw-r--r--   0 yw         (501) staff       (20)     9844 2024-03-28 18:15:37.000000 tmart-2.3.2/tmart/AEC/compute_masks.py
+-rw-r--r--   0 yw         (501) staff       (20)      648 2023-10-18 00:57:41.000000 tmart-2.3.2/tmart/AEC/fillnan.py
+-rw-r--r--   0 yw         (501) staff       (20)     9982 2024-03-10 16:15:20.000000 tmart-2.3.2/tmart/AEC/get_AOT.py
+-rw-r--r--   0 yw         (501) staff       (20)     1579 2023-12-14 02:45:52.000000 tmart-2.3.2/tmart/AEC/get_ancillary.py
+-rw-r--r--   0 yw         (501) staff       (20)     6588 2024-03-10 16:17:43.000000 tmart-2.3.2/tmart/AEC/get_parameters.py
+-rw-r--r--   0 yw         (501) staff       (20)      995 2024-03-10 16:16:22.000000 tmart-2.3.2/tmart/AEC/identify_sensor.py
+-rw-r--r--   0 yw         (501) staff       (20)     4553 2024-03-10 16:14:57.000000 tmart-2.3.2/tmart/AEC/irradiance_correction.py
+-rw-r--r--   0 yw         (501) staff       (20)     1184 2024-01-11 18:18:13.000000 tmart-2.3.2/tmart/AEC/read_PRISMA_north.py
+-rw-r--r--   0 yw         (501) staff       (20)     2886 2023-10-18 01:13:05.000000 tmart-2.3.2/tmart/AEC/read_PRISMA_vaa.py
+-rw-r--r--   0 yw         (501) staff       (20)     1060 2024-03-10 16:17:04.000000 tmart-2.3.2/tmart/AEC/read_config.py
+-rw-r--r--   0 yw         (501) staff       (20)    11907 2024-03-28 21:59:35.000000 tmart-2.3.2/tmart/AEC/read_metadata_Landsat.py
+-rw-r--r--   0 yw         (501) staff       (20)     6684 2024-03-10 16:17:00.000000 tmart-2.3.2/tmart/AEC/read_metadata_S2.py
+-rw-r--r--   0 yw         (501) staff       (20)     2036 2023-10-18 01:15:47.000000 tmart-2.3.2/tmart/AEC/read_xml_S2.py
+-rw-r--r--   0 yw         (501) staff       (20)     1331 2023-10-18 01:14:23.000000 tmart-2.3.2/tmart/AEC/read_xml_S2_scene.py
+-rw-r--r--   0 yw         (501) staff       (20)     4979 2024-04-26 02:46:10.000000 tmart-2.3.2/tmart/AEC/run.py
+-rw-r--r--   0 yw         (501) staff       (20)    12107 2024-04-26 02:47:20.000000 tmart-2.3.2/tmart/AEC/run_acoliteL1R.py
+-rw-r--r--   0 yw         (501) staff       (20)     2780 2024-04-26 02:47:20.000000 tmart-2.3.2/tmart/AEC/run_regular.py
+-rw-r--r--   0 yw         (501) staff       (20)     1144 2024-01-11 21:20:16.000000 tmart-2.3.2/tmart/AEC/write_atm_info.py
+-rw-r--r--   0 yw         (501) staff       (20)     1811 2024-01-18 16:28:44.000000 tmart-2.3.2/tmart/Aerosol.py
+-rw-r--r--   0 yw         (501) staff       (20)    11377 2024-03-10 16:08:40.000000 tmart-2.3.2/tmart/Atmosphere.py
+-rw-r--r--   0 yw         (501) staff       (20)     9961 2024-01-18 16:27:41.000000 tmart-2.3.2/tmart/Surface.py
+-rw-r--r--   0 yw         (501) staff       (20)    13680 2024-01-18 16:35:11.000000 tmart-2.3.2/tmart/Tmart.py
+-rw-r--r--   0 yw         (501) staff       (20)    38594 2024-04-11 14:37:47.000000 tmart-2.3.2/tmart/Tmart2.py
+-rw-r--r--   0 yw         (501) staff       (20)      550 2023-12-28 20:42:03.000000 tmart-2.3.2/tmart/__init__.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 02:50:50.420518 tmart-2.3.2/tmart/ancillary/
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 02:50:50.425917 tmart-2.3.2/tmart/ancillary/aerosolSPF/
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:20:25.000000 tmart-2.3.2/tmart/ancillary/aerosolSPF/BiomassBurning.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:49:56.000000 tmart-2.3.2/tmart/ancillary/aerosolSPF/Continental.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:55:10.000000 tmart-2.3.2/tmart/ancillary/aerosolSPF/Desert.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 16:59:28.000000 tmart-2.3.2/tmart/ancillary/aerosolSPF/Maritime.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:21:44.000000 tmart-2.3.2/tmart/ancillary/aerosolSPF/Stratospheric.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:53:59.000000 tmart-2.3.2/tmart/ancillary/aerosolSPF/Urban.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1763 2022-12-14 22:44:42.000000 tmart-2.3.2/tmart/ancillary/conifer_forest.csv
+-rw-r--r--   0 yw         (501) staff       (20)      838 2022-12-14 22:45:12.000000 tmart-2.3.2/tmart/ancillary/dry_beach_sand.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1618 2022-12-14 22:45:48.000000 tmart-2.3.2/tmart/ancillary/lawn_grass.csv
+-rw-r--r--   0 yw         (501) staff       (20)      794 2021-08-03 20:21:41.000000 tmart-2.3.2/tmart/ancillary/soil.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1190 2021-08-03 20:22:22.000000 tmart-2.3.2/tmart/ancillary/vegetation.csv
+-rw-r--r--   0 yw         (501) staff       (20)      284 2021-08-03 20:21:58.000000 tmart-2.3.2/tmart/ancillary/water.csv
+-rw-r--r--   0 yw         (501) staff       (20)      707 2022-02-08 17:04:47.000000 tmart-2.3.2/tmart/ancillary/water_chl1.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1015 2022-12-14 22:46:19.000000 tmart-2.3.2/tmart/ancillary/wet_beach_sand.csv
+-rw-r--r--   0 yw         (501) staff       (20)      181 2023-03-31 22:46:09.000000 tmart-2.3.2/tmart/ancillary/whitecap_factor.csv
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 02:50:50.426659 tmart-2.3.2/tmart/config/
+-rw-r--r--   0 yw         (501) staff       (20)     1303 2024-03-28 18:02:22.000000 tmart-2.3.2/tmart/config/config.txt
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 02:50:50.427163 tmart-2.3.2/tmart/surface_rho/
+-rw-r--r--   0 yw         (501) staff       (20)      341 2023-05-23 22:27:30.000000 tmart-2.3.2/tmart/surface_rho/__init__.py
+-rw-r--r--   0 yw         (501) staff       (20)     5038 2023-05-26 07:42:38.000000 tmart-2.3.2/tmart/surface_rho/calculate.py
+-rw-r--r--   0 yw         (501) staff       (20)     2003 2024-03-10 16:10:22.000000 tmart-2.3.2/tmart/tm_OT.py
+-rw-r--r--   0 yw         (501) staff       (20)     3195 2024-01-18 16:28:32.000000 tmart-2.3.2/tmart/tm_calcref.py
+-rw-r--r--   0 yw         (501) staff       (20)     3976 2024-03-10 16:09:31.000000 tmart-2.3.2/tmart/tm_geometry.py
+-rw-r--r--   0 yw         (501) staff       (20)    12883 2024-03-10 16:09:57.000000 tmart-2.3.2/tmart/tm_intersect.py
+-rw-r--r--   0 yw         (501) staff       (20)    11243 2024-03-10 16:10:06.000000 tmart-2.3.2/tmart/tm_move.py
+-rw-r--r--   0 yw         (501) staff       (20)     6748 2024-01-18 16:33:59.000000 tmart-2.3.2/tmart/tm_sampling.py
+-rw-r--r--   0 yw         (501) staff       (20)    12104 2024-04-11 14:31:53.000000 tmart-2.3.2/tmart/tm_water.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 02:50:50.412685 tmart-2.3.2/tmart.egg-info/
+-rw-r--r--   0 yw         (501) staff       (20)     5181 2024-04-26 02:50:50.000000 tmart-2.3.2/tmart.egg-info/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)     2067 2024-04-26 02:50:50.000000 tmart-2.3.2/tmart.egg-info/SOURCES.txt
+-rw-r--r--   0 yw         (501) staff       (20)        1 2024-04-26 02:50:50.000000 tmart-2.3.2/tmart.egg-info/dependency_links.txt
+-rw-r--r--   0 yw         (501) staff       (20)       70 2024-04-26 02:50:50.000000 tmart-2.3.2/tmart.egg-info/requires.txt
+-rw-r--r--   0 yw         (501) staff       (20)        6 2024-04-26 02:50:50.000000 tmart-2.3.2/tmart.egg-info/top_level.txt
```

### Comparing `tmart-2.3.1/PKG-INFO` & `tmart-2.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmart
-Version: 2.3.1
+Version: 2.3.2
 Summary: Modelling and correcting for the adjacency effect in aquatic remote sensing
 Author: Yulun Wu
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
@@ -60,15 +60,15 @@
 
 ```bash
 pip3 install tmart
 ```
 
 ## Quick Start: Adjacency-Effect Correction 
 
-T-Mart supports adjacency-effect correction for Sentinel-2 MSI and Landsat 8 OLI products. Correction is performed directly on level-1 products therefore can be followed by any amtospheric-correction tools. Minimal inputs are: 
+T-Mart supports adjacency-effect correction for Sentinel-2 MSI and Landsat 8/9 OLI/OLI-2 products. Correction is performed directly on level-1 products therefore can be followed by any amtospheric-correction tools. Minimal inputs are: 
 
 ```python
 import tmart
 file = 'user/test/S2A_MSIL1C_20160812T143752_N0204_R096_T20MKB_20160812T143749.SAFE'
 
 # NASA EarthData Credentials, OB.DAAC Data Access needs to be approved
 username = 'abcdef'
@@ -100,25 +100,24 @@
 my_surface = tmart.Surface(DEM = image_DEM,
                            reflectance = image_reflectance,
                            isWater = image_isWater,
                            cell_size = 10_000)  
                                
 ### Atmosphere ###
 atm_profile = AtmosProfile.PredefinedType(AtmosProfile.MidlatitudeSummer) 
-aerosol_type = 'Maritime'  
-my_atm = tmart.Atmosphere(atm_profile, aot550 = 0, aerosol_type = 'Maritime'  )
+my_atm = tmart.Atmosphere(atm_profile, aot550 = 0, aerosol_type = 'Maritime')
 
 ### Create T-Mart Object ###
 my_tmart = tmart.Tmart(Surface = my_surface, Atmosphere= my_atm, shadow=False)
 my_tmart.set_geometry(sensor_coords=[51,50,130_000], 
                       target_pt_direction=[180,0],
                       sun_dir=[0,0])
 
 ### Multiprocessing needs to be wrapped in 'if __name__ == "__main__":' for Windows systems. 
-### This can be skipped for Linux-based systems. 
+### This can be skipped for Unix-based systems. 
 if __name__ == "__main__":
     results = my_tmart.run(wl=wl, band=None, n_photon=10_000)
     
     # Calculate reflectances using recorded photon information 
     R = tmart.calc_ref(results)
     for k, v in R.items():
         print(k, '     ' , v)
```

### Comparing `tmart-2.3.1/README.md` & `tmart-2.3.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 ```bash
 pip3 install tmart
 ```
 
 ## Quick Start: Adjacency-Effect Correction 
 
-T-Mart supports adjacency-effect correction for Sentinel-2 MSI and Landsat 8 OLI products. Correction is performed directly on level-1 products therefore can be followed by any amtospheric-correction tools. Minimal inputs are: 
+T-Mart supports adjacency-effect correction for Sentinel-2 MSI and Landsat 8/9 OLI/OLI-2 products. Correction is performed directly on level-1 products therefore can be followed by any amtospheric-correction tools. Minimal inputs are: 
 
 ```python
 import tmart
 file = 'user/test/S2A_MSIL1C_20160812T143752_N0204_R096_T20MKB_20160812T143749.SAFE'
 
 # NASA EarthData Credentials, OB.DAAC Data Access needs to be approved
 username = 'abcdef'
@@ -76,25 +76,24 @@
 my_surface = tmart.Surface(DEM = image_DEM,
                            reflectance = image_reflectance,
                            isWater = image_isWater,
                            cell_size = 10_000)  
                                
 ### Atmosphere ###
 atm_profile = AtmosProfile.PredefinedType(AtmosProfile.MidlatitudeSummer) 
-aerosol_type = 'Maritime'  
-my_atm = tmart.Atmosphere(atm_profile, aot550 = 0, aerosol_type = 'Maritime'  )
+my_atm = tmart.Atmosphere(atm_profile, aot550 = 0, aerosol_type = 'Maritime')
 
 ### Create T-Mart Object ###
 my_tmart = tmart.Tmart(Surface = my_surface, Atmosphere= my_atm, shadow=False)
 my_tmart.set_geometry(sensor_coords=[51,50,130_000], 
                       target_pt_direction=[180,0],
                       sun_dir=[0,0])
 
 ### Multiprocessing needs to be wrapped in 'if __name__ == "__main__":' for Windows systems. 
-### This can be skipped for Linux-based systems. 
+### This can be skipped for Unix-based systems. 
 if __name__ == "__main__":
     results = my_tmart.run(wl=wl, band=None, n_photon=10_000)
     
     # Calculate reflectances using recorded photon information 
     R = tmart.calc_ref(results)
     for k, v in R.items():
         print(k, '     ' , v)
```

### Comparing `tmart-2.3.1/setup.py` & `tmart-2.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tmart",                     # This is the name of the package
-    version="2.3.1",                       
+    version="2.3.2",                       
     author="Yulun Wu",                     # Full name of the author
     description="Modelling and correcting for the adjacency effect in aquatic remote sensing",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     # packages=setuptools.find_packages(),    # List of all python modules to be installed
     packages = ['tmart','tmart.surface_rho','tmart.AEC','tmart.ancillary','tmart.ancillary.aerosolSPF','tmart.config'],
     include_package_data=True,
```

### Comparing `tmart-2.3.1/tests/test_AE_modelling.py` & `tmart-2.3.2/tests/test_AE_modelling.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tests/test_E_diffuse.py` & `tmart-2.3.2/tests/test_E_diffuse.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tests/test_L_sky.py` & `tmart-2.3.2/tests/test_L_sky.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tests/test_basic.py` & `tmart-2.3.2/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tests/test_basic_import.py` & `tmart-2.3.2/tests/test_basic_import.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tests/test_calc_rho.py` & `tmart-2.3.2/tests/test_calc_rho.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tests/test_calcref.py` & `tmart-2.3.2/tests/test_calcref.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tests/test_fresnel.py` & `tmart-2.3.2/tests/test_fresnel.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tests/test_modelling.py` & `tmart-2.3.2/tests/test_modelling.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tests/test_plot.py` & `tmart-2.3.2/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tests/test_quickstart.py` & `tmart-2.3.2/tests/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tests/test_specular_contribution.py` & `tmart-2.3.2/tests/test_specular_contribution.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tests/test_typical_ocean.py` & `tmart-2.3.2/tests/test_typical_ocean.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tests/test_whales_SR.py` & `tmart-2.3.2/tests/test_whales_SR.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/AEC.py` & `tmart-2.3.2/tmart/AEC/AEC.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/__init__.py` & `tmart-2.3.2/tmart/AEC/__init__.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/anci_download.py` & `tmart-2.3.2/tmart/AEC/anci_download.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/anci_get_AER.py` & `tmart-2.3.2/tmart/AEC/anci_get_AER.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/anci_get_OWV.py` & `tmart-2.3.2/tmart/AEC/anci_get_OWV.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/anci_list_files.py` & `tmart-2.3.2/tmart/AEC/anci_list_files.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/compute_gas_transmittance.py` & `tmart-2.3.2/tmart/AEC/compute_gas_transmittance.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/compute_masks.py` & `tmart-2.3.2/tmart/AEC/compute_masks.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/fillnan.py` & `tmart-2.3.2/tmart/AEC/fillnan.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/get_AOT.py` & `tmart-2.3.2/tmart/AEC/get_AOT.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/get_ancillary.py` & `tmart-2.3.2/tmart/AEC/get_ancillary.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/get_parameters.py` & `tmart-2.3.2/tmart/AEC/get_parameters.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/identify_sensor.py` & `tmart-2.3.2/tmart/AEC/identify_sensor.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/irradiance_correction.py` & `tmart-2.3.2/tmart/AEC/irradiance_correction.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/read_PRISMA_north.py` & `tmart-2.3.2/tmart/AEC/read_PRISMA_north.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/read_PRISMA_vaa.py` & `tmart-2.3.2/tmart/AEC/read_PRISMA_vaa.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/read_config.py` & `tmart-2.3.2/tmart/AEC/read_config.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/read_metadata_Landsat.py` & `tmart-2.3.2/tmart/AEC/read_metadata_Landsat.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/read_metadata_S2.py` & `tmart-2.3.2/tmart/AEC/read_metadata_S2.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/read_xml_S2.py` & `tmart-2.3.2/tmart/AEC/read_xml_S2.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/read_xml_S2_scene.py` & `tmart-2.3.2/tmart/AEC/read_xml_S2_scene.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/AEC/run.py` & `tmart-2.3.2/tmart/AEC/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 # TMart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # Overall control of AEC
 
-def run(file, username, password, overwrite=False, AOT = 'MERRA2', n_photon = 100_000):
+def run(file, username, password, overwrite=False, AOT = 'MERRA2', n_photon = 100_000, AOT_offset = 0.0):
     '''Run adjacency-effect correction on satellite files. See 'Introduction - Adjacency-Effect Correction' for detailed instructions.
     
     Arguments:
         
     * ``file`` -- String. Path to satellite files. For L8/S2: provide path to the folder. For PRISMA: provide ACOLITE L1R file. 
     * ``username`` -- String. Username of EarthData account.
     * ``password`` -- String. Password of EarthData account.
     * ``overwrite`` -- Boolean. If overwrite the existing files. The default is False and it creates a folder in the same directory that starts with AEC in the name
-    * ``AOT`` -- Float. AOT at 550nm, calculated in T-Mart if not specified. 'MERRA2' ancillary data is the default option. 
-    * ``n_photon`` -- Int. Number of photons in each T-Mart run, 100_000 is recommended for accurate results.   
+    * ``AOT`` -- Float. AOT at 550nm. 'NIR': calculate in T-Mart. 'MERRA2': use ancillary data (default).
+    * ``n_photon`` -- Int. Number of photons in each T-Mart run, 100_000 is recommended for accurate results.
+    * ``AOT_offset`` -- Float. Value added to AOT at 550nm. If resulted AOT is negative, it will be corrected to 0.
 
     Example usage::
         
         file = 'user/test/S2A_MSIL1C_20160812T143752_N0204_R096_T20MKB_20160812T143749.SAFE'
         username = 'abcdef'
         password = '123456'
         
@@ -96,21 +97,22 @@
             self.console.flush()
             self.file.flush()
 
     sys.stdout = Logger(log_file)
     print('T-Mart version: ' + str(version('tmart')))
     print('System time: ' + time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(time.time())))
     print('File: ' + str(file))
+    print('AOT_offset: ' + str(AOT_offset))
     
-    # S2/L8
+    # S2/L89
     if file_is_dir: 
-        tmart_out = tmart.AEC.run_regular(file, username, password, AOT, n_photon, AEC_record, basename_before_period)
+        tmart_out = tmart.AEC.run_regular(file, username, password, AOT, AOT_offset, n_photon, AEC_record, basename_before_period)
     # ACOLITE L1R 
     else:
-        tmart_out = tmart.AEC.run_acoliteL1R(file, username, password, AOT, n_photon, AEC_record, basename_before_period)
+        tmart_out = tmart.AEC.run_acoliteL1R(file, username, password, AOT, AOT_offset, n_photon, AEC_record, basename_before_period)
     
     # Stop logging 
     sys.stdout = orig_stdout
 
     return tmart_out
```

### Comparing `tmart-2.3.1/tmart/AEC/run_acoliteL1R.py` & `tmart-2.3.2/tmart/AEC/run_acoliteL1R.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 # TMart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # Run on ACOLITE L1R files, currently supports PRSIMA only 
 
-
-def run_acoliteL1R(file, username, password, AOT, n_photon, AEC_record, basename):
+def run_acoliteL1R(file, username, password, AOT, AOT_offset, n_photon, AEC_record, basename):
  
     import tmart
     import sys, os, time
     import netCDF4 as nc4
     import numpy as np
     import scipy
         
@@ -89,22 +88,25 @@
         mask_highTOA = np.logical_or(mask_highTOA, image_highTOA > float(config['mask_highTOA_threshold']))
     
     # Combine highTOA and SWIR masks, original resolution 
     mask_all = np.logical_or(mask_highTOA, mask_SWIR)
     
     
     # AOT
-    if AOT == None:
+    if AOT == 'NIR':
         sys.exit('The default estimating AOT from the NIR band is not tested on PRISMA data, please use MERRA2 or user input instead.')
     elif AOT == 'MERRA2':
         AOT = anci['AOT_MERRA2']
         print('\nUsing AOT from MERRA2: ' + str(AOT))
     else:
         print('\nUser input AOT: ' + str(AOT))
     
+    # Add offset
+    AOT = max(0, AOT + AOT_offset)
+    
     # Write atm information
     tmart.AEC.write_atm_info(metadata['file'], basename, anci, AOT)
     print('\nWrote aerosol and atmosphere information.')
     
     
     ### T-Mart calculate correction parameters
```

### Comparing `tmart-2.3.1/tmart/AEC/run_regular.py` & `tmart-2.3.2/tmart/AEC/run_regular.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,30 +5,27 @@
 # TMart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # Run on Landsat and Sentinel series 
 
-def run_regular(file, username, password, AOT, n_photon, AEC_record, basename): 
+def run_regular(file, username, password, AOT, AOT_offset, n_photon, AEC_record, basename): 
  
     import tmart
     import sys, os
     
     # Read configuration
     config = tmart.AEC.read_config()
 
     # Identify sensor
     print('\nReading image files: ')
     print(file)
     sensor = tmart.AEC.identify_sensor(file)
     
-    
-    print('\ntesting')
-    
     # Extract metadata
     if sensor == 'S2A' or sensor == 'S2B':
         metadata = tmart.AEC.read_metadata_S2(file, config, sensor)
     elif sensor == 'L8' or sensor == 'L9':
         metadata = tmart.AEC.read_metadata_Landsat(file, config, sensor)
     else: sys.exit('Warning: unrecognized sensor')
     
@@ -45,23 +42,26 @@
     # Compute cloud and non-Water masks 
     print('\nComputing masks: ')
     mask_cloud = tmart.AEC.compute_masks(metadata, config, 'cloud')
     mask_all   = tmart.AEC.compute_masks(metadata, config, 'all')   
     print('Done')
     
     # AOT
-    if AOT == None:
+    if AOT == 'NIR':
         print('\nEstimating AOT from the NIR band: ')
         AOT = tmart.AEC.get_AOT(metadata, config, anci, mask_cloud, mask_all, n_photon)
     elif AOT == 'MERRA2':
         AOT = anci['AOT_MERRA2']
         print('\nUsing AOT from MERRA2: ' + str(AOT))
     else:
         print('\nUser input AOT: ' + str(AOT))
     
+    # Add offset
+    AOT = max(0, AOT + AOT_offset)
+    
     # Write atm information
     tmart.AEC.write_atm_info(file, basename, anci, AOT)
     print('\nWrote aerosol and atmosphere information.')
     
     # Make a record file for AEC 
     file_AEC_record = open(AEC_record,"w")
     file_AEC_record.flush()
```

### Comparing `tmart-2.3.1/tmart/AEC/write_atm_info.py` & `tmart-2.3.2/tmart/AEC/write_atm_info.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/Aerosol.py` & `tmart-2.3.2/tmart/Aerosol.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/Atmosphere.py` & `tmart-2.3.2/tmart/Atmosphere.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/Surface.py` & `tmart-2.3.2/tmart/Surface.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/Tmart.py` & `tmart-2.3.2/tmart/Tmart.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/Tmart2.py` & `tmart-2.3.2/tmart/Tmart2.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/__init__.py` & `tmart-2.3.2/tmart/__init__.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/ancillary/aerosolSPF/BiomassBurning.csv` & `tmart-2.3.2/tmart/ancillary/aerosolSPF/BiomassBurning.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/ancillary/aerosolSPF/Continental.csv` & `tmart-2.3.2/tmart/ancillary/aerosolSPF/Continental.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/ancillary/aerosolSPF/Desert.csv` & `tmart-2.3.2/tmart/ancillary/aerosolSPF/Desert.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/ancillary/aerosolSPF/Maritime.csv` & `tmart-2.3.2/tmart/ancillary/aerosolSPF/Maritime.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/ancillary/aerosolSPF/Stratospheric.csv` & `tmart-2.3.2/tmart/ancillary/aerosolSPF/Stratospheric.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/ancillary/aerosolSPF/Urban.csv` & `tmart-2.3.2/tmart/ancillary/aerosolSPF/Urban.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/ancillary/conifer_forest.csv` & `tmart-2.3.2/tmart/ancillary/conifer_forest.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/ancillary/dry_beach_sand.csv` & `tmart-2.3.2/tmart/ancillary/dry_beach_sand.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/ancillary/lawn_grass.csv` & `tmart-2.3.2/tmart/ancillary/lawn_grass.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/ancillary/soil.csv` & `tmart-2.3.2/tmart/ancillary/soil.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/ancillary/vegetation.csv` & `tmart-2.3.2/tmart/ancillary/vegetation.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/ancillary/water_chl1.csv` & `tmart-2.3.2/tmart/ancillary/water_chl1.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/ancillary/wet_beach_sand.csv` & `tmart-2.3.2/tmart/ancillary/wet_beach_sand.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/config/config.txt` & `tmart-2.3.2/tmart/config/config.txt`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/surface_rho/calculate.py` & `tmart-2.3.2/tmart/surface_rho/calculate.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/tm_OT.py` & `tmart-2.3.2/tmart/tm_OT.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/tm_calcref.py` & `tmart-2.3.2/tmart/tm_calcref.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/tm_geometry.py` & `tmart-2.3.2/tmart/tm_geometry.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/tm_intersect.py` & `tmart-2.3.2/tmart/tm_intersect.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/tm_move.py` & `tmart-2.3.2/tmart/tm_move.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/tm_sampling.py` & `tmart-2.3.2/tmart/tm_sampling.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart/tm_water.py` & `tmart-2.3.2/tmart/tm_water.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.1/tmart.egg-info/PKG-INFO` & `tmart-2.3.2/tmart.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmart
-Version: 2.3.1
+Version: 2.3.2
 Summary: Modelling and correcting for the adjacency effect in aquatic remote sensing
 Author: Yulun Wu
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
@@ -60,15 +60,15 @@
 
 ```bash
 pip3 install tmart
 ```
 
 ## Quick Start: Adjacency-Effect Correction 
 
-T-Mart supports adjacency-effect correction for Sentinel-2 MSI and Landsat 8 OLI products. Correction is performed directly on level-1 products therefore can be followed by any amtospheric-correction tools. Minimal inputs are: 
+T-Mart supports adjacency-effect correction for Sentinel-2 MSI and Landsat 8/9 OLI/OLI-2 products. Correction is performed directly on level-1 products therefore can be followed by any amtospheric-correction tools. Minimal inputs are: 
 
 ```python
 import tmart
 file = 'user/test/S2A_MSIL1C_20160812T143752_N0204_R096_T20MKB_20160812T143749.SAFE'
 
 # NASA EarthData Credentials, OB.DAAC Data Access needs to be approved
 username = 'abcdef'
@@ -100,25 +100,24 @@
 my_surface = tmart.Surface(DEM = image_DEM,
                            reflectance = image_reflectance,
                            isWater = image_isWater,
                            cell_size = 10_000)  
                                
 ### Atmosphere ###
 atm_profile = AtmosProfile.PredefinedType(AtmosProfile.MidlatitudeSummer) 
-aerosol_type = 'Maritime'  
-my_atm = tmart.Atmosphere(atm_profile, aot550 = 0, aerosol_type = 'Maritime'  )
+my_atm = tmart.Atmosphere(atm_profile, aot550 = 0, aerosol_type = 'Maritime')
 
 ### Create T-Mart Object ###
 my_tmart = tmart.Tmart(Surface = my_surface, Atmosphere= my_atm, shadow=False)
 my_tmart.set_geometry(sensor_coords=[51,50,130_000], 
                       target_pt_direction=[180,0],
                       sun_dir=[0,0])
 
 ### Multiprocessing needs to be wrapped in 'if __name__ == "__main__":' for Windows systems. 
-### This can be skipped for Linux-based systems. 
+### This can be skipped for Unix-based systems. 
 if __name__ == "__main__":
     results = my_tmart.run(wl=wl, band=None, n_photon=10_000)
     
     # Calculate reflectances using recorded photon information 
     R = tmart.calc_ref(results)
     for k, v in R.items():
         print(k, '     ' , v)
```

### Comparing `tmart-2.3.1/tmart.egg-info/SOURCES.txt` & `tmart-2.3.2/tmart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

