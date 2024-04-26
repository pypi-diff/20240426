# Comparing `tmp/dynareadout-24.3.tar.gz` & `tmp/dynareadout-24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynareadout-24.3.tar", last modified: Thu Mar 28 15:19:58 2024, max compression
+gzip compressed data, was "dynareadout-24.4.tar", last modified: Fri Apr 26 06:43:47 2024, max compression
```

## Comparing `dynareadout-24.3.tar` & `dynareadout-24.4.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:58.429347 dynareadout-24.3/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-28 15:19:45.000000 dynareadout-24.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-28 15:19:45.000000 dynareadout-24.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-03-28 15:19:58.429347 dynareadout-24.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-03-28 15:19:45.000000 dynareadout-24.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:58.413347 dynareadout-24.3/dynareadout.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-03-28 15:19:58.000000 dynareadout-24.3/dynareadout.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-03-28 15:19:58.000000 dynareadout-24.3/dynareadout.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 15:19:58.000000 dynareadout-24.3/dynareadout.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 15:19:58.000000 dynareadout-24.3/dynareadout.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-28 15:19:58.000000 dynareadout-24.3/dynareadout.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:58.413347 dynareadout-24.3/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:58.413347 dynareadout-24.3/lib/dynareadout/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:58.421347 dynareadout-24.3/lib/dynareadout/src/
--rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/binary_search.c
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/binary_search.h
--rw-r--r--   0 runner    (1001) docker     (127)    25475 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/binout.c
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/binout.h
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/binout_defines.h
--rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/binout_directory.c
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/binout_directory.h
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/binout_glob.c
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/binout_glob.h
--rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/binout_read.c
--rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/binout_read.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:58.421347 dynareadout-24.3/lib/dynareadout/src/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/cpp/array.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/cpp/binout.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/cpp/binout.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18885 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/cpp/d3plot.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/cpp/d3plot.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/cpp/d3plot_part.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/cpp/d3plot_part.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/cpp/d3plot_state.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/cpp/d3plot_state.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/cpp/filesystem_bridge.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/cpp/include_transform.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/cpp/include_transform.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/cpp/key.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    17854 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/cpp/key.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/cpp/vec.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    24726 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/d3_buffer.c
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/d3_buffer.h
--rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/d3_defines.h
--rw-r--r--   0 runner    (1001) docker     (127)   108881 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/d3plot.c
--rw-r--r--   0 runner    (1001) docker     (127)    20876 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/d3plot.h
--rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/d3plot_data.c
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/d3plot_error_macros.h
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/d3plot_part_nodes.c
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/d3plot_part_nodes.h
--rw-r--r--   0 runner    (1001) docker     (127)    15769 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/d3plot_state.c
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/extra_string.c
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/extra_string.h
--rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/include_transform.c
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/include_transform.h
--rw-r--r--   0 runner    (1001) docker     (127)    45357 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/key.c
--rw-r--r--   0 runner    (1001) docker     (127)    12336 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/key.h
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/line.c
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/line.h
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/multi_file.c
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/multi_file.h
--rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/path.c
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/path.h
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/path_view.c
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/path_view.h
--rw-r--r--   0 runner    (1001) docker     (127)    24817 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/pgni.h
--rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/profiling.c
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/profiling.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:58.425347 dynareadout-24.3/lib/dynareadout/src/python/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/python/abi-suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)    19234 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/python/conversions.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/python/pybind11_binout.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    23473 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/python/pybind11_d3plot.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/python/pybind11_key.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/python/pybind11_module.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/python/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/string_builder.c
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/string_builder.h
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/sync.c
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-03-28 15:19:47.000000 dynareadout-24.3/lib/dynareadout/src/sync.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:58.425347 dynareadout-24.3/lib/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:58.413347 dynareadout-24.3/lib/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:58.425347 dynareadout-24.3/lib/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)    24334 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (127)    67312 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:58.429347 dynareadout-24.3/lib/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (127)    28518 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (127)    53480 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (127)    17859 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (127)    28221 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (127)    48364 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:58.429347 dynareadout-24.3/lib/pybind11/include/pybind11/eigen/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/eigen/common.h
--rw-r--r--   0 runner    (1001) docker     (127)    32135 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    18442 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (127)    13459 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (127)    79725 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (127)   126706 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (127)    98455 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:58.429347 dynareadout-24.3/lib/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (127)    15477 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (127)    29897 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-28 15:19:49.000000 dynareadout-24.3/lib/pybind11/include/pybind11/type_caster_pyobject_ptr.h
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-28 15:19:45.000000 dynareadout-24.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 15:19:58.429347 dynareadout-24.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-03-28 15:19:45.000000 dynareadout-24.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:43:47.845458 dynareadout-24.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-26 06:43:43.000000 dynareadout-24.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-26 06:43:43.000000 dynareadout-24.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-04-26 06:43:47.845458 dynareadout-24.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-26 06:43:43.000000 dynareadout-24.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:43:47.833458 dynareadout-24.4/dynareadout.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-04-26 06:43:47.000000 dynareadout-24.4/dynareadout.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-26 06:43:47.000000 dynareadout-24.4/dynareadout.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 06:43:47.000000 dynareadout-24.4/dynareadout.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 06:43:47.000000 dynareadout-24.4/dynareadout.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 06:43:47.000000 dynareadout-24.4/dynareadout.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:43:47.829458 dynareadout-24.4/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:43:47.829458 dynareadout-24.4/lib/dynareadout/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:43:47.837458 dynareadout-24.4/lib/dynareadout/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/binary_search.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/binary_search.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25475 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/binout.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/binout.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/binout_defines.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/binout_directory.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/binout_directory.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/binout_glob.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/binout_glob.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/binout_read.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/binout_read.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:43:47.841458 dynareadout-24.4/lib/dynareadout/src/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/cpp/array.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/cpp/binout.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/cpp/binout.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18885 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/cpp/d3plot.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/cpp/d3plot.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/cpp/d3plot_part.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/cpp/d3plot_part.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/cpp/d3plot_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/cpp/d3plot_state.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/cpp/filesystem_bridge.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/cpp/include_transform.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/cpp/include_transform.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/cpp/key.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18578 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/cpp/key.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/cpp/vec.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24726 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/d3_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/d3_buffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/d3_defines.h
+-rw-r--r--   0 runner    (1001) docker     (127)   108881 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/d3plot.c
+-rw-r--r--   0 runner    (1001) docker     (127)    20876 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/d3plot.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/d3plot_data.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/d3plot_error_macros.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/d3plot_part_nodes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/d3plot_part_nodes.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15769 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/d3plot_state.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/extra_string.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/extra_string.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/include_transform.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/include_transform.h
+-rw-r--r--   0 runner    (1001) docker     (127)    46191 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/key.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12865 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/key.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/line.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/line.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/multi_file.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/multi_file.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/path.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/path.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/path_view.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/path_view.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24817 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/pgni.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/profiling.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/profiling.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:43:47.841458 dynareadout-24.4/lib/dynareadout/src/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/python/abi-suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19234 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/python/conversions.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/python/pybind11_binout.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23473 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/python/pybind11_d3plot.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/python/pybind11_key.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/python/pybind11_module.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/python/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/string_builder.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/string_builder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/sync.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-26 06:43:44.000000 dynareadout-24.4/lib/dynareadout/src/sync.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:43:47.841458 dynareadout-24.4/lib/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:43:47.829458 dynareadout-24.4/lib/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:43:47.845458 dynareadout-24.4/lib/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)    24334 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (127)    67312 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:43:47.845458 dynareadout-24.4/lib/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)    28518 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (127)    53480 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17859 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28221 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (127)    48364 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:43:47.845458 dynareadout-24.4/lib/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/eigen/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32135 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18442 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13459 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (127)    79725 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (127)   126706 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (127)    98455 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:43:47.845458 dynareadout-24.4/lib/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15477 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29897 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-26 06:43:45.000000 dynareadout-24.4/lib/pybind11/include/pybind11/type_caster_pyobject_ptr.h
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-26 06:43:43.000000 dynareadout-24.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 06:43:47.845458 dynareadout-24.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-26 06:43:43.000000 dynareadout-24.4/setup.py
```

### Comparing `dynareadout-24.3/LICENSE` & `dynareadout-24.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/PKG-INFO` & `dynareadout-24.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynareadout
-Version: 24.3
+Version: 24.4
 Summary: High-Performance and Thread-Safe library for parsing binary output files and key files of LS Dyna (d3plot, binout, input deck)
 Author-email: PucklaJ <jonaas.pucher000000@gmail.com>
 Project-URL: Homepage, https://github.com/PucklaJ/dynareadout
 Project-URL: Bug Trackers, https://github.com/PucklaJ/dynareadout/issues
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: zlib/libpng License
```

### Comparing `dynareadout-24.3/README.md` & `dynareadout-24.4/README.md`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/dynareadout.egg-info/PKG-INFO` & `dynareadout-24.4/dynareadout.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynareadout
-Version: 24.3
+Version: 24.4
 Summary: High-Performance and Thread-Safe library for parsing binary output files and key files of LS Dyna (d3plot, binout, input deck)
 Author-email: PucklaJ <jonaas.pucher000000@gmail.com>
 Project-URL: Homepage, https://github.com/PucklaJ/dynareadout
 Project-URL: Bug Trackers, https://github.com/PucklaJ/dynareadout/issues
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: zlib/libpng License
```

