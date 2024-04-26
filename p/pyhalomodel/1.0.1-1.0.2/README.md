# Comparing `tmp/pyhalomodel-1.0.1.tar.gz` & `tmp/pyhalomodel-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhalomodel-1.0.1.tar", max compression
+gzip compressed data, was "pyhalomodel-1.0.2.tar", max compression
```

## Comparing `pyhalomodel-1.0.1.tar` & `pyhalomodel-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1038 2023-02-12 08:54:25.293024 pyhalomodel-1.0.1/LICENSE
--rw-r--r--   0        0        0    11200 2023-02-28 20:22:40.004721 pyhalomodel-1.0.1/README.md
--rw-r--r--   0        0        0       73 2023-02-23 23:12:12.011408 pyhalomodel-1.0.1/pyhalomodel/__init__.py
--rw-r--r--   0        0        0     1595 2023-02-23 23:12:12.011760 pyhalomodel-1.0.1/pyhalomodel/camb_stuff.py
--rw-r--r--   0        0        0      557 2023-02-16 11:29:27.296012 pyhalomodel-1.0.1/pyhalomodel/constants.py
--rw-r--r--   0        0        0     5540 2023-02-23 23:12:12.013020 pyhalomodel-1.0.1/pyhalomodel/cosmology.py
--rw-r--r--   0        0        0    14335 2023-02-16 11:38:53.878251 pyhalomodel-1.0.1/pyhalomodel/darkquest.py
--rw-r--r--   0        0        0    51558 2023-02-28 15:46:09.685484 pyhalomodel-1.0.1/pyhalomodel/pyhalomodel.py
--rw-r--r--   0        0        0     2410 2023-02-28 15:42:14.790929 pyhalomodel-1.0.1/pyhalomodel/utility.py
--rw-r--r--   0        0        0      708 2023-03-09 23:23:32.837358 pyhalomodel-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    12050 1970-01-01 00:00:00.000000 pyhalomodel-1.0.1/setup.py
--rw-r--r--   0        0        0    12027 1970-01-01 00:00:00.000000 pyhalomodel-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1038 2023-03-02 09:21:00.351723 pyhalomodel-1.0.2/LICENSE
+-rw-r--r--   0        0        0    11416 2024-04-26 21:20:15.043058 pyhalomodel-1.0.2/README.md
+-rw-r--r--   0        0        0       73 2023-03-02 09:21:00.358056 pyhalomodel-1.0.2/pyhalomodel/__init__.py
+-rw-r--r--   0        0        0     1595 2023-03-02 09:21:00.358129 pyhalomodel-1.0.2/pyhalomodel/camb_stuff.py
+-rw-r--r--   0        0        0      557 2023-03-02 09:21:00.358194 pyhalomodel-1.0.2/pyhalomodel/constants.py
+-rw-r--r--   0        0        0     5657 2024-04-26 21:20:17.808752 pyhalomodel-1.0.2/pyhalomodel/cosmology.py
+-rw-r--r--   0        0        0    14335 2023-03-02 09:21:00.358427 pyhalomodel-1.0.2/pyhalomodel/darkquest.py
+-rw-r--r--   0        0        0    53856 2024-04-26 21:20:17.809296 pyhalomodel-1.0.2/pyhalomodel/pyhalomodel.py
+-rw-r--r--   0        0        0     2410 2023-03-02 09:21:00.358790 pyhalomodel-1.0.2/pyhalomodel/utility.py
+-rw-r--r--   0        0        0      793 2024-04-26 21:20:17.809517 pyhalomodel-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    12244 1970-01-01 00:00:00.000000 pyhalomodel-1.0.2/PKG-INFO
```

### Comparing `pyhalomodel-1.0.1/LICENSE` & `pyhalomodel-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhalomodel-1.0.1/README.md` & `pyhalomodel-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-# Halo model
-This repository is home to the `pyhalomodel` package, which was written as part of the [Asgari, Mead & Heymans (2023)](https://arxiv.org/) halo-model review paper. The software is written entirely in `Python`, with extendability and reusability in mind. The purpose of this software is to take some of the drudgery out of performing basic calculations using the halo model. While the integrals that the halo model requires the researcher to evaluate are simple, in practice the changes of variables required to integrate halo profiles against halo mass functions can be confusing and tedious. In our experience this confusion has led to bugs and misunderstandings over the years, and our hope for this software is to reduce the proliferation of these somewhat. Our software can produce power spectra for *any* combinations of tracers, and simply requires halo profiles for the tracers to be specified. These could be matter profiles, galaxy profiles, or anything else, for example electron-pressure or HI profiles.
+# `pyhalomodel`
+
+![image](https://user-images.githubusercontent.com/9140961/228342339-e1f908c7-e2ac-46c2-bb2a-1878bbfa3cf0.png)
+
+This repository is home to the `pyhalomodel` package, which was written as part of the [Asgari, Mead & Heymans (2023)](https://arxiv.org/abs/2303.08752) halo-model review paper. The software is written entirely in `Python`, with extendability and reusability in mind. The purpose of this software is to take some of the drudgery out of performing basic calculations using the halo model. While the integrals that the halo model requires the researcher to evaluate are simple, in practice the changes of variables required to integrate halo profiles against halo mass functions can be confusing and tedious. In our experience this confusion has led to bugs and misunderstandings over the years, and our hope for this software is to reduce the proliferation of these somewhat. Our software can produce power spectra for *any* combinations of tracers, and simply requires halo profiles for the tracers to be specified. These could be matter profiles, galaxy profiles, or anything else, for example electron-pressure or HI profiles.
 
 You might also be interested in this pure `Python` implementation of [HMcode](https://github.com/alexander-mead/HMcode-python), which makes use of the `pyhalomodel` package.
 
 ## Dependencies
 * `numpy`
 * `scipy`
 
 ## Installation
 For the general user, `pyhalomodel` can be installed using `pip`:
-```
-pip install pyhalomodel
+```bash
+> pip install pyhalomodel
 ```
 If you you want to modify the source, or use the demo notebooks, then simply clone the repository. You can then create an environment with all necessary dependencies using [poetry](https://python-poetry.org/). From the cloned `pyhalomodel` directory:
-```
-poetry install
+```bash
+> poetry install
 ```
 The demo notebooks require some additional dependencies: `camb`; `dark-emulator`; `ipykernel`; `matplotlib`; `halomod`. These will be installed in the environment automatically. You can also install without `poetry`, either system wide or using another environment manager; we include a `requirements.txt`.
 
 ## Usage
 Start a script with
-```
+```python
 import numpy as np
 import pyhalomodel as halo
 ```
 Importing via `import pyhalomodel as halo` is nice because the functions and classes then have readable names (e.g., `halo.model`, `halo.profile`). To make non-linear power spectrum predictions using the halo model requires a linear power spectrum. In our demonstration notebooks we always take this from `CAMB`, but it could come from any source. Calculations also require the variance in the linear density field when smoothed on comoving scale $R$: $\sigma^2(R)$. Once again, this function could come from any source, but we take it from `CAMB`.
 
 A typical call to create an instance of a `model` object looks like
-```
+```python
 model = halo.model(z, Omega_m, name='Tinker et al. (2010)', Dv=330., dc=1.686, verbose=True)
 ```
 where:
 - `z` is the redshift
 - `Omega_m` is the cosmological matter density parameter (at $z=0$)
 - `name` is the name of the halo mass function/linear halo bias pair to use
 - `Dv` is the halo overdensity definition
@@ -43,28 +46,28 @@
 - `Sheth, Mo & Tormen (2001)`
 - `Tinker et al. (2010)`
 - `Despali et al. (2016)`
 
 When the `model` instance is created the desired mass function is initialised.
 
 To make a power-spectrum calculation one simply calls:
-```
+```python
 Pk_2h, Pk_1h, Pk_hm = model.power_spectrum(k, Pk_lin, M, sigmaM, profiles)
 ```
 where: 
 - `k` is an array of comoving Fourier wavenumbers (units: $h\mathrm{Mpc}^{-1}$)
 - `Pk_lin` is an array of linear power spectrum values at a given `k` (units: $(h^{-1}\mathrm{Mpc})^3$)
 - `M` is an array of halo masses (units: $h^{-1}M_\odot$)
 - `sigmaM` is an array of root-variance linear density values at Lagrangian scales corresponding to `M`
 - `profiles` is a dictionary of halo `profile`s (which could contain a single entry)
 
 The function returns a tuple of `Pk_2h` (two-halo), `Pk_1h` (one-halo), and `Pk_hm` (halo model) power at the chosen `k` values. The `power_spectrum` method computes all possible auto- and cross-spectra given the dictionary of halo profiles. For example, if three profiles were in the dictionary this would compute the three autospectra and the three unique cross spectra. The returned `Pk` are then dictionaries containing all possible spectra. For example, if `profiles={'a':profile_a, 'b':profile_b, 'c':profile_c}` then the `Pk` dictionaries will contain the keys: `a-a`; `a-b`; `a-c`; `b-b`; `b-c`, `c-c`. It will also contain symmetric combinations (e.g., `b-a` as well as `a-b`) but the values will be identical. Each value in the `Pk` dictionary is an array of the power at all `k`.
 
 Halo profiles are instances of the `profile` class. These are initialised in Fourier space like:
-```
+```python
 profile = halo.profile.Fourier(k, M, Uk, amplitude=None, normalisation=1., variance=None, mass_tracer=False, discrete_tracer=False)
 ```
 where
 - `k` is an array of comoving Fourier wavenumbers (units: $h\mathrm{Mpc}^{-1}$)
 - `M` is an array of halo masses (units: $h^{-1}M_\odot$)
 - `Uk` is a 2D array of the Fourier halo profile at each `k` (first index) and `M` (second index) value
 - `amplitude` is an array of (mean) profile amplitudes, corresponding to each `M`
@@ -72,54 +75,54 @@
 - `variance` is an array containing the variance in the profile amplitude at each `M`
 - `mass_tracer` is a boolean telling the code if the profile corresponds to mass density
 - `discrete_tracer` is a boolean telling the code if it dealing with a discrete tracer or not
 
 The arrays `k` and `M` be identical to those in the subsequent `model.power_spectrum` call. If `amplitude=None` the Fourier profile is assumed to be normalised such that $U(k\to0, M)$ gives the total contribution of the halo to the field. Otherwise the profile is renormalised by the `amplitude`, and $U(k\to0, M)=1$ is assumed.
 
 Some examples best illustrate how to create your own halo profiles:
-```
+```python
 matter_profile = halo.profile.Fourier(k, M, Uk_matter, amplitude=M, normalisation=rho_matter, mass_tracer=True)
 ```
 would create a matter profile. Here `Uk_matter` would be the normalised Fourier transform of a matter profile (e.g., an NFW profile), the amplitude of each profile is exactly `M` (because the haloes are the mass), but the field normalisation is `rho_matter` (which can be accessed via `model.rhom`) because the field we are usually interested in is matter *overdensity*. We use `mass_tracer=True` to tell the code that the profile corresponds to mass. Note that in this case we would get identical behaviour if we fixed the profile amplitude as `amplitude=M/rho_matter` and the field normalisation as `normalisation=1.`.
-```
+```python
 galaxy_profile = halo.profile.Fourier(k, M, Uk_galaxy, amplitude=N_galaxy, normalisation=rho_galaxy, variance=var_galaxy, discrete_tracer=True)
 ```
 would create a galaxy profile. Here `Uk_galaxy` would be the normalised Fourier transform of a galaxy profile (e.g., an isothermal profile). The amplitude of the profile is the mean galaxy-occupation number at each `M`: `N_galaxy`. The field is normalised by the mean galaxy density: `rho_galaxy`. For a given assumption about the mean galaxy-occupation number and halo model this can be calculated using the `average` method of the `model` class:
-```
+```python
 rho_galaxy = hmod.average(M, sigmaM, N_galaxy)
 ```
 The variance in galaxy number at each `M` is `var_galaxy`. If one is assuming Poisson statistics then `variance=N_galaxy` is appropriate, but any value can be used in principle, including `variance=None`, which ignores the contribution of tracer-occupation variance to the power. We tell the code that `discrete_tracer=True` because in the discrete-tracer case it is essential to split the profile amplitude from the field normalisation if the discreteness of the tracer is to be accounted for properly.
 
 Halo profiles can also be specified in configuration (real) space, via a function of radius from the halo centre. This is slower than specifying the Fourier profiles since the conversion of the profile to Fourier space will need to be performed internally.
-```
+```python
 halo.profile.configuration(k, M, rv, c, differential_profile, amplitude=None, normalisation=1., variance=None, mass_tracer=False, discrete_tracer=False):
 ```
 the arguments are similar to those for Fourier-space profiles, except that
 - `differential_profile` is a the halo profile multiplied by $4\pi r^2$ with call signature `differential_profile(r, M, rv, c)`
 - `rv` is the halo virial radius (units: $h^{-1}\mathrm{Mpc}$)
 - `c` is the halo concentration
 
 the differential halo profile is the function defined such that integrating in radius between $0$ and $r_\mathrm{v}$ gives the total contribution of an individual halo to the field. It is usually the standard density profile multiplied $4\pi r^2$. This convention is used so as to avoid singularities that often occur in halo profiles at $r=0$. Again, some examples best illustrate how to use this
-```
+```python
 def differential_profile_matter(r, M, rv, c):
     # This is NFW (1./((r/rs)*(1.+r/rs)**2)) multiplied by 4pir^2 with constant factors ignored
     rs = rv/c
     return r/(1.+r/rs)**2.
 
 matter_profile = halo.profile.configuration(k, M, rv, c, differential_profile_matter, amplitude=M/rho_matter, mass_tracer=True)
 ```
 note that because we specify the amplitude here we do not need to worry about constant factors in the `differential_profile` definition, since the profile normalisation will be calculated self consistently. Note also that because we set `amplitude=M/rho_matter` (matter *overdensity*) we can omit the `normalisation` argument, which defaults to `1.`.
-```
+```python
 # Isothermal profile: 1/r^2, multiplied by 4pir^2 with constant factors ignored
 differential_profile_gal = lambda r, M, rv, c: 1. 
 
 galaxy_profile = halo.profile.configuration(k, M, rv, c, differential_profile_gal, amplitude=N_galaxy, normalisation=rho_galaxy, discrete_tracer=True)
 ```
 in the discrete tracer case it is important to split up `normalisation` and `amplitude` so that `amplitude` is something that can be interpreted as the mean of a discrete probability distribution. In this example we have also decided to ignore the contribution of the variance in the number of galaxies at fixed halo mass to the eventual power spectrum calculation.
 
 Note that the *covariance* in the mean profile amplitude between two different tracers is not currently supported. This can be important in halo-occupation models where galaxies are split into centrals and satellites and the presence of a satellite galaxy is conditional on the halo first containing a central galaxy. We hope to include this in future. Also any *spatial* variance or covariance in halo profiles at fixed mass is not currently supported; we have no plans to include this in future.
 
 ## Notebooks
 There are several `jupyter` notebooks in the `notebooks/` directory giving examples of how to use the code. The first one to try is `demo-basic.ipynb`, which gives an overview of the main features of `pyhalomodel`. As a bonus, we include notebooks that produce (almost) all of the plots from the review paper.
 
 ## Citation
-Please add a citation to [Asgari, Mead & Heymans (2023)](https://arxiv.org/) if you use this code.
+Please add a citation to [Asgari, Mead & Heymans (2023)](https://arxiv.org/abs/2303.08752) if you use this code.
```

### Comparing `pyhalomodel-1.0.1/pyhalomodel/camb_stuff.py` & `pyhalomodel-1.0.2/pyhalomodel/camb_stuff.py`

 * *Files identical despite different names*

### Comparing `pyhalomodel-1.0.1/pyhalomodel/constants.py` & `pyhalomodel-1.0.2/pyhalomodel/constants.py`

 * *Files identical despite different names*

### Comparing `pyhalomodel-1.0.1/pyhalomodel/cosmology.py` & `pyhalomodel-1.0.2/pyhalomodel/cosmology.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,177 +1,185 @@
 # Standard imports
 import numpy as np
-import scipy.integrate as integrate
+from scipy.integrate import quad
 
 # Project imports
 from . import constants as const
 from . import utility as util
 
 # Constants
-Dv0 = 18.*np.pi**2 # Delta_v = ~178, EdS halo virial overdensity
-dc0 = (3./20.)*(12.*np.pi)**(2./3.) # delta_c = ~1.686' EdS linear collapse threshold
+Dv0 = 18.*np.pi**2  # Delta_v = ~178, EdS halo virial overdensity
+# delta_c = ~1.686' EdS linear collapse threshold
+dc0 = (3./20.)*(12.*np.pi)**(2./3.)
 
 # Parameters
-xmin_Tk = 1e-5 # Scale at which to switch to Taylor expansion approximation in tophat Fourier functions
+xmin_Tk = 1e-5  # Scale at which to switch to Taylor expansion approximation in tophat Fourier functions
 
 ### Backgroud ###
 
+
 def redshift_from_scalefactor(a):
     return -1.+1./a
 
 
 def scalefactor_from_redshift(z):
     return 1./(1.+z)
 
 
-def comoving_matter_density(Om_m:float) -> float:
+def comoving_matter_density(Om_m: float) -> float:
     '''
     Comoving matter density, not a function of time [Msun/h / (Mpc/h)^3]
     args:
         Om_m: Cosmological matter density (at z=0)
     '''
     return const.rho_critical*Om_m
 
 ### ###
 
 ### Linear perturbations ###
 
-def _Tophat_k(x:np.ndarray) -> np.ndarray:
+
+def _Tophat_k(x: np.ndarray) -> np.ndarray:
     '''
     Fourier transform of a tophat function.
     args:
         x: Usually kR
     '''
     xmin = xmin_Tk
-    return np.where(np.abs(x)<xmin, 1.-x**2/10., (3./x**3)*(np.sin(x)-x*np.cos(x)))
+    return np.where(np.abs(x) < xmin, 1.-x**2/10., (3./x**3)*(np.sin(x)-x*np.cos(x)))
 
 
-def _dTophat_k(x:np.ndarray) -> np.ndarray:
+def _dTophat_k(x: np.ndarray) -> np.ndarray:
     '''
     Derivative of the tophat Fourier transform function
     args:
         x: Usually kR
     '''
     xmin = xmin_Tk
-    return np.where(np.abs(x)<xmin, -x/5.+x**3/70., (3./x**4)*((x**2-3.)*np.sin(x)+3.*x*np.cos(x)))
+    return np.where(np.abs(x) < xmin, -x/5.+x**3/70., (3./x**4)*((x**2-3.)*np.sin(x)+3.*x*np.cos(x)))
 
 
-def sigmaR(Rs:np.ndarray, Pk_lin:callable, kmin=1e-5, kmax=1e5, nk=int(1e5), integration_type='brute') -> np.ndarray:
+def sigmaR(Rs: np.ndarray, Pk_lin: callable, kmin=1e-5, kmax=1e5, nk=int(1e5), integration_type='brute') -> np.ndarray:
     '''
     Get the square-root of the variance, sigma(R), in the density field
     at comoving Lagrangian scale R
-    ''' 
+    '''
     if integration_type == 'brute':
         sigmaR_arr = _sigmaR_brute_log(Rs, Pk_lin, kmin=kmin, kmax=kmax, nk=nk)
     elif integration_type == 'quad':
         sigmaR_arr = _sigmaR_quad(Rs, Pk_lin)
     else:
         print('Not a recognised integration_type. Try one of the following:')
         print('brute for brute force integration')
         print('quad for the general purpose quad integration')
     return sigmaR_arr
 
 
-def _sigmaR_integrand(k:np.array, R:float, Pk:callable) -> np.ndarray:
+def _sigmaR_integrand(k: np.array, R: float, Pk: callable) -> np.ndarray:
     '''
     Integrand for calculating sigma(R)
     Note that k can be a float or an arraay here
     args:
         k: Fourier wavenumber (or array of these) [h/Mpc]
         R: Comoving Lagrangian radius [Mpc/h]
         Pk: Function of k to evaluate the linear power spectrum
     '''
     return Pk(k)*(k**2)*_Tophat_k(k*R)**2
 
 
-def _sigmaR_brute_log(R:float, Pk:callable, kmin=1e-5, kmax=1e5, nk=int(1e5)) -> float:
+def _sigmaR_brute_log(R: float, Pk: callable, kmin=1e-5, kmax=1e5, nk=int(1e5)) -> float:
     '''
     Brute force integration, this is only slightly faster than using a loop
     args:
         R: Comoving Lagrangian radius [Mpc/h]
         Pk: Function of k to evaluate the linear power spectrum
         kmin: Minimum wavenumber [h/Mpc]
         kmax: Maximum wavenumber [h/Mpc]
         nk: Number of bins in wavenumber
     '''
     k = util.logspace(kmin, kmax, nk)
     dlnk = np.log(k[1]/k[0])
+
     def sigmaR_vec(R, Pk):
-        sigmaR= np.sqrt(sum(dlnk*k*_sigmaR_integrand(k, R, Pk))/(2.*np.pi**2))
+        sigmaR = np.sqrt(sum(dlnk*k*_sigmaR_integrand(k, R, Pk))/(2.*np.pi**2))
         return sigmaR
     sigma_func = np.vectorize(sigmaR_vec, excluded=['Pk'])
     return sigma_func(R, Pk)
- 
 
-def _sigmaR_quad(R:float, Pk:callable) -> float:
+
+def _sigmaR_quad(R: float, Pk: callable) -> float:
     '''
     Quad integration
     args:
         R: Comoving Lagrangian radius [Mpc/h]
         Pk: Function of k to evaluate the linear power spectrum
     '''
-    def sigmaR_vec(R:float, Pk:callable):
+    def sigmaR_vec(R: float, Pk: callable):
         kmin, kmax = 0., np.inf
-        sigma_squared, _ = integrate.quad(lambda k: _sigmaR_integrand(k, R, Pk), kmin, kmax)
+        sigma_squared, _ = quad(lambda k: _sigmaR_integrand(k, R, Pk),
+                                kmin, kmax, epsrel=1e-4, epsabs=0.)
         sigma = np.sqrt(sigma_squared/(2.*np.pi**2))
         return sigma
     sigma_func = np.vectorize(sigmaR_vec, excluded=['Pk'])
     return sigma_func(R, Pk)
 
 
-def _dsigmaR_integrand(k:float, R:float, Pk) -> float:
+def _dsigmaR_integrand(k: float, R: float, Pk) -> float:
     return Pk(k)*(k**3)*_Tophat_k(k*R)*_dTophat_k(k*R)
 
 
-def dlnsigma2_dlnR(R:float, Pk:callable) -> float:
+def dlnsigma2_dlnR(R: float, Pk: callable) -> float:
     '''
     Calculates d(ln sigma^2)/d(ln R) by integration
     '''
     def dsigmaR_vec(R, Pk):
-        kmin, kmax = 0., np.inf # Evaluate the integral and convert to a nicer form
-        dsigma, _ = integrate.quad(lambda k: _dsigmaR_integrand(k, R, Pk), kmin, kmax)
+        kmin, kmax = 0., np.inf  # Evaluate the integral and convert to a nicer form
+        dsigma, _ = quad(lambda k: _dsigmaR_integrand(k, R, Pk),
+                         kmin, kmax, epsrel=1e-4, epsabs=0.)
         dsigma = R*dsigma/(np.pi*_sigmaR_quad(R, Pk))**2
         return dsigma
     dsigma_func = np.vectorize(dsigmaR_vec, excluded=['Pk'])
     return dsigma_func(R, Pk)
 
 ### ###
 
 ### Haloes ###
 
-def Lagrangian_radius(M:float, Om_m:float) -> float:
+
+def Lagrangian_radius(M: float, Om_m: float) -> float:
     '''
     Radius [Mpc/h] of a sphere containing mass M in a homogeneous universe
     args:
         M: Halo mass [Msun/h]
         Om_m: Cosmological matter density (at z=0)
     '''
     return np.cbrt(3.*M/(4.*np.pi*comoving_matter_density(Om_m)))
 
 
-def mass(R:float, Om_m:float) -> float:
+def mass(R: float, Om_m: float) -> float:
     '''
     Mass [Msun/h] contained within a sphere of radius 'R' [Mpc/h] in a homogeneous universe
     '''
     return (4./3.)*np.pi*R**3*comoving_matter_density(Om_m)
 
 ### ###
 
 ### Spherical collapse ###
 
-def dc_NakamuraSuto(Om_mz:float) -> float:
+
+def dc_NakamuraSuto(Om_mz: float) -> float:
     '''
     LCDM fitting function for the critical linear collapse density from Nakamura & Suto
     (1997; https://arxiv.org/abs/astro-ph/9612074)
     Cosmology dependence is very weak
     '''
     return dc0*(1.+0.012299*np.log10(Om_mz))
 
 
-def Dv_BryanNorman(Om_mz:float) -> float:
+def Dv_BryanNorman(Om_mz: float) -> float:
     '''
     LCDM fitting function for virial overdensity from Bryan & Norman
     (1998; https://arxiv.org/abs/astro-ph/9710107)
     Note that here Dv is defined relative to background matter density,
     whereas in paper it is relative to critical density
     For Omega_m = 0.3 LCDM Dv ~ 330.
     '''
```

### Comparing `pyhalomodel-1.0.1/pyhalomodel/darkquest.py` & `pyhalomodel-1.0.2/pyhalomodel/darkquest.py`

 * *Files identical despite different names*

### Comparing `pyhalomodel-1.0.1/pyhalomodel/pyhalomodel.py` & `pyhalomodel-1.0.2/pyhalomodel/pyhalomodel.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,48 +12,52 @@
 # TODO: Add checks for Dv, dc value compatability with mass functions (complicated with virial definition)
 # TODO: Add covariance between profile amplitudes (low priority; hard and annoying)
 # TODO: Raise errors if halo masses do not cover relevant portion of the mass function (usually a high-z problem)
 
 # Parameters
 dc_rel_tol = 1e-3    # Relative tolerance for checking 'closeness' of delta_c
 Dv_rel_tol = 1e-3    # Relative tolerance for checking 'closeness' of Delta_v
-Tinker_z_dep = False # Use redshift-dependent parameters for Tinker formula (only calibrated for M200)
-Tinker_PBS = False   # Get the bias from the peak-background split, rather than using the calibrated formula
+# Use redshift-dependent parameters for Tinker formula (only calibrated for M200)
+Tinker_z_dep = False
+# Get the bias from the peak-background split, rather than using the calibrated formula
+Tinker_PBS = False
 
 # Halo-model integration scheme for integration in nu
 # NOTE: Cannot use Romberg because integration is done in nu, not M, and this will generally be uneven
 # NOTE: In HMx I use trapezoid because of fast osciallations, maybe should also use that here?
 halo_integration = integrate.trapezoid
-#halo_integration = integrate.simps
+# halo_integration = integrate.simps
 
 # W(k) integration scheme integration in r
 # TODO: Implement fast schemes utilising sin(kR)/kR kernel
-#win_integration = integrate.trapezoid
-#win_integration = integrate.simps
-#win_integration = integrate.romb # Needs 2^m+1 (integer m) evenly-spaced samples in R
+# win_integration = integrate.trapezoid
+# win_integration = integrate.simps
+# win_integration = integrate.romb # Needs 2^m+1 (integer m) evenly-spaced samples in R
 win_integration = integrate.quad
-#win_integration = integrate.quadrature
-#win_integration = integrate.romberg
-nr_win_integration = 1+2**8 # Number of points in r (sample methods)
-eps_win_integration = 1e-3 # Integration accuracy (continuous methods)
+# win_integration = integrate.quadrature
+# win_integration = integrate.romberg
+nr_win_integration = 1+2**8  # Number of points in r (sample methods)
+eps_win_integration = 1e-3  # Integration accuracy (continuous methods)
 
 # Mass function
-eps_deriv_mf = 1e-3 # R -> dR for numerical sigma derivative
+eps_deriv_mf = 1e-3  # R -> dR for numerical sigma derivative
 
 # beta_NL
 do_I11 = True     # Compute and add low M1 and M2 portion of the integral
-do_I12_I21 = True # Compute and add low M1 or low M2 portion of the integral
+do_I12_I21 = True  # Compute and add low M1 or low M2 portion of the integral
 
 ### Class definition ###
 
+
 class model():
     '''
     Class for halo model
     '''
-    def __init__(self, z:float, Om_m:float, name='Tinker et al. (2010)', Dv=200., dc=1.686, verbose=False):
+
+    def __init__(self, z: float, Om_m: float, name='Tinker et al. (2010)', Dv=200., dc=1.686, verbose=False):
         '''
         Class initialisation; configures mass function and halo bias.
         Args:
             z: Redshift
             Om_m: Cosmological matter density
             name: Name of halo model, one of:
                 'Press & Schecter (1974)'
@@ -74,241 +78,265 @@
         self.Dv = Dv
         self.rhom = cosmology.comoving_matter_density(Om_m)
 
         # Write to screen
         if verbose:
             print('Initialising halo model')
             print('Halo model:', self.name)
-            print('Redshift: %1.3f'%(self.z))
-            print('Scale factor: %1.3f'%(self.a))
-            print('Omega_m(z=0): %1.3f'%(self.Om_m))
-            print('delta_c: %1.4f'%(self.dc))
-            print('Delta_v: %4.1f'%(self.Dv))
+            print('Redshift: %1.3f' % (self.z))
+            print('Scale factor: %1.3f' % (self.a))
+            print('Omega_m(z=0): %1.3f' % (self.Om_m))
+            print('delta_c: %1.4f' % (self.dc))
+            print('Delta_v: %4.1f' % (self.Dv))
 
         # Initialise mass functions
         if name == 'Press & Schecter (1974)':
             # No initialisation required for Press & Schecter (1974)
             pass
         elif name in ['Sheth & Tormen (1999)', 'Sheth, Mo & Tormen (2001)']:
             # Sheth & Tormen (1999; https://arxiv.org/abs/astro-ph/9901122)
             # Virial halo definition
             from scipy.special import gamma as Gamma
             p = 0.3
             q = 0.707
-            self.p_ST = p; self.q_ST = q
-            self.A_ST = np.sqrt(2.*q)/(np.sqrt(np.pi)+Gamma(0.5-p)/2**p) # A ~ 0.2161
+            self.p_ST = p
+            self.q_ST = q
+            self.A_ST = np.sqrt(2.*q)/(np.sqrt(np.pi) +
+                                       Gamma(0.5-p)/2**p)  # A ~ 0.2161
             if verbose:
-                print('p: %1.3f; q: %1.3f; A: %1.4f'%(self.p_ST, self.q_ST, self.A_ST))
+                print('p: %1.3f; q: %1.3f; A: %1.4f' %
+                      (self.p_ST, self.q_ST, self.A_ST))
             if name in ['Sheth, Mo & Tormen (2001)']:
                 self.a_SMT = 0.707
                 self.b_SMT = 0.5
                 self.c_SMT = 0.6
                 if verbose:
-                    print('a: %1.3f; b: %1.3f; c: %1.3f'%(self.a_SMT, self.b_SMT, self.c_SMT))
+                    print('a: %1.3f; b: %1.3f; c: %1.3f' %
+                          (self.a_SMT, self.b_SMT, self.c_SMT))
         elif name in ['Despali et al. (2016)']:
             # Despali et al. (2016; https://arxiv.org/abs/1507.05627)
             # Note that this mass function is not correctly normalised
             # Virial halo definition
             self.p_ST = 0.2536
             self.q_ST = 0.7689
-            self.A_ST = 0.3295*np.sqrt(2.*self.q_ST/np.pi) # Careful with factors of sqrt(2q/pi) in normalisation
+            # Careful with factors of sqrt(2q/pi) in normalisation
+            self.A_ST = 0.3295*np.sqrt(2.*self.q_ST/np.pi)
             if verbose:
-                print('p: %1.3f; q: %1.3f; A: %1.4f'%(self.p_ST, self.q_ST, self.A_ST))
+                print('p: %1.3f; q: %1.3f; A: %1.4f' %
+                      (self.p_ST, self.q_ST, self.A_ST))
         elif name in ['Tinker et al. (2010)']:
             # Tinker et al. (2010; https://arxiv.org/abs/1001.3162)
             # A range of Delta_v are available, interpolate/extrapolate between them
             from math import isclose
-            Dv_array = np.array([200., 300., 400., 600., 800., 1200., 1600, 2400., 3200.])
+            Dv_array = np.array(
+                [200., 300., 400., 600., 800., 1200., 1600, 2400., 3200.])
             # Check Delta_v and delta_c values
             # if (Dv < Dv_array[0]) or (Dv > Dv_array[-1]):
             #     print('Dv:', Dv)
             #     warnings.warn('Dv is outside supported range for Tinker et al. (2010)', RuntimeWarning)
             # if not isclose(dc, 1.686, rel_tol=dc_rel_tol):
             #     print('dc:', dc)
             #     warnings.warn('dc = 1.686 assumed in Tinker et al. (2010)', RuntimeWarning)
             # Mass function from Table 4
             logDv = np.log(self.Dv)
             logDv_array = np.log(Dv_array)
-            alpha_array = np.array([0.368, 0.363, 0.385, 0.389, 0.393, 0.365, 0.379, 0.355, 0.327])
-            beta_array = np.array([0.589, 0.585, 0.544, 0.543, 0.564, 0.623, 0.637, 0.673, 0.702])
-            gamma_array = np.array([0.864, 0.922, 0.987, 1.09, 1.20, 1.34, 1.50, 1.68, 1.81])
-            phi_array = np.array([-0.729, -0.789, -0.910, -1.05, -1.20, -1.26, -1.45, -1.50, -1.49])
-            eta_array = np.array([-0.243, -0.261, -0.261, -0.273, -0.278, -0.301, -0.301, -0.319, -0.336])
-            alpha = interp(logDv_array, alpha_array, fill_value='extrapolate')(logDv) # Linear interpolation/extrapolation
-            beta = interp(logDv_array, beta_array, fill_value='extrapolate')(logDv)
-            gamma = interp(logDv_array, gamma_array, fill_value='extrapolate')(logDv)
-            phi = interp(logDv_array, phi_array, fill_value='extrapolate')(logDv)
-            eta = interp(logDv_array, eta_array, fill_value='extrapolate')(logDv)
-            if Tinker_z_dep: # Redshift dependence from equations (9-12); only calibrated for M200
+            alpha_array = np.array(
+                [0.368, 0.363, 0.385, 0.389, 0.393, 0.365, 0.379, 0.355, 0.327])
+            beta_array = np.array(
+                [0.589, 0.585, 0.544, 0.543, 0.564, 0.623, 0.637, 0.673, 0.702])
+            gamma_array = np.array(
+                [0.864, 0.922, 0.987, 1.09, 1.20, 1.34, 1.50, 1.68, 1.81])
+            phi_array = np.array(
+                [-0.729, -0.789, -0.910, -1.05, -1.20, -1.26, -1.45, -1.50, -1.49])
+            eta_array = np.array(
+                [-0.243, -0.261, -0.261, -0.273, -0.278, -0.301, -0.301, -0.319, -0.336])
+            alpha = interp(logDv_array, alpha_array, fill_value='extrapolate')(
+                logDv)  # Linear interpolation/extrapolation
+            beta = interp(logDv_array, beta_array,
+                          fill_value='extrapolate')(logDv)
+            gamma = interp(logDv_array, gamma_array,
+                           fill_value='extrapolate')(logDv)
+            phi = interp(logDv_array, phi_array,
+                         fill_value='extrapolate')(logDv)
+            eta = interp(logDv_array, eta_array,
+                         fill_value='extrapolate')(logDv)
+            # Redshift dependence from equations (9-12); only calibrated for M200
+            if Tinker_z_dep:
                 beta *= (1.+z)**0.20
                 gamma *= (1.+z)**-0.01
                 phi *= (1.+z)**-0.08
                 eta *= (1.+z)**0.27
             self.alpha_Tinker = alpha
             self.beta_Tinker = beta
             self.gamma_Tinker = gamma
             self.phi_Tinker = phi
             self.eta_Tinker = eta
             if verbose:
-                print('alpha: %1.3f; beta: %1.3f; gamma: %1.3f; phi: %1.3f; eta: %1.3f'%(alpha, beta, gamma, phi, eta))
+                print('alpha: %1.3f; beta: %1.3f; gamma: %1.3f; phi: %1.3f; eta: %1.3f' % (
+                    alpha, beta, gamma, phi, eta))
             # Calibrated halo bias parameters (not from peak-background split) from Table 2
             y = np.log10(self.Dv)
             exp = np.exp(-(4./y)**4)
             self.A_Tinker = 1.+0.24*y*exp
             self.a_Tinker = 0.44*y-0.88
             self.B_Tinker = 0.183
             self.b_Tinker = 1.5
             self.C_Tinker = 0.019+0.107*y+0.19*exp
             self.c_Tinker = 2.4
             if verbose:
-                print('A: %1.3f; a: %1.3f'%(self.A_Tinker, self.a_Tinker))
-                print('B: %1.3f; b: %1.3f'%(self.B_Tinker, self.b_Tinker))
-                print('C: %1.3f; c: %1.3f'%(self.C_Tinker, self.c_Tinker))
+                print('A: %1.3f; a: %1.3f' % (self.A_Tinker, self.a_Tinker))
+                print('B: %1.3f; b: %1.3f' % (self.B_Tinker, self.b_Tinker))
+                print('C: %1.3f; c: %1.3f' % (self.C_Tinker, self.c_Tinker))
         else:
             raise ValueError('Halo model not recognised')
         if verbose:
             print()
 
-
     def __str__(self):
         print('Halo model:', self.name)
-        print('Scale factor: %1.3f'%(self.a))
-        print('Redshift: %1.3f'%(self.z))
-        print('Omega_m(z=0): %1.3f'%(self.Om_m))
-        print('delta_c: %1.4f'%(self.dc))
-        print('Delta_v: %4.1f'%(self.Dv))
+        print('Scale factor: %1.3f' % (self.a))
+        print('Redshift: %1.3f' % (self.z))
+        print('Omega_m(z=0): %1.3f' % (self.Om_m))
+        print('delta_c: %1.4f' % (self.dc))
+        print('Delta_v: %4.1f' % (self.Dv))
         if self.name != 'Press & Schecter (1974)':
             print('Parameters:')
         if self.name in ['Sheth & Tormen (1999)', 'Sheth, Mo & Tormen (2001)', 'Despali et al. (2016)']:
-            print('p: %1.3f; q: %1.3f; A: %1.4f'%(self.p_ST, self.q_ST, self.A_ST))
+            print('p: %1.3f; q: %1.3f; A: %1.4f' %
+                  (self.p_ST, self.q_ST, self.A_ST))
             if self.name in ['Sheth, Mo & Tormen (2001)']:
-                print('a: %1.3f; b: %1.3f; c: %1.3f'%(self.a_SMT, self.b_SMT, self.c_SMT))
+                print('a: %1.3f; b: %1.3f; c: %1.3f' %
+                      (self.a_SMT, self.b_SMT, self.c_SMT))
         elif self.name in ['Tinker et al. (2010)']:
             print('alpha: %1.3f; beta: %1.3f; gamma: %1.3f; phi: %1.3f; eta: %1.3f'
-                %(self.alpha_Tinker, self.beta_Tinker, self.gamma_Tinker, self.phi_Tinker, self.eta_Tinker))
-            print('A: %1.3f; a: %1.3f'%(self.A_Tinker, self.a_Tinker))
-            print('B: %1.3f; b: %1.3f'%(self.B_Tinker, self.b_Tinker))
-            print('C: %1.3f; c: %1.3f'%(self.C_Tinker, self.c_Tinker))
+                  % (self.alpha_Tinker, self.beta_Tinker, self.gamma_Tinker, self.phi_Tinker, self.eta_Tinker))
+            print('A: %1.3f; a: %1.3f' % (self.A_Tinker, self.a_Tinker))
+            print('B: %1.3f; b: %1.3f' % (self.B_Tinker, self.b_Tinker))
+            print('C: %1.3f; c: %1.3f' % (self.C_Tinker, self.c_Tinker))
         return ''
 
-
-    def _mass_function_nu(self, nu:np.ndarray) -> np.ndarray:
+    def _mass_function_nu(self, nu: np.ndarray) -> np.ndarray:
         '''
         Halo mass function g(nu) with nu=delta_c/sigma(M)
         Integral of g(nu) over all nu is unity
         '''
         if self.name == 'Press & Schecter (1974)':
             return np.sqrt(2./np.pi)*np.exp(-(nu**2)/2.)
         elif self.name in ['Sheth & Tormen (1999)', 'Sheth, Mo & Tormen (2001)', 'Despali et al. (2016)']:
-            A = self.A_ST; q = self.q_ST; p = self.p_ST
+            A = self.A_ST
+            q = self.q_ST
+            p = self.p_ST
             return A*(1.+((q*nu**2)**(-p)))*np.exp(-q*nu**2/2.)
         elif self.name == 'Tinker et al. (2010)':
             alpha = self.alpha_Tinker
             beta = self.beta_Tinker
             gamma = self.gamma_Tinker
             phi = self.phi_Tinker
             eta = self.eta_Tinker
             f1 = 1.+(beta*nu)**(-2.*phi)
             f2 = nu**(2.*eta)
             f3 = np.exp(-gamma*nu**2/2.)
             return alpha*f1*f2*f3
         else:
             raise ValueError('Halo model not recognised in mass_function')
 
-
-    def _linear_bias_nu(self, nu:np.ndarray) -> np.ndarray:
+    def _linear_bias_nu(self, nu: np.ndarray) -> np.ndarray:
         '''
         Halo linear bias b(nu) with nu=delta_c/sigma(M)
         Integral of b(nu)*g(nu) over all nu is unity
         '''
         if self.name == 'Press & Schecter (1974)':
             return 1.+(nu**2-1.)/self.dc
         elif self.name in ['Sheth & Tormen (1999)', 'Despali et al. (2016)']:
-            p = self.p_ST; q = self.q_ST
+            p = self.p_ST
+            q = self.q_ST
             return 1.+(q*(nu**2)-1.+2.*p/(1.+(q*nu**2)**p))/self.dc
         elif self.name == 'Sheth, Mo & Tormen (2001)':
-            a = self.a_SMT; b = self.b_SMT; c = self.c_SMT
+            a = self.a_SMT
+            b = self.b_SMT
+            c = self.c_SMT
             anu2 = a*nu**2
             f1 = np.sqrt(a)*anu2
             f2 = np.sqrt(a)*b*anu2**(1.-c)
             f3 = anu2**c
             f4 = anu2**c+b*(1.-c)*(1.-c/2.)
             return 1.+(f1+f2-f3/f4)/(self.dc*np.sqrt(a))
         elif self.name == 'Tinker et al. (2010)':
             if Tinker_PBS:
-                beta = self.beta_Tinker; gamma = self.gamma_Tinker
-                phi = self.phi_Tinker; eta = self.eta_Tinker
+                beta = self.beta_Tinker
+                gamma = self.gamma_Tinker
+                phi = self.phi_Tinker
+                eta = self.eta_Tinker
                 f1 = (gamma*nu**2-(1.+2.*eta))/self.dc
                 f2 = (2.*phi/self.dc)/(1.+(beta*nu)**(2.*phi))
                 return 1.+f1+f2
             else:
-                A = self.A_Tinker; a = self.a_Tinker
-                B = self.B_Tinker; b = self.b_Tinker
-                C = self.C_Tinker; c = self.c_Tinker
+                A = self.A_Tinker
+                a = self.a_Tinker
+                B = self.B_Tinker
+                b = self.b_Tinker
+                C = self.C_Tinker
+                c = self.c_Tinker
                 fA = A*nu**a/(nu**a+self.dc**a)
                 fB = B*nu**b
                 fC = C*nu**c
                 return 1.-fA+fB+fC
         else:
             raise ValueError('Halo model not recognised in linear_bias')
 
-
-    def mass_function(self, M:np.ndarray, sigmaM:np.ndarray) -> np.ndarray:
+    def mass_function(self, M: np.ndarray, sigmaM: np.ndarray) -> np.ndarray:
         '''
         Calculates the halo mass function as a function of halo mass
         This is the comoving number-density of haloes per halo mass
         Sometimes referred to as n(M) or dn/dM in the literature
         Args:
             M: Halo masses [Msun/h]
             sigmaM: Standard deviation in overdensity on mass scale M
         '''
         F = self.multiplicity_function(M, sigmaM)
         return F*self.rhom/M**2
 
-
-    def multiplicity_function(self, M:np.ndarray, sigmaM:np.ndarray) -> np.ndarray:
+    def multiplicity_function(self, M: np.ndarray, sigmaM: np.ndarray) -> np.ndarray:
         '''
         Calculates M^2 n(M) / rhobar, the so-called halo multiplicity function
         Note that this is dimensionless
         Args:
             M: Halo masses [Msun/h]
             sigmaM(M): Standard deviation in overdensity on mass scale M
         '''
         nu = self._peak_height(M, sigmaM)
         R = self.Lagrangian_radius(M)
         deriv = np.zeros(len(R))
         logR, logsigmaM = np.log(R), np.log(sigmaM)
-        for iR, _logR in enumerate(logR): # TODO: Avoid loop with a vectorised function here
+        # TODO: Avoid loop with a vectorised function here
+        for iR, _logR in enumerate(logR):
             deriv[iR] = 2.*util.derivative_from_samples(_logR, logR, logsigmaM)
-        #dlnsigma2_dlnR = 2.*util.derivative_from_samples(np.log(R), np.log(R), np.log(sigmas)) # Does not work
+        # dlnsigma2_dlnR = 2.*util.derivative_from_samples(np.log(R), np.log(R), np.log(sigmas)) # Does not work
         dnu_dlnm = -(nu/6.)*deriv
         return self._mass_function_nu(nu)*dnu_dlnm
 
-
-    def linear_bias(self, M:np.ndarray, sigmaM:np.ndarray) -> np.ndarray:
+    def linear_bias(self, M: np.ndarray, sigmaM: np.ndarray) -> np.ndarray:
         '''
         Calculates the linear halo bias as a function of halo mass
         Args:
             M: Halo masses [Msun/h]
             sigmaM(M): Standard deviation in overdensity on mass scale M
         '''
         nu = self._peak_height(M, sigmaM)
         return self._linear_bias_nu(nu)
 
-
-    def Lagrangian_radius(self, M:np.ndarray) -> np.ndarray:
+    def Lagrangian_radius(self, M: np.ndarray) -> np.ndarray:
         '''
         Radius [Mpc/h] of a sphere containing mass M in a homogeneous universe
         Args:
             M: Halo masses [Msun/h]
         '''
         return cosmology.Lagrangian_radius(M, self.Om_m)
 
-
-    def average(self, M:np.ndarray, sigmaM:np.ndarray, func:np.ndarray) -> np.ndarray:
+    def average(self, M: np.ndarray, sigmaM: np.ndarray, func: np.ndarray) -> np.ndarray:
         '''
         Calculate the mean of some f(M) over halo mass <f>: int f(M)n(M)dM where n(M) = dn/dM in some notations.
         Note that the units of n(M) are [(Msun/h)^{-1} (Mpc/h)^{-3}] so the units of the result are [f (Mpc/h)^{-3}].
         This corresponds to the mean of f(M) over haloes, weighted by their mass.
         Common use cases:
             <M> = rho: The mean matter density in the universe
             <M/rho> = 1: over all halo mass (equivalent to int g(nu)dnu = 1)
@@ -318,22 +346,24 @@
             <N(M)> = rhog: with N the number of galaxies in each halo of mass M; gives mean number density of galaxies, rhog
             <b(M)N(M)>/<N(M)> = bg: with N the number of galaxies in each halo of mass M; gives mean bias of galaxies, bg
         Args:
             M: Halo masses [Msun/h]
             sigmaM(M): Standard deviation in overdensity on mass scale M
             func(M): Function values, evaluated at M, of which to calculate mean
         '''
-        if not util.is_array_monotonic(M): raise ValueError('Halo mass array must be increasing monotonically')
-        nu = self._peak_height(M, sigmaM) # TODO: Raise error if nu[0] isn't << 1? or nu[-1] isn't >> 1?
+        if not util.is_array_monotonic(M):
+            raise ValueError(
+                'Halo mass array must be increasing monotonically')
+        # TODO: Raise error if nu[0] isn't << 1? or nu[-1] isn't >> 1?
+        nu = self._peak_height(M, sigmaM)
         integrand = (func/M)*self._mass_function_nu(nu)
         return halo_integration(integrand, nu)*self.rhom
 
-
-    def power_spectrum(self, k:np.ndarray, Pk_lin:np.ndarray, M:np.ndarray, sigmaM:np.ndarray, profiles:dict, 
-                       beta=None, simple_twohalo=False, subtract_shotnoise=True, correct_discrete=True, 
+    def power_spectrum(self, k: np.ndarray, Pk_lin: np.ndarray, M: np.ndarray, sigmaM: np.ndarray, profiles: dict,
+                       beta=None, simple_twohalo=False, subtract_shotnoise=True, correct_discrete=True,
                        k_trunc=None, verbose=False) -> tuple:
         '''
         Computes power spectra given that halo model. Returns the two-halo, one-halo and sum terms.
         Args:
             k: Comoving wavenumbers [h/Mpc]
             Pk_lin(k): Linear power at each wavenumber [(Mpc/h)^3]
             M: Halo masses [Msun/h]
@@ -343,160 +373,190 @@
             simple_twohalo: Should the scale-dependence of the two-halo term be ignored?
             subtract_shotnoise: Should shot noise be subtracted from discrete spectra?
             correct_discrete: Properly treat discrete tracers with <N(N-1)> rather than <N^2>?
             k_trunc: None or wavenumber [h/Mpc] at which to truncate the one-halo term at large scales
             verbose: verbosity
         '''
         from time import time
-        if verbose: t_start = time() # Initial time
+        if verbose:
+            t_start = time()  # Initial time
 
         # Checks
-        if simple_twohalo and (beta is not None): raise ValueError('A simple two-halo term is not compatible with non-linear halo bias')
-        if not util.is_array_monotonic(M): raise ValueError('Halo mass array must be increasing monotonically')
-        if not isinstance(profiles, dict): raise TypeError('profiles must be a dictionary')
+        if simple_twohalo and (beta is not None):
+            raise ValueError(
+                'A simple two-halo term is not compatible with non-linear halo bias')
+        if not util.is_array_monotonic(M):
+            raise ValueError(
+                'Halo mass array must be increasing monotonically')
+        if not isinstance(profiles, dict):
+            raise TypeError('profiles must be a dictionary')
         for profile in profiles.values():
-            if (k != profile.k).all(): raise ValueError('k arrays must all be identical to those in profiles')
-            if (M != profile.M).all(): raise ValueError('Mass arrays must be identical to those in profiles')
+            if (k != profile.k).all():
+                raise ValueError(
+                    'k arrays must all be identical to those in profiles')
+            if (M != profile.M).all():
+                raise ValueError(
+                    'Mass arrays must be identical to those in profiles')
 
         # Create arrays of nu values that correspond to the halo mass
-        nu = self._peak_height(M, sigmaM) # TODO: Raise error if nu[0] isn't << 1? or nu[-1] isn't >> 1?
+        # TODO: Raise error if nu[0] isn't << 1? or nu[-1] isn't >> 1?
+        nu = self._peak_height(M, sigmaM)
 
         # Useful information
         if verbose:
             print('Redshift:', self.z)
-            print('Halo mass range [log10(Msun/h)]:', np.log10(M[0]), np.log10(M[-1]))
+            print('Halo mass range [log10(Msun/h)]:',
+                  np.log10(M[0]), np.log10(M[-1]))
             print('Peak height range:', nu[0], nu[-1])
             print('Number of integration points:', len(nu))
 
         # Calculate the missing halo-bias from the low-mass part of the integral
-        A = 1.-integrate.quad(lambda nu: self._mass_function_nu(nu)*self._linear_bias_nu(nu), nu[0], np.inf)[0]
-        if verbose: print('Missing halo-bias-mass from the low-mass end of the two-halo integrand:', A)
-        if A < 0.:  warnings.warn('Warning: Mass function/bias correction is negative!', RuntimeWarning)
+        A = 1.-integrate.quad(lambda nu: self._mass_function_nu(nu)
+                              * self._linear_bias_nu(nu), nu[0], np.inf)[0]
+        if verbose:
+            print(
+                'Missing halo-bias-mass from the low-mass end of the two-halo integrand:', A)
+        if A < 0.:
+            warnings.warn(
+                'Warning: Mass function/bias correction is negative!', RuntimeWarning)
 
         # Shot noise calculations
         Pk_SN = {}
         for name, profile in profiles.items():
-            Pk_SN[name] = self._Pk_1h(M, nu, profile.amplitude/profile.normalisation**2) if profile.discrete_tracer else 0.
+            Pk_SN[name] = self._Pk_1h(M, nu, profile.amplitude/profile.normalisation **
+                                      2) if profile.discrete_tracer else 0.
 
         # Fill arrays for results
         Pk_2h_dict, Pk_1h_dict, Pk_hm_dict = {}, {}, {}
         Pk_2h, Pk_1h = np.zeros_like(k), np.zeros_like(k)
 
         # Loop over halo profiles/fields
-        for iu, (name_u, profile_u) in enumerate(profiles.items()): 
+        for iu, (name_u, profile_u) in enumerate(profiles.items()):
             for iv, (name_v, profile_v) in enumerate(profiles.items()):
 
                 # Naming conventions
-                power_name = name_u+'-'+name_v # Name for this two-point combination
-                reverse_name = name_v+'-'+name_u # Reverse name to avoid double computations for cross terms
+                power_name = name_u+'-'+name_v  # Name for this two-point combination
+                # Reverse name to avoid double computations for cross terms
+                reverse_name = name_v+'-'+name_u
 
                 # Two-halo term if scale-dependence ignored
                 if simple_twohalo:
-                    Pk_2h = self._Pk_2h(Pk_lin, M, nu, 
-                                        profile_u.amplitude/profile_u.normalisation, 
+                    Pk_2h = self._Pk_2h(Pk_lin, M, nu,
+                                        profile_u.amplitude/profile_u.normalisation,
                                         profile_v.amplitude/profile_v.normalisation,
                                         profile_u.mass_tracer, profile_v.mass_tracer, A)
 
                 # Power calculation for this tracer pair
-                if verbose: print('Calculating power:', power_name)
+                if verbose:
+                    print('Calculating power:', power_name)
                 if iu <= iv:
-                    for ik, _Pk_lin in enumerate(Pk_lin): # Loop over wavenumbers
+                    # Loop over wavenumbers
+                    for ik, _Pk_lin in enumerate(Pk_lin):
 
                         # Two-halo term, treat non-linear halo bias carefully
                         if not simple_twohalo:
-                            if beta is None: 
+                            if beta is None:
                                 Pk_2h[ik] = self._Pk_2h(_Pk_lin, M, nu, profile_u.Wk[ik, :], profile_v.Wk[ik, :],
                                                         profile_u.mass_tracer, profile_v.mass_tracer, A)
                             else:
                                 Pk_2h[ik] = self._Pk_2h(_Pk_lin, M, nu, profile_u.Wk[ik, :], profile_v.Wk[ik, :],
                                                         profile_u.mass_tracer, profile_v.mass_tracer, A, beta=beta[ik, :, :])
 
                         # One-halo term, treat discrete auto case carefully
-                        if name_u == name_v: 
-                            if correct_discrete and profile_u.discrete_tracer: # Treat discrete tracers
-                                Wfac = profile_u.amplitude*(profile_u.amplitude-1.) # <N(N-1)> for discrete tracers
+                        if name_u == name_v:
+                            if correct_discrete and profile_u.discrete_tracer:  # Treat discrete tracers
+                                # <N(N-1)> for discrete tracers
+                                Wfac = profile_u.amplitude * \
+                                    (profile_u.amplitude-1.)
                             else:
-                                Wfac = profile_u.amplitude**2 # <N^2> for others
-                            if profile_u.variance is not None: Wfac += profile_u.variance # Add variance
-                            Wprod = Wfac*(profile_u.Uk[ik, :]/profile_u.normalisation)**2 # Multiply by factors of normalisataion and profile
+                                Wfac = profile_u.amplitude**2  # <N^2> for others
+                            if profile_u.variance is not None:
+                                Wfac += profile_u.variance  # Add variance
+                            # Multiply by factors of normalisataion and profile
+                            Wprod = Wfac * \
+                                (profile_u.Uk[ik, :] /
+                                 profile_u.normalisation)**2
                         else:
                             Wprod = profile_u.Wk[ik, :]*profile_v.Wk[ik, :]
                         Pk_1h[ik] = self._Pk_1h(M, nu, Wprod)
 
                     # Shot noise corrections
                     # If '(not discrete) and shot' or 'discrete and (not shot)' no need to do anything as shot noise already correct
                     if (name_u == name_v) and profile_u.discrete_tracer:
                         if correct_discrete and (not subtract_shotnoise):
-                            Pk_1h += Pk_SN[name_u] # Need to add shot noise
+                            Pk_1h += Pk_SN[name_u]  # Need to add shot noise
                         elif (not correct_discrete) and subtract_shotnoise:
-                            warnings.warn('Warning: Subtracting shot noise while not treating discreteness properly is bad', RuntimeWarning)
-                            Pk_1h[:] -= Pk_SN[name_u] # Need to subtract shot noise
+                            warnings.warn(
+                                'Warning: Subtracting shot noise while not treating discreteness properly is bad', RuntimeWarning)
+                            # Need to subtract shot noise
+                            Pk_1h[:] -= Pk_SN[name_u]
 
                     # Suppress one-halo term
-                    if k_trunc is not None: Pk_1h *= 1.-np.exp(-(k/k_trunc)**2)
+                    if k_trunc is not None:
+                        Pk_1h *= 1.-np.exp(-(k/k_trunc)**2)
 
                     # Finish
-                    Pk_2h_dict[power_name], Pk_1h_dict[power_name] = Pk_2h.copy(), Pk_1h.copy()
-                    Pk_hm_dict[power_name] = Pk_2h_dict[power_name]+Pk_1h_dict[power_name]
+                    Pk_2h_dict[power_name], Pk_1h_dict[power_name] = Pk_2h.copy(
+                    ), Pk_1h.copy()
+                    Pk_hm_dict[power_name] = Pk_2h_dict[power_name] + \
+                        Pk_1h_dict[power_name]
 
                 else:
                     # No need to do these calculations twice
                     Pk_2h_dict[power_name] = Pk_2h_dict[reverse_name]
                     Pk_1h_dict[power_name] = Pk_1h_dict[reverse_name]
                     Pk_hm_dict[power_name] = Pk_hm_dict[reverse_name]
 
         # Finish
-        if verbose: 
+        if verbose:
             t_end = time()
             print('Halomodel calculation time [s]:', t_end-t_start, '\n')
         return Pk_2h_dict, Pk_1h_dict, Pk_hm_dict
 
-
-    def _Pk_2h(self, Pk_lin:float, M:np.ndarray, nu:np.ndarray, Wu:float, Wv:float,
-               mass_u:bool, mass_v:bool, A:float, beta=None) -> float:
+    def _Pk_2h(self, Pk_lin: float, M: np.ndarray, nu: np.ndarray, Wu: float, Wv: float,
+               mass_u: bool, mass_v: bool, A: float, beta=None) -> float:
         '''
         Two-halo term at a specific wavenumber
         '''
-        I_NL = 0. if beta is None else self._I_beta(beta, M, nu, Wu, Wv, mass_u, mass_v, A)
+        I_NL = 0. if beta is None else self._I_beta(
+            beta, M, nu, Wu, Wv, mass_u, mass_v, A)
         Iu = self._I_2h(M, nu, Wu, mass_u, A)
         Iv = self._I_2h(M, nu, Wv, mass_v, A)
         return (Iu*Iv+I_NL)*Pk_lin
 
-
-    def _Pk_1h(self, M:np.ndarray, nu:np.ndarray, WuWv:float) -> float:
+    def _Pk_1h(self, M: np.ndarray, nu: np.ndarray, WuWv: float) -> float:
         '''
         One-halo term at a specific wavenumber
         '''
         integrand = WuWv*self._mass_function_nu(nu)/M
         P_1h = halo_integration(integrand, nu)
         P_1h = P_1h*self.rhom
         return P_1h
 
-
-    def _I_2h(self, M:np.ndarray, nu:np.ndarray, W:float, mass:bool, A:float) -> float:
+    def _I_2h(self, M: np.ndarray, nu: np.ndarray, W: float, mass: bool, A: float) -> float:
         '''
         Evaluate the integral that appears in the two-halo term
         '''
         integrand = W*self._linear_bias_nu(nu)*self._mass_function_nu(nu)/M
         I_2h = halo_integration(integrand, nu)
-        if mass: I_2h += A*W[0]/M[0]
+        if mass:
+            I_2h += A*W[0]/M[0]
         I_2h = I_2h*self.rhom
         return I_2h
 
-
-    def _I_beta(self, beta:np.ndarray, M:np.ndarray, nu:np.ndarray, Wu:float, Wv:float, 
-                massu:bool, massv:bool, A:float) -> float:
+    def _I_beta(self, beta: np.ndarray, M: np.ndarray, nu: np.ndarray, Wu: float, Wv: float,
+                massu: bool, massv: bool, A: float) -> float:
         '''
         Evaluates the beta_NL double integral
         '''
         from numpy import trapz
         integrand = np.zeros((len(nu), len(nu)))
         W1W2 = np.outer(Wu, Wv)
         g1g2 = np.outer(self._mass_function_nu(nu), self._mass_function_nu(nu))
-        b1b2 =  np.outer(self._linear_bias_nu(nu), self._linear_bias_nu(nu))
+        b1b2 = np.outer(self._linear_bias_nu(nu), self._linear_bias_nu(nu))
         M1M2 = np.outer(M, M)
         integrand = beta*W1W2*g1g2*b1b2/M1M2
         integral = util.trapz2d(integrand, nu, nu)
         if do_I11 and massu and massv:
             integral += beta[0, 0]*(A**2)*Wu[0]*Wv[0]/M[0]**2
         if do_I12_I21 and massu:
             g = self._mass_function_nu(nu)
@@ -506,17 +566,16 @@
         if do_I12_I21 and massv:
             g = self._mass_function_nu(nu)
             b = self._linear_bias_nu(nu)
             integrand = beta[:, 0]*Wu*g*b/M
             integral += (A*Wv[0]/M[0])*trapz(integrand, nu)
         return integral*self.rhom**2
 
-
-    def cross_halo_spectrum(self, k:np.ndarray, Pk_lin:np.ndarray, M:np.ndarray, sigmaM:np.ndarray, 
-                            profiles:dict, M_halo:float, beta=None, simple_twohalo=False, k_trunc=None, verbose=False) -> tuple:
+    def cross_halo_spectrum(self, k: np.ndarray, Pk_lin: np.ndarray, M: np.ndarray, sigmaM: np.ndarray,
+                            profiles: dict, M_halo: float, beta=None, simple_twohalo=False, k_trunc=None, verbose=False) -> tuple:
         '''
         Computes the power spectrum of a single tracer crossed with haloes of a single specific mass
         Args:
             k: Comoving wavenumbers [h/Mpc]
             Pk_lin(k): Linear power at each wavenumber [(Mpc/h)^3]
             M: Halo masses [Msun/h]
             sigmaM(M): Standard deviation of density field at scale corresponding to halo mass M
@@ -525,131 +584,150 @@
             beta(k, M): Optional array of beta_NL values at points M, k
             simple_twohalo: Should the scale-dependence of the two-halo term be ignored?
             k_trunc: None or wavenumber [h/Mpc] at which to truncate the one-halo term at large scales
             verbose: verbosity
         '''
         from time import time
         from scipy.interpolate import interp1d
-        if verbose: t_start = time() # Initial time
+        if verbose:
+            t_start = time()  # Initial time
 
         # Checks
-        if simple_twohalo and (beta is not None): raise ValueError('A simple two-halo term is not compatible with non-linear halo bias')
-        if not util.is_array_monotonic(M): raise ValueError('Halo mass array must be increasing monotonically')
-        if not isinstance(profiles, dict): raise TypeError('profiles must be a dictionary')
+        if simple_twohalo and (beta is not None):
+            raise ValueError(
+                'A simple two-halo term is not compatible with non-linear halo bias')
+        if not util.is_array_monotonic(M):
+            raise ValueError(
+                'Halo mass array must be increasing monotonically')
+        if not isinstance(profiles, dict):
+            raise TypeError('profiles must be a dictionary')
         for profile in profiles.values():
-            if (k != profile.k).all(): raise ValueError('k arrays must all be identical to those in profiles')
-            if (M != profile.M).all(): raise ValueError('Mass arrays must be identical to those in profiles')
+            if (k != profile.k).all():
+                raise ValueError(
+                    'k arrays must all be identical to those in profiles')
+            if (M != profile.M).all():
+                raise ValueError(
+                    'Mass arrays must be identical to those in profiles')
 
         # Create arrays of nu values that correspond to the halo mass
-        nu = self._peak_height(M, sigmaM) # TODO: Raise error if nu[0] isn't << 1? or nu[-1] isn't >> 1?
+        # TODO: Raise error if nu[0] isn't << 1? or nu[-1] isn't >> 1?
+        nu = self._peak_height(M, sigmaM)
 
         # Useful information
         if verbose:
             print('Redshift:', self.z)
-            print('Halo mass range [log10(Msun/h)]:', np.log10(M[0]), np.log10(M[-1]))
+            print('Halo mass range [log10(Msun/h)]:',
+                  np.log10(M[0]), np.log10(M[-1]))
             print('Peak height range:', nu[0], nu[-1])
             print('Number of integration points:', len(nu))
 
         # Calculate the missing halo-bias from the low-mass part of the integral
         integrand = self._mass_function_nu(nu)*self._linear_bias_nu(nu)
         A = 1.-halo_integration(integrand, nu)
-        if verbose: print('Missing halo-bias-mass from two-halo integrand:', A)
+        if verbose:
+            print('Missing halo-bias-mass from two-halo integrand:', A)
 
         # Calculate nu(Mh) and W(Mh, k) by interpolating the input arrays
         # NOTE: Wk_halo_mass is not the halo profile, but the profile of the field evaluated at the halo mass!
         nu_M_interp = interp1d(np.log(M), nu, kind='cubic')
         nu_halo = nu_M_interp(np.log(M_halo))
         Wk_halo_mass = {}
         for name, profile in profiles.items():
             Wk = np.empty_like(profile.Wk[:, 0])
             for ik, _ in enumerate(k):
-                WM_interp = interp1d(np.log(M), profile.Wk[ik, :], kind='cubic')
+                WM_interp = interp1d(
+                    np.log(M), profile.Wk[ik, :], kind='cubic')
                 Wk[ik] = WM_interp(np.log(M_halo))
             Wk_halo_mass[name] = Wk.copy()
 
         # Combine everything and return
         Pk_2h_dict, Pk_1h_dict, Pk_hm_dict = {}, {}, {}
         Pk_2h, Pk_1h = np.zeros_like(k), np.zeros_like(k)
         for name, profile in profiles.items():
 
             # Two-halo term if scale-dependence ignored
             if simple_twohalo:
-                Pk_2h = self._Pk_2h_hu(Pk_lin, M, nu_halo, nu, profile.amplitude/profile.normalisation, profile.mass_tracer, A)
+                Pk_2h = self._Pk_2h_hu(
+                    Pk_lin, M, nu_halo, nu, profile.amplitude/profile.normalisation, profile.mass_tracer, A)
 
             # Loop over wavenumbers
             for ik, _Pk_lin in enumerate(Pk_lin):
                 if not simple_twohalo:
                     if beta is None:
-                        Pk_2h[ik] = self._Pk_2h_hu(_Pk_lin, M, nu_halo, nu, profile.Wk[ik, :], profile.mass_tracer, A)
+                        Pk_2h[ik] = self._Pk_2h_hu(
+                            _Pk_lin, M, nu_halo, nu, profile.Wk[ik, :], profile.mass_tracer, A)
                     else:
-                        Pk_2h[ik] = self._Pk_2h_hu(_Pk_lin, M, nu_halo, nu, profile.Wk[ik, :], profile.mass_tracer, A, beta[ik, :])
-                Pk_1h[ik] = Wk_halo_mass[name][ik] # Simply the halo profile at M=Mh here
-            
+                        Pk_2h[ik] = self._Pk_2h_hu(
+                            _Pk_lin, M, nu_halo, nu, profile.Wk[ik, :], profile.mass_tracer, A, beta[ik, :])
+                # Simply the halo profile at M=Mh here
+                Pk_1h[ik] = Wk_halo_mass[name][ik]
+
             # Suppress one-halo term
-            if k_trunc is not None: Pk_1h *= 1.-np.exp(-(k/k_trunc)**2)
+            if k_trunc is not None:
+                Pk_1h *= 1.-np.exp(-(k/k_trunc)**2)
 
             # Finish
             Pk_2h_dict[name], Pk_1h_dict[name] = Pk_2h.copy(), Pk_1h.copy()
             Pk_hm_dict[name] = Pk_2h_dict[name]+Pk_1h_dict[name]
 
         # Finalise
-        if verbose: 
+        if verbose:
             t_end = time()
             print('Halomodel calculation time [s]:', t_end-t_start)
             print()
         return Pk_2h_dict, Pk_1h_dict, Pk_hm_dict
 
-
-    def _Pk_2h_hu(self, Pk_lin:float, M:np.ndarray, nuh:float, nu:np.ndarray, 
-                  Wk:float, mass:bool, A:float, beta=None) -> float:
+    def _Pk_2h_hu(self, Pk_lin: float, M: np.ndarray, nuh: float, nu: np.ndarray,
+                  Wk: float, mass: bool, A: float, beta=None) -> float:
         '''
         Two-halo term for halo-u at a specific wavenumber
         '''
-        I_NL = 0. if beta is None else self._I_beta_hu(beta, M, nuh, nu, Wk, mass, A)
-        Ih = self._linear_bias_nu(nuh) # Simply the linear bias
-        Iu = self._I_2h(M, nu, Wk, mass, A) # Same as for the standard two-halo term
+        I_NL = 0. if beta is None else self._I_beta_hu(
+            beta, M, nuh, nu, Wk, mass, A)
+        Ih = self._linear_bias_nu(nuh)  # Simply the linear bias
+        # Same as for the standard two-halo term
+        Iu = self._I_2h(M, nu, Wk, mass, A)
         return (Ih*Iu+I_NL)*Pk_lin
 
-
-    def _I_beta_hu(self, beta:np.ndarray, M:np.ndarray, nu_halo:float, nu:np.ndarray, 
-                   Wk:np.ndarray, mass:bool, A:float) -> float:
+    def _I_beta_hu(self, beta: np.ndarray, M: np.ndarray, nu_halo: float, nu: np.ndarray,
+                   Wk: np.ndarray, mass: bool, A: float) -> float:
         '''
         Evaluates the beta_NL integral for halo-u
         '''
         from numpy import trapz
         b_halo = self._linear_bias_nu(nu_halo)
         g = self._mass_function_nu(nu)
         b = self._linear_bias_nu(nu)
         integrand = beta*Wk*g*b/M
         integral = trapz(integrand, nu)
-        if mass: integral += A*beta[0]*Wk[0]/M[0]
+        if mass:
+            integral += A*beta[0]*Wk[0]/M[0]
         return b_halo*integral*self.rhom
 
-
-    def _peak_height(self, M:np.ndarray, sigmaM:np.ndarray) -> np.ndarray:
+    def _peak_height(self, M: np.ndarray, sigmaM: np.ndarray) -> np.ndarray:
         '''
         Calculate peak-height (nu) values from array of halo masses
         '''
         nu = self.dc/sigmaM
         return nu
 
-
-    def virial_radius(self, M:np.ndarray) -> np.ndarray:
+    def virial_radius(self, M: np.ndarray) -> np.ndarray:
         '''
         Halo virial radius based on the halo mass and overdensity condition
         Args:
             M: Halo masses [Msun/h]
         '''
         return self.Lagrangian_radius(M)/np.cbrt(self.Dv)
 
 ### ###
 
 ### Beta_NL ###
 
-def interpolate_beta_NL(k:np.ndarray, M:np.ndarray, M_small:np.ndarray, beta_NL_small:np.ndarray, 
+
+def interpolate_beta_NL(k: np.ndarray, M: np.ndarray, M_small: np.ndarray, beta_NL_small: np.ndarray,
                         scheme='RegularGridInterp', **kwargs) -> np.ndarray:
     '''
     Wrapper for various beta_NL interpolation schemes to go from coarse grid of halo masses
     to a finer grid of halo masses.
     Args:
         k: Comoving wavenumbers [h/Mpc]
         M: Desired halo masses [Msun/h]
@@ -657,114 +735,127 @@
         beta_NL_small: Small beta_NL(k, M_small, M_small) array, which needs to be expanded
         scheme: Interpolation scheme
         **kwargs: To be passed to interpolation schemes
     '''
     if scheme == 'interp2d':
         beta_NL = _interpolate_beta_NL(k, M, M_small, beta_NL_small, **kwargs)
     elif scheme == 'RegularGridInterp':
-        beta_NL = _RegularGridInterp_beta_NL(k, M_small, beta_NL_small, k, M, **kwargs)
+        beta_NL = _RegularGridInterp_beta_NL(
+            k, M_small, beta_NL_small, k, M, **kwargs)
     elif scheme == 'RegularGridInterp_log':
-        beta_NL = _RegularGridInterp_beta_NL_log(k, M_small, beta_NL_small, k, M, **kwargs)
+        beta_NL = _RegularGridInterp_beta_NL_log(
+            k, M_small, beta_NL_small, k, M, **kwargs)
     else:
         raise ValueError('beta_NL interpolation method not recognised')
     return beta_NL
 
 
-def _interpolate_beta_NL(k:np.ndarray, M:np.ndarray, M_small:np.ndarray, beta_NL_small:np.ndarray, 
+def _interpolate_beta_NL(k: np.ndarray, M: np.ndarray, M_small: np.ndarray, beta_NL_small: np.ndarray,
                          fill_value=0.) -> np.ndarray:
     '''
     Interpolate beta_NL from a small grid to a large grid for halo-model calculations.
     TODO: Can I remove inefficient loops here?
     '''
     from scipy.interpolate import interp2d
-    beta_NL = np.zeros((len(k), len(M), len(M))) # Array for output
+    beta_NL = np.zeros((len(k), len(M), len(M)))  # Array for output
     for ik, _ in enumerate(k):
         beta_NL_interp = interp2d(np.log(M_small), np.log(M_small), beta_NL_small[ik, :, :],
-            kind='linear', fill_value=fill_value)
+                                  kind='linear', fill_value=fill_value)
         for iM1, M1 in enumerate(M):
             for iM2, M2 in enumerate(M):
                 beta_NL[ik, iM1, iM2] = beta_NL_interp(np.log(M1), np.log(M2))
     return beta_NL
 
 
-def _RegularGridInterp_beta_NL(k_in:np.ndarray, M_in:np.ndarray, beta_NL_in:np.ndarray, 
-                               k_out:np.ndarray, M_out:np.ndarray, method='linear') -> np.ndarray:
+def _RegularGridInterp_beta_NL(k_in: np.ndarray, M_in: np.ndarray, beta_NL_in: np.ndarray,
+                               k_out: np.ndarray, M_out: np.ndarray, method='linear') -> np.ndarray:
     '''
     Supported methods are 'linear', 'nearest', 'slinear', 'cubic', and 'quintic'
     '''
     from scipy.interpolate import RegularGridInterpolator
     bnl_interp = RegularGridInterpolator([np.log(k_in), M_in, M_in], beta_NL_in,
-        method=method, fill_value=None, bounds_error=False)
+                                         method=method, fill_value=None, bounds_error=False)
     bnl_out = np.zeros((len(k_out), len(M_out), len(M_out)))
     indices = np.vstack(np.meshgrid(np.arange(k_out.size), np.arange(M_out.size), np.arange(M_out.size),
                                     copy=False)).reshape(3, -1).T
-    values = np.vstack(np.meshgrid(np.log(k_out), M_out, M_out, 
+    values = np.vstack(np.meshgrid(np.log(k_out), M_out, M_out,
                                    copy=False)).reshape(3, -1).T
     bnl_out[indices[:, 0], indices[:, 1], indices[:, 2]] = bnl_interp(values)
     return bnl_out
 
 
-def _RegularGridInterp_beta_NL_log(k_in:np.ndarray, M_in:np.ndarray, beta_NL_in:np.ndarray, 
-                                   k_out:np.ndarray, M_out:np.ndarray, method='linear') -> np.ndarray:
+def _RegularGridInterp_beta_NL_log(k_in: np.ndarray, M_in: np.ndarray, beta_NL_in: np.ndarray,
+                                   k_out: np.ndarray, M_out: np.ndarray, method='linear') -> np.ndarray:
     '''
     Supported methods are 'linear', 'nearest', 'slinear', 'cubic', and 'quintic'
     '''
     from scipy.interpolate import RegularGridInterpolator
     bnl_interp = RegularGridInterpolator([np.log10(M_in), np.log10(M_in), np.log(k_in)], beta_NL_in,
-        method=method, fill_value=None, bounds_error=False)
+                                         method=method, fill_value=None, bounds_error=False)
     bnl_out = np.zeros((len(k_out), len(M_out), len(M_out)))
-    indices = np.vstack(np.meshgrid(np.arange(k_out.size), np.arange(M_out.size), np.arange(M_out.size), 
+    indices = np.vstack(np.meshgrid(np.arange(k_out.size), np.arange(M_out.size), np.arange(M_out.size),
                                     copy=False)).reshape(3, -1).T
-    values = np.vstack(np.meshgrid(np.log(k_out), np.log10(M_out), np.log10(M_out), 
+    values = np.vstack(np.meshgrid(np.log(k_out), np.log10(M_out), np.log10(M_out),
                                    copy=False)).reshape(3, -1).T
     bnl_out[indices[:, 0], indices[:, 1], indices[:, 2]] = bnl_interp(values)
     return bnl_out
 
 ### ###
 
 ### Halo profiles ###
 
+
 class profile():
     '''
     Class for halo profiles
     '''
-    def __init__(self, k:np.ndarray, M:np.ndarray, Uk:np.ndarray, Wk:np.ndarray, 
+
+    def __init__(self, k: np.ndarray, M: np.ndarray, Uk: np.ndarray, Wk: np.ndarray,
                  amplitude=None, normalisation=1., variance=None, mass_tracer=False, discrete_tracer=False):
         self.k, self.M = k.copy(), M.copy()
         self.Uk, self.Wk = Uk.copy(), Wk.copy()
         self.amplitude = amplitude.copy() if amplitude is not None else None
         self.normalisation = normalisation
         self.variance = variance.copy() if variance is not None else None
         self.mass_tracer, self.discrete_tracer = mass_tracer, discrete_tracer
 
     def __str__(self):
         log_limit = 1e5
         print('Mass tracer:', self.mass_tracer)
         print('Discrete tracer:', self.discrete_tracer)
-        if self.normalisation != 1.: print('Field normalisation:', self.normalisation)
+        if self.normalisation != 1.:
+            print('Field normalisation:', self.normalisation)
         print('Number of wavenumber bins:', len(self.k))
         print('Number of mass bins:', len(self.M))
-        print('Wavenumber range [log10(h/Mpc)]: %1.3f %1.3f'%(np.log10(self.k[0]), np.log10(self.k[-1])))
-        print('Halo mass range [log10(Msun/h)]: %1.3f %1.3f'%(np.log10(self.M[0]), np.log10(self.M[-1])))
+        print('Wavenumber range [log10(h/Mpc)]: %1.3f %1.3f' %
+              (np.log10(self.k[0]), np.log10(self.k[-1])))
+        print('Halo mass range [log10(Msun/h)]: %1.3f %1.3f' %
+              (np.log10(self.M[0]), np.log10(self.M[-1])))
         print('The following are at the low and high halo mass ends')
         if self.amplitude[0] > log_limit:
-            print('Profile amplitude mean [log10]:', np.log10(self.amplitude[0]), np.log10(self.amplitude[-1]))
+            print('Profile amplitude mean [log10]:', np.log10(
+                self.amplitude[0]), np.log10(self.amplitude[-1]))
         else:
-            print('Profile amplitude mean:', self.amplitude[0], self.amplitude[-1])
+            print('Profile amplitude mean:',
+                  self.amplitude[0], self.amplitude[-1])
         if self.variance is not None:
             if self.variance[0] > log_limit:
-                print('Profile amplitude variance [log10]:', np.log10(self.variance[0]), np.log10(self.variance[-1]))
+                print('Profile amplitude variance [log10]:', np.log10(
+                    self.variance[0]), np.log10(self.variance[-1]))
             else:
-                print('Profile amplitude variance:', self.variance[0], self.variance[-1])
-        print('Dimensionless profiles at low k (should be ~1):', self.Uk[0, 0], self.Uk[0, -1])
-        print('Dimensionful profiles at low k (should be amplitudes):', self.Wk[0, 0], self.Wk[0, -1])
+                print('Profile amplitude variance:',
+                      self.variance[0], self.variance[-1])
+        print('Dimensionless profiles at low k (should be ~1):',
+              self.Uk[0, 0], self.Uk[0, -1])
+        print('Dimensionful profiles at low k (should be amplitudes):',
+              self.Wk[0, 0], self.Wk[0, -1])
         return ''
 
     @classmethod
-    def Fourier(cls, k:np.ndarray, M:np.ndarray, Uk:np.ndarray,
+    def Fourier(cls, k: np.ndarray, M: np.ndarray, Uk: np.ndarray,
                 amplitude=None, normalisation=1., variance=None, mass_tracer=False, discrete_tracer=False):
         '''
         Class initialisation for Fourier space halo profiles.
         Uk is assumed to be an array Uk(k, M) of the profile Fourier transform.
         If amplitude=None then Uk is assumed to be dimensionful, otherwise Uk is assumed dimensionless with Uk(k->0, M) = 1
         Matter profiles have amplitude=M (halo mass), galaxy profiles have amplitude=N (number of galaxies)
         Args:
@@ -774,28 +865,30 @@
             amplitude: Halo profile amplitudes at halo masses 'M' (e.g., M for mass; N for galaxies)
             normalisation: Field normalisation (e.g., rhom for mass, mean galaxy number density for galaxies)
             variance: Variance in the profile amplitude at each halo mass (e.g., N for Poisson galaxies)
             mass_tracer: Are contributions expected for M < M[0] (e.g., matter)?
             discrete_tracer: Does the profile correspond to that of a discrete tracer (e.g., galaxies)?
         '''
         # Set internal variables
-        if Uk.shape != (k.shape[0], M.shape[0]): raise ValueError('k, M, array shapes do not match')
+        if Uk.shape != (k.shape[0], M.shape[0]):
+            raise ValueError('k, M, array shapes do not match')
         if amplitude is None:
-            amplitude = Uk[0, :] # TODO: Integrate to get this? This relies on k[0] being small!
+            # TODO: Integrate to get this? This relies on k[0] being small!
+            amplitude = Uk[0, :]
             Wk = Uk.copy()
             _Uk = Uk/amplitude
         else:
             _Uk = Uk.copy()
             Wk = (amplitude*Uk)/normalisation
-        profile = cls(k, M, _Uk, Wk, amplitude=amplitude, normalisation=normalisation, variance=variance, 
+        profile = cls(k, M, _Uk, Wk, amplitude=amplitude, normalisation=normalisation, variance=variance,
                       mass_tracer=mass_tracer, discrete_tracer=discrete_tracer)
         return profile
 
     @classmethod
-    def configuration(cls, k:np.ndarray, M:np.ndarray, rv:np.ndarray, c:np.ndarray, differential_profile:callable,
+    def configuration(cls, k: np.ndarray, M: np.ndarray, rv: np.ndarray, c: np.ndarray, differential_profile: callable,
                       amplitude=None, normalisation=1., variance=None, mass_tracer=False, discrete_tracer=False):
         ''''
         Alternative class initialisation for configuration-space haloes.
         differential_profile is a halo (density or whatever) profile multiplied by 4pi r^2.
         If amp=None then Prho is assumed to be normalised correctly, otherwise Phro can
         have any normalisation and will be renormalaised by amp to have the correct 'mass'.
         TODO: Are loops necessary here?
@@ -810,57 +903,65 @@
             var: Var(N(M)) (auto)variance in the profile amplitude at each halo mass (e.g., N for Poisson galaxies)
             mass_tracer: Are contributions expected for M < M[0] (e.g., matter)?
             discrete_tracer: Does the profile correspond to that of a discrete tracer (e.g., galaxies)?
         '''
         _amplitude = np.zeros_like(M)
         Uk, Wk = np.zeros((len(k), len(M))), np.zeros((len(k), len(M)))
         for iM, (_M, _rv, _c) in enumerate(zip(M, rv, c)):
-            _amplitude[iM] = _halo_window(0., _M, _rv, _c, differential_profile) # Amplitiude
+            _amplitude[iM] = _halo_window(
+                0., _M, _rv, _c, differential_profile)  # Amplitiude
         for ik, _k in enumerate(k):
             for iM, (_M, _rv, _c) in enumerate(zip(M, rv, c)):
                 W = _halo_window(_k, _M, _rv, _c, differential_profile)
                 if amplitude is None:
                     Wk[ik, iM] = W
-                    Uk[ik, iM] = Wk[ik, iM]/_amplitude[iM] # Normalise
+                    Uk[ik, iM] = Wk[ik, iM]/_amplitude[iM]  # Normalise
                 else:
                     Uk[ik, iM] = W/_amplitude[iM]
                     Wk[ik, iM] = Uk[ik, iM]*amplitude[iM]
-        if amplitude is not None: _amplitude = amplitude.copy()
-        profile = cls.Fourier(k, M, Uk, amplitude=_amplitude, normalisation=normalisation, variance=variance, 
+        if amplitude is not None:
+            _amplitude = amplitude.copy()
+        profile = cls.Fourier(k, M, Uk, amplitude=_amplitude, normalisation=normalisation, variance=variance,
                               mass_tracer=mass_tracer, discrete_tracer=discrete_tracer)
         return profile
 
 ### Halo profiles in configuration space ###
 
-def _halo_window(k:float, M:float, rv:float, c:float, diff_profile:callable) -> float:
+
+def _halo_window(k: float, M: float, rv: float, c: float, diff_profile: callable) -> float:
     '''
     Compute the halo window function via integration given a differential 'density' profile P(r) = 4*pi*r^2*rho(r)
     TODO: This should almost certainly be done with a dedicated integration routine
     TODO: Can this be made to accept arrays of M, rv, c as arguments? This would avoid loops
     '''
     from scipy.special import spherical_jn
 
     if win_integration in [integrate.trapezoid, integrate.simps, integrate.romb]:
         R = np.linspace(0., rv, nr_win_integration)
         integrand = spherical_jn(0, k*R)*diff_profile(R, M, rv, c)
-        if win_integration in [integrate.romb]: dR = R[1]-R[0]
+        if win_integration in [integrate.romb]:
+            dR = R[1]-R[0]
 
     # Integration
     if win_integration in [integrate.trapezoid, integrate.simps]:
         Wk = win_integration(integrand, R)
     elif win_integration in [integrate.romb]:
         Wk = win_integration(integrand, dR)
     elif win_integration in [integrate.quad]:
-        Wk, _ = win_integration(lambda r: spherical_jn(0, k*r)*diff_profile(r, M, rv, c), 0., rv, epsrel=eps_win_integration)
+        Wk, _ = win_integration(lambda r: spherical_jn(
+            0, k*r)*diff_profile(r, M, rv, c), 0., rv, epsrel=eps_win_integration, epsabs=0.)
     elif win_integration in [integrate.quadrature]:
-        Wk, _ = win_integration(lambda r: spherical_jn(0, k*r)*diff_profile(r, M, rv, c), 0., rv, rtol=eps_win_integration)
+        Wk, _ = win_integration(lambda r: spherical_jn(
+            0, k*r)*diff_profile(r, M, rv, c), 0., rv, rtol=eps_win_integration, tol=0.)
     elif win_integration in [integrate.romberg]:
-        Wk = win_integration(lambda r: spherical_jn(0, k*r)*diff_profile(r, M, rv, c), 0., rv, rtol=eps_win_integration)
+        Wk = win_integration(lambda r: spherical_jn(
+            0, k*r)*diff_profile(r, M, rv, c), 0., rv, rtol=eps_win_integration, tol=0.)
     else:
-        raise ValueError('Halo window function integration method not recognised')
+        raise ValueError(
+            'Halo window function integration method not recognised')
     return Wk
 
 
 # def differential_profile(r:float, M:float, rv:float, c:float, name=None) -> np.ndarray:
 #     '''
 #     Differential halo profile as a function of radius from the halo centre
 #     Integrating this against r, from 0 to rv, gives the total contribution from the halo
@@ -898,15 +999,15 @@
 #     rs = rv/c
 #     return (M/c)*(r/rv**2)*(c**3)*_NFW_factor(c)/(1.+r/rs)**2
 
 ### ###
 
 ### Halo profiles in Fourier space ###
 
-def window_function(k:np.ndarray, rv:np.ndarray, *args, profile=None) -> np.ndarray:
+def window_function(k: np.ndarray, rv: np.ndarray, *args, profile=None) -> np.ndarray:
     '''
     Fourier transforms of halo profiles
     Args:
         k: Comoving wavenumbers [h/Mpc]
         rv: Comoving halo virial radii [Mpc/h]
         *args: Additional arguments for halo profiles (e.g., concentration)
         profile: Profile name: 
@@ -921,26 +1022,26 @@
     elif profile == 'NFW':
         Wk = _win_NFW(k, rv, *args)
     else:
         raise ValueError('Halo profile not recognised')
     return Wk
 
 
-def _win_isothermal(k:np.ndarray, rv:np.ndarray) -> np.ndarray:
+def _win_isothermal(k: np.ndarray, rv: np.ndarray) -> np.ndarray:
     '''
     Normalised Fourier transform for an isothermal profile
     '''
     from scipy.special import sici
     kv = np.outer(k, rv)
     Si, _ = sici(kv)
     Wk = Si/(kv)
     return Wk
 
 
-def _win_NFW(k:np.ndarray, rv:np.ndarray, c:np.ndarray) -> np.ndarray:
+def _win_NFW(k: np.ndarray, rv: np.ndarray, c: np.ndarray) -> np.ndarray:
     '''
     Normalised Fourier transform for an NFW profile
     '''
     from scipy.special import sici
     rs = rv/c
     kv = np.outer(k, rv)
     ks = np.outer(k, rs)
@@ -950,22 +1051,22 @@
     f2 = np.sin(ks)*(Sisv-Sis)
     f3 = np.sin(kv)/(ks+kv)
     f4 = _NFW_factor(c)
     Wk = (f1+f2-f3)/f4
     return Wk
 
 
-def _NFW_factor(c:np.ndarray) -> np.ndarray:
+def _NFW_factor(c: np.ndarray) -> np.ndarray:
     '''
     Factor from normalisation that always appears in NFW equations
     '''
     return np.log(1.+c)-c/(1.+c)
 
 
-def matter_profile(k:np.ndarray, M:np.ndarray, rv:np.ndarray, c:np.ndarray, Om_m:float) -> profile:
+def matter_profile(k: np.ndarray, M: np.ndarray, rv: np.ndarray, c: np.ndarray, Om_m: float) -> profile:
     '''
     Pre-configured matter NFW profile
     Args:
         k: Comoving wavenumbers [h/Mpc]
         M: Halo masses [Msun/h]
         rv: Comoving halo virial radii [Mpc/h]
         c: Halo concentrations
@@ -973,17 +1074,18 @@
     '''
     rhom = cosmology.comoving_matter_density(Om_m)
     Uk = window_function(k, rv, c, profile='NFW')
     return profile.Fourier(k, M, Uk, amplitude=M, normalisation=rhom, mass_tracer=True)
 
 ### ###
 
-### Halo concentration
+# Halo concentration
+
 
-def concentration(M:np.ndarray, z:float, method='Duffy et al. (2008)', halo_definition='M200') -> np.ndarray:
+def concentration(M: np.ndarray, z: float, method='Duffy et al. (2008)', halo_definition='M200') -> np.ndarray:
     '''
     Halo concentration as a function of halo mass and redshift
     Args:
         M: Halo masses [Msun/h]
         z: redshift
         method: Name of concentration-mass relataion
             Duffy et al. (2008)
@@ -995,35 +1097,42 @@
     if method == 'Duffy et al. (2008)':
         c = _concentration_Duffy(M, z, halo_definition)
     else:
         raise ValueError('Halo concentration not recognised')
     return c
 
 
-def _concentration_Duffy(M:np.ndarray, z:float, halo_definition='M200') -> np.ndarray:
+def _concentration_Duffy(M: np.ndarray, z: float, halo_definition='M200') -> np.ndarray:
     '''
     Duffy et al (2008; 0804.2486) c(M) relation for WMAP5, See Table 1
     Appropriate for the full (rather than relaxed) samples
     '''
-    M_piv = 2e12 # Pivot mass [Msun/h]
+    M_piv = 2e12  # Pivot mass [Msun/h]
     if halo_definition in ['M200', '200', '200b']:
-        A = 10.14; B = -0.081; C = -1.01
+        A = 10.14
+        B = -0.081
+        C = -1.01
     elif halo_definition in ['vir', 'virial', 'Mvir']:
-        A = 7.85; B = -0.081; C = -0.71
+        A = 7.85
+        B = -0.081
+        C = -0.71
     elif halo_definition in ['M200c', '200c']:
-        A = 5.71; B = -0.084; C = -0.47
+        A = 5.71
+        B = -0.084
+        C = -0.47
     else:
         raise ValueError('Halo definition not recognised')
-    return A*(M/M_piv)**B*(1.+z)**C # Equation (4) in 0804.2486
+    return A*(M/M_piv)**B*(1.+z)**C  # Equation (4) in 0804.2486
 
 ### ###
 
 ### Halo-occupation distribution (HOD) ###
 
-def HOD_mean(M:np.ndarray, method='Zheng et al. (2005)', **kwargs) -> tuple:
+
+def HOD_mean(M: np.ndarray, method='Zheng et al. (2005)', **kwargs) -> tuple:
     '''
     Returns the expected (mean) number of central and satellite galaxies as a tuple
     Halo occupation distribution (HOD)
     Args:
         M: Halo masses [Msun/h]
         method: Name of 
             'simple': Very basic HOD, see code
@@ -1041,73 +1150,74 @@
     elif method == 'Zhai et al. (2017)':
         result = _HOD_Zhai(M, **kwargs)
     else:
         raise ValueError('HOD method not recognised')
     return result
 
 
-def _HOD_simple(M:np.ndarray, Mmin=1e12, Msat=1e13, alpha=1.) -> tuple:
+def _HOD_simple(M: np.ndarray, Mmin=1e12, Msat=1e13, alpha=1.) -> tuple:
     '''
     Simple HOD model
     '''
     Nc = np.heaviside(M-Mmin, 1.)
     Ns = Nc*(M/Msat)**alpha
     return Nc, Ns
 
 
-def _HOD_Zehavi(M:np.ndarray, Mmin=1e12, M1=1e13, alpha=1.) -> tuple:
+def _HOD_Zehavi(M: np.ndarray, Mmin=1e12, M1=1e13, alpha=1.) -> tuple:
     '''
     HOD model from Zehavi et al. (2004; https://arxiv.org/abs/astro-ph/0703457)
     Same as Zheng model in the limit that sigma=0 and M0=0
     Mean number of central galaxies is only ever 0 or 1 in this HOD
     '''
     Nc = np.heaviside(M-Mmin, 1.)
     Ns = (M/M1)**alpha
     return Nc, Ns
 
 
-def _HOD_Zheng(M:np.ndarray, Mmin=1e12, sigma=0.15, M0=1e12, M1=1e13, alpha=1.) -> tuple:
+def _HOD_Zheng(M: np.ndarray, Mmin=1e12, sigma=0.15, M0=1e12, M1=1e13, alpha=1.) -> tuple:
     '''
     Zheng et al. (2005; https://arxiv.org/abs/astro-ph/0408564) HOD model
     '''
     from scipy.special import erf
     if sigma == 0.:
         Nc = np.heaviside(M-Mmin, 1.)
     else:
         Nc = 0.5*(1.+erf(np.log10(M/Mmin)/sigma))
     Ns = (np.heaviside(M-M0, 1.)*(M-M0)/M1)**alpha
     return Nc, Ns
 
 
-def _HOD_Zhai(M:np.ndarray, Mmin=10**13.68, sigma=0.82, Msat=10**14.87, alpha=0.41, Mcut=10**12.32) -> tuple:
+def _HOD_Zhai(M: np.ndarray, Mmin=10**13.68, sigma=0.82, Msat=10**14.87, alpha=0.41, Mcut=10**12.32) -> tuple:
     '''
     HOD model from Zhai et al. (2017; https://arxiv.org/abs/1607.05383)
     '''
     from scipy.special import erf
     if sigma == 0.:
         Nc = np.heaviside(M-Mmin, 1.)
     else:
         Nc = 0.5*(1.+erf(np.log10(M/Mmin)/sigma))
-    Ns = ((M/Msat)**alpha)*np.exp(-Mcut/M) # Paper has a Nc(M) multiplication, but I think the central condition covers this
+    # Paper has a Nc(M) multiplication, but I think the central condition covers this
+    Ns = ((M/Msat)**alpha)*np.exp(-Mcut/M)
     return Nc, Ns
 
 
-def HOD_variance(p:np.ndarray, lam:np.ndarray, central_condition=False) -> tuple:
+def HOD_variance(p: np.ndarray, lam: np.ndarray, central_condition=False) -> tuple:
     '''
     Expected variance (and covariance) in the numbers of central and satellite galaxies
     Assumes Bernoulli statistics for centrals and Poisson statistics for satellites
     The central condition modifies an 'underlying' Poisson distribution in a calculable way
     Args:
         p: Probability of halo hosting a central galaxy
         lam: Mean number of satellite galaxies (iff central_condition=False)
         central_condition: Does a central need to be present in order for there to be a satellite?
     '''
-    vcc = p*(1.-p) # Bernoulli
+    vcc = p*(1.-p)  # Bernoulli
     if central_condition:
-        vss = p*lam*(1.+lam*(1.-p)) # Modified Poisson
+        vss = p*lam*(1.+lam*(1.-p))  # Modified Poisson
         vcs = lam*(1.-p)            # Induced covariance
     else:
-        vss = lam # Poisson
+        vss = lam  # Poisson
         vcs = 0.  # No covariance
     return vcc, vss, vcs
 
-### ###
+### ###
```

### Comparing `pyhalomodel-1.0.1/pyhalomodel/utility.py` & `pyhalomodel-1.0.2/pyhalomodel/utility.py`

 * *Files identical despite different names*

### Comparing `pyhalomodel-1.0.1/pyproject.toml` & `pyhalomodel-1.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 [tool.poetry]
 name = "pyhalomodel"
-version = "1.0.1"
+version = "1.0.2"
 description = "Halo model power spectrum calculations"
 authors = ["Alexander Mead <alexander.j.mead@googlemail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/alexander-mead/pyhalomodel"
 keywords = ["cosmology", "halo model", "dark matter", "dark energy", "galaxies"]
-include = [
-    "LICENSE",
-]
+include = ["LICENSE"]
+
+[tool.poetry.group.notebooks]
+optional = true
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.9,<3.13"
 numpy = "^1.24.1"
 scipy = "^1.10.0"
 
 [tool.poetry.group.dev.dependencies]
 camb = "^1.4.0"
-dark-emulator = "^1.0.23"
 ipykernel = "^6.21.1"
 matplotlib = "^3.6.3"
+
+[tool.poetry.group.notebooks.dependencies]
+dark-emulator = "^1.0.23"
 hmf = "^3.4.4"
 halomod = "^2.1.0"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `pyhalomodel-1.0.1/setup.py` & `pyhalomodel-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,150 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyhalomodel
+Version: 1.0.2
+Summary: Halo model power spectrum calculations
+Home-page: https://github.com/alexander-mead/pyhalomodel
+License: MIT
+Keywords: cosmology,halo model,dark matter,dark energy,galaxies
+Author: Alexander Mead
+Author-email: alexander.j.mead@googlemail.com
+Requires-Python: >=3.9,<3.13
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: numpy (>=1.24.1,<2.0.0)
+Requires-Dist: scipy (>=1.10.0,<2.0.0)
+Project-URL: Repository, https://github.com/alexander-mead/pyhalomodel
+Description-Content-Type: text/markdown
+
+# `pyhalomodel`
+
+![image](https://user-images.githubusercontent.com/9140961/228342339-e1f908c7-e2ac-46c2-bb2a-1878bbfa3cf0.png)
+
+This repository is home to the `pyhalomodel` package, which was written as part of the [Asgari, Mead & Heymans (2023)](https://arxiv.org/abs/2303.08752) halo-model review paper. The software is written entirely in `Python`, with extendability and reusability in mind. The purpose of this software is to take some of the drudgery out of performing basic calculations using the halo model. While the integrals that the halo model requires the researcher to evaluate are simple, in practice the changes of variables required to integrate halo profiles against halo mass functions can be confusing and tedious. In our experience this confusion has led to bugs and misunderstandings over the years, and our hope for this software is to reduce the proliferation of these somewhat. Our software can produce power spectra for *any* combinations of tracers, and simply requires halo profiles for the tracers to be specified. These could be matter profiles, galaxy profiles, or anything else, for example electron-pressure or HI profiles.
+
+You might also be interested in this pure `Python` implementation of [HMcode](https://github.com/alexander-mead/HMcode-python), which makes use of the `pyhalomodel` package.
+
+## Dependencies
+* `numpy`
+* `scipy`
+
+## Installation
+For the general user, `pyhalomodel` can be installed using `pip`:
+```bash
+> pip install pyhalomodel
+```
+If you you want to modify the source, or use the demo notebooks, then simply clone the repository. You can then create an environment with all necessary dependencies using [poetry](https://python-poetry.org/). From the cloned `pyhalomodel` directory:
+```bash
+> poetry install
+```
+The demo notebooks require some additional dependencies: `camb`; `dark-emulator`; `ipykernel`; `matplotlib`; `halomod`. These will be installed in the environment automatically. You can also install without `poetry`, either system wide or using another environment manager; we include a `requirements.txt`.
+
+## Usage
+Start a script with
+```python
+import numpy as np
+import pyhalomodel as halo
+```
+Importing via `import pyhalomodel as halo` is nice because the functions and classes then have readable names (e.g., `halo.model`, `halo.profile`). To make non-linear power spectrum predictions using the halo model requires a linear power spectrum. In our demonstration notebooks we always take this from `CAMB`, but it could come from any source. Calculations also require the variance in the linear density field when smoothed on comoving scale $R$: $\sigma^2(R)$. Once again, this function could come from any source, but we take it from `CAMB`.
+
+A typical call to create an instance of a `model` object looks like
+```python
+model = halo.model(z, Omega_m, name='Tinker et al. (2010)', Dv=330., dc=1.686, verbose=True)
+```
+where:
+- `z` is the redshift
+- `Omega_m` is the cosmological matter density parameter (at $z=0$)
+- `name` is the name of the halo mass function/linear halo bias pair to use
+- `Dv` is the halo overdensity definition
+- `dc` is the linear collapse threshold
+
+Currently supported `name` choices are:
+- `Press & Schecter (1974)`
+- `Sheth & Tormen (1999)`
+- `Sheth, Mo & Tormen (2001)`
+- `Tinker et al. (2010)`
+- `Despali et al. (2016)`
+
+When the `model` instance is created the desired mass function is initialised.
+
+To make a power-spectrum calculation one simply calls:
+```python
+Pk_2h, Pk_1h, Pk_hm = model.power_spectrum(k, Pk_lin, M, sigmaM, profiles)
+```
+where: 
+- `k` is an array of comoving Fourier wavenumbers (units: $h\mathrm{Mpc}^{-1}$)
+- `Pk_lin` is an array of linear power spectrum values at a given `k` (units: $(h^{-1}\mathrm{Mpc})^3$)
+- `M` is an array of halo masses (units: $h^{-1}M_\odot$)
+- `sigmaM` is an array of root-variance linear density values at Lagrangian scales corresponding to `M`
+- `profiles` is a dictionary of halo `profile`s (which could contain a single entry)
+
+The function returns a tuple of `Pk_2h` (two-halo), `Pk_1h` (one-halo), and `Pk_hm` (halo model) power at the chosen `k` values. The `power_spectrum` method computes all possible auto- and cross-spectra given the dictionary of halo profiles. For example, if three profiles were in the dictionary this would compute the three autospectra and the three unique cross spectra. The returned `Pk` are then dictionaries containing all possible spectra. For example, if `profiles={'a':profile_a, 'b':profile_b, 'c':profile_c}` then the `Pk` dictionaries will contain the keys: `a-a`; `a-b`; `a-c`; `b-b`; `b-c`, `c-c`. It will also contain symmetric combinations (e.g., `b-a` as well as `a-b`) but the values will be identical. Each value in the `Pk` dictionary is an array of the power at all `k`.
+
+Halo profiles are instances of the `profile` class. These are initialised in Fourier space like:
+```python
+profile = halo.profile.Fourier(k, M, Uk, amplitude=None, normalisation=1., variance=None, mass_tracer=False, discrete_tracer=False)
+```
+where
+- `k` is an array of comoving Fourier wavenumbers (units: $h\mathrm{Mpc}^{-1}$)
+- `M` is an array of halo masses (units: $h^{-1}M_\odot$)
+- `Uk` is a 2D array of the Fourier halo profile at each `k` (first index) and `M` (second index) value
+- `amplitude` is an array of (mean) profile amplitudes, corresponding to each `M`
+- `normalisation` is a float containing the field normalisation
+- `variance` is an array containing the variance in the profile amplitude at each `M`
+- `mass_tracer` is a boolean telling the code if the profile corresponds to mass density
+- `discrete_tracer` is a boolean telling the code if it dealing with a discrete tracer or not
+
+The arrays `k` and `M` be identical to those in the subsequent `model.power_spectrum` call. If `amplitude=None` the Fourier profile is assumed to be normalised such that $U(k\to0, M)$ gives the total contribution of the halo to the field. Otherwise the profile is renormalised by the `amplitude`, and $U(k\to0, M)=1$ is assumed.
+
+Some examples best illustrate how to create your own halo profiles:
+```python
+matter_profile = halo.profile.Fourier(k, M, Uk_matter, amplitude=M, normalisation=rho_matter, mass_tracer=True)
+```
+would create a matter profile. Here `Uk_matter` would be the normalised Fourier transform of a matter profile (e.g., an NFW profile), the amplitude of each profile is exactly `M` (because the haloes are the mass), but the field normalisation is `rho_matter` (which can be accessed via `model.rhom`) because the field we are usually interested in is matter *overdensity*. We use `mass_tracer=True` to tell the code that the profile corresponds to mass. Note that in this case we would get identical behaviour if we fixed the profile amplitude as `amplitude=M/rho_matter` and the field normalisation as `normalisation=1.`.
+```python
+galaxy_profile = halo.profile.Fourier(k, M, Uk_galaxy, amplitude=N_galaxy, normalisation=rho_galaxy, variance=var_galaxy, discrete_tracer=True)
+```
+would create a galaxy profile. Here `Uk_galaxy` would be the normalised Fourier transform of a galaxy profile (e.g., an isothermal profile). The amplitude of the profile is the mean galaxy-occupation number at each `M`: `N_galaxy`. The field is normalised by the mean galaxy density: `rho_galaxy`. For a given assumption about the mean galaxy-occupation number and halo model this can be calculated using the `average` method of the `model` class:
+```python
+rho_galaxy = hmod.average(M, sigmaM, N_galaxy)
+```
+The variance in galaxy number at each `M` is `var_galaxy`. If one is assuming Poisson statistics then `variance=N_galaxy` is appropriate, but any value can be used in principle, including `variance=None`, which ignores the contribution of tracer-occupation variance to the power. We tell the code that `discrete_tracer=True` because in the discrete-tracer case it is essential to split the profile amplitude from the field normalisation if the discreteness of the tracer is to be accounted for properly.
+
+Halo profiles can also be specified in configuration (real) space, via a function of radius from the halo centre. This is slower than specifying the Fourier profiles since the conversion of the profile to Fourier space will need to be performed internally.
+```python
+halo.profile.configuration(k, M, rv, c, differential_profile, amplitude=None, normalisation=1., variance=None, mass_tracer=False, discrete_tracer=False):
+```
+the arguments are similar to those for Fourier-space profiles, except that
+- `differential_profile` is a the halo profile multiplied by $4\pi r^2$ with call signature `differential_profile(r, M, rv, c)`
+- `rv` is the halo virial radius (units: $h^{-1}\mathrm{Mpc}$)
+- `c` is the halo concentration
+
+the differential halo profile is the function defined such that integrating in radius between $0$ and $r_\mathrm{v}$ gives the total contribution of an individual halo to the field. It is usually the standard density profile multiplied $4\pi r^2$. This convention is used so as to avoid singularities that often occur in halo profiles at $r=0$. Again, some examples best illustrate how to use this
+```python
+def differential_profile_matter(r, M, rv, c):
+    # This is NFW (1./((r/rs)*(1.+r/rs)**2)) multiplied by 4pir^2 with constant factors ignored
+    rs = rv/c
+    return r/(1.+r/rs)**2.
+
+matter_profile = halo.profile.configuration(k, M, rv, c, differential_profile_matter, amplitude=M/rho_matter, mass_tracer=True)
+```
+note that because we specify the amplitude here we do not need to worry about constant factors in the `differential_profile` definition, since the profile normalisation will be calculated self consistently. Note also that because we set `amplitude=M/rho_matter` (matter *overdensity*) we can omit the `normalisation` argument, which defaults to `1.`.
+```python
+# Isothermal profile: 1/r^2, multiplied by 4pir^2 with constant factors ignored
+differential_profile_gal = lambda r, M, rv, c: 1. 
+
+galaxy_profile = halo.profile.configuration(k, M, rv, c, differential_profile_gal, amplitude=N_galaxy, normalisation=rho_galaxy, discrete_tracer=True)
+```
+in the discrete tracer case it is important to split up `normalisation` and `amplitude` so that `amplitude` is something that can be interpreted as the mean of a discrete probability distribution. In this example we have also decided to ignore the contribution of the variance in the number of galaxies at fixed halo mass to the eventual power spectrum calculation.
 
-packages = \
-['pyhalomodel']
+Note that the *covariance* in the mean profile amplitude between two different tracers is not currently supported. This can be important in halo-occupation models where galaxies are split into centrals and satellites and the presence of a satellite galaxy is conditional on the halo first containing a central galaxy. We hope to include this in future. Also any *spatial* variance or covariance in halo profiles at fixed mass is not currently supported; we have no plans to include this in future.
 
-package_data = \
-{'': ['*']}
+## Notebooks
+There are several `jupyter` notebooks in the `notebooks/` directory giving examples of how to use the code. The first one to try is `demo-basic.ipynb`, which gives an overview of the main features of `pyhalomodel`. As a bonus, we include notebooks that produce (almost) all of the plots from the review paper.
 
-install_requires = \
-['numpy>=1.24.1,<2.0.0', 'scipy>=1.10.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'pyhalomodel',
-    'version': '1.0.1',
-    'description': 'Halo model power spectrum calculations',
-    'long_description': "# Halo model\nThis repository is home to the `pyhalomodel` package, which was written as part of the [Asgari, Mead & Heymans (2023)](https://arxiv.org/) halo-model review paper. The software is written entirely in `Python`, with extendability and reusability in mind. The purpose of this software is to take some of the drudgery out of performing basic calculations using the halo model. While the integrals that the halo model requires the researcher to evaluate are simple, in practice the changes of variables required to integrate halo profiles against halo mass functions can be confusing and tedious. In our experience this confusion has led to bugs and misunderstandings over the years, and our hope for this software is to reduce the proliferation of these somewhat. Our software can produce power spectra for *any* combinations of tracers, and simply requires halo profiles for the tracers to be specified. These could be matter profiles, galaxy profiles, or anything else, for example electron-pressure or HI profiles.\n\nYou might also be interested in this pure `Python` implementation of [HMcode](https://github.com/alexander-mead/HMcode-python), which makes use of the `pyhalomodel` package.\n\n## Dependencies\n* `numpy`\n* `scipy`\n\n## Installation\nFor the general user, `pyhalomodel` can be installed using `pip`:\n```\npip install pyhalomodel\n```\nIf you you want to modify the source, or use the demo notebooks, then simply clone the repository. You can then create an environment with all necessary dependencies using [poetry](https://python-poetry.org/). From the cloned `pyhalomodel` directory:\n```\npoetry install\n```\nThe demo notebooks require some additional dependencies: `camb`; `dark-emulator`; `ipykernel`; `matplotlib`; `halomod`. These will be installed in the environment automatically. You can also install without `poetry`, either system wide or using another environment manager; we include a `requirements.txt`.\n\n## Usage\nStart a script with\n```\nimport numpy as np\nimport pyhalomodel as halo\n```\nImporting via `import pyhalomodel as halo` is nice because the functions and classes then have readable names (e.g., `halo.model`, `halo.profile`). To make non-linear power spectrum predictions using the halo model requires a linear power spectrum. In our demonstration notebooks we always take this from `CAMB`, but it could come from any source. Calculations also require the variance in the linear density field when smoothed on comoving scale $R$: $\\sigma^2(R)$. Once again, this function could come from any source, but we take it from `CAMB`.\n\nA typical call to create an instance of a `model` object looks like\n```\nmodel = halo.model(z, Omega_m, name='Tinker et al. (2010)', Dv=330., dc=1.686, verbose=True)\n```\nwhere:\n- `z` is the redshift\n- `Omega_m` is the cosmological matter density parameter (at $z=0$)\n- `name` is the name of the halo mass function/linear halo bias pair to use\n- `Dv` is the halo overdensity definition\n- `dc` is the linear collapse threshold\n\nCurrently supported `name` choices are:\n- `Press & Schecter (1974)`\n- `Sheth & Tormen (1999)`\n- `Sheth, Mo & Tormen (2001)`\n- `Tinker et al. (2010)`\n- `Despali et al. (2016)`\n\nWhen the `model` instance is created the desired mass function is initialised.\n\nTo make a power-spectrum calculation one simply calls:\n```\nPk_2h, Pk_1h, Pk_hm = model.power_spectrum(k, Pk_lin, M, sigmaM, profiles)\n```\nwhere: \n- `k` is an array of comoving Fourier wavenumbers (units: $h\\mathrm{Mpc}^{-1}$)\n- `Pk_lin` is an array of linear power spectrum values at a given `k` (units: $(h^{-1}\\mathrm{Mpc})^3$)\n- `M` is an array of halo masses (units: $h^{-1}M_\\odot$)\n- `sigmaM` is an array of root-variance linear density values at Lagrangian scales corresponding to `M`\n- `profiles` is a dictionary of halo `profile`s (which could contain a single entry)\n\nThe function returns a tuple of `Pk_2h` (two-halo), `Pk_1h` (one-halo), and `Pk_hm` (halo model) power at the chosen `k` values. The `power_spectrum` method computes all possible auto- and cross-spectra given the dictionary of halo profiles. For example, if three profiles were in the dictionary this would compute the three autospectra and the three unique cross spectra. The returned `Pk` are then dictionaries containing all possible spectra. For example, if `profiles={'a':profile_a, 'b':profile_b, 'c':profile_c}` then the `Pk` dictionaries will contain the keys: `a-a`; `a-b`; `a-c`; `b-b`; `b-c`, `c-c`. It will also contain symmetric combinations (e.g., `b-a` as well as `a-b`) but the values will be identical. Each value in the `Pk` dictionary is an array of the power at all `k`.\n\nHalo profiles are instances of the `profile` class. These are initialised in Fourier space like:\n```\nprofile = halo.profile.Fourier(k, M, Uk, amplitude=None, normalisation=1., variance=None, mass_tracer=False, discrete_tracer=False)\n```\nwhere\n- `k` is an array of comoving Fourier wavenumbers (units: $h\\mathrm{Mpc}^{-1}$)\n- `M` is an array of halo masses (units: $h^{-1}M_\\odot$)\n- `Uk` is a 2D array of the Fourier halo profile at each `k` (first index) and `M` (second index) value\n- `amplitude` is an array of (mean) profile amplitudes, corresponding to each `M`\n- `normalisation` is a float containing the field normalisation\n- `variance` is an array containing the variance in the profile amplitude at each `M`\n- `mass_tracer` is a boolean telling the code if the profile corresponds to mass density\n- `discrete_tracer` is a boolean telling the code if it dealing with a discrete tracer or not\n\nThe arrays `k` and `M` be identical to those in the subsequent `model.power_spectrum` call. If `amplitude=None` the Fourier profile is assumed to be normalised such that $U(k\\to0, M)$ gives the total contribution of the halo to the field. Otherwise the profile is renormalised by the `amplitude`, and $U(k\\to0, M)=1$ is assumed.\n\nSome examples best illustrate how to create your own halo profiles:\n```\nmatter_profile = halo.profile.Fourier(k, M, Uk_matter, amplitude=M, normalisation=rho_matter, mass_tracer=True)\n```\nwould create a matter profile. Here `Uk_matter` would be the normalised Fourier transform of a matter profile (e.g., an NFW profile), the amplitude of each profile is exactly `M` (because the haloes are the mass), but the field normalisation is `rho_matter` (which can be accessed via `model.rhom`) because the field we are usually interested in is matter *overdensity*. We use `mass_tracer=True` to tell the code that the profile corresponds to mass. Note that in this case we would get identical behaviour if we fixed the profile amplitude as `amplitude=M/rho_matter` and the field normalisation as `normalisation=1.`.\n```\ngalaxy_profile = halo.profile.Fourier(k, M, Uk_galaxy, amplitude=N_galaxy, normalisation=rho_galaxy, variance=var_galaxy, discrete_tracer=True)\n```\nwould create a galaxy profile. Here `Uk_galaxy` would be the normalised Fourier transform of a galaxy profile (e.g., an isothermal profile). The amplitude of the profile is the mean galaxy-occupation number at each `M`: `N_galaxy`. The field is normalised by the mean galaxy density: `rho_galaxy`. For a given assumption about the mean galaxy-occupation number and halo model this can be calculated using the `average` method of the `model` class:\n```\nrho_galaxy = hmod.average(M, sigmaM, N_galaxy)\n```\nThe variance in galaxy number at each `M` is `var_galaxy`. If one is assuming Poisson statistics then `variance=N_galaxy` is appropriate, but any value can be used in principle, including `variance=None`, which ignores the contribution of tracer-occupation variance to the power. We tell the code that `discrete_tracer=True` because in the discrete-tracer case it is essential to split the profile amplitude from the field normalisation if the discreteness of the tracer is to be accounted for properly.\n\nHalo profiles can also be specified in configuration (real) space, via a function of radius from the halo centre. This is slower than specifying the Fourier profiles since the conversion of the profile to Fourier space will need to be performed internally.\n```\nhalo.profile.configuration(k, M, rv, c, differential_profile, amplitude=None, normalisation=1., variance=None, mass_tracer=False, discrete_tracer=False):\n```\nthe arguments are similar to those for Fourier-space profiles, except that\n- `differential_profile` is a the halo profile multiplied by $4\\pi r^2$ with call signature `differential_profile(r, M, rv, c)`\n- `rv` is the halo virial radius (units: $h^{-1}\\mathrm{Mpc}$)\n- `c` is the halo concentration\n\nthe differential halo profile is the function defined such that integrating in radius between $0$ and $r_\\mathrm{v}$ gives the total contribution of an individual halo to the field. It is usually the standard density profile multiplied $4\\pi r^2$. This convention is used so as to avoid singularities that often occur in halo profiles at $r=0$. Again, some examples best illustrate how to use this\n```\ndef differential_profile_matter(r, M, rv, c):\n    # This is NFW (1./((r/rs)*(1.+r/rs)**2)) multiplied by 4pir^2 with constant factors ignored\n    rs = rv/c\n    return r/(1.+r/rs)**2.\n\nmatter_profile = halo.profile.configuration(k, M, rv, c, differential_profile_matter, amplitude=M/rho_matter, mass_tracer=True)\n```\nnote that because we specify the amplitude here we do not need to worry about constant factors in the `differential_profile` definition, since the profile normalisation will be calculated self consistently. Note also that because we set `amplitude=M/rho_matter` (matter *overdensity*) we can omit the `normalisation` argument, which defaults to `1.`.\n```\n# Isothermal profile: 1/r^2, multiplied by 4pir^2 with constant factors ignored\ndifferential_profile_gal = lambda r, M, rv, c: 1. \n\ngalaxy_profile = halo.profile.configuration(k, M, rv, c, differential_profile_gal, amplitude=N_galaxy, normalisation=rho_galaxy, discrete_tracer=True)\n```\nin the discrete tracer case it is important to split up `normalisation` and `amplitude` so that `amplitude` is something that can be interpreted as the mean of a discrete probability distribution. In this example we have also decided to ignore the contribution of the variance in the number of galaxies at fixed halo mass to the eventual power spectrum calculation.\n\nNote that the *covariance* in the mean profile amplitude between two different tracers is not currently supported. This can be important in halo-occupation models where galaxies are split into centrals and satellites and the presence of a satellite galaxy is conditional on the halo first containing a central galaxy. We hope to include this in future. Also any *spatial* variance or covariance in halo profiles at fixed mass is not currently supported; we have no plans to include this in future.\n\n## Notebooks\nThere are several `jupyter` notebooks in the `notebooks/` directory giving examples of how to use the code. The first one to try is `demo-basic.ipynb`, which gives an overview of the main features of `pyhalomodel`. As a bonus, we include notebooks that produce (almost) all of the plots from the review paper.\n\n## Citation\nPlease add a citation to [Asgari, Mead & Heymans (2023)](https://arxiv.org/) if you use this code.\n",
-    'author': 'Alexander Mead',
-    'author_email': 'alexander.j.mead@googlemail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/alexander-mead/pyhalomodel',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.12',
-}
+## Citation
+Please add a citation to [Asgari, Mead & Heymans (2023)](https://arxiv.org/abs/2303.08752) if you use this code.
 
-
-setup(**setup_kwargs)
```

