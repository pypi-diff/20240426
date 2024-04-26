# Comparing `tmp/ambit-fe-1.2.5.tar.gz` & `tmp/ambit_fe-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambit-fe-1.2.5.tar", last modified: Wed Mar 27 07:22:27 2024, max compression
+gzip compressed data, was "ambit_fe-1.2.6.tar", last modified: Fri Apr 26 13:05:20 2024, max compression
```

## Comparing `ambit-fe-1.2.5.tar` & `ambit_fe-1.2.6.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-03-27 07:22:27.542615 ambit-fe-1.2.5/
--rw-rw-r--   0 mh        (1001) mh        (1001)     1073 2024-01-13 20:57:23.000000 ambit-fe-1.2.5/LICENSE
--rw-r--r--   0 mh        (1001) mh        (1001)     6227 2024-03-27 07:22:27.542615 ambit-fe-1.2.5/PKG-INFO
--rw-rw-r--   0 mh        (1001) mh        (1001)     4368 2024-03-06 11:21:34.000000 ambit-fe-1.2.5/README.md
--rw-rw-r--   0 mh        (1001) mh        (1001)      853 2024-03-27 07:10:33.000000 ambit-fe-1.2.5/pyproject.toml
--rw-rw-r--   0 mh        (1001) mh        (1001)       38 2024-03-27 07:22:27.542615 ambit-fe-1.2.5/setup.cfg
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-03-27 07:22:27.526617 ambit-fe-1.2.5/src/
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-03-27 07:22:27.526617 ambit-fe-1.2.5/src/ambit_fe/
--rw-rw-r--   0 mh        (1001) mh        (1001)      283 2024-01-13 19:07:42.000000 ambit-fe-1.2.5/src/ambit_fe/__init__.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-03-27 07:22:27.526617 ambit-fe-1.2.5/src/ambit_fe/ale/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:09.000000 ambit-fe-1.2.5/src/ambit_fe/ale/__init__.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     1757 2024-02-16 14:30:37.000000 ambit-fe-1.2.5/src/ambit_fe/ale/ale_kinematics_constitutive.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    14358 2024-03-15 15:14:34.000000 ambit-fe-1.2.5/src/ambit_fe/ale/ale_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     1726 2024-02-16 14:32:55.000000 ambit-fe-1.2.5/src/ambit_fe/ale/ale_material.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     1920 2024-03-19 13:53:01.000000 ambit-fe-1.2.5/src/ambit_fe/ale/ale_variationalform.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    15484 2024-03-21 20:03:07.000000 ambit-fe-1.2.5/src/ambit_fe/ambit_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    12383 2024-03-15 15:13:07.000000 ambit-fe-1.2.5/src/ambit_fe/base.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    29257 2024-03-07 14:00:37.000000 ambit-fe-1.2.5/src/ambit_fe/boundaryconditions.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-03-27 07:22:27.526617 ambit-fe-1.2.5/src/ambit_fe/coupling/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:12.000000 ambit-fe-1.2.5/src/ambit_fe/coupling/__init__.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    21916 2024-03-19 15:26:52.000000 ambit-fe-1.2.5/src/ambit_fe/coupling/fluid_ale_flow0d_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    26863 2024-03-19 15:25:24.000000 ambit-fe-1.2.5/src/ambit_fe/coupling/fluid_ale_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    30999 2024-03-11 10:36:13.000000 ambit-fe-1.2.5/src/ambit_fe/coupling/fluid_flow0d_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    17910 2024-03-11 10:30:46.000000 ambit-fe-1.2.5/src/ambit_fe/coupling/fsi_flow0d_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    17544 2024-03-11 10:30:29.000000 ambit-fe-1.2.5/src/ambit_fe/coupling/fsi_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    22030 2024-03-11 10:23:21.000000 ambit-fe-1.2.5/src/ambit_fe/coupling/solid_constraint_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    38846 2024-03-11 10:23:19.000000 ambit-fe-1.2.5/src/ambit_fe/coupling/solid_flow0d_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     5219 2024-03-09 22:52:23.000000 ambit-fe-1.2.5/src/ambit_fe/coupling/solid_flow0d_periodicref_main.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-03-27 07:22:27.526617 ambit-fe-1.2.5/src/ambit_fe/electrophysiology/
--rw-rw-r--   0 mh        (1001) mh        (1001)     1480 2024-02-12 18:01:07.000000 ambit-fe-1.2.5/src/ambit_fe/electrophysiology/electrophysiology_constitutive.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    14936 2024-03-05 07:16:52.000000 ambit-fe-1.2.5/src/ambit_fe/electrophysiology/electrophysiology_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)      947 2024-02-14 11:55:11.000000 ambit-fe-1.2.5/src/ambit_fe/electrophysiology/electrophysiology_variationalform.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     1242 2024-01-21 16:56:18.000000 ambit-fe-1.2.5/src/ambit_fe/expression.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-03-27 07:22:27.526617 ambit-fe-1.2.5/src/ambit_fe/flow0d/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:17.000000 ambit-fe-1.2.5/src/ambit_fe/flow0d/__init__.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    18497 2024-01-13 19:08:17.000000 ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     3521 2024-01-13 19:08:16.000000 ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D_2elwindkessel.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     4692 2024-01-13 19:08:16.000000 ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D_4elwindkesselLpZ.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     4369 2024-01-13 19:08:16.000000 ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D_4elwindkesselLsZ.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     3939 2024-01-13 19:08:16.000000 ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D_CRLinoutlink.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    15029 2024-01-13 19:08:16.000000 ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D_coronary.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    30594 2024-01-13 19:08:17.000000 ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D_syspul.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    78326 2024-01-13 19:08:17.000000 ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D_syspulcap.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    54451 2024-01-13 19:08:17.000000 ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D_syspulcaprespir.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     1666 2024-01-13 19:08:17.000000 ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D_vad.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    22429 2024-03-19 13:34:41.000000 ambit-fe-1.2.5/src/ambit_fe/flow0d/flow0d_main.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-03-27 07:22:27.530616 ambit-fe-1.2.5/src/ambit_fe/fluid/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:05.000000 ambit-fe-1.2.5/src/ambit_fe/fluid/__init__.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     2990 2024-03-19 16:09:06.000000 ambit-fe-1.2.5/src/ambit_fe/fluid/fluid_kinematics_constitutive.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    71883 2024-03-25 11:39:21.000000 ambit-fe-1.2.5/src/ambit_fe/fluid/fluid_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)      581 2024-01-13 19:08:05.000000 ambit-fe-1.2.5/src/ambit_fe/fluid/fluid_material.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    17744 2024-02-22 09:45:59.000000 ambit-fe-1.2.5/src/ambit_fe/fluid/fluid_variationalform.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     8332 2024-03-25 08:40:33.000000 ambit-fe-1.2.5/src/ambit_fe/ioparams.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    65866 2024-03-25 11:40:22.000000 ambit-fe-1.2.5/src/ambit_fe/ioroutines.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     3372 2024-01-13 19:07:42.000000 ambit-fe-1.2.5/src/ambit_fe/mathutils.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     5319 2024-01-13 19:07:42.000000 ambit-fe-1.2.5/src/ambit_fe/meshutils.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-03-27 07:22:27.530616 ambit-fe-1.2.5/src/ambit_fe/mor/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:53.000000 ambit-fe-1.2.5/src/ambit_fe/mor/__init__.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    23624 2024-03-25 11:46:44.000000 ambit-fe-1.2.5/src/ambit_fe/mor/mor_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     1667 2024-01-13 19:07:42.000000 ambit-fe-1.2.5/src/ambit_fe/mpiroutines.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-03-27 07:22:27.530616 ambit-fe-1.2.5/src/ambit_fe/multiscale/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:48.000000 ambit-fe-1.2.5/src/ambit_fe/multiscale/__init__.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    15481 2024-01-21 16:15:11.000000 ambit-fe-1.2.5/src/ambit_fe/multiscale/solid_flow0d_growthremodel_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     9642 2024-01-13 19:07:42.000000 ambit-fe-1.2.5/src/ambit_fe/oderoutines.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-03-27 07:22:27.530616 ambit-fe-1.2.5/src/ambit_fe/postprocess/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:38.000000 ambit-fe-1.2.5/src/ambit_fe/postprocess/__init__.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    72147 2024-01-29 08:41:01.000000 ambit-fe-1.2.5/src/ambit_fe/postprocess/flow0d_plot.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     4022 2024-03-04 18:00:59.000000 ambit-fe-1.2.5/src/ambit_fe/resultcheck.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-03-27 07:22:27.530616 ambit-fe-1.2.5/src/ambit_fe/signet/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:26.000000 ambit-fe-1.2.5/src/ambit_fe/signet/__init__.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    37626 2024-01-13 19:08:26.000000 ambit-fe-1.2.5/src/ambit_fe/signet/signet_hypertrophy.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    10380 2024-03-08 08:28:58.000000 ambit-fe-1.2.5/src/ambit_fe/signet/signet_main.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-03-27 07:22:27.530616 ambit-fe-1.2.5/src/ambit_fe/solid/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:01.000000 ambit-fe-1.2.5/src/ambit_fe/solid/__init__.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    26329 2024-03-15 14:40:16.000000 ambit-fe-1.2.5/src/ambit_fe/solid/solid_kinematics_constitutive.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    68939 2024-03-25 11:39:07.000000 ambit-fe-1.2.5/src/ambit_fe/solid/solid_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    14578 2024-03-15 14:39:57.000000 ambit-fe-1.2.5/src/ambit_fe/solid/solid_material.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     5572 2024-01-13 19:08:01.000000 ambit-fe-1.2.5/src/ambit_fe/solid/solid_variationalform.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-03-27 07:22:27.530616 ambit-fe-1.2.5/src/ambit_fe/solver/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:07:57.000000 ambit-fe-1.2.5/src/ambit_fe/solver/__init__.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    33179 2024-03-26 19:09:30.000000 ambit-fe-1.2.5/src/ambit_fe/solver/preconditioner.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     1904 2024-01-13 19:07:57.000000 ambit-fe-1.2.5/src/ambit_fe/solver/projection.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    44985 2024-03-18 17:08:30.000000 ambit-fe-1.2.5/src/ambit_fe/solver/solver_nonlin.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    26668 2024-01-13 19:07:57.000000 ambit-fe-1.2.5/src/ambit_fe/solver/solver_utils.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    30344 2024-03-09 21:38:39.000000 ambit-fe-1.2.5/src/ambit_fe/timeintegration.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     5823 2024-03-27 07:11:03.000000 ambit-fe-1.2.5/src/ambit_fe/utilities.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    12381 2024-03-19 17:33:23.000000 ambit-fe-1.2.5/src/ambit_fe/variationalform.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-03-27 07:22:27.542615 ambit-fe-1.2.5/src/ambit_fe.egg-info/
--rw-r--r--   0 mh        (1001) mh        (1001)     6227 2024-03-27 07:22:27.000000 ambit-fe-1.2.5/src/ambit_fe.egg-info/PKG-INFO
--rw-rw-r--   0 mh        (1001) mh        (1001)     5406 2024-03-27 07:22:27.000000 ambit-fe-1.2.5/src/ambit_fe.egg-info/SOURCES.txt
--rw-rw-r--   0 mh        (1001) mh        (1001)        1 2024-03-27 07:22:27.000000 ambit-fe-1.2.5/src/ambit_fe.egg-info/dependency_links.txt
--rw-rw-r--   0 mh        (1001) mh        (1001)       13 2024-03-27 07:22:27.000000 ambit-fe-1.2.5/src/ambit_fe.egg-info/requires.txt
--rw-rw-r--   0 mh        (1001) mh        (1001)        9 2024-03-27 07:22:27.000000 ambit-fe-1.2.5/src/ambit_fe.egg-info/top_level.txt
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-03-27 07:22:27.542615 ambit-fe-1.2.5/tests/
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3042 2024-02-23 10:07:29.000000 ambit-fe-1.2.5/tests/test_ale_linelast.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     2937 2024-02-13 18:57:20.000000 ambit-fe-1.2.5/tests/test_electrophysiology.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     7081 2024-02-23 10:07:26.000000 ambit-fe-1.2.5/tests/test_flow0d_0dheart_syspul.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    15443 2024-02-23 10:07:22.000000 ambit-fe-1.2.5/tests/test_flow0d_0dheart_syspulcap.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    15626 2024-02-23 10:07:19.000000 ambit-fe-1.2.5/tests/test_flow0d_0dheart_syspulcapcor.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    22686 2024-02-23 10:07:15.000000 ambit-fe-1.2.5/tests/test_flow0d_0dheart_syspulcaprespir_periodic.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     7490 2024-02-23 10:07:09.000000 ambit-fe-1.2.5/tests/test_flow0d_0dheart_syspulcor.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     8426 2024-02-23 10:07:05.000000 ambit-fe-1.2.5/tests/test_flow0d_0dheart_syspulcorvad.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     2424 2024-02-23 10:07:01.000000 ambit-fe-1.2.5/tests/test_flow0d_0dvol_4elwindkesselLpZ.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     2358 2024-02-23 10:06:57.000000 ambit-fe-1.2.5/tests/test_flow0d_0dvol_4elwindkesselLsZ.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    10674 2024-02-23 10:06:53.000000 ambit-fe-1.2.5/tests/test_fluid_ale_flow0d_lalv_syspul_prescribed.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4535 2024-02-23 10:06:47.000000 ambit-fe-1.2.5/tests/test_fluid_flow0d_monolagr_taylorhood_cylinder.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3913 2024-02-23 10:06:29.000000 ambit-fe-1.2.5/tests/test_fluid_p1p1_stab_cylinder.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4357 2024-02-23 10:06:25.000000 ambit-fe-1.2.5/tests/test_fluid_p1p1_stab_cylinder_schur2x2.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4850 2024-03-15 15:06:23.000000 ambit-fe-1.2.5/tests/test_fluid_p1p1_stab_cylinder_valve.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3640 2024-02-23 10:06:18.000000 ambit-fe-1.2.5/tests/test_fluid_taylorhood_cylinder.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     5724 2024-03-25 09:30:47.000000 ambit-fe-1.2.5/tests/test_frsi_artseg_modepartitionunity.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4804 2024-03-25 09:01:11.000000 ambit-fe-1.2.5/tests/test_frsi_artseg_prefile.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     6016 2024-03-25 09:01:16.000000 ambit-fe-1.2.5/tests/test_frsi_artseg_prefile_partitioned_schur3x3.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     5744 2024-03-25 09:01:20.000000 ambit-fe-1.2.5/tests/test_frsi_artseg_prefile_schurbgs4x4.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     5344 2024-03-25 09:01:24.000000 ambit-fe-1.2.5/tests/test_frsi_artseg_prestress.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     7742 2024-02-23 10:05:54.000000 ambit-fe-1.2.5/tests/test_fsi_flow0d_p1p1_stab_artseg.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     6614 2024-02-23 10:06:38.000000 ambit-fe-1.2.5/tests/test_fsi_p1p1_stab_artseg.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     5667 2024-02-23 10:06:33.000000 ambit-fe-1.2.5/tests/test_fsi_taylorhood_artseg.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     2313 2024-03-08 08:27:18.000000 ambit-fe-1.2.5/tests/test_signet_0d_hypertrophy.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     2815 2024-03-15 14:39:36.000000 ambit-fe-1.2.5/tests/test_solid_2d_pres.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4995 2024-03-07 06:30:09.000000 ambit-fe-1.2.5/tests/test_solid_2dheart_frankstarling.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3769 2024-02-23 10:05:10.000000 ambit-fe-1.2.5/tests/test_solid_bodyforce_gravity.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3390 2024-02-23 10:05:06.000000 ambit-fe-1.2.5/tests/test_solid_constraint_volume_chamber.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3036 2024-02-23 10:05:02.000000 ambit-fe-1.2.5/tests/test_solid_divcont_ptc.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4079 2024-02-23 10:04:58.000000 ambit-fe-1.2.5/tests/test_solid_flow0d_monodir2field_4elwindkesselLpZ_chamber.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    18260 2024-02-23 10:04:55.000000 ambit-fe-1.2.5/tests/test_solid_flow0d_monodir2field_flux_syspulcap_3Dheart_schur3x3.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3997 2024-02-23 10:04:50.000000 ambit-fe-1.2.5/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4444 2024-02-23 10:04:46.000000 ambit-fe-1.2.5/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber_bgs2x2.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4619 2024-02-23 10:04:42.000000 ambit-fe-1.2.5/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber_bgs2x2fieldsplit.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    18144 2024-02-23 10:04:38.000000 ambit-fe-1.2.5/tests/test_solid_flow0d_monodir_flux_syspulcap_3Dheart_simple2x2.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    10261 2024-03-05 08:28:49.000000 ambit-fe-1.2.5/tests/test_solid_flow0d_monodir_syspul_2dheart_prestress.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    10378 2024-03-25 08:40:46.000000 ambit-fe-1.2.5/tests/test_solid_flow0d_monodir_syspulcor_2dheart_rom.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4196 2024-03-05 18:14:14.000000 ambit-fe-1.2.5/tests/test_solid_flow0d_monolagr2field_2elwindkessel_chamber.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4969 2024-02-23 10:04:20.000000 ambit-fe-1.2.5/tests/test_solid_flow0d_monolagr_CRLinoutlink_chambers.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    19455 2024-02-23 10:04:16.000000 ambit-fe-1.2.5/tests/test_solid_flow0d_multiscalegrowthremodeling_concentric.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    19437 2024-02-23 10:04:11.000000 ambit-fe-1.2.5/tests/test_solid_flow0d_multiscalegrowthremodeling_eccentric.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    11399 2024-03-09 22:53:35.000000 ambit-fe-1.2.5/tests/test_solid_flow0d_periodicref_syspul_lvchamber.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3302 2024-02-23 10:03:13.000000 ambit-fe-1.2.5/tests/test_solid_growth_prescribed_iso_lv.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3859 2024-02-23 10:04:01.000000 ambit-fe-1.2.5/tests/test_solid_growth_volstressmandel.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4034 2024-02-23 10:03:58.000000 ambit-fe-1.2.5/tests/test_solid_growth_volstressmandel_incomp.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4595 2024-02-23 10:03:55.000000 ambit-fe-1.2.5/tests/test_solid_growthremodeling_fiberstretch.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     7304 2024-02-23 10:03:51.000000 ambit-fe-1.2.5/tests/test_solid_mat_uniax_hex_2field.py
--rwxr-xr-x   0 mh        (1001) mh        (1001)     7538 2024-01-21 17:16:25.000000 ambit-fe-1.2.5/tests/test_solid_membrane.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3710 2024-02-23 10:03:41.000000 ambit-fe-1.2.5/tests/test_solid_pinch_edge.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     3171 2024-02-23 10:03:37.000000 ambit-fe-1.2.5/tests/test_solid_plasticity_vonmises.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3523 2024-02-23 10:03:34.000000 ambit-fe-1.2.5/tests/test_solid_robin_genalpha.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3921 2024-03-19 07:42:47.000000 ambit-fe-1.2.5/tests/test_solid_robin_genalpha_amg.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3108 2024-02-23 10:03:26.000000 ambit-fe-1.2.5/tests/test_solid_robin_static_prestress.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3114 2024-02-23 10:03:22.000000 ambit-fe-1.2.5/tests/test_solid_robin_visco.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-04-26 13:05:20.271347 ambit_fe-1.2.6/
+-rw-rw-r--   0 mh        (1001) mh        (1001)     1073 2024-01-13 20:57:23.000000 ambit_fe-1.2.6/LICENSE
+-rw-r--r--   0 mh        (1001) mh        (1001)     6223 2024-04-26 13:05:20.271347 ambit_fe-1.2.6/PKG-INFO
+-rw-rw-r--   0 mh        (1001) mh        (1001)     4368 2024-03-06 11:21:34.000000 ambit_fe-1.2.6/README.md
+-rw-rw-r--   0 mh        (1001) mh        (1001)      849 2024-04-26 13:00:28.000000 ambit_fe-1.2.6/pyproject.toml
+-rw-rw-r--   0 mh        (1001) mh        (1001)       38 2024-04-26 13:05:20.271347 ambit_fe-1.2.6/setup.cfg
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-04-26 13:05:20.251347 ambit_fe-1.2.6/src/
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-04-26 13:05:20.255347 ambit_fe-1.2.6/src/ambit_fe/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      283 2024-01-13 19:07:42.000000 ambit_fe-1.2.6/src/ambit_fe/__init__.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-04-26 13:05:20.255347 ambit_fe-1.2.6/src/ambit_fe/ale/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:09.000000 ambit_fe-1.2.6/src/ambit_fe/ale/__init__.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     1757 2024-02-16 14:30:37.000000 ambit_fe-1.2.6/src/ambit_fe/ale/ale_kinematics_constitutive.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    14114 2024-04-11 18:48:26.000000 ambit_fe-1.2.6/src/ambit_fe/ale/ale_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     1726 2024-02-16 14:32:55.000000 ambit_fe-1.2.6/src/ambit_fe/ale/ale_material.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     1920 2024-03-19 13:53:01.000000 ambit_fe-1.2.6/src/ambit_fe/ale/ale_variationalform.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    15484 2024-03-21 20:03:07.000000 ambit_fe-1.2.6/src/ambit_fe/ambit_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    12435 2024-04-20 20:55:31.000000 ambit_fe-1.2.6/src/ambit_fe/base.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    30256 2024-04-16 13:12:25.000000 ambit_fe-1.2.6/src/ambit_fe/boundaryconditions.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-04-26 13:05:20.255347 ambit_fe-1.2.6/src/ambit_fe/coupling/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:12.000000 ambit_fe-1.2.6/src/ambit_fe/coupling/__init__.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    21903 2024-04-20 20:54:02.000000 ambit_fe-1.2.6/src/ambit_fe/coupling/fluid_ale_flow0d_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    26536 2024-04-26 12:29:31.000000 ambit_fe-1.2.6/src/ambit_fe/coupling/fluid_ale_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    30684 2024-04-20 20:52:35.000000 ambit_fe-1.2.6/src/ambit_fe/coupling/fluid_flow0d_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    17941 2024-04-20 20:53:18.000000 ambit_fe-1.2.6/src/ambit_fe/coupling/fsi_flow0d_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    17156 2024-04-20 20:52:58.000000 ambit_fe-1.2.6/src/ambit_fe/coupling/fsi_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    21708 2024-04-20 20:52:44.000000 ambit_fe-1.2.6/src/ambit_fe/coupling/solid_constraint_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    38494 2024-04-20 20:52:51.000000 ambit_fe-1.2.6/src/ambit_fe/coupling/solid_flow0d_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     5219 2024-03-09 22:52:23.000000 ambit_fe-1.2.6/src/ambit_fe/coupling/solid_flow0d_periodicref_main.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-04-26 13:05:20.255347 ambit_fe-1.2.6/src/ambit_fe/electrophysiology/
+-rw-rw-r--   0 mh        (1001) mh        (1001)     1480 2024-02-12 18:01:07.000000 ambit_fe-1.2.6/src/ambit_fe/electrophysiology/electrophysiology_constitutive.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    14716 2024-04-11 19:20:57.000000 ambit_fe-1.2.6/src/ambit_fe/electrophysiology/electrophysiology_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)      947 2024-02-14 11:55:11.000000 ambit_fe-1.2.6/src/ambit_fe/electrophysiology/electrophysiology_variationalform.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     1242 2024-01-21 16:56:18.000000 ambit_fe-1.2.6/src/ambit_fe/expression.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-04-26 13:05:20.255347 ambit_fe-1.2.6/src/ambit_fe/flow0d/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:17.000000 ambit_fe-1.2.6/src/ambit_fe/flow0d/__init__.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    18497 2024-01-13 19:08:17.000000 ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     3521 2024-04-10 15:12:29.000000 ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D_2elwindkessel.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     4754 2024-04-10 15:13:30.000000 ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D_4elwindkesselLpZ.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     4431 2024-04-10 15:10:50.000000 ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D_4elwindkesselLsZ.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     3939 2024-01-13 19:08:16.000000 ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D_CRLinoutlink.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    15029 2024-01-13 19:08:16.000000 ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D_coronary.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    30594 2024-01-13 19:08:17.000000 ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D_syspul.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    78326 2024-01-13 19:08:17.000000 ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D_syspulcap.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    54451 2024-01-13 19:08:17.000000 ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D_syspulcaprespir.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     1666 2024-01-13 19:08:17.000000 ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D_vad.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    22429 2024-03-19 13:34:41.000000 ambit_fe-1.2.6/src/ambit_fe/flow0d/flow0d_main.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-04-26 13:05:20.255347 ambit_fe-1.2.6/src/ambit_fe/fluid/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:05.000000 ambit_fe-1.2.6/src/ambit_fe/fluid/__init__.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     2990 2024-04-09 07:24:44.000000 ambit_fe-1.2.6/src/ambit_fe/fluid/fluid_kinematics_constitutive.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    80725 2024-04-22 09:09:05.000000 ambit_fe-1.2.6/src/ambit_fe/fluid/fluid_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)      581 2024-01-13 19:08:05.000000 ambit_fe-1.2.6/src/ambit_fe/fluid/fluid_material.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    17756 2024-04-13 12:59:10.000000 ambit_fe-1.2.6/src/ambit_fe/fluid/fluid_variationalform.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     8416 2024-04-18 17:08:25.000000 ambit_fe-1.2.6/src/ambit_fe/ioparams.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    65866 2024-04-04 12:42:34.000000 ambit_fe-1.2.6/src/ambit_fe/ioroutines.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     3372 2024-01-13 19:07:42.000000 ambit_fe-1.2.6/src/ambit_fe/mathutils.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     5319 2024-01-13 19:07:42.000000 ambit_fe-1.2.6/src/ambit_fe/meshutils.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-04-26 13:05:20.255347 ambit_fe-1.2.6/src/ambit_fe/mor/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:53.000000 ambit_fe-1.2.6/src/ambit_fe/mor/__init__.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    31475 2024-04-26 12:41:43.000000 ambit_fe-1.2.6/src/ambit_fe/mor/mor_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     1667 2024-01-13 19:07:42.000000 ambit_fe-1.2.6/src/ambit_fe/mpiroutines.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-04-26 13:05:20.255347 ambit_fe-1.2.6/src/ambit_fe/multiscale/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:48.000000 ambit_fe-1.2.6/src/ambit_fe/multiscale/__init__.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    15481 2024-01-21 16:15:11.000000 ambit_fe-1.2.6/src/ambit_fe/multiscale/solid_flow0d_growthremodel_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     9642 2024-01-13 19:07:42.000000 ambit_fe-1.2.6/src/ambit_fe/oderoutines.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-04-26 13:05:20.255347 ambit_fe-1.2.6/src/ambit_fe/postprocess/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:38.000000 ambit_fe-1.2.6/src/ambit_fe/postprocess/__init__.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    72147 2024-01-29 08:41:01.000000 ambit_fe-1.2.6/src/ambit_fe/postprocess/flow0d_plot.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     4022 2024-03-04 18:00:59.000000 ambit_fe-1.2.6/src/ambit_fe/resultcheck.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-04-26 13:05:20.255347 ambit_fe-1.2.6/src/ambit_fe/signet/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:26.000000 ambit_fe-1.2.6/src/ambit_fe/signet/__init__.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    37626 2024-01-13 19:08:26.000000 ambit_fe-1.2.6/src/ambit_fe/signet/signet_hypertrophy.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    10380 2024-03-08 08:28:58.000000 ambit_fe-1.2.6/src/ambit_fe/signet/signet_main.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-04-26 13:05:20.255347 ambit_fe-1.2.6/src/ambit_fe/solid/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:01.000000 ambit_fe-1.2.6/src/ambit_fe/solid/__init__.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    26329 2024-03-15 14:40:16.000000 ambit_fe-1.2.6/src/ambit_fe/solid/solid_kinematics_constitutive.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    68974 2024-04-21 19:13:57.000000 ambit_fe-1.2.6/src/ambit_fe/solid/solid_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    14578 2024-03-15 14:39:57.000000 ambit_fe-1.2.6/src/ambit_fe/solid/solid_material.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     5572 2024-01-13 19:08:01.000000 ambit_fe-1.2.6/src/ambit_fe/solid/solid_variationalform.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-04-26 13:05:20.259347 ambit_fe-1.2.6/src/ambit_fe/solver/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:07:57.000000 ambit_fe-1.2.6/src/ambit_fe/solver/__init__.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    44975 2024-04-15 20:38:15.000000 ambit_fe-1.2.6/src/ambit_fe/solver/preconditioner.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     1904 2024-01-13 19:07:57.000000 ambit_fe-1.2.6/src/ambit_fe/solver/projection.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    47493 2024-04-18 13:23:14.000000 ambit_fe-1.2.6/src/ambit_fe/solver/solver_nonlin.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    26668 2024-01-13 19:07:57.000000 ambit_fe-1.2.6/src/ambit_fe/solver/solver_utils.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    31528 2024-04-26 12:42:52.000000 ambit_fe-1.2.6/src/ambit_fe/timeintegration.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     5823 2024-03-27 07:11:03.000000 ambit_fe-1.2.6/src/ambit_fe/utilities.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    12381 2024-03-19 17:33:23.000000 ambit_fe-1.2.6/src/ambit_fe/variationalform.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-04-26 13:05:20.271347 ambit_fe-1.2.6/src/ambit_fe.egg-info/
+-rw-r--r--   0 mh        (1001) mh        (1001)     6223 2024-04-26 13:05:20.000000 ambit_fe-1.2.6/src/ambit_fe.egg-info/PKG-INFO
+-rw-rw-r--   0 mh        (1001) mh        (1001)     5405 2024-04-26 13:05:20.000000 ambit_fe-1.2.6/src/ambit_fe.egg-info/SOURCES.txt
+-rw-rw-r--   0 mh        (1001) mh        (1001)        1 2024-04-26 13:05:20.000000 ambit_fe-1.2.6/src/ambit_fe.egg-info/dependency_links.txt
+-rw-rw-r--   0 mh        (1001) mh        (1001)       13 2024-04-26 13:05:20.000000 ambit_fe-1.2.6/src/ambit_fe.egg-info/requires.txt
+-rw-rw-r--   0 mh        (1001) mh        (1001)        9 2024-04-26 13:05:20.000000 ambit_fe-1.2.6/src/ambit_fe.egg-info/top_level.txt
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-04-26 13:05:20.271347 ambit_fe-1.2.6/tests/
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3042 2024-02-23 10:07:29.000000 ambit_fe-1.2.6/tests/test_ale_linelast.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     2937 2024-02-13 18:57:20.000000 ambit_fe-1.2.6/tests/test_electrophysiology.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     7081 2024-02-23 10:07:26.000000 ambit_fe-1.2.6/tests/test_flow0d_0dheart_syspul.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    15443 2024-02-23 10:07:22.000000 ambit_fe-1.2.6/tests/test_flow0d_0dheart_syspulcap.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    15626 2024-02-23 10:07:19.000000 ambit_fe-1.2.6/tests/test_flow0d_0dheart_syspulcapcor.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    22686 2024-02-23 10:07:15.000000 ambit_fe-1.2.6/tests/test_flow0d_0dheart_syspulcaprespir_periodic.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     7490 2024-02-23 10:07:09.000000 ambit_fe-1.2.6/tests/test_flow0d_0dheart_syspulcor.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     8426 2024-02-23 10:07:05.000000 ambit_fe-1.2.6/tests/test_flow0d_0dheart_syspulcorvad.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     2424 2024-02-23 10:07:01.000000 ambit_fe-1.2.6/tests/test_flow0d_0dvol_4elwindkesselLpZ.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     2358 2024-02-23 10:06:57.000000 ambit_fe-1.2.6/tests/test_flow0d_0dvol_4elwindkesselLsZ.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    10709 2024-04-13 13:02:57.000000 ambit_fe-1.2.6/tests/test_fluid_ale_flow0d_lalv_syspul_prescribed.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4535 2024-02-23 10:06:47.000000 ambit_fe-1.2.6/tests/test_fluid_flow0d_monolagr_taylorhood_cylinder.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3937 2024-04-09 06:48:19.000000 ambit_fe-1.2.6/tests/test_fluid_p1p1_stab_cylinder.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4356 2024-04-09 06:47:16.000000 ambit_fe-1.2.6/tests/test_fluid_p1p1_stab_cylinder_schur2x2.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4962 2024-04-16 13:13:06.000000 ambit_fe-1.2.6/tests/test_fluid_p1p1_stab_cylinder_valve.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3640 2024-02-23 10:06:18.000000 ambit_fe-1.2.6/tests/test_fluid_taylorhood_cylinder.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     6058 2024-04-22 10:18:34.000000 ambit_fe-1.2.6/tests/test_frsi_artseg_modepartitionunity.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4804 2024-03-25 09:01:11.000000 ambit_fe-1.2.6/tests/test_frsi_artseg_prefile.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     5868 2024-04-13 08:29:00.000000 ambit_fe-1.2.6/tests/test_frsi_artseg_prefile_bgsschur4x4.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     6016 2024-03-25 09:01:16.000000 ambit_fe-1.2.6/tests/test_frsi_artseg_prefile_partitioned_schur3x3.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     5358 2024-04-08 21:22:19.000000 ambit_fe-1.2.6/tests/test_frsi_artseg_prestress.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     7766 2024-04-09 06:52:03.000000 ambit_fe-1.2.6/tests/test_fsi_flow0d_p1p1_stab_artseg.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     6638 2024-04-09 06:51:31.000000 ambit_fe-1.2.6/tests/test_fsi_p1p1_stab_artseg.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     5667 2024-02-23 10:06:33.000000 ambit_fe-1.2.6/tests/test_fsi_taylorhood_artseg.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     2313 2024-03-08 08:27:18.000000 ambit_fe-1.2.6/tests/test_signet_0d_hypertrophy.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     2815 2024-03-15 14:39:36.000000 ambit_fe-1.2.6/tests/test_solid_2d_pres.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4995 2024-03-07 06:30:09.000000 ambit_fe-1.2.6/tests/test_solid_2dheart_frankstarling.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3769 2024-02-23 10:05:10.000000 ambit_fe-1.2.6/tests/test_solid_bodyforce_gravity.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3390 2024-02-23 10:05:06.000000 ambit_fe-1.2.6/tests/test_solid_constraint_volume_chamber.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3036 2024-02-23 10:05:02.000000 ambit_fe-1.2.6/tests/test_solid_divcont_ptc.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4079 2024-02-23 10:04:58.000000 ambit_fe-1.2.6/tests/test_solid_flow0d_monodir2field_4elwindkesselLpZ_chamber.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    18369 2024-04-13 14:32:00.000000 ambit_fe-1.2.6/tests/test_solid_flow0d_monodir2field_flux_syspulcap_3Dheart_schur3x3.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3997 2024-02-23 10:04:50.000000 ambit_fe-1.2.6/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4444 2024-03-30 11:46:33.000000 ambit_fe-1.2.6/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber_bgs2x2.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4619 2024-02-23 10:04:42.000000 ambit_fe-1.2.6/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber_bgs2x2fieldsplit.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    18252 2024-04-13 08:32:04.000000 ambit_fe-1.2.6/tests/test_solid_flow0d_monodir_flux_syspulcap_3Dheart_schur2x2.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    10261 2024-03-05 08:28:49.000000 ambit_fe-1.2.6/tests/test_solid_flow0d_monodir_syspul_2dheart_prestress.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    10378 2024-03-25 08:40:46.000000 ambit_fe-1.2.6/tests/test_solid_flow0d_monodir_syspulcor_2dheart_rom.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4196 2024-03-05 18:14:14.000000 ambit_fe-1.2.6/tests/test_solid_flow0d_monolagr2field_2elwindkessel_chamber.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4969 2024-02-23 10:04:20.000000 ambit_fe-1.2.6/tests/test_solid_flow0d_monolagr_CRLinoutlink_chambers.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    19455 2024-02-23 10:04:16.000000 ambit_fe-1.2.6/tests/test_solid_flow0d_multiscalegrowthremodeling_concentric.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    19437 2024-02-23 10:04:11.000000 ambit_fe-1.2.6/tests/test_solid_flow0d_multiscalegrowthremodeling_eccentric.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    11399 2024-03-09 22:53:35.000000 ambit_fe-1.2.6/tests/test_solid_flow0d_periodicref_syspul_lvchamber.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3302 2024-02-23 10:03:13.000000 ambit_fe-1.2.6/tests/test_solid_growth_prescribed_iso_lv.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3859 2024-02-23 10:04:01.000000 ambit_fe-1.2.6/tests/test_solid_growth_volstressmandel.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4034 2024-02-23 10:03:58.000000 ambit_fe-1.2.6/tests/test_solid_growth_volstressmandel_incomp.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4595 2024-02-23 10:03:55.000000 ambit_fe-1.2.6/tests/test_solid_growthremodeling_fiberstretch.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     7304 2024-02-23 10:03:51.000000 ambit_fe-1.2.6/tests/test_solid_mat_uniax_hex_2field.py
+-rwxr-xr-x   0 mh        (1001) mh        (1001)     7538 2024-01-21 17:16:25.000000 ambit_fe-1.2.6/tests/test_solid_membrane.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3710 2024-02-23 10:03:41.000000 ambit_fe-1.2.6/tests/test_solid_pinch_edge.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     3171 2024-02-23 10:03:37.000000 ambit_fe-1.2.6/tests/test_solid_plasticity_vonmises.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3523 2024-02-23 10:03:34.000000 ambit_fe-1.2.6/tests/test_solid_robin_genalpha.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3921 2024-03-19 07:42:47.000000 ambit_fe-1.2.6/tests/test_solid_robin_genalpha_amg.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3108 2024-02-23 10:03:26.000000 ambit_fe-1.2.6/tests/test_solid_robin_static_prestress.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3114 2024-02-23 10:03:22.000000 ambit_fe-1.2.6/tests/test_solid_robin_visco.py
```

### Comparing `ambit-fe-1.2.5/LICENSE` & `ambit_fe-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/PKG-INFO` & `ambit_fe-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ambit-fe
-Version: 1.2.5
+Version: 1.2.6
 Summary: A FEniCS-based cardiovascular multi-physics solver