### Comparing `dynareadout-24.3/dynareadout.egg-info/SOURCES.txt` & `dynareadout-24.4/dynareadout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/binary_search.c` & `dynareadout-24.4/lib/dynareadout/src/binary_search.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/binary_search.h` & `dynareadout-24.4/lib/dynareadout/src/binary_search.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/binout.c` & `dynareadout-24.4/lib/dynareadout/src/binout.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/binout.h` & `dynareadout-24.4/lib/dynareadout/src/binout.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/binout_defines.h` & `dynareadout-24.4/lib/dynareadout/src/binout_defines.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/binout_directory.c` & `dynareadout-24.4/lib/dynareadout/src/binout_directory.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/binout_directory.h` & `dynareadout-24.4/lib/dynareadout/src/binout_directory.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/binout_glob.c` & `dynareadout-24.4/lib/dynareadout/src/binout_glob.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/binout_glob.h` & `dynareadout-24.4/lib/dynareadout/src/binout_glob.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/binout_read.c` & `dynareadout-24.4/lib/dynareadout/src/binout_read.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/binout_read.h` & `dynareadout-24.4/lib/dynareadout/src/binout_read.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/cpp/array.hpp` & `dynareadout-24.4/lib/dynareadout/src/cpp/array.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/cpp/binout.cpp` & `dynareadout-24.4/lib/dynareadout/src/cpp/binout.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/cpp/binout.hpp` & `dynareadout-24.4/lib/dynareadout/src/cpp/binout.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/cpp/d3plot.cpp` & `dynareadout-24.4/lib/dynareadout/src/cpp/d3plot.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/cpp/d3plot.hpp` & `dynareadout-24.4/lib/dynareadout/src/cpp/d3plot.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/cpp/d3plot_part.cpp` & `dynareadout-24.4/lib/dynareadout/src/cpp/d3plot_part.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/cpp/d3plot_part.hpp` & `dynareadout-24.4/lib/dynareadout/src/cpp/d3plot_part.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/cpp/d3plot_state.cpp` & `dynareadout-24.4/lib/dynareadout/src/cpp/d3plot_state.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/cpp/d3plot_state.hpp` & `dynareadout-24.4/lib/dynareadout/src/cpp/d3plot_state.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/cpp/filesystem_bridge.hpp` & `dynareadout-24.4/lib/dynareadout/src/cpp/filesystem_bridge.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/cpp/include_transform.cpp` & `dynareadout-24.4/lib/dynareadout/src/cpp/include_transform.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/cpp/include_transform.hpp` & `dynareadout-24.4/lib/dynareadout/src/cpp/include_transform.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/cpp/key.cpp` & `dynareadout-24.4/lib/dynareadout/src/cpp/key.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -75,14 +75,22 @@
 
 void Card::next(uint8_t value_width) noexcept {
   card_parse_next_width(m_handle, value_width);
 }
 
 bool Card::done() const noexcept { return card_parse_done(m_handle) != 0; }
 
