# Comparing `tmp/rt_opt-0.1.1.tar.gz` & `tmp/rt_opt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/alexander/Projects/RunAndTumbleOptimizer/dist/tmpuet7_u5x/rt_opt-0.1.1.tar", last modified: Mon Sep 20 16:04:00 2021, max compression
+gzip compressed data, was "rt_opt-0.2.0.tar", last modified: Fri Apr 26 18:19:07 2024, max compression
```

## Comparing `rt_opt-0.1.1.tar` & `rt_opt-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2021-09-20 16:04:00.000000 rt_opt-0.1.1/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1104 2021-03-21 14:24:07.000000 rt_opt-0.1.1/LICENSE
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     6720 2021-09-20 16:04:00.000000 rt_opt-0.1.1/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     6151 2021-03-23 17:13:55.000000 rt_opt-0.1.1/README.md
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      104 2021-03-21 14:04:52.000000 rt_opt-0.1.1/pyproject.toml
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2021-09-20 16:04:00.000000 rt_opt-0.1.1/rt_opt/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2021-01-06 21:00:42.000000 rt_opt-0.1.1/rt_opt/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     8986 2021-03-13 16:10:26.000000 rt_opt-0.1.1/rt_opt/global_search.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    16004 2021-09-19 19:12:03.000000 rt_opt-0.1.1/rt_opt/local_search.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    27883 2021-09-20 08:12:53.000000 rt_opt-0.1.1/rt_opt/optimizer.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    12420 2021-03-09 18:00:53.000000 rt_opt-0.1.1/rt_opt/testproblems.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2774 2021-03-21 13:36:04.000000 rt_opt-0.1.1/rt_opt/testproblems_shifted.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2021-09-20 16:04:00.000000 rt_opt-0.1.1/rt_opt.egg-info/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     6720 2021-09-20 16:04:00.000000 rt_opt-0.1.1/rt_opt.egg-info/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      331 2021-09-20 16:04:00.000000 rt_opt-0.1.1/rt_opt.egg-info/SOURCES.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2021-09-20 16:04:00.000000 rt_opt-0.1.1/rt_opt.egg-info/dependency_links.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       27 2021-09-20 16:04:00.000000 rt_opt-0.1.1/rt_opt.egg-info/requires.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        7 2021-09-20 16:04:00.000000 rt_opt-0.1.1/rt_opt.egg-info/top_level.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      696 2021-09-20 16:04:00.000000 rt_opt-0.1.1/setup.cfg
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-04-26 18:19:07.554470 rt_opt-0.2.0/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1104 2021-03-21 14:24:07.000000 rt_opt-0.2.0/LICENSE
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     6768 2024-04-26 18:19:07.554470 rt_opt-0.2.0/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     6177 2024-04-25 17:28:47.000000 rt_opt-0.2.0/README.md
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      104 2024-04-26 18:11:21.000000 rt_opt-0.2.0/pyproject.toml
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-04-26 18:19:07.554470 rt_opt-0.2.0/rt_opt/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2021-01-06 21:00:42.000000 rt_opt-0.2.0/rt_opt/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     8988 2024-04-25 16:37:32.000000 rt_opt-0.2.0/rt_opt/global_search.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    16004 2022-05-23 17:50:49.000000 rt_opt-0.2.0/rt_opt/local_search.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    27883 2024-04-25 17:26:11.000000 rt_opt-0.2.0/rt_opt/optimizer.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    12420 2021-03-09 18:00:53.000000 rt_opt-0.2.0/rt_opt/testproblems.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2774 2021-03-21 13:36:04.000000 rt_opt-0.2.0/rt_opt/testproblems_shifted.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-04-26 18:19:07.554470 rt_opt-0.2.0/rt_opt.egg-info/
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     6768 2024-04-26 18:19:07.000000 rt_opt-0.2.0/rt_opt.egg-info/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      358 2024-04-26 18:19:07.000000 rt_opt-0.2.0/rt_opt.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2024-04-26 18:19:07.000000 rt_opt-0.2.0/rt_opt.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       28 2024-04-26 18:19:07.000000 rt_opt-0.2.0/rt_opt.egg-info/requires.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        7 2024-04-26 18:19:07.000000 rt_opt-0.2.0/rt_opt.egg-info/top_level.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      698 2024-04-26 18:19:07.554470 rt_opt-0.2.0/setup.cfg
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-04-26 18:19:07.554470 rt_opt-0.2.0/tests/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     5307 2021-03-21 13:36:29.000000 rt_opt-0.2.0/tests/test_testproblems.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rt_opt-0.1.1/LICENSE` & `rt_opt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rt_opt-0.1.1/PKG-INFO` & `rt_opt-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: rt_opt
-Version: 0.1.1
+Version: 0.2.0
 Summary: Metaheuristic global optimization algorithm
 Home-page: https://github.com/don-alejandrino/rt_opt
 Author: Alexander Geiseler
 Author-email: don-alejandrino@outlook.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/don-alejandrino/rt_opt/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy~=1.26.4