-Author-email: Marc Hirschvogel <marc.hirschvogel@deepambit.com>
+Author-email: Marc Hirschvogel <marc.hirschvogel@ambit.net>
 License: MIT License
         
         Copyright (c) 2024 Marc Hirschvogel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `ambit-fe-1.2.5/README.md` & `ambit_fe-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/pyproject.toml` & `ambit_fe-1.2.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system] # Require setuptool version due to https://github.com/pypa/setuptools/issues/2938
 requires = ["setuptools>=61.0.0", "wheel"]
 
 [project]
 name = "ambit-fe"
-version = "v1.2.5"
+version = "v1.2.6"
 description = "A FEniCS-based cardiovascular multi-physics solver"
-authors = [{name = "Marc Hirschvogel", email = "marc.hirschvogel@deepambit.com"}]
+authors = [{name = "Marc Hirschvogel", email = "marc.hirschvogel@ambit.net"}]
 license = {file = "LICENSE"}
 readme = "README.md"
 keywords = [
     "finite elements",
     "solid mechanics",
     "fluid mechanics",
     "fluid-solid interaction",
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/ale/ale_kinematics_constitutive.py` & `ambit_fe-1.2.6/src/ambit_fe/ale/ale_kinematics_constitutive.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/ale/ale_main.py` & `ambit_fe-1.2.6/src/ambit_fe/ale/ale_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,30 +252,24 @@
         fem.petsc.assemble_vector(self.r_d, self.res_d)
         fem.apply_lifting(self.r_d, [self.jac_dd], [self.bc.dbcs], x0=[self.d.vector], scale=-1.0)
         self.r_d.ghostUpdate(addv=PETSc.InsertMode.ADD, mode=PETSc.ScatterMode.REVERSE)
         fem.set_bc(self.r_d, self.bc.dbcs, x0=self.d.vector, scale=-1.0)
 
         self.r_list[0] = self.r_d
 
-        if bool(self.pbase.residual_scale):
-            self.scale_residual_list(self.r_list, self.pbase.residual_scale)
-
 
     def assemble_stiffness(self, t, subsolver=None):
 
         # assemble system matrix
         self.K_dd.zeroEntries()
         fem.petsc.assemble_matrix(self.K_dd, self.jac_dd, self.bc.dbcs)
         self.K_dd.assemble()
 
         self.K_list[0][0] = self.K_dd
 
-        if bool(self.pbase.residual_scale):
-            self.scale_jacobian_list(self.K_list, self.pbase.residual_scale)
-
 
     ### now the base routines for this problem
 
     def read_restart(self, sname, N):
 
         # read restart information
         if self.pbase.restart_step > 0:
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/ale/ale_material.py` & `ambit_fe-1.2.6/src/ambit_fe/ale/ale_material.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/ale/ale_variationalform.py` & `ambit_fe-1.2.6/src/ambit_fe/ale/ale_variationalform.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/ambit_main.py` & `ambit_fe-1.2.6/src/ambit_fe/ambit_main.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/base.py` & `ambit_fe-1.2.6/src/ambit_fe/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,25 +116,25 @@
         raise RuntimeError("Problem misses function implementation!")
 
 
     def destroy(self):
         raise RuntimeError("Problem misses function implementation!")
 
 
-    def scale_residual_list(self, rlist, fac):
+    def scale_residual_list(self, rlist):
 
         for n in range(len(rlist)):
-            rlist[n].scale(fac[n])
+            rlist[n].scale(self.pbase.residual_scale[n])
 
 
-    def scale_jacobian_list(self, Klist, fac):
+    def scale_jacobian_list(self, Klist):
 
         for n in range(len(Klist)):
             for m in range(len(Klist)):
-                if Klist[n][m] is not None: Klist[n][m].scale(fac[n])
+                if Klist[n][m] is not None: Klist[n][m].scale(self.pbase.residual_scale[n])
 
 
 
 class solver_base():
 
     def __init__(self, problem, solver_params):
 
@@ -347,20 +347,20 @@
             self.pb.r_list[n].destroy()
             for m in range(self.pb.nfields):
                 if self.pb.K_list[n][m] is not None:
                     self.pb.K_list[n][m].destroy()
 
         # destroy ROM-specific ones
         if self.pb.pbase.have_rom:
-            if self.pb.pbrom.rom:
-                self.pb.pbrom.rom.destroy()
-                self.pb.pbrom.K_list_tmp[0][0].destroy()
-                for n in range(self.pb.pbrom.nfields):
-                    self.pb.pbrom.r_list_rom[n].destroy()
-                    for m in range(self.pb.pbrom.nfields):
-                        if self.pb.pbrom.K_list_rom[n][m] is not None:
-                            self.pb.pbrom.K_list_rom[n][m].destroy()
+            if self.pb.rom:
+                self.pb.rom.destroy()
+                self.pb.pbrom_host.K_list_tmp[0][0].destroy()
+                for n in range(self.pb.pbrom_host.nfields):
+                    self.pb.pbrom_host.r_list_rom[n].destroy()
+                    for m in range(self.pb.pbrom_host.nfields):
+                        if self.pb.pbrom_host.K_list_rom[n][m] is not None:
+                            self.pb.pbrom_host.K_list_rom[n][m].destroy()
 
         # destroy solver data structures
         self.solnln.destroy()
         try: self.solverprestr.destroy()
         except: pass
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/boundaryconditions.py` & `ambit_fe-1.2.6/src/ambit_fe/boundaryconditions.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,36 +51,42 @@
             if codim==self.dim-1: mdata = self.io.mt_b1
             if codim==self.dim-2: mdata = self.io.mt_b2
             if codim==self.dim-3: mdata = self.io.mt_b3
 
             func = fem.Function(V)
 
             if 'curve' in d.keys():
-                assert('val' not in d.keys() and 'expression' not in d.keys())
+                assert('val' not in d.keys() and 'expression' not in d.keys() and 'file' not in d.keys())
                 load = expression.template_vector(dim=self.dim)
                 if d['dir'] == 'all': curve_x, curve_y, curve_z = d['curve'][0], d['curve'][1], d['curve'][2]
                 else:                 curve_x, curve_y, curve_z = d['curve'], d['curve'], d['curve']
                 load.val_x, load.val_y, load.val_z = self.ti.timecurves(curve_x)(self.ti.t_init), self.ti.timecurves(curve_y)(self.ti.t_init), self.ti.timecurves(curve_z)(self.ti.t_init)
                 func.interpolate(load.evaluate)
                 func.vector.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
                 self.ti.funcs_to_update_vec.append({func : [self.ti.timecurves(curve_x), self.ti.timecurves(curve_y), self.ti.timecurves(curve_z)]})
                 self.ti.funcs_to_update_vec_old.append({None : -1}) # DBCs don't need an old state
             elif 'val' in d.keys():
-                assert('curve' not in d.keys() and 'expression' not in d.keys())
+                assert('curve' not in d.keys() and 'expression' not in d.keys() and 'file' not in d.keys())
                 func.vector.set(d['val'])
             elif 'expression' in d.keys():
-                assert('curve' not in d.keys() and 'val' not in d.keys())
+                assert('curve' not in d.keys() and 'val' not in d.keys() and 'file' not in d.keys())
                 expr = d['expression']()
                 expr.t = self.ti.t_init
                 func.interpolate(expr.evaluate)
                 func.vector.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
                 self.ti.funcsexpr_to_update_vec[func] = expr
                 self.ti.funcsexpr_to_update_vec_old[func] = None # DBCs don't need an old state
+            elif 'file' in d.keys():
+                assert('curve' not in d.keys() and 'val' not in d.keys() and 'expression' not in d.keys())
+                fle = d['file'] # a single file
+                try: ftype = d['ftype']
+                except: ftype = 'id_val'
+                self.io.readfunction(func, fle, filetype=ftype)
             else:
-                raise RuntimeError("Need to have 'curve', 'val', or 'expression' specified!")
+                raise RuntimeError("Need to have 'curve', 'val', 'expression', or 'file' specified!")
 
             if d['dir'] == 'all':
                 for i in range(len(d['id'])):
                     self.dbcs.append( fem.dirichletbc(func, fem.locate_dofs_topological(V, codim, mdata.indices[mdata.values == d['id'][i]])) )
 
             elif d['dir'] == 'x':
                 for i in range(len(d['id'])):
@@ -116,31 +122,28 @@
     def dirichlet_vol(self, bcdict, V):
 
         for d in bcdict:
 
             func = fem.Function(V)
 
             if 'curve' in d.keys():
-                assert('val' not in d.keys())
-                assert('file' not in d.keys())
+                assert('val' not in d.keys() and 'file' not in d.keys())
                 load = expression.template_vector(dim=self.dim)
                 if d['dir'] == 'all': curve_x, curve_y, curve_z = d['curve'][0], d['curve'][1], d['curve'][2]
                 else:                 curve_x, curve_y, curve_z = d['curve'], d['curve'], d['curve']
                 load.val_x, load.val_y, load.val_z = self.ti.timecurves(curve_x)(self.ti.t_init), self.ti.timecurves(curve_y)(self.ti.t_init), self.ti.timecurves(curve_z)(self.ti.t_init)
                 func.interpolate(load.evaluate)
                 func.vector.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
                 self.ti.funcs_to_update_vec.append({func : [self.ti.timecurves(curve_x), self.ti.timecurves(curve_y), self.ti.timecurves(curve_z)]})
                 self.ti.funcs_to_update_vec_old.append({None : -1}) # DBCs don't need an old state
             elif 'val' in d.keys():
-                assert('curve' not in d.keys())
-                assert('file' not in d.keys())
+                assert('curve' not in d.keys() and 'file' not in d.keys())
                 func.vector.set(d['val'])
-            elif 'file' in d.keys():
-                assert('val' not in d.keys())
-                assert('curve' not in d.keys())
+            elif 'file' in d.keys(): # file series, where we'd have one file per time step
+                assert('val' not in d.keys() and 'curve' not in d.keys())
                 try: scale = d['scale']
                 except: scale = 1.0
                 self.ti.funcs_data.append({func : d['file'], 'scale' : scale})
                 self.have_dirichlet_file = True
             else:
                 raise RuntimeError("Need to have 'curve', 'val', or 'file' specified!")
 
@@ -540,19 +543,41 @@
 
             if codim==self.dim-1: dind=0
             elif codim==self.dim-2: dind=1
             else: raise ValueError("Wrong codimension of boundary.")
 
             for i in range(len(sn['id'])):
 
-                par1 = sn['par1']
-                try: par2 = sn['par2']
-                except: par2 = 0.
+                beta = sn['beta']
+
+                w += self.vf.deltaW_ext_stabilized_neumann(v, beta, ds_[dind](sn['id'][i]), w=wel, F=F)
+
+        return w
+
+
+    # set mod. stabilized Neumann BCs
+    def stabilized_neumann_mod_bcs(self, bcdict, v, ds_, wel=None, F=None):
+
+        w = ufl.as_ufl(0)
+
+        for sn in bcdict:
+
+            try: codim = sn['codimension']
+            except: codim = self.dim - 1
+
+            if codim==self.dim-1: dind=0
+            elif codim==self.dim-2: dind=1
+            else: raise ValueError("Wrong codimension of boundary.")
+
+            for i in range(len(sn['id'])):
+
+                beta = sn['beta']
+                gamma = sn['gamma']
 
-                w += self.vf.deltaW_ext_stabilized_neumann(v, par1, par2, ds_[dind](sn['id'][i]), w=wel, F=F)
+                w += self.vf.deltaW_ext_stabilized_neumann_mod(v, beta, gamma, ds_[dind](sn['id'][i]), w=wel, F=F)
 
         return w
 
 
     # set Robin valve BCs
     def robin_valve_bcs(self, bcdict, v, V_real, beta_, dS_, wel=None, F=None):
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/coupling/fluid_ale_flow0d_main.py` & `ambit_fe-1.2.6/src/ambit_fe/coupling/fluid_ale_flow0d_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         alevariables = {'Fale' : self.pba.ki.F(self.pba.d), 'Fale_old' : self.pba.ki.F(self.pba.d_old), 'w' : self.pba.wel, 'w_old' : self.pba.w_old}
         self.pbf0 = FluidmechanicsFlow0DProblem(pbase, io_params, time_params_fluid, time_params_flow0d, fem_params_fluid, constitutive_models_fluid, model_params_flow0d, bc_dict_fluid, time_curves, coupling_params_fluid_flow0d, io, mor_params=mor_params, alevar=alevariables)
 
         self.pbf = self.pbf0.pbf
         self.pb0 = self.pbf0.pb0
 
         self.pbrom = self.pbf # ROM problem can only be fluid
+        self.pbrom_host = self
 
         # modify results to write...
         self.pbf.results_to_write = io_params['results_to_write'][0]
         self.pba.results_to_write = io_params['results_to_write'][1]
 
         self.io = io
 
@@ -244,17 +245,14 @@
             # NOTE: only set the surface-subset of the k_sd vector entries to avoid placing unnecessary zeros!
             self.k_sd_vec[i].getSubVector(self.dofs_coupling_vq[i], subvec=self.k_sd_subvec[i])
             self.K_sd.setValues(self.pbf0.row_ids[i], self.dofs_coupling_vq[i], self.k_sd_subvec[i].array, addv=PETSc.InsertMode.INSERT)
             self.k_sd_vec[i].restoreSubVector(self.dofs_coupling_vq[i], subvec=self.k_sd_subvec[i])
 
         self.K_sd.assemble()
 
-        if bool(self.pbase.residual_scale):
-            self.K_sd.scale(self.pbase.residual_scale[2])
-
         self.K_list[2][3] = self.K_sd
         self.K_list[3][3] = self.pba.K_list[0][0]
 
 
     def get_index_sets(self, isoptions={}):
 
         if self.rom is not None: # currently, ROM can only be on (subset of) first variable
@@ -500,14 +498,15 @@
                     self.pb.pbf.rom.set_reduced_data_structures_residual(self.pb.pbf.r_list, self.pb.pbf.r_list_rom)
                     self.pb.pbf.K_list_tmp = [[None]]
                     self.pb.pbf.rom.set_reduced_data_structures_matrix(self.pb.pbf.K_list, self.pb.pbf.K_list_rom, self.pb.pbf.K_list_tmp)
 
         elif self.pb.coupling_strategy=='partitioned':
 
             self.pb.pbf0.rom = self.pb.rom
+            self.pb.pbrom_host = self.pb.pbf0 # overridden
 
             self.pb.assemble_residual(self.pb.pbase.t_init, subsolver=None)
             self.pb.pbf0.assemble_stiffness(self.pb.pbase.t_init, subsolver=subsolver)
             self.pb.pba.assemble_stiffness(self.pb.pbase.t_init)
 
             # create ROM matrix structures
             if self.pb.pbf0.rom:
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/coupling/fluid_ale_main.py` & `ambit_fe-1.2.6/src/ambit_fe/coupling/fluid_ale_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         # initialize problem instances (also sets the variational forms for the fluid and ALE problem)
         self.pba = AleProblem(pbase, io_params, time_params, fem_params_ale, constitutive_models_ale, bc_dict_ale, time_curves, io, mor_params=mor_params)
         # ALE variables that are handed to fluid problem
         alevariables = {'Fale' : self.pba.ki.F(self.pba.d), 'Fale_old' : self.pba.ki.F(self.pba.d_old), 'w' : self.pba.wel, 'w_old' : self.pba.w_old}
         self.pbf = FluidmechanicsProblem(pbase, io_params, time_params, fem_params_fluid, constitutive_models_fluid, bc_dict_fluid, time_curves, io, mor_params=mor_params, alevar=alevariables)
 
         self.pbrom = self.pbf # ROM problem can only be fluid
+        self.pbrom_host = self
 
         # modify results to write...
         self.pbf.results_to_write = io_params['results_to_write'][0]
         self.pba.results_to_write = io_params['results_to_write'][1]
 
         self.io = io
 
@@ -335,23 +336,21 @@
         self.K_list[2][2] = self.pba.K_list[0][0]
 
 
     def evaluate_residual_dbc_coupling(self):
 
         if self.have_dbc_fluid_ale:
             # we need a vector representation of ufluid to apply in ALE DBCs
-            if self.pbf.ti.timint == 'ost': self.pbf.ti.update_varint_ost(self.pbf.v.vector, self.pbf.v_old.vector, self.pbf.uf_old.vector, varintout=self.pbf.uf.vector, ufl=False)
-            if self.pbf.ti.timint == 'genalpha': self.pbf.ti.update_varint_newmark_1st(self.pbf.v.vector, self.pbf.v_old.vector, self.pbf.uf_old.vector, varintout=self.pbf.uf.vector, ufl=False)
+            self.pbf.ti.update_varint(self.pbf.v.vector, self.pbf.v_old.vector, self.pbf.uf_old.vector, self.pbase.dt, varintout=self.pbf.uf.vector, uflform=False)
             self.ufa.vector.axpby(1.0, 0.0, self.pbf.uf.vector)
             self.ufa.vector.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
 
         if self.have_dbc_ale_fluid:
             # we need a vector representation of w to apply in fluid DBCs
-            if self.pbf.ti.timint == 'ost': self.pba.ti.update_dvar_ost(self.pba.d.vector, self.pba.d_old.vector, self.pba.w_old.vector, dvarout=self.pba.w.vector, ufl=False)
-            if self.pbf.ti.timint == 'genalpha': self.pba.ti.update_dvar_newmark_1st(self.pba.d.vector, self.pba.d_old.vector, self.pba.w_old.vector, dvarout=self.pba.w.vector, ufl=False)
+            self.pba.ti.update_dvar(self.pba.d.vector, self.pba.d_old.vector, self.pba.w_old.vector, self.pbase.dt, dvarout=self.pba.w.vector, uflform=False)
             self.wf.vector.axpby(1.0, 0.0, self.pba.w.vector)
             self.wf.vector.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
 
 
     def get_index_sets(self, isoptions={}):
 
         if self.rom is not None: # currently, ROM can only be on (subset of) first variable
@@ -576,14 +575,15 @@
                     self.pb.pbf.rom.set_reduced_data_structures_residual(self.pb.pbf.r_list, self.pb.pbf.r_list_rom)
                     self.pb.pbf.K_list_tmp = [[None]]
                     self.pb.pbf.rom.set_reduced_data_structures_matrix(self.pb.pbf.K_list, self.pb.pbf.K_list_rom, self.pb.pbf.K_list_tmp)
 
         elif self.pb.coupling_strategy=='partitioned':
 
             self.pb.pbf.rom = self.pb.rom
+            self.pb.pbrom_host = self.pb.pbf # overridden
 
             self.pb.assemble_residual(self.pb.pbase.t_init)
             self.pb.pbf.assemble_stiffness(self.pb.pbase.t_init)
             self.pb.pba.assemble_stiffness(self.pb.pbase.t_init)
 
             # create ROM matrix structures
             if self.pb.pbf.rom:
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/coupling/fluid_flow0d_main.py` & `ambit_fe-1.2.6/src/ambit_fe/coupling/fluid_flow0d_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         time_params_flow0d['numstep'] = time_params_fluid['numstep']
 
         # initialize problem instances (also sets the variational forms for the fluid problem)
         self.pbf = FluidmechanicsProblem(pbase, io_params, time_params_fluid, fem_params, constitutive_models, bc_dict, time_curves, io, mor_params=mor_params, alevar=alevar)
         self.pb0 = Flow0DProblem(pbase, io_params, time_params_flow0d, model_params_flow0d, time_curves, coupling_params)
 
         self.pbrom = self.pbf # ROM problem can only be fluid
+        self.pbrom_host = self
 
         # indicator for no periodic reference state estimation
         self.noperiodicref = 1
 
         self.set_variational_forms()
 
         self.numdof = self.pbf.numdof + self.LM.getSize()
@@ -320,17 +321,14 @@
 
         self.r_lm.assemble()
 
         self.r_list[2] = self.r_lm
 
         del LM_sq
 
-        if bool(self.pbase.residual_scale):
-            self.scale_residual_list([self.r_lm], [self.pbase.residual_scale[2]])
-
 
     def assemble_stiffness(self, t, subsolver=None):
 
         # Lagrange multipliers (pressures) to be passed to 0D model
         LM_sq = allgather_vec(self.LM, self.comm)
 
         for i in range(self.num_coupling_surf):
@@ -423,19 +421,14 @@
             # NOTE: only set the surface-subset of the k_sv vector entries to avoid placing unnecessary zeros!
             self.k_sv_vec[i].getSubVector(self.dofs_coupling_vq[i], subvec=self.k_sv_subvec[i])
             self.K_sv.setValues(self.row_ids[i], self.dofs_coupling_vq[i], self.k_sv_subvec[i].array, addv=PETSc.InsertMode.INSERT)
             self.k_sv_vec[i].restoreSubVector(self.dofs_coupling_vq[i], subvec=self.k_sv_subvec[i])
 
         self.K_sv.assemble()
 
-        if bool(self.pbase.residual_scale):
-            self.K_vs.scale(self.pbase.residual_scale[0])
-            self.K_sv.scale(self.pbase.residual_scale[2])
-            self.K_lm.scale(self.pbase.residual_scale[2])
-
         self.K_list[0][2] = self.K_vs
         self.K_list[2][0] = self.K_sv
 
 
     def get_index_sets(self, isoptions={}):
 
         if self.rom is not None: # currently, ROM can only be on (subset of) first variable
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/coupling/fsi_flow0d_main.py` & `ambit_fe-1.2.6/src/ambit_fe/coupling/fsi_flow0d_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,16 @@
         self.pbfa0 = FluidmechanicsAleFlow0DProblem(pbase, io_params, time_params_fluid, time_params_flow0d, fem_params_fluid, fem_params_ale, constitutive_models_fluid_ale[0], constitutive_models_fluid_ale[1], model_params_flow0d, bc_dict_fluid_ale[0], bc_dict_fluid_ale[1], time_curves, coupling_params_fluid_ale, coupling_params_fluid_flow0d, iof, mor_params=mor_params)
 
         self.pbf = self.pbfa0.pbf
         self.pbf0 = self.pbfa0.pbf0
         self.pb0 = self.pbfa0.pb0
         self.pba = self.pbfa0.pba
 
-        self.pbrom = self.pbf # ROM problem can only be fluid
+        self.pbrom = self.pbs # ROM problem can only be solid
+        self.pbrom_host = self
 
         # modify results to write...
         self.pbs.results_to_write = io_params['results_to_write'][0]
         self.pbf.results_to_write = io_params['results_to_write'][1][0]
         self.pba.results_to_write = io_params['results_to_write'][1][1]
 
         self.incompressible_2field = self.pbs.incompressible_2field
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/coupling/fsi_main.py` & `ambit_fe-1.2.6/src/ambit_fe/coupling/fsi_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
             assert(time_params_fluid['dt'] == time_params_solid['dt'])
 
         # initialize problem instances (also sets the variational forms for the solid and fluid problem)
         self.pbs  = SolidmechanicsProblem(pbase, io_params, time_params_solid, fem_params_solid, constitutive_models_solid, bc_dict_solid, time_curves, ios, mor_params=mor_params)
         self.pbfa = FluidmechanicsAleProblem(pbase, io_params, time_params_fluid, fem_params_fluid, fem_params_ale, constitutive_models_fluid_ale[0], constitutive_models_fluid_ale[1], bc_dict_fluid_ale[0], bc_dict_fluid_ale[1], time_curves, coupling_params, iof, mor_params=mor_params)
 
         self.pbrom = self.pbs # ROM problem can only be solid so far...
+        self.pbrom_host = self
 
         self.pbf = self.pbfa.pbf
         self.pba = self.pbfa.pba
 
         # modify results to write...
         self.pbs.results_to_write = io_params['results_to_write'][0]
         self.pbf.results_to_write = io_params['results_to_write'][1][0]
@@ -210,17 +211,14 @@
 
         self.r_list[1+off] = self.pbfa.r_list[0]
         self.r_list[2+off] = self.pbfa.r_list[1]
 
         self.r_list[3+off] = self.r_l
         self.r_list[4+off] = self.pbfa.r_list[2]
 
-        if bool(self.pbase.residual_scale):
-            self.scale_residual_list([self.r_l], [self.pbase.residual_scale[3+off]])
-
 
     def assemble_stiffness(self, t, subsolver=None):
 
         if self.pbs.incompressible_2field: off = 1
         else: off = 0
 
         self.pbs.assemble_stiffness(t)
@@ -269,20 +267,14 @@
         fem.petsc.assemble_matrix(self.K_ll, self.jac_ll, self.bclm.dbcs)
         self.K_ll.assemble()
         self.K_list[3+off][3+off] = self.K_ll
 
         # ALE displacement
         self.K_list[4+off][4+off] = self.pbfa.K_list[2][2]
 
-        if bool(self.pbase.residual_scale):
-            self.K_ul.scale(self.pbase.residual_scale[0])
-            self.K_lu.scale(self.pbase.residual_scale[3+off])
-            self.K_vl.scale(self.pbase.residual_scale[1+off])
-            self.K_lv.scale(self.pbase.residual_scale[3+off])
-
 
     ### now the base routines for this problem
 
     def read_restart(self, sname, N):
 
         # read restart information
         if N > 0:
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/coupling/solid_constraint_main.py` & `ambit_fe-1.2.6/src/ambit_fe/coupling/solid_constraint_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
         self.prescribed_curve = self.coupling_params['prescribed_curve']
 
         # initialize problem instances (also sets the variational forms for the solid problem)
         self.pbs = SolidmechanicsProblem(pbase, io_params, time_params_solid, fem_params, constitutive_models, bc_dict, time_curves, io, mor_params=mor_params)
 
         self.pbrom = self.pbs
+        self.pbrom_host = self
 
         self.incompressible_2field = self.pbs.incompressible_2field
 
         self.set_variational_forms_and_jacobians()
 
         self.numdof = self.pbs.numdof + self.LM.getSize()
 
@@ -276,17 +277,14 @@
         for i in range(ls,le):
             self.r_lm[i] = self.constr[i] - val[i]
 
         self.r_lm.assemble()
 
         self.r_list[1+off] = self.r_lm
 
-        if bool(self.pbase.residual_scale):
-            self.scale_residual_list([r_lm], [self.pbase.residual_scale[1+off]])
-
 
     def assemble_stiffness(self, t, subsolver=None):
 
         if self.pbs.incompressible_2field: off = 1
         else: off = 0
 
         # add to solid momentum equation
@@ -329,19 +327,14 @@
             # NOTE: only set the surface-subset of the k_su vector entries to avoid placing unnecessary zeros!
             self.k_su_vec[i].getSubVector(self.dofs_coupling[i], subvec=self.k_su_subvec[i])
             self.K_su.setValues(self.row_ids[i], self.dofs_coupling[i], self.k_su_subvec[i].array, addv=PETSc.InsertMode.INSERT)
             self.k_su_vec[i].restoreSubVector(self.dofs_coupling[i], subvec=self.k_su_subvec[i])
 
         self.K_su.assemble()
 
-        if bool(self.pbase.residual_scale):
-            self.K_us.scale(self.pbase.residual_scale[0])
-            self.K_su.scale(self.pbase.residual_scale[1+off])
-            self.K_lm.scale(self.pbase.residual_scale[1+off])
-
         self.K_list[0][1+off] = self.K_us
         self.K_list[1+off][0] = self.K_su
 
 
     def get_index_sets(self, isoptions={}):
 
         if self.rom is not None: # currently, ROM can only be on (subset of) first variable
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/coupling/solid_flow0d_main.py` & `ambit_fe-1.2.6/src/ambit_fe/coupling/solid_flow0d_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
         time_params_flow0d['numstep'] = time_params_solid['numstep']
 
         # initialize problem instances (also sets the variational forms for the solid problem)
         self.pbs = SolidmechanicsProblem(pbase, io_params, time_params_solid, fem_params, constitutive_models, bc_dict, time_curves, io, mor_params=mor_params)
         self.pb0 = Flow0DProblem(pbase, io_params, time_params_flow0d, model_params_flow0d, time_curves, coupling_params)
 
         self.pbrom = self.pbs # ROM problem can only be solid
+        self.pbrom_host = self
 
         self.incompressible_2field = self.pbs.incompressible_2field
 
         # for multiscale G&R analysis
         self.t_prev = 0
         self.t_gandr_setpoint = 0
         self.restart_multiscale = False
@@ -451,17 +452,14 @@
 
             self.r_lm.assemble()
 
             self.r_list[1+off] = self.r_lm
 
             del LM_sq
 
-        if bool(self.pbase.residual_scale):
-            self.scale_residual_list([self.r_list[1+off]], [self.pbase.residual_scale[1+off]])
-
 
     def assemble_stiffness(self, t, subsolver=None):
 
         if self.pbs.incompressible_2field: off = 1
         else: off = 0
 
         if self.coupling_type == 'monolithic_lagrange':
@@ -574,19 +572,14 @@
             # NOTE: only set the surface-subset of the k_su vector entries to avoid placing unnecessary zeros!
             self.k_su_vec[i].getSubVector(self.dofs_coupling_vq[i], subvec=self.k_su_subvec[i])
             self.K_su.setValues(self.row_ids[i], self.dofs_coupling_vq[i], self.k_su_subvec[i].array, addv=PETSc.InsertMode.INSERT)
             self.k_su_vec[i].restoreSubVector(self.dofs_coupling_vq[i], subvec=self.k_su_subvec[i])
 
         self.K_su.assemble()
 
-        if bool(self.pbase.residual_scale):
-            self.K_us.scale(self.pbase.residual_scale[0])
-            self.K_su.scale(self.pbase.residual_scale[1+off])
-            self.K_list[1+off][1+off].scale(self.pbase.residual_scale[1+off])
-
         self.K_list[0][1+off] = self.K_us
         self.K_list[1+off][0] = self.K_su
 
 
     def get_index_sets(self, isoptions={}):
 
         if self.rom is not None: # currently, ROM can only be on (subset of) first variable
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/coupling/solid_flow0d_periodicref_main.py` & `ambit_fe-1.2.6/src/ambit_fe/coupling/solid_flow0d_periodicref_main.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/electrophysiology/electrophysiology_constitutive.py` & `ambit_fe-1.2.6/src/ambit_fe/electrophysiology/electrophysiology_constitutive.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/electrophysiology/electrophysiology_main.py` & `ambit_fe-1.2.6/src/ambit_fe/electrophysiology/electrophysiology_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,30 +250,24 @@
         fem.petsc.assemble_vector(self.r_phi, self.res_phi)
         fem.apply_lifting(self.r_phi, [self.jac_phiphi], [self.bc.dbcs], x0=[self.phi.vector], scale=-1.0)
         self.r_phi.ghostUpdate(addv=PETSc.InsertMode.ADD, mode=PETSc.ScatterMode.REVERSE)
         fem.set_bc(self.r_phi, self.bc.dbcs, x0=self.phi.vector, scale=-1.0)
 
         self.r_list[0] = self.r_phi
 
-        if bool(self.residual_scale):
-            self.scale_residual_list(self.r_list, self.residual_scale)
-
 
     def assemble_stiffness(self, t, subsolver=None):
 
         # assemble system matrix
         self.K_phiphi.zeroEntries()
         fem.petsc.assemble_matrix(self.K_phiphi, self.jac_phiphi, self.bc.dbcs)
         self.K_phiphi.assemble()
 
         self.K_list[0][0] = self.K_phiphi
 
-        if bool(self.residual_scale):
-            self.scale_jacobian_list(self.K_list, self.residual_scale)
-
 
     ### now the base routines for this problem
 
     def read_restart(self, sname, N):
 
         # read restart information
         if self.restart_step > 0:
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/electrophysiology/electrophysiology_variationalform.py` & `ambit_fe-1.2.6/src/ambit_fe/electrophysiology/electrophysiology_variationalform.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/expression.py` & `ambit_fe-1.2.6/src/ambit_fe/expression.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D.py` & `ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D_2elwindkessel.py` & `ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D_2elwindkessel.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D_4elwindkesselLpZ.py` & `ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D_4elwindkesselLpZ.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,23 +59,25 @@
 
     def setup_arrays(self):
 
         # number of degrees of freedom
         self.numdof = 4
 
         self.v_ids = [0]
-        self.c_ids = [2]
 
         if self.cq[0] == 'volume':
+            self.c_ids = [2]
             assert(self.vq[0]=='pressure')
             self.switch_V, self.cname, self.vname = 1, 'V', 'p'
         elif self.cq[0] == 'flux':
+            self.c_ids = [2]
             assert(self.vq[0]=='pressure')
             self.switch_V, self.cname, self.vname = 0, 'Q', 'p'
         elif self.cq[0] == 'pressure':
+            self.c_ids = [0]
             if self.vq[0] == 'flux':
                 self.switch_V, self.cname, self.vname = 0, 'p', 'Q'
             elif self.vq[0] == 'volume':
                 self.switch_V, self.cname, self.vname = 1, 'p', 'V'
             else:
                 raise ValueError("Unknown variable quantity!")
         else:
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D_4elwindkesselLsZ.py` & `ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D_4elwindkesselLsZ.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,23 +58,25 @@
 
     def setup_arrays(self):
 
         # number of degrees of freedom
         self.numdof = 3
 
         self.v_ids = [0]
-        self.c_ids = [1]
 
         if self.cq[0] == 'volume':
+            self.c_ids = [1]
             assert(self.vq[0]=='pressure')
             self.switch_V, self.cname, self.vname = 1, 'V', 'p'
         elif self.cq[0] == 'flux':
+            self.c_ids = [1]
             assert(self.vq[0]=='pressure')
             self.switch_V, self.cname, self.vname = 0, 'Q', 'p'
         elif self.cq[0] == 'pressure':
+            self.c_ids = [0]
             if self.vq[0] == 'flux':
                 self.switch_V, self.cname, self.vname = 0, 'p', 'Q'
             elif self.vq[0] == 'volume':
                 self.switch_V, self.cname, self.vname = 1, 'p', 'V'
             else:
                 raise ValueError("Unknown variable quantity!")
         else:
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D_CRLinoutlink.py` & `ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D_CRLinoutlink.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D_coronary.py` & `ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D_coronary.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D_syspul.py` & `ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D_syspul.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D_syspulcap.py` & `ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D_syspulcap.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D_syspulcaprespir.py` & `ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D_syspulcaprespir.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/flow0d/cardiovascular0D_vad.py` & `ambit_fe-1.2.6/src/ambit_fe/flow0d/cardiovascular0D_vad.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/flow0d/flow0d_main.py` & `ambit_fe-1.2.6/src/ambit_fe/flow0d/flow0d_main.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/fluid/fluid_kinematics_constitutive.py` & `ambit_fe-1.2.6/src/ambit_fe/fluid/fluid_kinematics_constitutive.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/fluid/fluid_main.py` & `ambit_fe-1.2.6/src/ambit_fe/fluid/fluid_main.py`

 * *Files 13% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         except: self.prestress_numstep = 1
         try: self.prestress_dt = fem_params['prestress_dt']
         except: self.prestress_dt = self.prestress_maxtime/self.prestress_numstep
         if 'prestress_dt' in fem_params.keys(): self.prestress_numstep = int(self.prestress_maxtime/self.prestress_dt)
         try: self.prestress_ptc = fem_params['prestress_ptc']
         except: self.prestress_ptc = False
         try: self.prestress_kinetic = fem_params['prestress_kinetic']
