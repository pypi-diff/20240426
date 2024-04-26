# Comparing `tmp/dtai-veritas-0.2.1.tar.gz` & `tmp/dtai_veritas-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtai-veritas-0.2.1.tar", last modified: Mon Mar 25 14:29:06 2024, max compression
+gzip compressed data, was "dtai_veritas-0.2.2.tar", last modified: Fri Apr 26 11:42:40 2024, max compression
```

## Comparing `dtai-veritas-0.2.1.tar` & `dtai_veritas-0.2.2.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:29:06.205865 dtai-veritas-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-25 14:29:06.205865 dtai-veritas-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:29:06.185865 dtai-veritas-0.2.1/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:29:06.185865 dtai-veritas-0.2.1/lib/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)    13003 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:29:06.185865 dtai-veritas-0.2.1/lib/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:29:06.189865 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)    24334 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (127)    68054 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:29:06.193865 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (127)    28445 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (127)    53681 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (127)    28553 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (127)    49736 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:29:06.193865 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/eigen/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/eigen/common.h
--rw-r--r--   0 runner    (1001) docker     (127)    32135 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    18442 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (127)    13459 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/gil_safe_call_once.h
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (127)    80720 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (127)   129145 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (127)    98896 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:29:06.193865 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (127)    15477 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (127)    30013 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/type_caster_pyobject_ptr.h
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/include/pybind11/typing.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:29:06.193865 dtai-veritas-0.2.1/lib/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/tools/JoinPaths.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    14798 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    10888 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     8569 2024-03-25 14:28:59.000000 dtai-veritas-0.2.1/lib/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 14:29:06.205865 dtai-veritas-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:29:06.185865 dtai-veritas-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:29:06.197865 dtai-veritas-0.2.1/src/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)    12593 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/cpp/addtree.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/cpp/addtree.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/cpp/basics.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/cpp/block_store.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/cpp/box.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/cpp/features.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/cpp/fp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    38409 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/cpp/fp_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/cpp/fp_search.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12846 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/cpp/heuristics.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/cpp/interval.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/cpp/json_io.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/cpp/json_io.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/cpp/json_io_nlohmann.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/cpp/leafiter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/cpp/tree.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18223 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/cpp/tree.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:29:06.185865 dtai-veritas-0.2.1/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:29:06.205865 dtai-veritas-0.2.1/src/python/dtai_veritas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-25 14:29:06.000000 dtai-veritas-0.2.1/src/python/dtai_veritas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-03-25 14:29:06.000000 dtai-veritas-0.2.1/src/python/dtai_veritas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 14:29:06.000000 dtai-veritas-0.2.1/src/python/dtai_veritas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 14:29:05.000000 dtai-veritas-0.2.1/src/python/dtai_veritas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-25 14:29:06.000000 dtai-veritas-0.2.1/src/python/dtai_veritas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-25 14:29:06.000000 dtai-veritas-0.2.1/src/python/dtai_veritas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:29:06.197865 dtai-veritas-0.2.1/src/python/veritas/
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/python/veritas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/python/veritas/addtree_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/python/veritas/groot.py
--rw-r--r--   0 runner    (1001) docker     (127)    22163 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/python/veritas/kantchelian.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/python/veritas/lgbm_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14953 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/python/veritas/robustness.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/python/veritas/sklearn_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/python/veritas/smt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/python/veritas/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/python/veritas/xgb_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/src/python/veritas/z3backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:29:06.201865 dtai-veritas-0.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:29:06.201865 dtai-veritas-0.2.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/data/img.npy
--rw-r--r--   0 runner    (1001) docker     (127)    11440 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/gen_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/generate_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:29:06.205865 dtai-veritas-0.2.1/tests/models/
--rw-r--r--   0 runner    (1001) docker     (127)   478522 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/models/rf-img-multiclass.json
--rw-r--r--   0 runner    (1001) docker     (127)    13834 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/models/rf_model.json
--rw-r--r--   0 runner    (1001) docker     (127)    44989 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/models/xgb-img-easy-new.json
--rw-r--r--   0 runner    (1001) docker     (127)    59797 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/models/xgb-img-easy.json
--rw-r--r--   0 runner    (1001) docker     (127)   183264 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/models/xgb-img-hard-new.json
--rw-r--r--   0 runner    (1001) docker     (127)   289996 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/models/xgb-img-hard.json
--rw-r--r--   0 runner    (1001) docker     (127)   121071 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/models/xgb-img-multiclass-multivalue.json
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/models/xgb-img-multiclass-very-easy.json
--rw-r--r--   0 runner    (1001) docker     (127)   272991 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/models/xgb-img-multiclass.json
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/models/xgb-img-very-easy-new.json
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/models/xgb-img-very-easy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/readme_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/test_groot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/test_rfmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    14381 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/test_verifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-03-25 14:28:55.000000 dtai-veritas-0.2.1/tests/test_z3backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:42:40.657445 dtai_veritas-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-26 11:42:40.657445 dtai_veritas-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:42:40.633444 dtai_veritas-0.2.2/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:42:40.637444 dtai_veritas-0.2.2/lib/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)    13003 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:42:40.633444 dtai_veritas-0.2.2/lib/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:42:40.641445 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)    24334 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (127)    68054 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:42:40.641445 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)    28445 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (127)    53681 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28553 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (127)    49736 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:42:40.641445 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/eigen/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32135 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18442 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13459 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/gil_safe_call_once.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (127)    80720 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (127)   129145 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (127)    98896 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:42:40.641445 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15477 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30013 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/type_caster_pyobject_ptr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/include/pybind11/typing.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:42:40.645444 dtai_veritas-0.2.2/lib/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/tools/JoinPaths.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    14798 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    10888 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     8569 2024-04-26 11:42:36.000000 dtai_veritas-0.2.2/lib/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 11:42:40.657445 dtai_veritas-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:42:40.633444 dtai_veritas-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:42:40.645444 dtai_veritas-0.2.2/src/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)    12798 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/cpp/addtree.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/cpp/addtree.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/cpp/basics.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/cpp/block_store.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/cpp/box.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/cpp/features.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/cpp/fp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    38409 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/cpp/fp_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/cpp/fp_search.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12846 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/cpp/heuristics.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/cpp/interval.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/cpp/json_io.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/cpp/json_io.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/cpp/json_io_nlohmann.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/cpp/leafiter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/cpp/tree.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18449 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/cpp/tree.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:42:40.633444 dtai_veritas-0.2.2/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:42:40.657445 dtai_veritas-0.2.2/src/python/dtai_veritas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-26 11:42:40.000000 dtai_veritas-0.2.2/src/python/dtai_veritas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-26 11:42:40.000000 dtai_veritas-0.2.2/src/python/dtai_veritas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:42:40.000000 dtai_veritas-0.2.2/src/python/dtai_veritas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:42:40.000000 dtai_veritas-0.2.2/src/python/dtai_veritas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 11:42:40.000000 dtai_veritas-0.2.2/src/python/dtai_veritas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 11:42:40.000000 dtai_veritas-0.2.2/src/python/dtai_veritas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:42:40.649445 dtai_veritas-0.2.2/src/python/veritas/
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/python/veritas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/python/veritas/addtree_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/python/veritas/groot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22163 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/python/veritas/kantchelian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/python/veritas/lgbm_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14953 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/python/veritas/robustness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/python/veritas/sklearn_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/python/veritas/smt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/python/veritas/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/python/veritas/xgb_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/src/python/veritas/z3backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:42:40.653445 dtai_veritas-0.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:42:40.653445 dtai_veritas-0.2.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/data/img.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    11440 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/gen_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/generate_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:42:40.657445 dtai_veritas-0.2.2/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)   478522 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/models/rf-img-multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13834 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/models/rf_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44989 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/models/xgb-img-easy-new.json
+-rw-r--r--   0 runner    (1001) docker     (127)    59797 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/models/xgb-img-easy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   183264 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/models/xgb-img-hard-new.json
+-rw-r--r--   0 runner    (1001) docker     (127)   289996 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/models/xgb-img-hard.json
+-rw-r--r--   0 runner    (1001) docker     (127)   121071 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/models/xgb-img-multiclass-multivalue.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/models/xgb-img-multiclass-very-easy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   272991 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/models/xgb-img-multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/models/xgb-img-very-easy-new.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/models/xgb-img-very-easy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/readme_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/test_groot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/test_rfmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14381 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/test_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-26 11:42:31.000000 dtai_veritas-0.2.2/tests/test_z3backend.py
```

### Comparing `dtai-veritas-0.2.1/CMakeLists.txt` & `dtai_veritas-0.2.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/LICENSE` & `dtai_veritas-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/README.md` & `dtai_veritas-0.2.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -26,14 +26,40 @@
 pip install .
 ```
 
 Veritas should work on Linux (GCC), Mac (LLVM), and Windows (MSVC). If you encounter issues, feel free to contact me or open an issue.
 
 To pull the latest updates from Github, simply `git pull` the changes and reinstall using `pip`: `pip install --force-reinstall .`.
 
+### Developer Installation
+
+```
+# clone this repository
+git clone https://github.com/laudv/veritas.git
+cd veritas
+git submodule init && git submodule update
+
+# editable install
+pip install —editable .
+
+# build manually to avoid scikit-learn issues
+mkdir manual_build && cd manual_build
+cmake -DCMAKE_BUILD_TYPE=Release ..
+cmake --build .
+
+# symlink to .so in src/python/veritas
+cd .. 
+ln -sr manual_build/veritas_core_XXX.so src/python/veritas 
+[on Mac no relative symlink: need to do ln -sf ../../../manual_build/...  ]
+```
+
+`ls -l src/python/veritas` should show symlink - if so, we're done!
+
+To recompile, just run `make -C manual_build` in veritas root.
+
 ## Example
 
 You can convert an existing ensemble using the `veritas.get_addtree` function for XGBoost, LightGBM and scikit-learn.
 
 Here's an example of a model trained by XGBoost that has been converted to Veritas' own tree ensemble representation.
 
 ```python
