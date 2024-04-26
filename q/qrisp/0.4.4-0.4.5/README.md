# Comparing `tmp/qrisp-0.4.4.tar.gz` & `tmp/qrisp-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrisp-0.4.4.tar", last modified: Fri Feb 16 13:02:56 2024, max compression
+gzip compressed data, was "qrisp-0.4.5.tar", last modified: Fri Apr 26 14:31:41 2024, max compression
```

## Comparing `qrisp-0.4.4.tar` & `qrisp-0.4.5.tar`

### file list

```diff
@@ -1,276 +1,276 @@
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:56.303351 qrisp-0.4.4/
--rw-rw-rw-   0        0        0    14474 2024-01-25 09:27:23.000000 qrisp-0.4.4/LICENSE
--rw-rw-rw-   0        0        0     3480 2024-02-16 13:02:56.300817 qrisp-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     2586 2024-01-25 09:27:23.000000 qrisp-0.4.4/README.md
--rw-rw-rw-   0        0        0      206 2024-01-25 09:27:25.000000 qrisp-0.4.4/pyproject.toml
--rw-rw-rw-   0        0        0      605 2024-02-16 13:02:56.306975 qrisp-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1981 2024-01-25 09:27:25.000000 qrisp-0.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.096768 qrisp-0.4.4/src/
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.158571 qrisp-0.4.4/src/qrisp/
--rw-rw-rw-   0        0        0     1161 2024-01-25 09:30:07.000000 qrisp-0.4.4/src/qrisp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.210160 qrisp-0.4.4/src/qrisp/arithmetic/
--rw-rw-rw-   0        0        0    36443 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/SBP_arithmetic.py
--rw-rw-rw-   0        0        0     1121 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.230796 qrisp-0.4.4/src/qrisp/arithmetic/adders/
--rw-rw-rw-   0        0        0     1189 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/__init__.py
--rw-rw-rw-   0        0        0     8304 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/adder_tools.py
--rw-rw-rw-   0        0        0     4110 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/cuccaro.py
--rw-rw-rw-   0        0        0     3721 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/fourier_adder.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.249254 qrisp-0.4.4/src/qrisp/arithmetic/adders/gidney/
--rw-rw-rw-   0        0        0      895 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/gidney/__init__.py
--rw-rw-rw-   0        0        0     8185 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/gidney/cq_gidney_adder.py
--rw-rw-rw-   0        0        0     2327 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/gidney/gidney_adder.py
--rw-rw-rw-   0        0        0     2999 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/gidney/qq_gidney_adder.py
--rw-rw-rw-   0        0        0     6797 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/incrementation.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.255776 qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/
--rw-rw-rw-   0        0        0     1024 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.271607 qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/classical_quantum/
--rw-rw-rw-   0        0        0     1062 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/classical_quantum/__init__.py
--rw-rw-rw-   0        0        0    13995 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/classical_quantum/cq_carry_path.py
--rw-rw-rw-   0        0        0     4144 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/classical_quantum/cq_qcla_adder.py
--rw-rw-rw-   0        0        0     4099 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/classical_quantum/cq_sum_path.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.288194 qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/quantum_quantum/
--rw-rw-rw-   0        0        0     1054 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/quantum_quantum/__init__.py
--rw-rw-rw-   0        0        0    12139 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/quantum_quantum/qq_carry_path.py
--rw-rw-rw-   0        0        0     3847 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/quantum_quantum/qq_qcla_adder.py
--rw-rw-rw-   0        0        0     7110 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/quantum_quantum/qq_sum_path.py
--rw-rw-rw-   0        0        0     6671 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/wrapper_function.py
--rw-rw-rw-   0        0        0    11595 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/adders/ripple_carry_adder.py
--rw-rw-rw-   0        0        0     7378 2024-02-16 08:42:23.000000 qrisp-0.4.4/src/qrisp/arithmetic/comparisons.py
--rw-rw-rw-   0        0        0    26875 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/matrix_multiplication.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.310360 qrisp-0.4.4/src/qrisp/arithmetic/modular_arithmetic/
--rw-rw-rw-   0        0        0     1119 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/modular_arithmetic/__init__.py
--rw-rw-rw-   0        0        0     1367 2024-02-08 11:34:33.000000 qrisp-0.4.4/src/qrisp/arithmetic/modular_arithmetic/mod_tools.py
--rw-rw-rw-   0        0        0    13918 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/arithmetic/modular_arithmetic/modular_multiplication.py
--rw-rw-rw-   0        0        0     2905 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/modular_arithmetic/modular_qft_addition.py
--rw-rw-rw-   0        0        0     7208 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/modular_arithmetic/modular_qft_multiplication.py
--rw-rw-rw-   0        0        0     3717 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/poly_tools.py
--rw-rw-rw-   0        0        0    22973 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/qcla_adder.py
--rw-rw-rw-   0        0        0    16837 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/ripple_division.py
--rw-rw-rw-   0        0        0     1549 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/arithmetic/ripple_mult.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.365714 qrisp-0.4.4/src/qrisp/circuit/
--rw-rw-rw-   0        0        0     1227 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/circuit/__init__.py
--rw-rw-rw-   0        0        0     1649 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/circuit/clbit.py
--rw-rw-rw-   0        0        0     1370 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/circuit/compilation_acceleration.py
--rw-rw-rw-   0        0        0     7663 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/circuit/controlled_operations.py
--rw-rw-rw-   0        0        0     4229 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/circuit/instruction.py
--rw-rw-rw-   0        0        0      928 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/circuit/library.py
--rw-rw-rw-   0        0        0    31232 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/circuit/operation.py
--rw-rw-rw-   0        0        0    78358 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/circuit/quantum_circuit.py
--rw-rw-rw-   0        0        0     2092 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/circuit/qubit.py
--rw-rw-rw-   0        0        0     7259 2024-02-04 17:41:26.000000 qrisp-0.4.4/src/qrisp/circuit/standard_operations.py
--rw-rw-rw-   0        0        0     5925 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/circuit/transpiler.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.408288 qrisp-0.4.4/src/qrisp/core/
--rw-rw-rw-   0        0        0     1194 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/core/__init__.py
--rw-rw-rw-   0        0        0    39127 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/core/compilation.py
--rw-rw-rw-   0        0        0    74112 2024-02-16 09:02:01.000000 qrisp-0.4.4/src/qrisp/core/library.py
--rw-rw-rw-   0        0        0    32782 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/core/quantum_array.py
--rw-rw-rw-   0        0        0     9524 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/core/quantum_dictionary.py
--rw-rw-rw-   0        0        0    51031 2024-02-16 08:33:03.000000 qrisp-0.4.4/src/qrisp/core/quantum_session.py
--rw-rw-rw-   0        0        0    50580 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/core/quantum_variable.py
--rw-rw-rw-   0        0        0    14462 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/core/session_merging_tools.py
--rw-rw-rw-   0        0        0     1457 2024-02-12 16:08:45.000000 qrisp-0.4.4/src/qrisp/default_backend.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.456102 qrisp-0.4.4/src/qrisp/environments/
--rw-rw-rw-   0        0        0     7248 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/environments/GMS_environment.py
--rw-rw-rw-   0        0        0     1335 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/environments/__init__.py
--rw-rw-rw-   0        0        0    11909 2024-02-08 12:05:33.000000 qrisp-0.4.4/src/qrisp/environments/conjugation_environment.py
--rw-rw-rw-   0        0        0    17239 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/environments/control_environment.py
--rw-rw-rw-   0        0        0     9319 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/environments/custom_control_environment.py
--rw-rw-rw-   0        0        0     6692 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/environments/gate_wrap_environment.py
--rw-rw-rw-   0        0        0    10116 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/environments/iteration_environment.py
--rw-rw-rw-   0        0        0    27368 2024-02-16 08:43:35.000000 qrisp-0.4.4/src/qrisp/environments/quantum_conditionals.py
--rw-rw-rw-   0        0        0    17500 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/environments/quantum_environments.py
--rw-rw-rw-   0        0        0    20583 2024-02-04 12:33:13.000000 qrisp-0.4.4/src/qrisp/environments/quantum_inversion.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.466574 qrisp-0.4.4/src/qrisp/grover/
--rw-rw-rw-   0        0        0      877 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/grover/__init__.py
--rw-rw-rw-   0        0        0    14126 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/grover/grover_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.484733 qrisp-0.4.4/src/qrisp/interface/
--rw-rw-rw-   0        0        0     1149 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/interface/__init__.py
--rw-rw-rw-   0        0        0     9759 2024-02-16 09:19:10.000000 qrisp-0.4.4/src/qrisp/interface/backends.py
--rw-rw-rw-   0        0        0    18524 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/circuit_converter.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.503285 qrisp-0.4.4/src/qrisp/interface/converter/
--rw-rw-rw-   0        0        0     1092 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/converter/__init__.py
--rw-rw-rw-   0        0        0     7497 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/converter/convert_to_pytket.py
--rw-rw-rw-   0        0        0     6751 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/interface/converter/convert_to_qml.py
--rw-rw-rw-   0        0        0     2513 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/converter/convert_to_qulacs.py
--rw-rw-rw-   0        0        0     1516 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/interface/docker_backends.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.523073 qrisp-0.4.4/src/qrisp/interface/openapi_interface/
--rw-rw-rw-   0        0        0     1281 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/openapi_interface/__init__.py
--rw-rw-rw-   0        0        0     1951 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/openapi_interface/backend_client.py
--rw-rw-rw-   0        0        0     4290 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/openapi_interface/backend_server.py
--rw-rw-rw-   0        0        0     1596 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/openapi_interface/interface_types.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.537529 qrisp-0.4.4/src/qrisp/interface/qunicorn/
--rw-rw-rw-   0        0        0      970 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/qunicorn/__init__.py
--rw-rw-rw-   0        0        0     5064 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/qunicorn/backend_client.py
--rw-rw-rw-   0        0        0    10827 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/qunicorn/backend_server.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.560323 qrisp-0.4.4/src/qrisp/interface/thrift_interface/
--rw-rw-rw-   0        0        0     1050 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/thrift_interface/__init__.py
--rw-rw-rw-   0        0        0     3752 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/thrift_interface/backend_client.py
--rw-rw-rw-   0        0        0     6310 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/thrift_interface/backend_server.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.583977 qrisp-0.4.4/src/qrisp/interface/thrift_interface/codegen/
--rw-rw-rw-   0        0        0    16898 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/thrift_interface/codegen/BackendService.py
--rw-rw-rw-   0        0        0      887 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/thrift_interface/codegen/__init__.py
--rw-rw-rw-   0        0        0     1247 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/thrift_interface/codegen/constants.py
--rw-rw-rw-   0        0        0    29052 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/thrift_interface/codegen/ttypes.py
--rw-rw-rw-   0        0        0     1480 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/thrift_interface/interface_types.py
--rw-rw-rw-   0        0        0     2057 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/interface/thrift_interface/stoppable_thrift_server.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.594016 qrisp-0.4.4/src/qrisp/iterators/
--rw-rw-rw-   0        0        0      904 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/iterators/__init__.py
--rw-rw-rw-   0        0        0     4056 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/iterators/qrange.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.617176 qrisp-0.4.4/src/qrisp/logic_synthesis/
--rw-rw-rw-   0        0        0     1017 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/logic_synthesis/__init__.py
--rw-rw-rw-   0        0        0    22990 2024-02-08 12:51:17.000000 qrisp-0.4.4/src/qrisp/logic_synthesis/gray_synthesis.py
--rw-rw-rw-   0        0        0     3256 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/logic_synthesis/pprm_synthesis.py
--rw-rw-rw-   0        0        0    15890 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/logic_synthesis/truth_tables.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.671081 qrisp-0.4.4/src/qrisp/mcx_algs/
--rw-rw-rw-   0        0        0     1901 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/mcx_algs/__init__.py
--rw-rw-rw-   0        0        0     1667 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/mcx_algs/amy.py
--rw-rw-rw-   0        0        0    14148 2024-02-16 08:57:13.000000 qrisp-0.4.4/src/qrisp/mcx_algs/balauca.py
--rw-rw-rw-   0        0        0     4516 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/mcx_algs/circuit_library.py
--rw-rw-rw-   0        0        0     2531 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/mcx_algs/gidney.py
--rw-rw-rw-   0        0        0     1874 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/mcx_algs/gms.py
--rw-rw-rw-   0        0        0     2002 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/mcx_algs/gray.py
--rw-rw-rw-   0        0        0     2458 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/mcx_algs/gray_pt.py
--rw-rw-rw-   0        0        0     2766 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/mcx_algs/jones.py
--rw-rw-rw-   0        0        0     2162 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/mcx_algs/maslov.py
--rw-rw-rw-   0        0        0      838 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/mcx_algs/multi_cx.py
--rw-rw-rw-   0        0        0     3138 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/mcx_algs/yong.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.691532 qrisp-0.4.4/src/qrisp/misc/
--rw-rw-rw-   0        0        0    18042 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/misc/GMS_tools.py
--rw-rw-rw-   0        0        0      912 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/misc/__init__.py
--rw-rw-rw-   0        0        0     7877 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/misc/depth_reduction.py
--rw-rw-rw-   0        0        0    73278 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/misc/utility.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.715216 qrisp-0.4.4/src/qrisp/qaoa/
--rw-rw-rw-   0        0        0      987 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qaoa/__init__.py
--rw-rw-rw-   0        0        0     7543 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qaoa/mixers.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.724849 qrisp-0.4.4/src/qrisp/qaoa/optimization_wrappers/
--rw-rw-rw-   0        0        0     1304 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qaoa/optimization_wrappers/__init__.py
--rw-rw-rw-   0        0        0     2292 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qaoa/optimization_wrappers/fourier_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.733960 qrisp-0.4.4/src/qrisp/qaoa/parameters/
--rw-rw-rw-   0        0        0     1304 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qaoa/parameters/__init__.py
--rw-rw-rw-   0        0        0     2383 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qaoa/parameters/fourier_params.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.794720 qrisp-0.4.4/src/qrisp/qaoa/problems/
--rw-rw-rw-   0        0        0     2286 2024-02-13 15:04:49.000000 qrisp-0.4.4/src/qrisp/qaoa/problems/MaxIndep_qiroBM.py
--rw-rw-rw-   0        0        0     6546 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/qaoa/problems/QUBO.py
--rw-rw-rw-   0        0        0     1348 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qaoa/problems/__init__.py
--rw-rw-rw-   0        0        0     1256 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qaoa/problems/create_rdm_graph.py
--rw-rw-rw-   0        0        0     4020 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qaoa/problems/eThrTwoLinInfrastr.py
--rw-rw-rw-   0        0        0     3152 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qaoa/problems/maxCliqueInfrastr.py
--rw-rw-rw-   0        0        0     3599 2024-02-15 16:49:13.000000 qrisp-0.4.4/src/qrisp/qaoa/problems/maxCut.py
--rw-rw-rw-   0        0        0     3270 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qaoa/problems/maxIndepSetInfrastr.py
--rw-rw-rw-   0        0        0    10423 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qaoa/problems/maxKColorableSubgraph.py
--rw-rw-rw-   0        0        0     8208 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qaoa/problems/maxSatInfrastr.py
--rw-rw-rw-   0        0        0     7907 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qaoa/problems/maxSetPackInfrastr.py
--rw-rw-rw-   0        0        0     7313 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qaoa/problems/minSetCoverInfrastr.py
--rw-rw-rw-   0        0        0    22852 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qaoa/qaoa_benchmark_data.py
--rw-rw-rw-   0        0        0    38509 2024-02-13 17:26:49.000000 qrisp-0.4.4/src/qrisp/qaoa/qaoa_problem.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.824787 qrisp-0.4.4/src/qrisp/qtypes/
--rw-rw-rw-   0        0        0     1074 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qtypes/__init__.py
--rw-rw-rw-   0        0        0     6993 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qtypes/quantum_bool.py
--rw-rw-rw-   0        0        0     2611 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qtypes/quantum_char.py
--rw-rw-rw-   0        0        0    32899 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qtypes/quantum_float.py
--rw-rw-rw-   0        0        0     8471 2024-02-08 11:34:33.000000 qrisp-0.4.4/src/qrisp/qtypes/quantum_modulus.py
--rw-rw-rw-   0        0        0     5109 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/qtypes/quantum_string.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.833692 qrisp-0.4.4/src/qrisp/quantum_backtracking/
--rw-rw-rw-   0        0        0      923 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/quantum_backtracking/__init__.py
--rw-rw-rw-   0        0        0    67118 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/quantum_backtracking/backtracking_tree.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.867435 qrisp-0.4.4/src/qrisp/quantum_network/
--rw-rw-rw-   0        0        0     1048 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/quantum_network/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.871283 qrisp-0.4.4/src/qrisp/quantum_network/interface/
--rw-rw-rw-   0        0        0      420 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/quantum_network/interface/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.894580 qrisp-0.4.4/src/qrisp/quantum_network/interface/codegen/
--rw-rw-rw-   0        0        0    57112 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/quantum_network/interface/codegen/QuantumNetworkService.py
--rw-rw-rw-   0        0        0      894 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/quantum_network/interface/codegen/__init__.py
--rw-rw-rw-   0        0        0     1247 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/quantum_network/interface/codegen/constants.py
--rw-rw-rw-   0        0        0    23701 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/quantum_network/interface/codegen/ttypes.py
--rw-rw-rw-   0        0        0     1760 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/quantum_network/interface_connection_example.py
--rw-rw-rw-   0        0        0    13691 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/quantum_network/qn_client.py
--rw-rw-rw-   0        0        0     5880 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/quantum_network/qn_server.py
--rw-rw-rw-   0        0        0     5638 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/quantum_network/qn_simulator_server.py
--rw-rw-rw-   0        0        0     6839 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/quantum_network/quantum_network_session.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.909380 qrisp-0.4.4/src/qrisp/shor/
--rw-rw-rw-   0        0        0      915 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/shor/__init__.py
--rw-rw-rw-   0        0        0     6452 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/shor/crypto_tools.py
--rw-rw-rw-   0        0        0     5274 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/shor/shors_algorithm.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.964610 qrisp-0.4.4/src/qrisp/simulator/
--rw-rw-rw-   0        0        0     1177 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/simulator/__init__.py
--rw-rw-rw-   0        0        0    17320 2024-02-16 10:56:01.000000 qrisp-0.4.4/src/qrisp/simulator/bi_array_helper.py
--rw-rw-rw-   0        0        0    53993 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/simulator/bi_arrays.py
--rw-rw-rw-   0        0        0    32351 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/simulator/circuit_preprocessing.py
--rw-rw-rw-   0        0        0    14930 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/simulator/circuit_reordering.py
--rw-rw-rw-   0        0        0      926 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/simulator/numerics_config.py
--rw-rw-rw-   0        0        0    12441 2024-02-14 13:22:48.000000 qrisp-0.4.4/src/qrisp/simulator/quantum_state.py
--rw-rw-rw-   0        0        0    14967 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/simulator/simulator.py
--rw-rw-rw-   0        0        0    10702 2024-02-14 13:23:01.000000 qrisp-0.4.4/src/qrisp/simulator/tensor_factor.py
--rw-rw-rw-   0        0        0    12954 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/simulator/unitary_management.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:55.988201 qrisp-0.4.4/src/qrisp/uncomputation/
--rw-rw-rw-   0        0        0      975 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/uncomputation/__init__.py
--rw-rw-rw-   0        0        0     6399 2024-01-25 09:27:25.000000 qrisp-0.4.4/src/qrisp/uncomputation/type_checker.py
--rw-rw-rw-   0        0        0     5073 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/uncomputation/uncomputation.py
--rw-rw-rw-   0        0        0    13395 2024-02-15 16:55:06.000000 qrisp-0.4.4/src/qrisp/uncomputation/unqomp.py
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:56.297600 qrisp-0.4.4/src/qrisp.egg-info/
--rw-rw-rw-   0        0        0     3480 2024-02-16 13:02:54.000000 qrisp-0.4.4/src/qrisp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9137 2024-02-16 13:02:55.000000 qrisp-0.4.4/src/qrisp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-16 13:02:54.000000 qrisp-0.4.4/src/qrisp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2024-02-16 13:02:54.000000 qrisp-0.4.4/src/qrisp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-02-16 13:02:54.000000 qrisp-0.4.4/src/qrisp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-16 13:02:56.291730 qrisp-0.4.4/tests/
--rw-rw-rw-   0        0        0     1539 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_GMS_environment_example.py
--rw-rw-rw-   0        0        0     1917 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_GXX_converter_example.py
--rw-rw-rw-   0        0        0     2803 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_GXX_gates_example.py
--rw-rw-rw-   0        0        0     3567 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_GZZ_gates_example.py
--rw-rw-rw-   0        0        0     2033 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_QAE.py
--rw-rw-rw-   0        0        0     7224 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_QAOAMkCS.py
--rw-rw-rw-   0        0        0     2554 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_QAOAQUBO.py
--rw-rw-rw-   0        0        0     3175 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_QAOA_TQA_warm_start.py
--rw-rw-rw-   0        0        0     3532 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_QAOAeTwoThrLin.py
--rw-rw-rw-   0        0        0     4793 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_QAOAmaxClique.py
--rw-rw-rw-   0        0        0     2690 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_QAOAmaxCut.py
--rw-rw-rw-   0        0        0     4879 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_QAOAmaxIndepSet.py
--rw-rw-rw-   0        0        0     2979 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_QAOAmaxSat.py
--rw-rw-rw-   0        0        0     6483 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_QAOAmaxSetPacking.py
--rw-rw-rw-   0        0        0     5433 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_QAOAminSetCover.py
--rw-rw-rw-   0        0        0     3701 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_QAOAtrain_func.py
--rw-rw-rw-   0        0        0     3950 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_abstr_params_printing.py
--rw-rw-rw-   0        0        0     3017 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_abstract_parameters.py
--rw-rw-rw-   0        0        0     1589 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_amplitude_amplification.py
--rw-rw-rw-   0        0        0     2359 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_amy_mcx.py
--rw-rw-rw-   0        0        0     1327 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_array_entry_manipulation.py
--rw-rw-rw-   0        0        0     5496 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_backtracking.py
--rw-rw-rw-   0        0        0     4501 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_comparisons.py
--rw-rw-rw-   0        0        0     4368 2024-02-13 10:45:16.000000 qrisp-0.4.4/tests/test_conditional_environments_example.py
--rw-rw-rw-   0        0        0     1721 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_conjugation_environment.py
--rw-rw-rw-   0        0        0     3580 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_controlled_gates.py
--rw-rw-rw-   0        0        0     4463 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_converter_QrispToQml.py
--rw-rw-rw-   0        0        0     3203 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_custom_control.py
--rw-rw-rw-   0        0        0     1986 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_cycling_function.py
--rw-rw-rw-   0        0        0     1230 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_depth_calculation.py
--rw-rw-rw-   0        0        0     4781 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_diagonal_hamiltonian_application.py
--rw-rw-rw-   0        0        0      981 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_fourier_adder.py
--rw-rw-rw-   0        0        0     2400 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_gidney_mcx.py
--rw-rw-rw-   0        0        0     2104 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_gray_synthesis_example.py
--rw-rw-rw-   0        0        0     4508 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_grovers_algorithm.py
--rw-rw-rw-   0        0        0     1108 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_hello_world.py
--rw-rw-rw-   0        0        0     2133 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_inpl_matrix_multiplication_example.py
--rw-rw-rw-   0        0        0     3174 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_iteration_environment.py
--rw-rw-rw-   0        0        0     2373 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_jones_mcx.py
--rw-rw-rw-   0        0        0     1417 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_loops.py
--rw-rw-rw-   0        0        0     2543 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_matrix_multiplication_example.py
--rw-rw-rw-   0        0        0     2836 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_mcx.py
--rw-rw-rw-   0        0        0     1092 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_measurement_reduction.py
--rw-rw-rw-   0        0        0     4580 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_modular_arithmetic.py
--rw-rw-rw-   0        0        0     1070 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_outcome_array.py
--rw-rw-rw-   0        0        0    12375 2024-02-04 12:21:53.000000 qrisp-0.4.4/tests/test_qcla.py
--rw-rw-rw-   0        0        0     2354 2024-02-16 09:29:43.000000 qrisp-0.4.4/tests/test_qiskit_backend_client.py
--rw-rw-rw-   0        0        0     1247 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_qompiler.py
--rw-rw-rw-   0        0        0     4476 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_quantum_arithmetic.py
--rw-rw-rw-   0        0        0     3428 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_quantum_dictionary.py
--rw-rw-rw-   0        0        0     1499 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_quantum_division.py
--rw-rw-rw-   0        0        0     2584 2024-02-04 13:35:31.000000 qrisp-0.4.4/tests/test_sc_gidney_adder.py
--rw-rw-rw-   0        0        0     1667 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_state_preparation.py
--rw-rw-rw-   0        0        0     1406 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_string_test.py
--rw-rw-rw-   0        0        0     5245 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_sudoku.py
--rw-rw-rw-   0        0        0     3925 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_tket_converter.py
--rw-rw-rw-   0        0        0     5748 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/test_uncomputation_example.py
--rw-rw-rw-   0        0        0     2070 2024-02-16 09:28:56.000000 qrisp-0.4.4/tests/test_unitary_calculation.py
--rw-rw-rw-   0        0        0     4549 2024-01-25 09:27:25.000000 qrisp-0.4.4/tests/tests_doc_examples.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:41.883036 qrisp-0.4.5/
+-rw-rw-rw-   0        0        0    14474 2024-01-25 09:27:23.000000 qrisp-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0     3480 2024-04-26 14:31:41.881028 qrisp-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2586 2024-01-25 09:27:23.000000 qrisp-0.4.5/README.md
+-rw-rw-rw-   0        0        0      206 2024-01-25 09:27:25.000000 qrisp-0.4.5/pyproject.toml
+-rw-rw-rw-   0        0        0      605 2024-04-26 14:31:41.889755 qrisp-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1983 2024-04-26 14:24:39.000000 qrisp-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:37.226017 qrisp-0.4.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:37.436738 qrisp-0.4.5/src/qrisp/
+-rw-rw-rw-   0        0        0     1161 2024-04-26 13:25:59.000000 qrisp-0.4.5/src/qrisp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:37.680698 qrisp-0.4.5/src/qrisp/arithmetic/
+-rw-rw-rw-   0        0        0    36443 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/SBP_arithmetic.py
+-rw-rw-rw-   0        0        0     1121 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:37.789782 qrisp-0.4.5/src/qrisp/arithmetic/adders/
+-rw-rw-rw-   0        0        0     1189 2024-02-23 11:53:38.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/__init__.py
+-rw-rw-rw-   0        0        0     8304 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/adder_tools.py
+-rw-rw-rw-   0        0        0     4110 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/cuccaro.py
+-rw-rw-rw-   0        0        0     3721 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/fourier_adder.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:37.874469 qrisp-0.4.5/src/qrisp/arithmetic/adders/gidney/
+-rw-rw-rw-   0        0        0      895 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/gidney/__init__.py
+-rw-rw-rw-   0        0        0     8185 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/gidney/cq_gidney_adder.py
+-rw-rw-rw-   0        0        0     2327 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/gidney/gidney_adder.py
+-rw-rw-rw-   0        0        0     2999 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/gidney/qq_gidney_adder.py
+-rw-rw-rw-   0        0        0     6797 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/incrementation.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:37.894678 qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/
+-rw-rw-rw-   0        0        0     1024 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:37.953934 qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/classical_quantum/
+-rw-rw-rw-   0        0        0     1062 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/classical_quantum/__init__.py
+-rw-rw-rw-   0        0        0    13995 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/classical_quantum/cq_carry_path.py
+-rw-rw-rw-   0        0        0     4144 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/classical_quantum/cq_qcla_adder.py
+-rw-rw-rw-   0        0        0     4099 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/classical_quantum/cq_sum_path.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:37.997864 qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/quantum_quantum/
+-rw-rw-rw-   0        0        0     1054 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/quantum_quantum/__init__.py
+-rw-rw-rw-   0        0        0    12139 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/quantum_quantum/qq_carry_path.py
+-rw-rw-rw-   0        0        0     3847 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/quantum_quantum/qq_qcla_adder.py
+-rw-rw-rw-   0        0        0     7110 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/quantum_quantum/qq_sum_path.py
+-rw-rw-rw-   0        0        0     6671 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/wrapper_function.py
+-rw-rw-rw-   0        0        0    11595 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/adders/ripple_carry_adder.py
+-rw-rw-rw-   0        0        0     7378 2024-04-10 11:10:50.000000 qrisp-0.4.5/src/qrisp/arithmetic/comparisons.py
+-rw-rw-rw-   0        0        0    26875 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/matrix_multiplication.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:38.093427 qrisp-0.4.5/src/qrisp/arithmetic/modular_arithmetic/
+-rw-rw-rw-   0        0        0     1119 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/modular_arithmetic/__init__.py
+-rw-rw-rw-   0        0        0     1381 2024-04-19 10:52:04.000000 qrisp-0.4.5/src/qrisp/arithmetic/modular_arithmetic/mod_tools.py
+-rw-rw-rw-   0        0        0    13923 2024-04-17 09:08:53.000000 qrisp-0.4.5/src/qrisp/arithmetic/modular_arithmetic/modular_multiplication.py
+-rw-rw-rw-   0        0        0     2905 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/modular_arithmetic/modular_qft_addition.py
+-rw-rw-rw-   0        0        0     7276 2024-04-26 13:25:59.000000 qrisp-0.4.5/src/qrisp/arithmetic/modular_arithmetic/modular_qft_multiplication.py
+-rw-rw-rw-   0        0        0     3717 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/poly_tools.py
+-rw-rw-rw-   0        0        0    22973 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/qcla_adder.py
+-rw-rw-rw-   0        0        0    16837 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/ripple_division.py
+-rw-rw-rw-   0        0        0     1549 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/arithmetic/ripple_mult.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:38.254587 qrisp-0.4.5/src/qrisp/circuit/
+-rw-rw-rw-   0        0        0     1227 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/circuit/__init__.py
+-rw-rw-rw-   0        0        0     1649 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/circuit/clbit.py
+-rw-rw-rw-   0        0        0     1370 2024-03-22 03:36:48.000000 qrisp-0.4.5/src/qrisp/circuit/compilation_acceleration.py
+-rw-rw-rw-   0        0        0     7663 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/circuit/controlled_operations.py
+-rw-rw-rw-   0        0        0     4229 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/circuit/instruction.py
+-rw-rw-rw-   0        0        0      928 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/circuit/library.py
+-rw-rw-rw-   0        0        0    31232 2024-04-26 13:25:59.000000 qrisp-0.4.5/src/qrisp/circuit/operation.py
+-rw-rw-rw-   0        0        0    78681 2024-04-26 13:38:06.000000 qrisp-0.4.5/src/qrisp/circuit/quantum_circuit.py
+-rw-rw-rw-   0        0        0     2092 2024-04-10 12:52:07.000000 qrisp-0.4.5/src/qrisp/circuit/qubit.py
+-rw-rw-rw-   0        0        0     7259 2024-02-04 17:41:26.000000 qrisp-0.4.5/src/qrisp/circuit/standard_operations.py
+-rw-rw-rw-   0        0        0     5925 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/circuit/transpiler.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:38.435541 qrisp-0.4.5/src/qrisp/core/
+-rw-rw-rw-   0        0        0     1194 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/core/__init__.py
+-rw-rw-rw-   0        0        0    39127 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/core/compilation.py
+-rw-rw-rw-   0        0        0    74112 2024-04-26 13:25:59.000000 qrisp-0.4.5/src/qrisp/core/library.py
+-rw-rw-rw-   0        0        0    32782 2024-04-19 10:59:45.000000 qrisp-0.4.5/src/qrisp/core/quantum_array.py
+-rw-rw-rw-   0        0        0     9524 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/core/quantum_dictionary.py
+-rw-rw-rw-   0        0        0    51031 2024-04-26 13:25:59.000000 qrisp-0.4.5/src/qrisp/core/quantum_session.py
+-rw-rw-rw-   0        0        0    50580 2024-04-26 13:25:59.000000 qrisp-0.4.5/src/qrisp/core/quantum_variable.py
+-rw-rw-rw-   0        0        0    14462 2024-04-26 13:25:59.000000 qrisp-0.4.5/src/qrisp/core/session_merging_tools.py
+-rw-rw-rw-   0        0        0     1457 2024-02-19 09:49:00.000000 qrisp-0.4.5/src/qrisp/default_backend.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:38.527380 qrisp-0.4.5/src/qrisp/environments/
+-rw-rw-rw-   0        0        0     7248 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/environments/GMS_environment.py
+-rw-rw-rw-   0        0        0     1335 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/environments/__init__.py
+-rw-rw-rw-   0        0        0    11909 2024-02-19 09:49:00.000000 qrisp-0.4.5/src/qrisp/environments/conjugation_environment.py
+-rw-rw-rw-   0        0        0    17239 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/environments/control_environment.py
+-rw-rw-rw-   0        0        0     9319 2024-02-19 09:49:00.000000 qrisp-0.4.5/src/qrisp/environments/custom_control_environment.py
+-rw-rw-rw-   0        0        0     6692 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/environments/gate_wrap_environment.py
+-rw-rw-rw-   0        0        0    10116 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/environments/iteration_environment.py
+-rw-rw-rw-   0        0        0    27512 2024-04-19 10:59:45.000000 qrisp-0.4.5/src/qrisp/environments/quantum_conditionals.py
+-rw-rw-rw-   0        0        0    17500 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/environments/quantum_environments.py
+-rw-rw-rw-   0        0        0    20583 2024-02-04 12:33:13.000000 qrisp-0.4.5/src/qrisp/environments/quantum_inversion.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:38.554358 qrisp-0.4.5/src/qrisp/grover/
+-rw-rw-rw-   0        0        0      877 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/grover/__init__.py
+-rw-rw-rw-   0        0        0    14126 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/grover/grover_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:38.611634 qrisp-0.4.5/src/qrisp/interface/
+-rw-rw-rw-   0        0        0     1149 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/interface/__init__.py
+-rw-rw-rw-   0        0        0     9979 2024-04-26 14:23:11.000000 qrisp-0.4.5/src/qrisp/interface/backends.py
+-rw-rw-rw-   0        0        0    18524 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/circuit_converter.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:38.652111 qrisp-0.4.5/src/qrisp/interface/converter/
+-rw-rw-rw-   0        0        0     1092 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/converter/__init__.py
+-rw-rw-rw-   0        0        0     7497 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/converter/convert_to_pytket.py
+-rw-rw-rw-   0        0        0     6751 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/interface/converter/convert_to_qml.py
+-rw-rw-rw-   0        0        0     2513 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/converter/convert_to_qulacs.py
+-rw-rw-rw-   0        0        0     1657 2024-02-19 09:48:34.000000 qrisp-0.4.5/src/qrisp/interface/docker_backends.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:38.695635 qrisp-0.4.5/src/qrisp/interface/openapi_interface/
+-rw-rw-rw-   0        0        0     1281 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/openapi_interface/__init__.py
+-rw-rw-rw-   0        0        0     1951 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/openapi_interface/backend_client.py
+-rw-rw-rw-   0        0        0     4290 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/openapi_interface/backend_server.py
+-rw-rw-rw-   0        0        0     1596 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/openapi_interface/interface_types.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:38.760892 qrisp-0.4.5/src/qrisp/interface/qunicorn/
+-rw-rw-rw-   0        0        0      970 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/qunicorn/__init__.py
+-rw-rw-rw-   0        0        0     5064 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/qunicorn/backend_client.py
+-rw-rw-rw-   0        0        0    10827 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/qunicorn/backend_server.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:38.810595 qrisp-0.4.5/src/qrisp/interface/thrift_interface/
+-rw-rw-rw-   0        0        0     1050 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/thrift_interface/__init__.py
+-rw-rw-rw-   0        0        0     3752 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/thrift_interface/backend_client.py
+-rw-rw-rw-   0        0        0     6310 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/thrift_interface/backend_server.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:38.856518 qrisp-0.4.5/src/qrisp/interface/thrift_interface/codegen/
+-rw-rw-rw-   0        0        0    16898 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/thrift_interface/codegen/BackendService.py
+-rw-rw-rw-   0        0        0      887 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/thrift_interface/codegen/__init__.py
+-rw-rw-rw-   0        0        0     1247 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/thrift_interface/codegen/constants.py
+-rw-rw-rw-   0        0        0    29052 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/thrift_interface/codegen/ttypes.py
+-rw-rw-rw-   0        0        0     1480 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/thrift_interface/interface_types.py
+-rw-rw-rw-   0        0        0     2057 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/interface/thrift_interface/stoppable_thrift_server.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:38.893877 qrisp-0.4.5/src/qrisp/iterators/
+-rw-rw-rw-   0        0        0      904 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/iterators/__init__.py
+-rw-rw-rw-   0        0        0     4056 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/iterators/qrange.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:38.936182 qrisp-0.4.5/src/qrisp/logic_synthesis/
+-rw-rw-rw-   0        0        0     1017 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/logic_synthesis/__init__.py
+-rw-rw-rw-   0        0        0    22990 2024-02-08 12:51:17.000000 qrisp-0.4.5/src/qrisp/logic_synthesis/gray_synthesis.py
+-rw-rw-rw-   0        0        0     3256 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/logic_synthesis/pprm_synthesis.py
+-rw-rw-rw-   0        0        0    15890 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/logic_synthesis/truth_tables.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:39.098410 qrisp-0.4.5/src/qrisp/mcx_algs/
+-rw-rw-rw-   0        0        0     1901 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/mcx_algs/__init__.py
+-rw-rw-rw-   0        0        0     1667 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/mcx_algs/amy.py
+-rw-rw-rw-   0        0        0    14148 2024-02-21 00:04:03.000000 qrisp-0.4.5/src/qrisp/mcx_algs/balauca.py
+-rw-rw-rw-   0        0        0     4516 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/mcx_algs/circuit_library.py
+-rw-rw-rw-   0        0        0     2531 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/mcx_algs/gidney.py
+-rw-rw-rw-   0        0        0     1874 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/mcx_algs/gms.py
+-rw-rw-rw-   0        0        0     2002 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/mcx_algs/gray.py
+-rw-rw-rw-   0        0        0     2458 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/mcx_algs/gray_pt.py
+-rw-rw-rw-   0        0        0     2766 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/mcx_algs/jones.py
+-rw-rw-rw-   0        0        0     2162 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/mcx_algs/maslov.py
+-rw-rw-rw-   0        0        0      838 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/mcx_algs/multi_cx.py
+-rw-rw-rw-   0        0        0     3138 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/mcx_algs/yong.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:39.137313 qrisp-0.4.5/src/qrisp/misc/
+-rw-rw-rw-   0        0        0    18042 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/misc/GMS_tools.py
+-rw-rw-rw-   0        0        0      912 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/misc/__init__.py
+-rw-rw-rw-   0        0        0     7877 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/misc/depth_reduction.py
+-rw-rw-rw-   0        0        0    73278 2024-04-19 10:59:45.000000 qrisp-0.4.5/src/qrisp/misc/utility.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:39.182569 qrisp-0.4.5/src/qrisp/qaoa/
+-rw-rw-rw-   0        0        0      987 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/qaoa/__init__.py
+-rw-rw-rw-   0        0        0     7543 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/qaoa/mixers.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:39.202103 qrisp-0.4.5/src/qrisp/qaoa/optimization_wrappers/
+-rw-rw-rw-   0        0        0     1304 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/qaoa/optimization_wrappers/__init__.py
+-rw-rw-rw-   0        0        0     2292 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/qaoa/optimization_wrappers/fourier_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:39.323831 qrisp-0.4.5/src/qrisp/qaoa/parameters/
+-rw-rw-rw-   0        0        0     1304 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/qaoa/parameters/__init__.py
+-rw-rw-rw-   0        0        0     2383 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/qaoa/parameters/fourier_params.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:40.063695 qrisp-0.4.5/src/qrisp/qaoa/problems/
+-rw-rw-rw-   0        0        0     2352 2024-02-19 09:49:00.000000 qrisp-0.4.5/src/qrisp/qaoa/problems/MaxIndep_qiroBM.py
+-rw-rw-rw-   0        0        0     6546 2024-02-19 09:49:00.000000 qrisp-0.4.5/src/qrisp/qaoa/problems/QUBO.py
+-rw-rw-rw-   0        0        0     1348 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/qaoa/problems/__init__.py
+-rw-rw-rw-   0        0        0     1256 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/qaoa/problems/create_rdm_graph.py
+-rw-rw-rw-   0        0        0     4020 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/qaoa/problems/eThrTwoLinInfrastr.py
+-rw-rw-rw-   0        0        0     3152 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/qaoa/problems/maxCliqueInfrastr.py
+-rw-rw-rw-   0        0        0     3599 2024-04-19 10:59:45.000000 qrisp-0.4.5/src/qrisp/qaoa/problems/maxCut.py
+-rw-rw-rw-   0        0        0     3270 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/qaoa/problems/maxIndepSetInfrastr.py
+-rw-rw-rw-   0        0        0    10423 2024-02-20 18:44:10.000000 qrisp-0.4.5/src/qrisp/qaoa/problems/maxKColorableSubgraph.py
+-rw-rw-rw-   0        0        0     8208 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/qaoa/problems/maxSatInfrastr.py
+-rw-rw-rw-   0        0        0     7907 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/qaoa/problems/maxSetPackInfrastr.py
+-rw-rw-rw-   0        0        0     7313 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/qaoa/problems/minSetCoverInfrastr.py
+-rw-rw-rw-   0        0        0    22852 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/qaoa/qaoa_benchmark_data.py
+-rw-rw-rw-   0        0        0    38509 2024-04-19 10:59:45.000000 qrisp-0.4.5/src/qrisp/qaoa/qaoa_problem.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:40.367289 qrisp-0.4.5/src/qrisp/qtypes/
+-rw-rw-rw-   0        0        0     1074 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/qtypes/__init__.py
+-rw-rw-rw-   0        0        0     6993 2024-04-10 11:10:50.000000 qrisp-0.4.5/src/qrisp/qtypes/quantum_bool.py
+-rw-rw-rw-   0        0        0     2611 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/qtypes/quantum_char.py
+-rw-rw-rw-   0        0        0    32899 2024-04-19 10:59:45.000000 qrisp-0.4.5/src/qrisp/qtypes/quantum_float.py
+-rw-rw-rw-   0        0        0    12190 2024-04-26 13:25:59.000000 qrisp-0.4.5/src/qrisp/qtypes/quantum_modulus.py
+-rw-rw-rw-   0        0        0     5109 2024-04-19 10:59:45.000000 qrisp-0.4.5/src/qrisp/qtypes/quantum_string.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:40.443529 qrisp-0.4.5/src/qrisp/quantum_backtracking/
+-rw-rw-rw-   0        0        0      923 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/quantum_backtracking/__init__.py
+-rw-rw-rw-   0        0        0    67118 2024-02-19 09:49:00.000000 qrisp-0.4.5/src/qrisp/quantum_backtracking/backtracking_tree.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:40.609394 qrisp-0.4.5/src/qrisp/quantum_network/
+-rw-rw-rw-   0        0        0     1048 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/quantum_network/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:40.635375 qrisp-0.4.5/src/qrisp/quantum_network/interface/
+-rw-rw-rw-   0        0        0      420 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/quantum_network/interface/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:40.758063 qrisp-0.4.5/src/qrisp/quantum_network/interface/codegen/
+-rw-rw-rw-   0        0        0    57112 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/quantum_network/interface/codegen/QuantumNetworkService.py
+-rw-rw-rw-   0        0        0      894 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/quantum_network/interface/codegen/__init__.py
+-rw-rw-rw-   0        0        0     1247 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/quantum_network/interface/codegen/constants.py
+-rw-rw-rw-   0        0        0    23701 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/quantum_network/interface/codegen/ttypes.py
+-rw-rw-rw-   0        0        0     1760 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/quantum_network/interface_connection_example.py
+-rw-rw-rw-   0        0        0    13691 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/quantum_network/qn_client.py
+-rw-rw-rw-   0        0        0     5880 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/quantum_network/qn_server.py
+-rw-rw-rw-   0        0        0     5638 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/quantum_network/qn_simulator_server.py
+-rw-rw-rw-   0        0        0     6839 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/quantum_network/quantum_network_session.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:40.853588 qrisp-0.4.5/src/qrisp/shor/
+-rw-rw-rw-   0        0        0      915 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/shor/__init__.py
+-rw-rw-rw-   0        0        0     6452 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/shor/crypto_tools.py
+-rw-rw-rw-   0        0        0     5274 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/shor/shors_algorithm.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:41.030261 qrisp-0.4.5/src/qrisp/simulator/
+-rw-rw-rw-   0        0        0     1177 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/simulator/__init__.py
+-rw-rw-rw-   0        0        0    17320 2024-04-19 10:59:45.000000 qrisp-0.4.5/src/qrisp/simulator/bi_array_helper.py
+-rw-rw-rw-   0        0        0    53993 2024-04-19 10:59:45.000000 qrisp-0.4.5/src/qrisp/simulator/bi_arrays.py
+-rw-rw-rw-   0        0        0    32351 2024-04-19 10:59:45.000000 qrisp-0.4.5/src/qrisp/simulator/circuit_preprocessing.py
+-rw-rw-rw-   0        0        0    14930 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/simulator/circuit_reordering.py
+-rw-rw-rw-   0        0        0      926 2024-04-19 10:59:45.000000 qrisp-0.4.5/src/qrisp/simulator/numerics_config.py
+-rw-rw-rw-   0        0        0    12441 2024-04-19 10:59:45.000000 qrisp-0.4.5/src/qrisp/simulator/quantum_state.py
+-rw-rw-rw-   0        0        0    14967 2024-04-19 10:59:45.000000 qrisp-0.4.5/src/qrisp/simulator/simulator.py
+-rw-rw-rw-   0        0        0    10702 2024-04-19 10:59:45.000000 qrisp-0.4.5/src/qrisp/simulator/tensor_factor.py
+-rw-rw-rw-   0        0        0    12954 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/simulator/unitary_management.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:41.099805 qrisp-0.4.5/src/qrisp/uncomputation/
+-rw-rw-rw-   0        0        0      975 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/uncomputation/__init__.py
+-rw-rw-rw-   0        0        0     6399 2024-01-25 09:27:25.000000 qrisp-0.4.5/src/qrisp/uncomputation/type_checker.py
+-rw-rw-rw-   0        0        0     5073 2024-02-15 16:55:06.000000 qrisp-0.4.5/src/qrisp/uncomputation/uncomputation.py
+-rw-rw-rw-   0        0        0    13395 2024-04-17 08:49:22.000000 qrisp-0.4.5/src/qrisp/uncomputation/unqomp.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:41.874034 qrisp-0.4.5/src/qrisp.egg-info/
+-rw-rw-rw-   0        0        0     3480 2024-04-26 14:31:36.000000 qrisp-0.4.5/src/qrisp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9137 2024-04-26 14:31:37.000000 qrisp-0.4.5/src/qrisp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 14:31:36.000000 qrisp-0.4.5/src/qrisp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2024-04-26 14:31:36.000000 qrisp-0.4.5/src/qrisp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-26 14:31:36.000000 qrisp-0.4.5/src/qrisp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 14:31:41.859032 qrisp-0.4.5/tests/
+-rw-rw-rw-   0        0        0     1539 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_GMS_environment_example.py
+-rw-rw-rw-   0        0        0     1917 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_GXX_converter_example.py
+-rw-rw-rw-   0        0        0     2803 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_GXX_gates_example.py
+-rw-rw-rw-   0        0        0     3567 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_GZZ_gates_example.py
+-rw-rw-rw-   0        0        0     2033 2024-04-19 10:59:45.000000 qrisp-0.4.5/tests/test_QAE.py
+-rw-rw-rw-   0        0        0     7224 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_QAOAMkCS.py
+-rw-rw-rw-   0        0        0     2554 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_QAOAQUBO.py
+-rw-rw-rw-   0        0        0     3175 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_QAOA_TQA_warm_start.py
+-rw-rw-rw-   0        0        0     3532 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_QAOAeTwoThrLin.py
+-rw-rw-rw-   0        0        0     4793 2024-04-19 10:59:45.000000 qrisp-0.4.5/tests/test_QAOAmaxClique.py
+-rw-rw-rw-   0        0        0     2690 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_QAOAmaxCut.py
+-rw-rw-rw-   0        0        0     4879 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_QAOAmaxIndepSet.py
+-rw-rw-rw-   0        0        0     2979 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_QAOAmaxSat.py
+-rw-rw-rw-   0        0        0     6483 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_QAOAmaxSetPacking.py
+-rw-rw-rw-   0        0        0     5433 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_QAOAminSetCover.py
+-rw-rw-rw-   0        0        0     3701 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_QAOAtrain_func.py
+-rw-rw-rw-   0        0        0     3950 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_abstr_params_printing.py
+-rw-rw-rw-   0        0        0     3017 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_abstract_parameters.py
+-rw-rw-rw-   0        0        0     1589 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_amplitude_amplification.py
+-rw-rw-rw-   0        0        0     2359 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_amy_mcx.py
+-rw-rw-rw-   0        0        0     1327 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_array_entry_manipulation.py
+-rw-rw-rw-   0        0        0     5496 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_backtracking.py
+-rw-rw-rw-   0        0        0     5467 2024-04-26 13:25:59.000000 qrisp-0.4.5/tests/test_comparisons.py
+-rw-rw-rw-   0        0        0     4368 2024-02-13 10:45:16.000000 qrisp-0.4.5/tests/test_conditional_environments_example.py
+-rw-rw-rw-   0        0        0     1721 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_conjugation_environment.py
+-rw-rw-rw-   0        0        0     3580 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_controlled_gates.py
+-rw-rw-rw-   0        0        0     4463 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_converter_QrispToQml.py
+-rw-rw-rw-   0        0        0     3203 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_custom_control.py
+-rw-rw-rw-   0        0        0     1986 2024-04-19 10:59:45.000000 qrisp-0.4.5/tests/test_cycling_function.py
+-rw-rw-rw-   0        0        0     1230 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_depth_calculation.py
+-rw-rw-rw-   0        0        0     4781 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_diagonal_hamiltonian_application.py
+-rw-rw-rw-   0        0        0      981 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_fourier_adder.py
+-rw-rw-rw-   0        0        0     2400 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_gidney_mcx.py
+-rw-rw-rw-   0        0        0     2104 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_gray_synthesis_example.py
+-rw-rw-rw-   0        0        0     4508 2024-04-19 10:59:45.000000 qrisp-0.4.5/tests/test_grovers_algorithm.py
+-rw-rw-rw-   0        0        0     1108 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_hello_world.py
+-rw-rw-rw-   0        0        0     2133 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_inpl_matrix_multiplication_example.py
+-rw-rw-rw-   0        0        0     3174 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_iteration_environment.py
+-rw-rw-rw-   0        0        0     2373 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_jones_mcx.py
+-rw-rw-rw-   0        0        0     1417 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_loops.py
+-rw-rw-rw-   0        0        0     2543 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_matrix_multiplication_example.py
+-rw-rw-rw-   0        0        0     2836 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_mcx.py
+-rw-rw-rw-   0        0        0     1092 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_measurement_reduction.py
+-rw-rw-rw-   0        0        0     4580 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_modular_arithmetic.py
+-rw-rw-rw-   0        0        0     1070 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_outcome_array.py
+-rw-rw-rw-   0        0        0    12375 2024-02-04 12:21:53.000000 qrisp-0.4.5/tests/test_qcla.py
+-rw-rw-rw-   0        0        0     2457 2024-04-26 13:26:30.000000 qrisp-0.4.5/tests/test_qiskit_backend_client.py
+-rw-rw-rw-   0        0        0     1247 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_qompiler.py
+-rw-rw-rw-   0        0        0     4476 2024-02-20 09:26:04.000000 qrisp-0.4.5/tests/test_quantum_arithmetic.py
+-rw-rw-rw-   0        0        0     3428 2024-02-19 21:18:01.000000 qrisp-0.4.5/tests/test_quantum_dictionary.py
+-rw-rw-rw-   0        0        0     1499 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_quantum_division.py
+-rw-rw-rw-   0        0        0     2584 2024-02-04 13:35:31.000000 qrisp-0.4.5/tests/test_sc_gidney_adder.py
+-rw-rw-rw-   0        0        0     1667 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_state_preparation.py
+-rw-rw-rw-   0        0        0     1406 2024-04-19 10:59:45.000000 qrisp-0.4.5/tests/test_string_test.py
+-rw-rw-rw-   0        0        0     5245 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_sudoku.py
+-rw-rw-rw-   0        0        0     3925 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/test_tket_converter.py
+-rw-rw-rw-   0        0        0     5748 2024-04-19 10:59:45.000000 qrisp-0.4.5/tests/test_uncomputation_example.py
+-rw-rw-rw-   0        0        0     2070 2024-02-19 09:49:00.000000 qrisp-0.4.5/tests/test_unitary_calculation.py
+-rw-rw-rw-   0        0        0     4549 2024-01-25 09:27:25.000000 qrisp-0.4.5/tests/tests_doc_examples.py
```

### Comparing `qrisp-0.4.4/LICENSE` & `qrisp-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/PKG-INFO` & `qrisp-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: qrisp
-Version: 0.4.4
+Version: 0.4.5
 Summary: Qrisp - A high level language for gate-based quantum computing
 Home-page: https://github.com/fraunhoferfokus/Qrisp
 Author: Raphael Seidel
 Author-email: raphael.seidel@fokus.fraunhofer.de
 Project-URL: Bug Tracker, https://github.com/fraunhoferfokus/Qrisp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: connexion>=2.12.0
