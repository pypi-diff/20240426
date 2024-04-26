# Comparing `tmp/vbayesfa-0.0.22.tar.gz` & `tmp/vbayesfa-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbayesfa-0.0.22.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vbayesfa-0.0.23.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vbayesfa-0.0.22.tar` & `vbayesfa-0.0.23.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0      234 2024-04-24 20:35:53.884246 vbayesfa-0.0.22/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-01-31 17:01:44.847879 vbayesfa-0.0.22/src/vbayesfa/.DS_Store
--rw-r--r--   0        0        0       69 2023-12-05 19:18:02.101247 vbayesfa-0.0.22/src/vbayesfa/__init__.py
--rw-r--r--   0        0        0    16841 2024-04-08 17:09:57.330242 vbayesfa-0.0.22/src/vbayesfa/bayes_factors.py
--rw-r--r--   0        0        0    28671 2024-03-14 18:29:17.477573 vbayesfa-0.0.22/src/vbayesfa/exp_families.py
--rw-r--r--   0        0        0     7482 2024-04-14 18:39:13.977771 vbayesfa-0.0.22/src/vbayesfa/finite_lpa.py
--rw-r--r--   0        0        0     4176 2024-04-11 18:23:10.081833 vbayesfa-0.0.22/src/vbayesfa/fit_finite_lpa.py
--rw-r--r--   0        0        0     3800 2024-04-15 14:08:40.305148 vbayesfa-0.0.22/src/vbayesfa/fit_lpa.py
--rw-r--r--   0        0        0     3893 2024-04-15 14:10:42.994079 vbayesfa-0.0.22/src/vbayesfa/fit_lpa2.py
--rw-r--r--   0        0        0     9420 2023-07-05 21:34:32.174051 vbayesfa-0.0.22/src/vbayesfa/ibp/discrete_finite.py
--rw-r--r--   0        0        0     3726 2023-06-16 14:40:29.441517 vbayesfa-0.0.22/src/vbayesfa/ibp/fit_ibp.py
--rw-r--r--   0        0        0     9770 2023-07-05 21:33:47.123462 vbayesfa-0.0.22/src/vbayesfa/ibp/full_discrete_finite.py
--rw-r--r--   0        0        0     3164 2023-05-25 19:01:25.945355 vbayesfa-0.0.22/src/vbayesfa/ibp/make_sim_data.py
--rw-r--r--   0        0        0    11261 2024-04-04 15:36:07.290321 vbayesfa-0.0.22/src/vbayesfa/ibp/sparse_cont_finite.py
--rw-r--r--   0        0        0    16282 2023-07-05 21:31:30.740293 vbayesfa-0.0.22/src/vbayesfa/ibp/sparse_pos_cont_finite.py
--rw-r--r--   0        0        0    10883 2024-04-24 20:20:51.773733 vbayesfa-0.0.22/src/vbayesfa/lpa.py
--rw-r--r--   0        0        0    20925 2024-04-10 19:09:07.425525 vbayesfa-0.0.22/src/vbayesfa/lpa_outcome_analysis.py
--rw-r--r--   0        0        0    35869 2024-04-24 20:25:44.549383 vbayesfa-0.0.22/src/vbayesfa/mixture_model.py
--rw-r--r--   0        0        0    40897 2024-04-09 19:30:59.411472 vbayesfa-0.0.22/src/vbayesfa/old_lpa.py
--rw-r--r--   0        0        0    10712 2024-04-17 21:13:53.670539 vbayesfa-0.0.22/src/vbayesfa/simulate_data.py
--rw-r--r--   0        0        0     6148 2024-01-30 20:49:54.836172 vbayesfa-0.0.22/src/vbayesfa/tests/.DS_Store
--rw-r--r--   0        0        0     5776 2024-02-29 18:02:24.703820 vbayesfa-0.0.22/src/vbayesfa/tests/test_exp_families.py
--rw-r--r--   0        0        0     1633 2024-04-12 14:18:41.718223 vbayesfa-0.0.22/src/vbayesfa/tests/test_lpa.py
--rw-r--r--   0        0        0     2147 2024-03-11 15:41:20.385592 vbayesfa-0.0.22/src/vbayesfa/tests/test_lpa_outcome_analysis.py
--rw-r--r--   0        0        0      180 1970-01-01 00:00:00.000000 vbayesfa-0.0.22/PKG-INFO
+-rw-r--r--   0        0        0      234 2024-04-26 17:46:51.889270 vbayesfa-0.0.23/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-01-31 17:01:44.847879 vbayesfa-0.0.23/src/vbayesfa/.DS_Store
+-rw-r--r--   0        0        0       69 2023-12-05 19:18:02.101247 vbayesfa-0.0.23/src/vbayesfa/__init__.py
+-rw-r--r--   0        0        0    16841 2024-04-08 17:09:57.330242 vbayesfa-0.0.23/src/vbayesfa/bayes_factors.py
+-rw-r--r--   0        0        0    28671 2024-03-14 18:29:17.477573 vbayesfa-0.0.23/src/vbayesfa/exp_families.py
+-rw-r--r--   0        0        0     7498 2024-04-26 15:44:45.654627 vbayesfa-0.0.23/src/vbayesfa/finite_lpa.py
+-rw-r--r--   0        0        0     2565 2024-04-26 17:40:28.877298 vbayesfa-0.0.23/src/vbayesfa/fit_finite_lpa.py
+-rw-r--r--   0        0        0     2576 2024-04-26 16:42:01.807322 vbayesfa-0.0.23/src/vbayesfa/fit_lpa.py
+-rw-r--r--   0        0        0     3896 2024-04-25 20:52:37.200820 vbayesfa-0.0.23/src/vbayesfa/fit_lpa2.py
+-rw-r--r--   0        0        0     3627 2024-04-26 17:26:36.489698 vbayesfa-0.0.23/src/vbayesfa/fit_mixture_model.py
+-rw-r--r--   0        0        0     9420 2023-07-05 21:34:32.174051 vbayesfa-0.0.23/src/vbayesfa/ibp/discrete_finite.py
+-rw-r--r--   0        0        0     3726 2023-06-16 14:40:29.441517 vbayesfa-0.0.23/src/vbayesfa/ibp/fit_ibp.py
+-rw-r--r--   0        0        0     9770 2023-07-05 21:33:47.123462 vbayesfa-0.0.23/src/vbayesfa/ibp/full_discrete_finite.py
+-rw-r--r--   0        0        0     3164 2023-05-25 19:01:25.945355 vbayesfa-0.0.23/src/vbayesfa/ibp/make_sim_data.py
+-rw-r--r--   0        0        0    11261 2024-04-04 15:36:07.290321 vbayesfa-0.0.23/src/vbayesfa/ibp/sparse_cont_finite.py
+-rw-r--r--   0        0        0    16282 2023-07-05 21:31:30.740293 vbayesfa-0.0.23/src/vbayesfa/ibp/sparse_pos_cont_finite.py
+-rw-r--r--   0        0        0    10900 2024-04-26 15:44:53.989278 vbayesfa-0.0.23/src/vbayesfa/lpa.py
+-rw-r--r--   0        0        0    20925 2024-04-10 19:09:07.425525 vbayesfa-0.0.23/src/vbayesfa/lpa_outcome_analysis.py
+-rw-r--r--   0        0        0    35808 2024-04-26 16:31:13.132014 vbayesfa-0.0.23/src/vbayesfa/mixture_model.py
+-rw-r--r--   0        0        0    40897 2024-04-09 19:30:59.411472 vbayesfa-0.0.23/src/vbayesfa/old_lpa.py
+-rw-r--r--   0        0        0    10712 2024-04-17 21:13:53.670539 vbayesfa-0.0.23/src/vbayesfa/simulate_data.py
+-rw-r--r--   0        0        0     6148 2024-01-30 20:49:54.836172 vbayesfa-0.0.23/src/vbayesfa/tests/.DS_Store
+-rw-r--r--   0        0        0     5776 2024-02-29 18:02:24.703820 vbayesfa-0.0.23/src/vbayesfa/tests/test_exp_families.py
+-rw-r--r--   0        0        0     1625 2024-04-26 17:43:28.152597 vbayesfa-0.0.23/src/vbayesfa/tests/test_finite_lpa.py
+-rw-r--r--   0        0        0     1595 2024-04-26 17:42:56.650573 vbayesfa-0.0.23/src/vbayesfa/tests/test_lpa.py
+-rw-r--r--   0        0        0     2147 2024-03-11 15:41:20.385592 vbayesfa-0.0.23/src/vbayesfa/tests/test_lpa_outcome_analysis.py
+-rw-r--r--   0        0        0      180 1970-01-01 00:00:00.000000 vbayesfa-0.0.23/PKG-INFO
```

### Comparing `vbayesfa-0.0.22/src/vbayesfa/.DS_Store` & `vbayesfa-0.0.23/src/vbayesfa/.DS_Store`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.22/src/vbayesfa/bayes_factors.py` & `vbayesfa-0.0.23/src/vbayesfa/bayes_factors.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.22/src/vbayesfa/exp_families.py` & `vbayesfa-0.0.23/src/vbayesfa/exp_families.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.22/src/vbayesfa/finite_lpa.py` & `vbayesfa-0.0.23/src/vbayesfa/finite_lpa.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,21 +149,21 @@
         Notes
         -----
         The means (mu) and precisions (xi) have a multi-mean normal-gamma prior.
         
         The fact that the prior alpha_xi = prior beta_xi implies that the prior distribution on xi
         has a mean of 1.
         '''
-        super().__init__(x = x, T = T, prior_hpar = {'alpha_pi': prior_alpha_pi, 'lambda_mu': prior_lambda_mu, 'strength_for_xi': prior_strength_for_xi}, phi = phi, seed = seed)
+        super().__init__(x = x, T = T, prior_alpha_pi = prior_alpha_pi, prior_lambda_mu = prior_lambda_mu, prior_strength_for_xi = prior_strength_for_xi, phi = phi, seed = seed)
     
-    def _initialize_q_pi(self, prior_hpar):
+    def _initialize_q_pi(self, prior_alpha_pi, **other_prior_hpar):
         '''
         Initialize the variational distribution of latent class/profile base rates (pi).
         '''
-        self.prior_alpha_pi = prior_hpar['alpha_pi']
+        self.prior_alpha_pi = prior_alpha_pi
         self.alpha_pi = self.prior_alpha_pi*np.ones(self.T)
         self._update_q_pi()
     
     def _update_q_pi(self):
         '''
         Update the variational distribution of latent class/profile base rates (pi).
         '''
```