```

### Comparing `dtai-veritas-0.2.1/lib/pybind11/CMakeLists.txt` & `dtai_veritas-0.2.2/lib/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/attr.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/buffer_info.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/cast.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/chrono.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/complex.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/detail/class.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/detail/common.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/detail/descr.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/detail/init.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/detail/internals.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/detail/type_caster_base.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/detail/typeid.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/eigen/matrix.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/eigen/tensor.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/embed.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/eval.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/functional.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/gil.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/gil_safe_call_once.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/gil_safe_call_once.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/iostream.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/numpy.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/operators.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/options.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/pybind11.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/pytypes.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/stl/filesystem.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/stl.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/stl_bind.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/type_caster_pyobject_ptr.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/type_caster_pyobject_ptr.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/include/pybind11/typing.h` & `dtai_veritas-0.2.2/lib/pybind11/include/pybind11/typing.h`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/tools/FindCatch.cmake` & `dtai_veritas-0.2.2/lib/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/tools/FindEigen3.cmake` & `dtai_veritas-0.2.2/lib/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/tools/FindPythonLibsNew.cmake` & `dtai_veritas-0.2.2/lib/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/tools/JoinPaths.cmake` & `dtai_veritas-0.2.2/lib/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/tools/pybind11Common.cmake` & `dtai_veritas-0.2.2/lib/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/tools/pybind11NewTools.cmake` & `dtai_veritas-0.2.2/lib/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/lib/pybind11/tools/pybind11Tools.cmake` & `dtai_veritas-0.2.2/lib/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/pyproject.toml` & `dtai_veritas-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/setup.py` & `dtai_veritas-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/cpp/addtree.cpp` & `dtai_veritas-0.2.2/src/cpp/addtree.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -139,16 +139,17 @@
         throw std::runtime_error("AddTree::make_singleclass: already singleclass");
     if (this->num_leaf_values() <= c)
         throw std::runtime_error("AddTree::make_singleclass: num_leaf_values <= c");
 
     GAddTree<TreeT> new_at(1, at_type_);
 
     for (const TreeT& t : *this) {
-        if (!t.is_all_zeros(c))
+        if (!t.is_all_zeros(c)) {
             new_at.add_tree(t.make_singleclass(c));
+        }
     }
 
     new_at.base_score(0) = base_score(c);
 
     return new_at;
 }
 
@@ -198,14 +199,22 @@
     size_t c = 0;
     for (const TreeT& tree : *this)
         c += tree.num_leaves();
     return c;
 }
 
 template <typename TreeT>
+int GAddTree<TreeT>::max_depth() const {
+    int mx = 0;
+    for (const TreeT& tree : *this)
+        mx = std::max(mx, tree.max_depth(tree.root()));
+    return mx;
+}
+
+template <typename TreeT>
 typename GAddTree<TreeT>::SplitMapT
 GAddTree<TreeT>::get_splits() const {
     SplitMapT splits;
 
     // collect all the split values
     for (const TreeT& tree : *this) {
         tree.collect_split_values(tree.root(), splits);
```

