# Comparing `tmp/jz3-0.1.1.tar.gz` & `tmp/jz3-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jz3-0.1.1.tar", last modified: Fri Apr 19 17:19:55 2024, max compression
+gzip compressed data, was "jz3-0.1.2.tar", last modified: Fri Apr 26 02:55:34 2024, max compression
```

## Comparing `jz3-0.1.1.tar` & `jz3-0.1.2.tar`

### file list

```diff
@@ -1,210 +1,209 @@
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.988700 jz3-0.1.1/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1096 2024-04-18 04:18:37.000000 jz3-0.1.1/LICENSE-Z3.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1092 2024-04-18 04:24:33.000000 jz3-0.1.1/LICENSE.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3012 2024-04-19 17:19:55.988443 jz3-0.1.1/PKG-INFO
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2347 2024-04-19 04:33:39.000000 jz3-0.1.1/README.md
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.965530 jz3-0.1.1/jz3/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:07:29.000000 jz3-0.1.1/jz3/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.966861 jz3-0.1.1/jz3/analysis/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.1/jz3/analysis/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.967141 jz3-0.1.1/jz3/analysis/archive/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.1/jz3/analysis/archive/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2859 2024-04-19 01:59:02.000000 jz3-0.1.1/jz3/analysis/archive/export_to_excel.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     7252 2024-04-19 16:25:42.000000 jz3-0.1.1/jz3/analysis/compare_easy_sudokus.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     6709 2024-04-19 16:49:43.000000 jz3-0.1.1/jz3/analysis/plot_comparison.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:07:38.000000 jz3-0.1.1/jz3/solver.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.967396 jz3-0.1.1/jz3/solvers/
--rw-------   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.1/jz3/solvers/__init__ 2.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.967623 jz3-0.1.1/jz3/solvers/cvc5-main/
--rw-------   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.1/jz3/solvers/cvc5-main/__init__ 2.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.967735 jz3-0.1.1/jz3/solvers/cvc5-main/build/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.967849 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.967980 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.968101 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.968224 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.968764 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     3116 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/cad.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     1148 2024-03-01 13:47:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/plot.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     1462 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/sign_table.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.968938 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.969349 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     1801 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/check.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     4904 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/polypy_test.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.971847 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     4580 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/algebraic_number.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     5869 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_arithmetic.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1595 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_eval.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3805 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_factorization.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     5610 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_feasibility.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     4946 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_gcd.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     4434 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_mgcd.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     6784 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_resultants.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     4241 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_roots.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3185 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_sgn.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     3694 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/upolynomial_factor.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     3292 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/upolynomial_gcd.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     3150 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/upolynomial_roots.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2528 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/value.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     1941 2023-11-02 19:49:25.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/variable.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.972437 jz3-0.1.1/jz3/solvers/cvc5-main/contrib/
--rw-------   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.1/jz3/solvers/cvc5-main/contrib/__init__ 2.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/contrib/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     6875 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/contrib/learn_resource_weights.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     3724 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/contrib/make-release.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.972829 jz3-0.1.1/jz3/solvers/cvc5-main/contrib/packaging_python/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/contrib/packaging_python/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1258 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/contrib/packaging_python/mk_build_dir.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     4275 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/contrib/packaging_python/mk_wheel.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     1501 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/contrib/uncovered-api-functions.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.972960 jz3-0.1.1/jz3/solvers/cvc5-main/docs/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/docs/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.973716 jz3-0.1.1/jz3/solvers/cvc5-main/docs/ext/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/docs/ext/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1380 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/docs/ext/autoenum.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     4089 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/docs/ext/examples.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1522 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/docs/ext/include_build_file.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1809 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/docs/ext/run_command.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     6014 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/docs/ext/smtliblexer.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.973934 jz3-0.1.1/jz3/solvers/cvc5-main/examples/
--rw-------   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/__init__ 2.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.974024 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.977188 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3445 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/bags.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     4302 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/bitvectors.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3399 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/bitvectors_and_arrays.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3390 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/combination.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     6001 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/datatypes.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1428 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/exceptions.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1570 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/extract.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1538 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/finite_field.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     4111 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/floating_point.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      842 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/helloworld.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1026 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/id.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2257 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/linear_arith.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.979132 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1000 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/bitvectors.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      946 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/bitvectors_and_arrays.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      801 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/combination.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1459 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/datatypes.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      390 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/exceptions.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      402 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/extract.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      766 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/floating_point.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      102 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/helloworld.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      348 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/id.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      232 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/linear_arith.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1444 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/quickstart.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      441 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/sets.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      156 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/transcendentals.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     6561 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/quickstart.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     6283 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/relations.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2035 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/sequences.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2878 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/sets.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3128 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/strings.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3243 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/sygus-fun.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2152 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/sygus-inv.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1375 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/transcendentals.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1847 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/utils.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.979250 jz3-0.1.1/jz3/solvers/cvc5-main/src/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/src/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.979427 jz3-0.1.1/jz3/solvers/cvc5-main/src/api/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/src/api/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.979572 jz3-0.1.1/jz3/solvers/cvc5-main/src/api/java/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/src/api/java/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     7110 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/src/api/parseenums.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.979668 jz3-0.1.1/jz3/solvers/cvc5-main/src/api/python/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/src/api/python/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.979873 jz3-0.1.1/jz3/solvers/cvc5-main/src/base/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/src/base/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3208 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/src/base/collect_tags.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.980106 jz3-0.1.1/jz3/solvers/cvc5-main/src/options/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/src/options/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    43409 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/src/options/mkoptions.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.981307 jz3-0.1.1/jz3/solvers/cvc5-main/src/rewriter/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/src/rewriter/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    11371 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/src/rewriter/mkrewrites.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     7288 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/src/rewriter/node.py
--rw-------   0 jiazhenghao   (501) staff       (20)     1382 2023-11-02 15:53:34.000000 jz3-0.1.1/jz3/solvers/cvc5-main/src/rewriter/rule 2.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1382 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/src/rewriter/rule.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    10506 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/src/rewriter/rw_parser.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2178 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/src/rewriter/util.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.981624 jz3-0.1.1/jz3/solvers/cvc5-main/test/
--rw-------   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/__init__ 2.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.981755 jz3-0.1.1/jz3/solvers/cvc5-main/test/api/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/api/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.983182 jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      824 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/boilerplate.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1433 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/finite_field.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1127 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/issue4889.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      888 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/issue5074.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1519 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/issue6111.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1008 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/proj-issue306.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1545 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/reset_assertions.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     6607 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/sep_log_api.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      756 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/two_solvers.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.983421 jz3-0.1.1/jz3/solvers/cvc5-main/test/binary/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/binary/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2445 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/binary/interactive_shell.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.983549 jz3-0.1.1/jz3/solvers/cvc5-main/test/regress/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/regress/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.983789 jz3-0.1.1/jz3/solvers/cvc5-main/test/regress/cli/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/regress/cli/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)    31784 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/regress/cli/run_regression.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.983950 jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.984062 jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.986012 jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    18818 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_datatype_api.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1506 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_finite_field.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     4112 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_grammar.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     7537 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_op.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2221 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_proof.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2456 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_result.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    99840 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_solver.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    19318 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_sort.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1822 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_synth_result.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    42934 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_term.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3300 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_to_python_obj.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.986695 jz3-0.1.1/jz3/src/
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.987077 jz3-0.1.1/jz3/src/SMTs/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    11530 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/src/SMTs/SMTs.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.1/jz3/src/SMTs/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.987656 jz3-0.1.1/jz3/src/Sudokus/
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)    36816 2024-04-19 04:21:10.000000 jz3-0.1.1/jz3/src/Sudokus/Sudoku.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.1/jz3/src/Sudokus/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)    22629 2024-04-19 16:54:47.000000 jz3-0.1.1/jz3/src/Sudokus/sudoku_exhaustive_search_condition.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    22912 2024-04-19 04:23:09.000000 jz3-0.1.1/jz3/src/Sudokus/sudoku_heuristic_search_condition.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.1/jz3/src/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)       84 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/src/clean_up.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2709 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/src/run_solvers.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      335 2024-04-18 02:04:15.000000 jz3-0.1.1/jz3/src/z3_quick_start_guide.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    10955 2024-04-19 04:23:09.000000 jz3-0.1.1/jz3/src/z3_wrapper.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.987909 jz3-0.1.1/jz3/tests/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:12.000000 jz3-0.1.1/jz3/tests/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:20.000000 jz3-0.1.1/jz3/tests/test_solver.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 17:19:55.988109 jz3-0.1.1/jz3.egg-info/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3012 2024-04-19 17:19:55.000000 jz3-0.1.1/jz3.egg-info/PKG-INFO
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     8424 2024-04-19 17:19:55.000000 jz3-0.1.1/jz3.egg-info/SOURCES.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        1 2024-04-19 17:19:55.000000 jz3-0.1.1/jz3.egg-info/dependency_links.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)       21 2024-04-19 17:19:55.000000 jz3-0.1.1/jz3.egg-info/requires.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        4 2024-04-19 17:19:55.000000 jz3-0.1.1/jz3.egg-info/top_level.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)       38 2024-04-19 17:19:55.988754 jz3-0.1.1/setup.cfg
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      810 2024-04-19 17:18:43.000000 jz3-0.1.1/setup.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.322820 jz3-0.1.2/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1096 2024-04-18 04:18:37.000000 jz3-0.1.2/LICENSE-Z3.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1092 2024-04-18 04:24:33.000000 jz3-0.1.2/LICENSE.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2961 2024-04-26 02:55:34.322669 jz3-0.1.2/PKG-INFO
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2347 2024-04-19 04:33:39.000000 jz3-0.1.2/README.md
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.288528 jz3-0.1.2/jz3/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      134 2024-04-26 02:43:34.000000 jz3-0.1.2/jz3/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.290135 jz3-0.1.2/jz3/analysis/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.2/jz3/analysis/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.290657 jz3-0.1.2/jz3/analysis/archive/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.2/jz3/analysis/archive/__init__.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2859 2024-04-19 01:59:02.000000 jz3-0.1.2/jz3/analysis/archive/export_to_excel.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     7252 2024-04-19 16:25:42.000000 jz3-0.1.2/jz3/analysis/compare_whole_problems.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     6709 2024-04-21 00:45:55.000000 jz3-0.1.2/jz3/analysis/plot_comparison.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.291133 jz3-0.1.2/jz3/solvers/
+-rw-------   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.2/jz3/solvers/__init__ 2.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.291340 jz3-0.1.2/jz3/solvers/cvc5-main/
+-rw-------   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.2/jz3/solvers/cvc5-main/__init__ 2.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.291436 jz3-0.1.2/jz3/solvers/cvc5-main/build/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.291530 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.291622 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.291728 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.291837 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.292764 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/__init__.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     3116 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/cad.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     1148 2024-03-01 13:47:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/plot.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     1462 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/sign_table.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.293016 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.293662 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/__init__.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     1801 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/check.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     4904 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/polypy_test.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.297870 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/__init__.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     4580 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/algebraic_number.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     5869 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_arithmetic.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1595 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_eval.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     3805 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_factorization.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     5610 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_feasibility.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     4946 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_gcd.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     4434 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_mgcd.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     6784 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_resultants.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     4241 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_roots.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     3185 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_sgn.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     3694 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/upolynomial_factor.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     3292 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/upolynomial_gcd.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     3150 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/upolynomial_roots.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2528 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/value.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     1941 2023-11-02 19:49:25.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/variable.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.298813 jz3-0.1.2/jz3/solvers/cvc5-main/contrib/
+-rw-------   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.2/jz3/solvers/cvc5-main/contrib/__init__ 2.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/contrib/__init__.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     6875 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/contrib/learn_resource_weights.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     3724 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/contrib/make-release.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.299275 jz3-0.1.2/jz3/solvers/cvc5-main/contrib/packaging_python/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/contrib/packaging_python/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1258 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/contrib/packaging_python/mk_build_dir.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     4275 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/contrib/packaging_python/mk_wheel.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     1501 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/contrib/uncovered-api-functions.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.299541 jz3-0.1.2/jz3/solvers/cvc5-main/docs/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/docs/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.300467 jz3-0.1.2/jz3/solvers/cvc5-main/docs/ext/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/docs/ext/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1380 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/docs/ext/autoenum.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     4089 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/docs/ext/examples.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1522 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/docs/ext/include_build_file.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1809 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/docs/ext/run_command.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     6014 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/docs/ext/smtliblexer.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.300853 jz3-0.1.2/jz3/solvers/cvc5-main/examples/
+-rw-------   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/__init__ 2.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.300959 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.305221 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     3445 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/bags.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     4302 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/bitvectors.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     3399 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/bitvectors_and_arrays.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     3390 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/combination.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     6001 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/datatypes.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1428 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/exceptions.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1570 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/extract.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1538 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/finite_field.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     4111 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/floating_point.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      842 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/helloworld.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1026 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/id.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2257 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/linear_arith.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.307320 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1000 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/bitvectors.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      946 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/bitvectors_and_arrays.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      801 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/combination.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1459 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/datatypes.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      390 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/exceptions.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      402 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/extract.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      766 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/floating_point.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      102 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/helloworld.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      348 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/id.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      232 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/linear_arith.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1444 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/quickstart.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      441 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/sets.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      156 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/transcendentals.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     6561 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/quickstart.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     6283 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/relations.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2035 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/sequences.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2878 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/sets.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     3128 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/strings.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     3243 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/sygus-fun.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2152 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/sygus-inv.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1375 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/transcendentals.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1847 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/utils.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.307477 jz3-0.1.2/jz3/solvers/cvc5-main/src/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/src/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.307669 jz3-0.1.2/jz3/solvers/cvc5-main/src/api/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/src/api/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.307985 jz3-0.1.2/jz3/solvers/cvc5-main/src/api/java/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/src/api/java/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     7110 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/src/api/parseenums.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.308102 jz3-0.1.2/jz3/solvers/cvc5-main/src/api/python/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/src/api/python/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.308323 jz3-0.1.2/jz3/solvers/cvc5-main/src/base/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/src/base/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     3208 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/src/base/collect_tags.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.308864 jz3-0.1.2/jz3/solvers/cvc5-main/src/options/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/src/options/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)    43409 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/src/options/mkoptions.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.311682 jz3-0.1.2/jz3/solvers/cvc5-main/src/rewriter/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/src/rewriter/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)    11371 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/src/rewriter/mkrewrites.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     7288 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/src/rewriter/node.py
+-rw-------   0 jiazhenghao   (501) staff       (20)     1382 2023-11-02 15:53:34.000000 jz3-0.1.2/jz3/solvers/cvc5-main/src/rewriter/rule 2.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1382 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/src/rewriter/rule.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)    10506 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/src/rewriter/rw_parser.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2178 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/src/rewriter/util.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.312077 jz3-0.1.2/jz3/solvers/cvc5-main/test/
+-rw-------   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/__init__ 2.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.312195 jz3-0.1.2/jz3/solvers/cvc5-main/test/api/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/api/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.314096 jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      824 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/boilerplate.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1433 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/finite_field.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1127 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/issue4889.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      888 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/issue5074.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1519 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/issue6111.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1008 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/proj-issue306.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1545 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/reset_assertions.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     6607 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/sep_log_api.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      756 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/two_solvers.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.314389 jz3-0.1.2/jz3/solvers/cvc5-main/test/binary/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/binary/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2445 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/binary/interactive_shell.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.314556 jz3-0.1.2/jz3/solvers/cvc5-main/test/regress/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/regress/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.314748 jz3-0.1.2/jz3/solvers/cvc5-main/test/regress/cli/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/regress/cli/__init__.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)    31784 2024-04-18 02:04:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/regress/cli/run_regression.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.315042 jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.315138 jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.318817 jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)    18818 2024-04-18 02:04:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_datatype_api.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1506 2024-04-18 02:04:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_finite_field.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     4112 2024-04-18 02:04:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_grammar.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     7537 2024-04-18 02:04:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_op.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2221 2024-04-18 02:04:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_proof.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2456 2024-04-18 02:04:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_result.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)    99840 2024-04-18 02:04:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_solver.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)    19318 2024-04-18 02:04:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_sort.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1822 2024-04-18 02:04:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_synth_result.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)    42934 2024-04-18 02:04:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_term.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     3300 2024-04-18 02:04:15.000000 jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_to_python_obj.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.320076 jz3-0.1.2/jz3/src/
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.320876 jz3-0.1.2/jz3/src/SMTs/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)    11530 2024-04-18 02:04:15.000000 jz3-0.1.2/jz3/src/SMTs/SMTs.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.2/jz3/src/SMTs/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.322063 jz3-0.1.2/jz3/src/Sudokus/
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)    36804 2024-04-26 02:43:34.000000 jz3-0.1.2/jz3/src/Sudokus/Sudoku.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.2/jz3/src/Sudokus/__init__.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)    23168 2024-04-26 02:29:33.000000 jz3-0.1.2/jz3/src/Sudokus/sudoku_exhaustive_search_condition.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)    22912 2024-04-19 04:23:09.000000 jz3-0.1.2/jz3/src/Sudokus/sudoku_heuristic_search_condition.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.2/jz3/src/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)       84 2024-04-18 02:04:15.000000 jz3-0.1.2/jz3/src/clean_up.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     3311 2024-04-26 01:21:03.000000 jz3-0.1.2/jz3/src/run_solvers.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      335 2024-04-18 02:04:15.000000 jz3-0.1.2/jz3/src/z3_quick_start_guide.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)    10939 2024-04-26 02:43:34.000000 jz3-0.1.2/jz3/src/z3_wrapper.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.322490 jz3-0.1.2/jz3/tests/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:12.000000 jz3-0.1.2/jz3/tests/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:20.000000 jz3-0.1.2/jz3/tests/test_solver.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 02:55:34.289464 jz3-0.1.2/jz3.egg-info/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2961 2024-04-26 02:55:34.000000 jz3-0.1.2/jz3.egg-info/PKG-INFO
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     8412 2024-04-26 02:55:34.000000 jz3-0.1.2/jz3.egg-info/SOURCES.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        1 2024-04-26 02:55:34.000000 jz3-0.1.2/jz3.egg-info/dependency_links.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)       21 2024-04-26 02:55:34.000000 jz3-0.1.2/jz3.egg-info/requires.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        4 2024-04-26 02:55:34.000000 jz3-0.1.2/jz3.egg-info/top_level.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)       38 2024-04-26 02:55:34.322864 jz3-0.1.2/setup.cfg
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      810 2024-04-26 02:44:46.000000 jz3-0.1.2/setup.py
```

### Comparing `jz3-0.1.1/LICENSE-Z3.txt` & `jz3-0.1.2/LICENSE-Z3.txt`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/LICENSE.txt` & `jz3-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/PKG-INFO` & `jz3-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: jz3
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple wrapper for Z3 solver
 Home-page: https://github.com/Robert-Jia00129/jz3
 Author: Sebastiaan Joosten, Zheng Robert Jia
 Author-email: jia00129@umn.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE-Z3.txt
 License-File: LICENSE.txt
-Requires-Dist: z3-solver
-Requires-Dist: matplotlib
 
 # Argyle_Sudoku
 > This project was partly based on the code from [z3-sudoku](https://github.com/awkwardbunny/z3-sudoku)
 
 This project uses python z3-solver to benchmark encoding techniques to solving the same problem. 
 It then compares the efficiency of each method and between different encoding techniques.
```

