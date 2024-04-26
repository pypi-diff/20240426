# Comparing `tmp/pyteomics-4.7.1.tar.gz` & `tmp/pyteomics-4.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyteomics-4.7.1.tar", last modified: Wed Feb 14 15:32:24 2024, max compression
+gzip compressed data, was "pyteomics-4.7.2.tar", last modified: Fri Apr 26 16:47:41 2024, max compression
```

## Comparing `pyteomics-4.7.1.tar` & `pyteomics-4.7.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:32:24.803399 pyteomics-4.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-14 15:32:13.000000 pyteomics-4.7.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-02-14 15:32:13.000000 pyteomics-4.7.1/INSTALL
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-02-14 15:32:13.000000 pyteomics-4.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-14 15:32:13.000000 pyteomics-4.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-02-14 15:32:13.000000 pyteomics-4.7.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-02-14 15:32:24.803399 pyteomics-4.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-02-14 15:32:13.000000 pyteomics-4.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:32:24.791399 pyteomics-4.7.1/pyteomics/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24735 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/_schema_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    49354 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/achrom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:32:24.795399 pyteomics-4.7.1/pyteomics/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/auxiliary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    83715 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/auxiliary/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    41078 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/auxiliary/file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/auxiliary/math.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/auxiliary/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    15295 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/auxiliary/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)    41524 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/auxiliary/target_decoy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/auxiliary/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/electrochem.py
--rw-r--r--   0 runner    (1001) docker     (127)    38703 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/fasta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:32:24.795399 pyteomics-4.7.1/pyteomics/mass/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/mass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49952 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/mass/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)    25502 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/mass/unimod.py
--rw-r--r--   0 runner    (1001) docker     (127)    33608 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/mgf.py
--rw-r--r--   0 runner    (1001) docker     (127)    18868 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/ms1.py
--rw-r--r--   0 runner    (1001) docker     (127)    16538 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/ms2.py
--rw-r--r--   0 runner    (1001) docker     (127)    17527 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/mzid.py
--rw-r--r--   0 runner    (1001) docker     (127)    21208 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/mzml.py
--rw-r--r--   0 runner    (1001) docker     (127)    19939 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/mzmlb.py
--rw-r--r--   0 runner    (1001) docker     (127)    27739 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/mztab.py
--rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/mzxml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:32:24.795399 pyteomics-4.7.1/pyteomics/openms/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/openms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/openms/featurexml.py
--rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/openms/idxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/openms/trafoxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    41491 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/peff.py
--rw-r--r--   0 runner    (1001) docker     (127)    24099 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/pepxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    79162 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/proforma.py
--rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/protxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    33521 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/pylab_aux.py
--rw-r--r--   0 runner    (1001) docker     (127)    13835 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/tandem.py
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/traml.py
--rw-r--r--   0 runner    (1001) docker     (127)    17738 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/usi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    48336 2024-02-14 15:32:13.000000 pyteomics-4.7.1/pyteomics/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:32:24.799399 pyteomics-4.7.1/pyteomics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-02-14 15:32:24.000000 pyteomics-4.7.1/pyteomics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-02-14 15:32:24.000000 pyteomics-4.7.1/pyteomics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 15:32:24.000000 pyteomics-4.7.1/pyteomics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-14 15:32:24.000000 pyteomics-4.7.1/pyteomics.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 15:32:24.000000 pyteomics-4.7.1/pyteomics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-14 15:32:24.000000 pyteomics-4.7.1/pyteomics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-14 15:32:24.000000 pyteomics-4.7.1/pyteomics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 15:32:24.803399 pyteomics-4.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-02-14 15:32:13.000000 pyteomics-4.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:32:24.799399 pyteomics-4.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_achrom.py
--rw-r--r--   0 runner    (1001) docker     (127)    45521 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_electrochem.py
--rw-r--r--   0 runner    (1001) docker     (127)    15007 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_featurexml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_idxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    15430 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_mass.py
--rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_mgf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_ms1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_ms2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_mzid.py
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_mzml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_mzmlb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_mztab.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_mzxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_peff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_pepxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_proforma.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_protxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_tandem.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_trafoxml.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_traml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_unimod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-02-14 15:32:13.000000 pyteomics-4.7.1/tests/test_usi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:47:41.181831 pyteomics-4.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-26 16:47:30.000000 pyteomics-4.7.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-26 16:47:30.000000 pyteomics-4.7.2/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-04-26 16:47:30.000000 pyteomics-4.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-26 16:47:30.000000 pyteomics-4.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-26 16:47:30.000000 pyteomics-4.7.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-26 16:47:41.181831 pyteomics-4.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-26 16:47:30.000000 pyteomics-4.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:47:41.169831 pyteomics-4.7.2/pyteomics/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24735 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/_schema_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49354 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/achrom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:47:41.169831 pyteomics-4.7.2/pyteomics/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/auxiliary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83715 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/auxiliary/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41078 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/auxiliary/file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/auxiliary/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/auxiliary/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15295 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/auxiliary/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41524 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/auxiliary/target_decoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/auxiliary/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/electrochem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38703 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/fasta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:47:41.173831 pyteomics-4.7.2/pyteomics/mass/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/mass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49952 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/mass/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25623 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/mass/unimod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33608 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/mgf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18894 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/ms1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16538 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/ms2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17527 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/mzid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21208 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/mzml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19939 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/mzmlb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27739 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/mztab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/mzxml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:47:41.173831 pyteomics-4.7.2/pyteomics/openms/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/openms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/openms/featurexml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/openms/idxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/openms/trafoxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41491 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/peff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24099 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/pepxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84843 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/proforma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/protxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33521 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/pylab_aux.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13835 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/tandem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/traml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17738 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/usi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48336 2024-04-26 16:47:30.000000 pyteomics-4.7.2/pyteomics/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:47:41.177831 pyteomics-4.7.2/pyteomics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-26 16:47:41.000000 pyteomics-4.7.2/pyteomics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-26 16:47:41.000000 pyteomics-4.7.2/pyteomics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:47:41.000000 pyteomics-4.7.2/pyteomics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 16:47:41.000000 pyteomics-4.7.2/pyteomics.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:47:41.000000 pyteomics-4.7.2/pyteomics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-26 16:47:41.000000 pyteomics-4.7.2/pyteomics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 16:47:41.000000 pyteomics-4.7.2/pyteomics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:47:41.181831 pyteomics-4.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-26 16:47:30.000000 pyteomics-4.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:47:41.177831 pyteomics-4.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_achrom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45521 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_electrochem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15007 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_featurexml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_idxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15430 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_mgf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_ms1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_ms2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_mzid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_mzml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_mzmlb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_mztab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_mzxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_peff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_pepxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_proforma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_protxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_tandem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_trafoxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_traml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_unimod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-26 16:47:30.000000 pyteomics-4.7.2/tests/test_usi.py
```

### Comparing `pyteomics-4.7.1/AUTHORS` & `pyteomics-4.7.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/INSTALL` & `pyteomics-4.7.2/INSTALL`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/LICENSE` & `pyteomics-4.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/NOTICE` & `pyteomics-4.7.2/NOTICE`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/PKG-INFO` & `pyteomics-4.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyteomics
-Version: 4.7.1
+Version: 4.7.2
 Summary: A framework for proteomics data analysis.
 Home-page: http://pyteomics.readthedocs.io
 Author: Anton Goloborodko & Lev Levitsky
 Author-email: pyteomics@googlegroups.com
 License: License :: OSI Approved :: Apache Software License
 Project-URL: Documentation, http://pyteomics.readthedocs.io
 Project-URL: Source Code, https://github.com/levitsky/pyteomics