### Comparing `vbayesfa-0.0.22/src/vbayesfa/fit_finite_lpa.py` & `vbayesfa-0.0.23/src/vbayesfa/fit_lpa2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import numpy as np
-import pandas as pd
 import functools
 import multiprocessing
-from .finite_lpa import finite_lpa_model
+from .fit_finite_lpa import fit_finite_lpa
+from .lpa import lpa_model
 from time import perf_counter
 
-def fit_finite_lpa(x, n_workers = 4, restarts = 10, T_range = np.arange(2, 11), prior_alpha_pi = 1.0, prior_lambda_mu = 0.5, prior_strength_for_xi = 10.0, seed = 1234, tolerance = 1e-05, max_iter = 50, min_iter = 30):
+def fit_lpa2(x, n_workers = 4, restarts = 20, T = 20, prior_w1 = 3.0, prior_w2 = 1.0, prior_lambda_mu = 0.5, prior_strength_for_xi = 10.0, seed = 1234, tolerance = 1e-05, max_iter = 1000, min_iter = 10):
     """
-    Fit series of finite latent profile analysis (DPM-LPA) models of different sizes (number of profile, T)
-    using mean field variational Bayes.
+    Fit a Dirichlet process latent profile analysis (DPM-LPA) model using mean field
+    variational Bayes.
+    
+    This version of the function fits finite LPA models first to provide starting points
+    for DPM-LPA of varying sizes.
     
     Parameters
     ----------
     x: data frame or array
         Observed data (data frame or matrix).  If a matrix then rows are variables and columns
         are observations; if a data frame then rows are observations and columns are variables.
     n_workers: int, optional
         Number of workers in the pool for parallel processing; should be less than
         or equal to the number of available CPUs.
     restarts: int, optional
-        Number of random restarts per value of T (number of latent profiles).
-    T_range: array of integers, optional
-        Range of values of T (number of latent profiles) to fit.
-    prior_alpha_pi: float, optional
-        Prior strength of the Dirichlet prior distribution on pi.
+        Number of random restarts for finite LPA models.
+    T: integer, optional
+        Truncation level of the variational approximation.
+    prior_w1: float, optional
+        First prior hyperparameter on alpha.
+    prior_w2: float, optional
+        Second prior hyperparameter on alpha.
     prior_lambda_mu: float, optional
         Controls the width of the prior distribution on mu: 
         higher values -> tighter prior around 0.
     prior_strength_for_xi: float, optional
         Controls the strength of the gamma prior distribution on xi.
         This prior is assumed to have a mean of 1, with alpha = prior_strength_for_xi/2
         and beta = prior_strength_for_xi/2.
@@ -38,49 +43,35 @@
     max_iter: integer, optional
         Maximum number of iterations to run the optimization.
     min_iter: integer, optional
         Minimum number of iterations to run the optimization.
         
     Notes
     -----
-    This creates multiple finite_lpa_model objects from the finite_lpa.py module and fits them with using parallel
+    This creates multiple lpa_model objects from the lpa.py module and fits them with using parallel
     processing. See the documentation for the lpa_model object for more details.
     """