-Requires-Dist: qiskit>=0.34.2
+Requires-Dist: qiskit>=0.44.0
 Requires-Dist: thrift>=0.15.0
 Requires-Dist: matplotlib>=3.5.1
 Requires-Dist: waitress>=2.1.1
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: numba
 Requires-Dist: networkx
 Requires-Dist: tdqm
```

### Comparing `qrisp-0.4.4/README.md` & `qrisp-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/setup.cfg` & `qrisp-0.4.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2071 7269 7370 0d0a 7665 7273 696f   = qrisp..versio
-00000020: 6e20 3d20 302e 342e 340d 0a61 7574 686f  n = 0.4.4..autho
+00000020: 6e20 3d20 302e 342e 350d 0a61 7574 686f  n = 0.4.5..autho
 00000030: 7220 3d20 5261 7068 6165 6c20 5365 6964  r = Raphael Seid
 00000040: 656c 0d0a 6175 7468 6f72 5f65 6d61 696c  el..author_email
 00000050: 203d 2072 6170 6861 656c 2e73 6569 6465   = raphael.seide
 00000060: 6c40 666f 6b75 732e 6672 6175 6e68 6f66  l@fokus.fraunhof
 00000070: 6572 2e64 650d 0a64 6573 6372 6970 7469  er.de..descripti
 00000080: 6f6e 203d 2041 2068 6967 682d 6c65 7665  on = A high-leve
 00000090: 6c20 7175 616e 7475 6d20 7072 6f67 7261  l quantum progra
