# Comparing `tmp/SAMBA_ilum-1.0.0.4.tar.gz` & `tmp/SAMBA_ilum-1.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAMBA_ilum-1.0.0.4.tar", last modified: Wed Apr 24 18:28:05 2024, max compression
+gzip compressed data, was "SAMBA_ilum-1.0.0.5.tar", last modified: Fri Apr 26 12:24:00 2024, max compression
```

## Comparing `SAMBA_ilum-1.0.0.4.tar` & `SAMBA_ilum-1.0.0.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 18:28:05.249023 SAMBA_ilum-1.0.0.4/
--rw-rw-rw-   0        0        0       13 2024-04-24 12:22:55.000000 SAMBA_ilum-1.0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      297 2024-04-24 18:28:05.249023 SAMBA_ilum-1.0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       56 2024-04-24 12:23:43.000000 SAMBA_ilum-1.0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 18:28:04.875237 SAMBA_ilum-1.0.0.4/SAMBA_ilum.egg-info/
--rw-rw-rw-   0        0        0      297 2024-04-24 18:28:04.000000 SAMBA_ilum-1.0.0.4/SAMBA_ilum.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1711 2024-04-24 18:28:04.000000 SAMBA_ilum-1.0.0.4/SAMBA_ilum.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 18:28:04.000000 SAMBA_ilum-1.0.0.4/SAMBA_ilum.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-04-24 18:28:04.000000 SAMBA_ilum-1.0.0.4/SAMBA_ilum.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-04-24 18:28:04.000000 SAMBA_ilum-1.0.0.4/SAMBA_ilum.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-24 18:28:04.000000 SAMBA_ilum-1.0.0.4/SAMBA_ilum.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-24 18:28:04.890846 SAMBA_ilum-1.0.0.4/samba_ilum/
--rw-rw-rw-   0        0        0       57 2024-04-24 12:22:49.000000 SAMBA_ilum-1.0.0.4/samba_ilum/__init__.py
--rw-rw-rw-   0        0        0     8209 2024-04-24 18:27:51.000000 SAMBA_ilum-1.0.0.4/samba_ilum/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 18:28:05.109511 SAMBA_ilum-1.0.0.4/samba_ilum/src/
--rw-rw-rw-   0        0        0    67526 2024-04-24 12:21:15.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/HeteroStructure_Generator.py
-drwxrwxrwx   0        0        0        0 2024-04-24 18:28:05.186523 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/
--rw-rw-rw-   0        0        0      267 2024-04-17 14:51:50.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/INCAR_bader
--rw-rw-rw-   0        0        0      308 2024-04-17 14:52:00.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/INCAR_bader.SO
--rw-rw-rw-   0        0        0      262 2024-04-17 14:52:22.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/INCAR_bands
--rw-rw-rw-   0        0        0      303 2024-04-17 14:52:42.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/INCAR_bands.SO
--rw-rw-rw-   0        0        0      251 2024-04-17 15:10:48.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/INCAR_dos
--rw-rw-rw-   0        0        0      292 2024-04-17 14:53:00.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/INCAR_dos.SO
--rw-rw-rw-   0        0        0      240 2024-04-17 14:53:10.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/INCAR_relax
--rw-rw-rw-   0        0        0      253 2024-04-17 14:53:18.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/INCAR_scf
--rw-rw-rw-   0        0        0      294 2024-04-17 14:53:24.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/INCAR_scf.SO
--rw-rw-rw-   0        0        0      238 2024-04-19 19:19:42.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/INCAR_xy-scan
--rw-rw-rw-   0        0        0      238 2024-04-19 19:19:50.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/INCAR_z-scan
-drwxrwxrwx   0        0        0        0 2024-04-24 18:28:05.249023 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/inputs_VASProcar/
--rw-rw-rw-   0        0        0     4485 2024-03-20 16:04:46.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.bands
--rw-rw-rw-   0        0        0     3123 2024-04-08 15:25:48.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar
--rw-rw-rw-   0        0        0     2525 2024-03-20 16:04:58.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.dos
--rw-rw-rw-   0        0        0     9603 2024-03-21 16:46:56.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.location
--rw-rw-rw-   0        0        0     1187 2024-03-23 20:35:58.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot
--rw-rw-rw-   0        0        0     6378 2024-03-20 16:05:20.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals
--rw-rw-rw-   0        0        0     7790 2024-03-20 16:06:00.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.spin
--rw-rw-rw-   0        0        0     3968 2024-04-10 01:37:38.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/SAMBA_HeteroStructure.input
--rw-rw-rw-   0        0        0     3013 2024-04-24 18:27:35.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/SAMBA_WorkFlow.input
--rw-rw-rw-   0        0        0     1094 2024-04-24 12:22:37.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/_info_pseudo.py
--rw-rw-rw-   0        0        0  4715152 2023-08-19 14:41:30.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/bader
--rw-rw-rw-   0        0        0     4527 2024-04-24 12:20:31.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/bader_poscar.py
--rw-rw-rw-   0        0        0     2527 2024-04-24 12:20:40.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/bader_update.py
--rw-rw-rw-   0        0        0     7060 2024-04-24 12:20:49.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/charge_transfer.py
--rw-rw-rw-   0        0        0     2139 2019-12-02 15:59:08.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/chgsum.pl
--rw-rw-rw-   0        0        0      330 2024-04-24 12:20:58.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/contcar_update.py
--rw-rw-rw-   0        0        0      600 2024-04-24 12:21:06.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/energy_scan.py
--rw-rw-rw-   0        0        0    13083 2024-04-24 12:21:25.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/job.py
--rw-rw-rw-   0        0        0     6760 2024-04-24 12:50:00.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/kpoints.py
--rw-rw-rw-   0        0        0    21404 2024-04-24 12:21:42.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/make_files.py
--rw-rw-rw-   0        0        0     5959 2024-04-24 12:21:48.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/output.py
--rw-rw-rw-   0        0        0     1053 2024-04-24 12:21:58.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/potcar.py
--rw-rw-rw-   0        0        0     7975 2024-04-24 12:22:07.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/xy-scan.py
--rw-rw-rw-   0        0        0    15612 2024-04-24 12:22:13.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/xy-scan_analysis.py
--rw-rw-rw-   0        0        0     9644 2024-04-24 12:22:20.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/z-scan.py
--rw-rw-rw-   0        0        0     4348 2024-04-24 12:22:26.000000 SAMBA_ilum-1.0.0.4/samba_ilum/src/z-scan_analysis.py
--rw-rw-rw-   0        0        0      167 2024-04-24 18:28:05.249023 SAMBA_ilum-1.0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      733 2024-04-24 18:27:44.000000 SAMBA_ilum-1.0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:24:00.955067 SAMBA_ilum-1.0.0.5/
+-rw-rw-rw-   0        0        0       13 2024-04-24 12:22:55.000000 SAMBA_ilum-1.0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      297 2024-04-26 12:24:00.955067 SAMBA_ilum-1.0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2024-04-24 12:23:43.000000 SAMBA_ilum-1.0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 12:24:00.548811 SAMBA_ilum-1.0.0.5/SAMBA_ilum.egg-info/
+-rw-rw-rw-   0        0        0      297 2024-04-26 12:24:00.000000 SAMBA_ilum-1.0.0.5/SAMBA_ilum.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1711 2024-04-26 12:24:00.000000 SAMBA_ilum-1.0.0.5/SAMBA_ilum.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 12:24:00.000000 SAMBA_ilum-1.0.0.5/SAMBA_ilum.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-04-26 12:24:00.000000 SAMBA_ilum-1.0.0.5/SAMBA_ilum.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-04-26 12:24:00.000000 SAMBA_ilum-1.0.0.5/SAMBA_ilum.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-26 12:24:00.000000 SAMBA_ilum-1.0.0.5/SAMBA_ilum.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 12:24:00.564437 SAMBA_ilum-1.0.0.5/samba_ilum/
+-rw-rw-rw-   0        0        0       57 2024-04-24 12:22:49.000000 SAMBA_ilum-1.0.0.5/samba_ilum/__init__.py
+-rw-rw-rw-   0        0        0     8209 2024-04-26 12:23:34.000000 SAMBA_ilum-1.0.0.5/samba_ilum/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:24:00.783278 SAMBA_ilum-1.0.0.5/samba_ilum/src/
+-rw-rw-rw-   0        0        0    67526 2024-04-24 12:21:15.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/HeteroStructure_Generator.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:24:00.876940 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/
+-rw-rw-rw-   0        0        0      267 2024-04-17 14:51:50.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/INCAR_bader
+-rw-rw-rw-   0        0        0      308 2024-04-17 14:52:00.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/INCAR_bader.SO
+-rw-rw-rw-   0        0        0      262 2024-04-17 14:52:22.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/INCAR_bands
+-rw-rw-rw-   0        0        0      303 2024-04-17 14:52:42.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/INCAR_bands.SO
+-rw-rw-rw-   0        0        0      251 2024-04-17 15:10:48.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/INCAR_dos
+-rw-rw-rw-   0        0        0      292 2024-04-17 14:53:00.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/INCAR_dos.SO
+-rw-rw-rw-   0        0        0      240 2024-04-17 14:53:10.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/INCAR_relax
+-rw-rw-rw-   0        0        0      253 2024-04-17 14:53:18.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/INCAR_scf
+-rw-rw-rw-   0        0        0      294 2024-04-17 14:53:24.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/INCAR_scf.SO
+-rw-rw-rw-   0        0        0      238 2024-04-19 19:19:42.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/INCAR_xy-scan
+-rw-rw-rw-   0        0        0      238 2024-04-19 19:19:50.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/INCAR_z-scan
+drwxrwxrwx   0        0        0        0 2024-04-26 12:24:00.955067 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/inputs_VASProcar/
+-rw-rw-rw-   0        0        0     4485 2024-03-20 16:04:46.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.bands
+-rw-rw-rw-   0        0        0     3123 2024-04-08 15:25:48.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar
+-rw-rw-rw-   0        0        0     2525 2024-03-20 16:04:58.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.dos
+-rw-rw-rw-   0        0        0     9603 2024-03-21 16:46:56.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.location
+-rw-rw-rw-   0        0        0     1187 2024-03-23 20:35:58.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot
+-rw-rw-rw-   0        0        0     6378 2024-03-20 16:05:20.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals
+-rw-rw-rw-   0        0        0     7790 2024-03-20 16:06:00.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.spin
+-rw-rw-rw-   0        0        0     3968 2024-04-10 01:37:38.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/SAMBA_HeteroStructure.input
+-rw-rw-rw-   0        0        0     3048 2024-04-26 12:23:25.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/SAMBA_WorkFlow.input
+-rw-rw-rw-   0        0        0     1094 2024-04-24 12:22:37.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/_info_pseudo.py
+-rw-rw-rw-   0        0        0  4715152 2023-08-19 14:41:30.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/bader
+-rw-rw-rw-   0        0        0     4527 2024-04-24 12:20:31.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/bader_poscar.py
+-rw-rw-rw-   0        0        0     2527 2024-04-24 12:20:40.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/bader_update.py
+-rw-rw-rw-   0        0        0     7060 2024-04-24 12:20:49.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/charge_transfer.py
+-rw-rw-rw-   0        0        0     2139 2019-12-02 15:59:08.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/chgsum.pl
+-rw-rw-rw-   0        0        0      330 2024-04-24 12:20:58.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/contcar_update.py
+-rw-rw-rw-   0        0        0      600 2024-04-24 12:21:06.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/energy_scan.py
+-rw-rw-rw-   0        0        0    13083 2024-04-24 12:21:25.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/job.py
+-rw-rw-rw-   0        0        0     7163 2024-04-26 12:22:49.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/kpoints.py
+-rw-rw-rw-   0        0        0    21404 2024-04-24 12:21:42.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/make_files.py
+-rw-rw-rw-   0        0        0     5959 2024-04-24 12:21:48.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/output.py
+-rw-rw-rw-   0        0        0     1053 2024-04-24 12:21:58.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/potcar.py
+-rw-rw-rw-   0        0        0     7975 2024-04-24 12:22:07.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/xy-scan.py
+-rw-rw-rw-   0        0        0    15612 2024-04-24 12:22:13.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/xy-scan_analysis.py
+-rw-rw-rw-   0        0        0     9644 2024-04-24 12:22:20.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/z-scan.py
+-rw-rw-rw-   0        0        0     4348 2024-04-24 12:22:26.000000 SAMBA_ilum-1.0.0.5/samba_ilum/src/z-scan_analysis.py
+-rw-rw-rw-   0        0        0      167 2024-04-26 12:24:00.955067 SAMBA_ilum-1.0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      733 2024-04-26 12:23:47.000000 SAMBA_ilum-1.0.0.5/setup.py
```

### Comparing `SAMBA_ilum-1.0.0.4/SAMBA_ilum.egg-info/SOURCES.txt` & `SAMBA_ilum-1.0.0.5/SAMBA_ilum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/__main__.py` & `SAMBA_ilum-1.0.0.5/samba_ilum/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pyfiglet
 import shutil
 import time
 import sys
 import os
 
 
