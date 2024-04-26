# Comparing `tmp/deepbays-0.0.1.tar.gz` & `tmp/deepbays-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepbays-0.0.1.tar", last modified: Wed Apr 24 20:30:29 2024, max compression
+gzip compressed data, was "deepbays-0.0.3.tar", last modified: Fri Apr 26 10:48:40 2024, max compression
```

## Comparing `deepbays-0.0.1.tar` & `deepbays-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 rosalba    (501) staff       (20)        0 2024-04-24 20:30:29.307853 deepbays-0.0.1/
--rw-r--r--   0 rosalba    (501) staff       (20)      481 2024-04-24 20:30:29.307632 deepbays-0.0.1/PKG-INFO
-drwxr-xr-x   0 rosalba    (501) staff       (20)        0 2024-04-24 20:30:29.304960 deepbays-0.0.1/deepbays/
-drwxr-xr-x   0 rosalba    (501) staff       (20)        0 2024-04-24 20:30:29.306326 deepbays-0.0.1/deepbays/NN/
--rw-r--r--   0 rosalba    (501) staff       (20)      191 2024-04-18 14:22:31.000000 deepbays-0.0.1/deepbays/NN/__init__.py
--rw-r--r--   0 rosalba    (501) staff       (20)     2076 2024-04-02 07:52:33.000000 deepbays-0.0.1/deepbays/NN/networks.py
--rw-r--r--   0 rosalba    (501) staff       (20)     4677 2024-04-18 20:35:49.000000 deepbays-0.0.1/deepbays/NN/training.py
--rw-r--r--   0 rosalba    (501) staff       (20)      201 2024-04-24 20:12:20.000000 deepbays-0.0.1/deepbays/__init__.py
--rw-r--r--   0 rosalba    (501) staff       (20)     1477 2024-04-24 20:04:25.000000 deepbays-0.0.1/deepbays/kernels.py
-drwxr-xr-x   0 rosalba    (501) staff       (20)        0 2024-04-24 20:30:29.307051 deepbays-0.0.1/deepbays/tasks/
--rw-r--r--   0 rosalba    (501) staff       (20)       99 2024-04-11 14:57:39.000000 deepbays-0.0.1/deepbays/tasks/__init__.py
--rw-r--r--   0 rosalba    (501) staff       (20)    10851 2024-04-12 20:53:10.000000 deepbays-0.0.1/deepbays/tasks/tasks.py
--rw-r--r--   0 rosalba    (501) staff       (20)     2315 2024-04-24 20:10:40.000000 deepbays-0.0.1/deepbays/theory_1HL_FC.py
--rw-r--r--   0 rosalba    (501) staff       (20)     3019 2024-04-24 20:11:31.000000 deepbays-0.0.1/deepbays/theory_deep_FC.py
--rw-r--r--   0 rosalba    (501) staff       (20)     7920 2024-04-24 20:11:21.000000 deepbays-0.0.1/deepbays/theory_multitask.py
-drwxr-xr-x   0 rosalba    (501) staff       (20)        0 2024-04-24 20:30:29.307393 deepbays-0.0.1/deepbays.egg-info/
--rw-r--r--   0 rosalba    (501) staff       (20)      481 2024-04-24 20:30:29.000000 deepbays-0.0.1/deepbays.egg-info/PKG-INFO
--rw-r--r--   0 rosalba    (501) staff       (20)      413 2024-04-24 20:30:29.000000 deepbays-0.0.1/deepbays.egg-info/SOURCES.txt
--rw-r--r--   0 rosalba    (501) staff       (20)        1 2024-04-24 20:30:29.000000 deepbays-0.0.1/deepbays.egg-info/dependency_links.txt
--rw-r--r--   0 rosalba    (501) staff       (20)       30 2024-04-24 20:30:29.000000 deepbays-0.0.1/deepbays.egg-info/requires.txt
--rw-r--r--   0 rosalba    (501) staff       (20)        9 2024-04-24 20:30:29.000000 deepbays-0.0.1/deepbays.egg-info/top_level.txt
--rw-r--r--   0 rosalba    (501) staff       (20)       38 2024-04-24 20:30:29.307905 deepbays-0.0.1/setup.cfg
--rw-r--r--   0 rosalba    (501) staff       (20)      916 2024-04-11 12:19:41.000000 deepbays-0.0.1/setup.py
+drwxr-xr-x   0 rosalba    (501) staff       (20)        0 2024-04-26 10:48:40.838388 deepbays-0.0.3/
+-rw-r--r--   0 rosalba    (501) staff       (20)      481 2024-04-26 10:48:40.838190 deepbays-0.0.3/PKG-INFO
+drwxr-xr-x   0 rosalba    (501) staff       (20)        0 2024-04-26 10:48:40.836497 deepbays-0.0.3/deepbays/
+drwxr-xr-x   0 rosalba    (501) staff       (20)        0 2024-04-26 10:48:40.837478 deepbays-0.0.3/deepbays/NN/
+-rw-r--r--   0 rosalba    (501) staff       (20)      191 2024-04-18 14:22:31.000000 deepbays-0.0.3/deepbays/NN/__init__.py
+-rw-r--r--   0 rosalba    (501) staff       (20)     2075 2024-04-24 20:36:28.000000 deepbays-0.0.3/deepbays/NN/networks.py
+-rw-r--r--   0 rosalba    (501) staff       (20)     4677 2024-04-18 20:35:49.000000 deepbays-0.0.3/deepbays/NN/training.py
+-rw-r--r--   0 rosalba    (501) staff       (20)      201 2024-04-24 20:12:20.000000 deepbays-0.0.3/deepbays/__init__.py
+-rw-r--r--   0 rosalba    (501) staff       (20)     1477 2024-04-24 20:04:25.000000 deepbays-0.0.3/deepbays/kernels.py
+drwxr-xr-x   0 rosalba    (501) staff       (20)        0 2024-04-26 10:48:40.837763 deepbays-0.0.3/deepbays/tasks/
+-rw-r--r--   0 rosalba    (501) staff       (20)       99 2024-04-11 14:57:39.000000 deepbays-0.0.3/deepbays/tasks/__init__.py
+-rw-r--r--   0 rosalba    (501) staff       (20)    10851 2024-04-12 20:53:10.000000 deepbays-0.0.3/deepbays/tasks/tasks.py
+-rw-r--r--   0 rosalba    (501) staff       (20)     2315 2024-04-24 20:10:40.000000 deepbays-0.0.3/deepbays/theory_1HL_FC.py
+-rw-r--r--   0 rosalba    (501) staff       (20)     2959 2024-04-24 21:29:41.000000 deepbays-0.0.3/deepbays/theory_deep_FC.py
+-rw-r--r--   0 rosalba    (501) staff       (20)     7920 2024-04-24 20:11:21.000000 deepbays-0.0.3/deepbays/theory_multitask.py
+drwxr-xr-x   0 rosalba    (501) staff       (20)        0 2024-04-26 10:48:40.838001 deepbays-0.0.3/deepbays.egg-info/
+-rw-r--r--   0 rosalba    (501) staff       (20)      481 2024-04-26 10:48:40.000000 deepbays-0.0.3/deepbays.egg-info/PKG-INFO
+-rw-r--r--   0 rosalba    (501) staff       (20)      413 2024-04-26 10:48:40.000000 deepbays-0.0.3/deepbays.egg-info/SOURCES.txt
+-rw-r--r--   0 rosalba    (501) staff       (20)        1 2024-04-26 10:48:40.000000 deepbays-0.0.3/deepbays.egg-info/dependency_links.txt
+-rw-r--r--   0 rosalba    (501) staff       (20)       30 2024-04-26 10:48:40.000000 deepbays-0.0.3/deepbays.egg-info/requires.txt
+-rw-r--r--   0 rosalba    (501) staff       (20)        9 2024-04-26 10:48:40.000000 deepbays-0.0.3/deepbays.egg-info/top_level.txt
+-rw-r--r--   0 rosalba    (501) staff       (20)       38 2024-04-26 10:48:40.838438 deepbays-0.0.3/setup.cfg
+-rw-r--r--   0 rosalba    (501) staff       (20)      916 2024-04-26 10:48:15.000000 deepbays-0.0.3/setup.py
```

### Comparing `deepbays-0.0.1/deepbays/NN/networks.py` & `deepbays-0.0.3/deepbays/NN/networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import torch, torch.nn as nn
 import torch.backends.cudnn as cudnn
 import torch.nn.init as init
 import torch.optim as optim
 from torch import nn
 from torch.optim import Optimizer
 