```

### Comparing `qrisp-0.4.4/setup.py` & `qrisp-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 * SPDX-License-Identifier: EPL-2.0 OR GPL-2.0 WITH Classpath-exception-2.0
 ********************************************************************************/
 """
 
 import setuptools
 
 REQUIREMENTS = ["connexion>=2.12.0",
-                "qiskit>=0.34.2",
+                "qiskit>=0.44.0",
                 "thrift>=0.15.0",
                 "matplotlib>=3.5.1",
                 "waitress>=2.1.1",
                 "scipy>=1.10.0",
                 "numba",
                 "networkx",
                 "tdqm",
@@ -47,8 +47,8 @@
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     install_requires = REQUIREMENTS,
     setup_requires = REQUIREMENTS,
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.8",
-)
+)
```

### Comparing `qrisp-0.4.4/src/qrisp/__init__.py` & `qrisp-0.4.5/src/qrisp/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/SBP_arithmetic.py` & `qrisp-0.4.5/src/qrisp/arithmetic/SBP_arithmetic.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/__init__.py` & `qrisp-0.4.5/src/qrisp/arithmetic/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/__init__.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/adder_tools.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/adder_tools.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/cuccaro.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/cuccaro.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/fourier_adder.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/fourier_adder.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/gidney/__init__.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/gidney/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/gidney/cq_gidney_adder.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/gidney/cq_gidney_adder.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/gidney/gidney_adder.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/gidney/gidney_adder.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/gidney/qq_gidney_adder.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/gidney/qq_gidney_adder.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/incrementation.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/incrementation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/__init__.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/classical_quantum/__init__.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/classical_quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/classical_quantum/cq_carry_path.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/classical_quantum/cq_carry_path.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/classical_quantum/cq_qcla_adder.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/classical_quantum/cq_qcla_adder.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/classical_quantum/cq_sum_path.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/classical_quantum/cq_sum_path.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/quantum_quantum/__init__.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/quantum_quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/quantum_quantum/qq_carry_path.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/quantum_quantum/qq_carry_path.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/quantum_quantum/qq_qcla_adder.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/quantum_quantum/qq_qcla_adder.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/quantum_quantum/qq_sum_path.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/quantum_quantum/qq_sum_path.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/qcla/wrapper_function.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/qcla/wrapper_function.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/adders/ripple_carry_adder.py` & `qrisp-0.4.5/src/qrisp/arithmetic/adders/ripple_carry_adder.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/comparisons.py` & `qrisp-0.4.5/src/qrisp/arithmetic/comparisons.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/matrix_multiplication.py` & `qrisp-0.4.5/src/qrisp/arithmetic/matrix_multiplication.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/modular_arithmetic/__init__.py` & `qrisp-0.4.5/src/qrisp/arithmetic/modular_arithmetic/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/modular_arithmetic/mod_tools.py` & `qrisp-0.4.5/src/qrisp/arithmetic/modular_arithmetic/mod_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     if 0 < R < 1:
         R = modinv(R**-1, N)
     return (y*modinv(R, N))%N
 
 def montgomery_encoder(y, R, N):
     if 0 < R < 1:
         R = modinv(R**-1, N)
-    return (y*R)%N
+    return (int(y)%N*int(R)%N)%N
     
 
 def egcd(a, b):
     if a == 0:
         return (b, 0, 1)
     else:
         g, y, x = egcd(b % a, a)
```

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/modular_arithmetic/modular_multiplication.py` & `qrisp-0.4.5/src/qrisp/arithmetic/modular_arithmetic/modular_multiplication.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 def find_best_montgomery_shift(b, N):
     # The idea is now to try out increasingly large m, compute the corresponding
     # Montgomery form of the (classical) multiplication value b and check, if it
     # satisfies the above condition
     
     m = 0
     while True:
-        b_trial = montgomery_encoder(b, 2**m, N)%N
+        b_trial = montgomery_encoder(int(b), 1<<m, N)%N
         # Since a is reduced, in the worst case, it is equal to N-1
         if (N-1)*b_trial < N*2**m:
             return m
         m += 1
 
 
 # This function performs semi classical out of place multiplication follow by a
```

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/modular_arithmetic/modular_qft_addition.py` & `qrisp-0.4.5/src/qrisp/arithmetic/modular_arithmetic/modular_qft_addition.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/modular_arithmetic/modular_qft_multiplication.py` & `qrisp-0.4.5/src/qrisp/arithmetic/modular_arithmetic/modular_qft_multiplication.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,15 @@
     for i in range(a.size):
         multi_controlled_U_g(t, [a[i]], (2**i*b))
     
     from qrisp import QuantumModulus
     t.__class__ = QuantumModulus
     t.modulus = a.modulus
     t.m = a.m + m
+    t.inpl_adder = a.inpl_adder
     
     
     
     return montgomery_red(t, a, b, N, m, permeable_if_zero = permeable_if_zero)
 
 
 def montgomery_red(t, a, b, N, m, permeable_if_zero = False):
@@ -152,15 +153,15 @@
     u.delete(verify = False)
     
     return t
 
 from qrisp import merge
 def montgomery_mod_mul(a, b, output_qg = None):
     
-    m = int(np.ceil(np.log2((a.modulus-1)**2))) - a.size
+    m = int(np.ceil(np.log2((a.modulus-1)**2)+1)) - a.size
     
     if a.modulus != b.modulus:
         raise Exception("Tried to multiply two QuantumModulus with differing modulus")
         
     if output_qg is None:
         t = QuantumFloat(a.size + m, signed = True)
         h(t)
@@ -180,14 +181,15 @@
     
     t = hybrid_mult(a, b, init_op = None, terminal_op = None, output_qf = t)
     
     from qrisp import QuantumModulus
     t.__class__ = QuantumModulus
     t.modulus = a.modulus
     t.m = (a.m + b.m)
+    t.inpl_adder = a.inpl_adder
     
     t = montgomery_red(t, a, b, a.modulus, m)
     
     return t
 
 from qrisp import invert
 from qrisp.environments import custom_control
```

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/poly_tools.py` & `qrisp-0.4.5/src/qrisp/arithmetic/poly_tools.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/qcla_adder.py` & `qrisp-0.4.5/src/qrisp/arithmetic/qcla_adder.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/ripple_division.py` & `qrisp-0.4.5/src/qrisp/arithmetic/ripple_division.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/arithmetic/ripple_mult.py` & `qrisp-0.4.5/src/qrisp/arithmetic/ripple_mult.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/circuit/__init__.py` & `qrisp-0.4.5/src/qrisp/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/circuit/clbit.py` & `qrisp-0.4.5/src/qrisp/circuit/clbit.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/circuit/compilation_acceleration.py` & `qrisp-0.4.5/src/qrisp/circuit/compilation_acceleration.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/circuit/controlled_operations.py` & `qrisp-0.4.5/src/qrisp/circuit/controlled_operations.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/circuit/instruction.py` & `qrisp-0.4.5/src/qrisp/circuit/instruction.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/circuit/library.py` & `qrisp-0.4.5/src/qrisp/circuit/library.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/circuit/operation.py` & `qrisp-0.4.5/src/qrisp/circuit/operation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/circuit/quantum_circuit.py` & `qrisp-0.4.5/src/qrisp/circuit/quantum_circuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1055,15 +1055,25 @@
 
         Returns
         -------
         string
             The OPENQASM string.
 
         """