### Comparing `dtai-veritas-0.2.1/src/cpp/addtree.hpp` & `dtai_veritas-0.2.2/src/cpp/addtree.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -157,14 +157,15 @@
     /** Number of leaf values */
     inline int num_leaf_values() const {
         return static_cast<int>(base_scores_.size());
     }
 
     size_t num_nodes() const;
     size_t num_leafs() const;
+    int max_depth() const;
 
     inline AddTreeType get_type() const { return at_type_; }
 
     /** Map feature -> [list of split values, sorted, unique]. */
     SplitMapT get_splits() const;
 
     /** Get the maximum feat id value that is used in the trees */
```

### Comparing `dtai-veritas-0.2.1/src/cpp/basics.hpp` & `dtai_veritas-0.2.2/src/cpp/basics.hpp`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/cpp/block_store.hpp` & `dtai_veritas-0.2.2/src/cpp/block_store.hpp`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/cpp/box.hpp` & `dtai_veritas-0.2.2/src/cpp/box.hpp`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/cpp/features.hpp` & `dtai_veritas-0.2.2/src/cpp/features.hpp`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/cpp/fp.hpp` & `dtai_veritas-0.2.2/src/cpp/fp.hpp`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/cpp/fp_search.cpp` & `dtai_veritas-0.2.2/src/cpp/fp_search.cpp`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/cpp/fp_search.hpp` & `dtai_veritas-0.2.2/src/cpp/fp_search.hpp`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/cpp/heuristics.hpp` & `dtai_veritas-0.2.2/src/cpp/heuristics.hpp`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/cpp/interval.hpp` & `dtai_veritas-0.2.2/src/cpp/interval.hpp`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/cpp/json_io.cpp` & `dtai_veritas-0.2.2/src/cpp/json_io.cpp`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/cpp/json_io.hpp` & `dtai_veritas-0.2.2/src/cpp/json_io.hpp`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/cpp/json_io_nlohmann.cpp` & `dtai_veritas-0.2.2/src/cpp/json_io_nlohmann.cpp`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/cpp/leafiter.hpp` & `dtai_veritas-0.2.2/src/cpp/leafiter.hpp`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/cpp/tree.cpp` & `dtai_veritas-0.2.2/src/cpp/tree.cpp`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/cpp/tree.hpp` & `dtai_veritas-0.2.2/src/cpp/tree.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -209,14 +209,22 @@
         while (!is_root(id)) {
             id = parent(id);
             depth++;
         }
         return depth;
     }
 
