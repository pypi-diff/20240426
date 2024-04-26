# Comparing `tmp/exl2conv-0.0.18.tar.gz` & `tmp/exl2conv-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exl2conv-0.0.18.tar", last modified: Mon Apr  8 00:56:26 2024, max compression
+gzip compressed data, was "exl2conv-0.0.19.tar", last modified: Fri Apr 26 11:14:48 2024, max compression
```

## Comparing `exl2conv-0.0.18.tar` & `exl2conv-0.0.19.tar`

### file list

```diff
@@ -1,170 +1,186 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:56:26.160509 exl2conv-0.0.18/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-08 00:55:44.000000 exl2conv-0.0.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 00:55:44.000000 exl2conv-0.0.18/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-08 00:56:26.160509 exl2conv-0.0.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-08 00:55:44.000000 exl2conv-0.0.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:56:26.148509 exl2conv-0.0.18/exl2conv/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17069 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/architecture.py
--rw-r--r--   0 runner    (1001) docker     (127)    32609 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/attn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:56:26.148509 exl2conv-0.0.18/exl2conv/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)    21405 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/conversion/adaptivegptq.py
--rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/conversion/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/conversion/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    24397 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/conversion/measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/conversion/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/conversion/qparams.py
--rw-r--r--   0 runner    (1001) docker     (127)    18875 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/conversion/quantize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:56:26.148509 exl2conv-0.0.18/exl2conv/conversion/standard_cal_data/
--rw-r--r--   0 runner    (1001) docker     (127)   332173 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/conversion/standard_cal_data/c4.utf8
--rw-r--r--   0 runner    (1001) docker     (127)   248834 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/conversion/standard_cal_data/code.utf8
--rw-r--r--   0 runner    (1001) docker     (127)   222555 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/conversion/standard_cal_data/multilingual.utf8
--rw-r--r--   0 runner    (1001) docker     (127)   196701 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/conversion/standard_cal_data/technical.utf8
--rw-r--r--   0 runner    (1001) docker     (127)   261693 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/conversion/standard_cal_data/tiny.utf8
--rw-r--r--   0 runner    (1001) docker     (127)  2093275 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/conversion/standard_cal_data/wiki.utf8
--rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/conversion/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:56:26.152509 exl2conv-0.0.18/exl2conv/exl2conv_ext/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:56:26.152509 exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/avx2_target.h
--rw-r--r--   0 runner    (1001) docker     (127)    24414 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/avx_mathfun.h
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/profiling.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/profiling.h
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/quantize_func.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/quantize_func.h
--rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/safetensors.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/safetensors.h
--rw-r--r--   0 runner    (1001) docker     (127)    20254 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/sampling.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/sampling.h
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/sampling_avx2.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/sampling_avx2.h
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/util.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:56:26.156509 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/cache.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/cache.cuh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:56:26.156509 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cu
--rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cuh
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1a.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1b.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2a.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2b.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3a.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3b.cu
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_1.cu
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_2.cu
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_3.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/compat.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/h_add.cu
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/h_add.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/h_gemm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/h_gemm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/head_norm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/head_norm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/layer_norm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/layer_norm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/lora.cu
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/lora.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/matrix_view.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/pack_tensor.cu
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/pack_tensor.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_attn.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_attn.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_gemm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_gemm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_gemm_autotune.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    19672 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_gemm_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_gemm_kernel_gptq.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    21831 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_matrix.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_matrix.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_mlp.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_mlp.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_mlp_activation.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_mlp_softmax.cuh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:56:26.156509 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quant/
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quant/qdq_2.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quant/qdq_3.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quant/qdq_4.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quant/qdq_5.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quant/qdq_6.cuh
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quant/qdq_8.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quant/qdq_util.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quantize.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quantize.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/rms_norm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/rms_norm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/rope.cu
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/rope.cuh
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/util.cu
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/util.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_cache.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_cache.h
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_gemm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_gemm.h
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_norm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_norm.h
--rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_qattn.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_qattn.h
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_qmatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_qmatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_qmlp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_qmlp.h
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_quant.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_quant.h
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_rope.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_rope.h
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_safetensors.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_safetensors.h
--rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_sampling.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_sampling.h
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/fasttensors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:56:26.156509 exl2conv-0.0.18/exl2conv/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12746 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/generator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:56:26.156509 exl2conv-0.0.18/exl2conv/generator/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/generator/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/generator/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/generator/filters/prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/generator/filters/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/generator/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/generator/ngram.py
--rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/generator/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    33049 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/generator/streaming.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/headnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    28424 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/model_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/moe_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/parallel_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/rmsnorm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:56:26.156509 exl2conv-0.0.18/exl2conv/server/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/server/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/server/websocket_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:56:26.160509 exl2conv-0.0.18/exl2conv/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/tokenizer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/tokenizer/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/tokenizer/spm.py
--rw-r--r--   0 runner    (1001) docker     (127)    22386 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/tokenizer/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22386 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 00:55:44.000000 exl2conv-0.0.18/exl2conv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:56:26.148509 exl2conv-0.0.18/exl2conv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-08 00:56:26.000000 exl2conv-0.0.18/exl2conv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-08 00:56:26.000000 exl2conv-0.0.18/exl2conv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 00:56:26.000000 exl2conv-0.0.18/exl2conv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-08 00:56:26.000000 exl2conv-0.0.18/exl2conv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 00:56:26.000000 exl2conv-0.0.18/exl2conv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 00:56:26.160509 exl2conv-0.0.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-08 00:55:44.000000 exl2conv-0.0.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.690673 exl2conv-0.0.19/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-26 11:14:22.000000 exl2conv-0.0.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 11:14:22.000000 exl2conv-0.0.19/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-26 11:14:48.690673 exl2conv-0.0.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-26 11:14:22.000000 exl2conv-0.0.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.678673 exl2conv-0.0.19/exl2conv/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17069 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/architecture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32609 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/attn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14232 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.678673 exl2conv-0.0.19/exl2conv/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)    21674 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/adaptivegptq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24398 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/qparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18875 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/quantize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.678673 exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   332173 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/c4.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)   248834 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/code.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)   222555 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/multilingual.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)   196701 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/technical.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)   261693 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/tiny.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)  2093275 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/wiki.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.682673 exl2conv-0.0.19/exl2conv/exl2conv_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.682673 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/avx2_target.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24414 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/avx_mathfun.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/profiling.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/profiling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/quantize_func.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/quantize_func.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/safetensors.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/safetensors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20254 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/sampling.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/sampling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/sampling_avx2.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/sampling_avx2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/util.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.686673 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/
+-rw-r--r--   0 runner    (1001) docker     (127)    10058 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/cache.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/cache.cuh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.686673 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1a.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1b.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2a.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2b.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3a.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3b.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_1.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_2.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_3.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/compat.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/h_add.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/h_add.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/h_gemm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/h_gemm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/head_norm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/head_norm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/layer_norm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/layer_norm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/lora.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/lora.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/matrix_view.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/pack_tensor.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/pack_tensor.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_attn.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_attn.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm_autotune.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    19672 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm_kernel_gptq.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    21853 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_matrix.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_matrix.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_mlp.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_mlp.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_mlp_activation.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_mlp_softmax.cuh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.686673 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_2.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_3.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_4.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_5.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_6.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_8.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_util.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quantize.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quantize.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/rms_norm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/rms_norm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/rope.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/rope.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/util.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/util.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_cache.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_cache.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_gemm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_gemm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_hadamard.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_hadamard.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_norm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_norm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qattn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qattn.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qmatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qmatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qmlp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qmlp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_quant.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_quant.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_rope.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_rope.h
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_safetensors.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_safetensors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_sampling.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_sampling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/fasttensors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.686673 exl2conv-0.0.19/exl2conv/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12746 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.686673 exl2conv-0.0.19/exl2conv/generator/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/filters/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/filters/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/ngram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33047 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.686673 exl2conv-0.0.19/exl2conv/hadamard/
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_100.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13571 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_116.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24491 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_156.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    29755 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_172.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35531 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_188.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    55931 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_236.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    59779 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_244.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   183612 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_428.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_52.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_92.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    58982 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/primes.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/headnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28424 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/model_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/moe_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/parallel_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/rmsnorm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.686673 exl2conv-0.0.19/exl2conv/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/server/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/server/websocket_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.686673 exl2conv-0.0.19/exl2conv/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/tokenizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/tokenizer/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/tokenizer/spm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22712 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/tokenizer/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22386 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.678673 exl2conv-0.0.19/exl2conv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-26 11:14:48.000000 exl2conv-0.0.19/exl2conv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-04-26 11:14:48.000000 exl2conv-0.0.19/exl2conv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:14:48.000000 exl2conv-0.0.19/exl2conv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-26 11:14:48.000000 exl2conv-0.0.19/exl2conv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 11:14:48.000000 exl2conv-0.0.19/exl2conv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 11:14:48.690673 exl2conv-0.0.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-26 11:14:22.000000 exl2conv-0.0.19/setup.py
```

### Comparing `exl2conv-0.0.18/LICENSE` & `exl2conv-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/README.md` & `exl2conv-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/architecture.py` & `exl2conv-0.0.19/exl2conv/architecture.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/attn.py` & `exl2conv-0.0.19/exl2conv/attn.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/cache.py` & `exl2conv-0.0.19/exl2conv/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import torch
 from exl2conv.ext import exl2conv_ext as ext_c
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
-    from exllamav2.model import ExLlamaV2
+    from exl2conv.model import ExLlamaV2
 
 
 class ExLlamaV2CacheBase:
 
     model = None
     max_seq_len: int
     batch_size: int