-version = '1.0.0.4'
+version = '1.0.0.5'
 
 
 print(" ")
 print("=============================================================")
 print(f'SAMBA_ilum v{version} Copyright (C) 2024 ----------------------')
 print("Closed source: Adalberto Fazzio's research group (Ilum|CNPEM)")
 print("Author: Augusto de Lelis Araujo -----------------------------")
```

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/HeteroStructure_Generator.py` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/HeteroStructure_Generator.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.bands` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.bands`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.dos` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.dos`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.location` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.location`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.spin` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.spin`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/SAMBA_HeteroStructure.input` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/SAMBA_HeteroStructure.input`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/SAMBA_WorkFlow.input` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/SAMBA_WorkFlow.input`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 type  = ['sem_SO','com_SO']                 # Define se as tarefas serão realizadas sem e/ou com SO.
 vdW   = 12                                  # Correção de van der Waals utilizada. [0] desabilita a inclusão de van der Waals nos cálculos.
 #=======================================
 # Backup das opções de cálculo:
 # tasks = ['z-scan', 'xy-scan', 'relax', 'scf', 'bands', 'dos', 'bader']  # Define se as tarefas serão realizadas sem e/ou com SO.
 # type  = ['sem_SO','com_SO']    
 #============================
-type_lattice = 2            # [1] Redes 1D;  [2] Redes 2D;  [3] Redes 3D
+type_lattice = 2            # [1] Redes 1D (Periodico em X);  [2] Redes 2D (Periodico em XY);  [3] Redes 3D
 type_k_dens  = 1            # [1] KPOINTS (Monkhorst-Pack);  [2]  KPOINTS (Gamma);  [3] INCAR (KSPACING Monkhorst-Pack);  [4] INCAR (KSPACING Gamma)
 k_dens_relax = 12           # Cálculo de relaxação:            nº de pontos-k por Å^-1
 k_dens_scf   = 12           # Cálculo auto-consistente (scf):  nº de pontos-k por Å^-1
 k_dens_dos   = 12           # Cálculo da DOS:                  nº de pontos-k por Å^-1
 k_dens_bader = 12           # Cálculo da Carga de Bader:       nº de pontos-k por Å^-1
 n_kpoints    = 50           # Cálculo das bandas (nscf):       nº de pontos-k em cada trecho do plot da banda
 nions_split  = 100          # nº de ions no arquivo POSCAR, para que o cálculo da banda seja executado em etapas (splitado)
