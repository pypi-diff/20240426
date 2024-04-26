# Comparing `tmp/teapy-0.7.2.tar.gz` & `tmp/teapy-0.7.3.tar.gz`

## Comparing `teapy-0.7.2.tar` & `teapy-0.7.3.tar`

### file list

```diff
@@ -1,188 +1,188 @@
--rw-r--r--   0     1001      127     1583 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/Cargo.toml
--rw-r--r--   0     1001      127    15544 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/arbarray.rs
--rw-r--r--   0     1001      127    25348 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/arrok.rs
--rw-r--r--   0     1001      127    16304 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/impl_1d_method.rs
--rw-r--r--   0     1001      127     4115 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/impl_basic.rs
--rw-r--r--   0     1001      127     8421 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/impl_method.rs
--rw-r--r--   0     1001      127     8160 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/impl_numeric.rs
--rw-r--r--   0     1001      127      648 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/impl_time.rs
--rw-r--r--   0     1001      127     6070 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/impl_traits.rs
--rw-r--r--   0     1001      127      451 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/linalg/generate.rs
--rw-r--r--   0     1001      127     7390 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/linalg/layout.rs
--rw-r--r--   0     1001      127     9188 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/linalg/least_squares.rs
--rw-r--r--   0     1001      127      242 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/linalg/mod.rs
--rw-r--r--   0     1001      127     5004 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/linalg/svd.rs
--rw-r--r--   0     1001      127      436 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/linalg/utils.rs
--rw-r--r--   0     1001      127      312 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/mod.rs
--rw-r--r--   0     1001      127    10460 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/iterators.rs
--rw-r--r--   0     1001      127    14095 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/lib.rs
--rw-r--r--   0     1001      127    10802 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/macros.rs
--rw-r--r--   0     1001      127     3011 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/own.rs
--rw-r--r--   0     1001      127      721 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/prelude.rs
--rw-r--r--   0     1001      127      694 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/traits.rs
--rw-r--r--   0     1001      127     3042 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/view.rs
--rw-r--r--   0     1001      127     2031 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/viewmut.rs
--rw-r--r--   0     1001      127     1030 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-groupby/Cargo.toml
--rw-r--r--   0     1001      127     1044 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-groupby/benches/groupby.rs
--rw-r--r--   0     1001      127      613 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-groupby/src/from_py.rs
--rw-r--r--   0     1001      127     9610 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-groupby/src/groupby_agg.rs
--rw-r--r--   0     1001      127     5202 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-groupby/src/impl_lazy.rs
--rw-r--r--   0     1001      127    15347 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-groupby/src/join.rs
--rw-r--r--   0     1001      127    15380 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-groupby/src/lib.rs
--rw-r--r--   0     1001      127     7106 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-groupby/src/unique.rs
--rw-r--r--   0     1001      127      488 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-macros/Cargo.toml
--rw-r--r--   0     1001      127    14011 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-macros/src/lazy_impls.rs
--rw-r--r--   0     1001      127     1606 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-macros/src/lib.rs
--rw-r--r--   0     1001      127     6291 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-macros/src/methods_impls.rs
--rw-r--r--   0     1001      127    21958 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-macros/src/tools.rs
--rw-r--r--   0     1001      127     1303 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/Cargo.toml
--rw-r--r--   0     1001      127      483 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/benches/inplace.rs
--rw-r--r--   0     1001      127     3128 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/benches/rolling.rs
--rw-r--r--   0     1001      127     7438 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/agg/corr.rs
--rw-r--r--   0     1001      127     4196 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/agg/impl_lazy.rs
--rw-r--r--   0     1001      127    15258 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/agg/mod.rs
--rw-r--r--   0     1001      127     2200 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/create.rs
--rw-r--r--   0     1001      127     3794 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/from_py.rs
--rw-r--r--   0     1001      127      507 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/lib.rs
--rw-r--r--   0     1001      127     8740 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/linalg.rs
--rw-r--r--   0     1001      127     1993 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/macros.rs
--rw-r--r--   0     1001      127     9585 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/impl_1d.rs
--rw-r--r--   0     1001      127     8689 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/impl_arrok.rs
--rw-r--r--   0     1001      127     9095 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/impl_inplace.rs
--rw-r--r--   0     1001      127    10333 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/impl_lazy/impl_view.rs
--rw-r--r--   0     1001      127    15659 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/impl_lazy/mod.rs
--rw-r--r--   0     1001      127     2000 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/impl_lazy/stat.rs
--rw-r--r--   0     1001      127     1220 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/impl_lazy/time.rs
--rw-r--r--   0     1001      127      834 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/impl_string.rs
--rw-r--r--   0     1001      127      787 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/impl_time.rs
--rw-r--r--   0     1001      127    21550 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/mod.rs
--rw-r--r--   0     1001      127    15701 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/rolling/cmp.rs
--rw-r--r--   0     1001      127     8069 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/rolling/corr.rs
--rw-r--r--   0     1001      127    26072 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/rolling/feature.rs
--rw-r--r--   0     1001      127    22724 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/rolling/impl_lazy/common.rs
--rw-r--r--   0     1001      127      311 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/rolling/impl_lazy/mod.rs
--rw-r--r--   0     1001      127      225 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/rolling/mod.rs
--rw-r--r--   0     1001      127     9721 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/rolling/norm.rs
--rw-r--r--   0     1001      127    32087 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/rolling/reg.rs
--rw-r--r--   0     1001      127      289 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/Cargo.toml
--rw-r--r--   0     1001      127      755 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/src/convert.rs
--rw-r--r--   0     1001      127     9202 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/src/datetime.rs
--rw-r--r--   0     1001      127     2062 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/src/impls/impl_datetime.rs
--rw-r--r--   0     1001      127     2135 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/src/impls/impl_ops.rs
--rw-r--r--   0     1001      127      869 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/src/impls/impl_timedelta.rs
--rw-r--r--   0     1001      127       53 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/src/impls/mod.rs
--rw-r--r--   0     1001      127      198 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/src/lib.rs
--rw-r--r--   0     1001      127     2980 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/src/timedelta.rs
--rw-r--r--   0     1001      127      842 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/src/timeunit.rs
--rw-r--r--   0     1001      127      286 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-error/Cargo.toml
--rw-r--r--   0     1001      127     1398 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-error/src/lib.rs
--rw-r--r--   0     1001      127      271 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-utils/Cargo.toml
--rw-r--r--   0     1001      127     3666 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-utils/src/algos.rs
--rw-r--r--   0     1001      127     1798 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-utils/src/alloc.rs
--rw-r--r--   0     1001      127      231 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-utils/src/lib.rs
--rw-r--r--   0     1001      127      324 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-utils/src/macros.rs
--rw-r--r--   0     1001      127     2274 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-utils/src/traits.rs
--rw-r--r--   0     1001      127      619 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-dtype/Cargo.toml
--rw-r--r--   0     1001      127    13696 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-dtype/src/cast.rs
--rw-r--r--   0     1001      127    14632 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-dtype/src/lib.rs
--rw-r--r--   0     1001      127    12152 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-dtype/src/option_datatype.rs
--rw-r--r--   0     1001      127     2752 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-dtype/src/pyvalue.rs
--rw-r--r--   0     1001      127      463 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-hash/Cargo.toml
--rw-r--r--   0     1001      127     3243 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-hash/src/lib.rs
--rw-r--r--   0     1001      127      811 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/Cargo.toml
--rw-r--r--   0     1001      127      236 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/datadict/context.rs
--rw-r--r--   0     1001      127    23144 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/datadict/dict.rs
--rw-r--r--   0     1001      127     3254 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/datadict/get_set.rs
--rw-r--r--   0     1001      127      189 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/datadict/mod.rs
--rw-r--r--   0     1001      127     3114 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/datadict/selector.rs
--rw-r--r--   0     1001      127    11891 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/data.rs
--rw-r--r--   0     1001      127    11943 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/expr.rs
--rw-r--r--   0     1001      127     1172 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/expr_element.rs
--rw-r--r--   0     1001      127    11553 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/expr_inner.rs
--rw-r--r--   0     1001      127     6642 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/impls/auto_impl.rs
--rw-r--r--   0     1001      127     3184 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/impls/impl_cast.rs
--rw-r--r--   0     1001      127     1394 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/impls/impl_dtype_judge.rs
--rw-r--r--   0     1001      127    15326 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/impls/impl_ops.rs
--rw-r--r--   0     1001      127      889 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/impls/mod.rs
--rw-r--r--   0     1001      127     2393 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/impls/utils.rs
--rw-r--r--   0     1001      127      404 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/mod.rs
--rw-r--r--   0     1001      127    14135 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/groupby.rs
--rw-r--r--   0     1001      127    11113 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/join.rs
--rw-r--r--   0     1001      127      355 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/lib.rs
--rw-r--r--   0     1001      127     8791 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/linalg.rs
--rw-r--r--   0     1001      127      708 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-io/Cargo.toml
--rw-r--r--   0     1001      127     2062 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-io/src/arrow_io/impl_lazy.rs
--rw-r--r--   0     1001      127     5281 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-io/src/arrow_io/ipc.rs
--rw-r--r--   0     1001      127      203 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-io/src/arrow_io/mod.rs
--rw-r--r--   0     1001      127      966 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-io/src/arrow_io/utils.rs
--rw-r--r--   0     1001      127     2394 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-io/src/colselect.rs
--rw-r--r--   0     1001      127      251 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-io/src/lib.rs
--rw-r--r--   0        0        0     2069 1970-01-01 00:00:00.000000 teapy-0.7.2/tea-py/Cargo.toml
--rw-r--r--   0     1001      127        8 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/.python-version
--rw-r--r--   0     1001      127     1053 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/LICENSE
--rw-r--r--   0     1001      127     1417 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/Makefile
--rw-r--r--   0     1001      127     2202 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/README.md
--rw-r--r--   0     1001      127      232 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/build.requirements.txt
--rw-r--r--   0     1001      127     2765 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/__init__.py
--rw-r--r--   0     1001      127     4525 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/array_func.py
--rw-r--r--   0     1001      127    11351 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/expr.py
--rw-r--r--   0     1001      127     3253 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/mod_func.py
--rw-r--r--   0     1001      127    18730 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/py_datadict.py
--rw-r--r--   0     1001      127     9635 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/regression.py
--rw-r--r--   0     1001      127     7368 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/selector.py
--rw-r--r--   0     1001      127     3455 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/testing.py
--rw-r--r--   0     1001      127    12448 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/test_array_func.py
--rw-r--r--   0     1001      127     2094 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/test_common.py
--rw-r--r--   0     1001      127      967 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/test_context.py
--rw-r--r--   0     1001      127     8565 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/test_datadict.py
--rw-r--r--   0     1001      127     2303 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/test_equity.py
--rw-r--r--   0     1001      127     4772 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/test_expr.py
--rw-r--r--   0     1001      127      465 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/test_memory.py
--rw-r--r--   0     1001      127      339 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/test_time.py
--rw-r--r--   0     1001      127     3210 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/window/test_compare.py
--rw-r--r--   0     1001      127     1417 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/window/test_corr.py
--rw-r--r--   0     1001      127     5771 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/window/test_feature.py
--rw-r--r--   0     1001      127     1994 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/window/test_norm.py
--rw-r--r--   0     1001      127     3194 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/window/test_reg.py
--rw-r--r--   0     1001      127     3458 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/window_func.py
--rw-r--r--   0     1001      127     1232 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/wrapper.py
--rw-r--r--   0     1001      127     1291 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/requirements-dev.lock
--rw-r--r--   0     1001      127      197 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/requirements.lock
--rw-r--r--   0     1001      127    23237 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/equity.rs
--rw-r--r--   0     1001      127     7135 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/from_py.rs
--rw-r--r--   0     1001      127     1127 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/lib.rs
--rw-r--r--   0     1001      127    13232 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/pylazy/datadict.rs
--rw-r--r--   0     1001      127      322 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/pylazy/export.rs
--rw-r--r--   0     1001      127     2929 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/pylazy/groupby.rs
--rw-r--r--   0     1001      127    97651 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/pylazy/impl_pyexpr.rs
--rw-r--r--   0     1001      127     1898 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/pylazy/mod.rs
--rw-r--r--   0     1001      127     5443 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/pylazy/pyexpr.rs
--rw-r--r--   0     1001      127    18957 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/pylazy/pyfunc.rs
--rw-r--r--   0     1001      127     2202 2024-04-25 09:24:05.000000 teapy-0.7.2/README.md
--rw-r--r--   0     1001      127    57288 2024-04-25 09:24:21.000000 teapy-0.7.2/Cargo.lock
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 teapy-0.7.2/Cargo.toml
--rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 teapy-0.7.2/pyproject.toml
--rw-r--r--   0     1001      127     3253 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/mod_func.py
--rw-r--r--   0     1001      127     1232 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/wrapper.py
--rw-r--r--   0     1001      127    18730 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/py_datadict.py
--rw-r--r--   0     1001      127     7368 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/selector.py
--rw-r--r--   0     1001      127     2765 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/__init__.py
--rw-r--r--   0     1001      127     4525 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/array_func.py
--rw-r--r--   0     1001      127      967 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/test_context.py
--rw-r--r--   0     1001      127    12448 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/test_array_func.py
--rw-r--r--   0     1001      127     4772 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/test_expr.py
--rw-r--r--   0     1001      127     2303 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/test_equity.py
--rw-r--r--   0     1001      127     1994 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/window/test_norm.py
--rw-r--r--   0     1001      127     3194 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/window/test_reg.py
--rw-r--r--   0     1001      127     1417 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/window/test_corr.py
--rw-r--r--   0     1001      127     5771 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/window/test_feature.py
--rw-r--r--   0     1001      127     3210 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/window/test_compare.py
--rw-r--r--   0     1001      127     8565 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/test_datadict.py
--rw-r--r--   0     1001      127      339 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/test_time.py
--rw-r--r--   0     1001      127      465 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/test_memory.py
--rw-r--r--   0     1001      127     2094 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/test_common.py
--rw-r--r--   0     1001      127     3458 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/window_func.py
--rw-r--r--   0     1001      127     9635 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/regression.py
--rw-r--r--   0     1001      127     3455 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/testing.py
--rw-r--r--   0     1001      127    11351 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/expr.py
--rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 teapy-0.7.2/PKG-INFO
+-rw-r--r--   0     1001      127      708 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-io/Cargo.toml
+-rw-r--r--   0     1001      127     2062 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-io/src/arrow_io/impl_lazy.rs
+-rw-r--r--   0     1001      127     5281 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-io/src/arrow_io/ipc.rs
+-rw-r--r--   0     1001      127      203 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-io/src/arrow_io/mod.rs
+-rw-r--r--   0     1001      127      966 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-io/src/arrow_io/utils.rs
+-rw-r--r--   0     1001      127     2394 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-io/src/colselect.rs
+-rw-r--r--   0     1001      127      251 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-io/src/lib.rs
+-rw-r--r--   0     1001      127      811 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/Cargo.toml
+-rw-r--r--   0     1001      127      236 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/datadict/context.rs
+-rw-r--r--   0     1001      127    23144 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/datadict/dict.rs
+-rw-r--r--   0     1001      127     3254 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/datadict/get_set.rs
+-rw-r--r--   0     1001      127      189 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/datadict/mod.rs
+-rw-r--r--   0     1001      127     3114 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/datadict/selector.rs
+-rw-r--r--   0     1001      127    11891 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/expr_core/data.rs
+-rw-r--r--   0     1001      127    11943 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/expr_core/expr.rs
+-rw-r--r--   0     1001      127     1172 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/expr_core/expr_element.rs
+-rw-r--r--   0     1001      127    11553 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/expr_core/expr_inner.rs
+-rw-r--r--   0     1001      127     6642 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/expr_core/impls/auto_impl.rs
+-rw-r--r--   0     1001      127     3184 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/expr_core/impls/impl_cast.rs
+-rw-r--r--   0     1001      127     1394 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/expr_core/impls/impl_dtype_judge.rs
+-rw-r--r--   0     1001      127    15326 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/expr_core/impls/impl_ops.rs
+-rw-r--r--   0     1001      127      889 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/expr_core/impls/mod.rs
+-rw-r--r--   0     1001      127     2393 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/expr_core/impls/utils.rs
+-rw-r--r--   0     1001      127      404 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/expr_core/mod.rs
+-rw-r--r--   0     1001      127    14135 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/groupby.rs
+-rw-r--r--   0     1001      127    11113 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/join.rs
+-rw-r--r--   0     1001      127      355 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/lib.rs
+-rw-r--r--   0     1001      127     8791 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-lazy/src/linalg.rs
+-rw-r--r--   0     1001      127     1583 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/Cargo.toml
+-rw-r--r--   0     1001      127    15544 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/arbarray.rs
+-rw-r--r--   0     1001      127    25348 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/arrok.rs
+-rw-r--r--   0     1001      127    16304 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/impls/impl_1d_method.rs
+-rw-r--r--   0     1001      127     4115 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/impls/impl_basic.rs
+-rw-r--r--   0     1001      127     8421 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/impls/impl_method.rs
+-rw-r--r--   0     1001      127     8160 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/impls/impl_numeric.rs
+-rw-r--r--   0     1001      127      648 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/impls/impl_time.rs
+-rw-r--r--   0     1001      127     6070 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/impls/impl_traits.rs
+-rw-r--r--   0     1001      127      451 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/impls/linalg/generate.rs
+-rw-r--r--   0     1001      127     7390 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/impls/linalg/layout.rs
+-rw-r--r--   0     1001      127     9188 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/impls/linalg/least_squares.rs
+-rw-r--r--   0     1001      127      242 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/impls/linalg/mod.rs
+-rw-r--r--   0     1001      127     5004 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/impls/linalg/svd.rs
+-rw-r--r--   0     1001      127      436 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/impls/linalg/utils.rs
+-rw-r--r--   0     1001      127      312 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/impls/mod.rs
+-rw-r--r--   0     1001      127    10460 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/iterators.rs
+-rw-r--r--   0     1001      127    14095 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/lib.rs
+-rw-r--r--   0     1001      127    10802 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/macros.rs
+-rw-r--r--   0     1001      127     3011 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/own.rs
+-rw-r--r--   0     1001      127      721 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/prelude.rs
+-rw-r--r--   0     1001      127      694 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/traits.rs
+-rw-r--r--   0     1001      127     3042 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/view.rs
+-rw-r--r--   0     1001      127     2031 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-core/src/viewmut.rs
+-rw-r--r--   0     1001      127      289 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-time/Cargo.toml
+-rw-r--r--   0     1001      127      755 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-time/src/convert.rs
+-rw-r--r--   0     1001      127     9202 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-time/src/datetime.rs
+-rw-r--r--   0     1001      127     2062 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-time/src/impls/impl_datetime.rs
+-rw-r--r--   0     1001      127     2135 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-time/src/impls/impl_ops.rs
+-rw-r--r--   0     1001      127      869 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-time/src/impls/impl_timedelta.rs
+-rw-r--r--   0     1001      127       53 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-time/src/impls/mod.rs
+-rw-r--r--   0     1001      127      198 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-time/src/lib.rs
+-rw-r--r--   0     1001      127     2980 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-time/src/timedelta.rs
+-rw-r--r--   0     1001      127      842 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-time/src/timeunit.rs
+-rw-r--r--   0     1001      127      286 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-error/Cargo.toml
+-rw-r--r--   0     1001      127     1398 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-error/src/lib.rs
+-rw-r--r--   0     1001      127      619 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-dtype/Cargo.toml
+-rw-r--r--   0     1001      127    13696 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-dtype/src/cast.rs
+-rw-r--r--   0     1001      127    14632 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-dtype/src/lib.rs
+-rw-r--r--   0     1001      127    12152 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-dtype/src/option_datatype.rs
+-rw-r--r--   0     1001      127     2752 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-dtype/src/pyvalue.rs
+-rw-r--r--   0     1001      127     1303 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/Cargo.toml
+-rw-r--r--   0     1001      127      483 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/benches/inplace.rs
+-rw-r--r--   0     1001      127     3128 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/benches/rolling.rs
+-rw-r--r--   0     1001      127     7438 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/agg/corr.rs
+-rw-r--r--   0     1001      127     4196 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/agg/impl_lazy.rs
+-rw-r--r--   0     1001      127    15258 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/agg/mod.rs
+-rw-r--r--   0     1001      127     2200 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/create.rs
+-rw-r--r--   0     1001      127     3794 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/from_py.rs
+-rw-r--r--   0     1001      127      507 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/lib.rs
+-rw-r--r--   0     1001      127     8740 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/linalg.rs
+-rw-r--r--   0     1001      127     1993 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/macros.rs
+-rw-r--r--   0     1001      127     9585 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/map/impl_1d.rs
+-rw-r--r--   0     1001      127     8689 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/map/impl_arrok.rs
+-rw-r--r--   0     1001      127     9095 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/map/impl_inplace.rs
+-rw-r--r--   0     1001      127    10333 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/map/impl_lazy/impl_view.rs
+-rw-r--r--   0     1001      127    15659 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/map/impl_lazy/mod.rs
+-rw-r--r--   0     1001      127     2000 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/map/impl_lazy/stat.rs
+-rw-r--r--   0     1001      127     1220 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/map/impl_lazy/time.rs
+-rw-r--r--   0     1001      127      834 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/map/impl_string.rs
+-rw-r--r--   0     1001      127      787 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/map/impl_time.rs
+-rw-r--r--   0     1001      127    21550 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/map/mod.rs
+-rw-r--r--   0     1001      127    15701 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/rolling/cmp.rs
+-rw-r--r--   0     1001      127     8069 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/rolling/corr.rs
+-rw-r--r--   0     1001      127    26072 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/rolling/feature.rs
+-rw-r--r--   0     1001      127    22724 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/rolling/impl_lazy/common.rs
+-rw-r--r--   0     1001      127      311 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/rolling/impl_lazy/mod.rs
+-rw-r--r--   0     1001      127      225 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/rolling/mod.rs
+-rw-r--r--   0     1001      127     9721 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/rolling/norm.rs
+-rw-r--r--   0     1001      127    32087 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-ext/src/rolling/reg.rs
+-rw-r--r--   0     1001      127     1030 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-groupby/Cargo.toml
+-rw-r--r--   0     1001      127     1044 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-groupby/benches/groupby.rs
+-rw-r--r--   0     1001      127      613 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-groupby/src/from_py.rs
+-rw-r--r--   0     1001      127     9610 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-groupby/src/groupby_agg.rs
+-rw-r--r--   0     1001      127     5202 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-groupby/src/impl_lazy.rs
+-rw-r--r--   0     1001      127    15347 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-groupby/src/join.rs
+-rw-r--r--   0     1001      127    15380 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-groupby/src/lib.rs
+-rw-r--r--   0     1001      127     7106 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-groupby/src/unique.rs
+-rw-r--r--   0     1001      127      463 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-hash/Cargo.toml
+-rw-r--r--   0     1001      127     3243 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-hash/src/lib.rs
+-rw-r--r--   0     1001      127      488 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-macros/Cargo.toml
+-rw-r--r--   0     1001      127    14011 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-macros/src/lazy_impls.rs
+-rw-r--r--   0     1001      127     1606 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-macros/src/lib.rs
+-rw-r--r--   0     1001      127     6291 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-macros/src/methods_impls.rs
+-rw-r--r--   0     1001      127    21958 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-macros/src/tools.rs
+-rw-r--r--   0     1001      127      271 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-utils/Cargo.toml
+-rw-r--r--   0     1001      127     3666 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-utils/src/algos.rs
+-rw-r--r--   0     1001      127     1798 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-utils/src/alloc.rs
+-rw-r--r--   0     1001      127      231 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-utils/src/lib.rs
+-rw-r--r--   0     1001      127      324 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-utils/src/macros.rs
+-rw-r--r--   0     1001      127     2274 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-utils/src/traits.rs
+-rw-r--r--   0        0        0     2069 1970-01-01 00:00:00.000000 teapy-0.7.3/tea-py/Cargo.toml
+-rw-r--r--   0     1001      127        8 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/.python-version
+-rw-r--r--   0     1001      127     1053 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/LICENSE
+-rw-r--r--   0     1001      127     1417 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/Makefile
+-rw-r--r--   0     1001      127     2202 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/README.md
+-rw-r--r--   0     1001      127      232 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/build.requirements.txt
+-rw-r--r--   0     1001      127     2765 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/__init__.py
+-rw-r--r--   0     1001      127     4525 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/array_func.py
+-rw-r--r--   0     1001      127    11351 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/expr.py
+-rw-r--r--   0     1001      127     3253 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/mod_func.py
+-rw-r--r--   0     1001      127    18730 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/py_datadict.py
+-rw-r--r--   0     1001      127     9635 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/regression.py
+-rw-r--r--   0     1001      127     7368 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/selector.py
+-rw-r--r--   0     1001      127     3455 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/testing.py
+-rw-r--r--   0     1001      127    12448 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/tests/test_array_func.py
+-rw-r--r--   0     1001      127     2094 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/tests/test_common.py
+-rw-r--r--   0     1001      127      967 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/tests/test_context.py
+-rw-r--r--   0     1001      127     8565 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/tests/test_datadict.py
+-rw-r--r--   0     1001      127     2303 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/tests/test_equity.py
+-rw-r--r--   0     1001      127     4772 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/tests/test_expr.py
+-rw-r--r--   0     1001      127      465 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/tests/test_memory.py
+-rw-r--r--   0     1001      127      339 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/tests/test_time.py
+-rw-r--r--   0     1001      127     3210 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/tests/window/test_compare.py
+-rw-r--r--   0     1001      127     1417 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/tests/window/test_corr.py
+-rw-r--r--   0     1001      127     5771 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/tests/window/test_feature.py
+-rw-r--r--   0     1001      127     1994 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/tests/window/test_norm.py
+-rw-r--r--   0     1001      127     3194 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/tests/window/test_reg.py
+-rw-r--r--   0     1001      127     3458 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/window_func.py
+-rw-r--r--   0     1001      127     1232 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/python/teapy/wrapper.py
+-rw-r--r--   0     1001      127     1291 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/requirements-dev.lock
+-rw-r--r--   0     1001      127      197 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/requirements.lock
+-rw-r--r--   0     1001      127    23237 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/src/equity.rs
+-rw-r--r--   0     1001      127     7135 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/src/from_py.rs
+-rw-r--r--   0     1001      127     1127 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/src/lib.rs
+-rw-r--r--   0     1001      127    13232 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/src/pylazy/datadict.rs
+-rw-r--r--   0     1001      127      322 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/src/pylazy/export.rs
+-rw-r--r--   0     1001      127     2929 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/src/pylazy/groupby.rs
+-rw-r--r--   0     1001      127    97651 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/src/pylazy/impl_pyexpr.rs
+-rw-r--r--   0     1001      127     1898 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/src/pylazy/mod.rs
+-rw-r--r--   0     1001      127     5443 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/src/pylazy/pyexpr.rs
+-rw-r--r--   0     1001      127    18648 2024-04-26 13:31:54.000000 teapy-0.7.3/tea-py/src/pylazy/pyfunc.rs
+-rw-r--r--   0     1001      127     2202 2024-04-26 13:31:54.000000 teapy-0.7.3/README.md
+-rw-r--r--   0     1001      127    57324 2024-04-26 13:32:07.000000 teapy-0.7.3/Cargo.lock
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 teapy-0.7.3/Cargo.toml
+-rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 teapy-0.7.3/pyproject.toml
+-rw-r--r--   0     1001      127     3253 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/mod_func.py
+-rw-r--r--   0     1001      127     1232 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/wrapper.py
+-rw-r--r--   0     1001      127    18730 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/py_datadict.py
+-rw-r--r--   0     1001      127     7368 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/selector.py
+-rw-r--r--   0     1001      127     2765 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/__init__.py
+-rw-r--r--   0     1001      127     4525 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/array_func.py
+-rw-r--r--   0     1001      127      967 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/tests/test_context.py
+-rw-r--r--   0     1001      127    12448 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/tests/test_array_func.py
+-rw-r--r--   0     1001      127     4772 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/tests/test_expr.py
+-rw-r--r--   0     1001      127     2303 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/tests/test_equity.py
+-rw-r--r--   0     1001      127     1994 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/tests/window/test_norm.py
+-rw-r--r--   0     1001      127     3194 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/tests/window/test_reg.py
+-rw-r--r--   0     1001      127     1417 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/tests/window/test_corr.py
+-rw-r--r--   0     1001      127     5771 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/tests/window/test_feature.py
+-rw-r--r--   0     1001      127     3210 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/tests/window/test_compare.py
+-rw-r--r--   0     1001      127     8565 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/tests/test_datadict.py
+-rw-r--r--   0     1001      127      339 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/tests/test_time.py
+-rw-r--r--   0     1001      127      465 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/tests/test_memory.py
+-rw-r--r--   0     1001      127     2094 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/tests/test_common.py
+-rw-r--r--   0     1001      127     3458 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/window_func.py
+-rw-r--r--   0     1001      127     9635 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/regression.py
+-rw-r--r--   0     1001      127     3455 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/testing.py
+-rw-r--r--   0     1001      127    11351 2024-04-26 13:31:54.000000 teapy-0.7.3/python/teapy/expr.py
+-rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 teapy-0.7.3/PKG-INFO
```