```

### Comparing `exl2conv-0.0.18/exl2conv/compat.py` & `exl2conv-0.0.19/exl2conv/compat.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/config.py` & `exl2conv-0.0.19/exl2conv/config.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/conversion/adaptivegptq.py` & `exl2conv-0.0.19/exl2conv/conversion/adaptivegptq.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,18 +65,22 @@
         best_pif = best_pi / self.p_grid
         best_p = self.max_p * best_pif + self.min_p * (1 - best_pif)
 
         self.qscale = qscale_t.to(torch.short)
         self.scale = qscale_tw * best_p
         self.qscale_max = qscale_max_t * best_p
 
+        # Make sure scales are rounded correctly for sanity test
+        prescale = torch.tensor([1 / 256], dtype = torch.half, device = self.scale.device)
+        self.scale = ((self.qscale * self.qscale).to(torch.half) * (self.qscale_max.half() * prescale)).float()
+
 
 class AdaptiveGPTQ:
 
-    percdamp: float = 0.07
+    percdamp: float = 0.12
 
     layer: nn.Linear
     device: torch.device
 
     group_size: int | dict
     bits: list
     bits_groups: list
```

### Comparing `exl2conv-0.0.18/exl2conv/conversion/compile.py` & `exl2conv-0.0.19/exl2conv/conversion/compile.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/conversion/convert.py` & `exl2conv-0.0.19/exl2conv/conversion/convert.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/conversion/measure.py` & `exl2conv-0.0.19/exl2conv/conversion/measure.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,15 +383,15 @@
     rolling_window_size = 10 # (increase to average over larger window)
     completed_steps = 0  
     accuracy_sum = 0  
     accuracy_count = 0  
     overall_rolling_accuracy = 0  
 
     last_snapshot_time = time.time()