-        return self.to_qiskit().qasm(formatted, filename, encoding)
+        qiskit_qc = self.to_qiskit()
+        if hasattr(qiskit_qc, "qasm"):
+            qasm_str = qiskit_qc.qasm(formatted, filename, encoding)
+        else:
+            from qiskit.qasm2 import dump, dumps
+            if filename:
+                qasm_str = dump(qiskit_qc, filename)
+            else:
+                qasm_str = dumps(qiskit_qc)
+        
+        return qasm_str
 
     def depth(self, depth_indicator = lambda x : 1, transpile=True):
         """
         Returns the depth of the QuantumCircuit. Note that the depth on QuantumCircuit
         which are not transpiled, might have very little correlation with the runtime.
 
         Parameters
```

### Comparing `qrisp-0.4.4/src/qrisp/circuit/qubit.py` & `qrisp-0.4.5/src/qrisp/circuit/qubit.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/circuit/standard_operations.py` & `qrisp-0.4.5/src/qrisp/circuit/standard_operations.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/circuit/transpiler.py` & `qrisp-0.4.5/src/qrisp/circuit/transpiler.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/core/__init__.py` & `qrisp-0.4.5/src/qrisp/core/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/core/compilation.py` & `qrisp-0.4.5/src/qrisp/core/compilation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/core/library.py` & `qrisp-0.4.5/src/qrisp/core/library.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/core/quantum_array.py` & `qrisp-0.4.5/src/qrisp/core/quantum_array.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/core/quantum_dictionary.py` & `qrisp-0.4.5/src/qrisp/core/quantum_dictionary.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/core/quantum_session.py` & `qrisp-0.4.5/src/qrisp/core/quantum_session.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/core/quantum_variable.py` & `qrisp-0.4.5/src/qrisp/core/quantum_variable.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/core/session_merging_tools.py` & `qrisp-0.4.5/src/qrisp/core/session_merging_tools.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/default_backend.py` & `qrisp-0.4.5/src/qrisp/default_backend.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/environments/GMS_environment.py` & `qrisp-0.4.5/src/qrisp/environments/GMS_environment.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/environments/__init__.py` & `qrisp-0.4.5/src/qrisp/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/environments/conjugation_environment.py` & `qrisp-0.4.5/src/qrisp/environments/conjugation_environment.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/environments/control_environment.py` & `qrisp-0.4.5/src/qrisp/environments/control_environment.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/environments/custom_control_environment.py` & `qrisp-0.4.5/src/qrisp/environments/custom_control_environment.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/environments/gate_wrap_environment.py` & `qrisp-0.4.5/src/qrisp/environments/gate_wrap_environment.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/environments/iteration_environment.py` & `qrisp-0.4.5/src/qrisp/environments/iteration_environment.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/environments/quantum_conditionals.py` & `qrisp-0.4.5/src/qrisp/environments/quantum_conditionals.py`

 * *Files 1% similar despite different names*

```diff
@@ -614,15 +614,19 @@
         if input_0.size != input_1.size:
             raise Exception(
                 "Tried to evaluate equality conditional"
                 "for QuantumVariables of differing size"
             )
 
         
-        with conjugate(cx)(input_0, input_1):
+        def multi_cx(input_0, input_1):
+            for i in range(len(input_0)):
+                cx(input_0[i], input_1[i])
+        
+        with conjugate(multi_cx)(input_0, input_1):
             mcx(input_1, res, method="balauca", ctrl_state=0)
         
 
 
     else:
         label_int = input_0.encoder(input_1)
```

### Comparing `qrisp-0.4.4/src/qrisp/environments/quantum_environments.py` & `qrisp-0.4.5/src/qrisp/environments/quantum_environments.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/environments/quantum_inversion.py` & `qrisp-0.4.5/src/qrisp/environments/quantum_inversion.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/grover/__init__.py` & `qrisp-0.4.5/src/qrisp/grover/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/grover/grover_tools.py` & `qrisp-0.4.5/src/qrisp/grover/grover_tools.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/__init__.py` & `qrisp-0.4.5/src/qrisp/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/backends.py` & `qrisp-0.4.5/src/qrisp/interface/backends.py`

 * *Files 10% similar despite different names*

```diff
@@ -152,17 +152,21 @@
     {9: 1.0}
 
 
     """
 
     def __init__(self, backend=None, port=8079):
         if backend is None:
-            from qiskit import Aer
-
-            backend = Aer.get_backend("qasm_simulator")
+            
+            try:
+                from qiskit import Aer
+                backend = Aer.get_backend("qasm_simulator")
+            except ImportError:
+                from qiskit.providers.basic_provider import BasicProvider
+                backend = BasicProvider().get_backend('basic_simulator')
 
         # Create the run method
         def run(qasm_str, shots, token = ""):
             # Convert to qiskit
             from qiskit import QuantumCircuit
 
             qiskit_qc = QuantumCircuit.from_qasm_str(qasm_str)
```

### Comparing `qrisp-0.4.4/src/qrisp/interface/circuit_converter.py` & `qrisp-0.4.5/src/qrisp/interface/circuit_converter.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/converter/__init__.py` & `qrisp-0.4.5/src/qrisp/interface/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/converter/convert_to_pytket.py` & `qrisp-0.4.5/src/qrisp/interface/converter/convert_to_pytket.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/converter/convert_to_qml.py` & `qrisp-0.4.5/src/qrisp/interface/converter/convert_to_qml.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/converter/convert_to_qulacs.py` & `qrisp-0.4.5/src/qrisp/interface/converter/convert_to_qulacs.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/docker_backends.py` & `qrisp-0.4.5/src/qrisp/interface/docker_backends.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,8 +41,12 @@
 
 def QSimCirq():
     return BackendClient(api_endpoint, port = 8089)
     
 def QiboSim():
     return BackendClient(api_endpoint, port = 8090)
 