-    tic = perf_counter()
-    # set up an empty data frame to hold results
-    n_T = T_range.shape[0]
-    all_results = pd.DataFrame({'final_elbo': n_T*[0.0], 'best_model': n_T*[np.nan]}, index = pd.Index(T_range, name = 'T'))
+    finite_fits = fit_finite_lpa(x, T_range = np.arange(2, T + 1), prior_alpha_pi = 0.5, prior_lambda_mu = prior_lambda_mu, prior_strength_for_xi = prior_strength_for_xi, restarts = restarts, seed = seed)
+    phi_list = [finite_fits.loc[Tval, 'best_model'].phi for Tval in np.arange(2, T + 1)]
+    model_list = []
+    final_elbo = []
     
-    # generate random seeds for each model based on the seed parameter
-    seed_list = []
-    rng = np.random.default_rng(seed)
-    for i in range(restarts):
-        seed_list += [rng.integers(low = 1000, high = 9999)]
+    with multiprocessing.Pool(n_workers) as pool:
+        fun = functools.partial(_model_fit_wrapper, x = x, T = T, prior_w1 = prior_w1, prior_w2 = prior_w2, prior_lambda_mu = prior_lambda_mu, prior_strength_for_xi = prior_strength_for_xi, tolerance = tolerance, max_iter = max_iter, min_iter = min_iter)        
+        results = pool.map(fun, phi_list)
+    for result in results:
+        model_list += [result]
+        final_elbo += [result.elbo_list[-1]]
+        
+    final_elbo = np.array(final_elbo)
     