-        except: self.prestress_kinetic = False
+        except: self.prestress_kinetic = 'none'
         try: self.prestress_from_file = fem_params['prestress_from_file']
         except: self.prestress_from_file = False
         try: self.initial_fluid_pressure = fem_params['initial_fluid_pressure']
         except: self.initial_fluid_pressure = []
 
         if self.prestress_from_file: self.prestress_initial, self.prestress_initial_only  = False, False
 
@@ -253,15 +253,15 @@
             # values of previous time step
             self.p_old_ = [ fem.Function(self.V_p_[0]) ]
 
         # values of previous time step
         self.v_old  = fem.Function(self.V_v)
         self.a_old  = fem.Function(self.V_v)
         # auxiliary acceleration vector
-        self.a     = fem.Function(self.V_v, name="Acceleration")
+        self.a      = fem.Function(self.V_v, name="Acceleration")
         # a fluid displacement
         self.uf     = fem.Function(self.V_v, name="FluidDisplacement")
         self.uf_old = fem.Function(self.V_v)
         # active stress for reduced solid
         self.tau_a  = fem.Function(self.Vd_scalar, name="tau_a")
         self.tau_a_old = fem.Function(self.Vd_scalar)
         # prestress displacement for FrSI
@@ -270,14 +270,19 @@
         else:
             self.uf_pre = None
         if (self.prestress_initial or self.prestress_initial_only) and self.pbase.restart_step == 0:
             self.pre = True
         else:
             self.pre = False
 
+        # for ROM, provide pointers to main variable, its derivative, and possibly its time integrated value
+        if self.pbase.have_rom:
+            self.xr_, self.xr_old_, self.xrpre_ = self.v, self.v_old, None
+            self.xdtr_old_, self.xintr_old_, self.xintrpre_ = self.a_old, self.uf_old, self.uf_pre
+
         # collect references to pressure vectors
         self.pvecs_, self.pvecs_old_ = [], []
         if self.num_dupl > 1:
             for mp in range(self.num_dupl):
                 self.pvecs_.append(self.p_[mp].vector)
                 self.pvecs_old_.append(self.p_old_[mp].vector)
                 # full pressure vectors - dummy function that holds a class variable "vector"
@@ -372,14 +377,15 @@
 
         if 'dirichlet_vol' in self.bc_dict.keys():
             self.bc.dirichlet_vol(self.bc_dict['dirichlet_vol'], self.V_v)
 
         self.set_variational_forms()
 
         self.pbrom = self # self-pointer needed for ROM solver access
+        self.pbrom_host = self
         self.V_rom = self.V_v
         self.print_enhanced_info = self.io.print_enhanced_info
 
         # number of fields involved
         self.nfields = 2
 
         # residual and matrix lists
@@ -416,14 +422,17 @@
         else:
             self.pf_mid_ = [ self.timefac * self.p_[0] + (1.-self.timefac) * self.p_old_[0] ]
 
         # kinetic, internal, and pressure virtual power
         self.deltaW_kin, self.deltaW_kin_old, self.deltaW_kin_mid = ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0)
         self.deltaW_int, self.deltaW_int_old, self.deltaW_int_mid = ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0)
         self.deltaW_p,   self.deltaW_p_old,   self.deltaW_p_mid   = [], [], []
+        # element level Reynolds number components
+        self.Re_c,      self.Re_c_old,        self.Re_c_mid       = ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0)
+        self.Re_ktilde, self.Re_ktilde_old,   self.Re_ktilde_mid  = ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0)
 
         for n, M in enumerate(self.domain_ids):
 
             if self.num_dupl==1: j=0
             else: j=n
 
             # kinetic virtual power
@@ -450,18 +459,27 @@
             self.deltaW_int_mid += self.vf.deltaW_int(self.ma[n].sigma(self.vel_mid, self.pf_mid_[j], F=self.alevar['Fale_mid']), self.io.dx(M), F=self.alevar['Fale_mid'])
 
             # pressure virtual power
             self.deltaW_p.append( self.vf.deltaW_int_pres(self.v, self.var_p_[j], self.io.dx(M), F=self.alevar['Fale']) )
             self.deltaW_p_old.append( self.vf.deltaW_int_pres(self.v_old, self.var_p_[j], self.io.dx(M), F=self.alevar['Fale_old']) )
             self.deltaW_p_mid.append( self.vf.deltaW_int_pres(self.vel_mid, self.var_p_[j], self.io.dx(M), F=self.alevar['Fale_mid']) )
 
+            # element level Reynolds number components - not used so far! Need to assemble a cell-based vector in order to evaluate these...
+            self.Re_c      += self.vf.re_c(self.rho[n], self.v, self.io.dx(M), w=self.alevar['w'], F=self.alevar['Fale'])
+            self.Re_c_old  += self.vf.re_c(self.rho[n], self.v_old, self.io.dx(M), w=self.alevar['w_old'], F=self.alevar['Fale_old'])
+            self.Re_c_mid  += self.vf.re_c(self.rho[n], self.vel_mid, self.io.dx(M), w=self.alevar['w_mid'], F=self.alevar['Fale_mid'])
+
+            self.Re_ktilde     += self.vf.re_ktilde(self.rho[n], self.v, self.io.dx(M), w=self.alevar['w'], F=self.alevar['Fale'])
+            self.Re_ktilde_old += self.vf.re_ktilde(self.rho[n], self.v_old, self.io.dx(M), w=self.alevar['w_old'], F=self.alevar['Fale_old'])
+            self.Re_ktilde_mid += self.vf.re_ktilde(self.rho[n], self.vel_mid, self.io.dx(M), w=self.alevar['w_mid'], F=self.alevar['Fale_mid'])
+
         # external virtual power (from Neumann or Robin boundary conditions, body forces, ...)
-        w_neumann, w_body, w_robin, w_stabneumann, w_robin_valve, w_membrane = ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0)
-        w_neumann_old, w_body_old, w_robin_old, w_stabneumann_old, w_robin_valve_old, w_membrane_old = ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0)
-        w_neumann_mid, w_body_mid, w_robin_mid, w_stabneumann_mid, w_robin_valve_mid, w_membrane_mid = ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0)
+        w_neumann, w_body, w_robin, w_stabneumann, w_stabneumann_mod, w_robin_valve, w_membrane = ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0)
+        w_neumann_old, w_body_old, w_robin_old, w_stabneumann_old, w_stabneumann_mod_old, w_robin_valve_old, w_membrane_old = ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0)
+        w_neumann_mid, w_body_mid, w_robin_mid, w_stabneumann_mid, w_stabneumann_mod_mid, w_robin_valve_mid, w_membrane_mid = ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0)
         if 'neumann' in self.bc_dict.keys():
             w_neumann     = self.bc.neumann_bcs(self.bc_dict['neumann'], self.V_v, self.Vd_scalar, self.io.bmeasures, F=self.alevar['Fale'], funcs_to_update=self.ti.funcs_to_update, funcs_to_update_vec=self.ti.funcs_to_update_vec, funcsexpr_to_update=self.ti.funcsexpr_to_update, funcsexpr_to_update_vec=self.ti.funcsexpr_to_update_vec)
             w_neumann_old = self.bc.neumann_bcs(self.bc_dict['neumann'], self.V_v, self.Vd_scalar, self.io.bmeasures, F=self.alevar['Fale_old'], funcs_to_update=self.ti.funcs_to_update_old, funcs_to_update_vec=self.ti.funcs_to_update_vec_old, funcsexpr_to_update=self.ti.funcsexpr_to_update_old, funcsexpr_to_update_vec=self.ti.funcsexpr_to_update_vec_old)
             w_neumann_mid = self.bc.neumann_bcs(self.bc_dict['neumann'], self.V_v, self.Vd_scalar, self.io.bmeasures, F=self.alevar['Fale_mid'], funcs_to_update=self.ti.funcs_to_update_mid, funcs_to_update_vec=self.ti.funcs_to_update_vec_mid, funcsexpr_to_update=self.ti.funcsexpr_to_update_mid, funcsexpr_to_update_vec=self.ti.funcsexpr_to_update_vec_mid)
         if 'bodyforce' in self.bc_dict.keys():
             w_body      = self.bc.bodyforce(self.bc_dict['bodyforce'], self.V_v, self.Vd_scalar, self.io.dx, F=self.alevar['Fale'], funcs_to_update=self.ti.funcs_to_update, funcsexpr_to_update=self.ti.funcsexpr_to_update)
             w_body_old  = self.bc.bodyforce(self.bc_dict['bodyforce'], self.V_v, self.Vd_scalar, self.io.dx, F=self.alevar['Fale_old'], funcs_to_update=self.ti.funcs_to_update_old, funcsexpr_to_update=self.ti.funcsexpr_to_update_old)
@@ -470,14 +488,18 @@
             w_robin     = self.bc.robin_bcs(self.bc_dict['robin'], self.v, self.io.bmeasures, F=self.alevar['Fale'])
             w_robin_old = self.bc.robin_bcs(self.bc_dict['robin'], self.v_old, self.io.bmeasures, F=self.alevar['Fale_old'])
             w_robin_mid = self.bc.robin_bcs(self.bc_dict['robin'], self.vel_mid, self.io.bmeasures, F=self.alevar['Fale_mid'])
         if 'stabilized_neumann' in self.bc_dict.keys():
             w_stabneumann     = self.bc.stabilized_neumann_bcs(self.bc_dict['stabilized_neumann'], self.v, self.io.bmeasures, wel=self.alevar['w'], F=self.alevar['Fale'])
             w_stabneumann_old = self.bc.stabilized_neumann_bcs(self.bc_dict['stabilized_neumann'], self.v_old, self.io.bmeasures, wel=self.alevar['w_old'], F=self.alevar['Fale_old'])
             w_stabneumann_mid = self.bc.stabilized_neumann_bcs(self.bc_dict['stabilized_neumann'], self.vel_mid, self.io.bmeasures, wel=self.alevar['w_mid'], F=self.alevar['Fale_mid'])
+        if 'stabilized_neumann_mod' in self.bc_dict.keys():
+            w_stabneumann_mod     = self.bc.stabilized_neumann_mod_bcs(self.bc_dict['stabilized_neumann_mod'], self.v, self.io.bmeasures, wel=self.alevar['w'], F=self.alevar['Fale'])
+            w_stabneumann_mod_old = self.bc.stabilized_neumann_mod_bcs(self.bc_dict['stabilized_neumann_mod'], self.v_old, self.io.bmeasures, wel=self.alevar['w_old'], F=self.alevar['Fale_old'])
+            w_stabneumann_mod_mid = self.bc.stabilized_neumann_mod_bcs(self.bc_dict['stabilized_neumann_mod'], self.vel_mid, self.io.bmeasures, wel=self.alevar['w_mid'], F=self.alevar['Fale_mid'])
         if 'robin_valve' in self.bc_dict.keys():
             assert(self.num_dupl>1) # only makes sense if we have duplicate pressure domains
             self.have_robin_valve = True
             self.beta_valve, self.beta_valve_old = [], []
             w_robin_valve     = self.bc.robin_valve_bcs(self.bc_dict['robin_valve'], self.v, self.Vd_scalar, self.beta_valve, [self.io.dS], wel=self.alevar['w'], F=self.alevar['Fale'])
             w_robin_valve_old = self.bc.robin_valve_bcs(self.bc_dict['robin_valve'], self.v_old, self.Vd_scalar, self.beta_valve_old, [self.io.dS], wel=self.alevar['w_old'], F=self.alevar['Fale_old'])
             w_robin_valve_mid = self.bc.robin_valve_bcs(self.bc_dict['robin_valve'], self.vel_mid, self.Vd_scalar, self.beta_valve_old, [self.io.dS], wel=self.alevar['w_mid'], F=self.alevar['Fale_mid'])
@@ -523,118 +545,182 @@
                     self.io.readfunction(h0_func, self.bc_dict['membrane'][nm]['params']['h0']['field'])
                     self.wallfields.append(h0_func)
 
             w_membrane, self.idmem, self.bstress, self.bstrainenergy, self.bintpower = self.bc.membranesurf_bcs(self.bc_dict['membrane'], self.ufluid, self.v, self.acc, self.io.bmeasures, ivar=self.internalvars, wallfields=self.wallfields)
             w_membrane_old, _, _, _, _                                               = self.bc.membranesurf_bcs(self.bc_dict['membrane'], self.uf_old, self.v_old, self.a_old, self.io.bmeasures, ivar=self.internalvars_old, wallfields=self.wallfields)
             w_membrane_mid, _, _, _, _                                               = self.bc.membranesurf_bcs(self.bc_dict['membrane'], self.ufluid_mid, self.vel_mid, self.acc_mid, self.io.bmeasures, ivar=self.internalvars_mid, wallfields=self.wallfields)
 
-        w_neumann_prestr, self.deltaW_prestr_kin = ufl.as_ufl(0), ufl.as_ufl(0)
+        w_neumann_prestr, self.deltaW_prestr_kin, self.deltaW_prestr_int, self.deltaW_p_prestr = ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0), []
         if self.prestress_initial or self.prestress_initial_only:
-            # Stokes kinetic virtual power
+            self.acc_prestr = (self.v - self.v_old)/self.prestress_dt # in case acceleration is used (for kinetic prestress option)
             for n, M in enumerate(self.domain_ids):
+                if self.num_dupl==1: j=0
+                else: j=n
+                self.deltaW_prestr_int += self.vf.deltaW_int(self.ma[n].sigma(self.v, self.p_[j], F=self.alevar['Fale']), self.io.dx(M), F=self.alevar['Fale'])
+                self.deltaW_p_prestr.append( self.vf.deltaW_int_pres(self.v, self.var_p_[j], self.io.dx(M), F=self.alevar['Fale']) )
                 # it seems that we need some slight inertia for this to work smoothly, so let's use transient Stokes here (instead of steady Navier-Stokes or steady Stokes...)
-                self.deltaW_prestr_kin += self.vf.deltaW_kin_stokes_transient(self.acc, self.v, self.rho[n], self.io.dx(M), w=self.alevar['w'], F=self.alevar['Fale'])
+                if self.prestress_kinetic=='navierstokes_transient':
+                    self.deltaW_prestr_kin += self.vf.deltaW_kin_navierstokes_transient(self.acc_prestr, self.v, self.rho[n], self.io.dx(M), w=self.alevar['w'], F=self.alevar['Fale'])
+                elif self.prestress_kinetic=='navierstokes_steady':
+                    self.deltaW_prestr_kin += self.vf.deltaW_kin_navierstokes_steady(self.v, self.rho[n], self.io.dx(M), w=self.alevar['w'], F=self.alevar['Fale'])
+                elif self.prestress_kinetic=='stokes_transient':
+                    self.deltaW_prestr_kin += self.vf.deltaW_kin_stokes_transient(self.acc_prestr, self.v, self.rho[n], self.io.dx(M), w=self.alevar['w'], F=self.alevar['Fale'])
+                elif self.prestress_kinetic=='none':
+                    pass
+                else:
+                    raise ValueError("Unknown prestress_kinetic option. Choose either 'navierstokes_transient', 'navierstokes_steady', 'stokes_transient', or 'none'.")
             if 'neumann_prestress' in self.bc_dict.keys():
                 w_neumann_prestr = self.bc.neumann_prestress_bcs(self.bc_dict['neumann_prestress'], self.V_v, self.Vd_scalar, self.io.bmeasures, funcs_to_update=self.ti.funcs_to_update_pre, funcs_to_update_vec=self.ti.funcs_to_update_vec_pre, funcsexpr_to_update=self.ti.funcsexpr_to_update_pre, funcsexpr_to_update_vec=self.ti.funcsexpr_to_update_vec_pre)
             if 'membrane' in self.bc_dict.keys():
                 self.ufluid_prestr = self.v * self.prestress_dt # only incremental displacement needed, since MULF update actually yields a zero displacement after the step
-                w_membrane_prestr, _, _, _, _ = self.bc.membranesurf_bcs(self.bc_dict['membrane'], self.ufluid_prestr, self.v, self.acc, self.io.bmeasures, ivar=self.internalvars, wallfields=self.wallfields)
-            self.deltaW_prestr_ext = w_neumann_prestr + w_robin + w_stabneumann + w_membrane_prestr + w_robin_valve
+                w_membrane_prestr, _, _, _, _ = self.bc.membranesurf_bcs(self.bc_dict['membrane'], self.ufluid_prestr, self.v, self.acc_prestr, self.io.bmeasures, ivar=self.internalvars, wallfields=self.wallfields)
+            self.deltaW_prestr_ext = w_neumann_prestr + w_robin + w_stabneumann + w_stabneumann_mod + w_membrane_prestr + w_robin_valve
         else:
             assert('neumann_prestress' not in self.bc_dict.keys())
 
-        self.deltaW_ext     = w_neumann + w_body + w_robin + w_stabneumann + w_membrane + w_robin_valve
-        self.deltaW_ext_old = w_neumann_old + w_body_old + w_robin_old + w_stabneumann_old + w_membrane_old + w_robin_valve_old
-        self.deltaW_ext_mid = w_neumann_mid + w_body_mid + w_robin_mid + w_stabneumann_mid + w_membrane_mid + w_robin_valve_mid
+        self.deltaW_ext     = w_neumann + w_body + w_robin + w_stabneumann + w_stabneumann_mod + w_membrane + w_robin_valve
+        self.deltaW_ext_old = w_neumann_old + w_body_old + w_robin_old + w_stabneumann_old + w_stabneumann_mod_old + w_membrane_old + w_robin_valve_old
+        self.deltaW_ext_mid = w_neumann_mid + w_body_mid + w_robin_mid + w_stabneumann_mid + w_stabneumann_mod_mid + w_membrane_mid + w_robin_valve_mid
 
         # stabilization
         if self.stabilization is not None:
 
             # should only be used for equal-order approximations
             assert(self.order_vel==self.order_pres)
 
             vscale = self.stabilization['vscale']