```

### Comparing `pyteomics-4.7.1/README.rst` & `pyteomics-4.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/__init__.py` & `pyteomics-4.7.2/pyteomics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/_schema_defaults.py` & `pyteomics-4.7.2/pyteomics/_schema_defaults.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/achrom.py` & `pyteomics-4.7.2/pyteomics/achrom.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/auxiliary/__init__.py` & `pyteomics-4.7.2/pyteomics/auxiliary/__init__.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/auxiliary/constants.py` & `pyteomics-4.7.2/pyteomics/auxiliary/constants.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/auxiliary/file_helpers.py` & `pyteomics-4.7.2/pyteomics/auxiliary/file_helpers.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/auxiliary/math.py` & `pyteomics-4.7.2/pyteomics/auxiliary/math.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/auxiliary/structures.py` & `pyteomics-4.7.2/pyteomics/auxiliary/structures.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/auxiliary/target_decoy.py` & `pyteomics-4.7.2/pyteomics/auxiliary/target_decoy.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/auxiliary/utils.py` & `pyteomics-4.7.2/pyteomics/auxiliary/utils.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/electrochem.py` & `pyteomics-4.7.2/pyteomics/electrochem.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/fasta.py` & `pyteomics-4.7.2/pyteomics/fasta.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/mass/mass.py` & `pyteomics-4.7.2/pyteomics/mass/mass.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/mass/unimod.py` & `pyteomics-4.7.2/pyteomics/mass/unimod.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,18 @@
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import re
 
 from lxml import etree
