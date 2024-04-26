# Comparing `tmp/pyatf-0.0.1.tar.gz` & `tmp/pyatf-0.0.2.tar.gz`

## Comparing `pyatf-0.0.1.tar` & `pyatf-0.0.2.tar`

### file list

```diff
@@ -1,53 +1,52 @@
--rw-r--r--   0        0        0    15273 2020-02-02 00:00:00.000000 pyatf-0.0.1/README.md
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 pyatf-0.0.1/examples/feature_demonstration/program_guided_tuning/program_guided_tuning.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 pyatf-0.0.1/examples/feature_demonstration/result_check/result_check.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pyatf-0.0.1/examples/full_examples/bash__gcc_flags/bash__gcc_flags.py
--rwxr-xr-x   0        0        0      151 2020-02-02 00:00:00.000000 pyatf-0.0.1/examples/full_examples/bash__gcc_flags/raytracer/compile_raytracer.sh
--rwxr-xr-x   0        0        0    43080 2020-02-02 00:00:00.000000 pyatf-0.0.1/examples/full_examples/bash__gcc_flags/raytracer/raytracer
--rw-r--r--   0        0        0    10585 2020-02-02 00:00:00.000000 pyatf-0.0.1/examples/full_examples/bash__gcc_flags/raytracer/raytracer.cpp
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pyatf-0.0.1/examples/full_examples/bash__opentuner_matmul/bash__opentuner_matmul.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pyatf-0.0.1/examples/full_examples/bash__opentuner_matmul/mmm_block.cpp
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 pyatf-0.0.1/examples/full_examples/cuda__saxpy/cuda__saxpy.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pyatf-0.0.1/examples/full_examples/opencl__saxpy/opencl__saxpy.py
--rw-r--r--   0        0        0    19051 2020-02-02 00:00:00.000000 pyatf-0.0.1/examples/full_examples/opencl__sgemm/cltune_gemm.cl
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 pyatf-0.0.1/examples/full_examples/opencl__sgemm/opencl__sgemm.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/__init__.py
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/range.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/result_check.py
--rw-r--r--   0        0        0    26618 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/search_space.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/tp.py
--rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/tuner.py
--rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/tuning_data.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/abort_conditions/__init__.py
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/abort_conditions/abort_condition.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/abort_conditions/cost.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/abort_conditions/duration.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/abort_conditions/evaluations.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/abort_conditions/fraction.py
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/abort_conditions/speedup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/cost_functions/__init__.py
--rw-r--r--   0        0        0    17931 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/cost_functions/cuda.py
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/cost_functions/generic.py
--rw-r--r--   0        0        0    14650 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/cost_functions/opencl.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/cost_functions/python.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/search_techniques/__init__.py
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/search_techniques/auc_bandit.py
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/search_techniques/differential_evolution.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/search_techniques/exhaustive.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/search_techniques/opentuner.py
--rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/search_techniques/pattern_search.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/search_techniques/random.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/search_techniques/round_robin.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/search_techniques/search_technique.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/search_techniques/search_technique_1d.py
--rw-r--r--   0        0        0     8375 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/search_techniques/simulated_annealing.py
--rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 pyatf-0.0.1/src/pyatf/search_techniques/torczon.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyatf-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 pyatf-0.0.1/tests/test_range.py
--rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 pyatf-0.0.1/tests/test_search_space.py
--rw-r--r--   0        0        0    15805 2020-02-02 00:00:00.000000 pyatf-0.0.1/tests/test_tuning_data.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pyatf-0.0.1/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 pyatf-0.0.1/LICENSE
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pyatf-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 pyatf-0.0.1/PyPI/README.md
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 pyatf-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    15623 2020-02-02 00:00:00.000000 pyatf-0.0.2/README.md
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/feature_demonstration/program_guided_tuning/program_guided_tuning.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/feature_demonstration/result_check/result_check.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/full_examples/bash__gcc_flags/bash__gcc_flags.py
+-rwxr-xr-x   0        0        0      151 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/full_examples/bash__gcc_flags/raytracer/compile_raytracer.sh
+-rw-r--r--   0        0        0    10585 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/full_examples/bash__gcc_flags/raytracer/raytracer.cpp
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/full_examples/bash__opentuner_matmul/bash__opentuner_matmul.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/full_examples/bash__opentuner_matmul/mmm_block.cpp
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/full_examples/cuda__saxpy/cuda__saxpy.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/full_examples/opencl__saxpy/opencl__saxpy.py
+-rw-r--r--   0        0        0    19051 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/full_examples/opencl__sgemm/cltune_gemm.cl
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/full_examples/opencl__sgemm/opencl__sgemm.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/__init__.py
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/range.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/result_check.py
+-rw-r--r--   0        0        0    26618 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_space.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/tp.py
+-rw-r--r--   0        0        0    13179 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/tuner.py
+-rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/tuning_data.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/abort_conditions/__init__.py
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/abort_conditions/abort_condition.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/abort_conditions/cost.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/abort_conditions/duration.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/abort_conditions/evaluations.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/abort_conditions/fraction.py
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/abort_conditions/speedup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/cost_functions/__init__.py
+-rw-r--r--   0        0        0    20784 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/cost_functions/cuda.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/cost_functions/generic.py
+-rw-r--r--   0        0        0    16487 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/cost_functions/opencl.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/cost_functions/python.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/__init__.py
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/auc_bandit.py
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/differential_evolution.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/exhaustive.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/opentuner.py
+-rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/pattern_search.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/random.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/round_robin.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/search_technique.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/search_technique_1d.py
+-rw-r--r--   0        0        0     8375 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/simulated_annealing.py
+-rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/torczon.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyatf-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 pyatf-0.0.2/tests/test_range.py
+-rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 pyatf-0.0.2/tests/test_search_space.py
+-rw-r--r--   0        0        0    14562 2020-02-02 00:00:00.000000 pyatf-0.0.2/tests/test_tuning_data.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pyatf-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 pyatf-0.0.2/LICENSE
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pyatf-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 pyatf-0.0.2/PyPI/README.md
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 pyatf-0.0.2/PKG-INFO
```