+            try: vscale_vel_dep = self.stabilization['vscale_vel_dep']
+            except: vscale_vel_dep = False
+
+            # TODO: Is this a good choice in general if we wanna make it state dependent?
+            if vscale_vel_dep:
+                vscale_max = ufl.max_value(ufl.sqrt(ufl.dot(self.v_old,self.v_old)), vscale)
+            else:
+                vscale_max = vscale
 
             h = self.io.hd0 # cell diameter (could also use max edge length self.io.emax0, but seems to yield similar/same results)
 
             try: symm = self.stabilization['symmetric']
             except: symm = False
 
+            # reduced stabiliztion scheme optimized for first-order: missing transient NS term as well as divergence stress term of strong residual
+            try: red_scheme = self.stabilization['reduced_scheme']
+            except: red_scheme = False
+
+            try: dscales = self.stabilization['dscales']
+            except: dscales = [1., 1., 1.]
+
+            if red_scheme:
+                assert(self.order_vel==1)
+                assert(self.order_pres==1)
+
             # full scheme
             if self.stabilization['scheme']=='supg_pspg':
 
                 for n, M in enumerate(self.domain_ids):
 
                     if self.num_dupl==1: j=0
                     else: j=n
 
-                    tau_supg = h / vscale
-                    tau_pspg = h / vscale
-                    tau_lsic = h * vscale
+                    dscales = self.stabilization['dscales']
+
+                    tau_supg = dscales[0] * h / vscale_max
+                    tau_pspg = dscales[1] * h / vscale_max
+                    tau_lsic = dscales[2] * h * vscale_max
 
                     # strong momentum residuals
                     if self.fluid_governing_type=='navierstokes_transient':
-                        residual_v_strong     = self.vf.res_v_strong_navierstokes_transient(self.acc, self.v, self.rho[n], self.ma[n].sigma(self.v, self.p_[j], F=self.alevar['Fale']), w=self.alevar['w'], F=self.alevar['Fale'])
-                        residual_v_strong_old = self.vf.res_v_strong_navierstokes_transient(self.a_old, self.v_old, self.rho[n], self.ma[n].sigma(self.v_old, self.p_old_[j], F=self.alevar['Fale_old']), w=self.alevar['w_old'], F=self.alevar['Fale_old'])
-                        residual_v_strong_mid = self.vf.res_v_strong_navierstokes_transient(self.acc_mid, self.vel_mid, self.rho[n], self.ma[n].sigma(self.vel_mid, self.pf_mid_[j], F=self.alevar['Fale_mid']), w=self.alevar['w_mid'], F=self.alevar['Fale_mid'])
+                        if not red_scheme:
+                            residual_v_strong     = self.vf.res_v_strong_navierstokes_transient(self.acc, self.v, self.rho[n], self.ma[n].sigma(self.v, self.p_[j], F=self.alevar['Fale']), w=self.alevar['w'], F=self.alevar['Fale'])
+                            residual_v_strong_old = self.vf.res_v_strong_navierstokes_transient(self.a_old, self.v_old, self.rho[n], self.ma[n].sigma(self.v_old, self.p_old_[j], F=self.alevar['Fale_old']), w=self.alevar['w_old'], F=self.alevar['Fale_old'])
+                            residual_v_strong_mid = self.vf.res_v_strong_navierstokes_transient(self.acc_mid, self.vel_mid, self.rho[n], self.ma[n].sigma(self.vel_mid, self.pf_mid_[j], F=self.alevar['Fale_mid']), w=self.alevar['w_mid'], F=self.alevar['Fale_mid'])
+                        else: # no viscous stress term and no dv/dt term
+                            residual_v_strong     = self.vf.f_inert_strong_navierstokes_steady(self.v, self.rho[n], w=self.alevar['w'], F=self.alevar['Fale']) + self.vf.f_gradp_strong(self.p_[j], F=self.alevar['Fale'])
+                            residual_v_strong_old = self.vf.f_inert_strong_navierstokes_steady(self.v_old, self.rho[n], w=self.alevar['w_old'], F=self.alevar['Fale_old']) + self.vf.f_gradp_strong(self.p_old_[j], F=self.alevar['Fale_old'])
+                            residual_v_strong_mid = self.vf.f_inert_strong_navierstokes_steady(self.vel_mid, self.rho[n], w=self.alevar['w_mid'], F=self.alevar['Fale_mid']) + self.vf.f_gradp_strong(self.pf_mid_[j], F=self.alevar['Fale_mid'])
                     elif self.fluid_governing_type=='navierstokes_steady':
-                        residual_v_strong     = self.vf.res_v_strong_navierstokes_steady(self.v, self.rho[n], self.ma[n].sigma(self.v, self.p_[j], F=self.alevar['Fale']), w=self.alevar['w'], F=self.alevar['Fale'])
-                        residual_v_strong_old = self.vf.res_v_strong_navierstokes_steady(self.v_old, self.rho[n], self.ma[n].sigma(self.v_old, self.p_old_[j], F=self.alevar['Fale_old']), w=self.alevar['w_old'], F=self.alevar['Fale_old'])
-                        residual_v_strong_mid = self.vf.res_v_strong_navierstokes_steady(self.vel_mid, self.rho[n], self.ma[n].sigma(self.vel_mid, self.pf_mid_[j], F=self.alevar['Fale_mid']), w=self.alevar['w_mid'], F=self.alevar['Fale_mid'])
+                        if not red_scheme:
+                            residual_v_strong     = self.vf.res_v_strong_navierstokes_steady(self.v, self.rho[n], self.ma[n].sigma(self.v, self.p_[j], F=self.alevar['Fale']), w=self.alevar['w'], F=self.alevar['Fale'])
+                            residual_v_strong_old = self.vf.res_v_strong_navierstokes_steady(self.v_old, self.rho[n], self.ma[n].sigma(self.v_old, self.p_old_[j], F=self.alevar['Fale_old']), w=self.alevar['w_old'], F=self.alevar['Fale_old'])
+                            residual_v_strong_mid = self.vf.res_v_strong_navierstokes_steady(self.vel_mid, self.rho[n], self.ma[n].sigma(self.vel_mid, self.pf_mid_[j], F=self.alevar['Fale_mid']), w=self.alevar['w_mid'], F=self.alevar['Fale_mid'])
+                        else: # no viscous stress term
+                            residual_v_strong     = self.vf.f_inert_strong_navierstokes_steady(self.v, self.rho[n], w=self.alevar['w'], F=self.alevar['Fale']) + self.vf.f_gradp_strong(self.p_[j], F=self.alevar['Fale'])
+                            residual_v_strong_old = self.vf.f_inert_strong_navierstokes_steady(self.v_old, self.rho[n], w=self.alevar['w_old'], F=self.alevar['Fale_old']) + self.vf.f_gradp_strong(self.p_old_[j], F=self.alevar['Fale_old'])
+                            residual_v_strong_mid = self.vf.f_inert_strong_navierstokes_steady(self.vel_mid, self.rho[n], w=self.alevar['w_mid'], F=self.alevar['Fale_mid']) + self.vf.f_gradp_strong(self.pf_mid_[j], F=self.alevar['Fale_mid'])
                     elif self.fluid_governing_type=='stokes_transient':
-                        residual_v_strong     = self.vf.res_v_strong_stokes_transient(self.acc, self.v, self.rho[n], self.ma[n].sigma(self.v, self.p_[j], F=self.alevar['Fale']), w=self.alevar['w'], F=self.alevar['Fale'])
-                        residual_v_strong_old = self.vf.res_v_strong_stokes_transient(self.a_old, self.v_old, self.rho[n], self.ma[n].sigma(self.v_old, self.p_old_[j], F=self.alevar['Fale_old']), w=self.alevar['w_old'], F=self.alevar['Fale_old'])
-                        residual_v_strong_mid = self.vf.res_v_strong_stokes_transient(self.acc_mid, self.vel_mid, self.rho[n], self.ma[n].sigma(self.vel_mid, self.pf_mid_[j], F=self.alevar['Fale_mid']), w=self.alevar['w_mid'], F=self.alevar['Fale_mid'])
+                        if not red_scheme:
+                            residual_v_strong     = self.vf.res_v_strong_stokes_transient(self.acc, self.v, self.rho[n], self.ma[n].sigma(self.v, self.p_[j], F=self.alevar['Fale']), w=self.alevar['w'], F=self.alevar['Fale'])
+                            residual_v_strong_old = self.vf.res_v_strong_stokes_transient(self.a_old, self.v_old, self.rho[n], self.ma[n].sigma(self.v_old, self.p_old_[j], F=self.alevar['Fale_old']), w=self.alevar['w_old'], F=self.alevar['Fale_old'])
+                            residual_v_strong_mid = self.vf.res_v_strong_stokes_transient(self.acc_mid, self.vel_mid, self.rho[n], self.ma[n].sigma(self.vel_mid, self.pf_mid_[j], F=self.alevar['Fale_mid']), w=self.alevar['w_mid'], F=self.alevar['Fale_mid'])
+                        else: # no viscous stress term
+                            residual_v_strong     = self.vf.f_inert_strong_stokes_transient(self.acc, self.v, self.rho[n], w=self.alevar['w'], F=self.alevar['Fale']) + self.vf.f_gradp_strong(self.p_[j], F=self.alevar['Fale'])
+                            residual_v_strong_old = self.vf.f_inert_strong_stokes_transient(self.a_old, self.v_old, self.rho[n], w=self.alevar['w_old'], F=self.alevar['Fale_old']) + self.vf.f_gradp_strong(self.p_old_[j], F=self.alevar['Fale_old'])
+                            residual_v_strong_mid = self.vf.f_inert_strong_stokes_transient(self.acc_mid, self.vel_mid, self.rho[n], w=self.alevar['w_mid'], F=self.alevar['Fale_mid']) + self.vf.f_gradp_strong(self.pf_mid_[j], F=self.alevar['Fale_mid'])
                     elif self.fluid_governing_type=='stokes_steady':
-                        residual_v_strong     = self.vf.res_v_strong_stokes_steady(self.rho[n], self.ma[n].sigma(self.v, self.p_[j], F=self.alevar['Fale']), F=self.alevar['Fale'])
-                        residual_v_strong_old = self.vf.res_v_strong_stokes_steady(self.rho[n], self.ma[n].sigma(self.v_old, self.p_old_[j], F=self.alevar['Fale_old']), F=self.alevar['Fale_old'])
-                        residual_v_strong_mid = self.vf.res_v_strong_stokes_steady(self.rho[n], self.ma[n].sigma(self.vel_mid, self.pf_mid_[j], F=self.alevar['Fale_mid']), F=self.alevar['Fale_mid'])
+                        if not red_scheme:
+                            residual_v_strong     = self.vf.res_v_strong_stokes_steady(self.rho[n], self.ma[n].sigma(self.v, self.p_[j], F=self.alevar['Fale']), F=self.alevar['Fale'])
+                            residual_v_strong_old = self.vf.res_v_strong_stokes_steady(self.rho[n], self.ma[n].sigma(self.v_old, self.p_old_[j], F=self.alevar['Fale_old']), F=self.alevar['Fale_old'])
+                            residual_v_strong_mid = self.vf.res_v_strong_stokes_steady(self.rho[n], self.ma[n].sigma(self.vel_mid, self.pf_mid_[j], F=self.alevar['Fale_mid']), F=self.alevar['Fale_mid'])
+                        else: # no viscous stress term
+                            residual_v_strong     = self.vf.f_gradp_strong(self.p_[j], F=self.alevar['Fale'])
+                            residual_v_strong_old = self.vf.f_gradp_strong(self.p_old_[j], F=self.alevar['Fale_old'])
+                            residual_v_strong_mid = self.vf.f_gradp_strong(self.pf_mid_[j], F=self.alevar['Fale_mid'])
                     else:
                         raise ValueError("Unknown fluid_governing_type!")
 
                     # SUPG (streamline-upwind Petrov-Galerkin) for Navier-Stokes
                     if self.fluid_governing_type=='navierstokes_transient' or self.fluid_governing_type=='navierstokes_steady':
-                        self.deltaW_int     += self.vf.stab_supg(self.acc, self.v, self.p_[j], residual_v_strong, tau_supg, self.rho[n], self.io.dx(M), w=self.alevar['w'], F=self.alevar['Fale'], symmetric=symm)
-                        self.deltaW_int_old += self.vf.stab_supg(self.a_old, self.v_old, self.p_old_[j], residual_v_strong_old, tau_supg, self.rho[n], self.io.dx(M), w=self.alevar['w_old'], F=self.alevar['Fale_old'], symmetric=symm)
-                        self.deltaW_int_mid += self.vf.stab_supg(self.acc_mid, self.vel_mid, self.pf_mid_[j], residual_v_strong_mid, tau_supg, self.rho[n], self.io.dx(M), w=self.alevar['w_mid'], F=self.alevar['Fale_mid'], symmetric=symm)
+                        self.deltaW_int     += self.vf.stab_supg(self.v, residual_v_strong, tau_supg, self.rho[n], self.io.dx(M), w=self.alevar['w'], F=self.alevar['Fale'], symmetric=symm)
+                        self.deltaW_int_old += self.vf.stab_supg(self.v_old, residual_v_strong_old, tau_supg, self.rho[n], self.io.dx(M), w=self.alevar['w_old'], F=self.alevar['Fale_old'], symmetric=symm)
+                        self.deltaW_int_mid += self.vf.stab_supg(self.vel_mid, residual_v_strong_mid, tau_supg, self.rho[n], self.io.dx(M), w=self.alevar['w_mid'], F=self.alevar['Fale_mid'], symmetric=symm)
                     # PSPG (pressure-stabilizing Petrov-Galerkin) for Navier-Stokes and Stokes
-                    self.deltaW_p[n]     += self.vf.stab_pspg(self.acc, self.v, self.p_[j], self.var_p_[j], residual_v_strong, tau_pspg, self.rho[n], self.io.dx(M), F=self.alevar['Fale'])
-                    self.deltaW_p_old[n] += self.vf.stab_pspg(self.a_old, self.v_old, self.p_old_[j], self.var_p_[j], residual_v_strong_old, tau_pspg, self.rho[n], self.io.dx(M), F=self.alevar['Fale_old'])
-                    self.deltaW_p_mid[n] += self.vf.stab_pspg(self.acc_mid, self.vel_mid, self.pf_mid_[j], self.var_p_[j], residual_v_strong_mid, tau_pspg, self.rho[n], self.io.dx(M), F=self.alevar['Fale_mid'])
+                    self.deltaW_p[n]     += self.vf.stab_pspg(self.var_p_[j], residual_v_strong, tau_pspg, self.rho[n], self.io.dx(M), F=self.alevar['Fale'])
+                    self.deltaW_p_old[n] += self.vf.stab_pspg(self.var_p_[j], residual_v_strong_old, tau_pspg, self.rho[n], self.io.dx(M), F=self.alevar['Fale_old'])
+                    self.deltaW_p_mid[n] += self.vf.stab_pspg(self.var_p_[j], residual_v_strong_mid, tau_pspg, self.rho[n], self.io.dx(M), F=self.alevar['Fale_mid'])
                     # LSIC (least-squares on incompressibility constraint) for Navier-Stokes and Stokes
                     self.deltaW_int     += self.vf.stab_lsic(self.v, tau_lsic, self.rho[n], self.io.dx(M), F=self.alevar['Fale'])
                     self.deltaW_int_old += self.vf.stab_lsic(self.v_old, tau_lsic, self.rho[n], self.io.dx(M), F=self.alevar['Fale_old'])
                     self.deltaW_int_mid += self.vf.stab_lsic(self.vel_mid, tau_lsic, self.rho[n], self.io.dx(M), F=self.alevar['Fale_mid'])
 
-            # reduced scheme: missing transient NS term as well as divergence stress term of strong residual
-            if self.stabilization['scheme']=='supg_pspg2':
+                    # now take care of stabilization for the prestress problem (only FrSI)
+                    if self.prestress_initial or self.prestress_initial_only:
+                        # LSIC term
+                        self.deltaW_prestr_int += self.vf.stab_lsic(self.v, tau_lsic, self.rho[n], self.io.dx(M), F=self.alevar['Fale'])
+                        # get the respective strong residual depending on the prestress kinetic type...
+                        if self.prestress_kinetic=='navierstokes_transient':
+                            if not red_scheme:
+                                residual_v_strong_prestr = self.vf.res_v_strong_navierstokes_transient(self.acc_prestr, self.v, self.rho[n], self.ma[n].sigma(self.v, self.p_[j], F=self.alevar['Fale']), w=self.alevar['w'], F=self.alevar['Fale'])
+                            else: # no viscous stress term and no dv/dt term
+                                residual_v_strong_prestr = self.vf.f_inert_strong_navierstokes_steady(self.v, self.rho[n], w=self.alevar['w'], F=self.alevar['Fale']) + self.vf.f_gradp_strong(self.p_[j], F=self.alevar['Fale'])
+                        elif self.prestress_kinetic=='navierstokes_steady':
+                            if not red_scheme:
+                                residual_v_strong_prestr = self.vf.res_v_strong_navierstokes_steady(self.v, self.rho[n], self.ma[n].sigma(self.v, self.p_[j], F=self.alevar['Fale']), w=self.alevar['w'], F=self.alevar['Fale'])
+                            else: # no viscous stress term
+                                residual_v_strong_prestr = self.vf.f_inert_strong_navierstokes_steady(self.v, self.rho[n], w=self.alevar['w'], F=self.alevar['Fale']) + self.vf.f_gradp_strong(self.p_[j], F=self.alevar['Fale'])
+                        elif self.prestress_kinetic=='stokes_transient':
+                            if not red_scheme:
+                                residual_v_strong_prestr = self.vf.res_v_strong_stokes_transient(self.acc_prestr, self.v, self.rho[n], self.ma[n].sigma(self.v, self.p_[j], F=self.alevar['Fale']), w=self.alevar['w'], F=self.alevar['Fale'])
+                            else: # no viscous stress term
+                                residual_v_strong_prestr = self.vf.f_inert_strong_stokes_transient(self.acc_prestr, self.v, self.rho[n], w=self.alevar['w'], F=self.alevar['Fale']) + self.vf.f_gradp_strong(self.p_[j], F=self.alevar['Fale'])
+                        elif self.prestress_kinetic=='none':
+                            if not red_scheme:
+                                residual_v_strong_prestr = self.vf.res_v_strong_stokes_steady(self.rho[n], self.ma[n].sigma(self.v, self.p_[j], F=self.alevar['Fale']), F=self.alevar['Fale'])
+                            else: # no viscous stress term
+                                residual_v_strong_prestr = self.vf.f_gradp_strong(self.p_[j], F=self.alevar['Fale'])
+                        else:
+                            raise ValueError("Unknown prestress_kinetic option!")
+                        # PSPG term
+                        self.deltaW_p_prestr[n] += self.vf.stab_pspg(self.var_p_[j], residual_v_strong_prestr, tau_pspg, self.rho[n], self.io.dx(M), F=self.alevar['Fale'])
+                        # SUPG term only for kinetic prestress...
+                        if self.prestress_kinetic=='navierstokes_transient' or self.prestress_kinetic=='navierstokes_steady':
+                            self.deltaW_prestr_int += self.vf.stab_supg(self.v, residual_v_strong_prestr, tau_supg, self.rho[n], self.io.dx(M), w=self.alevar['w'], F=self.alevar['Fale'], symmetric=symm)
 
-                # optimized for first-order
-                assert(self.order_vel==1)
-                assert(self.order_pres==1)
-
-                for n, M in enumerate(self.domain_ids):
-
-                    if self.num_dupl==1: j=0
-                    else: j=n
-
-                    dscales = self.stabilization['dscales']
+            else:
+                raise ValueError("Unknown stabilization scheme!")
 
-                    # yields same result as above for navierstokes_steady
-                    delta1 = dscales[0] * self.rho[n] * h / vscale
-                    delta2 = dscales[1] * self.rho[n] * h * vscale
-                    delta3 = dscales[2] * h / vscale
-
-                    self.deltaW_int     += self.vf.stab_v(delta1, delta2, delta3, self.v, self.p_[j], self.io.dx(M), w=self.alevar['w'], F=self.alevar['Fale'], symmetric=symm)
-                    self.deltaW_int_old += self.vf.stab_v(delta1, delta2, delta3, self.v_old, self.p_old_[j], self.io.dx(M), w=self.alevar['w_old'], F=self.alevar['Fale_old'], symmetric=symm)
-                    self.deltaW_int_mid += self.vf.stab_v(delta1, delta2, delta3, self.vel_mid, self.pf_mid_[j], self.io.dx(M), w=self.alevar['w_mid'], F=self.alevar['Fale_mid'], symmetric=symm)
-
-                    self.deltaW_p[n]     += self.vf.stab_p(delta1, delta3, self.v, self.p_[j], self.var_p_[j], self.rho[n], self.io.dx(M), w=self.alevar['w'], F=self.alevar['Fale'])
-                    self.deltaW_p_old[n] += self.vf.stab_p(delta1, delta3, self.v_old, self.p_old_[j], self.var_p_[j], self.rho[n], self.io.dx(M), w=self.alevar['w_old'], F=self.alevar['Fale_old'])
-                    self.deltaW_p_mid[n] += self.vf.stab_p(delta1, delta3, self.vel_mid, self.pf_mid_[j], self.var_p_[j], self.rho[n], self.io.dx(M), w=self.alevar['w_mid'], F=self.alevar['Fale_mid'])
 
         ### full weakforms
 
         # kinetic plus internal minus external virtual power
         # evaluate nonlinear terms trapezoidal-like: a * f(u_{n+1}) + (1-a) * f(u_{n})
         if self.ti.eval_nonlin_terms=='trapezoidal':
 
@@ -675,21 +761,18 @@
                     na+=1
                 else:
                     self.tau_a_.append(ufl.as_ufl(0))
 
         if self.prestress_initial or self.prestress_initial_only:
             # prestressing weak forms
             self.weakform_prestress_p, self.weakform_lin_prestress_vp, self.weakform_lin_prestress_pv, self.weakform_lin_prestress_pp = [], [], [], []
-            if self.prestress_kinetic:
-                self.weakform_prestress_v = self.deltaW_prestr_kin + self.deltaW_int - self.deltaW_prestr_ext
-            else:
-                self.weakform_prestress_v = self.deltaW_int - self.deltaW_prestr_ext
+            self.weakform_prestress_v = self.deltaW_prestr_kin + self.deltaW_prestr_int - self.deltaW_prestr_ext
             self.weakform_lin_prestress_vv = ufl.derivative(self.weakform_prestress_v, self.v, self.dv)
             for n in range(self.num_domains):
-                self.weakform_prestress_p.append( self.deltaW_p[n] )
+                self.weakform_prestress_p.append( self.deltaW_p_prestr[n] )
             for j in range(self.num_dupl):
                 self.weakform_lin_prestress_vp.append( ufl.derivative(self.weakform_prestress_v, self.p_[j], self.dp_[j]) )
             for n in range(self.num_domains):
                 self.weakform_lin_prestress_pv.append( ufl.derivative(self.weakform_prestress_p[n], self.v, self.dv) )
             if self.stabilization is not None:
                 for n in range(self.num_domains):
                     if self.num_dupl==1: j=0
@@ -904,17 +987,14 @@
         else:
             fem.petsc.assemble_vector(self.r_p, self.res_p)
             self.r_p.ghostUpdate(addv=PETSc.InsertMode.ADD, mode=PETSc.ScatterMode.REVERSE)
 
         self.r_list[0] = self.r_v
         self.r_list[1] = self.r_p
 
-        if bool(self.pbase.residual_scale):
-            self.scale_residual_list(self.r_list, self.pbase.residual_scale)
-
 
     def assemble_stiffness(self, t, subsolver=None):
 
         # assemble system matrix
         self.K_vv.zeroEntries()
         fem.petsc.assemble_matrix(self.K_vv, self.jac_vv, self.bc.dbcs)
         self.K_vv.assemble()
@@ -945,17 +1025,14 @@
             self.K_pp = None
 
         self.K_list[0][0] = self.K_vv
         self.K_list[0][1] = self.K_vp
         self.K_list[1][0] = self.K_pv
         self.K_list[1][1] = self.K_pp
 
-        if bool(self.pbase.residual_scale):
-            self.scale_jacobian_list(self.K_list, self.pbase.residual_scale)
-
 
     def get_index_sets(self, isoptions={}):
 
         if self.rom is not None: # currently, ROM can only be on (subset of) first variable
             vvec_or0 = self.rom.V.getOwnershipRangeColumn()[0]
             vvec_ls = self.rom.V.getLocalSize()[1]
         else:
@@ -1239,16 +1316,16 @@
 
             self.solnln.newton(tprestr)
 
             # update uf_pre
             self.pb.ki.prestress_update(self.pb.prestress_dt, self.pb.v.vector)
             utilities.print_prestress('updt', self.pb.comm)
 
-            # update fluid velocity: v_old <- v - if we want some slight inertia...
-            if self.pb.prestress_kinetic:
+            # update fluid velocity: v_old <- v
+            if self.pb.prestress_kinetic!='none':
                 self.pb.v_old.vector.axpby(1.0, 0.0, self.pb.v.vector)
                 self.pb.v_old.vector.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
 
             wt = time.time() - wts
 
             # print time step info to screen
             self.pb.ti.print_prestress_step(N, tprestr, self.pb.prestress_numstep, self.solnln.lsp, ni=self.solnln.ni, li=self.solnln.li, wt=wt)
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/fluid/fluid_material.py` & `ambit_fe-1.2.6/src/ambit_fe/fluid/fluid_material.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/fluid/fluid_variationalform.py` & `ambit_fe-1.2.6/src/ambit_fe/fluid/fluid_variationalform.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,88 +57,107 @@
 
     # TeX: \int\limits_{\Omega}\boldsymbol{\nabla}\cdot\boldsymbol{v}\,\delta p\,\mathrm{d}v
     def deltaW_int_pres(self, v, var_p, ddomain, w=None, F=None):
 
         return ufl.div(v)*var_p*ddomain
 
     def res_v_strong_navierstokes_transient(self, a, v, rho, sig, w=None, F=None):
+
+        return self.f_inert_strong_navierstokes_transient(a, v, rho, w=w, F=F) - self.f_stress_strong(sig, F=F)
+
+    def res_v_strong_navierstokes_steady(self, v, rho, sig, w=None, F=None):
+
+        return self.f_inert_strong_navierstokes_steady(v, rho, w=w, F=F) - self.f_stress_strong(sig, F=F)
+
+    def res_v_strong_stokes_transient(self, a, v, rho, sig, w=None, F=None):
+
+        return self.f_inert_strong_stokes_transient(a, rho) - self.f_stress_strong(sig, F=F)
+
+    def res_v_strong_stokes_steady(self, rho, sig, F=None):
+
+        return -self.f_stress_strong(sig, F=F)
+
+    def f_inert_strong_navierstokes_transient(self, a, v, rho, w=None, F=None):
         if self.formulation=='nonconservative':
-            return rho*(a + ufl.grad(v) * v) - ufl.div(sig)
+            return rho*(a + ufl.grad(v) * v)
         elif self.formulation=='conservative':
-            return rho*(a + ufl.div(ufl.outer(v,v))) - ufl.div(sig)
+            return rho*(a + ufl.div(ufl.outer(v,v)))
         else:
             raise ValueError("Unknown fluid formulation!")
 
-    def res_v_strong_navierstokes_steady(self, v, rho, sig, w=None, F=None):
+    def f_inert_strong_navierstokes_steady(self, v, rho, w=None, F=None):
         if self.formulation=='nonconservative':
-            return rho*(ufl.grad(v) * v) - ufl.div(sig)
+            return rho*(ufl.grad(v) * v)
         elif self.formulation=='conservative':
-            return rho*(ufl.div(ufl.outer(v,v))) - ufl.div(sig)
+            return rho*(ufl.div(ufl.outer(v,v)))
         else:
             raise ValueError("Unknown fluid formulation!")
 
-    def res_v_strong_stokes_transient(self, a, v, rho, sig, w=None, F=None):
+    def f_inert_strong_stokes_transient(self, a, rho):
 
-        return rho*a - ufl.div(sig)
+        return rho*a
 
-    def res_v_strong_stokes_steady(self, rho, sig, F=None):
+    def f_stress_strong(self, sig, F=None):
+
+        return ufl.div(sig)
 
-        return -ufl.div(sig)
+    def f_gradp_strong(self, p, F=None):
+
+        return ufl.grad(p)
 
     def res_p_strong(self, v, F=None):
 
         return ufl.div(v)
 
 
     # stabilized Neumann BC - Esmaily Moghadam et al. 2011
-    def deltaW_ext_stabilized_neumann(self, v, par1, par2, dboundary, w=None, F=None):
+    def deltaW_ext_stabilized_neumann(self, v, beta, dboundary, w=None, F=None):
+
+        vn = ufl.dot(v,self.n0)
+        return beta*(ufl.min_value(vn,0.) * ufl.dot(v,self.var_v)*dboundary)
+
+    # mod. stabilized Neumann BC
+    def deltaW_ext_stabilized_neumann_mod(self, v, beta, gamma, dboundary, w=None, F=None):
 
         vn = ufl.dot(v,self.n0)
-        return par1*((vn**2.)/(vn**2. + 0.01*par2**2.) * ufl.min_value(vn,0.) * ufl.dot(v,self.var_v)*dboundary) # version from Esmaily Moghadam et al. 2011 if par2 = 0
+        return beta*((vn**2.)/(vn**2. + 0.01*gamma**2.) * ufl.min_value(vn,0.) * ufl.dot(v,self.var_v)*dboundary) # version from Esmaily Moghadam et al. 2011 if gamma = 0
 
 
     # Robin condition for valve, over internal surface
     def deltaW_ext_robin_valve(self, v, beta, dboundary, fcts='+', w=None, F=None):
 
         return (-(beta*ufl.dot((v-w), self.var_v)))(fcts)*dboundary
 
 
     ### SUPG/PSPG stabilization - cf. Tezduyar and Osawa (2000), "Finite element stabilization parameters computed from element matrices and vectors"
-    def stab_supg(self, a, v, p, res_v_strong, tau_supg, rho, ddomain, w=None, F=None, symmetric=False):
+    def stab_supg(self, v, res_v_strong, tau_supg, rho, ddomain, w=None, F=None, symmetric=False):
 
-        if symmetric: # modification to make the effective stress symmetric
+        if symmetric: # modification to make the effective stress symmetric - experimental, use with care...
             return (1./rho) * ufl.dot(tau_supg*rho*ufl.sym(ufl.grad(self.var_v))*v, res_v_strong) * ddomain
         else:
             return (1./rho) * ufl.dot(tau_supg*rho*ufl.grad(self.var_v)*v, res_v_strong) * ddomain
 