### Comparing `teapy-0.7.2/tea-core/Cargo.toml` & `teapy-0.7.3/tea-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/arbarray.rs` & `teapy-0.7.3/tea-core/src/arbarray.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/arrok.rs` & `teapy-0.7.3/tea-core/src/arrok.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/impls/impl_1d_method.rs` & `teapy-0.7.3/tea-core/src/impls/impl_1d_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/impls/impl_basic.rs` & `teapy-0.7.3/tea-core/src/impls/impl_basic.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/impls/impl_method.rs` & `teapy-0.7.3/tea-core/src/impls/impl_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/impls/impl_numeric.rs` & `teapy-0.7.3/tea-core/src/impls/impl_numeric.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/impls/impl_time.rs` & `teapy-0.7.3/tea-core/src/impls/impl_time.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/impls/impl_traits.rs` & `teapy-0.7.3/tea-core/src/impls/impl_traits.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/impls/linalg/layout.rs` & `teapy-0.7.3/tea-core/src/impls/linalg/layout.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/impls/linalg/least_squares.rs` & `teapy-0.7.3/tea-core/src/impls/linalg/least_squares.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/impls/linalg/svd.rs` & `teapy-0.7.3/tea-core/src/impls/linalg/svd.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/iterators.rs` & `teapy-0.7.3/tea-core/src/iterators.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/lib.rs` & `teapy-0.7.3/tea-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/macros.rs` & `teapy-0.7.3/tea-core/src/macros.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/own.rs` & `teapy-0.7.3/tea-core/src/own.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/prelude.rs` & `teapy-0.7.3/tea-core/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/traits.rs` & `teapy-0.7.3/tea-core/src/traits.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/view.rs` & `teapy-0.7.3/tea-core/src/view.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-core/src/viewmut.rs` & `teapy-0.7.3/tea-core/src/viewmut.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-groupby/Cargo.toml` & `teapy-0.7.3/tea-groupby/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-groupby/benches/groupby.rs` & `teapy-0.7.3/tea-groupby/benches/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-groupby/src/from_py.rs` & `teapy-0.7.3/tea-groupby/src/from_py.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-groupby/src/groupby_agg.rs` & `teapy-0.7.3/tea-groupby/src/groupby_agg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-groupby/src/impl_lazy.rs` & `teapy-0.7.3/tea-groupby/src/impl_lazy.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-groupby/src/join.rs` & `teapy-0.7.3/tea-groupby/src/join.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-groupby/src/lib.rs` & `teapy-0.7.3/tea-groupby/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-groupby/src/unique.rs` & `teapy-0.7.3/tea-groupby/src/unique.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-macros/src/lazy_impls.rs` & `teapy-0.7.3/tea-macros/src/lazy_impls.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-macros/src/lib.rs` & `teapy-0.7.3/tea-macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-macros/src/methods_impls.rs` & `teapy-0.7.3/tea-macros/src/methods_impls.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-macros/src/tools.rs` & `teapy-0.7.3/tea-macros/src/tools.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/Cargo.toml` & `teapy-0.7.3/tea-ext/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/benches/rolling.rs` & `teapy-0.7.3/tea-ext/benches/rolling.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/agg/corr.rs` & `teapy-0.7.3/tea-ext/src/agg/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/agg/impl_lazy.rs` & `teapy-0.7.3/tea-ext/src/agg/impl_lazy.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/agg/mod.rs` & `teapy-0.7.3/tea-ext/src/agg/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/create.rs` & `teapy-0.7.3/tea-ext/src/create.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/from_py.rs` & `teapy-0.7.3/tea-ext/src/from_py.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/linalg.rs` & `teapy-0.7.3/tea-ext/src/linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/macros.rs` & `teapy-0.7.3/tea-ext/src/macros.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/map/impl_1d.rs` & `teapy-0.7.3/tea-ext/src/map/impl_1d.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/map/impl_arrok.rs` & `teapy-0.7.3/tea-ext/src/map/impl_arrok.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/map/impl_inplace.rs` & `teapy-0.7.3/tea-ext/src/map/impl_inplace.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/map/impl_lazy/impl_view.rs` & `teapy-0.7.3/tea-ext/src/map/impl_lazy/impl_view.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/map/impl_lazy/mod.rs` & `teapy-0.7.3/tea-ext/src/map/impl_lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/map/impl_lazy/stat.rs` & `teapy-0.7.3/tea-ext/src/map/impl_lazy/stat.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/map/impl_lazy/time.rs` & `teapy-0.7.3/tea-ext/src/map/impl_lazy/time.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/map/impl_string.rs` & `teapy-0.7.3/tea-ext/src/map/impl_string.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/map/impl_time.rs` & `teapy-0.7.3/tea-ext/src/map/impl_time.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/map/mod.rs` & `teapy-0.7.3/tea-ext/src/map/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/rolling/cmp.rs` & `teapy-0.7.3/tea-ext/src/rolling/cmp.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/rolling/corr.rs` & `teapy-0.7.3/tea-ext/src/rolling/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/rolling/feature.rs` & `teapy-0.7.3/tea-ext/src/rolling/feature.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/rolling/impl_lazy/common.rs` & `teapy-0.7.3/tea-ext/src/rolling/impl_lazy/common.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/rolling/norm.rs` & `teapy-0.7.3/tea-ext/src/rolling/norm.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-ext/src/rolling/reg.rs` & `teapy-0.7.3/tea-ext/src/rolling/reg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-time/src/convert.rs` & `teapy-0.7.3/tea-time/src/convert.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-time/src/datetime.rs` & `teapy-0.7.3/tea-time/src/datetime.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-time/src/impls/impl_datetime.rs` & `teapy-0.7.3/tea-time/src/impls/impl_datetime.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-time/src/impls/impl_ops.rs` & `teapy-0.7.3/tea-time/src/impls/impl_ops.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-time/src/impls/impl_timedelta.rs` & `teapy-0.7.3/tea-time/src/impls/impl_timedelta.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-time/src/timedelta.rs` & `teapy-0.7.3/tea-time/src/timedelta.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-time/src/timeunit.rs` & `teapy-0.7.3/tea-time/src/timeunit.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-error/src/lib.rs` & `teapy-0.7.3/tea-error/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-utils/src/algos.rs` & `teapy-0.7.3/tea-utils/src/algos.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-utils/src/alloc.rs` & `teapy-0.7.3/tea-utils/src/alloc.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-utils/src/traits.rs` & `teapy-0.7.3/tea-utils/src/traits.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-dtype/Cargo.toml` & `teapy-0.7.3/tea-dtype/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-dtype/src/cast.rs` & `teapy-0.7.3/tea-dtype/src/cast.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-dtype/src/lib.rs` & `teapy-0.7.3/tea-dtype/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-dtype/src/option_datatype.rs` & `teapy-0.7.3/tea-dtype/src/option_datatype.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-dtype/src/pyvalue.rs` & `teapy-0.7.3/tea-dtype/src/pyvalue.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-hash/src/lib.rs` & `teapy-0.7.3/tea-hash/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-lazy/Cargo.toml` & `teapy-0.7.3/tea-lazy/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-lazy/src/datadict/dict.rs` & `teapy-0.7.3/tea-lazy/src/datadict/dict.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-lazy/src/datadict/get_set.rs` & `teapy-0.7.3/tea-lazy/src/datadict/get_set.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-lazy/src/datadict/selector.rs` & `teapy-0.7.3/tea-lazy/src/datadict/selector.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-lazy/src/expr_core/data.rs` & `teapy-0.7.3/tea-lazy/src/expr_core/data.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-lazy/src/expr_core/expr.rs` & `teapy-0.7.3/tea-lazy/src/expr_core/expr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-lazy/src/expr_core/expr_element.rs` & `teapy-0.7.3/tea-lazy/src/expr_core/expr_element.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-lazy/src/expr_core/expr_inner.rs` & `teapy-0.7.3/tea-lazy/src/expr_core/expr_inner.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-lazy/src/expr_core/impls/auto_impl.rs` & `teapy-0.7.3/tea-lazy/src/expr_core/impls/auto_impl.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-lazy/src/expr_core/impls/impl_cast.rs` & `teapy-0.7.3/tea-lazy/src/expr_core/impls/impl_cast.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-lazy/src/expr_core/impls/impl_dtype_judge.rs` & `teapy-0.7.3/tea-lazy/src/expr_core/impls/impl_dtype_judge.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-lazy/src/expr_core/impls/impl_ops.rs` & `teapy-0.7.3/tea-lazy/src/expr_core/impls/impl_ops.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-lazy/src/expr_core/impls/mod.rs` & `teapy-0.7.3/tea-lazy/src/expr_core/impls/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-lazy/src/expr_core/impls/utils.rs` & `teapy-0.7.3/tea-lazy/src/expr_core/impls/utils.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-lazy/src/groupby.rs` & `teapy-0.7.3/tea-lazy/src/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-lazy/src/join.rs` & `teapy-0.7.3/tea-lazy/src/join.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-lazy/src/linalg.rs` & `teapy-0.7.3/tea-lazy/src/linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-io/Cargo.toml` & `teapy-0.7.3/tea-io/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-io/src/arrow_io/impl_lazy.rs` & `teapy-0.7.3/tea-io/src/arrow_io/impl_lazy.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-io/src/arrow_io/ipc.rs` & `teapy-0.7.3/tea-io/src/arrow_io/ipc.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-io/src/arrow_io/utils.rs` & `teapy-0.7.3/tea-io/src/arrow_io/utils.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-io/src/colselect.rs` & `teapy-0.7.3/tea-io/src/colselect.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/Cargo.toml` & `teapy-0.7.3/tea-py/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/LICENSE` & `teapy-0.7.3/tea-py/LICENSE`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/Makefile` & `teapy-0.7.3/tea-py/Makefile`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/README.md` & `teapy-0.7.3/tea-py/README.md`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/__init__.py` & `teapy-0.7.3/tea-py/python/teapy/__init__.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/array_func.py` & `teapy-0.7.3/tea-py/python/teapy/array_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/expr.py` & `teapy-0.7.3/tea-py/python/teapy/expr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/mod_func.py` & `teapy-0.7.3/tea-py/python/teapy/mod_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/py_datadict.py` & `teapy-0.7.3/tea-py/python/teapy/py_datadict.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/regression.py` & `teapy-0.7.3/tea-py/python/teapy/regression.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/selector.py` & `teapy-0.7.3/tea-py/python/teapy/selector.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/testing.py` & `teapy-0.7.3/tea-py/python/teapy/testing.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/tests/test_array_func.py` & `teapy-0.7.3/tea-py/python/teapy/tests/test_array_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/tests/test_common.py` & `teapy-0.7.3/tea-py/python/teapy/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/tests/test_context.py` & `teapy-0.7.3/tea-py/python/teapy/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/tests/test_datadict.py` & `teapy-0.7.3/tea-py/python/teapy/tests/test_datadict.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/tests/test_equity.py` & `teapy-0.7.3/tea-py/python/teapy/tests/test_equity.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/tests/test_expr.py` & `teapy-0.7.3/tea-py/python/teapy/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/tests/window/test_compare.py` & `teapy-0.7.3/tea-py/python/teapy/tests/window/test_compare.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/tests/window/test_corr.py` & `teapy-0.7.3/tea-py/python/teapy/tests/window/test_corr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/tests/window/test_feature.py` & `teapy-0.7.3/tea-py/python/teapy/tests/window/test_feature.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/tests/window/test_norm.py` & `teapy-0.7.3/tea-py/python/teapy/tests/window/test_norm.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/tests/window/test_reg.py` & `teapy-0.7.3/tea-py/python/teapy/tests/window/test_reg.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/window_func.py` & `teapy-0.7.3/tea-py/python/teapy/window_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/python/teapy/wrapper.py` & `teapy-0.7.3/tea-py/python/teapy/wrapper.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/requirements-dev.lock` & `teapy-0.7.3/tea-py/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/src/equity.rs` & `teapy-0.7.3/tea-py/src/equity.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/src/from_py.rs` & `teapy-0.7.3/tea-py/src/from_py.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/src/lib.rs` & `teapy-0.7.3/tea-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/src/pylazy/datadict.rs` & `teapy-0.7.3/tea-py/src/pylazy/datadict.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/src/pylazy/groupby.rs` & `teapy-0.7.3/tea-py/src/pylazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/src/pylazy/impl_pyexpr.rs` & `teapy-0.7.3/tea-py/src/pylazy/impl_pyexpr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/src/pylazy/mod.rs` & `teapy-0.7.3/tea-py/src/pylazy/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/src/pylazy/pyexpr.rs` & `teapy-0.7.3/tea-py/src/pylazy/pyexpr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/tea-py/src/pylazy/pyfunc.rs` & `teapy-0.7.3/tea-py/src/pylazy/pyfunc.rs`

 * *Files 0% similar despite different names*

