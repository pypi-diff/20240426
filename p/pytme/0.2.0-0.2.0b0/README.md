# Comparing `tmp/pytme-0.2.0.tar.gz` & `tmp/pytme-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytme-0.2.0.tar", last modified: Fri Apr 26 12:09:08 2024, max compression
+gzip compressed data, was "pytme-0.2.0b0.tar", last modified: Sat Apr 20 17:25:09 2024, max compression
```

## Comparing `pytme-0.2.0.tar` & `pytme-0.2.0b0.tar`

### file list

```diff
@@ -1,77 +1,70 @@
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-26 12:09:08.770971 pytme-0.2.0/
--rw-r--r--   0 vmaurer    (502) staff       (20)    18467 2023-10-21 17:18:54.000000 pytme-0.2.0/LICENSE
--rw-r--r--   0 vmaurer    (502) staff       (20)     1388 2024-04-25 20:49:56.000000 pytme-0.2.0/MANIFEST.in
--rw-r--r--   0 vmaurer    (502) staff       (20)     2156 2024-04-26 12:09:08.770765 pytme-0.2.0/PKG-INFO
--rw-r--r--   0 vmaurer    (502) staff       (20)     1348 2024-04-25 20:49:56.000000 pytme-0.2.0/README.md
--rw-r--r--   0 vmaurer    (502) staff       (20)     1237 2024-04-25 20:49:56.000000 pytme-0.2.0/pyproject.toml
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-26 12:09:08.770502 pytme-0.2.0/pytme.egg-info/
--rw-r--r--   0 vmaurer    (502) staff       (20)     1493 2024-04-26 12:09:08.000000 pytme-0.2.0/pytme.egg-info/SOURCES.txt
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-26 12:09:08.683495 pytme-0.2.0/scripts/
--rw-r--r--   0 vmaurer    (502) staff       (20)        0 2023-12-11 19:10:01.000000 pytme-0.2.0/scripts/__init__.py
--rwxr-xr-x   0 vmaurer    (502) staff       (20)     2768 2024-01-17 20:33:54.000000 pytme-0.2.0/scripts/estimate_ram_usage.py
--rwxr-xr-x   0 vmaurer    (502) staff       (20)     6871 2024-04-12 21:15:08.000000 pytme-0.2.0/scripts/extract_candidates.py
--rwxr-xr-x   0 vmaurer    (502) staff       (20)    35497 2024-04-25 12:52:58.000000 pytme-0.2.0/scripts/match_template.py
--rwxr-xr-x   0 vmaurer    (502) staff       (20)    35428 2024-04-25 10:36:56.000000 pytme-0.2.0/scripts/match_template_filters.py
--rwxr-xr-x   0 vmaurer    (502) staff       (20)    21012 2024-04-12 21:11:31.000000 pytme-0.2.0/scripts/postprocess.py
--rwxr-xr-x   0 vmaurer    (502) staff       (20)     2528 2023-10-17 21:34:50.000000 pytme-0.2.0/scripts/preprocess.py
--rwxr-xr-x   0 vmaurer    (502) staff       (20)    35190 2024-04-04 15:36:03.000000 pytme-0.2.0/scripts/preprocessor_gui.py
--rwxr-xr-x   0 vmaurer    (502) staff       (20)     7077 2024-03-04 16:26:50.000000 pytme-0.2.0/scripts/refine_matches.py
--rw-r--r--   0 vmaurer    (502) staff       (20)       38 2024-04-26 12:09:08.771011 pytme-0.2.0/setup.cfg
--rw-r--r--   0 vmaurer    (502) staff       (20)     1846 2024-04-25 20:49:56.000000 pytme-0.2.0/setup.py
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-26 12:09:08.683837 pytme-0.2.0/src/
--rw-r--r--   0 vmaurer    (502) staff       (20)    12912 2024-04-07 20:40:48.000000 pytme-0.2.0/src/extensions.cpp
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-26 12:09:08.691440 pytme-0.2.0/tme/
--rw-r--r--   0 vmaurer    (502) staff       (20)      251 2024-04-17 07:48:39.000000 pytme-0.2.0/tme/__init__.py
--rw-r--r--   0 vmaurer    (502) staff       (20)       22 2024-04-25 20:48:34.000000 pytme-0.2.0/tme/__version__.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    55480 2024-04-25 11:30:11.000000 pytme-0.2.0/tme/analyzer.py
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-26 12:09:08.693551 pytme-0.2.0/tme/backends/
--rw-r--r--   0 vmaurer    (502) staff       (20)     4366 2024-01-17 13:29:37.000000 pytme-0.2.0/tme/backends/__init__.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    13145 2024-04-20 16:51:24.000000 pytme-0.2.0/tme/backends/cupy_backend.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    29311 2024-01-17 20:33:54.000000 pytme-0.2.0/tme/backends/matching_backend.py
--rw-r--r--   0 vmaurer    (502) staff       (20)     8467 2024-01-17 20:33:54.000000 pytme-0.2.0/tme/backends/mlx_backend.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    27408 2024-04-23 20:22:10.000000 pytme-0.2.0/tme/backends/npfftw_backend.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    18293 2024-04-20 12:48:41.000000 pytme-0.2.0/tme/backends/pytorch_backend.py
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-26 12:09:08.764978 pytme-0.2.0/tme/data/
--rw-r--r--   0 vmaurer    (502) staff       (20)        0 2023-10-21 17:05:05.000000 pytme-0.2.0/tme/data/__init__.py
--rw-r--r--   0 vmaurer    (502) staff       (20)   296768 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c48n309.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)   506048 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c48n527.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)     8768 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c48n9.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)     1088 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c48u1.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  1107008 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c48u1153.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  1153088 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c48u1201.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  1575488 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c48u1641.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)   173888 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c48u181.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  2130368 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c48u2219.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)    26048 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c48u27.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  2829248 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c48u2947.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  3583808 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c48u3733.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  4559168 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c48u4749.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  5643968 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c48u5879.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  6826688 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c48u7111.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)   782528 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c48u815.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)    79808 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c48u83.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  8303168 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c48u8649.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)     2528 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c600v.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)    14528 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/c600vc.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)      750 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/metadata.yaml
--rwxr-xr-x   0 vmaurer    (502) staff       (20)     1333 2023-03-19 10:37:24.000000 pytme-0.2.0/tme/data/quat_to_numpy.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    88091 2024-04-23 20:35:14.000000 pytme-0.2.0/tme/density.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    23625 2023-10-17 21:31:49.000000 pytme-0.2.0/tme/helpers.py
--rw-r--r--   0 vmaurer    (502) staff       (20)     6725 2024-03-29 15:18:59.000000 pytme-0.2.0/tme/matching_constrained.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    24218 2024-04-25 11:29:35.000000 pytme-0.2.0/tme/matching_data.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    58993 2024-04-25 10:27:43.000000 pytme-0.2.0/tme/matching_exhaustive.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    11273 2024-04-05 10:38:07.000000 pytme-0.2.0/tme/matching_memory.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    41894 2024-04-20 21:05:56.000000 pytme-0.2.0/tme/matching_optimization.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    42520 2024-04-20 22:38:46.000000 pytme-0.2.0/tme/matching_utils.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    19118 2024-04-18 21:23:50.000000 pytme-0.2.0/tme/orientations.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    13887 2024-01-25 20:44:11.000000 pytme-0.2.0/tme/parser.py
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-26 12:09:08.770099 pytme-0.2.0/tme/preprocessing/
--rw-r--r--   0 vmaurer    (502) staff       (20)       98 2024-04-12 21:04:55.000000 pytme-0.2.0/tme/preprocessing/__init__.py
--rw-r--r--   0 vmaurer    (502) staff       (20)     4833 2024-04-25 20:09:00.000000 pytme-0.2.0/tme/preprocessing/_utils.py
--rw-r--r--   0 vmaurer    (502) staff       (20)      779 2024-04-25 20:08:57.000000 pytme-0.2.0/tme/preprocessing/composable_filter.py
--rw-r--r--   0 vmaurer    (502) staff       (20)     1321 2024-04-25 20:08:55.000000 pytme-0.2.0/tme/preprocessing/compose.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    10634 2024-04-25 20:08:51.000000 pytme-0.2.0/tme/preprocessing/frequency_filters.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    32661 2024-04-25 20:08:49.000000 pytme-0.2.0/tme/preprocessing/tilt_series.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    51111 2024-04-23 13:50:38.000000 pytme-0.2.0/tme/preprocessor.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    52465 2024-04-18 15:47:36.000000 pytme-0.2.0/tme/structure.py
--rw-r--r--   0 vmaurer    (502) staff       (20)      295 2024-01-17 13:38:48.000000 pytme-0.2.0/tme/types.py
+drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-20 17:25:09.230805 pytme-0.2.0b0/
+-rw-r--r--   0 vmaurer    (502) staff       (20)    18467 2023-10-21 17:18:54.000000 pytme-0.2.0b0/LICENSE
+-rw-r--r--   0 vmaurer    (502) staff       (20)     1411 2024-04-20 17:06:53.000000 pytme-0.2.0b0/MANIFEST.in
+-rw-r--r--   0 vmaurer    (502) staff       (20)     2163 2024-04-20 17:25:09.230580 pytme-0.2.0b0/PKG-INFO
+-rw-r--r--   0 vmaurer    (502) staff       (20)     1348 2024-04-20 17:06:53.000000 pytme-0.2.0b0/README.md
+-rw-r--r--   0 vmaurer    (502) staff       (20)     1243 2024-04-20 17:06:53.000000 pytme-0.2.0b0/pyproject.toml
+drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-20 17:25:09.230302 pytme-0.2.0b0/pytme.egg-info/
+-rw-r--r--   0 vmaurer    (502) staff       (20)     1295 2024-04-20 17:25:09.000000 pytme-0.2.0b0/pytme.egg-info/SOURCES.txt
+drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-20 17:25:09.152687 pytme-0.2.0b0/scripts/
+-rw-r--r--   0 vmaurer    (502) staff       (20)        0 2023-12-11 19:10:01.000000 pytme-0.2.0b0/scripts/__init__.py
+-rwxr-xr-x   0 vmaurer    (502) staff       (20)     2768 2024-01-17 20:33:54.000000 pytme-0.2.0b0/scripts/estimate_ram_usage.py
+-rwxr-xr-x   0 vmaurer    (502) staff       (20)     6871 2024-04-12 21:15:08.000000 pytme-0.2.0b0/scripts/extract_candidates.py
+-rwxr-xr-x   0 vmaurer    (502) staff       (20)    26664 2024-04-20 16:07:07.000000 pytme-0.2.0b0/scripts/match_template.py
+-rwxr-xr-x   0 vmaurer    (502) staff       (20)    28989 2024-04-12 21:04:56.000000 pytme-0.2.0b0/scripts/match_template_filters.py
+-rwxr-xr-x   0 vmaurer    (502) staff       (20)    21012 2024-04-12 21:11:31.000000 pytme-0.2.0b0/scripts/postprocess.py
+-rwxr-xr-x   0 vmaurer    (502) staff       (20)     2528 2023-10-17 21:34:50.000000 pytme-0.2.0b0/scripts/preprocess.py
+-rwxr-xr-x   0 vmaurer    (502) staff       (20)    35190 2024-04-04 15:36:03.000000 pytme-0.2.0b0/scripts/preprocessor_gui.py
+-rwxr-xr-x   0 vmaurer    (502) staff       (20)     7077 2024-03-04 16:26:50.000000 pytme-0.2.0b0/scripts/refine_matches.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)       38 2024-04-20 17:25:09.230847 pytme-0.2.0b0/setup.cfg
+-rw-r--r--   0 vmaurer    (502) staff       (20)     1846 2024-04-20 17:06:53.000000 pytme-0.2.0b0/setup.py
+drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-20 17:25:09.153081 pytme-0.2.0b0/src/
+-rw-r--r--   0 vmaurer    (502) staff       (20)    12912 2024-04-07 20:40:48.000000 pytme-0.2.0b0/src/extensions.cpp
+drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-20 17:25:09.156102 pytme-0.2.0b0/tme/
+-rw-r--r--   0 vmaurer    (502) staff       (20)      251 2024-04-17 07:48:39.000000 pytme-0.2.0b0/tme/__init__.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)       23 2024-04-20 16:16:07.000000 pytme-0.2.0b0/tme/__version__.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    55632 2024-04-20 14:56:49.000000 pytme-0.2.0b0/tme/analyzer.py
+drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-20 17:25:09.158240 pytme-0.2.0b0/tme/backends/
+-rw-r--r--   0 vmaurer    (502) staff       (20)     4366 2024-01-17 13:29:37.000000 pytme-0.2.0b0/tme/backends/__init__.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    13145 2024-04-20 16:51:24.000000 pytme-0.2.0b0/tme/backends/cupy_backend.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    29311 2024-01-17 20:33:54.000000 pytme-0.2.0b0/tme/backends/matching_backend.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)     8467 2024-01-17 20:33:54.000000 pytme-0.2.0b0/tme/backends/mlx_backend.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    27451 2024-04-20 12:48:22.000000 pytme-0.2.0b0/tme/backends/npfftw_backend.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    18293 2024-04-20 12:48:41.000000 pytme-0.2.0b0/tme/backends/pytorch_backend.py
+drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-20 17:25:09.228452 pytme-0.2.0b0/tme/data/
+-rw-r--r--   0 vmaurer    (502) staff       (20)        0 2023-10-21 17:05:05.000000 pytme-0.2.0b0/tme/data/__init__.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)   296768 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48n309.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)   506048 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48n527.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)     8768 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48n9.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)     1088 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u1.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  1107008 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u1153.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  1153088 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u1201.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  1575488 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u1641.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)   173888 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u181.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  2130368 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u2219.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)    26048 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u27.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  2829248 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u2947.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  3583808 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u3733.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  4559168 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u4749.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  5643968 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u5879.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  6826688 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u7111.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)   782528 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u815.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)    79808 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u83.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  8303168 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u8649.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)     2528 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c600v.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)    14528 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c600vc.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)      750 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/metadata.yaml
+-rwxr-xr-x   0 vmaurer    (502) staff       (20)     1333 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/quat_to_numpy.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    87856 2024-04-20 16:08:44.000000 pytme-0.2.0b0/tme/density.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    23625 2023-10-17 21:31:49.000000 pytme-0.2.0b0/tme/helpers.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)     6725 2024-03-29 15:18:59.000000 pytme-0.2.0b0/tme/matching_constrained.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    24135 2024-04-20 13:45:53.000000 pytme-0.2.0b0/tme/matching_data.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    59531 2024-04-20 16:09:35.000000 pytme-0.2.0b0/tme/matching_exhaustive.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    11273 2024-04-05 10:38:07.000000 pytme-0.2.0b0/tme/matching_memory.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    41138 2024-04-18 21:23:50.000000 pytme-0.2.0b0/tme/matching_optimization.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    42504 2024-04-20 16:45:46.000000 pytme-0.2.0b0/tme/matching_utils.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    19118 2024-04-18 21:23:50.000000 pytme-0.2.0b0/tme/orientations.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    13887 2024-01-25 20:44:11.000000 pytme-0.2.0b0/tme/parser.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    50760 2024-04-17 07:45:43.000000 pytme-0.2.0b0/tme/preprocessor.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    52465 2024-04-18 15:47:36.000000 pytme-0.2.0b0/tme/structure.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)      295 2024-01-17 13:38:48.000000 pytme-0.2.0b0/tme/types.py
```

### Comparing `pytme-0.2.0/LICENSE` & `pytme-0.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/MANIFEST.in` & `pytme-0.2.0b0/MANIFEST.in`

 * *Files 3% similar despite different names*

```diff
@@ -56,17 +56,18 @@
 prune target/
 
 # Other exclusions
 global-exclude .DS_Store
 global-exclude .gitconfig
 global-exclude *.pickle
 prune tme/temp