+bool Card::is_empty() const noexcept {
+  return card_parse_is_empty(m_handle) != 0;
+}
+
+bool Card::is_empty(uint8_t value_width) const noexcept {
+  return card_parse_is_empty_width(m_handle, value_width) != 0;
+}
+
 card_parse_type Card::parse_get_type() const noexcept {
   return card_parse_get_type(m_handle);
 }
 
 card_parse_type Card::parse_get_type(uint8_t value_width) const noexcept {
   return card_parse_get_type_width(m_handle, value_width);
 }
```

### Comparing `dynareadout-24.3/lib/dynareadout/src/cpp/key.hpp` & `dynareadout-24.4/lib/dynareadout/src/cpp/key.hpp`

 * *Files 15% similar despite different names*

```diff
@@ -68,14 +68,22 @@
   // Advance to the next value. Uses the value width from begin
   void next() noexcept;
   // Advance to the next value. Uses the value width provided here
   void next(uint8_t value_width) noexcept;
   // Returns wether the card has been completely parsed. Breaks if incorrect
   // value widths have been supplied
   bool done() const noexcept;
+  // Returns wether the currently value the shall be parsed is empty (i.e.
+  // consists only of whitespace). Uses the value_width provided at begin. If
+  // the card is done this also returns true*/
+  bool is_empty() const noexcept;
+  // Returns wether the currently value the shall be parsed is empty (i.e.
+  // consists only of whitespace). Uses the value_width provided here. If
+  // the card is done this also returns true*/
+  bool is_empty(uint8_t value_width) const noexcept;
   // Returns the type of the current value. Uses the value width from
   // begin. If CARD_PARSE_INT is returned the value can be parsed with an
   // integer type. If CARD_PARSE_FLOAT is returned the value can be parsed with
   // a floating point type. Else the value can only be parsed with a string
   // type.
   card_parse_type parse_get_type() const noexcept;
   // Returns the type of the current value. Uses the value width provided here.