-from sqlalchemy.ext.declarative import declarative_base, DeclarativeMeta
+try:
+    from sqlalchemy.orm import declarative_base, DeclarativeMeta
+except ImportError:  # Moved in sqlalchemy 2.0
+    from sqlalchemy.ext.declarative import declarative_base, DeclarativeMeta
 from sqlalchemy.orm import relationship, backref, object_session
 from sqlalchemy.ext.associationproxy import association_proxy
 from sqlalchemy import (Numeric, Unicode,
                         Column, Integer, ForeignKey,
                         UnicodeText, Boolean, event)
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
```

### Comparing `pyteomics-4.7.1/pyteomics/mgf.py` & `pyteomics-4.7.2/pyteomics/mgf.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/ms1.py` & `pyteomics-4.7.2/pyteomics/ms1.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     def _handle_S(self, line, sline, params):
         sline = line.strip().split(None, 3)
         params['scan'] = tuple(sline[1:3])
         if len(sline) == 4:  # in MS2 the S line contains the precursor m/z as a 4th column
             params['precursor m/z'] = float(sline[3])
 
     def _handle_I(self, line, sline, params):
-        params[sline[1]] = sline[2]
+        params[sline[1]] = sline[2] if len(sline) > 2 else ''
 
     def _handle_Z(self, line, sline, params):
         params.setdefault('charge', []).append(float(sline[1]))
         params.setdefault('neutral mass', []).append(float(sline[2]))
 
     def _handle_D(self, line, sline, params):
         params.setdefault('analyzer', []).append(sline[1:])
```

### Comparing `pyteomics-4.7.1/pyteomics/ms2.py` & `pyteomics-4.7.2/pyteomics/ms2.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/mzid.py` & `pyteomics-4.7.2/pyteomics/mzid.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/mzml.py` & `pyteomics-4.7.2/pyteomics/mzml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/mzmlb.py` & `pyteomics-4.7.2/pyteomics/mzmlb.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/mztab.py` & `pyteomics-4.7.2/pyteomics/mztab.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/mzxml.py` & `pyteomics-4.7.2/pyteomics/mzxml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/openms/featurexml.py` & `pyteomics-4.7.2/pyteomics/openms/featurexml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/openms/idxml.py` & `pyteomics-4.7.2/pyteomics/openms/idxml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/openms/trafoxml.py` & `pyteomics-4.7.2/pyteomics/openms/trafoxml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/parser.py` & `pyteomics-4.7.2/pyteomics/parser.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/peff.py` & `pyteomics-4.7.2/pyteomics/peff.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/pepxml.py` & `pyteomics-4.7.2/pyteomics/pepxml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/proforma.py` & `pyteomics-4.7.2/pyteomics/proforma.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,14 +267,37 @@
 
 
 class ModificationResolver(object):
     def __init__(self, name, **kwargs):
         self.name = name.lower()
         self.symbol = self.name[0]
         self._database = None
+        self._cache = {}
+
+    def clear_cache(self):
+        """Clear the modification definition cache"""
+        self._cache.clear()
+
+    def enable_caching(self, flag=True):
+        """
+        Enable or disable caching of modification definitions.
+
+        If `flag` is :const:`False`, this will also dispose of any
+        existing cached values.
+
+        Parameters
+        ----------
+        flag : :class:`bool`
+            Whether or not to disable the cache
+        """
+        if flag:
+            if not self._cache:
+                self._cache = {}
+        else:
+            self._cache = None
 
     def load_database(self):
         raise NotImplementedError()
 
     @property
     def database(self):
         if not self._database:
@@ -312,17 +335,27 @@
             id = int(identifier)
             name = None
         else:
             name = identifier
             id = None
         return name, id
 
-    def resolve(self, name=None, id=None, **kwargs):
+    def _resolve_impl(self, name=None, id=None, **kwargs):
         raise NotImplementedError()
 