+prune tme/preprocessing
 global-exclude doc/compileApiReference.sh
 prune public
 global-exclude tme/matching_backend.py
 prune doc/_build
 prune doc/reference/api
 global-exclude tme/scoring.py
 global-exclude tme/package.py
 global-exclude tme/transforms.py
 global-exclude tme/tests/test_packaging.py
-global-exclude scripts/match_template_devel.py
+global-exclude scripts/match_template_devel.py
```

### Comparing `pytme-0.2.0/PKG-INFO` & `pytme-0.2.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytme
-Version: 0.2.0
+Version: 0.2.0b0
 Summary: Python Template Matching Engine
 Author: Valentin Maurer
 Author-email: Valentin Maurer <valentin.maurer@embl-hamburg.de>
 License: Proprietary
 Project-URL: Homepage, https://github.com/KosinskiLab/pyTME
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 Requires-Dist: PyWavelets>=1.2.0
 Requires-Dist: PyYAML>=6.0
 Requires-Dist: scikit-image>=0.19.0
 Requires-Dist: scikit_learn>=1.2.1
 Requires-Dist: scipy>=1.9.1
 Requires-Dist: pybind11
 Requires-Dist: psutil
-Requires-Dist: tifffile
+Requires-Dist: tifffile[all]
 Requires-Dist: h5py
 
 # Python Template Matching Engine (PyTME)
 
 A software for template matching on electron microscopy data.
 
 📖 **[Official Documentation](https://kosinskilab.github.io/pyTME/)** | 🚀 **[Installation Guide](https://kosinskilab.github.io/pyTME/quickstart/installation.html)** | 📚 **[API Reference](https://kosinskilab.github.io/pyTME/reference/index.html)**
```

### Comparing `pytme-0.2.0/README.md` & `pytme-0.2.0b0/README.md`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/pyproject.toml` & `pytme-0.2.0b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name="pytme"
 authors = [
   { name = "Valentin Maurer", email = "valentin.maurer@embl-hamburg.de" },
 ]
-version="0.2.0"
+version="0.2.0b"
 description="Python Template Matching Engine"
 readme="README.md"
 requires-python = ">=3.11"
 dependencies=[
     "mrcfile>=1.4.3",
     "numpy>=1.22.2",
     "pyfftw>=0.13.1",
@@ -19,15 +19,15 @@
     "PyWavelets>=1.2.0",
     "PyYAML>=6.0",
     "scikit-image>=0.19.0",
     "scikit_learn>=1.2.1",
     "scipy>=1.9.1",
     "pybind11",
     "psutil",
-    "tifffile",
+    "tifffile[all]",
     "h5py"
 ]
 license = {text = "Proprietary"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
```

### Comparing `pytme-0.2.0/pytme.egg-info/SOURCES.txt` & `pytme-0.2.0b0/pytme.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -53,14 +53,8 @@
 tme/data/c48u7111.npy
 tme/data/c48u815.npy
 tme/data/c48u83.npy
 tme/data/c48u8649.npy
 tme/data/c600v.npy
 tme/data/c600vc.npy
 tme/data/metadata.yaml
-tme/data/quat_to_numpy.py
-tme/preprocessing/__init__.py
-tme/preprocessing/_utils.py
-tme/preprocessing/composable_filter.py
-tme/preprocessing/compose.py
-tme/preprocessing/frequency_filters.py
-tme/preprocessing/tilt_series.py
+tme/data/quat_to_numpy.py
```

### Comparing `pytme-0.2.0/scripts/estimate_ram_usage.py` & `pytme-0.2.0b0/scripts/estimate_ram_usage.py`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/scripts/extract_candidates.py` & `pytme-0.2.0b0/scripts/extract_candidates.py`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/scripts/match_template.py` & `pytme-0.2.0b0/scripts/match_template_filters.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,36 +9,35 @@
 import argparse
 import warnings
 import importlib.util
 from sys import exit
 from time import time
 from typing import Tuple
 from copy import deepcopy
-from os.path import abspath, exists
+from os.path import abspath
 
 import numpy as np
 
 from tme import Density, __version__
 from tme.matching_utils import (
     get_rotation_matrices,
-    get_rotations_around_vector,
     compute_parallelization_schedule,
     euler_from_rotationmatrix,
     scramble_phases,
     generate_tempfile_name,
     write_pickle,
 )
 from tme.matching_exhaustive import scan_subsets, MATCHING_EXHAUSTIVE_REGISTER
 from tme.matching_data import MatchingData
 from tme.analyzer import (
     MaxScoreOverRotations,
     PeakCallerMaximumFilter,
 )
-from tme.backends import backend
 from tme.preprocessing import Compose
+from tme.backends import backend
 
 
 def get_func_fullname(func) -> str:
     """Returns the full name of the given function, including its module."""
     return f"<function '{func.__module__}.{func.__name__}'>"
 
 
@@ -149,160 +148,14 @@
 
     if data_mask:
         data_mask.adjust_box(box)
 
     return True
 
 
-def parse_rotation_logic(args, ndim):
-    if args.angular_sampling is not None:
-        rotations = get_rotation_matrices(
-            angular_sampling=args.angular_sampling,
-            dim=ndim,
-            use_optimized_set=not args.no_use_optimized_set,
-        )
-        if args.angular_sampling >= 180:
-            rotations = np.eye(ndim).reshape(1, ndim, ndim)
-        return rotations
-
-    if args.axis_sampling is None:
-        args.axis_sampling = args.cone_sampling
-
-    rotations = get_rotations_around_vector(
-        cone_angle=args.cone_angle,
-        cone_sampling=args.cone_sampling,
-        axis_angle=args.axis_angle,
-        axis_sampling=args.axis_sampling,
-        n_symmetry=args.axis_symmetry,
-    )
-    return rotations
-
-
-# TODO: Think about whether wedge mask should also be added to target
-# For now leave it at the cost of incorrect upper bound on the scores
-def setup_filter(args, template: Density, target: Density) -> Tuple[Compose, Compose]:
-    from tme.preprocessing import LinearWhiteningFilter, BandPassFilter
-    from tme.preprocessing.tilt_series import (
-        Wedge,
-        WedgeReconstructed,
-        ReconstructFromTilt,
-    )
-
-    template_filter, target_filter = [], []
-    if args.tilt_angles is not None:
-        try:
-            wedge = Wedge.from_file(args.tilt_angles)
-            wedge.weight_type = args.tilt_weighting
-            if args.tilt_weighting in ("angle", None) and args.ctf_file is None:
-                wedge = WedgeReconstructed(
-                    angles=wedge.angles, weight_wedge=args.tilt_weighting == "angle"
-                )
-        except FileNotFoundError:
-            tilt_step, create_continuous_wedge = None, True
-            tilt_start, tilt_stop = args.tilt_angles.split(",")
-            if ":" in tilt_stop:
-                create_continuous_wedge = False
-                tilt_stop, tilt_step = tilt_stop.split(":")
-            tilt_start, tilt_stop = float(tilt_start), float(tilt_stop)
-            tilt_angles = (tilt_start, tilt_stop)
-            if tilt_step is not None:
-                tilt_step = float(tilt_step)
-                tilt_angles = np.arange(
-                    -tilt_start, tilt_stop + tilt_step, tilt_step
-                ).tolist()
-
-            if args.tilt_weighting is not None and tilt_step is None:
-                raise ValueError(
-                    "Tilt weighting is not supported for continuous wedges."
-                )
-            if args.tilt_weighting not in ("angle", None):
-                raise ValueError(
-                    "Tilt weighting schemes other than 'angle' or 'None' require "
-                    "a specification of electron doses."
-                )
-
-            wedge = Wedge(
-                angles=tilt_angles,
-                opening_axis=args.wedge_axes[0],
-                tilt_axis=args.wedge_axes[1],
-                shape=None,
-                weight_type=None,
-                weights=np.ones_like(tilt_angles),
-            )
-            if args.tilt_weighting in ("angle", None) and args.ctf_file is None:
-                wedge = WedgeReconstructed(
-                    angles=tilt_angles,
-                    weight_wedge=args.tilt_weighting == "angle",
-                    create_continuous_wedge=create_continuous_wedge,
-                )
-
-        wedge.opening_axis = args.wedge_axes[0]
-        wedge.tilt_axis = args.wedge_axes[1]
-        wedge.sampling_rate = template.sampling_rate
-        template_filter.append(wedge)
-        if not isinstance(wedge, WedgeReconstructed):
-            template_filter.append(ReconstructFromTilt(
-                reconstruction_filter = args.reconstruction_filter
-            ))
-
-    if args.ctf_file is not None:
-        from tme.preprocessing.tilt_series import CTF
-
-        ctf = CTF.from_file(args.ctf_file)
-        n_tilts_ctfs, n_tils_angles = len(ctf.defocus_x), len(wedge.angles)
-        if n_tilts_ctfs != n_tils_angles:
-            raise ValueError(
-                f"CTF file contains {n_tilts_ctfs} micrographs, but match_template "
-                f"recieved {n_tils_angles} tilt angles. Expected one angle "
-                "per micrograph."
-            )
-        ctf.angles = wedge.angles
-        ctf.opening_axis, ctf.tilt_axis = args.wedge_axes
-
-        if isinstance(template_filter[-1], ReconstructFromTilt):
-            template_filter.insert(-1, ctf)
-        else:
-            template_filter.insert(0, ctf)
-            template_filter.insert(1, ReconstructFromTilt(
-                reconstruction_filter = args.reconstruction_filter
-            ))
-
-    if args.lowpass or args.highpass is not None:
-        lowpass, highpass = args.lowpass, args.highpass
-        if args.pass_format == "voxel":
-            if lowpass is not None:
-                lowpass = np.max(np.multiply(lowpass, template.sampling_rate))
-            if highpass is not None:
-                highpass = np.max(np.multiply(highpass, template.sampling_rate))
-        elif args.pass_format == "frequency":
-            if lowpass is not None:
-                lowpass = np.max(np.divide(template.sampling_rate, lowpass))
-            if highpass is not None:
-                highpass = np.max(np.divide(template.sampling_rate, highpass))
-
-        bandpass = BandPassFilter(
-            use_gaussian=args.no_pass_smooth,
-            lowpass=lowpass,
-            highpass=highpass,
-            sampling_rate=template.sampling_rate,
-        )
-        template_filter.append(bandpass)
-        target_filter.append(bandpass)
-
-    if args.whiten_spectrum:
-        whitening_filter = LinearWhiteningFilter()
-        template_filter.append(whitening_filter)
-        target_filter.append(whitening_filter)
-
-    template_filter = Compose(template_filter) if len(template_filter) else None
-    target_filter = Compose(target_filter) if len(target_filter) else None
-
-    return template_filter, target_filter
-
-
 def parse_args():
     parser = argparse.ArgumentParser(description="Perform template matching.")
 
     io_group = parser.add_argument_group("Input / Output")
     io_group.add_argument(
         "-m",
         "--target",
@@ -367,79 +220,21 @@
         dest="score",
         type=str,
         default="FLCSphericalMask",
         choices=list(MATCHING_EXHAUSTIVE_REGISTER.keys()),
         help="Template matching scoring function.",
     )
     scoring_group.add_argument(
-        "-p",
-        dest="peak_calling",
-        action="store_true",
-        default=False,
-        help="Perform peak calling instead of score aggregation.",
-    )
-
-    angular_group = parser.add_argument_group("Angular Sampling")
-    angular_exclusive = angular_group.add_mutually_exclusive_group(required=True)
-
-    angular_exclusive.add_argument(
         "-a",
         dest="angular_sampling",
         type=check_positive,
-        default=None,
-        help="Angular sampling rate using optimized rotational sets."
+        default=40.0,
+        help="Angular sampling rate for template matching. "
         "A lower number yields more rotations. Values >= 180 sample only the identity.",
     )
-    angular_exclusive.add_argument(
-        "--cone_angle",
-        dest="cone_angle",
-        type=check_positive,
-        default=None,
-        help="Half-angle of the cone to be sampled in degrees. Allows to sample a "
-        "narrow interval around a known orientation, e.g. for surface oversampling.",
-    )
-    angular_group.add_argument(
-        "--cone_sampling",
-        dest="cone_sampling",
-        type=check_positive,
-        default=None,
-        help="Sampling rate of the cone in degrees.",
-    )
-    angular_group.add_argument(
-        "--axis_angle",
-        dest="axis_angle",
-        type=check_positive,
-        default=360.0,
-        required=False,
-        help="Sampling angle along the z-axis of the cone. Defaults to 360.",
-    )
-    angular_group.add_argument(
-        "--axis_sampling",
-        dest="axis_sampling",
-        type=check_positive,
-        default=None,
-        required=False,
-        help="Sampling rate along the z-axis of the cone. Defaults to --cone_sampling.",
-    )
-    angular_group.add_argument(
-        "--axis_symmetry",
-        dest="axis_symmetry",
-        type=check_positive,
-        default=1,
-        required=False,
-        help="N-fold symmetry around z-axis of the cone.",
-    )
-    angular_group.add_argument(
-        "--no_use_optimized_set",
-        dest="no_use_optimized_set",
-        action="store_true",
-        default=False,
-        required=False,
-        help="Whether to use random uniform instead of optimized rotation sets.",
-    )
 
     computation_group = parser.add_argument_group("Computation")
     computation_group.add_argument(
         "-n",
         dest="cores",
         required=False,
         type=int,
@@ -478,14 +273,29 @@
         required=False,
         type=float,
         default=0.85,
         help="Fraction of available memory that can be used. Defaults to 0.85 and is "
         "ignored if --ram is set",
     )
     computation_group.add_argument(
+        "--use_mixed_precision",
+        dest="use_mixed_precision",
+        action="store_true",
+        default=False,
+        help="Use float16 for real values operations where possible.",
+    )
+    computation_group.add_argument(
+        "--use_memmap",
+        dest="use_memmap",
+        action="store_true",
+        default=False,
+        help="Use memmaps to offload large data objects to disk. "
+        "Particularly useful for large inputs in combination with --use_gpu.",
+    )
+    computation_group.add_argument(
         "--temp_directory",
         dest="temp_directory",
         default=None,
         help="Directory for temporary objects. Faster I/O improves runtime.",
     )
 
     filter_group = parser.add_argument_group("Filters")
@@ -502,85 +312,60 @@
         dest="highpass",
         type=float,
         required=False,
         help="Resolution to highpass filter template and target to in the same unit "
         "as the sampling rate of template and target (typically Ångstrom).",
     )
     filter_group.add_argument(
-        "--no_pass_smooth",
-        dest="no_pass_smooth",
-        action="store_false",
-        default=True,
-        help="Whether a hard edge filter should be used for --lowpass and --highpass."
-    )
-    filter_group.add_argument(
-        "--pass_format",
-        dest="pass_format",
-        type=str,
-        required=False,
-        choices=["sampling_rate", "voxel", "frequency"],
-        help="How values passed to --lowpass and --highpass should be interpreted. "
-        "By default, they are assumed to be in units of sampling rate, e.g. Ångstrom."
-    )
-    filter_group.add_argument(
         "--whiten_spectrum",
         dest="whiten_spectrum",
         action="store_true",
-        default=None,
+        default=False,
         help="Apply spectral whitening to template and target based on target spectrum.",
     )
     filter_group.add_argument(
         "--wedge_axes",
         dest="wedge_axes",
         type=str,
         required=False,
-        default=None,
+        default="0,2",
         help="Indices of wedge opening and tilt axis, e.g. 0,2 for a wedge that is open "
         "in z-direction and tilted over the x axis.",
     )
     filter_group.add_argument(
         "--tilt_angles",
         dest="tilt_angles",
         type=str,
         required=False,
         default=None,
-        help="Path to a tab-separated file containing the column angles and optionally "
-        " weights, or comma separated start and stop stage tilt angle, e.g. 50,45, which "
-        " yields a continuous wedge mask. Alternatively, a tilt step size can be "
-        "specified like 50,45:5.0 to sample 5.0 degree tilt angle steps.",
+        help="Path to a file with angles and corresponding doses, or comma separated "
+        "start and stop stage tilt angle, e.g. 50,45, which yields a continuous wedge "
+        "mask. Alternatively, a tilt step size can be specified like 50,45:5.0 to "
+        "sample 5.0 degree tilt angle steps.",
     )
     filter_group.add_argument(
         "--tilt_weighting",
         dest="tilt_weighting",
         type=str,
         required=False,
         choices=["angle", "relion", "grigorieff"],
         default=None,
         help="Weighting scheme used to reweight individual tilts. Available options: "
         "angle (cosine based weighting), "
-        "relion (relion formalism for wedge weighting) requires,"
+        "relion (relion formalism for wedge weighting ),"
         "grigorieff (exposure filter as defined in Grant and Grigorieff 2015)."
-        "relion and grigorieff require electron doses in --tilt_angles weights column.",
+        "",
     )