@@ -355,14 +363,33 @@
 };
 
 template <typename T> constexpr bool is_string_v = false;
 template <typename T>
 static constexpr bool is_number_v =
     std::is_integral_v<T> || std::is_floating_point_v<T>;
 
+template <typename T> inline T empty_value_v = {0};
+template <> inline std::string empty_value_v<std::string> = "";
+template <>
+inline auto empty_value_v<dro::String> = dro::String(const_cast<char *>(""),
+                                                     false);
+template <>
+inline auto empty_value_v<dro::SizedString> =
+    dro::SizedString(const_cast<char *>(""), 0, false);
+
+template <typename T> inline T empty_value() noexcept {
+  if constexpr (std::is_same_v<char *, T>) {
+    char *v = static_cast<char *>(malloc(1));
+    *v = '\0';
+    return v;
+  } else {
+    return empty_value_v<T>;
+  }
+}
+
 template <typename T> T Card::parse() const {
   return parse<T>(m_handle->value_width);
 }
 
 template <typename T> T Card::parse(uint8_t value_width) const {
   if constexpr (std::is_integral_v<T>) {
     const auto value = card_parse_int_width(m_handle, value_width);
@@ -424,32 +451,27 @@
 
 template <typename T> T Card::parse_string_no_trim() const noexcept {
   return parse_string_no_trim<T>(m_handle->value_width);
 }
 
 template <typename... T> void Card::parse_whole(T &...rv) {
 
-  int i = 0;
-
   begin();
 
   (
       [&] {
         using parse_type = std::remove_reference_t<decltype(rv)>;
 
-        if (done()) {
-          THROW_KEY_FILE_EXCEPTION(
-              "Trying to parse %d values out of card \"%s\" with width %d",
-              i + 1, m_handle->string, DEFAULT_VALUE_WIDTH);
+        if (is_empty()) {
+          rv = empty_value<parse_type>();
+        } else {
+          rv = parse<parse_type>();
         }
 
-        rv = parse<parse_type>();
-
         next();
-        i++;
       }(),
       ...);
 }
 
 template <typename... T>
 void Card::parse_whole_width(std::array<uint8_t, sizeof...(T)> value_widths,
                              T &...rv) {
@@ -457,75 +479,67 @@
 
   begin();
 
   (
       [&] {
         using parse_type = std::remove_reference_t<decltype(rv)>;
 
-        if (done()) {
-          THROW_KEY_FILE_EXCEPTION("Trying to parse %d values out of card "
-                                   "\"%s\"",
-                                   i + 1, m_handle->string);
-        }
-
         if (value_widths[i] == 0) {
           value_widths[i] = DEFAULT_VALUE_WIDTH;
         }
 
-        rv = parse<parse_type>(value_widths[i]);
+        if (is_empty(value_widths[i])) {
+          rv = empty_value<parse_type>();
+        } else {
+          rv = parse<parse_type>(value_widths[i]);
+        }
 
         next(value_widths[i]);
         i++;
       }(),
       ...);
 }
 
 template <typename... T> std::tuple<T...> Card::parse_whole() {
-  int i = 0;
   begin();
 
   std::tuple<T...> t = {([&] {
-    if (done()) {
-      THROW_KEY_FILE_EXCEPTION(
-          "Trying to parse %d values out of card \"%s\" with width %d", i + 1,
-          m_handle->string, DEFAULT_VALUE_WIDTH);
+    if (is_empty()) {
+      auto value = empty_value<T>();
+      next();
+      return value;
+    } else {
+      auto value = parse<T>();
+      next();
+      return value;
     }
-
-    T value = parse<T>();
-
-    next();
-    i++;
-
-    return value;
   }())...};
 
   return t;
 }
 
 template <typename... T>
 std::tuple<T...>
 Card::parse_whole(std::array<uint8_t, sizeof...(T)> value_widths) {
   int i = 0;
   begin();
 
   std::tuple<T...> t = {([&] {
-    if (done()) {
-      THROW_KEY_FILE_EXCEPTION(
-          "Trying to parse %d values out of card \"%s\" with width %d", i + 1,
-          m_handle->string, DEFAULT_VALUE_WIDTH);
-    }
-
     if (value_widths[i] == 0) {
       value_widths[i] = DEFAULT_VALUE_WIDTH;
     }
 
-    T value = parse<T>(value_widths[i]);
-
-    next(value_widths[i++]);
-
-    return value;
+    if (is_empty(value_widths[i])) {
+      auto value = empty_value<T>();
+      next(value_widths[i++]);
+      return value;
+    } else {
+      auto value = parse<T>(value_widths[i]);
+      next(value_widths[i++]);
+      return value;
+    }
   }())...};
 
   return t;
 }
 
 } // namespace dro
```

### Comparing `dynareadout-24.3/lib/dynareadout/src/cpp/vec.hpp` & `dynareadout-24.4/lib/dynareadout/src/cpp/vec.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/d3_buffer.c` & `dynareadout-24.4/lib/dynareadout/src/d3_buffer.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/d3_buffer.h` & `dynareadout-24.4/lib/dynareadout/src/d3_buffer.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/d3_defines.h` & `dynareadout-24.4/lib/dynareadout/src/d3_defines.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/d3plot.c` & `dynareadout-24.4/lib/dynareadout/src/d3plot.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/d3plot.h` & `dynareadout-24.4/lib/dynareadout/src/d3plot.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/d3plot_data.c` & `dynareadout-24.4/lib/dynareadout/src/d3plot_data.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/d3plot_error_macros.h` & `dynareadout-24.4/lib/dynareadout/src/d3plot_error_macros.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/d3plot_part_nodes.c` & `dynareadout-24.4/lib/dynareadout/src/d3plot_part_nodes.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/d3plot_part_nodes.h` & `dynareadout-24.4/lib/dynareadout/src/d3plot_part_nodes.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/d3plot_state.c` & `dynareadout-24.4/lib/dynareadout/src/d3plot_state.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/extra_string.c` & `dynareadout-24.4/lib/dynareadout/src/extra_string.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/extra_string.h` & `dynareadout-24.4/lib/dynareadout/src/extra_string.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/include_transform.c` & `dynareadout-24.4/lib/dynareadout/src/include_transform.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/include_transform.h` & `dynareadout-24.4/lib/dynareadout/src/include_transform.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/key.c` & `dynareadout-24.4/lib/dynareadout/src/key.c`

 * *Files 2% similar despite different names*

```diff
@@ -811,23 +811,31 @@
 
   END_PROFILE_FUNC();
 }
 
 void card_parse_next(card_t *card) {
   BEGIN_PROFILE_FUNC();
 
-  card->current_index += card->value_width;
+  card_parse_next_width(card, card->value_width);
 
   END_PROFILE_FUNC();
 }
 
 void card_parse_next_width(card_t *card, uint8_t value_width) {
   BEGIN_PROFILE_FUNC();
 
-  card->current_index += value_width;
+  if (card->string[card->current_index] != '\0') {
+    if (card->current_index <= 255 - value_width) {
+      card->current_index += value_width;
+    } else {
+      while (card->string[card->current_index] != '\0') {
+        card->current_index++;
+      }
+    }
+  }
 
   END_PROFILE_FUNC();
 }
 
 int card_parse_done(const card_t *card) {
   BEGIN_PROFILE_FUNC();
 
@@ -1517,14 +1525,45 @@
     }
   }
 
   END_PROFILE_FUNC();
   return CARD_PARSE_STRING;
 }
 