-    snapshot_interval_s = 90
+    snapshot_interval_s = 180
 
     temp_filename = os.path.join(job["out_dir"], "hidden_states_temp.safetensors")
     states_filename = os.path.join(job["out_dir"], "hidden_states.safetensors")
     measurement = job.get("measurement", {})
 
     # Quantize
```

### Comparing `exl2conv-0.0.18/exl2conv/conversion/optimize.py` & `exl2conv-0.0.19/exl2conv/conversion/optimize.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/conversion/qparams.py` & `exl2conv-0.0.19/exl2conv/conversion/qparams.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/conversion/quantize.py` & `exl2conv-0.0.19/exl2conv/conversion/quantize.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,15 @@
 #     xx = 0
 
 
 @torch.inference_mode()
 def quant(job, save_fn, model):
 
     last_snapshot_time = time.time()
-    snapshot_interval_s = 90
+    snapshot_interval_s = 180
 
     temp_filename = os.path.join(job["out_dir"], "hidden_states_temp.safetensors")
     states_filename = os.path.join(job["out_dir"], "hidden_states.safetensors")
     strategy = job["strategy"]
 
     # Quantize
 
@@ -522,8 +522,8 @@
                 os.replace(temp_filename, states_filename)
 
             job["q_last_module_idx"] = index
 
             del job["invalid"]
             save_fn()
 