-    # filter_group.add_argument(
-    #     "--ctf_file",
-    #     dest="ctf_file",
-    #     type=str,
-    #     required=False,
-    #     default=None,
-    #     help="Path to a file with CTF parameters from CTFFIND4.",
-    # )
     filter_group.add_argument(
-        "--reconstruction_filter",
-        dest="reconstruction_filter",
+        "--ctf_file",
+        dest="ctf_file",
         type=str,
         required=False,
-        choices = ["ram-lak", "ramp", "shepp-logan", "cosine", "hamming"],
         default=None,
-        help="Filter applied when reconstructing (N+1)-D from N-D filters.",
+        help="Path to a file with CTF parameters.",
     )
 
     performance_group = parser.add_argument_group("Performance")
     performance_group.add_argument(
         "--cutoff_target",
         dest="cutoff_target",
         type=float,
@@ -624,47 +409,36 @@
         dest="interpolation_order",
         required=False,
         type=int,
         default=3,
         help="Spline interpolation used for template rotations. If less than zero "
         "no interpolation is performed.",
     )
-    performance_group.add_argument(
-        "--use_mixed_precision",
-        dest="use_mixed_precision",
-        action="store_true",
-        default=False,
-        help="Use float16 for real values operations where possible.",
-    )
-    performance_group.add_argument(
-        "--use_memmap",
-        dest="use_memmap",
-        action="store_true",
-        default=False,
-        help="Use memmaps to offload large data objects to disk. "
-        "Particularly useful for large inputs in combination with --use_gpu.",
-    )
 
     analyzer_group = parser.add_argument_group("Analyzer")
     analyzer_group.add_argument(
         "--score_threshold",
         dest="score_threshold",
         required=False,
         type=float,
         default=0,
         help="Minimum template matching scores to consider for analysis.",
     )