### Comparing `pyatf-0.0.1/README.md` & `pyatf-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   1. *Domain-Specific Language (DSL)*, for auto-tuning at compile time (a.k.a. offline tuning) (discussed [here](https://onlinelibrary.wiley.com/doi/full/10.1002/cpe.4423?casa_token=FO9i0maAi_MAAAAA%3AwSOYWsoqfLqcbazsprmzKkmI5msUCY4An5A7CCwi-_V8u10VdpgejcWuiTwYhWnZpaCJZ3NmXt86sg)); 
   2. *General Purpose Language (GPL)*, for auto-tuning at runtime (a.k.a. online tuning), e.g., of *C++ programs* (referred to as [cppATF](todo), and discussed [here](https://ieeexplore.ieee.org/abstract/document/8291912)) or *Python programs* (referred to as [pyATF](todo)).
 
 **This repository contains *pyATF*, i.e., ATF with its GPL-based *Python interface*.**
 
 ## Documentation
 
-The full documentation is available [here](https://mdh-project.gitlab.io/pyatf).
+The full documentation is available [here](https://atf-tuner.org/pyATF/).
 
 ## Installation
 
 pyATF requires Python 3.9+ and can be installed using `pip`:
 
     pip install pyatf
 
@@ -89,17 +89,17 @@
 
 pyATF's parameter constraints are described in detail [here](https://ieeexplore.ieee.org/abstract/document/8291912).
 
 
 
 ### Step 2: Implement a Cost Function
 
-For high flexibility, the pyATF user can use any arbitrary, self-implemented cost function. 
-pyATF allows as cost function any arbitrary Python function that takes as input a configuration of tuning parameters and returns a value for which operator `<` is defined.
-pyATF interprets the cost function’s return value (e.g., program’s runtime) as the cost that has to be minimized during the auto-tuning process.
+For high flexibility, the pyATF user can use any arbitrary, self-implemented cost function. pyATF allows as a cost function any Python function that takes as input a configuration of tuning parameters and returns a value of type `pyatf.tuning_data.Cost` (currently defined as `float`). pyATF interprets the cost function’s return value as the cost that has to be minimized during the auto-tuning process.
+
+A cost function can raise the error `pyatf.tuning_data.CostFunctionError` if the configuration to measure is invalid (e.g. because the configuration crashes due to too excessive memory usage) — the configuration is then penalized by the search technique (e.g., with a penalty cost). If any other error is raised, the tuning run is aborted by pyATF.
 
 For user’s convenience, pyATF provides pre-implemented cost functions for auto-tuning OpenCL and CUDA kernels in terms of runtime performance, because minimizing the runtime of OpenCL and CUDA applications is becoming increasingly important in the autotuning community.
 
 For our `saxpy` example, we use pyATF's pre-implemented OpenCL cost function `opencl.CostFunction`, as follows:
 
 ```python
 saxpy_kernel = opencl.Kernel( opencl.source(saxpy_kernel_as_string), 'saxpy' )  # kernel's code & name
@@ -157,15 +157,15 @@
   6. `Torczon` 
 
 *Meta Search Techniques:*
 
   1. `RoundRobin`
   2. `AUCBandit` (recommended as default)
 
-Further techniques can be easily added to pyATF by implementing a straightforward [interface](atf/search_techniques/search_technique.py).
+Further techniques can be easily added to pyATF by implementing a straightforward [interface](src/pyatf/search_techniques/search_technique.py).
 
 
 ### Abort Conditions
 
 pyATF currently provides the following, pre-implemented abort conditions:
 
 1. `Duration( timedelta(t) )`: stops exploration after a user-defined time interval `t`; here, `timedelta` is part of Python's [datetime module](https://docs.python.org/3/library/datetime.html) and thus `t` can be `hours=2` or `hours=2,minutes=30`, etc.;
@@ -180,15 +180,15 @@
 		
 6. `Speedup( s,n )`: stops when within the last `n` tested configurations the cost could not be lowered by a factor `>=s`.
 
 If no abort condition is set, pyATF uses `Evaluations( S )`, where `S` is the search space size.
 
 To meet complex user requirements, abort conditions can be combined by using the logical operators `And` and `Or`, e.g., `Or( Evaluations(100) , Duration(minutes=5) )` to stop tuning after 100 evaluations or 5 minutes, whichever comes first.
 
-New abort conditions can be easily added to pyATF by implementing the corresponding [interface](atf/abort_conditions/abort_condition.py).
+New abort conditions can be easily added to pyATF by implementing the corresponding [interface](src/pyatf/abort_conditions/abort_condition.py).
 
 
 
 ## Experimental Results
 
 We present experimental results (discussed in detail [here](https://dl.acm.org/doi/abs/10.1145/3427093)) for [MDH-based auto-tunable computations](https://ieeexplore.ieee.org/abstract/document/8891668?casa_token=mFNVnD2FYXMAAAAA:1DvXQy-Rl1Tm2eiYjaImBEylR0u-eHm-TbtyRs_yIgTdPKVpe5NhsPS-H414i0_ToRfVZyBdexsB) from popular domains:
 *Stencil*,
```

### Comparing `pyatf-0.0.1/examples/feature_demonstration/program_guided_tuning/program_guided_tuning.py` & `pyatf-0.0.2/examples/feature_demonstration/program_guided_tuning/program_guided_tuning.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,11 +30,11 @@
 
 # Steps 2 & 3: Program-Guided Search Space Exploration
 tuner = Tuner().tuning_parameters( CACHE_BLOCK_SIZE )  \
                .search_technique( AUCBandit() )
 
 data = np.random.rand( N+3,N+3 ).astype(np.float32)
 
-gaussian_cf = python.CostFunction(TunableGaussian)( data, N )
+cf_gaussian = python.CostFunction(TunableGaussian)( data, N )
 
 for _ in range(8):
-    tuner.make_step( gaussian_cf )
+    tuner.make_step( cf_gaussian )
```

### Comparing `pyatf-0.0.1/examples/feature_demonstration/result_check/result_check.py` & `pyatf-0.0.2/examples/feature_demonstration/result_check/result_check.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/examples/full_examples/bash__gcc_flags/bash__gcc_flags.py` & `pyatf-0.0.2/examples/full_examples/bash__gcc_flags/bash__gcc_flags.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 align_functions      = TP('align_functions',      Set( '-falign-functions', '-fno-align-functions' ) )
 early_inlining_insns = TP('early_inlining_insns', Interval( 0, 1000 )                                )
 
 # Step 2: Implement a Cost Function
 run_command     = './raytracer/raytracer'
 compile_command = './raytracer/compile_raytracer.sh'
 
-generic_cf = generic.CostFunction(run_command).compile_command(compile_command)
+cf_raytracer = generic.CostFunction(run_command).compile_command(compile_command)
 
 # Step 3: Explore the Search Space
 tuning_result = Tuner().tuning_parameters( opt_level, align_functions, early_inlining_insns )  \
                        .search_technique( AUCBandit() )                                        \
-                       .tune( generic_cf, Duration(timedelta(minutes=5)) )
+                       .tune( cf_raytracer, Duration(timedelta(minutes=5)) )
```

### Comparing `pyatf-0.0.1/examples/full_examples/bash__gcc_flags/raytracer/raytracer.cpp` & `pyatf-0.0.2/examples/full_examples/bash__gcc_flags/raytracer/raytracer.cpp`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/examples/full_examples/bash__opentuner_matmul/mmm_block.cpp` & `pyatf-0.0.2/examples/full_examples/bash__opentuner_matmul/mmm_block.cpp`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/examples/full_examples/cuda__saxpy/cuda__saxpy.py` & `pyatf-0.0.2/examples/full_examples/cuda__saxpy/cuda__saxpy.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/examples/full_examples/opencl__saxpy/opencl__saxpy.py` & `pyatf-0.0.2/examples/full_examples/opencl__saxpy/opencl__saxpy.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/examples/full_examples/opencl__sgemm/cltune_gemm.cl` & `pyatf-0.0.2/examples/full_examples/opencl__sgemm/cltune_gemm.cl`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/examples/full_examples/opencl__sgemm/opencl__sgemm.py` & `pyatf-0.0.2/examples/full_examples/opencl__sgemm/opencl__sgemm.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/range.py` & `pyatf-0.0.2/src/pyatf/range.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/search_space.py` & `pyatf-0.0.2/src/pyatf/search_space.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/tp.py` & `pyatf-0.0.2/src/pyatf/tp.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/tuner.py` & `pyatf-0.0.2/src/pyatf/tuner.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             if isinstance(self._search_technique, SearchTechnique):
                 self._get_next_coordinates_or_indices = self._search_technique.get_next_coordinates
                 self._coordinates_or_index_param_name = 'search_space_coordinates'
             else:
                 self._get_next_coordinates_or_indices = self._search_technique.get_next_indices
                 self._coordinates_or_index_param_name = 'search_space_index'
             self._coordinates_or_indices: Set[Union[Coordinates, Index]] = set()
-            self._costs: Dict[Coordinates, Union[Coordinates, Index]] = {}
+            self._costs: Dict[Union[Coordinates, Index], Cost] = {}
 
             # generate search space
             search_space_generation_start = time.perf_counter_ns()
             self._search_space = SearchSpace(*tps,
                                              enable_1d_access=isinstance(self._search_technique, SearchTechnique1D),
                                              silent=silent)
             search_space_generation_end = time.perf_counter_ns()
@@ -184,26 +184,24 @@
 
             # get configuration
             coords_or_index = self._coordinates_or_indices.pop()
             config = self._search_space.get_configuration(coords_or_index)
 
             # run cost function
             valid = True
-            meta_data = None
-            cost = None
             try:
-                cost_function_return_values = self._cost_function(config)
-                if isinstance(cost_function_return_values, tuple):
-                    cost, meta_data = cost_function_return_values
-                else:
-                    cost = cost_function_return_values
+                cost = self._cost_function(config)
             except CostFunctionError as e:
-                meta_data = e.meta_data
+                if not self._silent:
+                    print('\r' + ' ' * self._last_line_length + '\r', end='')
+                    print('Error raised: ' + e.message)
+                    self._last_line_length = 0
+                cost = None
                 valid = False
-            timestamp = self._tuning_data.record_evaluation(config, valid, cost, meta_data, **{
+            timestamp = self._tuning_data.record_evaluation(config, valid, cost, **{
                 self._coordinates_or_index_param_name: coords_or_index
             })
             self._costs[coords_or_index] = cost
 
             # print progress and dump log file (at most once every 5 minutes)
             if not self._silent:
                 self._print_progress(timestamp, cost)
@@ -259,27 +257,27 @@
 
     def log_file(self, log_file: str):
         if self._tuning_run is not None:
             raise ValueError('cannot change log file while tuning')
         self._log_file = log_file
         return self
 
-    def make_step(self, cost_function: CostFunction, progress: float = None):
+    def make_step(self, cost_function: CostFunction):
         if self._tuning_run is None:
             # create & initialize tuning run
             self._tuning_run = Tuner.TuningRun(
                 self._tps,
                 cost_function,
                 self._search_technique,
                 self._silent,
                 self._log_file,
                 None
             )
             self._tuning_run.initialize()
-        if cost_function != self._tuning_run.cost_function:
+        if cost_function is not self._tuning_run.cost_function:
             raise ValueError('a tuning run with another cost function is already in progress')
         self._tuning_run.make_step()
 
     def get_tuning_data(self):
         if self._tuning_run is None:
             raise ValueError('cannot get tuning data, because no tuning run is in progress')
         return self._tuning_run.tuning_data
```

### Comparing `pyatf-0.0.1/src/pyatf/tuning_data.py` & `pyatf-0.0.2/src/pyatf/tuning_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 import copy
 import time
 from datetime import timedelta, datetime
 from math import ceil
-from typing import Any, Dict, Optional, Tuple, Callable, List, Union
+from typing import Any, Dict, Optional, Tuple, Callable, List
 
 Configuration = Dict[str, Any]
 
 Cost = float
-MetaData = Dict[str, Any]
+CostFunction = Callable[[Configuration], Cost]
 
-# CostFunction returns Cost for a given Configuration and optional meta-data for logging purposes as a dictionary
-CostFunction = Callable[[Configuration], Union[Cost, Tuple[Cost, MetaData]]]
 
-
-# Error to be thrown in cost functions, when additional meta-data was collected
+# Error to be thrown in cost functions, when the configuration is expected to be interpreted as invalid
 class CostFunctionError(BaseException):
-    def __init__(self, meta_data: MetaData):
-        self.meta_data: MetaData = copy.deepcopy(meta_data)
+    def __init__(self, message):
+        self.message = message
 
 
 Coordinates = Tuple[float, ...]
 Index = int
 
 
 class History:
     class Entry:
         def __init__(self, timestamp: datetime, timedelta_since_tuning_start: timedelta,
                      evaluations: int, valid_evaluations: int,
                      configuration: Configuration, valid: bool, cost: Optional[Cost] = None,
-                     meta_data: Optional[Dict] = None,
                      search_space_coordinates: Optional[Coordinates] = None,
                      search_space_index: Optional[Index] = None):
             self._timestamp = timestamp
             self._timedelta_since_tuning_start = timedelta_since_tuning_start
             self._evaluations = evaluations
             self._valid_evaluations = valid_evaluations
             self._configuration = configuration.copy()
             self._valid = valid
             self._cost = cost
-            self._meta_data = copy.deepcopy(meta_data)
             self._search_space_coordinates = search_space_coordinates
             self._search_space_index = search_space_index
 
         @property
         def timestamp(self):
             return self._timestamp
 
@@ -67,18 +62,14 @@
             return self._valid
 
         @property
         def cost(self):
             return self._cost
 
         @property
-        def meta_data(self):
-            return self._meta_data
-
-        @property
         def search_space_coordinates(self):
             return self._search_space_coordinates
 
         @property
         def search_space_index(self):
             return self._search_space_index
 
@@ -93,16 +84,14 @@
                 'timedelta_since_tuning_start': timedelta_since_tuning_start_str,
                 'evaluations': self._evaluations,
                 'valid_evaluations': self._valid_evaluations,
                 'configuration': copy.deepcopy(self._configuration),
                 'valid': self._valid,
                 'cost': self._cost
             }
-            if self._meta_data is not None:
-                json['meta_data'] = copy.deepcopy(self._meta_data)
             if self._search_space_coordinates is not None:
                 json['search_space_coordinates'] = self._search_space_coordinates
             if self._search_space_index is not None:
                 json['search_space_index'] = self._search_space_index
             return json
 
     def __init__(self):
@@ -169,20 +158,14 @@
 
     def configuration_of_min_cost(self):
         if self.improvement_history.is_empty():
             return None
         else:
             return self.improvement_history[-1].configuration
 
-    def meta_data_of_min_cost(self):
-        if self.improvement_history.is_empty():
-            return None
-        else:
-            return self.improvement_history[-1].meta_data
-
     def search_space_coordinates_of_min_cost(self):
         if self.improvement_history.is_empty():
             return None
         else:
             return self.improvement_history[-1].search_space_coordinates
 
     def search_space_index_of_min_cost(self):
@@ -212,15 +195,14 @@
     def valid_evaluations_to_min_cost(self):
         if self.improvement_history.is_empty():
             return None
         else:
             return self.improvement_history[-1].valid_evaluations
 
     def record_evaluation(self, configuration: Configuration, valid: bool, cost: Optional[Cost] = None,
-                          meta_data: Optional[Dict] = None,
                           search_space_coordinates: Optional[Coordinates] = None,
                           search_space_index: Optional[Index] = None) -> datetime:
         now = self.tuning_start_timestamp + timedelta(
             microseconds=(time.perf_counter_ns() - self._tuning_start_perf_counter) / 1000
         )
         if valid and cost is None:
             raise ValueError('expecting cost if valid is True')
@@ -236,15 +218,14 @@
             now,
             now - self.tuning_start_timestamp,
             self.number_of_evaluated_configurations,
             self.number_of_evaluated_valid_configurations,
             configuration,
             valid,
             cost,
-            meta_data,
             search_space_coordinates,
             search_space_index
         )
         self.history.append(entry)
         new_best = valid and (self.improvement_history.is_empty() or cost < self.improvement_history[-1].cost)
         if new_best:
             self.improvement_history.append(entry)
@@ -286,15 +267,14 @@
             'history': self.history.to_json(),
             'improvement_history': self.improvement_history.to_json(),
             'number_of_evaluated_configurations': self.number_of_evaluated_configurations,
             'number_of_evaluated_valid_configurations': self.number_of_evaluated_valid_configurations,
             'number_of_evaluated_invalid_configurations': self.number_of_evaluated_invalid_configurations,
             'min_cost': self.min_cost(),
             'configuration_of_min_cost': copy.deepcopy(self.configuration_of_min_cost()),
-            'meta_data_of_min_cost': copy.deepcopy(self.meta_data_of_min_cost()),
             'search_space_coordinates_of_min_cost': self.search_space_coordinates_of_min_cost(),
             'search_space_index_of_min_cost': self.search_space_index_of_min_cost(),
             'timestamp_of_min_cost': timestamp_of_min_cost_str,
             'duration_to_min_cost': duration_to_min_cost_str,
             'evaluations_to_min_cost': self.evaluations_to_min_cost(),
             'valid_evaluations_to_min_cost': self.valid_evaluations_to_min_cost()
         }
```

### Comparing `pyatf-0.0.1/src/pyatf/abort_conditions/abort_condition.py` & `pyatf-0.0.2/src/pyatf/abort_conditions/abort_condition.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/abort_conditions/duration.py` & `pyatf-0.0.2/src/pyatf/abort_conditions/duration.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/abort_conditions/evaluations.py` & `pyatf-0.0.2/src/pyatf/abort_conditions/evaluations.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/abort_conditions/fraction.py` & `pyatf-0.0.2/src/pyatf/abort_conditions/fraction.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/abort_conditions/speedup.py` & `pyatf-0.0.2/src/pyatf/abort_conditions/speedup.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/cost_functions/cuda.py` & `pyatf-0.0.2/src/pyatf/cost_functions/cuda.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import csv
 import inspect
 import time
 from math import ceil
-from typing import Union, Tuple, Callable, Optional, Set, Dict, Iterable, Any
+from typing import Union, Tuple, Callable, Optional, Set, Dict, Iterable, Any, TextIO
 
 import numpy
 from cuda import cuda, nvrtc
 
 from pyatf.result_check import equality
-from pyatf.tuning_data import Configuration, Cost, MetaData, CostFunctionError
+from pyatf.tuning_data import Configuration, Cost, CostFunctionError
 
 cuda.cuInit(0)
 
 
 def source(source: str):
     return source
 
@@ -41,16 +42,26 @@
     @property
     def flags(self):
         return self._flags
 
 
 Input = Union[numpy.ndarray, numpy.generic]
 
+_LOG_FILE_COLUMNS = ('compile_time_ns',
+                     'cuda_error',
+                     'nvrtc_error',
+                     'gold_check',
+                     'checked_inputs')
+
 
 class CostFunction:
+    class _CUDAError(BaseException):
+        def __init__(self, message: str):
+            self.message = message
+
     def __init__(self, kernel: Kernel):
         self._kernel = kernel
 
         self._silent: bool = False
         self._device_id: Optional[int] = None
 
         self._inputs: Dict[int, Input] = {}
@@ -66,69 +77,73 @@
         self._block_dim_y: Union[int, Callable[..., int]] = 1
         self._block_dim_y_tps: Optional[Set[str, ...]] = None
         self._block_dim_z: Union[int, Callable[..., int]] = 1
         self._block_dim_z_tps: Optional[Set[str, ...]] = None
 
         self._gold_data: Dict[int, Tuple[Input, Callable[[numpy.generic, numpy.generic], bool]]] = {}
         self._gold_cmp_buffer: Dict[int, Input] = {}
+        self._abort_on_invalid_results: bool = False
+
+        self._abort_on_cuda_error: bool = False
 
         self._warmups: int = 0
         self._evaluations: int = 1
 
+        self._log_file: Optional[TextIO] = None
+        self._log_file_writer = None
+
         self._objects_to_free_on_error: Dict[Any, Callable] = {}
         self._cu_device: Optional[cuda.CUdevice] = None
         self._cu_context: Optional[cuda.CUcontext] = None
         self._cu_stream: Optional[cuda.CUstream] = None
         self._cu_device_ptr: Dict[int, cuda.CUdeviceptr] = {}
 
     def _free_objects_before_error(self):
         for obj, free_method in self._objects_to_free_on_error.items():
             free_method(obj)
         self._objects_to_free_on_error.clear()
 
     def _safe_call(
             self,
             returns: Union[cuda.CUresult, nvrtc.nvrtcResult, Tuple[Union[cuda.CUresult, nvrtc.nvrtcResult], ...]],
-            message: str, meta_data: Optional[MetaData] = None
+            message: str, meta_data: Dict[str, Any] = None
     ):
         if isinstance(returns, tuple):
             err = returns[0]
             returns = returns[1:]
         else:
             err = returns
-        raise_error = False
         if isinstance(err, cuda.CUresult):
             if err != cuda.CUresult.CUDA_SUCCESS:
                 if meta_data is not None:
-                    meta_data['cuda_error'] = str(err)
-                raise_error = True
+                    meta_data['cuda_error'] = err
+                raise CostFunction._CUDAError(f'CUDA failed with error: {err}\n{message}')
         elif isinstance(err, nvrtc.nvrtcResult):
             if err != nvrtc.nvrtcResult.NVRTC_SUCCESS:
                 if meta_data is not None:
-                    meta_data['nvrtc_error'] = str(err)
-                raise_error = True
+                    meta_data['nvrtc_error'] = err
+                raise CostFunction._CUDAError(f'CUDA failed with error: {err}\n{message}')
         else:
-            raise_error = True
-        if raise_error:
-            self._free_objects_before_error()
-            if meta_data is not None:
-                raise CostFunctionError(meta_data)
-            else:
-                raise ValueError(f'CUDA failed with error: {err}\n{message}')
+            raise RuntimeError(str(err))
         if len(returns) == 1:
             return returns[0]
         else:
             return returns
 
     def __del__(self):
         self._free_buffers()
         self._free_device()
+        if self._log_file:
+            self._log_file_writer = None
+            self._log_file.close()
+            self._log_file = None
 
     def silent(self, silent: bool):
         self._silent = silent
+        return self
 
     def device_id(self, device_id: int):
         self._free_buffers()
         self._free_device()
         self._device_id = device_id
         self._init_device()
         self._alloc_buffers()
@@ -189,185 +204,228 @@
             self._gold_cmp_buffer[index] = gold_data_or_callable.copy()
         else:
             gold_buffer = gold_data_or_callable(*self._inputs.values())
             self._gold_data[index] = (gold_buffer, comparator)
             self._gold_cmp_buffer[index] = gold_buffer.copy()
         return self
 
+    def abort_on_invalid_results(self, abort_on_invalid_results: bool):
+        self._abort_on_invalid_results = abort_on_invalid_results
+        return self
+
+    def abort_on_cuda_error(self, abort_on_cuda_error: bool):
+        self._abort_on_cuda_error = abort_on_cuda_error
+        return self
+
     def warmups(self, warmups: int):
         self._warmups = warmups
+        return self
 
     def evaluations(self, evaluations: int):
         self._evaluations = evaluations
+        return self
+
+    def log_file(self, log_file_path: str):
+        if self._log_file:
+            self._log_file_writer = None
+            self._log_file.close()
+            self._log_file = None
+        if log_file_path:
+            self._log_file = open(log_file_path, 'w')
+            self._log_file_writer = csv.writer(self._log_file)
+            self._log_file_writer.writerow(_LOG_FILE_COLUMNS)
+        return self
 
-    def __call__(self, configuration: Configuration) -> Tuple[Cost, MetaData]:
+    def __call__(self, configuration: Configuration) -> Cost:
         if self._device_id is None:
             raise ValueError('no CUDA device was selected')
 
-        meta_data = {}
+        meta_data: Dict[str, Any] = {c: None for c in _LOG_FILE_COLUMNS}
 
-        # create & compile program
-        nvrtc_program = self._safe_call(nvrtc.nvrtcCreateProgram(str.encode(self._kernel.source),
-                                                                 str.encode(self._kernel.name + '.cu'),
-                                                                 0, [], []),
-                                        'failed to create NVRTC program', meta_data)
-        self._objects_to_free_on_error[nvrtc_program] = nvrtc.nvrtcDestroyProgram
-        opts = []
-        for flag in self._kernel.flags:
-            opts.append(str.encode(flag))
-        for tp_name, tp_value in configuration.items():
-            opts.append(str.encode(f'-D{tp_name}={tp_value}'))
-        compile_start_ns = time.perf_counter_ns()
-        self._safe_call(nvrtc.nvrtcCompileProgram(nvrtc_program, len(opts), opts), 'failed to compile NVRTC program',
-                        meta_data)
-        compile_end_ns = time.perf_counter_ns()
-        meta_data['compile_time_ns'] = compile_end_ns - compile_start_ns
-        ptx_size = self._safe_call(nvrtc.nvrtcGetPTXSize(nvrtc_program), 'failed to get PTX size',
-                                   meta_data)
-        ptx = b' ' * ptx_size
-        self._safe_call(nvrtc.nvrtcGetPTX(nvrtc_program, ptx), 'failed to get PTX code',
-                        meta_data)
-
-        # load PTX as module and retrieve function
-        ptx = numpy.char.array(ptx)
-        module = self._safe_call(cuda.cuModuleLoadData(ptx.ctypes.data), 'failed to load PTX',
-                                 meta_data)
-        self._objects_to_free_on_error[module] = cuda.cuModuleUnload
-        kernel = self._safe_call(cuda.cuModuleGetFunction(module, str.encode(self._kernel.name)),
-                                 'failed to get module function', meta_data)
-
-        # calculate grid and block dim
-        grid_dim = [1, 1, 1]
-        if self._grid_dim_x_tps is None:
-            grid_dim[0] = self._grid_dim_x
-        else:
-            grid_dim[0] = int(self._grid_dim_x(**{
-                tp_name: configuration[tp_name] for tp_name in self._grid_dim_x_tps
-            }))
-        if self._grid_dim_y_tps is None:
-            grid_dim[1] = self._grid_dim_y
-        else:
-            grid_dim[1] = int(self._grid_dim_y(**{
-                tp_name: configuration[tp_name] for tp_name in self._grid_dim_y_tps
-            }))
-        if self._grid_dim_z_tps is None:
-            grid_dim[2] = self._grid_dim_z
-        else:
-            grid_dim[2] = int(self._grid_dim_z(**{
-                tp_name: configuration[tp_name] for tp_name in self._grid_dim_z_tps
-            }))
-        block_dim = [1, 1, 1]
-        if self._block_dim_x_tps is None:
-            block_dim[0] = self._block_dim_x
-        else:
-            block_dim[0] = int(self._block_dim_x(**{
-                tp_name: configuration[tp_name] for tp_name in self._block_dim_x_tps
-            }))
-        if self._block_dim_y_tps is None:
-            block_dim[1] = self._block_dim_y
-        else:
-            block_dim[1] = int(self._block_dim_y(**{
-                tp_name: configuration[tp_name] for tp_name in self._block_dim_y_tps
-            }))
-        if self._block_dim_z_tps is None:
-            block_dim[2] = self._block_dim_z
-        else:
-            block_dim[2] = int(self._block_dim_z(**{
-                tp_name: configuration[tp_name] for tp_name in self._block_dim_z_tps
-            }))
-
-        # prepare kernel arguments
-        args = []
-        for idx, inp in self._inputs.items():
-            if isinstance(inp, numpy.ndarray):
-                args.append(numpy.array([int(self._cu_device_ptr[idx])], dtype=numpy.uint64))
+        try:
+            # create & compile program
+            nvrtc_program = self._safe_call(nvrtc.nvrtcCreateProgram(str.encode(self._kernel.source),
+                                                                     str.encode(self._kernel.name + '.cu'),
+                                                                     0, [], []),
+                                            'failed to create NVRTC program', meta_data)
+            self._objects_to_free_on_error[nvrtc_program] = nvrtc.nvrtcDestroyProgram
+            opts = []
+            for flag in self._kernel.flags:
+                opts.append(str.encode(flag))
+            for tp_name, tp_value in configuration.items():
+                opts.append(str.encode(f'-D{tp_name}={tp_value}'))
+            compile_start_ns = time.perf_counter_ns()
+            self._safe_call(nvrtc.nvrtcCompileProgram(nvrtc_program, len(opts), opts),
+                            'failed to compile NVRTC program', meta_data)
+            compile_end_ns = time.perf_counter_ns()
+            meta_data['compile_time_ns'] = compile_end_ns - compile_start_ns
+            ptx_size = self._safe_call(nvrtc.nvrtcGetPTXSize(nvrtc_program),
+                                       'failed to get PTX size', meta_data)
+            ptx = b' ' * ptx_size
+            self._safe_call(nvrtc.nvrtcGetPTX(nvrtc_program, ptx),
+                            'failed to get PTX code', meta_data)
+
+            # load PTX as module and retrieve function
+            ptx = numpy.char.array(ptx)
+            module = self._safe_call(cuda.cuModuleLoadData(ptx.ctypes.data),
+                                     'failed to load PTX', meta_data)
+            self._objects_to_free_on_error[module] = cuda.cuModuleUnload
+            kernel = self._safe_call(cuda.cuModuleGetFunction(module, str.encode(self._kernel.name)),
+                                     'failed to get module function', meta_data)
+
+            # calculate grid and block dim
+            grid_dim = [1, 1, 1]
+            if self._grid_dim_x_tps is None:
+                grid_dim[0] = self._grid_dim_x
             else:
-                args.append(numpy.array([inp], dtype=inp.dtype))
-        args = numpy.array([arg.ctypes.data for arg in args], dtype=numpy.uint64)
-
-        # warmups
-        for _ in range(self._warmups):
-            self._cpy_to_device()
-            self._safe_call(cuda.cuLaunchKernel(kernel, *grid_dim, *block_dim, 0, self._cu_stream, args.ctypes.data, 0),
-                            'failed to launch kernel', meta_data)
-
-        # evaluations
-        avg_runtime = 0.0
-        for e in range(self._evaluations):
-            self._cpy_to_device()
-            pre_kernel_event = self._safe_call(cuda.cuEventCreate(0), 'failed to create pre-kernel event', meta_data)
-            self._objects_to_free_on_error[pre_kernel_event] = cuda.cuEventDestroy
-            post_kernel_event = self._safe_call(cuda.cuEventCreate(0), 'failed to create post-kernel event', meta_data)
-            self._objects_to_free_on_error[post_kernel_event] = cuda.cuEventDestroy
-            self._safe_call(cuda.cuEventRecord(pre_kernel_event, self._cu_stream),
-                            'failed to record pre-kernel event', meta_data)
-            self._safe_call(cuda.cuLaunchKernel(kernel, *grid_dim, *block_dim, 0, self._cu_stream, args.ctypes.data, 0),
-                            'failed to launch kernel', meta_data)
-            self._safe_call(cuda.cuEventRecord(post_kernel_event, self._cu_stream),
-                            'failed to record post-kernel event', meta_data)
-            self._safe_call(cuda.cuEventSynchronize(post_kernel_event),
-                            'failed to synchronize with post-kernel event', meta_data)
-            avg_runtime += self._safe_call(cuda.cuEventElapsedTime(pre_kernel_event, post_kernel_event),
-                                           'failed to get elapsed time between kernel events', meta_data) * 1000000
-            del self._objects_to_free_on_error[post_kernel_event]
-            self._safe_call(cuda.cuEventDestroy(post_kernel_event),
-                            'failed to destroy post-kernel event', meta_data)
-            del self._objects_to_free_on_error[pre_kernel_event]
-            self._safe_call(cuda.cuEventDestroy(pre_kernel_event),
-                            'failed to destroy pre-kernel event', meta_data)
-            # result check
-            if e == 0 and self._gold_data:
-                self._cpy_to_host(self._gold_cmp_buffer)
-                for idx, (gold_values, comparator) in self._gold_data.items():
-                    result_values = self._gold_cmp_buffer[idx]
-                    if result_values.size != gold_values.size:
-                        meta_data['result_check'] = {
-                            'status': 'failed',
-                            'input': idx,
-                            'reason': 'result size is not equal to gold size'
-                        }
-                        self._free_objects_before_error()
-                        raise CostFunctionError(meta_data)
-                    for value_idx, (result_value, gold_value) in enumerate(zip(result_values, gold_values)):
-                        if not comparator(result_value, gold_value):
-                            meta_data['result_check'] = {
-                                'status': 'failed',
-                                'input': idx,
-                                'position': value_idx,
-                                'expected': str(gold_value),
-                                'actual': str(result_value)
-                            }
-                            self._free_objects_before_error()
-                            raise CostFunctionError(meta_data)
-                meta_data['result_check'] = {'status': 'success', 'checked_inputs': tuple(self._gold_data.keys())}
-        avg_runtime /= self._evaluations
-        avg_runtime = float(ceil(avg_runtime))  # runtime can be ceiled, since nanoseconds are precise enough
-
-        # free program resources
-        del self._objects_to_free_on_error[module]
-        self._safe_call(cuda.cuModuleUnload(module), 'failed to unload module', meta_data)
-        del self._objects_to_free_on_error[nvrtc_program]
-        self._safe_call(nvrtc.nvrtcDestroyProgram(nvrtc_program), 'failed to destroy NVRTC program', meta_data)
+                grid_dim[0] = int(self._grid_dim_x(**{
+                    tp_name: configuration[tp_name] for tp_name in self._grid_dim_x_tps
+                }))
+            if self._grid_dim_y_tps is None:
+                grid_dim[1] = self._grid_dim_y
+            else:
+                grid_dim[1] = int(self._grid_dim_y(**{
+                    tp_name: configuration[tp_name] for tp_name in self._grid_dim_y_tps
+                }))
+            if self._grid_dim_z_tps is None:
+                grid_dim[2] = self._grid_dim_z
+            else:
+                grid_dim[2] = int(self._grid_dim_z(**{
+                    tp_name: configuration[tp_name] for tp_name in self._grid_dim_z_tps
+                }))
+            block_dim = [1, 1, 1]
+            if self._block_dim_x_tps is None:
+                block_dim[0] = self._block_dim_x
+            else:
+                block_dim[0] = int(self._block_dim_x(**{
+                    tp_name: configuration[tp_name] for tp_name in self._block_dim_x_tps
+                }))
+            if self._block_dim_y_tps is None:
+                block_dim[1] = self._block_dim_y
+            else:
+                block_dim[1] = int(self._block_dim_y(**{
+                    tp_name: configuration[tp_name] for tp_name in self._block_dim_y_tps
+                }))
+            if self._block_dim_z_tps is None:
+                block_dim[2] = self._block_dim_z
+            else:
+                block_dim[2] = int(self._block_dim_z(**{
+                    tp_name: configuration[tp_name] for tp_name in self._block_dim_z_tps
+                }))
+
+            # prepare kernel arguments
+            args = []
+            for idx, inp in self._inputs.items():
+                if isinstance(inp, numpy.ndarray):
+                    args.append(numpy.array([int(self._cu_device_ptr[idx])], dtype=numpy.uint64))
+                else:
+                    args.append(numpy.array([inp], dtype=inp.dtype))
+            args = numpy.array([arg.ctypes.data for arg in args], dtype=numpy.uint64)
+
+            # warmups
+            for _ in range(self._warmups):
+                self._cpy_to_device()
+                self._safe_call(cuda.cuLaunchKernel(kernel, *grid_dim, *block_dim, 0,
+                                                    self._cu_stream, args.ctypes.data, 0),
+                                'failed to launch kernel', meta_data)
+
+            # evaluations
+            avg_runtime = 0.0
+            for e in range(self._evaluations):
+                self._cpy_to_device()
+                pre_kernel_event = self._safe_call(cuda.cuEventCreate(0),
+                                                   'failed to create pre-kernel event', meta_data)
+                self._objects_to_free_on_error[pre_kernel_event] = cuda.cuEventDestroy
+                post_kernel_event = self._safe_call(cuda.cuEventCreate(0),
+                                                    'failed to create post-kernel event', meta_data)
+                self._objects_to_free_on_error[post_kernel_event] = cuda.cuEventDestroy
+                self._safe_call(cuda.cuEventRecord(pre_kernel_event, self._cu_stream),
+                                'failed to record pre-kernel event', meta_data)
+                self._safe_call(cuda.cuLaunchKernel(kernel, *grid_dim, *block_dim, 0,
+                                                    self._cu_stream, args.ctypes.data, 0),
+                                'failed to launch kernel', meta_data)
+                self._safe_call(cuda.cuEventRecord(post_kernel_event, self._cu_stream),
+                                'failed to record post-kernel event', meta_data)
+                self._safe_call(cuda.cuEventSynchronize(post_kernel_event),
+                                'failed to synchronize with post-kernel event', meta_data)
+                avg_runtime += self._safe_call(cuda.cuEventElapsedTime(pre_kernel_event, post_kernel_event),
+                                               'failed to get elapsed time between kernel events', meta_data) * 1000000
+                del self._objects_to_free_on_error[post_kernel_event]
+                self._safe_call(cuda.cuEventDestroy(post_kernel_event),
+                                'failed to destroy post-kernel event', meta_data)
+                del self._objects_to_free_on_error[pre_kernel_event]
+                self._safe_call(cuda.cuEventDestroy(pre_kernel_event),
+                                'failed to destroy pre-kernel event', meta_data)
+                # result check
+                if e == 0 and self._gold_data:
+                    self._cpy_to_host(self._gold_cmp_buffer)
+                    meta_data['checked_inputs'] = []
+                    for idx, (gold_values, comparator) in self._gold_data.items():
+                        meta_data['checked_inputs'].append(idx)
+                        result_values = self._gold_cmp_buffer[idx]
+                        if result_values.size != gold_values.size:
+                            meta_data['result_check'] = f'FAILED for input {idx}: result size is not equal to gold size'
+                            if self._abort_on_invalid_results:
+                                raise RuntimeError('invalid results')
+                            else:
+                                raise CostFunctionError('invalid results')
+                        for value_idx, (result_value, gold_value) in enumerate(zip(result_values, gold_values)):
+                            if not comparator(result_value, gold_value):
+                                meta_data['result_check'] = (f'FAILED for input {idx} at position {value_idx}: '
+                                                             f'expected {gold_value}, got {result_value}')
+                                if self._abort_on_invalid_results:
+                                    raise RuntimeError('invalid results')
+                                else:
+                                    raise CostFunctionError('invalid results')
+                    meta_data['result_check'] = 'SUCCESS'
+            avg_runtime /= self._evaluations
+            avg_runtime = float(ceil(avg_runtime))  # runtime can be ceiled, since nanoseconds are precise enough
+
+            # free program resources
+            del self._objects_to_free_on_error[module]
+            self._safe_call(cuda.cuModuleUnload(module),
+                            'failed to unload module', meta_data)
+            del self._objects_to_free_on_error[nvrtc_program]
+            self._safe_call(nvrtc.nvrtcDestroyProgram(nvrtc_program),
+                            'failed to destroy NVRTC program', meta_data)
+        except CostFunction._CUDAError as e:
+            self._free_objects_before_error()
+            if self._abort_on_cuda_error:
+                raise e
+            else:
+                raise CostFunctionError(e.message) from e
+        finally:
+            # log metadata
+            if self._log_file_writer:
+                self._log_file_writer.writerow((
+                    meta_data[c] if meta_data[c] is not None else ''
+                    for c in _LOG_FILE_COLUMNS
+                ))
 
-        return avg_runtime, meta_data
+        return avg_runtime
 
     def _init_device(self):
         if self._device_id is not None:
-            self._cu_device = self._safe_call(cuda.cuDeviceGet(self._device_id), 'failed to retrieve device handle')
+            self._cu_device = self._safe_call(cuda.cuDeviceGet(self._device_id),
+                                              'failed to retrieve device handle')
             if not self._silent:
-                device_name = self._safe_call(cuda.cuDeviceGetName(1024, self._cu_device), 'failed to get device name')
+                device_name = self._safe_call(cuda.cuDeviceGetName(1024, self._cu_device),
+                                              'failed to get device name')
                 device_name = str(device_name, encoding='ascii').strip()[:-1]
                 print(f'selecting CUDA device {self._device_id}: {device_name}')
-            self._cu_context = self._safe_call(cuda.cuCtxCreate(0, self._cu_device), 'failed to create context')
-            self._cu_stream = self._safe_call(cuda.cuStreamCreate(0), 'failed to create stream')
+            self._cu_context = self._safe_call(cuda.cuCtxCreate(0, self._cu_device),
+                                               'failed to create context')
+            self._cu_stream = self._safe_call(cuda.cuStreamCreate(0),
+                                              'failed to create stream')
 
     def _alloc_buffers(self):
         if self._cu_context is not None:
             self._cu_device_ptr = {
-                idx: self._safe_call(cuda.cuMemAlloc(inp.nbytes), f'failed to allocate CUDA device memory for input {idx}')
+                idx: self._safe_call(cuda.cuMemAlloc(inp.nbytes),
+                                     f'failed to allocate CUDA device memory for input {idx}')
                 for idx, inp in self._inputs.items() if isinstance(inp, numpy.ndarray)
             }
 
     def _cpy_to_device(self):
         if self._cu_stream is not None:
             for idx, deviceptr in self._cu_device_ptr.items():
                 ndarray = self._inputs[idx]
@@ -386,18 +444,21 @@
                                                            host_data.nbytes, self._cu_stream),
                                     f'failed to copy data from CUDA device memory to host for input {idx}')
             self._safe_call(cuda.cuStreamSynchronize(self._cu_stream),
                             f'failed to synchronize after device to host copy')
 
     def _free_buffers(self):
         for idx, deviceptr in self._cu_device_ptr.items():
