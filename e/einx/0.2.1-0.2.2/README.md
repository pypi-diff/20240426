# Comparing `tmp/einx-0.2.1.tar.gz` & `tmp/einx-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "einx-0.2.1.tar", last modified: Tue Apr 23 19:30:14 2024, max compression
+gzip compressed data, was "einx-0.2.2.tar", last modified: Fri Apr 26 09:50:21 2024, max compression
```

## Comparing `einx-0.2.1.tar` & `einx-0.2.2.tar`

### file list

```diff
@@ -1,67 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:30:14.767382 einx-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-23 19:30:09.000000 einx-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-23 19:30:14.767382 einx-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-23 19:30:09.000000 einx-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:30:14.755382 einx-0.2.1/einx/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-23 19:30:09.000000 einx-0.2.1/einx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:30:14.759382 einx-0.2.1/einx/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-23 19:30:09.000000 einx-0.2.1/einx/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-23 19:30:09.000000 einx-0.2.1/einx/backend/_dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-23 19:30:09.000000 einx-0.2.1/einx/backend/_jax.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-23 19:30:09.000000 einx-0.2.1/einx/backend/_mlx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-23 19:30:09.000000 einx-0.2.1/einx/backend/_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-04-23 19:30:09.000000 einx-0.2.1/einx/backend/_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    15560 2024-04-23 19:30:09.000000 einx-0.2.1/einx/backend/_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-04-23 19:30:09.000000 einx-0.2.1/einx/backend/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-23 19:30:09.000000 einx-0.2.1/einx/backend/register.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:30:14.759382 einx-0.2.1/einx/expr/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 19:30:09.000000 einx-0.2.1/einx/expr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-23 19:30:09.000000 einx-0.2.1/einx/expr/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    27957 2024-04-23 19:30:09.000000 einx-0.2.1/einx/expr/stage1.py
--rw-r--r--   0 runner    (1001) docker     (127)    40301 2024-04-23 19:30:09.000000 einx-0.2.1/einx/expr/stage2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16950 2024-04-23 19:30:09.000000 einx-0.2.1/einx/expr/stage3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-23 19:30:09.000000 einx-0.2.1/einx/expr/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:30:14.763382 einx-0.2.1/einx/nn/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 19:30:09.000000 einx-0.2.1/einx/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-23 19:30:09.000000 einx-0.2.1/einx/nn/equinox.py
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-23 19:30:09.000000 einx-0.2.1/einx/nn/flax.py
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-23 19:30:09.000000 einx-0.2.1/einx/nn/haiku.py
--rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-04-23 19:30:09.000000 einx-0.2.1/einx/nn/keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-04-23 19:30:09.000000 einx-0.2.1/einx/nn/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-04-23 19:30:09.000000 einx-0.2.1/einx/nn/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:30:14.763382 einx-0.2.1/einx/op/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/arange.py
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)    16570 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/elementwise.py
--rw-r--r--   0 runner    (1001) docker     (127)    19942 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/rearrange.py
--rw-r--r--   0 runner    (1001) docker     (127)    12633 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/solve.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    15807 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/vmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/vmap_with_axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-23 19:30:09.000000 einx-0.2.1/einx/traceback_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:30:14.767382 einx-0.2.1/einx/tracer/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 19:30:09.000000 einx-0.2.1/einx/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19049 2024-04-23 19:30:09.000000 einx-0.2.1/einx/tracer/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-04-23 19:30:09.000000 einx-0.2.1/einx/tracer/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-23 19:30:09.000000 einx-0.2.1/einx/tracer/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-23 19:30:09.000000 einx-0.2.1/einx/tracer/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-04-23 19:30:09.000000 einx-0.2.1/einx/tracer/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-04-23 19:30:09.000000 einx-0.2.1/einx/tracer/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-23 19:30:09.000000 einx-0.2.1/einx/tree_util.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-23 19:30:09.000000 einx-0.2.1/einx/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:30:14.767382 einx-0.2.1/einx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-23 19:30:14.000000 einx-0.2.1/einx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-23 19:30:14.000000 einx-0.2.1/einx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:30:14.000000 einx-0.2.1/einx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 19:30:14.000000 einx-0.2.1/einx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 19:30:14.000000 einx-0.2.1/einx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 19:30:14.767382 einx-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-23 19:30:09.000000 einx-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:30:14.767382 einx-0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-23 19:30:09.000000 einx-0.2.1/test/test_compare_einops.py
--rw-r--r--   0 runner    (1001) docker     (127)    10566 2024-04-23 19:30:09.000000 einx-0.2.1/test/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    31046 2024-04-23 19:30:09.000000 einx-0.2.1/test/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-23 19:30:09.000000 einx-0.2.1/test/test_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:50:21.447115 einx-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-26 09:50:15.000000 einx-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-26 09:50:21.447115 einx-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-26 09:50:15.000000 einx-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:50:21.435115 einx-0.2.2/einx/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-26 09:50:15.000000 einx-0.2.2/einx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:50:21.439115 einx-0.2.2/einx/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-26 09:50:15.000000 einx-0.2.2/einx/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-26 09:50:15.000000 einx-0.2.2/einx/backend/_dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-26 09:50:15.000000 einx-0.2.2/einx/backend/_jax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-26 09:50:15.000000 einx-0.2.2/einx/backend/_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-26 09:50:15.000000 einx-0.2.2/einx/backend/_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-04-26 09:50:15.000000 einx-0.2.2/einx/backend/_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15560 2024-04-26 09:50:15.000000 einx-0.2.2/einx/backend/_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-26 09:50:15.000000 einx-0.2.2/einx/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-26 09:50:15.000000 einx-0.2.2/einx/backend/register.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:50:21.439115 einx-0.2.2/einx/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 09:50:15.000000 einx-0.2.2/einx/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:50:21.439115 einx-0.2.2/einx/experimental/op/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-26 09:50:15.000000 einx-0.2.2/einx/experimental/op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-04-26 09:50:15.000000 einx-0.2.2/einx/experimental/op/shard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:50:21.439115 einx-0.2.2/einx/expr/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-26 09:50:15.000000 einx-0.2.2/einx/expr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9081 2024-04-26 09:50:15.000000 einx-0.2.2/einx/expr/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27957 2024-04-26 09:50:15.000000 einx-0.2.2/einx/expr/stage1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40311 2024-04-26 09:50:15.000000 einx-0.2.2/einx/expr/stage2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16913 2024-04-26 09:50:15.000000 einx-0.2.2/einx/expr/stage3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-26 09:50:15.000000 einx-0.2.2/einx/expr/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:50:21.443115 einx-0.2.2/einx/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 09:50:15.000000 einx-0.2.2/einx/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-26 09:50:15.000000 einx-0.2.2/einx/nn/equinox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-26 09:50:15.000000 einx-0.2.2/einx/nn/flax.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-26 09:50:15.000000 einx-0.2.2/einx/nn/haiku.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-04-26 09:50:15.000000 einx-0.2.2/einx/nn/keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-04-26 09:50:15.000000 einx-0.2.2/einx/nn/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-04-26 09:50:15.000000 einx-0.2.2/einx/nn/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:50:21.443115 einx-0.2.2/einx/op/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-26 09:50:15.000000 einx-0.2.2/einx/op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-26 09:50:15.000000 einx-0.2.2/einx/op/arange.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-04-26 09:50:15.000000 einx-0.2.2/einx/op/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16570 2024-04-26 09:50:15.000000 einx-0.2.2/einx/op/elementwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19942 2024-04-26 09:50:15.000000 einx-0.2.2/einx/op/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-26 09:50:15.000000 einx-0.2.2/einx/op/rearrange.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12633 2024-04-26 09:50:15.000000 einx-0.2.2/einx/op/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-26 09:50:15.000000 einx-0.2.2/einx/op/solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-26 09:50:15.000000 einx-0.2.2/einx/op/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15807 2024-04-26 09:50:15.000000 einx-0.2.2/einx/op/vmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-04-26 09:50:15.000000 einx-0.2.2/einx/op/vmap_with_axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-26 09:50:15.000000 einx-0.2.2/einx/traceback_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:50:21.443115 einx-0.2.2/einx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-26 09:50:15.000000 einx-0.2.2/einx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19166 2024-04-26 09:50:15.000000 einx-0.2.2/einx/tracer/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-04-26 09:50:15.000000 einx-0.2.2/einx/tracer/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-26 09:50:15.000000 einx-0.2.2/einx/tracer/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-26 09:50:15.000000 einx-0.2.2/einx/tracer/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-04-26 09:50:15.000000 einx-0.2.2/einx/tracer/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-26 09:50:15.000000 einx-0.2.2/einx/tracer/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-26 09:50:15.000000 einx-0.2.2/einx/tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-26 09:50:15.000000 einx-0.2.2/einx/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:50:21.447115 einx-0.2.2/einx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-26 09:50:21.000000 einx-0.2.2/einx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-26 09:50:21.000000 einx-0.2.2/einx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:50:21.000000 einx-0.2.2/einx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 09:50:21.000000 einx-0.2.2/einx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 09:50:21.000000 einx-0.2.2/einx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-26 09:50:21.447115 einx-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-26 09:50:15.000000 einx-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:50:21.447115 einx-0.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-26 09:50:15.000000 einx-0.2.2/test/test_compare_einops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-26 09:50:15.000000 einx-0.2.2/test/test_experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10566 2024-04-26 09:50:15.000000 einx-0.2.2/test/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31046 2024-04-26 09:50:15.000000 einx-0.2.2/test/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-26 09:50:15.000000 einx-0.2.2/test/test_values.py
```

### Comparing `einx-0.2.1/LICENSE` & `einx-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/PKG-INFO` & `einx-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: einx
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tensor Operations Expressed in Einstein-Inspired Notation
 Home-page: https://github.com/fferflo/einx
 Author: Florian Fervers
 Author-email: florian.fervers@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `einx-0.2.1/README.md` & `einx-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/backend/_dask.py` & `einx-0.2.2/einx/backend/_dask.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/backend/_jax.py` & `einx-0.2.2/einx/backend/_jax.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/backend/_mlx.py` & `einx-0.2.2/einx/backend/_mlx.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/backend/_numpy.py` & `einx-0.2.2/einx/backend/_numpy.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/backend/_tensorflow.py` & `einx-0.2.2/einx/backend/_tensorflow.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/backend/_torch.py` & `einx-0.2.2/einx/backend/_torch.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/backend/base.py` & `einx-0.2.2/einx/backend/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,35 +52,40 @@
     inner.__name__ = f"vmap({op.__name__ if '__name__' in dir(op) else str(op)}, "
     f"in_axes={in_axes}, out_axes={out_axes})"
 
     return inner
 
 
 _thread_local = threading.local()
-_thread_local.default_backend_stack = []
+
+
+def _get_backend_stack():
+    if not hasattr(_thread_local, "backend_stack"):
+        _thread_local.backend_stack = []
+    return _thread_local.backend_stack
 
 
 def get_default():
-    if len(_thread_local.default_backend_stack) > 0:
-        return _thread_local.default_backend_stack[-1]
+    if len(_get_backend_stack()) > 0:
+        return _get_backend_stack()[-1]
     else:
         return None
 
 
 class Backend:
     function_name = None
     decorators = []
 
     def __enter__(backend):
-        _thread_local.default_backend_stack.append(backend)
+        _get_backend_stack().append(backend)
         return backend
 
     def __exit__(backend, *args):
-        assert _thread_local.default_backend_stack[-1] is backend
-        _thread_local.default_backend_stack.pop()
+        assert _get_backend_stack()[-1] is backend
+        _get_backend_stack().pop()
 
     @staticmethod
     def _decorate_construct_graph(f):
         return f
 
     @classmethod
     @einx.trace
```