-
+    analyzer_group.add_argument(
+        "-p",
+        dest="peak_calling",
+        action="store_true",
+        default=False,
+        help="Perform peak calling instead of score aggregation.",
+    )
     args = parser.parse_args()
 
     if args.interpolation_order < 0:
         args.interpolation_order = None
 
-    args.ctf_file = None
-
     if args.temp_directory is None:
         default = abspath(".")
         if os.environ.get("TMPDIR", None) is not None:
             default = os.environ.get("TMPDIR")
         args.temp_directory = default
 
     os.environ["TMPDIR"] = args.temp_directory
@@ -689,32 +463,104 @@
                 "Assuming device 0.",
             )
             os.environ["CUDA_VISIBLE_DEVICES"] = "0"
         args.gpu_indices = [
             int(x) for x in os.environ["CUDA_VISIBLE_DEVICES"].split(",")
         ]
 
-    if args.tilt_angles is not None:
-        if args.wedge_axes is None:
-            raise ValueError("Need to specify --wedge_axes when --tilt_angles is set.")
-        if not exists(args.tilt_angles):
-            try:
-                float(args.tilt_angles.split(",")[0])
-            except ValueError:
-                raise ValueError(f"{args.tilt_angles} is not a file nor a range.")
+    if args.wedge_axes is not None:
+        args.wedge_axes = [int(x) for x in args.wedge_axes.split(",")]
 