-            time_since_snapshot = time.time()
+            last_snapshot_time = time.time()
```

### Comparing `exl2conv-0.0.18/exl2conv/conversion/standard_cal_data/c4.utf8` & `exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/c4.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/conversion/standard_cal_data/code.utf8` & `exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/code.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/conversion/standard_cal_data/multilingual.utf8` & `exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/multilingual.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/conversion/standard_cal_data/technical.utf8` & `exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/technical.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/conversion/standard_cal_data/tiny.utf8` & `exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/tiny.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/conversion/standard_cal_data/wiki.utf8` & `exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/wiki.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/conversion/tokenize.py` & `exl2conv-0.0.19/exl2conv/conversion/tokenize.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/embedding.py` & `exl2conv-0.0.19/exl2conv/embedding.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/avx2_target.h` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/avx2_target.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/avx_mathfun.h` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/avx_mathfun.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/profiling.cpp` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/profiling.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/quantize_func.cpp` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/quantize_func.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/quantize_func.h` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/quantize_func.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/safetensors.cpp` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/safetensors.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/safetensors.h` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/safetensors.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/sampling.cpp` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/sampling.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/sampling.h` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/sampling.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/sampling_avx2.cpp` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/sampling_avx2.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cpp/util.h` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/util.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/cache.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/cache.cu`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #include "quant/qdq_util.cuh"
 #include "util.cuh"
 #include "compat.cuh"
 
 #define THREADS 32
 #define BLOCKSIZE_Q 256
 #define THREADS_Q (BLOCKSIZE_Q / 2)
+#define HADAMARD_Q4
 
 // The upper 8 bits of FP16 are equivalent to FP8 E5M2.
 //
 // The range of values typically cached seem to be in the range of +/- 16, with an exponent component (with bias) up to
 // about 20. Empirically, the MSE over the whole range of observed values in the K/V cache works out the same for E4M3
 // and E5M2. However, over 80% of values in the cache tensors fall within the range of -1..1, where E5M2 produces about
 // a 25% lower MSE.
@@ -160,27 +161,43 @@
     const half2* in2 = (const half2*) (in + block_offset);
     __shared__ uint32_t q_buffer[BLOCKSIZE_Q / 8];
     __shared__ half s_buffer[BLOCKSIZE_Q / 32];
 
     half2 w2 = in2[t];
     half2 o = w2;
 
+    // Perform hadamard transform on two interleaved 32-element groups. Don't scale output by 1/sqrt(32) here, instead
+    // scale by 1/32 when dequantizing
+
+    #ifdef HADAMARD_Q4
+
+        for (int i = 1; i < 32; i <<= 1)
+        {
+            half2 pw2 = __shfl_xor_sync(0xffffffff, w2, i);
+            uint32_t* w2i = reinterpret_cast<uint32_t*>(&w2);
+            int32_t sfm = -static_cast<int32_t>(t & i) >> 31;
+            *w2i ^= (sfm & 0x80008000);
+            w2 = __hadd2(w2, pw2);
+        }
+
+    #endif
+
     // Max abs value for lane_id 0..15, 16..31
 
     half2 absmax2 = __habs2(w2);
     half absmax = __hmax(__low2half(absmax2), __high2half(absmax2));
     absmax = __hmax(absmax, __shfl_xor_sync(0xffffffff, absmax, 8));
     absmax = __hmax(absmax, __shfl_xor_sync(0xffffffff, absmax, 4));
     absmax = __hmax(absmax, __shfl_xor_sync(0xffffffff, absmax, 2));
     absmax = __hmax(absmax, __shfl_xor_sync(0xffffffff, absmax, 1));
     absmax2 = __half2half2(absmax);
 
     // Normalize
 