```diff
@@ -81,25 +81,23 @@
             )));
         }
     } else if obj.get_type().qualname()? == "Series" {
         // cast pandas.Series to PyExpr
         let module_name = obj.getattr("__module__")?.extract::<&str>()?;
         let module_name = module_name.split('.').next().unwrap();
         if module_name == "pandas" {
-            dbg!("parse pd Series");
+            // dbg!("parse pd Series");
             let obj = obj.getattr("values")?;
             return parse_expr(obj, copy);
         } else if module_name == "polars" {
             let kwargs = PyDict::new(obj.py());
             kwargs.set_item("writable", false)?;
             let dtype = obj.getattr("dtype")?.str()?.to_str()?;
-            // let mut obj = obj.getattr("to_numpy")?.call((), Some(kwargs))?;
             let mut obj = obj.call_method("to_numpy", (), Some(kwargs))?;
             if dtype == "Utf8" {
-                // obj = obj.getattr("astype")?.call1(("str",))?;
                 obj = obj.call_method("astype", ("str",), None)?;
             }
             return parse_expr(obj, copy);
         } else {
             return Err(PyValueError::new_err(format!(
                 "Series of module {module_name} is not supported"
             )));
@@ -508,13 +506,8 @@
     use tea_io::scan_ipc_lazy;
     let out: Vec<PyExpr> = scan_ipc_lazy(path, columns.0)
         .map_err(StrError::to_py)?
         .into_iter()
         .map(|e| e.into())
         .collect();
     Ok(out)
-    // let dd = DataDict::scan_ipc(path, columns.0).map_err(StrError::to_py)?;
-    // Ok(PyDataDict {
-    //     dd,
-    //     obj_map: Default::default(),
-    // })
 }
```