### Comparing `jz3-0.1.1/README.md` & `jz3-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/analysis/archive/export_to_excel.py` & `jz3-0.1.2/jz3/analysis/archive/export_to_excel.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/analysis/compare_easy_sudokus.py` & `jz3-0.1.2/jz3/analysis/compare_whole_problems.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/analysis/plot_comparison.py` & `jz3-0.1.2/jz3/analysis/plot_comparison.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/cad.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/cad.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/plot.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/plot.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/sign_table.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/sign_table.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/check.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/check.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/polypy_test.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/polypy_test.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/algebraic_number.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/algebraic_number.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_arithmetic.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_arithmetic.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_eval.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_eval.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_factorization.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_factorization.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_feasibility.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_feasibility.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_gcd.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_gcd.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_mgcd.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_mgcd.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_resultants.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_resultants.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_roots.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_roots.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_sgn.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_sgn.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/upolynomial_factor.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/upolynomial_factor.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/upolynomial_gcd.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/upolynomial_gcd.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/upolynomial_roots.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/upolynomial_roots.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/value.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/value.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/variable.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/variable.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/contrib/learn_resource_weights.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/contrib/learn_resource_weights.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/contrib/make-release.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/contrib/make-release.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/contrib/packaging_python/mk_build_dir.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/contrib/packaging_python/mk_build_dir.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/contrib/packaging_python/mk_wheel.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/contrib/packaging_python/mk_wheel.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/contrib/uncovered-api-functions.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/contrib/uncovered-api-functions.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/docs/ext/autoenum.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/docs/ext/autoenum.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/docs/ext/examples.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/docs/ext/examples.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/docs/ext/include_build_file.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/docs/ext/include_build_file.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/docs/ext/run_command.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/docs/ext/run_command.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/docs/ext/smtliblexer.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/docs/ext/smtliblexer.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/bags.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/bags.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/bitvectors.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/bitvectors.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/bitvectors_and_arrays.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/bitvectors_and_arrays.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/combination.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/combination.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/datatypes.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/datatypes.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/exceptions.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/exceptions.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/extract.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/extract.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/finite_field.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/finite_field.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/floating_point.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/floating_point.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/helloworld.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/helloworld.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/id.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/id.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/linear_arith.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/linear_arith.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/bitvectors.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/bitvectors.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/bitvectors_and_arrays.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/bitvectors_and_arrays.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/combination.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/combination.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/datatypes.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/datatypes.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/floating_point.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/floating_point.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/pythonic/quickstart.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/pythonic/quickstart.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/quickstart.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/quickstart.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/relations.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/relations.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/sequences.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/sequences.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/sets.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/sets.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/strings.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/strings.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/sygus-fun.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/sygus-fun.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/sygus-inv.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/sygus-inv.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/transcendentals.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/transcendentals.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/examples/api/python/utils.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/examples/api/python/utils.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/src/api/parseenums.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/src/api/parseenums.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/src/base/collect_tags.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/src/base/collect_tags.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/src/options/mkoptions.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/src/options/mkoptions.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/src/rewriter/mkrewrites.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/src/rewriter/mkrewrites.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/src/rewriter/node.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/src/rewriter/node.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/src/rewriter/rule 2.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/src/rewriter/rule 2.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/src/rewriter/rule.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/src/rewriter/rule.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/src/rewriter/rw_parser.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/src/rewriter/rw_parser.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/src/rewriter/util.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/src/rewriter/util.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/boilerplate.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/boilerplate.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/finite_field.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/finite_field.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/issue4889.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/issue4889.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/issue5074.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/issue5074.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/issue6111.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/issue6111.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/proj-issue306.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/proj-issue306.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/reset_assertions.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/reset_assertions.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/sep_log_api.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/sep_log_api.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/api/python/two_solvers.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/api/python/two_solvers.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/binary/interactive_shell.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/binary/interactive_shell.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/regress/cli/run_regression.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/regress/cli/run_regression.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_datatype_api.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_datatype_api.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_finite_field.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_finite_field.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_grammar.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_grammar.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_op.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_op.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_proof.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_proof.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_result.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_result.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_solver.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_solver.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_sort.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_sort.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_synth_result.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_synth_result.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_term.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_term.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/solvers/cvc5-main/test/unit/api/python/test_to_python_obj.py` & `jz3-0.1.2/jz3/solvers/cvc5-main/test/unit/api/python/test_to_python_obj.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/src/SMTs/SMTs.py` & `jz3-0.1.2/jz3/src/SMTs/SMTs.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/src/Sudokus/Sudoku.py` & `jz3-0.1.2/jz3/src/Sudokus/Sudoku.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import z3
 import numpy as np
 import random
 from copy import deepcopy
 import time
 from typing import List
 from pathlib import Path