-    half2 c_8 = __half2half2(__int2half_rn(8));
+    half2 c_8 = __half2half2(__float2half_rn(8));
     half c_i = __float2half_rn(1.0f / 8.0f);
 
     w2 = __h2div(w2, absmax2);
     w2 = __hfma2(w2, c_8, c_8);
 
     // Quantize & pack
 
@@ -251,14 +268,31 @@
     int q1 = ((int) ((q >> shift1) & 0x0f)) - 8;
 
     half w0 = __int2half_rn(q0);
     half w1 = __int2half_rn(q1);
     half2 w2 = __halves2half2(w0, w1);
     w2 = __hmul2(w2, scale2);
 
+    // Perform hadamard transform on two interleaved 32-element groups. Skipped scaling when quantizing, so result
+    // is scaled by 1/32 here
+
+    #ifdef HADAMARD_Q4
+
+        for (int i = 1; i < 32; i <<= 1)
+        {
+            half2 pw2 = __shfl_xor_sync(0xffffffff, w2, i);
+            uint32_t* w2i = reinterpret_cast<uint32_t*>(&w2);
+            int32_t sfm = -static_cast<int32_t>(t & i) >> 31;
+            *w2i ^= (sfm & 0x80008000);
+            w2 = __hadd2(w2, pw2);
+        }
+        w2 = __hmul2(w2, __float2half2_rn(1.0f/32.0f));
+
+    #endif
+
     // Store
 
     half2* out2 = (half2*) (out + block_offset);
     out2[t] = w2;
 }
 
 void array_fp16_to_q4_kv_cuda
```

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/cache.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/cache.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1a.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1a.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1b.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1b.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2a.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2a.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2b.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2b.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3a.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3a.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3b.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3b.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_1.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_1.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_2.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_2.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_3.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_3.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/compat.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/compat.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/h_add.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/h_add.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/h_gemm.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/h_gemm.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/h_gemm.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/h_gemm.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/head_norm.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/head_norm.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/layer_norm.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/layer_norm.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/lora.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/lora.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/matrix_view.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/matrix_view.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/pack_tensor.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/pack_tensor.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/pack_tensor.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/pack_tensor.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_attn.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_attn.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_attn.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_attn.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_gemm.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_gemm.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_gemm_autotune.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm_autotune.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_gemm_kernel.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm_kernel.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_gemm_kernel_gptq.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm_kernel_gptq.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_matrix.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_matrix.cu`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,16 @@
 
     if (b_q_perm)
     {
         if (offset_k + t < size_k)
             perm[t] = b_q_perm[offset_k + t];
     }
 
+    __syncthreads();
+
     // Column
 
     int n = offset_n + t * 4;
     if (n >= size_n) return;
 
     // Find initial group
```

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_matrix.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_matrix.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_mlp.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_mlp.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_mlp.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_mlp.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_mlp_activation.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_mlp_activation.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/q_mlp_softmax.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_mlp_softmax.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quant/qdq_2.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_2.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quant/qdq_3.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_3.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quant/qdq_4.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_4.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quant/qdq_5.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_5.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quant/qdq_6.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_6.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quant/qdq_8.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_8.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quant/qdq_util.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_util.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quantize.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quantize.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/quantize.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quantize.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/rms_norm.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/rms_norm.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/rope.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/rope.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/rope.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/rope.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/util.cu` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/util.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/cuda/util.cuh` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/util.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_bindings.cpp` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_bindings.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -11,28 +11,30 @@
 #include "ext_quant.h"
 #include "ext_sampling.h"
 #include "ext_safetensors.h"
 #include "ext_qmatrix.h"
 #include "ext_qattn.h"
 #include "ext_qmlp.h"
 #include "ext_cache.h"