### Comparing `teapy-0.7.2/README.md` & `teapy-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/Cargo.lock` & `teapy-0.7.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -110,20 +110,14 @@
 name = "base16ct"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c7f02d4ea65f2c1853089ffd8d2787bdbc63de2f0d29dedbcf8ccdfa0ccd4cf"
 
 [[package]]
 name = "base64"
-version = "0.21.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
-
-[[package]]
-name = "base64"
 version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
@@ -442,23 +436,23 @@
 name = "filetime"
 version = "0.2.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ee447700ac8aa0b2f2bd7bc4462ad686ba06baa6727ac149a2d6277f0d240fd"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.4.1",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.28"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
+checksum = "4556222738635b7a3417ae6130d8f52201e45a0c4d1a907f0826383adb5f85e7"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
@@ -703,17 +697,17 @@
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -955,15 +949,15 @@
 [[package]]
 name = "ocipkg"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9bb3293021f06540803301af45e7ab81693d50e89a7398a3420bdab139e7ba5e"
 dependencies = [
  "base16ct",
- "base64 0.22.0",
+ "base64",
  "chrono",
  "directories",
  "flate2",
  "lazy_static",
  "log",
  "oci-spec",
  "regex",
@@ -1059,33 +1053,33 @@
 name = "option-ext"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.5.1",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "paste"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
@@ -1301,14 +1295,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
+dependencies = [
+ "bitflags 2.5.0",
+]
+
+[[package]]
 name = "redox_users"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd283d9651eeda4b2a83a43c1c91b266c40fd76ecd39a50a8c630ae69dc72891"
 dependencies = [
  "getrandom",
  "libredox",
@@ -1416,15 +1419,15 @@
 
 [[package]]
 name = "rustls-pemfile"
 version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29993a25686778eb88d4189742cd713c9bce943bc54251a33509dc63cbacf73d"
 dependencies = [
- "base64 0.22.0",
+ "base64",
  "rustls-pki-types",
 ]
 
 [[package]]
 name = "rustls-pki-types"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1653,15 +1656,15 @@
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tea-core"
-version = "0.7.2"
+version = "0.7.3"
 dependencies = [
  "arrow2",
  "intel-mkl-src",
  "lapack-sys",
  "libc",
  "ndarray",
  "num",
@@ -1671,36 +1674,36 @@
  "tea-dtype",
  "tea-error",
  "tea-utils",
 ]
 
 [[package]]
 name = "tea-dtype"
-version = "0.7.2"
+version = "0.7.3"
 dependencies = [
  "ndarray",
  "num",
  "numpy",
  "pyo3",
  "serde",
  "tea-time",
  "tea-utils",
 ]
 
 [[package]]
 name = "tea-error"
-version = "0.7.2"
+version = "0.7.3"
 dependencies = [
  "arrow2",
  "pyo3",
 ]
 
 [[package]]
 name = "tea-ext"
-version = "0.7.2"
+version = "0.7.3"
 dependencies = [
  "ndarray",
  "num",
  "paste",
  "pyo3",
  "rayon",
  "statrs",
@@ -1708,74 +1711,74 @@
  "tea-hash",
  "tea-lazy",
  "tea-macros",
 ]
 
 [[package]]
 name = "tea-groupby"
-version = "0.7.2"
+version = "0.7.3"
 dependencies = [
  "ndarray",
  "pyo3",
  "rayon",
  "tea-core",
  "tea-ext",
  "tea-hash",
  "tea-lazy",
  "tea-macros",
 ]
 
 [[package]]
 name = "tea-hash"
-version = "0.7.2"
+version = "0.7.3"
 dependencies = [
  "ahash",
  "gxhash",
  "tea-dtype",
 ]
 
 [[package]]
 name = "tea-io"
-version = "0.7.2"
+version = "0.7.3"
 dependencies = [
  "arrow2",
  "memmap2",
  "rayon",
  "tea-core",
  "tea-hash",
  "tea-lazy",
  "tea-macros",
 ]
 
 [[package]]
 name = "tea-lazy"
-version = "0.7.2"
+version = "0.7.3"
 dependencies = [
  "ndarray",
  "parking_lot",
  "pyo3",
  "rayon",
  "regex",
  "tea-core",
  "tea-hash",
 ]
 
 [[package]]
 name = "tea-macros"
-version = "0.7.2"
+version = "0.7.3"
 dependencies = [
  "ndarray",
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "tea-py"
-version = "0.7.2"
+version = "0.7.3"
 dependencies = [
  "ahash",
  "chrono",
  "ndarray",
  "numpy",
  "once_cell",
  "parking_lot",
@@ -1788,25 +1791,25 @@
  "tea-hash",
  "tea-io",
  "tea-lazy",
 ]
 
 [[package]]
 name = "tea-time"
-version = "0.7.2"
+version = "0.7.3"
 dependencies = [
  "chrono",
  "ndarray",
  "numpy",
  "pyo3",
 ]
 
 [[package]]
 name = "tea-utils"
-version = "0.7.2"
+version = "0.7.3"
 
 [[package]]
 name = "tempfile"
 version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
@@ -1922,19 +1925,19 @@
 name = "untrusted"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
 
 [[package]]
 name = "ureq"
-version = "2.9.6"
+version = "2.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11f214ce18d8b2cbe84ed3aa6486ed3f5b285cf8d8fbdbce9f3f767a724adc35"
+checksum = "d11a831e3c0b56e438a28308e7c810799e3c118417f342d30ecec080105395cd"
 dependencies = [
- "base64 0.21.7",
+ "base64",
  "flate2",
  "log",
  "native-tls",
  "once_cell",
  "rustls",
  "rustls-native-certs",
  "rustls-pki-types",
@@ -2283,17 +2286,17 @@
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "zeroize"
-version = "1.8.0"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "63381fa6624bf92130a6b87c0d07380116f80b565c42cf0d754136f0238359ef"
+checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
 
 [[package]]
 name = "zstd"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a27595e173641171fc74a1232b7b1c7a7cb6e18222c11e9dfb9888fa424c53c"
 dependencies = [
```

### Comparing `teapy-0.7.2/Cargo.toml` & `teapy-0.7.3/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 resolver = "2"
 members = ["tea-core", "tea-dtype", "tea-error", "tea-ext", "tea-groupby", "tea-hash", "tea-io", "tea-lazy", "tea-macros", "tea-py", "tea-time", "tea-utils"]
 
 [workspace.package]
-version = "0.7.2"
+version = "0.7.3"
 authors = ["Teamon"]
 edition = "2021"
 repository = "https://github.com/Teamon9161/teapy"
 license = "MIT"
 
 [profile.release]
 lto = true
```

### Comparing `teapy-0.7.2/pyproject.toml` & `teapy-0.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/mod_func.py` & `teapy-0.7.3/python/teapy/mod_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/wrapper.py` & `teapy-0.7.3/python/teapy/wrapper.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/py_datadict.py` & `teapy-0.7.3/python/teapy/py_datadict.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/selector.py` & `teapy-0.7.3/python/teapy/selector.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/__init__.py` & `teapy-0.7.3/python/teapy/__init__.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/array_func.py` & `teapy-0.7.3/python/teapy/array_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/tests/test_context.py` & `teapy-0.7.3/python/teapy/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/tests/test_array_func.py` & `teapy-0.7.3/python/teapy/tests/test_array_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/tests/test_expr.py` & `teapy-0.7.3/python/teapy/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/tests/test_equity.py` & `teapy-0.7.3/python/teapy/tests/test_equity.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/tests/window/test_norm.py` & `teapy-0.7.3/python/teapy/tests/window/test_norm.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/tests/window/test_reg.py` & `teapy-0.7.3/python/teapy/tests/window/test_reg.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/tests/window/test_corr.py` & `teapy-0.7.3/python/teapy/tests/window/test_corr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/tests/window/test_feature.py` & `teapy-0.7.3/python/teapy/tests/window/test_feature.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/tests/window/test_compare.py` & `teapy-0.7.3/python/teapy/tests/window/test_compare.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/tests/test_datadict.py` & `teapy-0.7.3/python/teapy/tests/test_datadict.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/tests/test_common.py` & `teapy-0.7.3/python/teapy/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/window_func.py` & `teapy-0.7.3/python/teapy/window_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/regression.py` & `teapy-0.7.3/python/teapy/regression.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/testing.py` & `teapy-0.7.3/python/teapy/testing.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/python/teapy/expr.py` & `teapy-0.7.3/python/teapy/expr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.2/PKG-INFO` & `teapy-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: teapy
-Version: 0.7.2
+Version: 0.7.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy >=1.16.0
 License-File: LICENSE
 Summary: A blazingly fast datadict library
```