-
 class Erf(torch.nn.Module):
     def __init__(self):
         super().__init__()
     def forward(self, x):
         return torch.erf(x)
 
 class Id(torch.nn.Module):
```

### Comparing `deepbays-0.0.1/deepbays/NN/training.py` & `deepbays-0.0.3/deepbays/NN/training.py`

 * *Files identical despite different names*

### Comparing `deepbays-0.0.1/deepbays/kernels.py` & `deepbays-0.0.3/deepbays/kernels.py`

 * *Files identical despite different names*

### Comparing `deepbays-0.0.1/deepbays/tasks/tasks.py` & `deepbays-0.0.3/deepbays/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `deepbays-0.0.1/deepbays/theory_1HL_FC.py` & `deepbays-0.0.3/deepbays/theory_1HL_FC.py`

 * *Files identical despite different names*

### Comparing `deepbays-0.0.1/deepbays/theory_deep_FC.py` & `deepbays-0.0.3/deepbays/theory_deep_FC.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import numpy as np
 from scipy.optimize import fsolve
-from kernels import kernel_erf, kernel_relu, kernel_id, computeKmatrix, computeKmatrixTorch, kernel_erf_torch
-import time, torch
-from functools import reduce
-from copy import deepcopy
+from .kernels import kernel_erf, kernel_relu, kernel_id, computeKmatrix, computeKmatrixTorch, kernel_erf_torch
+import torch
 
 class prop_width_GP_deep_FC():
     def __init__(self, N1, l0, l1, act, T, L):
         self.N1 = N1
         self.l0 = l0
         self.l1 = l1 
         self.T = T
```

### Comparing `deepbays-0.0.1/deepbays/theory_multitask.py` & `deepbays-0.0.3/deepbays/theory_multitask.py`

 * *Files identical despite different names*

### Comparing `deepbays-0.0.1/setup.py` & `deepbays-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'Bayesian deep neural networks in the proportional regime'
 LONG_DESCRIPTION = 'Compute expected predictor of a Bayesian deep neural networks in the proportional regime in a non-parametric way using the equivalent GP'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name='deepbays',
```

