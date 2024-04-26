# Comparing `tmp/lips-benchmark-0.2.1.tar.gz` & `tmp/lips-benchmark-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lips-benchmark-0.2.1.tar", last modified: Wed Dec 13 18:44:31 2023, max compression
+gzip compressed data, was "lips-benchmark-0.2.2.tar", last modified: Fri Apr 26 09:33:41 2024, max compression
```

## Comparing `lips-benchmark-0.2.1.tar` & `lips-benchmark-0.2.2.tar`

### file list

```diff
@@ -1,148 +1,152 @@
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.371201 lips-benchmark-0.2.1/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    14980 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/LICENSE
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      252 2023-12-13 18:16:50.000000 lips-benchmark-0.2.1/MANIFEST.in
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    16928 2023-12-13 18:44:31.371201 lips-benchmark-0.2.1/PKG-INFO
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    15944 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/README.md
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.355201 lips-benchmark-0.2.1/configurations/
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.355201 lips-benchmark-0.2.1/configurations/airfoil/
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.359201 lips-benchmark-0.2.1/configurations/airfoil/benchmarks/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      817 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/configurations/airfoil/benchmarks/confAirfoil.ini
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.359201 lips-benchmark-0.2.1/configurations/airfoil/simulators/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      514 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/configurations/airfoil/simulators/tf_fc.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      495 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/configurations/airfoil/simulators/torch_fc.ini
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.359201 lips-benchmark-0.2.1/configurations/pneumatic/
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.359201 lips-benchmark-0.2.1/configurations/pneumatic/benchmarks/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5383 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/configurations/pneumatic/benchmarks/confWheel.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)       84 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/configurations/pneumatic/readme.md
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.359201 lips-benchmark-0.2.1/configurations/pneumatic/simulators/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1959 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/configurations/pneumatic/simulators/torch_fc.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      385 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/configurations/pneumatic/simulators/torch_unet.ini
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.359201 lips-benchmark-0.2.1/configurations/powergrid/
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.367201 lips-benchmark-0.2.1/configurations/powergrid/benchmarks/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)  4397595 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_Neurips.ipynb
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)   563174 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_Sandbox.ipynb
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)   901428 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_WCCI_2022.ipynb
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    11499 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/configurations/powergrid/benchmarks/l2rpn_case14_sandbox.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    14288 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/configurations/powergrid/benchmarks/l2rpn_neurips_2020_track1_small.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13277 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/configurations/powergrid/benchmarks/l2rpn_wcci_2022.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)       96 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/configurations/powergrid/readme.md
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.367201 lips-benchmark-0.2.1/configurations/powergrid/simulators/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      502 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/configurations/powergrid/simulators/tf_fc.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      753 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/configurations/powergrid/simulators/tf_leapnet.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      514 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/configurations/powergrid/simulators/torch_fc.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4294 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/configurations/powergrid/simulators/torch_gnn.ini
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.367201 lips-benchmark-0.2.1/lips/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1099 2023-12-13 18:42:42.000000 lips-benchmark-0.2.1/lips/__init__.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.367201 lips-benchmark-0.2.1/lips/augmented_simulators/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      804 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4454 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/augmented_simulator.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4678 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/hyperParameterTuner.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.367201 lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      724 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/__init__.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.367201 lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/airfoil/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      587 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/airfoil/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4149 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/airfoil/fully_connected.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     7843 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/fully_connected.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.367201 lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/powergrid/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      705 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/powergrid/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3653 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/powergrid/fully_connected.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    12387 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/powergrid/leap_net.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4969 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/powergrid/resnet.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    11374 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/powergrid/utils.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13324 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_simulator.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.367201 lips-benchmark-0.2.1/lips/augmented_simulators/torch_models/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      188 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/torch_models/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    10797 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/torch_models/fully_connected.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    15654 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/torch_models/gnn.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13038 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/torch_models/gnn_powergrid_utils.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    15899 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/torch_models/u_net.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5411 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/torch_models/utils.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    20429 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/augmented_simulators/torch_simulator.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.367201 lips-benchmark-0.2.1/lips/benchmark/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      516 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/benchmark/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13640 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/benchmark/airfransBenchmark.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     7009 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/benchmark/benchmark.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    23120 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/benchmark/powergridBenchmark.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    32452 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/benchmark/wheelBenchmark.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.367201 lips-benchmark-0.2.1/lips/config/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      579 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/config/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5617 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/config/configmanager.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.367201 lips-benchmark-0.2.1/lips/dataset/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      752 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/dataset/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13145 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/dataset/airfransDataSet.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5832 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/dataset/dataSet.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    39804 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/dataset/pneumaticWheelDataSet.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    25768 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/dataset/powergridDataSet.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     6342 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/dataset/sampler.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.371201 lips-benchmark-0.2.1/lips/dataset/scaler/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      259 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/dataset/scaler/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    10324 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/dataset/scaler/powergrid_scaler.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4176 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/dataset/scaler/rolling_scaler.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      419 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/dataset/scaler/scaler.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3412 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/dataset/scaler/standard_scaler.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4404 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/dataset/scaler/standard_scaler_iterative.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     7630 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/dataset/scaler/standard_scaler_per_channel.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.371201 lips-benchmark-0.2.1/lips/dataset/utils/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      453 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/dataset/utils/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    24384 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/dataset/utils/powergrid_utils.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.371201 lips-benchmark-0.2.1/lips/evaluation/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      742 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/evaluation/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    10617 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/evaluation/airfrans_evaluation.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5567 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/evaluation/evaluation.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     8720 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/evaluation/pneumatic_evaluation.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     9953 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/evaluation/powergrid_evaluation.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1713 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/evaluation/utils.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.371201 lips-benchmark-0.2.1/lips/logger/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      522 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/logger/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1497 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/logger/customLogger.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.371201 lips-benchmark-0.2.1/lips/metrics/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      443 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/metrics/__init__.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.371201 lips-benchmark-0.2.1/lips/metrics/ml_metrics/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/metrics/ml_metrics/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      952 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/metrics/ml_metrics/external_metrics.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     2022 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/metrics/ml_metrics/mean_absolute_error.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     2312 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/metrics/ml_metrics/mean_absolute_percentage_error.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     2259 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/metrics/ml_metrics/mean_squared_error.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1737 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/metrics/ml_metrics/metrics.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3124 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/metrics/ml_metrics/normalized_mean_squared_error.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.371201 lips-benchmark-0.2.1/lips/metrics/power_grid/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1231 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/metrics/power_grid/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3512 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/metrics/power_grid/global_conservation.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5147 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/metrics/power_grid/joule_law.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    12945 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/metrics/power_grid/kirchhoff_law.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5784 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/metrics/power_grid/local_conservation.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    11086 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/metrics/power_grid/ohm_law.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13900 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/metrics/power_grid/physics_compliances.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    10297 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/metrics/power_grid/verify_voltage_equality.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.371201 lips-benchmark-0.2.1/lips/physical_simulator/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1092 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/physical_simulator/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     7263 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/physical_simulator/dcApproximationAS.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     8358 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/physical_simulator/getfemSimulator.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    11935 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/physical_simulator/grid2opSimulator.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1934 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/physical_simulator/physicalSimulator.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1912 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/physical_simulator/physicsSolver.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.371201 lips-benchmark-0.2.1/lips/plot/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      453 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/plot/__init__.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.371201 lips-benchmark-0.2.1/lips/plot/power_grid/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      529 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/plot/power_grid/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     2857 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/plot/power_grid/plotting.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.359201 lips-benchmark-0.2.1/lips/tests/
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.359201 lips-benchmark-0.2.1/lips/tests/configs/
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.359201 lips-benchmark-0.2.1/lips/tests/configs/powergrid/
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.371201 lips-benchmark-0.2.1/lips/tests/configs/powergrid/benchmarks/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     7890 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/tests/configs/powergrid/benchmarks/l2rpn_case14_sandbox.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    12948 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/tests/configs/powergrid/benchmarks/l2rpn_neurips_2020_track1_small.ini
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.371201 lips-benchmark-0.2.1/lips/tests/configs/powergrid/simulators/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      502 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/tests/configs/powergrid/simulators/tf_fc.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      753 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/tests/configs/powergrid/simulators/tf_leapnet.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      514 2023-12-12 21:47:49.000000 lips-benchmark-0.2.1/lips/tests/configs/powergrid/simulators/torch_fc.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1395 2023-12-12 21:47:50.000000 lips-benchmark-0.2.1/lips/utils.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-13 18:44:31.371201 lips-benchmark-0.2.1/lips_benchmark.egg-info/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    16928 2023-12-13 18:44:31.000000 lips-benchmark-0.2.1/lips_benchmark.egg-info/PKG-INFO
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4786 2023-12-13 18:44:31.000000 lips-benchmark-0.2.1/lips_benchmark.egg-info/SOURCES.txt
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        1 2023-12-13 18:44:31.000000 lips-benchmark-0.2.1/lips_benchmark.egg-info/dependency_links.txt
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        1 2023-12-12 22:19:39.000000 lips-benchmark-0.2.1/lips_benchmark.egg-info/not-zip-safe
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      812 2023-12-13 18:44:31.000000 lips-benchmark-0.2.1/lips_benchmark.egg-info/requires.txt
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        5 2023-12-13 18:44:31.000000 lips-benchmark-0.2.1/lips_benchmark.egg-info/top_level.txt
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      563 2023-12-13 18:44:31.375201 lips-benchmark-0.2.1/setup.cfg
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3856 2023-12-13 18:16:50.000000 lips-benchmark-0.2.1/setup.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.829346 lips-benchmark-0.2.2/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    14980 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/LICENSE
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      252 2023-12-13 18:16:50.000000 lips-benchmark-0.2.2/MANIFEST.in
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    16928 2024-04-26 09:33:41.829346 lips-benchmark-0.2.2/PKG-INFO
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    15944 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/README.md
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.125360 lips-benchmark-0.2.2/configurations/
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.125360 lips-benchmark-0.2.2/configurations/airfoil/
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.137360 lips-benchmark-0.2.2/configurations/airfoil/benchmarks/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      817 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/configurations/airfoil/benchmarks/confAirfoil.ini
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.137360 lips-benchmark-0.2.2/configurations/airfoil/simulators/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      514 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/configurations/airfoil/simulators/tf_fc.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      495 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/configurations/airfoil/simulators/torch_fc.ini
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.137360 lips-benchmark-0.2.2/configurations/pneumatic/
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.141360 lips-benchmark-0.2.2/configurations/pneumatic/benchmarks/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5383 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/configurations/pneumatic/benchmarks/confWheel.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)       84 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/configurations/pneumatic/readme.md
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.141360 lips-benchmark-0.2.2/configurations/pneumatic/simulators/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1959 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/configurations/pneumatic/simulators/torch_fc.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      385 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/configurations/pneumatic/simulators/torch_unet.ini
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.141360 lips-benchmark-0.2.2/configurations/powergrid/
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.161360 lips-benchmark-0.2.2/configurations/powergrid/benchmarks/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)  4397595 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_Neurips.ipynb
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)   563174 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_Sandbox.ipynb
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)   901428 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_WCCI_2022.ipynb
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     2168 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/configurations/powergrid/benchmarks/fine_tuning.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13713 2024-04-26 09:33:21.000000 lips-benchmark-0.2.2/configurations/powergrid/benchmarks/l2rpn_case14_sandbox.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    15575 2024-04-26 09:33:21.000000 lips-benchmark-0.2.2/configurations/powergrid/benchmarks/l2rpn_idf_2023.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    16794 2024-04-26 09:33:21.000000 lips-benchmark-0.2.2/configurations/powergrid/benchmarks/l2rpn_neurips_2020_track1_small.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13277 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/configurations/powergrid/benchmarks/l2rpn_wcci_2022.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)       96 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/configurations/powergrid/readme.md
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.165360 lips-benchmark-0.2.2/configurations/powergrid/simulators/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      502 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/configurations/powergrid/simulators/tf_fc.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      753 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/configurations/powergrid/simulators/tf_leapnet.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      514 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/configurations/powergrid/simulators/torch_fc.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4294 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/configurations/powergrid/simulators/torch_gnn.ini
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.169359 lips-benchmark-0.2.2/lips/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1099 2024-04-26 09:33:21.000000 lips-benchmark-0.2.2/lips/__init__.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.217358 lips-benchmark-0.2.2/lips/augmented_simulators/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      804 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/augmented_simulators/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4454 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/augmented_simulators/augmented_simulator.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4678 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/augmented_simulators/hyperParameterTuner.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.233358 lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      724 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/__init__.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.245358 lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/airfoil/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      587 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/airfoil/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4149 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/airfoil/fully_connected.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     7947 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/fully_connected.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.293357 lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/powergrid/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      705 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/powergrid/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3653 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/powergrid/fully_connected.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    12493 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/powergrid/leap_net.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5600 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/powergrid/resnet.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    11374 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/powergrid/utils.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13324 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_simulator.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.349356 lips-benchmark-0.2.2/lips/augmented_simulators/torch_models/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      188 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/augmented_simulators/torch_models/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    10903 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/augmented_simulators/torch_models/fully_connected.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    16278 2024-01-04 10:17:47.000000 lips-benchmark-0.2.2/lips/augmented_simulators/torch_models/gnn.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    14260 2024-01-04 10:17:47.000000 lips-benchmark-0.2.2/lips/augmented_simulators/torch_models/gnn_powergrid_utils.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    15899 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/augmented_simulators/torch_models/u_net.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5411 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/augmented_simulators/torch_models/utils.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    20434 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/augmented_simulators/torch_simulator.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.397355 lips-benchmark-0.2.2/lips/benchmark/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      516 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/benchmark/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    14302 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/benchmark/airfransBenchmark.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     7009 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/benchmark/benchmark.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    24021 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/benchmark/powergridBenchmark.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    32452 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/benchmark/wheelBenchmark.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.409355 lips-benchmark-0.2.2/lips/config/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      579 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/config/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5627 2024-01-04 10:17:47.000000 lips-benchmark-0.2.2/lips/config/configmanager.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.469353 lips-benchmark-0.2.2/lips/dataset/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      752 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/dataset/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13145 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/dataset/airfransDataSet.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5881 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/dataset/dataSet.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    39804 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/dataset/pneumaticWheelDataSet.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    29814 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/dataset/powergridDataSet.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     6342 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/dataset/sampler.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.525352 lips-benchmark-0.2.2/lips/dataset/scaler/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      259 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/dataset/scaler/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    10324 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/dataset/scaler/powergrid_scaler.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4176 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/dataset/scaler/rolling_scaler.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      419 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/dataset/scaler/scaler.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3412 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/dataset/scaler/standard_scaler.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4404 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/dataset/scaler/standard_scaler_iterative.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     7630 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/dataset/scaler/standard_scaler_per_channel.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.541352 lips-benchmark-0.2.2/lips/dataset/utils/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      453 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/dataset/utils/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    25342 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/dataset/utils/powergrid_utils.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.597351 lips-benchmark-0.2.2/lips/evaluation/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      742 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/evaluation/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    12403 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/evaluation/airfrans_evaluation.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4968 2024-01-04 10:17:47.000000 lips-benchmark-0.2.2/lips/evaluation/evaluation.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     8952 2024-01-04 10:17:47.000000 lips-benchmark-0.2.2/lips/evaluation/pneumatic_evaluation.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    10018 2024-01-04 10:17:47.000000 lips-benchmark-0.2.2/lips/evaluation/powergrid_evaluation.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1713 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/evaluation/utils.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.609350 lips-benchmark-0.2.2/lips/logger/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      522 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/logger/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1497 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/logger/customLogger.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.613350 lips-benchmark-0.2.2/lips/metrics/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      443 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/metrics/__init__.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.653349 lips-benchmark-0.2.2/lips/metrics/ml_metrics/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/metrics/ml_metrics/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1661 2024-04-26 09:33:21.000000 lips-benchmark-0.2.2/lips/metrics/ml_metrics/external_metrics.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     2022 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/metrics/ml_metrics/mean_absolute_error.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     2312 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/metrics/ml_metrics/mean_absolute_percentage_error.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     2259 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/metrics/ml_metrics/mean_squared_error.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1737 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/metrics/ml_metrics/metrics.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3124 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/metrics/ml_metrics/normalized_mean_squared_error.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.745348 lips-benchmark-0.2.2/lips/metrics/power_grid/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1231 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/metrics/power_grid/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4252 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/metrics/power_grid/compute_solver_time.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3736 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/metrics/power_grid/compute_solver_time_grid2op.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3512 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/metrics/power_grid/global_conservation.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5147 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/metrics/power_grid/joule_law.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    12945 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/metrics/power_grid/kirchhoff_law.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5784 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/metrics/power_grid/local_conservation.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    11086 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/metrics/power_grid/ohm_law.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13878 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/metrics/power_grid/physics_compliances.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    10297 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/metrics/power_grid/verify_voltage_equality.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.797346 lips-benchmark-0.2.2/lips/physical_simulator/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1092 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/physical_simulator/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     7878 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/physical_simulator/dcApproximationAS.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     8358 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/physical_simulator/getfemSimulator.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13657 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/physical_simulator/grid2opSimulator.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1934 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/physical_simulator/physicalSimulator.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1912 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/physical_simulator/physicsSolver.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.801346 lips-benchmark-0.2.2/lips/plot/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      453 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/plot/__init__.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.817346 lips-benchmark-0.2.2/lips/plot/power_grid/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      604 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/plot/power_grid/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     6097 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/lips/plot/power_grid/plotting.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.125360 lips-benchmark-0.2.2/lips/tests/
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.125360 lips-benchmark-0.2.2/lips/tests/configs/
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.125360 lips-benchmark-0.2.2/lips/tests/configs/powergrid/
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.817346 lips-benchmark-0.2.2/lips/tests/configs/powergrid/benchmarks/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    11499 2024-01-04 10:17:47.000000 lips-benchmark-0.2.2/lips/tests/configs/powergrid/benchmarks/l2rpn_case14_sandbox.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    15575 2024-01-04 10:17:47.000000 lips-benchmark-0.2.2/lips/tests/configs/powergrid/benchmarks/l2rpn_neurips_2020_track1_small.ini
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.821346 lips-benchmark-0.2.2/lips/tests/configs/powergrid/simulators/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      502 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/tests/configs/powergrid/simulators/tf_fc.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      753 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/tests/configs/powergrid/simulators/tf_leapnet.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      514 2023-12-12 21:47:49.000000 lips-benchmark-0.2.2/lips/tests/configs/powergrid/simulators/torch_fc.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1395 2023-12-12 21:47:50.000000 lips-benchmark-0.2.2/lips/utils.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-26 09:33:41.829346 lips-benchmark-0.2.2/lips_benchmark.egg-info/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    16928 2024-04-26 09:33:39.000000 lips-benchmark-0.2.2/lips_benchmark.egg-info/PKG-INFO
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4995 2024-04-26 09:33:41.000000 lips-benchmark-0.2.2/lips_benchmark.egg-info/SOURCES.txt
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        1 2024-04-26 09:33:39.000000 lips-benchmark-0.2.2/lips_benchmark.egg-info/dependency_links.txt
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        1 2023-12-12 22:19:39.000000 lips-benchmark-0.2.2/lips_benchmark.egg-info/not-zip-safe
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1133 2024-04-26 09:33:39.000000 lips-benchmark-0.2.2/lips_benchmark.egg-info/requires.txt
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        5 2024-04-26 09:33:39.000000 lips-benchmark-0.2.2/lips_benchmark.egg-info/top_level.txt
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      563 2024-04-26 09:33:41.837346 lips-benchmark-0.2.2/setup.cfg
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4258 2024-04-18 13:19:41.000000 lips-benchmark-0.2.2/setup.py
```

### Comparing `lips-benchmark-0.2.1/LICENSE` & `lips-benchmark-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/PKG-INFO` & `lips-benchmark-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lips-benchmark
-Version: 0.2.1
+Version: 0.2.2
 Summary: LIPS : Learning Industrial Physical Simulation benchmark suite
 Home-page: https://github.com/IRT-SystemX/LIPS
 Author: Milad Leyli-abadi
 Author-email: milad.leyli-abadi@irt-systemx.fr
 License: MPL
 Keywords: Physical system solver,augmented simulator,benchmarking
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lips-benchmark-0.2.1/README.md` & `lips-benchmark-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/configurations/airfoil/benchmarks/confAirfoil.ini` & `lips-benchmark-0.2.2/configurations/airfoil/benchmarks/confAirfoil.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/configurations/airfoil/simulators/tf_fc.ini` & `lips-benchmark-0.2.2/configurations/airfoil/simulators/tf_fc.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/configurations/pneumatic/benchmarks/confWheel.ini` & `lips-benchmark-0.2.2/configurations/pneumatic/benchmarks/confWheel.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/configurations/pneumatic/simulators/torch_fc.ini` & `lips-benchmark-0.2.2/configurations/pneumatic/simulators/torch_fc.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_Neurips.ipynb` & `lips-benchmark-0.2.2/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_Neurips.ipynb`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_Sandbox.ipynb` & `lips-benchmark-0.2.2/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_Sandbox.ipynb`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_WCCI_2022.ipynb` & `lips-benchmark-0.2.2/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_WCCI_2022.ipynb`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/configurations/powergrid/benchmarks/l2rpn_case14_sandbox.ini` & `lips-benchmark-0.2.2/lips/tests/configs/powergrid/benchmarks/l2rpn_case14_sandbox.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/configurations/powergrid/benchmarks/l2rpn_neurips_2020_track1_small.ini` & `lips-benchmark-0.2.2/lips/tests/configs/powergrid/benchmarks/l2rpn_neurips_2020_track1_small.ini`

 * *Files 14% similar despite different names*