-    if args.ctf_file is not None and args.tilt_angles is None:
-        raise ValueError("Need to specify --tilt_angles when --ctf_file is set.")
+    if args.tilt_angles is not None and args.wedge_axes is None:
+        raise ValueError("Wedge axes have to be specified with tilt angles.")
 
-    if args.wedge_axes is not None:
-        args.wedge_axes = tuple(int(i) for i in args.wedge_axes.split(","))
+    if args.ctf_file is not None and args.wedge_axes is None:
+        raise ValueError("Wedge axes have to be specified with CTF parameters.")
+    if args.ctf_file is not None and args.tilt_angles is None:
+        raise ValueError("Angles have to be specified with CTF parameters.")
 
     return args
 
 
+def setup_filter(args, template: Density, target: Density) -> Tuple[Compose, Compose]:
+    from tme.preprocessing import LinearWhiteningFilter, BandPassFilter
+
+    template_filter, target_filter = [], []
+    if args.tilt_angles is not None:
+        from tme.preprocessing.tilt_series import (
+            Wedge,
+            WedgeReconstructed,
+            ReconstructFromTilt,
+        )
+
+        try:
+            wedge = Wedge.from_file(args.tilt_angles)
+            wedge.weight_type = args.tilt_weighting
+        except FileNotFoundError:
+            tilt_step = None
+            tilt_start, tilt_stop = args.tilt_angles.split(",")
+            if ":" in tilt_stop:
+                tilt_stop, tilt_step = tilt_stop.split(":")
+            tilt_start, tilt_stop = float(tilt_start), float(tilt_stop)
+            tilt_angles = None
+            if tilt_step is not None:
+                tilt_step = float(tilt_step)
+                tilt_angles = np.arange(
+                    -tilt_start, tilt_stop + tilt_step, tilt_step
+                ).tolist()
+            wedge = WedgeReconstructed(
+                angles=tilt_angles,
+                start_tilt=tilt_start,
+                stop_tilt=tilt_stop,
+            )
+        wedge.opening_axis = args.wedge_axes[0]
+        wedge.tilt_axis = args.wedge_axes[1]
+        wedge.sampling_rate = template.sampling_rate
+        template_filter.append(wedge)
+        if not isinstance(wedge, WedgeReconstructed):
+            template_filter.append(ReconstructFromTilt())
+
+    if args.ctf_file is not None:
+        from tme.preprocessing.tilt_series import CTF
+
+        ctf = CTF.from_file(args.ctf_file)
+        ctf.tilt_axis = args.wedge_axes[1]
+        ctf.opening_axis = args.wedge_axes[0]
+        template_filter.append(ctf)
+        if isinstance(template_filter[-1], ReconstructFromTilt):
+            template_filter.insert(-1, ctf)
+        else:
+            template_filter.insert(0, ctf)
+            template_filter.isnert(1, ReconstructFromTilt())
+
+    if args.lowpass or args.highpass is not None:
+        from tme.preprocessing import BandPassFilter
+
+        bandpass = BandPassFilter(
+            use_gaussian=True,
+            lowpass=args.lowpass,
+            highpass=args.highpass,
+            sampling_rate=template.sampling_rate,
+        )
+        template_filter.append(bandpass)
+        target_filter.append(bandpass)
+
+    if args.whiten_spectrum:
+        from tme.preprocessing import LinearWhiteningFilter
+
+        whitening_filter = LinearWhiteningFilter()
+        template_filter.append(whitening_filter)
+        target_filter.append(whitening_filter)
+
+    template_filter = Compose(template_filter) if len(template_filter) else None
+    target_filter = Compose(target_filter) if len(target_filter) else None
+
+    return template_filter, target_filter
+
+
 def main():
     args = parse_args()
     print_entry()
 
     target = Density.from_file(args.target, use_memmap=True)
 
     try:
@@ -893,23 +739,34 @@
     if splits is None:
         print(
             "Found no suitable parallelization schedule. Consider increasing"
             " available RAM or decreasing number of cores."
         )
         exit(-1)
 
+    analyzer_args = {
+        "score_threshold": args.score_threshold,
+        "number_of_peaks": 1000,
+        "convolution_mode": "valid",
+        "use_memmap": args.use_memmap,
+    }
+
     matching_setup, matching_score = MATCHING_EXHAUSTIVE_REGISTER[args.score]
     matching_data = MatchingData(target=target, template=template.data)
-    matching_data.rotations = parse_rotation_logic(args=args, ndim=target.data.ndim)
+    matching_data.rotations = get_rotation_matrices(
+        angular_sampling=args.angular_sampling, dim=target.data.ndim
+    )
+    if args.angular_sampling >= 180:
+        ndim = target.data.ndim
+        matching_data.rotations = np.eye(ndim).reshape(1, ndim, ndim)
 
     template_filter, target_filter = setup_filter(args, template, target)
     matching_data.template_filter = template_filter
     matching_data.target_filter = target_filter
 
-    matching_data.template_filter = template_filter
     matching_data._invert_target = args.invert_target_contrast
     if target_mask is not None:
         matching_data.target_mask = target_mask
     if template_mask is not None:
         matching_data.template_mask = template_mask.data
 
     n_splits = np.prod(list(splits.values()))
@@ -937,43 +794,18 @@
 
     print_block(
         name="Template Matching Options",
         data=options,
         label_width=max(len(key) for key in options.keys()) + 2,
     )
 
-    filter_args = {
-        "Lowpass": args.lowpass,
-        "Highpass": args.highpass,
-        "Smooth Pass": args.no_pass_smooth,
-        "Pass Format" : args.pass_format,
-        "Spectral Whitening": args.whiten_spectrum,
-        "Wedge Axes": args.wedge_axes,
-        "Tilt Angles": args.tilt_angles,
-        "Tilt Weighting": args.tilt_weighting,
-        "CTF": args.ctf_file,
-    }
-    filter_args = {k: v for k, v in filter_args.items() if v is not None}
-    if len(filter_args):
-        print_block(
-            name="Filters",
-            data=filter_args,
-            label_width=max(len(key) for key in options.keys()) + 2,
-        )
-
-    analyzer_args = {
-        "score_threshold": args.score_threshold,
-        "number_of_peaks": 1000,
-        "convolution_mode": "valid",
-        "use_memmap": args.use_memmap,
-    }
-    analyzer_args = {"Analyzer": callback_class, **analyzer_args}
+    options = {"Analyzer": callback_class, **analyzer_args}
     print_block(
         name="Score Analysis Options",
-        data=analyzer_args,
+        data=options,
         label_width=max(len(key) for key in options.keys()) + 2,
     )
     print("\n" + "-" * 80)
 
     outer_jobs = f"{schedule[0]} job{'s' if schedule[0] > 1 else ''}"
     inner_jobs = f"{schedule[1]} core{'s' if schedule[1] > 1 else ''}"
     n_splits = f"{n_splits} split{'s' if n_splits > 1 else ''}"
@@ -1004,14 +836,15 @@
                 x: euler_from_rotationmatrix(
                     np.frombuffer(i, dtype=matching_data.rotations.dtype).reshape(
                         candidates[0].ndim, candidates[0].ndim
                     )
                 )
                 for i, x in candidates[3].items()
             }
+
     candidates.append((target.origin, template.origin, target.sampling_rate, args))
     write_pickle(data=candidates, filename=args.output)
 
     runtime = time() - start
     print(f"\nRuntime real: {runtime:.3f}s user: {(runtime * args.cores):.3f}s.")
