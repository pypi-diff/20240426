# Comparing `tmp/ricciardi-0.1.1.tar.gz` & `tmp/ricciardi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ricciardi-0.1.1.tar", last modified: Sun Apr 21 19:02:10 2024, max compression
+gzip compressed data, was "ricciardi-0.1.2.tar", last modified: Thu Apr 25 22:35:44 2024, max compression
```

## Comparing `ricciardi-0.1.1.tar` & `ricciardi-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:02:10.579081 ricciardi-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-21 19:02:06.000000 ricciardi-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-21 19:02:10.579081 ricciardi-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-21 19:02:06.000000 ricciardi-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-21 19:02:06.000000 ricciardi-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:02:10.579081 ricciardi-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:02:10.575081 ricciardi-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:02:10.575081 ricciardi-0.1.1/src/ricciardi/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-21 19:02:06.000000 ricciardi-0.1.1/src/ricciardi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-21 19:02:06.000000 ricciardi-0.1.1/src/ricciardi/ricciardi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:02:10.575081 ricciardi-0.1.1/src/ricciardi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-21 19:02:10.000000 ricciardi-0.1.1/src/ricciardi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-21 19:02:10.000000 ricciardi-0.1.1/src/ricciardi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:02:10.000000 ricciardi-0.1.1/src/ricciardi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 19:02:10.000000 ricciardi-0.1.1/src/ricciardi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 19:02:10.000000 ricciardi-0.1.1/src/ricciardi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:02:10.575081 ricciardi-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-21 19:02:06.000000 ricciardi-0.1.1/test/test_ricciardi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:35:44.491787 ricciardi-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-25 22:35:40.000000 ricciardi-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-25 22:35:44.491787 ricciardi-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-25 22:35:40.000000 ricciardi-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-25 22:35:40.000000 ricciardi-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 22:35:44.491787 ricciardi-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:35:44.487787 ricciardi-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:35:44.487787 ricciardi-0.1.2/src/ricciardi/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 22:35:40.000000 ricciardi-0.1.2/src/ricciardi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-25 22:35:40.000000 ricciardi-0.1.2/src/ricciardi/ricciardi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:35:44.491787 ricciardi-0.1.2/src/ricciardi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-25 22:35:44.000000 ricciardi-0.1.2/src/ricciardi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-25 22:35:44.000000 ricciardi-0.1.2/src/ricciardi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 22:35:44.000000 ricciardi-0.1.2/src/ricciardi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 22:35:44.000000 ricciardi-0.1.2/src/ricciardi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 22:35:44.000000 ricciardi-0.1.2/src/ricciardi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:35:44.491787 ricciardi-0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-25 22:35:40.000000 ricciardi-0.1.2/test/test_ricciardi.py
```

### Comparing `ricciardi-0.1.1/LICENSE` & `ricciardi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ricciardi-0.1.1/PKG-INFO` & `ricciardi-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ricciardi
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyTorch implementation of the Ricciardi transfer function.
 Author: Ho Yin Chau
 License: MIT License
         
         Copyright (c) 2023 hchau630
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ricciardi-0.1.1/README.md` & `ricciardi-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ricciardi-0.1.1/pyproject.toml` & `ricciardi-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0"]  # editable install using setuptool available since v64.0.0
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ricciardi"
-version = "0.1.1"
+version = "0.1.2"
 description = "PyTorch implementation of the Ricciardi transfer function."
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     {name = "Ho Yin Chau"},
 ]
 classifiers = [
```

### Comparing `ricciardi-0.1.1/src/ricciardi/ricciardi.py` & `ricciardi-0.1.2/src/ricciardi/ricciardi.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,41 +70,51 @@
     Returns:
         torch.Tensor: Tensor with shape broadcast(x, y).shape
 
     """
     return Ierfcx.apply(x, y, n)
 
 
-def ricciardi(mu, sigma=0.01, tau=0.02, tau_rp=0.002, V_r=0.01, theta=0.02):
+def ricciardi(mu, sigma=0.01, tau=0.02, tau_rp=0.002, V_r=0.01, theta=0.02, n=None):
     """Ricciardi transfer function.
 
     Computes the firing rate of an LIF neuron as a function of the mean and variance
     of the presynaptic input current, with default values and notation following
     Sanzeni et al. (2020). Default values assume SI units (i.e. seconds and volts).
 
     Args:
         mu (torch.Tensor): Mean of presynaptic input current.
         sigma (float | torch.Tensor, optional): Standard deviation of presynaptic input current.
         tau (float | torch.Tensor, optional): Time constant of the membrane potential.
         tau_rp (float | torch.Tensor, optional): Refractory period.
         V_r (float | torch.Tensor, optional): Reset membrane potential.
         theta (float | torch.Tensor, optional): Firing threshold membrane potential.
+        n (int, optional):
+            Precision level, roughly equivalent to the order of Gauss-Legendre quadrature used to compute
+            the integral of the complementary error function. If None, defaults to 4, 5, or 6 for
+            input dtypes torch.half, torch.float, and torch.double, respectively.
 
     Returns:
         torch.Tensor: Tensor of firing rates with shape broadcast(mu, sigma, tau, tau_rp, V_r, theta).shape
 
     """
-    u_min = (V_r - mu) / sigma
-    u_max = (theta - mu) / sigma
+    dtype = mu.dtype
+    if n is None:
+        n = {torch.half: 4, torch.float: 5, torch.double: 6}[dtype]
 
-    if (-u_min).min() > -10:
+    mu = mu.float() if n <= 5 else mu.double()
+
+    umin = (V_r - mu) / sigma
+    umax = (theta - mu) / sigma
+
+    if (-umin).min() > -10:
         # slightly faster path when there is no extreme value
-        out = 1.0 / (tau_rp + tau * sqrtpi * ierfcx(-u_max, -u_min))
+        out = 1 / (tau_rp + tau * sqrtpi * ierfcx(-umax, -umin, n=n))
     else:
         # Handle extreme values separately to avoid numerical issues
-        mask = -u_min > -10
+        mask = -umin > -10
         out = torch.empty_like(mu)
-        out[mask] = 1.0 / (tau_rp + tau * sqrtpi * ierfcx(-u_max[mask], -u_min[mask]))
-        u = u_max[~mask]
+        out[mask] = 1 / (tau_rp + tau * sqrtpi * ierfcx(-umax[mask], -umin[mask], n=n))
+        u = umax[~mask]
         out[~mask] = u * torch.exp(-(u**2)) / (tau * sqrtpi)
 
-    return out
+    return out.to(dtype)
```

### Comparing `ricciardi-0.1.1/src/ricciardi.egg-info/PKG-INFO` & `ricciardi-0.1.2/src/ricciardi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ricciardi
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyTorch implementation of the Ricciardi transfer function.
 Author: Ho Yin Chau
 License: MIT License
         
         Copyright (c) 2023 hchau630
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ricciardi-0.1.1/test/test_ricciardi.py` & `ricciardi-0.1.2/test/test_ricciardi.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,18 +27,20 @@
 @pytest.mark.parametrize(
     "x",
     [
         torch.linspace(-0.01, 0.1, 1001),
         torch.linspace(-10.0, 50.0, 1001),
     ],
 )
-def test_ricciardi(x, params):
+@pytest.mark.parametrize("dtype", [torch.half, torch.float, torch.double])
+def test_ricciardi(x, params, dtype):
+    x = x.to(dtype)
     out = ricciardi(x, **params)
     expected = ricciardi_exact(x.double().numpy(), **params)
-    expected = torch.from_numpy(expected).float().nan_to_num()
+    expected = torch.from_numpy(expected).to(dtype).nan_to_num()
     torch.testing.assert_close(out, expected)
 
 
 @pytest.mark.parametrize(
     "x",
     [
         torch.linspace(-0.01, 0.1, 1001, requires_grad=True).double(),
```