-    
+def QrispSim():
+    return BackendClient(api_endpoint, port = 8090)
+
+def QiskitSim():
+    return BackendClient(api_endpoint, port = 8090)
```

### Comparing `qrisp-0.4.4/src/qrisp/interface/openapi_interface/__init__.py` & `qrisp-0.4.5/src/qrisp/interface/openapi_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/openapi_interface/backend_client.py` & `qrisp-0.4.5/src/qrisp/interface/openapi_interface/backend_client.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/openapi_interface/backend_server.py` & `qrisp-0.4.5/src/qrisp/interface/openapi_interface/backend_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/openapi_interface/interface_types.py` & `qrisp-0.4.5/src/qrisp/interface/openapi_interface/interface_types.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/qunicorn/__init__.py` & `qrisp-0.4.5/src/qrisp/interface/qunicorn/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/qunicorn/backend_client.py` & `qrisp-0.4.5/src/qrisp/interface/qunicorn/backend_client.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/qunicorn/backend_server.py` & `qrisp-0.4.5/src/qrisp/interface/qunicorn/backend_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/thrift_interface/__init__.py` & `qrisp-0.4.5/src/qrisp/interface/thrift_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/thrift_interface/backend_client.py` & `qrisp-0.4.5/src/qrisp/interface/thrift_interface/backend_client.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/thrift_interface/backend_server.py` & `qrisp-0.4.5/src/qrisp/interface/thrift_interface/backend_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/thrift_interface/codegen/BackendService.py` & `qrisp-0.4.5/src/qrisp/interface/thrift_interface/codegen/BackendService.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/thrift_interface/codegen/__init__.py` & `qrisp-0.4.5/src/qrisp/interface/thrift_interface/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/thrift_interface/codegen/constants.py` & `qrisp-0.4.5/src/qrisp/interface/thrift_interface/codegen/constants.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/thrift_interface/codegen/ttypes.py` & `qrisp-0.4.5/src/qrisp/interface/thrift_interface/codegen/ttypes.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/thrift_interface/interface_types.py` & `qrisp-0.4.5/src/qrisp/interface/thrift_interface/interface_types.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/interface/thrift_interface/stoppable_thrift_server.py` & `qrisp-0.4.5/src/qrisp/interface/thrift_interface/stoppable_thrift_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/iterators/__init__.py` & `qrisp-0.4.5/src/qrisp/iterators/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/iterators/qrange.py` & `qrisp-0.4.5/src/qrisp/iterators/qrange.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/logic_synthesis/__init__.py` & `qrisp-0.4.5/src/qrisp/logic_synthesis/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/logic_synthesis/gray_synthesis.py` & `qrisp-0.4.5/src/qrisp/logic_synthesis/gray_synthesis.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/logic_synthesis/pprm_synthesis.py` & `qrisp-0.4.5/src/qrisp/logic_synthesis/pprm_synthesis.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/logic_synthesis/truth_tables.py` & `qrisp-0.4.5/src/qrisp/logic_synthesis/truth_tables.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/mcx_algs/__init__.py` & `qrisp-0.4.5/src/qrisp/mcx_algs/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/mcx_algs/amy.py` & `qrisp-0.4.5/src/qrisp/mcx_algs/amy.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/mcx_algs/balauca.py` & `qrisp-0.4.5/src/qrisp/mcx_algs/balauca.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/mcx_algs/circuit_library.py` & `qrisp-0.4.5/src/qrisp/mcx_algs/circuit_library.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/mcx_algs/gidney.py` & `qrisp-0.4.5/src/qrisp/mcx_algs/gidney.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/mcx_algs/gms.py` & `qrisp-0.4.5/src/qrisp/mcx_algs/gms.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/mcx_algs/gray.py` & `qrisp-0.4.5/src/qrisp/mcx_algs/gray.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/mcx_algs/gray_pt.py` & `qrisp-0.4.5/src/qrisp/mcx_algs/gray_pt.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/mcx_algs/jones.py` & `qrisp-0.4.5/src/qrisp/mcx_algs/jones.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/mcx_algs/maslov.py` & `qrisp-0.4.5/src/qrisp/mcx_algs/maslov.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/mcx_algs/multi_cx.py` & `qrisp-0.4.5/src/qrisp/mcx_algs/multi_cx.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/mcx_algs/yong.py` & `qrisp-0.4.5/src/qrisp/mcx_algs/yong.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/misc/GMS_tools.py` & `qrisp-0.4.5/src/qrisp/misc/GMS_tools.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/misc/__init__.py` & `qrisp-0.4.5/src/qrisp/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/misc/depth_reduction.py` & `qrisp-0.4.5/src/qrisp/misc/depth_reduction.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/misc/utility.py` & `qrisp-0.4.5/src/qrisp/misc/utility.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/__init__.py` & `qrisp-0.4.5/src/qrisp/qaoa/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/mixers.py` & `qrisp-0.4.5/src/qrisp/qaoa/mixers.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/optimization_wrappers/__init__.py` & `qrisp-0.4.5/src/qrisp/qaoa/optimization_wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/optimization_wrappers/fourier_wrapper.py` & `qrisp-0.4.5/src/qrisp/qaoa/optimization_wrappers/fourier_wrapper.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/parameters/__init__.py` & `qrisp-0.4.5/src/qrisp/qaoa/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/parameters/fourier_params.py` & `qrisp-0.4.5/src/qrisp/qaoa/parameters/fourier_params.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/problems/MaxIndep_qiroBM.py` & `qrisp-0.4.5/src/qrisp/qaoa/problems/MaxIndep_qiroBM.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-import qrisp
-
-from qrisp.qiroStuff.qiroProblem import QIROProblem
-
-from qrisp.qiroStuff.qiroMaxIndepSetInfrastr import *
-
-from qrisp.qaoa.qaoa_problem import QAOAProblem
-from qrisp.qaoa.problems.create_rdm_graph import create_rdm_graph
-from qrisp.qaoa.problems.maxIndepSetInfrastr import maxIndepSetCostOp, maxIndepSetclCostfct
-from qrisp.qaoa.mixers import RX_mixer
-from qrisp import QuantumVariable
-from qrisp.qaoa.qaoa_benchmark_data import approximation_ratio
-import matplotlib.pyplot as plt
-import numpy as np
-import networkx as nx
-import itertools
-
-# qiskit mps simulator
-
-optimal_sols = "10000000000000000000"
-num_nodes = 20
-
-recursive_array = []
-normal_array = []
-
-
-for index in range(30):
-    giraf = create_rdm_graph(num_nodes,0.3, seed =  index*3)
-    qarg = QuantumVariable(giraf.number_of_nodes())
-
-    maxindep_instance = QAOAProblem(maxIndepSetCostOp(giraf), RX_mixer, maxIndepSetclCostfct(giraf))
-    the_recursive = QIROProblem(giraf, maxindep_instance, 
-                                     replacement_routine=create_maxIndep_replacement_routine, 
-                                     qiro_cost_operator= create_maxIndep_cost_operator_reduced,
-                                     qiro_mixer= create_maxIndep_mixer_reduced,
-                                     qiro_init_function= init_function_reduced
-                                     )
-
-    res, solutions,  exclusions, corr_vals = the_recursive.run_new_idea(qarg=qarg, depth = 3, n_recursions = 1)
-    testCostFun = maxIndepSetclCostfct(giraf)
-
-    approx_rat = approximation_ratio(res, optimal_sols,testCostFun)
-    print(approx_rat)
-    recursive_array.append(approx_rat)
-    qarg.delete()
-
-
-for index2 in range(30):
-
-    giraf = create_rdm_graph(num_nodes,0.3, seed =  index2*3)
-
-    qarg = QuantumVariable(giraf.number_of_nodes())
-
-    maxindep_instance = QAOAProblem(maxIndepSetCostOp(giraf), RX_mixer, maxIndepSetclCostfct(giraf))
-    res = maxindep_instance.run(qarg=qarg, depth = 5)
-    testCostFun = maxIndepSetclCostfct(giraf)
-
-    approx_rat = approximation_ratio(res, optimal_sols,testCostFun)
-    print(approx_rat)
-    normal_array.append(approx_rat)
-    qarg.delete()
-
-print("recursive")
-print(sum(recursive_array)/len(recursive_array))
-
-print("normal")
+import qrisp
+
+from qrisp.qiroStuff.qiroProblem import QIROProblem
+
+from qrisp.qiroStuff.qiroMaxIndepSetInfrastr import *
+
+from qrisp.qaoa.qaoa_problem import QAOAProblem
+from qrisp.qaoa.problems.create_rdm_graph import create_rdm_graph
+from qrisp.qaoa.problems.maxIndepSetInfrastr import maxIndepSetCostOp, maxIndepSetclCostfct
+from qrisp.qaoa.mixers import RX_mixer
+from qrisp import QuantumVariable
+from qrisp.qaoa.qaoa_benchmark_data import approximation_ratio
+import matplotlib.pyplot as plt
+import numpy as np
+import networkx as nx
+import itertools
+
+# qiskit mps simulator
+
+optimal_sols = "10000000000000000000"
+num_nodes = 20
+
+recursive_array = []
+normal_array = []
+
+
+for index in range(30):
+    giraf = create_rdm_graph(num_nodes,0.3, seed =  index*3)
+    qarg = QuantumVariable(giraf.number_of_nodes())
+
+    maxindep_instance = QAOAProblem(maxIndepSetCostOp(giraf), RX_mixer, maxIndepSetclCostfct(giraf))
+    the_recursive = QIROProblem(giraf, maxindep_instance, 
+                                     replacement_routine=create_maxIndep_replacement_routine, 
+                                     qiro_cost_operator= create_maxIndep_cost_operator_reduced,
+                                     qiro_mixer= create_maxIndep_mixer_reduced,
+                                     qiro_init_function= init_function_reduced
+                                     )
+
+    res, solutions,  exclusions, corr_vals = the_recursive.run_new_idea(qarg=qarg, depth = 3, n_recursions = 1)
+    testCostFun = maxIndepSetclCostfct(giraf)
+
+    approx_rat = approximation_ratio(res, optimal_sols,testCostFun)
+    print(approx_rat)
+    recursive_array.append(approx_rat)
+    qarg.delete()
+
+
+for index2 in range(30):
+
+    giraf = create_rdm_graph(num_nodes,0.3, seed =  index2*3)
+
+    qarg = QuantumVariable(giraf.number_of_nodes())
+
+    maxindep_instance = QAOAProblem(maxIndepSetCostOp(giraf), RX_mixer, maxIndepSetclCostfct(giraf))
+    res = maxindep_instance.run(qarg=qarg, depth = 5)
+    testCostFun = maxIndepSetclCostfct(giraf)
+
+    approx_rat = approximation_ratio(res, optimal_sols,testCostFun)
+    print(approx_rat)
+    normal_array.append(approx_rat)
+    qarg.delete()
+
+print("recursive")
+print(sum(recursive_array)/len(recursive_array))
+
+print("normal")
 print(sum(normal_array)/len(normal_array))