```

### Comparing `pytme-0.2.0/scripts/postprocess.py` & `pytme-0.2.0b0/scripts/postprocess.py`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/scripts/preprocess.py` & `pytme-0.2.0b0/scripts/preprocess.py`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/scripts/preprocessor_gui.py` & `pytme-0.2.0b0/scripts/preprocessor_gui.py`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/scripts/refine_matches.py` & `pytme-0.2.0b0/scripts/refine_matches.py`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/setup.py` & `pytme-0.2.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/src/extensions.cpp` & `pytme-0.2.0b0/src/extensions.cpp`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/analyzer.py` & `pytme-0.2.0b0/tme/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,49 +404,54 @@
             peak_positions = backend.add(peak_positions, fourier_shift)
             backend.divide(peak_positions, score_space_shape).astype(int)
 
             backend.subtract(
                 peak_positions,
                 backend.multiply(
                     backend.divide(peak_positions, score_space_shape).astype(int),
-                    score_space_shape,
+                    score_space_shape
                 ),
-                out=peak_positions,
+                out = peak_positions
             )
 
         if convolution_mode is None:
             return None
 
         if convolution_mode == "full":
             output_shape = score_space_shape
         elif convolution_mode == "same":
             output_shape = targetshape
         elif convolution_mode == "valid":
             output_shape = backend.add(
                 backend.subtract(targetshape, templateshape),
-                backend.mod(templateshape, 2),
+                backend.mod(templateshape, 2)
             )
 
         output_shape = backend.to_backend_array(output_shape)
-        starts = backend.divide(backend.subtract(score_space_shape, output_shape), 2)
+        starts = backend.divide(
+            backend.subtract(score_space_shape, output_shape),
+            2
+        )
         starts = backend.astype(starts, int)
         stops = backend.add(starts, output_shape)
 
         valid_peaks = (
             backend.sum(
-                backend.multiply(peak_positions > starts, peak_positions <= stops),
+                backend.multiply(
+                    peak_positions > starts,
+                    peak_positions <= stops
+                ),
                 axis=1,
             )
             == peak_positions.shape[1]
         )
         self.peak_list[0] = backend.subtract(peak_positions, starts)
         self.peak_list = [x[valid_peaks] for x in self.peak_list]
         return self
 
-
 class PeakCallerSort(PeakCaller):
     """
     A :py:class:`PeakCaller` subclass that first selects ``number_of_peaks``
     highest scores and subsequently filters local maxima to suffice a distance
     from one another of ``min_distance``.
 
     """
@@ -1197,71 +1202,76 @@
         self.translation_offset = backend.astype(translation_offset, int)
         self.score_space_shape = score_space_shape
         self.rotation_space_dtype = rotation_space_dtype
         self.score_space_dtype = score_space_dtype
 
         self.use_memmap = use_memmap
         self.lock = Manager().Lock() if thread_safe else nullcontext()
-        self.lock_is_nullcontext = isinstance(
-            self.score_space, type(backend.zeros((1)))
-        )
+        self.lock_is_nullcontext = isinstance(self.score_space, type(backend.zeros((1))))
         self.observed_rotations = Manager().dict() if thread_safe else {}
 
-    def _postprocess(
-        self,
+
+    def _postprocess(self,
         fourier_shift,
         convolution_mode,
         targetshape,
         templateshape,
         shared_memory_handler=None,
-        **kwargs,
-    ):
+        **kwargs
+        ):
         internal_scores = backend.sharedarr_to_arr(
             shape=self.score_space_shape,
             dtype=self.score_space_dtype,
             shm=self.score_space,
         )
         internal_rotations = backend.sharedarr_to_arr(
             shape=self.score_space_shape,
             dtype=self.rotation_space_dtype,
             shm=self.rotations,
         )
 
         if fourier_shift is not None:
             axis = tuple(i for i in range(len(fourier_shift)))
             internal_scores = backend.roll(
-                internal_scores, shift=fourier_shift, axis=axis
+                internal_scores,
+                shift=fourier_shift,
+                axis=axis
             )
             internal_rotations = backend.roll(
-                internal_rotations, shift=fourier_shift, axis=axis
+                internal_rotations,
+                shift=fourier_shift,
+                axis=axis
             )
 
         if convolution_mode is not None:
             internal_scores = apply_convolution_mode(
                 internal_scores,
                 convolution_mode=convolution_mode,
                 s1=targetshape,
-                s2=templateshape,
+                s2=templateshape
             )
             internal_rotations = apply_convolution_mode(
                 internal_rotations,
                 convolution_mode=convolution_mode,
                 s1=targetshape,
-                s2=templateshape,
+                s2=templateshape
             )
 
         self.score_space_shape = internal_scores.shape
         self.score_space = backend.arr_to_sharedarr(
-            internal_scores, shared_memory_handler
+            internal_scores,
+            shared_memory_handler
         )
         self.rotations = backend.arr_to_sharedarr(
-            internal_rotations, shared_memory_handler
+            internal_rotations,
+            shared_memory_handler
         )
         return self
 
+
     def __iter__(self):
         internal_scores = backend.sharedarr_to_arr(
             shape=self.score_space_shape,
             dtype=self.score_space_dtype,
             shm=self.score_space,
         )
         internal_rotations = backend.sharedarr_to_arr(
@@ -1633,7 +1643,9 @@
         Returns
         -------
         str
             String representation of the rotation matrix.
         """
         rotation_string = "_".join(rotation_matrix.ravel().astype(str))
         return self._path_translation[rotation_string]
+
+
```

### Comparing `pytme-0.2.0/tme/backends/__init__.py` & `pytme-0.2.0b0/tme/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/backends/cupy_backend.py` & `pytme-0.2.0b0/tme/backends/cupy_backend.py`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/backends/matching_backend.py` & `pytme-0.2.0b0/tme/backends/matching_backend.py`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/backends/mlx_backend.py` & `pytme-0.2.0b0/tme/backends/mlx_backend.py`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/backends/npfftw_backend.py` & `pytme-0.2.0b0/tme/backends/npfftw_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -652,16 +652,18 @@
             out_offset = coordinates_rotated.min(axis=1)
             coordinates_rotated -= out_offset[:, None]
             out = np.zeros(coordinates_rotated.max(axis=1) + 1, dtype=arr.dtype)
 
         if rotate_mask:
             mask_rotated = mask_rotated.astype(int)
             if out_mask is None:
-                # mask_rotated -= out_offset[:, None]
-                out_mask = np.zeros(mask_rotated.max(axis=1) + 1, dtype=arr.dtype)
+                mask_rotated -= out_offset[:, None]
+                out_mask = np.zeros(
+                    coordinates_rotated.max(axis=1) + 1, dtype=arr.dtype
+                )
 
             in_box = np.logical_and(
                 mask_rotated < np.array(out_mask.shape)[:, None],
                 mask_rotated >= 0,
             ).min(axis=0)
             out_of_box = np.invert(in_box).sum()
             if out_of_box != 0:
