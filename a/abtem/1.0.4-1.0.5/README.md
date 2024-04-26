# Comparing `tmp/abtem-1.0.4.tar.gz` & `tmp/abtem-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abtem-1.0.4.tar", last modified: Mon Nov 20 14:28:23 2023, max compression
+gzip compressed data, was "abtem-1.0.5.tar", last modified: Fri Apr 26 16:41:21 2024, max compression
```

## Comparing `abtem-1.0.4.tar` & `abtem-1.0.5.tar`

### file list

```diff
@@ -1,120 +1,133 @@
-drwxrwxrwx   0        0        0        0 2023-11-20 14:28:23.022481 abtem-1.0.4/
--rw-rw-rw-   0        0        0    35823 2023-04-22 18:02:13.000000 abtem-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      144 2023-04-22 18:10:15.000000 abtem-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      841 2023-11-20 14:28:23.023481 abtem-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2958 2023-11-12 14:39:54.000000 abtem-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-11-20 14:28:22.952419 abtem-1.0.4/abtem/
--rw-rw-rw-   0        0        0     1168 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/__init__.py
--rw-rw-rw-   0        0        0       52 2023-11-20 14:26:11.000000 abtem-1.0.4/abtem/_version.py
--rw-rw-rw-   0        0        0     2469 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/antialias.py
--rw-rw-rw-   0        0        0    55179 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/array.py
--rw-rw-rw-   0        0        0    27592 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/atoms.py
-drwxrwxrwx   0        0        0        0 2023-11-20 14:28:22.974419 abtem-1.0.4/abtem/core/
--rw-rw-rw-   0        0        0      245 2023-04-22 18:10:15.000000 abtem-1.0.4/abtem/core/__init__.py
--rw-rw-rw-   0        0        0     5328 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/core/_cuda.py
--rw-rw-rw-   0        0        0      719 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/core/abtem.yaml
--rw-rw-rw-   0        0        0    12214 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/core/axes.py
--rw-rw-rw-   0        0        0     3057 2023-11-12 14:39:54.000000 abtem-1.0.4/abtem/core/backend.py
--rw-rw-rw-   0        0        0     6163 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/core/chunks.py
--rw-rw-rw-   0        0        0    32748 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/core/colors.py
--rw-rw-rw-   0        0        0     1156 2023-04-22 18:10:15.000000 abtem-1.0.4/abtem/core/complex.py
--rw-rw-rw-   0        0        0    11989 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/core/config.py
--rw-rw-rw-   0        0        0      321 2023-04-22 18:10:15.000000 abtem-1.0.4/abtem/core/constants.py
--rw-rw-rw-   0        0        0     8723 2023-04-22 18:10:15.000000 abtem-1.0.4/abtem/core/electron_configurations.py
--rw-rw-rw-   0        0        0     5401 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/core/energy.py
--rw-rw-rw-   0        0        0     7224 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/core/ensemble.py
--rw-rw-rw-   0        0        0    10649 2023-11-12 14:39:54.000000 abtem-1.0.4/abtem/core/fft.py
--rw-rw-rw-   0        0        0    14351 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/core/grid.py
--rw-rw-rw-   0        0        0     2434 2023-05-12 09:09:37.000000 abtem-1.0.4/abtem/core/units.py
--rw-rw-rw-   0        0        0     6212 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/core/utils.py
--rw-rw-rw-   0        0        0    29725 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/detectors.py
--rw-rw-rw-   0        0        0    15738 2023-11-12 14:39:54.000000 abtem-1.0.4/abtem/distributions.py
--rw-rw-rw-   0        0        0    10805 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/indexing.py
-drwxrwxrwx   0        0        0        0 2023-11-20 14:28:22.978423 abtem-1.0.4/abtem/inelastic/
--rw-rw-rw-   0        0        0        0 2023-04-22 18:10:15.000000 abtem-1.0.4/abtem/inelastic/__init__.py
--rw-rw-rw-   0        0        0    43408 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/inelastic/core_loss.py
--rw-rw-rw-   0        0        0    21444 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/inelastic/phonons.py
--rw-rw-rw-   0        0        0    18766 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/inelastic/plasmons.py
--rw-rw-rw-   0        0        0    28655 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/integrals.py
-drwxrwxrwx   0        0        0        0 2023-11-20 14:28:22.981426 abtem-1.0.4/abtem/magnetism/
--rw-rw-rw-   0        0        0        0 2023-04-22 18:10:15.000000 abtem-1.0.4/abtem/magnetism/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-20 14:28:22.982424 abtem-1.0.4/abtem/magnetism/data/
--rw-rw-rw-   0        0        0     4780 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/magnetism/data/lyon.json
--rw-rw-rw-   0        0        0    13013 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/magnetism/parametrization.py
--rw-rw-rw-   0        0        0     4437 2023-11-12 14:39:54.000000 abtem-1.0.4/abtem/magnetism/realspace_multislice.py
--rw-rw-rw-   0        0        0        0 2023-04-22 18:10:15.000000 abtem-1.0.4/abtem/magnetism/vector_potential.py
--rw-rw-rw-   0        0        0     7501 2023-04-22 18:10:15.000000 abtem-1.0.4/abtem/mcf.py
--rw-rw-rw-   0        0        0   134155 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/measurements.py
--rw-rw-rw-   0        0        0     2567 2023-04-22 18:10:15.000000 abtem-1.0.4/abtem/mtf.py
--rw-rw-rw-   0        0        0    25733 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/multislice.py
--rw-rw-rw-   0        0        0     3048 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/noise.py
-drwxrwxrwx   0        0        0        0 2023-11-20 14:28:22.983425 abtem-1.0.4/abtem/parametrizations/
--rw-rw-rw-   0        0        0    24071 2023-11-12 14:39:54.000000 abtem-1.0.4/abtem/parametrizations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-20 14:28:22.989424 abtem-1.0.4/abtem/parametrizations/data/
--rw-rw-rw-   0        0        0    31766 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/parametrizations/data/kirkland.json
--rw-rw-rw-   0        0        0    31360 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/parametrizations/data/lobato.json
--rw-rw-rw-   0        0        0    19124 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/parametrizations/data/peng_high.json
--rw-rw-rw-   0        0        0    19180 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/parametrizations/data/peng_ionic.json
--rw-rw-rw-   0        0        0    22039 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/parametrizations/data/peng_low.json
--rw-rw-rw-   0        0        0    39350 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/parametrizations/data/waasmaier_kirfel.json
-drwxrwxrwx   0        0        0        0 2023-11-20 14:28:22.993480 abtem-1.0.4/abtem/parametrizations/functions/
--rw-rw-rw-   0        0        0        0 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/parametrizations/functions/__init__.py
--rw-rw-rw-   0        0        0      590 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/parametrizations/functions/ewald.py
--rw-rw-rw-   0        0        0     2455 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/parametrizations/functions/kirkland.py
--rw-rw-rw-   0        0        0     4475 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/parametrizations/functions/lobato.py
--rw-rw-rw-   0        0        0      999 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/parametrizations/functions/peng.py
-drwxrwxrwx   0        0        0        0 2023-11-20 14:28:22.997480 abtem-1.0.4/abtem/potentials/
--rw-rw-rw-   0        0        0       52 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/potentials/__init__.py
--rw-rw-rw-   0        0        0     2902 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/potentials/_poisson.py
--rw-rw-rw-   0        0        0    19569 2023-11-20 11:46:20.000000 abtem-1.0.4/abtem/potentials/charge_density.py
--rw-rw-rw-   0        0        0    29597 2023-11-20 11:46:20.000000 abtem-1.0.4/abtem/potentials/gpaw.py
--rw-rw-rw-   0        0        0    52122 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/potentials/iam.py
-drwxrwxrwx   0        0        0        0 2023-11-20 14:28:23.003481 abtem-1.0.4/abtem/prism/
--rw-rw-rw-   0        0        0       75 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/prism/__init__.py
--rw-rw-rw-   0        0        0     4895 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/prism/_natural_neighbors.py
--rw-rw-rw-   0        0        0     5081 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/prism/_partitioned_s_matrix.py
--rw-rw-rw-   0        0        0     8643 2023-11-20 13:26:58.000000 abtem-1.0.4/abtem/prism/bloch.py
--rw-rw-rw-   0        0        0    74228 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/prism/s_matrix.py
--rw-rw-rw-   0        0        0     6605 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/prism/utils.py
--rw-rw-rw-   0        0        0   193265 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/reconstruct.py
--rw-rw-rw-   0        0        0    31866 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/scan.py
--rw-rw-rw-   0        0        0    10246 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/slicing.py
--rw-rw-rw-   0        0        0     6975 2023-11-12 14:26:21.000000 abtem-1.0.4/abtem/tilt.py
--rw-rw-rw-   0        0        0    60806 2023-11-12 14:39:54.000000 abtem-1.0.4/abtem/transfer.py
--rw-rw-rw-   0        0        0    21124 2023-11-12 14:39:54.000000 abtem-1.0.4/abtem/transform.py
--rw-rw-rw-   0        0        0    83448 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/visualize.py
--rw-rw-rw-   0        0        0    93332 2023-11-12 15:03:25.000000 abtem-1.0.4/abtem/visualize_new.py
--rw-rw-rw-   0        0        0    60501 2023-11-20 11:40:42.000000 abtem-1.0.4/abtem/waves.py
-drwxrwxrwx   0        0        0        0 2023-11-20 14:28:22.958421 abtem-1.0.4/abtem.egg-info/
--rw-rw-rw-   0        0        0      841 2023-11-20 14:28:22.000000 abtem-1.0.4/abtem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2600 2023-11-20 14:28:22.000000 abtem-1.0.4/abtem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-20 14:28:22.000000 abtem-1.0.4/abtem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-22 18:10:55.000000 abtem-1.0.4/abtem.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      355 2023-11-20 14:28:22.000000 abtem-1.0.4/abtem.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-11-20 14:28:22.000000 abtem-1.0.4/abtem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      101 2023-04-22 18:10:16.000000 abtem-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0     1291 2023-11-20 14:28:23.024481 abtem-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-04-22 18:10:16.000000 abtem-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-20 14:28:23.022481 abtem-1.0.4/test/
--rw-rw-rw-   0        0        0    10960 2023-11-12 14:26:21.000000 abtem-1.0.4/test/test_array.py
--rw-rw-rw-   0        0        0     5855 2023-11-12 14:39:54.000000 abtem-1.0.4/test/test_atomic_potential.py
--rw-rw-rw-   0        0        0      912 2023-06-18 13:35:57.000000 abtem-1.0.4/test/test_copy.py
--rw-rw-rw-   0        0        0      815 2023-11-12 14:26:21.000000 abtem-1.0.4/test/test_ctf.py
--rw-rw-rw-   0        0        0     4743 2023-11-12 14:26:21.000000 abtem-1.0.4/test/test_detect.py
--rw-rw-rw-   0        0        0      394 2023-04-22 18:10:16.000000 abtem-1.0.4/test/test_distributions.py
--rw-rw-rw-   0        0        0     4056 2023-11-12 14:26:21.000000 abtem-1.0.4/test/test_ensemble.py
--rw-rw-rw-   0        0        0      878 2023-04-22 18:10:16.000000 abtem-1.0.4/test/test_ewald.py
--rw-rw-rw-   0        0        0     5300 2023-11-12 14:39:54.000000 abtem-1.0.4/test/test_gpaw.py
--rw-rw-rw-   0        0        0     3552 2023-04-22 18:10:16.000000 abtem-1.0.4/test/test_grid.py
--rw-rw-rw-   0        0        0     1081 2023-11-12 14:26:21.000000 abtem-1.0.4/test/test_hyperspy.py
--rw-rw-rw-   0        0        0        0 2023-04-22 18:10:16.000000 abtem-1.0.4/test/test_ionization.py
--rw-rw-rw-   0        0        0     1062 2023-06-18 17:49:12.000000 abtem-1.0.4/test/test_kirkland.py
--rw-rw-rw-   0        0        0    18418 2023-11-12 14:26:21.000000 abtem-1.0.4/test/test_measure.py
--rw-rw-rw-   0        0        0     1749 2023-11-12 14:26:21.000000 abtem-1.0.4/test/test_potential_parametrization.py
--rw-rw-rw-   0        0        0     8993 2023-05-12 13:30:58.000000 abtem-1.0.4/test/test_potentials.py
--rw-rw-rw-   0        0        0    10888 2023-11-12 14:39:54.000000 abtem-1.0.4/test/test_prism.py
--rw-rw-rw-   0        0        0     1267 2023-04-22 18:10:16.000000 abtem-1.0.4/test/test_scan.py
--rw-rw-rw-   0        0        0     8084 2023-11-12 14:26:21.000000 abtem-1.0.4/test/test_simulate.py
--rw-rw-rw-   0        0        0     3008 2023-04-22 18:10:16.000000 abtem-1.0.4/test/test_structures.py
--rw-rw-rw-   0        0        0     1637 2023-11-12 14:26:21.000000 abtem-1.0.4/test/test_temperature.py
--rw-rw-rw-   0        0        0    12692 2023-11-20 11:40:42.000000 abtem-1.0.4/test/test_waves.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:41:21.693640 abtem-1.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-04-22 18:02:13.000000 abtem-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      144 2023-04-22 18:10:15.000000 abtem-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1901 2024-04-26 16:41:21.693640 abtem-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2958 2024-04-22 16:38:24.000000 abtem-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 16:41:21.609433 abtem-1.0.5/abtem/
+-rw-rw-rw-   0        0        0     1183 2024-04-17 11:49:45.000000 abtem-1.0.5/abtem/__init__.py
+-rw-rw-rw-   0        0        0       52 2024-04-22 17:00:46.000000 abtem-1.0.5/abtem/_version.py
+-rw-rw-rw-   0        0        0     2469 2024-02-25 12:08:08.000000 abtem-1.0.5/abtem/antialias.py
+-rw-rw-rw-   0        0        0    61458 2024-04-25 11:11:50.000000 abtem-1.0.5/abtem/array.py
+-rw-rw-rw-   0        0        0    32088 2024-03-27 14:09:19.000000 abtem-1.0.5/abtem/atoms.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:41:21.619953 abtem-1.0.5/abtem/bloch/
+-rw-rw-rw-   0        0        0       63 2024-03-31 10:47:14.000000 abtem-1.0.5/abtem/bloch/__init__.py
+-rw-rw-rw-   0        0        0    38462 2024-04-26 09:47:37.000000 abtem-1.0.5/abtem/bloch/dynamical.py
+-rw-rw-rw-   0        0        0     5942 2024-04-22 17:00:46.000000 abtem-1.0.5/abtem/bloch/indexing.py
+-rw-rw-rw-   0        0        0     2078 2024-03-02 20:52:23.000000 abtem-1.0.5/abtem/bloch/matrix_exponential.py
+-rw-rw-rw-   0        0        0     5334 2024-04-22 17:00:46.000000 abtem-1.0.5/abtem/bloch/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:41:21.637972 abtem-1.0.5/abtem/core/
+-rw-rw-rw-   0        0        0      245 2023-04-22 18:10:15.000000 abtem-1.0.5/abtem/core/__init__.py
+-rw-rw-rw-   0        0        0     5328 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/core/_cuda.py
+-rw-rw-rw-   0        0        0      769 2024-04-22 17:00:46.000000 abtem-1.0.5/abtem/core/abtem.yaml
+-rw-rw-rw-   0        0        0    14626 2024-04-26 07:42:27.000000 abtem-1.0.5/abtem/core/axes.py
+-rw-rw-rw-   0        0        0    12844 2024-04-22 17:00:46.000000 abtem-1.0.5/abtem/core/axes_new.py
+-rw-rw-rw-   0        0        0     3061 2024-04-22 17:00:46.000000 abtem-1.0.5/abtem/core/backend.py
+-rw-rw-rw-   0        0        0     6288 2024-02-25 08:19:08.000000 abtem-1.0.5/abtem/core/chunks.py
+-rw-rw-rw-   0        0        0    32748 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/core/colors.py
+-rw-rw-rw-   0        0        0     1883 2024-03-23 16:32:23.000000 abtem-1.0.5/abtem/core/complex.py
+-rw-rw-rw-   0        0        0    11989 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/core/config.py
+-rw-rw-rw-   0        0        0      321 2023-04-22 18:10:15.000000 abtem-1.0.5/abtem/core/constants.py
+-rw-rw-rw-   0        0        0     2134 2024-02-22 14:45:55.000000 abtem-1.0.5/abtem/core/diagnostics.py
+-rw-rw-rw-   0        0        0     8723 2023-04-22 18:10:15.000000 abtem-1.0.5/abtem/core/electron_configurations.py
+-rw-rw-rw-   0        0        0     5401 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/core/energy.py
+-rw-rw-rw-   0        0        0     7141 2024-04-22 17:00:46.000000 abtem-1.0.5/abtem/core/ensemble.py
+-rw-rw-rw-   0        0        0    10699 2024-02-28 10:57:27.000000 abtem-1.0.5/abtem/core/fft.py
+-rw-rw-rw-   0        0        0    14638 2024-04-26 13:22:03.000000 abtem-1.0.5/abtem/core/grid.py
+-rw-rw-rw-   0        0        0     3173 2024-04-26 13:29:50.000000 abtem-1.0.5/abtem/core/units.py
+-rw-rw-rw-   0        0        0     7556 2024-03-31 08:53:22.000000 abtem-1.0.5/abtem/core/utils.py
+-rw-rw-rw-   0        0        0    32700 2024-03-29 12:54:19.000000 abtem-1.0.5/abtem/detectors.py
+-rw-rw-rw-   0        0        0    16782 2024-03-29 15:51:31.000000 abtem-1.0.5/abtem/distributions.py
+-rw-rw-rw-   0        0        0    12126 2024-02-26 10:52:06.000000 abtem-1.0.5/abtem/finite_difference.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:41:21.640972 abtem-1.0.5/abtem/inelastic/
+-rw-rw-rw-   0        0        0        0 2023-04-22 18:10:15.000000 abtem-1.0.5/abtem/inelastic/__init__.py
+-rw-rw-rw-   0        0        0    34549 2024-03-29 12:54:21.000000 abtem-1.0.5/abtem/inelastic/core_loss.py
+-rw-rw-rw-   0        0        0    21444 2024-01-27 15:03:02.000000 abtem-1.0.5/abtem/inelastic/phonons.py
+-rw-rw-rw-   0        0        0    18766 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/inelastic/plasmons.py
+-rw-rw-rw-   0        0        0    31037 2024-03-09 12:19:50.000000 abtem-1.0.5/abtem/integrals.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:41:21.642475 abtem-1.0.5/abtem/magnetism/
+-rw-rw-rw-   0        0        0        0 2023-04-22 18:10:15.000000 abtem-1.0.5/abtem/magnetism/__init__.py
+-rw-rw-rw-   0        0        0    21265 2024-02-22 14:45:56.000000 abtem-1.0.5/abtem/magnetism/iam.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:41:21.643481 abtem-1.0.5/abtem/magnetism/parametrizations/
+-rw-rw-rw-   0        0        0      461 2024-02-22 14:45:56.000000 abtem-1.0.5/abtem/magnetism/parametrizations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:41:21.644480 abtem-1.0.5/abtem/magnetism/parametrizations/data/
+-rw-rw-rw-   0        0        0     5886 2024-02-22 14:45:56.000000 abtem-1.0.5/abtem/magnetism/parametrizations/data/lyon.json
+-rw-rw-rw-   0        0        0     7501 2023-04-22 18:10:15.000000 abtem-1.0.5/abtem/mcf.py
+-rw-rw-rw-   0        0        0   154556 2024-04-26 08:05:26.000000 abtem-1.0.5/abtem/measurements.py
+-rw-rw-rw-   0        0        0     2567 2024-04-22 16:38:24.000000 abtem-1.0.5/abtem/mtf.py
+-rw-rw-rw-   0        0        0    38155 2024-04-22 17:00:46.000000 abtem-1.0.5/abtem/multislice.py
+-rw-rw-rw-   0        0        0    11980 2024-04-22 16:38:24.000000 abtem-1.0.5/abtem/noise.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:41:21.645480 abtem-1.0.5/abtem/parametrizations/
+-rw-rw-rw-   0        0        0    24113 2024-02-26 10:52:06.000000 abtem-1.0.5/abtem/parametrizations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:41:21.651481 abtem-1.0.5/abtem/parametrizations/data/
+-rw-rw-rw-   0        0        0    31766 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/parametrizations/data/kirkland.json
+-rw-rw-rw-   0        0        0    31360 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/parametrizations/data/lobato.json
+-rw-rw-rw-   0        0        0    19124 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/parametrizations/data/peng_high.json
+-rw-rw-rw-   0        0        0    19180 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/parametrizations/data/peng_ionic.json
+-rw-rw-rw-   0        0        0    22039 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/parametrizations/data/peng_low.json
+-rw-rw-rw-   0        0        0    39350 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/parametrizations/data/waasmaier_kirfel.json
+drwxrwxrwx   0        0        0        0 2024-04-26 16:41:21.656025 abtem-1.0.5/abtem/parametrizations/functions/
+-rw-rw-rw-   0        0        0        0 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/parametrizations/functions/__init__.py
+-rw-rw-rw-   0        0        0      590 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/parametrizations/functions/ewald.py
+-rw-rw-rw-   0        0        0     2455 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/parametrizations/functions/kirkland.py
+-rw-rw-rw-   0        0        0     4475 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/parametrizations/functions/lobato.py
+-rw-rw-rw-   0        0        0      999 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/parametrizations/functions/peng.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:41:21.660023 abtem-1.0.5/abtem/potentials/
+-rw-rw-rw-   0        0        0       52 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/potentials/__init__.py
+-rw-rw-rw-   0        0        0     2902 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/potentials/_poisson.py
+-rw-rw-rw-   0        0        0    19569 2024-02-22 14:45:56.000000 abtem-1.0.5/abtem/potentials/charge_density.py
+-rw-rw-rw-   0        0        0    29821 2024-02-26 10:56:17.000000 abtem-1.0.5/abtem/potentials/gpaw.py
+-rw-rw-rw-   0        0        0    54597 2024-04-26 08:56:08.000000 abtem-1.0.5/abtem/potentials/iam.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:41:21.664568 abtem-1.0.5/abtem/prism/
+-rw-rw-rw-   0        0        0       75 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/prism/__init__.py
+-rw-rw-rw-   0        0        0     4895 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/prism/_natural_neighbors.py
+-rw-rw-rw-   0        0        0     5081 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/prism/_partitioned_s_matrix.py
+-rw-rw-rw-   0        0        0    74228 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/prism/s_matrix.py
+-rw-rw-rw-   0        0        0     6605 2023-11-12 14:26:21.000000 abtem-1.0.5/abtem/prism/utils.py
+-rw-rw-rw-   0        0        0   193265 2024-04-22 16:38:24.000000 abtem-1.0.5/abtem/reconstruct.py
+-rw-rw-rw-   0        0        0    32534 2024-04-26 08:20:27.000000 abtem-1.0.5/abtem/scan.py
+-rw-rw-rw-   0        0        0    10972 2024-03-08 14:43:53.000000 abtem-1.0.5/abtem/slicing.py
+-rw-rw-rw-   0        0        0     6973 2024-02-22 14:45:56.000000 abtem-1.0.5/abtem/tilt.py
+-rw-rw-rw-   0        0        0    62210 2024-04-26 08:57:50.000000 abtem-1.0.5/abtem/transfer.py
+-rw-rw-rw-   0        0        0    21662 2024-03-29 17:02:49.000000 abtem-1.0.5/abtem/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:41:21.669587 abtem-1.0.5/abtem/visualize/
+-rw-rw-rw-   0        0        0       86 2024-04-22 16:38:24.000000 abtem-1.0.5/abtem/visualize/__init__.py
+-rw-rw-rw-   0        0        0    33714 2024-04-22 17:00:46.000000 abtem-1.0.5/abtem/visualize/artists.py
+-rw-rw-rw-   0        0        0    11505 2024-04-26 10:56:47.000000 abtem-1.0.5/abtem/visualize/axes_grid.py
+-rw-rw-rw-   0        0        0    26110 2024-04-26 13:26:20.000000 abtem-1.0.5/abtem/visualize/visualizations.py
+-rw-rw-rw-   0        0        0    13599 2024-04-22 17:00:46.000000 abtem-1.0.5/abtem/visualize/widgets.py
+-rw-rw-rw-   0        0        0    69312 2024-04-22 17:00:46.000000 abtem-1.0.5/abtem/waves.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:41:21.691639 abtem-1.0.5/abtem.egg-info/
+-rw-rw-rw-   0        0        0     1901 2024-04-26 16:41:21.000000 abtem-1.0.5/abtem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2882 2024-04-26 16:41:21.000000 abtem-1.0.5/abtem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 16:41:21.000000 abtem-1.0.5/abtem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-22 18:10:55.000000 abtem-1.0.5/abtem.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      355 2024-04-26 16:41:21.000000 abtem-1.0.5/abtem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-26 16:41:21.000000 abtem-1.0.5/abtem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      101 2023-04-22 18:10:16.000000 abtem-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1291 2024-04-26 16:41:21.695144 abtem-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0       73 2024-04-22 16:38:24.000000 abtem-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:41:21.690639 abtem-1.0.5/test/
+-rw-rw-rw-   0        0        0    10960 2023-11-12 14:26:21.000000 abtem-1.0.5/test/test_array.py
+-rw-rw-rw-   0        0        0     6065 2024-02-22 14:45:56.000000 abtem-1.0.5/test/test_atomic_potential.py
+-rw-rw-rw-   0        0        0      912 2023-06-18 13:35:57.000000 abtem-1.0.5/test/test_copy.py
+-rw-rw-rw-   0        0        0      815 2023-11-12 14:26:21.000000 abtem-1.0.5/test/test_ctf.py
+-rw-rw-rw-   0        0        0     5428 2024-03-07 22:22:43.000000 abtem-1.0.5/test/test_detect.py
+-rw-rw-rw-   0        0        0      394 2023-04-22 18:10:16.000000 abtem-1.0.5/test/test_distributions.py
+-rw-rw-rw-   0        0        0     4058 2024-04-22 17:00:46.000000 abtem-1.0.5/test/test_ensemble.py
+-rw-rw-rw-   0        0        0      878 2023-04-22 18:10:16.000000 abtem-1.0.5/test/test_ewald.py
+-rw-rw-rw-   0        0        0        0 2024-02-26 10:57:41.000000 abtem-1.0.5/test/test_fft.py
+-rw-rw-rw-   0        0        0     5300 2023-11-12 14:39:54.000000 abtem-1.0.5/test/test_gpaw.py
+-rw-rw-rw-   0        0        0     3552 2024-04-22 16:38:24.000000 abtem-1.0.5/test/test_grid.py
+-rw-rw-rw-   0        0        0     1081 2023-11-12 14:26:21.000000 abtem-1.0.5/test/test_hyperspy.py
+-rw-rw-rw-   0        0        0        0 2023-04-22 18:10:16.000000 abtem-1.0.5/test/test_ionization.py
+-rw-rw-rw-   0        0        0     1062 2024-04-22 16:38:24.000000 abtem-1.0.5/test/test_kirkland.py
+-rw-rw-rw-   0        0        0    20157 2024-04-22 17:00:46.000000 abtem-1.0.5/test/test_magnetics.py
+-rw-rw-rw-   0        0        0    18626 2024-04-22 17:00:46.000000 abtem-1.0.5/test/test_measure.py
+-rw-rw-rw-   0        0        0     1749 2023-11-12 14:26:21.000000 abtem-1.0.5/test/test_potential_parametrization.py
+-rw-rw-rw-   0        0        0     8993 2024-04-22 16:38:24.000000 abtem-1.0.5/test/test_potentials.py
+-rw-rw-rw-   0        0        0    10888 2024-04-22 16:38:24.000000 abtem-1.0.5/test/test_prism.py
+-rw-rw-rw-   0        0        0     1267 2023-04-22 18:10:16.000000 abtem-1.0.5/test/test_scan.py
+-rw-rw-rw-   0        0        0     8517 2024-02-23 14:22:11.000000 abtem-1.0.5/test/test_simulate.py
+-rw-rw-rw-   0        0        0     3008 2023-04-22 18:10:16.000000 abtem-1.0.5/test/test_structures.py
+-rw-rw-rw-   0        0        0     1637 2023-11-12 14:26:21.000000 abtem-1.0.5/test/test_temperature.py
+-rw-rw-rw-   0        0        0    13006 2024-04-26 13:22:56.000000 abtem-1.0.5/test/test_waves.py
```

### Comparing `abtem-1.0.4/LICENSE` & `abtem-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/README.md` & `abtem-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/__init__.py` & `abtem-1.0.5/abtem/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,10 +22,10 @@
     IndexedDiffractionPatterns,
 )
 from abtem.prism.s_matrix import SMatrix, SMatrixArray
 from abtem.inelastic.phonons import FrozenPhonons, AtomsEnsemble
 from abtem.potentials.iam import Potential, CrystalPotential, PotentialArray
 from abtem.scan import CustomScan, LineScan, GridScan
 from abtem.transfer import CTF, Aperture, TemporalEnvelope, SpatialEnvelope
-from abtem.visualize import show_atoms
+from abtem.visualize.visualizations import show_atoms
 from abtem.waves import Waves, Probe, PlaneWave
 from abtem import transfer
```

### Comparing `abtem-1.0.4/abtem/antialias.py` & `abtem-1.0.5/abtem/antialias.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/array.py` & `abtem-1.0.5/abtem/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for describing array objects."""
+
 from __future__ import annotations
 
 import copy
 import json
 import warnings
 from abc import ABCMeta
 from contextlib import nullcontext, contextmanager
@@ -22,30 +23,28 @@
 from abtem.core.axes import (
     UnknownAxis,
     axis_to_dict,
     axis_from_dict,
     AxisMetadata,
     OrdinalAxis,
     AxesMetadataList,
-    NonLinearAxis,
     LinearAxis,
 )
 from abtem.core.backend import (
     get_array_module,
     copy_to_device,
     cp,
     device_name_from_array_module,
     check_cupy_is_installed,
 )
 from abtem.core.chunks import Chunks, validate_chunks, chunk_shape, iterate_chunk_ranges
 from abtem.core.ensemble import (
     Ensemble,
     _wrap_with_array,
     unpack_blockwise_args,
-    concatenate_array_blocks,
 )
 from abtem.core.utils import (
     normalize_axes,
     CopyMixin,
     tuple_range,
     EqualityMixin,
     interleave,
@@ -195,15 +194,20 @@
 def _compute_context(
     progress_bar: bool = None, profiler=False, resource_profiler=False
 ):
     if progress_bar is None:
         progress_bar = config.get("local_diagnostics.progress_bar")
 
     if progress_bar:
-        progress_bar = ProgressBar()
+        if progress_bar == "tqdm":
+            from tqdm.dask import TqdmCallback
+
+            progress_bar = TqdmCallback(desc="tasks")
+        else:
+            progress_bar = ProgressBar()
     else:
         progress_bar = nullcontext()
 
     if profiler:
         profiler = Profiler()
     else:
         profiler = nullcontext()
@@ -318,15 +322,15 @@
         """Number of base dimensions."""
         return self._base_dims
 
     @property
     def ensemble_dims(self):
         """Number of ensemble dimensions."""
         return len(self.shape) - self.base_dims
-
+    
     @property
     def base_axes_metadata(self) -> list[AxisMetadata]:
         return [UnknownAxis() for _ in range(self._base_dims)]
 
     @property
     def shape(self) -> tuple[int, ...]:
         """Shape of the underlying array."""
@@ -371,14 +375,49 @@
     def _is_base_axis(self, axis: int | tuple[int, ...]) -> bool:
         if isinstance(axis, Number):
             axis = (axis,)
 
         base_axes = tuple(range(len(self.ensemble_shape), len(self.shape)))
         return len(set(axis).intersection(base_axes)) > 0
 
+    def apply_func(self, func, **kwargs) -> T:
+        from abtem.transform import TransformFromFunc
+
+        transform = TransformFromFunc(func, func_kwargs=kwargs)
+        return self.apply_transform(transform)
+
+    def get_from_metadata(self, name: str, broadcastable: bool = False):
+
+        axes_metadata_index = None
+        for i, (n, axis) in enumerate(zip(self.shape, self.ensemble_axes_metadata)):
+            if axis.label == name:
+                data = axis.coordinates(n)
+                axes_metadata_index = i
+
+        if axes_metadata_index is not None and broadcastable:
+            return np.array(data)[
+                (
+                    *((None,) * axes_metadata_index),
+                    slice(None),
+                    *((None,) * (len(self.ensemble_shape) - 1 - axes_metadata_index)),
+                )
+            ]
+        elif axes_metadata_index is not None:
+            if name in self.metadata.keys():
+                raise RuntimeError(
+                    f"Could not resolve metadata for {name}, found in both ensemble axes metadata and metadata"
+                )
+
+            return data
+        else:
+            try:
+                return self.metadata[name]
+            except KeyError:
+                raise RuntimeError(f"Could not resolve metadata for {name}")
+
     @classmethod
     def from_array_and_metadata(
         cls,
         array: np.ndarray | da.core.Array,
         axes_metadata: list[AxisMetadata],
         metadata: dict,
     ) -> T:
@@ -436,14 +475,30 @@
     @property
     def array(self) -> np.ndarray | da.core.Array:
         """
         Underlying array describing the array object.
         """
         return self._array
 
+    @array.setter
+    def array(self, array):
+        """
+        Set underlying array describing the array object.
+        """
+        if not array.shape == self.shape:
+            raise ValueError("Shape of array must match shape of object.")
+
+        if not array.dtype == self.dtype:
+            raise ValueError("Datatype of array must match datatype of object.")
+
+        if self.is_lazy != isinstance(array, da.core.Array):
+            raise ValueError("Type of array must match type of object.")
+
+        self._array = array
+
     @property
     def dtype(self) -> np.dtype.base:
         """
         Datatype of array.
         """
         return self._array.dtype
 
@@ -473,25 +528,25 @@
 
     def _check_is_compatible(self, other: ArrayObject):
         if not isinstance(other, self.__class__):
             raise RuntimeError(
                 f"incompatible types ({self.__class__} != {other.__class__})"
             )
 
-        if self.shape != other.shape:
-            raise RuntimeError(f"incompatible shapes ({self.shape} != {other.shape})")
+        # if self.shape != other.shape:
+        #    raise RuntimeError(f"incompatible shapes ({self.shape} != {other.shape})")
 
-        for (key, value), (other_key, other_value) in zip(
-            self._copy_kwargs(exclude=("array", "metadata")).items(),
-            other._copy_kwargs(exclude=("array", "metadata")).items(),
-        ):
-            if np.any(value != other_value):
-                raise RuntimeError(
-                    f"incompatible values for {key} ({value} != {other_value})"
-                )
+        # for (key, value), (other_key, other_value) in zip(
+        #     self._copy_kwargs(exclude=("array", "metadata")).items(),
+        #     other._copy_kwargs(exclude=("array", "metadata")).items(),
+        # ):
+        #     if np.any(value != other_value):
+        #         raise RuntimeError(
+        #             f"incompatible values for {key} ({value} != {other_value})"
+        #         )
 
     def generate_ensemble(self, keepdims: bool = False):
         """
         Generate every member of the ensemble.
 
         Parameters
         ----------
@@ -500,15 +555,15 @@
 
         Yields
         ------
         ArrayObject or subclass of ArrayObject
             Member of the ensemble.
         """
         for i in np.ndindex(*self.ensemble_shape):
-            yield i, self.get_items(i, keepdims=keepdims)
+            yield i, self.__class__(**self.get_items(i, keepdims=keepdims))
 
     def mean(
         self,
         axis: int | tuple[int, ...] = None,
         keepdims: bool = False,
         split_every: int = 2,
     ) -> T:
@@ -738,38 +793,21 @@
 
     def __pow__(self, other) -> T:
         return self._arithmetic(other, "__pow__")
 
     __rmul__ = __mul__
     __rtruediv__ = __truediv__
 
-    def get_items(
-        self, items: int | tuple[int, ...] | slice, keepdims: bool = False
-    ) -> T:
-        """
-        Index the array and the corresponding axes metadata. Only ensemble axes can be indexed.
-
-        Parameters
-        ----------
-        items : int or tuple of int or slice
-            The array is indexed according to this.
-        keepdims : bool, optional
-            If True, all ensemble axes are left in the result as dimensions with size one. Default is False.
-
-        Returns
-        -------
-        indexed_array : ArrayObject or subclass of ArrayObject
-            The indexed array object.
-        """
-        if isinstance(items, (Number, slice, type(None))):
+    def _validate_items(self, items, keepdims: bool = False):
+        if isinstance(items, (Number, slice, type(None), list, np.ndarray)):
             items = (items,)
 
         elif not isinstance(items, tuple):
             raise NotImplementedError(
-                "Indices must be integers or slices or a tuple of integers or slices or None."
+                f"Indices must be integers or slices or a tuple of integers or slices or None, not {type(items).__name__}."
             )
 
         if keepdims:
             items = tuple(
                 slice(item, item + 1) if isinstance(item, int) else item
                 for item in items
             )
@@ -780,41 +818,74 @@
             raise NotImplementedError
 
         if len(tuple(item for item in items if item is not None)) > len(
             self.ensemble_shape
         ):
             raise RuntimeError("Base axes cannot be indexed.")
 
-        expanded_axes_metadata = [
+        return items
+
+    def _get_ensemble_axes_metadata_items(self, items):
+        expanded_axes_metadatas = [
             axis_metadata.copy() for axis_metadata in self.ensemble_axes_metadata
         ]
         for i, item in enumerate(items):
             if item is None:
-                expanded_axes_metadata.insert(i, UnknownAxis())
+                expanded_axes_metadatas.insert(i, UnknownAxis())
 
         metadata = {}
         axes_metadata = []
         last_indexed = 0
-        for i, item in enumerate(items):
+        for item, expanded_axes_metadata in zip(items, expanded_axes_metadatas):
             last_indexed += 1
             if isinstance(item, Number):
-                metadata = {**metadata, **expanded_axes_metadata[i].item_metadata(item)}
+                metadata = {**metadata, **expanded_axes_metadata.item_metadata(item)}
             else:
-                axes_metadata += [expanded_axes_metadata[i][item].copy()]
+                try:
+                    axes_metadata += [expanded_axes_metadata[item].copy()]
+                except TypeError:
+                    axes_metadata += [expanded_axes_metadata.copy()]
+
+        axes_metadata += expanded_axes_metadatas[last_indexed:]
+        return axes_metadata, metadata
+
+    def get_items(
+        self,
+        items: int | tuple[int, ...] | slice,
+        keepdims: bool = False,
+    ) -> T:
+        """
+        Index the array and the corresponding axes metadata. Only ensemble axes can be indexed.
+
+        Parameters
+        ----------
+        items : int or tuple of int or slice
+            The array is indexed according to this.
+        keepdims : bool, optional
+            If True, all ensemble axes are left in the result as dimensions with size one. Default is False.
 
-        axes_metadata += expanded_axes_metadata[last_indexed:]
+        Returns
+        -------
+        indexed_array : ArrayObject or subclass of ArrayObject
+            The indexed array object.
+        """
 
-        d = self._copy_kwargs(exclude=("array", "ensemble_axes_metadata", "metadata"))
-        d["array"] = self._array[items]
-        d["ensemble_axes_metadata"] = axes_metadata
-        d["metadata"] = {**self.metadata, **metadata}
-        return self.__class__(**d)
+        items = self._validate_items(items, keepdims)
+        ensemble_axes_metadata, metadata = self._get_ensemble_axes_metadata_items(items)
+
+        kwargs = self._copy_kwargs(
+            exclude=("array", "ensemble_axes_metadata", "metadata")
+        )
+        kwargs["array"] = self._array[items]
+        kwargs["ensemble_axes_metadata"] = ensemble_axes_metadata
+        kwargs["metadata"] = {**self.metadata, **metadata}
+        return kwargs
 
     def __getitem__(self, items) -> T:
-        return self.get_items(items)
+        return self.__class__(**self.get_items(items))
 
     def expand_dims(
         self, axis: tuple[int, ...] = None, axis_metadata: list[AxisMetadata] = None
     ) -> T:
         """
         Expand the shape of the array object.
 
@@ -917,14 +988,17 @@
         if chunks == "auto":
             chunks = ("auto",) * len(self.ensemble_shape) + (-1,) * len(self.base_shape)
 
         array = da.from_array(self.array, chunks=chunks)
 
         return self.__class__(array, **self._copy_kwargs(exclude=("array",)))
 
+    def lazy(self, chunks: str = "auto") -> T:
+        return self.ensure_lazy(chunks)
+
     def compute(
         self,
         progress_bar: bool = None,
         profiler: bool = False,
         resource_profiler: bool = False,
         **kwargs,
     ):
@@ -972,14 +1046,15 @@
 
         Returns
         -------
         object_on_device : T
         """
         kwargs = self._copy_kwargs(exclude=("array",))
         kwargs["array"] = copy_to_device(self.array, device)
+        
         return self.__class__(**kwargs)
 
     def to_cpu(self) -> T:
         """
         Move the array to the host memory from an arbitrary source array.
         """
         return self.copy_to_device("cpu")
@@ -1286,15 +1361,15 @@
             self._check_axes_metadata()
         except RuntimeError:
             self._ensemble_axes_metadata = old_axes_metadata
 
         return self
 
     def to_hyperspy(self):
-        """Convert measurement to a Hyperspy signal."""
+        """Convert ArrayObject to a Hyperspy signal."""
 
         try:
             import hyperspy.api as hs
         except ImportError:
             raise ImportError(
                 "This functionality of *ab*TEM requires Hyperspy, see https://hyperspy.org."
             )
@@ -1313,36 +1388,68 @@
         ensemble_axes_metadata = _to_hyperspy_axes_metadata(
             self.ensemble_axes_metadata,
             self.ensemble_shape,
         )
 
         xp = get_array_module(self.device)
 
-        base_axes = tuple_range(
-            offset=len(self.ensemble_shape),
-            length=len(self.shape) - len(self.ensemble_shape),
+        axes_base_indices = tuple_range(
+            offset=len(self.ensemble_shape), length=len(self.base_shape)
         )
+
         ensemble_axes = tuple_range(
             offset=0,
             length=len(self.ensemble_shape),
         )
 
-        array = xp.transpose(self.array, ensemble_axes + base_axes[::-1])
+        array = xp.transpose(self.array, ensemble_axes + axes_base_indices[::-1])
 
         s = signal_type(array, axes=ensemble_axes_metadata + axes_base[::-1])
 
         if self.is_lazy:
             s = s.as_lazy()
 
         return s
 
+    def to_data_array(self):
+        """Convert ArrayObject to a xarray DataArray."""
+
+        try:
+            import xarray as xr
+        except ImportError:
+            raise ImportError(
+                "This functionality of *ab*TEM requires xarray, see https://xarray.dev/."
+            )
+
+        coords = {}
+        dims = []
+        for n, axis in zip(self.shape, self.axes_metadata):
+            x = np.array(axis.coordinates(n))
+            if isinstance(x, np.ndarray) and len(x.shape) == 2:
+                x = [f"{i}" for i in x]
+            elif len(x.shape) == 1:
+                pass
+            else:
+                raise ValueError("The shape of the coordinates is not supported.")
+
+            dims.append(axis.label)
+            
+            coords[axis.label] = xr.DataArray(
+                x, name=axis.label, dims=(axis.label,), attrs={"units": axis.units}
+            )
+        
+        attrs = self.metadata
+        attrs["long_name"] = self.metadata["label"]
+
+        return xr.DataArray(self.array, dims=dims, coords=coords, attrs=attrs)
+
     def _stack(self, arrays, axis_metadata, axis):
         xp = get_array_module(arrays[0].array)
 
-        if arrays[0].is_lazy:
+        if any(array.is_lazy for array in arrays):
             array = da.stack([measurement.array for measurement in arrays], axis=axis)
         else:
             array = xp.stack([measurement.array for measurement in arrays], axis=axis)
 
         cls = arrays[0].__class__
         kwargs = arrays[0]._copy_kwargs(exclude=("array",))
 
@@ -1360,21 +1467,32 @@
         if len(self.ensemble_shape) == 0:
             ensemble_axes_metadata = _wrap_with_array([], 1)
         else:
             chunks = self._validate_ensemble_chunks(chunks)
 
             ensemble_axes_metadata = np.zeros(chunk_shape(chunks), dtype=object)
             for index, slic in iterate_chunk_ranges(chunks):
-                ensemble_axes_metadata.itemset(
-                    index,
-                    [
-                        self.ensemble_axes_metadata[i][slic[i]]
-                        for i, axis in enumerate(self.ensemble_axes_metadata)
-                    ],
-                )
+                new_ensemble_axes_metadata = []
+
+                # ensemble_axes_metadata.itemset(
+                #     index,
+                #     [
+                #         self.ensemble_axes_metadata[i][slic[i]]
+                #         for i, axis in enumerate(self.ensemble_axes_metadata)
+                #     ],
+                # )
+                for i, axis in enumerate(self.ensemble_axes_metadata):
+                    try:
+                        axis = axis[slic[i]]
+                    except TypeError:
+                        axis = axis.copy()
+
+                    new_ensemble_axes_metadata.append(axis)
+
+                ensemble_axes_metadata.itemset(index, new_ensemble_axes_metadata)
 
         if lazy:
             ensemble_axes_metadata = da.from_array(ensemble_axes_metadata, chunks=1)
 
         return ensemble_axes_metadata
 
     @property
@@ -1557,14 +1675,20 @@
     if axis_metadata is None:
         axis_metadata = UnknownAxis()
 
     elif isinstance(axis_metadata, (tuple, list)):
         if not all(isinstance(element, str) for element in axis_metadata):
             raise ValueError()
         axis_metadata = OrdinalAxis(values=axis_metadata)
+    
+    elif isinstance(axis_metadata, dict):
+        axis_metadata = OrdinalAxis(**axis_metadata)
+    
+    elif not isinstance(axis_metadata, AxisMetadata):
+        raise ValueError()
 
     return arrays[0]._stack(arrays, axis_metadata, axis)
 
 
 def concatenate(arrays: Sequence[ArrayObject], axis: int = 0) -> T:
     """
     Join a sequence of abTEM array classes along an existing axis.
@@ -1602,56 +1726,105 @@
     axes_metadata[axis] = concatenated_axes_metadata
 
     return cls.from_array_and_metadata(
         array=array, axes_metadata=axes_metadata, metadata=arrays[0].metadata
     )
 
 
-def _unpack_array_object_blocks(blocks):
-    new_blocks = np.empty(blocks.shape, dtype=object)
-    for indices in np.ndindex(blocks.shape):
-        new_blocks[indices] = blocks[indices].array
-    return new_blocks
+def swapaxes(array_object, axis1, axis2):
+    xp = get_array_module(array_object.array)
+
+    if array_object.is_lazy:
+        array = da.swapaxes(array_object.array, axis1, axis2)
+    else:
+        array = xp.swapaxes(array_object.array, axis1, axis2)
+
+    cls = array_object.__class__
+
+    axes_metadata = copy.copy(array_object.axes_metadata)
+    axes_metadata[axis2], axes_metadata[axis1] = (
+        axes_metadata[axis1],
+        axes_metadata[axis2],
+    )
+
+    return cls.from_array_and_metadata(
+        array=array, axes_metadata=axes_metadata, metadata=array_object.metadata
+    )
+
+
+def move_item(lst, from_index, to_index):
+    element = lst.pop(from_index)
+    lst.insert(to_index, element)
+    return lst
+
 
+def moveaxis(array_object, source, destination):
+    xp = get_array_module(array_object.array)
+
+    if array_object.is_lazy:
+        array = da.moveaxis(array_object.array, source, destination)
+    else:
+        array = xp.moveaxis(array_object.array, source, destination)
+
+    cls = array_object.__class__
+
+    axes_metadata = copy.copy(array_object.axes_metadata)
+
+    for s, d in zip(reversed(source), reversed(destination)):
+        axes_metadata = move_item(axes_metadata, s, d)
+
+    return cls.from_array_and_metadata(
+        array=array, axes_metadata=axes_metadata, metadata=array_object.metadata
+    )
 
 def _concatenate_axes_metadata(axes_metadata):
     if len(axes_metadata) == 0:
         raise RuntimeError()
 
     while len(axes_metadata) > 1:
         axes_metadata = [
             *axes_metadata[:-2],
             axes_metadata[-2].concatenate(axes_metadata[-1]),
         ]
     return axes_metadata[0]
 
 
-def _axes_metadata_from_array_object_blocks(blocks):
-    if blocks.ravel()[0].ensemble_dims == 0:
-        return []
-
-    axes_metadata = []
-    for i, n in enumerate(blocks.shape):
-        index = tuple(slice(None) if j == i else 0 for j in range(len(blocks.shape)))
-
-        axes_metadata.append(
-            _concatenate_axes_metadata(
-                [
-                    block.ensemble_axes_metadata[i]
-                    for block in blocks[index]
-                    if len(block.ensemble_axes_metadata)
-                ]
-            )
-        )
-    return axes_metadata
-
-
-def _concat_array_object_ensemble_blocks(blocks):
-    array_blocks = _unpack_array_object_blocks(blocks)
-    concat_array = concatenate_array_blocks(array_blocks)
-    concat_axes_metadata = _axes_metadata_from_array_object_blocks(blocks)
-
-    concat_array_object = ArrayObject(
-        array=concat_array,
-        ensemble_axes_metadata=concat_axes_metadata,
-    )
-    return concat_array_object
+# def _unpack_array_object_blocks(blocks):
+#     new_blocks = np.empty(blocks.shape, dtype=object)
+#     for indices in np.ndindex(blocks.shape):
+#         new_blocks[indices] = blocks[indices].array
+#     return new_blocks
+
+# def _axes_metadata_from_array_object_blocks(blocks):
+#     if blocks.ravel()[0].ensemble_dims == 0:
+#         return []
+
+#     axes_metadata = []
+#     for i, n in enumerate(blocks.shape):
+#         index = tuple(slice(None) if j == i else 0 for j in range(len(blocks.shape)))
+
+#         axes_metadata.append(
+#             _concatenate_axes_metadata(
+#                 [
+#                     block.ensemble_axes_metadata[i]
+#                     for block in blocks[index]
+#                     if len(block.ensemble_axes_metadata)
+#                 ]
+#             )
+#         )
+#     return axes_metadata
+
+# def _concat_array_object_ensemble_blocks(blocks) -> ArrayObject:
+#     array_blocks = _unpack_array_object_blocks(blocks)
+#     concat_array = concatenate_array_blocks(array_blocks)
+#     #concat_axes_metadata = _axes_metadata_from_array_object_blocks(blocks)
+    
+#     concat_array_object = ArrayObject(array=concat_array)
+#     #concat_array_object = ArrayObject(array=concat_array, ensemble_axes_metadata=concat_axes_metadata)
+#     return concat_array_object
+
+
+# def _concat_array_object_ensemble_blocks2(blocks) -> ArrayObject:
+#     array_blocks = _unpack_array_object_blocks(blocks)
+#     concat_array = concatenate_array_blocks(array_blocks)
+#     concat_array_object = ArrayObject(array=concat_array)
+#     return concat_array_object
```

### Comparing `abtem-1.0.4/abtem/atoms.py` & `abtem-1.0.5/abtem/atoms.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,88 @@
 """Module for modifying ASE `Atoms` objects for use in abTEM."""
+
 from __future__ import annotations
+
 from numbers import Number
 
 import numpy as np
 from ase import Atoms
 from ase.build.tools import rotation_matrix, cut
 from ase.cell import Cell
 from scipy.cluster.hierarchy import fcluster, linkage
 from scipy.spatial.distance import pdist
 
 from abtem.core.utils import label_to_index
 
-# Converting Cartesian string representations of Cartesian axes to numerical.
-_axes2tuple = {
-    "sxyz": (0, 0, 0, 0),
-    "sxyx": (0, 0, 1, 0),
-    "sxzy": (0, 1, 0, 0),
-    "sxzx": (0, 1, 1, 0),
-    "syzx": (1, 0, 0, 0),
-    "syzy": (1, 0, 1, 0),
-    "syxz": (1, 1, 0, 0),
-    "syxy": (1, 1, 1, 0),
-    "szxy": (2, 0, 0, 0),
-    "szxz": (2, 0, 1, 0),
-    "szyx": (2, 1, 0, 0),
-    "szyz": (2, 1, 1, 0),
-    "rzyx": (0, 0, 0, 1),
-    "rxyx": (0, 0, 1, 1),
-    "ryzx": (0, 1, 0, 1),
-    "rxzx": (0, 1, 1, 1),
-    "rxzy": (1, 0, 0, 1),
-    "ryzy": (1, 0, 1, 1),
-    "rzxy": (1, 1, 0, 1),
-    "ryxy": (1, 1, 1, 1),
-    "ryxz": (2, 0, 0, 1),
-    "rzxz": (2, 0, 1, 1),
-    "rxyz": (2, 1, 0, 1),
-    "rzyz": (2, 1, 1, 1),
-}
-
 axis_mapping = {"x": (1, 0, 0), "y": (0, 1, 0), "z": (0, 0, 1)}
 
 
+def euler_sequence(axes: str, convention: str):
+    """
+    Parameters
+    ----------
+    axes : str
+        Specifies the order of rotation axes. It should be a string representing a valid combination of the letters 'x',
+        'y', and 'z' in any order. For example, 'xyz' represents a sequence of rotations about the x-axis, y-axis,
+        and z-axis in that order.
+
+    convention : str
+        Specifies the convention used for the Euler angles. It should be either 'intrinsic' or 'static' for rotations
+        applied to a fixed frame or 'extrinsic' or 'rotating' for rotations applied to a rotating frame.
+
+    Returns
+    -------
+    tuple
+        A tuple of four angles (theta1, theta2, theta3, phi) representing the Euler sequence specified by the given
+        axes and convention.
+
+    Raises
+    ------
+    ValueError
+        If the given convention is not one of the valid options ('intrinsic', 'static', 'extrinsic', 'rotating').
+
+    """
+    if convention in ("intrinsic", "static"):
+        sequences = {
+            "xyz": (0, 0, 0, 0),
+            "xyx": (0, 0, 1, 0),
+            "xzy": (0, 1, 0, 0),
+            "xzx": (0, 1, 1, 0),
+            "yzx": (1, 0, 0, 0),
+            "yzy": (1, 0, 1, 0),
+            "yxz": (1, 1, 0, 0),
+            "yxy": (1, 1, 1, 0),
+            "zxy": (2, 0, 0, 0),
+            "zxz": (2, 0, 1, 0),
+            "zyx": (2, 1, 0, 0),
+            "zyz": (2, 1, 1, 0),
+        }
+    elif convention in ("extrinsic", "rotating"):
+        sequences = {
+            "zyx": (0, 0, 0, 1),
+            "xyx": (0, 0, 1, 1),
+            "yzx": (0, 1, 0, 1),
+            "xzx": (0, 1, 1, 1),
+            "xzy": (1, 0, 0, 1),
+            "yzy": (1, 0, 1, 1),
+            "zxy": (1, 1, 0, 1),
+            "yxy": (1, 1, 1, 1),
+            "yxz": (2, 0, 0, 1),
+            "zxz": (2, 0, 1, 1),
+            "xyz": (2, 1, 0, 1),
+            "zyz": (2, 1, 1, 1),
+        }
+    else:
+        raise ValueError(
+            f"convention must be either 'intrinsic', 'static', 'extrinsic', or 'rotating', not {convention}."
+        )
+
+    return sequences[axes]
+
+
 def plane_to_axes(plane: str) -> tuple:
     """
     Convert string representation of Cartesian axes to numerical.
 
     Parameters
     ----------
     plane : str
@@ -217,15 +254,17 @@
         raise RuntimeError(
             "This cell cannot be made orthogonal using currently implemented methods."
         )
 
     return atoms
 
 
-def rotation_matrix_to_euler(R: np.ndarray, axes: str = "sxyz", eps: float = 1e-6):
+def rotation_matrix_to_euler(
+    R: np.ndarray, axes: str = "xyz", convention: str = "intrinsic", eps: float = 1e-6
+):
     """
     Convert a Cartesian rotation matrix to Euler angles.
 
     Parameters
     ----------
     R : np.ndarray
         Rotation array of dimension 3x3.
@@ -235,19 +274,21 @@
         Components of the rotation matrix whose magnitude is below this value are ignored.
 
     Returns
     -------
     angles : tuple
         Euler angles corresponding to the given rotation matrix.
     """
-    first_axis, parity, repetition, frame = _axes2tuple[axes.lower()]
+
+    first_axis, parity, repetition, frame = euler_sequence(axes, convention)
+    next_axis = [1, 2, 0, 1]
 
     i = first_axis
-    j = [1, 2, 0, 1][i + parity]
-    k = [1, 2, 0, 1][i - parity + 1]
+    j = next_axis[i + parity]
+    k = next_axis[i - parity + 1]
 
     R = np.array(R, dtype=float)
     if repetition:
         sy = np.sqrt(R[i, j] * R[i, j] + R[i, k] * R[i, k])
         if sy > eps:
             ax = np.arctan2(R[i, j], R[i, k])
             ay = np.arctan2(sy, R[i, i])
@@ -270,14 +311,81 @@
     if parity:
         ax, ay, az = -ax, -ay, -az
     if frame:
         ax, az = az, ax
     return ax, ay, az
 
 
+def euler_to_rotation(
+    ai: float, aj: float, ak: float, axes: str = "xyz", convention: str = "intrinsic"
+):
+    """
+    Convert sequence of Euler angles to Cartesian rotation matrix.
+
+    Parameters
+    ----------
+    ai : float
+        First Euler angle.
+    aj : float
+        Second Euler angle.
+    ak : float
+        Third Euler angle.
+    axes : str, optional
+        String representation of the axes of rotation. Default is "xyz".
+    convention : str, optional
+        Convention for rotation order. Default is "intrinsic".
+
+    Returns
+    -------
+    R : ndarray
+        3x3 rotation matrix
+
+    """
+    firstaxis, parity, repetition, frame = euler_sequence(axes, convention)
+
+    next_axis = [1, 2, 0, 1]
+
+    i = firstaxis
+    j = next_axis[i + parity]
+    k = next_axis[i - parity + 1]
+
+    if frame:
+        ai, ak = ak, ai
+    if parity:
+        ai, aj, ak = -ai, -aj, -ak
+
+    si, sj, sk = np.sin(ai), np.sin(aj), np.sin(ak)
+    ci, cj, ck = np.cos(ai), np.cos(aj), np.cos(ak)
+    cc, cs = ci * ck, ci * sk
+    sc, ss = si * ck, si * sk
+
+    R = np.eye(3)
+    if repetition:
+        R[i, i] = cj
+        R[i, j] = sj * si
+        R[i, k] = sj * ci
+        R[j, i] = sj * sk
+        R[j, j] = -cj * ss + cc
+        R[j, k] = -cj * cs - sc
+        R[k, i] = -sj * ck
+        R[k, j] = cj * sc + cs
+        R[k, k] = cj * cc - ss
+    else:
+        R[i, i] = cj * ck
+        R[i, j] = sj * sc - cs
+        R[i, k] = sj * cc + ss
+        R[j, i] = cj * sk
+        R[j, j] = sj * ss + cc
+        R[j, k] = sj * cs - sc
+        R[k, i] = -sj
+        R[k, j] = cj * si
+        R[k, k] = cj * ci
+    return R
+
+
 def decompose_affine_transform(
     affine_transform: np.ndarray,
 ) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
     """
     Decompose an affine transform into rotation, scale and shear.
 
     Parameters
@@ -479,14 +587,58 @@
 
     if np.any(x_vector != old_x_vector) or np.any(y_vector != old_y_vector):
         return rotation_matrix(old_x_vector, x_vector, old_y_vector, y_vector)
     else:
         return np.eye(3)
 
 
+def rotate_atoms(
+    atoms: Atoms,
+    axes: str = "zxz",
+    angles: tuple[float, float, float] = (0.0, 0.0, 0.0),
+    convention: str = "intrinsic",
+) -> Atoms:
+    """
+    Rotate the positions and cell vectors of atoms using Euler angles.
+
+    Parameters
+    ----------
+    atoms : Atoms
+        The atoms object to rotate.
+    axes : str, optional
+        The sequence of axes for rotation. Default is "zxz".
+    angles : tuple[float, float, float], optional
+        The Euler angles in radians. Default is (0.0, 0.0, 0.0).
+    convention : str, optional
+        The convention for Euler angles. Default is "intrinsic".
+
+    Returns
+    -------
+    Atoms
+        The rotated atoms object.
+    """
+    atoms = atoms.copy()
+
+    if isinstance(angles, Number):
+        angles = (angles,)
+
+    angles = angles + (0.0,) * (3 - len(angles))
+
+    if not len(angles) == 3:
+        raise ValueError("Angles must be a tuple of length 3.")
+
+    axes = axes + "x" * (3 - len(axes))
+
+    R = euler_to_rotation(*angles, axes=axes, convention=convention)
+
+    atoms.positions[:] = np.dot(atoms.positions, R.T)
+    atoms.cell[:] = np.dot(atoms.cell, R.T)
+    return atoms
+
+
 def rotate_atoms_to_plane(
     atoms: Atoms,
     plane: str | tuple[tuple[float, float, float], tuple[float, float, float]] = "xy",
 ) -> Atoms:
     """
     Rotate atoms so that their `xy` plane is rotated into a given plane.
 
@@ -681,15 +833,18 @@
     if plane != "xy":
         atoms = rotate_atoms_to_plane(atoms, plane)
 
     if box is None:
         box = best_orthogonal_cell(atoms.cell, max_repetitions=max_repetitions)
 
     if tuple(np.diag(atoms.cell)) == tuple(box):
-        return atoms
+        if return_transform:
+            return atoms, (np.zeros(3), np.ones(3), np.zeros(3))
+        else:
+            return atoms
 
     if np.any(atoms.cell.lengths() < tolerance):
         raise RuntimeError("Cell vectors must have non-zero length.")
 
     inv = np.linalg.inv(atoms.cell)
     vectors = np.dot(np.diag(box), inv)
     vectors = np.round(vectors)
```

### Comparing `abtem-1.0.4/abtem/core/_cuda.py` & `abtem-1.0.5/abtem/core/_cuda.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/core/abtem.yaml` & `abtem-1.0.5/abtem/core/abtem.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 device: cpu
 fft: fftw
+precision: float32
 local_diagnostics:
   progress_bar: true
+  task_level_progress: false
 dask:
   fuse: true
   worker-saturation: 1.0
   lazy: true
   scheduler: threads
   chunk-size: 128 MB
   chunk-size-gpu: 512 MB
```

### Comparing `abtem-1.0.4/abtem/core/axes.py` & `abtem-1.0.5/abtem/core/axes_new.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,30 +44,30 @@
         return f"{base} \\times 10^{{{int(exponent)}}}"
     else:
         return float_str
 
 
 def format_value(value: Union[tuple, float], formatting: str, tolerance: float = 1e-14):
     if isinstance(value, tuple):
-        return ", ".join(format_value(v, formatting=formatting) for v in value)
+        return ", ".join(str(format_value(v, formatting=formatting)) for v in value)
 
     if isinstance(value, float):
         if np.abs(value) < tolerance:
             value = 0.0
 
         if config.get("visualize.use_tex", False):
-            return latex_float(value, formatting)
+            return f"${latex_float(value, formatting)}$"
         else:
             return f"{value:>{formatting}}"
 
     return value
 
 
 def format_title(
-        axes, formatting: str = ".3f", units: str = None, include_label: bool = True
+    axes, formatting: str = ".3f", units: str = None, include_label: bool = True
 ):
     try:
         value = axes.values[0] * _get_conversion_factor(units, axes.units)
     except KeyError:
         value = axes.values[0]
 
     units = _validate_units(units, axes.units)
@@ -85,15 +85,21 @@
         units = f" {_format_units(units)}"
     elif units is not None:
         units = f" {units}"
     else:
         units = ""
 
     if use_tex:
-        return f"{label}${format_value(value, formatting)}${units}"
+        value = format_value(value, formatting)
+        # if isinstance(value, Number):
+        #     value = f"${value}$"
+        # else:
+        # value = f"{value}"
+
+        return f"{label}{value}{units}"
     else:
         return f"{label}{value:>{formatting}}{units}"
 
 
 @dataclass(eq=False, repr=False, unsafe_hash=True)
 class AxisMetadata:
     label: str = ""
@@ -160,14 +166,20 @@
         return self
 
     @staticmethod
     def from_dict(d):
         cls = globals()[d["type"]]
         return cls(**{key: value for key, value in d.items() if key != "type"})
 
+    def limits(self, n=None):
+        coordinates = self.coordinates(n)
+        min_limit = coordinates[0]
+        max_limit = coordinates[-1]
+        return min_limit, max_limit
+
 
 @dataclass(eq=False, repr=False, unsafe_hash=True)
 class UnknownAxis(AxisMetadata):
     label: str = "unknown"
 
 
 @dataclass(eq=False, repr=False, unsafe_hash=True)
@@ -185,26 +197,31 @@
         coordinates = self.coordinates(n)
         if n > 3:
             coordinates = [f"{coord:.2f}" for coord in coordinates[[0, 1, -1]]]
             return f"{coordinates[0]} {coordinates[1]} ... {coordinates[2]}"
         else:
             return " ".join([f"{coord:.2f}" for coord in coordinates])
 
-    def coordinates(self, n: int) -> np.ndarray:
+    def coordinates(self, n: int = None) -> np.ndarray:
+        if n is None:
+            raise ValueError("n is required")
+
         return np.linspace(
             self.offset, self.offset + self.sampling * n, n, endpoint=False
         )
 
     def to_nonlinear_axis(self, n):
         values = tuple(self.coordinates(n))
-        return NonLinearAxis(label=self.label,
-                           _tex_label=self._tex_label,
-                           units=self.units,
-                           values=values,
-                           _concatenate=self._concatenate)
+        return NonLinearAxis(
+            label=self.label,
+            _tex_label=self._tex_label,
+            units=self.units,
+            values=values,
+            _concatenate=self._concatenate,
+        )
 
 
 @dataclass(eq=False, repr=False, unsafe_hash=True)
 class RealSpaceAxis(LinearAxis):
     sampling: float = 1.0
     units: str = "pixels"
     endpoint: bool = True
@@ -224,15 +241,17 @@
 
 
 @dataclass(eq=False, repr=False, unsafe_hash=True)
 class OrdinalAxis(AxisMetadata):
     values: Union[Sequence, ArrayLike] = ()
 
     def format_title(self, formatting, include_label: bool = True, **kwargs):
-        return format_title(self, formatting=formatting, include_label=include_label, **kwargs)
+        return format_title(
+            self, formatting=formatting, include_label=include_label, **kwargs
+        )
 
     def concatenate(self, other):
         if not safe_equality(self, other, ("values",)):
             raise RuntimeError()
 
         kwargs = dataclasses.asdict(self)
         kwargs["values"] = kwargs["values"] + other.values
@@ -372,14 +391,24 @@
 
 
 @dataclass(eq=False, repr=False, unsafe_hash=True)
 class PrismPlaneWavesAxis(AxisMetadata):
     pass
 
 
+@dataclass(eq=False, repr=False, unsafe_hash=True)
+class ScaleAxis:
+    label: str = ""
+    units: str = None
+    _tex_label: str | None = None
+
+    def format_label(self):
+        return format_label(self)
+
+
 def axis_to_dict(axis: AxisMetadata):
     d = dataclasses.asdict(axis)
     for key, value in d.items():
         if isinstance(value, np.ndarray):
             d[key] = tuple(value.tolist())
 
     d["type"] = axis.__class__.__name__
@@ -418,8 +447,8 @@
 
 class AxesMetadataList(list):
     def __init__(self, l, shape):
         self._shape = shape
         super().__init__(l)
 
     def __repr__(self):
-        return format_axes_metadata(self, self._shape)
+        return format_axes_metadata(self, self._shape)
```

### Comparing `abtem-1.0.4/abtem/core/backend.py` & `abtem-1.0.5/abtem/core/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
     if isinstance(array, da.core.Array):
         return array.map_blocks(asnumpy)
 
     return cp.asnumpy(array)
 
 
-def copy_to_device(array, device):
+def copy_to_device(array, device:str):
     old_xp = get_array_module(array)
     new_xp = get_array_module(device)
 
     if old_xp is new_xp:
         return array
 
     if isinstance(array, da.core.Array):
```

### Comparing `abtem-1.0.4/abtem/core/chunks.py` & `abtem-1.0.5/abtem/core/chunks.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     ):
         slic = tuple(slice(*cr) for cr in chunk_range)
 
         yield block_indices, slic
 
 
 def config_chunk_size(device):
-
     if device == "gpu":
         return parse_bytes(config.get("dask.chunk-size-gpu"))
 
     if device != "cpu":
         raise RuntimeError()
 
     return parse_bytes(config.get("dask.chunk-size"))
@@ -50,15 +49,14 @@
 def validate_chunks(
     shape: tuple[int, ...],
     chunks: Chunks,
     limit: int | str = "auto",
     dtype: np.dtype.base = None,
     device: str = "cpu",
 ) -> ValidatedChunks:
-
     if chunks == -1:
         return validate_chunks(shape, shape)
 
     if isinstance(chunks, int):
         limit = chunks
         chunks = ("auto",) * len(shape)
         return auto_chunks(shape, chunks, limit, dtype=dtype, device=device)
@@ -68,19 +66,18 @@
         return chunks
 
     if any(isinstance(c, str) for c in chunks):
         return auto_chunks(shape, chunks, limit, dtype=dtype, device=device)
 
     if len(shape) == 1 and len(chunks) != len(shape):
         assert sum(chunks) == shape[0]
-        return chunks,
+        return (chunks,)
 
     validated_chunks = ()
     for s, c in zip(shape, chunks):
-
         if isinstance(c, tuple):
             assert sum(c) == s
             validated_chunks += (c,)
 
         elif isinstance(c, int):
             if c == -1:
                 validated_chunks += ((s,),)
@@ -99,15 +96,14 @@
 def auto_chunks(
     shape: tuple[int, ...],
     chunks: Chunks,
     limit: str | int = "auto",
     dtype: np.dtype.base = None,
     device: str = "cpu",
 ) -> ValidatedChunks:
-
     if limit == "auto":
         if dtype is None:
             raise ValueError("auto selecting chunk limits requires dtype")
 
         limit = int(np.floor(config_chunk_size(device)) / np.dtype(dtype).itemsize)
 
     elif isinstance(limit, str):
@@ -137,21 +133,23 @@
         else:
             raise RuntimeError()
 
     autodims = [i for i, c in enumerate(normalized_chunks) if c == "auto"]
 
     j = 0
     while len(autodims):
-        #autodims = [i for i in autodims if current_chunks[i] != maximum_chunks[i]]
+        # autodims = [i for i in autodims if current_chunks[i] != maximum_chunks[i]]
         if len(autodims) == 0:
             break
 
         j = j % len(autodims)
 
-        current_chunks[autodims[j]] = min(current_chunks[autodims[j]] + 1, shape[autodims[j]])
+        current_chunks[autodims[j]] = min(
+            current_chunks[autodims[j]] + 1, shape[autodims[j]]
+        )
 
         total = reduce(mul, current_chunks)
 
         if total > limit:
             current_chunks[autodims[j]] -= 1
             break
 
@@ -163,15 +161,15 @@
     chunks = ()
     for i, c in enumerate(normalized_chunks):
         if c == "auto":
             chunks += (current_chunks[i],)
         else:
             chunks += (c,)
 
-    #current_chunks = tuple(current_chunks)
+    # current_chunks = tuple(current_chunks)
     chunks = validate_chunks(shape, chunks, limit, dtype)
     return chunks
 
 
 def equal_sized_chunks(num_items: int, num_chunks: int = None, chunks: int = None):
     """
     Split an n integer into m (almost) equal integers, such that the sum of smaller integers equals n.
@@ -193,15 +191,17 @@
     if (num_chunks is not None) & (chunks is not None):
         raise RuntimeError()
 
     if (num_chunks is None) & (chunks is not None):
         num_chunks = (num_items + (-num_items % chunks)) // chunks
 
     if num_items < num_chunks:
-        raise RuntimeError("num_chunks may not be larger than num_items")
+        raise RuntimeError(
+            f"num_chunks ({num_chunks}) may not be larger than num_items ({num_items})"
+        )
 
     elif num_items % num_chunks == 0:
         return tuple([num_items // num_chunks] * num_chunks)
     else:
         v = []
         zp = num_chunks - (num_items % num_chunks)
         pp = num_items // num_chunks
@@ -213,10 +213,14 @@
         return tuple(v)
 
 
 def generate_chunks(
     num_items: int, num_chunks: int = None, chunks: int = None, start: int = 0
 ):
     for batch in equal_sized_chunks(num_items, num_chunks, chunks):
+        if num_items == 0:
+            break
+
         end = start + batch
+
         yield start, end
         start = end
```

### Comparing `abtem-1.0.4/abtem/core/colors.py` & `abtem-1.0.5/abtem/core/colors.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/core/config.py` & `abtem-1.0.5/abtem/core/config.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/core/electron_configurations.py` & `abtem-1.0.5/abtem/core/electron_configurations.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/core/energy.py` & `abtem-1.0.5/abtem/core/energy.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/core/ensemble.py` & `abtem-1.0.5/abtem/core/ensemble.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,39 +6,34 @@
 from functools import reduce, partial
 from typing import Tuple, List, Union, TYPE_CHECKING
 
 import dask.array as da
 import numpy as np
 
 from abtem.core import config
-#from abtem.core.axes import AxisMetadata, AxesMetadataList
+from abtem.core.axes import AxisMetadata, AxesMetadataList
 from abtem.core.chunks import (
     chunk_ranges,
     validate_chunks,
     Chunks,
 )
 from abtem.core.utils import tuple_range, interleave
 
-if TYPE_CHECKING:
-    from abtem.core.axes import AxisMetadata, AxesMetadataList
-
-
-def _wrap_with_array(x, ndims:int=None):
 
+def _wrap_with_array(x, ndims: int = None):
     if ndims is None:
         ndims = len(x.ensemble_shape)
 
     wrapped = np.zeros((1,) * ndims, dtype=object)
     wrapped.itemset(0, x)
     return wrapped
 
 
 def _wrap_args_with_array(*args, ndims):
     args = _wrap_with_array(args, ndims)
-    print(args)
     return args
 
 
 def unpack_blockwise_args(args):
     unpacked = ()
     for arg in args:
         if hasattr(arg, "item"):
@@ -56,19 +51,15 @@
 #     if ndims:
 #         return _wrap_with_array(new, len(new.ensemble_shape))
 #
 #     return new
 #
 
 
-
-
-
 class Ensemble:
-
     @property
     def ensemble_shape(self) -> tuple[int, ...]:
         """Shape of the ensemble axes."""
         return ()
 
     @property
     def ensemble_axes_metadata(self) -> list[AxisMetadata]:
@@ -139,15 +130,15 @@
 
         chunks = self._validate_ensemble_chunks(chunks)
 
         args = self._partition_args(chunks, lazy=True)
 
         out_symbols = tuple_range(sum(len(arg.shape) for arg in args))
 
-        #assert len(out_symbols) == max(len(self.ensemble_shape), 1)
+        # assert len(out_symbols) == max(len(self.ensemble_shape), 1)
 
         arg_symbols = ()
         offset = 0
         for arg in args:
             arg_symbols += (tuple_range(len(arg.shape), offset),)
             offset += len(arg.shape)
 
@@ -183,34 +174,34 @@
             if len(block.shape) > 1:
                 raise NotImplementedError
 
         for block_indices, start_stop in zip(
             itertools.product(*(range(block.shape[0]) for block in blocks)),
             itertools.product(*chunk_ranges(chunks)),
         ):
-
             block = tuple(block[i] for i, block in zip(block_indices, blocks))
             slics = tuple(slice(start, stop) for start, stop in start_stop)
 
             yield block_indices, slics, self._from_partitioned_args()(*block)
 
-    def _validate_ensemble_chunks(self, chunks: Chunks, limit: Union[str, int] = "auto"):
+    def _validate_ensemble_chunks(
+        self, chunks: Chunks, limit: Union[str, int] = "auto"
+    ):
         if chunks is None:
             chunks = self._default_ensemble_chunks
 
         chunks = validate_chunks(self.ensemble_shape, chunks, limit=limit)
         return chunks
 
     def _ensemble_chunks(
         self,
         max_batch: Union[str, int] = None,
         base_shape: Tuple[int, ...] = (),
         dtype=np.dtype("complex64"),
     ):
-
         shape = self.ensemble_shape
         chunks = self._default_ensemble_chunks
 
         if max_batch == "auto":
             max_batch = config.get("dask.chunk-size")
 
         if base_shape is not None:
@@ -244,15 +235,15 @@
         return self.__class__
 
     @property
     def ensemble_shape(self):
         return ()
 
 
-def concatenate_array_blocks(blocks):
+def concatenate_array_blocks(blocks) -> np.ndarray:
     for i in range(len(blocks.shape)):
         new_blocks = np.empty(blocks.shape[:-1], dtype=object)
 
         for indices in np.ndindex(blocks.shape):
             concat_index = len(indices) - 1
             indices = indices[:-1]
             new_blocks[indices] = np.concatenate(blocks[indices], axis=concat_index)
```

### Comparing `abtem-1.0.4/abtem/core/fft.py` & `abtem-1.0.5/abtem/core/fft.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from abtem.core import config
 from abtem.core.backend import get_array_module, check_cupy_is_installed
 from abtem.core.complex import complex_exponential
 from abtem.core.grid import spatial_frequencies
 from threadpoolctl import threadpool_limits
 import warnings
 
+from abtem.core.utils import get_dtype
 
 try:
     import pyfftw
 except (ModuleNotFoundError, ImportError):
     pyfftw = None
 
 try:
@@ -352,33 +353,30 @@
     normalization: str = "values",
     overwrite_x: bool = False,
 ):
     xp = get_array_module(array)
     old_size = np.prod(array.shape[-len(new_shape) :])
 
     is_complex = np.iscomplexobj(array)
-    array = array.astype(xp.complex64)
+
+    array = array.astype(get_dtype(complex=True))
 
     if len(new_shape) == 2:
         array = fft2(array, overwrite_x=overwrite_x)
         array = fft_crop(array, new_shape)
         array = ifft2(array, overwrite_x=overwrite_x)
     else:
         if len(new_shape) != len(array.shape):
             axes = tuple(range(len(array.shape) - len(new_shape), len(array.shape)))
         else:
             axes = tuple(range(len(array.shape)))
 
-        print(axes)
-
-        array = ifftn(
-            fft_crop(fftn(array, axes=axes), new_shape),
-            overwrite_x=overwrite_x,
-            axes=axes,
-        )
+        array = fftn(array, overwrite_x=overwrite_x, axes=axes)
+        array = fft_crop(array, new_shape)
+        array = ifftn(array, overwrite_x=overwrite_x, axes=axes)
 
     if not is_complex:
         array = array.real
 
     if normalization == "values":
         array *= np.prod(array.shape[-len(new_shape) :]) / old_size
```

### Comparing `abtem-1.0.4/abtem/core/grid.py` & `abtem-1.0.5/abtem/core/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from copy import copy
 from typing import Union, Sequence, Iterable, Any
 
 import numpy as np
 
 from abtem.core import config
 from abtem.core.backend import get_array_module, xp_to_str
-from abtem.core.utils import CopyMixin, EqualityMixin
+from abtem.core.utils import CopyMixin, EqualityMixin, get_dtype
 
 
 def validate_gpts(gpts):
     if not all(gpts):
         raise ValueError("gpts must be greater than 0")
 
 
@@ -67,15 +67,14 @@
         sampling: float | Sequence[float] = None,
         dimensions: int = 2,
         endpoint: bool | Sequence[bool] = False,
         lock_extent: bool = False,
         lock_gpts: bool = False,
         lock_sampling: bool = False,
     ):
-
         self._dimensions = dimensions
 
         if isinstance(endpoint, bool):
             endpoint = (endpoint,) * dimensions
 
         self._endpoint = tuple(endpoint)
 
@@ -144,15 +143,16 @@
     @property
     def extent(self) -> tuple[float, ...]:
         """Grid extent in each dimension [Å]."""
         return self._extent
 
     @extent.setter
     def extent(self, extent: float | Sequence[float]):
-        if self._lock_extent:
+        
+        if self._lock_extent and not np.allclose(extent, self.extent):
             raise RuntimeError("Extent cannot be modified")
 
         extent = self._validate(extent, dtype=float)
 
         if self._lock_sampling or (self.gpts is None):
             self._adjust_gpts(extent, self.sampling)
             self._adjust_sampling(extent, self.gpts)
@@ -341,14 +341,17 @@
             best_n = powers[0] ** np.ceil(np.log(n) / np.log(powers[0]))
             for power in powers[1:]:
                 best_n = min(power ** np.ceil(np.log(n) / np.log(power)), best_n)
             gpts += (best_n,)
 
         self.gpts = gpts
 
+    def spatial_frequencies(self):
+        return spatial_frequencies(self.gpts, self.sampling)
+
 
 class HasGridMixin:
     _grid: Grid
 
     @property
     def grid(self) -> Grid:
         """Simulation grid."""
@@ -378,26 +381,31 @@
         return self.grid.sampling
 
     @sampling.setter
     def sampling(self, sampling: tuple[float, ...]):
         self.grid.sampling = sampling
 
     @property
-    def reciprocal_space_sampling(self) -> tuple[float] | tuple[float, float] | tuple[float, ...]:
+    def reciprocal_space_sampling(
+        self,
+    ) -> tuple[float] | tuple[float, float] | tuple[float, ...]:
         """Reciprocal-space sampling in reciprocal Ångstrom."""
         return self.grid.reciprocal_space_sampling
 
     def match_grid(self, other: "HasGridMixin", check_match: bool = False):
         """Match the grid to another object with a Grid."""
         self.grid.match(other, check_match=check_match)
         return self
 
 
 def spatial_frequencies(
-    gpts: tuple[int, ...], sampling: tuple[float, ...], return_grid: bool = False, xp=np, dtype=np.float32
+    gpts: tuple[int, ...],
+    sampling: tuple[float, ...],
+    return_grid: bool = False,
+    xp=np,
 ):
     """
     Calculate spatial frequencies of a grid.
 
     Parameters
     ----------
     gpts: tuple of int
@@ -406,37 +414,43 @@
         Sampling of the potential [1 / Å].
 
     Returns
     -------
     tuple of arrays
     """
 
+    dtype = get_dtype(complex=False)
     xp = get_array_module(xp)
 
     out = ()
     for n, d in zip(gpts, sampling):
         out += (xp.fft.fftfreq(n, d).astype(dtype),)
 
     if return_grid:
         return xp.meshgrid(*out, indexing="ij")
     else:
         return out
 
 
 def polar_spatial_frequencies(
-    gpts: tuple[int, ...], sampling: tuple[float, ...], xp=np, dtype=np.float32
+    gpts: tuple[int, ...], sampling: tuple[float, ...], xp=np, dtype=None
 ) -> tuple[np.ndarray, np.ndarray]:
     xp = get_array_module(xp)
-    kx, ky = spatial_frequencies(gpts, sampling, False, xp_to_str(xp), dtype=dtype)
+    kx, ky = spatial_frequencies(gpts, sampling, False, xp_to_str(xp))
     k = xp.sqrt(kx[:, None] ** 2 + ky[None] ** 2)
     phi = xp.arctan2(ky[None], kx[:, None])
+
+    if dtype is not None:
+        k = k.astype(dtype)
+        phi = phi.astype(dtype)
+
     return k, phi
 
 
-def disc_meshgrid(r: int) -> np.ndarray:
+def disk_meshgrid(r: int) -> np.ndarray:
     """
     Return all indices inside a disk with a given radius.
 
     Parameters
     ----------
     r : int
         Radius of disc in pixels.
```

### Comparing `abtem-1.0.4/abtem/core/units.py` & `abtem-1.0.5/abtem/core/units.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,75 @@
+import numpy as np
+
 from abtem.core import config
+from abtem.core.energy import energy2wavelength
+
+categories = {
+    "real_space": ["Å", "Angstrom", "nm", "um", "mm", "m"],
+    "reciprocal_space": ["1/Å", "1/Angstrom", "1/nm", "1/um", "1/mm", "1/m"],
+    "angular": ["rad", "mrad", "deg"],
+    "energy": ["eV", "keV"],
+}
 
+# Use a dictionary comprehension to create the final mapping
 units_type = {
-    **dict(zip(("Å", "Angstrom", "nm", "um", "mm", "m"), ("real_space",) * 6)),
-    **dict(
-        zip(
-            ("1/Å", "1/Angstrom", "1/nm", "1/um", "1/mm", "1/m"),
-            ("reciprocal_space",) * 6,
-        )
-    ),
-    **dict(zip(("rad", "mrad", "deg",), ("angular",) * 3)),
-    **dict(
-        zip(
-            (
-                "eV",
-                "keV",
-            ),
-            ("energy",) * 2,
-        )
-    ),
+    unit: category for category, units in categories.items() for unit in units
 }
 
 _conversion_factors = {
     "Å": 1,
     "nm": 1e-1,
     "um": 1e-4,
     "mm": 1e-7,
     "m": 1e-10,
     "1/Å": 1,
     "1/nm": 10,
     "1/um": 1e4,
     "1/mm": 1e7,
     "1/m": 1e10,
+    "mrad": 1,
+    "rad": 1e3,
+    "deg": 1e3 / np.pi * 180.0,
 }
+
 _tex_units = {
     "Å": "\mathrm{\AA}",
     "nm": "\mathrm{nm}",
     "um": "\mathrm{\mu m}",
     "mm": "\mathrm{mm}",
     "m": "\mathrm{mm}",
-    "1/Å": "\AA^{-1}",
+    "1/Å": "\mathrm{\AA}^{-1}",
     "1/nm": "\mathrm{nm}^{-1}",
     "1/um": "\mathrm{\mu m}^{-1}",
     "1/mm": "\mathrm{mm}^{-1}",
     "1/m": "\mathrm{m}^{-1}",
     "mrad": "\mathrm{mrad}",
     "deg": "\mathrm{deg}",
-    "e/Å^2": "\mathrm{e}^-/\mathrm{\AA}^2"
+    "e/Å^2": "\mathrm{e}^-/\mathrm{\AA}^2",
 }
 
 
 def _format_units(units):
-    if config.get("visualize.use_tex", False):
-        units = _tex_units.get(units, f'\mathrm{{{units}}}')
+    
+    if config.get("visualize.use_tex", False) is True:
+        try:
+            units = _tex_units[units]
+        except KeyError:
+            if units == "%":
+                units = "\mathrm{\%}"
+                # TODO: temporary fix for the percent sign
+            else:
+                units = f"\mathrm{{{units}}}"
+        
         return f"${units}$"
     else:
         return units
 
 
-def _validate_units(units, old_units):
-
+def _validate_units(units, old_units=None):
     if old_units is None and units is None:
         return None
     elif units is None:
         units = old_units
     elif units is not None and old_units is not None:
         if units_type[units] != units_type[old_units]:
             raise RuntimeError(f"cannot convert units {old_units} to {units}")
@@ -88,9 +95,22 @@
         return units
     elif units_type[units] == "angular":
         return units
     else:
         raise NotImplementedError
 
 
-def _get_conversion_factor(units, old_units):
+def _get_conversion_factor(units: str, old_units: str, energy: float = None):
+    if units is None:
+        return 1.0
+
+    if units_type[old_units] == "reciprocal_space" and units_type[units] == "angular":
+        if energy is None:
+            raise RuntimeError("")
+
+        wavelength = energy2wavelength(energy)
+        conversion = (
+            wavelength * 1e3 * _conversion_factors[_validate_units(units, "mrad")]
+        )
+        return conversion
+
     return _conversion_factors[_validate_units(units, old_units)]
```

### Comparing `abtem-1.0.4/abtem/core/utils.py` & `abtem-1.0.5/abtem/core/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 """Module for various convenient utilities."""
 from __future__ import annotations
+
 import copy
 import inspect
+import itertools
+import os
 import warnings
-from typing import Tuple
 
 import numpy as np
 
-from abtem.core.backend import get_array_module
-import dask.array as da
 from abtem.core.backend import cp
-
+from abtem.core.backend import get_array_module
+from abtem.core.config import config
 
 
 def is_array_like(x):
     if isinstance(x, np.ndarray) or (cp is not None and isinstance(x, cp.ndarray)):
         return True
     else:
         return False
 
 
+def is_broadcastable(shape1, shape2):
+    for a, b in zip(shape1[::-1], shape2[::-1]):
+        if a == 1 or b == 1 or a == b:
+            pass
+        else:
+            return False
+    return True
+
+
 class CopyMixin:
     _exclude_from_copy: tuple = ()
 
     def _arg_keys(self, cls):
         parameters = inspect.signature(cls).parameters
         return tuple(
             key
@@ -42,42 +52,44 @@
 
     def copy(self):
         """Make a copy."""
         return copy.deepcopy(self)
 
 
 def safe_equality(a, b, exclude: tuple[str, ...] = ()) -> bool:
-
     if not isinstance(b, a.__class__):
         return False
 
     for key, value in a.__dict__.items():
-
         if key in exclude:
             continue
 
         try:
             equal = value == b.__dict__[key]
         except (KeyError, TypeError, ValueError):
             return False
 
         from abtem.core.ensemble import EmptyEnsemble
-        if isinstance(value, EmptyEnsemble) and isinstance(b.__dict__[key], EmptyEnsemble):
+
+        if isinstance(value, EmptyEnsemble) and isinstance(
+            b.__dict__[key], EmptyEnsemble
+        ):
             return True
 
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=np.VisibleDeprecationWarning)
 
             try:
                 equal = np.allclose(value, b.__dict__[key])
 
             except (ValueError, TypeError):
                 if isinstance(value, EqualityMixin):
                     equal = safe_equality(value, b.__dict__[key])
 
+        # print(equal, key, b.__dict__[key], a.__dict__[key])
         if equal is False:
             return False
 
     return True
 
 
 class EqualityMixin:
@@ -116,17 +128,35 @@
             break
 
         if a1 is True and a2 is True:
             match_axis1.insert(len(match_axis1) - i, None)
             break
 
 
-def normalize_axes(dims, shape: tuple[int, ...]):
-    num_dims = len(shape)
-    return tuple(dim if dim >= 0 else num_dims + dim for dim in dims)
+def normalize_axes(axes, shape):
+    """
+    Normalize the axes tuple so that all axes are non-negative.
+
+    Parameters:
+    - shape: The shape of the numpy array (as returned by np.shape())
+    - axes: A tuple or integer representing the axes. Can contain negative indices.
+
+    Returns:
+    - A tuple with normalized axes.
+    """
+    ndim = len(shape)
+
+    # Ensure that 'axes' is a tuple
+    if not isinstance(axes, tuple):
+        axes = (axes,)
+
+    # Normalize negative indices
+    normalized_axes = tuple(axis if axis >= 0 else axis + ndim for axis in axes)
+
+    return normalized_axes
 
 
 def _get_dims_to_broadcast(
     arr1: np.ndarray,
     arr2: np.ndarray,
     match_dims: list[tuple[int, ...], tuple[int, ...]] = None,
 ) -> tuple[tuple[int, ...], tuple[int, ...]]:
@@ -164,15 +194,14 @@
 
 def expand_dims_to_broadcast(
     arr1: np.ndarray,
     arr2: np.ndarray,
     match_dims: list[tuple[int, ...], tuple[int, ...]] = None,
     broadcast: bool = False,
 ):
-
     xp = get_array_module(arr1)
 
     axis1, axis2 = _get_dims_to_broadcast(arr1, arr2, match_dims)
 
     arr1 = xp.expand_dims(arr1, axis=axis1)
     arr2 = xp.expand_dims(arr2, axis=axis2)
 
@@ -188,21 +217,45 @@
     return tuple(range(offset, offset + length))
 
 
 def interleave(l1: list | tuple, l2: list | tuple):
     return tuple(val for pair in zip(l1, l2) for val in pair)
 
 
+def flatten_list_of_lists(l):
+    return list(itertools.chain(*l))
+
+
 def label_to_index(labels, max_label=None):
     if max_label is None:
         max_label = np.max(labels)
 
     xp = get_array_module(labels)
     labels = labels.flatten()
     labels_order = labels.argsort()
     sorted_labels = labels[labels_order]
     indices = xp.arange(0, len(labels) + 1)[labels_order]
     index = xp.arange(0, max_label + 1)
     lo = xp.searchsorted(sorted_labels, index, side="left")
     hi = xp.searchsorted(sorted_labels, index, side="right")
     for i, (l, h) in enumerate(zip(lo, hi)):
         yield indices[l:h]
+
+
+def get_data_path(file):
+    this_file = os.path.abspath(os.path.dirname(file))
+    return os.path.join(this_file, "data")
+
+
+def get_dtype(complex):
+    dtype = config.get("precision")
+
+    if dtype == "float32" and complex:
+        return np.complex64
+    elif dtype == "float32":
+        return np.float32
+    elif dtype == "float64" and complex:
+        return np.complex128
+    elif dtype == "float64":
+        return np.float64
+    else:
+        raise RuntimeError("")
```

### Comparing `abtem-1.0.4/abtem/detectors.py` & `abtem-1.0.5/abtem/detectors.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,30 +8,32 @@
 
 import numpy as np
 
 from abtem.array import T
 from abtem.core.axes import ReciprocalSpaceAxis, RealSpaceAxis, LinearAxis, AxisMetadata
 from abtem.core.backend import get_array_module
 from abtem.core.chunks import Chunks
+from abtem.core.energy import energy2wavelength
 from abtem.core.ensemble import _wrap_with_array
 from abtem.measurements import (
     DiffractionPatterns,
     PolarMeasurements,
     Images,
     RealSpaceLineProfiles,
     _scanned_measurement_type,
-    _polar_detector_bins, _scan_shape,
+    _polar_detector_bins,
+    _scan_shape,
+    _scan_axes,
 )
 from abtem.transform import ArrayObjectTransform
-from abtem.visualize import discrete_cmap
+from abtem.visualize.visualizations import discrete_cmap
 
 if TYPE_CHECKING:
     from abtem.waves import BaseWaves, Waves
     from abtem.measurements import BaseMeasurements
-    from abtem.visualize import MeasurementVisualization2D
 
 
 def _validate_detectors(
     detectors: BaseDetector | list[BaseDetector],
 ) -> list[BaseDetector]:
     if hasattr(detectors, "detect"):
         detectors = [detectors]
@@ -39,15 +41,14 @@
     elif detectors is None:
         detectors = [WavesDetector()]
 
     elif not (
         isinstance(detectors, list)
         and all(hasattr(detector, "detect") for detector in detectors)
     ):
-
         raise RuntimeError(
             "Detectors must be AbstractDetector or list of AbstractDetector."
         )
 
     return detectors
 
 
@@ -176,15 +177,14 @@
         self,
         inner: float,
         outer: float,
         offset: tuple[float, float] = (0.0, 0.0),
         to_cpu: bool = True,
         url: str = None,
     ):
-
         self._inner = inner
         self._outer = outer
         self._offset = offset
         super().__init__(to_cpu=to_cpu, url=url)
 
     @property
     def inner(self) -> float:
@@ -224,22 +224,34 @@
         if self.outer is not None:
             outer = self.outer
         else:
             outer = min(waves.cutoff_angles)
 
         return inner, outer
 
+    def _out_ensemble_axes_metadata(
+        self, waves: BaseWaves, index: int = 0
+    ) -> list[AxisMetadata]:
+        source = _scan_axes(waves)
+        scan_axes_metadata = [waves.ensemble_axes_metadata[i] for i in source]
+        ensemble_axes_metadata = [
+            m for i, m in enumerate(waves.ensemble_axes_metadata) if i not in source
+        ]
+        return ensemble_axes_metadata + scan_axes_metadata
+
     def _out_base_axes_metadata(
         self, waves: BaseWaves, index: int = 0
     ) -> list[AxisMetadata]:
+        # source = _scan_axes(waves)
+        # scan_axes_metadata = [waves.ensemble_axes_metadata[i] for i in source]
         return []
 
     def _out_ensemble_shape(self, waves: BaseWaves, index: int = 0) -> tuple:
-        ensemble_shape = super()._out_ensemble_shape(waves, index) # noqa
-        return ensemble_shape[:-len(_scan_shape(waves))]
+        ensemble_shape = super()._out_ensemble_shape(waves, index)  # noqa
+        return ensemble_shape[: -len(_scan_shape(waves))]
 
     def _out_base_shape(self, waves: BaseWaves, index: int = 0) -> tuple:
         return _scan_shape(waves)
 
     def _out_dtype(self, array_object, index: int = 0) -> np.dtype.base:
         return np.float32
 
@@ -287,20 +299,19 @@
         waves : Waves
             The waves to detect.
 
         Returns
         -------
         measurement : Images
         """
-        return self.apply(waves) # noqa
+        return self.apply(waves)  # noqa
 
     def _get_detector_region_array(
         self, waves: BaseWaves, fftshift: bool = True
     ) -> np.ndarray:
-
         array = _polar_detector_bins(
             gpts=waves._gpts_within_angle("cutoff"),
             sampling=waves.angular_sampling,
             inner=self.inner,
             outer=self.outer,
             nbins_radial=1,
             nbins_azimuthal=1,
@@ -383,32 +394,32 @@
 
     @property
     @abstractmethod
     def azimuthal_sampling(self):
         """Spacing between the azimuthal detector bins [mrad]."""
         pass
 
+    @property
     @abstractmethod
-    def _calculate_nbins_radial(self, waves: BaseWaves):
+    def nbins_radial(self):
+        """Spacing between the azimuthal detector bins [mrad]."""
         pass
 
+    @property
     @abstractmethod
-    def _calculate_nbins_azimuthal(self, waves: BaseWaves):
+    def nbins_azimuthal(self):
+        """Spacing between the azimuthal detector bins [mrad]."""
         pass
 
     def _out_dtype(self, waves: Waves, index: bool = 0):
         return np.float32
 
     def _out_base_shape(self, waves: Waves, index: bool = 0):
-        shape = (
-            self._calculate_nbins_radial(waves),
-            self._calculate_nbins_azimuthal(waves),
-        )
-
-        return shape
+        self._match_waves(waves)
+        return self.nbins_radial, self.nbins_azimuthal
 
     def _out_type(self, waves: Waves, index: bool = 0):
         return PolarMeasurements
 
     def _out_metadata(self, waves: Waves, index: bool = 0) -> dict:
         metadata = super()._out_metadata(waves)
         metadata["label"] = "intensity"
@@ -460,41 +471,45 @@
         measurement : PolarMeasurements
         """
         inner, outer = self.angular_limits(waves)
 
         measurement = waves.diffraction_patterns(max_angle="cutoff", parity="same")
 
         measurement = measurement.polar_binning(
-            nbins_radial=self._calculate_nbins_radial(waves),
-            nbins_azimuthal=self._calculate_nbins_azimuthal(waves),
+            nbins_radial=self.nbins_radial,
+            nbins_azimuthal=self.nbins_azimuthal,
             inner=inner,
             outer=outer,
             rotation=self._rotation,
             offset=self._offset,
         )
 
         if self.to_cpu:
             measurement = measurement.to_cpu()
 
         return measurement.array
 
+    def _match_waves(self, waves):
+        if self.outer is None:
+            self._outer = min(waves.cutoff_angles)
+
     def detect(self, waves: Waves) -> PolarMeasurements:
         """
         Detect the given waves producing polar measurements.
 
         Parameters
         ----------
         waves : Waves
             The waves to detect.
 
         Returns
         -------
         measurement : PolarMeasurements
         """
-        return self.apply(waves) # noqa
+        return self.apply(waves)  # noqa
 
     def get_detector_regions(self, waves: BaseWaves = None):
         """
         Get the polar detector regions as a polar measurement.
 
         Parameters
         ----------
@@ -502,25 +517,16 @@
             The waves to derive the polar detector regions from.
 
         Returns
         -------
         detector_region : PolarMeasurements
         """
 
-        bins = np.arange(
-            0,
-            self._calculate_nbins_radial(waves)
-            * self._calculate_nbins_azimuthal(waves),
-        )
-        bins = bins.reshape(
-            (
-                self._calculate_nbins_radial(waves),
-                self._calculate_nbins_azimuthal(waves),
-            )
-        )
+        bins = np.arange(0, self.nbins_radial * self.nbins_azimuthal)
+        bins = bins.reshape((self.nbins_radial, self.nbins_azimuthal))
 
         metadata = copy(waves.metadata)
         metadata.update({"label": "detector regions", "units": ""})
 
         polar_measurements = PolarMeasurements(
             bins,
             radial_sampling=self.radial_sampling,
@@ -528,33 +534,104 @@
             radial_offset=self.inner,
             metadata=metadata,
             azimuthal_offset=self._rotation,
         )
 
         return polar_measurements
 
-    def show(self, waves: BaseWaves = None, **kwargs):
+    def show(
+        self,
+        waves: BaseWaves = None,
+        gpts: int | tuple[int, int] = None,
+        sampling: float | tuple[int, int] = None,
+        energy: float = None,
+        **kwargs,
+    ):
         """
         Show the segmented detector regions as a polar plot.
 
         Parameters
         ----------
         waves : BaseWaves
             The waves to derive the segmented detector regions from.
+        gpts : two int, optional
+            Number of grid points describing the wave functions to be detected.
+        sampling : two float, optional
+            Lateral sampling of the wave functions to be detected [1 / Å].
+        energy : float, optional
+            Electron energy of the wave functions to be detected [eV].
         kwargs :
-            Optional keyword arguments for PolarMeasurements.show.
+            Optional keyword arguments for DiffractionPatterns.show.
 
         Returns
         -------
-        visualization : MeasurementVisualization2D
+        visualization : Visualization
         """
 
-        num_colors = self._calculate_nbins_radial(
-            waves
-        ) * self._calculate_nbins_azimuthal(waves)
+        if waves is not None:
+            if gpts is not None or sampling is not None or energy is not None:
+                raise ValueError(
+                    "provide either waves or 'gpts', 'sampling' and 'energy'"
+                )
+            segmented_regions = self.get_detector_regions(waves)
+            diffraction_patterns = segmented_regions.to_diffraction_patterns(waves.gpts)
+
+        elif energy is None:
+            raise ValueError("provide the waves or the energy of waves")
+        else:
+            if gpts is None:
+                gpts = 1024
+
+            if not hasattr(gpts, "__len__"):
+                gpts = (gpts,) * 2
+
+            if sampling is None:
+                angular_sampling = (
+                    self.outer / gpts[0] * 2 * 1.1,
+                    self.outer / gpts[1] * 2 * 1.1,
+                )
+                reciprocal_space_sampling = (
+                    angular_sampling[0] / (energy2wavelength(energy) * 1e3),
+                    angular_sampling[1] / (energy2wavelength(energy) * 1e3),
+                )
+            else:
+                if not hasattr(sampling, "__len__"):
+                    sampling = (sampling,) * 2
+
+                reciprocal_space_sampling = 1 / (gpts[0] * sampling[0]), 1 / (
+                    gpts[0] * sampling[0]
+                )
+                angular_sampling = (
+                    reciprocal_space_sampling[0] * energy2wavelength(energy) * 1e3,
+                    reciprocal_space_sampling[1] * energy2wavelength(energy) * 1e3,
+                )
+
+            regions = _polar_detector_bins(
+                gpts=gpts,
+                sampling=angular_sampling,
+                inner=self.inner,
+                outer=self.outer,
+                nbins_radial=self.nbins_radial,
+                nbins_azimuthal=self.nbins_azimuthal,
+                fftshift=True,
+                rotation=self.rotation,
+                offset=(0.0, 0.0),
+                return_indices=False,
+            )
+            
+            regions = regions.astype(np.float32)
+            regions[..., regions < 0] = np.nan
+
+            diffraction_patterns = DiffractionPatterns(
+                regions, sampling=reciprocal_space_sampling, metadata={"energy": energy}
+            )
+
+        n_bins_radial = self.nbins_radial
+        n_bins_azimuthal = self.nbins_azimuthal
+        num_colors = n_bins_radial * n_bins_azimuthal
 
         if "cmap" not in kwargs:
             if num_colors <= 10:
                 kwargs["cmap"] = "tab10"
             else:
                 kwargs["cmap"] = "tab20"
 
@@ -565,19 +642,15 @@
 
         if "vmax" not in kwargs:
             kwargs["vmax"] = num_colors - 0.5
 
         if "units" not in kwargs:
             kwargs["units"] = "mrad"
 
-        segmented_regions = self.get_detector_regions(waves).to_diffraction_patterns(
-            waves.gpts
-        )
-
-        return segmented_regions.show(**kwargs)
+        return diffraction_patterns.show(**kwargs)
 
 
 class FlexibleAnnularDetector(_AbstractRadialDetector):
     """
     The flexible annular detector allows choosing the integration limits after running the simulation by binning the
     intensity in annular integration regions.
 
@@ -613,14 +686,22 @@
             rotation=0.0,
             offset=(0.0, 0.0),
             to_cpu=to_cpu,
             url=url,
         )
 
     @property
+    def nbins_radial(self):
+        return int(np.floor(self.outer - self.inner) / self.step_size)
+
+    @property
+    def nbins_azimuthal(self):
+        return 1
+
+    @property
     def step_size(self) -> float:
         """Step size [mrad]."""
         return self._step_size
 
     @step_size.setter
     def step_size(self, value: float):
         self._step_size = value
@@ -629,24 +710,17 @@
     def radial_sampling(self) -> float:
         return self.step_size
 
     @property
     def azimuthal_sampling(self) -> float:
         return 2 * np.pi
 
-    def _calculate_nbins_radial(self, waves: Waves) -> int:
-        if self.outer is None:
-            outer = min(waves.cutoff_angles)
-        else:
-            outer = self.outer
-
-        return int(np.floor(outer - self.inner) / self.step_size)
-
-    def _calculate_nbins_azimuthal(self, waves: Waves) -> int:
-        return 1
+    def detect(self, waves: Waves) -> PolarMeasurements:
+        self._match_waves(waves)
+        return super().detect(waves)
 
 
 class SegmentedDetector(_AbstractRadialDetector):
     """
     The segmented detector covers an annular angular range, and is partitioned into several integration regions
     divided to radial and angular segments. This can be used for simulating differential phase contrast (DPC)
     imaging.
@@ -722,20 +796,14 @@
         """Number of angular bins."""
         return self._nbins_azimuthal
 
     @nbins_azimuthal.setter
     def nbins_azimuthal(self, value: float):
         self._nbins_azimuthal = value
 
-    def _calculate_nbins_radial(self, waves: Waves = None):
-        return self.nbins_radial
-
-    def _calculate_nbins_azimuthal(self, waves: Waves = None):
-        return self.nbins_azimuthal
-
 
 class PixelatedDetector(BaseDetector):
     """
     The pixelated detector records the intensity of the Fourier-transformed exit wave function, i.e. the diffraction
     patterns. This may be used for example for simulating 4D-STEM.
 
     Parameters
@@ -826,23 +894,23 @@
             return [
                 ReciprocalSpaceAxis(
                     sampling=sampling[0],
                     offset=-(gpts[0] // 2) * sampling[0],
                     label="kx",
                     units="1/Å",
                     fftshift=True,
-                    _tex_label="$k_x$",
+                    tex_label="$k_x$",
                 ),
                 ReciprocalSpaceAxis(
                     sampling=sampling[1],
                     offset=-(gpts[1] // 2) * sampling[1],
                     label="ky",
                     units="1/Å",
                     fftshift=True,
-                    _tex_label="$k_y$",
+                    tex_label="$k_y$",
                 ),
             ]
         else:
             return [
                 RealSpaceAxis(label="x", sampling=waves.sampling[0], units="Å"),
                 RealSpaceAxis(label="y", sampling=waves.sampling[1], units="Å"),
             ]
@@ -894,15 +962,15 @@
         waves : Waves
             The waves to detect.
 
         Returns
         -------
         measurement : DiffractionPatterns
         """
-        return self.apply(waves) # noqa
+        return self.apply(waves)  # noqa
 
 
 class WavesDetector(BaseDetector):
     """
     Detect the complex wave functions.
 
     Parameters
@@ -926,15 +994,14 @@
 
     def _out_metadata(self, waves: Waves, index=0) -> dict:
         metadata = super()._out_metadata(array_object=waves, index=index)
         metadata["reciprocal_space"] = False
         return metadata
 
     def _calculate_new_array(self, waves):
-
         waves = waves.ensure_real_space()
 
         if self.to_cpu:
             waves = waves.to_cpu()
 
         return waves.array
```

### Comparing `abtem-1.0.4/abtem/distributions.py` & `abtem-1.0.5/abtem/distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for describing distributions of simulation parameters."""
+
 from __future__ import annotations
 
 from abc import abstractmethod, ABCMeta
 from functools import partial
 from numbers import Number
 from typing import Sequence, Iterable, Iterator
 
@@ -356,31 +357,58 @@
                 values=values, weights=weights, ensemble_mean=ensemble_mean[i]
             )
         )
 
     return MultidimensionalDistribution(distributions=distributions)
 
 
-def _validate_distribution(
+def validate_distribution(
     distribution: BaseDistribution | Iterable | Number,
 ) -> BaseDistribution | Number:
+    """
+    Parameters
+    ----------
+    distribution : BaseDistribution or Iterable or Number
+        The input distribution to be validated.
 
-    if isinstance(distribution, (BaseDistribution, Number)):
+    Returns
+    -------
+    BaseDistribution or Number
+        The validated distribution. If the input distribution is already a
+        valid distribution, it is returned as is. If the input distribution is
+        a single number, it is returned unchanged. If the input distribution is
+        an ndarray with shape (0,), its single element is returned. If the input
+        distribution is a tuple, list, or ndarray, it is converted to an ndarray
+        and wrapped into a DistributionFromValues object where each value has
+        equal weight. Otherwise, a ValueError is raised.
+
+    Raises
+    ------
+    ValueError
+        If the input distribution is not a valid distribution or .
+    """
+    if isinstance(distribution, (BaseDistribution, Number, str)):
         return distribution
 
     if isinstance(distribution, np.ndarray) and len(distribution.shape) == 0:
         return distribution.item()
 
     if isinstance(distribution, (tuple, list, np.ndarray)):
-        distribution = np.array(distribution)
+        try:
+            distribution = np.array(distribution)
+        except ValueError:
+            distribution = np.array(distribution, dtype=object)
+
         return DistributionFromValues(
             distribution, np.ones_like(distribution, dtype=np.float32)
         )
 
-    raise ValueError(f"value {distribution} is not a valid distribution")
+    raise ValueError(
+        f"value {distribution} is not a single number or could not be converted to a valid distribution"
+    )
 
 
 def _unpack_distributions(
     *args: float | BaseDistribution, shape: tuple, xp: ArrayModule = np
 ):
     if len(args) == 0:
         return (), 1.0
```

### Comparing `abtem-1.0.4/abtem/inelastic/phonons.py` & `abtem-1.0.5/abtem/inelastic/phonons.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/inelastic/plasmons.py` & `abtem-1.0.5/abtem/inelastic/plasmons.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/integrals.py` & `abtem-1.0.5/abtem/integrals.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,44 +2,67 @@
 
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from typing import TYPE_CHECKING
 
 import numpy as np
+from ase import Atoms
+from ase.data import chemical_symbols
 from numba import jit
 from scipy import integrate
 from scipy.interpolate import interp1d
 from scipy.optimize import brentq, fsolve
 from scipy.special import erf
 
-from abtem.core.backend import cp, get_array_module
+from abtem.core.backend import (
+    cp,
+    get_array_module,
+    get_scipy_module,
+    get_ndimage_module,
+)
 from abtem.core.backend import cupyx
 from abtem.core.backend import device_name_from_array_module
 from abtem.core.fft import fft2, ifft2
-from abtem.core.grid import disc_meshgrid
+from abtem.core.grid import disk_meshgrid
 from abtem.core.grid import polar_spatial_frequencies
 from abtem.core.grid import spatial_frequencies
-from abtem.core.utils import EqualityMixin, CopyMixin
+from abtem.core.utils import EqualityMixin, CopyMixin, get_dtype
 from abtem.parametrizations import validate_parametrization
 
 if cp is not None:
     from abtem.core._cuda import (
         interpolate_radial_functions as interpolate_radial_functions_cuda,
     )
 else:
     interpolate_radial_functions_cuda = None
 
 if TYPE_CHECKING:
     from abtem.parametrizations import Parametrization
 
 
-class ProjectionIntegrator:
-    """Base class for projection integrator object used for calculating projection integrals of radial potentials."""
+class FieldIntegrator(EqualityMixin, CopyMixin, metaclass=ABCMeta):
+    """Base class for projection integrator object used for calculating projection integrals of radial potentials.
 
+    Parameters
+    ----------
+    periodic : bool
+        True indicates that the projection integrals are periodic perpendicular to the projection direction.
+    finite : bool
+        True indicates that the projection integrals are finite along the projection direction.
+    retain_data : bool, optional
+        If True, intermediate calculations are kept.
+    """
+
+    def __init__(self, periodic: bool, finite: bool, retain_data: bool = False):
+        self._periodic = periodic
+        self._finite = finite
+        self._retain_data = retain_data
+
+    @abstractmethod
     def integrate_on_grid(
         self,
         positions: np.ndarray,
         a: np.ndarray,
         b: np.ndarray,
         gpts: tuple[int, int],
         sampling: tuple[float, float],
@@ -50,96 +73,93 @@
         only used when the integration method is finite.
 
         Parameters
         ----------
         positions : np.ndarray
             2D array of xy-positions of the centers of each radial function [Å].
         a : np.ndarray
-            Lower integration limit of the projection integrals along z for each position [Å]. The limit is given
+            Lower integration limit of the pr
+            ojection integrals along z for each position [Å]. The limit is given
             relative to the center of the radial function.
         b : np.ndarray
             Upper integration limit of the projection integrals along z for each position [Å]. The limit is given
             relative to the center of the radial function.
         gpts : two int
             Number of grid points in `x` and `y` describing each slice of the potential.
         sampling : two float
             Sampling of the potential in `x` and `y` [1 / Å].
         device : str, optional
             The device used for calculating the potential, 'cpu' or 'gpu'. The default is determined by the user
             configuration file.
         """
         pass
 
-
-class ProjectionIntegratorPlan(EqualityMixin, CopyMixin, metaclass=ABCMeta):
-    """
-    The ProjectionIntegratorPlan facilitates the creation of :class:`.ProjectionIntegrator` objects using the ``.build``
-    method given a grid and a chemical symbol.
-
-    Parameters
-    ----------
-    periodic : bool
-        True indicates that the projection integrals are periodic perpendicular to the projection direction.
-    finite : bool
-        True indicates that the projection integrals are finite along the projection direction.
-    """
-
-    def __init__(self, periodic: bool, finite: bool):
-        self._periodic = periodic
-        self._finite = finite
-
     @property
     def periodic(self) -> bool:
         """True indicates that the created projection integrators are implemented only for periodic potentials."""
         return self._periodic
 
     @property
     def finite(self) -> bool:
         """True indicates that the created projection integrators are implemented only for infinite potential
         projections."""
         return self._finite
 
-    @abstractmethod
-    def build(
-        self,
-        symbol: str,
-        gpts: tuple[int, int],
-        sampling: tuple[float, float],
-        device: str,
-    ) -> ProjectionIntegrator:
-        """
-        Build projection integrator for given chemical symbol, grid and device.
-
-        Parameters
-        ----------
-        symbol : str
-            Chemical symbol to build the projection integrator for.
-        gpts : two int
-            Number of grid points in `x` and `y` describing each slice of the potential.
-        sampling : two float
-            Sampling of the potential in `x` and `y` [1 / Å].
-        device : str, optional
-            The device used for calculating the potential, 'cpu' or 'gpu'. The default is determined by the user
-            configuration file.
-
-        Returns
-        -------
-        projection_integrator : ProjectionIntegrator
-            The projection integrator for the specified chemical symbol.
-        """
-
-        pass
+    # @abstractmethod
+    # def build(
+    #     self,
+    #     symbol: str,
+    #     gpts: tuple[int, int],
+    #     sampling: tuple[float, float],
+    #     device: str,
+    # ):
+    #     """
+    #     Build projection integrator for given chemical symbol, grid and device.
+    #
+    #     Parameters
+    #     ----------
+    #     symbol : str
+    #         Chemical symbol to build the projection integrator for.
+    #     gpts : two int
+    #         Number of grid points in `x` and `y` describing each slice of the potential.
+    #     sampling : two float
+    #         Sampling of the potential in `x` and `y` [1 / Å].
+    #     device : str, optional
+    #         The device used for calculating the potential, 'cpu' or 'gpu'. The default is determined by the user
+    #         configuration file.
+    #
+    #     Returns
+    #     -------
+    #     projection_integrator : ProjectionIntegrator
+    #         The projection integrator for the specified chemical symbol.
+    #     """
+    #     pass
 
     @abstractmethod
     def cutoff(self, symbol: str) -> float:
         """Radial cutoff of the potential for the given chemical symbol."""
         pass
 
 
-class GaussianScatteringFactors(ProjectionIntegrator):
+# class ProjectionIntegratorPlan(EqualityMixin, CopyMixin, metaclass=ABCMeta):
+#     """
+#     The ProjectionIntegratorPlan facilitates the creation of :class:`.ProjectionIntegrator` objects using the ``.build``
+#     method given a grid and a chemical symbol.
+#
+#     Parameters
+#     ----------
+#
+#     """
+#
+#     def __init__(self, periodic: bool, finite: bool):
+#         self._periodic = periodic
+#         self._finite = finite
+
+
+class GaussianScatteringFactors(FieldIntegrator):
     def __init__(
         self,
         gaussian_scattering_factors,
         error_function_scales,
         correction_scattering_factors,
     ):
         self._gaussian_scattering_factors = gaussian_scattering_factors
@@ -200,15 +220,14 @@
         a: np.ndarray,
         b: np.ndarray,
         gpts: tuple[int, int],
         sampling: tuple[float, float],
         device: str = "cpu",
         fourier_space: bool = False,
     ) -> np.ndarray:
-
         shape = self._gaussian_scattering_factors.shape[-2:]
 
         assert gpts == shape
 
         array = self._integrate_gaussian_scattering_factors(
             positions, a, b, sampling, device
         )
@@ -220,15 +239,15 @@
 
         if fourier_space:
             return array
         else:
             return ifft2(array / sinc(shape, sampling, device)).real
 
 
-class GaussianProjectionIntegrals(ProjectionIntegratorPlan):
+class GaussianProjectionIntegrals(FieldIntegrator):
     """
     Parameters
     ----------
     gaussian_parametrization : str or Parametrization, optional
         The Gaussian radial potential parametrization to integrate. Must be parametrization described by a superposition
         of Gaussians. Default is the Peng parametrization.
     correction_parametrization : str or Parametrization, optional
@@ -240,15 +259,14 @@
 
     def __init__(
         self,
         gaussian_parametrization: str | Parametrization = "peng",
         correction_parametrization: str | Parametrization = "lobato",
         cutoff_tolerance: float = 1e-3,
     ):
-
         self._gaussian_parametrization = validate_parametrization(
             gaussian_parametrization
         )
 
         if correction_parametrization is not None:
             self._correction_parametrization = validate_parametrization(
                 correction_parametrization
@@ -256,14 +274,18 @@
         else:
             self._correction_parametrization = correction_parametrization
 
         self._cutoff_tolerance = cutoff_tolerance
 
         super().__init__(periodic=True, finite=True)
 
+        self._gaussian_scattering_factors = None
+        self._error_function_scales = None
+        self._correction_scattering_factors = None
+
     @property
     def cutoff_tolerance(self):
         """The error tolerance used for deciding the radial cutoff distance of the potential [eV / e]."""
         return self._cutoff_tolerance
 
     @property
     def gaussian_parametrization(self):
@@ -376,142 +398,146 @@
     shape = array.shape
 
     positions = xp.array(positions)
 
     if round_positions:
         rounded = xp.round(positions).astype(xp.int32)
         i, j = rounded[:, 0][None] % shape[0], rounded[:, 1][None] % shape[1]
-        v = xp.array([1.0], dtype=xp.float32)[:, None]
+        v = xp.array([1.0], dtype=get_dtype(complex=False))[:, None]
     else:
         rounded = xp.floor(positions).astype(xp.int32)
         rows, cols = rounded[:, 0], rounded[:, 1]
         x = positions[:, 0] - rows
         y = positions[:, 1] - cols
         xy = x * y
         i = xp.array([rows % shape[0], (rows + 1) % shape[0]] * 2)
         j = xp.array([cols % shape[1]] * 2 + [(cols + 1) % shape[1]] * 2)
-        v = xp.array([1 + xy - y - x, x - xy, y - xy, xy], dtype=xp.float32)
+        v = xp.array(
+            [1 + xy - y - x, x - xy, y - xy, xy], dtype=get_dtype(complex=False)
+        )
 
     if weights is not None:
         v = v * weights[None]
 
     if device_name_from_array_module(xp) == "cpu":
         xp.add.at(array, (i, j), v)
     elif device_name_from_array_module(xp) == "gpu":
         cupyx.scatter_add(array, (i, j), v)
     else:
         raise RuntimeError()
 
     return array
 
 
-class ProjectedScatteringFactorIntegrator(ProjectionIntegrator):
+class ScatteringFactorProjectionIntegrals(FieldIntegrator):
     """
-    A ProjectionIntegrator calculating infinite projections of radial potential parametrizations. The hybrid real and
+    A FieldIntegrator calculating infinite projections of radial potential parametrizations. The hybrid real and
     reciprocal space method by Wouter Van den Broek et al. is used.
 
     Parameters
     ----------
-    scattering_factor : 2d array
-        Array representing a projected scattering factor. The zero-frequency is assumed to be at [0,0].
+    parametrization : str or Parametrization, optional
+        The radial potential parametrization to integrate. Default is the Lobato parametrization.
 
     References
     ----------
     W. Van den Broek et al. Ultramicroscopy, 158:89–97, 2015. doi:10.1016/j.ultramic.2015.07.005.
     """
 
-    def __init__(self, scattering_factor: np.ndarray):
-        self._scattering_factor = scattering_factor
-
-    @property
-    def scattering_factor(self) -> np.ndarray:
-        """Projected scattering factor array on a 2D grid."""
-        return self._scattering_factor
-
-    def integrate_on_grid(
-        self,
-        positions: np.ndarray,
-        a: np.ndarray,
-        b: np.ndarray,
-        gpts: tuple[int, int],
-        sampling: tuple[float, float],
-        device: str = "cpu",
-        fourier_space: bool = False,
-    ):
-        xp = get_array_module(device)
-
-        if len(positions) == 0:
-            return xp.zeros(gpts, dtype=xp.float32)
-
-        positions = (positions[:, :2] / sampling).astype(xp.float32)
-
-        array = xp.zeros(gpts, dtype=xp.float32)
-
-        array = superpose_deltas(positions, array).astype(xp.complex64)
-
-        array = fft2(array, overwrite_x=True)
-
-        f = self.scattering_factor / sinc(
-            self._scattering_factor.shape[-2:], sampling, device
-        )
-
-        array *= f
-
-        if fourier_space:
-            return array.real
-        else:
-            array = ifft2(array, overwrite_x=True).real
-            return array
-
-
-class ProjectedScatteringFactors(ProjectionIntegratorPlan):
-    """
-    The :class:`.ProjectedScatteringFactors` facilitates the creation of :class:`.ProjectedScatteringFactorIntegrator`
-    objects using the ``.build`` method given a grid and a chemical symbol.
-
-    Parameters
-    ----------
-    parametrization : str or Parametrization, optional
-        The radial potential parametrization to integrate. Default is the Lobato parametrization.
-    """
-
     def __init__(self, parametrization: str | Parametrization = "lobato"):
         self._parametrization = validate_parametrization(parametrization)
+        self._scattering_factors = {}
         super().__init__(periodic=True, finite=False)
 
     @property
     def parametrization(self) -> Parametrization:
         return self._parametrization
 
     def cutoff(self, symbol: str) -> float:
         return np.inf
 
-    def build(
+    def _calculate_scattering_factor(
         self,
         symbol: str,
         gpts: tuple[int, int],
         sampling: tuple[float, float],
         device: str = "cpu",
-    ) -> ProjectedScatteringFactorIntegrator:
-
+    ):
         xp = get_array_module(device)
         kx, ky = spatial_frequencies(gpts, sampling, xp=np)
 
         k2 = kx[:, None] ** 2 + ky[None] ** 2
         f = self.parametrization.projected_scattering_factor(symbol)(k2)
-        f = xp.asarray(f, dtype=xp.float32)
+        f = xp.asarray(f, dtype=get_dtype(complex=False))
 
         if symbol in self.parametrization.sigmas.keys():
             sigma = self.parametrization.sigmas[symbol]
             f = f * xp.exp(
-                -xp.asarray(k2, dtype=xp.float32)
+                -xp.asarray(k2, dtype=get_dtype(complex=False))
                 * (xp.pi * sigma / xp.sqrt(3 / 2)) ** 2
             )
 
-        return ProjectedScatteringFactorIntegrator(f)
+        return f
+
+    def get_scattering_factor(self, symbol, gpts, sampling, device):
+        try:
+            scattering_factor = self.scattering_factors[symbol]
+        except KeyError:
+            scattering_factor = self._calculate_scattering_factor(
+                symbol, gpts, sampling, device
+            )
+            self._scattering_factors[symbol] = scattering_factor
+
+        return scattering_factor
+
+    @property
+    def scattering_factors(self) -> dict[str, np.ndarray]:
+        """Projected scattering factor array on a 2D grid."""
+        return self._scattering_factors
+
+    def integrate_on_grid(
+        self,
+        atoms: Atoms,
+        a: np.ndarray,
+        b: np.ndarray,
+        gpts: tuple[int, int],
+        sampling: tuple[float, float],
+        device: str = "cpu",
+        fourier_space: bool = False,
+    ):
+        xp = get_array_module(device)
+        if len(atoms) == 0:
+            return xp.zeros(gpts, dtype=get_dtype(complex=False))
+
+        array = xp.zeros(gpts, dtype=get_dtype(complex=False))
+        for number in np.unique(atoms.numbers):
+            scattering_factor = self.get_scattering_factor(
+                chemical_symbols[number], gpts, sampling, device
+            )
+
+            positions = atoms.positions[atoms.numbers == number]
+
+            positions = (positions[:, :2] / sampling).astype(get_dtype(complex=False))
+
+            temp_array = xp.zeros(gpts, dtype=get_dtype(complex=False))
+
+            temp_array = superpose_deltas(positions, temp_array).astype(
+                get_dtype(complex=True)
+            )
+
+            temp_array = fft2(temp_array, overwrite_x=True)
+
+            temp_array *= scattering_factor / sinc(gpts, sampling, device)
+
+            if not fourier_space:
+                temp_array = ifft2(temp_array, overwrite_x=True).real
+
+            array += temp_array
+
+        return array
 
 
 @jit(nopython=True, nogil=True)
 def interpolate_radial_functions(
     array: np.ndarray,
     positions: np.ndarray,
     disk_indices: np.ndarray,
@@ -520,15 +546,14 @@
     radial_functions: np.ndarray,
     radial_derivative: np.ndarray,
 ):
     n = radial_gpts.shape[0]
     dt = np.log(radial_gpts[-1] / radial_gpts[0]) / (n - 1)
 
     for i in range(positions.shape[0]):
-
         px = int(round(positions[i, 0] / sampling[0]))
         py = int(round(positions[i, 1] / sampling[1]))
 
         for j in range(disk_indices.shape[0]):
             k = px + disk_indices[j, 0]
             m = py + disk_indices[j, 1]
 
@@ -545,15 +570,15 @@
                 elif idx < n - 1:
                     slope = radial_derivative[i, idx]
                     array[k, m] += (
                         radial_functions[i, idx] + (r_interp - radial_gpts[idx]) * slope
                     )
 
 
-class ProjectionIntegralTable(ProjectionIntegrator):
+class ProjectionIntegralTable:
     """
     A ProjectionIntegrator calculating finite projections of radial potential parametrizations. An integral table
     for each used to evaluate the projection integrals for each atom in a slice given p integral limits.
     The projected potential evaluated along the
 
     Parameters
     ----------
@@ -585,80 +610,14 @@
 
     def integrate(self, a: float | np.ndarray, b: float | np.ndarray) -> np.ndarray:
         f = interp1d(
             self.limits, self.values, axis=0, kind="linear", fill_value="extrapolate"
         )
         return f(b) - f(a)
 
-    def integrate_on_grid(
-        self,
-        positions: np.ndarray,
-        a: float,
-        b: float,
-        gpts: tuple[int, int],
-        sampling: tuple[float, float],
-        device: str = "cpu",
-    ) -> np.ndarray:
-
-        # assert len(a) == len(b) == len(positions)
-        # assert len(a.shape) == 1
-        # assert len(b.shape) == 1
-        if np.isscalar(a):
-            a = np.array([a] * len(positions))
-
-        if np.isscalar(b):
-            b = np.array([b] * len(positions))
-
-        assert len(sampling) == 2
-
-        xp = get_array_module(device)
-
-        array = xp.zeros(gpts, dtype=xp.float32)
-
-        a = a - positions[:, 2]
-        b = b - positions[:, 2]
-
-        disk_indices = xp.asarray(
-            disc_meshgrid(int(np.ceil(self._radial_gpts[-1] / np.min(sampling))))
-        )
-        radial_potential = xp.asarray(self.integrate(a, b))
-
-        positions = xp.asarray(positions, dtype=np.float32)
-
-        # sampling = xp.array(sampling, dtype=xp.float32)
-        # positions[:, :2] = xp.round(positions[:, :2] / sampling) * sampling
-
-        radial_potential_derivative = xp.zeros_like(radial_potential)
-        radial_potential_derivative[:, :-1] = (
-            xp.diff(radial_potential, axis=1) / xp.diff(self.radial_gpts)[None]
-        )
-
-        if xp is cp:
-            interpolate_radial_functions_cuda(
-                array=array,
-                positions=positions,
-                disk_indices=disk_indices,
-                sampling=sampling,
-                radial_gpts=xp.asarray(self.radial_gpts),
-                radial_functions=radial_potential,
-                radial_derivative=radial_potential_derivative,
-            )
-        else:
-            interpolate_radial_functions(
-                array=array,
-                positions=positions,
-                disk_indices=disk_indices,
-                sampling=sampling,
-                radial_gpts=self.radial_gpts,
-                radial_functions=radial_potential,
-                radial_derivative=radial_potential_derivative,
-            )
-
-        return array
-
 
 def cutoff(func: callable, tolerance: float, a: float, b: float) -> float:
     """
     Calculate the point where a function becomes lower than a given tolerance within a given bracketing interval.
 
     Parameters
     ----------
@@ -686,15 +645,15 @@
     taper_values[taper_mask] = (
         np.cos(np.pi * (radial_gpts[taper_mask] - taper_start) / (cutoff - taper_start))
         + 1.0
     ) / 2
     return taper_values
 
 
-class ProjectionQuadratureRule(ProjectionIntegratorPlan):
+class QuadratureProjectionIntegrals(FieldIntegrator):
     """
     Projection integration plan for calculating finite projection integrals based on Gaussian quadrature rule.
 
     Parameters
     ----------
     parametrization : str or Parametrization, optional
         The potential parametrization describing the radial dependence of the potential. Default is 'lobato'.
@@ -708,38 +667,43 @@
     quad_order : int, optional
         Order of quadrature integration passed to scipy.integrate.fixed_quad. Default is 8.
     """
 
     def __init__(
         self,
         parametrization: str | Parametrization = "lobato",
-        cutoff_tolerance: float = 1e-3,
+        cutoff_tolerance: float = 1e-4,
         taper: float = 0.85,
         integration_step: float = 0.02,
         quad_order: int = 8,
     ):
-
         self._parametrization = validate_parametrization(parametrization)
         self._taper = taper
         self._quad_order = quad_order
         self._cutoff_tolerance = cutoff_tolerance
         self._integration_step = integration_step
+        self._tables = {}
+
         super().__init__(periodic=False, finite=True)
 
     @property
     def parametrization(self):
         """The potential parametrization describing the radial dependence of the potential."""
         return self._parametrization
 
     @property
     def quad_order(self):
         """Order of quadrature integration."""
         return self._quad_order
 
     @property
+    def tables(self):
+        return self._tables
+
+    @property
     def cutoff_tolerance(self) -> float:
         """The error tolerance used for deciding the radial cutoff distance of the potential [eV / e]."""
         return self._cutoff_tolerance
 
     @property
     def integration_step(self) -> float:
         """The step size between integration limits used for calculating the integral table."""
@@ -768,58 +732,149 @@
         ) / 2
         return taper_values
 
     def _integral_limits(self, cutoff: float):
         limits = np.linspace(-cutoff, 0, int(np.ceil(cutoff / self._integration_step)))
         return np.concatenate((limits, -limits[::-1][1:]))
 
-    def build_integral_table(
-        self, symbol: str, inner_limit: float
+    def _calculate_integral_table(
+        self, symbol: str, sampling: tuple[float, float]
     ) -> ProjectionIntegralTable:
-        """
-        Build table of projection integrals of the radial atomic potential.
-
-        Parameters
-        ----------
-        symbol : str
-            Chemical symbol to build the integral table.
-        inner_limit : float, optional
-            Smallest radius from the core at which to calculate the projection integral [Å].
-
-        Returns
-        -------
-        projection_integral_table :
-            ProjectionIntegralTable
-        """
         potential = self.parametrization.potential(symbol)
         cutoff = self.cutoff(symbol)
 
+        inner_limit = min(sampling) / 2
         radial_gpts = self._radial_gpts(inner_limit, cutoff)
         limits = self._integral_limits(cutoff)
 
+        # def potential_blurred(r, func):
+        #     ri = np.linspace(-4, 4, 101)[(None,) * len(r.shape)]
+        #     r = r[..., None]
+        #     r = np.abs(r + ri)
+        #     f = (
+        #         func(r) * r[None, None] ** 2 * np.exp(-(ri**2) / 0.1)[None, None]
+        #     ).sum(-1)
+        #     return f
+        #
+        # potential_blurred_ = lambda r: potential_blurred(r, potential)
+        #
+        # projection = lambda z: potential_blurred_(
+        #     np.sqrt(radial_gpts[:, None] ** 2 + z[None] ** 2)
+        # )
+
         projection = lambda z: potential(
             np.sqrt(radial_gpts[:, None] ** 2 + z[None] ** 2)
         )
+        # * np.exp(-(radial_gpts[:, None] ** 2) / 10000)
 
         table = np.zeros((len(limits) - 1, len(radial_gpts)))
         table[0, :] = integrate.fixed_quad(
             projection, -limits[0] * 2, limits[0], n=self._quad_order
         )[0]
 
         for j, (a, b) in enumerate(zip(limits[1:-1], limits[2:])):
             table[j + 1] = (
                 table[j] + integrate.fixed_quad(projection, a, b, n=self._quad_order)[0]
             )
 
         table = table * self._taper_values(radial_gpts, cutoff, self._taper)[None]
 
-        return ProjectionIntegralTable(radial_gpts, limits[1:], table)
+        self._tables[symbol] = ProjectionIntegralTable(radial_gpts, limits[1:], table)
 
-    def build(
+        return self._tables[symbol]
+
+    def get_integral_table(self, symbol, sampling):
+        """
+        Build table of projection integrals of the radial atomic potential.
+
+        Parameters
+        ----------
+        symbol : str
+            Chemical symbol to build the integral table.
+        inner_limit : float, optional
+            Smallest radius from the core at which to calculate the projection integral [Å].
+
+        Returns
+        -------
+        projection_integral_table :
+            ProjectionIntegralTable
+        """
+        try:
+            scattering_factor = self.tables[symbol]
+        except KeyError:
+            scattering_factor = self._calculate_integral_table(symbol, sampling)
+            self._tables[symbol] = scattering_factor
+
+        return scattering_factor
+
+    def integrate_on_grid(
         self,
-        symbol: str,
+        atoms: Atoms,
+        a: float,
+        b: float,
         gpts: tuple[int, int],
         sampling: tuple[float, float],
         device: str = "cpu",
-    ) -> ProjectionIntegralTable:
-        inner_limit = min(sampling) / 2
-        return self.build_integral_table(symbol, inner_limit)
+    ) -> np.ndarray:
+        xp = get_array_module(device)
+
+        array = xp.zeros(gpts, dtype=get_dtype(complex=False))
+        for number in np.unique(atoms.numbers):
+            table = self.get_integral_table(chemical_symbols[number], sampling)
+
+            positions = atoms.positions[atoms.numbers == number]
+
+            shifted_a = a - positions[:, 2]
+            shifted_b = b - positions[:, 2]
+
+            disk_indices = xp.asarray(
+                disk_meshgrid(int(np.ceil(table.radial_gpts[-1] / np.min(sampling))))
+            )
+            radial_potential = xp.asarray(table.integrate(shifted_a, shifted_b))
+
+            positions = xp.asarray(positions, dtype=get_dtype(complex=False))
+
+            radial_potential_derivative = xp.zeros_like(radial_potential)
+            radial_potential_derivative[:, :-1] = (
+                xp.diff(radial_potential, axis=1) / xp.diff(table.radial_gpts)[None]
+            )
+
+            if len(self._parametrization.sigmas):
+                temp = xp.zeros(gpts, dtype=get_dtype(complex=False))
+            else:
+                temp = array
+
+            if xp is cp:
+                interpolate_radial_functions_cuda(
+                    array=temp,
+                    positions=positions,
+                    disk_indices=disk_indices,
+                    sampling=sampling,
+                    radial_gpts=xp.asarray(table.radial_gpts),
+                    radial_functions=radial_potential,
+                    radial_derivative=radial_potential_derivative,
+                )
+            else:
+                interpolate_radial_functions(
+                    array=temp,
+                    positions=positions,
+                    disk_indices=disk_indices,
+                    sampling=sampling,
+                    radial_gpts=table.radial_gpts,
+                    radial_functions=radial_potential,
+                    radial_derivative=radial_potential_derivative,
+                )
+
+            symbol = chemical_symbols[number]
+
+            if symbol in self._parametrization.sigmas:
+                sigma = (
+                    self._parametrization.sigmas[symbol]
+                    / np.array(sampling)
+                    / np.sqrt(3)
+                )
+                temp = get_ndimage_module(temp).gaussian_filter(
+                    temp, sigma=sigma, mode="wrap"
+                )
+                array += temp
+
+        return array
```

### Comparing `abtem-1.0.4/abtem/magnetism/data/lyon.json` & `abtem-1.0.5/abtem/magnetism/parametrizations/data/lyon.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8999999999999997%*

 * *Differences: {"'Ag'": '{insert: [(4, [2.32, 21.11])]}',*

 * * "'Au'": '{insert: [(4, [2.102, 0.776])]}',*

 * * "'Co'": '{insert: [(4, [-0.5211, 0.1285])]}',*

 * * "'Cr'": '{insert: [(4, [3.88, 1.312])]}',*

 * * "'Cu'": '{insert: [(4, [-0.4434, 0.5774])]}',*

 * * "'Fe'": '{insert: [(4, [-0.5191, 0.1693])]}',*

 * * "'Hf'": '{insert: [(4, [-0.1149, 0.3384])]}',*

 * * "'Ir'": '{insert: [(4, [-0.02924, 0.04927])]}',*

 * * "'Mn'": '{insert: [(4, [-0.754, 0.245])]}',*

 * * "'Mo'": '{insert: [(4, [0.1815, 0.1724])]}',*

 * * "'Nb'": '{insert: [(4, [0.6619, 0.2939])]}',*

 * * "'Ni'": […]*

```diff
@@ -11,14 +11,18 @@
         [
             0.4611,
             0.2675
         ],
         [
             -0.6189,
             0.3481
+        ],
+        [
+            2.32,
+            21.11
         ]
     ],
     "Au": [
         [
             0.61,
             1.747
         ],
@@ -29,14 +33,18 @@
         [
             0.6258,
             0.2764
         ],
         [
             -3.433,
             0.634
+        ],
+        [
+            2.102,
+            0.776
         ]
     ],
     "Co": [
         [
             5.324,
             271.6
         ],
@@ -47,14 +55,18 @@
         [
             -31.58,
             2386.0
         ],
         [
             -0.8253,
             0.9567
+        ],
+        [
+            -0.5211,
+            0.1285
         ]
     ],
     "Cr": [
         [
             1.201,
             4.655
         ],
@@ -65,14 +77,18 @@
         [
             -5.867,
             1.045
         ],
         [
             3.577,
             5.462
+        ],
+        [
+            3.88,
+            1.312
         ]
     ],
     "Cu": [
         [
             1.684,
             0.01976
         ],
@@ -83,14 +99,18 @@
         [
             -0.07235,
             0.002058
         ],
         [
             -0.1153,
             0.004499
+        ],
+        [
+            -0.4434,
+            0.5774
         ]
     ],
     "Fe": [
         [
             6.967,
             435.7
         ],
@@ -101,14 +121,18 @@
         [
             -44.85,
             3955.0
         ],
         [
             -0.6665,
             1.294
+        ],
+        [
+            -0.5191,
+            0.1693
         ]
     ],
     "Hf": [
         [
             0.8602,
             1.201
         ],
@@ -119,14 +143,18 @@
         [
             -0.1946,
             1.345
         ],
         [
             -0.1715,
             0.05218
+        ],
+        [
+            -0.1149,
+            0.3384
         ]
     ],
     "Ir": [
         [
             0.02514,
             0.02202
         ],
@@ -137,14 +165,18 @@
         [
             -21.54,
             299.2
         ],
         [
             2.05,
             6.562
+        ],
+        [
+            -0.02924,
+            0.04927
         ]
     ],
     "Mn": [
         [
             0.8182,
             4.156
         ],
@@ -155,14 +187,18 @@
         [
             -6.858,
             3.055
         ],
         [
             6.222,
             4.96
+        ],
+        [
+            -0.754,
+            0.245
         ]
     ],
     "Mo": [
         [
             1.15,
             0.7032
         ],
@@ -173,14 +209,18 @@
         [
             -1.331,
             0.03853
         ],
         [
             0.7077,
             0.03072
+        ],
+        [
+            0.1815,
+            0.1724
         ]
     ],
     "Nb": [
         [
             0.985,
             0.0648
         ],
@@ -191,14 +231,18 @@
         [
             -0.3161,
             0.02979
         ],
         [
             -1.071,
             0.2602
+        ],
+        [
+            0.6619,
+            0.2939
         ]
     ],
     "Ni": [
         [
             2.123,
             0.2109
         ],
@@ -209,14 +253,18 @@
         [
             -42.32,
             0.9541
         ],
         [
             70.1,
             1.139
+        ],
+        [
+            -30.31,
+            1.325
         ]
     ],
     "Os": [
         [
             1.042,
             1.469
         ],
@@ -227,14 +275,18 @@
         [
             -1.514,
             0.1153
         ],
         [
             1.086,
             0.9417
+        ],
+        [
+            0.7026,
+            0.1142
         ]
     ],
     "Pd": [
         [
             0.007623,
             0.0004048
         ],
@@ -245,14 +297,18 @@
         [
             9.942,
             169.1
         ],
         [
             2.203,
             11.02
+        ],
+        [
+            0.2391,
+            0.4986
         ]
     ],
     "Pt": [
         [
             2.001,
             0.1925
         ],
@@ -263,14 +319,18 @@
         [
             1.185,
             8.158
         ],
         [
             3.716,
             0.2857
+        ],
+        [
+            -2.088,
+            0.3153
         ]
     ],
     "Re": [
         [
             2.07,
             669.7
         ],
@@ -281,14 +341,18 @@
         [
             0.4992,
             13.97
         ],
         [
             -0.563,
             0.04738
+        ],
+        [
+            -0.4218,
+            0.2385
         ]
     ],
     "Rh": [
         [
             0.02283,
             0.001625
         ],
@@ -299,14 +363,18 @@
         [
             -2.187,
             2.573
         ],
         [
             -0.1444,
             0.04847
+        ],
+        [
+            0.1402,
+            0.0681
         ]
     ],
     "Ru": [
         [
             1.141,
             0.7594
         ],
@@ -317,14 +385,18 @@
         [
             -1.329,
             0.04251
         ],
         [
             0.585,
             0.1624
+        ],
+        [
+            0.3849,
+            0.02449
         ]
     ],
     "Sc": [
         [
             0.9627,
             1.298
         ],
@@ -335,14 +407,18 @@
         [
             0.003207,
             0.0007223
         ],
         [
             0.1746,
             0.2624
+        ],
+        [
+            0.02062,
+            0.0374
         ]
     ],
     "Ta": [
         [
             0.9782,
             1.502
         ],
@@ -353,14 +429,18 @@
         [
             -0.6757,
             0.1135
         ],
         [
             0.39,
             1.21
+        ],
+        [
+            0.2566,
+            0.1225
         ]
     ],
     "Ti": [
         [
             0.9865,
             2.0
         ],
@@ -371,14 +451,18 @@
         [
             0.3906,
             0.2528
         ],
         [
             -0.5238,
             6.228
+        ],
+        [
+            -0.1731,
+            0.3869
         ]
     ],
     "V": [
         [
             6.594,
             463.8
         ],
@@ -389,14 +473,18 @@
         [
             -41.02,
             3962.0
         ],
         [
             -1.165,
             2.72
+        ],
+        [
+            -0.7793,
+            0.4911
         ]
     ],
     "W": [
         [
             0.8705,
             1.171
         ],
@@ -407,14 +495,18 @@
         [
             -1.546,
             0.07871
         ],
         [
             0.271,
             0.2382
+        ],
+        [
+            0.3197,
+            0.05784
         ]
     ],
     "Y": [
         [
             1.808,
             0.001824
         ],
@@ -425,14 +517,18 @@
         [
             -1.824,
             0.0003088
         ],
         [
             1.045,
             0.0001321
+        ],
+        [
+            -0.1714,
+            5.709e-05
         ]
     ],
     "Zr": [
         [
             0.002954,
             0.0003582
         ],
@@ -443,10 +539,14 @@
         [
             0.9615,
             5.496
         ],
         [
             -0.1008,
             0.2481
+        ],
+        [
+            0.1946,
+            0.574
         ]
     ]
 }
```

### Comparing `abtem-1.0.4/abtem/mcf.py` & `abtem-1.0.5/abtem/mcf.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/measurements.py` & `abtem-1.0.5/abtem/measurements.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,160 +1,184 @@
 """Module for describing abTEM measurement objects."""
+
 from __future__ import annotations
 
 import copy
 import itertools
 from abc import ABCMeta, abstractmethod
 from collections import defaultdict
-from typing import (
-    TypeVar,
-    Dict,
-    Sequence,
-    Type,
-    TYPE_CHECKING,
-)
+from numbers import Number
+from typing import TYPE_CHECKING, Dict, Sequence, Type, TypeVar
 
 import dask.array as da
-import matplotlib.pyplot as plt
 import numpy as np
 from ase import Atom
 from ase.cell import Cell
 from matplotlib.axes import Axes
-from numba import prange, jit
+from numba import jit, prange
 
 from abtem.array import ArrayObject, stack
+from abtem.core import config
 from abtem.core.axes import (
-    RealSpaceAxis,
     AxisMetadata,
-    ReciprocalSpaceAxis,
     LinearAxis,
     NonLinearAxis,
-    ScanAxis, OrdinalAxis,
+    RealSpaceAxis,
+    ReciprocalSpaceAxis,
+    ScaleAxis,
+    ScanAxis,
 )
-from abtem.core.backend import cp, get_array_module, get_ndimage_module
+from abtem.core.backend import asnumpy, cp, get_array_module, get_ndimage_module
 from abtem.core.complex import abs2
 from abtem.core.energy import energy2wavelength
-from abtem.core.fft import fft_interpolate, fft_crop
+from abtem.core.fft import fft_crop, fft_interpolate
 from abtem.core.grid import (
     adjusted_gpts,
     polar_spatial_frequencies,
     spatial_frequencies,
 )
-from abtem.core import config
 from abtem.core.units import _get_conversion_factor, _validate_units
-from abtem.core.utils import CopyMixin, EqualityMixin, label_to_index
-from abtem.distributions import BaseDistribution
-from abtem.indexing import _index_diffraction_patterns, _format_miller_indices
-from abtem.noise import NoiseTransform
-from abtem.visualize import (
-    MeasurementVisualization2D,
-    MeasurementVisualization1D,
-    DiffractionSpotsVisualization,
+from abtem.core.utils import (
+    CopyMixin,
+    EqualityMixin,
+    is_broadcastable,
+    label_to_index,
 )
+from abtem.distributions import BaseDistribution
+from abtem.noise import NoiseTransform, ScanNoiseTransform
+from abtem.visualize.visualizations import Visualization
+from abtem.visualize.widgets import ImageGUI, LinesGUI, ScatterGUI
 
 # Enables CuPy-accelerated functions if it is available.
 if cp is not None:
-    from abtem.core._cuda import sum_run_length_encoded as sum_run_length_encoded_cuda
     from abtem.core._cuda import interpolate_bilinear as interpolate_bilinear_cuda
+    from abtem.core._cuda import sum_run_length_encoded as sum_run_length_encoded_cuda
 else:
     sum_run_length_encoded_cuda = None
     interpolate_bilinear_cuda = None
 
-try:
-    import ipywidgets as widgets
-except ImportError:
-    widgets = None
 
 if TYPE_CHECKING:
     from abtem.waves import BaseWaves
 
 # Ensures that `Measurement` objects created by `Measurement` objects retain their type (e.g. `Images`).
-T = TypeVar("T", bound="BaseMeasurement")
+T = TypeVar("T", bound="BaseMeasurements")
 
 
 def _scanned_measurement_type(
     measurement: BaseMeasurements | BaseWaves,
 ) -> Type["BaseMeasurements"]:
     if len(_scan_shape(measurement)) == 1:
         return RealSpaceLineProfiles
 
     elif len(_scan_shape(measurement)) == 2:
         return Images
 
     else:
-        return None
-        # raise RuntimeError(
-        #     f"no measurement type for {measurement.__class__} with {len(_scan_shape(measurement))} scan "
-        #     f"axes"
-        # )
+        return MeasurementsEnsemble
 
 
 def _bin_extent(n):
     if n % 2 == 0:
         return -n // 2 - 0.5, n // 2 - 0.5
     else:
         return -n // 2 + 0.5, n // 2 + 0.5
 
 
+# def _move_scan_axes_to_back(measurement):
+#     ensemble_axes = tuple(range(len(measurement.ensemble_shape)))
+#
+#     source = _scan_axes(measurement)
+#     destination = tuple(range(len(ensemble_axes) - len(source), len(ensemble_axes)))
+#
+#     if source != destination:
+#         measurement = moveaxis(measurement, source, destination)
+#     return measurement
+
+
 def _reduced_scanned_images_or_line_profiles(
     new_array,
     old_measurement,
     metadata=None,
-) -> RealSpaceLineProfiles | Images | np.ndarray:
+) -> RealSpaceLineProfiles | Images | MeasurementsEnsemble | np.ndarray:
     if metadata is None:
         metadata = {}
 
     metadata = {**old_measurement.metadata, **metadata}
 
-    if _scanned_measurement_type(old_measurement) is RealSpaceLineProfiles:
-        sampling = old_measurement.ensemble_axes_metadata[-1].sampling
+    ensemble_axes = tuple(range(len(old_measurement.ensemble_shape)))
+
+    source = _scan_axes(old_measurement)
+    destination = tuple(range(len(ensemble_axes) - len(source), len(ensemble_axes)))
+    scan_axes_metadata = [old_measurement.ensemble_axes_metadata[i] for i in source]
+
+    ensemble_axes_metadata = [
+        m
+        for i, m in enumerate(old_measurement.ensemble_axes_metadata)
+        if i not in source
+    ]
+
+    if source != destination:
+        xp = get_array_module(new_array)
+        if old_measurement.is_lazy:
+            new_array = da.moveaxis(new_array, source, destination)
+        else:
+            new_array = xp.moveaxis(new_array, source, destination)
 
-        ensemble_axes_metadata = old_measurement.ensemble_axes_metadata[:-1]
+    if len(scan_axes_metadata) == 1:
+        sampling = scan_axes_metadata[-1].sampling
 
         return RealSpaceLineProfiles(
             new_array,
             sampling=sampling,
             ensemble_axes_metadata=ensemble_axes_metadata,
             metadata=metadata,
         )
 
-    elif _scanned_measurement_type(old_measurement) is Images:
-        ensemble_axes_metadata = old_measurement.ensemble_axes_metadata[:-2]
-
+    elif len(scan_axes_metadata) == 2:
         sampling = (
-            old_measurement.ensemble_axes_metadata[-2].sampling,
-            old_measurement.ensemble_axes_metadata[-1].sampling,
+            scan_axes_metadata[-2].sampling,
+            scan_axes_metadata[-1].sampling,
         )
 
         images = Images(
             new_array,
             sampling=sampling,
             ensemble_axes_metadata=ensemble_axes_metadata,
             metadata=metadata,
         )
 
         return images
+    elif _scanned_measurement_type(old_measurement) is MeasurementsEnsemble:
+        ensemble_axes_metadata = old_measurement.ensemble_axes_metadata
+
+        measurement_ensemble = MeasurementsEnsemble(
+            new_array,
+            ensemble_axes_metadata=ensemble_axes_metadata,
+            metadata=metadata,
+        )
+        return measurement_ensemble
     else:
         return new_array
 
 
-def _scan_axes(self):
-    num_trailing_scan_axes = 0
-    for axis in reversed(self.ensemble_axes_metadata):
-        if not isinstance(axis, ScanAxis) or num_trailing_scan_axes == 2:
+def _scan_axes(measurement):
+    num_scan_axes = 0
+    scan_axes = ()
+    for i, axis in enumerate(measurement.ensemble_axes_metadata):
+        if num_scan_axes == 2:
             break
 
-        num_trailing_scan_axes += 1
+        if isinstance(axis, ScanAxis) and axis._main is True:
+            scan_axes += (i,)
+            num_scan_axes += 1
 
-    return tuple(
-        range(
-            len(self.ensemble_shape) - num_trailing_scan_axes,
-            len(self.ensemble_shape),
-        )
-    )
+    scan_axes = scan_axes[-2:]
+
+    return scan_axes
 
 
 def _scan_sampling(measurements):
     return tuple(
         measurements.axes_metadata[i].sampling for i in _scan_axes(measurements)
     )
 
@@ -224,17 +248,17 @@
     nbins_azimuthal: int,
     rotation: float = 0.0,
     offset: tuple[float, float] = (0.0, 0.0),
     fftshift: bool = False,
     return_indices: bool = False,
 ) -> np.ndarray | list[np.ndarray]:
     alpha, phi = polar_spatial_frequencies(
-        gpts, (1 / sampling[0] / gpts[0], 1 / sampling[1] / gpts[1])
+        gpts, sampling=(1 / sampling[0] / gpts[0], 1 / sampling[1] / gpts[1])
     )
-    phi = (phi + rotation) % (2 * np.pi)
+    phi = (phi - rotation) % (2 * np.pi)
 
     radial_bins = -np.ones(gpts, dtype=int)
     valid = (alpha >= inner) & (alpha < outer)
 
     radial_bins[valid] = nbins_radial * (alpha[valid] - inner) / (outer - inner)
 
     angular_bins = np.floor(nbins_azimuthal * (phi / (2 * np.pi)))
@@ -262,17 +286,17 @@
         for i in label_to_index(bins, nbins_radial * nbins_azimuthal - 1):
             indices.append(i)
         return indices
     else:
         return bins
 
 
-@jit(nopython=True, nogil=True, fastmath=True)
+@jit(nopython=True, nogil=True, fastmath=True, parallel=True)
 def _sum_run_length_encoded(array, result, separators):
-    for x in prange(result.shape[1]):
+    for x in prange(result.shape[1]):  # pylint: disable=not-an-iterable
         for i in range(result.shape[0]):
             for j in range(separators[x], separators[x + 1]):
                 result[i, x] += array[i, j]
 
 
 def _interpolate_stack(array, positions, mode, order, **kwargs):
     map_coordinates = get_ndimage_module(array).map_coordinates
@@ -282,15 +306,15 @@
     positions = positions.reshape((-1, 2))
 
     old_shape = array.shape
     array = array.reshape((-1,) + array.shape[-2:])
     array = xp.pad(array, ((0, 0), (2 * order,) * 2, (2 * order,) * 2), mode=mode)
 
     positions = positions + 2 * order
-    output = xp.zeros((array.shape[0], positions.shape[0]), dtype=np.float32)
+    output = xp.zeros((array.shape[0], positions.shape[0]), dtype=array.dtype)
 
     for i in range(array.shape[0]):
         map_coordinates(array[i], positions.T, output=output[i], order=order, **kwargs)
 
     output = output.reshape(old_shape[:-2] + positions_shape[:-1])
     return output
 
@@ -340,41 +364,48 @@
     def _check_is_complex(self):
         if not np.iscomplexobj(self.array):
             raise RuntimeError("Function not implemented for non-complex measurements.")
 
     def real(self) -> T:
         """Returns the real part of a complex-valued measurement."""
         self._check_is_complex()
+        self.metadata["label"] = "real"
+        self.metadata["units"] = "arb. unit"
         return self._apply_element_wise_func(get_array_module(self.array).real)
 
     def imag(self) -> T:
         """Returns the imaginary part of a complex-valued measurement."""
         self._check_is_complex()
+        self.metadata["label"] = "imaginary"
+        self.metadata["units"] = "arb. unit"
         return self._apply_element_wise_func(get_array_module(self.array).imag)
 
     def phase(self) -> T:
         """Calculates the phase of a complex-valued measurement."""
         self._check_is_complex()
         self.metadata["label"] = "phase"
+        self.metadata["units"] = "rad."
         return self._apply_element_wise_func(get_array_module(self.array).angle)
 
     def abs(self) -> T:
         """Calculates the absolute value of a complex-valued measurement."""
         # self._check_is_complex()
+        self.metadata["label"] = "amplitude"
+        self.metadata["units"] = "arb. unit"
         return self._apply_element_wise_func(get_array_module(self.array).abs)
 
     def intensity(self) -> T:
         """Calculates the squared norm of a complex-valued measurement."""
         self._check_is_complex()
         self.metadata["label"] = "intensity"
         self.metadata["units"] = "arb. unit"
         return self._apply_element_wise_func(abs2)
 
     def relative_difference(
-        self, other: "BaseMeasurements", min_relative_tol: float = 0.0
+        self, other: BaseMeasurements, min_relative_tol: float = 0.0
     ) -> T:
         """
         Calculates the relative difference with respect to another compatible measurement.
 
         Parameters
         ----------
         other : BaseMeasurements
@@ -394,14 +425,15 @@
         valid = xp.abs(self.array) >= min_relative_tol * self.array.max()
         difference._array[valid] /= self.array[valid]
         difference._array[valid == 0] = np.nan
         difference._array *= 100.0
 
         difference.metadata["label"] = "Relative difference"
         difference.metadata["units"] = "%"
+        difference.metadata["tex_units"] = "$\%$"
         return difference
 
     def normalize_ensemble(self, scale: str = "max", shift: str = "mean"):
         """
         Normalize the ensemble by shifting ad scaling each member.
 
         Parameters
@@ -450,16 +482,16 @@
     @property
     @abstractmethod
     def _area_per_pixel(self):
         pass
 
     def poisson_noise(
         self,
-        dose_per_area: float | Sequence[float] = None,
-        total_dose: float | Sequence[float] = None,
+        dose_per_area: float | Sequence[float] | None = None,
+        total_dose: float | Sequence[float] | None = None,
         samples: int = 1,
         seed: int = None,
     ):
         """
         Add Poisson noise (i.e. shot noise) to a measurement corresponding to the provided 'total_dose' (per measurement
         if applied to an ensemble) or 'dose_per_area' (not applicable for single measurements).
 
@@ -481,19 +513,19 @@
             The noisy measurement.
         """
 
         wrong_dose_error = RuntimeError(
             "Provide one of 'dose_per_area' or 'total_dose'."
         )
 
+        if (dose_per_area is not None) and (total_dose is not None):
+            raise RuntimeError("Provide one of 'dose_per_area' or 'total_dose'.")
+
         dose_axes_metadata = None
         if dose_per_area is not None:
-            if total_dose is not None:
-                raise wrong_dose_error
-
             if np.isscalar(dose_per_area):
                 total_dose = self._area_per_pixel * dose_per_area
             else:
                 total_dose = self._area_per_pixel * np.array(
                     dose_per_area, dtype=np.float32
                 )
                 dose_axes_metadata = NonLinearAxis(
@@ -517,20 +549,205 @@
         if isinstance(transform.dose, BaseDistribution) and dose_axes_metadata:
             measurement = measurement.set_ensemble_axes_metadata(
                 dose_axes_metadata, axis=0
             )
 
         return measurement
 
+    def _scale_axis_from_metadata(self):
+        return ScaleAxis(
+            label=self.metadata.get("label", ""),
+            units=self.metadata.get("units", None),
+            tex_label=None,
+        )
+
+    def to_measurement_ensemble(self):
+        return MeasurementsEnsemble(
+            array=self.array,
+            ensemble_axes_metadata=self.axes_metadata,
+            metadata=self.metadata,
+        )
+
     @abstractmethod
     def show(self, *args, **kwargs):
         """Documented in subclasses"""
         pass
 
 
+class MeasurementsEnsemble(BaseMeasurements):
+    _base_dims = 0
+
+    def __init__(
+        self,
+        array: np.ndarray,
+        ensemble_axes_metadata: list[AxisMetadata],
+        metadata: dict = None,
+    ):
+        super().__init__(
+            array=array,
+            ensemble_axes_metadata=ensemble_axes_metadata,
+            metadata=metadata,
+        )
+
+    @property
+    def _area_per_pixel(self):
+        raise RuntimeError("Cannot infer pixel area from metadata.")
+
+    @property
+    def base_axes_metadata(self):
+        return []
+
+    @classmethod
+    def from_array_and_metadata(
+        cls, array: np.ndarray, axes_metadata: list[AxisMetadata], metadata: dict
+    ) -> "T":
+        return cls(array, axes_metadata, metadata)
+
+    def show(
+        self,
+        type: str = "lines",
+        ax: Axes = None,
+        power: float = 1.0,
+        common_scale: bool = False,
+        explode: bool | Sequence[int] = (),
+        overlay: bool | Sequence[int] = (),
+        figsize: tuple[int, int] = None,
+        title: bool | str = True,
+        units: str = None,
+        interact: bool = False,
+        display: bool = True,
+        **kwargs,
+    ) -> Visualization:
+        """
+        Show the image(s) using matplotlib.
+
+        Parameters
+        ----------
+        ax : matplotlib.axes.Axes, optional
+            If given the plots are added to the axis. This is not available for exploded plots.
+        cbar : bool, optional
+            Add colorbar(s) to the image(s). The size and padding of the colorbars may be adjusted using the
+            `set_cbar_size` and `set_cbar_padding` methods.
+        cmap : str, optional
+            Matplotlib colormap name used to map scalar data to colors. If the measurement is complex the colormap
+            must be one of 'hsv' or 'hsluv'.
+        vmin : float, optional
+            Minimum of the intensity color scale. Default is the minimum of the array values.
+        vmax : float, optional
+            Maximum of the intensity color scale. Default is the maximum of the array values.
+        power : float
+            Show image on a power scale.
+        common_color_scale : bool, optional
+            If True all images in an image grid are shown on the same colorscale, and a single colorbar is created (if
+            it is requested). Default is False.
+        explode : bool, optional
+            If True, a grid of images is created for all the items of the last two ensemble axes. If False, the first
+            ensemble item is shown. May be given as a sequence of axis indices to create a grid of images from
+            the specified axes. The default is determined by the axis metadata.
+        figsize : two int, optional
+            The figure size given as width and height in inches, passed to `matplotlib.pyplot.figure`.
+        title : bool or str, optional
+            Set the column title of the images. If True is given instead of a string the title will be given by the
+            value corresponding to the "name" key of the axes metadata dictionary, if this item exists.
+        units : str
+            The units used for the x and y axes. The given units must be compatible with the axes of the images.
+        interact : bool
+            If True, create an interactive visualization. This requires enabling the ipympl Matplotlib backend.
+        display : bool, optional
+            If True (default) the figure is displayed immediately.
+
+        Returns
+        -------
+        measurement_visualization_2d : VisualizationImshow
+        """
+        pass
+        # if not interact:
+        #     self.compute()
+
+        # scale_axis = self._scale_axis_from_metadata()
+
+        # # base_axes_metadata = self._plot_base_axes_metadata(units)
+
+        # array = self.array
+
+        # # raise RuntimeError("Cannot infer pixel area from metadata.")
+
+        # #if display_axes != (-2, -1):
+        # #    array = np.moveaxis(self.array, source=display_axes, destination=(-2, -1))
+
+        # display_axes = normalize_axes(display_axes, self.shape)
+
+        # # base_axes_metadata = [self.axes_metadata[i] for i in display_axes]
+        # # ensemble_axes_metadata = [
+        # #     self.axes_metadata[i]
+        # #     for i in range(len(self.shape))
+        # #     if i not in display_axes
+        # # ]
+
+        # artist_type = LinesArtist
+
+        # visualization = Visualization(
+        #     self,
+        #     ax=ax,
+        #     artist_type=artist_type,
+        #     power=power,
+        #     common_scale=common_scale,
+        #     explode=explode,
+        #     overlay=overlay,
+        #     figsize=figsize,
+        #     interact=interact,
+        #     title=title,
+        #     **kwargs,
+        # )
+
+        # return visualization
+
+    # def show(
+    #     self,
+    #     ax: Axes = None,
+    #     common_scale: bool = True,
+    #     explode: bool | Sequence[int] = None,
+    #     overlay: bool | Sequence[int] = None,
+    #     figsize: tuple[int, int] = None,
+    #     title: str = None,
+    #     units: str = None,
+    #     legend: bool = False,
+    #     interact: bool = False,
+    #     display: bool = True,
+    #     **kwargs,
+    # ):
+    #     # if not interact:
+    #     #     self.compute()
+    #
+    #     visualization = VisualizationLines(
+    #         array=self.array,
+    #         coordinate_axes=self.ensemble_axes_metadata[-1:],
+    #         scale_axis=self._scale_axis_from_metadata(),
+    #         ensemble_axes=self.ensemble_axes_metadata[:-1],
+    #         ax=ax,
+    #         common_scale=common_scale,
+    #         explode=explode,
+    #         overlay=overlay,
+    #         figsize=figsize,
+    #         interact=interact,
+    #         title=title,
+    #         **kwargs,
+    #     )
+    #
+    #     if not display and not interact:
+    #         plt.close()
+    #
+    #     if interact and display:
+    #         from IPython.display import display as ipython_display
+    #
+    #         ipython_display(visualization.layout_widgets())
+    #
+    #     return visualization
+
+
 class _BaseMeasurement2D(BaseMeasurements):
     _base_dims = 2
 
     @abstractmethod
     def _get_1d_equivalent(self):
         pass
 
@@ -597,16 +814,16 @@
         Returns
         -------
         line_profiles : RealSpaceLineProfiles
             The interpolated line(s).
         """
         from abtem.scan import LineScan
 
-        if self.is_complex:
-            raise NotImplementedError
+        # if self.is_complex:
+        #    raise NotImplementedError
 
         if (sampling is None) and (gpts is None):
             sampling = min(self.sampling)
 
         xp = get_array_module(self.array)
 
         if start is None:
@@ -672,18 +889,14 @@
 
         if width:
             array = array.mean(-1)
             metadata["width"] = width
 
         ensemble_axes_metadata = self.ensemble_axes_metadata
 
-        for axis in ensemble_axes_metadata:
-            if isinstance(axis, OrdinalAxis):
-                axis._default_type = "overlay"
-
         return self._get_1d_equivalent()(
             array=array,
             sampling=scan.sampling,
             ensemble_axes_metadata=ensemble_axes_metadata,
             metadata=metadata,
         )
 
@@ -820,21 +1033,23 @@
         ax: Axes = None,
         cbar: bool = False,
         cmap: str = None,
         vmin: float = None,
         vmax: float = None,
         power: float = 1.0,
         common_color_scale: bool = False,
-        explode: bool | Sequence[bool] = None,
+        explode: bool | Sequence[int] = (),
+        overlay: bool | Sequence[int] = (),
         figsize: tuple[int, int] = None,
         title: bool | str = True,
         units: str = None,
         interact: bool = False,
         display: bool = True,
-    ) -> MeasurementVisualization2D:
+        **kwargs,
+    ) -> Visualization:
         """
         Show the image(s) using matplotlib.
 
         Parameters
         ----------
         ax : matplotlib.axes.Axes, optional
             If given the plots are added to the axis. This is not available for exploded plots.
@@ -867,48 +1082,39 @@
         interact : bool
             If True, create an interactive visualization. This requires enabling the ipympl Matplotlib backend.
         display : bool, optional
             If True (default) the figure is displayed immediately.
 
         Returns
         -------
-        measurement_visualization_2d : MeasurementVisualization2D
+        measurement_visualization_2d : VisualizationImshow
         """
 
-        if not interact:
-            self.compute()
-
-        visualization = MeasurementVisualization2D(
-            measurements=self,
+        visualization = Visualization(
+            measurement=self,
             ax=ax,
-            cbar=cbar,
-            cmap=cmap,
-            vmin=vmin,
-            vmax=vmax,
-            power=power,
             common_scale=common_color_scale,
-            explode=explode,
             figsize=figsize,
-            interact=interact,
+            title=title,
+            aspect=True,
+            share_x=True,
+            share_y=True,
+            explode=explode,
+            overlay=overlay,
+            interactive=not interact and display,
+            value_limits=(vmin, vmax),
+            power=power,
+            cmap=cmap,
+            cbar=cbar,
+            units=units,
+            **kwargs,
         )
 
-        if title is not None:
-            visualization.set_column_titles(title)
-
-        if units is not None:
-            visualization.set_xunits(units)
-            visualization.set_yunits(units)
-
-        if not display and not interact:
-            plt.close()
-
-        if interact and display:
-            from IPython.display import display as ipython_display
-
-            ipython_display(visualization.widgets)
+        if interact:
+            gui = visualization.interact(ImageGUI, display=display)
 
         return visualization
 
 
 class Images(_BaseMeasurement2D):
     """
     A collection of 2D measurements such as HRTEM or STEM-ADF images. May be used to represent a reconstructed phase.
@@ -1015,18 +1221,18 @@
         y = np.linspace(0.0, self.shape[-1] * self.sampling[1], self.shape[-1])
         return x, y
 
     @property
     def base_axes_metadata(self) -> list[AxisMetadata]:
         return [
             RealSpaceAxis(
-                label="x", sampling=self.sampling[0], units="Å", _tex_label="$x$"
+                label="x", sampling=self.sampling[0], units="Å", tex_label="$x$"
             ),
             RealSpaceAxis(
-                label="y", sampling=self.sampling[1], units="Å", _tex_label="$y$"
+                label="y", sampling=self.sampling[1], units="Å", tex_label="$y$"
             ),
         ]
 
     def integrate_gradient(self):
         """
         Calculate integrated gradients. Requires complex images whose real and imaginary parts represent the `x` and `y`
         components of a gradient.
@@ -1258,14 +1464,47 @@
             raise RuntimeError()
         kwargs = self._copy_kwargs(exclude=("array",))
         kwargs["array"] = np.tile(
             self.array, (1,) * (len(self.array.shape) - 2) + repetitions
         )
         return self.__class__(**kwargs)
 
+    def scan_noise(
+        self,
+        dwell_time: float,
+        flyback_time: float,
+        rms_power: float,
+        max_frequency: float = 500.0,
+        num_components: int = 200,
+        seed: int = None,
+    ):
+        """
+        Apply scan noise to images.
+
+        Parameters
+        ----------
+        dwell_time : float
+            Dwell time of the beam [s].
+        flyback_time : float
+            Flyback time of the beam [s].
+        rms_power : float
+            RMS power of the scan noise [V].
+        max_frequency : float
+            Maximum frequency of the scan noise [1/Å].
+        """
+        transform = ScanNoiseTransform(
+            dwell_time=dwell_time,
+            flyback_time=flyback_time,
+            rms_power=rms_power,
+            max_frequency=max_frequency,
+            num_components=num_components,
+            seeds=seed,
+        )
+        return self.apply_transform(transform)
+
     def diffractograms(self) -> DiffractionPatterns:
         """
         Calculate diffractograms (i.e. power spectra) from image(s).
 
         Returns
         -------
         diffractograms : DiffractionPatterns
@@ -1291,21 +1530,16 @@
         return DiffractionPatterns(
             array=array,
             sampling=sampling,
             ensemble_axes_metadata=self.ensemble_axes_metadata,
             metadata=self.metadata,
         )
 
-    def _plot_extent_x(self, units=None):
-        scale = _get_conversion_factor(units, "Å")
-        return [0, self.extent[0] * scale]
-
-    def _plot_extent_y(self, units=None):
-        scale = _get_conversion_factor(units, "Å")
-        return [0, self.extent[1] * scale]
+    def _plot_base_axes_metadata(self, units: str = None):
+        return self.base_axes_metadata
 
 
 class _BaseMeasurement1D(BaseMeasurements):
     _base_dims = 1
 
     def __init__(
         self,
@@ -1358,26 +1592,14 @@
         return cls(
             array,
             sampling=sampling,
             ensemble_axes_metadata=axes_metadata,
             metadata=metadata,
         )
 
-    @abstractmethod
-    def _plot_extent(self, units):
-        pass
-
-    @abstractmethod
-    def _plot_x_label(self, units):
-        pass
-
-    @abstractmethod
-    def _plot_y_label(self, units):
-        pass
-
     @property
     def extent(self) -> float:
         """
         Extent of measurements [Å] or [1/Å].
         """
         return self.sampling * self.shape[-1]
 
@@ -1523,24 +1745,24 @@
         kwargs["sampling"] = sampling
         return self.__class__(**kwargs)
 
     def show(
         self,
         ax: Axes = None,
         common_scale: bool = True,
-        explode: bool | Sequence[int] = None,
+        explode: bool | Sequence[int] = False,
         overlay: bool | Sequence[int] = None,
         figsize: tuple[int, int] = None,
-        title: str = None,
+        title: str = True,
         units: str = None,
         legend: bool = False,
         interact: bool = False,
         display: bool = True,
         **kwargs,
-    ) -> MeasurementVisualization1D:
+    ) -> Visualization:
         """
         Show the reciprocal-space line profile(s) using matplotlib.
 
         Parameters
         ----------
         ax : matplotlib Axes, optional
             If given the plots are added to the Axes. This is not available for image grids.
@@ -1566,45 +1788,43 @@
         interact : bool
             If True, create an interactive visualization. This requires enabling the ipympl Matplotlib backend.
         display : bool, optional
             If True (default) the figure is displayed immediately.
 
         Returns
         -------
-        visualization : MeasurementVisualization1D
+        visualization : Visualization
         """
 
-        if not interact:
-            self.compute()
+        if overlay is None and explode is False:
+            overlay = True
+        elif overlay is False or overlay is None:
+            overlay = ()
 
-        visualization = MeasurementVisualization1D(
-            self,
+        visualization = Visualization(
+            measurement=self,
             ax=ax,
-            common_scale=common_scale,
+            figsize=figsize,
+            title=title,
+            aspect=False,
+            share_x=True,
+            share_y=common_scale,
             explode=explode,
             overlay=overlay,
-            figsize=figsize,
-            interact=interact,
-            **kwargs
+            interactive=not interact and display,
+            legend=legend,
+            common_scale=common_scale,
+            **kwargs,
         )
 
-        if title is not None:
-            visualization.set_column_titles(title)
-
-        if units is not None:
-            visualization.set_xunits(units)
-            visualization.set_yunits(units)
-
-        if legend:
-            visualization.set_legends()
-
-        if interact and display:
-            from IPython.display import display as ipython_display
+        if interact:
+            gui = visualization.interact(LinesGUI, display=display)
 
-            ipython_display(visualization.widgets)
+        if common_scale is False and visualization._explode:
+            visualization.axes.set_sizes(padding=0.8)
 
         return visualization
 
 
 class RealSpaceLineProfiles(_BaseMeasurement1D):
     """
     A collection of real-space line profile(s).
@@ -1634,17 +1854,15 @@
             ensemble_axes_metadata=ensemble_axes_metadata,
             metadata=metadata,
         )
 
     @property
     def base_axes_metadata(self) -> list[RealSpaceAxis]:
         return [
-            RealSpaceAxis(
-                label="r", sampling=self.sampling, units="Å", _tex_label="$r$"
-            )
+            RealSpaceAxis(label="r", sampling=self.sampling, units="Å", tex_label="$r$")
         ]
 
     def tile(self, repetitions: int) -> "RealSpaceLineProfiles":
         """
         Tile line profiles(s).
 
         Parameters
@@ -1714,15 +1932,15 @@
             metadata=metadata,
         )
 
     @property
     def base_axes_metadata(self) -> list[AxisMetadata]:
         return [
             ReciprocalSpaceAxis(
-                label="k", sampling=self.sampling, units="1/Å", _tex_label="$k$"
+                label="k", sampling=self.sampling, units="1/Å", tex_label="$k$"
             )
         ]
 
     @property
     def angular_extent(self):
         """Extent of line profiles given as scattering angels [mrad]."""
         wavelength = energy2wavelength(self._get_from_metadata("energy"))
@@ -2007,23 +2225,23 @@
         return [
             ReciprocalSpaceAxis(
                 sampling=self.sampling[0],
                 offset=limits[0][0],
                 label="kx",
                 units="1/Å",
                 fftshift=self.fftshift,
-                _tex_label="$k_x$",
+                tex_label="$k_x$",
             ),
             ReciprocalSpaceAxis(
                 sampling=self.sampling[1],
                 offset=limits[1][0],
                 label="ky",
                 units="1/Å",
                 fftshift=self.fftshift,
-                _tex_label="$k_y$",
+                tex_label="$k_y$",
             ),
         ]
 
     def tile_scan(self, repetitions: tuple[int, int]) -> DiffractionPatterns:
         """
         Tile the scan axes of the diffraction patterns. The diffraction patterns must have one or more scan axes.
 
@@ -2059,68 +2277,112 @@
         kwargs = self._copy_kwargs(exclude=("array",))
         kwargs["array"] = array
         return self.__class__(**kwargs)
 
     def index_diffraction_spots(
         self,
         cell: Cell | float | tuple[float, float, float],
-        threshold: float = 0.001,
-        distance_threshold: float = 0.15,
-        min_distance: float = 0.0,
-        integration_radius: float = 0.0,
-        max_index: int = None,
+        orientation_matrices: np.ndarray = None,
+        sg_max: float = None,
+        k_max: float = None,
+        energy: float = None,
         centering: str = "P",
     ) -> IndexedDiffractionPatterns:
         """
         Indexes the Bragg reflections (diffraction spots) by their Miller indices.
 
         Parameters
         ----------
         cell : ase.cell.Cell or float or tuple of float
             The assumed unit cell with respect to the diffraction pattern should be indexed. Must be one of ASE `Cell`
             object, float (for a cubic unit cell) or three floats (for orthorhombic unit cells).
-        threshold : float
-            Minimum intensity of the diffraction spot peaks. Default is 0.001.
-        distance_threshold : float
-            Maximum reciprocal distance to the Ewald sphere of diffraction spots [1/Å]. Default is 0.15.
-        min_distance : float
-            The minimal allowed distance separating peaks [1/Å]. Default is 0.0.
-        integration_radius : float
-            If a non-zero value is given the intensity of diffraction spots is integrated over a disk of the given
-            value [1/Å].
-        max_index : int
-            Maximum miller index of diffraction spots. Default is determined from the maximum scattering angle of the
-            diffraction patterns.
         centering : {'P', 'F', 'I', 'A', 'B', 'C'}
             Assumed lattice centering used for determining the reflection conditions.
 
         Returns
         -------
         indexed_patterns : IndexedDiffractionPatterns
             The indexed diffraction pattern(s).
         """
+        from abtem.bloch.indexing import (
+            estimate_necessary_excitation_error,
+            index_diffraction_spots,
+            validate_cell,
+        )
+        from abtem.bloch.utils import filter_reciprocal_space_vectors, make_hkl_grid
 
-        if self.is_lazy:
-            raise RuntimeError("indexing not implemented for lazy measurement")
+        if orientation_matrices is not None and not is_broadcastable(
+            self.ensemble_shape, orientation_matrices.shape[:-2]
+        ):
+
+            raise ValueError(
+                "The ensemble shape and the shape of the orientation matrices must be broadcastable."
+            )
+
+        if energy is None:
+            energy = self._get_from_metadata("energy")
+
+        if k_max is None:
+            k_max = max(self.max_frequency)
 
-        hkl, intensities, positions = _index_diffraction_patterns(
-            self,
+        if sg_max is None:
+            sg_max = estimate_necessary_excitation_error(energy, k_max)
+
+        cell = validate_cell(cell)
+
+        hkl = make_hkl_grid(cell, k_max)
+
+        mask = filter_reciprocal_space_vectors(
+            hkl,
             cell,
-            threshold=threshold,
-            distance_threshold=distance_threshold,
-            min_distance=min_distance,
-            integration_radius=integration_radius,
-            max_index=max_index,
+            energy=energy,
+            sg_max=sg_max,
+            k_max=k_max,
             centering=centering,
+            orientation_matrices=orientation_matrices,
         )
 
-        ensemble_axes_metadata = self.ensemble_axes_metadata
+        hkl = hkl[mask]
+
+        if self.is_lazy:
+            intensities = self.array.map_blocks(
+                index_diffraction_spots,
+                hkl=hkl,
+                sampling=self.sampling,
+                cell=cell,
+                energy=energy,
+                orientation_matrices=orientation_matrices,
+                drop_axis=len(self.array.shape) - 1,
+                chunks=self.array.chunks[:-2] + (hkl.shape[0],),
+                meta=np.array((), dtype=self.dtype),
+            )
+        else:
+            intensities = index_diffraction_spots(
+                array=self.array,
+                hkl=hkl,
+                sampling=self.sampling,
+                cell=cell,
+                energy=energy,
+                orientation_matrices=orientation_matrices,
+            )
+
+        if orientation_matrices is None:
+            orientation_matrices = np.eye(3)[(None,) * len(self.array.shape[:-2])]
+
+        reciprocal_lattice_vectors = np.matmul(
+            cell.reciprocal(),
+            np.swapaxes(orientation_matrices, -2, -1),
+        )
 
         return IndexedDiffractionPatterns(
-            intensities, hkl, positions, ensemble_axes_metadata, metadata=self.metadata
+            intensities,
+            hkl,
+            reciprocal_lattice_vectors=reciprocal_lattice_vectors,
+            ensemble_axes_metadata=self.ensemble_axes_metadata,
+            metadata=self.metadata,
         )
 
     @property
     def fftshift(self) -> bool:
         """
         True if the zero-frequency is shifted to the center of the array.
         """
@@ -2146,14 +2408,18 @@
         """Maximum scattering angle in `x` and `y` [mrad]."""
         return (
             self.shape[-2] // 2 * self.angular_sampling[0],
             self.shape[-1] // 2 * self.angular_sampling[1],
         )
 
     @property
+    def max_frequency(self):
+        return abs(self.limits[0][1]), abs(self.limits[1][1])
+
+    @property
     def limits(self) -> list[tuple[float, float]]:
         """Lowest and highest spatial frequency in `x` and `y` [1 / Å]."""
         limits = []
         for i in (-2, -1):
             if self.shape[i] % 2:
                 limits += [
                     (
@@ -2516,15 +2782,15 @@
             azimuthal_offset=rotation,
             ensemble_axes_metadata=self.ensemble_axes_metadata,
             metadata=self.metadata,
         )
 
     def radial_binning(
         self, step_size: float = 1.0, inner: float = 0.0, outer: float = None
-    ) -> "PolarMeasurements":
+    ) -> PolarMeasurements:
         """
         Create polar measurement(s) from the diffraction pattern(s) by binning the measurements in annular regions. This
         method may be used to simulate a segmented detector with a specified number of radial bins.
 
         This is equivalent to detecting a wave function using the `FlexibleAnnularDetector`.
 
         Parameters
@@ -2566,14 +2832,34 @@
             Offset of center of annular integration region [mrad].
 
         Returns
         -------
         integrated_images : Images
             The integrated images.
         """
+        if isinstance(inner, Sequence) or isinstance(outer, Sequence):
+            if isinstance(inner, Number):
+                inners = (inner,) * len(outer)
+                outers = outer
+            else:
+                outers = (outer,) * len(inner)
+                inners = inner
+
+            measurements = [
+                self.integrate_radial(inner=inner, outer=outer)
+                for inner, outer in zip(inners, outers)
+            ]
+
+            measurements = stack(
+                measurements,
+                axis_metadata=NonLinearAxis(
+                    label="Limits", values=tuple(zip(inners, outers)), units="mrad"
+                ),
+            )
+            return measurements
 
         self._check_integration_limits(inner, outer)
 
         xp = get_array_module(self.array)
 
         def _integrate_fourier_space(array, sampling):
             xp = get_array_module(array)
@@ -2756,23 +3042,161 @@
                 int(2 * np.round(max_frequency / self.sampling[0])) + 1,
                 int(2 * np.round(max_frequency / self.sampling[1])) + 1,
             )
 
         if gpts is None:
             raise ValueError()
 
-        xp = get_array_module(self.array)
-        array = xp.fft.fftshift(
-            fft_crop(xp.fft.ifftshift(self.array, axes=(-2, -1)), new_shape=gpts),
-            axes=(-2, -1),
-        )
+        def _do_crop(array):
+            xp = get_array_module(array)
+            array = xp.fft.fftshift(
+                fft_crop(xp.fft.ifftshift(array, axes=(-2, -1)), new_shape=gpts),
+                axes=(-2, -1),
+            )
+            return array
+
+        if self.is_lazy:
+            xp = get_array_module(self.array)
+            array = self.array.map_blocks(
+                _do_crop,
+                chunks=self.array.chunks[:-2] + gpts,
+                meta=xp.array((), dtype=self.dtype),
+            )
+        else:
+            array = _do_crop(self.array)
+
         kwargs = self._copy_kwargs(exclude=("array",))
         kwargs["array"] = array
         return self.__class__(**kwargs)
 
+    def azimuthal_average(
+        self,
+        max_angle: float = None,
+        radial_sampling: float = 1.0,
+        weighting_function: str = "step",
+        width: float = 1.0,
+    ) -> ReciprocalSpaceLineProfiles:
+        """
+        Calculate the azimuthal averages of the diffraction patterns.
+
+        Parameters
+        ----------
+        max_angle : float, optional
+            The maximum included scattering angle in the azimuthal averages [mrad].
+        order : float, optional
+            The spline interpolation order. Default is 1.
+        radial_sampling : float, optional
+            The radial sampling of the azimuthal averages [mrad]. Default is equal to the smallest value of the x and y
+            component of the angular sampling.
+        weigthing_method : str
+
+        """
+
+        def _map_azimuthal_average(
+            array,
+            angular_coordinates,
+            max_angle,
+            radial_sampling,
+            weighting_function,
+            width,
+        ):
+            x, y = np.meshgrid(*angular_coordinates, indexing="ij")
+            r = np.sqrt(x**2 + y**2)
+
+            centers = np.arange(0, max_angle, radial_sampling)
+
+            values = np.zeros(array.shape[:-2] + centers.shape)
+            for i, center in enumerate(centers):
+                if weighting_function == "step":
+                    mask = np.abs(r - center) < width
+                elif weighting_function == "gaussian":
+                    mask = np.exp(-((r - center) ** 2) / (width**2 / 2))
+                else:
+                    raise ValueError()
+
+                weight = np.sum(mask)
+
+                if weight > 0:
+                    values[..., i] = np.sum(array * mask, axis=(-2, -1)) / weight
+                else:
+                    values[..., i] = 0.0
+
+            return values
+
+        if max_angle is None:
+            max_angle = -min(min(self.angular_limits))
+
+        radial_sampling = radial_sampling * min(self.angular_sampling)
+        width = width * min(self.angular_sampling)
+
+        if self.is_lazy:
+            xp = get_array_module(self.array)
+            n = int(max_angle / radial_sampling)
+            base_axes = tuple(
+                range(
+                    len(self.ensemble_shape),
+                    len(self.ensemble_shape) + len(self.base_shape),
+                )
+            )
+            array = self.array.map_blocks(
+                _map_azimuthal_average,
+                angular_coordinates=self.angular_coordinates,
+                max_angle=max_angle,
+                radial_sampling=radial_sampling,
+                weighting_function=weighting_function,
+                width=width,
+                drop_axis=base_axes,
+                new_axis=base_axes[0],
+                chunks=self.array.chunks[:-2] + (n,),
+                meta=xp.array((), dtype=np.float32),
+            )
+        else:
+            array = _map_azimuthal_average(
+                self.array,
+                angular_coordinates=self.angular_coordinates,
+                max_angle=max_angle,
+                radial_sampling=radial_sampling,
+                weighting_function=weighting_function,
+                width=width,
+            )
+
+        wavelength = energy2wavelength(self._get_from_metadata("energy"))
+
+        return ReciprocalSpaceLineProfiles(
+            array,
+            sampling=radial_sampling / (wavelength * 1e3),
+            ensemble_axes_metadata=self.ensemble_axes_metadata,
+            metadata=self.metadata,
+        )
+
+    def fourier_shell_correlation(
+        self,
+        other: DiffractionPatterns,
+        radial_sampling: float = 1.0,
+        width: float = 1.0,
+        weighting_function: str = "step",
+    ):
+        fsc = (self**0.5 * other**0.5).azimuthal_average(
+            radial_sampling=radial_sampling,
+            width=width,
+            weighting_function=weighting_function,
+        ) / (
+            self.azimuthal_average(
+                radial_sampling=radial_sampling,
+                width=width,
+                weighting_function=weighting_function,
+            )
+            * other.azimuthal_average(
+                radial_sampling=radial_sampling,
+                width=width,
+                weighting_function=weighting_function,
+            )
+        )
+        return fsc
+
     def block_direct(
         self, radius: float = None, margin: bool = None
     ) -> DiffractionPatterns:
         """
         Block the direct beam by setting the pixels of the zeroth-order Bragg reflection (non-scattered beam) to zero.
 
         Parameters
@@ -2814,47 +3238,37 @@
         if len(bins.shape) == 2:
             array = self.array[..., indices[:, 0], indices[:, 1]]
         else:
             array = self.array[..., indices[0], indices[1]]
 
         return array
 
-    def _plot_extent_x(self, units: str = None):
-        if units is None:
-            units = "1/Å"
-
-        if units == "mrad":
-            return list(self.angular_limits[0])
-        elif units == "1/Å":
-            return [
-                self.limits[0][0] - self.sampling[0] / 2,
-                self.limits[0][1] + self.sampling[0] / 2,
-            ]
-
-        elif units == "bins":
-            return _bin_extent(self.base_shape[0])
-        else:
-            raise RuntimeError()
-
-    def _plot_extent_y(self, units: str = None):
-        if units is None:
-            units = "1/Å"
-
-        if units == "mrad":
-            return list(self.angular_limits[1])
-        elif units == "1/Å":
-            return [
-                self.limits[1][0] - self.sampling[1] / 2,
-                self.limits[1][1] + self.sampling[1] / 2,
-            ]
-
-        elif units == "bins":
-            return _bin_extent(self.base_shape[1])
-        else:
-            raise RuntimeError()
+    # def _plot_base_axes_metadata(self, units: str = None):
+    #     if units is None:
+    #         return self.base_axes_metadata
+    #
+    #     if units == "mrad":
+    #         return [
+    #             ReciprocalSpaceAxis(
+    #                 sampling=self.angular_sampling[0],
+    #                 offset=self.angular_limits[0][0],
+    #                 label="kx",
+    #                 units="mrad",
+    #                 fftshift=self.fftshift,
+    #                 _tex_label="$k_x$",
+    #             ),
+    #             ReciprocalSpaceAxis(
+    #                 sampling=self.angular_sampling[1],
+    #                 offset=self.angular_limits[1][0],
+    #                 label="ky",
+    #                 units="mrad",
+    #                 fftshift=self.fftshift,
+    #                 _tex_label="$k_y$",
+    #             ),
+    #         ]
 
 
 class PolarMeasurements(BaseMeasurements):
     """
     Class describing polar measurements with a specified number of radial and azimuthal bins.
 
     Each bin is a segment of an annulus and the bins are spaced equally in the radial and azimuthal directions.
@@ -3257,29 +3671,30 @@
             sampling=(sampling[0], sampling[1]),
             ensemble_axes_metadata=ensemble_axes_metadata,
             metadata=self.metadata,
         )
 
     def show(
         self,
-        gpts: int | tuple[int, int] = (512, 512),
         ax: Axes = None,
+        gpts: int | tuple[int, int] = (512, 512),
         cbar: bool = False,
         cmap: str = None,
         vmin: float = None,
         vmax: float = None,
         power: float = 1.0,
         common_color_scale: bool = False,
-        explode: bool | Sequence[bool] = None,
+        explode: bool | Sequence[bool] = (),
+        overlay: bool | Sequence[int] = (),
         figsize: tuple[int, int] = None,
         title: bool | str = True,
         units: str = None,
         interact: bool = False,
         display: bool = True,
-    ) -> MeasurementVisualization2D:
+    ) -> Visualization:
         """
         Show the image(s) using matplotlib.
 
         Parameters
         ----------
         gpts : int or tuple of int, optional
         ax : matplotlib.axes.Axes, optional
@@ -3313,15 +3728,15 @@
         interact : bool
             If True, create an interactive visualization. This requires enabling the ipympl Matplotlib backend.
         display : bool, optional
             If True (default) the figure is displayed immediately.
 
         Returns
         -------
-        measurement_visualization_2d : MeasurementVisualization2D
+        measurement_visualization_2d : MeasurementVisualizationImshow
         """
 
         diffraction_patterns = self.to_diffraction_patterns(gpts=gpts)
 
         if not interact:
             diffraction_patterns.compute()
 
@@ -3330,67 +3745,129 @@
             cbar=cbar,
             cmap=cmap,
             vmin=vmin,
             vmax=vmax,
             power=power,
             common_color_scale=common_color_scale,
             explode=explode,
+            overlay=overlay,
             figsize=figsize,
             title=title,
             units=units,
             interact=interact,
             display=display,
         )
 
 
+@jit(nopython=True, nogil=True, fastmath=True)
+def calculate_max_reciprocal_space_vector(hkl, reciprocal_lattice_vectors):
+
+    k_max = 0.0
+    for i in range(len(hkl)):
+        lengths = (
+            (
+                hkl[i, 0] * reciprocal_lattice_vectors[..., 0, :]
+                + hkl[i, 1] * reciprocal_lattice_vectors[..., 1, :]
+                + hkl[i, 2] * reciprocal_lattice_vectors[..., 2, :]
+            )
+            ** 2
+        ).sum(-1)
+
+        if hasattr(lengths, "max"):
+            lengths = lengths.max()
+
+        k_max = max(k_max, lengths)
+
+    return np.sqrt(k_max)
+
+
+@jit(nopython=True, nogil=True, fastmath=True, parallel=True)
+def reciprocal_lattice_vector_mask(mask, hkl, reciprocal_lattice_vectors, k_max):
+
+    for i in prange(len(hkl)):  # pylint: disable=not-an-iterable
+        lengths = (
+            (
+                hkl[i, 0] * reciprocal_lattice_vectors[..., 0, :]
+                + hkl[i, 1] * reciprocal_lattice_vectors[..., 1, :]
+                + hkl[i, 2] * reciprocal_lattice_vectors[..., 2, :]
+            )
+            ** 2
+        ).sum(-1)
+
+        include = lengths < k_max**2
+
+        if hasattr(lengths, "any"):
+            include = include.any()
+
+        mask[i] = include
+
+    return mask
+
+
 class IndexedDiffractionPatterns(BaseMeasurements):
     """
     Diffraction patterns indexed by their Miller indices.
 
     Parameters
     ----------
     array : np.ndarray
-        1D or greater array of type `float`. The last axis represents the diffraction spots and should have the same
+        1D or greater array of type `float` or `complex`. The last axis represents the diffraction spots and should have the same
         length as the number of miller indices, any preceding axis represents an ensemble axis.
     miller_indices : np.ndarray
         The miller indices of the diffraction spots as an N x 3 array where N is the number of miller indices. The
         order of the miller indices must correspond to the array of intensities. The second axis represents each
         hkl miller index.
-    positions : np.ndarray
-        The reciprocal space coordinates of the diffraction spots as an N x 3 array. The first axis represents
+    reciprocal_lattice_vectors : np.ndarray
+        The reciprocal lattice vectors of the crystal as a 3 x 3 array. The first axis represents
         miller indices and the order of the items must correspond to the array of intensities. The second axis
         represents the reciprocal space positions in x, y and z [1/Å].
     ensemble_axes_metadata : list of AxisMetadata, optional
         List of metadata associated with the ensemble axes. The length and item order must match the ensemble axes.
     metadata : dict, optional
         A dictionary defining measurement metadata.
     """
 
     _base_dims = 1
 
     def __init__(
         self,
         array: np.ndarray,
         miller_indices: np.ndarray,
-        positions: np.ndarray,
+        reciprocal_lattice_vectors: np.ndarray,
         ensemble_axes_metadata: list[AxisMetadata] = None,
         metadata: dict = None,
     ):
-        assert len(miller_indices) == array.shape[-1]
-        assert len(miller_indices) == len(positions)
+
+        if len(reciprocal_lattice_vectors.shape) <= len(array.shape):
+            reciprocal_lattice_vectors = reciprocal_lattice_vectors[
+                (None,) * (len(reciprocal_lattice_vectors.shape) - len(array.shape) + 1)
+            ]
+
+        # if not is_broadcastable(array.shape[:-1], reciprocal_lattice_vectors.shape[:-2]):
+        #    raise ValueError()
+
+        # if not len(miller_indices) == reciprocal_lattice_vectors.shape[-3]:
+        #     raise ValueError(
+        #         "The number of miller indices and reciprocal space positions must be equal."
+        #     )
+
+        if not len(miller_indices) == array.shape[-1]:
+            raise ValueError(
+                "The number of miller indices must be equal to the number of diffraction spots."
+            )
 
         super().__init__(
             array=array,
             ensemble_axes_metadata=ensemble_axes_metadata,
             metadata=metadata,
         )
 
         self._miller_indices = miller_indices
         self._intensities = array
-        self._positions = positions
+        self._reciprocal_lattice_vectors = reciprocal_lattice_vectors
 
     def from_array_and_metadata(
         self, array: np.ndarray, axes_metadata: list[AxisMetadata], metadata: dict
     ) -> "T":
         raise NotImplementedError
 
     def _area_per_pixel(self):
@@ -3404,19 +3881,44 @@
     def intensities(self) -> np.ndarray:
         """
         Intensities of the diffraction spots.
         """
         return self._array
 
     @property
+    def reciprocal_lattice_vectors(self) -> np.ndarray:
+        """
+        Reciprocal lattice vectors of the diffraction spots.
+        """
+        return self._reciprocal_lattice_vectors
+
+    @property
     def positions(self) -> np.ndarray:
         """
         Reciprocal space positions of the diffraction spots.
         """
-        return self._positions
+        positions = self.miller_indices @ self.reciprocal_lattice_vectors
+        return positions
+
+    @property
+    def all_positions(self) -> np.ndarray:
+        """
+        Reciprocal space positions of the diffraction spots.
+        """
+        repeats = ()
+        for n, m in zip(self.shape[:-1], self.reciprocal_lattice_vectors.shape[:-2]):
+            if n == m:
+                repeats += (1,)
+            elif m == 1:
+                repeats += (n,)
+            else:
+                raise RuntimeError("Incompatible shapes.")
+
+        positions = np.tile(self.positions, repeats + (1, 1))
+        return positions
 
     @property
     def miller_indices(self) -> np.ndarray:
         """
         Miller indices of the diffraction spots.
         """
         return self._miller_indices
@@ -3442,42 +3944,70 @@
         ]
         return super()._pack_kwargs(kwargs)
 
     @classmethod
     def _unpack_kwargs(cls, attrs):
         kwargs = super()._unpack_kwargs(attrs)
         kwargs["miller_indices"] = np.array(kwargs["miller_indices"], dtype=int)
-        kwargs["positions"] = np.array(kwargs["positions"], dtype=np.float32)
         return kwargs
 
+    def __getitem__(self, items):
+        items = self._validate_items(items)
+        kwargs = self.get_items(items)
+
+        new_items = ()
+        for i, n in zip(items, self.reciprocal_lattice_vectors.shape):
+            if n == 1:
+                if isinstance(i, int):
+                    new_items += (0,)
+                else:
+                    new_items += (slice(None),)
+            else:
+                new_items += (i,)
+
+        # items = tuple(
+        #    0 if (isinstance(i, int) and (n == 1)) else slice(None)
+        #    for i, n in zip(items, self.reciprocal_lattice_vectors.shape)
+        # )
+        kwargs["reciprocal_lattice_vectors"] = self.reciprocal_lattice_vectors[
+            new_items
+        ]
+        return self.__class__(**kwargs)
+
     def remove_low_intensity(self, threshold: float = 1e-3):
         """
         Remove diffraction spots with intensity below a threshold for all ensemble dimensions.
 
         Parameters
         ----------
         threshold : float
             Intensity threshold for removing diffraction spots.
 
         Returns
         -------
         thresholded_spots : IndexedDiffractionPatterns
             The indexed diffraction spots with an intensity above the given threshold.
         """
-        ensemble_axes = tuple(range(len(self.ensemble_shape)))
-        mask = np.max(self.intensities, axis=ensemble_axes) > threshold
+        if self.is_lazy:
+            raise RuntimeError("Cannot threshold lazy IndexedDiffractionPatterns.")
+
+        ensemble_axes = tuple(range(self.ensemble_dims))
+
+        xp = get_array_module(self.intensities)
+        mask = xp.max(self.intensities, axis=ensemble_axes) > threshold
+
+        mask = asnumpy(mask)
 
         miller_indices = self.miller_indices[mask]
         intensities = self.intensities[..., mask]
-        positions = self.positions[mask]
 
         return self.__class__(
             intensities,
             miller_indices,
-            positions,
+            reciprocal_lattice_vectors=self.reciprocal_lattice_vectors,
             ensemble_axes_metadata=self.ensemble_axes_metadata,
             metadata=self._metadata,
         )
 
     def sort(self, criterion: str = "distance"):
         """
         Sort the diffraction spots according to a given criterion.
@@ -3494,67 +4024,78 @@
                 ``intensity`` :
                     Sort according to the intensity of the diffraction spots.
 
         Returns
         -------
         sorted_spots : IndexedDiffractionPatterns
         """
+        if self.lazy:
+            raise RuntimeError("Cannot sort lazy IndexedDiffractionPatterns.")
+
         if criterion == "distance":
             criterion = -np.linalg.norm(self.positions, axis=1)
         elif criterion == "intensity":
             ensemble_axes = tuple(range(len(self.ensemble_shape)))
             criterion = -np.max(self.intensities, axis=ensemble_axes)
         else:
             raise ValueError()
 
-        # print(criterion.shape)
-
         order = np.argsort(criterion)
-        positions = self.positions[order]
         array = self.array[..., order]
         miller_indices = self.miller_indices[order]
+        reciprocal_lattice_vectors = self.reciprocal_lattice_vectors[..., order, :, :]
 
         return self.__class__(
             array,
             miller_indices,
-            positions,
+            reciprocal_lattice_vectors=reciprocal_lattice_vectors,
             ensemble_axes_metadata=self.ensemble_axes_metadata,
             metadata=self._metadata,
         )
 
-    def crop(self, max_angle: float = None, max_frequency: float = None):
+    def crop(self, max_angle: float = None, k_max: float = None):
         """
         Crop the indexed diffraction patterns such that they only include spots with spatial frequencies
         (scattering angles) up to a given limit.
 
         Parameters
         ----------
         max_angle : float, optional
             The maximum included scattering angle in the cropped diffraction patterns.
-        max_frequency : float, optional
-            The maximum included spatial frequency in the cropped diffraction patterns.
+        k_max : float, optional
+            The maximum included reciprocal lattice vector in the cropped diffraction spots.
 
         Returns
         -------
         cropped : IndexedDiffractionPatterns
         """
-        if max_angle is not None and max_frequency is None:
-            mask = np.linalg.norm(self.angular_positions, axis=1) < max_angle
-        elif max_frequency is not None and max_angle is None:
-            mask = np.linalg.norm(self.positions, axis=1) < max_angle
-        else:
-            raise ValueError()
+
+        if max_angle is not None and k_max is None:
+            wavelength = energy2wavelength(self._get_from_metadata("energy"))
+            k_max = max_angle / wavelength / 1e3
+
+        elif not k_max or max_angle:
+            raise ValueError("Either 'max_angle' or 'k_max' must be given.")
+
+        mask = np.zeros(len(self.miller_indices), dtype=bool)
+
+        mask = reciprocal_lattice_vector_mask(
+            mask,
+            self.miller_indices.astype(self.reciprocal_lattice_vectors.dtype),
+            self.reciprocal_lattice_vectors,
+            k_max,
+        )
 
         miller_indices = self.miller_indices[mask]
         array = self.array[..., mask]
-        positions = self.positions[mask]
+
         return self.__class__(
             array,
             miller_indices,
-            positions,
+            reciprocal_lattice_vectors=self.reciprocal_lattice_vectors,
             ensemble_axes_metadata=self.ensemble_axes_metadata,
             metadata=self._metadata,
         )
 
     def normalize_to_spot(self, spot: tuple[int, int, int] = None):
         """
         Normalize the intensity of the diffraction spots.
@@ -3605,37 +4146,45 @@
             axes_metadata.label for axes_metadata in self.ensemble_axes_metadata
         ] + ["hkl"]
 
         data = xarray.DataArray(
             self.array,
             coords=coords,
             dims=dims,
+            attrs={
+                "long_name": "intensity",
+                "units": self.metadata.get("units", "arb. unit"),
+            },
         )
+
         return data
 
+    def _miller_indices_to_string(self):
+        return ["{} {} {}".format(*hkl) for hkl in self.miller_indices]
+
     def to_dataframe(self):
         """
         Convert the indexed diffraction patterns to pandas DataFrame.
 
         Returns
         -------
-        data_frame_of_indexed_spots : pd.DataFrame
+        data_frame : pd.DataFrame
         """
         import pandas as pd
 
         if self.ensemble_shape:
             if len(self.ensemble_shape) > 1:
                 raise RuntimeError(
                     "cannot convert indexed diffraction patterns with more than one ensemble axis to"
                     "dataframe"
                 )
 
             intensities = {
-                _format_miller_indices(hkl): self.intensities[..., i]
-                for i, hkl in enumerate(self.miller_indices)
+                hkl: self.intensities[..., i]
+                for i, hkl in enumerate(self._miller_indices_to_string())
             }
 
             axes_metadata = self.ensemble_axes_metadata[0]
 
             if hasattr(axes_metadata, "values"):
                 index = axes_metadata.values
             else:
@@ -3646,16 +4195,18 @@
             with config.set({"visualize.use_tex": False}):
                 df.index.name = self.axes_metadata[0].format_label()
                 df.columns.name = self.axes_metadata[1].format_label()
 
             return df
         else:
             intensities = {
-                _format_miller_indices(hkl): intensity
-                for hkl, intensity in zip(self.miller_indices, self.intensities)
+                hkl: intensity
+                for hkl, intensity in zip(
+                    self._miller_indices_to_string(), self.intensities
+                )
             }
             return pd.DataFrame(intensities, index=[0])
 
     def block_direct(self):
         """
         Remove the zero-order spot.
 
@@ -3665,43 +4216,49 @@
             The indexed diffraction spots without the zero-order spot.
         """
 
         to_delete = np.where(np.all(self.miller_indices == 0, axis=1))[0]
 
         miller_indices = np.delete(self.miller_indices, to_delete, axis=0)
         intensities = np.delete(self.intensities, to_delete, axis=-1)
-        positions = np.delete(self.positions, to_delete, axis=0)
 
         return self.__class__(
             intensities,
             miller_indices,
-            positions,
-            self.ensemble_axes_metadata,
-            self.metadata,
+            reciprocal_lattice_vectors=self.reciprocal_lattice_vectors,
+            ensemble_axes_metadata=self.ensemble_axes_metadata,
+            metadata=self._metadata,
+        )
+
+    def max_reciprocal_space_vector_length(self):
+        return calculate_max_reciprocal_space_vector(
+            self.miller_indices, self.reciprocal_lattice_vectors
         )
 
     def show(
         self,
         ax: Axes = None,
         cbar: bool = False,
         cmap: str = None,
         vmin: float = None,
         vmax: float = None,
         power: float = 1.0,
         common_color_scale: bool = False,
-        scale: float = 1,
-        explode: bool | Sequence[bool] = None,
+        scale: float = 0.5,
+        explode: bool | Sequence[bool] = (),
+        overlay: bool | Sequence[bool] = (),
         figsize: tuple[int, int] = None,
         title: bool | str = True,
         units: str = None,
         interact: bool = False,
         display: bool = True,
+        **kwargs,
     ):
         """
-        Show the diffraction spots using matplotlib.
+        Show the diffraction spots as an EllipseCollection using matplotlib.
 
         Parameters
         ----------
         ax : matplotlib.axes.Axes, optional
             If given the plots are added to the axis. This is not available for exploded plots.
         cbar : bool, optional
             Add colorbar(s) to the image(s). The size and padding of the colorbars may be adjusted using the
@@ -3723,60 +4280,60 @@
         explode : bool or sequence of bool, optional
             If True, a grid of plots is created for all the items of the last two ensemble axes. If False, the first
             ensemble item is shown. May be given as a sequence of axis indices to create a grid of plots from
             the specified axes. The default is determined by the axis metadata.
         figsize : two int, optional
             The figure size given as width and height in inches, passed to `matplotlib.pyplot.figure`.
         title : bool or str, optional
-            Set the column title of the images. If True is given instead of a string the title will be given by the
+            Set the column title of the plots. If True is given instead of a string the title will be given by the
             value corresponding to the "name" key of the axes metadata dictionary, if this item exists.
         units : str
-            The units used for the x and y axes. The given units must be compatible with the axes of the images.
+            The units used for the x and y axes. The given units must be compatible with the axes of the plots.
         interact : bool
             If True, create an interactive visualization. This requires enabling the ipympl Matplotlib backend.
         display : bool, optional
             If True (default) the figure is displayed immediately.
 
         Returns
         -------
-        measurement_visualization_2d : MeasurementVisualization2D
+        visualization : Visualization
         """
 
-        if not interact:
-            self.compute()
+        k_max = self.max_reciprocal_space_vector_length() * _get_conversion_factor(
+            units, "1/Å", self.metadata.get("energy", None)
+        )
+
+        xlim = [-k_max, k_max]
+        ylim = [-k_max, k_max]
 
-        visualization = DiffractionSpotsVisualization(
-            self,
+        visualization = Visualization(
+            measurement=self,
             ax=ax,
+            common_scale=common_color_scale,
+            figsize=figsize,
+            title=title,
+            aspect=True,
+            share_x=True,
+            share_y=True,
+            explode=explode,
+            overlay=overlay,
+            interactive=not interact and display,
+            value_limits=(vmin, vmax),
             power=power,
             cmap=cmap,
-            scale=scale,
             cbar=cbar,
-            common_scale=common_color_scale,
-            vmin=vmin,
-            vmax=vmax,
-            explode=explode,
-            figsize=figsize,
-            interact=interact,
+            scale=scale,
+            units=units,
+            xlim=xlim,
+            ylim=ylim,
+            **kwargs,
         )
 
-        if title is not None:
-            visualization.set_column_titles(title)
-
-        if units is not None:
-            visualization.set_xunits(units)
-            visualization.set_yunits(units)
-
-        if not display and not interact:
-            plt.close()
-
-        if interact and display:
-            from IPython.display import display as ipython_display
-
-            ipython_display(visualization.widgets)
+        if interact:
+            gui = visualization.interact(ScatterGUI, display=display)
 
         return visualization
 
     @property
     def intensities_dict(self) -> Dict[tuple[int, int, int], np.ndarray]:
         """
         A dictionary mapping miller indices to intensities.
@@ -3794,54 +4351,70 @@
         return intensities
 
     @property
     def positions_dict(self) -> Dict[tuple[int, int, int], np.ndarray]:
         """
         A dictionary mapping miller indices to reciprocal space positions [1/Å].
         """
+
         positions = {
             tuple(hkl): position
-            for hkl, position in zip(self.miller_indices, self.positions)
+            for hkl, position in zip(
+                self.miller_indices,
+                np.moveaxis(self.reciprocal_lattice_vectors, -2, 0),
+            )
         }
         return positions
 
     @classmethod
     def _stack(
         cls,
         diffraction_spots: IndexedDiffractionPatterns,
         axis_metadata: list[AxisMetadata],
         axis: int,
     ):
         intensities = [spots.intensities_dict for spots in diffraction_spots]
-        positions_dicts = [spots.positions_dict for spots in diffraction_spots]
-        positions = {k: v for d in positions_dicts for k, v in d.items()}
+        # positions = [spots.positions_dict for spots in diffraction_spots]
+
+        # def merge_dicts_no_overwrite(dict1, dict2):
+        #     return {**dict1, **{k: v for k, v in dict2.items() if k not in dict1}}
+
+        # merged = {}
+        # for positions1 in positions:
+        #     merged = merge_dicts_no_overwrite(merged, positions1)
+
+        # positions = [
+        #     merge_dicts_no_overwrite(positions1, merged) for positions1 in positions
+        # ]
 
         miller_indices = list(
             set(itertools.chain(*[intensities1.keys() for intensities1 in intensities]))
         )
 
-        # print(miller_indices)
-        # sss
-
         new_intensities = {}
+        # new_positions = {}
         for hkl in miller_indices:
             new_intensities[hkl] = []
+            # new_positions[hkl] = []
 
-            for intensity in intensities:
-                new_intensities[hkl].append(intensity[hkl])
+            for intensities1 in intensities:
+                new_intensities[hkl].append(intensities1[hkl])
+                # new_positions[hkl].append(positions1[hkl])
 
             new_intensities[hkl] = np.stack(new_intensities[hkl], axis=axis)
+            # new_positions[hkl] = np.stack(new_positions[hkl], axis=axis)
 
-        positions = dict(sorted(positions.items()))
-        intensities = dict(sorted(new_intensities.items()))
+        miller_indices = np.stack(list(new_intensities.keys()), axis=0)
 
-        miller_indices = np.stack(list(intensities.keys()), axis=0)
+        # positions = np.stack(list(new_positions.values()), axis=-2)
+        intensities = np.stack(list(new_intensities.values()), axis=-1)
 
-        positions = np.stack(list(positions.values()))
-        intensities = np.stack(list(intensities.values()), axis=-1)
+        positions = np.stack(
+            [spots.reciprocal_lattice_vectors for spots in diffraction_spots], axis=0
+        )
 
         ensemble_axes_metadata = [
             axis_metadata.copy()
             for axis_metadata in diffraction_spots[0].ensemble_axes_metadata
         ]
         ensemble_axes_metadata.insert(axis, axis_metadata)
         metadata = diffraction_spots[0].metadata
```

### Comparing `abtem-1.0.4/abtem/mtf.py` & `abtem-1.0.5/abtem/mtf.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/parametrizations/__init__.py` & `abtem-1.0.5/abtem/parametrizations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 
 import numpy as np
 from ase.data import chemical_symbols
 from scipy.optimize import least_squares
 
 from abtem.array import concatenate
 from abtem.core.axes import OrdinalAxis
+from abtem.core.config import config
 from abtem.core.constants import kappa
-from abtem.core.utils import EqualityMixin
+from abtem.core.utils import EqualityMixin, get_dtype
 from abtem.measurements import ReciprocalSpaceLineProfiles, RealSpaceLineProfiles
 from abtem.parametrizations.functions import kirkland, ewald, peng, lobato
 
 
 def _get_data_path():
     this_file = os.path.abspath(os.path.dirname(__file__))
     return os.path.join(this_file, "data")
@@ -66,15 +67,14 @@
         "x_ray_scattering_factor",
         "finite_projected_scattering_factor",
     )
 
     def __init__(
         self, parameters: dict[str, np.ndarray] | str, sigmas: dict[str, float] = None
     ):
-
         self._parameters = validate_parameters(parameters)
         self._sigmas = validate_sigmas(sigmas)
 
     def to_json(self, file: str):
         with open(file, "w") as fp:
             data = {
                 symbol: parameters.tolist()
@@ -293,15 +293,16 @@
             charge_symbol = "+" * int(abs(charge))
         else:
             charge_symbol = "-" * int(abs(charge))
 
         try:
             func = self._functions[name]
             parameters = self.scaled_parameters(symbol + charge_symbol, name)
-            parameters = np.array(parameters, dtype=np.float32)
+            dtype = get_dtype(complex=False)
+            parameters = np.array(parameters, dtype=dtype)
             return lambda r, *args, **kwargs: func(r, parameters, *args, **kwargs)
         except KeyError:
             raise RuntimeError(
                 f'parametrized function "{name}" does not exist for element {symbol} with charge {charge}'
             )
 
     def line_profiles(
@@ -396,15 +397,14 @@
         "projected_potential": kirkland.projected_potential,
         "projected_scattering_factor": kirkland.projected_scattering_factor,
     }
 
     def __init__(
         self, parameters: str | dict = "kirkland.json", sigmas: dict[str, float] = None
     ):
-
         super().__init__(parameters=parameters, sigmas=sigmas)
 
     def fit(self, Z, k, f, guess=None):
         def reshape_parameters(p):
             p = p.reshape((4, 3))
             return p
 
@@ -435,15 +435,14 @@
 
         result = least_squares(residuals_func, guess.ravel())
         p_optimal = reshape_parameters(result.x)
         p_optimal = apply_constraint(p_optimal)
         self.parameters[chemical_symbols[Z]] = p_optimal
         return p_optimal
 
-
     def scaled_parameters(self, symbol: str, name: str) -> np.ndarray:
         parameters = np.array(self.parameters[symbol])
 
         a = np.pi * parameters[0] / kappa
         b = 2.0 * np.pi * np.sqrt(parameters[1])
         c = np.pi ** (3.0 / 2.0) * parameters[2] / parameters[3] ** (3.0 / 2.0) / kappa
         d = np.pi**2 / parameters[3]
@@ -534,17 +533,17 @@
         parameters = np.array(self.parameters[symbol])
 
         a = np.pi**2 * parameters[0] / parameters[1] ** (3 / 2.0) / kappa
         b = 2 * np.pi / np.sqrt(parameters[1])
         scaled_parameters = np.vstack((a, b))
 
         scaled_parameters = {
-            "potential": scaled_parameters.astype(np.float32),
+            "potential": scaled_parameters,
             "scattering_factor": parameters,
-            "projected_potential": scaled_parameters.astype(np.float32),
+            "projected_potential": scaled_parameters,
             "projected_scattering_factor": scaled_parameters,
             "x_ray_scattering_factor": parameters,
             "charge": parameters,
         }
 
         return scaled_parameters[name]
 
@@ -659,17 +658,15 @@
     if isinstance(parametrization, str):
         parametrization = named_parametrizations[parametrization]()
 
     return parametrization
 
 
 def validate_parameters(parameters: str | dict) -> dict:
-
     if isinstance(parameters, str):
-
         if os.path.isabs(parameters):
             path = parameters
         else:
             path = os.path.join(_get_data_path(), parameters)
 
         with open(path, "r") as f:
             parameters = json.load(f)
```

### Comparing `abtem-1.0.4/abtem/parametrizations/data/kirkland.json` & `abtem-1.0.5/abtem/parametrizations/data/kirkland.json`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/parametrizations/data/lobato.json` & `abtem-1.0.5/abtem/parametrizations/data/lobato.json`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/parametrizations/data/peng_high.json` & `abtem-1.0.5/abtem/parametrizations/data/peng_high.json`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/parametrizations/data/peng_ionic.json` & `abtem-1.0.5/abtem/parametrizations/data/peng_ionic.json`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/parametrizations/data/peng_low.json` & `abtem-1.0.5/abtem/parametrizations/data/peng_low.json`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/parametrizations/data/waasmaier_kirfel.json` & `abtem-1.0.5/abtem/parametrizations/data/waasmaier_kirfel.json`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/parametrizations/functions/ewald.py` & `abtem-1.0.5/abtem/parametrizations/functions/ewald.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/parametrizations/functions/kirkland.py` & `abtem-1.0.5/abtem/parametrizations/functions/kirkland.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/parametrizations/functions/lobato.py` & `abtem-1.0.5/abtem/parametrizations/functions/lobato.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/parametrizations/functions/peng.py` & `abtem-1.0.5/abtem/parametrizations/functions/peng.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/potentials/_poisson.py` & `abtem-1.0.5/abtem/potentials/_poisson.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/potentials/charge_density.py` & `abtem-1.0.5/abtem/potentials/charge_density.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,15 @@
         )
 
     @property
     def frozen_phonons(self):
         return self._frozen_phonons
 
     @property
-    def num_frozen_phonons(self):
+    def num_configurations(self):
         return len(self.frozen_phonons)
 
     @property
     def ensemble_axes_metadata(self):
         return self.frozen_phonons.ensemble_axes_metadata
 
     @property
```

### Comparing `abtem-1.0.4/abtem/potentials/gpaw.py` & `abtem-1.0.5/abtem/potentials/gpaw.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     DummyFrozenPhonons,
     FrozenPhonons,
     BaseFrozenPhonons,
     _safe_read_atoms,
 )
 from abtem.potentials.charge_density import _generate_slices
 from abtem.potentials.charge_density import _interpolate_slice
-from abtem.potentials.iam import _PotentialBuilder, Potential
+from abtem.potentials.iam import _PotentialBuilder, Potential, PotentialArray
 
 try:
     from gpaw import GPAW
     from gpaw.lfc import LFC, BasisFunctions
     from gpaw.transformers import Transformer
     from gpaw.utilities import unpack2
     from gpaw.atom.aeatom import AllElectronAtom
@@ -230,28 +230,33 @@
     def __init__(self, potential):
         self._potential = potential
         super().__init__()
 
     def potential(self, symbol):
         return self._potential
 
+    @property
+    def sigmas(self):
+        return {}
+
 
 def _generate_slices(
     interpolators,
     valence_potential,
     atoms,
     gpts,
     slice_thickness,
     first_slice=0,
     last_slice=None,
 ):
 
     potential_generators = []
     for i, interpolator in enumerate(interpolators):
         parametrization = _DummyParametrization(interpolator)
+
         potential = Potential(
             gpts=gpts,
             atoms=atoms[i : i + 1],
             parametrization=parametrization,
             slice_thickness=slice_thickness,
             projection="finite",
         )
@@ -395,14 +400,15 @@
         self._gridrefinement = gridrefinement
         self._repetitions = repetitions
 
         cell = frozen_phonons.atoms.cell * repetitions
         frozen_phonons.atoms.calc = None
 
         super().__init__(
+            array_object=PotentialArray,
             gpts=gpts,
             sampling=sampling,
             cell=cell,
             slice_thickness=slice_thickness,
             exit_planes=exit_planes,
             device=device,
             plane=plane,
@@ -412,14 +418,18 @@
         )
 
     @property
     def frozen_phonons(self):
         return self._frozen_phonons
 
     @property
+    def num_configurations(self):
+        return self.frozen_phonons.num_configs
+
+    @property
     def repetitions(self):
         return self._repetitions
 
     @property
     def gridrefinement(self):
         return self._gridrefinement
 
@@ -459,15 +469,15 @@
             nt_sG = calculator.nt_sG
 
         random_atoms = self.frozen_phonons.randomize(atoms)
 
         calc = GPAW(txt=None, mode=calculator.setup_mode, xc=calculator.setup_xc)
         calc.initialize(random_atoms)
 
-        return _get_all_electron_density(
+        return self._get_all_electron_density(
             nt_sG=nt_sG,
             gd=gd,
             D_asp=calculator.D_asp,
             setups=calc.setups,
             gridrefinement=self.gridrefinement,
             atoms=random_atoms,
         )
```

### Comparing `abtem-1.0.4/abtem/potentials/iam.py` & `abtem-1.0.5/abtem/potentials/iam.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Module for describing electrostatic potentials using the independent atom model."""
+
 from __future__ import annotations
 
 import warnings
-from abc import abstractmethod
+from abc import abstractmethod, ABCMeta
 from functools import partial
 from functools import reduce
 from numbers import Number
 from operator import mul
-from typing import Sequence, TYPE_CHECKING
+from typing import Sequence, TYPE_CHECKING, Type
 
 import dask
 import dask.array as da
 import numpy as np
 from ase import Atoms
 from ase.cell import Cell
 from ase.data import chemical_symbols
@@ -34,79 +35,62 @@
 from abtem.core.backend import get_array_module, validate_device
 from abtem.core.chunks import generate_chunks, Chunks, chunk_ranges
 from abtem.core.chunks import validate_chunks
 from abtem.core.complex import complex_exponential
 from abtem.core.energy import HasAcceleratorMixin, Accelerator, energy2sigma
 from abtem.core.ensemble import Ensemble, _wrap_with_array, unpack_blockwise_args
 from abtem.core.grid import Grid, HasGridMixin
-
-from abtem.integrals import GaussianProjectionIntegrals
-from abtem.integrals import ProjectedScatteringFactors
-from abtem.integrals import ProjectionQuadratureRule
-from abtem.core.utils import EqualityMixin, CopyMixin
+from abtem.core.utils import EqualityMixin, CopyMixin, get_dtype
 from abtem.inelastic.phonons import (
     BaseFrozenPhonons,
     DummyFrozenPhonons,
     _validate_seeds,
-    AtomsEnsemble, _safe_read_atoms,
+    AtomsEnsemble,
+)
+from abtem.integrals import (
+    ScatteringFactorProjectionIntegrals,
+    QuadratureProjectionIntegrals,
 )
 from abtem.measurements import Images
 from abtem.slicing import (
     _validate_slice_thickness,
     SliceIndexedAtoms,
     SlicedAtoms,
     BaseSlicedAtoms,
 )
 
 if TYPE_CHECKING:
     from abtem.waves import Waves, BaseWaves
     from abtem.parametrizations import Parametrization
-    from abtem.integrals import ProjectionIntegratorPlan
-
+    from abtem.integrals import FieldIntegrator
 
-class BasePotential(
-    Ensemble,
-    HasGridMixin,
-    EqualityMixin,
-    CopyMixin,
-):
-    """Base class of all potentials. Documented in the subclasses."""
 
+class BaseField(Ensemble, HasGridMixin, EqualityMixin, CopyMixin, metaclass=ABCMeta):
     @property
+    @abstractmethod
     def base_shape(self) -> tuple[int, ...]:
-        """Shape of the base axes of the potential."""
-        return (self.num_slices,) + self.gpts
+        pass
 
     @property
     @abstractmethod
-    def num_frozen_phonons(self) -> int:
+    def num_configurations(self):
         """Number of frozen phonons in the ensemble of potentials."""
         pass
 
     @property
-    def base_axes_metadata(self) -> list[AxisMetadata]:
-        """List of AxisMetadata for the base axes."""
-        return [
-            ThicknessAxis(
-                label="z", values=tuple(np.cumsum(self.slice_thickness)), units="Å"
-            ),
-            RealSpaceAxis(
-                label="x", sampling=self.sampling[0], units="Å", endpoint=False
-            ),
-            RealSpaceAxis(
-                label="y", sampling=self.sampling[1], units="Å", endpoint=False
-            ),
-        ]
+    @abstractmethod
+    def base_axes_metadata(self):
+        pass
 
     def _get_exit_planes_axes_metadata(self):
         return ThicknessAxis(label="z", values=tuple(self.exit_thicknesses))
 
     @property
     @abstractmethod
-    def exit_planes(self) -> tuple[int, ...]:
+    def exit_planes(self) -> tuple[int]:
         """The "exit planes" of the potential. The indices of slices where a measurement is returned."""
         pass
 
     @property
     def _exit_plane_after(self):
         exit_plane_index = 0
         exit_planes = self.exit_planes
@@ -207,15 +191,15 @@
         Converts the potential to an ensemble of images.
 
         Returns
         -------
         image_ensemble : Images
             The potential slices as images.
         """
-        return self.build().complex_images()
+        return self.build().to_images()
 
     def show(self, project: bool = True, **kwargs):
         """
         Show the potential projection. This requires building all potential slices.
 
         Parameters
         ----------
@@ -230,14 +214,38 @@
         else:
             if "explode" not in kwargs.keys():
                 kwargs["explode"] = True
 
             return self.to_images().show(**kwargs)
 
 
+class BasePotential(BaseField):
+    """Base class of all potentials. Documented in the subclasses."""
+
+    @property
+    def base_shape(self):
+        """Shape of the base axes of the potential."""
+        return (self.num_slices,) + self.gpts
+
+    @property
+    def base_axes_metadata(self):
+        """List of AxisMetadata for the base axes."""
+        return [
+            ThicknessAxis(
+                label="z", values=tuple(np.cumsum(self.slice_thickness)), units="Å"
+            ),
+            RealSpaceAxis(
+                label="x", sampling=self.sampling[0], units="Å", endpoint=False
+            ),
+            RealSpaceAxis(
+                label="y", sampling=self.sampling[1], units="Å", endpoint=False
+            ),
+        ]
+
+
 def _validate_potential(
     potential: Atoms | BasePotential, waves: BaseWaves = None
 ) -> BasePotential:
     if isinstance(potential, (Atoms, BaseFrozenPhonons)):
         device = None
         if waves is not None:
             device = waves.device
@@ -263,31 +271,52 @@
         exit_planes = (-1,) + tuple(exit_planes)
     elif exit_planes is None:
         exit_planes = (num_slices - 1,)
 
     return exit_planes
 
 
-class _PotentialBuilder(BasePotential):
+def _require_cell_transform(cell, box, plane, origin):
+    if box == tuple(np.diag(cell)):
+        return False
+
+    if not is_cell_orthogonal(cell):
+        return True
+
+    if box is not None:
+        return True
+
+    if plane != "xy":
+        return True
+
+    if origin != (0.0, 0.0, 0.0):
+        return True
+
+    return False
+
+
+class _FieldBuilder(BaseField):
     def __init__(
         self,
+        array_object: Type[FieldArray],
         slice_thickness: float | tuple[float, ...],
         exit_planes: int | tuple[int, ...],
         cell: np.ndarray | Cell,
         gpts: int | tuple[int, int] = None,
         sampling: float | tuple[float, float] = None,
         box: tuple[float, float, float] = None,
-        plane: str
-        | tuple[tuple[float, float, float], tuple[float, float, float]] = "xy",
+        plane: (
+            str | tuple[tuple[float, float, float], tuple[float, float, float]]
+        ) = "xy",
         origin: tuple[float, float, float] = (0.0, 0.0, 0.0),
         periodic: bool = True,
         device: str = None,
     ):
-
-        if self._require_cell_transform(cell, box=box, plane=plane, origin=origin):
+        self._array_object = array_object
+        if _require_cell_transform(cell, box=box, plane=plane, origin=origin):
             axes = plane_to_axes(plane)
             cell = cell[:, list(axes)]
             box = tuple(best_orthogonal_cell(cell))
 
         elif box is None:
             box = tuple(np.diag(cell))
 
@@ -338,49 +367,30 @@
         return self._box
 
     @property
     def origin(self) -> tuple[float, float, float]:
         """The origin relative to the provided atoms mapped to the origin of the potential."""
         return self._origin
 
-    def _require_cell_transform(self, cell, box, plane, origin):
-
-        if box == tuple(np.diag(cell)):
-            return False
-
-        if not is_cell_orthogonal(cell):
-            return True
-
-        if box is not None:
-            return True
-
-        if plane != "xy":
-            return True
-
-        if origin != (0.0, 0.0, 0.0):
-            return True
-
-        return False
-
-    def __getitem__(self, item) -> "PotentialArray":
+    def __getitem__(self, item) -> PotentialArray:
         return self.build(lazy=False)[item]
 
     @staticmethod
     def _wrap_build_potential(potential, first_slice, last_slice):
         potential = potential.item()
         array = potential.build(first_slice, last_slice, lazy=False).array
         return array
 
     def build(
         self,
         first_slice: int = 0,
         last_slice: int = None,
         max_batch: int | str = 1,
         lazy: bool = None,
-    ) -> PotentialArray:
+    ) -> FieldArray:
         """
         Build the potential.
 
         Parameters
         ----------
         first_slice : int, optional
             Index of the first slice of the generated potential.
@@ -406,176 +416,92 @@
             last_slice = len(self)
 
         if lazy:
             blocks = self.ensemble_blocks(self._default_ensemble_chunks)
 
             xp = get_array_module(self.device)
             chunks = validate_chunks(self.ensemble_shape, self._default_ensemble_chunks)
-            chunks = chunks + ((len(self),), (self.gpts[0],), (self.gpts[1],))
+            chunks = chunks + self.base_shape
 
             if self.ensemble_shape:
                 new_axis = tuple(
-                    range(len(self.ensemble_shape), len(self.ensemble_shape) + 3)
+                    range(
+                        len(self.ensemble_shape),
+                        len(self.ensemble_shape) + len(self.base_shape),
+                    )
                 )
             else:
-                new_axis = tuple(range(1, 3))
+                new_axis = tuple(range(1, len(self.base_shape)))
 
             array = blocks.map_blocks(
                 self._wrap_build_potential,
                 new_axis=new_axis,
                 first_slice=first_slice,
                 last_slice=last_slice,
                 chunks=chunks,
-                meta=xp.array((), dtype=np.float32),
+                meta=xp.array((), dtype=get_dtype(complex=False)),
             )
 
-
         else:
             xp = get_array_module(self.device)
 
             array = xp.zeros(
-                self.ensemble_shape + (last_slice - first_slice,) + self.gpts,
-                dtype=xp.float32,
+                self.ensemble_shape + (last_slice - first_slice,) + self.base_shape[1:],
+                dtype=get_dtype(complex=False),
             )
 
             if self.ensemble_shape:
                 for i, _, potential in self.generate_blocks(1):
                     potential = potential.item()
                     i = np.unravel_index((0,), self.ensemble_shape)
 
                     for j, slic in enumerate(
                         potential.generate_slices(first_slice, last_slice)
                     ):
-
                         array[i + (j,)] = slic.array[0]
 
             else:
                 for j, slic in enumerate(self.generate_slices(first_slice, last_slice)):
                     array[j] = slic.array[0]
 
-        potential = PotentialArray(
+        potential = self._array_object(
             array,
             sampling=(self.sampling[0], self.sampling[1]),
             slice_thickness=self.slice_thickness[first_slice:last_slice],
             exit_planes=self.exit_planes,
             ensemble_axes_metadata=self.ensemble_axes_metadata,
         )
         return potential
 
 
-class Potential(_PotentialBuilder):
-    """
-    Calculate the electrostatic potential of a set of atoms or frozen phonon configurations. The potential is calculated
-    with the Independent Atom Model (IAM) using a user-defined parametrization of the atomic potentials.
-
-    Parameters
-    ----------
-    atoms : ase.Atoms or abtem.FrozenPhonons
-        Atoms or FrozenPhonons defining the atomic configuration(s) used in the independent atom model for calculating
-        the electrostatic potential(s).
-    gpts : one or two int, optional
-        Number of grid points in `x` and `y` describing each slice of the potential. Provide either "sampling" (spacing
-        between consecutive grid points) or "gpts" (total number of grid points).
-    sampling : one or two float, optional
-        Sampling of the potential in `x` and `y` [1 / Å]. Provide either "sampling" or "gpts".
-    slice_thickness : float or sequence of float, optional
-        Thickness of the potential slices in the propagation direction in [Å] (default is 0.5 Å).
-        If given as a float, the number of slices is calculated by dividing the slice thickness into the `z`-height of
-        supercell. The slice thickness may be given as a sequence of values for each slice, in which case an error will
-        be thrown if the sum of slice thicknesses is not equal to the height of the atoms.
-    parametrization : 'lobato' or 'kirkland', optional
-        The potential parametrization describes the radial dependence of the potential for each element. Two of the
-        most accurate parametrizations are available (by Lobato et al. and Kirkland; default is 'lobato').
-        See the citation guide for references.
-    projection : 'finite' or 'infinite', optional
-        If 'finite' the 3D potential is numerically integrated between the slice boundaries. If 'infinite' (default),
-        the infinite potential projection of each atom will be assigned to a single slice.
-    exit_planes : int or tuple of int, optional
-        The `exit_planes` argument can be used to calculate thickness series.
-        Providing `exit_planes` as a tuple of int indicates that the tuple contains the slice indices after which an
-        exit plane is desired, and hence during a multislice simulation a measurement is created. If `exit_planes` is
-        an integer a measurement will be collected every `exit_planes` number of slices.
-    plane : str or two tuples of three float, optional
-        The plane relative to the provided atoms mapped to `xy` plane of the potential, i.e. provided plane is
-        perpendicular to the propagation direction. If string, it must be a concatenation of two of 'x', 'y' and 'z';
-        the default value 'xy' indicates that potential slices are cuts along the `xy`-plane of the atoms.
-        The plane may also be specified with two arbitrary 3D vectors, which are mapped to the `x` and `y` directions of
-        the potential, respectively. The length of the vectors has no influence. If the vectors are not perpendicular,
-        the second vector is rotated in the plane to become perpendicular to the first. Providing a value of
-        ((1., 0., 0.), (0., 1., 0.)) is equivalent to providing 'xy'.
-    origin : three float, optional
-        The origin relative to the provided atoms mapped to the origin of the potential. This is equivalent to
-        translating the atoms. The default is (0., 0., 0.).
-    box : three float, optional
-        The extent of the potential in `x`, `y` and `z`. If not given this is determined from the atoms' cell.
-        If the box size does not match an integer number of the atoms' supercell, an affine transformation may be
-        necessary to preserve periodicity, determined by the `periodic` keyword.
-    periodic : bool, True
-        If a transformation of the atomic structure is required, `periodic` determines how the atomic structure is
-        transformed. If True, the periodicity of the Atoms is preserved, which may require applying a small affine
-        transformation to the atoms. If False, the transformed potential is effectively cut out of a larger repeated
-        potential, which may not preserve periodicity.
-    integrator : ProjectionIntegrator, optional
-        Provide a custom integrator for the projection integrals of the potential slicing.
-    device : str, optional
-        The device used for calculating the potential, 'cpu' or 'gpu'. The default is determined by the user
-        configuration file.
-    """
-
-    _exclude_from_copy = ("parametrization", "projection", "integral_method")
-
+class _FieldBuilderFromAtoms(_FieldBuilder):
     def __init__(
         self,
-        atoms: Atoms | BaseFrozenPhonons = None,
+        atoms: Atoms | BaseFrozenPhonons,
+        array_object: Type[FieldArray],
         gpts: int | tuple[int, int] = None,
         sampling: float | tuple[float, float] = None,
         slice_thickness: float | tuple[float, ...] = 1,
-        parametrization: str | Parametrization = "lobato",
-        projection: str = "infinite",
         exit_planes: int | tuple[int, ...] = None,
-        plane: str
-        | tuple[tuple[float, float, float], tuple[float, float, float]] = "xy",
+        plane: (
+            str | tuple[tuple[float, float, float], tuple[float, float, float]]
+        ) = "xy",
         origin: tuple[float, float, float] = (0.0, 0.0, 0.0),
         box: tuple[float, float, float] = None,
         periodic: bool = True,
-        integrator: ProjectionIntegratorPlan = None,
+        integrator=None,
         device: str = None,
     ):
-
-        if isinstance(atoms, Atoms):
-            atoms = atoms.copy()
-            atoms.calc = None
-
-        if not hasattr(atoms, "randomize"):
-
-            if isinstance(atoms, (list, tuple)):
-                self._frozen_phonons = AtomsEnsemble(atoms)
-            elif isinstance(atoms, Atoms):
-                self._frozen_phonons = DummyFrozenPhonons(atoms)
-            elif isinstance(atoms, str):
-                self._frozen_phonons = DummyFrozenPhonons(_safe_read_atoms(atoms))
-            else:
-                raise ValueError()
-        else:
-            self._frozen_phonons = atoms
-
-        if integrator is None:
-            if projection == "finite":
-                integrator = ProjectionQuadratureRule(parametrization=parametrization)
-            elif projection == "infinite":
-                integrator = ProjectedScatteringFactors(
-                    parametrization=parametrization
-                )
-            else:
-                raise NotImplementedError
-
+        self._frozen_phonons = _validate_frozen_phonons(atoms)
         self._integrator = integrator
         self._sliced_atoms = None
+        self._array_object = array_object
 
         super().__init__(
+            array_object=array_object,
             gpts=gpts,
             sampling=sampling,
             cell=self._frozen_phonons.cell,
             slice_thickness=slice_thickness,
             exit_planes=exit_planes,
             device=device,
             plane=plane,
@@ -586,27 +512,30 @@
 
     @property
     def frozen_phonons(self) -> BaseFrozenPhonons:
         """Ensemble of atomic configurations representing frozen phonons."""
         return self._frozen_phonons
 
     @property
-    def num_frozen_phonons(self) -> int:
+    def num_configurations(self) -> int:
         """Size of the ensemble of atomic configurations representing frozen phonons."""
         return len(self.frozen_phonons)
 
     @property
-    def integrator(self) -> ProjectionIntegratorPlan:
+    def integrator(self):
         """The integrator determining how the projection integrals for each slice is calculated."""
         return self._integrator
 
     def _cutoffs(self):
         atoms = self.frozen_phonons.atoms
         unique_numbers = np.unique(atoms.numbers)
-        return tuple(self._integrator.cutoff(number) for number in unique_numbers)
+        return tuple(
+            self._integrator.cutoff(chemical_symbols[number])
+            for number in unique_numbers
+        )
 
     def get_transformed_atoms(self):
         """
         The atoms used in the multislice algorithm, transformed to the given plane, origin and box.
 
         Returns
         -------
@@ -638,15 +567,14 @@
                     origin=self.origin,
                     margin=max(cutoffs) if cutoffs else 0.0,
                 )
 
         return atoms
 
     def _prepare_atoms(self):
-
         atoms = self.get_transformed_atoms()
 
         if self.integrator.finite:
             cutoffs = self._cutoffs()
             margins = max(cutoffs) if len(cutoffs) else 0.0
         else:
             margins = 0.0
@@ -714,75 +642,65 @@
 
         xp = get_array_module(self.device)
 
         sliced_atoms = self.get_sliced_atoms()
 
         numbers = np.unique(sliced_atoms.atoms.numbers)
 
-        integrators = {
-            number: self.integrator.build(
-                chemical_symbols[number],
-                gpts=self.gpts,
-                sampling=self.sampling,
-                device=self.device,
-            )
-            for number in numbers
-        }
-
         exit_plane_after = self._exit_plane_after
 
-        cum_thickness = np.cumsum(self.slice_thickness)
+        cumulative_thickness = np.cumsum(self.slice_thickness)
 
         for start, stop in generate_chunks(
             last_slice - first_slice, chunks=1, start=first_slice
         ):
-
             if len(numbers) > 1 or stop - start > 1:
-                array = xp.zeros((stop - start,) + self.gpts, dtype=np.float32)
+                array = xp.zeros(
+                    (stop - start,) + self.base_shape[1:],
+                    dtype=get_dtype(complex=False),
+                )
             else:
                 array = None
 
             for i, slice_idx in enumerate(range(start, stop)):
+                atoms = sliced_atoms.get_atoms_in_slices(slice_idx)
 
-                for Z, integrator in integrators.items():
-                    atoms = sliced_atoms.get_atoms_in_slices(slice_idx, atomic_number=Z)
-
-                    new_array = integrator.integrate_on_grid(
-                        positions=atoms.positions,
-                        a=sliced_atoms.slice_limits[slice_idx][0],
-                        b=sliced_atoms.slice_limits[slice_idx][1],
-                        gpts=self.gpts,
-                        sampling=self.sampling,
-                        device=self.device,
-                    )
-
-                    if array is not None:
-                        array[i] += new_array
-                    else:
-                        array = new_array[None]
-
-
+                new_array = self._integrator.integrate_on_grid(
+                    atoms,
+                    a=sliced_atoms.slice_limits[slice_idx][0],
+                    b=sliced_atoms.slice_limits[slice_idx][1],
+                    gpts=self.gpts,
+                    sampling=self.sampling,
+                    device=self.device,
+                )
 
+                if array is not None:
+                    array[i] += new_array
+                else:
+                    array = new_array[None]
 
             if array is None:
-                array = xp.zeros((stop - start,) + self.gpts, dtype=np.float32)
+                array = xp.zeros(
+                    (stop - start,) + self.base_shape[1:],
+                    dtype=get_dtype(complex=False),
+                )
 
-            array -= array.min()
+            # array -= array.min()
 
             exit_planes = tuple(np.where(exit_plane_after[start:stop])[0])
 
-            potential_array = PotentialArray(
+            potential_array = self._array_object(
                 array,
                 slice_thickness=self.slice_thickness[start:stop],
                 exit_planes=exit_planes,
                 extent=self.extent,
             )
 
             if return_depth:
-                depth = cum_thickness[stop - 1]
+                depth = cumulative_thickness[stop - 1]
                 yield depth, potential_array
             else:
                 yield potential_array
 
     @property
     def ensemble_axes_metadata(self):
         return self.frozen_phonons.ensemble_axes_metadata
@@ -814,125 +732,195 @@
             **kwargs,
         )
 
     def _partition_args(self, chunks: Chunks = (1,), lazy: bool = True):
         return self.frozen_phonons._partition_args(chunks, lazy=lazy)
 
 
-class PotentialArray(BasePotential, ArrayObject):
+class _PotentialBuilder(_FieldBuilder, BasePotential):
+    pass
+
+
+def _validate_frozen_phonons(atoms):
+    if isinstance(atoms, Atoms):
+        atoms = atoms.copy()
+        atoms.calc = None
+
+    if not hasattr(atoms, "randomize"):
+        if isinstance(atoms, (list, tuple)):
+            frozen_phonons = AtomsEnsemble(atoms)
+        elif isinstance(atoms, Atoms):
+            frozen_phonons = DummyFrozenPhonons(atoms)
+        else:
+            raise ValueError()
+    else:
+        frozen_phonons = atoms
+
+    return frozen_phonons
+
+
+class Potential(_FieldBuilderFromAtoms, BasePotential):
     """
-    The potential array represents slices of the electrostatic potential as an array. All other potentials build
-    potential arrays.
+    Calculate the electrostatic potential of a set of atoms or frozen phonon configurations. The potential is calculated
+    with the Independent Atom Model (IAM) using a user-defined parametrization of the atomic potentials.
 
     Parameters
     ----------
-    array: 3D np.ndarray
-        The array representing the potential slices. The first dimension is the slice index and the last two are the
-        spatial dimensions.
-    slice_thickness: float
-        The thicknesses of potential slices [Å]. If a float, the thickness is the same for all slices.
-        If a sequence, the length must equal the length of the potential array.
-    extent: one or two float, optional
-        Lateral extent of the potential [Å].
-    sampling: one or two float, optional
-        Lateral sampling of the potential [1 / Å].
+    atoms : ase.Atoms or abtem.FrozenPhonons
+        Atoms or FrozenPhonons defining the atomic configuration(s) used in the independent atom model for calculating
+        the electrostatic potential(s).
+    gpts : one or two int, optional
+        Number of grid points in `x` and `y` describing each slice of the potential. Provide either "sampling" (spacing
+        between consecutive grid points) or "gpts" (total number of grid points).
+    sampling : one or two float, optional
+        Sampling of the potential in `x` and `y` [1 / Å]. Provide either "sampling" or "gpts".
+    slice_thickness : float or sequence of float, optional
+        Thickness of the potential slices in the propagation direction in [Å] (default is 0.5 Å).
+        If given as a float, the number of slices is calculated by dividing the slice thickness into the `z`-height of
+        supercell. The slice thickness may be given as a sequence of values for each slice, in which case an error will
+        be thrown if the sum of slice thicknesses is not equal to the height of the atoms.
+    parametrization : 'lobato' or 'kirkland', optional
+        The potential parametrization describes the radial dependence of the potential for each element. Two of the
+        most accurate parametrizations are available (by Lobato et al. and Kirkland; default is 'lobato').
+        See the citation guide for references.
+    projection : 'finite' or 'infinite', optional
+        If 'finite' the 3D potential is numerically integrated between the slice boundaries. If 'infinite' (default),
+        the infinite potential projection of each atom will be assigned to a single slice.
     exit_planes : int or tuple of int, optional
         The `exit_planes` argument can be used to calculate thickness series.
         Providing `exit_planes` as a tuple of int indicates that the tuple contains the slice indices after which an
         exit plane is desired, and hence during a multislice simulation a measurement is created. If `exit_planes` is
         an integer a measurement will be collected every `exit_planes` number of slices.
-    ensemble_axes_metadata : list of AxesMetadata
-        Axis metadata for each ensemble axis. The axis metadata must be compatible with the shape of the array.
-    metadata : dict
-        A dictionary defining wave function metadata. All items will be added to the metadata of measurements derived
-        from the waves.
+    plane : str or two tuples of three float, optional
+        The plane relative to the provided atoms mapped to `xy` plane of the potential, i.e. provided plane is
+        perpendicular to the propagation direction. If string, it must be a concatenation of two of 'x', 'y' and 'z';
+        the default value 'xy' indicates that potential slices are cuts along the `xy`-plane of the atoms.
+        The plane may also be specified with two arbitrary 3D vectors, which are mapped to the `x` and `y` directions of
+        the potential, respectively. The length of the vectors has no influence. If the vectors are not perpendicular,
+        the second vector is rotated in the plane to become perpendicular to the first. Providing a value of
+        ((1., 0., 0.), (0., 1., 0.)) is equivalent to providing 'xy'.
+    origin : three float, optional
+        The origin relative to the provided atoms mapped to the origin of the potential. This is equivalent to
+        translating the atoms. The default is (0., 0., 0.).
+    box : three float, optional
+        The extent of the potential in `x`, `y` and `z`. If not given this is determined from the atoms' cell.
+        If the box size does not match an integer number of the atoms' supercell, an affine transformation may be
+        necessary to preserve periodicity, determined by the `periodic` keyword.
+    periodic : bool, True
+        If a transformation of the atomic structure is required, `periodic` determines how the atomic structure is
+        transformed. If True, the periodicity of the Atoms is preserved, which may require applying a small affine
+        transformation to the atoms. If False, the transformed potential is effectively cut out of a larger repeated
+        potential, which may not preserve periodicity.
+    integrator : ProjectionIntegrator, optional
+        Provide a custom integrator for the projection integrals of the potential slicing.
+    device : str, optional
+        The device used for calculating the potential, 'cpu' or 'gpu'. The default is determined by the user
+        configuration file.
     """
-    _base_dims = 3
+
+    _exclude_from_copy = ("parametrization", "projection")
+
+    def __init__(
+        self,
+        atoms: Atoms | BaseFrozenPhonons = None,
+        gpts: int | tuple[int, int] = None,
+        sampling: float | tuple[float, float] = None,
+        slice_thickness: float | tuple[float, ...] = 1,
+        parametrization: str | Parametrization = "lobato",
+        projection: str = "infinite",
+        exit_planes: int | tuple[int, ...] = None,
+        plane: (
+            str | tuple[tuple[float, float, float], tuple[float, float, float]]
+        ) = "xy",
+        origin: tuple[float, float, float] = (0.0, 0.0, 0.0),
+        box: tuple[float, float, float] = None,
+        periodic: bool = True,
+        integrator: FieldIntegrator = None,
+        device: str = None,
+    ):
+        if integrator is None:
+            if projection == "finite":
+                integrator = QuadratureProjectionIntegrals(
+                    parametrization=parametrization
+                )
+            elif projection == "infinite":
+                integrator = ScatteringFactorProjectionIntegrals(
+                    parametrization=parametrization
+                )
+            else:
+                raise NotImplementedError
+
+        super().__init__(
+            atoms=atoms,
+            array_object=PotentialArray,
+            gpts=gpts,
+            sampling=sampling,
+            slice_thickness=slice_thickness,
+            exit_planes=exit_planes,
+            device=device,
+            plane=plane,
+            origin=origin,
+            box=box,
+            periodic=periodic,
+            integrator=integrator,
+        )
+
+
+class FieldArray(BaseField, ArrayObject):
     def __init__(
         self,
         array: np.ndarray | da.core.Array,
         slice_thickness: float | tuple[float, ...] = None,
         extent: float | tuple[float, float] = None,
         sampling: float | tuple[float, float] = None,
         exit_planes: int | tuple[int, ...] = None,
         ensemble_axes_metadata: list[AxisMetadata] = None,
         metadata: dict = None,
     ):
         self._slice_thickness = _validate_slice_thickness(
-            slice_thickness, num_slices=array.shape[-3]
+            slice_thickness, num_slices=array.shape[-self._base_dims]
         )
+
         self._exit_planes = _validate_exit_planes(
             exit_planes, len(self._slice_thickness)
         )
         self._grid = Grid(extent=extent, gpts=array.shape[-2:], sampling=sampling)
 
         super().__init__(
             array=array,
             ensemble_axes_metadata=ensemble_axes_metadata,
             metadata=metadata,
         )
 
     @property
-    def num_frozen_phonons(self):
+    def num_configurations(self):
         indices = _find_axes_type(self, FrozenPhononsAxis)
         if indices:
             return reduce(mul, tuple(self.array.shape[i] for i in indices))
         else:
             return 1
 
     @property
     def slice_thickness(self) -> tuple[float, ...]:
         return self._slice_thickness
 
     @property
     def exit_planes(self) -> tuple[int, ...]:
         return self._exit_planes
 
-    def __getitem__(self, items):
-        if isinstance(items, (Number, slice)):
-            items = (items,)
-
-        ensemble_items = items[: len(self.ensemble_shape)]
-        slic_items = items[len(self.ensemble_shape) :]
-
-        if len(ensemble_items):
-            potential_array = super().__getitem__(ensemble_items)
-        else:
-            potential_array = self
-
-        if len(slic_items) == 0:
-            return potential_array
-
-        padded_items = (slice(None),) * len(potential_array.ensemble_shape) + slic_items
-
-        array = potential_array._array[padded_items]
-        slice_thickness = np.array(potential_array.slice_thickness)[slic_items]
-
-        if len(array.shape) < len(potential_array.shape):
-            array = array[
-                (slice(None),) * len(potential_array.ensemble_shape) + (None,)
-            ]
-            slice_thickness = slice_thickness[None]
-
-        kwargs = potential_array._copy_kwargs(exclude=("array", "slice_thickness"))
-        kwargs["array"] = array
-        kwargs["slice_thickness"] = slice_thickness
-        kwargs["sampling"] = None
-        return potential_array.__class__(**kwargs)
-
     def build(
         self,
         first_slice: int = 0,
         last_slice: int = None,
         chunks: int = 1,
         lazy: bool = None,
     ):
         raise RuntimeError("potential is already built")
 
-    def generate_slices(self, first_slice=0, last_slice=None):
+    def generate_slices(self, first_slice: int = 0, last_slice: int = None):
         """
         Generate the slices for the potential.
 
         Parameters
         ----------
         first_slice : int, optional
             Index of the first slice of the generated potential.
@@ -965,58 +953,53 @@
             slic._exit_planes = exit_planes
 
             start += 1
             stop += 1
 
             yield slic
 
-    def transmission_function(self, energy: float) -> "TransmissionFunction":
-        """
-        Calculate the transmission functions for each slice for a specific energy.
+    def __getitem__(self, items):
+        if isinstance(items, (Number, slice)):
+            items = (items,)
 
-        Parameters
-        ----------
-        energy: float
-            Electron energy [eV].
+        ensemble_items = items[: len(self.ensemble_shape)]
+        slic_items = items[len(self.ensemble_shape) :]
 
-        Returns
-        -------
-        transmissionfunction : TransmissionFunction
-            Transmission functions for each slice.
-        """
-        xp = get_array_module(self.array)
+        if len(ensemble_items):
+            potential_array = super().__getitem__(ensemble_items)
+        else:
+            potential_array = self
 
-        def _transmission_function(array, energy):
-            array = complex_exponential(xp.float32(energy2sigma(energy)) * array)
-            return array
+        if len(slic_items) == 0:
+            return potential_array
 
-        if self.is_lazy:
-            array = self._array.map_blocks(
-                _transmission_function,
-                energy=energy,
-                meta=xp.array((), dtype=xp.complex64),
-            )
-        else:
-            array = _transmission_function(self._array, energy=energy)
+        padded_items = (slice(None),) * len(potential_array.ensemble_shape) + slic_items
 
-        t = TransmissionFunction(
-            array,
-            slice_thickness=self.slice_thickness,
-            extent=self.extent,
-            energy=energy,
-        )
-        return t
+        array = potential_array._array[padded_items]
+        slice_thickness = np.array(potential_array.slice_thickness)[slic_items]
+
+        if len(array.shape) < len(potential_array.shape):
+            array = array[
+                (slice(None),) * len(potential_array.ensemble_shape) + (None,)
+            ]
+            slice_thickness = slice_thickness[None]
+
+        kwargs = potential_array._copy_kwargs(exclude=("array", "slice_thickness"))
+        kwargs["array"] = array
+        kwargs["slice_thickness"] = slice_thickness
+        kwargs["sampling"] = None
+        return potential_array.__class__(**kwargs)
 
     def tile(self, repetitions: tuple[int, int] | tuple[int, int, int]):
         """
         Tile the potential.
 
         Parameters
         ----------
-        multiples: two or three int
+        repetitions: two or three int
             The number of repetitions of the potential along each axis. NOTE: if three integers are given, the first
             represents the number of repetitions along the `z`-axis.
 
         Returns
         -------
         PotentialArray object
             The tiled potential.
@@ -1037,35 +1020,14 @@
             extent=new_extent,
             ensemble_axes_metadata=self.ensemble_axes_metadata,
         )
 
     def to_hyperspy(self):
         return self.to_images().to_hyperspy()
 
-    def transmit(self, waves: "Waves", conjugate: bool = False) -> "Waves":
-        """
-        Transmit a wave function through a potential slice.
-
-        Parameters
-        ----------
-        waves: Waves
-            Waves object to transmit.
-        conjugate : bool, optional
-            If True, use the conjugate of the transmission function. Default is False.
-
-        Returns
-        -------
-        transmission_function : TransmissionFunction
-            Transmission function for the wave function through the potential slice.
-        """
-
-        transmission_function = self.transmission_function(waves.energy)
-
-        return transmission_function.transmit(waves, conjugate=conjugate)
-
     def to_images(self):
         """Convert slices of the potential to a stack of images."""
         metadata = {"label": "potential", "units": "eV / e"}
 
         return Images(
             array=self._array,
             sampling=(self.sampling[0], self.sampling[1]),
@@ -1079,24 +1041,140 @@
 
         Returns
         -------
         images : Images
             One or more images of the projected potential(s).
         """
         metadata = {"label": "potential", "units": "eV / e"}
-        array = self.array.sum(-3)
-        array -= array.min((-2, -1), keepdims=True)
+        array = self.array.sum(-self._base_dims)
+        # array -= array.min((-2, -1), keepdims=True)
+
+        ensemble_axes_metadata = (
+            self.ensemble_axes_metadata + self.base_axes_metadata[1:-2]
+        )
 
         return Images(
             array=array,
             sampling=self.sampling,
-            ensemble_axes_metadata=self.ensemble_axes_metadata,
+            ensemble_axes_metadata=ensemble_axes_metadata,
+            metadata=metadata,
+        )
+
+
+class PotentialArray(BasePotential, FieldArray):
+    """
+    The potential array represents slices of the electrostatic potential as an array. All other potentials build
+    potential arrays.
+
+    Parameters
+    ----------
+    array: 3D np.ndarray
+        The array representing the potential slices. The first dimension is the slice index and the last two are the
+        spatial dimensions.
+    slice_thickness: float
+        The thicknesses of potential slices [Å]. If a float, the thickness is the same for all slices.
+        If a sequence, the length must equal the length of the potential array.
+    extent: one or two float, optional
+        Lateral extent of the potential [Å].
+    sampling: one or two float, optional
+        Lateral sampling of the potential [1 / Å].
+    exit_planes : int or tuple of int, optional
+        The `exit_planes` argument can be used to calculate thickness series.
+        Providing `exit_planes` as a tuple of int indicates that the tuple contains the slice indices after which an
+        exit plane is desired, and hence during a multislice simulation a measurement is created. If `exit_planes` is
+        an integer a measurement will be collected every `exit_planes` number of slices.
+    ensemble_axes_metadata : list of AxesMetadata
+        Axis metadata for each ensemble axis. The axis metadata must be compatible with the shape of the array.
+    metadata : dict
+        A dictionary defining wave function metadata. All items will be added to the metadata of measurements derived
+        from the waves.
+    """
+
+    _base_dims = 3
+
+    def __init__(
+        self,
+        array: np.ndarray | da.core.Array,
+        slice_thickness: float | tuple[float, ...] = None,
+        extent: float | tuple[float, float] = None,
+        sampling: float | tuple[float, float] = None,
+        exit_planes: int | tuple[int, ...] = None,
+        ensemble_axes_metadata: list[AxisMetadata] = None,
+        metadata: dict = None,
+    ):
+        super().__init__(
+            array=array,
+            slice_thickness=slice_thickness,
+            extent=extent,
+            sampling=sampling,
+            exit_planes=exit_planes,
+            ensemble_axes_metadata=ensemble_axes_metadata,
             metadata=metadata,
         )
 
+    def transmission_function(self, energy: float) -> TransmissionFunction:
+        """
+        Calculate the transmission functions for each slice for a specific energy.
+
+        Parameters
+        ----------
+        energy: float
+            Electron energy [eV].
+
+        Returns
+        -------
+        transmissionfunction : TransmissionFunction
+            Transmission functions for each slice.
+        """
+        xp = get_array_module(self.array)
+
+        def _transmission_function(array, energy):
+            dtype = get_dtype(complex=False)
+            sigma = dtype(energy2sigma(energy))
+            array = complex_exponential(sigma * array)
+            return array
+
+        if self.is_lazy:
+            array = self._array.map_blocks(
+                _transmission_function,
+                energy=energy,
+                meta=xp.array((), dtype=get_dtype(complex=True)),
+            )
+        else:
+            array = _transmission_function(self._array, energy=energy)
+
+        t = TransmissionFunction(
+            array,
+            slice_thickness=self.slice_thickness,
+            extent=self.extent,
+            energy=energy,
+        )
+        return t
+
+    def transmit(self, waves: Waves, conjugate: bool = False) -> Waves:
+        """
+        Transmit a wave function through a potential slice.
+
+        Parameters
+        ----------
+        waves: Waves
+            Waves object to transmit.
+        conjugate : bool, optional
+            If True, use the conjugate of the transmission function. Default is False.
+
+        Returns
+        -------
+        transmission_function : TransmissionFunction
+            Transmission function for the wave function through the potential slice.
+        """
+
+        transmission_function = self.transmission_function(waves.energy)
+
+        return transmission_function.transmit(waves, conjugate=conjugate)
+
 
 class TransmissionFunction(PotentialArray, HasAcceleratorMixin):
     """Class to describe transmission functions.
 
     Parameters
     ----------
     array : 3D np.ndarray
@@ -1117,30 +1195,29 @@
         self,
         array: np.ndarray,
         slice_thickness: float | Sequence[float],
         extent: float | tuple[float, float] = None,
         sampling: float | tuple[float, float] = None,
         energy: float = None,
     ):
-
         self._accelerator = Accelerator(energy=energy)
         super().__init__(array, slice_thickness, extent, sampling)
 
-    def get_chunk(self, first_slice, last_slice) -> "TransmissionFunction":
+    def get_chunk(self, first_slice, last_slice) -> TransmissionFunction:
         array = self.array[first_slice:last_slice]
         if len(array.shape) == 2:
             array = array[None]
         return self.__class__(
             array,
             self.slice_thickness[first_slice:last_slice],
             extent=self.extent,
             energy=self.energy,
         )
 
-    def transmission_function(self, energy) -> "TransmissionFunction":
+    def transmission_function(self, energy) -> TransmissionFunction:
         """
         Calculate the transmission functions for each slice for a specific energy.
 
         Parameters
         ----------
         energy: float
             Electron energy [eV].
@@ -1213,27 +1290,26 @@
         self,
         potential_unit: BasePotential,
         repetitions: tuple[int, int, int],
         num_frozen_phonons: int = None,
         exit_planes: int = None,
         seeds: int | tuple[int, ...] = None,
     ):
-
         if num_frozen_phonons is None and seeds is None:
             self._seeds = None
         else:
             if num_frozen_phonons is None and seeds:
                 num_frozen_phonons = len(seeds)
             elif num_frozen_phonons is None and seeds is None:
                 num_frozen_phonons = 1
 
             self._seeds = _validate_seeds(seeds, num_frozen_phonons)
 
         if (
-            (potential_unit.num_frozen_phonons == 1)
+            (potential_unit.num_configurations == 1)
             and (num_frozen_phonons is not None)
             and (num_frozen_phonons > 1)
         ):
             warnings.warn(
                 "'num_frozen_phonons' is greater than one, but the potential unit does not have frozen phonons"
             )
 
@@ -1250,14 +1326,15 @@
             potential_unit.extent[0] * repetitions[0],
             potential_unit.extent[1] * repetitions[1],
         )
 
         box = extent + (potential_unit.thickness * repetitions[2],)
         slice_thickness = potential_unit.slice_thickness * repetitions[2]
         super().__init__(
+            array_object=PotentialArray,
             gpts=gpts,
             cell=Cell(np.diag(box)),
             slice_thickness=slice_thickness,
             exit_planes=exit_planes,
             device=potential_unit.device,
             plane="xy",
             origin=(0.0, 0.0, 0.0),
@@ -1269,18 +1346,18 @@
         self._repetitions = repetitions
 
     @property
     def ensemble_shape(self) -> tuple[int, ...]:
         if self._seeds is None:
             return ()
         else:
-            return (self.num_frozen_phonons,)
+            return (self.num_configurations,)
 
     @property
-    def num_frozen_phonons(self):
+    def num_configurations(self):
         if self._seeds is None:
             return 1
         else:
             return len(self._seeds)
 
     @property
     def seeds(self):
@@ -1333,50 +1410,53 @@
             potential = potential.item()
 
         if seed is not None:
             num_frozen_phonons = len(seed)
         else:
             num_frozen_phonons = None
 
-        new = cls(potential_unit=potential, seeds=seed, num_frozen_phonons=num_frozen_phonons, **kwargs)
+        new = cls(
+            potential_unit=potential,
+            seeds=seed,
+            num_frozen_phonons=num_frozen_phonons,
+            **kwargs,
+        )
         return _wrap_with_array(new)
 
     def _from_partitioned_args(self):
-        kwargs = self._copy_kwargs(exclude=("potential_unit", "seeds", "num_frozen_phonons"))
+        kwargs = self._copy_kwargs(
+            exclude=("potential_unit", "seeds", "num_frozen_phonons")
+        )
         output = partial(self._from_partitioned_args_func, **kwargs)
         return output
 
     def _partition_args(self, chunks: int = 1, lazy: bool = True):
-
         chunks = validate_chunks(self.ensemble_shape, chunks)
 
         if chunks == ():
             chunks = ((1,),)
 
         if lazy:
             arrays = []
 
             for i, (start, stop) in enumerate(chunk_ranges(chunks)[0]):
-
                 if self.seeds is not None:
                     seeds = self.seeds[start:stop]
                 else:
                     seeds = None
 
                 lazy_atoms = dask.delayed(self.potential_unit)
                 lazy_args = dask.delayed(_wrap_with_array)((lazy_atoms, seeds), ndims=1)
                 lazy_array = da.from_delayed(lazy_args, shape=(1,), dtype=object)
                 arrays.append(lazy_array)
 
             array = da.concatenate(arrays)
         else:
-
-
             potential_unit = self.potential_unit
-            #if self.potential_unit.array:
+            # if self.potential_unit.array:
             #    atoms = atoms.compute()
             array = np.zeros((len(chunks[0]),), dtype=object)
             for i, (start, stop) in enumerate(chunk_ranges(chunks)[0]):
                 if self.seeds is not None:
                     seeds = self.seeds[start:stop]
                 else:
                     seeds = None
@@ -1468,7 +1548,10 @@
                 start += 1
                 stop += 1
 
                 if return_depth:
                     yield cum_thickness[stop - 1], slic
                 else:
                     yield slic
+                
+                if i == last_slice:
+                    break
```

### Comparing `abtem-1.0.4/abtem/prism/_natural_neighbors.py` & `abtem-1.0.5/abtem/prism/_natural_neighbors.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/prism/_partitioned_s_matrix.py` & `abtem-1.0.5/abtem/prism/_partitioned_s_matrix.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/prism/s_matrix.py` & `abtem-1.0.5/abtem/prism/s_matrix.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/prism/utils.py` & `abtem-1.0.5/abtem/prism/utils.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/reconstruct.py` & `abtem-1.0.5/abtem/reconstruct.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/abtem/scan.py` & `abtem-1.0.5/abtem/scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for describing different types of scans."""
+
 from __future__ import annotations
 
 import itertools
 from abc import abstractmethod
 from typing import TYPE_CHECKING
 
 import dask.array as da
@@ -14,14 +15,15 @@
 from abtem.array import ArrayObject, T
 from abtem.core.axes import ScanAxis, PositionsAxis, AxisMetadata
 from abtem.core.backend import get_array_module, validate_device
 from abtem.core.chunks import validate_chunks
 from abtem.core.ensemble import _wrap_with_array, unpack_blockwise_args
 from abtem.core.fft import fft_shift_kernel
 from abtem.core.grid import Grid, HasGridMixin
+from abtem.measurements import _scan_axes
 from abtem.potentials.iam import BasePotential, _validate_potential
 from abtem.transfer import nyquist_sampling
 from abtem.transform import ReciprocalSpaceMultiplication
 
 if TYPE_CHECKING:
     from abtem.waves import Waves, Probe
     from abtem.prism.s_matrix import BaseSMatrix
@@ -204,15 +206,14 @@
     ----------
     positions : np.ndarray, optional
         Scan positions [Å]. Anything that can be converted to an ndarray of shape (n, 3) is accepted. Default is
         (0., 0.).
     """
 
     def __init__(self, positions: np.ndarray = (0.0, 0.0), squeeze: bool = False):
-
         positions = np.array(positions, dtype=np.float32)
 
         if len(positions.shape) == 1:
             positions = positions[None]
 
         self._positions = positions
         self._squeeze = squeeze
@@ -355,15 +356,14 @@
 
 def _validate_coordinates(
     start: tuple[float, float] | Atom,
     end: tuple[float, float] | Atom,
     potential: BasePotential | Atoms,
     fractional: bool,
 ) -> tuple[tuple[float, float], tuple[float, float]]:
-
     if fractional:
         potential = _validate_potential(potential)
 
     start = _validate_coordinate(start, potential, fractional)
     end = _validate_coordinate(end, potential, fractional)
 
     if start is not None and end is not None:
@@ -403,15 +403,14 @@
         end: tuple[float, float] | Atom = None,
         gpts: int = None,
         sampling: float = None,
         endpoint: bool = True,
         fractional: bool = False,
         potential: BasePotential | Atoms = None,
     ):
-
         self._gpts = gpts
         self._sampling = sampling
 
         self._start, self._end = _validate_coordinates(
             start, end, potential, fractional
         )
 
@@ -527,15 +526,14 @@
             return
 
         self._gpts = int(np.ceil(self.extent / self.sampling))
 
         self._adjust_sampling()
 
     def _adjust_sampling(self):
-
         if self.extent is None or self.gpts is None:
             return
 
         if self.endpoint and self.gpts > 1:
             self._sampling = self.extent / (self.gpts - 1)
         else:
             self._sampling = self.extent / self.gpts
@@ -626,15 +624,21 @@
         self, array_object: ArrayObject, index: int = 0
     ) -> tuple[int, ...]:
         return self.ensemble_shape + array_object.ensemble_shape
 
     def _out_ensemble_axes_metadata(
         self, array_object: ArrayObject | T, index: int = 0
     ) -> list[AxisMetadata] | tuple[list[AxisMetadata], ...]:
-        return [*self.ensemble_axes_metadata, *array_object.ensemble_axes_metadata]
+        ensemble_axes_metadata = self.ensemble_axes_metadata
+
+        if len(_scan_axes(array_object)) > 0:
+            for axis in ensemble_axes_metadata:
+                axis._main = False
+
+        return [*ensemble_axes_metadata, *array_object.ensemble_axes_metadata]
 
     @property
     def _default_ensemble_chunks(self):
         return ("auto",)
 
     def _sort_into_extents(self, extents):
         raise NotImplementedError
@@ -753,15 +757,14 @@
         end: tuple[float, float] | Atom = None,
         gpts: int | tuple[int, int] = None,
         sampling: float | tuple[float, float] = None,
         endpoint: bool | tuple[bool, bool] = False,
         fractional: bool = False,
         potential: BasePotential | Atoms = None,
     ):
-
         super().__init__()
 
         start, end = _validate_coordinates(start, end, potential, fractional)
 
         if start is not None:
             if np.isscalar(start):
                 start = (start,) * 2
@@ -877,15 +880,14 @@
 
         if len(xi) == 1:
             return xi[0]
 
         return np.stack(np.meshgrid(*xi, indexing="ij"), axis=-1)
 
     def _sort_into_extents(self, extents):
-
         x = np.linspace(
             self.start[0], self.end[0], self.gpts[0], endpoint=self.endpoint[0]
         )
 
         separators = [l for _, l in extents[0]]
 
         unique, x_chunks = np.unique(np.digitize(x, separators), return_counts=True)
@@ -930,14 +932,25 @@
                     offset=offset,
                     units="Å",
                     endpoint=endpoint,
                 )
             )
         return axes_metadata
 
+    def _out_ensemble_axes_metadata(
+        self, array_object: ArrayObject | T, index: int = 0
+    ) -> list[AxisMetadata] | tuple[list[AxisMetadata], ...]:
+        ensemble_axes_metadata = self.ensemble_axes_metadata
+
+        if len(_scan_axes(array_object)) > 0:
+            for axis in ensemble_axes_metadata:
+                axis._main = False
+
+        return [*ensemble_axes_metadata, *array_object.ensemble_axes_metadata]
+
     @classmethod
     def _from_partitioned_args_func(cls, *args, **kwargs):
         x_scan, y_scan = unpack_blockwise_args(args)
         start = (x_scan["start"], y_scan["start"])
         end = (x_scan["end"], y_scan["end"])
         gpts = (x_scan["gpts"], y_scan["gpts"])
         endpoint = (x_scan["endpoint"], y_scan["endpoint"])
```

### Comparing `abtem-1.0.4/abtem/slicing.py` & `abtem-1.0.5/abtem/slicing.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     slice_thickness : float or sequence of float, optional
         Thickness of the potential slices in the propagation direction in [Å] (default is 0.5 Å).
         If given as a float, the number of slices is calculated by dividing the slice thickness into the `z`-height of
         supercell. The slice thickness may be given as a sequence of values for each slice, in which case an error will
         be thrown if the sum of slice thicknesses is not equal to the height of the atoms.
     """
 
-    def __init__(self, atoms: Atoms, slice_thickness: float | np.ndarray | str):
+    def __init__(self, atoms: Atoms, slice_thickness: float | Sequence[float] | str):
         if not is_cell_orthogonal(atoms):
             raise RuntimeError("atoms must have an orthogonal cell")
 
         self._atoms = atoms
 
         if isinstance(slice_thickness, str):
             raise NotImplementedError
@@ -191,14 +191,28 @@
         for i in range(first_slice, last_slice):
             yield self.get_atoms_in_slices(i, atomic_number=atomic_number)
 
     def __getitem__(self, item: int | slice) -> Atoms:
         return self.get_atoms_in_slices(*_unpack_item(item, len(self)))
 
 
+def find_closest_indices(list1, list2):
+    # Convert lists to NumPy arrays
+    arr1 = np.array(list1)[:, np.newaxis]  # Convert to column vector
+    arr2 = np.array(list2)
+
+    # Calculate the absolute differences using broadcasting
+    differences = np.abs(arr1 - arr2)
+
+    # Find the indices of the minimum differences
+    closest_indices = np.argmin(differences, axis=1)
+
+    return closest_indices
+
+
 class SliceIndexedAtoms(BaseSlicedAtoms):
     """
     Sliced atoms assigning each atom to a specific slice index.
 
     Parameters
     ----------
     atoms: Atoms
@@ -206,20 +220,33 @@
     slice_thickness : float or sequence of float, optional
         Thickness of the potential slices in the propagation direction in [Å] (default is 0.5 Å).
         If given as a float, the number of slices is calculated by dividing the slice thickness into the `z`-height of
         supercell. The slice thickness may be given as a sequence of values for each slice, in which case an error will
         be thrown if the sum of slice thicknesses is not equal to the height of the atoms.
     """
 
-    def __init__(self, atoms: Atoms, slice_thickness: float | tuple[float, ...]):
+    def __init__(
+        self, atoms: Atoms, slice_thickness: float | Sequence[float], method="closest"
+    ):
         super().__init__(atoms, slice_thickness)
 
-        labels = np.digitize(
-            self.atoms.positions[:, 2], np.cumsum(self.slice_thickness)
+        # labels = np.digitize(
+        #     self.atoms.positions[:, 2], np.cumsum(self.slice_thickness)
+        # )
+        #
+        #
+
+        # print(self.slice_thickness)
+
+        labels = find_closest_indices(
+            atoms.positions[:, 2], np.cumsum((0,) + self.slice_thickness[:-1])
         )
+        # print(np.cumsum(self.slice_thickness))
+        # sss
+
         self._slice_index = [
             indices for indices in label_to_index(labels, max_label=len(self) - 1)
         ]
 
     def get_atoms_in_slices(
         self, first_slice: int, last_slice: int = None, atomic_number: int = None
     ) -> Atoms:
```

### Comparing `abtem-1.0.4/abtem/tilt.py` & `abtem-1.0.5/abtem/tilt.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from abtem.core.backend import get_array_module
 from abtem.transform import CompositeArrayObjectTransform, ArrayObjectTransform
 from abtem.distributions import (
     BaseDistribution,
     MultidimensionalDistribution,
     EnsembleFromDistributions,
     from_values,
-    _validate_distribution,
+    validate_distribution,
 )
 
 if TYPE_CHECKING:
     from abtem.waves import Waves
 
 
 def _validate_tilt(
@@ -183,15 +183,15 @@
     direction : str
         Cartesian axis, should be either 'x' or 'y'.
     """
 
     def __init__(self, tilt: float | BaseDistribution = 0.0, direction: str = "x"):
 
         if isinstance(tilt, (np.ndarray, list, tuple)):
-            tilt = _validate_distribution(tilt)
+            tilt = validate_distribution(tilt)
 
         if not isinstance(tilt, BaseDistribution):
             tilt = float(tilt)
 
         self._tilt = tilt
         self._direction = direction
         super().__init__(distributions=("tilt",))
```

### Comparing `abtem-1.0.4/abtem/transfer.py` & `abtem-1.0.5/abtem/transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 """Module to describe the contrast transfer function (CTF) and the related apertures."""
+
 from __future__ import annotations
 
 import copy
 import re
 from abc import abstractmethod
 from collections import defaultdict
 from functools import reduce
 from typing import TYPE_CHECKING
 
 import numpy as np
 
-from abtem.core.axes import AxisMetadata, ParameterAxis
-from abtem.core.axes import OrdinalAxis
-from abtem.core.backend import cp
-from abtem.core.backend import get_array_module
+from abtem.core.axes import AxisMetadata, OrdinalAxis, ParameterAxis
+from abtem.core.backend import cp, get_array_module
 from abtem.core.complex import complex_exponential
 from abtem.core.energy import (
     Accelerator,
-    energy2wavelength,
     HasAcceleratorMixin,
+    energy2wavelength,
     reciprocal_space_sampling_to_angular_sampling,
 )
 from abtem.core.fft import fft_crop
-from abtem.core.grid import HasGridMixin, polar_spatial_frequencies, Grid
-from abtem.core.utils import expand_dims_to_broadcast
+from abtem.core.grid import Grid, HasGridMixin, polar_spatial_frequencies
+from abtem.core.utils import expand_dims_to_broadcast, get_dtype
 from abtem.distributions import (
     BaseDistribution,
     _unpack_distributions,
-    _validate_distribution,
+    validate_distribution,
 )
 from abtem.measurements import ReciprocalSpaceLineProfiles
 from abtem.transform import ReciprocalSpaceMultiplication
 
 if TYPE_CHECKING:
     from abtem.waves import BaseWaves
 
@@ -43,15 +42,15 @@
 
     def __init__(
         self,
         energy: float = None,
         extent: float | tuple[float, float] = None,
         gpts: int | tuple[int, int] = None,
         sampling: float | tuple[float, float] = None,
-        distributions: tuple[str] = (),
+        distributions: tuple[str, ...] = (),
     ):
         self._accelerator = Accelerator(energy=energy)
         self._grid = Grid(extent=extent, gpts=gpts, sampling=sampling)
         super().__init__(distributions=distributions)
 
     @abstractmethod
     def _evaluate_from_angular_grid(self, alpha, phi):
@@ -99,15 +98,33 @@
         return self._evaluate_from_angular_grid(alpha, phi)
 
     def to_diffraction_patterns(
         self,
         max_angle: float = None,
         gpts: int | tuple[int, int] = None,
     ):
-        """ """
+        """Converts the transfer function instance to DiffractionPatterns.
+
+        Parameters
+        ----------
+        max_angle : float, optional
+            The maximum diffraction angle in radians. If not provided, the maximum angle
+            will be determined based on the `self._max_semiangle_cutoff` attribute of the instance.
+            If neither `max_angle` nor `self._max_semiangle_cutoff` is available, a `RuntimeError`
+            will be raised.
+        gpts : int | tuple[int, int], optional
+            The number of grid points in reciprocal space for performing Fourier Transform.
+            If not provided, a default value of 128 will be used.
+
+        Returns
+        -------
+        abtem.measurements.DiffractionPatterns
+            The diffraction patterns obtained from the conversion.
+
+        """
         from abtem.measurements import DiffractionPatterns
 
         if (self.sampling is None) or (max_angle is not None):
             if max_angle is None and hasattr(self, "_max_semiangle_cutoff"):
                 max_angle = self._max_semiangle_cutoff
 
             elif max_angle is None:
@@ -145,15 +162,15 @@
     def __init__(
         self,
         semiangle_cutoff: float | BaseDistribution = None,
         energy: float = None,
         extent: float | tuple[float, float] = None,
         gpts: int | tuple[int, int] = None,
         sampling: float | tuple[float, float] = None,
-        distributions: tuple[str] = (),
+        distributions: tuple[str, ...] = (),
     ):
         self._semiangle_cutoff = semiangle_cutoff
         super().__init__(
             energy=energy,
             extent=extent,
             gpts=gpts,
             sampling=sampling,
@@ -185,15 +202,15 @@
 
     @property
     def semiangle_cutoff(self):
         """Semiangle cutoff of the aperture [mrad]."""
         return self._semiangle_cutoff
 
     @semiangle_cutoff.setter
-    def semiangle_cutoff(self, semiangle_cutoff:float | BaseDistribution):
+    def semiangle_cutoff(self, semiangle_cutoff: float | BaseDistribution):
         self._semiangle_cutoff = semiangle_cutoff
 
     def _cropped_aperture(self):
         if self._max_semiangle_cutoff == np.inf:
             return self
 
         gpts = (
@@ -235,24 +252,24 @@
 
     Returns
     -------
     soft_aperture_array : 2D or 3D np.ndarray
     """
     xp = get_array_module(alpha)
 
-    semiangle_cutoff = xp.array(semiangle_cutoff, dtype=xp.float32)
+    semiangle_cutoff = xp.array(semiangle_cutoff, dtype=get_dtype(complex=False))
 
     base_ndims = len(alpha.shape)
 
     semiangle_cutoff, alpha = expand_dims_to_broadcast(semiangle_cutoff, alpha)
     semiangle_cutoff, phi = expand_dims_to_broadcast(
         semiangle_cutoff, phi, match_dims=[(-2, -1), (-2, -1)]
     )
 
-    angular_sampling = xp.array(angular_sampling, dtype=xp.float32) * 1e-3
+    angular_sampling = xp.array(angular_sampling, dtype=get_dtype(complex=False)) * 1e-3
 
     denominator = xp.sqrt(
         (xp.cos(phi) * angular_sampling[0]) ** 2
         + (xp.sin(phi) * angular_sampling[1]) ** 2
     )
 
     ndims = len(alpha.shape)
@@ -282,15 +299,15 @@
         represents a different aperture for each item in the array of semiangle cutoffs.
 
     Returns
     -------
     hard_aperture_array : 2D or 3D np.ndarray
     """
     xp = get_array_module(alpha)
-    return xp.array(alpha <= semiangle_cutoff).astype(xp.float32)
+    return xp.array(alpha <= semiangle_cutoff).astype(get_dtype(complex=False))
 
 
 class Aperture(BaseAperture):
     """
     A circular aperture cutting off the wave function at a specified angle, employed in both STEM and HRTEM.
     The abrupt cutoff may be softened by tapering it.
 
@@ -315,15 +332,15 @@
         semiangle_cutoff: float | BaseDistribution,
         soft: bool = True,
         energy: float = None,
         extent: float | tuple[float, float] = None,
         gpts: int | tuple[int, int] = None,
         sampling: float | tuple[float, float] = None,
     ):
-        semiangle_cutoff = _validate_distribution(semiangle_cutoff)
+        semiangle_cutoff = validate_distribution(semiangle_cutoff)
         self._soft = soft
 
         super().__init__(
             distributions=("semiangle_cutoff",),
             energy=energy,
             semiangle_cutoff=semiangle_cutoff,
             extent=extent,
@@ -333,30 +350,31 @@
 
     @property
     def ensemble_axes_metadata(self) -> list[AxisMetadata]:
         ensemble_axes_metadata = []
         if isinstance(self.semiangle_cutoff, BaseDistribution):
             ensemble_axes_metadata += [
                 ParameterAxis(
-                    label="semiangle cutoff",
+                    label="semiangle_cutoff",
                     values=self.semiangle_cutoff,
                     units="mrad",
+                    tex_label="$\\alpha_{cut}$",
                     _ensemble_mean=self.semiangle_cutoff.ensemble_mean,
                 )
             ]
         return ensemble_axes_metadata
 
     @property
     def soft(self) -> bool:
         """True if the aperture has a soft edge."""
         return self._soft
 
     def _evaluate_from_angular_grid(
         self, alpha: np.ndarray, phi: np.ndarray
-    ) -> np.ndarray:
+    ) -> np.ndarray | float:
         xp = get_array_module(alpha)
 
         if self.semiangle_cutoff == xp.inf:
             return xp.ones_like(alpha)
 
         semiangle_cutoff = xp.array(self.semiangle_cutoff) * 1e-3
 
@@ -589,18 +607,18 @@
         xp = get_array_module(alpha)
         alpha = xp.array(alpha)
 
         semiangle_cutoff = self.semiangle_cutoff / 1e3
         center_hole_cutoff = self.center_hole_cutoff / 1e3
         phase_shift = self.phase_shift
 
-        amplitude = xp.asarray(alpha < semiangle_cutoff, dtype=np.float32)
+        amplitude = xp.asarray(alpha < semiangle_cutoff, dtype=get_dtype(complex=False))
         phase_array = xp.asarray(
             xp.logical_and(alpha > center_hole_cutoff, alpha < semiangle_cutoff),
-            dtype=np.float32,
+            dtype=get_dtype(complex=False),
         )
         phase = xp.exp(1.0j * phase_shift * phase_array)
         array = amplitude * phase
 
         return array
 
 
@@ -628,15 +646,15 @@
         focal_spread: float | BaseDistribution,
         energy: float = None,
         extent: float | tuple[float, float] = None,
         gpts: int | tuple[int, int] = None,
         sampling: float | tuple[float, float] = None,
     ):
         self._accelerator = Accelerator(energy=energy)
-        self._focal_spread = _validate_distribution(focal_spread)
+        self._focal_spread = validate_distribution(focal_spread)
         super().__init__(
             distributions=("focal_spread",),
             energy=energy,
             extent=extent,
             gpts=gpts,
             sampling=sampling,
         )
@@ -644,15 +662,15 @@
     @property
     def focal_spread(self):
         """The standard deviation of the focal spread [Å]."""
         return self._focal_spread
 
     @focal_spread.setter
     def focal_spread(self, value):
-        self._focal_spread = _validate_distribution(value)
+        self._focal_spread = validate_distribution(value)
 
     @property
     def ensemble_axes_metadata(self) -> list[AxisMetadata]:
         return self._get_axes_metadata_from_distributions(
             focal_spread={"units": "mrad"}
         )
 
@@ -665,28 +683,28 @@
         (focal_spread,) = unpacked
 
         alpha = xp.array(alpha)
         alpha = xp.expand_dims(alpha, axis=tuple(range(0, self._num_ensemble_axes)))
 
         array = xp.exp(
             -((0.5 * xp.pi / self.wavelength * focal_spread * alpha**2) ** 2)
-        ).astype(xp.float32)
+        ).astype(get_dtype(complex=False))
 
         return array
 
 
 def _aberration_property(name, key):
     def _getter(self):
         try:
             return getattr(self, name)[key]
         except KeyError:
             return 0.0
 
     def _setter(self, value):
-        value = _validate_distribution(value)
+        value = validate_distribution(value)
         getattr(self, name)[key] = value
 
     return property(_getter, _setter)
 
 
 class _HasAberrations:
     _aberration_coefficients: dict
@@ -860,22 +878,27 @@
 
     @property
     def _phase_aberrations_ensemble_axes_metadata(self) -> list[AxisMetadata]:
         axes_metadata = []
         for parameter_name, value in self._aberration_coefficients.items():
             if isinstance(value, BaseDistribution):
                 m = re.search(r"\d", parameter_name).start()
-                _tex_label = f"${parameter_name[:m]}_{{{parameter_name[m:]}}}$"
+
+                if parameter_name[:m] == "phi":
+                    _tex_label = f"$\\phi_{{{parameter_name[m:]}}}$"
+                else:
+                    _tex_label = f"${parameter_name[:m]}_{{{parameter_name[m:]}}}$"
+
                 axes_metadata += [
                     ParameterAxis(
                         label=parameter_name,
                         values=tuple(value.values),
                         units="Å",
                         _ensemble_mean=value.ensemble_mean,
-                        _tex_label=_tex_label,
+                        tex_label=_tex_label,
                     )
                 ]
         return axes_metadata
 
     @property
     def aberration_coefficients(self) -> dict[str, float | BaseDistribution]:
         """The aberration coefficients as a dictionary."""
@@ -899,28 +922,28 @@
         Parameters
         ----------
         aberration_coefficients : dict
             Mapping from aberration symbols to their corresponding values.
         """
 
         for symbol, value in aberration_coefficients.items():
-            value = _validate_distribution(value)
+            value = validate_distribution(value)
 
             if symbol in self._symbols():
                 self._aberration_coefficients[symbol] = value
 
             elif symbol in self._aliases().keys():
                 self._aberration_coefficients[self._aliases()[symbol]] = value
 
             else:
                 raise ValueError("{} not a recognized parameter".format(symbol))
 
         for symbol, value in aberration_coefficients.items():
             if symbol in ("defocus", "C10"):
-                value = _validate_distribution(value)
+                value = validate_distribution(value)
 
                 if isinstance(value, str) and value.lower() == "scherzer":
                     if self.energy is None:
                         raise RuntimeError(
                             "energy undefined, Scherzer defocus cannot be evaluated"
                         )
 
@@ -977,15 +1000,15 @@
             distributions=polar_symbols + ("angular_spread",),
             energy=energy,
             extent=extent,
             gpts=gpts,
             sampling=sampling,
         )
 
-        self._angular_spread = _validate_distribution(angular_spread)
+        self._angular_spread = validate_distribution(angular_spread)
         self._aberration_coefficients = self._default_aberration_coefficients()
 
         aberration_coefficients = (
             {} if aberration_coefficients is None else aberration_coefficients
         )
         aberration_coefficients = {**aberration_coefficients, **kwargs}
         self.set_aberrations(aberration_coefficients)
@@ -1185,27 +1208,29 @@
 
     def _evaluate_from_angular_grid(
         self, alpha: np.ndarray, phi: np.ndarray
     ) -> np.ndarray:
         xp = get_array_module(alpha)
 
         if not self._has_aberrations:
-            return xp.ones(self.ensemble_shape + alpha.shape, dtype=xp.complex64)
+            return xp.ones(
+                self.ensemble_shape + alpha.shape, dtype=get_dtype(complex=True)
+            )
 
         parameters, weights = _unpack_distributions(
             *tuple(self.aberration_coefficients.values()), shape=alpha.shape, xp=xp
         )
 
         parameters = dict(zip(polar_symbols, parameters))
 
         axis = tuple(range(0, len(self.ensemble_shape)))
         alpha = xp.expand_dims(alpha, axis=axis)
-        phi = xp.expand_dims(phi, axis=axis).astype(xp.float32)
+        phi = xp.expand_dims(phi, axis=axis).astype(get_dtype(complex=False))
 
-        array = xp.zeros(alpha.shape, dtype=np.float32)
+        array = xp.zeros(alpha.shape, dtype=get_dtype(complex=False))
         if self._nonzero_coefficients(("C10", "C12", "phi12")):
             array = array + (
                 1
                 / 2
                 * alpha**2
                 * (
                     parameters["C10"]
@@ -1259,22 +1284,23 @@
                     parameters["C50"]
                     + parameters["C52"] * xp.cos(2 * (phi - parameters["phi52"]))
                     + parameters["C54"] * xp.cos(4 * (phi - parameters["phi54"]))
                     + parameters["C56"] * xp.cos(6 * (phi - parameters["phi56"]))
                 )
             )
 
-        array *= np.float32(2 * xp.pi / self.wavelength)
+        dtype = get_dtype(complex=False)
+        array *= dtype(2 * xp.pi / self.wavelength)
         array = complex_exponential(-array)
 
         if cp is not None:
             weights = cp.asnumpy(weights)
 
         if weights is not None:
-            array = xp.asarray(weights, dtype=xp.float32) * array
+            array = xp.asarray(weights, dtype=dtype) * array
 
         return array
 
 
 class CTF(_HasAberrations, BaseAperture):
     """
     The contrast transfer function (CTF) describes the aberrations of the objective lens in HRTEM and specifies how
@@ -1337,21 +1363,22 @@
         extent: float | tuple[float, float] = None,
         gpts: int | tuple[int, int] = None,
         sampling: float | tuple[float, float] = None,
         flip_phase: bool = False,
         wiener_snr: float = 0.0,
         **kwargs,
     ):
+        distributions = polar_symbols + (
+            "angular_spread",
+            "focal_spread",
+            "semiangle_cutoff",
+        )
+
         super().__init__(
-            distributions=polar_symbols
-            + (
-                "angular_spread",
-                "focal_spread",
-                "semiangle_cutoff",
-            ),
+            distributions=distributions,
             energy=energy,
             semiangle_cutoff=semiangle_cutoff,
             extent=extent,
             gpts=gpts,
             sampling=sampling,
         )
 
@@ -1359,17 +1386,17 @@
 
         aberration_coefficients = (
             {} if aberration_coefficients is None else aberration_coefficients
         )
         aberration_coefficients = {**aberration_coefficients, **kwargs}
         self.set_aberrations(aberration_coefficients)
 
-        self._angular_spread = _validate_distribution(angular_spread)
-        self._focal_spread = _validate_distribution(focal_spread)
-        self._semiangle_cutoff = _validate_distribution(semiangle_cutoff)
+        self._angular_spread = validate_distribution(angular_spread)
+        self._focal_spread = validate_distribution(focal_spread)
+        self._semiangle_cutoff = validate_distribution(semiangle_cutoff)
         self._soft = soft
         self._flip_phase = flip_phase
         self._wiener_snr = wiener_snr
 
     @property
     def aberration_coefficients(self):
         return self._aberration_coefficients
@@ -1550,18 +1577,23 @@
         self, gpts: int | tuple[int, int], extent: float | tuple[float, float]
     ):
         from abtem.waves import Probe
 
         return (
             Probe(gpts=gpts, extent=extent, energy=self.energy, aperture=self)
             .build()
-            .complex_images()
+            .to_images()
         )
 
-    def profiles(self, gpts: int = 1000, max_angle: float = None, phi: float = 0.0):
+    def profiles(
+        self,
+        gpts: int = 1000,
+        max_angle: float = None,
+        phi: float = 0.0,
+    ):
         """
         Calculate radial line profiles for each included component (phase aberrations, aperture, temporal and spatial
         envelopes) of the contrast transfer function.
 
         Parameters
         ----------
         gpts: int
@@ -1582,27 +1614,30 @@
                 max_angle = 50
             else:
                 max_angle = self._max_semiangle_cutoff * 1.6
 
         self.accelerator.check_is_defined()
 
         sampling = max_angle / (gpts - 1) / (self.wavelength * 1e3)
-        alpha = np.linspace(0, max_angle * 1e-3, gpts).astype(np.float32)
+        alpha = np.linspace(0, max_angle * 1e-3, gpts).astype(get_dtype(complex=False))
+
+        # TODO : implement different complex representations
 
         components = dict()
 
         components["ctf"] = self._evaluate_to_match(self._aberrations, alpha, phi).imag
+        # components["ctf"] = convert_complex(components["ctf"], method=complex_representation)
 
         if self._spatial_envelope.angular_spread != 0.0:
-            components["spatial_envelope"] = self._evaluate_to_match(
+            components["spatial envelope"] = self._evaluate_to_match(
                 self._spatial_envelope, alpha, phi
             )
 
         if self._temporal_envelope.focal_spread != 0.0:
-            components["temporal_envelope"] = self._evaluate_to_match(
+            components["temporal envelope"] = self._evaluate_to_match(
                 self._temporal_envelope, alpha, phi
             )
 
         if self._aperture.semiangle_cutoff != np.inf:
             components["aperture"] = self._evaluate_to_match(self._aperture, alpha, phi)
 
         components["ctf"] = reduce(lambda x, y: x * y, tuple(components.values()))
@@ -1612,15 +1647,16 @@
             profiles = np.stack(
                 np.broadcast_arrays(*list(components.values())),
                 axis=-2,
             )
 
             component_metadata = [
                 OrdinalAxis(
-                    label="", values=tuple(components.keys()), _default_type="overlay"
+                    label="",
+                    values=tuple(components.keys()),
                 )
             ]
 
             ensemble_axes_metadata = ensemble_axes_metadata + component_metadata
         else:
             profiles = components["ctf"]
```

### Comparing `abtem-1.0.4/abtem/transform.py` & `abtem-1.0.5/abtem/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module to describe wave function transformations."""
+
 from __future__ import annotations
 
 import itertools
 from abc import abstractmethod, ABCMeta
 from functools import partial, reduce
 from typing import TYPE_CHECKING, Iterator
 
@@ -23,18 +24,19 @@
 from abtem.core.utils import (
     CopyMixin,
     expand_dims_to_broadcast,
     EqualityMixin,
 )
 from abtem.distributions import (
     EnsembleFromDistributions,
-    _validate_distribution,
+    validate_distribution,
     BaseDistribution,
 )
 
+
 if TYPE_CHECKING:
     from abtem.waves import Waves
     from abtem.array import ArrayObject
 
 
 class ArrayObjectTransform(Ensemble, EqualityMixin, CopyMixin, metaclass=ABCMeta):
     _allow_base_chunks: bool = False
@@ -168,15 +170,14 @@
     ) -> list[AxisMetadata] | tuple[list[AxisMetadata], ...]:
         return [*self.ensemble_axes_metadata, *array_object.ensemble_axes_metadata]
 
     def __add__(self, other: ArrayObjectTransform) -> CompositeArrayObjectTransform:
         transforms = []
 
         for transform in (self, other):
-
             if hasattr(transform, "transforms"):
                 transforms += transform.transforms
             else:
                 transforms += [transform]
 
         return CompositeArrayObjectTransform(transforms)
 
@@ -211,15 +212,14 @@
     def _extract(array, index):
         array = array.item()[index]
         return array
 
     def _pack_multiple_outputs(
         self, array_object: T, new_arrays: np.ndarray | da.core.Array
     ):
-
         is_lazy = isinstance(new_arrays, da.core.Array)
         # if is_lazy:
         #    assert ensemble_shape == new_arrays.shape
 
         outputs = ()
         for output_index in range(self._num_outputs):
             base_shape = self._out_base_shape(array_object, output_index)
@@ -269,15 +269,14 @@
         return outputs
 
     def _pack_single_output(
         self,
         array_object: T,
         new_array: np.ndarray,
     ):
-
         ensemble_axes_metadata = self._out_ensemble_axes_metadata(array_object)
 
         base_axes_metadata = self._out_base_axes_metadata(array_object)
 
         axes_metadata = ensemble_axes_metadata + base_axes_metadata
 
         metadata = self._out_metadata(array_object)
@@ -304,14 +303,17 @@
         array_object : ArrayObject
             The array object to transform.
 
         Returns
         -------
         transformed_array_object : ArrayObject
         """
+        # if not isinstance(array_object, ArrayObject):
+        # raise ValueError("Input must be an ArrayObject.")
+
         new_array = self._calculate_new_array(array_object)
         if self._num_outputs > 1:
             return self._pack_multiple_outputs(array_object, new_array)
         else:
             return self._pack_single_output(array_object, new_array)
 
 
@@ -322,22 +324,22 @@
 
 class EnsembleTransform(EnsembleFromDistributions, ArrayObjectTransform):
     def __init__(self, distributions: tuple[str, ...] = ()):
         super().__init__(distributions=distributions)
 
     @staticmethod
     def _validate_distribution(distribution):
-        return _validate_distribution(distribution)
+        return validate_distribution(distribution)
 
-    # def _validate_ensemble_axes_metadata(self, ensemble_axes_metadata):
-    #     if isinstance(ensemble_axes_metadata, AxisMetadata):
-    #         ensemble_axes_metadata = [ensemble_axes_metadata]
-    #
-    #     assert len(ensemble_axes_metadata) == len(self.ensemble_shape)
-    #     return ensemble_axes_metadata
+    def _validate_ensemble_axes_metadata(self, ensemble_axes_metadata):
+        if isinstance(ensemble_axes_metadata, AxisMetadata):
+            ensemble_axes_metadata = [ensemble_axes_metadata]
+
+        assert len(ensemble_axes_metadata) == len(self.ensemble_shape)
+        return ensemble_axes_metadata
 
     def _get_axes_metadata_from_distributions(self, **kwargs):
         ensemble_axes_metadata = []
         for name in kwargs.keys():
             assert name in self._distributions
             distribution = getattr(self, name)
             if isinstance(distribution, BaseDistribution):
@@ -362,14 +364,33 @@
         return self._distributions
 
     def apply(self, waves: Waves) -> Waves:
         waves = super().apply(waves)
         return waves
 
 
+class TransformFromFunc(WavesTransform):
+
+    def __init__(self, func, func_kwargs):
+        self._func = func
+        self._func_kwargs = func_kwargs
+        super().__init__()
+
+    @property
+    def func(self):
+        return self._func
+
+    @property
+    def func_kwargs(self):
+        return self._func_kwargs
+
+    def _calculate_new_array(self, array_object):
+        return self.func(array_object, **self.func_kwargs)
+
+
 class CompositeArrayObjectTransform(ArrayObjectTransform):
     """
     Combines multiple array object transformations into a single transformation.
 
     Parameters
     ----------
     transforms : ArrayObject
@@ -396,15 +417,14 @@
         super().__init__()
 
     @property
     def _num_outputs(self) -> int:
         return self._transforms[0]._num_outputs
 
     def set_output_specification(self, array_object):
-
         for transform in reversed(self.transforms):
             array_object = array_object.apply_transform(transform)
 
         if self._num_outputs == 1:
             output = [array_object]
         else:
             output = array_object
@@ -472,15 +492,14 @@
         ]
         ensemble_axes_metadata = list(itertools.chain(*ensemble_axes_metadata))
         return ensemble_axes_metadata
 
     def _out_ensemble_axes_metadata(self, array_object, index=0) -> list[AxisMetadata]:
         if self._ensemble_axes_metadata is not None:
             return self._ensemble_axes_metadata[index]
-
         return self.ensemble_axes_metadata + array_object.ensemble_axes_metadata
 
     def _out_base_axes_metadata(self, array_object, index=0) -> list[AxisMetadata]:
         if self._base_axes_metadata is not None:
             return self._base_axes_metadata[index]
         return self._transforms[0]._out_base_axes_metadata(array_object, index)
 
@@ -536,15 +555,14 @@
             return super().apply(array_object)
         else:
             return array_object
 
     def _calculate_new_array(
         self, array_object: T
     ) -> np.ndarray | tuple[np.ndarray, ...]:
-
         for transform in reversed(self.transforms):
             array_object = transform.apply(array_object)
 
         if self._num_outputs > 1:
             return tuple(array_object[i].array for i in range(self._num_outputs))
         else:
             return array_object.array
@@ -602,15 +620,14 @@
     """
 
     def __init__(
         self,
         in_place: bool = False,
         distributions: tuple[str, ...] = (),
     ):
-
         self._in_place = in_place
         super().__init__(distributions=distributions)
 
     @property
     def in_place(self) -> bool:
         """The array representing the waves may be modified in-place."""
         return self._in_place
```

### Comparing `abtem-1.0.4/abtem/waves.py` & `abtem-1.0.5/abtem/waves.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for describing wave functions of the incoming electron beam and the exit wave."""
+
 from __future__ import annotations
 
 import itertools
 from abc import abstractmethod
 from copy import copy
 from functools import partial
 from numbers import Number
@@ -15,14 +16,15 @@
 import abtem
 from abtem.array import ArrayObject, ComputableList, _expand_dims, _validate_lazy
 from abtem.core.axes import (
     RealSpaceAxis,
     ReciprocalSpaceAxis,
     AxisMetadata,
     AxesMetadataList,
+    OrdinalAxis,
 )
 from abtem.core.backend import (
     get_array_module,
     validate_device,
     device_name_from_array_module,
 )
 from abtem.core.chunks import validate_chunks
@@ -39,29 +41,38 @@
 from abtem.core.grid import Grid, validate_gpts, polar_spatial_frequencies
 from abtem.core.grid import HasGridMixin
 from abtem.core.utils import (
     safe_floor_int,
     CopyMixin,
     EqualityMixin,
     tuple_range,
+    get_dtype,
 )
 from abtem.detectors import (
     BaseDetector,
     FlexibleAnnularDetector,
 )
 from abtem.distributions import BaseDistribution
+from abtem.inelastic.core_loss import (
+    BaseTransitionPotential,
+    _validate_transition_potentials,
+)
 from abtem.measurements import (
     DiffractionPatterns,
     Images,
     BaseMeasurements,
     RealSpaceLineProfiles,
 )
-from abtem.multislice import MultisliceTransform
+from abtem.multislice import (
+    MultisliceTransform,
+    transition_potential_multislice_and_detect,
+)
 from abtem.potentials.iam import BasePotential, _validate_potential
-from abtem.scan import BaseScan, GridScan, _validate_scan
+from abtem.scan import BaseScan, GridScan, _validate_scan, CustomScan
+from abtem.slicing import SliceIndexedAtoms
 from abtem.tilt import _validate_tilt
 from abtem.transfer import Aberrations, CTF, Aperture, BaseAperture
 from abtem.transform import (
     ArrayObjectTransform,
 )
 
 
@@ -111,15 +122,15 @@
     def device(self):
         """The device where the waves are built or stored."""
         pass
 
     @property
     def dtype(self):
         """The datatype of waves."""
-        return np.complex64
+        return get_dtype(complex=True)
 
     @property
     @abstractmethod
     def metadata(self) -> dict:
         """Metadata stored as a dictionary."""
         pass
 
@@ -188,15 +199,14 @@
             return n, m
 
         return valid_gpts
 
     def _gpts_within_angle(
         self, angle: float | str, parity: str = "same"
     ) -> tuple[int, int]:
-
         if angle is None or angle == "full":
             return self.gpts
 
         elif isinstance(angle, (Number, float)):
             gpts = (
                 int(2 * np.ceil(angle / self.angular_sampling[0])) + 1,
                 int(2 * np.ceil(angle / self.angular_sampling[1])) + 1,
@@ -295,15 +305,14 @@
         energy: float,
         extent: float | tuple[float, float] = None,
         sampling: float | tuple[float, float] = None,
         reciprocal_space: bool = False,
         ensemble_axes_metadata: list[AxisMetadata] = None,
         metadata: dict = None,
     ):
-
         if sampling is not None and extent is not None:
             extent = None
 
         self._grid = Grid(
             extent=extent, gpts=array.shape[-2:], sampling=sampling, lock_gpts=True
         )
         self._accelerator = Accelerator(energy=energy)
@@ -342,15 +351,14 @@
         self._metadata["reciprocal_space"] = self.reciprocal_space
         return self._metadata
 
     @classmethod
     def from_array_and_metadata(
         cls, array: np.ndarray, axes_metadata: list[AxisMetadata], metadata: dict = None
     ) -> Waves:
-
         """
         Creates wave functions from a given array and metadata.
 
         Parameters
         ----------
         array : array
             Complex array defining one or more 2D wave functions. The second-to-last and last dimensions are the wave
@@ -607,65 +615,87 @@
             return xp.exp(1.0j * amount) * array
 
         d = self._copy_kwargs(exclude=("array",))
         d["array"] = _phase_shift(self.array)
         d["reciprocal_space"] = False
         return self.__class__(**d)
 
-    def intensity(self) -> Images:
+    def to_images(self, convert_complex: str = None) -> Images:
         """
-        Calculate the intensity of the wave functions.
+        The complex array of the wave functions at the image plane.
 
         Returns
         -------
-        intensity_images : Images
-            The intensity of the wave functions.
+        images : Images
+            The wave functions as an image.
         """
-
-        def _intensity(array):
-            return abs2(array)
-
+        array = self.array.copy()
         metadata = copy(self.metadata)
         metadata["label"] = "intensity"
         metadata["units"] = "arb. unit"
-
-        xp = get_array_module(self.array)
-
-        if self.is_lazy:
-            array = self.array.map_blocks(_intensity, dtype=xp.float32)
-        else:
-            array = _intensity(self.array)
-
-        return Images(
+        images = Images(
             array,
             sampling=self.sampling,
             ensemble_axes_metadata=self.ensemble_axes_metadata,
             metadata=metadata,
         )
 
-    def complex_images(self):
+        if not convert_complex:
+            return images
+
+        if convert_complex in ("intensity", "phase", "real", "imag"):
+            return getattr(images, convert_complex)()
+        else:
+            raise ValueError(
+                f"convert_complex must be one of 'intensity', 'phase', 'real', 'imag'"
+            )
+
+    def intensity(self) -> Images:
         """
-        The complex array of the wave functions at the image plane.
+        Calculate the intensity of the wave functions.
 
         Returns
         -------
-        complex_images : Images
-            The wave functions as a complex image.
+        intensity_images : Images
+            The intensity of the wave functions.
         """
+        return self.to_images(convert_complex="intensity")
 
-        array = self.array.copy()
-        metadata = copy(self.metadata)
-        metadata["label"] = "intensity"
-        metadata["units"] = "arb. unit"
-        return Images(
-            array,
-            sampling=self.sampling,
-            ensemble_axes_metadata=self.ensemble_axes_metadata,
-            metadata=metadata,
-        )
+    def phase(self) -> Images:
+        """
+        Calculate the phase of the wave functions.
+
+        Returns
+        -------
+        phase_images : Images
+            The phase of the wave functions.
+        """
+        return self.to_images(convert_complex="phase")
+
+    def real(self) -> Images:
+        """
+        Calculate the real part of the wave functions.
+
+        Returns
+        -------
+        real_images : Images
+            The real part of the wave functions.
+        """
+        return self.to_images(convert_complex="real")
+
+    def imag(self) -> Images:
+        """
+        Calculate the imaginary part of the wave functions.
+
+        Returns
+        -------
+        imaginary_images : Images
+            The imaginary part of the wave functions.
+        """
+        return self.to_images(convert_complex="imag")
 
     def downsample(
         self,
         max_angle: str | float = "cutoff",
         gpts: tuple[int, int] = None,
         normalization: str = "values",
     ) -> Waves:
@@ -712,15 +742,15 @@
 
         if self.is_lazy:
             array = self.array.map_blocks(
                 fft_interpolate,
                 new_shape=gpts,
                 normalization=normalization,
                 chunks=self.array.chunks[:-2] + gpts,
-                meta=xp.array((), dtype=xp.complex64),
+                meta=xp.array((), dtype=get_dtype(complex=True)),
             )
         else:
             array = fft_interpolate(
                 self.array, new_shape=gpts, normalization=normalization
             )
 
         kwargs = self._copy_kwargs(exclude=("array",))
@@ -783,15 +813,15 @@
             The diffraction pattern(s).
         """
 
         def _diffraction_pattern(array, new_gpts, return_complex, fftshift, normalize):
             xp = get_array_module(array)
 
             if normalize:
-                array = array / np.prod(array.shape[-2:])
+                array = array / float(np.prod(array.shape[-2:]))
 
             array = fft2(array, overwrite_x=False)
 
             if array.shape[-2:] != new_gpts:
                 array = fft_crop(array, new_shape=array.shape[:-2] + new_gpts)
 
             if not return_complex:
@@ -821,15 +851,15 @@
                 raise RuntimeError(
                     f"normalization {metadata['normalization']} not recognized"
                 )
 
         validate_gpts(new_gpts)
 
         if self.is_lazy:
-            dtype = xp.complex64 if return_complex else xp.float32
+            dtype = get_dtype(complex=return_complex)
 
             pattern = self.array.map_blocks(
                 _diffraction_pattern,
                 new_gpts=new_gpts,
                 fftshift=fftshift,
                 return_complex=return_complex,
                 normalize=normalize,
@@ -893,14 +923,61 @@
             ctf.accelerator.match(self.accelerator)
 
         self.accelerator.match(ctf.accelerator, check_match=True)
         self.accelerator.check_is_defined()
 
         return self.apply_transform(ctf, max_batch=max_batch)
 
+    def transition_potential_multislice(
+        self,
+        potential: BasePotential,
+        transition_potentials: BaseTransitionPotential | list[BaseTransitionPotential],
+        detectors: BaseDetector | list[BaseDetector] = None,
+        sites: SliceIndexedAtoms | Atoms = None,
+    ) -> Waves | BaseMeasurements:
+        transition_potentials = _validate_transition_potentials(transition_potentials)
+
+        potential = _validate_potential(potential, self)
+
+        measurements = []
+        for transition_potential in transition_potentials:
+            multislice_transform = MultisliceTransform(
+                potential=potential,
+                detectors=detectors,
+                multislice_func=transition_potential_multislice_and_detect,
+                transition_potential=transition_potential,
+                sites=sites,
+            )
+            measurements.append(self.apply_transform(transform=multislice_transform))
+
+        if len(measurements) > 1:
+            axis_metadata = OrdinalAxis(
+                label="Z, n, l",
+                values=[
+                    ",".join(
+                        (
+                            str(transition_potential.metadata["Z"]),
+                            str(transition_potential.metadata["n"]),
+                            str(transition_potential.metadata["l"]),
+                        )
+                    )
+                    for transition_potential in transition_potentials
+                ],
+                tex_label="$Z, n, \ell$",
+            )
+
+            measurements = abtem.stack(
+                measurements,
+                axis_metadata,
+            )
+        else:
+            measurements = measurements[0]
+
+        return _reduce_ensemble(measurements)
+
     def multislice(
         self,
         potential: BasePotential,
         detectors: BaseDetector | list[BaseDetector] = None,
     ) -> Waves:
         """
         Propagate and transmit wave function through the provided potential using the multislice algorithm. When
@@ -930,15 +1007,60 @@
             potential=potential, detectors=detectors
         )
 
         waves = self.apply_transform(transform=multislice_transform)
 
         return _reduce_ensemble(waves)
 
-    def show(self, complex_images:bool=False, **kwargs):
+    def scan(
+        self,
+        scan: BaseScan | np.ndarray | Sequence,
+        potential: Atoms | BasePotential = None,
+        detectors: BaseDetector | Sequence[BaseDetector] = None,
+        max_batch: int | str = "auto",
+    ) -> BaseMeasurements | Waves | list[BaseMeasurements | Waves]:
+        """
+        Run the multislice algorithm from probe wave functions over the provided scan.
+
+        Parameters
+        ----------
+        potential : BasePotential or Atoms
+            The scattering potential.
+        scan : BaseScan
+            Positions of the probe wave functions. If not given, scans across the entire potential at Nyquist sampling.
+        detectors : BaseDetector, list of BaseDetector, optional
+            A detector or a list of detectors defining how the wave functions should be converted to measurements after
+            running the multislice algorithm. See abtem.measurements.detect for a list of implemented detectors.
+        max_batch : int, optional
+            The number of wave functions in each chunk of the Dask array. If 'auto' (default), the batch size is
+            automatically chosen based on the abtem user configuration settings "dask.chunk-size" and
+            "dask.chunk-size-gpu".
+
+        Returns
+        -------
+        detected_waves : BaseMeasurements or list of BaseMeasurement
+            The detected measurement (if detector(s) given).
+        exit_waves : Waves
+            Wave functions at the exit plane(s) of the potential (if no detector(s) given).
+        """
+        scan = _validate_scan(scan)
+
+        waves = self.apply_transform(scan, max_batch=max_batch)
+
+        if potential is None:
+            return waves
+
+        measurements = waves.multislice(
+            potential=potential,
+            detectors=detectors,
+        )
+
+        return measurements
+
+    def show(self, complex_images: bool = False, **kwargs):
         """
         Show the wave-function intensities.
 
         kwargs :
             Keyword arguments for `abtem.measurements.Images.show`.
         """
 
@@ -968,19 +1090,23 @@
         output = output.reduce_ensemble()
 
     return output
 
 
 class _WavesBuilder(BaseWaves, Ensemble, CopyMixin, EqualityMixin):
     def __init__(self, ensemble_names: tuple[str, ...], device: str):
-
         self._ensemble_names = ensemble_names
         self._device = device
         super().__init__()
 
+    def apply_transform(
+        self, transform, max_batch: int | str = "auto", lazy: bool = True
+    ):
+        return self.build(lazy=lazy).apply_transform(transform, max_batch=max_batch)
+
     def check_can_build(self, potential: BasePotential = None):
         """Check whether the wave functions can be built."""
         if potential is not None:
             self.grid.match(potential)
         self.grid.check_is_defined()
         self.accelerator.check_is_defined()
 
@@ -1029,15 +1155,15 @@
             for i in range(len(cumulative_shapes) - 1)
         ]
 
     def _partition_args(self, chunks=(1,), lazy: bool = True):
         if chunks is None:
             chunks = self._default_ensemble_chunks
             chunks = validate_chunks(
-                self.ensemble_shape, chunks, limit="auto", dtype=np.complex64
+                self.ensemble_shape, chunks, limit="auto", dtype=get_dtype(complex=True)
             )
 
         chunks = validate_chunks(self.ensemble_shape, chunks)
 
         args = ()
         for arg_split, ensemble in zip(self._chunk_splits(), self._ensembles.values()):
             arg_chunks = chunks[slice(*arg_split)]
@@ -1049,15 +1175,14 @@
     def _from_partitioned_args_func(
         cls,
         *args,
         partials,
         arg_splits,
         **kwargs,
     ):
-
         args = unpack_blockwise_args(args)
         for arg_split, (name, partial) in zip(arg_splits, partials.items()):
             kwargs[name] = partial(*args[slice(*arg_split)]).item()
 
         new_probe = cls(
             **kwargs,
         )
@@ -1125,15 +1250,15 @@
 
         blocks = waves_builder.ensemble_blocks(chunks=chunks[:-2])
 
         xp = get_array_module(waves_builder.device)
 
         array = blocks.map_blocks(
             waves_builder._build_waves,
-            meta=xp.array((), dtype=np.complex64),
+            meta=xp.array((), dtype=get_dtype(complex=True)),
             new_axis=tuple_range(2, len(waves_builder.ensemble_shape)),
             chunks=blocks.chunks + waves_builder.gpts,
             wrapped=False,
         )
 
         return Waves(
             array,
@@ -1175,15 +1300,14 @@
         gpts: int | tuple[int, int] = None,
         sampling: float | tuple[float, float] = None,
         energy: float = None,
         normalize: bool = False,
         tilt: tuple[float, float] = (0.0, 0.0),
         device: str = None,
     ):
-
         self._grid = Grid(extent=extent, gpts=gpts, sampling=sampling)
         self._accelerator = Accelerator(energy=energy)
         self._tilt = _validate_tilt(tilt=tilt)
         self._normalize = normalize
         device = validate_device(device)
 
         super().__init__(ensemble_names=("tilt",), device=device)
@@ -1216,19 +1340,21 @@
         if hasattr(waves_builder, "item"):
             waves_builder = waves_builder.item()
 
         xp = get_array_module(waves_builder.device)
 
         if waves_builder.normalize:
             array = xp.full(
-                waves_builder.gpts, 1 / np.prod(waves_builder.gpts), dtype=xp.complex64
+                waves_builder.gpts,
+                1 / np.prod(waves_builder.gpts),
+                dtype=get_dtype(complex=True),
             )
 
         else:
-            array = xp.ones(waves_builder.gpts, dtype=xp.complex64)
+            array = xp.ones(waves_builder.gpts, dtype=get_dtype(complex=True))
 
         waves = Waves(
             array,
             energy=waves_builder.energy,
             extent=waves_builder.extent,
             metadata=waves_builder.metadata,
             reciprocal_space=False,
@@ -1364,27 +1490,27 @@
         self,
         semiangle_cutoff: float = None,
         extent: float | tuple[float, float] = None,
         gpts: int | tuple[int, int] = None,
         sampling: float | tuple[float, float] = None,
         energy: float = None,
         soft: bool = True,
-        tilt: tuple[float | BaseDistribution, float | BaseDistribution]
-        | BaseDistribution = (
+        tilt: (
+            tuple[float | BaseDistribution, float | BaseDistribution] | BaseDistribution
+        ) = (
             0.0,
             0.0,
         ),
         device: str = None,
         aperture: BaseAperture = None,
         aberrations: Aberrations | dict = None,
         positions: BaseScan = None,
         metadata: dict = None,
         **kwargs,
     ):
-
         self._accelerator = Accelerator(energy=energy)
 
         # if not ((semiangle_cutoff is None) + (aperture is None) == 1):
         #     raise ValueError("provide exactly one of `semiangle_cutoff` or `aperture`")
         # elif semiangle_cutoff is None:
         #     semiangle_cutoff = 30.0
 
@@ -1528,14 +1654,48 @@
         waves = waves.ensure_real_space()
 
         if not wrapped:
             waves = waves.array
 
         return waves
 
+    def _validate_and_build(
+        self,
+        scan: Sequence | BaseScan = None,
+        max_batch: int | str = "auto",
+        lazy: bool = None,
+        potential=None,
+    ):
+        self.check_can_build(potential)
+        lazy = _validate_lazy(lazy)
+
+        probe = self.copy()
+
+        if potential is not None:
+            probe.grid.match(potential)
+
+        scan = _validate_scan(scan, probe)
+
+        if isinstance(scan, CustomScan):
+            squeeze = True
+        else:
+            squeeze = False
+
+        probe._positions = scan
+
+        if not lazy:
+            probes = self._build_waves(probe)
+        else:
+            probes = self._lazy_build_waves(probe, max_batch)
+
+        if squeeze:
+            probes = probes.squeeze(axis=(-3,))
+
+        return probes
+
     def build(
         self,
         scan: Sequence | BaseScan = None,
         max_batch: int | str = "auto",
         lazy: bool = None,
     ) -> Waves:
         """
@@ -1554,29 +1714,15 @@
             setting in the user configuration file.
 
         Returns
         -------
         probe_wave_functions : Waves
             The built probe wave functions.
         """
-        self.check_can_build()
-        lazy = _validate_lazy(lazy)
-
-        scan = _validate_scan(scan, self)
-
-        probe = self.copy()
-
-        probe._positions = scan
-
-        if not lazy:
-            probes = self._build_waves(probe)
-        else:
-            probes = self._lazy_build_waves(probe, max_batch)
-
-        return _reduce_ensemble(probes)
+        return self._validate_and_build(scan=scan, max_batch=max_batch, lazy=lazy)
 
     def multislice(
         self,
         potential: BasePotential | Atoms,
         scan: tuple | BaseScan = None,
         detectors: BaseDetector = None,
         max_batch: int | str = "auto",
@@ -1602,35 +1748,100 @@
             If True, create the wave functions lazily, otherwise, calculate instantly. If None, this defaults to the
             setting in the user configuration file.
 
         Returns
         -------
         measurements : BaseMeasurements or Waves or list of BaseMeasurement
         """
-
         potential = _validate_potential(potential)
 
-        self.check_can_build(potential)
+        probes = self._validate_and_build(
+            scan=scan, max_batch=max_batch, lazy=lazy, potential=potential
+        )
 
-        lazy = _validate_lazy(lazy)
+        multislice = MultisliceTransform(potential, detectors)
 
-        probe = self.copy()
+        measurements = probes.apply_transform(multislice)
+        return _reduce_ensemble(measurements)
+
+    def transition_potential_scan(
+        self,
+        potential: BasePotential | Atoms,
+        transition_potentials: BaseTransitionPotential | list[BaseTransitionPotential],
+        scan: tuple | BaseScan = None,
+        detectors: BaseDetector | list[BaseDetector] = None,
+        sites: SliceIndexedAtoms | Atoms = None,
+        # detectors_elastic: BaseDetector | list[BaseDetector] = None,
+        double_channel: bool = True,
+        threshold: float = 1.0,
+        max_batch: int | str = "auto",
+        lazy: bool = None,
+    ) -> Waves | BaseMeasurements:
+        """
+        Parameters
+        ----------
+        potential : BasePotential | Atoms
+            The potential to be used for calculating the transition potentials.
+            It can be an instance of `BasePotential` or an `Atoms` object.
+        transition_potentials : BaseTransitionPotential | list[BaseTransitionPotential]
+            The transition potentials to be used for multislice calculations.
+            It can be an instance of `BaseTransitionPotential` or a list of `BaseTransitionPotential` objects.
+        scan : tuple | BaseScan, optional
+            The scan parameters. It can be a tuple or an instance of `BaseScan`.
+            Defaults to None.
+        detectors : BaseDetector | list[BaseDetector], optional
+            A detector or a list of detectors defining how the wave functions should be converted to measurements after
+            running the multislice algorithm. See abtem.measurements.detect for a list of implemented detectors.
+            Defaults to None, which
+        sites : SliceIndexedAtoms | Atoms, optional
+            The slice indexed atoms to be used for multislice calculations.
+            It can be an instance of `SliceIndexedAtoms` or an `Atoms` object.
+            Defaults to None.
+        detectors_elastic : BaseDetector | list[BaseDetector], optional
+            The elastic detectors to be used for recording the measurements.
+            It can be an instance of `BaseDetector` or a list of `BaseDetector` objects.
+            Defaults to None.
+        double_channel : bool, optional
+            A boolean indicating whether to use double channel for recording the measurements.
+            Defaults to True.
+        max_batch : int | str, optional
+            The maximum batch size for parallel processing.
+            It can be an integer or the string "auto".
+            Defaults to "auto".
+        lazy : bool, optional
+            A boolean indicating whether to use lazy evaluation for the calculations.
+            Defaults to None.
 
-        probe.grid.match(potential)
+        Returns
+        -------
+        Waves | BaseMeasurements
+            The calculated waves or measurements, depending on the value of `lazy`.
 
-        scan = _validate_scan(scan, probe)
+        """
+        if scan is None:
+            scan = GridScan()
 
-        probe._positions = scan
+        if detectors is None:
+            detectors = FlexibleAnnularDetector()
 
-        if not lazy:
-            probes = self._build_waves(probe)
-        else:
-            probes = self._lazy_build_waves(probe, max_batch)
+        potential = _validate_potential(potential)
 
-        multislice = MultisliceTransform(potential, detectors)
+        probes = self._validate_and_build(
+            scan=scan, max_batch=max_batch, lazy=lazy, potential=potential
+        )
+
+        multislice = MultisliceTransform(
+            potential,
+            detectors,
+            multislice_func=transition_potential_multislice_and_detect,
+            transition_potential=transition_potentials,
+            sites=sites,
+            double_channel=double_channel,
+            threshold=threshold,
+        )
 
         measurements = probes.apply_transform(multislice)
 
         return _reduce_ensemble(measurements)
 
     def scan(
         self,
```

### Comparing `abtem-1.0.4/abtem.egg-info/SOURCES.txt` & `abtem-1.0.5/abtem.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,62 +7,66 @@
 abtem/__init__.py
 abtem/_version.py
 abtem/antialias.py
 abtem/array.py
 abtem/atoms.py
 abtem/detectors.py
 abtem/distributions.py
-abtem/indexing.py
+abtem/finite_difference.py
 abtem/integrals.py
 abtem/mcf.py
 abtem/measurements.py
 abtem/mtf.py
 abtem/multislice.py
 abtem/noise.py
 abtem/reconstruct.py
 abtem/scan.py
 abtem/slicing.py
 abtem/tilt.py
 abtem/transfer.py
 abtem/transform.py
-abtem/visualize.py
-abtem/visualize_new.py
 abtem/waves.py
 abtem.egg-info/PKG-INFO
 abtem.egg-info/SOURCES.txt
 abtem.egg-info/dependency_links.txt
 abtem.egg-info/not-zip-safe
 abtem.egg-info/requires.txt
 abtem.egg-info/top_level.txt
+abtem/bloch/__init__.py
+abtem/bloch/dynamical.py
+abtem/bloch/indexing.py
+abtem/bloch/matrix_exponential.py
+abtem/bloch/utils.py
 abtem/core/__init__.py
 abtem/core/_cuda.py
 abtem/core/abtem.yaml
 abtem/core/axes.py
+abtem/core/axes_new.py
 abtem/core/backend.py
 abtem/core/chunks.py
 abtem/core/colors.py
 abtem/core/complex.py
 abtem/core/config.py
 abtem/core/constants.py
+abtem/core/diagnostics.py
 abtem/core/electron_configurations.py
 abtem/core/energy.py
 abtem/core/ensemble.py
 abtem/core/fft.py
 abtem/core/grid.py
 abtem/core/units.py
 abtem/core/utils.py
 abtem/inelastic/__init__.py
 abtem/inelastic/core_loss.py
 abtem/inelastic/phonons.py
 abtem/inelastic/plasmons.py
 abtem/magnetism/__init__.py
-abtem/magnetism/parametrization.py
-abtem/magnetism/realspace_multislice.py
-abtem/magnetism/vector_potential.py
-abtem/magnetism/data/lyon.json
+abtem/magnetism/iam.py
+abtem/magnetism/parametrizations/__init__.py
+abtem/magnetism/parametrizations/data/lyon.json
 abtem/parametrizations/__init__.py
 abtem/parametrizations/data/kirkland.json
 abtem/parametrizations/data/lobato.json
 abtem/parametrizations/data/peng_high.json
 abtem/parametrizations/data/peng_ionic.json
 abtem/parametrizations/data/peng_low.json
 abtem/parametrizations/data/waasmaier_kirfel.json
@@ -75,30 +79,36 @@
 abtem/potentials/_poisson.py
 abtem/potentials/charge_density.py
 abtem/potentials/gpaw.py
 abtem/potentials/iam.py
 abtem/prism/__init__.py
 abtem/prism/_natural_neighbors.py
 abtem/prism/_partitioned_s_matrix.py
-abtem/prism/bloch.py
 abtem/prism/s_matrix.py
 abtem/prism/utils.py
+abtem/visualize/__init__.py
+abtem/visualize/artists.py
+abtem/visualize/axes_grid.py
+abtem/visualize/visualizations.py
+abtem/visualize/widgets.py
 test/test_array.py
 test/test_atomic_potential.py
 test/test_copy.py
 test/test_ctf.py
 test/test_detect.py
 test/test_distributions.py
 test/test_ensemble.py
 test/test_ewald.py
+test/test_fft.py
 test/test_gpaw.py
 test/test_grid.py
 test/test_hyperspy.py
 test/test_ionization.py
 test/test_kirkland.py
+test/test_magnetics.py
 test/test_measure.py
 test/test_potential_parametrization.py
 test/test_potentials.py
 test/test_prism.py
 test/test_scan.py
 test/test_simulate.py
 test/test_structures.py
```

### Comparing `abtem-1.0.4/setup.cfg` & `abtem-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/test/test_array.py` & `abtem-1.0.5/test/test_array.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/test/test_atomic_potential.py` & `abtem-1.0.5/test/test_atomic_potential.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import hypothesis.strategies as st
 import numpy as np
 import pytest
 from hypothesis import given
 
-from abtem.integrals import GaussianProjectionIntegrals
-from abtem.integrals import ProjectionQuadratureRule
+#from abtem.integrals import GaussianProjectionIntegrals
+from abtem.integrals import QuadratureProjectionIntegrals
 
 from abtem.parametrizations import LobatoParametrization, KirklandParametrization, PengParametrization
 
 
 @given(atomic_number=st.integers(min_value=1, max_value=98))
 @pytest.mark.parametrize('parametrization_a',
                          [LobatoParametrization(),
@@ -27,122 +27,122 @@
                        atol=10, rtol=0.1)
     r = np.linspace(.2, 5, 100)
     assert np.allclose(parametrization_a.projected_potential(atomic_number)(r),
                        parametrization_b.projected_potential(atomic_number)(r),
                        atol=20, rtol=0.1)
 
 
-@pytest.mark.parametrize('parameters',
-                         [{'gaussian_projection_integrals':
-                               GaussianProjectionIntegrals(correction_parametrization=None),
-                           'parametrization':
-                               PengParametrization()
-                           },
-                          {'gaussian_projection_integrals':
-                               GaussianProjectionIntegrals(correction_parametrization='lobato'),
-                           'parametrization': LobatoParametrization()
-                           }
-                          ], ids=['uncorrected', 'corrected'])
-def test_gaussian_projection_integrals(parameters):
-    parametrization = parameters['parametrization']
-    gaussian_projection_integrals = parameters['gaussian_projection_integrals']
-
-    symbol = 'C'
-    gpts = (256, 256)
-    sampling = (0.1, 0.1)
-    positions = np.array([[0, 0, 0]], dtype=np.float32)
-    a = -np.inf
-    b = np.inf
-
-    gaussian_scattering_factors = gaussian_projection_integrals.build('C', gpts, sampling)
-
-    projections = gaussian_scattering_factors.integrate_on_grid(
-        positions,
-        a,
-        b,
-        gpts,
-        sampling,
-        fourier_space=True)
-
-    k = np.abs(np.fft.fftfreq(gpts[0], sampling[0])).astype(np.float32)
-    analytical = parametrization.projected_scattering_factor(symbol)(k ** 2)
-    assert np.allclose(analytical, projections[0].real, rtol=1e-6)
-
-
-@pytest.mark.parametrize('fourier_space', [True, False])
-def test_finite_gaussian_projection_integrals(fourier_space):
-    gaussian_projection_integrals = GaussianProjectionIntegrals(correction_parametrization=None)
-
-    symbol = 'C'
-    gpts = (256, 256)
-    sampling = (0.02, 0.02)
-    positions = np.array([[0, 0, 0]], dtype=np.float32)
-    a = -.2
-    b = .2
-
-    gaussian_scattering_factors = gaussian_projection_integrals.build('C', gpts, sampling)
-
-    projections = gaussian_scattering_factors.integrate_on_grid(
-        positions,
-        a,
-        b,
-        gpts,
-        sampling,
-        fourier_space=fourier_space)
-
-    if fourier_space:
-        k = np.abs(np.fft.fftfreq(gpts[0], sampling[0])).astype(np.float32)
-        analytical = PengParametrization().finite_projected_scattering_factor(symbol)(k, a, b)
-        assert np.allclose(analytical, projections[0].real, rtol=1e-6)
-
-    else:
-        r = np.linspace(0, gpts[0] * sampling[0], gpts[0], endpoint=False)
-        analytical = PengParametrization().finite_projected_potential(symbol)(r, a, b)
-        assert np.allclose(analytical[:len(r) // 2], projections[0][:len(r) // 2], rtol=1e-6, atol=5)
-
-
-@pytest.mark.parametrize('parametrization',
-                         [LobatoParametrization(),
-                          KirklandParametrization()])
-def test_quadrature(parametrization):
-    quadrature = ProjectionQuadratureRule(parametrization, quad_order=20, cutoff_tolerance=1e-9)
-
-    symbol = 'Au'
-    gpts = (256, 256)
-    sampling = (0.05, 0.05)
-    xp = np
-    a = -20
-    b = 20
-
-    positions = xp.array([[0, 0, 0]], dtype=xp.float32)
-
-    table = quadrature.build_integral_table(symbol, min(sampling) / 2)
-
-    integrated = table.integrate_on_grid(positions, a, b, gpts, sampling)
-
-    r = np.linspace(0, gpts[0] * sampling[0], gpts[0], endpoint=False).astype(np.float32)
-    analytical = parametrization.projected_potential(symbol)(r[1:])
-
-    assert np.allclose(analytical, integrated[0, 1:], atol=2)
-
-
-def test_finite_projections():
-    quadrature = ProjectionQuadratureRule('lobato', quad_order=8, cutoff_tolerance=1e-4)
-    gaussian_projection_integrals = GaussianProjectionIntegrals()
-
-    symbol = 'C'
-    gpts = (256, 256)
-    sampling = (0.05, 0.05)
-    a = .1
-    b = 1
-
-    positions = np.array([[0, 0, 0]], dtype=np.float32)
-
-    table = quadrature.build_integral_table(symbol, min(sampling) / 2)
-
-    quadrature_potential = table.integrate_on_grid(positions, a, b, gpts, sampling)
-
-    gaussian_scattering_factors = gaussian_projection_integrals.build(symbol, gpts, sampling)
-
-    gaussian_potential = gaussian_scattering_factors.integrate_on_grid(positions, a, b, gpts, sampling)
-
-    assert np.allclose(quadrature_potential[0, :gpts[1] // 2], gaussian_potential[0, :gpts[1] // 2], atol=2)
+# @pytest.mark.parametrize('parameters',
+#                          [{'gaussian_projection_integrals':
+#                                GaussianProjectionIntegrals(correction_parametrization=None),
+#                            'parametrization':
+#                                PengParametrization()
+#                            },
+#                           {'gaussian_projection_integrals':
+#                                GaussianProjectionIntegrals(correction_parametrization='lobato'),
+#                            'parametrization': LobatoParametrization()
+#                            }
+#                           ], ids=['uncorrected', 'corrected'])
+# def test_gaussian_projection_integrals(parameters):
+#     parametrization = parameters['parametrization']
+#     gaussian_projection_integrals = parameters['gaussian_projection_integrals']
+#
+#     symbol = 'C'
+#     gpts = (256, 256)
+#     sampling = (0.1, 0.1)
+#     positions = np.array([[0, 0, 0]], dtype=np.float32)
+#     a = -np.inf
+#     b = np.inf
+#
+#     gaussian_scattering_factors = gaussian_projection_integrals.build('C', gpts, sampling)
+#
+#     projections = gaussian_scattering_factors.integrate_on_grid(
+#         positions,
+#         a,
+#         b,
+#         gpts,
+#         sampling,
+#         fourier_space=True)
+#
+#     k = np.abs(np.fft.fftfreq(gpts[0], sampling[0])).astype(np.float32)
+#     analytical = parametrization.projected_scattering_factor(symbol)(k ** 2)
+#     assert np.allclose(analytical, projections[0].real, rtol=1e-6)
+#
+#
+# @pytest.mark.parametrize('fourier_space', [True, False])
+# def test_finite_gaussian_projection_integrals(fourier_space):
+#     gaussian_projection_integrals = GaussianProjectionIntegrals(correction_parametrization=None)
+#
+#     symbol = 'C'
+#     gpts = (256, 256)
+#     sampling = (0.02, 0.02)
+#     positions = np.array([[0, 0, 0]], dtype=np.float32)
+#     a = -.2
+#     b = .2
+#
+#     gaussian_scattering_factors = gaussian_projection_integrals.build('C', gpts, sampling)
+#
+#     projections = gaussian_scattering_factors.integrate_on_grid(
+#         positions,
+#         a,
+#         b,
+#         gpts,
+#         sampling,
+#         fourier_space=fourier_space)
+#
+#     if fourier_space:
+#         k = np.abs(np.fft.fftfreq(gpts[0], sampling[0])).astype(np.float32)
+#         analytical = PengParametrization().finite_projected_scattering_factor(symbol)(k, a, b)
+#         assert np.allclose(analytical, projections[0].real, rtol=1e-6)
+#
+#     else:
+#         r = np.linspace(0, gpts[0] * sampling[0], gpts[0], endpoint=False)
+#         analytical = PengParametrization().finite_projected_potential(symbol)(r, a, b)
+#         assert np.allclose(analytical[:len(r) // 2], projections[0][:len(r) // 2], rtol=1e-6, atol=5)
+
+
+# @pytest.mark.parametrize('parametrization',
+#                          [LobatoParametrization(),
+#                           KirklandParametrization()])
+# def test_quadrature(parametrization):
+#     quadrature = QuadratureProjectionIntegrals(parametrization, quad_order=20, cutoff_tolerance=1e-9)
+#
+#     symbol = 'Au'
+#     gpts = (256, 256)
+#     sampling = (0.05, 0.05)
+#     xp = np
+#     a = -20
+#     b = 20
+#
+#     positions = xp.array([[0, 0, 0]], dtype=xp.float32)
+#
+#     table = quadrature.build_integral_table(symbol, min(sampling) / 2)
+#
+#     integrated = table.integrate_on_grid(positions, a, b, gpts, sampling)
+#
+#     r = np.linspace(0, gpts[0] * sampling[0], gpts[0], endpoint=False).astype(np.float32)
+#     analytical = parametrization.projected_potential(symbol)(r[1:])
+#
+#     assert np.allclose(analytical, integrated[0, 1:], atol=2)
+#
+
+# def test_finite_projections():
+#     quadrature = ProjectionQuadratureRule('lobato', quad_order=8, cutoff_tolerance=1e-4)
+#     gaussian_projection_integrals = GaussianProjectionIntegrals()
+#
+#     symbol = 'C'
+#     gpts = (256, 256)
+#     sampling = (0.05, 0.05)
+#     a = .1
+#     b = 1
+#
+#     positions = np.array([[0, 0, 0]], dtype=np.float32)
+#
+#     table = quadrature.build_integral_table(symbol, min(sampling) / 2)
+#
+#     quadrature_potential = table.integrate_on_grid(positions, a, b, gpts, sampling)
+#
+#     gaussian_scattering_factors = gaussian_projection_integrals.build(symbol, gpts, sampling)
+#
+#     gaussian_potential = gaussian_scattering_factors.integrate_on_grid(positions, a, b, gpts, sampling)
+#
+#     assert np.allclose(quadrature_potential[0, :gpts[1] // 2], gaussian_potential[0, :gpts[1] // 2], atol=2)
```

### Comparing `abtem-1.0.4/test/test_copy.py` & `abtem-1.0.5/test/test_copy.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/test/test_ctf.py` & `abtem-1.0.5/test/test_ctf.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/test/test_detect.py` & `abtem-1.0.5/test/test_detect.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,17 @@
     AnnularDetector,
     FlexibleAnnularDetector,
     PixelatedDetector,
 )
 from abtem.waves import Probe
 from utils import gpu
 
-#@reproduce_failure('6.61.0', b'AXicY2AAgwMGDCiA0aIBSAIAF6sBqg==')
-#"@reproduce_failure('6.59.0', b'AXicY2AAgwMGDCiA0aKBiYEBABexAaw=')
+
+# @reproduce_failure('6.61.0', b'AXicY2AAgwMGDCiA0aIBSAIAF6sBqg==')
+# "@reproduce_failure('6.59.0', b'AXicY2AAgwMGDCiA0aKBiYEBABexAaw=')
 @given(data=st.data())
 @pytest.mark.parametrize("lazy", [False, True])
 @pytest.mark.parametrize("device", ["cpu", gpu])
 @pytest.mark.parametrize(
     "detector",
     [
         abtem_st.segmented_detector,
@@ -75,35 +76,52 @@
     elif len(scan_axes) > 1:
         assert type(measurement) == Images
 
     if detector.to_cpu:
         assert measurement.device == "cpu"
 
 
+# @reproduce_failure("6.96.4", b"AXicY2BgZEAHBwyQ2JaMQMA5E8ZnKUBSiKRVAgB64wMe")
+# @reproduce_failure("6.96.4", b"AXicY+BkZEAHBwyQ2JZAgpEZrojx32aEJJJWKwCFMwPm")
+# @reproduce_failure("6.96.4", b"AXicYxBlZEAHBwyQ2MFAgrX9EYzP0t+PkKxBMK0BtY0FYQ==")
 @given(data=st.data())
-@pytest.mark.parametrize("lazy", [False])
-@pytest.mark.parametrize("device", [gpu, "cpu"])
-
+@pytest.mark.parametrize("lazy", [True, False])
+@pytest.mark.parametrize("device", ["cpu", gpu])
 def test_integrate_consistent(data, lazy, device):
     waves = data.draw(abtem_st.waves(lazy=lazy, device=device, min_scan_dims=1))
 
     assume(min(waves.cutoff_angles) > 10.0)
 
+    min_extent = max(waves.angular_sampling)
+    max_extent = np.floor(min(waves.cutoff_angles)) - 1.0
+
+    assume(min_extent < max_extent)
+
     extent = np.floor(
         data.draw(
-            st.floats(min_value=1.0, max_value=np.floor(min(waves.cutoff_angles)) - 1.0)
+            st.floats(
+                min_value=min_extent,
+                max_value=max_extent,
+            )
         )
     )
     inner = np.floor(
         data.draw(st.floats(min_value=0.0, max_value=min(waves.cutoff_angles) - extent))
     )
     outer = inner + extent
 
+    assume(
+        AnnularDetector(inner=inner, outer=outer).get_detector_region(waves).array.sum()
+        > 0
+    )
+
     annular_measurement = AnnularDetector(inner=inner, outer=outer).detect(waves)
-    flexible_measurement = FlexibleAnnularDetector().detect(waves)
+    flexible_measurement = FlexibleAnnularDetector(
+        step_size=1, outer=np.floor(min(waves.cutoff_angles))
+    ).detect(waves)
     pixelated_measurement = PixelatedDetector(max_angle="cutoff").detect(waves)
 
     assert annular_measurement == flexible_measurement.integrate_radial(inner, outer)
     assert annular_measurement == pixelated_measurement.integrate_radial(inner, outer)
 
 
 @given(
@@ -114,23 +132,30 @@
 def test_interpolate_diffraction_patterns(gpts, extent, device):
     probe1 = Probe(
         energy=100e3,
         semiangle_cutoff=30,
         extent=(extent * 2, extent),
         gpts=(gpts * 2, gpts),
         device=device,
-        soft = False
+        soft=False,
     )
     probe2 = Probe(
-        energy=100e3, semiangle_cutoff=30, extent=extent, gpts=gpts, device=device, soft=False
+        energy=100e3,
+        semiangle_cutoff=30,
+        extent=extent,
+        gpts=gpts,
+        device=device,
+        soft=False,
     )
 
     measurement1 = (
         probe1.build(lazy=False)
         .diffraction_patterns(max_angle=None)
         .interpolate("uniform")
         .to_cpu()
     )
 
-    measurement2 = probe2.build(lazy=False).diffraction_patterns(max_angle=None).to_cpu()
+    measurement2 = (
+        probe2.build(lazy=False).diffraction_patterns(max_angle=None).to_cpu()
+    )
 
     assert np.allclose(measurement1.array, measurement2.array)
```

### Comparing `abtem-1.0.4/test/test_ensemble.py` & `abtem-1.0.5/test/test_ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         abtem_st.temporal_envelope,
         abtem_st.spatial_envelope,
         abtem_st.composite_wave_transform,
     ],
 )
 def test_ensembles(data, ensemble):
     ensemble = data.draw(ensemble())
+
     if len(ensemble.ensemble_shape) > 0:
         chunks = data.draw(
             st.integers(min_value=1, max_value=reduce(mul, ensemble.ensemble_shape))
         )
     else:
         chunks = ()
```

### Comparing `abtem-1.0.4/test/test_ewald.py` & `abtem-1.0.5/test/test_ewald.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/test/test_gpaw.py` & `abtem-1.0.5/test/test_gpaw.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/test/test_grid.py` & `abtem-1.0.5/test/test_grid.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/test/test_hyperspy.py` & `abtem-1.0.5/test/test_hyperspy.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/test/test_kirkland.py` & `abtem-1.0.5/test/test_kirkland.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/test/test_measure.py` & `abtem-1.0.5/test/test_measure.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,19 @@
 from abtem.waves import Probe
 from utils import ensure_is_tuple, gpu, array_is_close
 
 
 def test_scanned_measurement_type():
     array = np.zeros((10, 10, 10, 10, 10))
 
-    ensemble_axes_metadata = [ScanAxis(), OrdinalAxis(values=(1,) * 10), ScanAxis()]
+    ensemble_axes_metadata = [
+        ScanAxis(_main=False),
+        OrdinalAxis(values=(1,) * 10),
+        ScanAxis(),
+    ]
     measurement = DiffractionPatterns(
         array,
         sampling=0.1,
         ensemble_axes_metadata=ensemble_axes_metadata,
         metadata={"energy": 100e3},
     )
     assert isinstance(
@@ -185,18 +189,21 @@
 @pytest.mark.parametrize("device", ["cpu", gpu])
 def test_gaussian_filter_images(data, sigma, lazy, device):
     if lazy is True and device == gpu.values[0]:
         return
 
     measurement = data.draw(abtem_st.images(lazy=lazy, device=device))
     assume(all(n > 1 for n in measurement.base_shape))
-    filtered = measurement.gaussian_filter(sigma)
-    filtered.compute()
-    measurement.compute()
-
+    try:
+        filtered = measurement.gaussian_filter(sigma)
+        filtered.compute()
+        measurement.compute()
+    except OSError:
+        pytest.skip("Known CuPy error, but only reproducible in pytest https://github.com/cupy/cupy/issues/8218")
+    
     if np.any(np.array(sigma)) > 1:
         assert not np.allclose(filtered.array, measurement.array)
 
 
 # @given(data=st.data())
 # @pytest.mark.parametrize('lazy', [True, False])
 # @pytest.mark.parametrize('device', ['cpu', gpu])
```

### Comparing `abtem-1.0.4/test/test_potential_parametrization.py` & `abtem-1.0.5/test/test_potential_parametrization.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/test/test_potentials.py` & `abtem-1.0.5/test/test_potentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,19 +77,19 @@
 def test_crystal_potential_with_frozen_phonons(data, potential_unit, tile, num_frozen_phonons, lazy):
     potential_unit = data.draw(potential_unit)
 
     crystal_potential = CrystalPotential(potential_unit, tile, num_frozen_phonons=num_frozen_phonons)
 
     crystal_potential = crystal_potential.build(lazy=lazy)
 
-    assert num_frozen_phonons == crystal_potential.num_frozen_phonons
+    assert num_frozen_phonons == crystal_potential.num_configurations
 
     crystal_potential.compute()
 
-    assert num_frozen_phonons == crystal_potential.num_frozen_phonons
+    assert num_frozen_phonons == crystal_potential.num_configurations
 
 # @given(data=st.data(),
 #        tile=st.tuples(st.integers(min_value=1, max_value=2),
 #                       st.integers(min_value=1, max_value=2),
 #                       st.integers(min_value=1, max_value=2)))
 # @pytest.mark.parametrize('lazy', [True, False])
 # @pytest.mark.parametrize('device', [gpu, 'cpu'])
```

### Comparing `abtem-1.0.4/test/test_prism.py` & `abtem-1.0.5/test/test_prism.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/test/test_scan.py` & `abtem-1.0.5/test/test_scan.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/test/test_simulate.py` & `abtem-1.0.5/test/test_simulate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import hypothesis.strategies as st
 import pytest
-from hypothesis import given
+from hypothesis import given, reproduce_failure
 
 import strategies as abtem_st
 from abtem import PixelatedDetector, AnnularDetector
 from abtem.scan import CustomScan, LineScan, GridScan
 from utils import gpu
 
+
 # @reproduce_failure('6.56.3', b'AXicY2BAAoxwhkUDA2HASppyFBtwMYEAAJNaAXw=')
 @given(data=st.data())
 @pytest.mark.parametrize("lazy", [True], ids=["not_lazy"])
 @pytest.mark.parametrize("device", ["cpu", gpu])
 @pytest.mark.parametrize("ensemble_mean", [True, False])
 @pytest.mark.parametrize(
     "waves_builder",
@@ -99,42 +100,39 @@
 def test_multislice_thickness_series(data, waves_builder, device, lazy):
     waves = data.draw(waves_builder(device=device, allow_distribution=False))
     potential = data.draw(abtem_st.potential(exit_planes=True, ensemble_mean=False))
     exit_waves = waves.multislice(potential, lazy=lazy)
 
     if len(potential.exit_planes) > 1:
         assert exit_waves.shape[1] == len(potential.exit_planes)
-    assert exit_waves.shape[0] == potential.num_frozen_phonons
+    assert exit_waves.shape[0] == potential.num_configurations
     assert exit_waves.gpts == potential.gpts
 
-#@reproduce_failure('6.80.0', b'AXicY2BAAkwwBqNFAwNhwEqacrhqQkwgAACZyAF9')
+
+# @reproduce_failure('6.80.0', b'AXicY2BAAkwwBqNFAwNhwEqacrhqQkwgAACZyAF9')
+# @reproduce_failure("6.96.4", b"AXicY2BAAoxwhkUDA2HASoJyRkIKiNKKnQkEAOBNAX0=")
+# @reproduce_failure("6.96.4", b"AXicY2BAAoxwhkUDA2HASoJyRkIKiNNLwBjsKlE1AQAgawF/")
 @given(data=st.data())
-@pytest.mark.parametrize("lazy", [True, False], ids=["lazy", "not_lazy"])
+@pytest.mark.parametrize("lazy", [True, False])
 @pytest.mark.parametrize("device", ["cpu", gpu])
-@pytest.mark.parametrize("frozen_phonons", [True])
+@pytest.mark.parametrize("frozen_phonons", [True, False])
 @pytest.mark.parametrize(
     "detector",
     [
         abtem_st.segmented_detector,
         abtem_st.flexible_annular_detector,
         abtem_st.pixelated_detector,
         abtem_st.waves_detector,
         abtem_st.annular_detector,
     ],
 )
 @pytest.mark.parametrize(
     "scan",
-    [
-        abtem_st.grid_scan,
-        abtem_st.line_scan,
-        abtem_st.custom_scan
-        #GridScan(),
-        #LineScan(),
-        #CustomScan(),
-    ],
+    [abtem_st.grid_scan, abtem_st.line_scan, abtem_st.custom_scan],
+    # [abtem_st.line_scan],
 )
 @pytest.mark.parametrize(
     "waves_builder",
     [
         abtem_st.probe,
     ],
 )
@@ -142,43 +140,50 @@
     probe = data.draw(waves_builder(allow_distribution=False))
     detector = data.draw(detector())
     scan = data.draw(scan())
 
     potential = data.draw(
         abtem_st.potential(no_frozen_phonons=not frozen_phonons, ensemble_mean=False)
     )
-    #scan.match_probe(probe)
+    # scan.match_probe(probe)
     probe.grid.match(potential)
 
     if isinstance(scan, CustomScan) and isinstance(detector, AnnularDetector):
         return
 
     measurement_shape = detector._out_shape(probe)
     measurement = probe.scan(potential, scan=scan, detectors=detector, lazy=lazy)
 
-    try:
-        assert (
-            measurement.shape
-            == potential.ensemble_shape + scan.ensemble_shape + measurement_shape
+    if isinstance(scan, CustomScan) and scan.shape == (1,):
+        expected_shape = potential.ensemble_shape + measurement_shape
+    else:
+        expected_shape = (
+            potential.ensemble_shape + scan.ensemble_shape + measurement_shape
         )
-    except:
-        print(potential.ensemble_shape, scan.ensemble_shape, measurement_shape)
-        print(measurement.shape)
-        raise
+
+    # print(potential.ensemble_shape, scan.ensemble_shape, measurement_shape)
+    # print(measurement.shape)
+    # try:
+    assert measurement.shape == expected_shape
+    #     )
+    # except:
+    #     print(frozen_phonons)
+    #     print(potential.ensemble_shape, scan.ensemble_shape, measurement_shape)
+    #     print(measurement.shape)
+    #     raise
 
     assert measurement.dtype == detector._out_dtype(probe)
     assert type(measurement) == detector._out_type(probe.build(scan))
 
     if not isinstance(detector, AnnularDetector):
         assert measurement.base_axes_metadata == detector._out_base_axes_metadata(
             probe.build(scan)
         )
 
 
-
 # # @given(data=st.data(),
 # #        gpts=core_st.gpts(min_value=32, max_value=64),
 # #        planewave_cutoff=st.floats(5, 10),
 # #        energy=st.floats(100e3, 200e3))
 # # @pytest.mark.parametrize('lazy', [True, False])
 # # @pytest.mark.parametrize('device', ['cpu', gpu])
 # # @pytest.mark.parametrize('detector', list(all_detectors.keys()))
```

### Comparing `abtem-1.0.4/test/test_structures.py` & `abtem-1.0.5/test/test_structures.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/test/test_temperature.py` & `abtem-1.0.5/test/test_temperature.py`

 * *Files identical despite different names*

### Comparing `abtem-1.0.4/test/test_waves.py` & `abtem-1.0.5/test/test_waves.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 # def test_energy_raises(grid_data, energy, builder):
 #     probe = builder(energy=energy, **grid_data)
 #     assume(energy is None)
 #     with pytest.raises(EnergyUndefinedError):
 #         probe.build()
 
 
-
 @pytest.mark.parametrize(
     "waves_builder", [abtem_st.probe, abtem_st.plane_wave, abtem_st.s_matrix]
 )
 @pytest.mark.parametrize("device", [gpu, "cpu"])
 @pytest.mark.parametrize("lazy", [False, True])
 @given(data=st.data())
 def test_can_build(data, waves_builder, device, lazy):
@@ -180,28 +179,28 @@
     except TypeError:
         waves_builder = data.draw(waves_builder())
 
     waves_builder.grid.match(potential)
 
     waves = waves_builder.build().compute()
 
-    #old_sum = waves.diffraction_patterns(max_angle="full").array.sum()
+    # old_sum = waves.diffraction_patterns(max_angle="full").array.sum()
 
     waves = waves.multislice(potential).compute()
 
     try:
         waves = waves.reduce()
     except AttributeError:
         pass
 
-    #new_sum = waves.diffraction_patterns(max_angle="full").array.sum()
+    # new_sum = waves.diffraction_patterns(max_angle="full").array.sum()
 
-    #print(old_sum, new_sum, old_sum > new_sum, potential.array)
+    # print(old_sum, new_sum, old_sum > new_sum, potential.array)
     # print(waves.diffraction_patterns(max_angle=None).array.sum(axis=(-2, -1)))
-    #
+    
     assert np.all(
         waves.diffraction_patterns(max_angle=None).array.sum(axis=(-2, -1)) < 1.0002
     )
 
 
 @given(data=st.data(), potential=abtem_st.potential())
 @pytest.mark.parametrize("lazy", [True, False])
@@ -224,15 +223,17 @@
 def test_build_then_multislice(data, waves_builder, detectors, potential, lazy):
     waves_builder = data.draw(waves_builder())
     waves_builder.grid.match(potential)
 
     if detectors is not None:
         detectors = data.draw(detectors())
 
-    waves = waves_builder.multislice(potential, detectors=detectors, lazy=lazy).compute()
+    waves = waves_builder.multislice(
+        potential, detectors=detectors, lazy=lazy
+    ).compute()
 
     build_waves = waves_builder.build(lazy=lazy)
     build_waves = build_waves.multislice(potential, detectors=detectors).compute()
 
     assert np.allclose(build_waves.array, waves.array)
 
 
@@ -295,15 +296,15 @@
 
 
 @given(data=st.data())
 @pytest.mark.parametrize("lazy", [True, False])
 @pytest.mark.parametrize("device", ["cpu", gpu])
 def test_images(data, lazy, device):
     waves = data.draw(abtem_st.waves(lazy=lazy, device=device))
-    images = waves.complex_images()
+    images = waves.to_images()
     assert images.shape == waves.shape
     assert images.array.dtype == np.complex64
 
 
 @given(
     data=st.data(),
     max_angle=st.just("valid")
@@ -317,36 +318,41 @@
     probe = data.draw(abtem_st.probe(device=device, allow_distribution=False))
     waves = probe.build(lazy=lazy)
     old_gpts = waves.gpts
     valid_gpts = waves.antialias_valid_gpts
     cutoff_gpts = waves.antialias_cutoff_gpts
     old_max = waves.intensity().array.max(axis=(-2, -1))
 
-    waves = waves.downsample(max_angle=max_angle, normalization=normalization)
+    downsampled_waves = waves.downsample(
+        max_angle=max_angle, normalization=normalization
+    )
 
     if isinstance(max_angle, float):
-        assume(max_angle < 0.8 * max(waves.cutoff_angles))
+        assume(max_angle < 0.8 * max(downsampled_waves.cutoff_angles))
         assume(max_angle > 1.2 * probe.aperture.semiangle_cutoff)
     elif max_angle == "valid":
         assume(
             min(probe.rectangle_cutoff_angles) > 1.1 * probe.aperture.semiangle_cutoff
         )
     elif max_angle == "cutoff":
         assume(min(probe.cutoff_angles) > 1.1 * probe.aperture.semiangle_cutoff)
 
-    assert waves.gpts != old_gpts
-    assert waves.array.dtype == np.complex64
+    assert downsampled_waves.gpts != old_gpts
+    assert downsampled_waves.array.dtype == np.complex64
+
+    assume(downsampled_waves.gpts[0] > 4)
+    assume(downsampled_waves.gpts[1] > 4)
 
     if max_angle == "valid":
-        assert waves.gpts == valid_gpts
+        assert downsampled_waves.gpts == valid_gpts
     elif max_angle == "cutoff":
-        assert waves.gpts == cutoff_gpts
+        assert downsampled_waves.gpts == cutoff_gpts
 
     if normalization == "intensity":
-        assert_is_normalized(waves)
+        assert_is_normalized(downsampled_waves)
     elif normalization == "values":
         np.allclose(old_max, waves.intensity().array.max(axis=(-2, -1)))
 
 
 @given(
     data=st.data(),
     max_angle=st.sampled_from(["cutoff", "valid"]),
@@ -376,17 +382,26 @@
     renormalize=st.booleans(),
 )
 @pytest.mark.parametrize("lazy", [True, False])
 @pytest.mark.parametrize("device", ["cpu", gpu])
 def test_tile(data, repetitions, renormalize, lazy, device):
     waves = data.draw(abtem_st.waves(lazy=lazy, device=device))
     old_extent = waves.extent
-    old_sum = waves.diffraction_patterns(max_angle=None).to_cpu().compute().array.sum((-2,-1))
+    old_sum = (
+        waves.diffraction_patterns(max_angle=None)
+        .to_cpu()
+        .compute()
+        .array.sum((-2, -1))
+    )
     tiled = waves.tile(repetitions, renormalize=renormalize)
 
-
     assert np.allclose(
         (old_extent[0] * repetitions[0], old_extent[1] * repetitions[1]), tiled.extent
     )
     if renormalize:
-        new_sum = tiled.diffraction_patterns(max_angle=None).to_cpu().compute().array.sum((-2, -1))
+        new_sum = (
+            tiled.diffraction_patterns(max_angle=None)
+            .to_cpu()
+            .compute()
+            .array.sum((-2, -1))
+        )
         assert np.allclose(old_sum, new_sum)
```