-            self._safe_call(cuda.cuMemFree(deviceptr), f'failed to free CUDA device memory for input {idx}')
+            self._safe_call(cuda.cuMemFree(deviceptr),
+                            f'failed to free CUDA device memory for input {idx}')
         self._cu_device_ptr.clear()
 
     def _free_device(self):
         if self._cu_stream is not None:
-            self._safe_call(cuda.cuStreamDestroy(self._cu_stream), 'failed to destroy stream')
+            self._safe_call(cuda.cuStreamDestroy(self._cu_stream),
+                            'failed to destroy stream')
             self._cu_stream = None
         if self._cu_context is not None:
-            self._safe_call(cuda.cuCtxDestroy(self._cu_context), 'failed to destroy context')
+            self._safe_call(cuda.cuCtxDestroy(self._cu_context),
+                            'failed to destroy context')
             self._cu_context = None
         self._cu_device = None
```

### Comparing `pyatf-0.0.1/src/pyatf/cost_functions/generic.py` & `pyatf-0.0.2/src/pyatf/cost_functions/generic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,47 @@
 import os
 import subprocess
 import time
-from typing import Optional, Any, Dict, Tuple
+from typing import Optional
 
-from pyatf.tuning_data import Configuration, CostFunctionError, Cost, MetaData
+from pyatf.tuning_data import Configuration, CostFunctionError, Cost
 
 
 class CostFunction:
-    def __init__(self, *run_command: str):
-        self._run_command: Tuple[str] = tuple(run_command)
-        self._compile_command: Optional[Tuple[str]] = None
+    def __init__(self, run_command: str):
+        self._run_command: str = run_command
+        self._compile_command: Optional[str] = None
         self._cost_file: Optional[str] = None
 
-    def compile_command(self, *compile_command: str):
-        self._compile_command = tuple(compile_command)
+    def compile_command(self, compile_command: str):
+        self._compile_command = compile_command
         return self
 
     def cost_file(self, cost_file: str):
         self._cost_file = cost_file
         return self
 
-    def __call__(self, configuration: Configuration) -> Tuple[Cost, MetaData]:
+    def __call__(self, configuration: Configuration) -> Cost:
         # add configuration to environment variables
         augmented_env = os.environ.copy()
         for tp_name, tp_value in configuration.items():
             augmented_env[tp_name] = str(tp_value)
 
-        # collect meta-data for logging
-        meta_data: Dict[str, Any] = {}
-
         # execute compile command
         if self._compile_command is not None:
-            compile_start = time.perf_counter_ns()
-            ret = subprocess.run(self._compile_command, env=augmented_env)
-            compile_end = time.perf_counter_ns()
-            meta_data['compile_command_exit_code'] = ret.returncode
-            meta_data['compile_command_ns'] = compile_end - compile_start
-            if meta_data['compile_command_exit_code'] != 0:
-                raise CostFunctionError(meta_data) \
-                    from RuntimeError('error while executing compile command: ' + ' '.join(self._compile_command))
+            ret = subprocess.run(self._compile_command, env=augmented_env, shell=True)
+            if ret.returncode != 0:
+                raise CostFunctionError('error while executing compile command: ' + self._compile_command)
 
         # execute run command
         run_start = time.perf_counter_ns()
