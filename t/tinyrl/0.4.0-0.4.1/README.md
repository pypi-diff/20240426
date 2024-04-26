# Comparing `tmp/tinyrl-0.4.0.tar.gz` & `tmp/tinyrl-0.4.1.tar.gz`

## Comparing `tinyrl-0.4.0.tar` & `tinyrl-0.4.1.tar`

### file list

```diff
@@ -1,299 +1,301 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/__init__.py
--rw-r--r--   0        0        0    10546 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers.h
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl_tools.h
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/version.h
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_arm.h
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu.h
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_blas.h
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_mkl.h
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_openblas.h
--rw-r--r--   0        0        0    13873 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cuda.h
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_dummy.h
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_esp32.h
--rw-r--r--   0        0        0    36524 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_generic.h
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/persist.h
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/persist_code.h
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/arm.h
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu.h
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_accelerate.h
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_blas.h
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_mkl.h
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_openblas.h
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_tensorboard.h
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cuda.h
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/devices.h
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/dummy.h
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/esp32.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/generic.h
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arduino.h
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arm.h
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu.h
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu_tensorboard.h
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cuda.h
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_dummy.h
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_arm.h
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_cpu.h
--rw-r--r--   0        0        0     9859 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_cuda.h
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_dummy.h
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_esp32.h
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_generic.h
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/activation_functions.h
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/nn.h
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu.h
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_blas.h
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mkl.h
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mux.h
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_openblas.h
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cuda.h
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_dummy.h
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_generic.h
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/persist.h
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/layers.h
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu.h
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_blas.h
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_mkl.h
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_openblas.h
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cuda.h
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_dummy.h
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_generic.h
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/layer.h
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/operations_generic.h
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/layer.h
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu.h
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_accelerate.h
--rw-r--r--   0        0        0    11332 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_blas.h
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_mkl.h
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_openblas.h
--rw-r--r--   0        0        0    25276 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cuda.h
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_dummy.h
--rw-r--r--   0        0        0    18492 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_generic.h
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist.h
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist_code.h
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/cuda/kernels.h
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/dsp.h
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/opt.h
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/dsp.h
--rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/opt.h
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/operations_generic.h
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/categorical_cross_entropy/operations_generic.h
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_cuda.h
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_generic.h
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/adam.h
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_cuda.h
--rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_generic.h
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist.h
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist_code.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/operations_generic.h
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/sgd.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_cuda.h
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_generic.h
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/parameters.h
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist.h
--rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist_code.h
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/models.h
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_cpu.h
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_cuda.h
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_dummy.h
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_generic.h
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/persist.h
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/persist_code.h
--rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/network.h
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_cpu.h
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_cuda.h
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_dummy.h
--rw-r--r--   0        0        0    21337 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_generic.h
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist.h
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist_code.h
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/network.h
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_cpu.h
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_generic.h
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/network.h
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_cpu.h
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_generic.h
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/output_view/model.h
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/model.h
--rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/operations_generic.h
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist.h
--rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist_code.h
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/arm.h
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu.h
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate.h
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl.h
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mux.h
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas.h
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard.h
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cuda.h
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy.h
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32.h
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_1.h
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_2.h
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_3.h
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_1.h
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_2.h
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_3.h
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_1.h
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_2.h
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_3.h
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_1.h
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_2.h
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_3.h
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_1.h
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_2.h
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_3.h
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_1.h
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_2.h
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_3.h
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_1.h
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_2.h
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_3.h
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_1.h
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_2.h
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_3.h
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_1.h
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_2.h
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_3.h
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/persist/code.h
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_arm.h
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_cpu.h
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_cuda.h
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_dummy.h
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_esp32.h
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_generic.h
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/operations_generic.h
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/rl.h
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/algorithms.h
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_cpu.h
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_cpu_mkl.h
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_generic.h
--rw-r--r--   0        0        0    21201 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic.h
--rw-r--r--   0        0        0    17846 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic_extensions.h
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/ppo.h
--rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/config.h
--rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/operations_generic.h
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/state.h
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu.h
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_mkl.h
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_mux.h
--rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cuda.h
--rw-r--r--   0        0        0    36332 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_generic.h
--rw-r--r--   0        0        0     8221 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/sac.h
--rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/config.h
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_cpu.h
--rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_generic.h
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/state.h
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu.h
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_mkl.h
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_mux.h
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cuda.h
--rw-r--r--   0        0        0    21772 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_generic.h
--rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/td3.h
--rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/config.h
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/operations_generic.h
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/state.h
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/components.h
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu.h
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu_mkl.h
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_generic.h
--rw-r--r--   0        0        0     8533 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/off_policy_runner.h
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu.h
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_accelerate.h
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_mkl.h
--rw-r--r--   0        0        0    10566 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cuda.h
--rw-r--r--   0        0        0    16438 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic.h
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic_per_env.h
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/on_policy_runner.h
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu.h
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_accelerate.h
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_mkl.h
--rw-r--r--   0        0        0    12759 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic.h
--rw-r--r--   0        0        0     8590 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_extensions.h
--rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_per_env.h
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/persist.h
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_cpu.h
--rw-r--r--   0        0        0     8285 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_generic.h
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/persist.h
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/replay_buffer.h
--rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/operations_generic.h
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/persist.h
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/running_normalizer.h
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/environments.h
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_cpu.h
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_generic.h
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/acrobot.h
--rw-r--r--   0        0        0    11982 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/operations_generic.h
--rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/ui.h
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/car.h
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_cpu.h
--rw-r--r--   0        0        0    10667 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_generic.h
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_json.h
--rw-r--r--   0        0        0    68731 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/track.h
--rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/ui.h
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/README.MD
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ant.h
--rw-r--r--   0        0        0    30495 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/model.h
--rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/operations_cpu.h
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ui.h
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_cpu.h
--rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_generic.h
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/pendulum.h
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui.h
--rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui_xeus.h
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/loop.h
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/config.h
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/operations_generic.h
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/state.h
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/config.h
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/operations_cpu.h
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/state.h
--rw-r--r--   0        0        0     8946 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/utils/evaluation.h
--rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation.h
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation_analysis.h
--rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/server.h
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/client.h
--rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_boost.h
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_cpu.h
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/persist.h
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/declarations_cpu.h
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_arm.h
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cpu.h
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cuda.h
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_dummy.h
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_esp32.h
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_generic.h
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/integrators.h
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/memcpy.h
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/typing.h
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/vector_operations.h
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_cuda.h
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_generic.h
--rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/interface/algorithms/ppo/template.h
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/interface/algorithms/sac/template.h
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/interface/algorithms/td3/template.h
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/interface/inference/inference.cpp
--rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/interface/python_environment/operations_cpu.h
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/interface/python_environment/python_environment.h
--rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/interface/training/training.cpp
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/__init__.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/accelerate.py
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/compile.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/link_accelerate.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/link_blas.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/link_mkl.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/load_checkpoint.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/load_module.py
--rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/ppo.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/render.py
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/sac.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/td3.py
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/training.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/utils.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 tinyrl-0.4.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 tinyrl-0.4.0/LICENSE
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 tinyrl-0.4.0/README.md
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 tinyrl-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 tinyrl-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/__init__.py
+-rw-r--r--   0        0        0    10546 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers.h
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl_tools.h
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/version.h
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_arm.h
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu.h
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_blas.h
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_mkl.h
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_openblas.h
+-rw-r--r--   0        0        0    13873 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cuda.h
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_dummy.h
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_esp32.h
+-rw-r--r--   0        0        0    36524 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_generic.h
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/persist.h
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/persist_code.h
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/arm.h
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu.h
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_accelerate.h
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_blas.h
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_mkl.h
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_openblas.h
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_tensorboard.h
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/cuda.h
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/devices.h
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/dummy.h
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/esp32.h
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/generic.h
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arduino.h
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arm.h
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu.h
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu_tensorboard.h
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cuda.h
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_dummy.h
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_arm.h
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_cpu.h
+-rw-r--r--   0        0        0     9859 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_cuda.h
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_dummy.h
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_esp32.h
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_generic.h
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/activation_functions.h
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/nn.h
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu.h
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_blas.h
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mkl.h
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mux.h
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_openblas.h
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cuda.h
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_dummy.h
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_generic.h
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/persist.h
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/layers.h
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu.h
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_blas.h
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_mkl.h
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_openblas.h
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cuda.h
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_dummy.h
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_generic.h
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/layer.h
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/operations_generic.h
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/layer.h
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu.h
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0    11380 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_blas.h
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_mkl.h
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_openblas.h
+-rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cuda.h
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_dummy.h
+-rw-r--r--   0        0        0    18598 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_generic.h
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist.h
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist_code.h
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/cuda/kernels.h
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/dsp.h
+-rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/opt.h
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/dsp.h
+-rw-r--r--   0        0        0     7162 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/opt.h
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/operations_generic.h
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/categorical_cross_entropy/operations_generic.h
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_cuda.h
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_generic.h
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/adam.h
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_cuda.h
+-rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_generic.h
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist.h
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist_code.h
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/operations_generic.h
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/sgd.h
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_cuda.h
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_generic.h
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/parameters.h
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist.h
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist_code.h
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/models.h
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_cpu.h
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_cuda.h
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_dummy.h
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_generic.h
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/persist.h
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/persist_code.h
+-rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/network.h
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_cpu.h
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_cuda.h
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_dummy.h
+-rw-r--r--   0        0        0    21585 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_generic.h
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist.h
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist_code.h
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/network.h
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_cpu.h
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_generic.h
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/network.h
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_cpu.h
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_generic.h
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/output_view/model.h
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/model.h
+-rw-r--r--   0        0        0    12469 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/operations_generic.h
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist.h
+-rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist_code.h
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/uniform_random/model.h
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/uniform_random/operations_generic.h
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/arm.h
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu.h
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate.h
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl.h
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mux.h
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas.h
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard.h
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cuda.h
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy.h
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32.h
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_1.h
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_2.h
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_3.h
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_1.h
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_2.h
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_3.h
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_1.h
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_2.h
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_3.h
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_1.h
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_2.h
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_3.h
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_1.h
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_2.h
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_3.h
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_1.h
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_2.h
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_3.h
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_1.h
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_2.h
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_3.h
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_1.h
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_2.h
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_3.h
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_1.h
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_2.h
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_3.h
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/persist/code.h
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_arm.h
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_cpu.h
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_cuda.h
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_dummy.h
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_esp32.h
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_generic.h
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/operations_generic.h
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/rl.h
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/algorithms.h
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_cpu.h
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_cpu_mkl.h
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_generic.h
+-rw-r--r--   0        0        0    21211 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic.h
+-rw-r--r--   0        0        0    17856 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic_extensions.h
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/ppo.h
+-rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/config.h
+-rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/operations_generic.h
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/state.h
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu.h
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_mkl.h
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_mux.h
+-rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cuda.h
+-rw-r--r--   0        0        0    37045 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_generic.h
+-rw-r--r--   0        0        0     8221 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/sac.h
+-rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/config.h
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_cpu.h
+-rw-r--r--   0        0        0     8107 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_generic.h
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/state.h
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu.h
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_mkl.h
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_mux.h
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cuda.h
+-rw-r--r--   0        0        0    21928 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_generic.h
+-rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/td3.h
+-rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/config.h
+-rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/operations_generic.h
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/state.h
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/components.h
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu.h
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu_mkl.h
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_generic.h
+-rw-r--r--   0        0        0     8533 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/off_policy_runner.h
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu.h
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_mkl.h
+-rw-r--r--   0        0        0    10600 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cuda.h
+-rw-r--r--   0        0        0    16980 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic.h
+-rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic_per_env.h
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/on_policy_runner.h
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu.h
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_mkl.h
+-rw-r--r--   0        0        0    12764 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic.h
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_extensions.h
+-rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_per_env.h
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/persist.h
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_cpu.h
+-rw-r--r--   0        0        0     8285 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_generic.h
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/persist.h
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/replay_buffer.h
+-rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/operations_generic.h
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/persist.h
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/running_normalizer.h
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/environments.h
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_cpu.h
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_generic.h
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/acrobot.h
+-rw-r--r--   0        0        0    11982 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/operations_generic.h
+-rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/ui.h
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/car.h
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_cpu.h
+-rw-r--r--   0        0        0    10667 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_generic.h
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_json.h
+-rw-r--r--   0        0        0    68731 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/track.h
+-rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/ui.h
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/README.MD
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ant.h
+-rw-r--r--   0        0        0    30495 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/model.h
+-rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/operations_cpu.h
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ui.h
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_cpu.h
+-rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_generic.h
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/pendulum.h
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui.h
+-rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui_xeus.h
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/loop.h
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/config.h
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/operations_generic.h
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/state.h
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/config.h
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/operations_cpu.h
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/state.h
+-rw-r--r--   0        0        0     8951 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/utils/evaluation.h
+-rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation.h
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation_analysis.h
+-rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/server.h
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/client.h
+-rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_boost.h
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_cpu.h
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/persist.h
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/declarations_cpu.h
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_arm.h
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cpu.h
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cuda.h
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_dummy.h
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_esp32.h
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_generic.h
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/integrators.h
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/memcpy.h
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/typing.h
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/vector_operations.h
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_cuda.h
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_generic.h
+-rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/interface/algorithms/ppo/template.h
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/interface/algorithms/sac/template.h
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/interface/algorithms/td3/template.h
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/interface/inference/inference.cpp
+-rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/interface/python_environment/operations_cpu.h
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/interface/python_environment/python_environment.h
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/interface/training/training.cpp
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/src/__init__.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/src/accelerate.py
+-rw-r--r--   0        0        0     7183 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/src/compile.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/src/link_accelerate.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/src/link_blas.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/src/link_mkl.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/src/load_checkpoint.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/src/load_module.py
+-rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/src/ppo.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/src/render.py
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/src/sac.py
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/src/td3.py
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/src/training.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 tinyrl-0.4.1/tinyrl/src/utils.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 tinyrl-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 tinyrl-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 tinyrl-0.4.1/README.md
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 tinyrl-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 tinyrl-0.4.1/PKG-INFO
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl_tools.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl_tools.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/version.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/version.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_arm.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_blas.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_blas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_mkl.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_openblas.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_openblas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cuda.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_dummy.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_esp32.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/persist.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/persist_code.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/containers/persist_code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/arm.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_accelerate.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_accelerate.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_blas.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_blas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_mkl.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_openblas.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_openblas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_tensorboard.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_tensorboard.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cuda.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/devices.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/devices.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/dummy.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/esp32.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/devices/esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arduino.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arduino.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arm.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu_tensorboard.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu_tensorboard.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cuda.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_dummy.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_arm.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_cpu.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_cuda.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_dummy.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_esp32.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/activation_functions.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/activation_functions.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mux.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mux.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/layer.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/layer.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/operations_generic.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #include "layer.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
-    template<typename DEVICE, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    void evaluate(DEVICE& device, const nn::layers::concat_constant::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output) {
+    template<typename DEVICE, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    void evaluate(DEVICE& device, const nn::layers::concat_constant::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         static_assert(nn::layers::concat_constant::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         // Warning do not use the same buffer for input and output!
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         using TI = typename DEVICE::index_t;
         auto input_target_view = view(device, output, matrix::ViewSpec<BATCH_SIZE, LAYER_SPEC::INPUT_DIM>{});
         auto constant_target_view = view(device, output, matrix::ViewSpec<BATCH_SIZE, LAYER_SPEC::INPUT_DIM>{}, 0, LAYER_SPEC::INPUT_DIM);
         copy(device, device, input, input_target_view);
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/layer.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/layer.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_accelerate.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_accelerate.h`

 * *Files 3% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 #include <Accelerate/Accelerate.h>
 #include "operations_cpu_blas.h"
 #include "../../../devices/cpu_accelerate.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