+#include "ext_hadamard.h"
 #include "ext_gemm.h"
 #include "ext_norm.h"
 #include "ext_rope.h"
 
 PYBIND11_MODULE(TORCH_EXTENSION_NAME, m)
 {
     // quant
 
     m.def("pack_rows_4", &pack_rows_4, "pack_rows_4");
     m.def("pack_columns", &pack_columns, "pack_columns");
     m.def("quantize", &quantize, "quantize");
     m.def("quantize_err", &quantize_err, "quantize_err");
     m.def("quantize_range", &quantize_range, "quantize_range");
     m.def("quantize_range_inplace", &quantize_range_inplace, "quantize_range_inplace");
+    m.def("sim_anneal", &sim_anneal, "sim_anneal");
 
     // sampling
 
     m.def("apply_rep_penalty", &apply_rep_penalty, "apply_rep_penalty");
     m.def("sample_basic", &sample_basic, "sample_basic");
     m.def("logit_filter_exclusive", &logit_filter_exclusive, "logit_filter_exclusive");
     m.def("fast_fill_cpu_ones_bool", &fast_fill_cpu_ones_bool, "fast_fill_cpu_ones_bool");
@@ -81,14 +83,19 @@
     m.def("fp16_to_fp8", &fp16_to_fp8, "fp16_to_fp8");
     m.def("fp8_to_fp16", &fp8_to_fp16, "fp8_to_fp16");
     m.def("fp16_to_q4_kv", &fp16_to_q4_kv, "fp16_to_q4_kv");
     m.def("q4_to_fp16_kv", &q4_to_fp16_kv, "q4_to_fp16_kv");
 //    m.def("array_fp16_to_fp8_ref", &array_fp16_to_fp8_ref, "array_fp16_to_fp8_ref");
 //    m.def("array_fp8_to_fp16_ref", &array_fp8_to_fp16_ref, "array_fp8_to_fp16_ref");
 
+    // hadamard
+
+    m.def("had_paley", &had_paley, "had_paley");
+    m.def("had_paley2", &had_paley2, "had_paley2");
+
     // gemm
 
     m.def("gemm_half_half_half", &gemm_half_half_half, "gemm_half_half_half");
 
     // norm
 
     m.def("rms_norm", &rms_norm, "rms_norm");
```

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_cache.cpp` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_cache.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_cache.h` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_cache.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_gemm.cpp` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_gemm.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_norm.cpp` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_norm.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_norm.h` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_norm.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_qattn.cpp` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qattn.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_qattn.h` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qattn.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_qmatrix.cpp` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qmatrix.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_qmatrix.h` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qmatrix.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_qmlp.cpp` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qmlp.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_qmlp.h` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qmlp.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_rope.cpp` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_rope.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_sampling.cpp` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_sampling.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/exl2conv_ext/ext_sampling.h` & `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_sampling.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/ext.py` & `exl2conv-0.0.19/exl2conv/ext.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
     sources_dir = os.path.join(library_dir, extension_name)
 
     sources_ = \
     [
         "ext_bindings.cpp",
         "ext_cache.cpp",
         "ext_gemm.cpp",
+        "ext_hadamard.cpp",
         "ext_norm.cpp",
         "ext_qattn.cpp",
         "ext_qmatrix.cpp",
         "ext_qmlp.cpp",
         "ext_quant.cpp",
         "ext_rope.cpp",
         "ext_safetensors.cpp",
```

### Comparing `exl2conv-0.0.18/exl2conv/fasttensors.py` & `exl2conv-0.0.19/exl2conv/fasttensors.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/generator/base.py` & `exl2conv-0.0.19/exl2conv/generator/base.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/generator/filters/base.py` & `exl2conv-0.0.19/exl2conv/generator/filters/base.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/generator/filters/prefix.py` & `exl2conv-0.0.19/exl2conv/generator/filters/prefix.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/generator/filters/select.py` & `exl2conv-0.0.19/exl2conv/generator/filters/select.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/generator/ngram.py` & `exl2conv-0.0.19/exl2conv/generator/ngram.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/generator/sampler.py` & `exl2conv-0.0.19/exl2conv/generator/sampler.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/generator/streaming.py` & `exl2conv-0.0.19/exl2conv/generator/streaming.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,19 +9,19 @@
     ExLlamaV2Tokenizer,
     ExLlamaV2Lora
 )
 from exl2conv.generator import (
     ExLlamaV2Sampler,
     ExLlamaV2BaseGenerator
 )
-from exllamav2.generator.ngram import NgramCache
+from exl2conv.generator.ngram import NgramCache
 import torch
 import random
 import threading
-from exllamav2.generator.hooks import ExLlamaV2PostSamplingHook, ExLlamaV2PostSamplingResult
+from exl2conv.generator.hooks import ExLlamaV2PostSamplingHook, ExLlamaV2PostSamplingResult
 
 class ExLlamaV2StreamingGenerator(ExLlamaV2BaseGenerator):
 
     # Constants
 
     tail_decode_tokens: int = 2
     max_fallback_tokens: int = 4
```

### Comparing `exl2conv-0.0.18/exl2conv/headnorm.py` & `exl2conv-0.0.19/exl2conv/headnorm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 import torch
 from torch import nn
-from exllamav2.module import ExLlamaV2Module
-from exllamav2.ext import exllamav2_ext as ext_c, none_tensor
+from exl2conv.module import ExLlamaV2Module
+from exl2conv.ext import exl2conv_ext as ext_c, none_tensor
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
-    from exllamav2.model import ExLlamaV2
+    from exl2conv.model import ExLlamaV2
 
 class ExLlamaV2HeadNorm(ExLlamaV2Module):
 
     name: str = "LayerNorm"
 
     layernorm: nn.LayerNorm | None
     weight: nn.Parameter | None
```

### Comparing `exl2conv-0.0.18/exl2conv/layernorm.py` & `exl2conv-0.0.19/exl2conv/layernorm.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import torch
 from torch import nn
 from exl2conv.module import ExLlamaV2Module
 from exl2conv.ext import exl2conv_ext as ext_c, none_tensor
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
-    from exllamav2.model import ExLlamaV2
+    from exl2conv.model import ExLlamaV2
 
 class ExLlamaV2LayerNorm(ExLlamaV2Module):
 
     name: str = "LayerNorm"
 
     layernorm: nn.LayerNorm | None
     weight: nn.Parameter | None
```

### Comparing `exl2conv-0.0.18/exl2conv/linear.py` & `exl2conv-0.0.19/exl2conv/linear.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/lora.py` & `exl2conv-0.0.19/exl2conv/lora.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/mlp.py` & `exl2conv-0.0.19/exl2conv/mlp.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/model.py` & `exl2conv-0.0.19/exl2conv/model.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/model_init.py` & `exl2conv-0.0.19/exl2conv/model_init.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/module.py` & `exl2conv-0.0.19/exl2conv/module.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/moe_mlp.py` & `exl2conv-0.0.19/exl2conv/moe_mlp.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/parallel_decoder.py` & `exl2conv-0.0.19/exl2conv/parallel_decoder.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/rmsnorm.py` & `exl2conv-0.0.19/exl2conv/rmsnorm.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import torch
 from torch import nn
 from exl2conv.module import ExLlamaV2Module
 from exl2conv.ext import exl2conv_ext as ext_c
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
-    from exllamav2.model import ExLlamaV2
+    from exl2conv.model import ExLlamaV2
 
 class ExLlamaV2RMSNorm(ExLlamaV2Module):
 
     name: str = "RMSNorm"
 
     weight: nn.Parameter | None
     bias: nn.Parameter | None
```

### Comparing `exl2conv-0.0.18/exl2conv/server/websocket.py` & `exl2conv-0.0.19/exl2conv/server/websocket.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/server/websocket_actions.py` & `exl2conv-0.0.19/exl2conv/server/websocket_actions.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/tokenizer/base.py` & `exl2conv-0.0.19/exl2conv/tokenizer/base.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/tokenizer/hf.py` & `exl2conv-0.0.19/exl2conv/tokenizer/hf.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/tokenizer/spm.py` & `exl2conv-0.0.19/exl2conv/tokenizer/spm.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/tokenizer/tokenizer.py` & `exl2conv-0.0.19/exl2conv/tokenizer.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv/tokenizer.py` & `exl2conv-0.0.19/exl2conv/tokenizer/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,14 +273,29 @@
         :return:
             LongTensor of shape (1, 1) of token ID
         """
 
         return torch.tensor([[token_id]], dtype = torch.long)
 
 
+    def single_id(self, token: str) -> torch.Tensor:
+        """
+        Get the ID of a single token from exact string match
+
+        :param token:
+            Token
+
+        :return:
+            int
+        """
+
+        tid = self.extended_piece_to_id.get(token, self.get_piece_to_id_dict().get(token))
+        return tid
+
+
     # Encode string with added, unspecial tokens
 
     def encode_unspecial(self, text: str) -> list[int]:
 
         if not self.unspecial_piece_to_id:
             return self.tokenizer_model.encode(text)
```

### Comparing `exl2conv-0.0.18/exl2conv/util.py` & `exl2conv-0.0.19/exl2conv/util.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.18/exl2conv.egg-info/SOURCES.txt` & `exl2conv-0.0.19/exl2conv.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 exl2conv/conversion/standard_cal_data/wiki.utf8
 exl2conv/exl2conv_ext/config.h
 exl2conv/exl2conv_ext/ext_bindings.cpp
 exl2conv/exl2conv_ext/ext_cache.cpp
 exl2conv/exl2conv_ext/ext_cache.h
 exl2conv/exl2conv_ext/ext_gemm.cpp
 exl2conv/exl2conv_ext/ext_gemm.h
+exl2conv/exl2conv_ext/ext_hadamard.cpp
+exl2conv/exl2conv_ext/ext_hadamard.h
 exl2conv/exl2conv_ext/ext_norm.cpp
 exl2conv/exl2conv_ext/ext_norm.h
 exl2conv/exl2conv_ext/ext_qattn.cpp
 exl2conv/exl2conv_ext/ext_qattn.h
 exl2conv/exl2conv_ext/ext_qmatrix.cpp
 exl2conv/exl2conv_ext/ext_qmatrix.h
 exl2conv/exl2conv_ext/ext_qmlp.cpp
@@ -140,14 +142,27 @@
 exl2conv/generator/ngram.py
 exl2conv/generator/sampler.py
 exl2conv/generator/streaming.py
 exl2conv/generator/filters/__init__.py
 exl2conv/generator/filters/base.py
 exl2conv/generator/filters/prefix.py
 exl2conv/generator/filters/select.py
+exl2conv/hadamard/hadamard.py
+exl2conv/hadamard/hadamard_1.txt
+exl2conv/hadamard/hadamard_100.txt
+exl2conv/hadamard/hadamard_116.txt
+exl2conv/hadamard/hadamard_156.txt
+exl2conv/hadamard/hadamard_172.txt
+exl2conv/hadamard/hadamard_188.txt
+exl2conv/hadamard/hadamard_236.txt
+exl2conv/hadamard/hadamard_244.txt
+exl2conv/hadamard/hadamard_428.txt
+exl2conv/hadamard/hadamard_52.txt
+exl2conv/hadamard/hadamard_92.txt
+exl2conv/hadamard/primes.txt
 exl2conv/server/__init__.py
 exl2conv/server/websocket.py
 exl2conv/server/websocket_actions.py
 exl2conv/tokenizer/__init__.py
 exl2conv/tokenizer/base.py
 exl2conv/tokenizer/hf.py
 exl2conv/tokenizer/spm.py
```

### Comparing `exl2conv-0.0.18/setup.py` & `exl2conv-0.0.19/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     "ext_modules": [
         cpp_extension.CUDAExtension(
             extension_name,
             [
                 "exl2conv/exl2conv_ext/ext_bindings.cpp",
                 "exl2conv/exl2conv_ext/ext_cache.cpp",
                 "exl2conv/exl2conv_ext/ext_gemm.cpp",
+                "exl2conv/exl2conv_ext/ext_hadamard.cpp",
                 "exl2conv/exl2conv_ext/ext_norm.cpp",
                 "exl2conv/exl2conv_ext/ext_qattn.cpp",
                 "exl2conv/exl2conv_ext/ext_qmatrix.cpp",
                 "exl2conv/exl2conv_ext/ext_qmlp.cpp",
                 "exl2conv/exl2conv_ext/ext_quant.cpp",
                 "exl2conv/exl2conv_ext/ext_rope.cpp",
                 "exl2conv/exl2conv_ext/ext_safetensors.cpp",
```

