# Comparing `tmp/jsmfsb-0.0.4.tar.gz` & `tmp/jsmfsb-0.0.5.tar.gz`

## Comparing `jsmfsb-0.0.4.tar` & `jsmfsb-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,54 @@
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/.readthedocs.yaml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/Makefile
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/demos/Makefile
--rw-r--r--   0        0        0    12569 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/demos/lv.pdf
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/demos/lv.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/demos/lv.txt
--rw-r--r--   0        0        0     8088 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/demos/lvH.pdf
--rw-r--r--   0        0        0    11053 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/demos/shbuild.pdf
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/demos/shbuild.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/demos/shbuild.txt
--rw-r--r--   0        0        0     9250 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/demos/shbuildH.pdf
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/docs/Makefile
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/docs/conf.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/docs/make.bat
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/docs/requirements.txt
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/docs/source/jsmfsb.rst
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/docs/source/modules.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/src/jsmfsb/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/src/jsmfsb/models.py
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/src/jsmfsb/sim.py
--rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/src/jsmfsb/smfsbSbml.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/src/jsmfsb/spn.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/tests/test_sim.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/tests/test_spn.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/LICENSE
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/README.md
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/.readthedocs.yaml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/Makefile
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/Makefile
+-rw-r--r--   0        0        0     8088 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/lv.pdf
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/lv.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/lv.txt
+-rw-r--r--   0        0        0     7727 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/m-bd.pdf
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/m-bd.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/m-bd.txt
+-rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/m-dimer.pdf
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/m-dimer.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/m-dimer.txt
+-rw-r--r--   0        0        0     7625 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/m-id.pdf
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/m-id.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/m-id.txt
+-rw-r--r--   0        0        0    12569 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/m-lv.pdf
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/m-lv.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/m-lv.txt
+-rw-r--r--   0        0        0    14775 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/m-mm.pdf
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/m-mm.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/m-mm.txt
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/m-sir.pdf
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/m-sir.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/m-sir.txt
+-rw-r--r--   0        0        0    11053 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/shbuild.pdf
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/shbuild.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/shbuild.txt
+-rw-r--r--   0        0        0     9250 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/shbuildH.pdf
+-rw-r--r--   0        0        0     8155 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/time-lv-cle.pdf
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/time-lv-cle.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/time-lv-cle.txt
+-rw-r--r--   0        0        0     8634 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/time-lv-gillespie.pdf
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/time-lv-gillespie.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/demos/time-lv-gillespie.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/docs/Makefile
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/docs/conf.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/docs/make.bat
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/docs/requirements.txt
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/docs/source/jsmfsb.rst
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/docs/source/modules.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/src/jsmfsb/__init__.py
+-rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/src/jsmfsb/models.py
+-rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/src/jsmfsb/sim.py
+-rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/src/jsmfsb/smfsbSbml.py
+-rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/src/jsmfsb/spn.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/tests/test_models.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/tests/test_sim.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/tests/test_spn.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/README.md
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 jsmfsb-0.0.5/PKG-INFO
```

### Comparing `jsmfsb-0.0.4/.readthedocs.yaml` & `jsmfsb-0.0.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.4/demos/lv.pdf` & `jsmfsb-0.0.5/demos/m-lv.pdf`

 * *Files 0% similar despite different names*

#### Comparing `jsmfsb-0.0.4/demos/lv.pdf` & `jsmfsb-0.0.5/demos/m-lv.pdf`

 * *Document info*

```diff
@@ -1,3 +1,3 @@
-CreationDate: "D:20240420231036+01'00'"
+CreationDate: "D:20240426170206+01'00'"
 Creator: 'Matplotlib v3.8.4, https://matplotlib.org'
 Producer: 'Matplotlib pdf backend v3.8.4'
```

### Comparing `jsmfsb-0.0.4/demos/lv.py` & `jsmfsb-0.0.5/demos/m-sir.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,29 @@
 #!/usr/bin/env python3