-        ret = subprocess.run(self._run_command, env=augmented_env)
+        ret = subprocess.run(self._run_command, env=augmented_env, shell=True)
         run_end = time.perf_counter_ns()
-        meta_data['run_command_exit_code'] = ret.returncode
-        meta_data['run_command_ns'] = run_end - run_start
-        if meta_data['run_command_exit_code'] != 0:
-            raise CostFunctionError(meta_data) \
-                from RuntimeError('error while executing run command: ' + ' '.join(self._run_command))
+        if ret.returncode != 0:
+            raise CostFunctionError('error while executing run command: ' + self._run_command)
 
         # get configuration cost
         if self._cost_file is None:
-            return float(meta_data['run_command_ns']), meta_data
+            return float(run_end - run_start)
         else:
             with open(self._cost_file, 'r') as cost_file:
-                return float(cost_file.read()), meta_data
+                return float(cost_file.read())
```

### Comparing `pyatf-0.0.1/src/pyatf/cost_functions/opencl.py` & `pyatf-0.0.2/src/pyatf/cost_functions/opencl.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import csv
 import inspect
 import time
 from math import ceil
-from typing import Union, Tuple, Callable, Optional, Set, Dict, Iterable
+from typing import Union, Tuple, Callable, Optional, Set, Dict, Iterable, TextIO, Any
 
 import numpy
 import pyopencl as cl
 
 from pyatf.result_check import equality
