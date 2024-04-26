# Comparing `tmp/ephysiopy-2.0.8.tar.gz` & `tmp/ephysiopy-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephysiopy-2.0.8.tar", last modified: Mon Jan 15 17:43:49 2024, max compression
+gzip compressed data, was "ephysiopy-2.0.9.tar", last modified: Wed Jan 17 14:20:15 2024, max compression
```

## Comparing `ephysiopy-2.0.8.tar` & `ephysiopy-2.0.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:43:49.431605 ephysiopy-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-01-15 17:43:49.431605 ephysiopy-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:43:49.427605 ephysiopy-2.0.8/ephysiopy/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:43:49.427605 ephysiopy-2.0.8/ephysiopy/axona/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/axona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21533 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/axona/axonaIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    13608 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/axona/file_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/axona/tetrode_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/axona/tintcolours.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:43:49.431605 ephysiopy-2.0.8/ephysiopy/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50965 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/common/binning.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/common/cluster_old.py
--rw-r--r--   0 runner    (1001) docker     (127)    21064 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/common/ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    41377 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/common/fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/common/gridcell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/common/mle_von_mises_vals.py
--rw-r--r--   0 runner    (1001) docker     (127)    48492 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/common/phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (127)    26453 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/common/rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (127)    45994 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/common/spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/common/statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:43:49.431605 ephysiopy-2.0.8/ephysiopy/format_converters/
--rw-r--r--   0 runner    (1001) docker     (127)    36244 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/format_converters/OE_Axona.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/format_converters/OE_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/format_converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:43:49.431605 ephysiopy-2.0.8/ephysiopy/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30059 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/io/recording.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:43:49.431605 ephysiopy-2.0.8/ephysiopy/openephys2py/
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/openephys2py/KiloSort.py
--rw-r--r--   0 runner    (1001) docker     (127)    10877 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/openephys2py/OESettings.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/openephys2py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:43:49.431605 ephysiopy-2.0.8/ephysiopy/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-01-15 17:43:43.000000 ephysiopy-2.0.8/ephysiopy/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-01-15 17:43:44.000000 ephysiopy-2.0.8/ephysiopy/tests/test_axona_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-01-15 17:43:44.000000 ephysiopy-2.0.8/ephysiopy/tests/test_axona_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-01-15 17:43:44.000000 ephysiopy-2.0.8/ephysiopy/tests/test_binning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-01-15 17:43:44.000000 ephysiopy-2.0.8/ephysiopy/tests/test_dacq2py.py
--rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-01-15 17:43:44.000000 ephysiopy-2.0.8/ephysiopy/tests/test_ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-01-15 17:43:44.000000 ephysiopy-2.0.8/ephysiopy/tests/test_fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-01-15 17:43:44.000000 ephysiopy-2.0.8/ephysiopy/tests/test_gridcell.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-15 17:43:44.000000 ephysiopy-2.0.8/ephysiopy/tests/test_openephys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-01-15 17:43:44.000000 ephysiopy-2.0.8/ephysiopy/tests/test_phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-01-15 17:43:44.000000 ephysiopy-2.0.8/ephysiopy/tests/test_rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-01-15 17:43:44.000000 ephysiopy-2.0.8/ephysiopy/tests/test_spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-01-15 17:43:44.000000 ephysiopy-2.0.8/ephysiopy/tests/test_statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-01-15 17:43:44.000000 ephysiopy-2.0.8/ephysiopy/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:43:49.431605 ephysiopy-2.0.8/ephysiopy/visualise/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 17:43:44.000000 ephysiopy-2.0.8/ephysiopy/visualise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52601 2024-01-15 17:43:44.000000 ephysiopy-2.0.8/ephysiopy/visualise/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:43:49.427605 ephysiopy-2.0.8/ephysiopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-01-15 17:43:49.000000 ephysiopy-2.0.8/ephysiopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-01-15 17:43:49.000000 ephysiopy-2.0.8/ephysiopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 17:43:49.000000 ephysiopy-2.0.8/ephysiopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-15 17:43:49.000000 ephysiopy-2.0.8/ephysiopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-15 17:43:49.000000 ephysiopy-2.0.8/ephysiopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-15 17:43:49.431605 ephysiopy-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-01-15 17:43:44.000000 ephysiopy-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 14:20:15.184084 ephysiopy-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-01-17 14:20:15.184084 ephysiopy-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 14:20:15.176083 ephysiopy-2.0.9/ephysiopy/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 14:20:15.176083 ephysiopy-2.0.9/ephysiopy/axona/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/axona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21533 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/axona/axonaIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13608 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/axona/file_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/axona/tetrode_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/axona/tintcolours.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 14:20:15.180084 ephysiopy-2.0.9/ephysiopy/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50965 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/common/binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/common/cluster_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21064 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/common/ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41377 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/common/fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/common/gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/common/mle_von_mises_vals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48492 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/common/phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26453 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/common/rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45994 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/common/spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/common/statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 14:20:15.180084 ephysiopy-2.0.9/ephysiopy/format_converters/
+-rw-r--r--   0 runner    (1001) docker     (127)    36244 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/format_converters/OE_Axona.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/format_converters/OE_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/format_converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 14:20:15.180084 ephysiopy-2.0.9/ephysiopy/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30059 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/io/recording.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 14:20:15.180084 ephysiopy-2.0.9/ephysiopy/openephys2py/
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/openephys2py/KiloSort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10877 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/openephys2py/OESettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/openephys2py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 14:20:15.180084 ephysiopy-2.0.9/ephysiopy/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-01-17 14:20:09.000000 ephysiopy-2.0.9/ephysiopy/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-01-17 14:20:10.000000 ephysiopy-2.0.9/ephysiopy/tests/test_axona_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-01-17 14:20:10.000000 ephysiopy-2.0.9/ephysiopy/tests/test_axona_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-01-17 14:20:10.000000 ephysiopy-2.0.9/ephysiopy/tests/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-01-17 14:20:10.000000 ephysiopy-2.0.9/ephysiopy/tests/test_dacq2py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-01-17 14:20:10.000000 ephysiopy-2.0.9/ephysiopy/tests/test_ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-01-17 14:20:10.000000 ephysiopy-2.0.9/ephysiopy/tests/test_fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-01-17 14:20:10.000000 ephysiopy-2.0.9/ephysiopy/tests/test_gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-17 14:20:10.000000 ephysiopy-2.0.9/ephysiopy/tests/test_openephys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-01-17 14:20:10.000000 ephysiopy-2.0.9/ephysiopy/tests/test_phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-01-17 14:20:10.000000 ephysiopy-2.0.9/ephysiopy/tests/test_rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-01-17 14:20:10.000000 ephysiopy-2.0.9/ephysiopy/tests/test_spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-01-17 14:20:10.000000 ephysiopy-2.0.9/ephysiopy/tests/test_statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-01-17 14:20:10.000000 ephysiopy-2.0.9/ephysiopy/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 14:20:15.184084 ephysiopy-2.0.9/ephysiopy/visualise/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 14:20:10.000000 ephysiopy-2.0.9/ephysiopy/visualise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52601 2024-01-17 14:20:10.000000 ephysiopy-2.0.9/ephysiopy/visualise/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 14:20:15.176083 ephysiopy-2.0.9/ephysiopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-01-17 14:20:15.000000 ephysiopy-2.0.9/ephysiopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-01-17 14:20:15.000000 ephysiopy-2.0.9/ephysiopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 14:20:15.000000 ephysiopy-2.0.9/ephysiopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-17 14:20:15.000000 ephysiopy-2.0.9/ephysiopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-17 14:20:15.000000 ephysiopy-2.0.9/ephysiopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-17 14:20:15.184084 ephysiopy-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-01-17 14:20:10.000000 ephysiopy-2.0.9/setup.py
```

### Comparing `ephysiopy-2.0.8/LICENSE` & `ephysiopy-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/PKG-INFO` & `ephysiopy-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 2.0.8
+Version: 2.0.9
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-2.0.8/README.md` & `ephysiopy-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/axona/axonaIO.py` & `ephysiopy-2.0.9/ephysiopy/axona/axonaIO.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/axona/file_headers.py` & `ephysiopy-2.0.9/ephysiopy/axona/file_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/axona/tetrode_dict.py` & `ephysiopy-2.0.9/ephysiopy/axona/tetrode_dict.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/axona/tintcolours.py` & `ephysiopy-2.0.9/ephysiopy/axona/tintcolours.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/common/binning.py` & `ephysiopy-2.0.9/ephysiopy/common/binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/common/cluster_old.py` & `ephysiopy-2.0.9/ephysiopy/common/cluster_old.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/common/ephys_generic.py` & `ephysiopy-2.0.9/ephysiopy/common/ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/common/fieldcalcs.py` & `ephysiopy-2.0.9/ephysiopy/common/fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/common/gridcell.py` & `ephysiopy-2.0.9/ephysiopy/common/gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/common/mle_von_mises_vals.py` & `ephysiopy-2.0.9/ephysiopy/common/mle_von_mises_vals.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/common/phasecoding.py` & `ephysiopy-2.0.9/ephysiopy/common/phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/common/rhythmicity.py` & `ephysiopy-2.0.9/ephysiopy/common/rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/common/spikecalcs.py` & `ephysiopy-2.0.9/ephysiopy/common/spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/common/statscalcs.py` & `ephysiopy-2.0.9/ephysiopy/common/statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/common/utils.py` & `ephysiopy-2.0.9/ephysiopy/common/utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/format_converters/OE_Axona.py` & `ephysiopy-2.0.9/ephysiopy/format_converters/OE_Axona.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/format_converters/OE_numpy.py` & `ephysiopy-2.0.9/ephysiopy/format_converters/OE_numpy.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/io/recording.py` & `ephysiopy-2.0.9/ephysiopy/io/recording.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/openephys2py/KiloSort.py` & `ephysiopy-2.0.9/ephysiopy/openephys2py/KiloSort.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/openephys2py/OESettings.py` & `ephysiopy-2.0.9/ephysiopy/openephys2py/OESettings.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/tests/conftest.py` & `ephysiopy-2.0.9/ephysiopy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/tests/test_axona_headers.py` & `ephysiopy-2.0.9/ephysiopy/tests/test_axona_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/tests/test_axona_io.py` & `ephysiopy-2.0.9/ephysiopy/tests/test_axona_io.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/tests/test_binning.py` & `ephysiopy-2.0.9/ephysiopy/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/tests/test_dacq2py.py` & `ephysiopy-2.0.9/ephysiopy/tests/test_dacq2py.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/tests/test_ephys_generic.py` & `ephysiopy-2.0.9/ephysiopy/tests/test_ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/tests/test_fieldcalcs.py` & `ephysiopy-2.0.9/ephysiopy/tests/test_fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/tests/test_gridcell.py` & `ephysiopy-2.0.9/ephysiopy/tests/test_gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/tests/test_phasecoding.py` & `ephysiopy-2.0.9/ephysiopy/tests/test_phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/tests/test_rhythmicity.py` & `ephysiopy-2.0.9/ephysiopy/tests/test_rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/tests/test_spikecalcs.py` & `ephysiopy-2.0.9/ephysiopy/tests/test_spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/tests/test_statscalcs.py` & `ephysiopy-2.0.9/ephysiopy/tests/test_statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/tests/test_utils.py` & `ephysiopy-2.0.9/ephysiopy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy/visualise/plotting.py` & `ephysiopy-2.0.9/ephysiopy/visualise/plotting.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/ephysiopy.egg-info/PKG-INFO` & `ephysiopy-2.0.9/ephysiopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 2.0.8
+Version: 2.0.9
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-2.0.8/ephysiopy.egg-info/SOURCES.txt` & `ephysiopy-2.0.9/ephysiopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ephysiopy-2.0.8/setup.py` & `ephysiopy-2.0.9/setup.py`

 * *Files identical despite different names*