+int card_parse_is_empty(const card_t *card) {
+  BEGIN_PROFILE_FUNC();
+
+  const int rv = card_parse_is_empty_width(card, card->value_width);
+
+  END_PROFILE_FUNC();
+  return rv;
+}
+
+int card_parse_is_empty_width(const card_t *card, uint8_t value_width) {
+  BEGIN_PROFILE_FUNC();
+
+  uint8_t i = card->current_index;
+  while (i - card->current_index < value_width) {
+    if (card->string[i] == '\0') {
+      break;
+    }
+
+    /* TODO: Handle other whitespace characters*/
+    if (card->string[i] != ' ') {
+      END_PROFILE_FUNC();
+      return 0;
+    }
+
+    i++;
+  }
+
+  END_PROFILE_FUNC();
+  return 1;
+}
+
 void _card_cpy(const card_t *card, char *dst, size_t len) {
   BEGIN_PROFILE_FUNC();
 
   memcpy(dst, card->string, len);
 
   END_PROFILE_FUNC();
 }
```

### Comparing `dynareadout-24.3/lib/dynareadout/src/key.h` & `dynareadout-24.4/lib/dynareadout/src/key.h`

 * *Files 6% similar despite different names*

```diff
@@ -226,14 +226,22 @@
 /* Returns the type of the current value. Uses the value width from
  * card_parse_begin. If CARD_PARSE_INT is returned the card_parse_int functions
  * can parse it. If CARD_PARSE_FLOAT is returned the card_parse_float functions
  * can parse it. Else only the card_parse_string functions can parse it. Uses
  * the value width provided here.*/
 card_parse_type card_parse_get_type_width(const card_t *card,
                                           uint8_t value_width);