```

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/problems/QUBO.py` & `qrisp-0.4.5/src/qrisp/qaoa/problems/QUBO.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/problems/__init__.py` & `qrisp-0.4.5/src/qrisp/qaoa/problems/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/problems/create_rdm_graph.py` & `qrisp-0.4.5/src/qrisp/qaoa/problems/create_rdm_graph.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/problems/eThrTwoLinInfrastr.py` & `qrisp-0.4.5/src/qrisp/qaoa/problems/eThrTwoLinInfrastr.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/problems/maxCliqueInfrastr.py` & `qrisp-0.4.5/src/qrisp/qaoa/problems/maxCliqueInfrastr.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/problems/maxCut.py` & `qrisp-0.4.5/src/qrisp/qaoa/problems/maxCut.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/problems/maxIndepSetInfrastr.py` & `qrisp-0.4.5/src/qrisp/qaoa/problems/maxIndepSetInfrastr.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/problems/maxKColorableSubgraph.py` & `qrisp-0.4.5/src/qrisp/qaoa/problems/maxKColorableSubgraph.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/problems/maxSatInfrastr.py` & `qrisp-0.4.5/src/qrisp/qaoa/problems/maxSatInfrastr.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/problems/maxSetPackInfrastr.py` & `qrisp-0.4.5/src/qrisp/qaoa/problems/maxSetPackInfrastr.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/problems/minSetCoverInfrastr.py` & `qrisp-0.4.5/src/qrisp/qaoa/problems/minSetCoverInfrastr.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/qaoa_benchmark_data.py` & `qrisp-0.4.5/src/qrisp/qaoa/qaoa_benchmark_data.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qaoa/qaoa_problem.py` & `qrisp-0.4.5/src/qrisp/qaoa/qaoa_problem.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qtypes/__init__.py` & `qrisp-0.4.5/src/qrisp/qtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qtypes/quantum_bool.py` & `qrisp-0.4.5/src/qrisp/qtypes/quantum_bool.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qtypes/quantum_char.py` & `qrisp-0.4.5/src/qrisp/qtypes/quantum_char.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/qtypes/quantum_float.py` & `qrisp-0.4.5/src/qrisp/qtypes/quantum_float.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,15 +462,15 @@
         if isinstance(other, QuantumFloat):
             return sbp_sub(other, self)
         elif isinstance(other, (int, float)):
             res = self.duplicate(init=True)
             if not res.signed:
                 res.add_sign()
             x(res)
-            res -= other - 2**res.exponent
+            res += other + 2**res.exponent
             return res
         else:
             raise Exception(
                 "Subtraction with type " + str(type(other)) + " not implemented"
             )
 
     @gate_wrap(permeability="args", is_qfree=True)
```

### Comparing `qrisp-0.4.4/src/qrisp/qtypes/quantum_string.py` & `qrisp-0.4.5/src/qrisp/qtypes/quantum_string.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/quantum_backtracking/__init__.py` & `qrisp-0.4.5/src/qrisp/quantum_backtracking/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/quantum_backtracking/backtracking_tree.py` & `qrisp-0.4.5/src/qrisp/quantum_backtracking/backtracking_tree.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/quantum_network/__init__.py` & `qrisp-0.4.5/src/qrisp/quantum_network/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/quantum_network/interface/codegen/QuantumNetworkService.py` & `qrisp-0.4.5/src/qrisp/quantum_network/interface/codegen/QuantumNetworkService.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/quantum_network/interface/codegen/__init__.py` & `qrisp-0.4.5/src/qrisp/quantum_network/interface/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/quantum_network/interface/codegen/constants.py` & `qrisp-0.4.5/src/qrisp/quantum_network/interface/codegen/constants.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/quantum_network/interface/codegen/ttypes.py` & `qrisp-0.4.5/src/qrisp/quantum_network/interface/codegen/ttypes.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/quantum_network/interface_connection_example.py` & `qrisp-0.4.5/src/qrisp/quantum_network/interface_connection_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/quantum_network/qn_client.py` & `qrisp-0.4.5/src/qrisp/quantum_network/qn_client.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/quantum_network/qn_server.py` & `qrisp-0.4.5/src/qrisp/quantum_network/qn_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/quantum_network/qn_simulator_server.py` & `qrisp-0.4.5/src/qrisp/quantum_network/qn_simulator_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/quantum_network/quantum_network_session.py` & `qrisp-0.4.5/src/qrisp/quantum_network/quantum_network_session.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/shor/__init__.py` & `qrisp-0.4.5/src/qrisp/shor/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/shor/crypto_tools.py` & `qrisp-0.4.5/src/qrisp/shor/crypto_tools.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/shor/shors_algorithm.py` & `qrisp-0.4.5/src/qrisp/shor/shors_algorithm.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/simulator/__init__.py` & `qrisp-0.4.5/src/qrisp/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/simulator/bi_array_helper.py` & `qrisp-0.4.5/src/qrisp/simulator/bi_array_helper.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/simulator/bi_arrays.py` & `qrisp-0.4.5/src/qrisp/simulator/bi_arrays.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/simulator/circuit_preprocessing.py` & `qrisp-0.4.5/src/qrisp/simulator/circuit_preprocessing.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/simulator/circuit_reordering.py` & `qrisp-0.4.5/src/qrisp/simulator/circuit_reordering.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/simulator/numerics_config.py` & `qrisp-0.4.5/src/qrisp/simulator/numerics_config.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/simulator/quantum_state.py` & `qrisp-0.4.5/src/qrisp/simulator/quantum_state.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/simulator/simulator.py` & `qrisp-0.4.5/src/qrisp/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/simulator/tensor_factor.py` & `qrisp-0.4.5/src/qrisp/simulator/tensor_factor.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/simulator/unitary_management.py` & `qrisp-0.4.5/src/qrisp/simulator/unitary_management.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/uncomputation/__init__.py` & `qrisp-0.4.5/src/qrisp/uncomputation/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/uncomputation/type_checker.py` & `qrisp-0.4.5/src/qrisp/uncomputation/type_checker.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/uncomputation/uncomputation.py` & `qrisp-0.4.5/src/qrisp/uncomputation/uncomputation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp/uncomputation/unqomp.py` & `qrisp-0.4.5/src/qrisp/uncomputation/unqomp.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/src/qrisp.egg-info/PKG-INFO` & `qrisp-0.4.5/src/qrisp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: qrisp
-Version: 0.4.4
+Version: 0.4.5
 Summary: Qrisp - A high level language for gate-based quantum computing
 Home-page: https://github.com/fraunhoferfokus/Qrisp
 Author: Raphael Seidel
 Author-email: raphael.seidel@fokus.fraunhofer.de
 Project-URL: Bug Tracker, https://github.com/fraunhoferfokus/Qrisp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: connexion>=2.12.0
-Requires-Dist: qiskit>=0.34.2
+Requires-Dist: qiskit>=0.44.0
 Requires-Dist: thrift>=0.15.0
 Requires-Dist: matplotlib>=3.5.1
 Requires-Dist: waitress>=2.1.1
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: numba
 Requires-Dist: networkx
 Requires-Dist: tdqm