-    def stab_pspg(self, a, v, p, var_p, res_v_strong, tau_pspg, rho, ddomain, F=None):
+    def stab_pspg(self, var_p, res_v_strong, tau_pspg, rho, ddomain, F=None):
 
         return (1./rho) * ufl.dot(tau_pspg*ufl.grad(var_p), res_v_strong) * ddomain
 
     def stab_lsic(self, v, tau_lsic, rho, ddomain, F=None):
 
         return tau_lsic*ufl.div(self.var_v)*rho*self.res_p_strong(v, F=F) * ddomain
 
 
-    # reduced stabilization scheme - cf. Hoffman and Johnson (2006), "A new approach to computational turbulence modeling"
-    def stab_v(self, delta1, delta2, delta3, v, p, ddomain, w=None, F=None, symmetric=False):
+    # components of element-level Reynolds number - cf. Tezduyar and Osawa (2000)
+    def re_c(self, rho, v, ddomain, w=None, F=None):
+
+        return rho * ufl.dot(ufl.grad(v)*v, self.var_v) * ddomain
 
-        if symmetric: # modification to make the effective stress symmetric
-            return ( delta1 * ufl.dot(ufl.grad(v)*v, ufl.sym(ufl.grad(self.var_v))*v) + \
-                     delta2 * ufl.div(v)*ufl.div(self.var_v) + \
-                     delta3 * ufl.dot(ufl.grad(p), ufl.sym(ufl.grad(self.var_v))*v) ) * ddomain
-        else:
-            return ( delta1 * ufl.dot(ufl.grad(v)*v, ufl.grad(self.var_v)*v) + \
-                     delta2 * ufl.div(v)*ufl.div(self.var_v) + \
-                     delta3 * ufl.dot(ufl.grad(p), ufl.grad(self.var_v)*v) ) * ddomain
+    def re_ktilde(self, rho, v, ddomain, w=None, F=None):
 
-    def stab_p(self, delta1, delta3, v, p, var_p, rho, ddomain, w=None, F=None):
+        return rho * ufl.dot(ufl.grad(v)*v, ufl.grad(self.var_v)*v) * ddomain
 
-        return (1./rho) * ( delta1 * ufl.dot(ufl.grad(v)*v, ufl.grad(var_p)) + \
-                            delta3 * ufl.dot(ufl.grad(p), ufl.grad(var_p)) ) * ddomain
 
     ### Flux coupling conditions
 
     # flux
     # TeX: \int\limits_{\Gamma} \boldsymbol{n}\cdot\boldsymbol{v}\,\mathrm{d}a
     def flux(self, v, dboundary, w=None, F=None, fcts=None):
         if fcts is None:
@@ -238,93 +257,113 @@
         J = ufl.det(F)
         if fcts is None:
             return beta*ufl.dot((v-vD), self.var_v) * J*ufl.sqrt(ufl.dot(self.n0, (ufl.inv(F)*ufl.inv(F).T)*self.n0))*dboundary
         else:
             return (beta*ufl.dot((v-vD), self.var_v) * J*ufl.sqrt(ufl.dot(self.n0, (ufl.inv(F)*ufl.inv(F).T)*self.n0)))(fcts)*dboundary
 
     def res_v_strong_navierstokes_transient(self, a, v, rho, sig, w=None, F=None):
-        i, j, k = ufl.indices(3)
+
+        return self.f_inert_strong_navierstokes_transient(a, v, rho, w=w, F=F) - self.f_stress_strong(sig, F=F)
+
+    def res_v_strong_navierstokes_steady(self, v, rho, sig, w=None, F=None):
+
+        return self.f_inert_strong_navierstokes_steady(v, rho, w=w, F=F) - self.f_stress_strong(sig, F=F)
+
+    def res_v_strong_stokes_transient(self, a, v, rho, sig, w=None, F=None):
+
+        return self.f_inert_strong_stokes_transient(a, v, rho, w=w, F=F) - self.f_stress_strong(sig, F=F)
+
+    def res_v_strong_stokes_steady(self, rho, sig, F=None):
+
+        return -self.f_stress_strong(sig, F=F)
+
+    def f_inert_strong_navierstokes_transient(self, a, v, rho, w=None, F=None):
         if self.formulation=='nonconservative':
-            return rho*(a + ufl.grad(v)*ufl.inv(F) * (v-w)) - ufl.as_vector(ufl.grad(sig)[i,j,k]*ufl.inv(F).T[j,k], i)
+            return rho*(a + ufl.grad(v)*ufl.inv(F) * (v-w))
         elif self.formulation=='conservative':
-            return rho*(a + ufl.as_vector(ufl.grad(ufl.outer(v,v-w))[i,j,k]*ufl.inv(F).T[j,k], i)) - ufl.as_vector(ufl.grad(sig)[l,m,n]*ufl.inv(F).T[j,k], i)
+            i, j, k = ufl.indices(3)
+            return rho*(a + ufl.as_vector(ufl.grad(ufl.outer(v,v-w))[i,j,k]*ufl.inv(F).T[j,k], i))
         else:
             raise ValueError("Unknown fluid formulation!")
 
-    def res_v_strong_navierstokes_steady(self, v, rho, sig, w=None, F=None):
-        i, j, k = ufl.indices(3)
+    def f_inert_strong_navierstokes_steady(self, v, rho, w=None, F=None):
         if self.formulation=='nonconservative':
-            return rho*(ufl.grad(v)*ufl.inv(F) * (v-w)) - ufl.as_vector(ufl.grad(sig)[i,j,k]*ufl.inv(F).T[j,k], i)
+            return rho*(ufl.grad(v)*ufl.inv(F) * (v-w))
         elif self.formulation=='conservative':
-            return rho*(ufl.as_vector(ufl.grad(ufl.outer(v,v-w))[i,j,k]*ufl.inv(F).T[j,k], i)) - ufl.as_vector(ufl.grad(sig)[l,m,n]*ufl.inv(F).T[j,k], i)
+            i, j, k = ufl.indices(3)
+            return rho*(ufl.as_vector(ufl.grad(ufl.outer(v,v-w))[i,j,k]*ufl.inv(F).T[j,k], i))
         else:
             raise ValueError("Unknown fluid formulation!")
 
-    def res_v_strong_stokes_transient(self, a, v, rho, sig, w=None, F=None):
-        i, j, k = ufl.indices(3)
+    def f_inert_strong_stokes_transient(self, a, v, rho, w=None, F=None):
         if self.formulation=='nonconservative':
-            return rho*(a + ufl.grad(v)*ufl.inv(F) * (-w)) - ufl.as_vector(ufl.grad(sig)[i,j,k]*ufl.inv(F).T[j,k], i)
+            return rho*(a + ufl.grad(v)*ufl.inv(F) * (-w))
         elif self.formulation=='conservative':
-            return rho*(a + ufl.as_vector(ufl.grad(ufl.outer(v,-w))[i,j,k]*ufl.inv(F).T[j,k], i)) - ufl.as_vector(ufl.grad(sig)[i,j,k]*ufl.inv(F).T[j,k], i)
+            i, j, k = ufl.indices(3)
+            return rho*(a + ufl.as_vector(ufl.grad(ufl.outer(v,-w))[i,j,k]*ufl.inv(F).T[j,k], i))
         else:
             raise ValueError("Unknown fluid formulation!")
 
-    def res_v_strong_stokes_steady(self, rho, sig, F=None):
+    def f_stress_strong(self, sig, F=None):
         i, j, k = ufl.indices(3)
-        return -ufl.as_vector(ufl.grad(sig)[i,j,k]*ufl.inv(F).T[j,k], i)
+        return ufl.as_vector(ufl.grad(sig)[i,j,k]*ufl.inv(F).T[j,k], i)
+
+    def f_gradp_strong(self, p, F=None):
+
+        return ufl.inv(F).T*ufl.grad(p)
 
     def res_p_strong(self, v, F=None):
 
         return ufl.inner(ufl.grad(v), ufl.inv(F).T)
 
 
     # stabilized Neumann BC - Esmaily Moghadam et al. 2011
-    def deltaW_ext_stabilized_neumann(self, v, par1, par2, dboundary, w=None, F=None):
+    def deltaW_ext_stabilized_neumann(self, v, beta, dboundary, w=None, F=None):
         J = ufl.det(F)
         vwn = ufl.dot(v-w, J*ufl.inv(F).T*self.n0)
-        return par1*((vwn**2.)/(vwn**2. + 0.01*par2**2.) * ufl.min_value(vwn,0.) * ufl.dot(v,self.var_v)*dboundary) # version from Esmaily Moghadam et al. 2011 if param2 = 0
+        return beta*(ufl.min_value(vwn,0.) * ufl.dot(v,self.var_v)*dboundary)
+
+    # mod. stabilized Neumann BC
+    def deltaW_ext_stabilized_neumann_mod(self, v, beta, gamma, dboundary, w=None, F=None):
+        J = ufl.det(F)
+        vwn = ufl.dot(v-w, J*ufl.inv(F).T*self.n0)
+        return beta*((vwn**2.)/(vwn**2. + 0.01*gamma**2.) * ufl.min_value(vwn,0.) * ufl.dot(v,self.var_v)*dboundary) # version from Esmaily Moghadam et al. 2011 if gamma = 0
 
 
     # Robin condition for valve, over internal surface
     def deltaW_ext_robin_valve(self, v, beta, dboundary, fcts='+', w=None, F=None):
         J = ufl.det(F)
         return (-(beta*ufl.dot((v-w), self.var_v) * J*ufl.sqrt(ufl.dot(self.n0, (ufl.inv(F)*ufl.inv(F).T)*self.n0))))(fcts)*dboundary
 
 
     ### SUPG/PSPG stabilization
-    def stab_supg(self, a, v, p, res_v_strong, tau_supg, rho, ddomain, w=None, F=None, symmetric=False):
+    def stab_supg(self, v, res_v_strong, tau_supg, rho, ddomain, w=None, F=None, symmetric=False):
         J = ufl.det(F)
-        if symmetric: # modification to make the effective stress symmetric
+        if symmetric: # modification to make the effective stress symmetric - experimental, use with care...
             return (1./rho) * ufl.dot(tau_supg*rho*ufl.sym(ufl.grad(self.var_v)*ufl.inv(F))*v, res_v_strong) * J*ddomain
         else:
             return (1./rho) * ufl.dot(tau_supg*rho*ufl.grad(self.var_v)*ufl.inv(F)*v, res_v_strong) * J*ddomain
 
-    def stab_pspg(self, a, v, p, var_p, res_v_strong, tau_pspg, rho, ddomain, F=None):
+    def stab_pspg(self, var_p, res_v_strong, tau_pspg, rho, ddomain, F=None):
         J = ufl.det(F)
         return (1./rho) * ufl.dot(tau_pspg*ufl.inv(F).T*ufl.grad(var_p), res_v_strong) * J*ddomain
 
     def stab_lsic(self, v, tau_lsic, rho, ddomain, F=None):
         J = ufl.det(F)
         return tau_lsic * ufl.inner(ufl.grad(self.var_v),ufl.inv(F).T) * rho*self.res_p_strong(v, F=F) * J*ddomain
 
-    def stab_v(self, delta1, delta2, delta3, v, p, ddomain, w=None, F=None, symmetric=False):
+
+    # components of element-level Reynolds number
+    def re_c(self, rho, v, ddomain, w=None, F=None):
         J = ufl.det(F)
-        if symmetric: # modification to make the effective stress symmetric
-            return ( delta1 * ufl.dot(ufl.grad(v)*ufl.inv(F)*(v-w), ufl.sym(ufl.grad(self.var_v)*ufl.inv(F))*v) + \
-                     delta2 * ufl.inner(ufl.grad(v),ufl.inv(F).T) * ufl.inner(ufl.grad(self.var_v),ufl.inv(F).T) + \
-                     delta3 * ufl.dot(ufl.inv(F).T*ufl.grad(p), ufl.sym(ufl.grad(self.var_v)*ufl.inv(F))*v) ) * J*ddomain
-        else:
-            return ( delta1 * ufl.dot(ufl.grad(v)*ufl.inv(F)*(v-w), ufl.grad(self.var_v)*ufl.inv(F)*v) + \
-                     delta2 * ufl.inner(ufl.grad(v),ufl.inv(F).T) * ufl.inner(ufl.grad(self.var_v),ufl.inv(F).T) + \
-                     delta3 * ufl.dot(ufl.inv(F).T*ufl.grad(p), ufl.grad(self.var_v)*ufl.inv(F)*v) ) * J*ddomain
+        return rho * ufl.dot(ufl.grad(v)*ufl.inv(F)*(v-w), self.var_v) * J*ddomain
 
-    def stab_p(self, delta1, delta3, v, p, var_p, rho, ddomain, w=None, F=None):
+    def re_ktilde(self, rho, v, ddomain, w=None, F=None):
         J = ufl.det(F)
-        return (1./rho) * ( delta1 * ufl.dot(ufl.grad(v)*ufl.inv(F)*(v-w), ufl.inv(F).T*ufl.grad(var_p)) + \
-                            delta3 * ufl.dot(ufl.inv(F).T*ufl.grad(p), ufl.inv(F).T*ufl.grad(var_p)) ) * J*ddomain
+        return rho * ufl.dot(ufl.grad(v)*ufl.inv(F)*(v-w), ufl.grad(self.var_v)*ufl.inv(F)*v) * J*ddomain
 
 
     ### Flux coupling conditions
 
     # flux
     # TeX: \int\limits_{\Gamma} (\boldsymbol{v}-\boldsymbol{w})\cdot\boldsymbol{n}\,\mathrm{d}a =
     #      \int\limits_{\Gamma_0} (\boldsymbol{v}-\boldsymbol{w})\cdot J\boldsymbol{F}^{-\mathrm{T}}\boldsymbol{n}_0\,\mathrm{d}A
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/ioparams.py` & `ambit_fe-1.2.6/src/ambit_fe/ioparams.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,15 +246,17 @@
                     'hdmfilenames',
                     'modes_from_files',
                     'numredbasisvec',
                     'numsnapshots',
                     'partitions',
                     'pod_only',
                     'print_eigenproblem',
-                    'redbasisvec_penalties',
+                    'regularizations',
+                    'regularizations_integ',
+                    'regularizations_deriv',
                     'snapshotincr',
                     'surface_rom',
                     'write_pod_modes']
 
     for k in params.keys():
         if k not in valid_params:
             raise RuntimeError("Unknown parameter found in ROM params: "+k)
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/ioroutines.py` & `ambit_fe-1.2.6/src/ambit_fe/ioroutines.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/mathutils.py` & `ambit_fe-1.2.6/src/ambit_fe/mathutils.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/meshutils.py` & `ambit_fe-1.2.6/src/ambit_fe/meshutils.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/mpiroutines.py` & `ambit_fe-1.2.6/src/ambit_fe/mpiroutines.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/multiscale/solid_flow0d_growthremodel_main.py` & `ambit_fe-1.2.6/src/ambit_fe/multiscale/solid_flow0d_growthremodel_main.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/oderoutines.py` & `ambit_fe-1.2.6/src/ambit_fe/oderoutines.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/postprocess/flow0d_plot.py` & `ambit_fe-1.2.6/src/ambit_fe/postprocess/flow0d_plot.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/resultcheck.py` & `ambit_fe-1.2.6/src/ambit_fe/resultcheck.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/signet/signet_hypertrophy.py` & `ambit_fe-1.2.6/src/ambit_fe/signet/signet_hypertrophy.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/signet/signet_main.py` & `ambit_fe-1.2.6/src/ambit_fe/signet/signet_main.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/solid/solid_kinematics_constitutive.py` & `ambit_fe-1.2.6/src/ambit_fe/solid/solid_kinematics_constitutive.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/solid/solid_main.py` & `ambit_fe-1.2.6/src/ambit_fe/solid/solid_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,19 @@
         else:
             self.u_pre = None
         if (self.prestress_initial or self.prestress_initial_only) and self.pbase.restart_step == 0:
             self.pre = True
         else:
             self.pre = False
 
+        # for ROM, provide pointers to main variable and its derivative
+        if self.pbase.have_rom:
+            self.xr_, self.xr_old_, self.xrpre_ = self.u, self.u_old, self.u_pre
+            self.xdtr_old_, self.xintrpre_ = self.v_old, None
+
         # own read function: requires plain txt format of type "node-id val-x val-y val-z" (or one value in case of a scalar)
         if bool(self.prestress_from_file):
             self.io.readfunction(self.u_pre, self.prestress_from_file[0])
             # if available, we might want to read in the pressure field, too
             if self.incompressible_2field:
                 if len(self.prestress_from_file)>1:
                     self.io.readfunction(self.p, self.prestress_from_file[1])
@@ -410,14 +415,15 @@
 
         if 'dirichlet_vol' in self.bc_dict.keys():
             self.bc.dirichlet_vol(self.bc_dict['dirichlet_vol'], self.V_u)
 
         self.set_variational_forms()
 
         self.pbrom = self # self-pointer needed for ROM solver access
+        self.pbrom_host = self
         self.V_rom = self.V_u
         self.print_enhanced_info = self.io.print_enhanced_info
 
 
     def get_problem_var_list(self):
 
         if self.incompressible_2field:
@@ -978,17 +984,14 @@
             self.r_list[0] = self.r_u
             self.r_list[1] = self.r_p
 
         else:
 
             self.r_list[0] = self.r_u
 
-        if bool(self.pbase.residual_scale):
-            self.scale_residual_list(self.r_list, self.pbase.residual_scale)
-
 
     def assemble_stiffness(self, t, subsolver=None):
 
         # assemble system matrix
         self.K_uu.zeroEntries()
         fem.petsc.assemble_matrix(self.K_uu, self.jac_uu, self.bc.dbcs)
         self.K_uu.assemble()
@@ -1017,17 +1020,14 @@
             self.K_list[1][0] = self.K_pu
             self.K_list[1][1] = self.K_pp
 
         else:
 
             self.K_list[0][0] = self.K_uu
 
-        if bool(self.pbase.residual_scale):
-            self.scale_jacobian_list(self.K_list, self.pbase.residual_scale)
-
 
     def get_index_sets(self, isoptions={}):
 
         assert(self.incompressible_2field) # index sets only needed for 2-field problem
 
         if self.rom is not None: # currently, ROM can only be on (subset of) first variable
             uvec_or0 = self.rom.V.getOwnershipRangeColumn()[0]
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/solid/solid_material.py` & `ambit_fe-1.2.6/src/ambit_fe/solid/solid_material.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/solid/solid_variationalform.py` & `ambit_fe-1.2.6/src/ambit_fe/solid/solid_variationalform.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/solver/preconditioner.py` & `ambit_fe-1.2.6/src/ambit_fe/solver/preconditioner.py`

 * *Files 17% similar despite different names*

```diff
@@ -48,15 +48,16 @@
 
         ts = time.time()
         utilities.print_status("Creating preconditioner objects...", self.comm, e=" ")
 
         # get reference to preconditioner matrix object
         _, self.P = pc.getOperators()
 
-        self.tpy = None
+        # reference to PETSc options
+        opts = PETSc.Options()
 
         self.check_field_size()
         operator_mats = self.init_mat_vec(pc)
 
         self.ksp_fields, self.ksp_py_solver = [], [None]*self.nfields
         # create field ksps
         for n in range(self.nfields):
@@ -80,18 +81,18 @@
                 except: amgtype = "hypre"
                 self.ksp_fields[n].getPC().setType(amgtype)
                 if amgtype=="hypre":
                     self.ksp_fields[n].getPC().setHYPREType("boomeramg")
                 # add PETSc options
                 if 'petsc_options' in self.precond_fields[n].keys():
                     opt_dict = self.precond_fields[n]['petsc_options']
-                    opts = PETSc.Options()
                     for o in opt_dict:
                         opts.setValue(o, opt_dict[o])
-                    self.ksp_fields[n].getPC().setFromOptions()
+                    self.ksp_fields[n].setFromOptions() # solver options
+                    self.ksp_fields[n].getPC().setFromOptions() # preconditioner options
                 # print to view some settings...
                 # print(self.ksp_fields[n].getPC().view())
                 if solvetype == 'python':
                     try: niter = self.precond_fields[n]['stat_iter']
                     except: niter = 1
                     if self.precond_fields[n]['py_solver'] == "stat_iter_fixed":
                         self.ksp_py_solver[n] = stat_iter_fixed(niter)
@@ -225,16 +226,14 @@
             y.axpy(1., wrk)
             yold.axpby(1., 0., y)
 
         ksp.setConvergedReason(1)
 
 
 
-
-
 # Schur complement preconditioner (using a modified diag(A)^{-1} instead of A^{-1} in the Schur complement)
 class schur_2x2(block_precond):
 
     def check_field_size(self):
         assert(self.nfields==2)
 
 
@@ -424,43 +423,39 @@
         self.Smoddinv = PETSc.Mat().createAIJ(self.C.getSizes(), bsize=None, nnz=(1,1), csr=None, comm=self.comm)
         self.Smoddinv.setUp()
         self.Smoddinv.assemble()
         # set 1's to get correct allocation pattern
         self.Smoddinv.shift(1.)
 
         self.Tmod = self.Et.copy(structure=PETSc.Mat.Structure.DIFFERENT_NONZERO_PATTERN)
+        self.Umod = self.E.copy(structure=PETSc.Mat.Structure.DIFFERENT_NONZERO_PATTERN)
         self.Wmod = self.R.copy(structure=PETSc.Mat.Structure.DIFFERENT_NONZERO_PATTERN)
 
         self.Adinv_Bt = self.Adinv.matMult(self.Bt)
-        self.DBt = self.D.matMult(self.Adinv_Bt)
+        self.D_Adinv_Bt = self.D.matMult(self.Adinv_Bt)
 
         self.B_Adinv_Bt = self.B.matMult(self.Adinv_Bt)
 
         self.Adinv_Dt = self.Adinv.matMult(self.Dt)
         self.B_Adinv_Dt = self.B.matMult(self.Adinv_Dt)
 
         self.D_Adinv_Dt = self.D.matMult(self.Adinv_Dt)
 
         # need to set Smod and Tmod here to get the data structures right
         self.Smod.axpy(-1., self.B_Adinv_Bt)
+        self.Umod.axpy(-1., self.D_Adinv_Bt)
         self.Tmod.axpy(-1., self.B_Adinv_Dt)
 
         self.Smoddinv_Tmod = self.Smoddinv.matMult(self.Tmod)
 
-        self.Bt_Smoddinv_Tmod = self.Bt.matMult(self.Smoddinv_Tmod)
-
-        self.Adinv_Bt_Smoddinv_Tmod = self.Adinv.matMult(self.Bt_Smoddinv_Tmod)
-        self.D_Adinv_Bt_Smoddinv_Tmod = self.D.matMult(self.Adinv_Bt_Smoddinv_Tmod)
-
-        self.E_Smoddinv_Tmod = self.E.matMult(self.Smoddinv_Tmod)
+        self.Umod_Smoddinv_Tmod = self.Umod.matMult(self.Smoddinv_Tmod)
 
         self.By1 = self.B.createVecLeft()
         self.Dy1 = self.D.createVecLeft()
-        self.DBty2 = self.DBt.createVecLeft()
-        self.Ey2 = self.E.createVecLeft()
+        self.Umody2 = self.E.createVecLeft()
         self.Tmody3 = self.Et.createVecLeft()
         self.Bty2 = self.Bt.createVecLeft()
         self.Dty3 = self.Dt.createVecLeft()
 
         self.x1, self.x2, self.x3 = self.A.createVecLeft(), self.Smod.createVecLeft(), self.Wmod.createVecLeft()
         self.y1, self.y2, self.y3 = self.A.createVecLeft(), self.Smod.createVecLeft(), self.Wmod.createVecLeft()
         self.z1, self.z2, self.z3 = self.A.createVecLeft(), self.Smod.createVecLeft(), self.Wmod.createVecLeft()
@@ -508,24 +503,30 @@
         self.B.matMult(self.Adinv_Bt, result=self.B_Adinv_Bt)  # B diag(A)^{-1} Bt
 
         # --- modified Schur complement Smod = C - B diag(A)^{-1} Bt
         # compute self.Smod = self.C - B_Adinv_Bt
         self.C.copy(result=self.Smod)
         self.Smod.axpy(-1., self.B_Adinv_Bt)
 
+        # --- Umod = E - D diag(A)^{-1} Bt
         # --- Tmod = Et - B diag(A)^{-1} Dt
 
         self.Adinv.matMult(self.Dt, result=self.Adinv_Dt)      # diag(A)^{-1} Dt
         self.B.matMult(self.Adinv_Dt, result=self.B_Adinv_Dt)  # B diag(A)^{-1} Dt
+        self.D.matMult(self.Adinv_Bt, result=self.D_Adinv_Bt)  # D diag(A)^{-1} Bt
+
+        # compute self.Umod = self.E - D_Adinv_Bt
+        self.E.copy(result=self.Umod)
+        self.Umod.axpy(-1., self.D_Adinv_Bt)
 
         # compute self.Tmod = self.Et - B_Adinv_Dt
         self.Et.copy(result=self.Tmod)
         self.Tmod.axpy(-1., self.B_Adinv_Dt)
 
-        # --- Wmod = R - D diag(A)^{-1} Dt - E diag(Smod)^{-1} Tmod + D diag(A)^{-1} Bt diag(Smod)^{-1} Tmod
+        # --- Wmod = R - D diag(A)^{-1} Dt - Umod diag(Smod)^{-1} Tmod
 
         if self.schur_block_scaling[1]['type']=='diag':
             self.Smod.getDiagonal(result=self.smoddinv_vec)
             self.smoddinv_vec.reciprocal()
         elif self.schur_block_scaling[1]['type']=='rowsum':
             self.Smod.getRowSum(result=self.smoddinv_vec)
             self.smoddinv_vec.abs()
@@ -538,31 +539,22 @@
         self.smoddinv_vec.scale(self.schur_block_scaling[1]['val'])
 
         # form diag(Smod)^{-1}
         self.Smoddinv.setDiagonal(self.smoddinv_vec, addv=PETSc.InsertMode.INSERT)
 
         self.Smoddinv.matMult(self.Tmod, result=self.Smoddinv_Tmod)                        # diag(Smod)^{-1} Tmod
 
-        self.Bt.matMult(self.Smoddinv_Tmod, result=self.Bt_Smoddinv_Tmod)                  # Bt diag(Smod)^{-1} Tmod
-
-        self.Adinv.matMult(self.Bt_Smoddinv_Tmod, result=self.Adinv_Bt_Smoddinv_Tmod)      # diag(A)^{-1} ( Bt diag(Smod)^{-1} Tmod )
-
-        self.D.matMult(self.Adinv_Bt_Smoddinv_Tmod, result=self.D_Adinv_Bt_Smoddinv_Tmod)  # D diag(A)^{-1} ( Bt diag(Smod)^{-1} Tmod )
-
-        self.D.matMult(self.Adinv_Bt, result=self.DBt)                                     # D diag(A)^{-1} Bt for later use
-
-        self.E.matMult(self.Smoddinv_Tmod, result=self.E_Smoddinv_Tmod)                    # E diag(Smod)^{-1} Tmod
+        self.Umod.matMult(self.Smoddinv_Tmod, result=self.Umod_Smoddinv_Tmod)              # Umod diag(Smod)^{-1} Tmod
 
         self.D.matMult(self.Adinv_Dt, result=self.D_Adinv_Dt)                              # D diag(A)^{-1} Dt
 
-        # compute self.Wmod = self.R - D_Adinv_Dt - E_Smoddinv_Tmod + D_Adinv_Bt_Smoddinv_Tmod
+        # compute self.Wmod = self.R - D_Adinv_Dt - Umod_Smoddinv_Tmod
         self.R.copy(result=self.Wmod)
         self.Wmod.axpy(-1., self.D_Adinv_Dt)
-        self.Wmod.axpy(-1., self.E_Smoddinv_Tmod)
-        self.Wmod.axpy(1., self.D_Adinv_Bt_Smoddinv_Tmod)
+        self.Wmod.axpy(-1., self.Umod_Smoddinv_Tmod)
 
         # operator values have changed - do we need to re-set them?
         self.ksp_fields[0].setOperators(self.A)
         self.ksp_fields[1].setOperators(self.Smod)
         self.ksp_fields[2].setOperators(self.Wmod)
 
         # Schur complement reduction
@@ -594,31 +586,27 @@
         self.z2.axpby(1., 0., self.x2)
         self.z2.axpy(-1., self.By1)
 
         # 2) solve Smod * y_2 = z_2
         self.ksp_fields[1].solve(self.z2, self.y2)
 
         self.D.mult(self.y1, self.Dy1)
-        self.DBt.mult(self.y2, self.DBty2)
-        self.E.mult(self.y2, self.Ey2)
+        self.Umod.mult(self.y2, self.Umody2)
 
-        # compute z3 = x3 - (self.Dy1 - self.DBty2 + self.Ey2)
+        # compute z3 = x3 - self.Dy1 - self.Umody2
         self.z3.axpby(1., 0., self.x3)
         self.z3.axpy(-1., self.Dy1)
-        self.z3.axpy(1., self.DBty2)
-        self.z3.axpy(-1., self.Ey2)
+        self.z3.axpy(-1., self.Umody2)
 
         # 3) solve Wmod * y_3 = z_3
         self.ksp_fields[2].solve(self.z3, self.y3)
 
         self.Tmod.mult(self.y3, self.Tmody3)
 
         # compute z2 = x2 - self.By1 - self.Tmody3
-        self.z2.axpby(1., 0., self.x2)
-        self.z2.axpy(-1., self.By1)
         self.z2.axpy(-1., self.Tmody3)
 
         # 4) solve Smod * y_2 = z_2
         self.ksp_fields[1].solve(self.z2, self.y2)
 
         self.Bt.mult(self.y2, self.Bty2)
         self.Dt.mult(self.y3, self.Dty3)
@@ -641,60 +629,123 @@
         y.setValues(self.iset[1], self.y2.array)
         y.setValues(self.iset[2], self.y3.array)
 
         y.assemble()
 
 
 