+/* Returns wether the currently value the shall be parsed is empty (i.e.
+ * consists only of whitespace). Uses the value_width provided at begin. If the
+ * card is done this also returns non zero (i.e. true)*/
+int card_parse_is_empty(const card_t *card);
+/* Returns wether the currently value the shall be parsed is empty (i.e.
+ * consists only of whitespace). Uses the value_width provided here. If the card
+ * is done this also returns zero (i.e. true)*/
+int card_parse_is_empty_width(const card_t *card, uint8_t value_width);
 
 /* ----- Private Functions -----*/
 /* Copy the contents of the card as a string directly into dst.*/
 void _card_cpy(const card_t *card, char *dst, size_t len);
 /* Handles the parsing of multi line string for include file names. Returns
  * wether the multi line string has been completely parsed.*/
 int _parse_multi_line_string(string_builder_t *multi_line_string,
```

### Comparing `dynareadout-24.3/lib/dynareadout/src/line.c` & `dynareadout-24.4/lib/dynareadout/src/line.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/line.h` & `dynareadout-24.4/lib/dynareadout/src/line.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/multi_file.c` & `dynareadout-24.4/lib/dynareadout/src/multi_file.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/multi_file.h` & `dynareadout-24.4/lib/dynareadout/src/multi_file.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/path.c` & `dynareadout-24.4/lib/dynareadout/src/path.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/path.h` & `dynareadout-24.4/lib/dynareadout/src/path.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/path_view.c` & `dynareadout-24.4/lib/dynareadout/src/path_view.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/path_view.h` & `dynareadout-24.4/lib/dynareadout/src/path_view.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/pgni.h` & `dynareadout-24.4/lib/dynareadout/src/pgni.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/profiling.c` & `dynareadout-24.4/lib/dynareadout/src/profiling.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/profiling.h` & `dynareadout-24.4/lib/dynareadout/src/profiling.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/python/conversions.hpp` & `dynareadout-24.4/lib/dynareadout/src/python/conversions.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/python/pybind11_binout.cpp` & `dynareadout-24.4/lib/dynareadout/src/python/pybind11_binout.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/python/pybind11_d3plot.cpp` & `dynareadout-24.4/lib/dynareadout/src/python/pybind11_d3plot.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/python/pybind11_key.cpp` & `dynareadout-24.4/lib/dynareadout/src/python/pybind11_key.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -37,49 +37,100 @@
 
 py::list python_card_parse_whole(dro::Card &self, py::list value_widths) {
   self.begin();
 
   py::list rv;
   int i = 0;
 
-  while ((value_widths.empty() && !self.done()) ||
-         (!value_widths.empty() && i < value_widths.size())) {
+  for (int i = 0;
+       (value_widths.empty() && !self.done()) || i < value_widths.size(); i++) {
     uint8_t value_width;
     if (value_widths.empty()) {
       value_width = DEFAULT_VALUE_WIDTH;
     } else {
-      if (self.done()) {
-        dro::String card_string =
-            self.parse_string_whole_no_trim<dro::String>();
-
-        THROW_KEY_FILE_EXCEPTION(
-            "Trying to parse %d values out of card \"%s\" with", i + 1,
-            card_string.data());
+      value_width = value_widths[i].cast<uint8_t>();
+    }
+
+    if (self.is_empty(value_width)) {
+      rv.append(py::none());
+    } else {
+      switch (self.parse_get_type(value_width)) {
+      case CARD_PARSE_INT:
+        rv.append(self.parse<int64_t>(value_width));
+        break;
+      case CARD_PARSE_FLOAT:
+        rv.append(self.parse<double>(value_width));
+        break;
+      case CARD_PARSE_STRING:
+        rv.append(self.parse<dro::String>(value_width));
+        break;
       }
+    }
 
-      value_width = value_widths[i].cast<uint8_t>();
+    self.next(value_width);
+  }
+
+  return rv;
+}
+
+#ifdef __APPLE__
+#define RDRT(val) read_return(std::move(val))
+template <typename T> inline py::object read_return(T arr) noexcept {
+  return py::cast(std::move(arr));
+}
+
+py::object
+#else
+#define RDRT(val) (val)
+
+std::variant<int64_t, double, dro::String, py::none>
+#endif
+python_card_parse(dro::Card &self, bool trim_string, py::object value_width) {
+  if (value_width.is_none()) {
+    if (self.is_empty()) {
+      return py::none();
     }
 
-    switch (self.parse_get_type(value_width)) {
+    const auto ty = self.parse_get_type();
+
+    switch (ty) {
     case CARD_PARSE_INT:
-      rv.append(self.parse<int64_t>(value_width));
-      break;
+      return RDRT(self.parse<int64_t>());
     case CARD_PARSE_FLOAT:
-      rv.append(self.parse<double>(value_width));
-      break;
+      return RDRT(self.parse<double>());
     case CARD_PARSE_STRING:
-      rv.append(self.parse<dro::String>(value_width));
-      break;
+      if (trim_string) {
+        return RDRT(self.parse<dro::String>());
+      } else {
+        return RDRT(self.parse_string_no_trim<dro::String>());
+      }
+    }
+  } else {
+    const auto vw = value_width.cast<uint8_t>();
+    if (self.is_empty(vw)) {
+      return py::none();
     }
 
-    self.next(value_width);
-    i++;
+    const auto ty = self.parse_get_type(vw);
+
+    switch (ty) {
+    case CARD_PARSE_INT:
+      return RDRT(self.parse<int64_t>(vw));
+    case CARD_PARSE_FLOAT:
+      return RDRT(self.parse<double>(vw));
+    case CARD_PARSE_STRING:
+      if (trim_string) {
+        return RDRT(self.parse<dro::String>(vw));
+      } else {
+        return RDRT(self.parse_string_no_trim<dro::String>(vw));
+      }
+    }
   }
 
-  return rv;
+  return py::none();
 }
 
 void add_key_library_to_module(py::module_ &m) {
   py::class_<dro::Keywords>(m, "Keywords")
       .def("__len__", [](dro::Keywords &self) { return self.size(); })
       .def("__getitem__", &dro::Keywords::operator[],
            py::return_value_policy::take_ownership)
@@ -100,73 +151,127 @@
 
       ;
 
   py::class_<dro::Card>(m, "Card")
       .def("begin", &dro::Card::begin, "Initialises the parsing of the card",
            py::arg("value_width") = DEFAULT_VALUE_WIDTH)
       .def(
-          "next", [](dro::Card &self) { self.next(); },
-          "Advance to the next value. Uses the value width from begin")
+          "next",
+          [](dro::Card &self, py::object value_width) {
+            if (value_width.is_none()) {
+              self.next();
+            } else {
+              self.next(value_width.cast<uint8_t>());
+            }
+          },
+          "Advance to the next value. Uses the value width from begin",
+          py::arg("value_width") = py::none())
       .def(
           "next_width",
           [](dro::Card &self, uint8_t value_width) { self.next(value_width); },
-          "Advance to the next value. Uses the value width provided here")
+          "DEPRECATED(use Card.next) Advance to the next value. Uses the value "
+          "width provided here",
+          py::arg("value_width"))
       .def("done", &dro::Card::done,
            "Returns wether the card has been completely parsed. Breaks if "
            "incorrect value widths have been supplied")
       .def(
+          "is_empty",
+          [](dro::Card &self, py::object value_width) {
+            if (value_width.is_none()) {
+              return self.is_empty();
+            }
+
+            self.is_empty(value_width.cast<uint8_t>());
+          },
+          "Returns wether the currently value that shall be parsed is empty "
+          "(i.e. consists only of whitespace). Uses the value_width "
+          "provided here. If the card is done this also returns True",
+          py::arg("value_width") = py::none())
+      .def(
           "parse_i64",
-          [](const dro::Card &self) { return self.parse<int64_t>(); },
-          "Parses the current value as an integer. Uses the value "
-          "width from begin")
+          [](const dro::Card &self, py::object value_width) {
+            if (value_width.is_none()) {
+              return self.parse<int64_t>();
+            } else {
+              return self.parse<int64_t>(value_width.cast<uint8_t>());
+            }
+          },
+          "Parses the current value as an integer",
+          py::arg("value_width") = py::none())
       .def(
           "parse_f64",
-          [](const dro::Card &self) { return self.parse<double>(); },
-          "Parses the current value as a float. Uses the value "
-          "width from begin")
+          [](const dro::Card &self, py::object value_width) {
+            if (value_width.is_none()) {
+              return self.parse<double>();
+            } else {
+              return self.parse<double>(value_width.cast<uint8_t>());
+            }
+          },
+          "Parses the current value as a float",
+          py::arg("value_width") = py::none())
       .def(
           "parse_str",
-          [](const dro::Card &self, bool trim) {
-            if (trim)
-              return self.parse<dro::String>();
-            else
-              return self.parse_string_no_trim<dro::String>();
+          [](const dro::Card &self, bool trim, py::object value_width) {
+            if (value_width.is_none()) {
+              if (trim) {
+                return self.parse<dro::String>();
+              } else {
+                return self.parse_string_no_trim<dro::String>();
+              }
+            } else {
+              if (trim) {
+                return self.parse<dro::String>(value_width.cast<uint8_t>());
+              } else {
+                return self.parse_string_no_trim<dro::String>(
+                    value_width.cast<uint8_t>());
+              }
+            }
           },
-          "Parses the current value as a string. Uses the value "
-          "width from begin. If trim is set to True then it trims leading and "
+          "Parses the current value as a string. If trim is set to True then "
+          "it trims leading and "
           "trailing whitespace",
-          py::arg("trim") = true, py::return_value_policy::take_ownership)
+          py::arg("trim") = true, py::arg("value_width") = py::none(),
+          py::return_value_policy::take_ownership)
       .def(
           "parse_width_i64",
           [](const dro::Card &self, uint8_t value_width) {
             return self.parse<int64_t>(value_width);
           },
-          "Parses the current value as an integer. Uses the value "
+          "DEPRECATED(use Card.parse_i64) Parses the current value as an "
+          "integer. Uses the value "
           "width provided here")
       .def(
           "parse_width_f64",
           [](const dro::Card &self, uint8_t value_width) {
             return self.parse<double>(value_width);
           },
-          "Parses the current value as a float. Uses the value "
+          "DEPRECATED(use Card.parse_f64) Parses the current value as a float. "
+          "Uses the value "
           "width provided here")
       .def(
           "parse_width_str",
           [](const dro::Card &self, uint8_t value_width, bool trim) {
             if (trim)
               return self.parse<dro::String>(value_width);
             else
               return self.parse_string_no_trim<dro::String>(value_width);
           },
-          "Parses the current value as a string. Uses the value "
+          "DEPRECATED(use Card.parse_str) Parses the current value as a "
+          "string. Uses the value "
           "width provided here. If trim is set to True then it trims leading "
           "and "
           "trailing whitespace",
           py::arg("value_width"), py::arg("trim") = true,
           py::return_value_policy::take_ownership)
+      .def("parse", &python_card_parse,
+           "Parses the current value as the recognized type (if it looks like "
+           "an int its an int and so on). If the value is empty then None is "
+           "returned",
+           py::arg("trim_string") = true, py::arg("value_width") = py::none())
       .def("parse_whole", &python_card_parse_whole,
            "Parses all values of the card as the correct types. The width of "
            "each value needs to be provided as a list through value_widths",
            py::arg("value_widths") = py::list(),
            py::return_value_policy::take_ownership)
       .def("__str__", &dro::Card::parse_string_whole_no_trim<std::string>)
```

### Comparing `dynareadout-24.3/lib/dynareadout/src/python/pybind11_module.cpp` & `dynareadout-24.4/lib/dynareadout/src/python/pybind11_module.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/string_builder.c` & `dynareadout-24.4/lib/dynareadout/src/string_builder.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/string_builder.h` & `dynareadout-24.4/lib/dynareadout/src/string_builder.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/sync.c` & `dynareadout-24.4/lib/dynareadout/src/sync.c`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/dynareadout/src/sync.h` & `dynareadout-24.4/lib/dynareadout/src/sync.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/LICENSE` & `dynareadout-24.4/lib/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/attr.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/buffer_info.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/cast.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/chrono.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/complex.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/detail/class.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/detail/common.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/detail/descr.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/detail/init.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/detail/internals.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/detail/type_caster_base.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/detail/typeid.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/eigen/matrix.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/eigen/tensor.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/embed.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/eval.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/functional.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/gil.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/iostream.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/numpy.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/operators.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/options.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/pybind11.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/pytypes.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/stl/filesystem.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/stl.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/stl_bind.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/lib/pybind11/include/pybind11/type_caster_pyobject_ptr.h` & `dynareadout-24.4/lib/pybind11/include/pybind11/type_caster_pyobject_ptr.h`

 * *Files identical despite different names*

### Comparing `dynareadout-24.3/pyproject.toml` & `dynareadout-24.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dynareadout"
-version = "24.03"
+version = "24.04"
 authors = [
   { name = "PucklaJ", email = "jonaas.pucher000000@gmail.com"},
 ]
 description = "High-Performance and Thread-Safe library for parsing binary output files and key files of LS Dyna (d3plot, binout, input deck)"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `dynareadout-24.3/setup.py` & `dynareadout-24.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,12 +76,12 @@
         os.path.join(dynareadout_dir, 'src', 'python', 'pybind11_key.cpp'),
         os.path.join(dynareadout_dir, 'src', 'python', 'pybind11_module.cpp'),
     ],
     libraries=['dynareadout_c'],
 )
 
 setup(name='dynareadout',
-      version='24.03',
+      version='24.04',
       ext_modules=[dynareadout],
       zip_safe=False,
       include_package_data=True,
       libraries=ext_libraries)
```