### Comparing `einx-0.2.1/einx/backend/register.py` & `einx-0.2.2/einx/backend/register.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/expr/solver.py` & `einx-0.2.2/einx/expr/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         if not isinstance(x, Expression):
             raise TypeError(f"Expected Expression, got {type(x)}")
         return x
 
 
 class SolveException(Exception):
     def __init__(self, message):
-        self.message = message
+        super().__init__(message)
 
 
 def solve(equations):
     equations = [(to_term(t1), to_term(t2)) for t1, t2 in equations]
     equations = [(t1, t2) for t1, t2 in equations if t1 != t2]
     equations = list(set(equations))
     variables = {
```

### Comparing `einx-0.2.1/einx/expr/stage1.py` & `einx-0.2.2/einx/expr/stage1.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/expr/stage2.py` & `einx-0.2.2/einx/expr/stage2.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         return Marker(self.inner.__deepcopy__(), ellipsis_indices=self.ellipsis_indices)
 
     def all(self):
         yield self
         yield from self.inner.all()
 
 
-class SolveDepthException(Exception):
+class SolveDepthException(solver.SolveException):
     def __init__(self, exprs1, exprs2, expansions1, expansions2, depths1, depths2, message):
         assert (
             len({
                 len(exprs1),
                 len(exprs2),
                 len(expansions1),
                 len(expansions2),
@@ -204,30 +204,31 @@
         )
         self.exprs1 = exprs1
         self.exprs2 = exprs2
         self.expansions1 = expansions1
         self.expansions2 = expansions2
         self.depths1 = depths1
         self.depths2 = depths2
-        self.message = (
+        message_in = message
+        message = (
             "Failed to solve for the depth of axes, i.e. the number of outer ellipses.\n"
             "Equations:\n"
         )
         for expr1, expr2 in zip(exprs1, exprs2):
             if expr1 is not None and expr2 is not None:
-                self.message += "    "
-                self.message += f"{einx.expr.util._to_str(expr1)}"
-                self.message += " = "
-                self.message += f"{einx.expr.util._to_str(expr2)}"
-                self.message += "\n"
-        self.message += f"Reason: {message}"
-        super().__init__(self.message)
+                message += "    "
+                message += f"{einx.expr.util._to_str(expr1)}"
+                message += " = "
+                message += f"{einx.expr.util._to_str(expr2)}"
+                message += "\n"
+        message += f"Reason: {message_in}"
+        super().__init__(message)
 
 
-class SolveExpansionException(Exception):
+class SolveExpansionException(solver.SolveException):
     def __init__(self, exprs1, exprs2, expansions1, expansions2, depths1, depths2, message):
         assert (
             len({
                 len(exprs1),
                 len(exprs2),
                 len(expansions1),
                 len(expansions2),
@@ -238,24 +239,25 @@
         )
         self.exprs1 = exprs1
         self.exprs2 = exprs2
         self.expansions1 = expansions1
         self.expansions2 = expansions2
         self.depths1 = depths1
         self.depths2 = depths2
-        self.message = "Failed to solve for the number of axes in the expressions.\nEquations:\n"
+        message_in = message
+        message = "Failed to solve for the number of axes in the expressions.\nEquations:\n"
         for expr1, expr2 in zip(exprs1, exprs2):
             if expr1 is not None and expr2 is not None:
-                self.message += "    "
-                self.message += f"{einx.expr.util._to_str(expr1)}"
-                self.message += " = "
-                self.message += f"{einx.expr.util._to_str(expr2)}"
-                self.message += "\n"
-        self.message += f"Reason: {message}"
-        super().__init__(self.message)
+                message += "    "
+                message += f"{einx.expr.util._to_str(expr1)}"
+                message += " = "
+                message += f"{einx.expr.util._to_str(expr2)}"
+                message += "\n"
+        message += f"Reason: {message_in}"
+        super().__init__(message)
 
 
 def solve(exprs1, exprs2, expansions1, expansions2, depths1, depths2):
     exprs1 = list(exprs1)
     exprs2 = list(exprs2)
     expansions1 = list(expansions1)
     expansions2 = list(expansions2)
```

### Comparing `einx-0.2.1/einx/expr/stage3.py` & `einx-0.2.2/einx/expr/stage3.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,24 +219,22 @@
         return 6433236 + hash(self.inner)
 
     def all(self):
         yield self
         yield from self.inner.all()
 
 
-class SolveValueException(Exception):
+class SolveValueException(solver.SolveException):
     def __init__(self, exprs1, exprs2, message):
         self.exprs1 = exprs1
         self.exprs2 = exprs2
-        self.message = f"Failed to solve values of expressions. {message}\nInput:\n"
+        message = f"Failed to solve values of expressions. {message}\nInput:\n"
         for expr1, expr2 in zip(exprs1, exprs2):
-            self.message += (
-                f"    '{einx.expr.util._to_str(expr1)} = {einx.expr.util._to_str(expr2)}'\n"
-            )
-        super().__init__(self.message)
+            message += f"    '{einx.expr.util._to_str(expr1)} = {einx.expr.util._to_str(expr2)}'\n"
+        super().__init__(message)
 
 
 def solve(exprs1, exprs2):
     exprs1 = list(exprs1)
     exprs2 = list(exprs2)
     if any(
         expr is not None and not isinstance(expr, stage2.Expression) for expr in exprs1 + exprs2
```

### Comparing `einx-0.2.1/einx/expr/util.py` & `einx-0.2.2/einx/expr/util.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/nn/equinox.py` & `einx-0.2.2/einx/nn/equinox.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/nn/flax.py` & `einx-0.2.2/einx/nn/flax.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/nn/haiku.py` & `einx-0.2.2/einx/nn/haiku.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/nn/keras.py` & `einx-0.2.2/einx/nn/keras.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/nn/nn.py` & `einx-0.2.2/einx/nn/nn.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/nn/torch.py` & `einx-0.2.2/einx/nn/torch.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/op/arange.py` & `einx-0.2.2/einx/op/arange.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/op/dot.py` & `einx-0.2.2/einx/op/dot.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/op/elementwise.py` & `einx-0.2.2/einx/op/elementwise.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/op/index.py` & `einx-0.2.2/einx/op/index.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/op/rearrange.py` & `einx-0.2.2/einx/op/rearrange.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/op/reduce.py` & `einx-0.2.2/einx/op/reduce.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/op/solve.py` & `einx-0.2.2/einx/op/solve.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/op/util.py` & `einx-0.2.2/einx/op/util.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/op/vmap.py` & `einx-0.2.2/einx/op/vmap.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/op/vmap_with_axis.py` & `einx-0.2.2/einx/op/vmap_with_axis.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/traceback_util.py` & `einx-0.2.2/einx/traceback_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,30 @@
 
 
 def include_frame(fname):
     return not fname.startswith(path)
 
 
 thread_local = threading.local()
-thread_local.in_reraise = False
+
+
+def _set_in_reraise():
+    if not hasattr(thread_local, "in_reraise"):
+        thread_local.in_reraise = False
+    assert not thread_local.in_reraise
+    thread_local.in_reraise = True
+
+
+def _unset_in_reraise():
+    assert thread_local.in_reraise
+    thread_local.in_reraise = False
+
+
+def _is_in_reraise():
+    return getattr(thread_local, "in_reraise", False)
 
 
 def _filter_tb(tb):
     tb_list = list(traceback.walk_tb(tb))
     first_excluded_idx = 0
     while first_excluded_idx < len(tb_list) and include_frame(
         tb_list[first_excluded_idx][0].f_code.co_filename
@@ -42,24 +57,24 @@
 def filter(func):
     filter = os.environ.get("EINX_FILTER_TRACEBACK", "true").lower() in ("true", "yes", "1")
 
     if filter:
 
         @functools.wraps(func)
         def func_with_reraise(*args, **kwargs):
-            if not thread_local.in_reraise:
-                thread_local.in_reraise = True
+            if not _is_in_reraise():
+                _set_in_reraise()
                 tb = None
                 try:
                     return func(*args, **kwargs)
                 except Exception as e:
                     tb = _filter_tb(e.__traceback__)
                     raise e.with_traceback(tb) from None
                 finally:
                     del tb
-                    thread_local.in_reraise = False
+                    _unset_in_reraise()
             else:
                 return func(*args, **kwargs)
 
         return func_with_reraise
     else:
         return func
```

### Comparing `einx-0.2.1/einx/tracer/compile.py` & `einx-0.2.2/einx/tracer/compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,19 +209,21 @@
 
         # Find block at which to execute the application (i.e. where all dependencies are defined)
         in_defs = [self.get_definition_of(x) for x in application.dependencies]
         block = self.join_blocks([d.block for d in in_defs])
 
         use_dynamic_output_check = False
         if isinstance(application.op, Import):
-            import_str = f"import {application.op.module}"
-            name = application.op.module
-            if not application.op.shorthand is None:
-                import_str += f" as {application.op.shorthand}"
-                name = application.op.shorthand
+            import_str = f"import {application.op.import_}"
+            name = application.op.import_
+            if not application.op.as_ is None:
+                import_str = f"{import_str} as {application.op.as_}"
+                name = application.op.as_
+            if not application.op.from_ is None:
+                import_str = f"from {application.op.from_} {import_str}"
 
             # Import only once
             if not any(
                 isinstance(line, str)
                 and (line == import_str or line.startswith(import_str + "  #"))
                 for line in block.code
             ):
```

### Comparing `einx-0.2.1/einx/tracer/decorator.py` & `einx-0.2.2/einx/tracer/decorator.py`

 * *Files 9% similar despite different names*

```diff
@@ -108,31 +108,36 @@
             func = functools.lru_cache(maxsize=None)(func)
     func = freeze(func)
 
     return func
 
 
 _thread_local = threading.local()
-_thread_local.stack = []
+
+
+def _get_trace_stack():
+    if not hasattr(_thread_local, "stack"):
+        _thread_local.stack = []
+    return _thread_local.stack
 
 
 class _trace_context:
     def __init__(self, backend):
         self.backend = backend
 
     def __enter__(self):
-        _thread_local.stack.append(self)
+        _get_trace_stack().append(self)
 
     def __exit__(self, *args):
-        assert id(_thread_local.stack[-1]) == id(self)
-        _thread_local.stack.pop()
+        assert id(_get_trace_stack()[-1]) == id(self)
+        _get_trace_stack().pop()
 
 
 def _is_tracing():
-    return len(_thread_local.stack) > 0
+    return len(_get_trace_stack()) > 0
 
 
 trace_all = lambda t, c: lambda *args, **kwargs: c(
     *[t(arg) for arg in args], **{k: t(v) for k, v in kwargs.items()}
 )
 trace_none = lambda t, c: lambda *args, **kwargs: c(args, kwargs)
 
@@ -183,16 +188,16 @@
     has_decorated = False
 
     @functools.wraps(func)
     def func_jit(*args, backend=None, graph=False, **kwargs):
         if _is_tracing():
             assert not graph
             if backend is None:
-                backend = _thread_local.stack[-1].backend
-            elif backend != _thread_local.stack[-1].backend:
+                backend = _get_trace_stack()[-1].backend
+            elif backend != _get_trace_stack()[-1].backend:
                 raise ValueError("Cannot change backend during tracing")
 
             return func(*args, backend=backend, **kwargs)
 
         return_graph = graph
 
         # Replace concrete values with tracers
```

### Comparing `einx-0.2.1/einx/tracer/input.py` & `einx-0.2.2/einx/tracer/input.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/tracer/optimize.py` & `einx-0.2.2/einx/tracer/optimize.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/tracer/tensor.py` & `einx-0.2.2/einx/tracer/tensor.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx/tracer/tracer.py` & `einx-0.2.2/einx/tracer/tracer.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,32 +80,37 @@
             op,
             args=args,
             kwargs=kwargs,
             output=output,
             signature=signature,
             inplace_updates=inplace_updates,
             comment=comment,
-            depend_on=depend_on + _thread_local.depend_on,
+            depend_on=depend_on + _get_depend_on_stack(),
         ).output
 
 
 _thread_local = threading.local()
-_thread_local.depend_on = []
+
+
+def _get_depend_on_stack():
+    if not hasattr(_thread_local, "depend_on"):
+        _thread_local.depend_on = []
+    return _thread_local.depend_on
 
 
 class depend_on:
     def __init__(self, tracers):
         self.tracer = list(einx.tree_util.tree_flatten(tracers))
 
     def __enter__(self):
-        _thread_local.depend_on.append(self.tracer)
+        _get_depend_on_stack().append(self.tracer)
 
     def __exit__(self, *args):
-        assert _thread_local.depend_on[-1] is self.tracer
-        _thread_local.depend_on.pop()
+        assert _get_depend_on_stack()[-1] is self.tracer
+        _get_depend_on_stack().pop()
 
 
 class Tracer:
     def __init__(self, origin=None):
         self.origin = origin
 
     def __getattr__(self, key):
@@ -122,25 +127,26 @@
 
     def __copy__(self):
         assert type(self) == Tracer
         return Tracer()
 
 
 class Import(Tracer):
-    def __init__(self, module, shorthand=None):
+    def __init__(self, import_, as_, from_):
         Tracer.__init__(self, origin="constant")
-        self.module = module
-        self.shorthand = shorthand
+        self.import_ = import_
+        self.as_ = as_
+        self.from_ = from_
 
     def __call__(self):  # Overwrite allowed arguments
         return apply(self)
 
 
-def import_(module, shorthand=None):
-    return Import(module, shorthand)()
+def import_(import_, as_=None, from_=None):
+    return Import(import_, as_, from_)()
 
 
 class MemberAccess(Tracer):
     def __init__(self):
         Tracer.__init__(self, origin="constant")
 
     def __call__(self, obj, key):  # Overwrite allowed arguments
```

### Comparing `einx-0.2.1/einx/tree_util.py` & `einx-0.2.2/einx/tree_util.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/einx.egg-info/PKG-INFO` & `einx-0.2.2/einx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: einx
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tensor Operations Expressed in Einstein-Inspired Notation
 Home-page: https://github.com/fferflo/einx
 Author: Florian Fervers
 Author-email: florian.fervers@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `einx-0.2.1/einx.egg-info/SOURCES.txt` & `einx-0.2.2/einx.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 einx/backend/_jax.py
 einx/backend/_mlx.py
 einx/backend/_numpy.py
 einx/backend/_tensorflow.py
 einx/backend/_torch.py
 einx/backend/base.py
 einx/backend/register.py
+einx/experimental/__init__.py
+einx/experimental/op/__init__.py
+einx/experimental/op/shard.py
 einx/expr/__init__.py
 einx/expr/solver.py
 einx/expr/stage1.py
 einx/expr/stage2.py
 einx/expr/stage3.py
 einx/expr/util.py
 einx/nn/__init__.py
@@ -48,10 +51,11 @@
 einx/tracer/compile.py
 einx/tracer/decorator.py
 einx/tracer/input.py
 einx/tracer/optimize.py
 einx/tracer/tensor.py
 einx/tracer/tracer.py
 test/test_compare_einops.py
+test/test_experimental.py
 test/test_nn.py
 test/test_shapes.py
 test/test_values.py
```

### Comparing `einx-0.2.1/setup.py` & `einx-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="einx",
-    version="0.2.1",
+    version="0.2.2",
     python_requires=">=3.8",
     description="Tensor Operations Expressed in Einstein-Inspired Notation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Florian Fervers",
     author_email="florian.fervers@gmail.com",
     url="https://github.com/fferflo/einx",
```

### Comparing `einx-0.2.1/test/test_compare_einops.py` & `einx-0.2.2/test/test_compare_einops.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/test/test_nn.py` & `einx-0.2.2/test/test_nn.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/test/test_shapes.py` & `einx-0.2.2/test/test_shapes.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.1/test/test_values.py` & `einx-0.2.2/test/test_values.py`

 * *Files identical despite different names*