-    # loop through values of T (number of latent profiles)
-    for T in T_range:
-        model_list = []
-        final_elbo = []
-
-        with multiprocessing.Pool(n_workers) as pool:
-            fun = functools.partial(__model_fit_wrapper__, x = x, T = T, prior_alpha_pi = prior_alpha_pi, prior_lambda_mu = prior_lambda_mu, prior_strength_for_xi = prior_strength_for_xi, tolerance = tolerance, max_iter = max_iter, min_iter = min_iter)
-            results = pool.map(fun, seed_list)
-            for result in results:
-                model_list += [result]
-                final_elbo += [result.elbo_list[-1]]
+    return {'final_elbo': final_elbo, 'model_list': model_list, 'best_model': model_list[final_elbo.argmax()]}
 
-        all_results.loc[T, 'final_elbo'] = np.array(final_elbo).max()
-        all_results.loc[T, 'best_model'] = model_list[np.array(final_elbo).argmax()]
     
-    toc = perf_counter()
-    print(f"Fit in {toc - tic:0.4f} seconds.")
-    
-    return all_results
-
-def __model_fit_wrapper__(seed, x, T, prior_alpha_pi, prior_lambda_mu, prior_strength_for_xi, tolerance, max_iter, min_iter):
+def _model_fit_wrapper(phi, x, T, prior_w1, prior_w2, prior_lambda_mu, prior_strength_for_xi, tolerance, max_iter, min_iter):
     """
-    Defines a finite LPA model and fits it to the data, returning the result.
+    Defines an LPA model and fits it to the data, returning the result.
     This function is only defined in order to get the parallelization to work.
     """
-    new_model = finite_lpa_model(x = x, T = T, prior_alpha_pi = prior_alpha_pi, prior_lambda_mu = prior_lambda_mu, prior_strength_for_xi = prior_strength_for_xi, seed = seed)
+    new_model = lpa_model(x = x, phi = phi, T = T, prior_w1 = prior_w1, prior_w2 = prior_w2, prior_lambda_mu = prior_lambda_mu, prior_strength_for_xi = prior_strength_for_xi, seed = None)
     new_model.fit(tolerance = tolerance, max_iter = max_iter, min_iter = min_iter)
     return new_model