```

### Comparing `pytme-0.2.0/tme/backends/pytorch_backend.py` & `pytme-0.2.0b0/tme/backends/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c48n309.npy` & `pytme-0.2.0b0/tme/data/c48n309.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c48n527.npy` & `pytme-0.2.0b0/tme/data/c48n527.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c48n9.npy` & `pytme-0.2.0b0/tme/data/c48n9.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c48u1.npy` & `pytme-0.2.0b0/tme/data/c48u1.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c48u1153.npy` & `pytme-0.2.0b0/tme/data/c48u1153.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c48u1201.npy` & `pytme-0.2.0b0/tme/data/c48u1201.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c48u1641.npy` & `pytme-0.2.0b0/tme/data/c48u1641.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c48u181.npy` & `pytme-0.2.0b0/tme/data/c48u181.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c48u2219.npy` & `pytme-0.2.0b0/tme/data/c48u2219.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c48u27.npy` & `pytme-0.2.0b0/tme/data/c48u27.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c48u2947.npy` & `pytme-0.2.0b0/tme/data/c48u2947.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c48u3733.npy` & `pytme-0.2.0b0/tme/data/c48u3733.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c48u4749.npy` & `pytme-0.2.0b0/tme/data/c48u4749.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c48u5879.npy` & `pytme-0.2.0b0/tme/data/c48u5879.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c48u7111.npy` & `pytme-0.2.0b0/tme/data/c48u7111.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c48u815.npy` & `pytme-0.2.0b0/tme/data/c48u815.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c48u83.npy` & `pytme-0.2.0b0/tme/data/c48u83.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c48u8649.npy` & `pytme-0.2.0b0/tme/data/c48u8649.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c600v.npy` & `pytme-0.2.0b0/tme/data/c600v.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/c600vc.npy` & `pytme-0.2.0b0/tme/data/c600vc.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/metadata.yaml` & `pytme-0.2.0b0/tme/data/metadata.yaml`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/data/quat_to_numpy.py` & `pytme-0.2.0b0/tme/data/quat_to_numpy.py`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/density.py` & `pytme-0.2.0b0/tme/density.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,15 +313,15 @@
                 "std": float(mrc.header.rms),
             }
 
         if is_gzipped(filename):
             if use_memmap:
                 warnings.warn(
                     f"Cannot open gzipped file {filename} as memmap."
-                    f" Please run 'gunzip {filename}' to use memmap functionality."
+                    f" Please gunzip {filename} to use memmap functionality."
                 )
             use_memmap = False
 
         if subset is not None:
             subset_shape = [x.stop - x.start for x in subset]
             if np.allclose(subset_shape, data_shape):
                 return cls._load_mrc(
@@ -1541,43 +1541,42 @@
         :py:meth:`Density.minimum_enclosing_box`
 
 
         Examples
         --------
         :py:meth:`Density.centered` returns a tuple containing a centered version
         of the current :py:class:`Density` instance, as well as an array with
-        translations. The translation corresponds to the shift between the original and
-        current center of mass.
+        translations. The translation corresponds to the shift that between the
+        center of mass and the center of the internal :py:attr:`Density.data` attribute.
 
         >>> import numpy as np
         >>> from tme import Density
         >>> dens = Density(np.ones((5,5)))
         >>> centered_dens, translation = dens.centered(0)
         >>> translation
-        array([-0.5, -0.5])
+        array([-4.4408921e-16,  4.4408921e-16])
 
         :py:meth:`Density.centered` extended the :py:attr:`Density.data` attribute
         of the current :py:class:`Density` instance and modified
         :py:attr:`Density.origin` accordingly.
 
         >>> centered_dens
-        Origin: (-1.0, -1.0), sampling_rate: (1, 1), Shape: (8, 8)
+        Origin: (-1.0, -1.0), sampling_rate: (1, 1), Shape: (7, 7)
 
-        :py:meth:`Density.centered` achieves centering via zero-padding and
-        transforming the internal :py:attr:`Density.data` attribute:
+        :py:meth:`Density.centered` achieves centering via zero-padding the
+        internal :py:attr:`Density.data` attribute:
 
         >>> centered_dens.data
-        array([[0.  , 0.  , 0.  , 0.  , 0.  , 0.  , 0.  , 0.  ],
-               [0.  , 0.25, 0.5 , 0.5 , 0.5 , 0.5 , 0.25, 0.  ],
-               [0.  , 0.5 , 1.  , 1.  , 1.  , 1.  , 0.5 , 0.  ],
-               [0.  , 0.5 , 1.  , 1.  , 1.  , 1.  , 0.5 , 0.  ],
-               [0.  , 0.5 , 1.  , 1.  , 1.  , 1.  , 0.5 , 0.  ],
-               [0.  , 0.5 , 1.  , 1.  , 1.  , 1.  , 0.5 , 0.  ],
-               [0.  , 0.25, 0.5 , 0.5 , 0.5 , 0.5 , 0.25, 0.  ],
-               [0.  , 0.  , 0.  , 0.  , 0.  , 0.  , 0.  , 0.  ]])
+        array([[0., 0., 0., 0., 0., 0., 0.],
+               [0., 1., 1., 1., 1., 1., 0.],
+               [0., 1., 1., 1., 1., 1., 0.],
+               [0., 1., 1., 1., 1., 1., 0.],
+               [0., 1., 1., 1., 1., 1., 0.],
+               [0., 1., 1., 1., 1., 1., 0.],
+               [0., 0., 0., 0., 0., 0., 0.]])
 
         `centered_dens` is sufficiently large to represent all rotations that
         could be applied to the :py:attr:`Density.data` attribute. Lets look
         at a random rotation obtained from
         :py:meth:`tme.matching_utils.get_rotation_matrices`.
 
         >>> from tme.matching_utils import get_rotation_matrices
@@ -1592,19 +1591,18 @@
         """
         ret = self.copy()
 
         box = ret.minimum_enclosing_box(cutoff=cutoff, use_geometric_center=False)
         ret.adjust_box(box)
 
         new_shape = np.maximum(ret.shape, self.shape)
-        new_shape = np.add(new_shape, np.mod(new_shape, 2))
         ret.pad(new_shape)
 
         center = self.center_of_mass(ret.data, cutoff)
-        shift = np.subtract(np.divide(np.subtract(ret.shape, 1), 2), center)
+        shift = np.subtract(np.divide(ret.shape, 2), center)
 
         ret = ret.rigid_transform(
             translation=shift,
             rotation_matrix=np.eye(ret.data.ndim),
             use_geometric_center=False,
             order=1,
         )
```

### Comparing `pytme-0.2.0/tme/helpers.py` & `pytme-0.2.0b0/tme/helpers.py`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/matching_constrained.py` & `pytme-0.2.0b0/tme/matching_constrained.py`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/matching_data.py` & `pytme-0.2.0b0/tme/matching_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -510,16 +510,14 @@
 
             if hasattr(self, "_batch_mask"):
                 batch_mask = backend.to_backend_array(self._batch_mask)
                 shape_diff[batch_mask] = 0
 
             backend.add(fourier_shift, shape_diff, out=fourier_shift)
 
-        fourier_shift = backend.astype(fourier_shift, backend._default_dtype_int)
-
         return fast_shape, fast_ft_shape, fourier_shift
 
     @property
     def rotations(self):
         """Return stored rotation matrices.."""
         return self._rotations
```

### Comparing `pytme-0.2.0/tme/matching_exhaustive.py` & `pytme-0.2.0b0/tme/matching_exhaustive.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,22 @@
 from multiprocessing.managers import SharedMemoryManager
 
 import numpy as np
 from scipy.ndimage import laplace
 
 from .analyzer import MaxScoreOverRotations
 from .matching_utils import (
+    apply_convolution_mode,
     handle_traceback,
     split_numpy_array_slices,
     conditional_execute,
 )
 from .matching_memory import MatchingMemoryUsage, MATCHING_MEMORY_REGISTRY
-from .preprocessing import Compose
+# from .preprocessing import Compose
+from .preprocessor import Preprocessor
 from .matching_data import MatchingData
 from .backends import backend
 from .types import NDArray, CallbackClass
 
 os.environ["MKL_NUM_THREADS"] = "1"
 os.environ["OMP_NUM_THREADS"] = "1"
 os.environ["PYFFTW_NUM_THREADS"] = "1"
@@ -1301,15 +1303,15 @@
             rotation_index=index,
             **callback_class_args,
         )
 
     return callback
 
 
-def _setup_template_filter_apply_target_filter(
+def _setup_template_filter(
     matching_data: MatchingData,
     rfftn: Callable,
     irfftn: Callable,
     fast_shape: Tuple[int],
     fast_ft_shape: Tuple[int],
 ):
     filter_template = isinstance(matching_data.template_filter, Compose)
@@ -1323,14 +1325,15 @@
         return template_filter
 
     target_temp = backend.astype(
         backend.topleft_pad(matching_data.target, fast_shape), backend._default_dtype
     )
     target_temp_ft = backend.preallocate_array(fast_ft_shape, backend._complex_dtype)
     rfftn(target_temp, target_temp_ft)
+
     if isinstance(matching_data.template_filter, Compose):
         template_filter = matching_data.template_filter(
             shape=fast_shape,
             return_real_fourier=True,
             shape_is_real_fourier=False,
             data_rfft=target_temp_ft,
         )
@@ -1430,37 +1433,37 @@
     shape_diff = backend.subtract(
         matching_data._output_target_shape, matching_data._output_template_shape
     )
     shape_diff = backend.multiply(shape_diff, ~matching_data._batch_mask)
     if backend.sum(shape_diff < 0) and not pad_fourier:
         warnings.warn(
             "Target is larger than template and Fourier padding is turned off."
-            " This can lead to shifted results. You can swap template and target, "
-            " zero-pad the target or turn off template centering."
+            " This can lead to shifted results. You can swap template and target, or"
+            " zero-pad the target."
         )
     fast_shape, fast_ft_shape, fourier_shift = matching_data.fourier_padding(
         pad_fourier=pad_fourier
     )
 
     callback_class_args["fourier_shift"] = fourier_shift
     rfftn, irfftn = backend.build_fft(
         fast_shape=fast_shape,
         fast_ft_shape=fast_ft_shape,
         real_dtype=matching_data._default_dtype,
         complex_dtype=matching_data._complex_dtype,
         fftargs=fftargs,
     )
 
-    template_filter = _setup_template_filter_apply_target_filter(
-        matching_data=matching_data,
-        rfftn=rfftn,
-        irfftn=irfftn,
-        fast_shape=fast_shape,
-        fast_ft_shape=fast_ft_shape,
-    )
+    # template_filter = _setup_template_filter(
+    #     matching_data=matching_data,
+    #     rfftn=rfftn,
+    #     irfftn=irfftn,
+    #     fast_shape=fast_shape,
+    #     fast_ft_shape=fast_ft_shape,
+    # )
 
     setup = matching_setup(
         rfftn=rfftn,
         irfftn=irfftn,
         template=matching_data.template,
         template_mask=matching_data.template_mask,
         target=matching_data.target,
@@ -1471,14 +1474,29 @@
         complex_dtype=matching_data._complex_dtype,
         callback_class=callback_class,
         callback_class_args=callback_class_args,
         **kwargs,
     )
     rfftn, irfftn = None, None
 
+
+    template_filter, preprocessor = None, Preprocessor()
+    for method, parameters in matching_data.template_filter.items():
+        parameters["shape"] = fast_shape
+        parameters["omit_negative_frequencies"] = True
+        out = preprocessor.apply_method(method=method, parameters=parameters)
+        if template_filter is None:
+            template_filter = out
+        np.multiply(template_filter, out, out=template_filter)
+
+    if template_filter is None:
+        template_filter = backend.full(
+            shape=(1,), fill_value=1, dtype=backend._default_dtype
+        )
+
     template_filter = backend.to_backend_array(template_filter)
     template_filter = backend.astype(template_filter, backend._default_dtype)
     template_filter_buffer = backend.arr_to_sharedarr(
         arr=template_filter,
         shared_memory_handler=kwargs.get("shared_memory_handler", None),
     )
     setup["template_filter"] = (
@@ -1498,14 +1516,15 @@
     callback_class_args = setup.pop("callback_class_args", callback_class_args)
     callback_classes = [callback_class for _ in range(n_callback_classes)]
 
     convolution_mode = "same"
     if backend.sum(backend.to_backend_array(matching_data._target_pad)) > 0:
         convolution_mode = "valid"
 
+
     callback_class_args["fourier_shift"] = fourier_shift
     callback_class_args["convolution_mode"] = convolution_mode
     callback_class_args["targetshape"] = setup["targetshape"]
     callback_class_args["templateshape"] = setup["templateshape"]
 
     if callback_class == MaxScoreOverRotations:
         callback_classes = [
@@ -1548,27 +1567,22 @@
             **setup,
         )
         for index, rotation in enumerate(rotation_list)
     )
 
     callbacks = callbacks[0:n_callback_classes]
     callbacks = [
-        tuple(
-            callback._postprocess(
-                fourier_shift=fourier_shift,
-                convolution_mode=convolution_mode,
-                targetshape=setup["targetshape"],
-                templateshape=setup["templateshape"],
-                shared_memory_handler=kwargs.get("shared_memory_handler", None),
-            )
-        )
-        if hasattr(callback, "_postprocess")
-        else tuple(callback)
-        for callback in callbacks
-        if callback is not None
+        tuple(callback._postprocess(
+            fourier_shift = fourier_shift,
+            convolution_mode = convolution_mode,
+            targetshape = setup["targetshape"],
+            templateshape = setup["templateshape"],
+            shared_memory_handler=kwargs.get("shared_memory_handler", None)
+        )) if hasattr(callback, "_postprocess") else tuple(callback)
+        for callback in callbacks if callback is not None
     ]
     backend.free_cache()
 
     merged_callback = None
     if callback_class is not None:
         merged_callback = callback_class.merge(
             callbacks,
```

### Comparing `pytme-0.2.0/tme/matching_memory.py` & `pytme-0.2.0b0/tme/matching_memory.py`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/matching_optimization.py` & `pytme-0.2.0b0/tme/matching_optimization.py`

 * *Files 1% similar despite different names*

```diff
@@ -517,41 +517,14 @@
         return self(
             transformed_coordinates=self.template_coordinates_rotated,
             transformed_coordinates_mask=self.template_mask_coordinates_rotated,
         )
 
 
 class FLC(_MatchDensityToDensity):
-    """
-    Computes a normalized cross-correlation score of a target f a template g
-    and a mask m:
-
-    .. math::
-
-        \\frac{CC(f, \\frac{g*m - \\overline{g*m}}{\\sigma_{g*m}})}
-        {N_m * \\sqrt{
-            \\frac{CC(f^2, m)}{N_m} - (\\frac{CC(f, m)}{N_m})^2}
-        }
-
-    Where:
-
-    .. math::
-
-        CC(f,g) = \\mathcal{F}^{-1}(\\mathcal{F}(f) \\cdot \\mathcal{F}(g)^*)
-
-    and Nm is the number of voxels within the template mask m.
-
-    References
-    ----------
-    .. [1]  W. Wan, S. Khavnekar, J. Wagner, P. Erdmann, and W. Baumeister
-            Microsc. Microanal. 26, 2516 (2020)
-    .. [2]  T. Hrabe, Y. Chen, S. Pfeffer, L. Kuhn Cuellar, A.-V. Mangold,
-            and F. Förster, J. Struct. Biol. 178, 177 (2012).
-    """
-
     __doc__ += _MatchDensityToDensity.__doc__
 
     def _post_init(self, **kwargs: Dict):
         if self.target_mask is not None:
             backend.multiply(self.target, self.target_mask, out=self.target)
 
         self.target_square = backend.square(self.target)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pytme-0.2.0/tme/matching_utils.py` & `pytme-0.2.0b0/tme/matching_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -682,15 +682,15 @@
         angles=rotation_aligning_vectors([1, 0, 0], vector, convention="zyx"),
         seq="zyx",
         degrees=True,
     )
 
     # phi, theta, psi
     axis_angle /= n_symmetry
-    phi_steps = np.maximum(np.round(axis_angle / axis_sampling), 1).astype(int)
+    phi_steps = np.max(np.round(axis_angle / axis_sampling), 1)
     phi = np.linspace(0, axis_angle, phi_steps + 1)[:-1]
     np.add(phi, angles_vector.as_euler("zyx", degrees=True)[0], out=phi)
     angles = np.stack(
         [radius * np.cos(theta), radius * np.sin(theta), np.zeros_like(radius)], axis=1
     )
     angles = np.repeat(angles, phi_steps, axis=0)
     angles[:, 2] = np.tile(phi, radius.size)
```

### Comparing `pytme-0.2.0/tme/orientations.py` & `pytme-0.2.0b0/tme/orientations.py`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/parser.py` & `pytme-0.2.0b0/tme/parser.py`

 * *Files identical despite different names*

### Comparing `pytme-0.2.0/tme/preprocessor.py` & `pytme-0.2.0b0/tme/preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 class Preprocessor:
     """
     Implements filtering operations on density arrays.
     """
 
     def apply_method(self, method: str, parameters: Dict):
         """
-        Invoke ``Preprocessor.method`` using ``parameters``.
+        Apply a method on the atomic structure.
 
         Parameters
         ----------
         method : str
             The name of the method to be used.
         parameters : dict
             The parameters for the specified method.
@@ -1131,15 +1131,14 @@
         stop_tilt: float,
         tilt_step: float,
         shape: Tuple[int],
         tilt_angles: Tuple[float] = None,
         opening_axis: int = 0,
         tilt_axis: int = 2,
         sigma: float = 0,
-        weights: float = 1,
         omit_negative_frequencies: bool = True,
     ) -> NDArray:
         """
         Create a wedge mask with the same shape as template by rotating a
         plane according to tilt angles. The DC component of the filter is at the origin.
 
         Parameters
@@ -1162,16 +1161,14 @@
         opening_axis : int, optional
             Axis running through the void defined by the wedge.
             - 0 for Z-axis
             - 1 for Y-axis
             - 2 for X-axis
         sigma : float, optional
             Standard deviation for Gaussian kernel used for smoothing the wedge.
-        weights : float, tuple of float
-            Weight of each element in the wedge. Defaults to one.
         omit_negative_frequencies : bool, optional
             Whether the wedge mask should omit negative frequencies, i.e. be
             applicable to symmetric Fourier transforms (see :obj:`numpy.fft.fftn`)
 
         Returns
         -------
         NDArray
@@ -1187,44 +1184,40 @@
         --------
         :py:meth:`Preprocessor.wedge_mask`
         :py:meth:`Preprocessor.continuous_wedge_mask`
         """
         if tilt_angles is None:
             tilt_angles = np.arange(-start_tilt, stop_tilt + tilt_step, tilt_step)
 