```diff
@@ -285,8 +285,44 @@
 	"ML": ["MSE_avg", "MAE_avg", "MAPE_avg", "MAPE_90_avg", "TIME_INF"],
 	"Physics": ["LOSS_POS"],
 	"IndRed": ["TIME_INF"],
 	"OOD": ["MSE_avg", "MAE_avg", "MAPE_avg", "MAPE_90_avg", "TIME_INF"]}
 
 eval_params = {
 	"inf_batch_size": 59000} # #pas_de_temps=100 x #ligne=20 x #topo=7
+	
+[Benchmark4_finetune]
+attr_x = ("prod_p", "load_p")
+attr_tau = ("line_status", "topo_vect")
+attr_y = ("theta_or", "theta_ex", "p_or", "p_ex")
+attr_physics = ("YBus", "SBus", "PV_nodes", "slack")
+dataset_create_params = {
+	"train": {
+		# SCENARIO TOPOLOGY : disconnect or not one line at each tim step
+		"prob_depth": (1.,), # sample from depth 1
+		"prob_type": (0., 1.), # sample only from line disconnection
+		"prob_do_nothing": 0.3,  # probability of do nothing
+		"max_disc": 1}, # authorize at most 1 disconnection
+	"test":{
+		# SCENARIO TOPOLOGY: disconnect one line at each time step
+		"prob_depth": (1.,), # sample from depth 1
+		"prob_type": (0., 1.), # sample only from line disconnection
+		"prob_do_nothing": 0.,  # No do nothing
+		"max_disc": 1}, # authorize at most 1 disconnection
+	"test_ood":{
+		# SCENARIO TOPOLOGY: disconnect two lines at each time step
+		"prob_depth": (0., 1.), # Sample only from depth 2
+		"prob_type": (0., 1.), # sample only from line disconnection
+		"prob_do_nothing": 0.,  # No do nothing
+		"max_disc": 2} # authorize at most 2 disconnection
+	}
+
+eval_dict = {
+	"ML": ["MSE_avg", "MAE_avg", "MAPE_avg", "MAPE_90_avg"],
+	"Physics": [],
+	"IndRed": [],
+	"OOD": []}
+
+eval_params = {
+	"inf_batch_size": 59000} # #pas_de_temps=100 x #ligne=20 x #topo=7
+
```

### Comparing `lips-benchmark-0.2.1/configurations/powergrid/benchmarks/l2rpn_wcci_2022.ini` & `lips-benchmark-0.2.2/configurations/powergrid/benchmarks/l2rpn_wcci_2022.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/configurations/powergrid/simulators/tf_leapnet.ini` & `lips-benchmark-0.2.2/configurations/powergrid/simulators/tf_leapnet.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/configurations/powergrid/simulators/torch_fc.ini` & `lips-benchmark-0.2.2/configurations/powergrid/simulators/torch_fc.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/configurations/powergrid/simulators/torch_gnn.ini` & `lips-benchmark-0.2.2/configurations/powergrid/simulators/torch_gnn.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/__init__.py` & `lips-benchmark-0.2.2/lips/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public License, version 2.0.
 # If a copy of the Mozilla Public License, version 2.0 was not distributed with this file,
 # you can obtain one at http://mozilla.org/MPL/2.0/.
 # SPDX-License-Identifier: MPL-2.0
 # This file is part of LIPS, LIPS is a python platform for power networks benchmarking
 import pathlib
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 here = pathlib.Path(__file__).parent.resolve()
 
 def get_version(rel_path="__init__.py"):
     init_content = (here / rel_path).read_text(encoding='utf-8')
     for line in init_content.split('\n'):
         if line.startswith('__version__'):
```

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/__init__.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/augmented_simulator.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/augmented_simulator.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/hyperParameterTuner.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/hyperParameterTuner.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/__init__.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/airfoil/__init__.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/airfoil/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/airfoil/fully_connected.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/airfoil/fully_connected.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/fully_connected.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/fully_connected.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,27 +50,29 @@
     RuntimeError
         _description_
     """
     def __init__(self,
                  sim_config_path: str,
                  bench_config_path: Union[str, pathlib.Path],
                  bench_config_name: Union[str, None]=None,
+                 bench_kwargs: dict={},
                  sim_config_name: Union[str, None]=None,
                  name: Union[str, None]=None,
                  scaler: Union[Scaler, None]=None,
                  log_path: Union[None, str]=None,
                  **kwargs):
         super().__init__(name=name, log_path=log_path, **kwargs)
         if not os.path.exists(sim_config_path):
             raise RuntimeError("Configuration path for the simulator not found!")
         if not str(sim_config_path).endswith(".ini"):
             raise RuntimeError("The configuration file should have `.ini` extension!")
         sim_config_name = sim_config_name if sim_config_name is not None else "DEFAULT"
         self.sim_config = ConfigManager(section_name=sim_config_name, path=sim_config_path)
         self.bench_config = ConfigManager(section_name=bench_config_name, path=bench_config_path)
+        self.bench_config.set_options_from_dict(**bench_kwargs)
         self.name = name if name is not None else self.sim_config.get_option("name")
         self.name = self.name + '_' + sim_config_name
         # scaler
         self.scaler = scaler() if scaler else None
         # Logger
         self.log_path = log_path
         self.logger = CustomLogger(__class__.__name__, log_path).logger
```

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/powergrid/__init__.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/powergrid/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/powergrid/fully_connected.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/powergrid/fully_connected.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/powergrid/leap_net.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/powergrid/leap_net.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,27 +69,29 @@
         _description_
     """
     def __init__(self,
                  sim_config_path: str,
                  bench_config_path: Union[str, pathlib.Path],
                  sim_config_name: Union[str, None]=None,
                  bench_config_name: Union[str, None]=None,
+                 bench_kwargs: dict = {},
                  name: Union[str, None]=None,
                  scaler: Union[Scaler, None]=None,
                  log_path: Union[None, str]=None,
                  **kwargs):
 
         super().__init__(name=name, log_path=log_path, **kwargs)
         if not os.path.exists(sim_config_path):
             raise RuntimeError("Configuration path for the simulator not found!")
         if not str(sim_config_path).endswith(".ini"):
             raise RuntimeError("The configuration file should have `.ini` extension!")
         sim_config_name = sim_config_name if sim_config_name is not None else "DEFAULT"
         self.sim_config = ConfigManager(section_name=sim_config_name, path=sim_config_path)
         self.bench_config = ConfigManager(section_name=bench_config_name, path=bench_config_path)
+        self.bench_config.set_options_from_dict(**bench_kwargs)
         self.name = name if name is not None else self.sim_config.get_option("name")
         self.name = name + '_' + sim_config_name
         # scaler
         self.scaler = scaler() if scaler else None
         # Logger
         self.log_path = log_path
         self.logger = CustomLogger(__class__.__name__, log_path).logger
```

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/powergrid/resnet.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/powergrid/resnet.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         # Define layer to be used for the model
         self.layers = {"resnet": ResNetLayer}
         self.layer = self.layers[self.params["layer"]]
+        self._topo_vect_transformer = None
 
     def build_model(self):
         """Build the model
         Returns
         -------
         Model
             _description_
@@ -73,14 +74,22 @@
             x = keras.layers.Activation(self.params["activation"], name=f"activation_{layer_id}")(x)
             x = keras.layers.Dropout(rate=self.params["dropout"], name=f"dropout_{layer_id}")(x)
         output_ = keras.layers.Dense(self.output_size)(x)
         self._model = keras.Model(inputs=input_,
                                   outputs=output_,
                                   name=f"{self.name}_model")
         return self._model
+    
+    def init_topo_vect_transformer(self, dataset: DataSet):
+        """Initialize the topo_vect_transformer using the training dataset
+
+        Args:
+            dataset (DataSet): _description_
+        """
+        self._topo_vect_transformer = TopoVectTransformation(self.bench_config, self.params, dataset)
 
     def process_dataset(self, dataset: DataSet, training: bool = False) -> tuple:
         """process the datasets for training and evaluation
 
         This function transforms all the dataset into something that can be used by the neural network (for example)
 
         Warning
@@ -103,15 +112,20 @@
         """
 
         # extract inputs, line_status, outputs without concatenation
         (inputs, extract_tau), outputs = dataset.extract_data(concat=False)
         line_status = extract_tau[0]
 
         if training:
-            self._topo_vect_transformer = TopoVectTransformation(self.bench_config, self.params, dataset)
+            self.init_topo_vect_transformer(dataset)
+            #self._topo_vect_transformer = TopoVectTransformation(self.bench_config, self.params, dataset)
+        else:
+            if self._topo_vect_transformer is None:
+                raise RuntimeError(f"If you load a pretrained model, you should first call the `init_topo_vect_transformer` function on training data!")
+
         # extract tau using LeapNetProxy function
         extract_tau = self._topo_vect_transformer.transform_topo_vect(dataset)
 
         # add tau and line_status to inputs
         inputs.extend([extract_tau, line_status])
 
         # concatenate input features
```

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_models/powergrid/utils.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_models/powergrid/utils.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/tensorflow_simulator.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/tensorflow_simulator.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/torch_models/fully_connected.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/torch_models/fully_connected.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,26 +49,28 @@
         You should provide a path to the configuration file for this augmented simulator
     """
     def __init__(self,
                  sim_config_path: Union[pathlib.Path, str],
                  bench_config_path: Union[str, pathlib.Path],
                  sim_config_name: Union[str, None]=None,
                  bench_config_name: Union[str, None]=None,
+                 bench_kwargs: dict = {},
                  name: Union[str, None]=None,
                  scaler: Union[Scaler, None]=None,
                  log_path: Union[None, pathlib.Path, str]=None,
                  **kwargs):
         super().__init__()
         if not os.path.exists(sim_config_path):
             raise RuntimeError("Configuration path for the simulator not found!")
         if not str(sim_config_path).endswith(".ini"):
             raise RuntimeError("The configuration file should have `.ini` extension!")
         sim_config_name = sim_config_name if sim_config_name is not None else "DEFAULT"
         self.sim_config = ConfigManager(section_name=sim_config_name, path=sim_config_path)
         self.bench_config = ConfigManager(section_name=bench_config_name, path=bench_config_path)
+        self.bench_config.set_options_from_dict(**bench_kwargs)
         self.name = name if name is not None else self.sim_config.get_option("name")
         # scaler
         self.scaler = scaler
         # Logger
         self.log_path = log_path
         self.logger = CustomLogger(__class__.__name__, log_path).logger
         # model parameters
```

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/torch_models/gnn.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/torch_models/gnn.py`

 * *Files 13% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         # Logger
         self.log_path = log_path
         self.logger = CustomLogger(__class__.__name__, log_path).logger
         # model parameters
         self.params = self.sim_config.get_options_dict()
         self.params.update(kwargs)
 
+        # TODO: verify that these parameters exist in config file
         self.encoder_sizes = self.params["encoder_sizes"]
         self.hidden_sizes = self.params["hidden_sizes"]
         self.decoder_sizes = self.params["decoder_sizes"]
 
         self.activation = {
             "relu": F.relu,
             "sigmoid": F.sigmoid,
@@ -100,19 +101,15 @@
             "PNA": pyg_nn.PNAConv
         }
         self.edge_dim = self.params["conv_layer_params"].get("edge_dim", None)
         self.consider_edge_weights = False if self.params["consider_edge_weights"] is False else True
         self.device = "cpu" if self.params.get("device") is None else self.params["device"]
 
         self.input_size = None if self.params.get("input_size") is None else self.params["input_size"]
-        self.output_size = None if self.params.get("output_size") is None else self.params["output_size"]
-        #TODO: Raise error if the following params keys could not be found
-        self.encoder_sizes = self.params["encoder_sizes"]
-        self.hidden_sizes = self.params["hidden_sizes"]
-        self.decoder_sizes = self.params["decoder_sizes"]
+        self.output_size = None if self.params.get("output_size") is None else self.params["output_size"]        
 
         self.input_layer = None
         self.encoder_layers = None
         self.conv_layers = None
         self.decoder_layers = None
         self.output_layer = None
 
@@ -201,39 +198,51 @@
             _description_, by default False
 
         Returns
         -------
         DataLoader
             _description_
         """
-        obs = self._get_obs()
-        if training:
+        load_from_file = kwargs.get("load_from_file", None)
+        if load_from_file is not None:
+            loader_name = dataset.name + "_loader.pth"
+            load_from_file = pathlib.Path(load_from_file)
+            path_to_loader = load_from_file / loader_name
+            if not path_to_loader.exists():
+                raise RuntimeError("Data loader path not found for the benchmark!")
             self._infer_size(dataset)
-            batch_size = self.params["train_batch_size"]
-            features, targets, edge_indices, edge_weights = prepare_dataset(obs, dataset.data, return_edge_weights=self.consider_edge_weights)
-            #extract_x, extract_y = dataset.extract_data()
-            #TODO: adapt the normalization for GNN
-            # if self.scaler is not None:
-            #     extract_x, extract_y = self.scaler.fit_transform(extract_x, extract_y)
-        else:
-            batch_size = self.params["eval_batch_size"]
-            #extract_x, extract_y = dataset.extract_data()
-            features, targets, edge_indices, edge_weights = prepare_dataset(obs, dataset.data, return_edge_weights=self.consider_edge_weights)
-            # if self.scaler is not None:
-            #     extract_x, extract_y = self.scaler.transform(extract_x, extract_y)
-
-        data_loader = get_batches_pyg(edge_indices=edge_indices,
-                                      features=features,
-                                      targets=targets,
-                                      edge_weights=edge_weights,
-                                      batch_size=batch_size,
-                                      #ybus=dataset.data["YBus"],
-                                      #line_status=dataset.data["line_status"],
-                                      #topo_vect=dataset.data["topo_vect"],
-                                      device=self.device)
+            data_loader = torch.load(path_to_loader)
+        else:
+            print("processing the dataset: ", dataset.name)
+            obs = self._get_obs()
+            device = kwargs.get("device", self.device)
+            if training:
+                self._infer_size(dataset)
+                batch_size = self.params["train_batch_size"]
+                features, targets, edge_indices, edge_weights = prepare_dataset(obs, dataset.data, return_edge_weights=self.consider_edge_weights)
+                #extract_x, extract_y = dataset.extract_data()
+                #TODO: adapt the normalization for GNN
+                # if self.scaler is not None:
+                #     extract_x, extract_y = self.scaler.fit_transform(extract_x, extract_y)
+            else:
+                batch_size = self.params["eval_batch_size"]
+                #extract_x, extract_y = dataset.extract_data()
+                features, targets, edge_indices, edge_weights = prepare_dataset(obs, dataset.data, return_edge_weights=self.consider_edge_weights)
+                # if self.scaler is not None:
+                #     extract_x, extract_y = self.scaler.transform(extract_x, extract_y)
+
+            data_loader = get_batches_pyg(edge_indices=edge_indices,
+                                        features=features,
+                                        targets=targets,
+                                        edge_weights=edge_weights,
+                                        batch_size=batch_size,
+                                        #ybus=dataset.data["YBus"],
+                                        #line_status=dataset.data["line_status"],
+                                        #topo_vect=dataset.data["topo_vect"],
+                                        device=device)
         #data_loader = DataLoader(torch_dataset, batch_size=batch_size, shuffle=self.params["shuffle"])
         return data_loader
     
     # def _post_process_inplace(self, predictions):
     #     """
     #     Post process if the conversion of theta_bus to active powers should happen here
 
@@ -282,17 +291,19 @@
         dataset : DataSet
             An object of the `DataSet` class 
         data : npt.NDArray[np.float64]
             the data which should be reconstructed to the desired form
         """
         outputs = []
         obs = self._get_obs()
-        p_ors_pred, p_exs_pred = get_all_active_powers(dataset.data, obs, theta_bus=data.reshape(-1, obs.n_sub))
-        outputs.append(dataset.data["theta_or"])
-        outputs.append(dataset.data["theta_ex"])
+        theta_bus = data.reshape(-1, obs.n_sub)
+        p_ors_pred, p_exs_pred = get_all_active_powers(dataset, obs, theta_bus=theta_bus)
+        theta_ors_pred, theta_exs_pred = reconstruct_theta_line(dataset, obs, theta_sub=theta_bus)
+        outputs.append(theta_ors_pred)
+        outputs.append(theta_exs_pred)
         outputs.append(p_ors_pred)
         outputs.append(p_exs_pred)
         outputs = np.hstack(outputs)
         outputs = dataset.reconstruct_output(outputs)
         return outputs
```

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/torch_models/gnn_powergrid_utils.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/torch_models/gnn_powergrid_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -327,28 +327,28 @@
     Returns
     -------
     _type_
         _description_
     """
     lor_bus, lor_conn = obs._get_bus_id(obs.line_or_pos_topo_vect, obs.line_or_to_subid)
     lex_bus, lex_conn = obs._get_bus_id(obs.line_ex_pos_topo_vect, obs.line_ex_to_subid)
-    index_array = np.vstack((np.arange(obs.n_line), lor_bus, lex_bus)).T 
+    index_array = np.vstack((np.arange(obs.n_line), lor_bus, lex_bus)).T
     # Create the adjacency matrix (MxN) M: branches and N: Nodes
     A_or = np.zeros((obs.n_line, obs.n_sub))
     A_ex = np.zeros((obs.n_line, obs.n_sub))
 
     for line in index_array[:,0]:
         if index_array[line,1] != -1:
             A_or[line, index_array[line,1]] = 1
             A_or[line, index_array[line,2]] = -1
             A_ex[line, index_array[line,1]] = -1
-            A_ex[line, index_array[line,2]] = 1        
+            A_ex[line, index_array[line,2]] = 1
     
     # Create the diagonal matrix D (MxM)
-    Ybus = dataset["YBus"][index][:14,:14]
+    Ybus = dataset["YBus"][index][:obs.n_sub,:obs.n_sub]
     D = np.zeros((obs.n_line, obs.n_line), dtype=complex)
     for line in index_array[:, 0]:
         bus_from = index_array[line, 1]
         bus_to = index_array[line, 2]
         D[line,line] = Ybus[bus_from, bus_to] * (-1)
 
     # Create the theta vector ((M-1)x1)
@@ -372,19 +372,54 @@
         _description_
 
     Returns
     -------
     _type_
         _description_
     """
-    data_size = len(dataset["p_or"])
-    p_or = np.zeros_like(dataset["p_or"])
-    p_ex = np.zeros_like(dataset["p_ex"])
+    data = dataset.data
+    p_or = np.zeros_like(data["p_or"])
+    p_ex = np.zeros_like(data["p_ex"])
 
     #theta_bus = get_theta_bus(dataset, obs)