-# lv.py
+# m-sir.py
 # use a pre-defined model
 
 import jax
 import jax.numpy as jnp
 import jax.scipy as jsp
 import jax.lax as jl
 from jax import grad, jit
 
 import jsmfsb
 
-lvmod = jsmfsb.models.lv()
-step = lvmod.stepGillespie()
+sirmod = jsmfsb.models.sir()
+step = sirmod.stepGillespie()
 k0 = jax.random.key(42)
-print(step(k0, lvmod.m, 0, 30))
+print(step(k0, sirmod.m, 0, 30))
 
-stepC = lvmod.stepCLE(0.01)
-print(stepC(k0, lvmod.m, 0, 30))
-
-
-# simTs
-out = jsmfsb.simTs(k0, lvmod.m, 0, 30, 0.1, step)
+out = jsmfsb.simTs(k0, sirmod.m, 0, 100, 0.1, step)
 
 import matplotlib.pyplot as plt
 fig, axis = plt.subplots()
-for i in range(2):
+for i in range(3):
 	axis.plot(range(out.shape[0]), out[:,i])
 
-axis.legend(lvmod.n)
-fig.savefig("lv.pdf")
-
-# simSample
-out = jsmfsb.simSample(k0, 10000, lvmod.m, 0, 30, stepC)
-out = jnp.where(out > 1000, 1000, out)
-import scipy as sp
-print(sp.stats.describe(out))
-fig, axes = plt.subplots(2,1)
-for i in range(2):
-    axes[i].hist(out[:,i], bins=50)
-fig.savefig("lvH.pdf")
+axis.legend(sirmod.n)
+fig.savefig("m-sir.pdf")
 
 # eof
```

### Comparing `jsmfsb-0.0.4/demos/lvH.pdf` & `jsmfsb-0.0.5/demos/lv.pdf`

 * *Files 2% similar despite different names*

#### Comparing `jsmfsb-0.0.4/demos/lvH.pdf` & `jsmfsb-0.0.5/demos/lv.pdf`

 * *Document info*

```diff
@@ -1,3 +1,3 @@
-CreationDate: "D:20240420231042+01'00'"
+CreationDate: "D:20240426165712+01'00'"
 Creator: 'Matplotlib v3.8.4, https://matplotlib.org'
 Producer: 'Matplotlib pdf backend v3.8.4'
```

### Comparing `jsmfsb-0.0.4/demos/shbuild.pdf` & `jsmfsb-0.0.5/demos/shbuild.pdf`

 * *Files 0% similar despite different names*

#### Comparing `jsmfsb-0.0.4/demos/shbuild.pdf` & `jsmfsb-0.0.5/demos/shbuild.pdf`

 * *Document info*

```diff
@@ -1,3 +1,3 @@
-CreationDate: "D:20240420231043+01'00'"
+CreationDate: "D:20240426165717+01'00'"
 Creator: 'Matplotlib v3.8.4, https://matplotlib.org'
 Producer: 'Matplotlib pdf backend v3.8.4'
```

### Comparing `jsmfsb-0.0.4/demos/shbuild.py` & `jsmfsb-0.0.5/demos/shbuild.py`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.4/demos/shbuildH.pdf` & `jsmfsb-0.0.5/demos/shbuildH.pdf`

 * *Files 1% similar despite different names*

#### Comparing `jsmfsb-0.0.4/demos/shbuildH.pdf` & `jsmfsb-0.0.5/demos/shbuildH.pdf`

 * *Document info*

```diff
@@ -1,3 +1,3 @@
-CreationDate: "D:20240420231044+01'00'"
+CreationDate: "D:20240426165721+01'00'"
 Creator: 'Matplotlib v3.8.4, https://matplotlib.org'
 Producer: 'Matplotlib pdf backend v3.8.4'
```