+    inline int max_depth(NodeId id, int depth = 0) const {
+        if (is_internal(id)) {
+            return 1 + std::max(max_depth(left(id)), max_depth(right(id)));
+        } else {
+            return depth;
+        }
+    }
+
     inline const SplitType& get_split(NodeId id) const {
         if (is_leaf(id)) throw std::runtime_error("get_split of leaf");
         return node(id).split();
     }
 
     inline const LeafValueType& leaf_value(NodeId id, int index) const {
         if (is_internal(id)) throw std::runtime_error("leaf_value of internal");
```

### Comparing `dtai-veritas-0.2.1/src/python/dtai_veritas.egg-info/SOURCES.txt` & `dtai_veritas-0.2.2/src/python/dtai_veritas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/python/veritas/__init__.py` & `dtai_veritas-0.2.2/src/python/veritas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         Search, \
         Solution
 
 
 
 # PACKAGE META
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 __title__ = "veritas"
 __description__ = "Versatile Verification of Tree Ensembles"
 __url__ = "https://github.com/laudv/veritas"
 __doc__ = __description__ + " <" + __url__ + ">"
 
 __author__ = "Laurens Devos"
 __email__ = ""
@@ -46,28 +46,28 @@
 
 
 def __interval_hash(self):
     return hash((self.lo, self.hi))
 
 setattr(Interval, "hash", __interval_hash)
 
-def __addtree_write(self, f, compress=False):
-    if compress:
+def __addtree_write(self, f, compressed=False):
+    if compressed:
         with _gzip.open(f, "wb") as fh:
             json = self.to_json()
             fh.write(json.encode("utf-8"))
     else:
         with open(f, "w") as fh:
             fh.write(self.to_json())
 
 def __addtree_read(f, compressed=False):
     if compressed:
         with _gzip.open(f, "rb") as fh:
             json = fh.read()
-            return AddTree.from_json(json.decode("asci"))
+            return AddTree.from_json(json.decode("utf-8"))
     else:
         with open(f, "r") as fh:
             return AddTree.from_json(fh.read())
 
 def __addtree_iter(self):
     for i in range(len(self)):
         yield self[i]
```

### Comparing `dtai-veritas-0.2.1/src/python/veritas/addtree_conversion.py` & `dtai_veritas-0.2.2/src/python/veritas/addtree_conversion.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,27 +9,24 @@
 class InapplicableAddTreeConverter(Exception):
     pass
 
 class NoRegisteredConverterException(Exception):
     pass
 
 class AddTreeConverter:
-    """ AddTreeConverter Base Interface
+    """AddTreeConverter Base Interface
 
     Interface that gives the opportunity to implement a conversion from one's
     own model to Veritas' represention of tree ensembles.
 
-    The function to implement is ``get_addtree(model)``. The converter then
-    needs to be added to the convertermanager using
-    ``add_addtree_converter()``.
-
-    For an example see :ref:`Model Conversion implementation`.
+    The function to implement is ``convert(model, silent)``. The converter then
+    needs to be added to the convertermanager using ``add_addtree_converter()``.
     """
 
-    def convert(self, model):
+    def convert(self, model, silent):
         """ Convert the given model to an `AddTree`
 
         This method throws an `InapplicableAddTreeConverter` if the given model
         is not of the right type.
         """
         raise NotImplementedError()
 
@@ -40,18 +37,18 @@
 
     def add_converter(self, converter):
         assert isinstance(converter, AddTreeConverter)
 
         # Prepend to the front so this new converter takes precedence
         self._converters.insert(0, converter)
 
-    def get_addtree(self, model):
+    def get_addtree(self, model, silent):
         for converter in self._converters:
             try:
-                addtree = converter.convert(model)
+                addtree = converter.convert(model, silent)
                 assert isinstance(addtree, AddTree)
                 return addtree
             except InapplicableAddTreeConverter:
                 pass
 
         raise NoRegisteredConverterException(
                 f"No conversion possible for model of type `{type(model)}`. "
@@ -66,15 +63,15 @@
     `get_addtree` function will now also use the added converter.
 
     :param converter: Instance of AddTreeConverter
     :type converter: AddTreeConverter
     """
     _converter_registry.add_converter(converter)
 
-def get_addtree(model):
+def get_addtree(model, silent=False):
     """Convert the given model to a Veritas `AddTree`.
 
     This will try each registered `AddTreeConverter` known to Veritas. There
     are default converters for XGBoost, LightGBM, and scikit-learn random
     forests.
 
     Add your own custom converters by implementing a `veritas.AddTreeConverter`
@@ -82,17 +79,17 @@
 
     If no converter is registered for the given `model`, this function will
     throw a `NoRegisteredConverterException` exception.
 
     :param model: model that needs to be converted to a Veritas tree ensemble
     :rtype: AddTree
     """
-    return _converter_registry.get_addtree(model)
+    return _converter_registry.get_addtree(model, silent=silent)
 
-def test_conversion(at, X, ypred_model, single_rel_tol=1e-5):
+def test_conversion(at, X, ypred_model, single_rel_tol=1e-5, silent=False):
     """Test the conversion of a model to a Veritas `AddTree`
 
     Test whether the outputs of `AddTree` generated by `get_addtree` match
     the original models outputs.
     """
     try:
         import pandas as pd
@@ -113,15 +110,15 @@
                 err = np.abs((at_pred[i]-ypred_model[i]))
                 print(f"┌ example {i:<6d}  at prediction: {at_pred[i]}")
                 print(f"│              model prediction: {ypred_model[i]}")
                 print( "│               abs / rel error:",
                       f"{err} / {err/ypred_model[i]}")
                 is_correct = False
                 is_split_float_error(at, X[i, :], rel_tol)
-    else:
+    elif not silent:
         print(f"test_conversion: no problems detected (rel_tol {rel_tol:g})")
 
     return is_correct
 
 def is_split_float_error(at, x, rel_tol):
     for m, tree in enumerate(at):
         n = tree.eval_node(x)[0]
```

### Comparing `dtai-veritas-0.2.1/src/python/veritas/groot.py` & `dtai_veritas-0.2.2/src/python/veritas/groot.py`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/python/veritas/kantchelian.py` & `dtai_veritas-0.2.2/src/python/veritas/kantchelian.py`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/python/veritas/lgbm_converter.py` & `dtai_veritas-0.2.2/src/python/veritas/lgbm_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Author: Laurens Devos, Alexander Schoeters
 
 from . import AddTree, AddTreeType, AddTreeConverter
 from . import InapplicableAddTreeConverter
 import numpy as np
 
 class LGBMAddTreeConverter(AddTreeConverter):
-    def convert(self,model):
+    def convert(self, model, silent):
         try:
             from lightgbm import LGBMModel
             from lightgbm import Booster as LGBMBooster
         except ModuleNotFoundError:
             raise InapplicableAddTreeConverter("lgbm not installed")
 
         if isinstance(model, LGBMModel):
```

### Comparing `dtai-veritas-0.2.1/src/python/veritas/robustness.py` & `dtai_veritas-0.2.2/src/python/veritas/robustness.py`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/python/veritas/sklearn_converter.py` & `dtai_veritas-0.2.2/src/python/veritas/sklearn_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import numpy as np
 
 from . import AddTree, AddTreeType, AddTreeConverter
 from . import InapplicableAddTreeConverter
 
 class SklRfAddTreeConverter(AddTreeConverter):
-    def convert(self, ensemble):
+    def convert(self, ensemble, silent):
         try:
             from sklearn.ensemble import \
                     RandomForestClassifier, \
                     RandomForestRegressor
         except ModuleNotFoundError:
             raise InapplicableAddTreeConverter("no sklearn")
 
@@ -27,28 +27,30 @@
         if isinstance(ensemble, RandomForestRegressor):
             at_type = AddTreeType.REGR_MEAN 
 
             num_leaf_values = ensemble.n_outputs_ 
             def extract_value_fun(v, i):
                 return v[i][0]
 
-            print(f"SKLEARN: RF regressor with {num_leaf_values} target(s)")
+            if not silent:
+                print(f"SKLEARN: RF regressor with {num_leaf_values} target(s)")
 
         elif isinstance(ensemble, RandomForestClassifier):
             at_type = AddTreeType.CLF_MEAN
             num_leaf_values = ensemble.n_classes_ if ensemble.n_classes_ > 2 else 1 
             if num_leaf_values > 2:
                 def extract_value_fun(v, i):
                     return v[0][i]/sum(v[0])
             else:
                 def extract_value_fun(v, i):
                     assert i == 0
                     return v[0][1]/sum(v[0])
 
-            print(f"SKLEARN: RF classifier with {num_leaf_values} classes")
+            if not silent:
+                print(f"SKLEARN: RF classifier with {num_leaf_values} classes")
 
         else:
             raise InapplicableAddTreeConverter(f"not sklearn rf: {type(ensemble)}")
 
         at = AddTree(num_leaf_values, at_type)
         for tree in ensemble.estimators_:
             addtree_sklearn_tree(at, tree.tree_, extract_value_fun)
@@ -56,30 +58,31 @@
         if at_type != AddTreeType.REGR_MEAN:
             for k in range(num_leaf_values):
                 at.set_base_score(k, -len(at)/2.0)
 
         return at
 
 class SklGbdtAddTreeConverter(AddTreeConverter):
-    def convert(self, ensemble):
+    def convert(self, ensemble, silent):
         try:
             from sklearn.ensemble import \
                     GradientBoostingClassifier, \
                     GradientBoostingRegressor
         except ModuleNotFoundError:
             raise InapplicableAddTreeConverter("no sklearn")
 
         if isinstance(ensemble, GradientBoostingRegressor):
             at_type = AddTreeType.REGR
             num_leaf_values = 1
             base_scores = [ensemble.init_.constant_[0][k] for k in range(num_leaf_values)]
             def extract_value_fun(v, i):
                 return v[i][0] * ensemble.learning_rate
 
-            print(f"SKLEARN: GDBT regressor with {num_leaf_values} target(s)")
+            if not silent:
+                print(f"SKLEARN: GDBT regressor with {num_leaf_values} target(s)")
 
         elif isinstance(ensemble, GradientBoostingClassifier):
             # __import__('pprint').pprint(ensemble.__dict__)
             test_instance = np.zeros((1, ensemble.n_features_in_))
             test_instance_pred = ensemble.init_.predict_proba(test_instance)
             size_pred = test_instance_pred.shape[1]
 
@@ -91,15 +94,16 @@
                 base_scores = ensemble._loss.link.link(test_instance_pred).ravel()
 
             at_type = AddTreeType.CLF_SOFTMAX
 
             def extract_value_fun(v, i):
                 return v[i][0] * ensemble.learning_rate
 
-            print(f"SKLEARN: GDBT regressor with {num_leaf_values} target(s)")
+            if not silent:
+                print(f"SKLEARN: GDBT regressor with {num_leaf_values} target(s)")
 
         else:
             raise InapplicableAddTreeConverter(f"not sklearn gbdt: {type(ensemble)}")
 
         at = AddTree(num_leaf_values, at_type)
         for trees in ensemble.estimators_:
             for k, tree in enumerate(trees):
@@ -113,29 +117,30 @@
         for k, val in enumerate(base_scores):
             at.set_base_score(k, val)
 
         return at
 
 
 class SklTreeAddTreeConverter(AddTreeConverter):
-    def convert(self, ensemble):
+    def convert(self, ensemble, silent):
         try:
             from sklearn.tree import DecisionTreeClassifier, DecisionTreeRegressor
         except ModuleNotFoundError:
             raise InapplicableAddTreeConverter("no sklearn")
 
         if isinstance(ensemble, DecisionTreeClassifier):
             tree = ensemble
             at_type = AddTreeType.CLF_MEAN
             num_leaf_values = 1
             def extract_value_fun(v, i):
                 assert i == 0
                 return v[0][1]/sum(v[0])
 
-            print(f"SKLEARN: single tree classifier with {num_leaf_values} classes")
+            if not silent:
+                print(f"SKLEARN: single tree classifier with {num_leaf_values} classes")
 
         elif isinstance(ensemble, DecisionTreeRegressor):
             tree = ensemble
             at_type = AddTreeType.REGR_MEAN
             num_leaf_values = 1
 
             def extract_value_fun(v, i):
```

### Comparing `dtai-veritas-0.2.1/src/python/veritas/smt.py` & `dtai_veritas-0.2.2/src/python/veritas/smt.py`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/python/veritas/util.py` & `dtai_veritas-0.2.2/src/python/veritas/util.py`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/src/python/veritas/xgb_converter.py` & `dtai_veritas-0.2.2/src/python/veritas/xgb_converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy as np
 
 from . import AddTree, AddTreeType, AddTreeConverter
 from . import InapplicableAddTreeConverter
 from . import FloatT
 
 class XGBAddTreeConverter(AddTreeConverter):
-    def convert(self, model):
+    def convert(self, model, silent):
         try:
             from xgboost import XGBModel
             from xgboost.core import Booster as XGBBooster
         except ModuleNotFoundError:
             raise InapplicableAddTreeConverter("xgb not installed")
 
         if isinstance(model, XGBModel):
@@ -66,29 +66,33 @@
             convert_xgb_json_tree(at, tree_json, clazz, version)
 
         single_rel_tol = 1e-5
         rel_tol = single_rel_tol * len(at)
         base_score_manual, base_score_diff_std = try_determine_base_score(
                 model, at, feature_names)
         err = np.abs(base_score_manual-base_score)
-        print()
-        print("| XGBOOST's base_score")
-        print("|   base_score diff std     ", base_score_diff_std,
-              "(!) NOT OK" if np.any(base_score_diff_std > 1e-5) else "OK")
-        print("|   base_score reported     ", base_score)
-        print("|   versus manually detected", base_score_manual)
-        print("|   abs err                 ", err)
-        print("|   rel err                 ", err/base_score)
+
+        if not silent:
+            print()
+            print("| XGBOOST's base_score")
+            print("|   base_score diff std     ", base_score_diff_std,
+                  "(!) NOT OK" if np.any(base_score_diff_std > 1e-5) else "OK")
+            print("|   base_score reported     ", base_score)
+            print("|   versus manually detected", base_score_manual)
+            print("|   abs err                 ", err)
+            print("|   rel err                 ", err/base_score)
         if not np.all(np.isclose(base_score_manual, base_score, rtol=rel_tol)):
-            msg = "(!) base_score NOT THE SAME"
+            if not silent:
+                msg = "(!) base_score NOT THE SAME"
             base_score = base_score_manual
-        else:
+        elif not silent:
             msg = "base_score OK"
-        print(f"|   {msg} with relative tolerance {rel_tol:g}")
-        print()
+        if not silent:
+            print(f"|   {msg} with relative tolerance {rel_tol:g}")
+            print()
 
         if isinstance(base_score, float):
             base_score = np.full(num_leaf_values, base_score)
         for k in range(num_leaf_values):
             at.set_base_score(k, base_score[k])
 
         return at
```

### Comparing `dtai-veritas-0.2.1/src/python/veritas/z3backend.py` & `dtai_veritas-0.2.2/src/python/veritas/z3backend.py`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/data/img.npy` & `dtai_veritas-0.2.2/tests/data/img.npy`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/gen_models.py` & `dtai_veritas-0.2.2/tests/gen_models.py`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/generate_models.py` & `dtai_veritas-0.2.2/tests/generate_models.py`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/models/rf-img-multiclass.json` & `dtai_veritas-0.2.2/tests/models/rf-img-multiclass.json`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/models/rf_model.json` & `dtai_veritas-0.2.2/tests/models/rf_model.json`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/models/xgb-img-easy-new.json` & `dtai_veritas-0.2.2/tests/models/xgb-img-easy-new.json`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/models/xgb-img-easy.json` & `dtai_veritas-0.2.2/tests/models/xgb-img-easy.json`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/models/xgb-img-hard-new.json` & `dtai_veritas-0.2.2/tests/models/xgb-img-hard-new.json`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/models/xgb-img-hard.json` & `dtai_veritas-0.2.2/tests/models/xgb-img-hard.json`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/models/xgb-img-multiclass-multivalue.json` & `dtai_veritas-0.2.2/tests/models/xgb-img-multiclass-multivalue.json`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/models/xgb-img-multiclass-very-easy.json` & `dtai_veritas-0.2.2/tests/models/xgb-img-multiclass-very-easy.json`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/models/xgb-img-multiclass.json` & `dtai_veritas-0.2.2/tests/models/xgb-img-multiclass.json`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/models/xgb-img-very-easy-new.json` & `dtai_veritas-0.2.2/tests/models/xgb-img-very-easy-new.json`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/models/xgb-img-very-easy.json` & `dtai_veritas-0.2.2/tests/models/xgb-img-very-easy.json`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/readme_code.py` & `dtai_veritas-0.2.2/tests/readme_code.py`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/test_converters.py` & `dtai_veritas-0.2.2/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/test_groot.py` & `dtai_veritas-0.2.2/tests/test_groot.py`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/test_rfmodel.py` & `dtai_veritas-0.2.2/tests/test_rfmodel.py`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/test_search.py` & `dtai_veritas-0.2.2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/test_tree.py` & `dtai_veritas-0.2.2/tests/test_tree.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,14 +36,23 @@
         self.myAssertAlmostEqual(np.array([[1.1, -1.1], [2.2, -2.2]],
                                           dtype=FloatT), y)
 
         self.assertRaises(RuntimeError, at.compute_box, [1, 2])
         self.assertEqual(at.compute_box([1]), {1: Interval.from_hi(16.0)})
         self.assertEqual(at.compute_box([2]), {1: Interval.from_lo(16.0)})
 
+        self.assertEqual(t.depth(t.root()), 0)
+        self.assertEqual(t.depth(t["l"]), 1)
+        self.assertEqual(t.depth(t["r"]), 1)
+        self.assertEqual(at.max_depth(), 1)
+        self.assertEqual(t.max_depth(), 1)
+        self.assertEqual(t.max_depth(t["l"]), 0)
+        self.assertEqual(t.max_depth(t["r"]), 0)
+        self.assertEqual(at.max_depth(), t.depth(t["l"]))
+
     def test_boolsplit(self):
         at = AddTree(2, AddTreeType.REGR)
         t = at.add_tree()
         t.split(t.root(), 0, 2.0)
         t.split(t.left(t.root()), 1, 1.0)
         t.split(t.right(t.root()), 2)
         t.set_leaf_value(t.left(t.left(t.root())), 0, 1.0)
@@ -53,14 +62,17 @@
         t.set_leaf_value(t.left(t.left(t.root())), 1, -1.0)
         t.set_leaf_value(t.right(t.left(t.root())), 1, -2.0)
         t.set_leaf_value(t.left(t.right(t.root())), 1, -4.0)
         t.set_leaf_value(t.right(t.right(t.root())), 1, -8.0)
 
         #print(at[0])
 
+        self.assertEqual(t.max_depth(), t.depth(t["ll"]))
+        self.assertTrue(t.is_leaf(t["ll"]))
+
         self.assertEqual(t.get_split(        t.root() ), LtSplit(0, 2.0))
         self.assertEqual(t.get_split( t.left(t.root())), LtSplit(1, 1.0))
         self.assertEqual(t.get_split(t.right(t.root())), LtSplit(2, BOOL_SPLIT_VALUE))
 
         self.assertEqual(at.compute_box([5]), {0: Interval.from_lo(2.0),
                                                2: FALSE_INTERVAL})
         self.assertEqual(at.compute_box([6]), {0: Interval.from_lo(2.0),
@@ -98,15 +110,15 @@
 
         self.assertEqual(at.compute_box([2]), {1: Interval.from_lo(2.0)})
         self.assertEqual(at.compute_box([3]), {1: Interval.from_hi(2.0),
                                                2: Interval.from_hi(4.0)})
         self.assertEqual(at.compute_box([4]), {1: Interval.from_hi(2.0),
                                                2: Interval.from_lo(4.0)})
 
-        s = at.to_json();
+        s = at.to_json()
         att = AddTree.from_json(s)
         tt = att[0]
 
         self.assertTrue(tt.is_internal(0))
         self.assertTrue(tt.is_internal(1))
         self.myAssertAlmostEqual(tt.get_split(0), LtSplit(1, 2.0))
         self.myAssertAlmostEqual(tt.get_split(1), LtSplit(2, 4.0))
```

### Comparing `dtai-veritas-0.2.1/tests/test_verifier.py` & `dtai_veritas-0.2.2/tests/test_verifier.py`

 * *Files identical despite different names*

### Comparing `dtai-veritas-0.2.1/tests/test_z3backend.py` & `dtai_veritas-0.2.2/tests/test_z3backend.py`

 * *Files identical despite different names*