+    def resolve(self, name=None, id=None, **kwargs):
+        if self._cache is None:
+            return self._resolve_impl(name, id, **kwargs)
+        cache_key = (name, id, frozenset(kwargs.items()))
+        if cache_key in self._cache:
+            return self._cache[cache_key].copy()
+        value = self._resolve_impl(name, id, **kwargs)
+        self._cache[cache_key] = value
+        return  value.copy()
+
     def __call__(self, name=None, id=None, **kwargs):
         return self.resolve(name, id, **kwargs)
 
     def __eq__(self, other):
         return self.name == other.name
 
     def __ne__(self, other):
@@ -339,15 +372,15 @@
         self.strict = kwargs.get("strict", True)
 
     def load_database(self):
         if _has_psims:
             return obo_cache.resolve("http://www.unimod.org/obo/unimod.obo")
         return Unimod()
 
-    def resolve(self, name=None, id=None, **kwargs):
+    def _resolve_impl(self, name=None, id=None, **kwargs):
         strict = kwargs.get("strict", self.strict)
         exhaustive = kwargs.get("exhaustive", True)
         if name is not None:
             defn = self.database.by_title(name, strict=strict)
             if not defn:
                 defn = self.database.by_name(name, strict=strict)
             if not defn and exhaustive and strict:
@@ -394,15 +427,15 @@
     def __init__(self, **kwargs):
         super(PSIModResolver, self).__init__('psimod', **kwargs)
         self._database = kwargs.get("database")
 
     def load_database(self):
         return load_psimod()
 
-    def resolve(self, name=None, id=None, **kwargs):
+    def _resolve_impl(self, name=None, id=None, **kwargs):
         if name is not None:
             defn = self.database[name]
         elif id is not None:
             defn = self.database['MOD:{:05d}'.format(id)]
         else:
             raise ValueError("Must provide one of `name` or `id`")
         try:
@@ -439,15 +472,15 @@
     def __init__(self, **kwargs):
         super(XLMODResolver, self).__init__('xlmod', **kwargs)
         self._database = kwargs.get("database")
 
     def load_database(self):
         return load_xlmod()
 
-    def resolve(self, name=None, id=None, **kwargs):
+    def _resolve_impl(self, name=None, id=None, **kwargs):
         if name is not None:
             defn = self.database[name]
         elif id is not None:
             defn = self.database['XLMOD:{:05d}'.format(id)]
         else:
             raise ValueError("Must provide one of `name` or `id`")
         try:
@@ -558,15 +591,15 @@
         if raw_mass is not None and abs(rough_mass - raw_mass) < 1:
             return raw_mass
         warnings.warn(
             ("An accurate glycan composition could not be inferred from %s. "
              "Only a rough approximation is available.") % (term, ))
         return rough_mass
 
-    def resolve(self, name=None, id=None, **kwargs):
+    def _resolve_impl(self, name=None, id=None, **kwargs):
         if name is not None:
             term = self.database[name]
         elif id is not None:
             term = self.database[id]
         else:
             raise ValueError("Must provide one of `name` or `id`")
         raw_mass, monosaccharides, composition = self.get_mass_from_glycan_composition(term)