### Comparing `jsmfsb-0.0.4/docs/Makefile` & `jsmfsb-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.4/docs/conf.py` & `jsmfsb-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.4/docs/make.bat` & `jsmfsb-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.4/docs/source/jsmfsb.rst` & `jsmfsb-0.0.5/docs/source/jsmfsb.rst`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.4/src/jsmfsb/sim.py` & `jsmfsb-0.0.5/src/jsmfsb/sim.py`

 * *Files 26% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         The terminal time of the simulation.
     dt: float
         The time step of the output. Note that this time step relates only to
         the recorded output, and has no bearing on the accuracy of the simulation
         process.
     stepFun: function
         A function (closure) for advancing the state of the process,
-        such as produced by ‘stepGillespie’ or ‘stepEuler’.
+        such as produced by ‘stepGillespie’ or ‘stepCLE’.
 
     Returns
     -------
     A matrix with rows representing the state of the system at successive times.
 
     Examples
     --------
@@ -66,14 +66,18 @@
     advancing the state of the model
 
     This function simulates many realisations of a model at a given
     fixed time in the future given an initial time and state, using a
     function (closure) for advancing the state of the model , such as
     created by ‘stepGillespie’ or ‘stepCLE’.
 
+    Note that this function is vectorised using `jax.vmap` rather than `jax.lax.map`.
+    This is usually (but not always) faster, especially on GPUs and TPUs. Note
+    that `simSampleMap` is identical except that it is vectorised using `jax.lax.map`.
+    
     Parameters
     ----------
     key: JAX random number key
         An unused random number key.
     n: int
         The number of samples required.
     x0: array of numbers
@@ -81,15 +85,15 @@
     t0: float
         The intial time to be associated with the initial state.
     deltat: float
         The amount of time in the future of t0 at which samples of the
         system state are required.
     stepFun: function
         A function (closure) for advancing the state of the process,
-        such as produced by `stepGillespie' or `stepEuler'.
+        such as produced by `stepGillespie' or `stepCLE'.
 
     Returns
     -------
     A matrix with rows representing simulated states at time t0+deltat.
 
     Examples
     --------
@@ -97,14 +101,64 @@
     >>> import jsmfsb.models
     >>> lv = jsmfsb.models.lv()
     >>> stepLv = lv.stepGillespie()
     >>> jsmfsb.simSample(jax.random.key(42), 10, lv.m, 0, 30, stepLv)
     """
     u = len(x0)
     keys = jax.random.split(key, n)
+    vstep = jit(jax.vmap(lambda k: stepFun(k, x0, t0, deltat)))
+    mat = vstep(keys)
+    return mat
+
+
+def simSampleMap(key, n, x0, t0, deltat, stepFun):
+    """Simulate a many realisations of a model at a given fixed time in the
+    future given an initial time and state, using a function (closure) for
+    advancing the state of the model
+
+    This function simulates many realisations of a model at a given
+    fixed time in the future given an initial time and state, using a
+    function (closure) for advancing the state of the model , such as
+    created by ‘stepGillespie’ or ‘stepCLE’.
+
+    Note that this function is vectorised using `jax.lax.map` rather than `jax.vmap`.
+    This is usually (but not always) slower, especially on GPUs and TPUs. Note
+    that `simSample` is identical except that it is vectorised using `jax.vmap`.
+    
+    Parameters
+    ----------
+    key: JAX random number key
+        An unused random number key.
+    n: int
+        The number of samples required.
+    x0: array of numbers
+        The intial state of the system at time t0.
+    t0: float
+        The intial time to be associated with the initial state.
+    deltat: float
+        The amount of time in the future of t0 at which samples of the
+        system state are required.
+    stepFun: function
+        A function (closure) for advancing the state of the process,
+        such as produced by `stepGillespie' or `stepCLE'.
+
+    Returns
+    -------
+    A matrix with rows representing simulated states at time t0+deltat.
+
+    Examples
+    --------
+    >>> import jax
+    >>> import jsmfsb.models
+    >>> lv = jsmfsb.models.lv()
+    >>> stepLv = lv.stepGillespie()
+    >>> jsmfsb.simSampleMap(jax.random.key(42), 10, lv.m, 0, 30, stepLv)
+    """
+    u = len(x0)
+    keys = jax.random.split(key, n)
     mat = jl.map(lambda k: stepFun(k, x0, t0, deltat), keys)
     return mat
```

### Comparing `jsmfsb-0.0.4/src/jsmfsb/smfsbSbml.py` & `jsmfsb-0.0.5/src/jsmfsb/smfsbSbml.py`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.4/src/jsmfsb/spn.py` & `jsmfsb-0.0.5/src/jsmfsb/spn.py`

 * *Files 9% similar despite different names*

```diff
@@ -73,25 +73,33 @@
     def stepGillespie(self, minHaz=1e-10, maxHaz=1e07):
         """Create a function for advancing the state of a SPN by using the
         Gillespie algorithm
 
         This method returns a function for advancing the state of an SPN
         model using the Gillespie algorithm. The resulting function
         (closure) can be used in conjunction with other functions (such as
-        ‘simTs’) for simulating realisations of SPN models.
+        `simTs`) for simulating realisations of SPN models.
+
+        Parameters
+        ----------
+        minHaz : float
+          Minimum hazard to consider before assuming 0. Defaults to 1e-10.
+        maxHaz : float
+          Maximum hazard to consider before assuming an explosion and
+          bailing out. Defaults to 1e07.
 
         Returns
         -------
         A function which can be used to advance the state of the SPN
         model by using the Gillespie algorithm. The function closure