-from jz3.src.z3_wrapper import Solver2SMT
+from jz3.src.z3_wrapper import Solver
 
 
 # z3.set_param('parallel.enable',True)
 
 class Sudoku:
     _grid = None  # Creating an empty matrix with None everywhere
     _solver = None  # The solver
@@ -49,15 +49,15 @@
                 boolean representation (val1, val2... val9): val2==True indicates the number is 2 at this index
         :param prefill: prefill the grid:
             per_col case: prefill the first row with 1-9 in random order
             not per_col case: prefill all the 1s with random numbers
         :param hard_smt_logPath:
         """
         # a 1-D sudoku_array
-        self._solver = Solver2SMT()
+        self._solver = Solver()
         self._timeout = 5000
         self._incTimeOut = self._timeout
         self._solver.set("timeout", self._timeout)
         # self._solver.from_file("fileName")
         self._classic = classic
         self._distinct = distinct
         self._no_num = no_num
@@ -73,15 +73,15 @@
         self._seed = seed
         self._store_global = False
         self._global_solver = z3.Solver()
         self._distinctdigits = distinct_digits
         self._condition_var_distinct = z3.Bool('distinct')
         self._condition_var_pbeq = z3.Bool('pbeq')
         self._heuristic_search_mode = heuristic_search_mode
-        self._heuristic_solver = Solver2SMT(benchmark_mode=benchmark_mode)
+        self._heuristic_solver = Solver(benchmark_mode=benchmark_mode)
         self._heuristic_solver.add_global_constraints(z3.Or(self._condition_var_distinct,self._condition_var_pbeq))
 
         if seed == 0:
             print("WARNING: NO random seed was set for solver class. "
                   "This would cause experiments to be unreliable when compared in across constraints."
                   "If this is intentional, please ignore .")
         random.seed(seed)
```

### Comparing `jz3-0.1.1/jz3/src/Sudokus/sudoku_exhaustive_search_condition.py` & `jz3-0.1.2/jz3/src/Sudokus/sudoku_exhaustive_search_condition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import subprocess
+import sys
 import time
 import zipfile
 from pathlib import Path
 from typing import List, Hashable
 from jz3.src.Sudokus import Sudoku
 
 
@@ -290,15 +291,15 @@
         return solve_with_z3(smt_file_path, time_out=time_out)
     elif solver_name == 'cvc5':
         return solve_with_cvc5(smt_file_path, time_out=time_out)
     # Add more elif blocks for other solvers
     raise ValueError(f"Unknown solver: {solver_name}, please implement the corresponding code")
 
 
-def load_and_alternative_solve_hard(hard_instances_txt_log_dir: str, is_classic: bool, num_iter: int,
+def load_and_alternative_solve_hard_once(hard_instances_txt_log_dir: str, is_classic: bool, num_iter: int,
                                     currline_path="curr_instance_line.txt", timeout=5,
                                     hard_smt_dir="../../problems_instances/particular_hard_instances_records/smt2_files/",
                                     time_record_dir:str=""):
     """
     Writes a dictionary with {problem: , cond_1_time: , cond_2_time: cond_3_time: cond_4_time: ...}
     Condition[0] MUST be TRUE when classic and FALSE when argyle
     :param file_path:
@@ -327,24 +328,32 @@
             "classic" if is_classic else "argyle"] += curr_line_num + num_iter  # record read lines up till now
 
         # skip current line numbers
         for _ in range(curr_line_num):
             fr.readline()
 
         for _ in range(num_iter):
-            line_to_solve = fr.readline().strip()
-            if not line_to_solve:
-                print("Not enough hard instances for experiment/Encountered an empty new line\n\n\n")
-            store_result_dict = {}
+            line_to_solve = fr.readline()
+            if line_to_solve == '\n':
+                print("Encountered an empty new line, skipping the empty line")
+                continue
+            elif line_to_solve=='':
+                print("Not enough hard instances for to solve for/\nExiting the program, consider running more experiments to find more hard instances. ")
+                sys.exit()
+            line_to_solve = line_to_solve.strip()
+
             try:
                 tgrid, tcondition, tindex, ttry_Val, tis_sat = line_to_solve.split("\t")
             except ValueError:
+                print(f"Encountered an error while trying to parse the hard instance:"
+                      f"{line_to_solve}")
                 continue
-            tcondition = eval(tcondition)
 
+            tcondition = eval(tcondition)
+            store_result_dict = {}
             # store problem and smt path
             store_result_dict["problem"] = {
                 "grid": tgrid,
                 "index": eval(tindex),
                 "try_Val": eval(ttry_Val),
                 "is_sat": tis_sat == "sat"
             }