```

### Comparing `vbayesfa-0.0.22/src/vbayesfa/fit_lpa.py` & `vbayesfa-0.0.23/src/vbayesfa/fit_lpa.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-import numpy as np
-import functools
-import multiprocessing
+from .fit_mixture_model import fit_mixture_model
 from .lpa import lpa_model
-from scipy.special import digamma
-from time import perf_counter
 
-def fit_lpa(x, n_workers = 4, restarts = 4, T = 20, prior_w1 = 3.0, prior_w2 = 1.0, prior_lambda_mu = 0.5, prior_strength_for_xi = 10.0, seed = 1234, tolerance = 1e-05, max_iter = 50, min_iter = 30):
+def fit_lpa(x, n_workers = 4, restarts = 20, T = 20, prior_w1 = 3.0, prior_w2 = 1.0, prior_lambda_mu = 0.5, prior_strength_for_xi = 10.0, seed = 1234, tolerance = 1e-05, max_iter = 1000, min_iter = 10):
     """
     Fit a Dirichlet process latent profile analysis (DPM-LPA) model using mean field
     variational Bayes.
     
     Parameters
     ----------
     x: data frame or array
@@ -38,45 +34,21 @@
     tolerance: float, optional
         Relative change in the ELBO at which the optimization should stop.
     max_iter: integer, optional
         Maximum number of iterations to run the optimization.
     min_iter: integer, optional
         Minimum number of iterations to run the optimization.
         
-    Notes
-    -----
-    This creates multiple lpa_model objects from the lpa.py module and fits them with using parallel
-    processing. See the documentation for the lpa_model object for more details.
-    """
-    tic = perf_counter()
-
-    model_list = []
-    final_elbo = []
-    
-    with multiprocessing.Pool(n_workers) as pool:
-        fun = functools.partial(__model_fit_wrapper__, x = x, T = T, prior_w1 = prior_w1, prior_w2 = prior_w2, prior_lambda_mu = prior_lambda_mu, prior_strength_for_xi = prior_strength_for_xi, tolerance = tolerance, max_iter = max_iter, min_iter = min_iter)
-        
-        # generate random seeds for each model based on the seed parameter
-        seed_list = []
-        rng = np.random.default_rng(seed)
-        for i in range(restarts):
-            seed_list += [rng.integers(low = 1000, high = 9999)]
-        
-        results = pool.map(fun, seed_list)
-        for result in results:
-            model_list += [result]
-            final_elbo += [result.elbo_list[-1]]
-        
-    final_elbo = np.array(final_elbo)
-    toc = perf_counter()
-    print(f"Fit the model in {toc - tic:0.4f} seconds.")
+    Output
+    ------
+    A dictionary with the following:
     
-    return {'final_elbo': final_elbo, 'model_list': model_list, 'best_model': model_list[final_elbo.argmax()]}
-
-def __model_fit_wrapper__(seed, x, T, prior_w1, prior_w2, prior_lambda_mu, prior_strength_for_xi, tolerance, max_iter, min_iter):
-    """
-    Defines an LPA model and fits it to the data, returning the result.
-    This function is only defined in order to get the parallelization to work.
+    final_elbo: list
+        Final ELBO (evidence lower bound) values of each model.
+    model_list: list
+        Fitted model objects.
+    best_model: mixture_model object
+        Best fitted model (i.e. the one with the highest ELBO).
+    fit_time: float
+        Total time used to fit.
     """