-    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    RL_TOOLS_FUNCTION_PLACEMENT void evaluate(devices::CPU_ACCELERATE<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output) {
-        evaluate((devices::CPU_BLAS<DEV_SPEC>&) device, layer, input, output);
+    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    RL_TOOLS_FUNCTION_PLACEMENT void evaluate(devices::CPU_ACCELERATE<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
+        evaluate((devices::CPU_BLAS<DEV_SPEC>&) device, layer, input, output, rng);
     }
 
-    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    RL_TOOLS_FUNCTION_PLACEMENT void forward(devices::CPU_ACCELERATE<DEV_SPEC>& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output) {
-        forward((devices::CPU_BLAS<DEV_SPEC>&) device, layer, input, output);
+    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    RL_TOOLS_FUNCTION_PLACEMENT void forward(devices::CPU_ACCELERATE<DEV_SPEC>& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
+        forward((devices::CPU_BLAS<DEV_SPEC>&) device, layer, input, output, rng);
     }
 
     template<typename DEV_SPEC, typename LAYER_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC>
     RL_TOOLS_FUNCTION_PLACEMENT void backward_input(devices::CPU_ACCELERATE<DEV_SPEC>& device, const nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
         backward_input((devices::CPU_BLAS<DEV_SPEC> &) device, layer, d_output, d_input);
     }
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC>
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_blas.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_blas.h`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 // extern "C" {
 //     void cblas_sgemm(const enum CBLAS_ORDER Order, const enum CBLAS_TRANSPOSE TransA, const enum CBLAS_TRANSPOSE TransB, const int M, const int N, const int K, const float alpha, const float *A, const int lda, const float *B, const int ldb, const float beta, float *C, const int ldc);
 //     void cblas_dgemm(const enum CBLAS_ORDER Order, const enum CBLAS_TRANSPOSE TransA, const enum CBLAS_TRANSPOSE TransB, const int M, const int N, const int K, const double alpha, const double *A, const int lda, const double *B, const int ldb, const double beta, double *C, const int ldc);
 // }
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
-    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    void evaluate(devices::CPU_BLAS<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output) {
+    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    void evaluate(devices::CPU_BLAS<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
 
         // Warning do not use the same buffer for input and output!
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         using DEVICE = devices::CPU_BLAS<DEV_SPEC>;
         using T = typename LAYER_SPEC::T;
         using TI = typename DEVICE::index_t;
@@ -44,16 +44,16 @@
         for(TI i = 0; i < BATCH_SIZE; i++){
             for(TI j = 0; j < LAYER_SPEC::OUTPUT_DIM; j++){
                 set(output, i, j, activation<typename DEVICE::SPEC::MATH, T, LAYER_SPEC::ACTIVATION_FUNCTION>(get(output, i, j)));
             }
         }
     }
 
-    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    void forward(devices::CPU_BLAS<DEV_SPEC>& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output) {
+    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    void forward(devices::CPU_BLAS<DEV_SPEC>& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         // Warning do not use the same buffer for input and output!
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         using T = typename LAYER_SPEC::T;
         using TI = typename devices::CPU_BLAS<DEV_SPEC>::index_t;
 
         constexpr T alpha = 1;
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_mkl.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_mkl.h`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 #define RL_TOOLS_NN_LAYERS_DENSE_OPERATIONS_CPU_MKL_H
 
 #include "operations_cpu_blas.h"
 #include "../../../devices/cpu_mkl.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
-    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    RL_TOOLS_FUNCTION_PLACEMENT void evaluate(devices::CPU_MKL<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output){
-        evaluate((devices::CPU_BLAS<DEV_SPEC>&) device, layer, input, output);
+    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    RL_TOOLS_FUNCTION_PLACEMENT void evaluate(devices::CPU_MKL<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng){
+        evaluate((devices::CPU_BLAS<DEV_SPEC>&) device, layer, input, output, rng);
     }
 
-    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    RL_TOOLS_FUNCTION_PLACEMENT void forward(devices::CPU_MKL<DEV_SPEC>& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output){
-        forward((devices::CPU_BLAS<DEV_SPEC>&) device, layer, input, output);
+    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    RL_TOOLS_FUNCTION_PLACEMENT void forward(devices::CPU_MKL<DEV_SPEC>& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng){
+        forward((devices::CPU_BLAS<DEV_SPEC>&) device, layer, input, output, rng);
     }
 
     template<typename DEV_SPEC, typename LAYER_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC>
     RL_TOOLS_FUNCTION_PLACEMENT void backward_input(devices::CPU_MKL<DEV_SPEC>& device, const nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
         backward_input((devices::CPU_BLAS<DEV_SPEC> &) device, layer, d_output, d_input);
     }
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC>
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_openblas.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_openblas.h`

 * *Files 5% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 #define RL_TOOLS_NN_LAYERS_DENSE_OPERATIONS_CPU_OPENBLAS_H
 
 #include "operations_cpu_blas.h"
 #include "../../../devices/cpu_openblas.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
-    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    RL_TOOLS_FUNCTION_PLACEMENT void evaluate(devices::CPU_OPENBLAS<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output) {
-        evaluate((devices::CPU_BLAS<DEV_SPEC>&) device, layer, input, output);
+    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    RL_TOOLS_FUNCTION_PLACEMENT void evaluate(devices::CPU_OPENBLAS<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
+        evaluate((devices::CPU_BLAS<DEV_SPEC>&) device, layer, input, output, rng);
     }
 
-    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    RL_TOOLS_FUNCTION_PLACEMENT void forward(devices::CPU_OPENBLAS<DEV_SPEC>& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output) {
-        forward((devices::CPU_BLAS<DEV_SPEC>&) device, layer, input, output);
+    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    RL_TOOLS_FUNCTION_PLACEMENT void forward(devices::CPU_OPENBLAS<DEV_SPEC>& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
+        forward((devices::CPU_BLAS<DEV_SPEC>&) device, layer, input, output, rng);
     }
 
     template<typename DEV_SPEC, typename LAYER_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC>
     RL_TOOLS_FUNCTION_PLACEMENT void backward_input(devices::CPU_OPENBLAS<DEV_SPEC>& device, const nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
         backward_input((devices::CPU_BLAS<DEV_SPEC> &) device, layer, d_output, d_input);
     }
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC>
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cuda.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cuda.h`

 * *Files 1% similar despite different names*

```diff
@@ -167,16 +167,16 @@
                 set(layer.weights.gradient_second_order_moment, output_i, input_i, d_weight_second_order_moment);
                 T weight_update = optimizer.parameters.alpha * optimizer.first_order_moment_bias_correction * d_weight_first_order_moment / (math::sqrt(typename DEVICE::SPEC::MATH_DEVICE_ACCURATE(), d_weight_second_order_moment * optimizer.second_order_moment_bias_correction) + optimizer.parameters.epsilon);
                 increment(layer.weights.parameters, output_i, input_i, -weight_update);
             }
         }
     }
 
-    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    void evaluate(devices::CUDA<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output){
+    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    void evaluate(devices::CUDA<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng){
         // Warning do not use the same buffer for input and output!
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         static_assert(INPUT_SPEC::COL_PITCH == 1);
         static_assert(OUTPUT_SPEC::COL_PITCH == 1);
         static_assert(decltype(layer.weights.parameters)::COL_PITCH == 1);
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         using DEVICE = devices::CUDA<DEV_SPEC>;
@@ -203,16 +203,16 @@
             if(stat != CUBLAS_STATUS_SUCCESS){
                 std::cout << "CUBLAS ERROR: " << cublasGetStatusString(stat) << std::endl;
             }
             nn::dense::cuda::activation(device, layer, output, output);
         }
     }
 
-    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    void forward(devices::CUDA<DEV_SPEC>& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output) {
+    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    void forward(devices::CUDA<DEV_SPEC>& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         // Warning do not use the same buffer for input and output!
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         static_assert(INPUT_SPEC::COL_PITCH == 1);
         static_assert(OUTPUT_SPEC::COL_PITCH == 1);
         static_assert(decltype(layer.weights.parameters)::COL_PITCH == 1);
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         using T = typename LAYER_SPEC::T;
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_generic.h`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,16 @@
     }
     template<typename DEVICE, typename SPEC, typename RNG>
     void init_weights(DEVICE& device, nn::layers::dense::Layer<SPEC>& layer, RNG& rng) {
         init_kaiming(device, layer, rng);
     }
 
 #ifndef RL_TOOLS_NN_DISABLE_GENERIC_FORWARD_BACKWARD
-    template<typename DEVICE, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    void evaluate(DEVICE& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output) {
+    template<typename DEVICE, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    void evaluate(DEVICE& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         // Warning do not use the same buffer for input and output!
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         using TI = typename DEVICE::index_t;
         for(TI batch_i=0; batch_i < BATCH_SIZE; batch_i++){
             for(TI output_i = 0; output_i < LAYER_SPEC::OUTPUT_DIM; output_i++) {
                 set(output, batch_i, output_i, get(layer.biases.parameters, 0, output_i));
@@ -80,16 +80,16 @@
                     increment(output, batch_i, output_i, get(layer.weights.parameters, output_i, input_i) * get(input, batch_i, input_i));
                 }
                 set(output, batch_i, output_i, activation<typename DEVICE::SPEC::MATH, typename LAYER_SPEC::T, LAYER_SPEC::ACTIVATION_FUNCTION>(get(output, batch_i, output_i)));
             }
         }
     }
 
-    template<typename DEVICE, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    void forward(DEVICE& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output){
+    template<typename DEVICE, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    void forward(DEVICE& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng){
         // Warning do not use the same buffer for input and output!
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         using T = typename LAYER_SPEC::T;
         using TI = typename DEVICE::index_t;
 
         for(TI batch_i=0; batch_i < BATCH_SIZE; batch_i++){
@@ -100,24 +100,24 @@
                 }
                 set(output, batch_i, i, activation<typename DEVICE::SPEC::MATH, T, LAYER_SPEC::ACTIVATION_FUNCTION>(get(layer.pre_activations, batch_i, i)));
             }
         }
     }
 #endif
 
-    template<typename DEVICE, typename LAYER_SPEC, typename INPUT_SPEC>
-    void forward(DEVICE& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input) {
+    template<typename DEVICE, typename LAYER_SPEC, typename INPUT_SPEC, typename RNG>
+    void forward(DEVICE& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, RNG& rng) {
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, typename decltype(layer.output)::SPEC>);
-        forward(device, (nn::layers::dense::LayerBackward<LAYER_SPEC>&)layer, input, layer.output);
+        forward(device, (nn::layers::dense::LayerBackward<LAYER_SPEC>&)layer, input, layer.output, rng);
     }
-    template<typename DEVICE, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    void forward(DEVICE& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output) {
+    template<typename DEVICE, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    void forward(DEVICE& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         // compile time warning if used
-        forward(device, layer, input);
+        forward(device, layer, input, rng);
         copy(device, device, layer.output, output);
     }
 
 #ifndef RL_TOOLS_NN_DISABLE_GENERIC_FORWARD_BACKWARD
     template<typename DEVICE, typename LAYER_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC>
     void backward_input(DEVICE& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input){
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, D_INPUT_SPEC, D_OUTPUT_SPEC>);
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist_code.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist_code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/cuda/kernels.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/cuda/kernels.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/dsp.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/dsp.h`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 #include "../../../../nn/layers/dense/operations_generic.h"
 //#include "../../../../utils/generic/memcpy.h"
 #include "../../../../devices/arm.h"
 #include "arm_math.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
-    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    void evaluate(devices::arm::DSP<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output) {
+    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    void evaluate(devices::arm::DSP<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         static_assert(INPUT_SPEC::ROW_PITCH == INPUT_SPEC::COLS);
         static_assert(INPUT_SPEC::COL_PITCH == 1);
         static_assert(OUTPUT_SPEC::ROW_PITCH == OUTPUT_SPEC::COLS);
         static_assert(OUTPUT_SPEC::COL_PITCH == 1);
         static_assert(decltype(layer.weights.parameters)::ROW_PITCH == INPUT_SPEC::COLS);
         static_assert(decltype(layer.weights.parameters)::COL_PITCH == 1);
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/opt.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/opt.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 #include "../../../../version.h"
-#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_NN_LAYERS_DENSE_OPERATIONS_ARM_OPT_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
+#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_NN_LAYERS_DENSE_OPERATIONS_ESP32_OPT_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
-#define RL_TOOLS_NN_LAYERS_DENSE_OPERATIONS_ARM_OPT_H
+#define RL_TOOLS_NN_LAYERS_DENSE_OPERATIONS_ESP32_OPT_H
 
-#include "../../../../nn/layers/dense/operations_generic.h"
-//#include "../../../../utils/generic/memcpy.h"
-#include "../../../../devices/arm.h"
+#include "../../../../devices/esp32.h"
+#include "../../../../nn/layers/dense/layer.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
-    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    void evaluate(devices::arm::OPT<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output) {
+    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    void evaluate(devices::esp32::OPT<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         // For performance reasons: restricted to dense row-major matrices (row-pitch is allowed)
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         static_assert(INPUT_SPEC::COL_PITCH == 1);
         static_assert(OUTPUT_SPEC::COL_PITCH == 1);
         static_assert(decltype(layer.weights.parameters)::COL_PITCH == 1);
         static_assert(decltype(layer.biases.parameters)::COL_PITCH == 1);
 //        static_assert(utils::typing::is_same_v<typename LAYER_SPEC::T, float>);
 
         // Warning do not use the same buffer for input and output!
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         // static_assert(BATCH_SIZE == 1);
-        using DEVICE = devices::ARM<DEV_SPEC>;
+        using DEVICE = devices::esp32::OPT<DEV_SPEC>;
         using T = typename LAYER_SPEC::T;
-        using TI = typename LAYER_SPEC::TI;
         {
 
             T *weights_row;
             T *input_row = input._data;
             T *output_row = output._data;
 
             T *weights_element, *biases_element, *input_element, *output_element;
 
             T acc;
-            TI weights_row_i, batch_i = BATCH_SIZE, input_i;
+            uint32_t weights_row_i, batch_i = BATCH_SIZE, input_i;
 
             {
                 do{
                     output_element = output_row;
                     biases_element = layer.biases.parameters._data;
 
                     weights_row_i = LAYER_SPEC::OUTPUT_DIM;
@@ -46,24 +44,24 @@
 
                     do{
                         acc = 0.0f;
                         input_element = input_row;
                         weights_element = weights_row;
 
                         // reduction
-                        input_i = ((TI)LAYER_SPEC::INPUT_DIM) >> 2U;
+                        input_i = ((uint32_t)LAYER_SPEC::INPUT_DIM) >> 2U;
                         while (input_i > 0U){
                             acc += *weights_element++ * *input_element++;
                             acc += *weights_element++ * *input_element++;
                             acc += *weights_element++ * *input_element++;
                             acc += *weights_element++ * *input_element++;
 
                             input_i--;
                         }
-                        input_i = ((TI)LAYER_SPEC::INPUT_DIM) % 0x4U;
+                        input_i = ((uint32_t)LAYER_SPEC::INPUT_DIM) % 0x4U;
                         while (input_i > 0U){
                             acc += *weights_element++ * *input_element++;
                             input_i--;
                         }
 
                         acc += *biases_element++;
                         acc = activation<typename DEVICE::SPEC::MATH, T, LAYER_SPEC::ACTIVATION_FUNCTION>(acc);
@@ -80,28 +78,28 @@
                     input_row += INPUT_SPEC::ROW_PITCH;
                     batch_i--;
                 }while (batch_i > 0U);
             }
         }
     }
 
-    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    void forward(devices::ARM<DEV_SPEC>& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output) {
+    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    void forward(devices::esp32::OPT<DEV_SPEC>& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         // For performance reasons: restricted to dense row-major matrices (row-pitch is allowed)
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         static_assert(INPUT_SPEC::COL_PITCH == 1);
         static_assert(OUTPUT_SPEC::COL_PITCH == 1);
         static_assert(decltype(layer.weights.parameters)::COL_PITCH == 1);
         static_assert(decltype(layer.biases.parameters)::COL_PITCH == 1);
 //        static_assert(utils::typing::is_same_v<typename LAYER_SPEC::T, float>);
 
         // Warning do not use the same buffer for input and output!
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         // static_assert(BATCH_SIZE == 1);
-        using DEVICE = devices::ARM<DEV_SPEC>;
+        using DEVICE = devices::esp32::OPT<DEV_SPEC>;
         using T = typename LAYER_SPEC::T;
         using TI = typename DEVICE::index_t;
         {
 
             T *weights_row;
             T *input_row = input._data;
             T *pre_activations_row = layer.pre_activations._data;
@@ -161,8 +159,8 @@
                 }while (batch_i > 0U);
             }
         }
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 
-#endif
+#endif
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/dsp.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/dsp.h`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 #include "../../../../devices/esp32.h"
 #include "../../../../nn/layers/dense/layer.h"
 
 #include "esp_dsp.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
-    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    void evaluate(devices::esp32::DSP<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output) {
+    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    void evaluate(devices::esp32::DSP<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         // For performance reasons: restricted to dense row-major matrices (row-pitch is allowed)
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         static_assert(INPUT_SPEC::ROWS == 1); // only supporting batch size of 1 for now
         static_assert(INPUT_SPEC::COL_PITCH == 1);
         static_assert(OUTPUT_SPEC::COL_PITCH == 1);
         static_assert(decltype(layer.weights.parameters)::COL_PITCH == 1);
         static_assert(decltype(layer.biases.parameters)::COL_PITCH == 1);
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/opt.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/opt.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 #include "../../../../version.h"
-#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_NN_LAYERS_DENSE_OPERATIONS_ESP32_OPT_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
+#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_NN_LAYERS_DENSE_OPERATIONS_ARM_OPT_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
-#define RL_TOOLS_NN_LAYERS_DENSE_OPERATIONS_ESP32_OPT_H
+#define RL_TOOLS_NN_LAYERS_DENSE_OPERATIONS_ARM_OPT_H
 
-#include "../../../../devices/esp32.h"
-#include "../../../../nn/layers/dense/layer.h"
+#include "../../../../nn/layers/dense/operations_generic.h"
+//#include "../../../../utils/generic/memcpy.h"
+#include "../../../../devices/arm.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
-    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    void evaluate(devices::esp32::OPT<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output) {
+    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    void evaluate(devices::arm::OPT<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         // For performance reasons: restricted to dense row-major matrices (row-pitch is allowed)
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         static_assert(INPUT_SPEC::COL_PITCH == 1);
         static_assert(OUTPUT_SPEC::COL_PITCH == 1);
         static_assert(decltype(layer.weights.parameters)::COL_PITCH == 1);
         static_assert(decltype(layer.biases.parameters)::COL_PITCH == 1);
 //        static_assert(utils::typing::is_same_v<typename LAYER_SPEC::T, float>);
 
         // Warning do not use the same buffer for input and output!
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         // static_assert(BATCH_SIZE == 1);
-        using DEVICE = devices::esp32::OPT<DEV_SPEC>;
+        using DEVICE = devices::ARM<DEV_SPEC>;
         using T = typename LAYER_SPEC::T;
+        using TI = typename LAYER_SPEC::TI;
         {
 
             T *weights_row;
             T *input_row = input._data;
             T *output_row = output._data;
 
             T *weights_element, *biases_element, *input_element, *output_element;
 
             T acc;
-            uint32_t weights_row_i, batch_i = BATCH_SIZE, input_i;
+            TI weights_row_i, batch_i = BATCH_SIZE, input_i;
 
             {
                 do{
                     output_element = output_row;
                     biases_element = layer.biases.parameters._data;
 
                     weights_row_i = LAYER_SPEC::OUTPUT_DIM;
@@ -44,24 +46,24 @@
 
                     do{
                         acc = 0.0f;
                         input_element = input_row;
                         weights_element = weights_row;
 
                         // reduction
-                        input_i = ((uint32_t)LAYER_SPEC::INPUT_DIM) >> 2U;
+                        input_i = ((TI)LAYER_SPEC::INPUT_DIM) >> 2U;
                         while (input_i > 0U){
                             acc += *weights_element++ * *input_element++;
                             acc += *weights_element++ * *input_element++;
                             acc += *weights_element++ * *input_element++;
                             acc += *weights_element++ * *input_element++;
 
                             input_i--;
                         }
-                        input_i = ((uint32_t)LAYER_SPEC::INPUT_DIM) % 0x4U;
+                        input_i = ((TI)LAYER_SPEC::INPUT_DIM) % 0x4U;
                         while (input_i > 0U){
                             acc += *weights_element++ * *input_element++;
                             input_i--;
                         }
 
                         acc += *biases_element++;
                         acc = activation<typename DEVICE::SPEC::MATH, T, LAYER_SPEC::ACTIVATION_FUNCTION>(acc);
@@ -78,28 +80,28 @@
                     input_row += INPUT_SPEC::ROW_PITCH;
                     batch_i--;
                 }while (batch_i > 0U);
             }
         }
     }
 
-    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    void forward(devices::esp32::OPT<DEV_SPEC>& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output) {
+    template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    void forward(devices::ARM<DEV_SPEC>& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         // For performance reasons: restricted to dense row-major matrices (row-pitch is allowed)
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         static_assert(INPUT_SPEC::COL_PITCH == 1);
         static_assert(OUTPUT_SPEC::COL_PITCH == 1);
         static_assert(decltype(layer.weights.parameters)::COL_PITCH == 1);
         static_assert(decltype(layer.biases.parameters)::COL_PITCH == 1);
 //        static_assert(utils::typing::is_same_v<typename LAYER_SPEC::T, float>);
 
         // Warning do not use the same buffer for input and output!
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         // static_assert(BATCH_SIZE == 1);
-        using DEVICE = devices::esp32::OPT<DEV_SPEC>;
+        using DEVICE = devices::ARM<DEV_SPEC>;
         using T = typename LAYER_SPEC::T;
         using TI = typename DEVICE::index_t;
         {
 
             T *weights_row;
             T *input_row = input._data;
             T *pre_activations_row = layer.pre_activations._data;
@@ -159,8 +161,8 @@
                 }while (batch_i > 0U);
             }
         }
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 
-#endif
+#endif
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/categorical_cross_entropy/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/categorical_cross_entropy/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_cuda.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/adam.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/adam.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_cuda.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist_code.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist_code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/sgd.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/sgd.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/parameters.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/parameters.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist_code.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist_code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/network.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/network.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_generic.h`

 * *Files 5% similar despite different names*

```diff
@@ -61,104 +61,104 @@
             static_assert(!MODEL_SPEC::ENFORCE_FLOATING_POINT_TYPE || utils::typing::is_same_v<typename MODEL_SPEC::T, typename INPUT_SPEC::T>);
             static_assert(!MODEL_SPEC::ENFORCE_FLOATING_POINT_TYPE || utils::typing::is_same_v<typename INPUT_SPEC::T, typename OUTPUT_SPEC::T>);
             return true;
         }
         template <typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
         constexpr bool check_input_output = check_input_output_f<MODEL_SPEC, INPUT_SPEC, OUTPUT_SPEC>();
     }
-    template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename TEMP_SPEC>
-    void evaluate_memless(DEVICE& device, const nn_models::mlp::NeuralNetwork<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, Matrix<TEMP_SPEC>& layer_output_tick, Matrix<TEMP_SPEC>& layer_output_tock){
+    template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename TEMP_SPEC, typename RNG>
+    void evaluate_memless(DEVICE& device, const nn_models::mlp::NeuralNetwork<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, Matrix<TEMP_SPEC>& layer_output_tick, Matrix<TEMP_SPEC>& layer_output_tock, RNG& rng){
         static_assert(nn_models::mlp::check_input_output<MODEL_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         static_assert(TEMP_SPEC::ROWS >= BATCH_SIZE);
         static_assert(TEMP_SPEC::COLS >= MODEL_SPEC::HIDDEN_DIM);
-        evaluate(device, network.input_layer, input, layer_output_tick);
+        evaluate(device, network.input_layer, input, layer_output_tick, rng);
         for (typename DEVICE::index_t layer_i = 0; layer_i < MODEL_SPEC::NUM_HIDDEN_LAYERS; layer_i++){
             if(layer_i % 2 == 0){
-                evaluate(device, network.hidden_layers[layer_i], layer_output_tick, layer_output_tock);
+                evaluate(device, network.hidden_layers[layer_i], layer_output_tick, layer_output_tock, rng);
             } else {
-                evaluate(device, network.hidden_layers[layer_i], layer_output_tock, layer_output_tick);
+                evaluate(device, network.hidden_layers[layer_i], layer_output_tock, layer_output_tick, rng);
             }
         }
         if constexpr(MODEL_SPEC::NUM_HIDDEN_LAYERS % 2 == 0){
-            evaluate(device, network.output_layer, layer_output_tick, output);
+            evaluate(device, network.output_layer, layer_output_tick, output, rng);
         } else {
-            evaluate(device, network.output_layer, layer_output_tock, output);
+            evaluate(device, network.output_layer, layer_output_tock, output, rng);
         }
     }
-    template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename BUFFER_MODEL_SPEC>
-    void evaluate(DEVICE& device, const nn_models::mlp::NeuralNetwork<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, nn_models::mlp::NeuralNetworkBuffers<BUFFER_MODEL_SPEC>& buffers){
+    template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename BUFFER_MODEL_SPEC, typename RNG>
+    void evaluate(DEVICE& device, const nn_models::mlp::NeuralNetwork<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, nn_models::mlp::NeuralNetworkBuffers<BUFFER_MODEL_SPEC>& buffers, RNG& rng){
         static_assert(BUFFER_MODEL_SPEC::BATCH_SIZE >= OUTPUT_SPEC::ROWS);
         static_assert(BUFFER_MODEL_SPEC::SPEC::HIDDEN_DIM == MODEL_SPEC::HIDDEN_DIM);
         auto tick = view(device, buffers.tick, matrix::ViewSpec<OUTPUT_SPEC::ROWS, BUFFER_MODEL_SPEC::SPEC::HIDDEN_DIM>{});
         auto tock = view(device, buffers.tock, matrix::ViewSpec<OUTPUT_SPEC::ROWS, BUFFER_MODEL_SPEC::SPEC::HIDDEN_DIM>{});
-        evaluate_memless(device, network, input, output, tick, tock);
+        evaluate_memless(device, network, input, output, tick, tock, rng);
     }
-    template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    void evaluate(DEVICE& device, const nn_models::mlp::NeuralNetwork<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output){
+    template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    void evaluate(DEVICE& device, const nn_models::mlp::NeuralNetwork<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng){
         static_assert(nn_models::mlp::check_input_output<MODEL_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         using T = typename MODEL_SPEC::T;
         using TICK_TOCK_SPEC = matrix::Specification<T, typename DEVICE::index_t, BATCH_SIZE, MODEL_SPEC::HIDDEN_DIM>;
 #ifndef RL_TOOLS_DISABLE_DYNAMIC_MEMORY_ALLOCATIONS
         MatrixDynamic<TICK_TOCK_SPEC> layer_output_tick;
         MatrixDynamic<TICK_TOCK_SPEC> layer_output_tock;
 #else
         MatrixStatic<TICK_TOCK_SPEC> layer_output_tick;
         MatrixStatic<TICK_TOCK_SPEC> layer_output_tock;
 #endif
         malloc(device, layer_output_tick);
         malloc(device, layer_output_tock);
-        evaluate_memless(device, network, input, output, layer_output_tick, layer_output_tock);
+        evaluate_memless(device, network, input, output, layer_output_tick, layer_output_tock, rng);
         free(device, layer_output_tick);
         free(device, layer_output_tock);
     }
 
     // forward modifies intermediate outputs and pre activations to facilitate backward pass
-    template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename TEMP_SPEC>
-    void forward_memless(DEVICE& device, const nn_models::mlp::NeuralNetwork<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, Matrix<TEMP_SPEC>& layer_output_tick, Matrix<TEMP_SPEC>& layer_output_tock){
+    template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename TEMP_SPEC, typename RNG>
+    void forward_memless(DEVICE& device, const nn_models::mlp::NeuralNetwork<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, Matrix<TEMP_SPEC>& layer_output_tick, Matrix<TEMP_SPEC>& layer_output_tock, RNG& rng){
         static_assert(nn_models::mlp::check_input_output<MODEL_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         static_assert(TEMP_SPEC::ROWS == BATCH_SIZE);
         static_assert(TEMP_SPEC::COLS == MODEL_SPEC::HIDDEN_DIM);
 
-        forward(network.input_layer, input, layer_output_tick);
+        forward(network.input_layer, input, layer_output_tick, rng);
         for (typename DEVICE::index_t layer_i = 0; layer_i < MODEL_SPEC::NUM_HIDDEN_LAYERS; layer_i++){
             if(layer_i % 2 == 0){
-                forward(network.hidden_layers[layer_i], layer_output_tick, layer_output_tock);
+                forward(network.hidden_layers[layer_i], layer_output_tick, layer_output_tock, rng);
             } else {
-                forward(network.hidden_layers[layer_i], layer_output_tock, layer_output_tick);
+                forward(network.hidden_layers[layer_i], layer_output_tock, layer_output_tick, rng);
             }
         }
         if constexpr(MODEL_SPEC::NUM_HIDDEN_LAYERS % 2 == 0){
-            forward(network.output_layer, layer_output_tick, output);
+            forward(network.output_layer, layer_output_tick, output, rng);
         } else {
-            forward(network.output_layer, layer_output_tock, output);
+            forward(network.output_layer, layer_output_tock, output, rng);
         }
     }
-    template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename BUFFER_MODEL_SPEC>
-    void forward(DEVICE& device, const nn_models::mlp::NeuralNetwork<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, nn_models::mlp::NeuralNetworkBuffers<BUFFER_MODEL_SPEC> buffers){
+    template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename BUFFER_MODEL_SPEC, typename RNG>
+    void forward(DEVICE& device, const nn_models::mlp::NeuralNetwork<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, nn_models::mlp::NeuralNetworkBuffers<BUFFER_MODEL_SPEC> buffers, RNG& rng){
         static_assert(BUFFER_MODEL_SPEC::BATCH_SIZE == OUTPUT_SPEC::ROWS);
         forward_memless(device, network, input, output, buffers.tick, buffers.tock);
     }
-    template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC>
-    void forward(DEVICE& device, nn_models::mlp::NeuralNetworkBackwardGradient<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input) {
-        forward(device, network.input_layer, input);
+    template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename RNG>
+    void forward(DEVICE& device, nn_models::mlp::NeuralNetworkBackwardGradient<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, RNG& rng) {
+        forward(device, network.input_layer, input, rng);
 
         auto current_output = network.input_layer.output;
         for (typename DEVICE::index_t layer_i = 0; layer_i < MODEL_SPEC::NUM_HIDDEN_LAYERS; layer_i++){
-            forward(device, network.hidden_layers[layer_i], current_output);
+            forward(device, network.hidden_layers[layer_i], current_output, rng);
             current_output = network.hidden_layers[layer_i].output;
         }
-        forward(device, network.output_layer, current_output);
+        forward(device, network.output_layer, current_output, rng);
     }
-    template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
-    void forward(DEVICE& device, nn_models::mlp::NeuralNetworkBackwardGradient<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output) {
+    template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
+    void forward(DEVICE& device, nn_models::mlp::NeuralNetworkBackwardGradient<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         static_assert(nn_models::mlp::check_input_output<MODEL_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
-        forward(device, network, input);
+        forward(device, network, input, rng);
         copy(device, device, network.output_layer.output, output);
     }
 
     template<typename DEVICE, typename SPEC>
     void zero_gradient(DEVICE& device, nn_models::mlp::NeuralNetwork<SPEC>& network) {
         zero_gradient(device, network.input_layer);
         for(typename DEVICE::index_t i = 0; i < SPEC::NUM_HIDDEN_LAYERS; i++){
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist_code.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist_code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/network.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/network.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/network.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/network.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/output_view/model.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/output_view/model.h`

 * *Files 3% similar despite different names*

```diff
@@ -24,23 +24,23 @@
         typename SPEC::MODEL& model;
         MODEL(typename SPEC::MODEL& model): model(model){}
     };
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
-    template <typename DEVICE, typename SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename BUFFERS>
-    void evaluate(DEVICE& device, const nn_models::output_view::MODEL<SPEC>& actor, Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, BUFFERS& eval_buffers){
+    template <typename DEVICE, typename SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename BUFFERS, typename RNG>
+    void evaluate(DEVICE& device, const nn_models::output_view::MODEL<SPEC>& actor, Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, BUFFERS& eval_buffers, RNG& rng){
         using T = typename OUTPUT_SPEC::T;
         using TI = typename OUTPUT_SPEC::TI;
         static_assert(OUTPUT_SPEC::COLS == SPEC::DIM);
         static_assert(BUFFERS::BATCH_SIZE == SPEC::DIM);
         MatrixDynamic<matrix::Specification<T, TI, OUTPUT_SPEC::ROWS, SPEC::MODEL::OUTPUT_DIM>> actor_output;
         malloc(device, actor_output);
-        evaluate(device, actor.model, input, actor_output, eval_buffers);
+        evaluate(device, actor.model, input, actor_output, eval_buffers, rng);
         auto output_view = view(device, actor_output, matrix::ViewSpec<OUTPUT_SPEC::ROWS, SPEC::DIM>{}, 0, SPEC::OFFSET);
         copy(device, device, output_view, output);
         free(device, actor_output);
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/model.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/model.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/operations_generic.h`

 * *Files 3% similar despite different names*

```diff
@@ -57,42 +57,42 @@
         if constexpr (utils::typing::is_same_v<typename SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
             return m.content.output;
         } else {
             return output(m.next_module);
         }
     }
     // Evaluate is like a forward pass but without saving intermediate activations (so a backward pass is not possible). Hence we can reuse the memory of the intermediate outputs and just require a double buffer where each buffer has to be able to contain the maximum hidden dimension of the module
-    template<typename DEVICE, typename MODULE_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename BUFFER_SPEC, bool TICK = true>
-    void evaluate(DEVICE& device, const nn_models::sequential::Module<MODULE_SPEC>& model, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, nn_models::sequential::ModuleBuffer<BUFFER_SPEC>& buffers){
+    template<bool TICK = true, typename DEVICE, typename MODULE_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename BUFFER_SPEC, typename RNG>
+    void evaluate(DEVICE& device, const nn_models::sequential::Module<MODULE_SPEC>& model, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, nn_models::sequential::ModuleBuffer<BUFFER_SPEC>& buffers, RNG& rng){
         static_assert(nn_models::sequential::buffer_compatible<BUFFER_SPEC, MODULE_SPEC>);
         static_assert(BUFFER_SPEC::BATCH_SIZE == OUTPUT_SPEC::ROWS);
         static_assert(nn_models::sequential::check_input_output<MODULE_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         using DOUBLE_BUFFER_TYPE = decltype(buffers.tick);
 
         if constexpr(utils::typing::is_same_v<typename MODULE_SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
-            evaluate(device, model.content, input, output);
+            evaluate(device, model.content, input, output, rng);
         }
         else{
             DOUBLE_BUFFER_TYPE& output_buffer = TICK ? buffers.tick : buffers.tock;
             auto output_buffer_view = view(device, output_buffer, matrix::ViewSpec<BATCH_SIZE, MODULE_SPEC::CONTENT::OUTPUT_DIM>{});
-            evaluate(device, model.content, input, output_buffer_view);
-            evaluate<DEVICE, typename MODULE_SPEC::NEXT_MODULE::SPEC, typename decltype(output_buffer_view)::SPEC, OUTPUT_SPEC, BUFFER_SPEC, !TICK>(device, model.next_module, output_buffer_view, output, buffers);
+            evaluate(device, model.content, input, output_buffer_view, rng);
+            evaluate<!TICK>(device, model.next_module, output_buffer_view, output, buffers, rng);
         }
     }
-    template <typename DEVICE, typename MODULE_SPEC, typename INPUT>
-    void forward(DEVICE& device, nn_models::sequential::Module<MODULE_SPEC>& module, INPUT& input){
-        forward(device, module.content, input);
+    template <typename DEVICE, typename MODULE_SPEC, typename INPUT, typename RNG>
+    void forward(DEVICE& device, nn_models::sequential::Module<MODULE_SPEC>& module, INPUT& input, RNG& rng){
+        forward(device, module.content, input, rng);
         if constexpr(!utils::typing::is_same_v<typename MODULE_SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
-            forward(device, module.next_module, module.content.output);
+            forward(device, module.next_module, module.content.output, rng);
         }
     }
-    template <typename DEVICE, typename MODULE_SPEC, typename INPUT, typename OUTPUT>
-    void forward(DEVICE& device, nn_models::sequential::Module<MODULE_SPEC>& module, INPUT& input, OUTPUT& output){
-        forward(device, module, input);
+    template <typename DEVICE, typename MODULE_SPEC, typename INPUT, typename OUTPUT, typename RNG>
+    void forward(DEVICE& device, nn_models::sequential::Module<MODULE_SPEC>& module, INPUT& input, OUTPUT& output, RNG& rng){
+        forward(device, module, input, rng);
         copy(device, device, rl_tools::output(module), output);
     }
     template <typename DEVICE, typename MODULE_SPEC>
     void zero_gradient(DEVICE& device, nn_models::sequential::Module<MODULE_SPEC>& module){
         zero_gradient(device, module.content);
         if constexpr(!utils::typing::is_same_v<typename MODULE_SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
             zero_gradient(device, module.next_module);
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist_code.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist_code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/arm.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mux.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mux.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cuda.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_1.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_1.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_1.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_2.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_1.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_2.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_1.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_2.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_1.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_2.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_1.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_1.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_2.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_1.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_2.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/persist/code.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/persist/code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_arm.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_arm.h`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,19 @@
     devices::random::ARM::index_t default_engine(const devices::random::ARM& dev, devices::random::ARM::index_t seed = 1){
 //        return 0b10101010101010101010101010101010 + seed;
         return default_engine(devices::random::Generic<devices::math::ARM>{}, seed);
     };
     constexpr devices::random::ARM::index_t next_max(const devices::random::ARM& dev){
         return devices::random::ARM::MAX_INDEX;
     }
+    template <typename TI, typename RNG>
+    auto split(const devices::random::ARM& dev, TI split_id, RNG& rng){
+        // this operation should not alter the state of rng
+        return split(devices::random::Generic<devices::math::ARM>{}, split_id, rng);
+    }
     template<typename RNG>
     void next(const devices::random::ARM& dev, RNG& rng){
 //        static_assert(utils::typing::is_same_v<RNG, devices::random::ARM::index_t>);
 //        rng ^= (rng << 13);
 //        rng ^= (rng >> 17);
 //        rng ^= (rng << 5);
         next(devices::random::Generic<devices::math::ARM>{}, rng);
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_cpu.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_cpu.h`

 * *Files 22% similar despite different names*

```diff
@@ -4,25 +4,34 @@
 #define RL_TOOLS_UTILS_RANDOM_OPERATIONS_CPU_H
 
 
 #include "../utils/generic/typing.h"
 #include "operations_generic.h"
 
 #include <random>
+#include <limits>
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools::random{
     auto default_engine(const devices::random::CPU& dev, devices::random::CPU::index_t seed = 0){
         return std::default_random_engine(seed+1);
     };
 
     template<typename T, typename RNG>
     T uniform_int_distribution(const devices::random::CPU& dev, T low, T high, RNG& rng){
         return std::uniform_int_distribution<T>(low, high)(rng);
     }
+    template <typename TI, typename RNG>
+    auto split(const devices::random::CPU& dev, TI split_id, RNG& rng){
+        // this operation should not alter the state of rng
+        RNG rng_copy = rng;
+        TI new_seed = random::uniform_int_distribution(dev, std::numeric_limits<TI>::min(), std::numeric_limits<TI>::max(), rng_copy);
+        return std::default_random_engine(new_seed + split_id);
+    }
+
     template<typename T, typename RNG>
     T uniform_real_distribution(const devices::random::CPU& dev, T low, T high, RNG& rng){
         static_assert(utils::typing::is_same_v<T, float> || utils::typing::is_same_v<T, double>);
         return std::uniform_real_distribution<T>(low, high)(rng);
     }
 //    template<typename T, typename RNG>
 //    const std::normal_distribution<T> standard_normal_distribution(0, 1);
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_cuda.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_dummy.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_esp32.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_generic.h`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,21 @@
    template<typename MATH_DEV, typename RNG>
    void next(const devices::random::Generic<MATH_DEV>& dev, RNG& rng){
        static_assert(utils::typing::is_same_v<RNG, typename MATH_DEV::index_t>);
        rng ^= (rng << 13);
        rng ^= (rng >> 17);
        rng ^= (rng << 5);
    }
+    template <typename MATH_DEV, typename TI, typename RNG>
+    auto split(const devices::random::Generic<MATH_DEV>& dev, TI split_id, RNG& rng){
+        // this operation should not alter the state of rng
+        RNG rng_copy = rng;
+        auto next_value = next(dev, rng_copy);
+        return default_engine(dev, next_value + split_id);
+    }
 
    template<typename MATH_DEV, typename T, typename RNG>
    T uniform_int_distribution(const devices::random::Generic<MATH_DEV>& dev, T low, T high, RNG& rng){
        static_assert(utils::typing::is_same_v<RNG, typename MATH_DEV::index_t>);
        using TI = typename MATH_DEV::index_t;
        TI range = static_cast<typename MATH_DEV::index_t>(high - low) + 1;
        next(dev, rng);
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic.h`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
                     advantage_mean /= BATCH_SIZE;
                     advantage_std /= BATCH_SIZE;
                     advantage_std = math::sqrt(device.math, advantage_std - advantage_mean * advantage_mean);
                 }
 //                add_scalar(device, device.logger, "ppo/advantage/mean", advantage_mean);
 //                add_scalar(device, device.logger, "ppo/advantage/std", advantage_std);
 
-                forward(device, ppo.actor, batch_observations, ppo_buffers.current_batch_actions);
+                forward(device, ppo.actor, batch_observations, ppo_buffers.current_batch_actions, rng);
 //                auto abs_diff = abs_diff(device, batch_actions, dataset.actions);
 
                 for(TI batch_step_i = 0; batch_step_i < BATCH_SIZE; batch_step_i++){
                     T action_log_prob = 0;
                     for(TI action_i = 0; action_i < ACTION_DIM; action_i++){
 
                         T current_action = get(ppo_buffers.current_batch_actions, batch_step_i, action_i);
@@ -253,15 +253,15 @@
                     if(batch_policy_kl_divergence < 0.5 * PPO_SPEC::PARAMETERS::ADAPTIVE_LEARNING_RATE_POLICY_KL_THRESHOLD){
                         actor_optimizer.parameters.alpha = math::min(device.math, actor_optimizer.parameters.alpha / PPO_SPEC::PARAMETERS::ADAPTIVE_LEARNING_RATE_DECAY, PPO_SPEC::PARAMETERS::ADAPTIVE_LEARNING_RATE_MAX);
                     }
                 }
                 backward(device, ppo.actor, batch_observations, ppo_buffers.d_action_log_prob_d_action, actor_buffers);
 //                forward_backward_mse(device, ppo.critic, batch_observations, batch_target_values, critic_buffers);
                 {
-                    forward(device, ppo.critic, batch_observations);
+                    forward(device, ppo.critic, batch_observations, rng);
                     nn::loss_functions::mse::gradient(device, output(ppo.critic), batch_target_values, ppo_buffers.d_critic_output, 0.5);
                     backward(device, ppo.critic, batch_observations, ppo_buffers.d_critic_output, critic_buffers);
                 }
                 T critic_loss = nn::loss_functions::mse::evaluate(device, output(ppo.critic), batch_target_values);
                 add_scalar(device, device.logger, "ppo/critic_loss", critic_loss);
                 step(device, actor_optimizer, ppo.actor);
                 step(device, actor_optimizer, ppo.critic); // todo: evaluate switch to critic_optimizer
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic_extensions.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic_extensions.h`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
                 advantage_std /= BATCH_SIZE;
 
                 advantage_std = math::sqrt(device.math, advantage_std - advantage_mean * advantage_mean);
 //                add_scalar(device, device.logger, "ppo/advantage/mean", advantage_mean);
 //                add_scalar(device, device.logger, "ppo/advantage/std", advantage_std);
 
                 copy(device, device_evaluation, batch_observations, hybrid_buffers.observations);
-                forward(device_evaluation, ppo_evaluation.actor, hybrid_buffers.observations, hybrid_buffers.actions);
+                forward(device_evaluation, ppo_evaluation.actor, hybrid_buffers.observations, hybrid_buffers.actions, rng);
                 copy(device_evaluation, device, hybrid_buffers.actions, ppo_buffers.current_batch_actions);
 //                auto abs_diff = abs_diff(device, batch_actions, buffer.actions);
 
                 copy(device_evaluation, device, ppo_evaluation.actor.log_std.parameters, ppo.actor.log_std.parameters);
                 copy(device_evaluation, device, ppo_evaluation.actor.log_std.gradient, ppo.actor.log_std.gradient);
                 for(TI batch_step_i = 0; batch_step_i < BATCH_SIZE; batch_step_i++){
                     T action_log_prob = 0;
@@ -214,15 +214,15 @@
                 copy(device, device_evaluation, ppo.actor.log_std.gradient, ppo_evaluation.actor.log_std.gradient);
 
                 copy(device, device_evaluation, ppo_buffers.d_action_log_prob_d_action, hybrid_buffers.d_action_log_prob_d_action);
                 backward(device_evaluation, ppo_evaluation.actor, hybrid_buffers.observations, hybrid_buffers.d_action_log_prob_d_action, actor_buffers);
                 copy(device, device_evaluation, batch_target_values, hybrid_buffers.target_values);
 //                forward_backward_mse(device_evaluation, ppo_evaluation.critic, hybrid_buffers.observations, hybrid_buffers.target_values, critic_buffers);
                 {
-                    forward(device_evaluation, ppo_evaluation.critic, hybrid_buffers.observations);
+                    forward(device_evaluation, ppo_evaluation.critic, hybrid_buffers.observations, rng);
                     nn::loss_functions::mse::gradient(device_evaluation, output(ppo_evaluation.critic), hybrid_buffers.target_values, hybrid_buffers.d_critic_output);
                     backward(device_evaluation, ppo_evaluation.critic, hybrid_buffers.observations, hybrid_buffers.d_critic_output, critic_buffers);
                 }
                 step(device_evaluation, actor_optimizer, ppo_evaluation.actor);
                 step(device_evaluation, critic_optimizer, ppo_evaluation.critic);
             }
         }
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/ppo.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/ppo.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/config.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/config.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/operations_generic.h`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     template <typename DEVICE, typename T_CONFIG>
     bool step(DEVICE& device, rl::algorithms::ppo::loop::core::State<T_CONFIG>& ts){
         using CONFIG = T_CONFIG;
         set_step(device, device.logger, ts.step);
         bool finished = false;
         collect(device, ts.on_policy_runner_dataset, ts.on_policy_runner, ts.ppo.actor, ts.actor_eval_buffers, ts.observation_normalizer.mean, ts.observation_normalizer.std, ts.rng);
         auto on_policy_runner_dataset_all_observations = CONFIG::PPO_SPEC::PARAMETERS::NORMALIZE_OBSERVATIONS ? ts.on_policy_runner_dataset.all_observations_normalized : ts.on_policy_runner_dataset.all_observations;
-        evaluate(device, ts.ppo.critic, on_policy_runner_dataset_all_observations, ts.on_policy_runner_dataset.all_values, ts.critic_buffers_gae);
+        evaluate(device, ts.ppo.critic, on_policy_runner_dataset_all_observations, ts.on_policy_runner_dataset.all_values, ts.critic_buffers_gae, ts.rng);
         estimate_generalized_advantages(device, ts.on_policy_runner_dataset, typename CONFIG::PPO_TYPE::SPEC::PARAMETERS{});
         train(device, ts.ppo, ts.on_policy_runner_dataset, ts.actor_optimizer, ts.critic_optimizer, ts.ppo_buffers, ts.actor_buffers, ts.critic_buffers, ts.rng);
 
 //        log(device, device.logger, "log_std: ", get(ts.ppo.actor.log_std.parameters, 0, 0));
 
         ts.step++;
         if(ts.step > CONFIG::CORE_PARAMETERS::STEP_LIMIT){
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/state.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/state.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cuda.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_generic.h`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 #define RL_TOOLS_RL_ALGORITHMS_SAC_OPERATIONS_GENERIC_H
 
 #include "sac.h"
 
 #include "../../../rl/components/replay_buffer/replay_buffer.h"
 #include "../../../rl/components/off_policy_runner/off_policy_runner.h"
 #include "../../../nn/nn.h"
-#include "../../../nn_models/operations_generic.h"
 #include "../../../utils/polyak/operations_generic.h"
 #include "../../../math/operations_generic.h"
 #include "../../../utils/generic/memcpy.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template <typename DEVICE, typename SPEC>
@@ -181,54 +180,54 @@
         constexpr TI BATCH_SIZE = rl::algorithms::sac::ActorTrainingBuffers<SPEC>::BATCH_SIZE;
         static_assert(BATCH_SIZE == ACTION_NOISE_SPEC::ROWS);
         static_assert(ACTION_DIM == ACTION_NOISE_SPEC::COLS);
         for(TI sample_i = 0; sample_i < BATCH_SIZE; sample_i++){
             sample_actions_critic_per_sample(device, training_buffers, action_noise, sample_i);
         }
     }
-    template <typename DEVICE, typename SPEC, typename CRITIC_TYPE, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE, typename OPTIMIZER, typename ACTOR_BUFFERS, typename CRITIC_BUFFERS, typename ACTION_NOISE_SPEC>
-    void train_critic(DEVICE& device, const rl::algorithms::sac::ActorCritic<SPEC>& actor_critic, CRITIC_TYPE& critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, OPTIMIZER& optimizer, ACTOR_BUFFERS& actor_buffers, CRITIC_BUFFERS& critic_buffers, rl::algorithms::sac::CriticTrainingBuffers<SPEC>& training_buffers, Matrix<ACTION_NOISE_SPEC>& action_noise){
+    template <typename DEVICE, typename SPEC, typename CRITIC_TYPE, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE, typename OPTIMIZER, typename ACTOR_BUFFERS, typename CRITIC_BUFFERS, typename ACTION_NOISE_SPEC, typename RNG>
+    void train_critic(DEVICE& device, const rl::algorithms::sac::ActorCritic<SPEC>& actor_critic, CRITIC_TYPE& critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, OPTIMIZER& optimizer, ACTOR_BUFFERS& actor_buffers, CRITIC_BUFFERS& critic_buffers, rl::algorithms::sac::CriticTrainingBuffers<SPEC>& training_buffers, Matrix<ACTION_NOISE_SPEC>& action_noise, RNG& rng){
         using T = typename SPEC::T;
         using TI = typename DEVICE::index_t;
         constexpr TI ACTION_DIM = SPEC::ENVIRONMENT::ACTION_DIM;
         static_assert(BATCH_SIZE == SPEC::PARAMETERS::CRITIC_BATCH_SIZE);
         static_assert(BATCH_SIZE == CRITIC_BUFFERS::BATCH_SIZE);
         static_assert(BATCH_SIZE == ACTOR_BUFFERS::BATCH_SIZE);
         static_assert(BATCH_SIZE == ACTION_NOISE_SPEC::ROWS);
         static_assert(ACTION_DIM == ACTION_NOISE_SPEC::COLS);
 
         zero_gradient(device, critic);
 
-        evaluate(device, actor_critic.actor, batch.next_observations, training_buffers.next_actions_distribution, actor_buffers);
+        evaluate(device, actor_critic.actor, batch.next_observations, training_buffers.next_actions_distribution, actor_buffers, rng);
         sample_actions_critic(device, training_buffers, action_noise);
         copy(device, device, batch.next_observations_privileged, training_buffers.next_observations);
-        evaluate(device, actor_critic.critic_target_1, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_1, critic_buffers);
-        evaluate(device, actor_critic.critic_target_2, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_2, critic_buffers);
+        evaluate(device, actor_critic.critic_target_1, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_1, critic_buffers, rng);
+        evaluate(device, actor_critic.critic_target_2, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_2, critic_buffers, rng);
 
         target_actions(device, batch, training_buffers, actor_critic.log_alpha);
-        forward(device, critic, batch.observations_and_actions);
+        forward(device, critic, batch.observations_and_actions, rng);
         nn::loss_functions::mse::gradient(device, output(critic), training_buffers.target_action_value, training_buffers.d_output, 0.5);
         backward(device, critic, batch.observations_and_actions, training_buffers.d_output, critic_buffers);
         step(device, optimizer, critic);
     }
-    template <typename DEVICE, typename SPEC, typename CRITIC_TYPE, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE>
-    typename SPEC::T critic_loss(DEVICE& device, const rl::algorithms::sac::ActorCritic<SPEC>& actor_critic, CRITIC_TYPE& critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, typename SPEC::ACTOR_NETWORK_TYPE::template Buffers<BATCH_SIZE>& actor_buffers, typename CRITIC_TYPE::template Buffers<BATCH_SIZE>& critic_buffers, rl::algorithms::sac::CriticTrainingBuffers<SPEC>& training_buffers) {
+    template <typename DEVICE, typename SPEC, typename CRITIC_TYPE, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE, typename RNG>
+    typename SPEC::T critic_loss(DEVICE& device, const rl::algorithms::sac::ActorCritic<SPEC>& actor_critic, CRITIC_TYPE& critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, typename SPEC::ACTOR_NETWORK_TYPE::template Buffers<BATCH_SIZE>& actor_buffers, typename CRITIC_TYPE::template Buffers<BATCH_SIZE>& critic_buffers, rl::algorithms::sac::CriticTrainingBuffers<SPEC>& training_buffers, RNG& rng) {
         using T = typename SPEC::T;
         using TI = typename DEVICE::index_t;
         static_assert(BATCH_SIZE == SPEC::PARAMETERS::CRITIC_BATCH_SIZE);
 
-        evaluate(device, actor_critic.actor, batch.next_observations, training_buffers.next_actions_distribution, actor_buffers);
+        evaluate(device, actor_critic.actor, batch.next_observations, training_buffers.next_actions_distribution, actor_buffers, rng);
         copy(device, device, batch.next_observations_privileged, training_buffers.next_observations);
-        evaluate(device, actor_critic.critic_target_1, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_1, critic_buffers);
-        evaluate(device, actor_critic.critic_target_2, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_2, critic_buffers);
+        evaluate(device, actor_critic.critic_target_1, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_1, critic_buffers, rng);
+        evaluate(device, actor_critic.critic_target_2, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_2, critic_buffers, rng);
 
         T log_alpha = get(actor_critic.log_alpha, 0, 0);
         T alpha = math::exp(typename DEVICE::SPEC::MATH{}, log_alpha);
         target_actions(device, batch, training_buffers, alpha);
-        evaluate(device, critic, batch.observations_and_actions, training_buffers.action_value, critic_buffers);
+        evaluate(device, critic, batch.observations_and_actions, training_buffers.action_value, critic_buffers, rng);
         return nn::loss_functions::mse::evaluate(device, training_buffers.action_value, training_buffers.target_action_value, 0.5);
     }
     template <typename DEVICE, typename OUTPUT_SPEC, typename SPEC, typename ACTION_NOISE_SPEC, typename TI_SAMPLE>
     RL_TOOLS_FUNCTION_PLACEMENT void sample_actions_actor_per_sample(DEVICE& device, Matrix<OUTPUT_SPEC>& output, rl::algorithms::sac::ActorTrainingBuffers<SPEC>& training_buffers, Matrix<ACTION_NOISE_SPEC>& action_noise, TI_SAMPLE batch_i) {
         using T = typename SPEC::T;
         using TI = typename DEVICE::index_t;
         constexpr TI ACTION_DIM = SPEC::ENVIRONMENT::ACTION_DIM;
@@ -271,57 +270,57 @@
                     = gaussian::prob(mu, std, action_sample) * | (d/d_action_sample tanh(action_sample))^{-1} |
                     = gaussian::prob(mu, std, action_sample) * | (d/d_action_sample tanh(action_sample))|^{-1}
                     = gaussian::prob(mu, std, action_sample) * ((1-tanh(action_sample)^2))^{-1}
         action_log_prob = gaussian::log_prob(mu, std, action_sample) - log(1-tanh(action_sample)^2))
         actor_loss = alpha  * action_log_prob - min(Q_1, Q_2);
         d/d_mu _actor_loss = alpha * d/d_mu action_log_prob - d/d_mu min(Q_1, Q_2)
         d/d_mu action_log_prob = d/d_mu gaussian::log_prob(mu, std, action_sample) + d/d_action_sample gaussian::log_prob(mu, std, action_sample) * d/d_mu action_sample - 1/(1-tanh(action_sample)^2) * (-2*tanh(action_sample))*(1-tanh(action_sample)^2) * d/d_mu action_sample)
-                               = d/d_mu gaussian::log_prob(mu, std, action_sample) + d/d_action_sample gaussian::log_prob(mu, std, action_sample) * d/d_mu action_sample + 2*tanh(action_sample)) * d/d_mu action_sample)
+                               = d/d_mu gaussian::log_prob(mu, std, action_sample) + d/d_action_sample gaussian::log_prob(mu, std, action_sample) * d/d_mu action_sample + 2*tanh(action_sample)) * d/d_mu action_sample
+        d/d_std action_log_prob = d/d_std gaussian::log_prob(mu, std, action_sample) + d/d_action_sample gaussian::log_prob(mu, std, action_sample) * d/d_std action_sample + 2*tanh(action_sample) * d/d_std action_sample
         d/d_mu action_sample = 1
         d/d_std action_sample = noise
         d/d_mu min(Q_1, Q_2) = d/d_action min(Q_1, Q_2) * d/d_mu action
         d/d_mu action = d/d_action_sample tanh(action_sample) * d/d_mu action_sample
 */
         bool critic_1_value = get(critic_1_output, batch_i, 0) < get(critic_2_output, batch_i, 0);
         T entropy = 0;
         for(TI action_i = 0; action_i < ACTION_DIM; action_i++){
-            T action = get(training_buffers.actions, batch_i, action_i);
+            T action = get(training_buffers.actions, batch_i, action_i); // tanh(action_sample)
             T d_mu = 0;
             T d_std = 0;
             {
                 T d_input = 0;
                 if(critic_1_value) {
                     d_input = get(training_buffers.d_critic_1_input, batch_i, SPEC::CRITIC_NETWORK_TYPE::INPUT_DIM - ACTION_DIM + action_i);
                 }
                 else{
                     d_input = get(training_buffers.d_critic_2_input, batch_i, SPEC::CRITIC_NETWORK_TYPE::INPUT_DIM - ACTION_DIM + action_i);
                 }
                 T d_tanh_pre_activation = d_input * (1-action*action);
-                d_mu = d_tanh_pre_activation/BATCH_SIZE;
-                d_std = d_tanh_pre_activation * get(training_buffers.action_noise, batch_i, action_i)/BATCH_SIZE;
+                d_mu = d_tanh_pre_activation;
+                d_std = d_tanh_pre_activation * get(training_buffers.action_noise, batch_i, action_i);
             }
             T log_std_pre_clamp = get(actions, batch_i, action_i + ACTION_DIM);
             T log_std_clamped = math::clamp(device.math, log_std_pre_clamp, (T)SPEC::PARAMETERS::ACTION_LOG_STD_LOWER_BOUND, (T)SPEC::PARAMETERS::ACTION_LOG_STD_UPPER_BOUND);
             T std = math::exp(typename DEVICE::SPEC::MATH{}, log_std_clamped);
 
             T d_log_std_clamped = std * d_std;
-            T d_log_std = log_std_pre_clamp < SPEC::PARAMETERS::ACTION_LOG_STD_LOWER_BOUND || log_std_pre_clamp > SPEC::PARAMETERS::ACTION_LOG_STD_UPPER_BOUND ? 0 : d_log_std_clamped;
 
-            // Entropy bonus
             T mu = get(actions, batch_i, action_i);
             T action_sample = get(training_buffers.action_sample, batch_i, action_i);
             T eps = 1e-6;
-//            T one_over_one_minus_action_square_plus_eps = 1/one_minus_action_square_plus_eps;
             T d_log_prob_d_mean = random::normal_distribution::d_log_prob_d_mean(device.random, mu, log_std_clamped, action_sample);
             T d_log_prob_d_sample = random::normal_distribution::d_log_prob_d_sample(device.random, mu, log_std_clamped, action_sample);
+            // NOTE: The following needs to be divided by BATCH_SIZE (in contrast to the previous d_mu and d_std). d_mu and d_std are already taking into account the mean prior to the backward call of the critic. Thence the d_critic_X_input is already divided by BATCH_SIZE
             d_mu += alpha/BATCH_SIZE * (d_log_prob_d_mean + d_log_prob_d_sample + 2*action);
 
             T noise = get(training_buffers.action_noise, batch_i, action_i);
             T d_log_prob_d_log_std = random::normal_distribution::d_log_prob_d_log_std(device.random, mu, log_std_clamped, action_sample);
-            d_log_std += alpha/BATCH_SIZE * (d_log_prob_d_log_std + d_log_prob_d_sample * noise * std + 2*action * noise * std);
+            d_log_std_clamped += alpha/BATCH_SIZE * (d_log_prob_d_log_std + d_log_prob_d_sample * noise * std + 2*action * noise * std);
+            T d_log_std = log_std_pre_clamp < SPEC::PARAMETERS::ACTION_LOG_STD_LOWER_BOUND || log_std_pre_clamp > SPEC::PARAMETERS::ACTION_LOG_STD_UPPER_BOUND ? 0 : d_log_std_clamped;
 
             set(training_buffers.d_actor_output, batch_i, action_i, d_mu);
             set(training_buffers.d_actor_output, batch_i, action_i + ACTION_DIM, d_log_std);
 
             T one_minus_action_square_plus_eps = (1-action*action + eps);
             T action_log_prob = random::normal_distribution::log_prob(device.random, mu, log_std_clamped, action_sample) - math::log(typename DEVICE::SPEC::MATH{}, one_minus_action_square_plus_eps);
             entropy += -action_log_prob;
@@ -341,56 +340,59 @@
         auto actions_full = output(actor_critic.actor);
         for(TI batch_i = 0; batch_i < BATCH_SIZE; batch_i++){
             d_alpha += d_action_d_action_distribution_per_sample(device, training_buffers, actions_full, output(actor_critic.critic_1), output(actor_critic.critic_2), alpha, batch_i);
         }
         d_alpha /= BATCH_SIZE;
         mean_entropy /= BATCH_SIZE;
 //            T d_log_alpha = 1/alpha * d_alpha; // This and the former optimize the same objective but the latter seems to work better
-        T d_log_alpha = d_alpha;
+        T d_log_alpha = alpha * d_alpha;
         set(actor_critic.log_alpha.gradient, 0, 0, d_log_alpha);
     }
-    template <typename DEVICE, typename SPEC, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE, typename OPTIMIZER, typename ACTOR_BUFFERS, typename CRITIC_BUFFERS, typename ACTION_NOISE_SPEC>
-    void train_actor(DEVICE& device, rl::algorithms::sac::ActorCritic<SPEC>& actor_critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, OPTIMIZER& optimizer, ACTOR_BUFFERS& actor_buffers, CRITIC_BUFFERS& critic_buffers, rl::algorithms::sac::ActorTrainingBuffers<SPEC>& training_buffers, Matrix<ACTION_NOISE_SPEC>& action_noise) {
+    template <typename DEVICE, typename SPEC, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE, typename OPTIMIZER, typename ACTOR_BUFFERS, typename CRITIC_BUFFERS, typename ACTION_NOISE_SPEC, typename RNG>
+    void train_actor(DEVICE& device, rl::algorithms::sac::ActorCritic<SPEC>& actor_critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, OPTIMIZER& optimizer, ACTOR_BUFFERS& actor_buffers, CRITIC_BUFFERS& critic_buffers, rl::algorithms::sac::ActorTrainingBuffers<SPEC>& training_buffers, Matrix<ACTION_NOISE_SPEC>& action_noise, RNG& rng) {
         using T = typename SPEC::T;
         using TI = typename DEVICE::index_t;
         static_assert(BATCH_SIZE == SPEC::PARAMETERS::ACTOR_BATCH_SIZE);
         static_assert(BATCH_SIZE == CRITIC_BUFFERS::BATCH_SIZE);
         static_assert(BATCH_SIZE == ACTOR_BUFFERS::BATCH_SIZE);
         constexpr auto ACTION_DIM = SPEC::ENVIRONMENT::ACTION_DIM;
         static_assert(SPEC::ACTOR_NETWORK_TYPE::OUTPUT_DIM == ACTION_DIM*2);
 
         zero_gradient(device, actor_critic.actor);
         zero_gradient(device, actor_critic.log_alpha);
-        forward(device, actor_critic.actor, batch.observations);
+        forward(device, actor_critic.actor, batch.observations, rng);
         sample_actions_actor(device, actor_critic, training_buffers, action_noise);
         copy(device, device, batch.observations_privileged, training_buffers.observations);
-        forward(device, actor_critic.critic_1, training_buffers.state_action_value_input);
-        forward(device, actor_critic.critic_2, training_buffers.state_action_value_input);
+        forward(device, actor_critic.critic_1, training_buffers.state_action_value_input, rng);
+        forward(device, actor_critic.critic_2, training_buffers.state_action_value_input, rng);
+        // we minimize the negative of the actor loss
+        // todo: evaluate only backpropagating the active values
+        // note: the alpha * entropy term is minimized according to d_action_d_action_distribution
         set_all(device, training_buffers.d_output, (T)-1/BATCH_SIZE);
         backward_input(device, actor_critic.critic_1, training_buffers.d_output, training_buffers.d_critic_1_input, critic_buffers);
         backward_input(device, actor_critic.critic_2, training_buffers.d_output, training_buffers.d_critic_2_input, critic_buffers);
         d_action_d_action_distribution(device, actor_critic, training_buffers);
         backward(device, actor_critic.actor, batch.observations, training_buffers.d_actor_output, actor_buffers);
         step(device, optimizer, actor_critic.actor);
         // adapting alpha
         if constexpr(SPEC::PARAMETERS::ADAPTIVE_ALPHA){
             step(device, actor_critic.alpha_optimizer, actor_critic.log_alpha);
         }
     }
 
-    template <typename DEVICE, typename SPEC, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE>
-    typename SPEC::T actor_value(DEVICE& device, rl::algorithms::sac::ActorCritic<SPEC>& actor_critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, typename SPEC::ACTOR_NETWORK_TYPE::template Buffers<BATCH_SIZE>& actor_buffers, typename SPEC::CRITIC_NETWORK_TYPE::template Buffers<BATCH_SIZE>& critic_buffers, rl::algorithms::sac::ActorTrainingBuffers<SPEC>& training_buffers) {
+    template <typename DEVICE, typename SPEC, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE, typename RNG>
+    typename SPEC::T actor_value(DEVICE& device, rl::algorithms::sac::ActorCritic<SPEC>& actor_critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, typename SPEC::ACTOR_NETWORK_TYPE::template Buffers<BATCH_SIZE>& actor_buffers, typename SPEC::CRITIC_NETWORK_TYPE::template Buffers<BATCH_SIZE>& critic_buffers, rl::algorithms::sac::ActorTrainingBuffers<SPEC>& training_buffers, RNG& rng) {
         using T = typename SPEC::T;
         using TI = typename DEVICE::index_t;
         static_assert(BATCH_SIZE == SPEC::PARAMETERS::ACTOR_BATCH_SIZE);
 
-        evaluate(device, actor_critic.actor, batch.observations, training_buffers.actions, actor_buffers);
+        evaluate(device, actor_critic.actor, batch.observations, training_buffers.actions, actor_buffers, rng);
         copy(device, device, batch.observations, training_buffers.observations);
         auto& critic = actor_critic.critic_1;
-        evaluate(device, critic, training_buffers.state_action_value_input, training_buffers.state_action_value, critic_buffers);
+        evaluate(device, critic, training_buffers.state_action_value_input, training_buffers.state_action_value, critic_buffers, rng);
         return mean(device, training_buffers.state_action_value);
     }
 
     namespace rl::algorithms::sac{
         template<typename DEVICE, typename SOURCE_SPEC, typename TARGET_SPEC>
         void update_target_layer(DEVICE& device, const  nn::layers::dense::Layer<SOURCE_SPEC>& source, nn::layers::dense::Layer<TARGET_SPEC>& target, typename SOURCE_SPEC::T polyak) {
             rl_tools::utils::polyak::update(device, source.weights.parameters, target.weights.parameters, polyak);
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/sac.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/sac.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/config.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/config.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 #include "../../../../../version.h"
 #if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_RL_ALGORITHMS_SAC_LOOP_CORE_CONFIG_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
 #define RL_TOOLS_RL_ALGORITHMS_SAC_LOOP_CORE_CONFIG_H
 
 #include "../../../../../nn_models/sequential/model.h"
 #include "../../../../../nn_models/mlp/network.h"
+#include "../../../../../nn_models/uniform_random/model.h"
 #include "../../../../../rl/algorithms/sac/sac.h"
 #include "../../../../../nn/optimizers/adam/adam.h"
 #include "state.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools::rl::algorithms::sac::loop::core{
     // Config State (Init/Step)
     using namespace nn_models::sequential::interface;
 
     template<typename T, typename TI, typename ENVIRONMENT>
     struct DefaultParameters{
         using SAC_PARAMETERS = rl::algorithms::sac::DefaultParameters<T, TI, ENVIRONMENT::ACTION_DIM>;
         static constexpr TI N_ENVIRONMENTS = 1;
-        static constexpr TI N_WARMUP_STEPS = SAC_PARAMETERS::ACTOR_BATCH_SIZE;
+        static constexpr TI N_WARMUP_STEPS = 100;
+        static_assert(N_WARMUP_STEPS >= SAC_PARAMETERS::ACTOR_BATCH_SIZE);
         static constexpr TI STEP_LIMIT = 10000;
         static constexpr TI REPLAY_BUFFER_CAP = STEP_LIMIT; // Note: when inheriting from this class for overwriting the default STEP_LIMIT you need to set the REPLAY_BUFFER_CAP as well otherwise it will be the default step limit
         static constexpr TI EPISODE_STEP_LIMIT = 200;
 
         static constexpr TI ACTOR_HIDDEN_DIM = 64;
         static constexpr TI ACTOR_NUM_LAYERS = 3;
         static constexpr auto ACTOR_ACTIVATION_FUNCTION = nn::activation_functions::ActivationFunction::RELU;
@@ -107,15 +109,16 @@
         using ENVIRONMENT_EVALUATION = T_ENVIRONMENT;
         using CORE_PARAMETERS = T_PARAMETERS;
         using CONTAINER_TYPE_TAG = T_CONTAINER_TYPE_TAG;
 
         using NN = APPROXIMATOR_CONFIG<T, TI, T_ENVIRONMENT, CORE_PARAMETERS, CONTAINER_TYPE_TAG>;
 //        using NN = ConfigApproximatorsMLP<T, TI, T_ENVIRONMENT, T_PARAMETERS>;
 
-
+        using EXPLORATION_POLICY_SPEC = nn_models::uniform_random::Specification<T, TI, ENVIRONMENT::OBSERVATION_DIM, ENVIRONMENT::ACTION_DIM, nn_models::uniform_random::Range::MINUS_ONE_TO_ONE>;
+        using EXPLORATION_POLICY = nn_models::UniformRandom<EXPLORATION_POLICY_SPEC>;
 
         using ALPHA_PARAMETER_TYPE = nn::parameters::Adam;
         using ALPHA_OPTIMIZER = nn::optimizers::Adam<typename NN::OPTIMIZER_SPEC>;
 
         using ACTOR_CRITIC_SPEC = rl::algorithms::sac::Specification<T, TI, ENVIRONMENT, typename NN::ACTOR_TYPE, typename NN::CRITIC_TYPE, typename NN::CRITIC_TARGET_TYPE, ALPHA_PARAMETER_TYPE, typename NN::OPTIMIZER, typename NN::OPTIMIZER, ALPHA_OPTIMIZER, typename CORE_PARAMETERS::SAC_PARAMETERS, CONTAINER_TYPE_TAG>;
         using ACTOR_CRITIC_TYPE = rl::algorithms::sac::ActorCritic<ACTOR_CRITIC_SPEC>;
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_cpu.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_cpu.h`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,28 @@
         set_step(device, device.logger, ts.step);
         bool finished = false;
         step(device, ts.off_policy_runner, ts.actor_critic.actor, ts.actor_buffers_eval, ts.rng);
         if(ts.step > CONFIG::CORE_PARAMETERS::N_WARMUP_STEPS){
             if(ts.step % CONFIG::CORE_PARAMETERS::SAC_PARAMETERS::CRITIC_TRAINING_INTERVAL == 0){
                 std::thread critic_threads[2];
                 auto train_critic_i = [&](TI critic_i){
-                    gather_batch(device, ts.off_policy_runner, ts.critic_batch[critic_i], ts.rng);
-                    randn(device, ts.action_noise_critic[critic_i], ts.rng);
-                    train_critic(device, ts.actor_critic, critic_i == 0 ? ts.actor_critic.critic_1 : ts.actor_critic.critic_2, ts.critic_batch[critic_i], ts.critic_optimizers[critic_i], ts.actor_buffers[critic_i], ts.critic_buffers[critic_i], ts.critic_training_buffers[critic_i], ts.action_noise_critic[critic_i]);
+                    auto rng = random::split(device.random, critic_i, ts.rng);
+                    gather_batch(device, ts.off_policy_runner, ts.critic_batch[critic_i], rng);
+                    randn(device, ts.action_noise_critic[critic_i], rng);
+                    train_critic(device, ts.actor_critic, critic_i == 0 ? ts.actor_critic.critic_1 : ts.actor_critic.critic_2, ts.critic_batch[critic_i], ts.critic_optimizers[critic_i], ts.actor_buffers[critic_i], ts.critic_buffers[critic_i], ts.critic_training_buffers[critic_i], ts.action_noise_critic[critic_i], rng);
                 };
                 critic_threads[0] = std::thread([&](){ train_critic_i(0); });
                 critic_threads[1] = std::thread([&](){ train_critic_i(1); });
                 critic_threads[0].join();
                 critic_threads[1].join();
             }
             if(ts.step % CONFIG::CORE_PARAMETERS::SAC_PARAMETERS::ACTOR_TRAINING_INTERVAL == 0){
                 gather_batch(device, ts.off_policy_runner, ts.actor_batch, ts.rng);
                 randn(device, ts.action_noise_actor, ts.rng);
-                train_actor(device, ts.actor_critic, ts.actor_batch, ts.actor_optimizer, ts.actor_buffers[0], ts.critic_buffers[0], ts.actor_training_buffers, ts.action_noise_actor);
+                train_actor(device, ts.actor_critic, ts.actor_batch, ts.actor_optimizer, ts.actor_buffers[0], ts.critic_buffers[0], ts.actor_training_buffers, ts.action_noise_actor, ts.rng);
                 update_critic_targets(device, ts.actor_critic);
             }
         }
         ts.step++;
         if(ts.step > CONFIG::CORE_PARAMETERS::STEP_LIMIT){
             return true;
         }
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_generic.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #include "../../../../../version.h"
 #if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_RL_ALGORITHMS_SAC_LOOP_CORE_OPERATIONS_GENERIC_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
 #define RL_TOOLS_RL_ALGORITHMS_SAC_LOOP_CORE_OPERATIONS_GENERIC_H
 
+#include "../../../../../nn_models/operations_generic.h"
+#include "../../../../../nn_models/uniform_random/operations_generic.h"
 #include "../../../../../rl/algorithms/sac/operations_generic.h"
 #include "../../../../../rl/components/off_policy_runner/operations_generic.h"
 #include "../../../../../rl/utils/evaluation.h"
 
 #include "config.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
@@ -114,27 +116,34 @@
     }
 
     template <typename DEVICE, typename T_CONFIG>
     bool step(DEVICE& device, rl::algorithms::sac::loop::core::State<T_CONFIG>& ts){
         using CONFIG = T_CONFIG;
         set_step(device, device.logger, ts.step);
         bool finished = false;
-        step(device, ts.off_policy_runner, ts.actor_critic.actor, ts.actor_buffers_eval, ts.rng);
-        if(ts.step > CONFIG::CORE_PARAMETERS::N_WARMUP_STEPS){
+        if(ts.step >= CONFIG::CORE_PARAMETERS::N_WARMUP_STEPS){
+            step(device, ts.off_policy_runner, get_actor(ts), ts.actor_buffers_eval, ts.rng);
+        }
+        else{
+            typename CONFIG::EXPLORATION_POLICY exploration_policy;
+            typename CONFIG::EXPLORATION_POLICY::template Buffer<> exploration_policy_buffer;
+            step(device, ts.off_policy_runner, exploration_policy, exploration_policy_buffer, ts.rng);
+        }
+        if(ts.step >= CONFIG::CORE_PARAMETERS::N_WARMUP_STEPS){
             if(ts.step % CONFIG::CORE_PARAMETERS::SAC_PARAMETERS::CRITIC_TRAINING_INTERVAL == 0){
                 for(int critic_i = 0; critic_i < 2; critic_i++){
                     gather_batch(device, ts.off_policy_runner, ts.critic_batch[critic_i], ts.rng);
                     randn(device, ts.action_noise_critic[critic_i], ts.rng);
-                    train_critic(device, ts.actor_critic, critic_i == 0 ? ts.actor_critic.critic_1 : ts.actor_critic.critic_2, ts.critic_batch[critic_i], ts.critic_optimizers[critic_i], ts.actor_buffers[critic_i], ts.critic_buffers[critic_i], ts.critic_training_buffers[critic_i], ts.action_noise_critic[critic_i]);
+                    train_critic(device, ts.actor_critic, critic_i == 0 ? ts.actor_critic.critic_1 : ts.actor_critic.critic_2, ts.critic_batch[critic_i], ts.critic_optimizers[critic_i], ts.actor_buffers[critic_i], ts.critic_buffers[critic_i], ts.critic_training_buffers[critic_i], ts.action_noise_critic[critic_i], ts.rng);
                 }
             }
             if(ts.step % CONFIG::CORE_PARAMETERS::SAC_PARAMETERS::ACTOR_TRAINING_INTERVAL == 0){
                 gather_batch(device, ts.off_policy_runner, ts.actor_batch, ts.rng);
                 randn(device, ts.action_noise_actor, ts.rng);
-                train_actor(device, ts.actor_critic, ts.actor_batch, ts.actor_optimizer, ts.actor_buffers[0], ts.critic_buffers[0], ts.actor_training_buffers, ts.action_noise_actor);
+                train_actor(device, ts.actor_critic, ts.actor_batch, ts.actor_optimizer, ts.actor_buffers[0], ts.critic_buffers[0], ts.actor_training_buffers, ts.action_noise_actor, ts.rng);
                 update_critic_targets(device, ts.actor_critic);
             }
         }
         ts.step++;
         if(ts.step > CONFIG::CORE_PARAMETERS::STEP_LIMIT){
             return true;
         }
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/state.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/state.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cuda.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_generic.h`

 * *Files 2% similar despite different names*

```diff
@@ -147,86 +147,86 @@
             T reward = get(batch.rewards, 0, batch_step_i);
             bool terminated = get(batch.terminated, 0, batch_step_i);
             T future_value = SPEC::PARAMETERS::IGNORE_TERMINATION || !terminated ? actor_critic.gamma * min_next_state_action_value : 0;
             T current_target_action_value = reward + future_value;
             set(training_buffers.target_action_value, batch_step_i, 0, current_target_action_value); // todo: improve pitch of target action values etc. (by transformig it into row vectors instead of column vectors)
         }
     }
-    template <typename DEVICE, typename SPEC, typename CRITIC_TYPE, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE, typename OPTIMIZER, typename ACTOR_BUFFERS, typename CRITIC_BUFFERS>
-    void train_critic(DEVICE& device, const rl::algorithms::td3::ActorCritic<SPEC>& actor_critic, CRITIC_TYPE& critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, OPTIMIZER& optimizer, ACTOR_BUFFERS& actor_buffers, CRITIC_BUFFERS& critic_buffers, rl::algorithms::td3::CriticTrainingBuffers<SPEC>& training_buffers) {
+    template <typename DEVICE, typename SPEC, typename CRITIC_TYPE, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE, typename OPTIMIZER, typename ACTOR_BUFFERS, typename CRITIC_BUFFERS, typename RNG>
+    void train_critic(DEVICE& device, const rl::algorithms::td3::ActorCritic<SPEC>& actor_critic, CRITIC_TYPE& critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, OPTIMIZER& optimizer, ACTOR_BUFFERS& actor_buffers, CRITIC_BUFFERS& critic_buffers, rl::algorithms::td3::CriticTrainingBuffers<SPEC>& training_buffers, RNG& rng) {
         // requires training_buffers.target_next_action_noise to be populated
         using T = typename SPEC::T;
         using TI = typename DEVICE::index_t;
         static_assert(BATCH_SIZE == SPEC::PARAMETERS::CRITIC_BATCH_SIZE);
         static_assert(BATCH_SIZE == CRITIC_BUFFERS::BATCH_SIZE);
         static_assert(BATCH_SIZE == ACTOR_BUFFERS::BATCH_SIZE);
         zero_gradient(device, critic);
 
-        evaluate(device, actor_critic.actor_target, batch.next_observations, training_buffers.next_actions, actor_buffers);
+        evaluate(device, actor_critic.actor_target, batch.next_observations, training_buffers.next_actions, actor_buffers, rng);
         noisy_next_actions(device, training_buffers);
         copy(device, device, batch.next_observations_privileged, training_buffers.next_observations);
-        evaluate(device, actor_critic.critic_target_1, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_1, critic_buffers);
-        evaluate(device, actor_critic.critic_target_2, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_2, critic_buffers);
+        evaluate(device, actor_critic.critic_target_1, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_1, critic_buffers, rng);
+        evaluate(device, actor_critic.critic_target_2, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_2, critic_buffers, rng);
 
         target_actions(device, actor_critic, batch, training_buffers);
-        forward(device, critic, batch.observations_and_actions);
+        forward(device, critic, batch.observations_and_actions, rng);
         nn::loss_functions::mse::gradient(device, output(critic), training_buffers.target_action_value, training_buffers.d_output);
         backward(device, critic, batch.observations_and_actions, training_buffers.d_output, critic_buffers);
         step(device, optimizer, critic);
     }
-    template <typename DEVICE, typename SPEC, typename CRITIC_TYPE, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE>
-    typename SPEC::T critic_loss(DEVICE& device, const rl::algorithms::td3::ActorCritic<SPEC>& actor_critic, CRITIC_TYPE& critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, typename SPEC::ACTOR_TYPE::template Buffer<BATCH_SIZE>& actor_buffers, typename CRITIC_TYPE::template Buffer<BATCH_SIZE>& critic_buffers, rl::algorithms::td3::CriticTrainingBuffers<SPEC>& training_buffers) {
+    template <typename DEVICE, typename SPEC, typename CRITIC_TYPE, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE, typename RNG>
+    typename SPEC::T critic_loss(DEVICE& device, const rl::algorithms::td3::ActorCritic<SPEC>& actor_critic, CRITIC_TYPE& critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, typename SPEC::ACTOR_TYPE::template Buffer<BATCH_SIZE>& actor_buffers, typename CRITIC_TYPE::template Buffer<BATCH_SIZE>& critic_buffers, rl::algorithms::td3::CriticTrainingBuffers<SPEC>& training_buffers, RNG& rng) {
         // requires training_buffers.target_next_action_noise to be populated
         using T = typename SPEC::T;
         using TI = typename DEVICE::index_t;
         static_assert(BATCH_SIZE == SPEC::PARAMETERS::CRITIC_BATCH_SIZE);
 
-        evaluate(device, actor_critic.actor_target, batch.next_observations, training_buffers.next_actions, actor_buffers);
+        evaluate(device, actor_critic.actor_target, batch.next_observations, training_buffers.next_actions, actor_buffers, rng);
         noisy_next_actions(device, training_buffers);
         copy(device, device, batch.next_observations_privileged, training_buffers.next_observations);
-        evaluate(device, actor_critic.critic_target_1, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_1, critic_buffers);
-        evaluate(device, actor_critic.critic_target_2, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_2, critic_buffers);
+        evaluate(device, actor_critic.critic_target_1, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_1, critic_buffers, rng);
+        evaluate(device, actor_critic.critic_target_2, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_2, critic_buffers, rng);
 
         target_actions(device, actor_critic, batch, training_buffers);
-        evaluate(device, critic, batch.observations_and_actions, training_buffers.action_value, critic_buffers);
+        evaluate(device, critic, batch.observations_and_actions, training_buffers.action_value, critic_buffers, rng);
         return nn::loss_functions::mse::evaluate(device, training_buffers.action_value, training_buffers.target_action_value);
     }
-    template <typename DEVICE, typename SPEC, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE, typename OPTIMIZER, typename ACTOR_BUFFERS, typename CRITIC_BUFFERS>
-    void train_actor(DEVICE& device, rl::algorithms::td3::ActorCritic<SPEC>& actor_critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, OPTIMIZER& optimizer, ACTOR_BUFFERS& actor_buffers, CRITIC_BUFFERS& critic_buffers, rl::algorithms::td3::ActorTrainingBuffers<SPEC>& training_buffers) {
+    template <typename DEVICE, typename SPEC, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE, typename OPTIMIZER, typename ACTOR_BUFFERS, typename CRITIC_BUFFERS, typename RNG>
+    void train_actor(DEVICE& device, rl::algorithms::td3::ActorCritic<SPEC>& actor_critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, OPTIMIZER& optimizer, ACTOR_BUFFERS& actor_buffers, CRITIC_BUFFERS& critic_buffers, rl::algorithms::td3::ActorTrainingBuffers<SPEC>& training_buffers, RNG& rng) {
         using T = typename SPEC::T;
         using TI = typename DEVICE::index_t;
         static_assert(BATCH_SIZE == SPEC::PARAMETERS::ACTOR_BATCH_SIZE);
         static_assert(BATCH_SIZE == CRITIC_BUFFERS::BATCH_SIZE);
         static_assert(BATCH_SIZE == ACTOR_BUFFERS::BATCH_SIZE);
         constexpr auto ACTION_DIM = SPEC::ENVIRONMENT::ACTION_DIM;
         static_assert(SPEC::ACTOR_TYPE::OUTPUT_DIM == ACTION_DIM);
 
         zero_gradient(device, actor_critic.actor);
-        forward(device, actor_critic.actor, batch.observations, training_buffers.actions);
+        forward(device, actor_critic.actor, batch.observations, training_buffers.actions, rng);
         copy(device, device, batch.observations_privileged, training_buffers.observations);
         auto& critic = actor_critic.critic_1;
-        forward(device, critic, training_buffers.state_action_value_input, training_buffers.state_action_value);
+        forward(device, critic, training_buffers.state_action_value_input, training_buffers.state_action_value, rng);
         set_all(device, training_buffers.d_output, (T)-1/BATCH_SIZE);
         backward_input(device, critic, training_buffers.d_output, training_buffers.d_critic_input, critic_buffers);
         auto d_actor_output = view(device, training_buffers.d_critic_input, matrix::ViewSpec<BATCH_SIZE, ACTION_DIM>{}, 0, SPEC::CRITIC_TYPE::INPUT_DIM - ACTION_DIM);
         backward(device, actor_critic.actor, batch.observations, d_actor_output, actor_buffers);
 
         step(device, optimizer, actor_critic.actor);
     }
 
-    template <typename DEVICE, typename SPEC, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE>
-    typename SPEC::T actor_value(DEVICE& device, rl::algorithms::td3::ActorCritic<SPEC>& actor_critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, typename SPEC::ACTOR_TYPE::template Buffers<BATCH_SIZE>& actor_buffers, typename SPEC::CRITIC_TYPE::template Buffers<BATCH_SIZE>& critic_buffers, rl::algorithms::td3::ActorTrainingBuffers<SPEC>& training_buffers) {
+    template <typename DEVICE, typename SPEC, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE, typename RNG>
+    typename SPEC::T actor_value(DEVICE& device, rl::algorithms::td3::ActorCritic<SPEC>& actor_critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, typename SPEC::ACTOR_TYPE::template Buffers<BATCH_SIZE>& actor_buffers, typename SPEC::CRITIC_TYPE::template Buffers<BATCH_SIZE>& critic_buffers, rl::algorithms::td3::ActorTrainingBuffers<SPEC>& training_buffers, RNG& rng) {
         using T = typename SPEC::T;
         using TI = typename DEVICE::index_t;
         static_assert(BATCH_SIZE == SPEC::PARAMETERS::ACTOR_BATCH_SIZE);
 
-        evaluate(device, actor_critic.actor, batch.observations, training_buffers.actions, actor_buffers);
+        evaluate(device, actor_critic.actor, batch.observations, training_buffers.actions, actor_buffers, rng);
         copy(device, device, batch.observations, training_buffers.observations);
         auto& critic = actor_critic.critic_1;
-        evaluate(device, critic, training_buffers.state_action_value_input, training_buffers.state_action_value, critic_buffers);
+        evaluate(device, critic, training_buffers.state_action_value_input, training_buffers.state_action_value, critic_buffers, rng);
         return mean(device, training_buffers.state_action_value);
     }
 
     namespace rl::algorithms::td3{
         template<typename DEVICE, typename SOURCE_SPEC, typename TARGET_SPEC>
         void update_target_layer(DEVICE& device, const  nn::layers::dense::Layer<SOURCE_SPEC>& source, nn::layers::dense::Layer<TARGET_SPEC>& target, typename SOURCE_SPEC::T polyak) {
             rl_tools::utils::polyak::update(device, source.weights.parameters, target.weights.parameters, polyak);
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/td3.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/td3.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/config.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/config.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/operations_generic.h`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         bool finished = false;
         step(device, ts.off_policy_runner, ts.actor_critic.actor, ts.actor_buffers_eval, ts.rng);
         if(ts.step > CONFIG::CORE_PARAMETERS::N_WARMUP_STEPS){
             if(ts.step % CONFIG::CORE_PARAMETERS::TD3_PARAMETERS::CRITIC_TRAINING_INTERVAL == 0){
                 for(int critic_i = 0; critic_i < 2; critic_i++){
                     gather_batch(device, ts.off_policy_runner, ts.critic_batch, ts.rng);
                     target_action_noise(device, ts.actor_critic, ts.critic_training_buffers.target_next_action_noise, ts.rng);
-                    train_critic(device, ts.actor_critic, critic_i == 0 ? ts.actor_critic.critic_1 : ts.actor_critic.critic_2, ts.critic_batch, ts.actor_critic.critic_optimizers[critic_i], ts.actor_buffers[critic_i], ts.critic_buffers[critic_i], ts.critic_training_buffers);
+                    train_critic(device, ts.actor_critic, critic_i == 0 ? ts.actor_critic.critic_1 : ts.actor_critic.critic_2, ts.critic_batch, ts.actor_critic.critic_optimizers[critic_i], ts.actor_buffers[critic_i], ts.critic_buffers[critic_i], ts.critic_training_buffers, ts.rng);
                 }
             }
             if(ts.step % CONFIG::CORE_PARAMETERS::TD3_PARAMETERS::ACTOR_TRAINING_INTERVAL == 0){
                 gather_batch(device, ts.off_policy_runner, ts.actor_batch, ts.rng);
                 train_actor(device, ts.actor_critic, ts.actor_batch, ts.actor_critic.actor_optimizer, ts.actor_buffers[0], ts.critic_buffers[0], ts.actor_training_buffers);
             }
             if(ts.step % CONFIG::CORE_PARAMETERS::TD3_PARAMETERS::CRITIC_TARGET_UPDATE_INTERVAL == 0){
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/state.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/state.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/off_policy_runner.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/off_policy_runner.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_accelerate.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_accelerate.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_mkl.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cuda.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cuda.h`

 * *Files 2% similar despite different names*

```diff
@@ -81,18 +81,18 @@
             constexpr TI N_BLOCKS_COLS = RL_TOOLS_DEVICES_CUDA_CEIL(SPEC::N_ENVIRONMENTS, BLOCKSIZE_COLS);
             dim3 grid(N_BLOCKS_COLS);
             dim3 block(BLOCKSIZE_COLS);
             devices::cuda::TAG<DEVICE, true> tag_device{};
             prologue_kernel<<<grid, block, 0, device.stream>>>(tag_device, runner, rng);
             check_status(device);
         }
-        template<typename DEV_SPEC, typename SPEC, typename POLICY>
-        void interlude(devices::CUDA<DEV_SPEC>& device, rl::components::OffPolicyRunner<SPEC>& runner, POLICY& policy, typename POLICY::template Buffer<SPEC::N_ENVIRONMENTS>& policy_eval_buffers) {
+        template<typename DEV_SPEC, typename SPEC, typename POLICY, typename RNG>
+        void interlude(devices::CUDA<DEV_SPEC>& device, rl::components::OffPolicyRunner<SPEC>& runner, POLICY& policy, typename POLICY::template Buffer<SPEC::N_ENVIRONMENTS>& policy_eval_buffers, RNG& rng) {
             // runner struct should be on the CPU while its buffers should be on the GPU
-            evaluate(device, policy, runner.buffers.observations, runner.buffers.actions, policy_eval_buffers);
+            evaluate(device, policy, runner.buffers.observations, runner.buffers.actions, policy_eval_buffers, rng);
         }
 
         template<typename DEVICE, typename SPEC, typename RNG>
         __global__
         void epilogue_kernel(DEVICE device, rl::components::OffPolicyRunner<SPEC>* runner, RNG rng) {
             using T = typename SPEC::T;
             using TI = typename SPEC::TI;
@@ -151,15 +151,15 @@
         using T = typename DEVICE_SPEC::T;
         using TI = typename DEVICE_SPEC::TI;
         using ENVIRONMENT = typename DEVICE_SPEC::ENVIRONMENT;
 
         rng = random::next(typename DEVICE::SPEC::RANDOM{}, rng);
         rl::components::off_policy_runner::prologue(device, runner_device, rng);
         rl::components::off_policy_runner::interlude(device, runner_host, policy_host, policy_eval_buffers_host);
-//        evaluate(device, policy_host, runner_host.buffers.observations, runner_host.buffers.actions, policy_eval_buffers_host);
+//        evaluate(device, policy_host, runner_host.buffers.observations, runner_host.buffers.actions, policy_eval_buffers_host, rng);
         rng = random::next(typename DEVICE::SPEC::RANDOM{}, rng);
         rl::components::off_policy_runner::epilogue(device, runner_device, rng);
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 #include "operations_generic.h"
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic.h`

 * *Files 1% similar despite different names*

```diff
@@ -116,42 +116,46 @@
         template<typename DEVICE, typename SPEC, typename RNG>
         void prologue(DEVICE& device, rl::components::OffPolicyRunner<SPEC>& runner, RNG &rng) {
             using TI = typename DEVICE::index_t;
             for (TI env_i = 0; env_i < SPEC::N_ENVIRONMENTS; env_i++) {
                 prologue_per_env(device, runner, rng, env_i);
             }
         }
-        template<typename DEVICE, typename SPEC, typename POLICY, typename POLICY_BUFFERS>
-        void interlude(DEVICE& device, rl::components::OffPolicyRunner<SPEC>& runner, POLICY &policy, POLICY_BUFFERS& policy_eval_buffers){
-            evaluate(device, policy, runner.buffers.observations, runner.buffers.actions, policy_eval_buffers);
+        template<typename DEVICE, typename SPEC, typename POLICY, typename POLICY_BUFFERS, typename RNG>
+        void interlude(DEVICE& device, rl::components::OffPolicyRunner<SPEC>& runner, POLICY &policy, POLICY_BUFFERS& policy_eval_buffers, RNG& rng){
+            using TI = typename DEVICE::index_t;
+            constexpr TI BATCH_SIZE = decltype(runner.buffers.actions)::ROWS;
+            auto action_view = view(device, runner.buffers.actions, matrix::ViewSpec<BATCH_SIZE, POLICY::OUTPUT_DIM>{});
+            evaluate(device, policy, runner.buffers.observations, action_view, policy_eval_buffers, rng);
         }
 
-        template<typename DEVICE, typename SPEC, typename RNG>
-        void epilogue(DEVICE& device, rl::components::OffPolicyRunner<SPEC>& runner, RNG &rng){
+        template<typename DEVICE, typename SPEC, typename POLICY, typename RNG>
+        void epilogue(DEVICE& device, rl::components::OffPolicyRunner<SPEC>& runner, const POLICY& policy, RNG& rng){
             using TI = typename DEVICE::index_t;
             for (TI env_i = 0; env_i < SPEC::N_ENVIRONMENTS; env_i++){
-                epilogue_per_env(device, runner, rng, env_i);
+                epilogue_per_env(device, runner, policy, rng, env_i);
             }
         }
     }
     template<typename DEVICE, typename SPEC, typename POLICY, typename POLICY_BUFFERS, typename RNG>
     void step(DEVICE& device, rl::components::OffPolicyRunner<SPEC>& runner, POLICY& policy, POLICY_BUFFERS& policy_eval_buffers, RNG &rng){
 #ifdef RL_TOOLS_DEBUG_RL_COMPONENTS_OFF_POLICY_RUNNER_CHECK_INIT
         utils::assert_exit(device, runner.initialized, "OffPolicyRunner not initialized");
 #endif
         static_assert(POLICY::INPUT_DIM == SPEC::ENVIRONMENT::OBSERVATION_DIM, "The policy's input dimension must match the environment's observation dimension.");
-        static_assert(POLICY::OUTPUT_DIM == (SPEC::ENVIRONMENT::ACTION_DIM * (SPEC::STOCHASTIC_POLICY ? 2 : 1)), "The policy's output dimension must match the environment's action dimension.");
+//        static_assert(POLICY::OUTPUT_DIM == (SPEC::ENVIRONMENT::ACTION_DIM * (SPEC::STOCHASTIC_POLICY ? 2 : 1)), "The policy's output dimension must match the environment's action dimension.");
+        static_assert(POLICY::OUTPUT_DIM == SPEC::ENVIRONMENT::ACTION_DIM ||  POLICY::OUTPUT_DIM == 2*SPEC::ENVIRONMENT::ACTION_DIM, "The policy's output dimension must match the environment's action dimension.");
         // todo: increase efficiency by removing the double observation of each state
         using T = typename SPEC::T;
         using TI = typename SPEC::TI;
         using ENVIRONMENT = typename SPEC::ENVIRONMENT;
 
         rl::components::off_policy_runner::prologue(device, runner, rng);
-        rl::components::off_policy_runner::interlude(device, runner, policy, policy_eval_buffers);
-        rl::components::off_policy_runner::epilogue(device, runner, rng);
+        rl::components::off_policy_runner::interlude(device, runner, policy, policy_eval_buffers, rng);
+        rl::components::off_policy_runner::epilogue(device, runner, policy, rng);
     }
     template <typename DEVICE, typename SPEC, typename BATCH_SPEC, typename RNG, bool DETERMINISTIC = false>
     void gather_batch(DEVICE& device, const rl::components::ReplayBuffer<SPEC>& replay_buffer, rl::components::off_policy_runner::Batch<BATCH_SPEC>& batch, typename DEVICE::index_t batch_step_i, RNG& rng) {
 #ifdef RL_TOOLS_DEBUG_RL_COMPONENTS_OFF_POLICY_RUNNER_GATHER_BATCH_CHECK_REPLAY_BUFFER_POSITION
         utils::assert_exit(device, replay_buffer.position > 0 || replay_buffer.full, "Replay buffer is empty");
 #endif
         typename DEVICE::index_t sample_index_max = (replay_buffer.full ? SPEC::CAPACITY : replay_buffer.position) - 1;
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic_per_env.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic_per_env.h`

 * *Files 2% similar despite different names*

```diff
@@ -39,20 +39,21 @@
         auto observation            = view<DEVICE, typename decltype(runner.buffers.observations           )::SPEC, 1, ENVIRONMENT::OBSERVATION_DIM           >(device, runner.buffers.observations           , env_i, 0);
         auto observation_privileged = view<DEVICE, typename decltype(runner.buffers.observations_privileged)::SPEC, 1, SPEC::OBSERVATION_DIM_PRIVILEGED>(device, runner.buffers.observations_privileged, env_i, 0);
         observe(device, env, state, observation, rng);
         if constexpr(SPEC::ASYMMETRIC_OBSERVATIONS){
             observe_privileged(device, env, state, observation_privileged, rng);
         }
     }
-    template<typename DEVICE, typename SPEC, typename RNG>
-    RL_TOOLS_FUNCTION_PLACEMENT auto process_and_get_action(DEVICE& device, rl::components::OffPolicyRunner<SPEC>& runner, RNG &rng, typename DEVICE::index_t env_i) {
+    template<typename DEVICE, typename SPEC, typename POLICY, typename RNG>
+    RL_TOOLS_FUNCTION_PLACEMENT auto process_and_get_action(DEVICE& device, rl::components::OffPolicyRunner<SPEC>& runner, const POLICY& policy, RNG &rng, typename DEVICE::index_t env_i) {
         using T = typename SPEC::T;
         using TI = typename SPEC::TI;
         using ENVIRONMENT = typename SPEC::ENVIRONMENT;
-        if constexpr(SPEC::STOCHASTIC_POLICY){
+        static constexpr bool STOCHASTIC_POLICY = POLICY::OUTPUT_DIM == ENVIRONMENT::ACTION_DIM * 2;
+        if constexpr(STOCHASTIC_POLICY){
             for (TI i = 0; i < ENVIRONMENT::ACTION_DIM; i++){
                 T log_std = get(runner.buffers.actions, env_i, ENVIRONMENT::ACTION_DIM+i);
                 T log_std_clip = math::clamp<T>(device.math, log_std, -20, 2); // todo: absorb this into the policy
                 T std = math::exp(typename DEVICE::SPEC::MATH{}, log_std_clip);
                 T mu = get(runner.buffers.actions, env_i, i);
                 T action_noisy = random::normal_distribution::sample(typename DEVICE::SPEC::RANDOM(), mu, std, rng);
                 static_assert(SPEC::ACTION_CLAMPING_TANH);
@@ -66,33 +67,34 @@
             return view(device, runner.buffers.actions, matrix::ViewSpec<1, SPEC::ENVIRONMENT::ACTION_DIM>{}, env_i, 0);
         }
         else{
             for (TI i = 0; i < ENVIRONMENT::ACTION_DIM; i++){
                 T action_noisy = get(runner.buffers.actions, env_i, i) + random::normal_distribution::sample(typename DEVICE::SPEC::RANDOM(), (T) 0, runner.parameters.exploration_noise, rng);
                 set(runner.buffers.actions, env_i, i, math::clamp<T>(device.math, action_noisy, -1, 1));
             }
-            return row(device, runner.buffers.actions, env_i);
+            return view(device, runner.buffers.actions, matrix::ViewSpec<1, SPEC::ENVIRONMENT::ACTION_DIM>{}, env_i, 0);
+//            return row(device, runner.buffers.actions, env_i);
         }
 
     }
-    template<typename DEVICE, typename SPEC, typename RNG>
-    RL_TOOLS_FUNCTION_PLACEMENT void epilogue_per_env(DEVICE& device, rl::components::OffPolicyRunner<SPEC>& runner, RNG &rng, typename DEVICE::index_t env_i) {
+    template<typename DEVICE, typename SPEC, typename POLICY, typename RNG>
+    RL_TOOLS_FUNCTION_PLACEMENT void epilogue_per_env(DEVICE& device, rl::components::OffPolicyRunner<SPEC>& runner, const POLICY& policy, RNG &rng, typename DEVICE::index_t env_i) {
         using T = typename SPEC::T;
         using TI = typename SPEC::TI;
         using ENVIRONMENT = typename SPEC::ENVIRONMENT;
         auto observation                 = view<DEVICE, typename decltype(runner.buffers.observations           )::SPEC, 1, ENVIRONMENT::OBSERVATION_DIM           >(device, runner.buffers.observations           , env_i, 0);
         auto observation_privileged      = view<DEVICE, typename decltype(runner.buffers.observations_privileged)::SPEC, 1, SPEC::OBSERVATION_DIM_PRIVILEGED>(device, runner.buffers.observations_privileged, env_i, 0);
         auto next_observation            = view<DEVICE, typename decltype(runner.buffers.observations           )::SPEC, 1, ENVIRONMENT::OBSERVATION_DIM           >(device, runner.buffers.next_observations           , env_i, 0);
         auto next_observation_privileged = view<DEVICE, typename decltype(runner.buffers.observations_privileged)::SPEC, 1, SPEC::OBSERVATION_DIM_PRIVILEGED>(device, runner.buffers.next_observations_privileged, env_i, 0);
 //        auto action_raw = view<DEVICE, typename decltype(runner.buffers.actions)::SPEC, 1, ENVIRONMENT::ACTION_DIM>(device, runner.buffers.actions, env_i, 0);
         auto& env = runner.envs[env_i];
         auto& state = get(runner.states, 0, env_i);
         typename ENVIRONMENT::State next_state;
 
-        auto action = process_and_get_action(device, runner, rng, env_i);
+        auto action = process_and_get_action(device, runner, policy, rng, env_i);
 
         step(device, env, state, action, next_state, rng);
 
         T reward_value = reward(device, env, state, action, next_state, rng);
 
         observe(device, env, next_state, next_observation, rng);
         if constexpr(SPEC::ASYMMETRIC_OBSERVATIONS) {
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/on_policy_runner.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/on_policy_runner.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_accelerate.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_accelerate.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_mkl.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic.h`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         using TI = typename SPEC::TI;
         for(TI step_i = 0; step_i < DATASET_SPEC::STEPS_PER_ENV; step_i++){
             auto actions_mean            = view(device, dataset.actions_mean           , matrix::ViewSpec<SPEC::N_ENVIRONMENTS, SPEC::ENVIRONMENT::ACTION_DIM>()     , step_i*SPEC::N_ENVIRONMENTS, 0);
             auto actions                 = view(device, dataset.actions                , matrix::ViewSpec<SPEC::N_ENVIRONMENTS, SPEC::ENVIRONMENT::ACTION_DIM>()     , step_i*SPEC::N_ENVIRONMENTS, 0);
             auto observations            = view(device, dataset.observations           , matrix::ViewSpec<SPEC::N_ENVIRONMENTS, SPEC::ENVIRONMENT::OBSERVATION_DIM>(), step_i*SPEC::N_ENVIRONMENTS, 0);
             auto observations_normalized = view(device, dataset.observations_normalized, matrix::ViewSpec<SPEC::N_ENVIRONMENTS, SPEC::ENVIRONMENT::OBSERVATION_DIM>(), step_i*SPEC::N_ENVIRONMENTS, 0);
             rl::components::on_policy_runner::prologue(device, observations, observations_normalized, runner, observation_mean, observation_std, rng, step_i);
-            evaluate(device, actor, observations_normalized, actions_mean, policy_eval_buffers);
+            evaluate(device, actor, observations_normalized, actions_mean, policy_eval_buffers, rng);
             rl::components::on_policy_runner::epilogue(device, dataset, runner, actions_mean, actions, actor.log_std.parameters, rng, step_i);
         }
         // final observation
         for(TI env_i = 0; env_i < SPEC::N_ENVIRONMENTS; env_i++){
             auto& env = get(runner.environments, 0, env_i);
             auto& state = get(runner.states, 0, env_i);
             TI row_i = DATASET_SPEC::STEPS_PER_ENV * SPEC::N_ENVIRONMENTS + env_i;
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_extensions.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_extensions.h`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 //                auto start = std::chrono::high_resolution_clock::now();
                 copy(device, device_evaluation, observations_normalized, evaluation_buffer_evaluation.observations);
 //                auto end = std::chrono::high_resolution_clock::now();
 //                copy_observations_time += std::chrono::duration_cast<std::chrono::microseconds>(end - start).count();
             }
             {
 //                auto start = std::chrono::high_resolution_clock::now();
-                evaluate(device_evaluation, actor_evaluation, evaluation_buffer_evaluation.observations, evaluation_buffer_evaluation.actions, policy_eval_buffers);
+                evaluate(device_evaluation, actor_evaluation, evaluation_buffer_evaluation.observations, evaluation_buffer_evaluation.actions, policy_eval_buffers, rng);
                 cudaDeviceSynchronize();
 //                auto end = std::chrono::high_resolution_clock::now();
 //                evaluate_time += std::chrono::duration_cast<std::chrono::microseconds>(end - start).count();
             }
             {
 
 //                auto start = std::chrono::high_resolution_clock::now();
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_per_env.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_per_env.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/persist.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/persist.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/replay_buffer.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/replay_buffer.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/persist.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/running_normalizer.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/running_normalizer.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/acrobot.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/acrobot.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/ui.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/ui.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/car.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/car.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_cpu.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_json.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_json.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/track.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/track.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/ui.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/ui.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ant.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ant.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/model.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/model.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/operations_cpu.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ui.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ui.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/pendulum.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/pendulum.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui_xeus.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui_xeus.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/config.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/config.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/state.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/state.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/operations_cpu.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/state.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/state.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/utils/evaluation.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/utils/evaluation.h`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         malloc(device, observation);
         malloc(device, observation_normalized);
         malloc(device, action_full);
         observe(device, env, state, observation, rng);
         normalize(device, observation_mean, observation_std, observation, observation_normalized);
 
         auto action = view(device, action_full, matrix::ViewSpec<1, ENVIRONMENT::ACTION_DIM>{});
-        evaluate(device, policy, observation_normalized, action_full, policy_eval_buffers);
+        evaluate(device, policy, observation_normalized, action_full, policy_eval_buffers, rng);
 
         if constexpr(STOCHASTIC_POLICY){ // todo: This is a special case for SAC, will be uneccessary once (https://github.com/rl-tools/rl-tools/blob/72a59eabf4038502c3be86a4f772bd72526bdcc8/TODO.md?plain=1#L22) is implemented
             for(TI action_i=0; action_i<ENVIRONMENT::ACTION_DIM; action_i++){
                     set(action, 0, action_i, math::tanh<T>(device.math, get(action, 0, action_i)));
             }
         }
         typename ENVIRONMENT::State next_state;
```

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation_analysis.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation_analysis.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/server.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/server.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_boost.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_boost.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_cpu.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/persist.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_arm.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cpu.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cuda.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_dummy.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_esp32.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/integrators.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/integrators.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/typing.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/typing.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/vector_operations.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/vector_operations.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_cuda.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_generic.h` & `tinyrl-0.4.1/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/interface/algorithms/ppo/template.h` & `tinyrl-0.4.1/tinyrl/interface/algorithms/ppo/template.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/interface/algorithms/sac/template.h` & `tinyrl-0.4.1/tinyrl/interface/algorithms/sac/template.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/interface/algorithms/td3/template.h` & `tinyrl-0.4.1/tinyrl/interface/algorithms/td3/template.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/interface/inference/inference.cpp` & `tinyrl-0.4.1/tinyrl/interface/inference/inference.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,16 @@
     rlt::MatrixStatic<rlt::matrix::Specification<T, TI, 1, MODEL_TYPE::INPUT_DIM>> input_rlt;
     rlt::malloc(device, input_rlt);
     for(TI input_i=0; input_i<num_elements; input_i++){
         rlt::set(input_rlt, 0, input_i, input_data_ptr[input_i]);
     }
     rlt::MatrixStatic<rlt::matrix::Specification<T, TI, 1, MODEL_TYPE::OUTPUT_DIM>> output_rlt;
     rlt::malloc(device, output_rlt);
-    rlt::evaluate(device, policy::model, input_rlt, output_rlt, buffer);
+    bool rng = false;
+    rlt::evaluate(device, policy::model, input_rlt, output_rlt, buffer, rng);
 
     std::vector<T> output(MODEL_TYPE::OUTPUT_DIM);
 
     for (TI output_i = 0; output_i < MODEL_TYPE::OUTPUT_DIM; output_i++) {
         output[output_i] = rlt::get(output_rlt, 0, output_i);
     }
```

### Comparing `tinyrl-0.4.0/tinyrl/interface/python_environment/operations_cpu.h` & `tinyrl-0.4.1/tinyrl/interface/python_environment/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/interface/python_environment/python_environment.h` & `tinyrl-0.4.1/tinyrl/interface/python_environment/python_environment.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/interface/training/training.cpp` & `tinyrl-0.4.1/tinyrl/interface/training/training.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,16 @@
             rlt::malloc(device, observation_rlt);
             for(TI observation_i=0; observation_i<num_elements; observation_i++){
                 rlt::set(observation_rlt, 0, observation_i, observation_data_ptr[observation_i]);
             }
             using ACTOR_TYPE = rlt::utils::typing::remove_reference<decltype(rlt::get_actor(*this))>::type;
             rlt::MatrixStatic<rlt::matrix::Specification<T, TI, 1, ACTOR_TYPE::OUTPUT_DIM>> action_distribution; //2x for mean and std
             rlt::malloc(device, action_distribution);
-            rlt::evaluate(device, rlt::get_actor(*this), observation_rlt, action_distribution, this->actor_deterministic_evaluation_buffers);
+            bool rng = false;
+            rlt::evaluate(device, rlt::get_actor(*this), observation_rlt, action_distribution, this->actor_deterministic_evaluation_buffers, rng);
             rlt::free(device, observation_rlt);
 
             auto action_rlt = rlt::view(device, action_distribution, rlt::matrix::ViewSpec<1, ENVIRONMENT::ACTION_DIM>{});
 
             std::vector<T> action(ENVIRONMENT::ACTION_DIM);
 
             for (TI action_i = 0; action_i < ENVIRONMENT::ACTION_DIM; action_i++){
```

### Comparing `tinyrl-0.4.0/tinyrl/src/accelerate.py` & `tinyrl-0.4.1/tinyrl/src/accelerate.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/src/compile.py` & `tinyrl-0.4.1/tinyrl/src/compile.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 
 def compile_option(type, option):
     if option is None:
         return ""
     if sys.platform in ["linux", "darwin"]:
         if type == "header_search_path":
-            return f"-I{option}"
+            return f"\"-I{option}\""
         elif type == "macro_definition":
-            return f"-D{option}"
+            return f"\"-D{option}\""
         else:
             raise Exception(f"Unknown option type {type}")
     elif sys.platform.startswith("win"):
         if type == "header_search_path":
-            return f"/I{option}"
+            return f"\"/I{option}\""
         elif type == "macro_definition":
-            return f"/D{option}"
+            return f"\"/D{option}\""
         else:
             raise Exception(f"Unknown option type {type}")
     else:
         raise Exception(f"Unknown platform {sys.platform}")
 
 
 absolute_path = os.path.dirname(os.path.abspath(__file__))
@@ -33,16 +33,21 @@
 def find_compiler():
     if "TINYRL_COMPILER" in os.environ:
         return [os.environ["TINYRL_COMPILER"]]
     unix_compilers = ["clang++", "g++"]
     windows_compilers = ["cl"]
     compilers = unix_compilers if (sys.platform in ["linux", "darwin"]) else windows_compilers
     compilers = [compiler for compiler in compilers if shutil.which(compiler) is not None]
-    raw_platform_compiler = platform.python_compiler().startswith("GCC")
-    platform_compiler = "g++" if raw_platform_compiler else None
+    raw_platform_compiler = platform.python_compiler()
+    if raw_platform_compiler.startswith("MSC"):
+        platform_compiler = "cl"
+    elif raw_platform_compiler.startswith("GCC"):
+        platform_compiler = "g++"
+    else:
+        platform_compiler = None
     if platform_compiler is None:
         warnings.warn(f"The platform compiler {raw_platform_compiler} is not recognized.")
     else:
         if platform_compiler not in compilers:
             warnings.warn(f"The platform compiler {platform_compiler} (used for compiling Python) is not found (found: {compilers}).")
         else:
             compilers = [platform_compiler]
@@ -72,22 +77,28 @@
     python_include_path = sysconfig.get_paths()['include']
     if sys.platform.startswith('win'):
         os.listdir(python_include_path) # check if the path is accessible on Windows (if not, you might need to uninstall the Windows Store version of python and install the installer version from the Python website)
     python_includes = [compile_option("header_search_path", python_include_path)]
     rl_tools_includes = [compile_option("header_search_path", str(os.path.join(absolute_path, "..", "external", "rl_tools", "include")))]
 
     if sys.platform in ["linux", "darwin"]:
-        link_python_args = ["-L"+sysconfig.get_config_var('LIBDIR'), "-lpython" + sysconfig.get_config_var('VERSION')]
+        extension = "so"
+        if platform.python_implementation() != "PyPy":
+            link_python_args = ["-L"+sysconfig.get_config_var('LIBDIR'), "-lpython" + sysconfig.get_config_var('VERSION')]
+        else:
+            link_python_args = ["-L"+sysconfig.get_config_var('LIBDIR'), f"-lpypy{sysconfig.get_config_var('VERSION')}-c"]
+            extension = f"pypy{sys.version_info.major}{sys.version_info.minor}-pp{sys.pypy_version_info.major}{sys.pypy_version_info.minor}-{sys.platform}.so"
     elif sys.platform.startswith('win'):
-        link_python_args = [f"/link /LIBPATH:"+os.path.join(sys.base_exec_prefix, "libs")]
+        extension = "pyd"
+        link_python_args = [f"/link \"/LIBPATH:"+os.path.join(sys.base_exec_prefix, "libs")+"\""]
     
     output_dir = f"{CACHE_PATH}/build/{module}"
     os.makedirs(output_dir, exist_ok=True)
     cmd_path = os.path.join(output_dir, f"cmd.txt")
-    output_path = os.path.join(output_dir, f"module.so" if not sys.platform.startswith('win') else f"module.pyd")
+    output_path = os.path.join(output_dir, f"module.{extension}")
 
     compilers = find_compiler()
 
     cmds = [
         [
             compiler,
             shared_flag, 
@@ -97,20 +108,20 @@
             arch_flag,
             fast_math_flag,
             verbose_flag,
             lto_flag,
             *pybind_includes,
             *python_includes,
             *rl_tools_includes,
-            source,
+            f"\"{source}\"",
             *flags,
             link_math_flag,
             link_stdlib_flag,
             *link_python_args,
-            *(["-o", output_path] if not sys.platform.startswith('win') else [f"/OUT:{output_path}"]),
+            *(["-o", output_path] if not sys.platform.startswith('win') else [f"\"/OUT:{output_path}\""]),
         ]
         for compiler in compilers
     ]
     command_strings = [" ".join(cmd) for cmd in cmds]
     old_command_string = None
     if os.path.exists(cmd_path):
         with open(cmd_path, "r") as f:
```

### Comparing `tinyrl-0.4.0/tinyrl/src/link_blas.py` & `tinyrl-0.4.1/tinyrl/src/link_blas.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/src/link_mkl.py` & `tinyrl-0.4.1/tinyrl/src/link_mkl.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/src/load_checkpoint.py` & `tinyrl-0.4.1/tinyrl/src/load_checkpoint.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/src/ppo.py` & `tinyrl-0.4.1/tinyrl/src/ppo.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/src/render.py` & `tinyrl-0.4.1/tinyrl/src/render.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/src/sac.py` & `tinyrl-0.4.1/tinyrl/src/sac.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/src/td3.py` & `tinyrl-0.4.1/tinyrl/src/td3.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/tinyrl/src/training.py` & `tinyrl-0.4.1/tinyrl/src/training.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/LICENSE` & `tinyrl-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/README.md` & `tinyrl-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.0/pyproject.toml` & `tinyrl-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tinyrl"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="Jonas Eschmann", email="jonas.eschmann@gmail.com" },
 ]
 description = "A Python wrapper for RLtools"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tinyrl-0.4.0/PKG-INFO` & `tinyrl-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tinyrl
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python wrapper for RLtools
 Project-URL: Homepage, https://github.com/rl-tools/tinyrl
 Project-URL: Issues, https://github.com/rl-tools/tinyrl/issues
 Author-email: Jonas Eschmann <jonas.eschmann@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