@@ -388,15 +397,16 @@
     time_record_whole_problem_dir = os.path.join(time_record_dir,"whole_problem_time_records")
     if not os.path.exists(time_record_whole_problem_dir):
         print(f"Provided directory does not exist, creating new directory: {time_record_whole_problem_dir}")
         os.makedirs(time_record_whole_problem_dir)
     store_time_comparison_path = os.path.join(time_record_whole_problem_dir,"time.txt")
 
     # Iterate through all possible condition combinations
-    for _ in range(num_iter):
+    for asdf in range(num_iter):
+        print(f'Solving the {asdf}th problem')
         store_result_dict = {}
         empty_list = [0 for i in range(9) for j in range(9)]
 
         store_result_dict["problem"] = {
             "grid": str(empty_list)
         }
         # iterate through possible combinations
@@ -428,24 +438,28 @@
             #
             # # Record the performance of different solvers for generating holes sudoku
             # for SOLVER in SOLVER_LIST:
             #     holes_time, holes_timeout, holes_result = solve_with_solver(SOLVER, smt_str_holes, time_out=timeout)
             #     # Record the results
             #     # ...
 
-def load_and_alternative_solve_hard_once():
+
+def load_and_alternative_solve_hard(num_iter:int=0):
+    """
+    Approximately 5 instances take a minute
+    """
     time_record_dir = "../../time-record/particular_hard_instance_time_record/"
     currline_path = "../../problems_instances/particular_hard_instances_records/txt_files/curr_instance_line.txt"
     hard_instances_txt_log_dir = "../../problems_instances/particular_hard_instances_records/txt_files/"
     # load_and_alternative_solve(hard_instances_time_record_dir, is_classic=True, num_iter=10,
     #                            currline_path=alternative_solve_curr_line_path, timeout=TIME_OUT)