-        weights = np.asarray(weights)
-        weights = np.repeat(weights, tilt_angles.size // weights.size)
         plane = np.zeros((shape[opening_axis], shape[tilt_axis]), dtype=np.float32)
         subset = tuple(
             slice(None) if i != 0 else slice(x // 2, x // 2 + 1)
             for i, x in enumerate(plane.shape)
         )
+        plane[subset] = 1
         plane_rotated, wedge_volume = np.zeros_like(plane), np.zeros_like(plane)
         for index in range(tilt_angles.shape[0]):
             plane_rotated.fill(0)
-            plane[subset] = weights[index]
+
             rotation_matrix = euler_to_rotationmatrix((tilt_angles[index], 0))
             rotation_matrix = rotation_matrix[np.ix_((0, 1), (0, 1))]
 
             Density.rotate_array(
                 arr=plane,
                 rotation_matrix=rotation_matrix,
                 out=plane_rotated,
                 use_geometric_center=True,
                 order=1,
             )
             wedge_volume += plane_rotated
 
-        # Ramp filtering would be more accurate
-        np.fmin(wedge_volume, np.max(weights), wedge_volume)
-
-        if sigma > 0:
-            wedge_volume = self.gaussian_filter(
-                template=wedge_volume, sigma=sigma, fourier=False
-            )
+        wedge_volume = self.gaussian_filter(
+            template=wedge_volume, sigma=sigma, fourier=False
+        )
+        wedge_volume = np.where(wedge_volume > np.exp(-2), 1, 0)
 
         if opening_axis > tilt_axis:
             wedge_volume = np.moveaxis(wedge_volume, 1, 0)
 
         reshape_dimensions = tuple(
             x if i in (opening_axis, tilt_axis) else 1 for i, x in enumerate(shape)
         )
```

### Comparing `pytme-0.2.0/tme/structure.py` & `pytme-0.2.0b0/tme/structure.py`

 * *Files identical despite different names*