-from pyatf.tuning_data import Configuration, Cost, MetaData, CostFunctionError
+from pyatf.tuning_data import Configuration, Cost, CostFunctionError
 
 
 def get_device(platform_id: int = 0, device_id: int = 0) -> cl.Device:
     platforms = cl.get_platforms()
     if platform_id >= len(platforms):
         raise ValueError(f'invalid platform id: {platform_id}')
     cl_platform = platforms[platform_id]
@@ -65,14 +66,20 @@
     @property
     def flags(self):
         return self._flags
 
 
 Input = Union[numpy.ndarray, numpy.generic]
 
+_LOG_FILE_COLUMNS = ('build_time_ns',
+                     'opencl_error_code',
+                     'opencl_error_routine',
+                     'result_check',
+                     'checked_inputs')
+
 
 class CostFunction:
     def __init__(self, kernel: Kernel):
         self._kernel = kernel
 
         self._silent: bool = False
         self._platform_id: Optional[int] = None
@@ -91,30 +98,41 @@
         self._local_size_y: Union[int, Callable[..., int]] = 1
         self._local_size_y_tps: Optional[Set[str, ...]] = None
         self._local_size_z: Union[int, Callable[..., int]] = 1
         self._local_size_z_tps: Optional[Set[str, ...]] = None
 
         self._gold_data: Dict[int, Tuple[Input, Callable[[numpy.generic, numpy.generic], bool]]] = {}
         self._gold_cmp_buffer: Dict[int, Input] = {}
+        self._abort_on_invalid_results: bool = False
+
+        self._abort_on_opencl_error: bool = False
 
         self._warmups: int = 0
         self._evaluations: int = 1
 
+        self._log_file: Optional[TextIO] = None
+        self._log_file_writer = None
+
         self._cl_platform: Optional[cl.Platform] = None
         self._cl_device: Optional[cl.Device] = None
         self._cl_context: Optional[cl.Context] = None
         self._cl_queue: Optional[cl.CommandQueue] = None
         self._cl_buffer: Dict[int, cl.Buffer] = {}
 
     def __del__(self):
         self._free_buffers()
         self._free_command_queue()
+        if self._log_file:
+            self._log_file_writer = None
+            self._log_file.close()
+            self._log_file = None
 
     def silent(self, silent: bool):
         self._silent = silent
+        return self
 
     def platform_id(self, platform_id: int):
         self._free_buffers()
         self._free_command_queue()
         self._platform_id = platform_id
         self._init_command_queue()
         self._alloc_buffers()
@@ -183,25 +201,46 @@
             self._gold_cmp_buffer[index] = gold_data_or_callable.copy()
         else:
             gold_buffer = gold_data_or_callable(*self._inputs.values())
             self._gold_data[index] = (gold_buffer, comparator)
             self._gold_cmp_buffer[index] = gold_buffer.copy()
         return self
 
+    def abort_on_invalid_results(self, abort_on_invalid_results: bool = True):
+        self._abort_on_invalid_results = abort_on_invalid_results
+        return self
+
+    def abort_on_opencl_error(self, abort_on_opencl_error: bool = True):
+        self._abort_on_opencl_error = abort_on_opencl_error
+        return self
+
     def warmups(self, warmups: int):
         self._warmups = warmups
+        return self
 
     def evaluations(self, evaluations: int):
         self._evaluations = evaluations
+        return self
 
-    def __call__(self, configuration: Configuration) -> Tuple[Cost, MetaData]:
+    def log_file(self, log_file_path: str):
+        if self._log_file:
+            self._log_file_writer = None
+            self._log_file.close()
+            self._log_file = None
+        if log_file_path:
+            self._log_file = open(log_file_path, 'w')
+            self._log_file_writer = csv.writer(self._log_file, delimiter=";")
+            self._log_file_writer.writerow(_LOG_FILE_COLUMNS)
+        return self
+
+    def __call__(self, configuration: Configuration) -> Cost:
         if self._platform_id is None or self._device_id is None:
             raise ValueError('no OpenCL platform or device was selected')
 
-        meta_data = {}
+        meta_data: Dict[str, Any] = {c: None for c in _LOG_FILE_COLUMNS}
 
         try:
             # create & build program, and get kernel object
             cl_program = cl.Program(self._cl_context, self._kernel.source)
             opts = list(self._kernel.flags)
             for tp_name, tp_value in configuration.items():
                 opts.append(f'-D{tp_name}={tp_value}')
@@ -270,56 +309,65 @@
                 kernel_event = cl.enqueue_nd_range_kernel(self._cl_queue, kernel, global_size, local_size)
                 kernel_event.wait()
                 avg_runtime += (kernel_event.get_profiling_info(cl.profiling_info.END)
                                 - kernel_event.get_profiling_info(cl.profiling_info.START))
                 # result check
                 if e == 0 and self._gold_data:
                     self._cpy_to_host(self._gold_cmp_buffer)
+                    meta_data['checked_inputs'] = []
                     for idx, (gold_values, comparator) in self._gold_data.items():
+                        meta_data['checked_inputs'].append(idx)
                         result_values = self._gold_cmp_buffer[idx]
                         if result_values.size != gold_values.size:
-                            meta_data['result_check'] = {
-                                'status': 'failed',
-                                'input': idx,
-                                'reason': 'result size is not equal to gold size'
-                            }
-                            raise CostFunctionError(meta_data)
+                            meta_data['result_check'] = f'FAILED for input {idx}: result size is not equal to gold size'
+                            if self._abort_on_invalid_results:
+                                raise RuntimeError('invalid results')
+                            else:
+                                raise CostFunctionError('invalid results')
                         for value_idx, (result_value, gold_value) in enumerate(zip(result_values, gold_values)):
                             if not comparator(result_value, gold_value):
-                                meta_data['result_check'] = {
-                                    'status': 'failed',
-                                    'input': idx,
-                                    'position': value_idx,
-                                    'expected': str(gold_value),
-                                    'actual': str(result_value)
-                                }
-                                raise CostFunctionError(meta_data)
-                    meta_data['result_check'] = {'status': 'success', 'checked_inputs': tuple(self._gold_data.keys())}
+                                meta_data['result_check'] = (f'FAILED for input {idx} at position {value_idx}: '
+                                                             f'expected {gold_value}, got {result_value}')
+                                if self._abort_on_invalid_results:
+                                    raise RuntimeError('invalid results')
+                                else:
+                                    raise CostFunctionError('invalid results')
+                    meta_data['result_check'] = 'SUCCESS'
             avg_runtime /= self._evaluations
             avg_runtime = float(ceil(avg_runtime))  # runtime can be ceiled, since nanoseconds are precise enough
         except cl.Error as e:
             meta_data['opencl_error_code'] = e.code
-            meta_data['opencl_error_what'] = e.what.what()
             meta_data['opencl_error_routine'] = e.routine
-            raise CostFunctionError(meta_data) from e
+            if self._abort_on_opencl_error:
+                raise e
+            else:
+                raise CostFunctionError(f'{e.routine} failed with error code {e.code}: {e.what.what()}') from e
         finally:
+            # log metadata
+            if self._log_file_writer:
+                self._log_file_writer.writerow((
+                    meta_data[c] if meta_data[c] is not None else ''
+                    for c in _LOG_FILE_COLUMNS
+                ))
+
             # free program resources
             del kernel
             del cl_program
 
-        return avg_runtime, meta_data
+        return avg_runtime
 
     def _init_command_queue(self):
         if self._platform_id is not None and self._device_id is not None:
             platforms = cl.get_platforms()
             if self._platform_id >= len(platforms):
                 raise ValueError(f'invalid platform id: {self._platform_id}')
             self._cl_platform = platforms[self._platform_id]
             if not self._silent:
-                print(f'selecting OpenCL platform {self._platform_id}: {self._cl_platform.get_info(cl.platform_info.NAME)}')
+                print(f'selecting OpenCL platform {self._platform_id}: '
+                      f'{self._cl_platform.get_info(cl.platform_info.NAME)}')
             devices = self._cl_platform.get_devices()
             if self._device_id >= len(devices):
                 raise ValueError(f'invalid device id: {self._device_id}')
             self._cl_device = devices[self._device_id]
             if not self._silent:
                 print(f'selecting OpenCL device {self._device_id}: {self._cl_device.get_info(cl.device_info.NAME)}')
             self._cl_context = cl.Context(devices=[self._cl_device])
```

### Comparing `pyatf-0.0.1/src/pyatf/cost_functions/python.py` & `pyatf-0.0.2/src/pyatf/cost_functions/python.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import time
-from typing import Type, Tuple, Any, Optional, Dict
+from typing import Type, Tuple, Any, Dict
 
 from pyatf.tuning_data import Configuration, Cost
 
 
 class CostFunction:
     class CostFunctionWithTypeAndArgs:
         def __init__(self, type_to_tune: Type, *call_args, **call_kwargs):
```

### Comparing `pyatf-0.0.1/src/pyatf/search_techniques/auc_bandit.py` & `pyatf-0.0.2/src/pyatf/search_techniques/auc_bandit.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/search_techniques/differential_evolution.py` & `pyatf-0.0.2/src/pyatf/search_techniques/differential_evolution.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/search_techniques/exhaustive.py` & `pyatf-0.0.2/src/pyatf/search_techniques/exhaustive.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/search_techniques/opentuner.py` & `pyatf-0.0.2/src/pyatf/search_techniques/opentuner.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/search_techniques/pattern_search.py` & `pyatf-0.0.2/src/pyatf/search_techniques/pattern_search.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/search_techniques/random.py` & `pyatf-0.0.2/src/pyatf/search_techniques/random.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/search_techniques/round_robin.py` & `pyatf-0.0.2/src/pyatf/search_techniques/round_robin.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/search_techniques/search_technique.py` & `pyatf-0.0.2/src/pyatf/search_techniques/search_technique.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/search_techniques/search_technique_1d.py` & `pyatf-0.0.2/src/pyatf/search_techniques/search_technique_1d.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/search_techniques/simulated_annealing.py` & `pyatf-0.0.2/src/pyatf/search_techniques/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/src/pyatf/search_techniques/torczon.py` & `pyatf-0.0.2/src/pyatf/search_techniques/torczon.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/tests/test_range.py` & `pyatf-0.0.2/tests/test_range.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/tests/test_search_space.py` & `pyatf-0.0.2/tests/test_search_space.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/tests/test_tuning_data.py` & `pyatf-0.0.2/tests/test_tuning_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,36 +10,34 @@
 from pyatf.tp import TP
 from pyatf.tuning_data import TuningData, Configuration, Cost, History, Coordinates, Index
 
 
 class TestTuningData(unittest.TestCase):
     def _check_history(self,
                        gold_history: Tuple[Tuple[datetime, int, int, Configuration, bool, Optional[Cost],
-                       Optional[Dict], Optional[Coordinates], Optional[Index]], ...],
+                       Optional[Coordinates], Optional[Index]], ...],
                        tuning_start: datetime,
                        history: History):
         self.assertEqual(len(gold_history), len(history))
         for record, gold_record in zip(history, gold_history):
             gold_record_timestamp = gold_record[0]
             gold_record_num_evaluations = gold_record[1]
             gold_record_num_valid_evaluations = gold_record[2]
             gold_record_configuration = gold_record[3]
             gold_record_valid = gold_record[4]
             gold_record_cost = gold_record[5]