```

### Comparing `qrisp-0.4.4/src/qrisp.egg-info/SOURCES.txt` & `qrisp-0.4.5/src/qrisp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_GMS_environment_example.py` & `qrisp-0.4.5/tests/test_GMS_environment_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_GXX_converter_example.py` & `qrisp-0.4.5/tests/test_GXX_converter_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_GXX_gates_example.py` & `qrisp-0.4.5/tests/test_GXX_gates_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_GZZ_gates_example.py` & `qrisp-0.4.5/tests/test_GZZ_gates_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_QAE.py` & `qrisp-0.4.5/tests/test_QAE.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_QAOAMkCS.py` & `qrisp-0.4.5/tests/test_QAOAMkCS.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_QAOAQUBO.py` & `qrisp-0.4.5/tests/test_QAOAQUBO.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_QAOA_TQA_warm_start.py` & `qrisp-0.4.5/tests/test_QAOA_TQA_warm_start.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_QAOAeTwoThrLin.py` & `qrisp-0.4.5/tests/test_QAOAeTwoThrLin.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_QAOAmaxClique.py` & `qrisp-0.4.5/tests/test_QAOAmaxClique.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_QAOAmaxCut.py` & `qrisp-0.4.5/tests/test_QAOAmaxCut.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_QAOAmaxIndepSet.py` & `qrisp-0.4.5/tests/test_QAOAmaxIndepSet.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_QAOAmaxSat.py` & `qrisp-0.4.5/tests/test_QAOAmaxSat.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_QAOAmaxSetPacking.py` & `qrisp-0.4.5/tests/test_QAOAmaxSetPacking.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_QAOAminSetCover.py` & `qrisp-0.4.5/tests/test_QAOAminSetCover.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_QAOAtrain_func.py` & `qrisp-0.4.5/tests/test_QAOAtrain_func.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_abstr_params_printing.py` & `qrisp-0.4.5/tests/test_abstr_params_printing.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_abstract_parameters.py` & `qrisp-0.4.5/tests/test_abstract_parameters.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_amplitude_amplification.py` & `qrisp-0.4.5/tests/test_amplitude_amplification.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_amy_mcx.py` & `qrisp-0.4.5/tests/test_amy_mcx.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_array_entry_manipulation.py` & `qrisp-0.4.5/tests/test_array_entry_manipulation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_backtracking.py` & `qrisp-0.4.5/tests/test_backtracking.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_comparisons.py` & `qrisp-0.4.5/tests/test_comparisons.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,119 +13,169 @@
 * available at https://www.gnu.org/software/classpath/license.html.
 *
 * SPDX-License-Identifier: EPL-2.0 OR GPL-2.0 WITH Classpath-exception-2.0
 ********************************************************************************/
 """
 
 
-from qrisp import h, QuantumFloat, multi_measurement
+from qrisp import h, QuantumFloat, multi_measurement, QuantumModulus
 import numpy as np
 
 
-def test_comparison():
-    def test_comparison_helper(qf_0, qf_1, comp):
-        qf_0 = qf_0.duplicate()
-        h(qf_0)
-
-        if isinstance(qf_1, QuantumFloat):
-            qf_1 = qf_1.duplicate()
-            h(qf_1)
-
-        if comp == "eq":
-            qf_res = qf_0 == qf_1
-        elif comp == "neq":
-            qf_res = qf_0 != qf_1
-        elif comp == "leq":
-            qf_res = qf_0 <= qf_1
-        elif comp == "geq":
-            qf_res = qf_0 >= qf_1
-        elif comp == "lt":
-            qf_res = qf_0 < qf_1
-        elif comp == "gt":
-            qf_res = qf_0 > qf_1
-
-        if isinstance(qf_1, QuantumFloat):
-            mes_res = multi_measurement([qf_0, qf_1, qf_res])
-            for a, b, c in mes_res.keys():
-                print(a, b, c)
-                if comp == "eq":
-                    assert (a == b) == c
-                elif comp == "neq":
-                    assert (a != b) == c
-                elif comp == "leq":
-                    assert (a <= b) == c
-                elif comp == "geq":
-                    assert (a >= b) == c
-                elif comp == "lt":
-                    assert (a < b) == c
-                elif comp == "gt":
-                    assert (a > b) == c
-
-            # Test correct phase behavior7
-            statevector = qf_res.qs.statevector("array")
-            angles = np.angle(
-                statevector[
-                    np.abs(statevector) > 1 / 2 ** ((qf_0.size + qf_1.size) / 2)
-                ]
-            )
-            assert np.sum(np.abs(angles)) < 0.1
-        else:
-            mes_res = multi_measurement([qf_0, qf_res])
-            for a, c in mes_res.keys():
-                b = qf_1
-                print(a, b, c)
-                if comp == "eq":
-                    assert (a == b) == c
-                elif comp == "neq":
-                    assert (a != b) == c
-                elif comp == "leq":
-                    assert (a <= b) == c
-                elif comp == "geq":
-                    assert (a >= b) == c
-                elif comp == "lt":
-                    assert (a < b) == c
-                elif comp == "gt":
-                    assert (a > b) == c
+def test_quantum_float_comparison():
 
     a = QuantumFloat(5, 2, signed=False)
     b = QuantumFloat(5, -1, signed=True)
     # Test all the operators
     for comp in ["eq", "neq", "lt", "gt", "leq", "geq"]:
-        test_comparison_helper(a, b, comp)
+        comparison_helper(a, b, comp)
 
     # Test specific constellations of QuantumFloat parameters
     a = QuantumFloat(3, -1, signed=True)
     b = QuantumFloat(5, 1, signed=True)
-    test_comparison_helper(a, b, "lt")
+    comparison_helper(a, b, "lt")
 
     a = QuantumFloat(5, 2, signed=False)
     b = QuantumFloat(5, -1, signed=True)
-    test_comparison_helper(a, b, "lt")
+    comparison_helper(a, b, "lt")
 
     a = QuantumFloat(4, -4, signed=False)
     b = QuantumFloat(4, 0, signed=True)
-    test_comparison_helper(a, b, "lt")
+    comparison_helper(a, b, "lt")
 
     a = QuantumFloat(4, 1, signed=True)
     b = QuantumFloat(3, -1, signed=False)
-    test_comparison_helper(a, b, "lt")
+    comparison_helper(a, b, "lt")
 
     # Test semi-classical comparisons
     a = QuantumFloat(4, signed=False)
     b = 4
-    test_comparison_helper(a, b, "lt")
-    test_comparison_helper(a, b, "gt")
+    comparison_helper(a, b, "lt")
+    comparison_helper(a, b, "gt")
 
     a = QuantumFloat(4, signed=True)
     b = 4
-    test_comparison_helper(a, b, "lt")
-    test_comparison_helper(a, b, "gt")
+    comparison_helper(a, b, "lt")
+    comparison_helper(a, b, "gt")
 
     a = QuantumFloat(4, -2, signed=False)
     b = 4
-    test_comparison_helper(a, b, "lt")
-    test_comparison_helper(a, b, "gt")
+    comparison_helper(a, b, "lt")
+    comparison_helper(a, b, "gt")
 
     a = QuantumFloat(8, 3, signed=False)
     b = 16
-    test_comparison_helper(a, b, "lt")
-    test_comparison_helper(a, b, "gt")
+    comparison_helper(a, b, "lt")
+    comparison_helper(a, b, "gt")
+
+
+def test_quantum_modulus_comparison():
+    
+    a = QuantumModulus(5)
+    b = QuantumModulus(5)
+    
+    for comp in ["eq", "neq", "lt", "gt", "leq", "geq"]:
+        comparison_helper(a, b, comp)
+        
+    a = QuantumModulus(7)
+    b = QuantumModulus(7)
+    
+    for comp in ["eq", "neq", "lt", "gt", "leq", "geq"]:
+        comparison_helper(a, b, comp)
+        
+    a = QuantumModulus(13)
+    b = QuantumModulus(13)
+    
+    for comp in ["eq", "neq", "lt", "gt", "leq", "geq"]:
+        comparison_helper(a, b, comp)
+        
+    a = QuantumModulus(5)
+    b = 3
+    
+    for comp in ["eq", "neq", "lt", "gt", "leq", "geq"]:
+        comparison_helper(a, b, comp)
+        
+    a = QuantumModulus(7)
+    b = 5
+    
+    for comp in ["eq", "neq", "lt", "gt", "leq", "geq"]:
+        comparison_helper(a, b, comp)
+        
+    a = QuantumModulus(13)
+    b = 7
+    
+    for comp in ["eq", "neq", "lt", "gt", "leq", "geq"]:
+        comparison_helper(a, b, comp)
+
+def comparison_helper(qf_0, qf_1, comp):
+    qf_0 = qf_0.duplicate()
+    h(qf_0)
+
+    if isinstance(qf_1, (QuantumFloat, QuantumModulus)):
+        qf_1 = qf_1.duplicate()
+        h(qf_1)
+
+    if comp == "eq":
+        qf_res = qf_0 == qf_1
+    elif comp == "neq":
+        qf_res = qf_0 != qf_1
+    elif comp == "leq":
+        qf_res = qf_0 <= qf_1
+    elif comp == "geq":
+        qf_res = qf_0 >= qf_1
+    elif comp == "lt":
+        qf_res = qf_0 < qf_1
+    elif comp == "gt":
+        qf_res = qf_0 > qf_1
+
+    if isinstance(qf_1, (QuantumFloat, QuantumModulus)):
+        mes_res = multi_measurement([qf_0, qf_1, qf_res])
+        for a, b, c in mes_res.keys():
+            
+            if a is np.nan or b is np.nan:
+                continue
+            
+            print(a, b, c)
+            
+            
+            if comp == "eq":
+                assert (a == b) == c
+            elif comp == "neq":
+                assert (a != b) == c
+            elif comp == "leq":
+                assert (a <= b) == c
+            elif comp == "geq":
+                assert (a >= b) == c
+            elif comp == "lt":
+                assert (a < b) == c
+            elif comp == "gt":
+                assert (a > b) == c
+
+        # Test correct phase behavior7
+        statevector = qf_res.qs.statevector("array")
+        angles = np.angle(
+            statevector[
+                np.abs(statevector) > 1 / 2 ** ((qf_0.size + qf_1.size) / 2)
+            ]
+        )
+        assert np.sum(np.abs(angles)) < 0.1
+    else:
+        mes_res = multi_measurement([qf_0, qf_res])
+        for a, c in mes_res.keys():
+            
+            if a is np.nan:
+                continue
+            
+            b = qf_1
+            print(a, b, c)
+            if comp == "eq":
+                assert (a == b) == c
+            elif comp == "neq":
+                assert (a != b) == c
+            elif comp == "leq":
+                assert (a <= b) == c
+            elif comp == "geq":
+                assert (a >= b) == c
+            elif comp == "lt":
+                assert (a < b) == c
+            elif comp == "gt":
+                assert (a > b) == c
```

### Comparing `qrisp-0.4.4/tests/test_conditional_environments_example.py` & `qrisp-0.4.5/tests/test_conditional_environments_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_conjugation_environment.py` & `qrisp-0.4.5/tests/test_conjugation_environment.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_controlled_gates.py` & `qrisp-0.4.5/tests/test_controlled_gates.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_converter_QrispToQml.py` & `qrisp-0.4.5/tests/test_converter_QrispToQml.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_custom_control.py` & `qrisp-0.4.5/tests/test_custom_control.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_cycling_function.py` & `qrisp-0.4.5/tests/test_cycling_function.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_depth_calculation.py` & `qrisp-0.4.5/tests/test_depth_calculation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_diagonal_hamiltonian_application.py` & `qrisp-0.4.5/tests/test_diagonal_hamiltonian_application.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_fourier_adder.py` & `qrisp-0.4.5/tests/test_fourier_adder.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_gidney_mcx.py` & `qrisp-0.4.5/tests/test_gidney_mcx.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_gray_synthesis_example.py` & `qrisp-0.4.5/tests/test_gray_synthesis_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_grovers_algorithm.py` & `qrisp-0.4.5/tests/test_grovers_algorithm.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_hello_world.py` & `qrisp-0.4.5/tests/test_hello_world.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_inpl_matrix_multiplication_example.py` & `qrisp-0.4.5/tests/test_inpl_matrix_multiplication_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_iteration_environment.py` & `qrisp-0.4.5/tests/test_iteration_environment.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_jones_mcx.py` & `qrisp-0.4.5/tests/test_jones_mcx.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_loops.py` & `qrisp-0.4.5/tests/test_loops.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_matrix_multiplication_example.py` & `qrisp-0.4.5/tests/test_matrix_multiplication_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_mcx.py` & `qrisp-0.4.5/tests/test_mcx.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_measurement_reduction.py` & `qrisp-0.4.5/tests/test_measurement_reduction.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_modular_arithmetic.py` & `qrisp-0.4.5/tests/test_modular_arithmetic.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_outcome_array.py` & `qrisp-0.4.5/tests/test_outcome_array.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_qcla.py` & `qrisp-0.4.5/tests/test_qcla.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_qiskit_backend_client.py` & `qrisp-0.4.5/tests/test_qiskit_backend_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,64 +15,70 @@
 * SPDX-License-Identifier: EPL-2.0 OR GPL-2.0 WITH Classpath-exception-2.0
 ********************************************************************************/
 """
 
 # Created by ann81984 at 23.05.2022
 import numpy as np
 
-from qrisp.core import QuantumSession
+from qrisp import QuantumCircuit
 from qrisp.interface.backends import VirtualBackend
 from qrisp.interface.backends import VirtualQiskitBackend
 
 
 
 def test_qiskit_backend_client():
-    # TO-DO prevent this test from crashing regardless of functionality
-    from qiskit import Aer
-    # Create QuantumSession
-    qs = QuantumSession()
+    
+    try:
+        from qiskit import Aer
+        backend = Aer.get_backend("qasm_simulator")
+    except ImportError:
+        from qiskit.providers.basic_provider import BasicProvider
+        backend = BasicProvider().get_backend('basic_simulator')
+
+    # Create QuantumCricuit
+    qc = QuantumCircuit()
+
+    qc.add_qubit()
+    qc.add_qubit()
+    
 
-    qs.add_qubit()
-    qs.add_qubit()
-    qs.add_clbit()
+    qc.h(0)
 
-    qs.h(0)
+    qc.rz(np.pi / 2, 0)
 
-    qs.rz(np.pi / 2, 0)
-
-    qs.x(0)
-    qs.cx(0, 1)
-    qs.measure(1, 0)
+    qc.x(0)
+    qc.cx(0, 1)
+    
 
-    qs.append(qs.to_op("composed_op"), qs.qubits, qs.clbits)
+    qc.append(qc.to_op("composed_op"), qc.qubits, qc.clbits)
 
-    qs.append(qs.to_op("multi_composed_op"), qs.qubits, qs.clbits)
+    qc.append(qc.to_op("multi_composed_op"), qc.qubits, qc.clbits)
 
-    print(qs)
+    qc.add_clbit()
+    qc.measure(1, 0)    
+    print(qc)
 
     ###################
 
     # Create VirtualBackend
-    def sample_run_func(qc, shots):
+    def sample_run_func(qc, shots, token):
         print("Executing Circuit")
         return {"0": shots}
 
     test_virtual_backend = VirtualBackend(sample_run_func)
 
-    print(test_virtual_backend.run(qs, 100))
-    assert str(test_virtual_backend.run(qs, 100)) == "{'0': 100}"
-    assert test_virtual_backend.run(qs, 100)["0"] == 100
+    print(test_virtual_backend.run(qc, 100))
+    assert str(test_virtual_backend.run(qc, 100)) == "{'0': 100}"
+    assert test_virtual_backend.run(qc, 100)["0"] == 100
 
     ###################
 
     # Create Qiskit Backend
-    test_qiskit_backend = VirtualQiskitBackend(Aer.get_backend("qasm_simulator"))
-
-    from qrisp import QuantumCircuit
+    test_qiskit_backend = VirtualQiskitBackend()
 
     qc = QuantumCircuit(4, 1)
     qc.x(0)
     qc.measure(0, 0)
 
     print(test_qiskit_backend.run(qc, 2000))
     # status = test_qiskit_backend.ping()
-    assert str(test_qiskit_backend.run(qc, 2000)) == "{'1': 2000}"
+    assert str(test_qiskit_backend.run(qc, 2000)) == "{'1': 2000}"
```

### Comparing `qrisp-0.4.4/tests/test_qompiler.py` & `qrisp-0.4.5/tests/test_qompiler.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_quantum_arithmetic.py` & `qrisp-0.4.5/tests/test_quantum_arithmetic.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_quantum_dictionary.py` & `qrisp-0.4.5/tests/test_quantum_dictionary.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_quantum_division.py` & `qrisp-0.4.5/tests/test_quantum_division.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_sc_gidney_adder.py` & `qrisp-0.4.5/tests/test_sc_gidney_adder.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_state_preparation.py` & `qrisp-0.4.5/tests/test_state_preparation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_string_test.py` & `qrisp-0.4.5/tests/test_string_test.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_sudoku.py` & `qrisp-0.4.5/tests/test_sudoku.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_tket_converter.py` & `qrisp-0.4.5/tests/test_tket_converter.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_uncomputation_example.py` & `qrisp-0.4.5/tests/test_uncomputation_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/test_unitary_calculation.py` & `qrisp-0.4.5/tests/test_unitary_calculation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.4.4/tests/tests_doc_examples.py` & `qrisp-0.4.5/tests/tests_doc_examples.py`

 * *Files identical despite different names*