-    load_and_alternative_solve_hard(hard_instances_txt_log_dir=hard_instances_txt_log_dir, time_record_dir=time_record_dir, is_classic=True, num_iter=10,
+    for i in range(num_iter):
+        load_and_alternative_solve_hard_once(hard_instances_txt_log_dir=hard_instances_txt_log_dir, time_record_dir=time_record_dir, is_classic=False, num_iter=1,
                                     currline_path=currline_path, timeout=TIME_OUT)
 
-
 def run_experiment(num_iter=0):
     # dictionary of file paths to feed into `run_experiment_once`
     dct = {"curr_line_path": '../../sudoku_database/curr_line_of_solving_full_sudokus.txt',
            "classic_full_path": '../../sudoku_database/classic_full_sudokus.txt',
            "argyle_full_path": '../../sudoku_database/argyle_full_sudokus.txt',
            "classic_holes_path": '../../sudoku_database/classic_holes_sudokus.txt',
            "argyle_holes_path": "../../sudoku_database/argyle_holes_sudokus.txt",
@@ -454,25 +468,16 @@
            "hard_smt_logPath": '../../problems_instances/particular_hard_instances_records/smt2_files/'}
     for i in range(num_iter):
         run_experiment_once(False,
                             **dct
                             )
 
 if __name__ == '__main__':
+    start_time = time.time()
     TIME_OUT = 5
-    # run_experiment(1)
-    load_and_alternative_solve_hard_once()
-    print("Process Complete")
+    # run_experiment(6*5)
+    load_and_alternative_solve_hard(5)
+    end_time = time.time()
+    print(f"Process Complete. Total time taken: {end_time-start_time}")
 
 
 # record timeout despite the output.
-
-
-
-
-
-
-# percentages of timeout
-# stack the time for each constraint together, and use percentages
-# arr in latex
-
-# more solvers
```

### Comparing `jz3-0.1.1/jz3/src/Sudokus/sudoku_heuristic_search_condition.py` & `jz3-0.1.2/jz3/src/Sudokus/sudoku_heuristic_search_condition.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.1/jz3/src/run_solvers.py` & `jz3-0.1.2/jz3/src/run_solvers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import subprocess
 import time
-
+import os
+from pathlib import Path
 
 def run_cvc5(smt2_file, time_out:int=5):
-    cvc_path = "../../solvers/cvc5-macOS-arm64"
+    cvc_path = get_executable_path("cvc5-macOS-arm64")
     command = [cvc_path,smt2_file,"--lang","smt2"]
     start_time = time.time()
     did_timeout = False
     try:
         result = subprocess.run(command,
                                 capture_output=True, text=True, timeout=time_out)
         combined_output = ((result.stdout if result.stdout is not None else "") +
@@ -82,9 +83,18 @@
             print(f"Running {solver}...")
         result = run_function(smt2_file)
         results[solver] = result
 
     return results
 
 
+def get_executable_path(solver_path_in_solvers_dir):
+    # Get the directory of the current file (__file__ refers to the script in which this code is written)
+    dir_of_jz3 = Path(os.path.dirname(__file__)).parent
+
+    # Build the path to the executable
+    executable_path = os.path.join(dir_of_jz3, "solvers/"+solver_path_in_solvers_dir)
 
+    return executable_path
 
+if __name__=='__main__':
+    print(run_cvc5('/Users/jiazhenghao/Desktop/CodingProjects/jz3/jz3/problems_instances/particular_hard_instances_records/smt2_files/04_25_00_58_021714024682.151314'))
```

### Comparing `jz3-0.1.1/jz3/src/z3_wrapper.py` & `jz3-0.1.2/jz3/src/z3_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from io import StringIO
 import z3
 import jz3.src.run_solvers as run_solvers
 import warnings
 
 
 # child class to write push and pop to SMT2 file
-class Solver2SMT(z3.Solver):
+class Solver(z3.Solver):
     def __init__(self, benchmark_mode=False, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.__start_recording = False
         self.__history = []
         self.__assertions = []
         self.__global_constraints = z3.BoolVal(True)
         self.__smt_str = ""
@@ -68,15 +68,15 @@
         if args:  # append the checked condition
             self.__assertions.append((args, condition))
 
         if s.check() == z3.sat:
             # possible combination of condition variables
             model = s.model()
 
-            solver_with_conditional_constraint = Solver2SMT()
+            solver_with_conditional_constraint = Solver()
 
             # add corresponding conditional constraints and try to solve
             for (conditional_constraint, condition) in self.__assertions:
                 if condition == z3.BoolVal(True) or model.eval(condition):
                     if self.__start_recording:
                         self.__history.append(("add", str(conditional_constraint.sexpr())))
                     solver_with_conditional_constraint.add(conditional_constraint)
@@ -94,15 +94,15 @@
 
                 # find different combinations
                 opt = z3.Optimize()
                 opt.add(self.__global_constraints)
                 dist = 1
                 count = 0
                 while (count < max_count) and (dist > 0):
-                    solver_with_conditional_constraint = Solver2SMT()
+                    solver_with_conditional_constraint = Solver()
 
                     # add corresponding conditional constraints and try to solve
                     for (conditional_constraint, condition) in self.__assertions:
                         if model.eval(condition):
                             if self.__start_recording:
                                 self.__history.append(("add", str(conditional_constraint.sexpr())))
                             solver_with_conditional_constraint.add(conditional_constraint)
@@ -205,15 +205,15 @@
         return self.__condition_var_assignment_model
 
     def get_latest_solvers_results(self):
         return self.__latest_solvers_results
 
 
 def simple_test():
-    solver = Solver2SMT(benchmark_mode=True)
+    solver = Solver(benchmark_mode=True)
 
     x = z3.Int('x')
     y = z3.Int('y')
 
     solver.add(x > 0)
     solver.add(y > 0)
```

### Comparing `jz3-0.1.1/jz3.egg-info/PKG-INFO` & `jz3-0.1.2/jz3.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: jz3
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple wrapper for Z3 solver
 Home-page: https://github.com/Robert-Jia00129/jz3
 Author: Sebastiaan Joosten, Zheng Robert Jia
 Author-email: jia00129@umn.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE-Z3.txt
 License-File: LICENSE.txt
-Requires-Dist: z3-solver
-Requires-Dist: matplotlib
 
 # Argyle_Sudoku
 > This project was partly based on the code from [z3-sudoku](https://github.com/awkwardbunny/z3-sudoku)
 
 This project uses python z3-solver to benchmark encoding techniques to solving the same problem. 
 It then compares the efficiency of each method and between different encoding techniques.
```

### Comparing `jz3-0.1.1/jz3.egg-info/SOURCES.txt` & `jz3-0.1.2/jz3.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 LICENSE-Z3.txt
 LICENSE.txt
 README.md
 setup.py
 jz3/__init__.py
-jz3/solver.py
 jz3.egg-info/PKG-INFO
 jz3.egg-info/SOURCES.txt
 jz3.egg-info/dependency_links.txt
 jz3.egg-info/requires.txt
 jz3.egg-info/top_level.txt
 jz3/analysis/__init__.py
-jz3/analysis/compare_easy_sudokus.py
+jz3/analysis/compare_whole_problems.py
 jz3/analysis/plot_comparison.py
 jz3/analysis/archive/__init__.py
 jz3/analysis/archive/export_to_excel.py
 jz3/solvers/__init__ 2.py
 jz3/solvers/__init__.py
 jz3/solvers/cvc5-main/__init__ 2.py
 jz3/solvers/cvc5-main/__init__.py
```