```

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/_info_pseudo.py` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/_info_pseudo.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/bader` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/bader`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/bader_poscar.py` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/bader_poscar.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/bader_update.py` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/bader_update.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/charge_transfer.py` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/charge_transfer.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/chgsum.pl` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/chgsum.pl`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/energy_scan.py` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/energy_scan.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/job.py` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/job.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/kpoints.py` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/kpoints.py`

 * *Files 5% similar despite different names*

```diff
@@ -148,15 +148,23 @@
    if (N1 < 3):    N1 = 3
    #-------------------------------------
    N2 = mB2 * k_dens; t = N2 - int(N2)
    if (t >= 0.5):  N2 = int(N2) + 1
    if (t <  0.5):  N2 = int(N2)
    if (N2 < 3):    N2 = 3
    #-------------------------------------
-   N3 = 1
+   N3 = mB3 * k_dens; t = N3 - int(N3)
+   if (t >= 0.5):  N3 = int(N3) + 1
+   if (t <  0.5):  N3 = int(N3)
+   if (N3 < 3):    N3 = 3
+   #--------------------------------------------------------------------------
+   if (type_lattice == 1  or  type_lattice == '1D'  or  type_lattice == '1d'):
+      N2 = 1;  N3 = 1
+   if (type_lattice == 2  or  type_lattice == '2D'  or  type_lattice == '2d'):
+      N3 = 1
 
    #---------------------------------
    # Escrevendo o arquivo KPOINTS ---
    #---------------------------------
    kpoints.write(f'KPOINTS {N1}x{N2}x{N3} \n')
    kpoints.write(f'0 \n')
    kpoints.write(f'{l_dens} \n')
```

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/make_files.py` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/make_files.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/output.py` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/output.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/potcar.py` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/potcar.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/xy-scan.py` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/xy-scan.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/xy-scan_analysis.py` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/xy-scan_analysis.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/z-scan.py` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/z-scan.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/samba_ilum/src/z-scan_analysis.py` & `SAMBA_ilum-1.0.0.5/samba_ilum/src/z-scan_analysis.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.4/setup.py` & `SAMBA_ilum-1.0.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 import json
 from pathlib import Path
 from typing import Optional
 
 setup(
     name = "SAMBA_ilum",
-    version = "1.0.0.4",
+    version = "1.0.0.5",
     entry_points={'console_scripts': ['samba_ilum = samba_ilum:main']},
     description = "...",
     author = "Augusto de Lelis Araujo", 
     author_email = "augusto-lelis@outlook.com",
     license = "Closed source",
     install_requires=['numpy',
                       'requests',
```