@@ -609,15 +642,15 @@
             :const:`None`.
         id : int, optional
             An integer ID embedded in the qualified identifier, if any, otherwise
             :const:`None`.
         """
         return identifier, None
 
-    def resolve(self, name=None, id=None, **kwargs):
+    def _resolve_impl(self, name=None, id=None, **kwargs):
         defn = None
         for resolver in self.resolvers:
             try:
                 defn = resolver(name=name, id=id, **kwargs)
                 break
             except KeyError:
                 continue
@@ -650,14 +683,27 @@
         if style is None:
             style = ModificationTagStyle.Unset
         super(ModificationBase, self).__init__(
             self._tag_type, value, extra, group_id)
         self._definition = None
         self.style = style
 
+    def __reduce__(self):
+        return self.__class__, (self.value, self.extra, self.group_id, self.style), self.__getstate__()
+
+    def __getstate__(self):
+        if self._definition is None:
+            return None
+        state = self._definition.copy()
+        state['source'] = None
+        return state
+
+    def __setstate__(self, state):
+        self._definition = state
+
     def __eq__(self, other):
         if isinstance(other, ModificationToken):
             return other == self
         return super(ModificationBase, self).__eq__(other)
 
     def __hash__(self):
         return hash((self.id, self.provider))
@@ -980,17 +1026,17 @@
         XLMODModification.resolver,
         GNOmeModification.resolver,
         # Some really common names aren't actually found in the XML exactly, so default
         # to non-strict matching now to avoid masking other sources here.
         partial(UnimodModification.resolver, strict=False)
     ])
 
-    def __init__(self, value, extra=None, group_id=None):
+    def __init__(self, value, extra=None, group_id=None, style=None):
         super(GenericModification, self).__init__(
-            value, extra, group_id)
+            value, extra, group_id, style)
 
     def _format_main(self):
         return self.value
 
     def resolve(self):
         '''Find the term, searching through all available vocabularies and
         return the first match's properties
@@ -1234,14 +1280,64 @@
                     part_str = ''.join(part)
                     extra_tag = GenericModification(part_str)
                 extras.append(extra_tag)
         main_tag.extra = extras
     return main_tag
 
 
+class ModificationTarget(object):
+    def __init__(self, aa, n_term=False, c_term=False):
+        self.aa = aa
+        self.n_term = n_term
+        self.c_term = c_term
+
+    def __eq__(self, other):
+        if isinstance(other, str):
+            return str(self) == other
+        else:
+            return (
+                self.aa == other.aa
+                and self.n_term == other.n_term
+                and self.c_term == other.c_term
+            )
+
+    def __ne__(self, other):
+        if isinstance(other, str):
+            return str(self) != other
+        else:
+            return (
+                self.aa != other.aa
+                or self.n_term != other.n_term
+                or self.c_term != other.c_term
+            )
+
+    def __hash__(self):
+        return hash(str(self))
+
+    def __str__(self):
+        buffer = []
+        if self.n_term:
+            buffer.append('N-term')
+        if self.c_term:
+            buffer.append('C-term')
+        if self.aa:
+            buffer.append(self.aa)
+        return ':'.join(buffer)
+
+    def __repr__(self):
+        return str(self)
+
+    def is_valid(self, aa, n_term, c_term):
+        if (n_term and self.n_term) or (c_term and self.c_term):
+            if (self.aa and aa == self.aa) or self.aa is None:
+                return True
+            return False
+        return self.aa == aa or self.aa is None
+
+
 class ModificationRule(object):
     '''Define a fixed modification rule which dictates a modification tag is
     always applied at one or more amino acid residues.
 
     Attributes
     ----------
     modification_tag: TagBase
@@ -1250,25 +1346,72 @@
         The list of amino acids this applies to
     '''
     __slots__ = ('modification_tag', 'targets')
 
     def __init__(self, modification_tag, targets=None):
         self.modification_tag = modification_tag
         self.targets = targets
+        self._validate_targets()
+
+    def is_valid(self, aa, n_term, c_term):
+        return any(target.is_valid(aa, n_term, c_term) for target in self.targets)
+
+    def _validate_targets(self):
+        validated_targets = []
+        if self.targets is None:
+            self.targets = []
+        elif not isinstance(self.targets, list):
+            self.targets = [self.targets]
+        for target in self.targets:
+            if target in VALID_AA:
+                validated_targets.append(ModificationTarget(target, False, False))
+            elif target in ("N-term", "C-term"):
+                n_term = target == "N-term"
+                c_term = target == "C-term"
+                validated_targets.append(ModificationTarget(None, n_term, c_term))
+            elif target.startswith(("N-term:", "C-term:")):
+                tokens = target.split(":")
+                if len(tokens) == 2:
+                    if tokens[1] in VALID_AA:
+                        n_term = tokens[0] == "N-term"
+                        c_term = tokens[0] == "C-term"
+                        validated_targets.append(ModificationTarget(tokens[1], n_term, c_term))
+                    else:
+                        raise PyteomicsError(
+                            "Modification rule {0} has an invalid amino acid specific terminal target {2} in {1}".format(
+                                self,
+                                target,
+                                tokens[1]
+                            )
+                        )
+                else:
+                    raise PyteomicsError(
+                        "Modification rule {0} has an empty amino acid specific terminal target {1}".format(
+                            self, target
+                        )
+                    )
+            else:
+                raise PyteomicsError(
+                    "Modification rule {0} has an invalid target {1}".format(
+                        self, target
+                    )
+                )
+
+        self.targets = validated_targets
 
     def __eq__(self, other):
         if other is None:
             return False
         return self.modification_tag == other.modification_tag and self.targets == other.targets
 
     def __ne__(self, other):
         return not self == other
 
     def __str__(self):
-        targets = ','.join(self.targets)
+        targets = ','.join(map(str, self.targets))
         return "<[{self.modification_tag}]@{targets}>".format(self=self, targets=targets)
 
     def __repr__(self):
         return "{self.__class__.__name__}({self.modification_tag!r}, {self.targets})".format(self=self)
 
 
 class StableIsotope(object):
@@ -1592,14 +1735,15 @@
     charge_state_start = 16
     charge_state_number = 17
     charge_state_adduct_start = 18
     charge_state_adduct_end = 19
     inter_chain_cross_link_start = 20
     chimeric_start = 21
     interval_initial = 22
+    post_global_terminal = 23
     done = 999
 
 
 BEFORE = ParserStateEnum.before_sequence
 TAG_BEFORE = ParserStateEnum.tag_before_sequence
 FIXED = ParserStateEnum.fixed_spec
 GLOBAL = ParserStateEnum.global_tag
@@ -1611,22 +1755,24 @@
 INTERVAL_INIT = ParserStateEnum.interval_initial
 TAG_AFTER = ParserStateEnum.tag_after_sequence
 POST_TAG_BEFORE = ParserStateEnum.post_tag_before
 POST_TAG_AFTER = ParserStateEnum.post_tag_after
 UNLOCALIZED_COUNT = ParserStateEnum.unlocalized_count
 POST_GLOBAL = ParserStateEnum.post_global
 POST_GLOBAL_AA = ParserStateEnum.post_global_aa
+POST_GLOBAL_TERM = ParserStateEnum.post_global_terminal
 POST_INTERVAL_TAG = ParserStateEnum.post_interval_tag
 CHARGE_START = ParserStateEnum.charge_state_start
 CHARGE_NUMBER = ParserStateEnum.charge_state_number
 ADDUCT_START = ParserStateEnum.charge_state_adduct_start
 ADDUCT_END = ParserStateEnum.charge_state_adduct_end
 DONE = ParserStateEnum.done
 
 VALID_AA = set("QWERTYIPASDFGHKLCVNMXUOJZB")
+TERMINAL_SPEC_CHARS = set('N-term') | set('C-term') | set("ncT: ")
 
 def parse(sequence):
     '''Tokenize a ProForma sequence into a sequence of amino acid+tag positions, and a
     mapping of sequence-spanning modifiers.
 
     .. note::
         This is a state machine parser, but with certain sub-state paths
@@ -1661,15 +1807,15 @@
     state = BEFORE
     depth = 0
 
     current_aa = None
     current_tag = TagParser()
     current_interval = None
     current_unlocalized_count = NumberParser()
-    current_aa_targets = TokenBuffer()
+    current_aa_targets = StringParser()
 
     charge_buffer = None
     adduct_buffer = None
 
     # A mostly context free finite state machine unrolled
     # by hand.
     while i < n:
@@ -1851,41 +1997,52 @@
             if c.isdigit():
                 current_unlocalized_count.append(c)
             elif c == '[':
                 state = TAG_BEFORE
                 depth = 1
                 tag = current_tag()[0]
                 multiplicity = current_unlocalized_count()
-                for i in range(multiplicity):
+                for _ in range(multiplicity):
                     unlocalized_modifications.append(tag)
             elif c == '?':
                 state = BEFORE
                 tag = current_tag()[0]
                 multiplicity = current_unlocalized_count()
-                for i in range(multiplicity):
+                for _ in range(multiplicity):
                     unlocalized_modifications.append(tag)
             else:
                 raise ProFormaError(
                     "Error In State {state}, unexpected {c} found at index {i}".format(**locals()), i, state)
         elif state == POST_GLOBAL:
             if c == '@':
                 state = POST_GLOBAL_AA
             else:
                 raise ProFormaError(
                     ("Error In State {state}, fixed modification detected without "
                      "target amino acids found at index {i}").format(**locals()), i, state)
         elif state == POST_GLOBAL_AA:
-            if c in VALID_AA:
+            if c in VALID_AA or c in TERMINAL_SPEC_CHARS:
                 current_aa_targets.append(c)
             elif c == ',':
                 # the next character should be another amino acid
-                pass
+                current_aa_targets.bound()
             elif c == '>':
-                fixed_modifications.append(
-                    ModificationRule(current_tag()[0], current_aa_targets()))
+                try:
+                    v = current_aa_targets()
+                    fixed_modifications.append(
+                        ModificationRule(current_tag()[0], v))
+                except PyteomicsError as err:
+                    raise ProFormaError(
+                        (
+                            "Error In State {state}, fixed modification detected invalid "
+                            "target found at index {i}: {err}"
+                        ).format(state=state, i=i, err=err),
+                        i,
+                        state,
+                    )
                 state = BEFORE
             else:
                 raise ProFormaError(
                     ("Error In State {state}, unclosed fixed modification rule").format(**locals()), i, state)
         elif state == POST_TAG_AFTER:
             if c == '/':
                 state = CHARGE_START
@@ -2147,27 +2304,28 @@
         return cls(*parse(string))
 
     @property
     def mass(self):
         mass = 0.0
 
         fixed_modifications = self.properties['fixed_modifications']
-        fixed_rules = {}
-        for rule in fixed_modifications:
-            for aa in rule.targets:
-                fixed_rules[aa] = rule.modification_tag.mass
 
-        for position in self.sequence:
+        n_term_v = 0
+        c_term_v = len(self) - 1
+        for i, position in enumerate(self.sequence):
             aa = position[0]
             try:
                 mass += std_aa_mass[aa]
             except KeyError:
                 warnings.warn("%r does not have an exact mass" % (aa, ))
-            if aa in fixed_rules:
-                mass += fixed_rules[aa]
+            n_term = i == n_term_v
+            c_term = i == c_term_v
+            for rule in fixed_modifications:
+                if rule.is_valid(aa, n_term, c_term):
+                    mass += rule.modification_tag.mass
             tags = position[1]
             if tags:
                 for tag in tags:
                     try:
                         mass += tag.mass
                     except (AttributeError, KeyError):
                         continue
@@ -2244,18 +2402,14 @@
         n = len(self.sequence)
         masses = _array('d')
 
         mass = 0
         mass += ion_shift
 
         fixed_modifications = self.properties['fixed_modifications']
-        fixed_rules = {}
-        for rule in fixed_modifications:
-            for aa in rule.targets:
-                fixed_rules[aa] = rule.modification_tag.mass
 
         intervals = self.intervals
         if intervals:
             intervals = sorted(intervals, key=lambda x: x.start)
         intervals = deque(intervals)
 
         if not include_labile:
@@ -2281,28 +2435,35 @@
             for mod in self.properties['unlocalized_modifications']:
                 mass += mod.mass
 
         mass += _WATER_MASS
 
         if not reverse:
             iterator = (iter(range(0, n - 1)))
+            n_term_v = 0
+            c_term_v = n - 1
         else:
             iterator = (reversed(range(1, n)))
+            n_term_v = n - 1
+            c_term_v = 0
 
         for i in iterator:
             position = self.sequence[i]
 
             aa = position[0]
             try:
                 mass += std_aa_mass[aa]
             except KeyError:
                 warnings.warn("%r does not have an exact mass" % (aa, ))
 
-            if aa in fixed_rules:
-                mass += fixed_rules[aa]
+            n_term = i == n_term_v
+            c_term = i == c_term_v
+            for rule in fixed_modifications:
+                if rule.is_valid(aa, n_term, c_term):
+                    mass += rule.modification_tag.mass
 
             tags = position[1]
             if tags:
                 for tag in tags:
                     try:
                         mass += tag.mass
                     except (AttributeError, KeyError):
```

### Comparing `pyteomics-4.7.1/pyteomics/protxml.py` & `pyteomics-4.7.2/pyteomics/protxml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/pylab_aux.py` & `pyteomics-4.7.2/pyteomics/pylab_aux.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/tandem.py` & `pyteomics-4.7.2/pyteomics/tandem.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/traml.py` & `pyteomics-4.7.2/pyteomics/traml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/usi.py` & `pyteomics-4.7.2/pyteomics/usi.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics/version.py` & `pyteomics-4.7.2/pyteomics/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
   :py:const:`version` - a string with the current version.
 
   :py:const:`version_info` - a tuple with structured information about the current version.
 
 """
 