-            gold_record_meta_data = gold_record[6]
-            gold_record_coordinates = gold_record[7]
-            gold_record_index = gold_record[8]
+            gold_record_coordinates = gold_record[6]
+            gold_record_index = gold_record[7]
             self.assertEqual(gold_record_timestamp, record.timestamp)
             self.assertEqual(record.timestamp - tuning_start, record.timedelta_since_tuning_start)
             self.assertEqual(gold_record_num_evaluations, record.evaluations)
             self.assertEqual(gold_record_num_valid_evaluations, record.valid_evaluations)
             self.assertEqual(gold_record_configuration, record.configuration)
             self.assertEqual(gold_record_valid, record.valid)
             self.assertEqual(gold_record_cost, record.cost)
-            self.assertEqual(gold_record_meta_data, record.meta_data)
             self.assertEqual(gold_record_coordinates, record.search_space_coordinates)
             self.assertEqual(gold_record_index, record.search_space_index)
 
     def test(self):
         tp1 = TP('tp1', Interval(1, 10))
         tp2 = TP('tp2', Interval(5, 10), lambda tp2, tp1: tp2 % tp1 == 0)
         tp3 = TP('tp3', Interval(2, 3), lambda tp3, tp1: tp1 % tp3 == 0)
@@ -71,184 +69,171 @@
         self._check_history(tuple(), tuning_data.tuning_start_timestamp, tuning_data.history)
         self._check_history(tuple(), tuning_data.tuning_start_timestamp, tuning_data.improvement_history)
         self.assertEqual(0, tuning_data.number_of_evaluated_configurations)
         self.assertEqual(0, tuning_data.number_of_evaluated_valid_configurations)
         self.assertEqual(0, tuning_data.number_of_evaluated_invalid_configurations)
         self.assertIsNone(tuning_data.min_cost())
         self.assertIsNone(tuning_data.configuration_of_min_cost())
-        self.assertIsNone(tuning_data.meta_data_of_min_cost())
         self.assertIsNone(tuning_data.search_space_coordinates_of_min_cost())
         self.assertIsNone(tuning_data.search_space_index_of_min_cost())
         self.assertIsNone(tuning_data.timestamp_of_min_cost())
         self.assertIsNone(tuning_data.duration_to_min_cost())
         self.assertIsNone(tuning_data.evaluations_to_min_cost())
         self.assertIsNone(tuning_data.valid_evaluations_to_min_cost())
 
         coords1 = (0.12938, 0.83746, 0.91349)
         index1 = None
         config1 = search_space.get_configuration(coords1 or index1)
         valid1 = False
         cost1 = None
-        meta_data1 = {'error_code': -4}
-        timestamp1 = tuning_data.record_evaluation(config1, valid1, cost1, meta_data1, coords1, index1)
+        timestamp1 = tuning_data.record_evaluation(config1, valid1, cost1, coords1, index1)
         self._check_history((
-            (timestamp1, 1, 0, config1, valid1, cost1, meta_data1, coords1, index1),
+            (timestamp1, 1, 0, config1, valid1, cost1, coords1, index1),
         ), tuning_data.tuning_start_timestamp, tuning_data.history)
         self._check_history(tuple(), tuning_data.tuning_start_timestamp, tuning_data.improvement_history)
         self.assertEqual(1, tuning_data.number_of_evaluated_configurations)
         self.assertEqual(0, tuning_data.number_of_evaluated_valid_configurations)
         self.assertEqual(1, tuning_data.number_of_evaluated_invalid_configurations)
         self.assertIsNone(tuning_data.min_cost())
         self.assertIsNone(tuning_data.configuration_of_min_cost())
-        self.assertIsNone(tuning_data.meta_data_of_min_cost())
         self.assertIsNone(tuning_data.search_space_coordinates_of_min_cost())
         self.assertIsNone(tuning_data.search_space_index_of_min_cost())
         self.assertIsNone(tuning_data.timestamp_of_min_cost())
         self.assertIsNone(tuning_data.duration_to_min_cost())
         self.assertIsNone(tuning_data.evaluations_to_min_cost())
         self.assertIsNone(tuning_data.valid_evaluations_to_min_cost())
 
         coords2 = None
         index2 = 3
         config2 = search_space.get_configuration(coords2 or index2)
         valid2 = False
         cost2 = None
-        meta_data2 = {'error_code': -6}
-        timestamp2 = tuning_data.record_evaluation(config2, valid2, cost2, meta_data2, coords2, index2)
+        timestamp2 = tuning_data.record_evaluation(config2, valid2, cost2, coords2, index2)
         self._check_history((
-            (timestamp1, 1, 0, config1, valid1, cost1, meta_data1, coords1, index1),
-            (timestamp2, 2, 0, config2, valid2, cost2, meta_data2, coords2, index2),
+            (timestamp1, 1, 0, config1, valid1, cost1, coords1, index1),
+            (timestamp2, 2, 0, config2, valid2, cost2, coords2, index2),
         ), tuning_data.tuning_start_timestamp, tuning_data.history)
         self._check_history(tuple(), tuning_data.tuning_start_timestamp, tuning_data.improvement_history)
         self.assertEqual(2, tuning_data.number_of_evaluated_configurations)
         self.assertEqual(0, tuning_data.number_of_evaluated_valid_configurations)
         self.assertEqual(2, tuning_data.number_of_evaluated_invalid_configurations)
         self.assertIsNone(tuning_data.min_cost())
         self.assertIsNone(tuning_data.configuration_of_min_cost())
-        self.assertIsNone(tuning_data.meta_data_of_min_cost())
         self.assertIsNone(tuning_data.search_space_coordinates_of_min_cost())
         self.assertIsNone(tuning_data.search_space_index_of_min_cost())
         self.assertIsNone(tuning_data.timestamp_of_min_cost())
         self.assertIsNone(tuning_data.duration_to_min_cost())
         self.assertIsNone(tuning_data.evaluations_to_min_cost())
         self.assertIsNone(tuning_data.valid_evaluations_to_min_cost())
 
         coords3 = (0.234124, 0.123123, 0.5382921)
         index3 = None
         config3 = search_space.get_configuration(coords3 or index3)
         valid3 = True
         cost3 = 10.23728
-        meta_data3 = None
-        timestamp3 = tuning_data.record_evaluation(config3, valid3, cost3, meta_data3, coords3, index3)
+        timestamp3 = tuning_data.record_evaluation(config3, valid3, cost3, coords3, index3)
         self._check_history((
-            (timestamp1, 1, 0, config1, valid1, cost1, meta_data1, coords1, index1),
-            (timestamp2, 2, 0, config2, valid2, cost2, meta_data2, coords2, index2),
-            (timestamp3, 3, 1, config3, valid3, cost3, meta_data3, coords3, index3),
+            (timestamp1, 1, 0, config1, valid1, cost1, coords1, index1),
+            (timestamp2, 2, 0, config2, valid2, cost2, coords2, index2),
+            (timestamp3, 3, 1, config3, valid3, cost3, coords3, index3),
         ), tuning_data.tuning_start_timestamp, tuning_data.history)
         self._check_history((
-            (timestamp3, 3, 1, config3, valid3, cost3, meta_data3, coords3, index3),
+            (timestamp3, 3, 1, config3, valid3, cost3, coords3, index3),
         ), tuning_data.tuning_start_timestamp, tuning_data.improvement_history)
         self.assertEqual(3, tuning_data.number_of_evaluated_configurations)
         self.assertEqual(1, tuning_data.number_of_evaluated_valid_configurations)
         self.assertEqual(2, tuning_data.number_of_evaluated_invalid_configurations)
         self.assertEqual(cost3, tuning_data.min_cost())
         self.assertEqual(config3, tuning_data.configuration_of_min_cost())
-        self.assertEqual(meta_data3, tuning_data.meta_data_of_min_cost())
         self.assertEqual(coords3, tuning_data.search_space_coordinates_of_min_cost())
         self.assertEqual(index3, tuning_data.search_space_index_of_min_cost())
         self.assertEqual(timestamp3, tuning_data.timestamp_of_min_cost())
         self.assertEqual(timestamp3 - tuning_data.tuning_start_timestamp, tuning_data.duration_to_min_cost())
         self.assertEqual(3, tuning_data.evaluations_to_min_cost())
         self.assertEqual(1, tuning_data.valid_evaluations_to_min_cost())
 
         coords4 = (0.49857, 0.9813284, 0.757172)
         index4 = None
         config4 = search_space.get_configuration(coords4 or index4)
         valid4 = False
         cost4 = None
-        meta_data4 = None
-        timestamp4 = tuning_data.record_evaluation(config4, valid4, cost4, meta_data4, coords4, index4)
+        timestamp4 = tuning_data.record_evaluation(config4, valid4, cost4, coords4, index4)
         self._check_history((
-            (timestamp1, 1, 0, config1, valid1, cost1, meta_data1, coords1, index1),
-            (timestamp2, 2, 0, config2, valid2, cost2, meta_data2, coords2, index2),
-            (timestamp3, 3, 1, config3, valid3, cost3, meta_data3, coords3, index3),
-            (timestamp4, 4, 1, config4, valid4, cost4, meta_data4, coords4, index4),
+            (timestamp1, 1, 0, config1, valid1, cost1, coords1, index1),
+            (timestamp2, 2, 0, config2, valid2, cost2, coords2, index2),
+            (timestamp3, 3, 1, config3, valid3, cost3, coords3, index3),
+            (timestamp4, 4, 1, config4, valid4, cost4, coords4, index4),
         ), tuning_data.tuning_start_timestamp, tuning_data.history)
         self._check_history((
-            (timestamp3, 3, 1, config3, valid3, cost3, meta_data3, coords3, index3),
+            (timestamp3, 3, 1, config3, valid3, cost3, coords3, index3),
         ), tuning_data.tuning_start_timestamp, tuning_data.improvement_history)
         self.assertEqual(4, tuning_data.number_of_evaluated_configurations)
         self.assertEqual(1, tuning_data.number_of_evaluated_valid_configurations)
         self.assertEqual(3, tuning_data.number_of_evaluated_invalid_configurations)
         self.assertEqual(cost3, tuning_data.min_cost())
         self.assertEqual(config3, tuning_data.configuration_of_min_cost())