-    new_model = lpa_model(x = x, T = T, prior_w1 = prior_w1, prior_w2 = prior_w2, prior_lambda_mu = prior_lambda_mu, prior_strength_for_xi = prior_strength_for_xi, seed = seed)
-    new_model.fit(tolerance = tolerance, max_iter = max_iter, min_iter = min_iter)
-    return new_model
+    return fit_mixture_model(x = x, model_class = lpa_model, n_workers = n_workers, restarts = restarts, T = T, prior_w1 = prior_w1, prior_w2 = prior_w2, prior_lambda_mu = prior_lambda_mu, prior_strength_for_xi = prior_strength_for_xi, seed = seed, tolerance = tolerance, max_iter = max_iter, min_iter = min_iter)
```

### Comparing `vbayesfa-0.0.22/src/vbayesfa/ibp/discrete_finite.py` & `vbayesfa-0.0.23/src/vbayesfa/ibp/discrete_finite.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.22/src/vbayesfa/ibp/fit_ibp.py` & `vbayesfa-0.0.23/src/vbayesfa/ibp/fit_ibp.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.22/src/vbayesfa/ibp/full_discrete_finite.py` & `vbayesfa-0.0.23/src/vbayesfa/ibp/full_discrete_finite.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.22/src/vbayesfa/ibp/make_sim_data.py` & `vbayesfa-0.0.23/src/vbayesfa/ibp/make_sim_data.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.22/src/vbayesfa/ibp/sparse_cont_finite.py` & `vbayesfa-0.0.23/src/vbayesfa/ibp/sparse_cont_finite.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.22/src/vbayesfa/ibp/sparse_pos_cont_finite.py` & `vbayesfa-0.0.23/src/vbayesfa/ibp/sparse_pos_cont_finite.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.22/src/vbayesfa/lpa.py` & `vbayesfa-0.0.23/src/vbayesfa/lpa.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,25 +177,25 @@
         Thus the prior mean of alpha is prior_w1/prior_w2.
 
         The means (mu) and precisions (xi) have a multi-mean normal-gamma prior.
         
         The fact that the prior alpha_xi = prior beta_xi implies that the prior distribution on xi
         has a mean of 1.
         '''
-        super().__init__(x = x, T = T, prior_hpar = {'lambda_mu': prior_lambda_mu, 'strength_for_xi': prior_strength_for_xi, 'w1': prior_w1, 'w2': prior_w2}, phi = phi, seed = seed)
+        super().__init__(x = x, T = T, prior_w1 = prior_w1, prior_w2 = prior_w2, prior_lambda_mu = prior_lambda_mu, prior_strength_for_xi = prior_strength_for_xi, phi = phi, seed = seed)
     
-    def _initialize_q_pi(self, prior_hpar):
+    def _initialize_q_pi(self, prior_w1, prior_w2, **other_prior_hpar):
         '''
         Initialize the variational distribution of latent class/profile base rates (pi),
         broken into stick-breaking lengths (V) and the Dirichlet process concentration
         parameter (alpha).
         '''
         # initialize distribution of the Dirichlet process concentration parameter (alpha)
-        self.prior_w1 = prior_hpar['w1']
-        self.prior_w2 = prior_hpar['w2']
+        self.prior_w1 = prior_w1
+        self.prior_w2 = prior_w2
         self.w1 = self.prior_w1 + self.T - 1
         self.w2 = self.prior_w2
         self.E_alpha = self.w1/self.w2
         self.E_log_alpha = digamma(self.w1) - np.log(self.w2)
         # initialize distribution of stick-breaking lengths (V)
         self.gamma1 = np.zeros(self.T)
         self.gamma2 = np.zeros(self.T)
```

### Comparing `vbayesfa-0.0.22/src/vbayesfa/lpa_outcome_analysis.py` & `vbayesfa-0.0.23/src/vbayesfa/lpa_outcome_analysis.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.22/src/vbayesfa/mixture_model.py` & `vbayesfa-0.0.23/src/vbayesfa/mixture_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,33 +11,33 @@
 from abc import ABC, abstractmethod
 
 class mixture_model(ABC):
     '''
     Abstract base class for mixture models.
     '''
     
-    def __init__(self, x, T = 20, prior_hpar = None, phi = None, seed = 1234):
+    def __init__(self, x, T = 20, phi = None, seed = 1234, **prior_hpar):
         """
         Parameters
         ----------
         x: data frame or array
             Observed data (data frame or matrix).  If a matrix then rows are variables and columns
             are observations; if a data frame then rows are observations and columns are variables.
             Missing values are replaced with 0 for computational reasons.
         T: integer, optional
             The maximum number of latent profiles that can be discovered.
-        prior_hpar: dict, optional,
-            Prior hyperparameters.
         phi: array or None, optional
             If None (the default) then profile membership probabilities (phi) are randomly
             sampled from a Dirichlet(1, 1, ...) distribution. Otherwise this is an array
             of starting values for phi, with a number columns equal to the number of 
             observations and number of rows equal to or less than T.
         seed: integer, optional
             The seed for random number generation.
+        prior_hpar:
+            Prior hyperparameters (specified with keywords).
         """
         # ----- SET UP SOME VARIABLES -----
         
         if isinstance(x, pd.DataFrame):
             self.x = x.values.copy().transpose()
             self.index = x.index.values
             self.x_names = pd.Categorical(x.columns.values, categories = x.columns.values, ordered = True)
@@ -66,17 +66,17 @@
         self.phi = np.zeros([self.T, self.n])
         if phi is None:
             for i in range(self.n):
                 self.phi[:,i] = self.rng.dirichlet(self.T*[1.0])
         else:
             self.phi[range(phi.shape[0]),:] = phi
         # initialize variational distribution for likelihood parameters (eta)
-        self._initialize_q_eta(prior_hpar)
+        self._initialize_q_eta(**prior_hpar)
         # initialize variational distribution over pi (latent class/profile base rates)
-        self._initialize_q_pi(prior_hpar)
+        self._initialize_q_pi(**prior_hpar)
         
         # ----- OTHER STUFF -----
         self._update_hard_assignment()
     
     def fit(self, tolerance = 1e-05, max_iter = 50, min_iter = 20):
         """
         Parameters
@@ -130,36 +130,33 @@
             else: # otherwise, continue if ELBO change is below threshold and we haven't yet hit the iteration limit
                 relative_elbo_change = np.abs((self.elbo_list[-2] - self.elbo_list[-1])/self.elbo_list[-2])
                 continue_loop = (relative_elbo_change > tolerance) and (itr < max_iter)
                 
         # ----- FINISH UP -----
         self._update_hard_assignment()
     
-    def _initialize_q_eta(self, prior_hpar):
+    def _initialize_q_eta(self, prior_lambda_mu, prior_strength_for_xi, **other_prior_hpar):
         '''
         Initialize the variational distribution of eta (likelihood parameters).
         
         Parameters
         ----------