-__version__ = '4.7.1'
+__version__ = '4.7.2'
 
 from collections import namedtuple
 import re
 
 
 class VersionInfo(namedtuple('VersionInfo', ('major', 'minor', 'micro', 'releaselevel', 'serial'))):
     """Tuple mimicking :py:const:`sys.version_info`"""
```

### Comparing `pyteomics-4.7.1/pyteomics/xml.py` & `pyteomics-4.7.2/pyteomics/xml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/pyteomics.egg-info/PKG-INFO` & `pyteomics-4.7.2/pyteomics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyteomics
-Version: 4.7.1
+Version: 4.7.2
 Summary: A framework for proteomics data analysis.
 Home-page: http://pyteomics.readthedocs.io
 Author: Anton Goloborodko & Lev Levitsky
 Author-email: pyteomics@googlegroups.com
 License: License :: OSI Approved :: Apache Software License
 Project-URL: Documentation, http://pyteomics.readthedocs.io
 Project-URL: Source Code, https://github.com/levitsky/pyteomics
```

### Comparing `pyteomics-4.7.1/pyteomics.egg-info/SOURCES.txt` & `pyteomics-4.7.2/pyteomics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/setup.py` & `pyteomics-4.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_auxiliary.py` & `pyteomics-4.7.2/tests/test_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_electrochem.py` & `pyteomics-4.7.2/tests/test_electrochem.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_fasta.py` & `pyteomics-4.7.2/tests/test_fasta.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_featurexml.py` & `pyteomics-4.7.2/tests/test_featurexml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_idxml.py` & `pyteomics-4.7.2/tests/test_idxml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_mass.py` & `pyteomics-4.7.2/tests/test_mass.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_mgf.py` & `pyteomics-4.7.2/tests/test_mgf.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_ms1.py` & `pyteomics-4.7.2/tests/test_ms1.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_ms2.py` & `pyteomics-4.7.2/tests/test_ms2.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_mzid.py` & `pyteomics-4.7.2/tests/test_mzid.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_mzml.py` & `pyteomics-4.7.2/tests/test_mzml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_mzmlb.py` & `pyteomics-4.7.2/tests/test_mzmlb.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_mztab.py` & `pyteomics-4.7.2/tests/test_mztab.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_mzxml.py` & `pyteomics-4.7.2/tests/test_mzxml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_parser.py` & `pyteomics-4.7.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_peff.py` & `pyteomics-4.7.2/tests/test_peff.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_pepxml.py` & `pyteomics-4.7.2/tests/test_pepxml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_proforma.py` & `pyteomics-4.7.2/tests/test_proforma.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from os import path
 import unittest