-        has interface ‘function(key, x0, t0, deltat)’, where ‘x0’ and ‘t0’
-        represent the initial state and time, and ‘deltat’ represents the
-        amount of time by which the process should be advanced. The
-        function closure returns a vector representing the simulated state
-        of the system at the new time.
+        has interface `function(key, x0, t0, deltat)`, where `key` is an
+        unused JAX random key, `x0` and `t0` represent the initial state 
+        and time, and `deltat` represents the amount of time by which the 
+        process should be advanced. The function closure returns a vector 
+        representing the simulated state of the system at the new time.
 
         Examples
         --------
         >>> import jsmfsb.models
         >>> import jax
         >>> lv = jsmfsb.models.lv()
         >>> stepLv = lv.stepGillespie()
@@ -126,15 +134,15 @@
         """Create a function for advancing the state of an SPN by using a simple
         Euler-Maruyama integration method for the associated CLE
 
         This method returns a function for advancing the state of an SPN
         model using a simple Euler-Maruyama integration method
         method for the chemical Langevin equation form of the model.The 
         resulting function (closure) can be used in
-        conjunction with other functions (such as ‘simTs’) for simulating
+        conjunction with other functions (such as `simTs`) for simulating
         realisations of SPN models.
 
         Parameters
         ----------
         dt : float
             The time step for the time-stepping integration method. Defaults to 0.01.
```

### Comparing `jsmfsb-0.0.4/.gitignore` & `jsmfsb-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.4/LICENSE` & `jsmfsb-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.4/README.md` & `jsmfsb-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.4/pyproject.toml` & `jsmfsb-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jsmfsb"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Darren Wilkinson", email="darrenjwilkinson@btinternet.com" },
 ]
 description = "Python+JAX code relating to the textbook, Stochastic modelling for systems biology, third edition"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `jsmfsb-0.0.4/PKG-INFO` & `jsmfsb-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jsmfsb
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python+JAX code relating to the textbook, Stochastic modelling for systems biology, third edition
 Project-URL: Homepage, https://github.com/darrenjw/jax-smfsb
 Project-URL: Documentation, https://jax-smfsb.readthedocs.io/
 Project-URL: Issues, https://github.com/darrenjw/jax-smfsb/issues
 Author-email: Darren Wilkinson <darrenjwilkinson@btinternet.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
```