-# symmetric BGS with inner schur_3x3 (tailored towards monolithic FrSI, where the 4th block is the ALE problem)
+# special MH Schur complement 3x3 preconditioner - SIMPLE version: spares the last A-solve by doing a diag(A)^{-1} update
+class schur_3x3simple(schur_3x3):
+
+    # computes y = P^{-1} x
+    def apply(self, pc, x, y):
+
+        # get subvectors (references!)
+        x.getSubVector(self.iset[0], subvec=self.x1)
+        x.getSubVector(self.iset[1], subvec=self.x2)
+        x.getSubVector(self.iset[2], subvec=self.x3)
+
+        tss = time.time()
+
+        # 1) solve A * y_1 = x_1
+        self.ksp_fields[0].solve(self.x1, self.y1)
+
+        self.B.mult(self.y1, self.By1)
+
+        # compute z2 = x2 - self.By1
+        self.z2.axpby(1., 0., self.x2)
+        self.z2.axpy(-1., self.By1)
+
+        # 2) solve Smod * y_2 = z_2
+        self.ksp_fields[1].solve(self.z2, self.y2)
+
+        self.D.mult(self.y1, self.Dy1)
+        self.Umod.mult(self.y2, self.Umody2)
+
+        # compute z3 = x3 - self.Dy1 - self.Umody2
+        self.z3.axpby(1., 0., self.x3)
+        self.z3.axpy(-1., self.Dy1)
+        self.z3.axpy(-1., self.Umody2)
+
+        # 3) solve Wmod * y_3 = z_3
+        self.ksp_fields[2].solve(self.z3, self.y3)
+
+        self.Tmod.mult(self.y3, self.Tmody3)
+
+        # compute z2 = x2 - self.By1 - self.Tmody3
+        self.z2.axpy(-1., self.Tmody3)
+
+        # 4) solve Smod * y_2 = z_2
+        self.ksp_fields[1].solve(self.z2, self.y2)
+
+        # 5) update y_1
+        self.Adinv_Bt.mult(self.y2, self.Bty2)
+        self.Adinv_Dt.mult(self.y3, self.Dty3)
+        # compute y1 -= (self.Bty2 + self.Dty3)
+        self.y1.axpy(-1., self.Bty2)
+        self.y1.axpy(-1., self.Dty3)
+
+        # restore/clean up
+        x.restoreSubVector(self.iset[0], subvec=self.x1)
+        x.restoreSubVector(self.iset[1], subvec=self.x2)
+        x.restoreSubVector(self.iset[2], subvec=self.x3)
+
+        # set into y vector
+        y.setValues(self.iset[0], self.y1.array)
+        y.setValues(self.iset[1], self.y2.array)
+        y.setValues(self.iset[2], self.y3.array)
+
+        y.assemble()
+
+
+
+# BGS with inner schur_3x3 (tailored towards monolithic FrSI, where the 4th block is the ALE problem)
 # influence ALE on fluid is much more relevant than vice versa: in BGS, solve ALE first and then do 3x3 solve for fluid
-class schur_bgssym_4x4(schur_3x3):
+# --> NO upward solve that accounts for fluid on ALE influence
+class bgs_schur_4x4(schur_3x3):
 
     def check_field_size(self):
         assert(self.nfields==4)
 
 
     def init_mat_vec(self, pc):
         opmats = super().init_mat_vec(pc)
 
-        self.G  = self.P.createSubMatrix(self.iset[3],self.iset[3])
+        self.G = self.P.createSubMatrix(self.iset[3],self.iset[3])
 
         # create index set encompassing the first 3 blocks
         self.iset_012 = self.iset[0].expand(self.iset[1])
         self.iset_012 = self.iset_012.expand(self.iset[2])
         self.iset_012.sort()
-        # get additional offdiagonal block
-        self.Ft = self.P.createSubMatrix(self.iset_012,self.iset[3])
-        self.F  = self.P.createSubMatrix(self.iset[3],self.iset_012)
+        # get additional offdiagonal blocks
+        self.H  = self.P.createSubMatrix(self.iset_012,self.iset[3])
 
         self.x4 = self.G.createVecLeft()
         self.y4 = self.G.createVecLeft()
         self.z4 = self.G.createVecLeft()
 
-        self.x123 = self.Ft.createVecLeft()
-        self.y123 = self.Ft.createVecLeft()
-        self.z123 = self.Ft.createVecLeft()
+        self.x123 = self.H.createVecLeft()
+        self.y123 = self.H.createVecLeft()
+        self.z123 = self.H.createVecLeft()
 
-        self.Fty4 = self.Ft.createVecLeft()
-        self.Fy123 = self.F.createVecLeft()
+        self.Hy4 = self.H.createVecLeft()
 
         self.xtmp = self.P.createVecLeft()
 
         # do we need this???
         self.G.setOption(PETSc.Mat.Option.NO_OFF_PROC_ZERO_ROWS, True)
 
         return [opmats[0], opmats[1], opmats[2], self.G]
 
 
     def setUp(self, pc):
         super().setUp(pc)
 
         self.P.createSubMatrix(self.iset[3],self.iset[3], submat=self.G)
-        self.P.createSubMatrix(self.iset_012,self.iset[3], submat=self.Ft)
-        self.P.createSubMatrix(self.iset[3],self.iset_012, submat=self.F)
+        self.P.createSubMatrix(self.iset_012,self.iset[3], submat=self.H)
 
         # operator values have changed - do we need to re-set it?
         self.ksp_fields[3].setOperators(self.G)
 
 
     # computes y = P^{-1} x
     def apply(self, pc, x, y):
@@ -702,91 +753,185 @@
         # get subvectors
         x.getSubVector(self.iset[3], subvec=self.x4)
         x.getSubVector(self.iset_012, subvec=self.x123)
 
         # 1) solve G * y_4 = x_4
         self.ksp_fields[3].solve(self.x4, self.y4)
 
-        self.Ft.mult(self.y4, self.Fty4)
+        self.H.mult(self.y4, self.Hy4)
 
-        # compute z123 = x123 - self.Fty4
+        # compute z123 = x123 - self.Hy4
         self.z123.axpby(1., 0., self.x123)
-        self.z123.axpy(-1., self.Fty4)
+        self.z123.axpy(-1., self.Hy4)
 
-        # 2) Schur solve A * y_123 = z_123
+        # 2) Schur solve F * y_123 = z_123
         self.xtmp.setValues(self.iset_012, self.z123.array)
         self.xtmp.assemble()
         super().apply(pc, self.xtmp, y)
 
-        y.getSubVector(self.iset_012, subvec=self.y123)
+        # restore/clean up
+        x.restoreSubVector(self.iset_012, subvec=self.x123)
+        x.restoreSubVector(self.iset[3], subvec=self.x4)
 
-        self.F.mult(self.y123, self.Fy123)
+        # set into y vector
+        y.setValues(self.iset[3], self.y4.array)
 
-        # compute z4 = x4 - self.Fy123
-        self.z4.axpby(1., 0., self.x4)
-        self.z4.axpy(-1., self.Fy123)
+        y.assemble()
 
-        # 3) solve G * y_4 = z_4
-        self.ksp_fields[3].solve(self.z4, self.y4)
+
+
+# SIMPLE version of above: last A-solve replaced by diag(A)^{-1} update
+class bgs_schur_4x4simple(bgs_schur_4x4):
+
+    # computes y = P^{-1} x
+    def apply(self, pc, x, y):
+
+        # get subvectors
+        x.getSubVector(self.iset[3], subvec=self.x4)
+        x.getSubVector(self.iset_012, subvec=self.x123)
+
+        # 1) solve G * y_4 = x_4
+        self.ksp_fields[3].solve(self.x4, self.y4)
+
+        self.H.mult(self.y4, self.Hy4)
+
+        # compute z123 = x123 - self.Hy4
+        self.z123.axpby(1., 0., self.x123)
+        self.z123.axpy(-1., self.Hy4)
+
+        # 2) Schur solve F * y_123 = z_123
+        self.xtmp.setValues(self.iset_012, self.z123.array)
+        self.xtmp.assemble()
+        schur_3x3simple.apply(self, pc, self.xtmp, y)
 
         # restore/clean up
-        y.restoreSubVector(self.iset_012, subvec=self.y123)
         x.restoreSubVector(self.iset_012, subvec=self.x123)
         x.restoreSubVector(self.iset[3], subvec=self.x4)
 
         # set into y vector
         y.setValues(self.iset[3], self.y4.array)
 
         y.assemble()
 
 
-class schur_bgs_4x4(schur_bgssym_4x4):
+
+# symmetric BGS with inner schur_3x3 (tailored towards monolithic FrSI, where the 4th block is the ALE problem)
+# influence ALE on fluid is much more relevant than vice versa: in BGS, solve ALE first and then do 3x3 solve for fluid
+# --> WITH upward solve that accounts for fluid on ALE influence (guess can often be neglected, since only little gain...)
+class bgssym_schur_4x4(bgs_schur_4x4):
+
+    def init_mat_vec(self, pc):
+        opmats = super().init_mat_vec(pc)
+
+        # get additional offdiagonal block
+        self.Ht = self.P.createSubMatrix(self.iset[3],self.iset_012)
+
+        self.Hty123 = self.Ht.createVecLeft()
+
+        return [opmats[0], opmats[1], opmats[2], opmats[3]]
+
 
     def setUp(self, pc):
         super().setUp(pc)
 
-        self.P.createSubMatrix(self.iset[3],self.iset[3], submat=self.G)
-        self.P.createSubMatrix(self.iset_012,self.iset[3], submat=self.Ft)
+        self.P.createSubMatrix(self.iset[3],self.iset_012, submat=self.Ht)
 
-        # operator values have changed - do we need to re-set it?
-        self.ksp_fields[3].setOperators(self.G)
 
     # computes y = P^{-1} x
     def apply(self, pc, x, y):
 
         # get subvectors
         x.getSubVector(self.iset[3], subvec=self.x4)
         x.getSubVector(self.iset_012, subvec=self.x123)
 
         # 1) solve G * y_4 = x_4
         self.ksp_fields[3].solve(self.x4, self.y4)
 
-        self.Ft.mult(self.y4, self.Fty4)
+        self.H.mult(self.y4, self.Hy4)
 
-        # compute z123 = x123 - self.Fty4
+        # compute z123 = x123 - self.Hy4
         self.z123.axpby(1., 0., self.x123)
-        self.z123.axpy(-1., self.Fty4)
+        self.z123.axpy(-1., self.Hy4)
 
-        # 2) Schur solve A * y_123 = z_123
+        # 2) Schur solve F * y_123 = z_123
         self.xtmp.setValues(self.iset_012, self.z123.array)
         self.xtmp.assemble()
         schur_3x3.apply(self, pc, self.xtmp, y)
 
+        y.getSubVector(self.iset_012, subvec=self.y123)
+
+        self.Ht.mult(self.y123, self.Hty123)
+
+        # compute z4 = x4 - self.Hty123
+        self.z4.axpby(1., 0., self.x4)
+        self.z4.axpy(-1., self.Hty123)
+
+        # 3) solve G * y_4 = z_4
+        self.ksp_fields[3].solve(self.z4, self.y4)
+
+        # restore/clean up
+        y.restoreSubVector(self.iset_012, subvec=self.y123)
+        x.restoreSubVector(self.iset_012, subvec=self.x123)
+        x.restoreSubVector(self.iset[3], subvec=self.x4)
+
+        # set into y vector
+        y.setValues(self.iset[3], self.y4.array)
+
+        y.assemble()
+
+
+# SIMPLE version of above: last A-solve replaced by diag(A)^{-1} update
+class bgssym_schur_4x4simple(bgssym_schur_4x4):
+
+    # computes y = P^{-1} x
+    def apply(self, pc, x, y):
+
+        # get subvectors
+        x.getSubVector(self.iset[3], subvec=self.x4)
+        x.getSubVector(self.iset_012, subvec=self.x123)
+
+        # 1) solve G * y_4 = x_4
+        self.ksp_fields[3].solve(self.x4, self.y4)
+
+        self.H.mult(self.y4, self.Hy4)
+
+        # compute z123 = x123 - self.Hy4
+        self.z123.axpby(1., 0., self.x123)
+        self.z123.axpy(-1., self.Hy4)
+
+        # 2) Schur solve F * y_123 = z_123
+        self.xtmp.setValues(self.iset_012, self.z123.array)
+        self.xtmp.assemble()
+        schur_3x3simple.apply(self, pc, self.xtmp, y)
+
+        y.getSubVector(self.iset_012, subvec=self.y123)
+
+        self.Ht.mult(self.y123, self.Hty123)
+
+        # compute z4 = x4 - self.Hty123
+        self.z4.axpby(1., 0., self.x4)
+        self.z4.axpy(-1., self.Hty123)
+
+        # 3) solve G * y_4 = z_4
+        self.ksp_fields[3].solve(self.z4, self.y4)
+
         # restore/clean up
+        y.restoreSubVector(self.iset_012, subvec=self.y123)
         x.restoreSubVector(self.iset_012, subvec=self.x123)
         x.restoreSubVector(self.iset[3], subvec=self.x4)
 
         # set into y vector
         y.setValues(self.iset[3], self.y4.array)
 
         y.assemble()
 
 
+
 # Schur complement preconditioner replacing the last solve with a diag(A)^{-1} update
-class simple_2x2(schur_2x2):
+class schur_2x2simple(schur_2x2):
 
     # computes y = P^{-1} x
     def apply(self, pc, x, y):
 
         # get subvectors
         x.getSubVector(self.iset[0], subvec=self.x1)
         x.getSubVector(self.iset[1], subvec=self.x2)
@@ -834,15 +979,14 @@
 
         self.A  = self.P.createSubMatrix(self.iset[0],self.iset[0])
         self.Bt = self.P.createSubMatrix(self.iset[0],self.iset[1])
         self.B  = self.P.createSubMatrix(self.iset[1],self.iset[0])
         self.C  = self.P.createSubMatrix(self.iset[1],self.iset[1])
 
         self.By1 = self.B.createVecLeft()
-        self.Bty2 = self.Bt.createVecLeft()
 
         self.x1, self.x2 = self.A.createVecLeft(), self.C.createVecLeft()
         self.y1, self.y2 = self.A.createVecLeft(), self.C.createVecLeft()
         self.z2 = self.C.createVecLeft()
 
         # do we need these???
         self.A.setOption(PETSc.Mat.Option.NO_OFF_PROC_ZERO_ROWS, True)
@@ -852,53 +996,310 @@
 
 
     def setUp(self, pc):
 
         ts = time.time()
 
         self.P.createSubMatrix(self.iset[0],self.iset[0], submat=self.A)
+        self.P.createSubMatrix(self.iset[1],self.iset[0], submat=self.B)
+        self.P.createSubMatrix(self.iset[1],self.iset[1], submat=self.C)
+
+        # operator values have changed - do we need to re-set them?
+        self.ksp_fields[0].setOperators(self.A)
+        self.ksp_fields[1].setOperators(self.C)
+
+        te = time.time() - ts
+        if self.printenh:
+            utilities.print_status("       === PREC setup, te = %.4f s" % (te), self.comm)
+
+
+    # computes y = P^{-1} x
+    def apply(self, pc, x, y):
+
+        # get subvectors
+        x.getSubVector(self.iset[0], subvec=self.x1)
+        x.getSubVector(self.iset[1], subvec=self.x2)
+
+        # 1) solve A * y_1 = x_1
+        self.ksp_fields[0].solve(self.x1, self.y1)
+
+        self.B.mult(self.y1, self.By1)
+
+        # compute z2 = x2 - self.By1
+        self.z2.axpby(1., 0., self.x2)
+        self.z2.axpy(-1., self.By1)
+
+        # 2) solve C * y_2 = z_2
+        self.ksp_fields[1].solve(self.z2, self.y2)
+
+        # restore/clean up
+        x.restoreSubVector(self.iset[0], subvec=self.x1)
+        x.restoreSubVector(self.iset[1], subvec=self.x2)
+
+        # set into y vector
+        y.setValues(self.iset[0], self.y1.array)
+        y.setValues(self.iset[1], self.y2.array)
+
+        y.assemble()
+
+
+
+# symmetric version of 2x2 BGS
+class bgssym_2x2(bgs_2x2):
+
+    def check_field_size(self):
+        assert(self.nfields==2)
+
+
+    def init_mat_vec(self, pc):
+        opmats = super().init_mat_vec(pc)
+
+        self.Bt = self.P.createSubMatrix(self.iset[0],self.iset[1])
+
+        self.Bty2 = self.Bt.createVecLeft()
+
+        self.z1 = self.A.createVecLeft()
+
+        return [opmats[0], opmats[1]]
+
+
+    def setUp(self, pc):
+        super().setUp(pc)
+
         self.P.createSubMatrix(self.iset[0],self.iset[1], submat=self.Bt)
+
+
+    # computes y = P^{-1} x
+    def apply(self, pc, x, y):
+
+        # get subvectors
+        x.getSubVector(self.iset[0], subvec=self.x1)
+        x.getSubVector(self.iset[1], subvec=self.x2)
+
+        # 1) solve A * y_1 = x_1
+        self.ksp_fields[0].solve(self.x1, self.y1)
+
+        self.B.mult(self.y1, self.By1)
+
+        # compute z2 = x2 - self.By1
+        self.z2.axpby(1., 0., self.x2)
+        self.z2.axpy(-1., self.By1)
+
+        # 2) solve C * y_2 = z_2
+        self.ksp_fields[1].solve(self.z2, self.y2)
+
+        self.Bt.mult(self.y2, self.Bty2)
+
+        # compute z1 = x1 - self.Bty1
+        self.z1.axpby(1., 0., self.x1)
+        self.z1.axpy(-1., self.Bty2)
+
+        # 3) solve A * y_1 = x_1
+        self.ksp_fields[0].solve(self.z1, self.y1)
+
+        # restore/clean up
+        x.restoreSubVector(self.iset[0], subvec=self.x1)
+        x.restoreSubVector(self.iset[1], subvec=self.x2)
+
+        # set into y vector
+        y.setValues(self.iset[0], self.y1.array)
+        y.setValues(self.iset[1], self.y2.array)
+
+        y.assemble()
+
+
+
+# own 3x3 Block Gauss-Seidel (can be also called via PETSc's fieldsplit) - implementation mainly for testing purposes
+class bgs_3x3(block_precond):
+
+    def check_field_size(self):
+        assert(self.nfields==3)
+
+
+    def init_mat_vec(self, pc):
+
+        self.A  = self.P.createSubMatrix(self.iset[0],self.iset[0])
+        self.B  = self.P.createSubMatrix(self.iset[1],self.iset[0])
+        self.C  = self.P.createSubMatrix(self.iset[1],self.iset[1])
+        self.D  = self.P.createSubMatrix(self.iset[2],self.iset[0])
+        self.E  = self.P.createSubMatrix(self.iset[2],self.iset[1])
+        self.R  = self.P.createSubMatrix(self.iset[2],self.iset[2])
+
+        self.By1 = self.B.createVecLeft()
+        self.Dy1 = self.D.createVecLeft()
+        self.Ey2 = self.E.createVecLeft()
+
+        self.x1, self.x2, self.x3 = self.A.createVecLeft(), self.C.createVecLeft(), self.R.createVecLeft()
+        self.y1, self.y2, self.y3 = self.A.createVecLeft(), self.C.createVecLeft(), self.R.createVecLeft()
+        self.z2, self.z3 = self.C.createVecLeft(), self.R.createVecLeft()
+
+        # do we need these???
+        self.A.setOption(PETSc.Mat.Option.NO_OFF_PROC_ZERO_ROWS, True)
+        self.C.setOption(PETSc.Mat.Option.NO_OFF_PROC_ZERO_ROWS, True)
+        self.R.setOption(PETSc.Mat.Option.NO_OFF_PROC_ZERO_ROWS, True)
+
+        return [self.A, self.C, self.R]
+
+
+    def setUp(self, pc):
+
+        ts = time.time()
+
+        self.P.createSubMatrix(self.iset[0],self.iset[0], submat=self.A)
         self.P.createSubMatrix(self.iset[1],self.iset[0], submat=self.B)
         self.P.createSubMatrix(self.iset[1],self.iset[1], submat=self.C)
+        self.P.createSubMatrix(self.iset[2],self.iset[0], submat=self.D)
+        self.P.createSubMatrix(self.iset[2],self.iset[1], submat=self.E)
+        self.P.createSubMatrix(self.iset[2],self.iset[2], submat=self.R)
 
         # operator values have changed - do we need to re-set them?
         self.ksp_fields[0].setOperators(self.A)
         self.ksp_fields[1].setOperators(self.C)
+        self.ksp_fields[2].setOperators(self.R)
 
         te = time.time() - ts
         if self.printenh:
             utilities.print_status("       === PREC setup, te = %.4f s" % (te), self.comm)
 
 
     # computes y = P^{-1} x
     def apply(self, pc, x, y):
 
         # get subvectors
         x.getSubVector(self.iset[0], subvec=self.x1)
         x.getSubVector(self.iset[1], subvec=self.x2)
+        x.getSubVector(self.iset[2], subvec=self.x3)
+
+        # 1) solve A * y_1 = x_1
+        self.ksp_fields[0].solve(self.x1, self.y1)
+
+        self.B.mult(self.y1, self.By1)
+
+        # compute z2 = x2 - self.By1
+        self.z2.axpby(1., 0., self.x2)
+        self.z2.axpy(-1., self.By1)
+
+        # 2) solve C * y_2 = z_2
+        self.ksp_fields[1].solve(self.z2, self.y2)
+
+        self.D.mult(self.y1, self.Dy1)
+        self.E.mult(self.y2, self.Ey2)
+
+        # compute z3 = x3 - self.Dy1 - self.Ey2
+        self.z3.axpby(1., 0., self.x3)
+        self.z3.axpy(-1., self.Dy1)
+        self.z3.axpy(-1., self.Ey2)
+
+        # 3) solve R * y_3 = z_3
+        self.ksp_fields[2].solve(self.z3, self.y3)
+
+        # restore/clean up
+        x.restoreSubVector(self.iset[0], subvec=self.x1)
+        x.restoreSubVector(self.iset[1], subvec=self.x2)
+        x.restoreSubVector(self.iset[2], subvec=self.x3)
+
+        # set into y vector
+        y.setValues(self.iset[0], self.y1.array)
+        y.setValues(self.iset[1], self.y2.array)
+        y.setValues(self.iset[2], self.y3.array)
+
+        y.assemble()
+
+
+
+# symmetric version of 3x3 BGS
+class bgssym_3x3(bgs_3x3):
+
+    def check_field_size(self):
+        assert(self.nfields==3)
+
+
+    def init_mat_vec(self, pc):
+        opmats = super().init_mat_vec(pc)
+
+        self.Bt = self.P.createSubMatrix(self.iset[0],self.iset[1])
+        self.Dt = self.P.createSubMatrix(self.iset[0],self.iset[2])
+        self.Et = self.P.createSubMatrix(self.iset[1],self.iset[2])
+
+        self.Ety3 = self.Et.createVecLeft()
+        self.Bty2 = self.Bt.createVecLeft()
+        self.Dty3 = self.Dt.createVecLeft()
+
+        self.z1 = self.A.createVecLeft()
+
+        return [opmats[0], opmats[1], opmats[2]]
+
+
+    def setUp(self, pc):
+        super().setUp(pc)
+
+        self.P.createSubMatrix(self.iset[0],self.iset[1], submat=self.Bt)
+        self.P.createSubMatrix(self.iset[0],self.iset[2], submat=self.Dt)
+        self.P.createSubMatrix(self.iset[1],self.iset[2], submat=self.Et)
+
+
+    # computes y = P^{-1} x
+    def apply(self, pc, x, y):
+
+        # get subvectors
+        x.getSubVector(self.iset[0], subvec=self.x1)
+        x.getSubVector(self.iset[1], subvec=self.x2)
+        x.getSubVector(self.iset[2], subvec=self.x3)
 
         # 1) solve A * y_1 = x_1
         self.ksp_fields[0].solve(self.x1, self.y1)
 
         self.B.mult(self.y1, self.By1)
 
         # compute z2 = x2 - self.By1
         self.z2.axpby(1., 0., self.x2)
         self.z2.axpy(-1., self.By1)
 
         # 2) solve C * y_2 = z_2
         self.ksp_fields[1].solve(self.z2, self.y2)
 
+        self.D.mult(self.y1, self.Dy1)
+        self.E.mult(self.y2, self.Ey2)
+
+        # compute z3 = x3 - self.Dy1 - self.Ey2
+        self.z3.axpby(1., 0., self.x3)
+        self.z3.axpy(-1., self.Dy1)
+        self.z3.axpy(-1., self.Ey2)
+
+        # 3) solve R * y_3 = z_3
+        self.ksp_fields[2].solve(self.z3, self.y3)
+
+        self.Et.mult(self.y3, self.Ety3)
+
+        # compute z2 = x2 - self.By1 - self.Ety3
+        self.z2.axpy(-1., self.Ety3)
+
+        # 4) solve C * y_2 = z_2
+        self.ksp_fields[1].solve(self.z2, self.y2)
+
+        self.Bt.mult(self.y2, self.Bty2)
+        self.Dt.mult(self.y3, self.Dty3)
+
+        # compute z1 = x1 - self.Bty2 - self.Dty3
+        self.z1.axpby(1., 0., self.x1)
+        self.z1.axpy(-1., self.Bty2)
+        self.z1.axpy(-1., self.Dty3)
+
+        # 5) solve A * y_1 = z_1
+        self.ksp_fields[0].solve(self.z1, self.y1)
+
         # restore/clean up
         x.restoreSubVector(self.iset[0], subvec=self.x1)
         x.restoreSubVector(self.iset[1], subvec=self.x2)
+        x.restoreSubVector(self.iset[2], subvec=self.x3)
 
         # set into y vector
         y.setValues(self.iset[0], self.y1.array)
         y.setValues(self.iset[1], self.y2.array)
+        y.setValues(self.iset[2], self.y3.array)
 
         y.assemble()
 
 
 
 # own 2x2 Jacobi (can be also called via PETSc's fieldsplit) - implementation mainly for testing purposes
 # P = [A  0], --> P^{-1} = [A^{-1}  0  ]
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/solver/projection.py` & `ambit_fe-1.2.6/src/ambit_fe/solver/projection.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/solver/solver_nonlin.py` & `ambit_fe-1.2.6/src/ambit_fe/solver/solver_nonlin.py`

 * *Files 5% similar despite different names*

```diff
@@ -289,15 +289,15 @@
         self.ksp = [[]]*self.nprob
 
         for npr in range(self.nprob):
 
             # perform initial matrix and residual reduction to set the correct arrays
             if self.pb[npr].rom:
                 self.pb[npr].rom.reduce_stiffness(self.pb[npr].K_list, self.pb[npr].K_list_rom, self.pb[npr].K_list_tmp)
-                self.pb[npr].rom.reduce_residual(self.pb[npr].r_list, self.pb[npr].r_list_rom, x=self.x[npr][0])
+                self.pb[npr].rom.reduce_residual(self.pb[npr].r_list, self.pb[npr].r_list_rom)
 
             # create nested matrix and residual structures
             self.K_full_nest[npr] = PETSc.Mat().createNest(self.K_list_sol[npr], isrows=None, iscols=None, comm=self.comm)
             self.r_full_nest[npr] = PETSc.Vec().createNest(self.r_list_sol[npr])
 
             #self.K_full_nest[npr].setOption(PETSc.Mat.Option.NO_OFF_PROC_ZERO_ROWS, True)
 
@@ -438,44 +438,80 @@
 
                     elif self.block_precond[npr] == 'schur2x2':
 
                         self.ksp[npr].getPC().setType(PETSc.PC.Type.PYTHON)
                         bj = preconditioner.schur_2x2(self.iset[npr], self.precond_fields[npr], self.printenh, self.solver_params, self.comm)
                         self.ksp[npr].getPC().setPythonContext(bj)
 
-                    elif self.block_precond[npr] == 'simple2x2':
+                    elif self.block_precond[npr] == 'schur2x2simple':
 
                         self.ksp[npr].getPC().setType(PETSc.PC.Type.PYTHON)
-                        bj = preconditioner.simple_2x2(self.iset[npr], self.precond_fields[npr], self.printenh, self.solver_params, self.comm)
+                        bj = preconditioner.schur_2x2simple(self.iset[npr], self.precond_fields[npr], self.printenh, self.solver_params, self.comm)
                         self.ksp[npr].getPC().setPythonContext(bj)
 
                     elif self.block_precond[npr] == 'schur3x3':
 
                         self.ksp[npr].getPC().setType(PETSc.PC.Type.PYTHON)
                         bj = preconditioner.schur_3x3(self.iset[npr], self.precond_fields[npr], self.printenh, self.solver_params, self.comm)
                         self.ksp[npr].getPC().setPythonContext(bj)
 
-                    elif self.block_precond[npr] == 'schurbgs4x4':
+                    elif self.block_precond[npr] == 'schur3x3simple':
 
                         self.ksp[npr].getPC().setType(PETSc.PC.Type.PYTHON)
-                        bj = preconditioner.schur_bgs_4x4(self.iset[npr], self.precond_fields[npr], self.printenh, self.solver_params, self.comm)
+                        bj = preconditioner.schur_3x3simple(self.iset[npr], self.precond_fields[npr], self.printenh, self.solver_params, self.comm)
                         self.ksp[npr].getPC().setPythonContext(bj)
 
-                    elif self.block_precond[npr] == 'schurbgssym4x4':
+                    elif self.block_precond[npr] == 'bgsschur4x4':
 
                         self.ksp[npr].getPC().setType(PETSc.PC.Type.PYTHON)
-                        bj = preconditioner.schur_bgssym_4x4(self.iset[npr], self.precond_fields[npr], self.printenh, self.solver_params, self.comm)
+                        bj = preconditioner.bgs_schur_4x4(self.iset[npr], self.precond_fields[npr], self.printenh, self.solver_params, self.comm)
+                        self.ksp[npr].getPC().setPythonContext(bj)
+
+                    elif self.block_precond[npr] == 'bgsschur4x4simple':
+
+                        self.ksp[npr].getPC().setType(PETSc.PC.Type.PYTHON)
+                        bj = preconditioner.bgs_schur_4x4simple(self.iset[npr], self.precond_fields[npr], self.printenh, self.solver_params, self.comm)
+                        self.ksp[npr].getPC().setPythonContext(bj)
+
+                    elif self.block_precond[npr] == 'bgssymschur4x4':
+
+                        self.ksp[npr].getPC().setType(PETSc.PC.Type.PYTHON)
+                        bj = preconditioner.bgssym_schur_4x4(self.iset[npr], self.precond_fields[npr], self.printenh, self.solver_params, self.comm)
+                        self.ksp[npr].getPC().setPythonContext(bj)
+
+                    elif self.block_precond[npr] == 'bgssymschur4x4simple':
+
+                        self.ksp[npr].getPC().setType(PETSc.PC.Type.PYTHON)
+                        bj = preconditioner.bgssym_schur_4x4simple(self.iset[npr], self.precond_fields[npr], self.printenh, self.solver_params, self.comm)
                         self.ksp[npr].getPC().setPythonContext(bj)
 
                     elif self.block_precond[npr] == 'bgs2x2': # can also be called via PETSc's fieldsplit
 
                         self.ksp[npr].getPC().setType(PETSc.PC.Type.PYTHON)
                         bj = preconditioner.bgs_2x2(self.iset[npr], self.precond_fields[npr], self.printenh, self.solver_params, self.comm)
                         self.ksp[npr].getPC().setPythonContext(bj)
 
