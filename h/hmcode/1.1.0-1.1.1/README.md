# Comparing `tmp/hmcode-1.1.0.tar.gz` & `tmp/hmcode-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmcode-1.1.0.tar", max compression
+gzip compressed data, was "hmcode-1.1.1.tar", max compression
```

## Comparing `hmcode-1.1.0.tar` & `hmcode-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1023 2023-02-22 15:20:40.854089 hmcode-1.1.0/LICENSE
--rw-r--r--   0        0        0     9291 2023-04-23 14:27:19.425647 hmcode-1.1.0/README.md
--rw-r--r--   0        0        0       25 2023-04-14 21:37:50.414430 hmcode-1.1.0/hmcode/__init__.py
--rw-r--r--   0        0        0     1879 2023-04-23 14:27:19.428579 hmcode-1.1.0/hmcode/camb_stuff.py
--rw-r--r--   0        0        0      641 2023-04-23 14:27:19.429409 hmcode-1.1.0/hmcode/constants.py
--rw-r--r--   0        0        0    10200 2023-04-23 14:27:19.429907 hmcode-1.1.0/hmcode/cosmology.py
--rw-r--r--   0        0        0    17838 2023-04-23 14:27:19.430740 hmcode-1.1.0/hmcode/hmcode.py
--rw-r--r--   0        0        0     3882 2023-04-23 14:27:19.431432 hmcode-1.1.0/hmcode/linear_growth.py
--rw-r--r--   0        0        0     1690 2023-04-23 14:27:19.431902 hmcode-1.1.0/hmcode/utility.py
--rw-r--r--   0        0        0      557 2023-04-23 14:28:26.892650 hmcode-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    10180 1970-01-01 00:00:00.000000 hmcode-1.1.0/setup.py
--rw-r--r--   0        0        0    10132 1970-01-01 00:00:00.000000 hmcode-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1023 2023-03-01 16:41:47.399743 hmcode-1.1.1/LICENSE
+-rw-r--r--   0        0        0     9291 2024-04-26 21:36:52.190292 hmcode-1.1.1/README.md
+-rw-r--r--   0        0        0       25 2023-03-01 16:41:47.400313 hmcode-1.1.1/hmcode/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-26 21:36:52.190802 hmcode-1.1.1/hmcode/camb_stuff.py
+-rw-r--r--   0        0        0      641 2024-04-26 21:36:52.190950 hmcode-1.1.1/hmcode/constants.py
+-rw-r--r--   0        0        0    10221 2024-04-26 21:36:57.910280 hmcode-1.1.1/hmcode/cosmology.py
+-rw-r--r--   0        0        0    17838 2024-04-26 21:36:52.191441 hmcode-1.1.1/hmcode/hmcode.py
+-rw-r--r--   0        0        0     3882 2024-04-26 21:36:52.191790 hmcode-1.1.1/hmcode/linear_growth.py
+-rw-r--r--   0        0        0     1690 2024-04-26 21:36:52.191952 hmcode-1.1.1/hmcode/utility.py
+-rw-r--r--   0        0        0      557 2024-04-26 21:36:57.910615 hmcode-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10133 1970-01-01 00:00:00.000000 hmcode-1.1.1/PKG-INFO
```

### Comparing `hmcode-1.1.0/LICENSE` & `hmcode-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hmcode-1.1.0/README.md` & `hmcode-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,20 +50,20 @@
 To whom it may concern,
 
 I coded this `Python` version of `HMcode-2020` ([Mead et al. 2021](https://arxiv.org/abs/2009.01858)) up quite quickly before leaving academia in February 2023. It is written in pure `Python` and doesn't use any of the original Fortran code whatsoever. There is something amazing/dispiriting about coding something up in 3 days that previously took 5 years. A tragic last hoorah! At least I switched to `Python` eventually...
 
 You might also be interested in [`pyhalomodel`](https://pypi.org/project/pyhalomodel/), upon which this code depends, which implements a vanilla halo-model calculation for any desired large-scale-structure tracer. Alternatively, and very confusingly, you might be interested in this [`pyhmcode`](https://pypi.org/project/pyhmcode/), which provides a wrapper around the original `Fortran` `HMcode` implementation.
 
 I compared it against the `CAMB-HMcode` version for 100 random sets of cosmological parameters ($k < 10 h\mathrm{Mpc}^{-1}$; $z < 3$). The level of agreement between the two codes is as follows:
-- LCDM: Mean error: 0.10%; Standard deviation of error: 0.03%; Worst-case error; 0.21%
-- k-LCDM: Mean error: 0.11%; Standard deviation of error: 0.03%; Worst-case error; 0.23%
-- w-CDM: Mean error: 0.10%; Standard deviation of error: 0.03%; Worst-case error; 0.20%
-- w(a)-CDM: Mean error: 0.13%; Standard deviation of error: 0.06%; Worst-case error; 0.48%
-- nu-LCDM: Mean error: 0.47%; Standard deviation of error: 0.44%; Worst-case error; 2.01% (larger errors strongly correlated with neutrino mass)
-- nu-k-w(a)-CDM: Mean error: 0.42%; Standard deviation of error: 0.43%; Worst-case error; 2.02% (larger errors strongly correlated with neutrino mass)
+- LCDM: Mean error: 0.10%; Standard deviation of error: 0.03%; Worst-case error; 0.28%
+- k-LCDM: Mean error: 0.12%; Standard deviation of error: 0.04%; Worst-case error; 0.32%
+- w-CDM: Mean error: 0.11%; Standard deviation of error: 0.03%; Worst-case error; 0.31%
+- w(a)-CDM: Mean error: 0.14%; Standard deviation of error: 0.08%; Worst-case error; 0.77%
+- nu-LCDM: Mean error: 0.45%; Standard deviation of error: 0.43%; Worst-case error; 1.97% (larger errors strongly correlated with neutrino mass)
+- nu-k-w(a)-CDM: Mean error: 0.41%; Standard deviation of error: 0.42%; Worst-case error; 1.99% (larger errors strongly correlated with neutrino mass)
 
 These comparisons can be reproduced using the `comparisons/CAMB.py` script.
 
 The power-spectrum suppression caused by baryonic feedback has also been implemented, and the level of agreement between the *suppression* predicted by this code and the same implementation in `CAMB` is as follows:
 - LCDM: Mean error: 0.02%; Standard deviation of error: <0.01%; Worst-case error; 0.03%
 - nu-k-w(a)-CDM: Mean error: 0.06%; Standard deviation of error: 0.07%; Worst-case error; 0.49% (larger errors strongly correlated with neutrino mass)
```

### Comparing `hmcode-1.1.0/hmcode/camb_stuff.py` & `hmcode-1.1.1/hmcode/camb_stuff.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import camb
 
 def run(zs, Omega_c, Omega_b, Omega_k, h, ns, sigma_8, 
     m_nu=0., w=-1., wa=0., log10_T_AGN=None,
     As=2e-9, norm_sigma8=True, kmax_CAMB=200., verbose=False):
 
     # Sets cosmological parameters in camb to calculate the linear power spectrum
-    # TODO: Setting 'WantCls=False' in CAMBparams spoils the agreement... why?
     if log10_T_AGN:
         non_linear_model = camb.nonlinear.Halofit(halofit_version="mead2020_feedback", 
                                                   HMCode_logT_AGN=log10_T_AGN)
     else:
         non_linear_model = camb.nonlinear.Halofit(halofit_version="mead2020")
-    pars = camb.CAMBparams(NonLinearModel=non_linear_model) 
+    # TODO: Setting 'WantCls=True' in CAMBparams changes the power a small amount, not sure why
+    pars = camb.CAMBparams(NonLinearModel=non_linear_model, WantCls=False)
     wb, wc = Omega_b*h**2, Omega_c*h**2
 
     # This function sets standard and helium set using BBN consistency
     pars.set_cosmology(ombh2=wb, omch2=wc, H0=100.*h, mnu=m_nu, omk=Omega_k)
     pars.set_dark_energy(w=w, wa=wa, dark_energy_model='ppf')
     pars.InitPower.set_params(As=As, ns=ns, r=0.)
     pars.set_matter_power(redshifts=zs, kmax=kmax_CAMB) # Linear matter power spectrum
```

### Comparing `hmcode-1.1.0/hmcode/constants.py` & `hmcode-1.1.1/hmcode/constants.py`

 * *Files identical despite different names*

### Comparing `hmcode-1.1.0/hmcode/cosmology.py` & `hmcode-1.1.1/hmcode/cosmology.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 # Constants
 Dv0 = 18.*np.pi**2                  # Delta_v = ~178, EdS halo virial overdensity
 dc0 = (3./20.)*(12.*np.pi)**(2./3.) # delta_c = ~1.686' EdS linear collapse threshold
 
 # Parameters
 xmin_Tk = 1e-5    # Scale at which to switch to Taylor expansion approximation in tophat Fourier functions
-eps_sigmaR = 1e-4 # Accuracy of the sigmaR integration
-eps_sigmaV = 1e-4 # Accuracy of the sigmaV integration
-eps_neff = 1e-4   # Accuracy of the neff integration (d ln sigma^2/d ln k)
+eps_sigmaR = 1e-4 # Relative accuracy of the sigmaR integration
+eps_sigmaV = 1e-4 # Relative accuracy of the sigmaV integration
+eps_neff = 1e-4   # Relative accuracy of the neff integration (d ln sigma^2/d ln k)
 
 ### Backgroud ###
 
 def redshift_from_scalefactor(a:float) -> float:
     return -1.+1./a
 
 
@@ -121,18 +121,18 @@
     args:
         R: Comoving Lagrangian radius [Mpc/h]
         Pk: Function of k to evaluate the linear power spectrum
     '''
     def sigmaR_vec(R:float, Pk:callable):
         if transform_integrand:
              sigmaR_squared, _ = integrate.quad(lambda t: _transformed_integrand(t, R, Pk, _sigmaR_integrand), 
-                                                0., 1., epsabs=eps, epsrel=eps)
+                                                0., 1., epsabs=0., epsrel=eps)
         else:
             sigmaR_squared, _ = integrate.quad(lambda k: _sigmaR_integrand(k, R, Pk), 
-                                               kmin, kmax, epsabs=eps, epsrel=eps)
+                                               kmin, kmax, epsabs=0., epsrel=eps)
         sigmaR = np.sqrt(sigmaR_squared/(2.*np.pi**2))
         return sigmaR
     sigmaR_func = np.vectorize(sigmaR_vec, excluded=['Pk'])
     return sigmaR_func(R, Pk)
 
 
 def _sigmaV_integrand(k:np.ndarray, R:float, Pk:callable) -> np.ndarray:
@@ -152,18 +152,18 @@
     TODO: I should look at how CAMB deals with these type of integrals (e.g., sigmaR).
     args:
         Pk: Function of k to evaluate the linear power spectrum
         eps: Integration accuracy
     '''
     if transform_integrand:
         sigmaV_squared, _ = integrate.quad(lambda t: _transformed_integrand(t, R, Pk, _sigmaV_integrand), 
-                                           0., 1., epsabs=eps, epsrel=eps)
+                                           0., 1., epsabs=0., epsrel=eps)
     else:
         sigmaV_squared, _ = integrate.quad(lambda k: _sigmaV_integrand(k, R, Pk), 
-                                           kmin, kmax, epsabs=eps, epsrel=eps)
+                                           kmin, kmax, epsabs=0., epsrel=eps)
     sigmaV = np.sqrt(sigmaV_squared/(2.*np.pi**2))
     sigmaV /= np.sqrt(3.) # Convert from 3D displacement to 1D displacement
     return sigmaV
 
 
 def _dsigmaR_integrand(k:float, R:float, Pk:callable) -> float:
     return Pk(k)*(k**3)*_Tophat_k(k*R)*_dTophat_k(k*R)
@@ -173,18 +173,18 @@
     '''
     Calculates d(ln sigma^2)/d(ln R) by integration
     3+neff = -d(ln sigma^2) / dR
     TODO: This is slow, regardless of whether transform_integrand is set or not
     '''
     if transform_integrand:
         dsigma, _ = integrate.quad(lambda t: _transformed_integrand(t, R, Pk, _dsigmaR_integrand), 
-                                   0., 1., epsabs=eps, epsrel=eps)
+                                   0., 1., epsabs=0., epsrel=eps)
     else:
         dsigma, _ = integrate.quad(lambda k: _dsigmaR_integrand(k, R, Pk), 
-                                   kmin, kmax, epsabs=eps, epsrel=eps)
+                                   kmin, kmax, epsabs=0., epsrel=eps)
     dsigma = R*dsigma/(np.pi*sigmaR(R, Pk))**2
     return dsigma
 
 
 def neff(R:float, Pk:callable) -> float:
     '''
     Effective index of the power spectrum at scale 'R'
```

### Comparing `hmcode-1.1.0/hmcode/hmcode.py` & `hmcode-1.1.1/hmcode/hmcode.py`

 * *Files identical despite different names*

### Comparing `hmcode-1.1.0/hmcode/linear_growth.py` & `hmcode-1.1.1/hmcode/linear_growth.py`

 * *Files identical despite different names*

### Comparing `hmcode-1.1.0/hmcode/utility.py` & `hmcode-1.1.1/hmcode/utility.py`

 * *Files identical despite different names*

### Comparing `hmcode-1.1.0/pyproject.toml` & `hmcode-1.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "hmcode"
-version = "1.1.0"
+version = "1.1.1"
 description = "Pure Python implementation of HMcode"
 authors = ["Alexander Mead <alexander.j.mead@googlemail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/alexander-mead/HMcode-python"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.9,<3.13"
 numpy = "^1.24.2"
 scipy = "^1.10.1"
 camb = "^1.4.0"
-pyhalomodel = "^1.0.1"
+pyhalomodel = "^1.0.2"
 
 [tool.poetry.group.dev.dependencies]
 matplotlib = "^3.7.0"
 ipykernel = "^6.21.2"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `hmcode-1.1.0/setup.py` & `hmcode-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,126 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: hmcode
+Version: 1.1.1
+Summary: Pure Python implementation of HMcode
+Home-page: https://github.com/alexander-mead/HMcode-python
+License: MIT
+Author: Alexander Mead
+Author-email: alexander.j.mead@googlemail.com
+Requires-Python: >=3.9,<3.13
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: camb (>=1.4.0,<2.0.0)
+Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: pyhalomodel (>=1.0.2,<2.0.0)
+Requires-Dist: scipy (>=1.10.1,<2.0.0)
+Project-URL: Repository, https://github.com/alexander-mead/HMcode-python
+Description-Content-Type: text/markdown
+
+# HMcode
+
+![image](https://user-images.githubusercontent.com/9140961/228345397-f33d2f94-e8e4-4eb0-9fc9-9b27df407fbc.png)
+
+A pure-`Python` implementation of the `HMcode-2020` method ([Mead et al. 2021](https://arxiv.org/abs/2009.01858)) for computing accurate non-linear matter power spectra across a wide range of cosmological parameters for $w(a)$-CDM models including curvature and massive neutrinos.
+
+## Installation
+
+Either
+```bash
+> pip install hmcode
+```
+or, if you want to edit the code, use the demo notebook, or run the tests or consistency checks, then clone the repository, `cd` into the directory, and then
+```bash
+> poetry install
+```
+to create a virtual environment with everything you need to get going.
+
+## Dependencies
+
+- `numpy`
+- `scipy`
+- `camb`
+- `pyhalomodel`
+
+## Use
+
+```
+import numpy as np
+import camb
+import hmcode
+
+# Ranges
+k = np.logspace(-3, 1, 100) # Wavenumbers [h/Mpc]
+zs = [3., 2., 1., 0.5, 0.]  # Redshifts
+T_AGN = 10**7.8             # Feedback temperature [K]
+
+# Run CAMB
+parameters = camb.CAMBparams(WantCls=False)
+parameters.set_cosmology(H0=70.)
+parameters.set_matter_power(redshifts=zs, kmax=100.) # kmax should be much larger than the wavenumber of interest
+results = camb.get_results(parameters)
+
+# HMcode
+Pk = hmcode.power(k, zs, results, T_AGN)
+```
+
+## Note
+
+To whom it may concern,
+
+I coded this `Python` version of `HMcode-2020` ([Mead et al. 2021](https://arxiv.org/abs/2009.01858)) up quite quickly before leaving academia in February 2023. It is written in pure `Python` and doesn't use any of the original Fortran code whatsoever. There is something amazing/dispiriting about coding something up in 3 days that previously took 5 years. A tragic last hoorah! At least I switched to `Python` eventually...
+
+You might also be interested in [`pyhalomodel`](https://pypi.org/project/pyhalomodel/), upon which this code depends, which implements a vanilla halo-model calculation for any desired large-scale-structure tracer. Alternatively, and very confusingly, you might be interested in this [`pyhmcode`](https://pypi.org/project/pyhmcode/), which provides a wrapper around the original `Fortran` `HMcode` implementation.
+
+I compared it against the `CAMB-HMcode` version for 100 random sets of cosmological parameters ($k < 10 h\mathrm{Mpc}^{-1}$; $z < 3$). The level of agreement between the two codes is as follows:
+- LCDM: Mean error: 0.10%; Standard deviation of error: 0.03%; Worst-case error; 0.28%
+- k-LCDM: Mean error: 0.12%; Standard deviation of error: 0.04%; Worst-case error; 0.32%
+- w-CDM: Mean error: 0.11%; Standard deviation of error: 0.03%; Worst-case error; 0.31%
+- w(a)-CDM: Mean error: 0.14%; Standard deviation of error: 0.08%; Worst-case error; 0.77%
+- nu-LCDM: Mean error: 0.45%; Standard deviation of error: 0.43%; Worst-case error; 1.97% (larger errors strongly correlated with neutrino mass)
+- nu-k-w(a)-CDM: Mean error: 0.41%; Standard deviation of error: 0.42%; Worst-case error; 1.99% (larger errors strongly correlated with neutrino mass)
+
+These comparisons can be reproduced using the `comparisons/CAMB.py` script.
+
+The power-spectrum suppression caused by baryonic feedback has also been implemented, and the level of agreement between the *suppression* predicted by this code and the same implementation in `CAMB` is as follows:
+- LCDM: Mean error: 0.02%; Standard deviation of error: <0.01%; Worst-case error; 0.03%
+- nu-k-w(a)-CDM: Mean error: 0.06%; Standard deviation of error: 0.07%; Worst-case error; 0.49% (larger errors strongly correlated with neutrino mass)
+
+The comparisons can be reproduced using the `comparisons/CAMB_feedback.py` script.
+
+While the quoted accuracy of `HMcode-2020` relative to simulations is RMS ~2.5%, note that the accuracy is anti-correlated with neutrino masses (cf. Fig. 2 of [Mead et al. 2021](https://arxiv.org/abs/2009.01858)). The larger discrepancies between the codes for massive neutrinos (2% for ~1eV) may seem worrisome, but here are some reasons why I am not that worried:
+- Here, neutrinos are treated as completely cold matter when calculating the linear growth factors, whereas in `CAMB-HMcode` the transition from behaving like radiation to behaving like matter is accounted for in the linear growth.
+- Here the *cold* matter power spectrum is taken directly from `CAMB` whereas in `CAMB-HMcode` the *cold* spectrum is calculated approximately from the total matter power spectrum using approximations for the scale-dependent growth rate from [Eisenstein & Hu (1999)](https://arxiv.org/abs/astro-ph/9710252).
+- If I resort to the old approximation for the *cold* matter power spectrum (and therefore the cold $\sigma(R)$) then the level of agreement between the codes for nu-k-w(a)-CDM improves to: Mean error: 0.15%; Std error: 0.11%; Worst error; 1.15%.
+
+Using the actual cold matter spectrum is definitely an improvement from a theoretical perspective (and for speed), so I decided to keep that at the cost of the disagreement between this code at `CAMB-HMcode` for models with very high neutrino mass. If better agreement between this code and `CAMB-HMcode` is important to you then the old approximate cold spectrum can be used by changing the `sigma_cold_approx` flag at the top of `hmcode.py`. Note that while ignoring the actual energy-density scaling of massive neutrinos might seem to be a (small) problem, keep in mind the comments below regarding the linear growth factor.
+
+I think any residual differences between codes must therefore stem from:
+- The BAO de-wiggling process (different `k` grids)
+- The $\sigma_\mathrm{v}$ numerical integration
+- The $n_\mathrm{eff}$ calculation (numerical differentiation here; numerical integration in `CAMB-HMcode`)
+- The $\sigma(R)$ numerical integration (using `CAMB` here; done internally in `CAMB-HMcode`)
+- The linear growth ODE solution
+- Root finding for the halo-collapse redshift and for $R_\mathrm{nl}$
+
+But I didn't have time to investigate these differences more thoroughly. Note that there are accuracy parameters in `CAMB-HMcode` fixed at the $10^{-4}$ level, so you would never expect better than 0.01% agreement. Given that `HMcode` is only accurate at the ~2.5% level compared to simulated power spectra, the level of agreement between the codes seems okay to me, with the caveats above regarding very massive neutrinos.
+
+While writing this code I had a few ideas for future improvements:
+- ~~Add the `HMcode-2020` baryon-feedback model; this would not be too hard for the enthusiastic student/postdoc.~~ (Thanks Laila Linke!)
+- The predictions are a bit sensitive to the smoothing $\sigma$ used for the dewiggling. This should probably be a fitted parameter.
+- It's annoying having to calculate linear growth functions (all, LCDM), especially since the linear growth doesn't really exist. One should probably use the $P(k)$ amplitude evolution over time at some cleverly chosen scale instead, or instead the evolution of $\sigma(R)$ over time at some pertinent $R$ value. Note that the growth factors are *only* used to calculate the [Dolag et al. (2004)](https://arxiv.org/abs/astro-ph/0309771) correction and [Mead (2017)](https://arxiv.org/abs/1606.05345) $\delta_\mathrm{c}$, $\Delta_\mathrm{v}$.
+- I never liked the halo bloating parameter, it's hard to understand the effect of modifying halo profiles in Fourier space. Someone should get rid of this (maybe modify the halo mass function instead?).
+- Redshift 'infinity' for the Dolag correction is actually $z_\infty = 10$. `HMcode` predictions *are* sensitive to this (particularly w(a)CDM). Either the redshift 'infinity' should be fitted or the halo-concentration model for beyond-LCDM should be improved.
+- The massive neutrino correction for the [Mead (2017)](https://arxiv.org/abs/1606.05345) $\delta_\mathrm{c}$, $\Delta_\mathrm{v}$ formulae (appendix A of [Mead et al. 2021](https://arxiv.org/abs/2009.01858)) is crude and should be improved. I guess using the intuition that hot neutrinos are ~smoothly distributed on halo scales. Currently neutrinos are treated as cold matter in the linear/accumulated growth calculation (used by [Mead 2017](https://arxiv.org/abs/1606.05345)), which seems a bit wrong.
+- I haven't checked how fast this code is, but there are a couple of TODO in the code that might improve speed if necessary.
+- The choices regarding how to account for massive neutrinos could usefully be revisited. This whole subject is a bit confusing and the code doesn't help to alleviate the confusion. Choices like what to use for: $\delta_\mathrm{c}$; $\Delta_\mathrm{v}$; $\sigma(R)$; $R_\mathrm{nl}$; $n_\mathrm{eff}$; $c(M)$.
+- Refit model (including $\sigma$ for BAO smoothing and $z_\infty$ for [Dolag et al. 2004](https://arxiv.org/abs/astro-ph/0309771)) to new emulator(s) (e.g., [Mira Titan IV](https://arxiv.org/abs/2207.12345)).
+- Don't be under any illusions that the `HMcode` parameters, or the forms of their dependence on the underlying power spectrum, are special in any particular way. A lot of experimentation went into finding these, but it was by no means exhaustive. However, please note that obviously these parameters should only depend on the underlying linear spectrum (rather than being random functions of $z$, $\Omega_\mathrm{m}$, $w$, or whatever).
 
-packages = \
-['hmcode']
+Have fun,
 
-package_data = \
-{'': ['*']}
+Alexander Mead (2023/02/28)
 
-install_requires = \
-['camb>=1.4.0,<2.0.0',
- 'numpy>=1.24.2,<2.0.0',
- 'pyhalomodel>=1.0.1,<2.0.0',
- 'scipy>=1.10.1,<2.0.0']
-
-setup_kwargs = {
-    'name': 'hmcode',
-    'version': '1.1.0',
-    'description': 'Pure Python implementation of HMcode',
-    'long_description': "# HMcode\n\n![image](https://user-images.githubusercontent.com/9140961/228345397-f33d2f94-e8e4-4eb0-9fc9-9b27df407fbc.png)\n\nA pure-`Python` implementation of the `HMcode-2020` method ([Mead et al. 2021](https://arxiv.org/abs/2009.01858)) for computing accurate non-linear matter power spectra across a wide range of cosmological parameters for $w(a)$-CDM models including curvature and massive neutrinos.\n\n## Installation\n\nEither\n```bash\n> pip install hmcode\n```\nor, if you want to edit the code, use the demo notebook, or run the tests or consistency checks, then clone the repository, `cd` into the directory, and then\n```bash\n> poetry install\n```\nto create a virtual environment with everything you need to get going.\n\n## Dependencies\n\n- `numpy`\n- `scipy`\n- `camb`\n- `pyhalomodel`\n\n## Use\n\n```\nimport numpy as np\nimport camb\nimport hmcode\n\n# Ranges\nk = np.logspace(-3, 1, 100) # Wavenumbers [h/Mpc]\nzs = [3., 2., 1., 0.5, 0.]  # Redshifts\nT_AGN = 10**7.8             # Feedback temperature [K]\n\n# Run CAMB\nparameters = camb.CAMBparams(WantCls=False)\nparameters.set_cosmology(H0=70.)\nparameters.set_matter_power(redshifts=zs, kmax=100.) # kmax should be much larger than the wavenumber of interest\nresults = camb.get_results(parameters)\n\n# HMcode\nPk = hmcode.power(k, zs, results, T_AGN)\n```\n\n## Note\n\nTo whom it may concern,\n\nI coded this `Python` version of `HMcode-2020` ([Mead et al. 2021](https://arxiv.org/abs/2009.01858)) up quite quickly before leaving academia in February 2023. It is written in pure `Python` and doesn't use any of the original Fortran code whatsoever. There is something amazing/dispiriting about coding something up in 3 days that previously took 5 years. A tragic last hoorah! At least I switched to `Python` eventually...\n\nYou might also be interested in [`pyhalomodel`](https://pypi.org/project/pyhalomodel/), upon which this code depends, which implements a vanilla halo-model calculation for any desired large-scale-structure tracer. Alternatively, and very confusingly, you might be interested in this [`pyhmcode`](https://pypi.org/project/pyhmcode/), which provides a wrapper around the original `Fortran` `HMcode` implementation.\n\nI compared it against the `CAMB-HMcode` version for 100 random sets of cosmological parameters ($k < 10 h\\mathrm{Mpc}^{-1}$; $z < 3$). The level of agreement between the two codes is as follows:\n- LCDM: Mean error: 0.10%; Standard deviation of error: 0.03%; Worst-case error; 0.21%\n- k-LCDM: Mean error: 0.11%; Standard deviation of error: 0.03%; Worst-case error; 0.23%\n- w-CDM: Mean error: 0.10%; Standard deviation of error: 0.03%; Worst-case error; 0.20%\n- w(a)-CDM: Mean error: 0.13%; Standard deviation of error: 0.06%; Worst-case error; 0.48%\n- nu-LCDM: Mean error: 0.47%; Standard deviation of error: 0.44%; Worst-case error; 2.01% (larger errors strongly correlated with neutrino mass)\n- nu-k-w(a)-CDM: Mean error: 0.42%; Standard deviation of error: 0.43%; Worst-case error; 2.02% (larger errors strongly correlated with neutrino mass)\n\nThese comparisons can be reproduced using the `comparisons/CAMB.py` script.\n\nThe power-spectrum suppression caused by baryonic feedback has also been implemented, and the level of agreement between the *suppression* predicted by this code and the same implementation in `CAMB` is as follows:\n- LCDM: Mean error: 0.02%; Standard deviation of error: <0.01%; Worst-case error; 0.03%\n- nu-k-w(a)-CDM: Mean error: 0.06%; Standard deviation of error: 0.07%; Worst-case error; 0.49% (larger errors strongly correlated with neutrino mass)\n\nThe comparisons can be reproduced using the `comparisons/CAMB_feedback.py` script.\n\nWhile the quoted accuracy of `HMcode-2020` relative to simulations is RMS ~2.5%, note that the accuracy is anti-correlated with neutrino masses (cf. Fig. 2 of [Mead et al. 2021](https://arxiv.org/abs/2009.01858)). The larger discrepancies between the codes for massive neutrinos (2% for ~1eV) may seem worrisome, but here are some reasons why I am not that worried:\n- Here, neutrinos are treated as completely cold matter when calculating the linear growth factors, whereas in `CAMB-HMcode` the transition from behaving like radiation to behaving like matter is accounted for in the linear growth.\n- Here the *cold* matter power spectrum is taken directly from `CAMB` whereas in `CAMB-HMcode` the *cold* spectrum is calculated approximately from the total matter power spectrum using approximations for the scale-dependent growth rate from [Eisenstein & Hu (1999)](https://arxiv.org/abs/astro-ph/9710252).\n- If I resort to the old approximation for the *cold* matter power spectrum (and therefore the cold $\\sigma(R)$) then the level of agreement between the codes for nu-k-w(a)-CDM improves to: Mean error: 0.15%; Std error: 0.11%; Worst error; 1.15%.\n\nUsing the actual cold matter spectrum is definitely an improvement from a theoretical perspective (and for speed), so I decided to keep that at the cost of the disagreement between this code at `CAMB-HMcode` for models with very high neutrino mass. If better agreement between this code and `CAMB-HMcode` is important to you then the old approximate cold spectrum can be used by changing the `sigma_cold_approx` flag at the top of `hmcode.py`. Note that while ignoring the actual energy-density scaling of massive neutrinos might seem to be a (small) problem, keep in mind the comments below regarding the linear growth factor.\n\nI think any residual differences between codes must therefore stem from:\n- The BAO de-wiggling process (different `k` grids)\n- The $\\sigma_\\mathrm{v}$ numerical integration\n- The $n_\\mathrm{eff}$ calculation (numerical differentiation here; numerical integration in `CAMB-HMcode`)\n- The $\\sigma(R)$ numerical integration (using `CAMB` here; done internally in `CAMB-HMcode`)\n- The linear growth ODE solution\n- Root finding for the halo-collapse redshift and for $R_\\mathrm{nl}$\n\nBut I didn't have time to investigate these differences more thoroughly. Note that there are accuracy parameters in `CAMB-HMcode` fixed at the $10^{-4}$ level, so you would never expect better than 0.01% agreement. Given that `HMcode` is only accurate at the ~2.5% level compared to simulated power spectra, the level of agreement between the codes seems okay to me, with the caveats above regarding very massive neutrinos.\n\nWhile writing this code I had a few ideas for future improvements:\n- ~~Add the `HMcode-2020` baryon-feedback model; this would not be too hard for the enthusiastic student/postdoc.~~ (Thanks Laila Linke!)\n- The predictions are a bit sensitive to the smoothing $\\sigma$ used for the dewiggling. This should probably be a fitted parameter.\n- It's annoying having to calculate linear growth functions (all, LCDM), especially since the linear growth doesn't really exist. One should probably use the $P(k)$ amplitude evolution over time at some cleverly chosen scale instead, or instead the evolution of $\\sigma(R)$ over time at some pertinent $R$ value. Note that the growth factors are *only* used to calculate the [Dolag et al. (2004)](https://arxiv.org/abs/astro-ph/0309771) correction and [Mead (2017)](https://arxiv.org/abs/1606.05345) $\\delta_\\mathrm{c}$, $\\Delta_\\mathrm{v}$.\n- I never liked the halo bloating parameter, it's hard to understand the effect of modifying halo profiles in Fourier space. Someone should get rid of this (maybe modify the halo mass function instead?).\n- Redshift 'infinity' for the Dolag correction is actually $z_\\infty = 10$. `HMcode` predictions *are* sensitive to this (particularly w(a)CDM). Either the redshift 'infinity' should be fitted or the halo-concentration model for beyond-LCDM should be improved.\n- The massive neutrino correction for the [Mead (2017)](https://arxiv.org/abs/1606.05345) $\\delta_\\mathrm{c}$, $\\Delta_\\mathrm{v}$ formulae (appendix A of [Mead et al. 2021](https://arxiv.org/abs/2009.01858)) is crude and should be improved. I guess using the intuition that hot neutrinos are ~smoothly distributed on halo scales. Currently neutrinos are treated as cold matter in the linear/accumulated growth calculation (used by [Mead 2017](https://arxiv.org/abs/1606.05345)), which seems a bit wrong.\n- I haven't checked how fast this code is, but there are a couple of TODO in the code that might improve speed if necessary.\n- The choices regarding how to account for massive neutrinos could usefully be revisited. This whole subject is a bit confusing and the code doesn't help to alleviate the confusion. Choices like what to use for: $\\delta_\\mathrm{c}$; $\\Delta_\\mathrm{v}$; $\\sigma(R)$; $R_\\mathrm{nl}$; $n_\\mathrm{eff}$; $c(M)$.\n- Refit model (including $\\sigma$ for BAO smoothing and $z_\\infty$ for [Dolag et al. 2004](https://arxiv.org/abs/astro-ph/0309771)) to new emulator(s) (e.g., [Mira Titan IV](https://arxiv.org/abs/2207.12345)).\n- Don't be under any illusions that the `HMcode` parameters, or the forms of their dependence on the underlying power spectrum, are special in any particular way. A lot of experimentation went into finding these, but it was by no means exhaustive. However, please note that obviously these parameters should only depend on the underlying linear spectrum (rather than being random functions of $z$, $\\Omega_\\mathrm{m}$, $w$, or whatever).\n\nHave fun,\n\nAlexander Mead (2023/02/28)\n",
-    'author': 'Alexander Mead',
-    'author_email': 'alexander.j.mead@googlemail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/alexander-mead/HMcode-python',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.12',
-}
-
-
-setup(**setup_kwargs)
```