+Requires-Dist: scipy~=1.12.0
 
 # rt_opt: Run-and-tumble global optimizer
 
 Metaheuristic global optimization algorithm combining a bacterial run-and-tumble chemotactic search
 (see, e.g., [here](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5418374/)) with a local,
 gradient-based search around the best minimum candidate points.
 The algorithm's goal is to find the global minimum of an objective function f over a (possibly
 bounded) region Ω, that is, to find
 
-<p align="center">
+<p style="text-align: center;">
 min f(x), x ∈ Ω, <br/>
 f: Ω ⊂ ℝ<sup>n</sup> → ℝ.
 </p>
 
 For the local, gradient-based search, a bounded BFGS algorithm is used.
 
 Since the chemotactic search becomes more and more ineffective with increasing problem
 dimensionality,
 [Sequential Random Embeddings](http://www.lamda.nju.edu.cn/huyq/papers/ijcai16-sre.pdf) are used
 to solve the optimization problem once its dimensionality exceeds a given threshold. The idea of
 Sequential Random Embeddings is basically to reduce high-dimensional problems to low-dimensional
 ones by embedding the original, high-dimensional search space ℝ<sup>n</sup> into a low dimensional
 one, ℝ<sup>m</sup>, by sequentially applying the random linear transformation
 
-<p align="center">
+<p style="text-align: center;">
 x<sub>0</sub> = 0<br>
 x<sub>k+1</sub> = α<sub>k+1</sub>x<sub>k</sub> + A • y<sub>k+1</sub>,<br>
 x ∈ ℝ<sup>n</sup>,&nbsp;&nbsp;&nbsp;&nbsp;y ∈ ℝ<sup>m</sup>,&nbsp;&nbsp;&nbsp;&nbsp;
 A ∈ N(0, 1)<sup>n×m</sup>,&nbsp;&nbsp;&nbsp;&nbsp;α ∈ ℝ,
 </p>
 
 and minimizing the objective function f(α<sub>k+1</sub>x<sub>k</sub> + A • y<sub>k+1</sub>) w.r.t.
@@ -170,9 +170,7 @@
 For a performance comparison of rt_opt with other global optimization algorithms, namely
 *differential_evolution* and *dual_annealing* from scipy, as well as dlib's
 [LIPO]( http://blog.dlib.net/2017/12/a-global-optimization-algorithm-worth.html )-based
 *find_min_global*, see [here](demo/results). The comparison results were obtained by running
 [demo.py](demo/demo.py), where each of these four algorithms was evaluated 100 times with default
 parameters on a couple of 2D and 15D test functions (details on these functions can be found 
 [here](https://en.wikipedia.org/wiki/Test_functions_for_optimization)).
-
-
```

### Comparing `rt_opt-0.1.1/README.md` & `rt_opt-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 Metaheuristic global optimization algorithm combining a bacterial run-and-tumble chemotactic search
 (see, e.g., [here](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5418374/)) with a local,
 gradient-based search around the best minimum candidate points.
 The algorithm's goal is to find the global minimum of an objective function f over a (possibly
 bounded) region Ω, that is, to find
 
-<p align="center">
+<p style="text-align: center;">
 min f(x), x ∈ Ω, <br/>
 f: Ω ⊂ ℝ<sup>n</sup> → ℝ.
 </p>
 
 For the local, gradient-based search, a bounded BFGS algorithm is used.
 
 Since the chemotactic search becomes more and more ineffective with increasing problem
 dimensionality,
 [Sequential Random Embeddings](http://www.lamda.nju.edu.cn/huyq/papers/ijcai16-sre.pdf) are used
 to solve the optimization problem once its dimensionality exceeds a given threshold. The idea of
 Sequential Random Embeddings is basically to reduce high-dimensional problems to low-dimensional
 ones by embedding the original, high-dimensional search space ℝ<sup>n</sup> into a low dimensional
 one, ℝ<sup>m</sup>, by sequentially applying the random linear transformation
 
-<p align="center">
+<p style="text-align: center;">
 x<sub>0</sub> = 0<br>
 x<sub>k+1</sub> = α<sub>k+1</sub>x<sub>k</sub> + A • y<sub>k+1</sub>,<br>
 x ∈ ℝ<sup>n</sup>,&nbsp;&nbsp;&nbsp;&nbsp;y ∈ ℝ<sup>m</sup>,&nbsp;&nbsp;&nbsp;&nbsp;
 A ∈ N(0, 1)<sup>n×m</sup>,&nbsp;&nbsp;&nbsp;&nbsp;α ∈ ℝ,
 </p>
 
 and minimizing the objective function f(α<sub>k+1</sub>x<sub>k</sub> + A • y<sub>k+1</sub>) w.r.t.
```

### Comparing `rt_opt-0.1.1/rt_opt/global_search.py` & `rt_opt-0.2.0/rt_opt/global_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
            that contributes to the attraction mechanism. We have to define this cut-off length,
            since otherwise calculating the bacteria attractions becomes computationally very
            expensive. This parameter only has an effect if attraction == True
     :param attraction_sigma: [float] The bacterial attractant concentration is modeled to decay
            according to a Gaussian distribution,
            -----
            attraction_strength / 2 / attraction_sigma ** 2
-                * exp(-(np.square(x - x_vis) / 2 / attraction_sigma ** 2),
+                * exp(-(np.square(x - x_vis) / 2 / attraction_sigma ** 2)),
            -----
            around each point x_vis visited thus far. This parameter only has an effect if
            attraction == True
     :param attraction_strength: [float] See description of parameter ``attraction_sigma``. Note that
            if attraction_strength < 0, the bacterial attraction turns into a repulsion. This
            parameter only has an effect if attraction == True
     :param bounds_reflection: [bool] Whether bacteria reverse their direction when hitting a
@@ -122,15 +122,15 @@
         # Calculate new orientation
         for m, tr in enumerate(tumble_rate):
             if bounds_reflection and bounds_hit[m].any():
                 # Reflection at boundaries
                 v[m] = -v[m]
             elif bounds_hit[m].any() or np.random.uniform() > 1 - tr:
                 # Realistically, tr must be clipped to [0, 1]. However, the inequality above is not
-                # influenced by this clipping and we thus omit it in order to save computation time
+                # influenced by this clipping, and we thus omit it in order to save computation time
                 v_m = np.random.uniform(-1, 1, n_dims)
                 while not v_m.any():
                     v_m = np.random.uniform(-1, 1, n_dims)
                 v_m = v_m / np.sqrt(np.sum(v_m ** 2))
                 v[m] = v_m
 
         # Remember best results
```

### Comparing `rt_opt-0.1.1/rt_opt/local_search.py` & `rt_opt-0.2.0/rt_opt/local_search.py`

 * *Files identical despite different names*

### Comparing `rt_opt-0.1.1/rt_opt/optimizer.py` & `rt_opt-0.2.0/rt_opt/optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     :param targetLength: [int] Desired length
     :return: Padded trace [np.array]
     """
 
     currentLength = trace.shape[0]
     paddingLength = (targetLength - currentLength)
 
-    return np.pad(trace, [(0, paddingLength), (0, 0)], mode="edge")
+    return np.pad(trace, ((0, paddingLength), (0, 0)), mode="edge")
 
 
 def _sequential_random_embeddings(f, x0, bounds, n_reduced_dims_eff=3, n_embeddings=10,
                                   verbosity=1, **optimizer_kwargs):
     """
     Implementation of the Sequential Random Embeddings algorithm described in
     +++++
```

### Comparing `rt_opt-0.1.1/rt_opt/testproblems.py` & `rt_opt-0.2.0/rt_opt/testproblems.py`

 * *Files identical despite different names*

### Comparing `rt_opt-0.1.1/rt_opt/testproblems_shifted.py` & `rt_opt-0.2.0/rt_opt/testproblems_shifted.py`

 * *Files identical despite different names*

### Comparing `rt_opt-0.1.1/rt_opt.egg-info/PKG-INFO` & `rt_opt-0.2.0/rt_opt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
-Name: rt-opt
-Version: 0.1.1
+Name: rt_opt
+Version: 0.2.0
 Summary: Metaheuristic global optimization algorithm
 Home-page: https://github.com/don-alejandrino/rt_opt
 Author: Alexander Geiseler
 Author-email: don-alejandrino@outlook.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/don-alejandrino/rt_opt/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy~=1.26.4
+Requires-Dist: scipy~=1.12.0
 
 # rt_opt: Run-and-tumble global optimizer
 
 Metaheuristic global optimization algorithm combining a bacterial run-and-tumble chemotactic search
 (see, e.g., [here](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5418374/)) with a local,
 gradient-based search around the best minimum candidate points.
 The algorithm's goal is to find the global minimum of an objective function f over a (possibly
 bounded) region Ω, that is, to find
 
-<p align="center">
+<p style="text-align: center;">
 min f(x), x ∈ Ω, <br/>
 f: Ω ⊂ ℝ<sup>n</sup> → ℝ.
 </p>
 
 For the local, gradient-based search, a bounded BFGS algorithm is used.
 
 Since the chemotactic search becomes more and more ineffective with increasing problem
 dimensionality,
 [Sequential Random Embeddings](http://www.lamda.nju.edu.cn/huyq/papers/ijcai16-sre.pdf) are used
 to solve the optimization problem once its dimensionality exceeds a given threshold. The idea of
 Sequential Random Embeddings is basically to reduce high-dimensional problems to low-dimensional
 ones by embedding the original, high-dimensional search space ℝ<sup>n</sup> into a low dimensional
 one, ℝ<sup>m</sup>, by sequentially applying the random linear transformation
 
-<p align="center">
+<p style="text-align: center;">
 x<sub>0</sub> = 0<br>
 x<sub>k+1</sub> = α<sub>k+1</sub>x<sub>k</sub> + A • y<sub>k+1</sub>,<br>
 x ∈ ℝ<sup>n</sup>,&nbsp;&nbsp;&nbsp;&nbsp;y ∈ ℝ<sup>m</sup>,&nbsp;&nbsp;&nbsp;&nbsp;
 A ∈ N(0, 1)<sup>n×m</sup>,&nbsp;&nbsp;&nbsp;&nbsp;α ∈ ℝ,
 </p>
 
 and minimizing the objective function f(α<sub>k+1</sub>x<sub>k</sub> + A • y<sub>k+1</sub>) w.r.t.
@@ -170,9 +170,7 @@
 For a performance comparison of rt_opt with other global optimization algorithms, namely
 *differential_evolution* and *dual_annealing* from scipy, as well as dlib's
 [LIPO]( http://blog.dlib.net/2017/12/a-global-optimization-algorithm-worth.html )-based
 *find_min_global*, see [here](demo/results). The comparison results were obtained by running
 [demo.py](demo/demo.py), where each of these four algorithms was evaluated 100 times with default
 parameters on a couple of 2D and 15D test functions (details on these functions can be found 
 [here](https://en.wikipedia.org/wiki/Test_functions_for_optimization)).
-
-
```

### Comparing `rt_opt-0.1.1/setup.cfg` & `rt_opt-0.2.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rt_opt
-version = 0.1.1
+version = 0.2.0
 author = Alexander Geiseler
 author_email = don-alejandrino@outlook.com
 description = Metaheuristic global optimization algorithm
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/don-alejandrino/rt_opt
 project_urls = 
@@ -13,18 +13,18 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.10
 install_requires = 
-	numpy==1.19.5
-	scipy==1.6.0
+	numpy~=1.26.4
+	scipy~=1.12.0
 
 [options.packages.find]
 where = 
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