+                    elif self.block_precond[npr] == 'bgssym2x2': # can also be called via PETSc's fieldsplit
+
+                        self.ksp[npr].getPC().setType(PETSc.PC.Type.PYTHON)
+                        bj = preconditioner.bgssym_2x2(self.iset[npr], self.precond_fields[npr], self.printenh, self.solver_params, self.comm)
+                        self.ksp[npr].getPC().setPythonContext(bj)
+
+                    elif self.block_precond[npr] == 'bgs3x3': # can also be called via PETSc's fieldsplit
+
+                        self.ksp[npr].getPC().setType(PETSc.PC.Type.PYTHON)
+                        bj = preconditioner.bgs_3x3(self.iset[npr], self.precond_fields[npr], self.printenh, self.solver_params, self.comm)
+                        self.ksp[npr].getPC().setPythonContext(bj)
+
+                    elif self.block_precond[npr] == 'bgssym3x3': # can also be called via PETSc's fieldsplit
+
+                        self.ksp[npr].getPC().setType(PETSc.PC.Type.PYTHON)
+                        bj = preconditioner.bgssym_3x3(self.iset[npr], self.precond_fields[npr], self.printenh, self.solver_params, self.comm)
+                        self.ksp[npr].getPC().setPythonContext(bj)
+
                     elif self.block_precond[npr] == 'jacobi2x2': # can also be called via PETSc's fieldsplit
 
                         self.ksp[npr].getPC().setType(PETSc.PC.Type.PYTHON)
                         bj = preconditioner.jacobi_2x2(self.iset[npr], self.precond_fields[npr], self.printenh, self.solver_params, self.comm)
                         self.ksp[npr].getPC().setPythonContext(bj)
 
                     else:
@@ -824,15 +860,18 @@
 
         tee = time.time() - tes
         if self.printenh:
             utilities.print_status(" "*self.indlen_[npr] + "      === Residual assemble, t = %.4f s" % (tee), self.comm)
 
         # apply model order reduction of residual
         if self.pb[npr].rom:
-            self.pb[npr].rom.reduce_residual(self.pb[npr].r_list, self.pb[npr].r_list_rom, x=self.x[npr][0])
+            self.pb[npr].rom.reduce_residual(self.pb[npr].r_list, self.pb[npr].r_list_rom)
+
+        if bool(self.pb[npr].pbase.residual_scale):
+            self.pb[npr].scale_residual_list(self.r_list_sol[npr])
 
         # get residual norms
         for n in range(self.nfields[npr]):
             self.r_list_sol[npr][n].assemble()
             self.resnorms[npr]['res'+str(n+1)] = self.r_list_sol[npr][n].norm()
 
 
@@ -847,14 +886,17 @@
         if self.printenh:
             utilities.print_status(" "*self.indlen_[npr] + "      === Jacobian assemble, t = %.4f s" % (tee), self.comm)
 
         # apply model order reduction of stiffness
         if self.pb[npr].rom:
             self.pb[npr].rom.reduce_stiffness(self.pb[npr].K_list, self.pb[npr].K_list_rom, self.pb[npr].K_list_tmp)
 
+        if bool(self.pb[npr].pbase.residual_scale):
+            self.pb[npr].scale_jacobian_list(self.K_list_sol[npr])
+
         if self.PTC:
             # computes K_00 + k_PTC * I
             self.K_list_sol[npr][0][0].shift(k_PTC)
 
 
     def reset_step(self, vec, vec_start, ghosted):
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/solver/solver_utils.py` & `ambit_fe-1.2.6/src/ambit_fe/solver/solver_utils.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/timeintegration.py` & `ambit_fe-1.2.6/src/ambit_fe/timeintegration.py`

 * *Files 11% similar despite different names*

```diff
@@ -178,129 +178,108 @@
         for (m, n) in zip(self.funcsexpr_to_update_old, self.funcsexpr_to_update):
             if self.funcsexpr_to_update_old[m] is not None:
                 m.vector.axpby(1.0, 0.0, n.vector)
                 m.vector.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
 
 
     # OST update formula for the time derivative of a variable
-    def update_dvar_ost(self, var, var_old, dvar_old, dvarout=None, ufl=True):
+    def update_dvar_ost(self, var, var_old, dvar_old, dt, dvarout=None, uflform=True):
 
-        if ufl: # ufl form
-            dt_ = self.dt
-            theta_ = self.theta_ost
-            return 1./(theta_*dt_) * (var - var_old) - (1.-theta_)/theta_ * dvar_old
+        if uflform: # ufl form
+            return 1./(self.theta_ost*dt) * (var - var_old) - (1.-self.theta_ost)/self.theta_ost * dvar_old
         else: # PETSc vector update
-            dt_ = float(self.dt)
-            theta_ = float(self.theta_ost)
-
-            dvarout.axpby(-(1.-theta_)/theta_, 0.0, dvar_old)
-            dvarout.axpy(1./(theta_*dt_), var)
-            dvarout.axpy(-1./(theta_*dt_), var_old)
+            dvarout.axpby(-(1.-self.theta_ost)/self.theta_ost, 0.0, dvar_old)
+            dvarout.axpy(1./(self.theta_ost*dt), var)
+            dvarout.axpy(-1./(self.theta_ost*dt), var_old)
 
 
     # OST update formula for the second time derivative of a variable
-    def update_d2var_ost(self, var, var_old, dvar_old, d2var_old, d2varout=None, ufl=True):
+    def update_d2var_ost(self, var, var_old, dvar_old, d2var_old, dt, d2varout=None, uflform=True):
 
-        if ufl: # ufl form
-            dt_ = self.dt
-            theta_ = self.theta_ost
-            return 1./(theta_*theta_*dt_*dt_) * (var - var_old) - 1./(theta_*theta_*dt_) * dvar_old - (1.-theta_)/theta_ * d2var_old
+        if uflform: # ufl form
+            return 1./(self.theta_ost*self.theta_ost*dt*dt) * (var - var_old) - 1./(self.theta_ost*self.theta_ost*dt) * dvar_old - (1.-self.theta_ost)/self.theta_ost * d2var_old
         else: # PETSc vector update
-            dt_ = float(self.dt)
-            theta_ = float(self.theta_ost)
-
-            d2varout.axpby(-(1.-theta_)/theta_, 0.0, d2var_old)
-            d2varout.axpy(-1./(theta_*theta_*dt_), dvar_old)
-            d2varout.axpy(1./(theta_*theta_*dt_*dt_), var)
-            d2varout.axpy(-1./(theta_*theta_*dt_*dt_), var_old)
+            d2varout.axpby(-(1.-self.theta_ost)/self.theta_ost, 0.0, d2var_old)
+            d2varout.axpy(-1./(self.theta_ost*self.theta_ost*dt), dvar_old)
+            d2varout.axpy(1./(self.theta_ost*self.theta_ost*dt*dt), var)
+            d2varout.axpy(-1./(self.theta_ost*self.theta_ost*dt*dt), var_old)
 
 
     # Newmark update formula for the time derivative of a variable: 1st order scheme
-    def update_dvar_newmark_1st(self, var, var_old, dvar_old, dvarout=None, ufl=True):
+    def update_dvar_newmark_1st(self, var, var_old, dvar_old, dt, dvarout=None, uflform=True):
 
-        if ufl: # ufl form
-            dt_ = self.dt
-            gamma_ = self.gamma
-            return 1./(gamma_*dt_) * (var - var_old) - (1.-gamma_)/gamma_ * dvar_old
+        if uflform: # ufl form
+            return 1./(self.gamma*dt) * (var - var_old) - (1.-self.gamma)/self.gamma * dvar_old
         else: # PETSc vector update
-            dt_ = float(self.dt)
-            gamma_ = float(self.gamma)
-
-            dvarout.axpby(-(1.-gamma_)/gamma_, 0.0, dvar_old)
-            dvarout.axpy(1./(gamma_*dt_), var)
-            dvarout.axpy(-1./(gamma_*dt_), var_old)
+            dvarout.axpby(-(1.-self.gamma)/self.gamma, 0.0, dvar_old)
+            dvarout.axpy(1./(self.gamma*dt), var)
+            dvarout.axpy(-1./(self.gamma*dt), var_old)
 
 
     # Newmark update formula for the time derivative of a variable: 2nd order scheme
-    def update_dvar_newmark_2nd(self, var, var_old, dvar_old, d2var_old, dvarout=None, ufl=True):
+    def update_dvar_newmark_2nd(self, var, var_old, dvar_old, d2var_old, dt, dvarout=None, uflform=True):
 
-        if ufl: # ufl form
-            dt_ = self.dt
-            gamma_ = self.gamma
-            beta_ = self.beta
-            return gamma_/(beta_*dt_) * (var - var_old) - (gamma_ - beta_)/beta_ * dvar_old - (gamma_-2.*beta_)/(2.*beta_) * dt_*d2var_old
+        if uflform: # ufl form
+            return self.gamma/(self.beta*dt) * (var - var_old) - (self.gamma - self.beta)/self.beta * dvar_old - (self.gamma-2.*self.beta)/(2.*self.beta) * dt*d2var_old
         else: # PETSc vector update
-            dt_ = float(self.dt)
-            gamma_ = float(self.gamma)
-            beta_ = float(self.beta)
-
-            dvarout.axpby(-(gamma_-beta_)/beta_, 0.0, dvar_old)
-            dvarout.axpy(-(gamma_-2.*beta_)/(2.*beta_) * dt_, d2var_old)
-            dvarout.axpy(gamma_/(beta_*dt_), var)
-            dvarout.axpy(-gamma_/(beta_*dt_), var_old)
+            dvarout.axpby(-(self.gamma-self.beta)/self.beta, 0.0, dvar_old)
+            dvarout.axpy(-(self.gamma-2.*self.beta)/(2.*self.beta) * dt, d2var_old)
+            dvarout.axpy(self.gamma/(self.beta*dt), var)
+            dvarout.axpy(-self.gamma/(self.beta*dt), var_old)
 
 
     # Newmark update formula for the second time derivative of a variable
-    def update_d2var_newmark(self, var, var_old, dvar_old, d2var_old, d2varout=None, ufl=True):
+    def update_d2var_newmark(self, var, var_old, dvar_old, d2var_old, dt, d2varout=None, uflform=True):
 
-        if ufl: # ufl form
-            dt_ = self.dt
-            beta_ = self.beta
-            return 1./(beta_*dt_*dt_) * (var - var_old) - 1./(beta_*dt_) * dvar_old - (1.-2.*beta_)/(2.*beta_) * d2var_old
+        if uflform: # ufl form
+            return 1./(self.beta*dt*dt) * (var - var_old) - 1./(self.beta*dt) * dvar_old - (1.-2.*self.beta)/(2.*self.beta) * d2var_old
         else: # PETSc vector update
-            dt_ = float(self.dt)
-            beta_ = float(self.beta)
-
-            d2varout.axpby(-(1.-2.*beta_)/(2.*beta_), 0.0, d2var_old)
-            d2varout.axpy(-1./(beta_*dt_), dvar_old)
-            d2varout.axpy(1./(beta_*dt_*dt_), var)
-            d2varout.axpy(-1./(beta_*dt_*dt_), var_old)
+            d2varout.axpby(-(1.-2.*self.beta)/(2.*self.beta), 0.0, d2var_old)
+            d2varout.axpy(-1./(self.beta*dt), dvar_old)
+            d2varout.axpy(1./(self.beta*dt*dt), var)
+            d2varout.axpy(-1./(self.beta*dt*dt), var_old)
 
 
     # OST update formula for the first integration of a variable
-    def update_varint_ost(self, var, var_old, varint_old, varintout=None, ufl=True):
+    def update_varint_ost(self, var, var_old, varint_old, dt, varintout=None, uflform=True):
 
-        if ufl: # ufl form
-            dt_ = self.dt
-            theta_ = self.theta_ost
-            return theta_*dt_ * var + (1.-theta_)*dt_ * var_old + varint_old
+        if uflform: # ufl form
+            return self.theta_ost*dt * var + (1.-self.theta_ost)*dt * var_old + varint_old
         else:
-            dt_ = float(self.dt)
-            theta_ = float(self.theta_ost)
-
             varintout.axpby(1., 0.0, varint_old)
-            varintout.axpy(theta_*dt_, var)
-            varintout.axpy((1.-theta_)*dt_, var_old)
+            varintout.axpy(self.theta_ost*dt, var)
+            varintout.axpy((1.-self.theta_ost)*dt, var_old)
 
 
     # Newmark update formula for the first integration of a variable: 1st order scheme
-    def update_varint_newmark_1st(self, var, var_old, varint_old, varintout=None, ufl=True):
+    def update_varint_newmark_1st(self, var, var_old, varint_old, dt, varintout=None, uflform=True):
 
-        if ufl: # ufl form
-            dt_ = self.dt
-            gamma_ = self.gamma
-            return gamma_*dt_ * var + (1.-gamma_)*dt_ * var_old + varint_old
+        if uflform: # ufl form
+            return self.gamma*dt * var + (1.-self.gamma)*dt * var_old + varint_old
         else: # PETSc vector update
-            dt_ = float(self.dt)
-            gamma_ = float(self.gamma)
-
             varintout.axpby(1., 0.0, varint_old)
-            varintout.axpy(gamma_*dt_, var)
-            varintout.axpy((1.-gamma_)*dt_, var_old)
+            varintout.axpy(self.gamma*dt, var)
+            varintout.axpy((1.-self.gamma)*dt, var_old)
 
+    # get constant time integration factors for the derivative w.r.t. the primary var
+    # (may be needed by some algorithms that don't use the ufl form)
+    def get_factor_deriv_dvar_ost(self, dt):
+        return 1./(self.theta_ost*dt)
+    def get_factor_deriv_d2var_ost(self, dt):
+        return 1./(self.theta_ost*self.theta_ost*dt*dt)
+    def get_factor_deriv_dvar_newmark_1st(self, dt):
+        return 1./(self.gamma*dt)
+    def get_factor_deriv_dvar_newmark_2nd(self, dt):
+        return self.gamma/(self.beta*dt)
+    def get_factor_deriv_d2var_newmark(self, dt):
+        return 1./(self.beta*dt*dt)
+    def get_factor_deriv_varint_ost(self, dt):
+        return self.theta_ost*dt
+    def get_factor_deriv_varint_newmark_1st(self, dt):
+        return self.gamma*dt
 
     # zero
     def zero(self, t):
         return 0.0
 
     def timecurves(self, cnum):
 
@@ -353,25 +332,20 @@
         try: self.incompressible_2field = fem_params['incompressible_2field']
         except: self.incompressible_2field = False
 
 
     def set_acc_vel(self, u, u_old, v_old, a_old):
 
         # set forms for acc and vel
-        if self.timint == 'genalpha':
-            acc = self.update_d2var_newmark(u, u_old, v_old, a_old, ufl=True)
-            vel = self.update_dvar_newmark_2nd(u, u_old, v_old, a_old, ufl=True)
-        elif self.timint == 'ost':
-            acc = self.update_d2var_ost(u, u_old, v_old, a_old, ufl=True)
-            vel = self.update_dvar_ost(u, u_old, v_old, a_old, ufl=True)
-        elif self.timint == 'static':
+        if self.timint == 'static':
             acc = ufl.constantvalue.zero(self.dim)
             vel = ufl.constantvalue.zero(self.dim)
         else:
-            raise NameError("Unknown time-integration algorithm for solid mechanics!")
+            acc = self.update_d2var(u, u_old, v_old, a_old, self.dt, uflform=True)
+            vel = self.update_dvar(u, u_old, v_old, a_old, self.dt, uflform=True)
 
         return acc, vel
 
 
     def timefactors(self):
 
         if self.timint=='genalpha': timefac_m, timefac = 1.-self.alpha_m, 1.-self.alpha_f
@@ -380,18 +354,15 @@
 
         return timefac_m, timefac
 
 
     def update_timestep(self, u, u_old, v, v_old, a, a_old, p, p_old, internalvars, internalvars_old):
 
         # now update old kinematic fields with new quantities
-        if self.timint == 'genalpha':
-            self.update_fields_newmark(u, u_old, v, v_old, a, a_old)
-        if self.timint == 'ost':
-            self.update_fields_ost(u, u_old, v, v_old, a, a_old)
+        self.update_fields(u, u_old, v, v_old, a, a_old)
 
         # update pressure variable
         if self.incompressible_2field:
             p_old.vector.axpby(1.0, 0.0, p.vector)
             p_old.vector.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
 
         # update internal variables (e.g. active stress, growth stretch, plastic strains, ...)
@@ -399,30 +370,45 @@
             list(internalvars_old.values())[i].vector.axpby(1.0, 0.0, list(internalvars.values())[i].vector)
             list(internalvars_old.values())[i].vector.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
 
         # update old time-dependent load curves
         self.update_time_funcs_old()
 
 
-    def update_fields_newmark(self, u, u_old, v, v_old, a, a_old):
+    def update_fields(self, u, u_old, v, v_old, a, a_old):
 
         # use update functions using vector arguments
-        self.update_d2var_newmark(u.vector, u_old.vector, v_old.vector, a_old.vector, d2varout=a.vector, ufl=False)
-        self.update_dvar_newmark_2nd(u.vector, u_old.vector, v_old.vector, a_old.vector, dvarout=v.vector, ufl=False)
+        self.update_d2var(u.vector, u_old.vector, v_old.vector, a_old.vector, self.dt, d2varout=a.vector, uflform=False)
+        self.update_dvar(u.vector, u_old.vector, v_old.vector, a_old.vector, self.dt, dvarout=v.vector, uflform=False)
 
         self.update_a_v_u_old(a_old, v_old, u_old, a, v, u)
 
 
-    def update_fields_ost(self, u, u_old, v, v_old, a, a_old):
+    def update_dvar(self, var, var_old, dvar_old, d2var_old, dt, dvarout=None, uflform=True):
 
-        # use update functions using vector arguments
-        self.update_d2var_ost(u.vector, u_old.vector, v_old.vector, a_old.vector, d2varout=a.vector, ufl=False)
-        self.update_dvar_ost(u.vector, u_old.vector, v_old.vector, dvarout=v.vector, ufl=False)
+        if self.timint == 'genalpha':
+            return self.update_dvar_newmark_2nd(var, var_old, dvar_old, d2var_old, dt, dvarout=dvarout, uflform=uflform)
+        elif self.timint == 'ost':
+            return self.update_dvar_ost(var, var_old, dvar_old, dt, dvarout=dvarout, uflform=uflform)
+        elif self.timint == 'static':
+            pass
+        else:
+            raise NameError("Unknown time-integration algorithm for solid mechanics!")
 
-        self.update_a_v_u_old(a_old, v_old, u_old, a, v, u)
+
+    def update_d2var(self, var, var_old, dvar_old, d2var_old, dt, d2varout=None, uflform=True):
+
+        if self.timint == 'genalpha':
+            return self.update_d2var_newmark(var, var_old, dvar_old, d2var_old, dt, d2varout=d2varout, uflform=uflform)
+        elif self.timint == 'ost':
+            return self.update_d2var_ost(var, var_old, dvar_old, d2var_old, dt, d2varout=d2varout, uflform=uflform)
+        elif self.timint == 'static':
+            pass
+        else:
+            raise NameError("Unknown time-integration algorithm for solid mechanics!")
 
 
     def update_a_v_u_old(self, a_old, v_old, u_old, a, v, u):
 
         # update acceleration: a_old <- a
         a_old.vector.axpby(1.0, 0.0, a.vector)
         a_old.vector.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
@@ -442,14 +428,36 @@
         alpha_f = rho_inf/(rho_inf+1.)
         beta    = 0.25*(1.-alpha_m+alpha_f)**2.
         gamma   = 0.5-alpha_m+alpha_f
 
         return alpha_m, alpha_f, beta, gamma
 
 
+    def get_factor_deriv_dvar(self, dt):
+        if self.timint == 'genalpha':
+            return self.get_factor_deriv_dvar_newmark_2nd(dt)
+        elif self.timint == 'ost':
+            return self.get_factor_deriv_dvar_ost(dt)
+        else:
+            raise NameError("Unknown time-integration algorithm for solid mechanics!")
+
+
+    def get_factor_deriv_d2var(self, dt):
+        if self.timint == 'genalpha':
+            return self.get_factor_deriv_d2var_newmark(dt)
+        elif self.timint == 'ost':
+            return self.get_factor_deriv_d2var_ost(dt)
+        else:
+            raise NameError("Unknown time-integration algorithm for solid mechanics!")
+
+
+    def get_factor_deriv_varint(self, dt):
+        raise RuntimeError("Why are you requesting this value?!")
+
+
 
 # Fluid mechanics time integration class
 class timeintegration_fluid(timeintegration):
 
     def __init__(self, time_params, dt, Nmax, fem_params, time_curves=None, t_init=0., dim=3, comm=None):
         timeintegration.__init__(self, time_params, dt, Nmax, time_curves=time_curves, t_init=t_init, dim=dim, comm=comm)
 
@@ -468,34 +476,24 @@
                 self.alpha_m = time_params['alpha_m']
                 self.alpha_f = time_params['alpha_f']
                 self.gamma = time_params['gamma']
 
 
     def set_acc(self, v, v_old, a_old):
 
-        # set forms for acc and vel
-        if self.timint == 'ost':
-            acc = self.update_dvar_ost(v, v_old, a_old, ufl=True)
-        elif self.timint == 'genalpha':
-            acc = self.update_dvar_newmark_1st(v, v_old, a_old, ufl=True)
-        else:
-            raise NameError("Unknown time-integration algorithm for fluid mechanics!")
+        # set form for acceleration
+        acc = self.update_dvar(v, v_old, a_old, self.dt, uflform=True)
 
         return acc
 
 
     def set_uf(self, v, v_old, uf_old):
 
-        # set forms for acc and vel
-        if self.timint == 'ost':
-            uf = self.update_varint_ost(v, v_old, uf_old, ufl=True)
-        elif self.timint == 'genalpha':
-            uf = self.update_varint_newmark_1st(v, v_old, uf_old, ufl=True)
-        else:
-            raise NameError("Unknown time-integration algorithm for fluid mechanics!")
+        # set form for fluid displacement
+        uf = self.update_varint(v, v_old, uf_old, self.dt, uflform=True)
 
         return uf
 
 
     def timefactors(self):
 
         if self.timint=='ost':      timefac_m, timefac = self.theta_ost, self.theta_ost
@@ -503,18 +501,15 @@
 
         return timefac_m, timefac
 
 
     def update_timestep(self, v, v_old, a, a_old, p, p_old, internalvars, internalvars_old, uf=None, uf_old=None):
 
         # update old fields with new quantities
-        if self.timint == 'ost':
-            self.update_fields_ost(v, v_old, a, a_old, uf=uf, uf_old=uf_old)
-        if self.timint == 'genalpha':
-            self.update_fields_genalpha(v, v_old, a, a_old, uf=uf, uf_old=uf_old)
+        self.update_fields(v, v_old, a, a_old, uf=uf, uf_old=uf_old)
 
         # update pressure variable
         p_old.vector.axpby(1.0, 0.0, p.vector)
         # for duplicate p-nodes, our combined (nested) pressure is not ghosted, but the subvecs
         try:
             p_old.vector.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
         except:
@@ -526,38 +521,45 @@
             list(internalvars_old.values())[i].vector.axpby(1.0, 0.0, list(internalvars.values())[i].vector)
             list(internalvars_old.values())[i].vector.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
 
         # update old time-dependent load curves
         self.update_time_funcs_old()
 
 
-    def update_fields_ost(self, v, v_old, a, a_old, uf=None, uf_old=None):
+    def update_fields(self, v, v_old, a, a_old, uf=None, uf_old=None):
 
         # use update functions using vector arguments
-        self.update_dvar_ost(v.vector, v_old.vector, a_old.vector, dvarout=a.vector, ufl=False)
+        self.update_dvar(v.vector, v_old.vector, a_old.vector, self.dt, dvarout=a.vector, uflform=False)
 
         if uf_old is not None:
 
             # use update functions using vector arguments
-            self.update_varint_ost(v.vector, v_old.vector, uf_old.vector, varintout=uf.vector, ufl=False)
+            self.update_varint(v.vector, v_old.vector, uf_old.vector, self.dt, varintout=uf.vector, uflform=False)
 
         self.update_a_v_old(a_old, v_old, a, v, uf_old=uf_old, uf=uf)
 
 
-    def update_fields_genalpha(self, v, v_old, a, a_old, uf=None, uf_old=None):
+    def update_dvar(self, var, var_old, dvar_old, dt, dvarout=None, uflform=True):
 
-        # use update functions using vector arguments
-        self.update_dvar_newmark_1st(v.vector, v_old.vector, a_old.vector, dvarout=a.vector, ufl=False)
+        if self.timint == 'ost':
+            return self.update_dvar_ost(var, var_old, dvar_old, dt, dvarout=dvarout, uflform=uflform)
+        elif self.timint == 'genalpha':
+            return self.update_dvar_newmark_1st(var, var_old, dvar_old, dt, dvarout=dvarout, uflform=uflform)
+        else:
+            raise NameError("Unknown time-integration algorithm for fluid mechanics!")
 
-        if uf_old is not None:
 
-            # use update functions using vector arguments
-            self.update_varint_newmark_1st(v.vector, v_old.vector, uf_old.vector, varintout=uf.vector, ufl=False)
+    def update_varint(self, var, var_old, varint_old, dt, varintout=None, uflform=True):
 
-        self.update_a_v_old(a_old, v_old, a, v, uf_old=uf_old, uf=uf)
+        if self.timint == 'ost':
+            return self.update_varint_ost(var, var_old, varint_old, dt, varintout=varintout, uflform=uflform)
+        elif self.timint == 'genalpha':
+            return self.update_varint_newmark_1st(var, var_old, varint_old, dt, varintout=varintout, uflform=uflform)
+        else:
+            raise NameError("Unknown time-integration algorithm for fluid mechanics!")
 
 
     def update_a_v_old(self, a_old, v_old, a, v, uf_old=None, uf=None):
         # update acceleration: a_old <- a
         a_old.vector.axpby(1.0, 0.0, a.vector)
         a_old.vector.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
 
@@ -578,53 +580,60 @@
         alpha_m = 0.5*(3.-rho_inf)/(1.+rho_inf)
         alpha_f = 1./(1.+rho_inf)
         gamma   = 0.5+alpha_m-alpha_f
 
         return alpha_m, alpha_f, gamma
 
 
+    def get_factor_deriv_dvar(self, dt):
+        if self.timint == 'genalpha':
+            return self.get_factor_deriv_dvar_newmark_1st(dt)
+        elif self.timint == 'ost':
+            return self.get_factor_deriv_dvar_ost(dt)
+        else:
+            raise NameError("Unknown time-integration algorithm for fluid mechanics!")
+
+
+    def get_factor_deriv_d2var(self, dt):
+        raise RuntimeError("Why are you requesting this value?!")
+
+
+    def get_factor_deriv_varint(self, dt):
+        if self.timint == 'genalpha':
+            return self.get_factor_deriv_varint_newmark_1st(dt)
+        elif self.timint == 'ost':
+            return self.get_factor_deriv_varint_ost(dt)
+        else:
+            raise NameError("Unknown time-integration algorithm for fluid mechanics!")
+
+
+
 # ALE time integration class
 class timeintegration_ale(timeintegration_fluid):
 
     def update_timestep(self, d, d_old, w, w_old):
 
         # update old fields with new quantities
-        if self.timint == 'ost':
-            self.update_fields_ost(d, d_old, w, w_old)
-        if self.timint == 'genalpha':
-            self.update_fields_genalpha(d, d_old, w, w_old)
+        self.update_fields(d, d_old, w, w_old)
 
         # no old time-dependent load curves to update - ALE is quasi-static
 
 
     def set_wel(self, d, d_old, w_old):
 
         # set form for domain velocity wel
-        if self.timint == 'ost':
-            wel = self.update_dvar_ost(d, d_old, w_old, ufl=True)
-        elif self.timint == 'genalpha':
-            wel = self.update_dvar_newmark_1st(d, d_old, w_old, ufl=True)
-        else:
-            raise NameError("Unknown time scheme for ALE mechanics!")
+        wel = self.update_dvar(d, d_old, w_old, self.dt, uflform=True)
 
         return wel
 
 
-    def update_fields_ost(self, d, d_old, w, w_old):
-
-        # use update functions using vector arguments
-        self.update_dvar_ost(d.vector, d_old.vector, w_old.vector, dvarout=w.vector, ufl=False)
-
-        self.update_w_d_old(w_old, d_old, w, d)
-
-
-    def update_fields_genalpha(self, d, d_old, w, w_old, uf=None, uf_old=None):
+    def update_fields(self, d, d_old, w, w_old):
 
         # use update functions using vector arguments
-        self.update_dvar_newmark_1st(d.vector, d_old.vector, w_old.vector, dvarout=w.vector, ufl=False)
+        self.update_dvar(d.vector, d_old.vector, w_old.vector, self.dt, dvarout=w.vector, uflform=False)
 
         self.update_w_d_old(w_old, d_old, w, d)
 
 
     def update_w_d_old(self, w_old, d_old, w, d):
         # update ALE velocity: w_old <- w
         w_old.vector.axpby(1.0, 0.0, w.vector)
@@ -633,41 +642,41 @@
         # update ALE displacement: d_old <- d
         d_old.vector.axpby(1.0, 0.0, d.vector)
         d_old.vector.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
 
 
 
 # Electrophysiology time integration class
-class timeintegration_electrophysiology(timeintegration):
+class timeintegration_electrophysiology(timeintegration_fluid):
 
     def __init__(self, time_params, dt, Nmax, fem_params, time_curves=None, t_init=0., dim=3, comm=None):
         timeintegration.__init__(self, time_params, dt, Nmax, time_curves=time_curves, t_init=t_init, dim=dim, comm=comm)
 
         assert(self.timint == 'ost')
         self.theta_ost = time_params['theta_ost']
 
 
     def update_timestep(self, phi, phi_old, phidot, phidot_old):
 
         # update old fields with new quantities