-        self.assertEqual(meta_data3, tuning_data.meta_data_of_min_cost())
         self.assertEqual(coords3, tuning_data.search_space_coordinates_of_min_cost())
         self.assertEqual(index3, tuning_data.search_space_index_of_min_cost())
         self.assertEqual(timestamp3, tuning_data.timestamp_of_min_cost())
         self.assertEqual(timestamp3 - tuning_data.tuning_start_timestamp, tuning_data.duration_to_min_cost())
         self.assertEqual(3, tuning_data.evaluations_to_min_cost())
         self.assertEqual(1, tuning_data.valid_evaluations_to_min_cost())
 
         coords5 = None
         index5 = 10
         config5 = search_space.get_configuration(coords5 or index5)
         valid5 = True
         cost5 = 8.46543
-        meta_data5 = {'compile_time': 929.224}
-        timestamp5 = tuning_data.record_evaluation(config5, valid5, cost5, meta_data5, coords5, index5)
+        timestamp5 = tuning_data.record_evaluation(config5, valid5, cost5, coords5, index5)
         self._check_history((
-            (timestamp1, 1, 0, config1, valid1, cost1, meta_data1, coords1, index1),
-            (timestamp2, 2, 0, config2, valid2, cost2, meta_data2, coords2, index2),
-            (timestamp3, 3, 1, config3, valid3, cost3, meta_data3, coords3, index3),
-            (timestamp4, 4, 1, config4, valid4, cost4, meta_data4, coords4, index4),
-            (timestamp5, 5, 2, config5, valid5, cost5, meta_data5, coords5, index5),
+            (timestamp1, 1, 0, config1, valid1, cost1, coords1, index1),
+            (timestamp2, 2, 0, config2, valid2, cost2, coords2, index2),
+            (timestamp3, 3, 1, config3, valid3, cost3, coords3, index3),
+            (timestamp4, 4, 1, config4, valid4, cost4, coords4, index4),
+            (timestamp5, 5, 2, config5, valid5, cost5, coords5, index5),
         ), tuning_data.tuning_start_timestamp, tuning_data.history)
         self._check_history((
-            (timestamp3, 3, 1, config3, valid3, cost3, meta_data3, coords3, index3),
-            (timestamp5, 5, 2, config5, valid5, cost5, meta_data5, coords5, index5),
+            (timestamp3, 3, 1, config3, valid3, cost3, coords3, index3),
+            (timestamp5, 5, 2, config5, valid5, cost5, coords5, index5),
         ), tuning_data.tuning_start_timestamp, tuning_data.improvement_history)
         self.assertEqual(5, tuning_data.number_of_evaluated_configurations)
         self.assertEqual(2, tuning_data.number_of_evaluated_valid_configurations)
         self.assertEqual(3, tuning_data.number_of_evaluated_invalid_configurations)
         self.assertEqual(cost5, tuning_data.min_cost())
         self.assertEqual(config5, tuning_data.configuration_of_min_cost())
-        self.assertEqual(meta_data5, tuning_data.meta_data_of_min_cost())
         self.assertEqual(coords5, tuning_data.search_space_coordinates_of_min_cost())
         self.assertEqual(index5, tuning_data.search_space_index_of_min_cost())
         self.assertEqual(timestamp5, tuning_data.timestamp_of_min_cost())
         self.assertEqual(timestamp5 - tuning_data.tuning_start_timestamp, tuning_data.duration_to_min_cost())
         self.assertEqual(5, tuning_data.evaluations_to_min_cost())
         self.assertEqual(2, tuning_data.valid_evaluations_to_min_cost())
 
         coords6 = (0.298382, 1.00000, 0.263831)
         index6 = None
         config6 = search_space.get_configuration(coords6 or index6)
         valid6 = True
         cost6 = 9.78224
-        meta_data6 = {'compile_time': 55.125}
-        timestamp6 = tuning_data.record_evaluation(config6, valid6, cost6, meta_data6, coords6, index6)
+        timestamp6 = tuning_data.record_evaluation(config6, valid6, cost6, coords6, index6)
         self._check_history((
-            (timestamp1, 1, 0, config1, valid1, cost1, meta_data1, coords1, index1),
-            (timestamp2, 2, 0, config2, valid2, cost2, meta_data2, coords2, index2),
-            (timestamp3, 3, 1, config3, valid3, cost3, meta_data3, coords3, index3),
-            (timestamp4, 4, 1, config4, valid4, cost4, meta_data4, coords4, index4),
-            (timestamp5, 5, 2, config5, valid5, cost5, meta_data5, coords5, index5),
-            (timestamp6, 6, 3, config6, valid6, cost6, meta_data6, coords6, index6),
+            (timestamp1, 1, 0, config1, valid1, cost1, coords1, index1),
+            (timestamp2, 2, 0, config2, valid2, cost2, coords2, index2),
+            (timestamp3, 3, 1, config3, valid3, cost3, coords3, index3),
+            (timestamp4, 4, 1, config4, valid4, cost4, coords4, index4),
+            (timestamp5, 5, 2, config5, valid5, cost5, coords5, index5),
+            (timestamp6, 6, 3, config6, valid6, cost6, coords6, index6),
         ), tuning_data.tuning_start_timestamp, tuning_data.history)
         self._check_history((
-            (timestamp3, 3, 1, config3, valid3, cost3, meta_data3, coords3, index3),
-            (timestamp5, 5, 2, config5, valid5, cost5, meta_data5, coords5, index5),
+            (timestamp3, 3, 1, config3, valid3, cost3, coords3, index3),
+            (timestamp5, 5, 2, config5, valid5, cost5, coords5, index5),
         ), tuning_data.tuning_start_timestamp, tuning_data.improvement_history)
         self.assertEqual(6, tuning_data.number_of_evaluated_configurations)
         self.assertEqual(3, tuning_data.number_of_evaluated_valid_configurations)
         self.assertEqual(3, tuning_data.number_of_evaluated_invalid_configurations)
         self.assertEqual(cost5, tuning_data.min_cost())
         self.assertEqual(config5, tuning_data.configuration_of_min_cost())
-        self.assertEqual(meta_data5, tuning_data.meta_data_of_min_cost())
         self.assertEqual(coords5, tuning_data.search_space_coordinates_of_min_cost())
         self.assertEqual(index5, tuning_data.search_space_index_of_min_cost())
         self.assertEqual(timestamp5, tuning_data.timestamp_of_min_cost())
         self.assertEqual(timestamp5 - tuning_data.tuning_start_timestamp, tuning_data.duration_to_min_cost())
         self.assertEqual(5, tuning_data.evaluations_to_min_cost())
         self.assertEqual(2, tuning_data.valid_evaluations_to_min_cost())
```

### Comparing `pyatf-0.0.1/LICENSE` & `pyatf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.1/pyproject.toml` & `pyatf-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyatf"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name="Richard Schulze", email="r.schulze@uni-muenster.de" },
     { name="Ari Rasch", email="a.rasch@uni-muenster.de" }
 ]
 description = "Auto-Tuning Framework (ATF) is a generic, general-purpose auto-tuning approach for programs whose tuning parameters may be constrained"
 readme = "./PyPI/README.md"
 requires-python = ">=3.9"
```

### Comparing `pyatf-0.0.1/PyPI/README.md` & `pyatf-0.0.2/PyPI/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 1. *Domain-Specific Language (DSL)*, for auto-tuning at compile time (a.k.a. offline tuning) (discussed [here](https://onlinelibrary.wiley.com/doi/full/10.1002/cpe.4423?casa_token=FO9i0maAi_MAAAAA%3AwSOYWsoqfLqcbazsprmzKkmI5msUCY4An5A7CCwi-_V8u10VdpgejcWuiTwYhWnZpaCJZ3NmXt86sg));
 2. *General Purpose Language (GPL)*, for auto-tuning at runtime (a.k.a. online tuning), e.g., of *C++ programs* (referred to as [cppATF](todo), and discussed [here](https://ieeexplore.ieee.org/abstract/document/8291912)) or *Python programs* (referred to as [pyATF](todo)).
 
 **The full GitHub repository for *pyATF*, i.e., ATF with its GPL-based Python interface can be found [here](https://github.com/atf-tuner/pyATF).**
 
 ## Documentation
 
-The full documentation is available [here](https://mdh-project.gitlab.io/pyatf).
+The full documentation is available [here](https://atf-tuner.org/pyATF/).
 
 ## Installation
 
 pyATF requires Python 3.9+ and can be installed using `pip`:
 
     pip install pyatf
```

### Comparing `pyatf-0.0.1/PKG-INFO` & `pyatf-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatf
-Version: 0.0.1
+Version: 0.0.2
 Summary: Auto-Tuning Framework (ATF) is a generic, general-purpose auto-tuning approach for programs whose tuning parameters may be constrained
 Project-URL: Homepage, https://atf-project.org/
 Project-URL: Issues, https://github.com/atf-tuner/pyATF/issues
 Author-email: Richard Schulze <r.schulze@uni-muenster.de>, Ari Rasch <a.rasch@uni-muenster.de>
 License-File: LICENSE
 Keywords: auto-tuning,constraints,optimization,performance,tuning
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 1. *Domain-Specific Language (DSL)*, for auto-tuning at compile time (a.k.a. offline tuning) (discussed [here](https://onlinelibrary.wiley.com/doi/full/10.1002/cpe.4423?casa_token=FO9i0maAi_MAAAAA%3AwSOYWsoqfLqcbazsprmzKkmI5msUCY4An5A7CCwi-_V8u10VdpgejcWuiTwYhWnZpaCJZ3NmXt86sg));
 2. *General Purpose Language (GPL)*, for auto-tuning at runtime (a.k.a. online tuning), e.g., of *C++ programs* (referred to as [cppATF](todo), and discussed [here](https://ieeexplore.ieee.org/abstract/document/8291912)) or *Python programs* (referred to as [pyATF](todo)).
 
 **The full GitHub repository for *pyATF*, i.e., ATF with its GPL-based Python interface can be found [here](https://github.com/atf-tuner/pyATF).**
 
 ## Documentation
 
-The full documentation is available [here](https://mdh-project.gitlab.io/pyatf).
+The full documentation is available [here](https://atf-tuner.org/pyATF/).
 
 ## Installation
 
 pyATF requires Python 3.9+ and can be installed using `pip`:
 
     pip install pyatf
```