+import pickle
 import pyteomics
 pyteomics.__path__ = [path.abspath(
     path.join(path.dirname(__file__), path.pardir, 'pyteomics'))]
 from pyteomics.proforma import (
     PSIModModification, ProForma, TaggedInterval, parse, MassModification, ProFormaError, TagTypeEnum,
     ModificationRule, StableIsotope, GenericModification, Composition, to_proforma, ModificationMassNotFoundError,
     obo_cache, process_tag_tokens)
@@ -176,9 +177,21 @@
         self.assertIn(mod.key, container)
 
         mod2 = MassModification(57.08 + 1e-19)
         self.assertIn(mod2.key, container)
         self.assertIn(mod2, container)
 
 
+class ModificationPicklingTest(unittest.TestCase):
+    def test_pickle(self):
+        mod = GenericModification("UNIMOD:1")
+        payload = pickle.dumps(mod)
+        dup = pickle.loads(payload)
+        self.assertEqual(mod, dup)
+        assert mod.mass is not None
+        payload = pickle.dumps(mod)
+        dup = pickle.loads(payload)
+        self.assertEqual(mod, dup)
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pyteomics-4.7.1/tests/test_protxml.py` & `pyteomics-4.7.2/tests/test_protxml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_tandem.py` & `pyteomics-4.7.2/tests/test_tandem.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_trafoxml.py` & `pyteomics-4.7.2/tests/test_trafoxml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_traml.py` & `pyteomics-4.7.2/tests/test_traml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_unimod.py` & `pyteomics-4.7.2/tests/test_unimod.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.7.1/tests/test_usi.py` & `pyteomics-4.7.2/tests/test_usi.py`

 * *Files identical despite different names*