-    for ind in range(data_size):
-        obs = create_fake_obs(obs, dataset, ind)
-        p_or_computed, p_ex_computed = get_active_power(dataset, obs, theta_bus, index=ind)
+    for ind in range(dataset.size):
+        obs = create_fake_obs(obs, data, ind)
+        p_or_computed, p_ex_computed = get_active_power(data, obs, theta_bus, index=ind)
         p_or[ind, :] = p_or_computed.flatten()
         p_ex[ind, :] = p_ex_computed.flatten()
 
     return p_or, p_ex
+
+def reconstruct_theta_line(dataset, obs, theta_sub) -> tuple:
+    """Reconstruct the voltage angles through lines from thetas on subs
+
+    Parameters
+    ----------
+    dataset : _type_
+        _description_
+    obs : _type_
+        _description_
+    theta_sub : _type_
+        _description_
+
+    Returns
+    -------
+    tuple
+        theta_or: voltage angle at the origin side of the power line
+        theta_ex: voltage angle at the extrem side of the power line
+    """
+    data = dataset.data
+    theta_or = np.zeros_like(data["theta_or"])
+    theta_ex = np.zeros_like(data["theta_ex"])
+
+    for idx in range(dataset.size):
+        obs.line_status = data["line_status"][idx]
+        obs.topo_vect = data["topo_vect"][idx]
+        lor_bus, _ = obs._get_bus_id(obs.line_or_pos_topo_vect, obs.line_or_to_subid)
+        lex_bus, _ = obs._get_bus_id(obs.line_ex_pos_topo_vect, obs.line_ex_to_subid)
+        index_array = np.vstack((np.arange(obs.n_line), lor_bus, lex_bus)).T
+
+        for line in range(obs.n_line):
+            if index_array[line, 1] != -1:
+                theta_or[idx][line] = theta_sub[idx][index_array[line, 1]]
+                theta_ex[idx][line] = theta_sub[idx][index_array[line, 2]]
+    return theta_or, theta_ex
```

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/torch_models/u_net.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/torch_models/u_net.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/torch_models/utils.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/torch_models/utils.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/augmented_simulators/torch_simulator.py` & `lips-benchmark-0.2.2/lips/augmented_simulators/torch_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,33 +432,33 @@
         # load scaler parameters
         if self.scaler is not None:
             self.scaler.load(path)
         self._load_losses(path)
         with open((path / "config.json"), "r", encoding="utf-8") as f:
             res_json = json.load(fp=f)
         self.params.update(res_json)
-        self.device = torch.device(self.params["device"])
+        #self.device = torch.device(self.params["device"])
         return self.params
 
     def _load_model(self, epoch, path: str):
         epoch = str(epoch) if epoch is not None else "_last"
         nm_file = "model" + epoch + ".pt"
         path_weights = path / nm_file
         if not path_weights.exists():
             raise FileNotFoundError(f"Weights file {path_weights} not found")
         self._model._load_metadata(path)
         self.build_model()
-        self._model.to(self.params["device"])
+        self._model.to(self.device)
         # load the weights
         with tempfile.TemporaryDirectory() as path_tmp:
             nm_tmp = os.path.join(path_tmp, nm_file)
             # copy the weights into this file
             shutil.copy(path_weights, nm_tmp)
             # load this copy (make sure the proper file is not corrupted even if the loading fails)
-            self._model.load_state_dict(torch.load(nm_tmp))
+            self._model.load_state_dict(torch.load(nm_tmp), strict=False)
 
     def _save_losses(self, path: Union[str, pathlib.Path]):
         """
         save the losses
         """
         if not isinstance(path, pathlib.Path):
             path = pathlib.Path(path)
```

### Comparing `lips-benchmark-0.2.1/lips/benchmark/__init__.py` & `lips-benchmark-0.2.2/lips/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/benchmark/airfransBenchmark.py` & `lips-benchmark-0.2.2/lips/benchmark/airfransBenchmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 import numpy as np
 
 from lips.benchmark import Benchmark
 from lips.augmented_simulators import AugmentedSimulator
 from lips.dataset.airfransDataSet import AirfRANSDataSet,extract_dataset_by_simulations
 from lips.evaluation.airfrans_evaluation import AirfRANSEvaluation
+from lips.dataset.scaler.standard_scaler_iterative import iterative_fit
 from lips.utils import NpEncoder
 
 def reynolds_filter(dataset):
     simulation_names=dataset.extra_data["simulation_names"]
     reynolds=np.array([float(name.split('_')[2])/1.56e-5 for name,numID in simulation_names])
     simulation_indices=np.where((reynolds>3e6) & (reynolds<5e6))[0]
     return simulation_indices
@@ -104,14 +105,15 @@
         self._test_ood_dataset = AirfRANSDataSet(name = "test_ood",
                                              config = self.config,
                                              attr_names = attr_names,
                                              task = 'reynolds',
                                              split = "testing",
                                              log_path = log_path
                                             )
+        self.ml_normalization = dict()
 
 
     def load(self,path):
         """
         load the already generated datasets
         """
         if self.is_loaded:
@@ -160,14 +162,22 @@
         Raises
         ------
         RuntimeError
             Unknown dataset selected
 
         """
         self.augmented_simulator = augmented_simulator
+
+        field_names = self.train_dataset._attr_y
+        chunk_sizes = [int(simulation[1]) for simulation in self.train_dataset.extra_data["simulation_names"]]
+        flattened_train = np.concatenate([self.train_dataset.data[field_name][:, None] for field_name in field_names], axis = 1)
+        mean_observ,std_observ = iterative_fit(flattened_train,chunk_sizes)
+        self.ml_normalization["mean"] = mean_observ
+        self.ml_normalization["std"] = std_observ
+
         if dataset == "all":
             li_dataset = [self._test_dataset, self._test_ood_dataset]
             keys = ["test", "test_ood"]
         elif dataset == "test":
             li_dataset = [self._test_dataset]
             keys = ["test"]
         elif dataset == "test_ood":
@@ -224,17 +234,19 @@
                                                                             )
 
         begin_ = time.perf_counter()
         predictions = self.augmented_simulator.predict(dataset, **kwargs)
         end_ = time.perf_counter()
         self.augmented_simulator.predict_time = end_ - begin_
         observation_metadata = dataset.extra_data
+
         res = self.evaluation.evaluate(observations=dataset.data,
                                        predictions=predictions,
-                                       observation_metadata=observation_metadata
+                                       observation_metadata=observation_metadata,
+                                       ml_normalization = self.ml_normalization
                                        )
         if save_path:
             if not isinstance(save_path, pathlib.Path):
                 save_path = pathlib.Path(save_path)
             save_path = save_path / augmented_simulator.name / dataset.name
             if save_path.exists():
                 self.logger.warning("Deleting path %s that might contain previous runs", save_path)
```

### Comparing `lips-benchmark-0.2.1/lips/benchmark/benchmark.py` & `lips-benchmark-0.2.2/lips/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/benchmark/powergridBenchmark.py` & `lips-benchmark-0.2.2/lips/benchmark/powergridBenchmark.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-"""
-Licence:
-    Copyright (c) 2021, IRT SystemX (https://www.irt-systemx.fr/en/)
-    See AUTHORS.txt
-    This Source Code Form is subject to the terms of the Mozilla Public License, version 2.0.
-    If a copy of the Mozilla Public License, version 2.0 was not distributed with this file,
-    you can obtain one at http://mozilla.org/MPL/2.0/.
-    SPDX-License-Identifier: MPL-2.0
-    This file is part of LIPS, LIPS is a python platform for power networks benchmarking
-
-"""
+# Copyright (c) 2021, IRT SystemX (https://www.irt-systemx.fr/en/)
+# See AUTHORS.txt
+# This Source Code Form is subject to the terms of the Mozilla Public License, version 2.0.
+# If a copy of the Mozilla Public License, version 2.0 was not distributed with this file,
+# you can obtain one at http://mozilla.org/MPL/2.0/.
+# SPDX-License-Identifier: MPL-2.0
+# This file is part of LIPS, LIPS is a python platform for power networks benchmarking
 
 import os
 import shutil
 import warnings
 import copy
 import json
 import time
@@ -29,16 +25,14 @@
 from ..physical_simulator.dcApproximationAS import DCApproximationAS
 from ..dataset.powergridDataSet import PowerGridDataSet
 from ..dataset.utils.powergrid_utils import get_kwargs_simulator_scenario
 from ..dataset.utils.powergrid_utils import XDepthAgent, get_action_list
 from ..evaluation.powergrid_evaluation import PowerGridEvaluation
 from ..utils import NpEncoder
 
-
-
 class PowerGridBenchmark(Benchmark):
     """PowerGrid Benchmark class
 
     This class allows to benchmark a power grid scenario which are defined in a config file.
 
     Parameters
     ----------
@@ -65,14 +59,15 @@
     can extend this class.
     """
     def __init__(self,
                  benchmark_path: Union[pathlib.Path, str, None],
                  config_path: Union[pathlib.Path, str],
                  benchmark_name: str="Benchmark1",
                  load_data_set: bool=False,
+                 load_ybus_as_sparse: bool=False,
                  evaluation: Union[PowerGridEvaluation, None]=None,
                  log_path: Union[pathlib.Path, str, None]=None,
                  **kwargs
                  ):
         super().__init__(benchmark_name=benchmark_name,
                          benchmark_path=benchmark_path,
                          config_path=config_path,
@@ -109,17 +104,25 @@
         self.val_actor_seed = kwargs.get("val_actor_seed") if "val_actor_seed" in kwargs else self.config.get_option("benchmark_seeds").get("val_actor_seed", 5)
         self.test_actor_seed = kwargs.get("test_actor_seed") if "test_actor_seed" in kwargs else self.config.get_option("benchmark_seeds").get("test_actor_seed", 6)
         self.test_ood_topo_actor_seed = kwargs.get("test_ood_topo_actor_seed") if "test_ood_topo_actor_seed" in kwargs else self.config.get_option("benchmark_seeds").get("test_ood_topo_actor_seed", 7)
 
         self.initial_chronics_id = kwargs.get("initial_chronics_id") if "initial_chronics_id" in kwargs else self.config.get_option("benchmark_seeds").get("initial_chronics_id", 0)
 
         # concatenate all the variables for data generation
-        attr_names = self.config.get_option("attr_x") + \
-                     self.config.get_option("attr_tau") + \
-                     self.config.get_option("attr_y")
+        attr_names = ()
+        if self.config.get_option("attr_x") is not None:
+            attr_names += self.config.get_option("attr_x")
+        if self.config.get_option("attr_tau") is not None:
+            attr_names += self.config.get_option("attr_tau")
+        if self.config.get_option("attr_y") is not None:
+            attr_names += self.config.get_option("attr_y")
+        
+        # attr_names = self.config.get_option("attr_x") + \
+        #              self.config.get_option("attr_tau") + \
+        #              self.config.get_option("attr_y")
 
         self.train_dataset = PowerGridDataSet(name="train",
                                               attr_names=attr_names,
                                               config=self.config,
                                               log_path=log_path
                                               )
 
@@ -138,35 +141,36 @@
         self._test_ood_topo_dataset = PowerGridDataSet(name="test_ood_topo",
                                                        attr_names=attr_names,
                                                        config=self.config,
                                                        log_path=log_path
                                                        )
 
         if load_data_set:
-            self.load()
+            self.load(load_ybus_as_sparse)
 
-    def load(self):
+    def load(self, load_ybus_as_sparse: bool = False):
         """
         load the already generated datasets
         """
         if self.is_loaded:
             #print("Previously saved data will be freed and new data will be reloaded")
             self.logger.info("Previously saved data will be freed and new data will be reloaded")
         if not os.path.exists(self.path_datasets):
             raise RuntimeError(f"No data are found in {self.path_datasets}. Have you generated or downloaded "
                                f"some data ?")
-        self.train_dataset.load(path=self.path_datasets)
-        self.val_dataset.load(path=self.path_datasets)
-        self._test_dataset.load(path=self.path_datasets)
-        self._test_ood_topo_dataset.load(path=self.path_datasets)
+        self.train_dataset.load(path=self.path_datasets, load_ybus_as_sparse=load_ybus_as_sparse)
+        self.val_dataset.load(path=self.path_datasets, load_ybus_as_sparse=load_ybus_as_sparse)
+        self._test_dataset.load(path=self.path_datasets, load_ybus_as_sparse=load_ybus_as_sparse)
+        self._test_ood_topo_dataset.load(path=self.path_datasets, load_ybus_as_sparse=load_ybus_as_sparse)
         self.is_loaded = True
 
     def generate(self, nb_sample_train: int, nb_sample_val: int,
-                 nb_sample_test: int, nb_sample_test_ood_topo: int, 
-                 do_store_physics: bool=False, is_dc: bool=False):
+                 nb_sample_test: int, nb_sample_test_ood_topo: int,
+                 do_store_physics: bool=False, is_dc: bool=False,
+                 store_as_sparse: bool=False):
         """
         generate the different datasets required for the benchmark
         """
         if self.path_datasets is not None:
             if self.is_loaded:
                 self.logger.warning("Previously saved data will be erased by this new generation")
             if os.path.exists(self.path_datasets):
@@ -188,39 +192,43 @@
 
         self.train_dataset.generate(simulator=self.training_simulator,
                                     actor=self.training_actor,
                                     path_out=self.path_datasets,
                                     nb_samples=nb_sample_train,
                                     nb_samples_per_chronic=self.config.get_option("samples_per_chronic").get("train", 864),
                                     do_store_physics=do_store_physics,
-                                    is_dc=is_dc
+                                    is_dc=is_dc,
+                                    store_as_sparse=store_as_sparse
                                     )
         self.val_dataset.generate(simulator=self.val_simulator,
                                   actor=self.val_actor,
                                   path_out=self.path_datasets,
                                   nb_samples=nb_sample_val,
                                   nb_samples_per_chronic=self.config.get_option("samples_per_chronic").get("val", 288),
                                   do_store_physics=do_store_physics,
-                                  is_dc=is_dc
+                                  is_dc=is_dc,
+                                  store_as_sparse=store_as_sparse
                                   )
         self._test_dataset.generate(simulator=self.test_simulator,
                                     actor=self.test_actor,
                                     path_out=self.path_datasets,
                                     nb_samples=nb_sample_test,
                                     nb_samples_per_chronic=self.config.get_option("samples_per_chronic").get("test", 288),
                                     do_store_physics=do_store_physics,
-                                    is_dc=is_dc
+                                    is_dc=is_dc,
+                                    store_as_sparse=store_as_sparse
                                     )
         self._test_ood_topo_dataset.generate(simulator=self.test_ood_topo_simulator,
                                              actor=self.test_ood_topo_actor,
                                              path_out=self.path_datasets,
                                              nb_samples=nb_sample_test_ood_topo,
                                              nb_samples_per_chronic=self.config.get_option("samples_per_chronic").get("test_ood", 288),
                                              do_store_physics=do_store_physics,
-                                             is_dc=is_dc
+                                             is_dc=is_dc,
+                                             store_as_sparse=store_as_sparse
                                              )
 
     def evaluate_simulator(self,
                            dataset: str = "all",
                            augmented_simulator: Union[PhysicalSimulator, AugmentedSimulator, None] = None,
                            save_path: Union[str, None]=None,
                            save_predictions: bool=False,
@@ -396,33 +404,33 @@
         self.test_ood_topo_simulator = Grid2opSimulator(get_kwargs_simulator_scenario(self.config),
                                                         initial_chronics_id=self.initial_chronics_id,
                                                         chronics_selected_regex=self.config.get_option("chronics").get("test_ood")
                                                         )
         self.test_ood_topo_simulator.seed(self.test_ood_topo_env_seed)
 
         all_topo_actions = get_action_list(self.env.action_space)
-        self.training_actor = XDepthAgent(self.env.action_space,
+        self.training_actor = XDepthAgent(self.env,
                                           all_topo_actions=all_topo_actions,
                                           reference_params=self.config.get_option("dataset_create_params").get("reference_args", None),
                                           scenario_params=self.config.get_option("dataset_create_params")["train"],
                                           seed=self.train_actor_seed,
                                           log_path=self.log_path)
-        self.val_actor = XDepthAgent(self.env.action_space,
+        self.val_actor = XDepthAgent(self.env,
                                      all_topo_actions=all_topo_actions,
                                      reference_params=self.config.get_option("dataset_create_params").get("reference_args", None),
                                      scenario_params=self.config.get_option("dataset_create_params")["test"],
                                      seed=self.val_actor_seed,
                                      log_path=self.log_path)
-        self.test_actor = XDepthAgent(self.env.action_space,
+        self.test_actor = XDepthAgent(self.env,
                                       all_topo_actions=all_topo_actions,
                                       reference_params=self.config.get_option("dataset_create_params").get("reference_args", None),
                                       scenario_params=self.config.get_option("dataset_create_params")["test"],
                                       seed=self.test_actor_seed,
                                       log_path=self.log_path)
-        self.test_ood_topo_actor = XDepthAgent(self.env.action_space,
+        self.test_ood_topo_actor = XDepthAgent(self.env,
                                                all_topo_actions=all_topo_actions,
                                                reference_params=self.config.get_option("dataset_create_params").get("reference_args", None),
                                                scenario_params=self.config.get_option("dataset_create_params")["test_ood"],
                                                seed=self.test_ood_topo_actor_seed,
                                                log_path=self.log_path)
 
 def get_env(env_kwargs: dict):
```

### Comparing `lips-benchmark-0.2.1/lips/benchmark/wheelBenchmark.py` & `lips-benchmark-0.2.2/lips/benchmark/wheelBenchmark.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/config/__init__.py` & `lips-benchmark-0.2.2/lips/config/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/config/configmanager.py` & `lips-benchmark-0.2.2/lips/config/configmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     def __init__(self,
                  path: Union[str, pathlib.Path],
                  section_name: str="DEFAULT",
                 ):
         if path is None:
             raise RuntimeError("A path should be indicated!")
         elif not os.path.exists(path):
-            raise RuntimeError("A path to a configuration file should be indicated!")
+            raise RuntimeError("A path to an existing configuration file should be indicated!")
         elif not str(path).endswith(".ini"):
             raise RuntimeError("The configuration file should have `.ini` extension!")
         else:
             self.path_config = path
         self.section_name = section_name
         self.config = ConfigParser()
         # if a config file exists already try to load it
```

### Comparing `lips-benchmark-0.2.1/lips/dataset/__init__.py` & `lips-benchmark-0.2.2/lips/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/dataset/airfransDataSet.py` & `lips-benchmark-0.2.2/lips/dataset/airfransDataSet.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/dataset/dataSet.py` & `lips-benchmark-0.2.2/lips/dataset/dataSet.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,15 @@
     name: str
         the name of the dataset
     """
     def __init__(self, name:str):
         self.name = name
         self.data = None
         self.size = 0
-
-    def __len__(self):
-        return self.size
+        self.current_index = 0
 
     def generate(self,
                  simulator: PhysicalSimulator,
                  actor: Union[None, object],
                  path_out: Union[str, None],
                  nb_samples: int,
                  simulator_seed: Union[None, int]=None,
@@ -129,24 +127,27 @@
 
         """
         if self.data is None:
             raise RuntimeError("Impossible to get_data from a non initialized dataset. "
                                "Have you called `dataset.load(...)` "
                                "or `dataset.generate(...)` ?")
 
-    def __len__(self)->int:
-        data=self.GetData()
-        return data[list(data.keys())[0]].shape[0]
+    def __len__(self):
+        return self.size
+    
+    # def __len__(self)->int:
+    #     data = self.get_data()
+    #     return data[list(data.keys())[0]].shape[0]
 
     def __iter__(self):
         self.current_index = 0
         return self
 
     def __next__(self):
         if self.current_index < len(self):
-            currentData=self.__getitem__(self.current_index)
+            current_data = self.__getitem__(self.current_index)
             self.current_index += 1
-            return currentData
+            return current_data
         raise StopIteration
 
-    def __getitem__(self, item:int):
+    def __getitem__(self, index:int):
         return self.get_data(index)
```

### Comparing `lips-benchmark-0.2.1/lips/dataset/pneumaticWheelDataSet.py` & `lips-benchmark-0.2.2/lips/dataset/pneumaticWheelDataSet.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/dataset/powergridDataSet.py` & `lips-benchmark-0.2.2/lips/dataset/powergridDataSet.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,25 +12,80 @@
 
 import os
 import warnings
 import shutil
 import copy
 from typing import Union, Callable
 import json
-from tqdm import tqdm  # TODO remove for final push
+from tqdm import tqdm 
+import zipfile
+from urllib.request import urlretrieve
 
 import numpy as np
+from scipy import sparse
 from grid2op.Agent import BaseAgent
 
 from . import DataSet
 from ..utils import NpEncoder
 from ..logger import CustomLogger
 from ..physical_simulator import Grid2opSimulator
 from ..config import ConfigManager
 
+class DownloadProgressBar(tqdm):
+    """Provides `update_to(n)` which uses `tqdm.update(delta_n)`."""
+    def update_to(self, b = 1, bsize = 1, tsize = None):
+        """
+        b  : int, optional
+            Number of blocks transferred so far [default: 1].
+        bsize  : int, optional
+            Size of each block (in tqdm units) [default: 1].
+        tsize  : int, optional
+            Total size (in tqdm units). If [default: None] remains unchanged.
+        """
+        if tsize is not None:
+            self.total = tsize
+        self.update(b*bsize - self.n) # also sets self.n = b * bsize
+
+def downloadPowergridDataset(path: str, dataset_name: str="lips_case14_sandbox", unzip: bool=True):
+    """Download the dataset
+
+    Parameters
+    ----------
+    path : ``str``
+        path to download the dataset
+
+    dataset_name : ``str``, optional
+        the dataset name, by default "l2rpn_case14_sandbox"
+    
+    unzip : ``bool``, optional
+        whether to unzip the downloaded file, by default True
+
+    Function
+    ------
+    Download the powergrid dataset and unzip it in the given path
+    available datasets are:
+        - lips_case14_sandbox
+        - lips_neurips_2020_track1_small
+        - lips_idf_2023 
+    """
+    try:
+        base_url = "https://data.lips.irt-systemx.fr/data/"
+        url = base_url + dataset_name + ".zip"
+        os.makedirs(path, exist_ok = True)
+        with DownloadProgressBar(unit = 'B', unit_scale = True, miniters = 1, unit_divisor = 1024, desc = 'Downloading test') as t:
+            urlretrieve(url, filename = os.path.join(path, dataset_name + '.zip'), reporthook = t.update_to)
+
+        if unzip:
+            print("Extracting " + dataset_name + ".zip at " + path + "...")
+            with zipfile.ZipFile(os.path.join(path, dataset_name + '.zip'), 'r') as zipf:
+                zipf.extractall(path)
+
+    except ImportError as exc_:
+        raise RuntimeError("Impossible to `download` powergrid ") from exc_
+        
 class PowerGridDataSet(DataSet):
     """Class to manage powergrid data
 
     This specific DataSet uses grid2op framework to simulate data coming from a powergrid.
 
     Attributes
     ----------
@@ -100,23 +155,28 @@
         self._attr_y = self.config.get_option("attr_y")
 
         self.env_data = dict()
         self._slack_id = None
 
         #TODO add a seed for reproducible experiment !
 
+    def download(self, path: str, dataset_name: str="lips_case14_sandbox", unzip: bool=True):
+        downloadPowergridDataset(path, dataset_name, unzip)
+            
+
     def generate(self,
                  simulator: Grid2opSimulator,
                  actor: Union[BaseAgent, None],
                  path_out: Union[str, None],
                  nb_samples: int,
                  nb_samples_per_chronic: int=288, # 1 day
                  simulator_seed: Union[None, int]=None,
                  actor_seed: Union[None, int]=None,
                  do_store_physics: bool=False,
+                 store_as_sparse: bool=False,
                  is_dc: bool=False):
         """Generate a powergrid dataset
 
         For this dataset, we use a Grid2opSimulator and a  grid2op Agent to generate data from a powergrid.
         This implementation can also serve as a reference for other implementation of the `generate` function.
 
         Parameters
@@ -168,58 +228,67 @@
             # this part is only temporary, until a viable way to store the complete resulting state is found
             array_ = getattr(init_state, attr_nm)
             self.data[attr_nm] = np.zeros((nb_samples, array_.shape[0]), dtype=array_.dtype)
         
         #to save physical variables if required
         if (do_store_physics):
             n_bus_bars = simulator._simulator.n_sub * 2
-            self.data["YBus"] = np.zeros((nb_samples, n_bus_bars, n_bus_bars), dtype=np.complex128) #for admittance matrix
+            # store the Ybus as sparse matrix, mendatory for large envs as the memory is highly impacted by this matrix
+            if store_as_sparse:
+                self.__ybus_data = []
+                self.__row_indices = []
+                self.__col_indices = []
+            else:
+                self.data["YBus"] = np.zeros((nb_samples, n_bus_bars, n_bus_bars), dtype=np.complex128) #for admittance matrix
             self.data["SBus"] = np.zeros((nb_samples, n_bus_bars), dtype=np.complex128) #for vector of nodal injections
             self.data["PV_nodes"] = np.zeros((nb_samples, n_bus_bars), dtype=bool) #for indices of P-V nodes
             self.data["slack"] = np.zeros((nb_samples, 2), dtype=np.float16) #for indice of slack and active power adjusment from chronic
 
         ds_size = 0
         pbar = tqdm(total = nb_samples)
         is_LightSimBackend = ("lightsim2grid" in str(simulator._simulator.backend.__class__))
         while ds_size < nb_samples:
             simulator.sample_chronics()
             nb_steps = 0
             while (nb_steps < nb_samples_per_chronic):
                 simulator.modify_state(actor)
                 current_state, _ = simulator.get_state()
                 grid = simulator._simulator.backend._grid
-                self._store_obs(ds_size, current_state, grid, do_store_physics, is_LightSimBackend, is_dc)
+                self._store_obs(ds_size, current_state, grid, do_store_physics, is_LightSimBackend, is_dc, store_as_sparse)
                 nb_steps += 1
                 ds_size += 1
                 pbar.update(1)
                 if ds_size >= nb_samples:
                     break
-
+        if do_store_physics & store_as_sparse:
+            sparse_matrix = sparse.csr_matrix((self.__ybus_data, (self.__row_indices, self.__col_indices)),
+                                              shape=(nb_samples,n_bus_bars*n_bus_bars))
+            self.data["YBus"] = sparse_matrix
         pbar.close()
         self.size = nb_samples
         self._init_sample()
         self._infer_sizes()
         self._store_env_data(simulator._simulator)
         self._store_chronics_info(simulator)
         if path_out is not None:
             # I should save the data
-            self._save_internal_data(path_out)
+            self._save_internal_data(path_out, do_save_physics=do_store_physics, store_as_sparse=store_as_sparse)
 
-    def _store_obs(self, current_size, obs, grid, do_store_physics=True, is_lightSimBackend=True, is_dc=False):
+    def _store_obs(self, current_size, obs, grid, do_store_physics=True, is_lightSimBackend=True, is_dc=False, store_as_sparse=False):
         """store an observation in self.data"""
         for attr_nm in self._attr_names:
             array_ = getattr(obs, attr_nm)
             self.data[attr_nm][current_size, :] = array_
 
         #Also Store Admittance Matrix YBus and Injection Vector SBus (if backend is LightSim2Grid
         if(do_store_physics):
-            self._store_physics(current_size, obs, grid, is_lightSimBackend, is_dc)
+            self._store_physics(current_size, obs, grid, is_lightSimBackend, is_dc, store_as_sparse)
 
 
-    def _store_physics(self, current_size: int, obs, grid, is_lightSimBackend: bool, is_dc: bool=False):
+    def _store_physics(self, current_size: int, obs, grid, is_lightSimBackend: bool, is_dc: bool=False, store_as_sparse: bool=False):
         """Store physical variables related to grid in addition to regular observations
 
         Parameters
         ----------
         current_size : _type_
             _description_
         obs : _type_
@@ -257,15 +326,23 @@
 
             #get info on slack
             prod_bus, _ = obs._get_bus_id(obs.gen_pos_topo_vect, obs.gen_to_subid)
             node_slack_id = prod_bus[-1]
             index_gens_slack = (prod_bus==node_slack_id)
             adjusted_prod_slack = obs.gen_p[index_gens_slack].sum() - Sbus[node_slack_id].real #after_powerflow - in_chronics
 
-            self.data["YBus"][current_size, :] = admittance_matrix
+            if store_as_sparse:
+                array_2d = admittance_matrix.reshape(1,-1)
+                row_index, col_index = np.nonzero(array_2d)
+                data = array_2d[row_index, col_index]
+                self.__row_indices.extend(row_index + current_size)
+                self.__col_indices.extend(col_index)
+                self.__ybus_data.extend(data)
+            else:
+                self.data["YBus"][current_size, :] = admittance_matrix
             self.data["SBus"][current_size, :] = Injection_vect
             self.data["PV_nodes"][current_size, :] = pv_nodes
             self.data["slack"][current_size, :] = np.array([node_slack_id,adjusted_prod_slack], dtype=np.float16)
         else:
             self.logger.warning("Cannot store physics data if not using LightSim2Grid backend")
 
     def _store_chronics_info(self, simulator):
@@ -298,15 +375,15 @@
         chronics_path = os.path.join(path_out, "chronics")
         os.mkdir(chronics_path)
         for attr_nm, array_ in self.chronics_info.items():
             if attr_nm == "time_stamps":
                 array_ = np.asanyarray(array_, dtype=object)
             np.savez_compressed(f"{os.path.join(chronics_path, attr_nm)}.npz", data=array_)
 
-    def _save_internal_data(self, path_out:str,do_save_physics=True):
+    def _save_internal_data(self, path_out:str,do_save_physics=True, store_as_sparse: bool=False):
         """save the self.data in a proper format
 
         Parameters
         ----------
         path_out : ``str``
             path to save the data
 
@@ -332,29 +409,32 @@
         self.logger.info(f"Creating the path {full_path_out} to store the dataset name {self.name}")
 
         #for attr_nm in (*self._attr_names, *self._theta_attr_names):
         for attr_nm in self._attr_names:
             np.savez_compressed(f"{os.path.join(full_path_out, attr_nm)}.npz", data=self.data[attr_nm])
         if(do_save_physics):
             if("YBus" in self.data.keys()):
-                np.savez_compressed(os.path.join(full_path_out, "YBus")+".npz", data=self.data["YBus"])
+                if store_as_sparse:
+                    sparse.save_npz(os.path.join(full_path_out, "YBus")+".npz", matrix=self.data["YBus"])
+                else:
+                    np.savez_compressed(os.path.join(full_path_out, "YBus")+".npz", data=self.data["YBus"])
             if("SBus" in self.data.keys()):
                 np.savez_compressed(os.path.join(full_path_out, "SBus") + ".npz", data=self.data["SBus"])
             if("PV_nodes" in self.data.keys()):
                 np.savez_compressed(os.path.join(full_path_out, "PV_nodes") + ".npz", data=self.data["PV_nodes"])
             if("slack" in self.data.keys()):
                 np.savez_compressed(os.path.join(full_path_out, "slack") + ".npz", data=self.data["slack"])
                 
         
         self._save_chronics_info(full_path_out)
         # save static_data
         with open(os.path.join(full_path_out ,"metadata.json"), "w", encoding="utf-8") as f:
             json.dump(obj=self.env_data, fp=f, indent=4, sort_keys=True, cls=NpEncoder)
 
-    def load(self, path:str):
+    def load(self, path:str, load_ybus_as_sparse: bool=False):
         """load the dataset from a path
 
         Parameters
         ----------
         path : ``str``
             path from which the data should be loaded
 
@@ -388,21 +468,25 @@
         if self.data is not None:
             warnings.warn(f"Deleting previous run in attempting to load the new one located at {path}")
         self.data = {}
         self.size = None
         #for attr_nm in (*self._attr_names, *self._theta_attr_names):
         if self.config.get_option("attr_physics"):
             attr_names = self._attr_names + self.config.get_option("attr_physics")
-        else: 
+        else:
             attr_names = self._attr_names
 
         for attr_nm in attr_names:
             path_this_array = f"{os.path.join(full_path, attr_nm)}.npz"
-            self.data[attr_nm] = np.load(path_this_array)["data"]
-            self.size = self.data[attr_nm].shape[0]
+            if (attr_nm == "YBus") and (load_ybus_as_sparse):
+                self.data[attr_nm] = sparse.load_npz(path_this_array)
+            else:
+                self.data[attr_nm] = np.load(path_this_array)["data"]
+
+        self.size = self.data[attr_nm].shape[0]
 
         self._init_sample()
         self._infer_sizes()
         self._load_env_data(full_path)
         self._load_chronics_info(full_path)
 
     def _load_env_data(self, path:str):
@@ -548,19 +632,20 @@
             res[el][:] = self.data[el][index, :]
 
         return res
 
     def _infer_sizes(self):
         #data = copy.deepcopy(self.data)
         self._sizes_x = np.array([self.data[el].shape[1] for el in self._attr_x], dtype=int)
-        self._sizes_tau = np.array([self.data[el].shape[1] for el in self._attr_tau], dtype=int)
-        self._sizes_y = np.array([self.data[el].shape[1] for el in self._attr_y], dtype=int)
         self._size_x = np.sum(self._sizes_x)
-        self._size_tau = np.sum(self._sizes_tau)
+        self._sizes_y = np.array([self.data[el].shape[1] for el in self._attr_y], dtype=int)
         self._size_y = np.sum(self._sizes_y)
+        if self._attr_tau is not None:
+            self._sizes_tau = np.array([self.data[el].shape[1] for el in self._attr_tau], dtype=int)
+            self._size_tau = np.sum(self._sizes_tau)
 
     def get_sizes(self, attr_x: Union[tuple, None]=None, attr_tau: Union[tuple, None]=None, attr_y: Union[tuple, None]=None):
         """Get the sizes of the dataset
 
         Returns
         -------
         tuple
@@ -569,26 +654,26 @@
         """
         if attr_x is not None:
             sizes_x = np.array([self.data[el].shape[1] for el in attr_x], dtype=int)
             size_x = np.sum(sizes_x)
         else:
             size_x = self._size_x
 
-        if attr_tau is not None:
-            sizes_tau = np.array([self.data[el].shape[1] for el in attr_tau], dtype=int)
-            size_tau = np.sum(sizes_tau)
-        else:
-            size_tau = self._size_tau
-
-
         if attr_y is not None:
             sizes_y = np.array([self.data[el].shape[1] for el in attr_y], dtype=int)
             size_y = np.sum(sizes_y)
         else:
             size_y = self._size_y
+
+        if attr_tau is not None:
+            sizes_tau = np.array([self.data[el].shape[1] for el in attr_tau], dtype=int)
+            size_tau = np.sum(sizes_tau)
+        else:
+            size_tau = self._size_tau
+            #return size_x, size_y
         
         return size_x, size_tau, size_y
 
     def extract_data(self, concat: bool=True) -> tuple:
         """extract the x and y data from the dataset
 
         Parameters
@@ -600,24 +685,29 @@
         tuple
             extracted inputs and outputs
         """
         # init the sizes and everything
         data = copy.deepcopy(self.data)
 
         if concat:
-            attr_x = self._attr_tau + self._attr_x
+            if self._attr_tau is not None:
+                attr_x = self._attr_x + self._attr_tau
+            else:
+                attr_x = self._attr_x
             extract_x = np.concatenate([data[el].astype(np.float32) for el in attr_x], axis=1)
             extract_y = np.concatenate([data[el].astype(np.float32) for el in self._attr_y], axis=1)
             return extract_x, extract_y
         else:
             extract_x = [data[el].astype(np.float32) for el in self._attr_x]
-            extract_tau = [data[el].astype(np.float32) for el in self._attr_tau]
             extract_y = [data[el].astype(np.float32) for el in self._attr_y]
-            return (extract_x, extract_tau), extract_y
-
+            if self._attr_tau is not None:
+                extract_tau = [data[el].astype(np.float32) for el in self._attr_tau]
+                return (extract_x, extract_tau), extract_y
+            else:
+                return extract_x, extract_y
 
     def reconstruct_output(self, data: "np.ndarray") -> dict:
         """It reconstruct the data from the extracted data
 
         Parameters
         ----------
         data : ``np.ndarray``
```

### Comparing `lips-benchmark-0.2.1/lips/dataset/sampler.py` & `lips-benchmark-0.2.2/lips/dataset/sampler.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/dataset/scaler/powergrid_scaler.py` & `lips-benchmark-0.2.2/lips/dataset/scaler/powergrid_scaler.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/dataset/scaler/rolling_scaler.py` & `lips-benchmark-0.2.2/lips/dataset/scaler/rolling_scaler.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/dataset/scaler/standard_scaler.py` & `lips-benchmark-0.2.2/lips/dataset/scaler/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/dataset/scaler/standard_scaler_iterative.py` & `lips-benchmark-0.2.2/lips/dataset/scaler/standard_scaler_iterative.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
         self.no_norm_x = no_norm_x
         self.no_norm_y = no_norm_y
 
     def fit(self, x, y):
         self._m_x,self._std_x = iterative_fit(data=x, chunk_sizes=self.chunk_sizes)
         self._m_y,self._std_y = iterative_fit(data=y, chunk_sizes=self.chunk_sizes)
         # to avoid division by 0.
-        self._std_x[np.abs(self._std_x) <= 1e-1] = 1
-        self._std_y[np.abs(self._std_y) <= 1e-1] = 1
+        self._std_x[np.abs(self._std_x) <= 1e-6] = 1
+        self._std_y[np.abs(self._std_y) <= 1e-6] = 1
         if self.no_norm_x is not None:
             self._m_x[self.no_norm_x]=0
             self._std_x[self.no_norm_x]=1
 
         if self.no_norm_y is not None:
             self._m_y[self.no_norm_y]=0
             self._std_y[self.no_norm_y]=1
```

### Comparing `lips-benchmark-0.2.1/lips/dataset/scaler/standard_scaler_per_channel.py` & `lips-benchmark-0.2.2/lips/dataset/scaler/standard_scaler_per_channel.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/dataset/utils/powergrid_utils.py` & `lips-benchmark-0.2.2/lips/dataset/utils/powergrid_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 PowerGrid general scenario utilities
 """
 from typing import Union
 import itertools
 import warnings
 import numpy as np
 
-from grid2op.Chronics import GridStateFromFile
-from grid2op.Action.DontAct import DontAct
+# from grid2op.Chronics import GridStateFromFile
+from grid2op.Chronics import GridStateFromFileWithForecasts
+from grid2op.Action import DontAct
 from grid2op.Action import PlayableAction
 from grid2op.Agent import BaseAgent
 from grid2op.Parameters import Parameters
 
 from ...logger import CustomLogger
 from ...config import ConfigManager
 
@@ -38,15 +39,15 @@
     env_name = config.get_option("env_name")
     param = Parameters()
     param.init_from_dict(config.get_option("env_params"))
 
     return {"dataset": env_name,
             "param": param,
             # disable maintenances
-            "data_feeding_kwargs": {"gridvalueClass": GridStateFromFile},
+            "data_feeding_kwargs": {"gridvalueClass": GridStateFromFileWithForecasts},
             # inhibit the opponent
             "action_class": PlayableAction,
             "opponent_init_budget": 0,
             "opponent_action_class": DontAct,
             "backend": BkCls()}
 
 class XDepthAgent(BaseAgent):
@@ -96,33 +97,39 @@
     -----
     # TODO: verify that number of actions listed in subs_to_change is more than ``prob_depth``
     # TODO: verify that when params is None, kwargs include all the required parameters
     # TODO: verify that we do not disconnect the same lines and change the same subs as the reference
     # TODO: Do not take the same actions as the opponent (if opponent is avoided, this is not necessary)
     """
     def __init__(self,
-                 action_space,
+                 env,
                  all_topo_actions: Union[list, None]=None,
                  reference_params: Union[dict, None]=None,
                  scenario_params: Union[dict, None]=None,
                  log_path: Union[str, None]=None,
                  seed: Union[int, None]=None,
                  **kwargs
                 ):
 
-        super().__init__(action_space)
+        super().__init__(env.action_space)
+        self.env = env
+        action_space = self.env.action_space
         self.params = scenario_params if scenario_params is not None else {}
         self.params.update(kwargs)
         self.topo_actions = self.params.get("topo_actions", None)
         self.lines_to_disc = self.params.get("lines_to_disc", None)
         self.prob_depth = self.params.get("prob_depth", (1., ))
         self.max_depth = len(self.prob_depth)
         self.prob_type = self.params.get("prob_type", (1., 0.))
         self.prob_do_nothing = self.params.get("prob_do_nothing", 1)
         self.max_disc = self.params.get("max_disc", 0)
+        self.action_by_area = self.params.get("action_by_area", False)
+        if self.action_by_area:
+            self.lines_id_by_area = list(env._game_rules.legal_action.lines_id_by_area.values())
+
         if reference_params == {}:
             self.reference_args = None
         else:
             self.reference_args = reference_params
 
         self.seed(seed)
 
@@ -171,15 +178,15 @@
             self.ref_lines_to_disc = self.reference_args.get("lines_to_disc", None)
             self.ref_topo_actions = self.reference_args.get("topo_actions", None)
             self.ref_prob_depth = self.reference_args.get("prob_depth", (1., ))
             self.ref_prob_type = self.reference_args.get("prob_type", (1., 0.))
             self.ref_prob_do_nothing = self.reference_args.get("prob_do_nothing", 1.)
             self.ref_max_disc = self.reference_args.get("max_disc", 0)
 
-            self.ref_agent = self.__class__(action_space=self.action_space,
+            self.ref_agent = self.__class__(self.env,
                                             all_topo_actions=self.all_topo_actions,
                                             log_path=self.log_path,
                                             seed=seed,
                                             topo_actions=self.ref_topo_actions,
                                             lines_to_disc=self.ref_lines_to_disc,
                                             prob_depth=self.ref_prob_depth,
                                             prob_type=self.ref_prob_type,
@@ -324,15 +331,24 @@
     def _select_line_action(self):
         """
         select randomly one line to disconnect
         """
         self._remaining_lines = list(set(np.arange(len(self.line_ids))) -
                                      set(self.disconnected_lines_id)) #-
                                      #set(self.opponent_attack_line))
-        id_ = self.space_prng.choice(self._remaining_lines)
+        #id_ = self.space_prng.choice(self._remaining_lines)
+        
+        # select a line if it is in the same region of the first disconnection
+        if (len(self.disconnected_lines_id) > 0) & (self.action_by_area): # ensure that there is already a disconnected line
+            # get the area in which we have already disconnected a line
+            area_id_ = [i for i, area in enumerate(self.lines_id_by_area) if self.disconnected_lines_id[-1] in area][0]
+            remaining_lines = list(set(self.lines_id_by_area[area_id_]) - set(self.disconnected_lines_id))
+            id_ = self.space_prng.choice(remaining_lines)
+        else:
+            id_ = self.space_prng.choice(self._remaining_lines)
         return self.line_ids[id_], self._disc_actions[id_]
 
     def _select_topo_action(self, sub_id):
         """
         select randomly one possible action for one substation with id ``sub_id``
         """
         id_ = self.space_prng.choice(len(self.topo_actions[sub_id]))
```

### Comparing `lips-benchmark-0.2.1/lips/evaluation/__init__.py` & `lips-benchmark-0.2.2/lips/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/evaluation/airfrans_evaluation.py` & `lips-benchmark-0.2.2/lips/evaluation/airfrans_evaluation.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,25 +8,34 @@
     If a copy of the Mozilla Public License, version 2.0 was not distributed with this file,
     you can obtain one at http://mozilla.org/MPL/2.0/.
     SPDX-License-Identifier: MPL-2.0
     This file is part of LIPS, LIPS is a python platform for power networks benchmarking
 """
 from typing import Union
 from collections.abc import Iterable
+
 import numpy as np
+from scipy.stats import spearmanr
 
 from lips.config.configmanager import ConfigManager
 from lips.logger import CustomLogger
-
 from lips.evaluation import Evaluation
 from lips.evaluation.utils import metric_factory
 from lips.metrics.ml_metrics import metrics
+from lips.dataset.scaler.standard_scaler_iterative import iterative_fit
 
 import airfrans as af
-from scipy.stats import spearmanr
+
+def normalize_data(data,mean,std,field_names):
+    flattened_data = np.concatenate([data[field_name][:, None] for field_name in field_names], axis = 1)
+    flattened_data -= mean
+    flattened_data /= std
+    normalized_data = {field_name:flattened_data[:,field_id] for field_id,field_name in enumerate(field_names)}
+    return normalized_data
+
 
 class AirfRANSEvaluation(Evaluation):
     """Evaluation of the AirfRANS specific metrics
 
     It is a subclass of the Evaluation class
 
     Parameters
@@ -53,93 +62,113 @@
                                                  log_path=log_path
                                                  )
 
         self.data_path = data_path
         self.eval_dict = self.config.get_option("eval_dict")
         self.logger = CustomLogger(__class__.__name__, self.log_path).logger
         self.observation_metadata = dict()
+        self.ml_normalization = None
 
     def evaluate(self,
                  observations: dict,
                  predictions: dict,
                  observation_metadata : dict,
+                 ml_normalization : Union[dict, None]=None,
                  save_path: Union[str, None]=None) -> dict:
         """The main function which evaluates all the required criteria noted in config file
 
         Parameters
         ----------
         observations
             observations from true observations used to evaluate the predictions
         predictions
             predictions obtained from augmented simulators
         save_path, optional
             path where the results should be saved, by default None
         """
         # call the base class for generic evaluations
         super().evaluate(observations, predictions, save_path)
+        criteria = {}
+        self.ml_normalization = ml_normalization
         self.observation_metadata = observation_metadata
 
         for cat in self.eval_dict.keys():
-            self._dispatch_evaluation(cat)
+            criteria = self._dispatch_evaluation(cat, criteria)
 
-        return self.metrics
+        return criteria
 
-    def _dispatch_evaluation(self, category: str):
+    def _dispatch_evaluation(self, category: str, criteria: dict):
         """
         This helper function select the evaluation function with respect to the category
 
         In AirfRANS case, the OOD generalization evaluation is performed using `Benchmark` class
         by iterating over all the datasets
 
         Parameters
         ----------
         category: `str`
             the evaluation criteria category, the values could be one of the [`ML`, `Physics`]
         """
         if category == self.MACHINE_LEARNING:
             if self.eval_dict[category]:
-                self.evaluate_ml()
+                criteria[self.MACHINE_LEARNING] = self.evaluate_ml()
         if category == self.PHYSICS_COMPLIANCES:
             if self.eval_dict[category]:
-                self.evaluate_physics()
+                criteria[self.PHYSICS_COMPLIANCES] = self.evaluate_physics()
         if category == self.INDUSTRIAL_READINESS:
             raise Exception("Not done yet, sorry")
+        
+        return criteria
 
-    def evaluate_ml(self):
+    def evaluate_ml(self) -> dict:
         """
         Verify AirfRANS Machine Learning metrics
         """
         self.logger.info("Evaluate machine learning metrics")
-        metric_val_by_name = self.metrics[self.MACHINE_LEARNING]
-        self.metrics[self.MACHINE_LEARNING]={}
+        #Normalize prediction and observation before computing mlMetrics
+
+        field_names = self.predictions.keys()
+        if self.ml_normalization is None:
+            self.logger.info("Using current dataset to normalize")
+            chunk_sizes = [int(simulation[1]) for simulation in self.observation_metadata["simulation_names"]]
+            flattened_observation = np.concatenate([self.observations[field_name][:, None] for field_name in field_names], axis = 1)
+            mean_observ,std_observ = iterative_fit(flattened_observation,chunk_sizes)
+        else:
+            self.logger.info("Using reference dataset data to normalize")
+            mean_observ,std_observ = self.ml_normalization["mean"],self.ml_normalization["std"]
+        normalized_predictions = normalize_data(data=self.predictions,mean=mean_observ,std=std_observ,field_names=field_names)
+        normalized_observations = normalize_data(data=self.observations,mean=mean_observ,std=std_observ,field_names=field_names)
+
+
+        metrics_ml = {}
         for metric_name in self.eval_dict[self.MACHINE_LEARNING]:
             metric_fun = metric_factory.get_metric(metric_name)
-            metric_val_by_name[metric_name] = {}
-            for nm_, pred_ in self.predictions.items():
-                self.logger.info("Evaluating metric %s on variable %s", metric_name, nm_)
-                true_ = self.observations[nm_]
+            metric_name_normalized = metric_name+"_normalized"
+            metrics_ml[metric_name_normalized] = {}
+            for nm_, pred_ in normalized_predictions.items():
+                self.logger.info("Evaluating metric %s on variable %s", metric_name_normalized, nm_)
+                true_ = normalized_observations[nm_]
                 tmp = metric_fun(true_, pred_)
 
                 if isinstance(tmp, Iterable):
-                    metric_val_by_name[metric_name][nm_] = [float(el) for el in tmp]
-                    self.logger.info("%s for %s: %s", metric_name, nm_, tmp)
+                    metrics_ml[metric_name_normalized][nm_] = [float(el) for el in tmp]
+                    self.logger.info("%s for %s: %s",metric_name_normalized, nm_, tmp)
                 else:
-                    metric_val_by_name[metric_name][nm_] = float(tmp)
-                    self.logger.info("%s for %s: %.2E", metric_name, nm_, tmp)
-            self.metrics[self.MACHINE_LEARNING][metric_name] = metric_val_by_name[metric_name]
-
+                    metrics_ml[metric_name_normalized][nm_] = float(tmp)
+                    self.logger.info("%s for %s: %.2E", metric_name_normalized, nm_, tmp)
             #Compute additional metric for pressure at surface
-            true_pressure = self.observations["pressure"]
-            pred_pressure = self.predictions["pressure"]
+            true_pressure = normalized_observations["pressure"]
+            pred_pressure = normalized_predictions["pressure"]
             surface_data=self.observation_metadata["surface"]
             tmp_surface = metric_fun(true_pressure[surface_data.astype(bool)], pred_pressure[surface_data.astype(bool)])
-            self.metrics[self.MACHINE_LEARNING][metric_name+"_surfacic"]={"pressure": float(tmp)}
-            self.logger.info("%s surfacic for %s: %s", metric_name, "pressure", tmp_surface)
-
-    def evaluate_physics(self):
+            metrics_ml[metric_name_normalized+"_surfacic"]={"pressure": float(tmp_surface)}
+            self.logger.info("%s surfacic for %s: %s", metric_name_normalized, "pressure", tmp_surface)
+        return metrics_ml
+    
+    def evaluate_physics(self) -> dict:
         """
         Evaluate physical criteria on given observations
         """
         self.logger.info("Evaluate physical metrics")
         simulation_names=self.observation_metadata["simulation_names"]
         pred_data = self.from_batch_to_simulation(data=self.predictions,simulation_names=simulation_names)
         true_coefs = []
@@ -174,16 +203,15 @@
         metrics_values["std_relative_drag"]=std_rel_err[0]
         self.logger.info('The standard deviation of the relative absolute error for the drag coefficient is: {:.3f}'.format(std_rel_err[0]))
         metrics_values["mean_relative_lift"]=mean_rel_err[1]
         self.logger.info('The mean relative absolute error for the lift coefficient is: {:.3f}'.format(mean_rel_err[1]))
         metrics_values["std_relative_lift"]=std_rel_err[1]
         self.logger.info('The standard deviation of the relative absolute error for the lift coefficient is: {:.3f}'.format(std_rel_err[1]))
 
-        self.metrics[self.PHYSICS_COMPLIANCES]=metrics_values
-        return {'target_coefficients': true_coefs, 'predicted_coefficients': coefs, 'relative absolute error': rel_err}
+        return metrics_values
 
     def from_batch_to_simulation(self, data, simulation_names):
         sim_data = {}
         keys = list(set(data.keys()) - set(['simulation_names']))
         for key in keys:
             sim_data[key] = []
             ind = 0
@@ -215,21 +243,24 @@
         'x-velocity', 
         'y-velocity', 
         'pressure', 
         'turbulent_viscosity',
         'surface'
     )
     attr_x = attr_names[:7]
-    attr_y = attr_names[7:]
+    attr_y = attr_names[7:-1]
     my_dataset = AirfRANSDataSet(config = None,
                                  name = 'train',
                                  task = 'scarce',
                                  split = "training",
                                  attr_names = attr_names,
                                  log_path = 'log',
                                  attr_x = attr_x,
                                  attr_y = attr_y)
     my_dataset.load(path = directory_name)
     print(my_dataset)
-    config_path_benchmark=get_root_path()+os.path.join("..","configurations","airfrans","benchmarks","confAirfoil.ini")
+    config_path_benchmark=get_root_path()+os.path.join("..","configurations","airfoil","benchmarks","confAirfoil.ini")
     evaluation = AirfRANSEvaluation(config_path=config_path_benchmark,scenario="Case1",data_path = directory_name, log_path = 'log_eval')
-    evaluation.evaluate(observations = my_dataset.data, predictions = my_dataset.data)
+    output_values = {key:value for key,value in my_dataset.data.items() if key in attr_y}
+    metrics = evaluation.evaluate(observations = output_values, predictions = output_values, observation_metadata = my_dataset.extra_data)
+    print("Evaluation for solution equal to reference")
+    print(metrics)
```

### Comparing `lips-benchmark-0.2.1/lips/evaluation/evaluation.py` & `lips-benchmark-0.2.2/lips/evaluation/evaluation.py`

 * *Files 18% similar despite different names*

```diff
@@ -54,16 +54,14 @@
             self.config = config
 
         self.observations = dict()
         self.predictions = dict()
         # logger
         self.log_path = log_path
         self.logger = CustomLogger(__class__.__name__, self.log_path).logger
-        #self.mapper = Mapper()
-        self.metrics = {}
 
     @classmethod
     #@abstractmethod
     def from_benchmark(cls,
                        benchmark: "Benchmark",
                        ):
         """
@@ -80,28 +78,14 @@
                      config_section: Union[str, None]=None,
                      log_path: Union[str, None]=None):
         """
         Class method to initialize the evaluation from DataSet instance
         """
         pass
 
-    def __init_metric_dict(self) -> dict:
-        """
-        Initialize the metrics dictionary structure
-
-        It should be called if any modification to default category names
-        """
-        metrics_cat = {}
-        metrics_cat[self.MACHINE_LEARNING] = {}
-        metrics_cat[self.PHYSICS_COMPLIANCES] = {}
-        metrics_cat[self.INDUSTRIAL_READINESS] = {}
-        # metrics_cat[self.OOD_GENERALIZATION] = {}
-
-        return metrics_cat
-
     def evaluate(self,
                  observations: dict,
                  predictions: dict,
                  save_path: Union[str, None]=None):
         """Evaluate the predictions of an AugmentedSimulator
 
         This function should be overridden to do all the required evaluations for each category
@@ -122,16 +106,14 @@
         predictions : ``dict``
             predictions obtained from augmented simulators
         save_path : Union[``str``, ``None``], optional
             path where the results should be saved, by default None, by default None
         """
         self.observations = observations #dataset.data
         self.predictions = predictions
-        # create metrics dictionary
-        self.metrics.update(self.__init_metric_dict())
         
     def evaluate_ml(self):
         """
         It evaluates machine learning specific criteria
         """
         pass
```

### Comparing `lips-benchmark-0.2.1/lips/evaluation/pneumatic_evaluation.py` & `lips-benchmark-0.2.2/lips/evaluation/pneumatic_evaluation.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,110 +89,118 @@
         predictions
             predictions obtained from augmented simulators
         save_path, optional
             path where the results should be saved, by default None
         """
         # call the base class for generic evaluations
         super().evaluate(observations, predictions, save_path)
+        criteria = {}
 
         for cat in self.eval_dict.keys():
-            self._dispatch_evaluation(cat)
+            self._dispatch_evaluation(cat, criteria)
 
         # TODO: save the self.metrics variable
         if save_path:
             pass
 
-        return self.metrics
+        return criteria
 
-    def _dispatch_evaluation(self, category: str):
+    def _dispatch_evaluation(self, category: str, criteria: dict):
         """
         This helper function select the evaluation function with respect to the category
 
         In PowerGrid case, the OOD generalization evaluation is performed using `Benchmark` class
         by iterating over all the datasets
 
         Parameters
         ----------
         category: `str`
             the evaluation criteria category, the values could be one of the [`ML`, `Physics`]
         """
         if category == self.MACHINE_LEARNING:
             if self.eval_dict[category]:
-                self.evaluate_ml()
+                criteria[self.MACHINE_LEARNING] = self.evaluate_ml()
         if category == self.PHYSICS_COMPLIANCES:
             if self.eval_dict[category]:
-                self.evaluate_physics()
+                criteria[self.PHYSICS_COMPLIANCES] = self.evaluate_physics()
         if category == self.INDUSTRIAL_READINESS:
             raise Exception("Not done yet, sorry")
 
-    def evaluate_ml(self):
+        return criteria
+
+    def evaluate_ml(self) -> dict:
         """
         Verify Pneumatic Machine Learning metrics
         """
-        metric_val_by_name = self.metrics[self.MACHINE_LEARNING]
+        metrics_ml = {}
+        #metric_val_by_name = self.metrics[self.MACHINE_LEARNING]
         for metric_name in self.eval_dict[self.MACHINE_LEARNING]:
             metric_fun = metric_factory.get_metric(metric_name)
-            metric_val_by_name[metric_name] = {}
+            metrics_ml[metric_name] = {}
             for nm_, pred_ in self.predictions.items():
                 true_ = self.observations[nm_]
                 tmp = metric_fun(true_, pred_)
                 if isinstance(tmp, Iterable):
-                    metric_val_by_name[metric_name][nm_] = [float(el) for el in tmp]
+                    metrics_ml[metric_name][nm_] = [float(el) for el in tmp]
                     self.logger.info("%s for %s: %s", metric_name, nm_, tmp)
                 else:
-                    metric_val_by_name[metric_name][nm_] = float(tmp)
+                    metrics_ml[metric_name][nm_] = float(tmp)
                     self.logger.info("%s for %s: %.2E", metric_name, nm_, tmp)
+        return metrics_ml
 
-    def evaluate_physics(self):
+    def evaluate_physics(self) -> dict:
         """
         function that evaluates physical criteria on given observations and may rely on the physical solver
         """
-        metric_val_by_name = self.metrics[self.PHYSICS_COMPLIANCES]
+        #metric_val_by_name = self.metrics[self.PHYSICS_COMPLIANCES]
+        metrics_physics = {}
         attr_x=self.config.get_option("attr_x")
         obs_inputs={key: self.observations[key] for key in attr_x}
         inputs_separated = [dict(zip(obs_inputs,t)) for t in zip(*obs_inputs.values())]
 
         attr_y=self.config.get_option("attr_y_eval")
         obs_outputs={key: self.observations[key] for key in attr_y}
         output_separated = [dict(zip(obs_outputs,t)) for t in zip(*obs_outputs.values())]
         
         prediction_separated = [dict(zip(self.predictions,t)) for t in zip(*self.predictions.values())]
 
-        metric_val_by_name = {metric_name:[] for metric_name in self.eval_dict[self.PHYSICS_COMPLIANCES]}
+        metrics_physics = {metric_name:[] for metric_name in self.eval_dict[self.PHYSICS_COMPLIANCES]}
         for obs_input,obs_output,predict_out in zip(inputs_separated,output_separated,prediction_separated):
             simulator=type(self.simulator)(simulator_instance=self.simulator)
             simulator.modify_state(state=obs_input)
             simulator.build_model()
 
             for metric_name in self.eval_dict[self.PHYSICS_COMPLIANCES]:
                 if self.eval_crit_args and self.eval_crit_args[metric_name]:
                     criteria_params=self.eval_crit_args[metric_name]
                 else:
                     criteria_params=None
                 obs_crit = PhysicalCriteriaComputation(criteria_type=metric_name,simulator=simulator,field=obs_output,criteria_params=criteria_params)
                 pred_crit = PhysicalCriteriaComputation(criteria_type=metric_name,simulator=simulator,field=predict_out,criteria_params=criteria_params)
 
-                delta_absolute=np.array(obs_crit)-np.array(pred_crit) 
-                delta_relative=delta_absolute/np.array(obs_crit)  
+                delta_absolute=np.array(obs_crit)-np.array(pred_crit)
+                delta_relative=delta_absolute/np.array(obs_crit)
                 delta={
                     "absolute":delta_absolute,
                     "relative":delta_relative
-                } 
-                metric_val_by_name[metric_name].append(delta)
+                }
+                metrics_physics[metric_name].append(delta)
 
         for metric_name in self.eval_dict[self.PHYSICS_COMPLIANCES]:
-            deltas=metric_val_by_name[metric_name]
+            deltas=metrics_physics[metric_name]
             deltas_united = {error_type: np.array([single_comparison[error_type] for single_comparison in deltas]) for error_type in deltas[0]}
 
             mean_relative_error=np.mean(deltas_united["relative"],axis=0)
             if isinstance(mean_relative_error, Iterable):
                 for component_id,value in enumerate(mean_relative_error):
                     self.logger.info("%s mean relative error for component %d: %.2E", metric_name, component_id, value)
             else:
                 self.logger.info("%s mean relative error for %.2E", metric_name, mean_relative_error)
 
             mean_absolute_error=np.mean(deltas_united["absolute"],axis=0)
             if isinstance(mean_absolute_error, Iterable):
                 for component_id,value in enumerate(mean_absolute_error):
                     self.logger.info("%s mean absolute error for component %d: %.2E", metric_name, component_id, value)
             else:
-                self.logger.info("%s mean absolute error for %.2E", metric_name, mean_absolute_error)
+                self.logger.info("%s mean absolute error for %.2E", metric_name, mean_absolute_error)
+
+        return metrics_physics
```

### Comparing `lips-benchmark-0.2.1/lips/evaluation/powergrid_evaluation.py` & `lips-benchmark-0.2.2/lips/evaluation/powergrid_evaluation.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,16 +47,14 @@
                          config_section=scenario,
                          log_path=log_path
                          )
         self.eval_dict = self.config.get_option("eval_dict")
         self.eval_params = self.config.get_option("eval_params")
 
         self.logger = CustomLogger(__class__.__name__, self.log_path).logger
-        # read the criteria and their mapped functions for power grid
-        # self.criteria = self.mapper.map_powergrid_criteria()
 
     @classmethod
     def from_benchmark(cls,
                        benchmark: "PowerGridBenchmark",
                       ):
         """ Intialize the evaluation class from a benchmark object
 
@@ -86,124 +84,130 @@
             predictions obtained from augmented simulators
         save_path, optional
             path where the results should be saved, by default None
         """
         # call the base class for generic evaluations
         super().evaluate(observations, predictions, save_path)
 
+        criteria = {}
+
         # evaluate powergrid specific evaluations based on config
         for cat in self.eval_dict.keys():
-            self._dispatch_evaluation(cat, **kwargs)
+            criteria = self._dispatch_evaluation(cat, criteria, **kwargs)
 
         # TODO: save the self.metrics variable
         if save_path:
             pass
 
-        return self.metrics
+        return criteria
 
-    def _dispatch_evaluation(self, category: str, **kwargs):
+    def _dispatch_evaluation(self, category: str, criteria: dict, **kwargs):
         """
         This helper function select the evaluation function with respect to the category
 
         In PowerGrid case, the OOD generalization evaluation is performed using `Benchmark` class
         by iterating over all the datasets
 
         Parameters
         ----------
         category: `str`
             the evaluation criteria category, the values could be one of the [`ML`, `Physics`, `IndRed`, `OOD`]
         """
         if category == self.MACHINE_LEARNING:
             if self.eval_dict[category]:
-                self.evaluate_ml(**kwargs)
+                criteria[self.MACHINE_LEARNING] = self.evaluate_ml(**kwargs)
         if category == self.PHYSICS_COMPLIANCES:
             if self.eval_dict[category]:
-                self.evaluate_physics(**kwargs)
+                criteria[self.PHYSICS_COMPLIANCES] = self.evaluate_physics(**kwargs)
         if category == self.INDUSTRIAL_READINESS:
             if self.eval_dict[category]:
-                self.evaluate_industrial_readiness(**kwargs)
+                criteria[self.INDUSTRIAL_READINESS] = self.evaluate_industrial_readiness(**kwargs)
+
+        return criteria
 
-    def evaluate_ml(self, **kwargs):
+    def evaluate_ml(self, **kwargs) -> dict:
         """
         Verify PowerGrid Specific Machine Learning metrics such as MAPE90
         """
-        metric_dict = self.metrics[self.MACHINE_LEARNING]
+        metrics_ml = {}
         for metric_name in self.eval_dict[self.MACHINE_LEARNING]:
             if metric_name == "TIME_INF":
                 try:
                     augmented_simulator = kwargs["augmented_simulator"]
                     dataset = kwargs["dataset"]
                     if not isinstance(augmented_simulator, DCApproximationAS):
                         # using the machine learning point of view (max possible batch_size)
                         beg_ = time.perf_counter()
                         _ = augmented_simulator.predict(dataset, eval_batch_size=dataset.size)
                         end_ = time.perf_counter()
                         total_time = end_ - beg_
-                        metric_dict[metric_name] = total_time
+                        metrics_ml[metric_name] = total_time
                         self.logger.info("%s for %s: %s", metric_name, augmented_simulator.name, total_time)
                     else:
                         dc_comp_time = augmented_simulator.comp_time
-                        metric_dict[metric_name] = dc_comp_time
+                        metrics_ml[metric_name] = dc_comp_time
                         self.logger.info("%s for %s: %s", metric_name, augmented_simulator.name, dc_comp_time)
                 except KeyError:
                     self.logger.error("The augmented simulator or dataset are not provided to estimate the inference time.")
             else:
                 metric_fun = metric_factory.get_metric(metric_name)
                 # metric_fun = self.criteria.get(metric_name)
-                metric_dict[metric_name] = {}
+                metrics_ml[metric_name] = {}
                 for nm_, pred_ in self.predictions.items():
                     if nm_ == "__prod_p_dc":
                         # fix for the DC approximation
                         continue
                     true_ = self.observations[nm_]
                     tmp = metric_fun(true_, pred_)
                     if isinstance(tmp, Iterable):
-                        metric_dict[metric_name][nm_] = [float(el) for el in tmp]
+                        metrics_ml[metric_name][nm_] = [float(el) for el in tmp]
                         self.logger.info("%s for %s: %s", metric_name, nm_, tmp)
                     else:
-                        metric_dict[metric_name][nm_] = float(tmp)
+                        metrics_ml[metric_name][nm_] = float(tmp)
                         self.logger.info("%s for %s: %.2f", metric_name, nm_, tmp)
+        return metrics_ml
 
-    def evaluate_physics(self, **kwargs):
+    def evaluate_physics(self, **kwargs) -> dict:
         """
         function that evaluates the physics compliances on given observations
         It comprises various verifications which are:
 
         - Basic verifications (current/voltage/loss positivity, current eq, disc_lines)
         - Verification of law of conservation of energy
         - Verification of electrical loss
         - Verification of Kirchhoff's current law
         - Verification of Joule's law
         """
         try:
             env = kwargs["env"]
         except KeyError:
             self.logger.error("The environment (physical solver) is required for some physics critiera and should be provided")
-        metric_dict = self.metrics[self.PHYSICS_COMPLIANCES]
+        metrics_physics = {}
         for metric_name in self.eval_dict[self.PHYSICS_COMPLIANCES]:
             metric_fun = metric_factory.get_metric(metric_name)
             #metric_fun = self.criteria.get(metric_name)
-            metric_dict[metric_name] = {}
+            metrics_physics[metric_name] = {}
             tmp = metric_fun(self.predictions,
                              log_path=self.log_path,
                              observations=self.observations,
                              config=self.config,
                              **kwargs)
                              #env=env)
-            metric_dict[metric_name] = tmp
+            metrics_physics[metric_name] = tmp
+        return metrics_physics
 
-    def evaluate_industrial_readiness(self, **kwargs):
+    def evaluate_industrial_readiness(self, **kwargs) -> dict:
         """
         Evaluate the augmented simulators from Industrial Readiness point of view
 
         - Inference time
         - Scalability
 
         """
-        metric_dict = self.metrics[self.INDUSTRIAL_READINESS]
+        metrics_ind = {}
         for metric_name in self.eval_dict[self.INDUSTRIAL_READINESS]:
             if metric_name == "TIME_INF":
                 try:
                     augmented_simulator = kwargs["augmented_simulator"]
                     dataset = kwargs["dataset"]
 
                     if not isinstance(augmented_simulator, DCApproximationAS):
@@ -213,16 +217,17 @@
                             eval_batch_size = kwargs.get("eval_batch_size", augmented_simulator.params["eval_batch_size"])
 
                         # using the industrial readiness point of view (max possible batch_size)
                         beg_ = time.perf_counter()
                         _ = augmented_simulator.predict(dataset, eval_batch_size=eval_batch_size)
                         end_ = time.perf_counter()
                         total_time = end_ - beg_
-                        metric_dict[metric_name] = total_time
+                        metrics_ind[metric_name] = total_time
                         self.logger.info("%s for %s: %s", metric_name, augmented_simulator.name, total_time)
 
                     else:
                         dc_comp_time = augmented_simulator.comp_time
-                        metric_dict[metric_name] = dc_comp_time
+                        metrics_ind[metric_name] = dc_comp_time
                         self.logger.info("%s for %s: %s", metric_name, augmented_simulator.name, dc_comp_time)
                 except KeyError:
                     self.logger.error("The augmented simulator or dataset are not provided to estimate the inference time.")
+        return metrics_ind
```

### Comparing `lips-benchmark-0.2.1/lips/evaluation/utils.py` & `lips-benchmark-0.2.2/lips/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/logger/__init__.py` & `lips-benchmark-0.2.2/lips/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/logger/customLogger.py` & `lips-benchmark-0.2.2/lips/logger/customLogger.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/metrics/ml_metrics/mean_absolute_error.py` & `lips-benchmark-0.2.2/lips/metrics/ml_metrics/mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/metrics/ml_metrics/mean_absolute_percentage_error.py` & `lips-benchmark-0.2.2/lips/metrics/ml_metrics/mean_absolute_percentage_error.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/metrics/ml_metrics/mean_squared_error.py` & `lips-benchmark-0.2.2/lips/metrics/ml_metrics/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/metrics/ml_metrics/metrics.py` & `lips-benchmark-0.2.2/lips/metrics/ml_metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/metrics/ml_metrics/normalized_mean_squared_error.py` & `lips-benchmark-0.2.2/lips/metrics/ml_metrics/normalized_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/metrics/power_grid/__init__.py` & `lips-benchmark-0.2.2/lips/metrics/power_grid/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/metrics/power_grid/global_conservation.py` & `lips-benchmark-0.2.2/lips/metrics/power_grid/global_conservation.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/metrics/power_grid/joule_law.py` & `lips-benchmark-0.2.2/lips/metrics/power_grid/joule_law.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/metrics/power_grid/kirchhoff_law.py` & `lips-benchmark-0.2.2/lips/metrics/power_grid/kirchhoff_law.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/metrics/power_grid/local_conservation.py` & `lips-benchmark-0.2.2/lips/metrics/power_grid/local_conservation.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/metrics/power_grid/ohm_law.py` & `lips-benchmark-0.2.2/lips/metrics/power_grid/ohm_law.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/metrics/power_grid/physics_compliances.py` & `lips-benchmark-0.2.2/lips/metrics/power_grid/physics_compliances.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         supplementary arguments
 
     Returns
     -------
     `dict`
         a dictionary reporting the evaluation results
     """
-    FLOW_VARIABLES = ("p_or", "p_ex", "q_or", "q_ex", "a_or", "a_ex")
+    FLOW_VARIABLES = ("p_or", "p_ex", "q_or", "q_ex", "a_or", "a_ex", "v_or", "v_ex")
     # logger
     logger = CustomLogger("PhysicsCompliances", log_path).logger
     try:
         observations = kwargs["observations"]
     except KeyError:
         logger.error("Kwargs of function verify_disc_lines does not include observations key")
 
@@ -197,24 +197,26 @@
     verifications = dict()
     sum_disconnected_values = 0
 
     ind_disc = line_status != 1
     len_disc = np.sum(ind_disc)
 
     if np.any(ind_disc):
-        for g, key_pairs in zip(("p", "q", "a"), FLOW_VARIABLES):
-            if key_pairs[0] in predictions.keys():
-                for key_ in key_pairs:
-                    pred_disc = predictions[key_][ind_disc]
-                    violation = float(np.sum(np.abs(pred_disc)>0))
-                    verifications[key_] = violation
-                    sum_disconnected_values += violation
-                verifications[g] = float(np.sum((np.abs(key_pairs[0]) +
-                                                        np.abs(key_pairs[1]))>0) /
-                                                        len_disc)
+        num_var = 0
+        for var_ in FLOW_VARIABLES:
+            if var_ in predictions.keys():
+                num_var += 1
+                pred_disc = predictions[var_][ind_disc]
+                violation = float(np.sum(np.abs(pred_disc)>0))
+                verifications[var_] = violation / len_disc
+                sum_disconnected_values += violation
+        mean_disconnected_values = sum_disconnected_values / (len_disc * num_var)
+        verifications["violation_proportion"] = mean_disconnected_values
+    else:
+        verifications["violation_proportion"] = 0.
 
     if sum_disconnected_values > 0:
         logger.info("Prediction in presence of line disconnection. Problem encountered !")
     else:
         logger.info("Prediction in presence of line disconnection. Check passed !")
     return verifications
```

### Comparing `lips-benchmark-0.2.1/lips/metrics/power_grid/verify_voltage_equality.py` & `lips-benchmark-0.2.2/lips/metrics/power_grid/verify_voltage_equality.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/physical_simulator/__init__.py` & `lips-benchmark-0.2.2/lips/physical_simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/physical_simulator/dcApproximationAS.py` & `lips-benchmark-0.2.2/lips/physical_simulator/dcApproximationAS.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 import numpy as np
 
 
 from grid2op.Backend import PandaPowerBackend
 from grid2op.Action._BackendAction import _BackendAction
 from grid2op.Action import CompleteAction
+from lightsim2grid import LightSimBackend
 
 from . import Grid2opSimulator
 from . import PhysicsSolver
 from ..dataset.powergridDataSet import PowerGridDataSet
 from ..config import ConfigManager
 
 
@@ -41,42 +42,46 @@
     """
     def __init__(self,
                  name: str = "dc_approximation",
                  benchmark_name: str = "Benchmark1",
                  config_path: Union[str, None] = None,
                  grid_path: Union[str, None] = None,
                  simulator: Union[Grid2opSimulator, None] = None,
+                 backend: Union[PandaPowerBackend, LightSimBackend]=PandaPowerBackend,
+                 is_dc: bool = True,
+                 ignore_assert: bool = False
                  ):
         PhysicsSolver.__init__(self, name=name)
         self.config_manager = ConfigManager(path=config_path, section_name=benchmark_name)
         # input that will be given to the augmented simulator
         self._attr_x = ("prod_p", "prod_v", "load_p", "load_q", "topo_vect")
         # output that we want the proxy to predict
         #self._attr_y = ("a_or", "a_ex", "p_or", "p_ex", "q_or", "q_ex", "prod_q", "load_v", "v_or", "v_ex")
         attr_y = {"a_or", "a_ex", "p_or", "p_ex", "q_or", "q_ex", "prod_q", "load_v", "v_or", "v_ex"}
         self._attr_y = tuple(set(self.config_manager.get_option("attr_y")).intersection(attr_y))
         # TODO : this attribute is not already used
         self._attr_fix_gen_p = "__prod_p_dc"
 
         if grid_path is not None:
-            self._raw_grid_simulator = PandaPowerBackend()
+            self._raw_grid_simulator = backend()
             self._raw_grid_simulator.load_grid(grid_path)
-            self._raw_grid_simulator.assert_grid_correct()
+            if not(ignore_assert):
+                self._raw_grid_simulator.assert_grid_correct()
         elif simulator is not None:
             assert isinstance(simulator, Grid2opSimulator), "To make the DC approximation augmented simulator, you " \
                                                             "should provide the reference grid as a Grid2opSimulator"
 
             self._raw_grid_simulator = simulator._simulator.backend.copy()
         else:
             raise RuntimeError("Impossible to initialize the DC approximation with a grid2op simulator or"
                                "a powergrid")
 
         self._bk_act_class = _BackendAction.init_grid(self._raw_grid_simulator)
         self._act_class = CompleteAction.init_grid(self._raw_grid_simulator)
-
+        self.is_dc = is_dc
         self.comp_time = 0
 
     def compute(self, dataset: PowerGridDataSet):
         """
         evaluate the model on the whole dataset. It returns a dictionnary with the keys in self._attr_y
         """
         if not isinstance(dataset, PowerGridDataSet):
@@ -152,17 +157,22 @@
                         "load_q": one_example["load_q"][0, :],
                     }
                     })
         modifer += act
         self._raw_grid_simulator.apply_action(modifer)
 
         # start the simulator
-        _beg = time.time()
-        self._raw_grid_simulator.runpf(is_dc=True)
-        self.comp_time += time.time() - _beg
+        if isinstance(self._raw_grid_simulator, PandaPowerBackend):
+            _beg = time.time()
+            self._raw_grid_simulator.runpf(is_dc=self.is_dc)
+            self.comp_time += time.time() - _beg
+        elif isinstance(self._raw_grid_simulator, LightSimBackend):
+            beg_ = self._raw_grid_simulator._timer_solver
+            self._raw_grid_simulator.runpf(is_dc=self.is_dc)
+            self.comp_time += self._raw_grid_simulator._timer_solver - beg_
 
     def save(self, path_out):
         """
         this is not used for now.
         Ideally it should save the grid
         """
         pass
```

### Comparing `lips-benchmark-0.2.1/lips/physical_simulator/getfemSimulator.py` & `lips-benchmark-0.2.2/lips/physical_simulator/getfemSimulator.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/physical_simulator/grid2opSimulator.py` & `lips-benchmark-0.2.2/lips/physical_simulator/grid2opSimulator.py`

 * *Files 15% similar despite different names*

```diff
@@ -72,14 +72,24 @@
 
 
         self._nb_divergence = 0  # number of failures of modify_state
         self._nb_output = 0  # number of time get_state is called
 
         self._time_powerflow = 0
         self.comp_time = 0
+        self._timer_solver = 0
+        self._timer_preproc = 0
+        self._timer_postproc = 0
+
+        try:
+            from lightsim2grid import LightSimBackend
+            self.lightsim_backend = LightSimBackend
+        except ImportError as exc_:
+            print(exc_)
+            self.lightsim_backend = None
 
     def seed(self, seed: int):
         """
         It seeds the environment, for reproducible experiments.
 
         Parameters
         ----------
@@ -144,19 +154,29 @@
         super().modify_state(actor)  # perform the check that the actor is legit
         done = True
         while done:
             # simulate data (resimulate in case of divergence of the simulator)
             act = actor.act(self._obs, self._reward, done)
             _beg_time_pf = self._simulator._time_powerflow
             _beg_time_cp = self._simulator.backend.comp_time
+            # LightSimBackend specific timers
+            if isinstance(self._simulator.backend, self.lightsim_backend):
+                beg_preproc_time = self._simulator.backend._timer_preproc
+                beg_solver_time = self._simulator.backend._timer_solver
+                beg_postproc_time = self._simulator.backend._timer_postproc
+
             self._obs, self._reward, done, self._info = self._simulator.step(act)
-            _end_time_cp = self._simulator.backend.comp_time
-            _end_time_pf = self._simulator._time_powerflow
-            _diff_time_pf = _end_time_pf - _beg_time_pf
-            _diff_time_cp = _end_time_cp - _beg_time_cp
+
+            if isinstance(self._simulator.backend, self.lightsim_backend):
+                diff_timer_preproc = self._simulator.backend._timer_preproc - beg_preproc_time
+                diff_timer_solver = self._simulator.backend._timer_solver - beg_solver_time
+                diff_timer_postproc = self._simulator.backend._timer_postproc - beg_postproc_time
+
+            _diff_time_pf = self._simulator._time_powerflow - _beg_time_pf
+            _diff_time_cp = self._simulator.backend.comp_time - _beg_time_cp
 
             # verify for isolated injections
             check = self.__any_isolated_injections(self._obs)
             if check:
                 done=True
 
             check = self.__any_nan_values(self._obs)
@@ -165,26 +185,38 @@
 
             check = self.__any_isolated_nodes(self._simulator)
             if check:
                 done = True
 
             self._time_powerflow += _diff_time_pf
             self.comp_time += _diff_time_cp
+            if isinstance(self._simulator.backend, self.lightsim_backend):
+                self._timer_preproc += diff_timer_preproc
+                self._timer_solver += diff_timer_solver
+                self._timer_postproc += diff_timer_postproc
 
             if self._info["is_illegal"]:
                 self._time_powerflow -= _diff_time_pf
                 self.comp_time -= _diff_time_cp
+                if isinstance(self._simulator.backend, self.lightsim_backend):
+                    self._timer_preproc -= diff_timer_preproc
+                    self._timer_solver -= diff_timer_solver
+                    self._timer_postproc -= diff_timer_postproc
                 raise RuntimeError("Your `actor` should not take illegal action. Please modify the environment "
                                    "or your actor.")
 
             if done:
                 self._nb_divergence += 1
                 self._reset_simulator()
                 self._time_powerflow -= _diff_time_pf
                 self.comp_time -= _diff_time_cp
+                if isinstance(self._simulator.backend, self.lightsim_backend):
+                    self._timer_preproc -= diff_timer_preproc
+                    self._timer_solver -= diff_timer_solver
+                    self._timer_postproc -= diff_timer_postproc
             else:
                 self.time_stamps[self._chronic_counter].append(self._simulator.chronics_handler.real_data.data.current_datetime)
                 self.chronics_id.append(self._chronic_id)
                 self.chronics_name.append(self._simulator.chronics_handler.get_name())
 
     def visualize_network(self) -> PlotMatplot:
         """
```

### Comparing `lips-benchmark-0.2.1/lips/physical_simulator/physicalSimulator.py` & `lips-benchmark-0.2.2/lips/physical_simulator/physicalSimulator.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/physical_simulator/physicsSolver.py` & `lips-benchmark-0.2.2/lips/physical_simulator/physicsSolver.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/plot/power_grid/__init__.py` & `lips-benchmark-0.2.2/lips/plot/power_grid/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,10 +2,11 @@
 # See AUTHORS.txt
 # This Source Code Form is subject to the terms of the Mozilla Public License, version 2.0.
 # If a copy of the Mozilla Public License, version 2.0 was not distributed with this file,
 # you can obtain one at http://mozilla.org/MPL/2.0/.
 # SPDX-License-Identifier: MPL-2.0
 # This file is part of LIPS, LIPS is a python platform for power networks benchmarking
 
-__all__ = ["PlotData"]
+__all__ = ["PlotData", "PlotDataPlotly"]
 
 from lips.plot.power_grid.plotting import PlotData
+from lips.plot.power_grid.plotting import PlotDataPlotly
```

### Comparing `lips-benchmark-0.2.1/lips/tests/configs/powergrid/benchmarks/l2rpn_neurips_2020_track1_small.ini` & `lips-benchmark-0.2.2/configurations/powergrid/benchmarks/l2rpn_case14_sandbox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [DEFAULT]
-env_name = "l2rpn_neurips_2020_track1_small"
+env_name = "l2rpn_case14_sandbox"
 env_params = {
 	"NO_OVERFLOW_DISCONNECTION": True,
 	"MAX_LINE_STATUS_CHANGED": 999999,
 	"MAX_SUB_CHANGED": 999999,
 	"NB_TIMESTEP_COOLDOWN_LINE": 0,
 	"NB_TIMESTEP_COOLDOWN_SUB": 0}
 chronics = {
-	"train": "^((?!(.*[3-4][0-9].*)).)*$",
-	"val": ".*3[0-5].*",
-	"test": ".*3[5-9].*",
-	"test_ood": ".*4[0-9].*"
+	"train": "^((?!(.*9[0-9][0-9].*)).)*$", # # i use 994 chronics out of the 904 for training
+	"val": ".*9[0-4][0-9].*", # i use 50 full chronics for validation
+	"test": ".*9[5-9][0-4].*", # i use 25 full chronics for testing
+	"test_ood": ".*9[5-9][5-9].*" # i use 25 full chronics for testing
 	}
 samples_per_chronic = {
 	"initial_chronics_id": 0,
 	"train": 864,
 	"val": 288,
 	"test": 288,
 	"test_ood": 288,
@@ -41,31 +41,25 @@
 [Benchmark1]
 attr_x = ("prod_p", "prod_v", "load_p", "load_q")
 attr_tau = ("line_status", "topo_vect")
 attr_y = ("a_or", "a_ex")
 dataset_create_params = {
 	# REFERENCE PARAMS
 	"reference_args" : {
-		#"lines_to_disc": [3],
+		# "lines_to_disc": [3],
+		# "subs_to_change": [(1,13), (3,8), (4, 3), (8,6)], # (sub_id, action_id)
 		"topo_actions": [
-				#{'set_bus':{'substations_id':[(1,(2,2,1,1,1,2))]}},#sub1
-				{'set_bus':{'substations_id':[(1,(2,2,1,1,2,2))]}},#sub1
-                #{'set_bus':{'substations_id':[(4,(2,1,2,2,2,1))]}},#action_sub4
-                #{'set_bus':{'substations_id':[(4,(2,2,2,2,1,1))]}},#action_sub4_2
-				{'set_bus':{'substations_id':[(16,(1,1,1,1,1,2,2,1,1,2,2,1,1,1,1,1,1))]}},#sub16
-				{'set_bus':{'substations_id':[(16,(1,2,2,1,1,2,2,1,1,1,1,1,1,1,1,1,1))]}},#sub16
-                {'set_bus':{'substations_id':[(28,(2,1,2,1,1))]}}#sub28
-				#{"set_bus": {"lines_ex_id": [(17,2), (21,2)], "generators_id": [(6,2)]}},#sub16
-				#{"set_bus": {"lines_ex_id": [(20,2)], "loads_id": [(17,2)]}}#sub16
+				{'set_bus':{'substations_id':[(4,(2,1,2,1,2))]}},#sub4
+ 				{'set_bus':{'substations_id':[(1,(1,2,1,2,2,2))]}},#sub1
+				{'set_bus':{'substations_id':[(5,(1,1,2,2,1,2,2))]}}#sub5
 			],
-		"prob_depth": (.5, .5),
-		"prob_type": (1., 0.),
-		"prob_do_nothing": .1,
-		"max_disc": 0},
-	# SCENARIO PARAMS
+		"prob_depth": (0.7, 0.3), # authorizing until depth 2 combinations for reference
+		"prob_type": (1., 0.), # only topology change actions
+		"prob_do_nothing": 0.2, # include 20 percent DoNothing actions
+		"max_disc": 0},#no line disconnections
 	"train": {
 		# SCENARIO TOPOLOGY : disconnect or not one line at each tim step
 		"prob_depth": (1.,), # sample from depth 1
 		"prob_type": (0., 1.), # sample only from line disconnection
 		"prob_do_nothing": 0.3,  # probability of do nothing
 		"max_disc": 1}, # authorize at most 1 disconnection
 	"test":{
@@ -74,187 +68,276 @@
 		"prob_type": (0., 1.), # sample only from line disconnection
 		"prob_do_nothing": 0.,  # No do nothing
 		"max_disc": 1}, # authorize at most 1 disconnection
 	"test_ood":{
 		# SCENARIO TOPOLOGY: disconnect two lines at each time step
 		"prob_depth": (0., 1.), # Sample only from depth 2
 		"prob_type": (0., 1.), # sample only from line disconnection
-		"prob_do_nothing": 0,  # No do nothing
+		"prob_do_nothing": 0.,  # No do nothing
 		"max_disc": 2} # authorize at most 2 disconnection
 	}
 
 eval_dict = {
-	"ML": ["MSE_avg", "MAE_avg", "mape_avg", "mape_90_avg", "TIME_INF"],
+	"ML": ["MSE_avg", "MAE_avg", "MAPE_avg", "MAPE_90_avg", "TIME_INF"],
 	"Physics": ["CURRENT_POS"],
 	"IndRed": ["TIME_INF"],
-	"OOD": ["MSE_avg", "MAE_avg", "mape_avg", "mape_90_avg", "TIME_INF"]}
+	"OOD": ["MSE_avg", "MAE_avg", "MAPE_avg", "MAPE_90_avg", "TIME_INF"]}
 
 eval_params = {
-	"inf_batch_size": 59000, # #pas_de_temps=100 x #ligne=59 x #topo=10
-	"EL_tolerance": 0.04,
-	"GC_tolerance": 1e-3,
-	"LC_tolerance": 1e-2,
-	"KCL_tolerance": 1e-2,
-	"ACTIVE_FLOW": True}
+	"inf_batch_size": 14000} # #pas_de_temps=100 x #ligne=20 x #topo=7
 
 [Benchmark2]
 attr_x = ("prod_p", "prod_v", "load_p", "load_q")
 attr_tau = ("line_status", "topo_vect")
 attr_y = ("a_or", "a_ex", "p_or", "p_ex", "v_or", "v_ex")
 dataset_create_params = {
 	# REFERENCE PARAMS
 	"reference_args" : {
-		"prob_depth": (0.5, 0.5), # authorizing until depth 2 combinations for reference
+		"prob_depth": (1.,), # authorizing until depth 1 combinations for reference
 		"prob_type": (0., 1.), # only disconnections
-		"prob_do_nothing": 0.05, # include 5 percent DoNothing actions
-		"max_disc": 2}, # at most 2 disconnection allowed
+		"prob_do_nothing": 0.5, # include 50 percent DoNothing actions
+		"max_disc": 1}, # at most 1 disconnection allowed
 	"train": {
-		# SCENARIO TOPOLOGY : one sub topo change at each time step
-        #These are taken from the actions of the best agent "rl_agent" on scenarios of Grid2viz demo
-		"topo_actions": [{'set_bus':{'substations_id':[(26,(2,1,1,2,1,1,1,1,1))]}},#action_sub26
-        {'set_bus':{'substations_id':[(26,(2,2,2,1,2,1,1,1,1))]}},#action_sub26_2
-        {'set_bus':{'substations_id':[(26,(2,2,1,1,2,2,1,1,1))]}},#action_sub26_3
-        {'set_bus':{'substations_id':[(23,(2,2,2,2,1,1,2,2,1,2))]}},#action_sub23
-        {'set_bus':{'substations_id':[(23,(2,2,1,2,1,1,2,2,1,1))]}},#action_sub23_2
-        {'set_bus':{'substations_id':[(23,(2,1,1,1,2,2,2,2,2,2))]}},#action_sub23_3
-        {'set_bus':{'substations_id':[(23,(2,2,1,1,2,2,2,1,2,2))]}},#action_sub23_4
-        {'set_bus':{'substations_id':[(16,(2,1,1,1,2,1,1,1,2,2,2,1,2,1,1,1,2))]}},#action_sub16
-        {'set_bus':{'substations_id':[(16,(2,1,1,2,2,2,2,1,1,2,2,1,1,2,2,1,1))]}},#action_sub16_2
-        {'set_bus':{'substations_id':[(16,(2,2,2,2,2,1,1,2,2,2,1,1,2,2,1,2,1))]}},#action_sub16_3
-        {'set_bus':{'substations_id':[(16,(2,2,2,2,2,1,1,2,2,1,1,2,2,2,1,2,2))]}},#action_sub16_4
-
-        {'set_bus':{'substations_id':[(16,(2,1,1,1,2,2,2,1,2,2,2,1,2,2,2,2,1))]}},#action_sub16_5
-        {'set_bus':{'substations_id':[(16,(2,1,1,2,2,1,1,2,2,2,2,2,1,1,1,1,2))]}},#action_sub16_6
-        {'set_bus':{'substations_id':[(16,(2,2,1,2,2,1,1,2,2,2,2,1,1,2,1,1,2))]}},#action_sub16_7
-        {'set_bus':{'substations_id':[(16,(1,2,2,1,1,2,2,1,1,1,1,1,1,1,1,1,1))]}},#action_sub16_8
-        {'set_bus':{'substations_id':[(16,(1,1,1,1,1,2,2,1,1,2,2,1,1,1,1,1,1))]}},#action_sub16_9
-        {'set_bus':{'substations_id':[(9,(2,2,1,1,1,1,2))]}},#action_sub9
-        {'set_bus':{'substations_id':[(1,(2,2,1,1,2,2))]}},#action_sub1
-        {'set_bus':{'substations_id':[(1,(2,2,1,1,1,2))]}},#action_sub1_2
-        {'set_bus':{'substations_id':[(32,(2,2,1,1,1))]}},#action_sub32
-        {'set_bus':{'substations_id':[(4,(2,1,2,2,2,1))]}},#action_sub4
-        {'set_bus':{'substations_id':[(4,(2,2,2,2,1,1))]}},#action_sub4_2
-        {'set_bus':{'substations_id':[(28,(2,1,2,1,1))]}}#action_sub28
-        ],
+		# SCENARIO TOPOLOGY : change or not one sub station among the given list
+		"topo_actions": [
+				{'set_bus':{'substations_id':[(5,(1,1,2,2,1,2,2))]}},#sub5
+				{'set_bus':{'substations_id':[(4,(2,1,2,1,2))]}},#sub4
+				{'set_bus':{'substations_id':[(3,(2,1,1,2,1,2))]}},#sub3
+				{'set_bus':{'substations_id':[(8,(2,1,1,2,2))]}},#sub8
+				{'set_bus':{'substations_id':[(1,(1,2,1,2,2,2))]}}#sub1
+			],
 		"prob_depth": (1.,), # sample from depth 1
 		"prob_type": (1., 0.), # sample only from topo change
 		"prob_do_nothing": 0.3,  # probability of do nothing
-		"max_disc": 0}, # not authorize disconnection
+		"max_disc": 0}, # not authorize additional disconnection
 	"test":{
 		# SCENARIO TOPOLOGY: one sub topo change at each time step
-		"topo_actions": [{'set_bus':{'substations_id':[(26,(2,1,1,2,1,1,1,1,1))]}},#action_sub26
-        {'set_bus':{'substations_id':[(26,(2,2,2,1,2,1,1,1,1))]}},#action_sub26_2
-        {'set_bus':{'substations_id':[(26,(2,2,1,1,2,2,1,1,1))]}},#action_sub26_3
-        {'set_bus':{'substations_id':[(23,(2,2,2,2,1,1,2,2,1,2))]}},#action_sub23
-        {'set_bus':{'substations_id':[(23,(2,2,1,2,1,1,2,2,1,1))]}},#action_sub23_2
-        {'set_bus':{'substations_id':[(23,(2,1,1,1,2,2,2,2,2,2))]}},#action_sub23_3
-        {'set_bus':{'substations_id':[(23,(2,2,1,1,2,2,2,1,2,2))]}},#action_sub23_4
-        {'set_bus':{'substations_id':[(16,(2,1,1,1,2,1,1,1,2,2,2,1,2,1,1,1,2))]}},#action_sub16
-        {'set_bus':{'substations_id':[(16,(2,1,1,2,2,2,2,1,1,2,2,1,1,2,2,1,1))]}},#action_sub16_2
-        {'set_bus':{'substations_id':[(16,(2,2,2,2,2,1,1,2,2,2,1,1,2,2,1,2,1))]}},#action_sub16_3
-        {'set_bus':{'substations_id':[(16,(2,2,2,2,2,1,1,2,2,1,1,2,2,2,1,2,2))]}},#action_sub16_4
-
-        {'set_bus':{'substations_id':[(16,(2,1,1,1,2,2,2,1,2,2,2,1,2,2,2,2,1))]}},#action_sub16_5
-        {'set_bus':{'substations_id':[(16,(2,1,1,2,2,1,1,2,2,2,2,2,1,1,1,1,2))]}},#action_sub16_6
-        {'set_bus':{'substations_id':[(16,(2,2,1,2,2,1,1,2,2,2,2,1,1,2,1,1,2))]}},#action_sub16_7
-        {'set_bus':{'substations_id':[(16,(1,2,2,1,1,2,2,1,1,1,1,1,1,1,1,1,1))]}},#action_sub16_8
-        {'set_bus':{'substations_id':[(16,(1,1,1,1,1,2,2,1,1,2,2,1,1,1,1,1,1))]}},#action_sub16_9
-        {'set_bus':{'substations_id':[(9,(2,2,1,1,1,1,2))]}},#action_sub9
-        {'set_bus':{'substations_id':[(1,(2,2,1,1,2,2))]}},#action_sub1
-        {'set_bus':{'substations_id':[(1,(2,2,1,1,1,2))]}},#action_sub1_2
-        {'set_bus':{'substations_id':[(32,(2,2,1,1,1))]}},#action_sub32
-        {'set_bus':{'substations_id':[(4,(2,1,2,2,2,1))]}},#action_sub4
-        {'set_bus':{'substations_id':[(4,(2,2,2,2,1,1))]}},#action_sub4_2
-        {'set_bus':{'substations_id':[(28,(2,1,2,1,1))]}}#action_sub28
-        ],
+		"topo_actions": [
+				{'set_bus':{'substations_id':[(5,(1,1,2,2,1,2,2))]}},#sub5
+				{'set_bus':{'substations_id':[(4,(2,1,2,1,2))]}},#sub4
+				{'set_bus':{'substations_id':[(3,(2,1,1,2,1,2))]}},#sub3
+				{'set_bus':{'substations_id':[(8,(2,1,1,2,2))]}},#sub8
+				{'set_bus':{'substations_id':[(1,(1,2,1,2,2,2))]}}#sub1
+			],
 		"prob_depth": (1.,), # sample from depth 1
 		"prob_type": (1., 0.), # sample only from topo change
 		"prob_do_nothing": 0.,  # No do nothing
-		"max_disc": 0}, # not authorize disconnection
+		"max_disc": 0}, # not authorize additional disconnection
 	"test_ood":{
 		# SCENARIO TOPOLOGY: two sub topo change at each time step
-		"topo_actions": [{'set_bus':{'substations_id':[(26,(2,1,1,2,1,1,1,1,1))]}},#action_sub26
-        {'set_bus':{'substations_id':[(26,(2,2,2,1,2,1,1,1,1))]}},#action_sub26_2
-        {'set_bus':{'substations_id':[(26,(2,2,1,1,2,2,1,1,1))]}},#action_sub26_3
-        {'set_bus':{'substations_id':[(23,(2,2,2,2,1,1,2,2,1,2))]}},#action_sub23
-        {'set_bus':{'substations_id':[(23,(2,2,1,2,1,1,2,2,1,1))]}},#action_sub23_2
-        {'set_bus':{'substations_id':[(23,(2,1,1,1,2,2,2,2,2,2))]}},#action_sub23_3
-        {'set_bus':{'substations_id':[(23,(2,2,1,1,2,2,2,1,2,2))]}},#action_sub23_4
-        {'set_bus':{'substations_id':[(16,(2,1,1,1,2,1,1,1,2,2,2,1,2,1,1,1,2))]}},#action_sub16
-        {'set_bus':{'substations_id':[(16,(2,1,1,2,2,2,2,1,1,2,2,1,1,2,2,1,1))]}},#action_sub16_2
-        {'set_bus':{'substations_id':[(16,(2,2,2,2,2,1,1,2,2,2,1,1,2,2,1,2,1))]}},#action_sub16_3
-        {'set_bus':{'substations_id':[(16,(2,2,2,2,2,1,1,2,2,1,1,2,2,2,1,2,2))]}},#action_sub16_4
-
-        {'set_bus':{'substations_id':[(16,(2,1,1,1,2,2,2,1,2,2,2,1,2,2,2,2,1))]}},#action_sub16_5
-        {'set_bus':{'substations_id':[(16,(2,1,1,2,2,1,1,2,2,2,2,2,1,1,1,1,2))]}},#action_sub16_6
-        {'set_bus':{'substations_id':[(16,(2,2,1,2,2,1,1,2,2,2,2,1,1,2,1,1,2))]}},#action_sub16_7
-        {'set_bus':{'substations_id':[(16,(1,2,2,1,1,2,2,1,1,1,1,1,1,1,1,1,1))]}},#action_sub16_8
-        {'set_bus':{'substations_id':[(16,(1,1,1,1,1,2,2,1,1,2,2,1,1,1,1,1,1))]}},#action_sub16_9
-        {'set_bus':{'substations_id':[(9,(2,2,1,1,1,1,2))]}},#action_sub9
-        {'set_bus':{'substations_id':[(1,(2,2,1,1,2,2))]}},#action_sub1
-        {'set_bus':{'substations_id':[(1,(2,2,1,1,1,2))]}},#action_sub1_2
-        {'set_bus':{'substations_id':[(32,(2,2,1,1,1))]}},#action_sub32
-        {'set_bus':{'substations_id':[(4,(2,1,2,2,2,1))]}},#action_sub4
-        {'set_bus':{'substations_id':[(4,(2,2,2,2,1,1))]}},#action_sub4_2
-        {'set_bus':{'substations_id':[(28,(2,1,2,1,1))]}}#action_sub28
-        ],
+		"topo_actions": [
+				{'set_bus':{'substations_id':[(5,(1,1,2,2,1,2,2))]}},#sub5
+				{'set_bus':{'substations_id':[(4,(2,1,2,1,2))]}},#sub4
+				{'set_bus':{'substations_id':[(3,(2,1,1,2,1,2))]}},#sub3
+				{'set_bus':{'substations_id':[(8,(2,1,1,2,2))]}},#sub8
+				{'set_bus':{'substations_id':[(1,(1,2,1,2,2,2))]}}#sub1
+			],
 		"prob_depth": (0., 1.), # Sample only from depth 2
 		"prob_type": (1., 0.), # sample only from topo change
 		"prob_do_nothing": 0.,  # No do nothing
-		"max_disc": 0} # Do not authorize disconnection
+		"max_disc": 0} # Do not authorize additional disconnection
 	}
 eval_dict = {
-	"ML": ["MSE_avg", "MAE_avg", "mape_avg", "mape_90_avg", "TIME_INF"],
-	"Physics": ["CURRENT_POS", "VOLTAGE_POS", "LOSS_POS", "DISC_LINES", "CHECK_LOSS", "CHECK_GC", "CHECK_LC", "CHECK_VOLTAGE_EQ"],
+	"ML": ["MSE_avg", "MAE_avg", "MAPE_avg", "MAPE_90_avg", "TIME_INF"],
+	"Physics": ["CURRENT_POS", "VOLTAGE_POS", "LOSS_POS", "DISC_LINES", "CHECK_LOSS", "CHECK_GC", "CHECK_LC", "CHECK_VOLTAGE_EQ", "CHECK_JOULE_LAW"],
 	"IndRed": ["TIME_INF"],
-	"OOD": ["MSE_avg", "MAE_avg", "mape_avg", "mape_90_avg", "TIME_INF"]}
+	"OOD": ["MSE_avg", "MAE_avg", "MAPE_avg", "MAPE_90_avg", "TIME_INF"]}
 eval_params = {
-	"inf_batch_size": 1000,
+	"inf_batch_size": 300,
 	"EL_tolerance": 0.04,
 	"GC_tolerance": 1e-3,
 	"LC_tolerance": 1e-2,
-	"KCL": {"tolerance": 1e-2,
-			"ACTIVE_FLOW": True},
 	"VOLTAGE_EQ": {"tolerance": 1e-4,
-				   "verify_theta": False}
+				   "verify_theta": False},
+	"JOULE_tolerance": 1e-2,
 	}
 
 [Benchmark3]
 attr_x = ("prod_p", "prod_v", "load_p", "load_q")
 attr_tau = ("line_status", "topo_vect")
 attr_y = ("a_or", "a_ex", "p_or", "p_ex", "q_or", "q_ex", "prod_q", "load_v", "v_or", "v_ex", "theta_or", "theta_ex")
 attr_physics = ("YBus", "SBus", "PV_nodes", "slack")
 dataset_create_params = {
 	"train": {
 		# SCENARIO TOPOLOGY: modify subs and disconnect line at maximum depth 4
 		"prob_depth": (.25,.25,.25,.25), # sample from depth 4
 		"prob_type": (.6, .4), # sample from both topo change nad line disc
-		"prob_do_nothing": .03,  # probability of do nothing (included only in train)
+		"prob_do_nothing": .05,  # probability of do nothing (included only in train)
 		"max_disc": 2}, # authorize at most 2 disconnections
 	"test":{
 		# SCENARIO TOPOLOGY: modify subs and disconnect line at maximum depth 4
 		"prob_depth": (.2,.2,.3,.3), # sample from depth 4
 		"prob_type": (.6, .4), # sample from both topo change nad line disc
 		"prob_do_nothing": .0,  # No Donthing
 		"max_disc": 2}, # authorize at most 2 disconnections
 	"test_ood":{
 		# SCENARIO TOPOLOGY: modify subs and disconnect line at maximum depth 5
-		"prob_depth": (0.,0.,0.,.1,.9), # Sample only from depth 5
+		"prob_depth": (0.,0.,0.,.1,.9), # Sample only from depth 2
 		"prob_type": (.6, .4), # sample from both topo change nad line disc
 		"prob_do_nothing": 0, # No Do nothing
 		"max_disc": 2} # authorize at most 2 disconnections
 	}
 eval_dict = {
-	"ML": ["MSE_avg", "MAE_avg", "mape_avg", "mape_90_avg", "TIME_INF"],
-	"Physics": ["CURRENT_POS", "VOLTAGE_POS", "LOSS_POS", "DISC_LINES", "CURRENT_EQ", "CHECK_LOSS", "CHECK_GC", "CHECK_LC", "CHECK_VOLTAGE_EQ"],#, "CHECK_KCL"],
+	"ML": ["MSE_avg", "MAE_avg", "MAPE_avg", "MAPE_90_avg", "TIME_INF"],
+	"Physics": ["CURRENT_POS", "VOLTAGE_POS", "LOSS_POS", "DISC_LINES", "CURRENT_EQ", "CHECK_LOSS", "CHECK_GC", "CHECK_LC", "CHECK_VOLTAGE_EQ", "CHECK_JOULE_LAW", "CHECK_OHM_LAW", "CHECK_KCL"],
 	"IndRed": ["TIME_INF"],
-	"OOD": ["MSE_avg", "MAE_avg", "mape_avg", "mape_90_avg", "TIME_INF"]}
+	"OOD": ["MSE_avg", "MAE_avg", "MAPE_avg", "MAPE_90_avg", "TIME_INF"]}
 eval_params = {
 	"inf_batch_size": 10,
 	"EL_tolerance": 0.04,
 	"GC_tolerance": 1e-3,
 	"LC_tolerance": 1e-2,
-	"KCL": {"tolerance": 1e-2,
-			"ACTIVE_FLOW": True},
 	"VOLTAGE_EQ": {"tolerance": 1e-4,
-				   "verify_theta": True}
+				   "verify_theta": True},
+	"OHM_tolerance": 1e-2,
+	"JOULE_tolerance": 1e-2,
+	"KCL": {"tolerance": 1e-1,
+			"verify_reactive_power": True},
+	}
+
+[Benchmark4]
+attr_x = ("prod_p", "load_p")
+attr_tau = ("line_status", "topo_vect")
+attr_y = ("theta_or", "theta_ex", "p_or", "p_ex")
+attr_physics = ("YBus", "SBus", "PV_nodes", "slack")
+dataset_create_params = {
+	"train": {
+		# SCENARIO TOPOLOGY : disconnect or not one line at each tim step
+		"prob_depth": (1.,), # sample from depth 1
+		"prob_type": (0., 1.), # sample only from line disconnection
+		"prob_do_nothing": 0.3,  # probability of do nothing
+		"max_disc": 1}, # authorize at most 1 disconnection
+	"test":{
+		# SCENARIO TOPOLOGY: disconnect one line at each time step
+		"prob_depth": (1.,), # sample from depth 1
+		"prob_type": (0., 1.), # sample only from line disconnection
+		"prob_do_nothing": 0.,  # No do nothing
+		"max_disc": 1}, # authorize at most 1 disconnection
+	"test_ood":{
+		# SCENARIO TOPOLOGY: disconnect two lines at each time step
+		"prob_depth": (0., 1.), # Sample only from depth 2
+		"prob_type": (0., 1.), # sample only from line disconnection
+		"prob_do_nothing": 0.,  # No do nothing
+		"max_disc": 2} # authorize at most 2 disconnection
+	}
+
+eval_dict = {
+	"ML": ["MSE_avg", "MAE_avg", "MAPE_avg", "MAPE_90_avg", "TIME_INF"],
+	"Physics": ["LOSS_POS"],
+	"IndRed": ["TIME_INF"],
+	"OOD": ["MSE_avg", "MAE_avg", "MAPE_avg", "MAPE_90_avg", "TIME_INF"]}
+
+eval_params = {
+	"inf_batch_size": 14000} # #pas_de_temps=100 x #ligne=20 x #topo=7
+
+# same as benchmark4 with reference actions
+[Benchmark5]
+attr_x = ("prod_p", "load_p")
+attr_tau = ("line_status", "topo_vect")
+attr_y = ("theta_or", "theta_ex", "p_or", "p_ex")
+attr_physics = ("YBus", "SBus", "PV_nodes", "slack")
+dataset_create_params = {
+	# REFERENCE PARAMS
+	"reference_args" : {
+		# "lines_to_disc": [3],
+		# "subs_to_change": [(1,13), (3,8), (4, 3), (8,6)], # (sub_id, action_id)
+		"topo_actions": [
+				{'set_bus':{'substations_id':[(4,(2,1,2,1,2))]}},#sub4
+ 				{'set_bus':{'substations_id':[(1,(1,2,1,2,2,2))]}},#sub1
+				{'set_bus':{'substations_id':[(5,(1,1,2,2,1,2,2))]}}#sub5
+			],
+		"prob_depth": (0.7, 0.3), # authorizing until depth 2 combinations for reference
+		"prob_type": (1., 0.), # only topology change actions
+		"prob_do_nothing": 0.2, # include 20 percent DoNothing actions
+		"max_disc": 0},#no line disconnections
+	"train": {
+		# SCENARIO TOPOLOGY : disconnect or not one line at each tim step
+		"prob_depth": (1.,), # sample from depth 1
+		"prob_type": (0., 1.), # sample only from line disconnection
+		"prob_do_nothing": 0.3,  # probability of do nothing
+		"max_disc": 1}, # authorize at most 1 disconnection
+	"test":{
+		# SCENARIO TOPOLOGY: disconnect one line at each time step
+		"prob_depth": (1.,), # sample from depth 1
+		"prob_type": (0., 1.), # sample only from line disconnection
+		"prob_do_nothing": 0.,  # No do nothing
+		"max_disc": 1}, # authorize at most 1 disconnection
+	"test_ood":{
+		# SCENARIO TOPOLOGY: disconnect two lines at each time step
+		"prob_depth": (0., 1.), # Sample only from depth 2
+		"prob_type": (0., 1.), # sample only from line disconnection
+		"prob_do_nothing": 0.,  # No do nothing
+		"max_disc": 2} # authorize at most 2 disconnection
+	}
+
+eval_dict = {
+	"ML": ["MSE_avg", "MAE_avg", "MAPE_avg", "MAPE_90_avg", "TIME_INF"],
+	"Physics": ["CURRENT_POS"],
+	"IndRed": ["TIME_INF"],
+	"OOD": ["MSE_avg", "MAE_avg", "MAPE_avg", "MAPE_90_avg", "TIME_INF"]}
+
+eval_params = {
+	"inf_batch_size": 14000} # #pas_de_temps=100 x #ligne=20 x #topo=7
+
+[DoNothing]
+attr_x = ("prod_p", "prod_v", "load_p", "load_q")
+attr_tau = ("line_status", "topo_vect")
+attr_y = ("a_or", "a_ex", "p_or", "p_ex", "q_or", "q_ex", "prod_q", "load_v", "v_or", "v_ex", "theta_or", "theta_ex")
+attr_physics = ("YBus", "SBus", "PV_nodes", "slack")
+dataset_create_params = {
+        "train": {},
+        "test": {},
+        "test_ood": {}
+    }
+
+[Benchmark_competition]
+attr_x = ("prod_p", "prod_v", "load_p", "load_q")
+attr_tau = ("line_status", "topo_vect")
+attr_y = ("a_or", "a_ex", "p_or", "p_ex", "v_or", "v_ex", "theta_or", "theta_ex")
+attr_physics = ("YBus", "SBus", "PV_nodes", "slack")
+
+dataset_create_params = {
+	# REFERENCE PARAMS
+	"reference_args" : {
+		# "lines_to_disc": [3],
+		# "subs_to_change": [(1,13), (3,8), (4, 3), (8,6)], # (sub_id, action_id)
+		"topo_actions": [
+				{'set_bus':{'substations_id':[(4,(2,1,2,1,2))]}},#sub4
+ 				{'set_bus':{'substations_id':[(1,(1,2,1,2,2,2))]}},#sub1
+				{'set_bus':{'substations_id':[(5,(1,1,2,2,1,2,2))]}}#sub5
+			],
+		"prob_depth": (0.7, 0.3), # authorizing until depth 2 combinations for reference
+		"prob_type": (1., 0.), # only topology change actions
+		"prob_do_nothing": 0.2, # include 20 percent DoNothing actions
+		"max_disc": 0},#no line disconnections
+	"train": {
+		# SCENARIO TOPOLOGY : disconnect or not one line at each tim step
+		"prob_depth": (1.,), # sample from depth 1
+		"prob_type": (0., 1.), # sample only from line disconnection
+		"prob_do_nothing": 0.3,  # probability of do nothing
+		"max_disc": 1}, # authorize at most 1 disconnection
+	"test":{
+		# SCENARIO TOPOLOGY: disconnect one line at each time step
+		"prob_depth": (1.,), # sample from depth 1
+		"prob_type": (0., 1.), # sample only from line disconnection
+		"prob_do_nothing": 0.,  # No do nothing
+		"max_disc": 1}, # authorize at most 1 disconnection
+	"test_ood":{
+		# SCENARIO TOPOLOGY: disconnect two lines at each time step
+		"prob_depth": (0., 1.), # Sample only from depth 2
+		"prob_type": (0., 1.), # sample only from line disconnection
+		"prob_do_nothing": 0.,  # No do nothing
+		"max_disc": 2} # authorize at most 2 disconnection
+	}
+eval_dict = {
+	"ML": ["MSE_avg", "MAE_avg", "MAPE_avg", "MAPE_90_avg", "MAPE_10_avg", "TIME_INF"],
+	"Physics": ["CURRENT_POS", "VOLTAGE_POS", "LOSS_POS", "DISC_LINES", "CHECK_LOSS", "CHECK_GC", "CHECK_LC", "CHECK_JOULE_LAW"],
+	"IndRed": ["TIME_INF"],
+	"OOD": ["MSE_avg", "MAE_avg", "MAPE_avg", "MAPE_90_avg", "MAPE_10_avg", "TIME_INF"]}
+eval_params = {
+	"inf_batch_size": 14000,
+	"EL_tolerance": 0.04,
+	"GC_tolerance": 1e-3,
+	"LC_tolerance": 1e-2,
+	"JOULE_tolerance": 1e-2,
 	}
+
```

### Comparing `lips-benchmark-0.2.1/lips/tests/configs/powergrid/simulators/tf_leapnet.ini` & `lips-benchmark-0.2.2/lips/tests/configs/powergrid/simulators/tf_leapnet.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/tests/configs/powergrid/simulators/torch_fc.ini` & `lips-benchmark-0.2.2/lips/tests/configs/powergrid/simulators/torch_fc.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips/utils.py` & `lips-benchmark-0.2.2/lips/utils.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/lips_benchmark.egg-info/PKG-INFO` & `lips-benchmark-0.2.2/lips_benchmark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lips-benchmark
-Version: 0.2.1
+Version: 0.2.2
 Summary: LIPS : Learning Industrial Physical Simulation benchmark suite
 Home-page: https://github.com/IRT-SystemX/LIPS
 Author: Milad Leyli-abadi
 Author-email: milad.leyli-abadi@irt-systemx.fr
 License: MPL
 Keywords: Physical system solver,augmented simulator,benchmarking
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lips-benchmark-0.2.1/lips_benchmark.egg-info/SOURCES.txt` & `lips-benchmark-0.2.2/lips_benchmark.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 configurations/pneumatic/benchmarks/confWheel.ini
 configurations/pneumatic/simulators/torch_fc.ini
 configurations/pneumatic/simulators/torch_unet.ini
 configurations/powergrid/readme.md
 configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_Neurips.ipynb
 configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_Sandbox.ipynb
 configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_WCCI_2022.ipynb
+configurations/powergrid/benchmarks/fine_tuning.ini
 configurations/powergrid/benchmarks/l2rpn_case14_sandbox.ini
+configurations/powergrid/benchmarks/l2rpn_idf_2023.ini
 configurations/powergrid/benchmarks/l2rpn_neurips_2020_track1_small.ini
 configurations/powergrid/benchmarks/l2rpn_wcci_2022.ini
 configurations/powergrid/simulators/tf_fc.ini
 configurations/powergrid/simulators/tf_leapnet.ini
 configurations/powergrid/simulators/torch_fc.ini
 configurations/powergrid/simulators/torch_gnn.ini
 lips/__init__.py
@@ -78,14 +80,16 @@
 lips/metrics/ml_metrics/external_metrics.py
 lips/metrics/ml_metrics/mean_absolute_error.py
 lips/metrics/ml_metrics/mean_absolute_percentage_error.py
 lips/metrics/ml_metrics/mean_squared_error.py
 lips/metrics/ml_metrics/metrics.py
 lips/metrics/ml_metrics/normalized_mean_squared_error.py
 lips/metrics/power_grid/__init__.py
+lips/metrics/power_grid/compute_solver_time.py
+lips/metrics/power_grid/compute_solver_time_grid2op.py
 lips/metrics/power_grid/global_conservation.py
 lips/metrics/power_grid/joule_law.py
 lips/metrics/power_grid/kirchhoff_law.py
 lips/metrics/power_grid/local_conservation.py
 lips/metrics/power_grid/ohm_law.py
 lips/metrics/power_grid/physics_compliances.py
 lips/metrics/power_grid/verify_voltage_equality.py
```

### Comparing `lips-benchmark-0.2.1/setup.cfg` & `lips-benchmark-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.1/setup.py` & `lips-benchmark-0.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,38 +31,53 @@
         "scipy<=1.6.0",
         "six",
         "pathlib",
         "numba",
     ],
     "extras": {
         "recommended": [
-            "grid2op==1.8.1", #>=1.7.2",
+            "grid2op==1.9.8", #>=1.7.2",
             "pybind11==2.8.1",
-            "lightsim2grid==0.7.1", #>=0.7.0.post1",
-            #"leap_net @ https://github.com/BDonnot/leap_net/tarball/master#egg=leap_net",
+            "lightsim2grid==0.7.5", #>=0.7.0.post1",
+            "leap-net==0.0.5",
             "protobuf==3.20.1",
             "pandapower==2.7.0",
             "pandas==1.4.2",
             "jupyter",
             "tensorflow==2.8.0",
-            "torch",
+            "torch==2.0.1",
+            "imageio==2.34.0",
+            "plotly==5.20.0"
         ],
         "docs": [
             "numpydoc>=0.9.2",
             "sphinx>=2.4.4",
             "sphinx-rtd-theme>=0.4.3",
             "sphinxcontrib-trio>=1.1.0",
             "autodocsumm>=0.1.13",
             "gym>=0.17.2"
         ],
         "codabench": [
+            "pybind11==2.8.1",
+            "protobuf==3.20.1",
+            "pandapower==2.7.0",
+            "pandas==1.4.2",
+            "jupyter",
+            "tensorflow==2.8.0",
+            "torch==2.0.1",
             "filelock==3.7.1",
             "json2table==1.1.5",
             "loguru==0.6.0",
-            "PyYAML==6.0"
+            "PyYAML==6.0",
+            "Grid2Op==1.9.8",
+            "lightsim2grid==0.7.5",
+            "leap-net==0.0.5",
+            "imageio==2.34.0",
+            "plotly==5.20.0",
+            "tqdm==4.62.3"
         ],
         "test": [
             "pytest",
             "pytest-cov",
             "pytest-html",
             "pytest-metadata",
             "ipykernel",
```