-        self.update_fields_ost(phi, phi_old, phidot, phidot_old)
+        self.update_fields(phi, phi_old, phidot, phidot_old)
 
         # update old time-dependent load curves
         self.update_time_funcs_old()
 
 
     def set_phidot(self, phi, phi_old, phidot_old):
 
-        return self.update_dvar_ost(phi, phi_old, phidot_old, ufl=True)
+        return self.update_dvar(phi, phi_old, phidot_old, self.dt, uflform=True)
 
 
-    def update_fields_ost(self, phi, phi_old, phidot, phidot_old):
+    def update_fields(self, phi, phi_old, phidot, phidot_old):
 
         # use update functions using vector arguments
-        self.update_dvar_ost(phi.vector, phi_old.vector, phidot_old.vector, dvarout=phidot.vector, ufl=False)
+        self.update_dvar(phi.vector, phi_old.vector, phidot_old.vector, self.dt, dvarout=phidot.vector, uflform=False)
 
         self.update_phidot_phi_old(phidot_old, phi_old, phidot, phi)
 
 
     def update_phidot_phi_old(self, w_old, d_old, w, d):
         # update time derivative of potential: phidot_old <- phidot
         phidot_old.vector.axpby(1.0, 0.0, phidot.vector)
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe/utilities.py` & `ambit_fe-1.2.6/src/ambit_fe/utilities.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe/variationalform.py` & `ambit_fe-1.2.6/src/ambit_fe/variationalform.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/src/ambit_fe.egg-info/PKG-INFO` & `ambit_fe-1.2.6/src/ambit_fe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ambit-fe
-Version: 1.2.5
+Version: 1.2.6
 Summary: A FEniCS-based cardiovascular multi-physics solver
-Author-email: Marc Hirschvogel <marc.hirschvogel@deepambit.com>
+Author-email: Marc Hirschvogel <marc.hirschvogel@ambit.net>
 License: MIT License
         
         Copyright (c) 2024 Marc Hirschvogel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `ambit-fe-1.2.5/src/ambit_fe.egg-info/SOURCES.txt` & `ambit_fe-1.2.6/src/ambit_fe.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,16 @@
 tests/test_fluid_flow0d_monolagr_taylorhood_cylinder.py
 tests/test_fluid_p1p1_stab_cylinder.py
 tests/test_fluid_p1p1_stab_cylinder_schur2x2.py
 tests/test_fluid_p1p1_stab_cylinder_valve.py
 tests/test_fluid_taylorhood_cylinder.py
 tests/test_frsi_artseg_modepartitionunity.py
 tests/test_frsi_artseg_prefile.py
+tests/test_frsi_artseg_prefile_bgsschur4x4.py
 tests/test_frsi_artseg_prefile_partitioned_schur3x3.py
-tests/test_frsi_artseg_prefile_schurbgs4x4.py
 tests/test_frsi_artseg_prestress.py
 tests/test_fsi_flow0d_p1p1_stab_artseg.py
 tests/test_fsi_p1p1_stab_artseg.py
 tests/test_fsi_taylorhood_artseg.py
 tests/test_signet_0d_hypertrophy.py
 tests/test_solid_2d_pres.py
 tests/test_solid_2dheart_frankstarling.py
@@ -105,15 +105,15 @@
 tests/test_solid_constraint_volume_chamber.py
 tests/test_solid_divcont_ptc.py
 tests/test_solid_flow0d_monodir2field_4elwindkesselLpZ_chamber.py
 tests/test_solid_flow0d_monodir2field_flux_syspulcap_3Dheart_schur3x3.py
 tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber.py
 tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber_bgs2x2.py
 tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber_bgs2x2fieldsplit.py
-tests/test_solid_flow0d_monodir_flux_syspulcap_3Dheart_simple2x2.py
+tests/test_solid_flow0d_monodir_flux_syspulcap_3Dheart_schur2x2.py
 tests/test_solid_flow0d_monodir_syspul_2dheart_prestress.py
 tests/test_solid_flow0d_monodir_syspulcor_2dheart_rom.py
 tests/test_solid_flow0d_monolagr2field_2elwindkessel_chamber.py
 tests/test_solid_flow0d_monolagr_CRLinoutlink_chambers.py
 tests/test_solid_flow0d_multiscalegrowthremodeling_concentric.py
 tests/test_solid_flow0d_multiscalegrowthremodeling_eccentric.py
 tests/test_solid_flow0d_periodicref_syspul_lvchamber.py
```

### Comparing `ambit-fe-1.2.5/tests/test_ale_linelast.py` & `ambit_fe-1.2.6/tests/test_ale_linelast.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_electrophysiology.py` & `ambit_fe-1.2.6/tests/test_electrophysiology.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_flow0d_0dheart_syspul.py` & `ambit_fe-1.2.6/tests/test_flow0d_0dheart_syspul.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_flow0d_0dheart_syspulcap.py` & `ambit_fe-1.2.6/tests/test_flow0d_0dheart_syspulcap.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_flow0d_0dheart_syspulcapcor.py` & `ambit_fe-1.2.6/tests/test_flow0d_0dheart_syspulcapcor.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_flow0d_0dheart_syspulcaprespir_periodic.py` & `ambit_fe-1.2.6/tests/test_flow0d_0dheart_syspulcaprespir_periodic.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_flow0d_0dheart_syspulcor.py` & `ambit_fe-1.2.6/tests/test_flow0d_0dheart_syspulcor.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_flow0d_0dheart_syspulcorvad.py` & `ambit_fe-1.2.6/tests/test_flow0d_0dheart_syspulcorvad.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_flow0d_0dvol_4elwindkesselLpZ.py` & `ambit_fe-1.2.6/tests/test_flow0d_0dvol_4elwindkesselLpZ.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_flow0d_0dvol_4elwindkesselLsZ.py` & `ambit_fe-1.2.6/tests/test_flow0d_0dvol_4elwindkesselLsZ.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_fluid_ale_flow0d_lalv_syspul_prescribed.py` & `ambit_fe-1.2.6/tests/test_fluid_ale_flow0d_lalv_syspul_prescribed.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                             'catch_max_res_value'   : 1e12}
 
     TIME_PARAMS          = {'maxtime'               : 1.0,
                             'numstep'               : 1000,
                             'numstep_stop'          : 2,
                             'timint'                : 'ost',
                             'theta_ost'             : 1.0,
-                            'residual_scale'        : [0.001,0.001,0.001]}
+                            'residual_scale'        : [0.001,0.001,0.001,0.001]}
 
     TIME_PARAMS_FLOW0D   = {'timint'                : 'ost',
                             'theta_ost'             : 0.5,
                             'initial_backwardeuler' : True,
                             'initial_conditions'    : init()}
 
     MODEL_PARAMS_FLOW0D  = {'modeltype'             : 'syspul',
@@ -72,15 +72,15 @@
                                                        'pv' : ['pwlin_pres'],
                                                        'tv' : ['pwlin_pres']},
                             'prescribed_variables'  : {'q_vin_l' : {'flux_monitor' : 0}}}
 
     FEM_PARAMS_FLUID     = {'order_vel'             : 1,
                             'order_pres'            : 1,
                             'quad_degree'           : 5,
-                            'stabilization'         : {'scheme' : 'supg_pspg2', 'vscale' : 1e3, 'dscales' : [1.,1.,1.], 'symmetric' : True} }
+                            'stabilization'         : {'scheme' : 'supg_pspg', 'vscale' : 1e3, 'dscales' : [1.,1.,1.], 'symmetric' : True, 'reduced_scheme' : True} }
 
     FEM_PARAMS_ALE       = {'order_disp'            : 1,
                             'quad_degree'           : 5}
 
     COUPLING_PARAMS_ALE_FLUID = {'coupling_ale_fluid' : [{'surface_ids' : [1], 'type' : 'strong_dirichlet'}]} # strong_dirichlet, weak_dirichlet
 
     COUPLING_PARAMS_FLUID_FLOW0D = {'surface_ids'   : [[5],[6],[7],[8], [4]],
@@ -114,15 +114,15 @@
 
 
     BC_DICT_ALE          = { 'dirichlet_vol' : [{'id' : [1,2], 'file' : basepath+'/input/aledisp_lalv_prescr-*.txt'}] }
 
     BC_DICT_FLUID        = { 'robin_valve' : [{'id' : [3], 'type' : 'temporal', 'beta_max' : 1e3, 'beta_min' : 0, 'to' : 0.0, 'tc' : 0.37}], # MV
                              'dp_monitor' : [{'id' : [3], 'upstream_domain' : 2, 'downstream_domain' : 1}], # MV
                              'flux_monitor' : [{'id' : [3], 'on_subdomain' : True, 'domain' : 2}],  # MV
-                             'stabilized_neumann' : [{'id' : [5,6,7,8, 4], 'par1' : 0.205e-6, 'par2' : 1.}] } # par1 should be ~ 0.2*rho
+                             'stabilized_neumann_mod' : [{'id' : [5,6,7,8, 4], 'beta' : 0.205e-6, 'gamma' : 1.}] } # beta should be ~ 0.2*rho
 
 
     # problem setup
     problem = ambit_fe.ambit_main.Ambit(IO_PARAMS, [TIME_PARAMS, TIME_PARAMS_FLOW0D], SOLVER_PARAMS, [FEM_PARAMS_FLUID, FEM_PARAMS_ALE], [MATERIALS_FLUID, MATERIALS_ALE, MODEL_PARAMS_FLOW0D], [BC_DICT_FLUID, BC_DICT_ALE], time_curves=time_curves(), coupling_params=[COUPLING_PARAMS_ALE_FLUID,COUPLING_PARAMS_FLUID_FLOW0D])
 
 
     # problem solve
```

### Comparing `ambit-fe-1.2.5/tests/test_fluid_flow0d_monolagr_taylorhood_cylinder.py` & `ambit_fe-1.2.6/tests/test_fluid_flow0d_monolagr_taylorhood_cylinder.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_fluid_p1p1_stab_cylinder.py` & `ambit_fe-1.2.6/tests/test_fluid_p1p1_stab_cylinder.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                            'theta_ost'             : 1.0,
                            'fluid_governing_type'  : 'navierstokes_steady'}
     
     FEM_PARAMS          = {'order_vel'             : 1,
                            'order_pres'            : 1,
                            'quad_degree'           : 5,
                            'fluid_formulation'     : 'nonconservative', # nonconservative (default), conservative
-                           'stabilization'         : {'scheme' : 'supg_pspg2', 'vscale' : 1e3, 'dscales' : [1.,1.,1.]}}
+                           'stabilization'         : {'scheme' : 'supg_pspg', 'vscale' : 1e3, 'dscales' : [1.,1.,1.], 'reduced_scheme' : True}}
 
 
     MATERIALS           = { 'MAT1' : {'newtonian' : {'mu' : 4.0e-6},
                                       'inertia' : {'rho' : 1.025e-6}},
                             'MAT2' : {'newtonian' : {'mu' : 4.0e-6},
                                       'inertia' : {'rho' : 1.025e-6}} }
```

### Comparing `ambit-fe-1.2.5/tests/test_fluid_p1p1_stab_cylinder_schur2x2.py` & `ambit_fe-1.2.6/tests/test_fluid_p1p1_stab_cylinder_schur2x2.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                            'theta_ost'             : 1.0,
                            'fluid_governing_type'  : 'navierstokes_steady'}
     
     FEM_PARAMS          = {'order_vel'             : 1,
                            'order_pres'            : 1,
                            'quad_degree'           : 5,
                            'fluid_formulation'     : 'nonconservative', # nonconservative (default), conservative
-                           'stabilization'         : {'scheme' : 'supg_pspg2', 'vscale' : 1e3, 'dscales' : [1.,1.,1.]}}
+                           'stabilization'         : {'scheme' : 'supg_pspg', 'vscale' : 1e3, 'dscales' : [1.,1.,1.]}}
 
 
     MATERIALS           = { 'MAT1' : {'newtonian' : {'mu' : 4.0e-6},
                                       'inertia' : {'rho' : 1.025e-6}},
                             'MAT2' : {'newtonian' : {'mu' : 4.0e-6},
                                       'inertia' : {'rho' : 1.025e-6}} }
```

### Comparing `ambit-fe-1.2.5/tests/test_fluid_p1p1_stab_cylinder_valve.py` & `ambit_fe-1.2.6/tests/test_fluid_p1p1_stab_cylinder_valve.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 transient incompressible Navier-Stokes flow in a cylinder with axial Neumann and two outflows
 - stabilized P1P1 elements for velocity and pressure (full SUPF/PSPG scheme)
 - Backward-Euler time stepping scheme
 - 2 material domains in fluid (w/ same parameters though)
 - internal valve, requiring duplicate pressure nodes at that internal surface
 - works currently only with mixed dolfinx branch (USE_MIXED_DOLFINX_BRANCH)
 - checkpoint writing of domain-wise discontinuous pressure field
+- DBC read-in from file
 """
 
 import ambit_fe
 
 import sys
 import numpy as np
 from pathlib import Path
@@ -73,15 +74,15 @@
             return 0.5*(-(pmax))*(1.-np.cos(np.pi*t/t_ramp))
 
         def tc2(self, t):
             pmax = 0.5
             return -pmax
 
 
-    BC_DICT        = { 'dirichlet'   : [{'id' : [1], 'dir' : 'all', 'val' : 0.}],
+    BC_DICT        = { 'dirichlet'   : [{'id' : [1], 'dir' : 'all', 'file' : basepath+'/input/cylinder_dbc0.txt'}], # read-in from file - equivalent to setting 'val':0.0
                        'neumann'     : [{'id' : [2], 'dir' : 'normal_ref', 'curve' : 1},
                                         {'id' : [4], 'dir' : 'normal_ref', 'curve' : 2}],
                        'robin_valve' : [{'id' : [5], 'type' : 'dp_smooth', 'beta_max' : 1e3, 'beta_min' : 1e-3, 'epsilon' : 1e-6, 'dp_monitor_id' : 0}], # 5 is internal surface (valve)
                        'dp_monitor'  : [{'id' : [5], 'upstream_domain' : 2, 'downstream_domain' : 1}], 
                        'flux_monitor': [{'id' : [5], 'on_subdomain' : True, 'internal' : False, 'domain' : 2}] }
```

### Comparing `ambit-fe-1.2.5/tests/test_fluid_taylorhood_cylinder.py` & `ambit_fe-1.2.6/tests/test_fluid_taylorhood_cylinder.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_frsi_artseg_modepartitionunity.py` & `ambit_fe-1.2.6/tests/test_frsi_artseg_modepartitionunity.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,17 @@
                             'partitions'            : [basepath+'/input/artseg_part-1.txt',basepath+'/input/artseg_part-2.txt',basepath+'/input/artseg_part-3.txt'],
                             'numsnapshots'          : 1,
                             'snapshotincr'          : 1,
                             'numredbasisvec'        : 1,
                             'eigenvalue_cutoff'     : 1.0e-8,
                             'print_eigenproblem'    : True,
                             'surface_rom'           : [1,6],
-                            'redbasisvec_penalties' : [0.0, 0.0, 0.0]} # only for code coverage test - applying zero terms
+                            'regularizations'       : [0.0, 0.0, 10.0], # add regularization to the mode at the junction in the middle (last one) ("dashpot-like")
+                            'regularizations_integ' : [0.0, 0.0, 0.0],  # regularization on integral of reduced variable (here 0) ("spring-like")
+                            'regularizations_deriv' : [0.0, 0.0, 0.0]}  # regularization on derivative of reduced variable (here 0) ("mass-like")
 
     SOLVER_PARAMS        = {'solve_type'            : 'direct',
                             'tol_res'               : [1.0e-8,1.0e-8,1.0e-8],
                             'tol_inc'               : [1.0e-8,1.0e-8,1.0e-8]}
 
     TIME_PARAMS          = {'maxtime'               : 3.0,
                             'numstep'               : 150,
@@ -107,16 +109,16 @@
 
     check_node = []
     check_node.append(np.array([7.071068, 7.071068, 2.500000]))
 
     v_corr = np.zeros(3*len(check_node))
 
     # correct results
-    v_corr[0] = 2.3582758194714750E+00 # x
-    v_corr[1] = 2.3582758194714755E+00 # y
+    v_corr[0] = -2.0812855650931343E+00 # x
+    v_corr[1] = -2.0812855650931343E+00 # y
     v_corr[2] = 0.0 # z
 
     check1 = ambit_fe.resultcheck.results_check_node(problem.mp.pbf.v, check_node, v_corr, problem.mp.pbf.V_v, problem.mp.comm, tol=tol, nm='v', readtol=1e-4)
 
     success = ambit_fe.resultcheck.success_check([check1], problem.mp.comm)
 
     if not success:
```

### Comparing `ambit-fe-1.2.5/tests/test_frsi_artseg_prefile.py` & `ambit_fe-1.2.6/tests/test_frsi_artseg_prefile.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_frsi_artseg_prefile_partitioned_schur3x3.py` & `ambit_fe-1.2.6/tests/test_frsi_artseg_prefile_partitioned_schur3x3.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_frsi_artseg_prefile_schurbgs4x4.py` & `ambit_fe-1.2.6/tests/test_frsi_artseg_prefile_bgsschur4x4.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 """
 FrSI test case of an axially clamped, prestressed arterial segment
-- iterative schurbgs4x4 solution
+- iterative bgsschur4x4simple solution
 """
 
 import ambit_fe
 
 import sys
 import numpy as np
 from pathlib import Path
@@ -22,31 +22,31 @@
 
     IO_PARAMS            = {'problem_type'          : 'fluid_ale',
                             'write_results_every'   : -1,
                             'output_path'           : basepath+'/tmp/',
                             'mesh_domain'           : basepath+'/input/artseg-quad_domain.xdmf',
                             'mesh_boundary'         : basepath+'/input/artseg-quad_boundary.xdmf',
                             'results_to_write'      : [['fluiddisplacement','velocity','pressure'],['aledisplacement','alevelocity'],'counters'], # first fluid, then ale results
-                            'simname'               : 'frsi_artseg_prefile_iterative'}
+                            'simname'               : 'frsi_artseg_prefile_bgsschur4x4'}
 
     ROM_PARAMS           = {'hdmfilenames'          : [basepath+'/input/artseg_vel_snapshot-*.txt'],
                             'numsnapshots'          : 1,
                             'snapshotincr'          : 1,
                             'numredbasisvec'        : 1,
                             'eigenvalue_cutoff'     : 1.0e-8,
                             'print_eigenproblem'    : True,
                             'surface_rom'           : [1,6]}
 
     SOLVER_PARAMS        = {'solve_type'            : 'iterative',
                             'iterative_solver'      : 'gmres',
-                            'block_precond'         : 'schurbgs4x4',
-                            'precond_fields'        : [{'prec':'amg'},    # fluid-v
-                                                       {'prec':'amg'},    # fluid-p (Schur)
-                                                       {'prec':'direct'}, # fluid-red.v
-                                                       {'prec':'amg'}],   # ale-d
+                            'block_precond'         : 'bgsschur4x4simple', # can as well use bgsschur4x4 version - interestingly, the SIMPLE version yields fewer linear iterations!
+                            'precond_fields'        : [{'prec':'amg'},     # fluid-v
+                                                       {'prec':'amg'},     # fluid-p (Schur)
+                                                       {'prec':'direct'},  # fluid-red.v
+                                                       {'prec':'amg'}],    # ale-d
                             'tol_lin_rel'           : 1.0e-5,
                             'tol_lin_abs'           : 1.0e-30,
                             'lin_norm_type'         : 'preconditioned',
                             'max_liniter'           : 1200,
                             'res_lin_monitor'       : 'abs',
                             'print_liniter_every'   : 50,
                             'indexset_options'      : {'rom_to_new' : True},
```

### Comparing `ambit-fe-1.2.5/tests/test_frsi_artseg_prestress.py` & `ambit_fe-1.2.6/tests/test_frsi_artseg_prestress.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                             'fluid_governing_type'  : 'stokes_transient'}
 
     FEM_PARAMS_FLUID     = {'order_vel'             : 2,
                             'order_pres'            : 1,
                             'quad_degree'           : 6,
                             'fluid_formulation'     : 'conservative',
                             'prestress_initial'     : True,
-                            'prestress_kinetic'     : True,
+                            'prestress_kinetic'     : 'stokes_transient',
                             'prestress_maxtime'     : 1.0,
                             'prestress_numstep'     : 30}
 
     FEM_PARAMS_ALE       = {'order_disp'            : 2,
                             'quad_degree'           : 6}
 
     COUPLING_PARAMS      = {'coupling_fluid_ale'    : [{'surface_ids' : [1,6], 'type' : 'strong_dirichlet'}]}
@@ -106,16 +106,16 @@
 
     check_node = []
     check_node.append(np.array([7.071068, 7.071068, 2.500000]))
 
     v_corr = np.zeros(3*len(check_node))
 
     # correct results
-    v_corr[0] = -6.9221857227068683E-03 # x
-    v_corr[1] = -6.9221857227068691E-03 # y
+    v_corr[0] = -4.8182947123710648E-03 # x
+    v_corr[1] = -4.8182947123710657E-03 # y
     v_corr[2] = 0.0 # z
 
     check1 = ambit_fe.resultcheck.results_check_node(problem.mp.pbf.v, check_node, v_corr, problem.mp.pbf.V_v, problem.mp.comm, tol=tol, nm='v', readtol=1e-4)
 
     success = ambit_fe.resultcheck.success_check([check1], problem.mp.comm)
 
     if not success:
```

### Comparing `ambit-fe-1.2.5/tests/test_fsi_flow0d_p1p1_stab_artseg.py` & `ambit_fe-1.2.6/tests/test_fsi_flow0d_p1p1_stab_artseg.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                             'order_pres'            : 1,
                             'quad_degree'           : 5,
                             'incompressible_2field' : False}
 
     FEM_PARAMS_FLUID     = {'order_vel'             : 1,
                             'order_pres'            : 1,
                             'quad_degree'           : 5,
-                            'stabilization'         : {'scheme' : 'supg_pspg2', 'vscale' : 1e3, 'dscales' : [1.,1.,1.], 'symmetric' : True}}
+                            'stabilization'         : {'scheme' : 'supg_pspg', 'vscale' : 1e3, 'dscales' : [1.,1.,1.], 'symmetric' : True, 'reduced_scheme' : True}}
     
     FEM_PARAMS_ALE       = {'order_disp'            : 1,
                             'quad_degree'           : 5}
     
     COUPLING_PARAMS_ALE_FLUID = {'coupling_fluid_ale'    : [{'surface_ids' : [1], 'type' : 'strong_dirichlet'}],
                                  'fsi_governing_type'    : 'fluid_governed'} # solid_governed, fluid_governed
```

### Comparing `ambit-fe-1.2.5/tests/test_fsi_p1p1_stab_artseg.py` & `ambit_fe-1.2.6/tests/test_fsi_p1p1_stab_artseg.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                             'order_pres'            : 1,
                             'quad_degree'           : 5,
                             'incompressible_2field' : False}
 
     FEM_PARAMS_FLUID     = {'order_vel'             : 1,
                             'order_pres'            : 1,
                             'quad_degree'           : 5,
-                            'stabilization'         : {'scheme' : 'supg_pspg2', 'vscale' : 1e3, 'dscales' : [1.,1.,1.], 'symmetric' : True}}
+                            'stabilization'         : {'scheme' : 'supg_pspg', 'vscale' : 1e3, 'dscales' : [1.,1.,1.], 'symmetric' : True, 'reduced_scheme' : True}}
     
     FEM_PARAMS_ALE       = {'order_disp'            : 1,
                             'quad_degree'           : 5}
     
     COUPLING_PARAMS      = {'coupling_fluid_ale'    : [{'surface_ids' : [1], 'type' : 'strong_dirichlet'}],
                             'fsi_governing_type'    : 'solid_governed'} # solid_governed, fluid_governed
```

### Comparing `ambit-fe-1.2.5/tests/test_fsi_taylorhood_artseg.py` & `ambit_fe-1.2.6/tests/test_fsi_taylorhood_artseg.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_signet_0d_hypertrophy.py` & `ambit_fe-1.2.6/tests/test_signet_0d_hypertrophy.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_2d_pres.py` & `ambit_fe-1.2.6/tests/test_solid_2d_pres.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_2dheart_frankstarling.py` & `ambit_fe-1.2.6/tests/test_solid_2dheart_frankstarling.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_bodyforce_gravity.py` & `ambit_fe-1.2.6/tests/test_solid_bodyforce_gravity.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_constraint_volume_chamber.py` & `ambit_fe-1.2.6/tests/test_solid_constraint_volume_chamber.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_divcont_ptc.py` & `ambit_fe-1.2.6/tests/test_solid_divcont_ptc.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_flow0d_monodir2field_4elwindkesselLpZ_chamber.py` & `ambit_fe-1.2.6/tests/test_solid_flow0d_monodir2field_4elwindkesselLpZ_chamber.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_flow0d_monodir2field_flux_syspulcap_3Dheart_schur3x3.py` & `ambit_fe-1.2.6/tests/test_solid_flow0d_monodir2field_flux_syspulcap_3Dheart_schur3x3.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                             'output_path'           : basepath+'/tmp/',
                             'results_to_write'      : ['displacement','pressure'],
                             'simname'               : 'test',
                             'ode_parallel'          : True}
 
     SOLVER_PARAMS        = {'solve_type'            : 'iterative',
                             'iterative_solver'      : 'gmres',
-                            'block_precond'         : 'schur3x3',
+                            'block_precond'         : 'schur3x3simple', # can as well use schur3x3 version - interestingly, the SIMPLE version yields fewer linear iterations!
                             'precond_fields'        : [{'prec':'amg'}, {'prec':'amg'}, {'prec':'direct'}],
                             'tol_res'               : [1.0e-8,1.0e-8,1.0e-6], # u,p,0d
                             'tol_inc'               : [1.0e-8,1.0e-8,1.0e-6], # u,p,0d
                             'tol_lin_rel'           : 1.0e-9,
                             'lin_norm_type'         : 'preconditioned',
                             'print_liniter_every'   : 50,
                             'divergence_continue'   : None,
```

### Comparing `ambit-fe-1.2.5/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber.py` & `ambit_fe-1.2.6/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber_bgs2x2.py` & `ambit_fe-1.2.6/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber_bgs2x2.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber_bgs2x2fieldsplit.py` & `ambit_fe-1.2.6/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber_bgs2x2fieldsplit.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_flow0d_monodir_flux_syspulcap_3Dheart_simple2x2.py` & `ambit_fe-1.2.6/tests/test_solid_flow0d_monodir_flux_syspulcap_3Dheart_schur2x2.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                             'output_path'           : basepath+'/tmp/',
                             'results_to_write'      : ['displacement'],
                             'simname'               : 'test',
                             'ode_parallel'          : True}
 
     SOLVER_PARAMS        = {'solve_type'            : 'iterative',
                             'iterative_solver'      : 'gmres',
-                            'block_precond'         : 'simple2x2',
+                            'block_precond'         : 'schur2x2simple', # can as well use schur2x2 version - interestingly, the SIMPLE version yields fewer linear iterations!
                             'precond_fields'        : [{'prec':'amg'}, {'prec':'direct'}],
                             'tol_res'               : [1.0e-8,1.0e-6], # u,0d
                             'tol_inc'               : [1.0e-8,1.0e-6], # u,0d
                             'tol_lin_rel'           : 1.0e-9,
                             'lin_norm_type'         : 'preconditioned',
                             'print_liniter_every'   : 50,
                             'divergence_continue'   : None,
```

### Comparing `ambit-fe-1.2.5/tests/test_solid_flow0d_monodir_syspul_2dheart_prestress.py` & `ambit_fe-1.2.6/tests/test_solid_flow0d_monodir_syspul_2dheart_prestress.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_flow0d_monodir_syspulcor_2dheart_rom.py` & `ambit_fe-1.2.6/tests/test_solid_flow0d_monodir_syspulcor_2dheart_rom.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_flow0d_monolagr2field_2elwindkessel_chamber.py` & `ambit_fe-1.2.6/tests/test_solid_flow0d_monolagr2field_2elwindkessel_chamber.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_flow0d_monolagr_CRLinoutlink_chambers.py` & `ambit_fe-1.2.6/tests/test_solid_flow0d_monolagr_CRLinoutlink_chambers.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_flow0d_multiscalegrowthremodeling_concentric.py` & `ambit_fe-1.2.6/tests/test_solid_flow0d_multiscalegrowthremodeling_concentric.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_flow0d_multiscalegrowthremodeling_eccentric.py` & `ambit_fe-1.2.6/tests/test_solid_flow0d_multiscalegrowthremodeling_eccentric.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_flow0d_periodicref_syspul_lvchamber.py` & `ambit_fe-1.2.6/tests/test_solid_flow0d_periodicref_syspul_lvchamber.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_growth_prescribed_iso_lv.py` & `ambit_fe-1.2.6/tests/test_solid_growth_prescribed_iso_lv.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_growth_volstressmandel.py` & `ambit_fe-1.2.6/tests/test_solid_growth_volstressmandel.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_growth_volstressmandel_incomp.py` & `ambit_fe-1.2.6/tests/test_solid_growth_volstressmandel_incomp.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_growthremodeling_fiberstretch.py` & `ambit_fe-1.2.6/tests/test_solid_growthremodeling_fiberstretch.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_mat_uniax_hex_2field.py` & `ambit_fe-1.2.6/tests/test_solid_mat_uniax_hex_2field.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_membrane.py` & `ambit_fe-1.2.6/tests/test_solid_membrane.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_pinch_edge.py` & `ambit_fe-1.2.6/tests/test_solid_pinch_edge.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_plasticity_vonmises.py` & `ambit_fe-1.2.6/tests/test_solid_plasticity_vonmises.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_robin_genalpha.py` & `ambit_fe-1.2.6/tests/test_solid_robin_genalpha.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_robin_genalpha_amg.py` & `ambit_fe-1.2.6/tests/test_solid_robin_genalpha_amg.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_robin_static_prestress.py` & `ambit_fe-1.2.6/tests/test_solid_robin_static_prestress.py`

 * *Files identical despite different names*

### Comparing `ambit-fe-1.2.5/tests/test_solid_robin_visco.py` & `ambit_fe-1.2.6/tests/test_solid_robin_visco.py`

 * *Files identical despite different names*