-        prior_hpar: dict
-            Should contain the following.
-            
-            lambda_mu: float
-                Controls the width of the prior distribution on mu: 
-                higher values -> tighter prior around 0.
-            strength_for_xi: float
-                Controls the strength of the gamma prior distribution on xi.
-                This prior is assumed to have a mean of 1, with alpha = prior_strength_for_xi/2
-                and beta = prior_strength_for_xi/2.
+        prior_lambda_mu: float
+            Controls the width of the prior distribution on mu: 
+            higher values -> tighter prior around 0.
+        prior_strength_for_xi: float
+            Controls the strength of the gamma prior distribution on xi.
+            This prior is assumed to have a mean of 1, with alpha = prior_strength_for_xi/2
+            and beta = prior_strength_for_xi/2.
         '''
         # prior conventional hyperparameters
-        self.prior_alpha_xi = 0.5*prior_hpar['strength_for_xi']
-        self.prior_beta_xi = 0.5*prior_hpar['strength_for_xi']
+        self.prior_alpha_xi = 0.5*prior_strength_for_xi
+        self.prior_beta_xi = 0.5*prior_strength_for_xi
         self.prior_m_mu = 0.0
-        self.prior_lambda_mu = prior_hpar['lambda_mu']
+        self.prior_lambda_mu = prior_lambda_mu
         # prior natural hyperparameters
         self.prior_tau1 = self.prior_lambda_mu*self.prior_m_mu
         self.prior_tau2 = -self.prior_beta_xi - 0.5*self.T*self.prior_lambda_mu*self.prior_m_mu**2
         self.prior_tau3 = 2*self.prior_alpha_xi + self.T - 2
         self.prior_tau4 = 0.5*self.prior_lambda_mu
         self.h_prior_tau = 0.5*self.T*np.log(2*np.pi) + loggamma(self.prior_alpha_xi) - self.prior_alpha_xi*np.log(self.prior_beta_xi) - 0.5*self.T*np.log(self.prior_lambda_mu) # prior log-normalizer for each of the observed variables
         # set up other variables
@@ -218,15 +215,15 @@
     def _E_log_prior_eta(self):
         '''
         Variational expectation of the log-prior of likelihood parameters (eta).
         '''
         return np.sum(np.sum(self.prior_tau1*self.E_xi_mu, axis = 1) + self.prior_tau2*self.E_xi + 0.5*self.prior_tau3*self.E_log_xi - np.sum(self.prior_tau4*self.E_xi_mu2, axis = 1) - self.h_prior_tau)
     
     @abstractmethod
-    def _initialize_q_pi(self, prior_hpar):
+    def _initialize_q_pi(self, **prior_hpar):
         '''
         Initialize the variational distribution of latent class/profile base rates (pi).
         '''
         pass
     
     @abstractmethod
     def _update_q_pi(self):
```

### Comparing `vbayesfa-0.0.22/src/vbayesfa/old_lpa.py` & `vbayesfa-0.0.23/src/vbayesfa/old_lpa.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.22/src/vbayesfa/simulate_data.py` & `vbayesfa-0.0.23/src/vbayesfa/simulate_data.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.22/src/vbayesfa/tests/.DS_Store` & `vbayesfa-0.0.23/src/vbayesfa/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.22/src/vbayesfa/tests/test_exp_families.py` & `vbayesfa-0.0.23/src/vbayesfa/tests/test_exp_families.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.22/src/vbayesfa/tests/test_lpa.py` & `vbayesfa-0.0.23/src/vbayesfa/tests/test_lpa.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import numpy as np
-import pandas as pd
 from numpy.testing import *
 from vbayesfa.fit_lpa import fit_lpa
-from scipy.stats import norm as norm_dist
+from vbayesfa import simulate_data
 
 # to run all tests: pytest /Users/sampaskewitz/Documents/vbayesfa/src/vbayesfa/tests
 
-def _simulate_test_lpa_data():
-    # create simple synthetic data
-    z = np.array(5*[0, 0, 0, 0, 0, 1, 1, 1, 2, 2]) # profile membership
-    n = z.shape[0] # number of participants/observations
-    m = 4 # number of observed variables
-    mu = np.array(m*[0, 2, -2]).reshape([m, 3]) # profile means
-    x = np.zeros([m, n]) # empty array for observed data
-    for i in range(n):
-        x[:, i] = norm_dist.rvs(loc = mu[:, z[i]], random_state = i) # fill in x
-    return x
-
 def test_fit_lpa():
     # create simple synthetic data
-    x = _simulate_test_lpa_data()
+    sim_data = simulate_data.latent_profile(n = 20, 
+                                            m = 5,
+                                            separation = 3.0,
+                                            n_profiles = 2,
+                                            sample_z = True,
+                                            seed = 1234,
+                                            mu = None,
+                                            pi = None)
 
     # fit the model
-    model = fit_lpa(x, T = 20, seed = 1234)['best_model']
-
-    # spot check results
-    assert_equal(model.z_hat,
-                 np.array([1, 0, 0, 0, 0, 1, 1, 1, 2, 2, 0, 0, 0, 0, 0, 1, 1, 1, 2, 2, 0, 0, 0, 0, 0, 1, 1, 1, 2, 2, 0, 0, 0, 0, 0, 0, 1, 1, 2, 2, 0, 0, 0, 0, 0, 1, 1, 1, 2, 2]))
-    assert_almost_equal(model.sorted_m_mu[:,0],
-                        np.array([0.28440915, -0.00614277, -0.21887377, -0.39339402]))
-    assert_almost_equal(model.sorted_m_mu[:,1],
-                        np.array([2.13501792, 1.87225139, 2.12624529, 1.92444134]))
-    assert_almost_equal(model.sorted_m_mu[:,2],
-                        np.array([-1.82014314, -1.62427792, -2.09733365, -2.02264288]))
-    assert_almost_equal(model.E_xi,
-                        np.array([1.21540675, 0.93334809, 0.99248329, 0.82400854]))
+    model = fit_lpa(sim_data['x'], 
+                    prior_w1 = 3.0,
+                    prior_w2 = 1.0,
+                    prior_lambda_mu = 0.5,
+                    prior_strength_for_xi = 10.0,
+                    max_iter = 50, 
+                    min_iter = 30, 
+                    restarts = 4, 
+                    T = 20, 
+                    tolerance = 1e-5, 
+                    seed = 1234)['best_model']
+    model.print_summary()
+    assert_equal(model.z_hat, np.array([0, 0, 1, 0, 0, 1, 0, 1, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 1, 1]))
+    assert_almost_equal(model.sorted_m_mu[:,0], np.array([1.49505099, 1.27884819, -2.37783417, -2.19846618, -1.26139709]))
+    assert_almost_equal(model.sorted_m_mu[:,1], np.array([1.01461892, 4.74435739, 1.54366584, 0.70047062, 2.47352321]))
+    assert_almost_equal(model.elbo_list[-1], -116.39303540575003)
```

### Comparing `vbayesfa-0.0.22/src/vbayesfa/tests/test_lpa_outcome_analysis.py` & `vbayesfa-0.0.23/src/vbayesfa/tests/test_lpa_outcome_analysis.py`

 * *Files identical despite different names*

