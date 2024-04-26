# Comparing `tmp/tad_dftd4-0.1.0.tar.gz` & `tmp/tad_dftd4-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tad_dftd4-0.1.0.tar", last modified: Fri Apr 12 09:24:40 2024, max compression
+gzip compressed data, was "tad_dftd4-0.1.1.tar", last modified: Fri Apr 26 07:41:26 2024, max compression
```

## Comparing `tad_dftd4-0.1.0.tar` & `tad_dftd4-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:24:40.183323 tad_dftd4-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-04-12 09:24:40.179323 tad_dftd4-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-12 09:24:40.183323 tad_dftd4-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:24:40.171323 tad_dftd4-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:24:40.175323 tad_dftd4-0.1.0/src/tad_dftd4/
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/cutoff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:24:40.179323 tad_dftd4-0.1.0/src/tad_dftd4/damping/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/damping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/damping/atm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/damping/rational.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:24:40.179323 tad_dftd4-0.1.0/src/tad_dftd4/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/data/hardness.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/data/r4r2.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/data/radii.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/data/zeff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/disp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12836 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:24:40.179323 tad_dftd4-0.1.0/src/tad_dftd4/ncoord/
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/ncoord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   795054 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/params.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:24:40.179323 tad_dftd4-0.1.0/src/tad_dftd4/typing/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/typing/builtin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/typing/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:24:40.179323 tad_dftd4-0.1.0/src/tad_dftd4.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-04-12 09:24:40.000000 tad_dftd4-0.1.0/src/tad_dftd4.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-12 09:24:40.000000 tad_dftd4-0.1.0/src/tad_dftd4.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:24:40.000000 tad_dftd4-0.1.0/src/tad_dftd4.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-12 09:24:40.000000 tad_dftd4-0.1.0/src/tad_dftd4.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 09:24:40.000000 tad_dftd4-0.1.0/src/tad_dftd4.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:41:26.231233 tad_dftd4-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11707 2024-04-26 07:41:26.231233 tad_dftd4-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-26 07:41:26.231233 tad_dftd4-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:41:26.223233 tad_dftd4-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:41:26.227234 tad_dftd4-0.1.1/src/tad_dftd4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/cutoff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:41:26.227234 tad_dftd4-0.1.1/src/tad_dftd4/damping/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/damping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/damping/atm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/damping/rational.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:41:26.227234 tad_dftd4-0.1.1/src/tad_dftd4/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/data/hardness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/data/r4r2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/data/radii.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/data/zeff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/disp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12836 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:41:26.227234 tad_dftd4-0.1.1/src/tad_dftd4/ncoord/
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/ncoord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   795054 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:41:26.227234 tad_dftd4-0.1.1/src/tad_dftd4/typing/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/typing/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-26 07:41:23.000000 tad_dftd4-0.1.1/src/tad_dftd4/typing/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:41:26.227234 tad_dftd4-0.1.1/src/tad_dftd4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11707 2024-04-26 07:41:26.000000 tad_dftd4-0.1.1/src/tad_dftd4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-26 07:41:26.000000 tad_dftd4-0.1.1/src/tad_dftd4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 07:41:26.000000 tad_dftd4-0.1.1/src/tad_dftd4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-26 07:41:26.000000 tad_dftd4-0.1.1/src/tad_dftd4.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 07:41:26.000000 tad_dftd4-0.1.1/src/tad_dftd4.egg-info/top_level.txt
```

### Comparing `tad_dftd4-0.1.0/LICENSE` & `tad_dftd4-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/PKG-INFO` & `tad_dftd4-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tad_dftd4
-Version: 0.1.0
+Version: 0.1.1
 Summary: Torch autodiff DFT-D4 implementation
 Author: "Marvin Friede"
 License: Apache-2.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -56,24 +56,33 @@
     <td>
       <a href="https://github.com/dftd4/tad-dftd4/releases/latest">
         <img src="https://img.shields.io/github/v/release/dftd4/tad-dftd4?color=orange" alt="Release"/>
       </a>
       <a href="https://pypi.org/project/tad-dftd4/">
         <img src="https://img.shields.io/pypi/v/tad-dftd4?color=orange" alt="PyPI"/>
       </a>
+      <a href="https://anaconda.org/conda-forge/tad-dftd4">
+        <img src="https://img.shields.io/conda/vn/conda-forge/tad-dftd4.svg" alt="Conda Version"/>
+      </a>
       <a href="http://www.apache.org/licenses/LICENSE-2.0">
         <img src="https://img.shields.io/badge/License-Apache%202.0-orange.svg" alt="Apache-2.0"/>
       </a>
     </td>
   </tr>
   <tr>
     <td>Status:</td>
     <td>
-      <a href="https://github.com/dftd4/tad-dftd4/actions/workflows/python.yaml">
-        <img src="https://github.com/dftd4/tad-dftd4/actions/workflows/python.yaml/badge.svg" alt="Test Status"/>
+      <a href="https://github.com/dftd4/tad-dftd4/actions/workflows/ubuntu.yaml">
+        <img src="https://github.com/dftd4/tad-dftd4/actions/workflows/ubuntu.yaml/badge.svg" alt="Test Status Ubuntu"/>
+      </a>
+      <a href="https://github.com/dftd4/tad-dftd4/actions/workflows/macos.yaml">
+        <img src="https://github.com/dftd4/tad-dftd4/actions/workflows/macos.yaml/badge.svg" alt="Test Status macOS"/>
+      </a>
+      <a href="https://github.com/dftd4/tad-dftd4/actions/workflows/windows.yaml">
+        <img src="https://github.com/dftd4/tad-dftd4/actions/workflows/windows.yaml/badge.svg" alt="Test Status Windows"/>
       </a>
       <a href="https://github.com/dftd4/tad-dftd4/actions/workflows/release.yaml">
         <img src="https://github.com/dftd4/tad-dftd4/actions/workflows/release.yaml/badge.svg" alt="Build Status"/>
       </a>
       <a href="https://tad-dftd4.readthedocs.io">
         <img src="https://readthedocs.org/projects/tad-dftd4/badge/?version=latest" alt="Documentation Status"/>
       </a>
@@ -108,14 +117,22 @@
 
 *tad-dftd4* can easily be installed with ``pip``.
 
 ```sh
 pip install tad-dftd4
 ```
 
+### conda
+
+*tad-dftd4* is also available from ``conda``.
+
+```sh
+conda install tad-dftd4
+```
+
 ### From source
 
 This project is hosted on GitHub at [dftd4/tad-dftd4](https://github.com/dftd4/tad-dftd4).
 Obtain the source by cloning the repository with
 
 ```sh
 git clone https://github.com/dftd4/tad-dftd4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tad_dftd4 Version: 0.1.0 Summary: Torch autodiff
+Metadata-Version: 2.1 Name: tad_dftd4 Version: 0.1.1 Summary: Torch autodiff
 DFT-D4 implementation Author: "Marvin Friede" License: Apache-2.0 Classifier:
 Framework :: Pytest Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
@@ -17,17 +17,18 @@
 Requires-Dist: pytest-random-order; extra == "dev" Requires-Dist: pytest-xdist;
 extra == "dev" Requires-Dist: tox; extra == "dev" Provides-Extra: tox Requires-
 Dist: covdefaults; extra == "tox" Requires-Dist: pytest; extra == "tox"
 Requires-Dist: pytest-cov; extra == "tox" Requires-Dist: pytest-random-order;
 extra == "tox" Requires-Dist: pytest-xdist; extra == "tox" # Torch Autodiff for
 DFT-D4
 Compatibility: [Python Versions][PyTorch Versions]
-Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_A_p_a_c_h_e_-_2_._0_]
-Status:        _[_T_e_s_t_ _S_t_a_t_u_s_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i
-               _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_]
+Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_C_o_n_d_a_ _V_e_r_s_i_o_n_]_[_A_p_a_c_h_e_-_2_._0_]
+               _[_T_e_s_t_ _S_t_a_t_u_s_ _U_b_u_n_t_u_]_[_T_e_s_t_ _S_t_a_t_u_s_ _m_a_c_O_S_]_[_T_e_s_t_ _S_t_a_t_u_s_ _W_i_n_d_o_w_s_]
+Status:        _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _S_t_a_t_u_s_]
+               _[_C_o_v_e_r_a_g_e_]
 
 Implementation of the DFT-D4 dispersion model in PyTorch. This module allows to
 process a single structure or a batch of structures for the calculation of
 atom-resolved dispersion energies. For details on the D4 dispersion model, see:
 - E. Caldeweyher, C. Bannwarth and S. Grimme, *J. Chem. Phys.*, 2017, 147,
 034112. [DOI: 10.1063/1.4993215](https://dx.doi.org/10.1063/1.4993215) - E.
 Caldeweyher, S. Ehlert, A. Hansen, H. Neugebauer, S. Spicher, C. Bannwarth and
@@ -35,87 +36,89 @@
 //dx.doi.org/10.1063/1.5090222) - E. Caldeweyher, J.-M. Mewes, S. Ehlert and S.
 Grimme, *Phys. Chem. Chem. Phys.*, 2020, 22, 8499-8512. [DOI: 10.1039/
 D0CP00502A](https://doi.org/10.1039/D0CP00502A) For alternative
 implementations, also check out: - [dftd4](https://dftd4.readthedocs.io):
 Implementation of the DFT-D4 dispersion model in Fortran with Python bindings.
 - [cpp-d4](https://github.com/dftd4/cpp-d4): Implementation of the DFT-D4
 dispersion model in C++. ## Installation ### pip *tad-dftd4* can easily be
-installed with ``pip``. ```sh pip install tad-dftd4 ``` ### From source This
-project is hosted on GitHub at [dftd4/tad-dftd4](https://github.com/dftd4/tad-
-dftd4). Obtain the source by cloning the repository with ```sh git clone https:
-//github.com/dftd4/tad-dftd4 cd tad-dftd4 ``` We recommend using a [conda]
-(https://conda.io/) environment to install the package. You can setup the
-environment manager using a [mambaforge](https://github.com/conda-forge/
-miniforge) installer. Install the required dependencies from the conda-forge
-channel. ```sh mamba env create -n torch -f environment.yaml mamba activate
-torch ``` Install this project with ``pip`` in the environment ```sh pip
-install . ``` The following dependencies are required - [numpy](https://
-numpy.org/) - [tad-mctc](https://github.com/tad-mctc/tad-mctc/) - [tad-
-multicharge](https://github.com/tad-mctc/tad-multicharge/) - [torch](https://
-pytorch.org/) - [pytest](https://docs.pytest.org/) (tests only) ## Development
-For development, additionally install the following tools in your environment.
-```sh mamba install black covdefaults mypy pre-commit pylint pytest pytest-cov
-pytest-xdist tox pip install pytest-random-order ``` With pip, add the option
-``-e`` for installing in development mode, and add ``[dev]`` for the
-development dependencies ```sh pip install -e .[dev] ``` The pre-commit hooks
-are initialized by running the following command in the root of the repository.
-```sh pre-commit install ``` For testing all Python environments, simply run
-`tox`. ```sh tox ``` Note that this randomizes the order of tests but skips
-"large" tests. To modify this behavior, `tox` has to skip the optional
-*posargs*. ```sh tox -- test ``` ## Examples The following example shows how to
-calculate the DFT-D4 dispersion energy for a single structure. ```python import
-torch import tad_dftd4 as d4 import tad_mctc as mctc numbers =
-mctc.convert.symbol_to_number(symbols="C C C C N C S H H H H H".split()) #
-coordinates in Bohr positions = torch.tensor( [ [-2.56745685564671, -
-0.02509985979910, 0.00000000000000], [-1.39177582455797, +2.27696188880014,
-0.00000000000000], [+1.27784995624894, +2.45107479759386, 0.00000000000000],
-[+2.62801937615793, +0.25927727028120, 0.00000000000000], [+1.41097033661123, -
-1.99890996077412, 0.00000000000000], [-1.17186102298849, -2.34220576284180,
-0.00000000000000], [-2.39505990368378, -5.22635838332362, 0.00000000000000],
-[+2.41961980455457, -3.62158019253045, 0.00000000000000], [-2.51744374846065,
-+3.98181713686746, 0.00000000000000], [+2.24269048384775, +4.24389473203647,
-0.00000000000000], [+4.66488984573956, +0.17907568006409, 0.00000000000000], [-
-4.60044244782237, -0.17794734637413, 0.00000000000000], ] ) # total charge of
-the system charge = torch.tensor(0.0) # TPSSh-D4-ATM parameters param = { "s6":
+installed with ``pip``. ```sh pip install tad-dftd4 ``` ### conda *tad-dftd4*
+is also available from ``conda``. ```sh conda install tad-dftd4 ``` ### From
+source This project is hosted on GitHub at [dftd4/tad-dftd4](https://
+github.com/dftd4/tad-dftd4). Obtain the source by cloning the repository with
+```sh git clone https://github.com/dftd4/tad-dftd4 cd tad-dftd4 ``` We
+recommend using a [conda](https://conda.io/) environment to install the
+package. You can setup the environment manager using a [mambaforge](https://
+github.com/conda-forge/miniforge) installer. Install the required dependencies
+from the conda-forge channel. ```sh mamba env create -n torch -
+f environment.yaml mamba activate torch ``` Install this project with ``pip``
+in the environment ```sh pip install . ``` The following dependencies are
+required - [numpy](https://numpy.org/) - [tad-mctc](https://github.com/tad-
+mctc/tad-mctc/) - [tad-multicharge](https://github.com/tad-mctc/tad-
+multicharge/) - [torch](https://pytorch.org/) - [pytest](https://
+docs.pytest.org/) (tests only) ## Development For development, additionally
+install the following tools in your environment. ```sh mamba install black
+covdefaults mypy pre-commit pylint pytest pytest-cov pytest-xdist tox pip
+install pytest-random-order ``` With pip, add the option ``-e`` for installing
+in development mode, and add ``[dev]`` for the development dependencies ```sh
+pip install -e .[dev] ``` The pre-commit hooks are initialized by running the
+following command in the root of the repository. ```sh pre-commit install ```
+For testing all Python environments, simply run `tox`. ```sh tox ``` Note that
+this randomizes the order of tests but skips "large" tests. To modify this
+behavior, `tox` has to skip the optional *posargs*. ```sh tox -- test ``` ##
+Examples The following example shows how to calculate the DFT-D4 dispersion
+energy for a single structure. ```python import torch import tad_dftd4 as d4
+import tad_mctc as mctc numbers = mctc.convert.symbol_to_number(symbols="C C C
+C N C S H H H H H".split()) # coordinates in Bohr positions = torch.tensor( [
+[-2.56745685564671, -0.02509985979910, 0.00000000000000], [-1.39177582455797,
++2.27696188880014, 0.00000000000000], [+1.27784995624894, +2.45107479759386,
+0.00000000000000], [+2.62801937615793, +0.25927727028120, 0.00000000000000],
+[+1.41097033661123, -1.99890996077412, 0.00000000000000], [-1.17186102298849, -
+2.34220576284180, 0.00000000000000], [-2.39505990368378, -5.22635838332362,
+0.00000000000000], [+2.41961980455457, -3.62158019253045, 0.00000000000000], [-
+2.51744374846065, +3.98181713686746, 0.00000000000000], [+2.24269048384775,
++4.24389473203647, 0.00000000000000], [+4.66488984573956, +0.17907568006409,
+0.00000000000000], [-4.60044244782237, -0.17794734637413, 0.00000000000000], ]
+) # total charge of the system charge = torch.tensor(0.0) # TPSSh-D4-ATM
+parameters param = { "s6": positions.new_tensor(1.0), "s8":
+positions.new_tensor(1.85897750), "s9": positions.new_tensor(1.0), "a1":
+positions.new_tensor(0.44286966), "a2": positions.new_tensor(4.60230534), }
+energy = d4.dftd4(numbers, positions, charge, param) torch.set_printoptions
+(precision=10) print(energy) # tensor([-0.0020841344, -0.0018971195, -
+0.0018107513, -0.0018305695, # -0.0021737693, -0.0019484236, -0.0022788253, -
+0.0004080658, # -0.0004261866, -0.0004199839, -0.0004280768, -0.0005108935])
+``` The next example shows the calculation of dispersion energies for a batch
+of structures. ```python import torch import tad_dftd4 as d4 import tad_mctc as
+mctc # S22 system 4: formamide dimer numbers = mctc.batch.pack(
+( mctc.convert.symbol_to_number("C C N N H H H H H H O O".split()),
+mctc.convert.symbol_to_number("C O N H H H".split()), )) # coordinates in Bohr
+positions = mctc.batch.pack(( torch.tensor([ [-3.81469488143921,
++0.09993441402912, 0.00000000000000], [+3.81469488143921, -0.09993441402912,
+0.00000000000000], [-2.66030049324036, -2.15898251533508, 0.00000000000000],
+[+2.66030049324036, +2.15898251533508, 0.00000000000000], [-0.73178529739380, -
+2.28237795829773, 0.00000000000000], [-5.89039325714111, -0.02589114569128,
+0.00000000000000], [-3.71254944801331, -3.73605775833130, 0.00000000000000],
+[+3.71254944801331, +3.73605775833130, 0.00000000000000], [+0.73178529739380,
++2.28237795829773, 0.00000000000000], [+5.89039325714111, +0.02589114569128,
+0.00000000000000], [-2.74426102638245, +2.16115570068359, 0.00000000000000],
+[+2.74426102638245, -2.16115570068359, 0.00000000000000], ]), torch.tensor([ [-
+0.55569743203406, +1.09030425468557, 0.00000000000000], [+0.51473634678469,
++3.15152550263611, 0.00000000000000], [+0.59869690244446, -1.16861263789477,
+0.00000000000000], [-0.45355203669134, -2.74568780438064, 0.00000000000000],
+[+2.52721209544999, -1.29200800956867, 0.00000000000000], [-2.63139587595376,
++0.96447869452240, 0.00000000000000], ]), )) # total charge of both system
+charge = torch.tensor([0.0, 0.0]) # TPSSh-D4-ATM parameters param = { "s6":
 positions.new_tensor(1.0), "s8": positions.new_tensor(1.85897750), "s9":
 positions.new_tensor(1.0), "a1": positions.new_tensor(0.44286966), "a2":
-positions.new_tensor(4.60230534), } energy = d4.dftd4(numbers, positions,
-charge, param) torch.set_printoptions(precision=10) print(energy) # tensor([-
-0.0020841344, -0.0018971195, -0.0018107513, -0.0018305695, # -0.0021737693, -
-0.0019484236, -0.0022788253, -0.0004080658, # -0.0004261866, -0.0004199839, -
-0.0004280768, -0.0005108935]) ``` The next example shows the calculation of
-dispersion energies for a batch of structures. ```python import torch import
-tad_dftd4 as d4 import tad_mctc as mctc # S22 system 4: formamide dimer numbers
-= mctc.batch.pack(( mctc.convert.symbol_to_number("C C N N H H H H H H O
-O".split()), mctc.convert.symbol_to_number("C O N H H H".split()), )) #
-coordinates in Bohr positions = mctc.batch.pack(( torch.tensor([ [-
-3.81469488143921, +0.09993441402912, 0.00000000000000], [+3.81469488143921, -
-0.09993441402912, 0.00000000000000], [-2.66030049324036, -2.15898251533508,
-0.00000000000000], [+2.66030049324036, +2.15898251533508, 0.00000000000000], [-
-0.73178529739380, -2.28237795829773, 0.00000000000000], [-5.89039325714111, -
-0.02589114569128, 0.00000000000000], [-3.71254944801331, -3.73605775833130,
-0.00000000000000], [+3.71254944801331, +3.73605775833130, 0.00000000000000],
-[+0.73178529739380, +2.28237795829773, 0.00000000000000], [+5.89039325714111,
-+0.02589114569128, 0.00000000000000], [-2.74426102638245, +2.16115570068359,
-0.00000000000000], [+2.74426102638245, -2.16115570068359, 0.00000000000000],
-]), torch.tensor([ [-0.55569743203406, +1.09030425468557, 0.00000000000000],
-[+0.51473634678469, +3.15152550263611, 0.00000000000000], [+0.59869690244446, -
-1.16861263789477, 0.00000000000000], [-0.45355203669134, -2.74568780438064,
-0.00000000000000], [+2.52721209544999, -1.29200800956867, 0.00000000000000], [-
-2.63139587595376, +0.96447869452240, 0.00000000000000], ]), )) # total charge
-of both system charge = torch.tensor([0.0, 0.0]) # TPSSh-D4-ATM parameters
-param = { "s6": positions.new_tensor(1.0), "s8": positions.new_tensor
-(1.85897750), "s9": positions.new_tensor(1.0), "a1": positions.new_tensor
-(0.44286966), "a2": positions.new_tensor(4.60230534), } # calculate dispersion
-energy in Hartree energy = torch.sum(d4.dftd4(numbers, positions, charge,
-param), -1) torch.set_printoptions(precision=10) print(energy) # tensor([-
-0.0088341432, -0.0027013607]) print(energy[0] - 2*energy[1]) # tensor(-
-0.0034314217) ``` ## Contributing This is a volunteer open source projects and
-contributions are always welcome. Please, take a moment to read the
-[contributing guidelines](CONTRIBUTING.md). ## License This project is licensed
-under the Apache License, Version 2.0 (the "License"); you may not use this
-project's files except in compliance with the License. You may obtain a copy of
-the License at http://www.apache.org/licenses/LICENSE-2.0 Unless required by
-applicable law or agreed to in writing, software distributed under the License
-is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-KIND, either express or implied. See the License for the specific language
-governing permissions and limitations under the License.
+positions.new_tensor(4.60230534), } # calculate dispersion energy in Hartree
+energy = torch.sum(d4.dftd4(numbers, positions, charge, param), -1)
+torch.set_printoptions(precision=10) print(energy) # tensor([-0.0088341432, -
+0.0027013607]) print(energy[0] - 2*energy[1]) # tensor(-0.0034314217) ``` ##
+Contributing This is a volunteer open source projects and contributions are
+always welcome. Please, take a moment to read the [contributing guidelines]
+(CONTRIBUTING.md). ## License This project is licensed under the Apache
+License, Version 2.0 (the "License"); you may not use this project's files
+except in compliance with the License. You may obtain a copy of the License at
+http://www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or
+agreed to in writing, software distributed under the License is distributed on
+an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
+or implied. See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `tad_dftd4-0.1.0/README.md` & `tad_dftd4-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,24 +13,33 @@
     <td>
       <a href="https://github.com/dftd4/tad-dftd4/releases/latest">
         <img src="https://img.shields.io/github/v/release/dftd4/tad-dftd4?color=orange" alt="Release"/>
       </a>
       <a href="https://pypi.org/project/tad-dftd4/">
         <img src="https://img.shields.io/pypi/v/tad-dftd4?color=orange" alt="PyPI"/>
       </a>
+      <a href="https://anaconda.org/conda-forge/tad-dftd4">
+        <img src="https://img.shields.io/conda/vn/conda-forge/tad-dftd4.svg" alt="Conda Version"/>
+      </a>
       <a href="http://www.apache.org/licenses/LICENSE-2.0">
         <img src="https://img.shields.io/badge/License-Apache%202.0-orange.svg" alt="Apache-2.0"/>
       </a>
     </td>
   </tr>
   <tr>
     <td>Status:</td>
     <td>
-      <a href="https://github.com/dftd4/tad-dftd4/actions/workflows/python.yaml">
-        <img src="https://github.com/dftd4/tad-dftd4/actions/workflows/python.yaml/badge.svg" alt="Test Status"/>
+      <a href="https://github.com/dftd4/tad-dftd4/actions/workflows/ubuntu.yaml">
+        <img src="https://github.com/dftd4/tad-dftd4/actions/workflows/ubuntu.yaml/badge.svg" alt="Test Status Ubuntu"/>
+      </a>
+      <a href="https://github.com/dftd4/tad-dftd4/actions/workflows/macos.yaml">
+        <img src="https://github.com/dftd4/tad-dftd4/actions/workflows/macos.yaml/badge.svg" alt="Test Status macOS"/>
+      </a>
+      <a href="https://github.com/dftd4/tad-dftd4/actions/workflows/windows.yaml">
+        <img src="https://github.com/dftd4/tad-dftd4/actions/workflows/windows.yaml/badge.svg" alt="Test Status Windows"/>
       </a>
       <a href="https://github.com/dftd4/tad-dftd4/actions/workflows/release.yaml">
         <img src="https://github.com/dftd4/tad-dftd4/actions/workflows/release.yaml/badge.svg" alt="Build Status"/>
       </a>
       <a href="https://tad-dftd4.readthedocs.io">
         <img src="https://readthedocs.org/projects/tad-dftd4/badge/?version=latest" alt="Documentation Status"/>
       </a>
@@ -65,14 +74,22 @@
 
 *tad-dftd4* can easily be installed with ``pip``.
 
 ```sh
 pip install tad-dftd4
 ```
 
+### conda
+
+*tad-dftd4* is also available from ``conda``.
+
+```sh
+conda install tad-dftd4
+```
+
 ### From source
 
 This project is hosted on GitHub at [dftd4/tad-dftd4](https://github.com/dftd4/tad-dftd4).
 Obtain the source by cloning the repository with
 
 ```sh
 git clone https://github.com/dftd4/tad-dftd4
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
 # Torch Autodiff for DFT-D4
 Compatibility: [Python Versions][PyTorch Versions]
-Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_A_p_a_c_h_e_-_2_._0_]
-Status:        _[_T_e_s_t_ _S_t_a_t_u_s_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i
-               _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_]
+Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_C_o_n_d_a_ _V_e_r_s_i_o_n_]_[_A_p_a_c_h_e_-_2_._0_]
+               _[_T_e_s_t_ _S_t_a_t_u_s_ _U_b_u_n_t_u_]_[_T_e_s_t_ _S_t_a_t_u_s_ _m_a_c_O_S_]_[_T_e_s_t_ _S_t_a_t_u_s_ _W_i_n_d_o_w_s_]
+Status:        _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _S_t_a_t_u_s_]
+               _[_C_o_v_e_r_a_g_e_]
 
 Implementation of the DFT-D4 dispersion model in PyTorch. This module allows to
 process a single structure or a batch of structures for the calculation of
 atom-resolved dispersion energies. For details on the D4 dispersion model, see:
 - E. Caldeweyher, C. Bannwarth and S. Grimme, *J. Chem. Phys.*, 2017, 147,
 034112. [DOI: 10.1063/1.4993215](https://dx.doi.org/10.1063/1.4993215) - E.
 Caldeweyher, S. Ehlert, A. Hansen, H. Neugebauer, S. Spicher, C. Bannwarth and
@@ -14,87 +15,89 @@
 //dx.doi.org/10.1063/1.5090222) - E. Caldeweyher, J.-M. Mewes, S. Ehlert and S.
 Grimme, *Phys. Chem. Chem. Phys.*, 2020, 22, 8499-8512. [DOI: 10.1039/
 D0CP00502A](https://doi.org/10.1039/D0CP00502A) For alternative
 implementations, also check out: - [dftd4](https://dftd4.readthedocs.io):
 Implementation of the DFT-D4 dispersion model in Fortran with Python bindings.
 - [cpp-d4](https://github.com/dftd4/cpp-d4): Implementation of the DFT-D4
 dispersion model in C++. ## Installation ### pip *tad-dftd4* can easily be
-installed with ``pip``. ```sh pip install tad-dftd4 ``` ### From source This
-project is hosted on GitHub at [dftd4/tad-dftd4](https://github.com/dftd4/tad-
-dftd4). Obtain the source by cloning the repository with ```sh git clone https:
-//github.com/dftd4/tad-dftd4 cd tad-dftd4 ``` We recommend using a [conda]
-(https://conda.io/) environment to install the package. You can setup the
-environment manager using a [mambaforge](https://github.com/conda-forge/
-miniforge) installer. Install the required dependencies from the conda-forge
-channel. ```sh mamba env create -n torch -f environment.yaml mamba activate
-torch ``` Install this project with ``pip`` in the environment ```sh pip
-install . ``` The following dependencies are required - [numpy](https://
-numpy.org/) - [tad-mctc](https://github.com/tad-mctc/tad-mctc/) - [tad-
-multicharge](https://github.com/tad-mctc/tad-multicharge/) - [torch](https://
-pytorch.org/) - [pytest](https://docs.pytest.org/) (tests only) ## Development
-For development, additionally install the following tools in your environment.
-```sh mamba install black covdefaults mypy pre-commit pylint pytest pytest-cov
-pytest-xdist tox pip install pytest-random-order ``` With pip, add the option
-``-e`` for installing in development mode, and add ``[dev]`` for the
-development dependencies ```sh pip install -e .[dev] ``` The pre-commit hooks
-are initialized by running the following command in the root of the repository.
-```sh pre-commit install ``` For testing all Python environments, simply run
-`tox`. ```sh tox ``` Note that this randomizes the order of tests but skips
-"large" tests. To modify this behavior, `tox` has to skip the optional
-*posargs*. ```sh tox -- test ``` ## Examples The following example shows how to
-calculate the DFT-D4 dispersion energy for a single structure. ```python import
-torch import tad_dftd4 as d4 import tad_mctc as mctc numbers =
-mctc.convert.symbol_to_number(symbols="C C C C N C S H H H H H".split()) #
-coordinates in Bohr positions = torch.tensor( [ [-2.56745685564671, -
-0.02509985979910, 0.00000000000000], [-1.39177582455797, +2.27696188880014,
-0.00000000000000], [+1.27784995624894, +2.45107479759386, 0.00000000000000],
-[+2.62801937615793, +0.25927727028120, 0.00000000000000], [+1.41097033661123, -
-1.99890996077412, 0.00000000000000], [-1.17186102298849, -2.34220576284180,
-0.00000000000000], [-2.39505990368378, -5.22635838332362, 0.00000000000000],
-[+2.41961980455457, -3.62158019253045, 0.00000000000000], [-2.51744374846065,
-+3.98181713686746, 0.00000000000000], [+2.24269048384775, +4.24389473203647,
-0.00000000000000], [+4.66488984573956, +0.17907568006409, 0.00000000000000], [-
-4.60044244782237, -0.17794734637413, 0.00000000000000], ] ) # total charge of
-the system charge = torch.tensor(0.0) # TPSSh-D4-ATM parameters param = { "s6":
+installed with ``pip``. ```sh pip install tad-dftd4 ``` ### conda *tad-dftd4*
+is also available from ``conda``. ```sh conda install tad-dftd4 ``` ### From
+source This project is hosted on GitHub at [dftd4/tad-dftd4](https://
+github.com/dftd4/tad-dftd4). Obtain the source by cloning the repository with
+```sh git clone https://github.com/dftd4/tad-dftd4 cd tad-dftd4 ``` We
+recommend using a [conda](https://conda.io/) environment to install the
+package. You can setup the environment manager using a [mambaforge](https://
+github.com/conda-forge/miniforge) installer. Install the required dependencies
+from the conda-forge channel. ```sh mamba env create -n torch -
+f environment.yaml mamba activate torch ``` Install this project with ``pip``
+in the environment ```sh pip install . ``` The following dependencies are
+required - [numpy](https://numpy.org/) - [tad-mctc](https://github.com/tad-
+mctc/tad-mctc/) - [tad-multicharge](https://github.com/tad-mctc/tad-
+multicharge/) - [torch](https://pytorch.org/) - [pytest](https://
+docs.pytest.org/) (tests only) ## Development For development, additionally
+install the following tools in your environment. ```sh mamba install black
+covdefaults mypy pre-commit pylint pytest pytest-cov pytest-xdist tox pip
+install pytest-random-order ``` With pip, add the option ``-e`` for installing
+in development mode, and add ``[dev]`` for the development dependencies ```sh
+pip install -e .[dev] ``` The pre-commit hooks are initialized by running the
+following command in the root of the repository. ```sh pre-commit install ```
+For testing all Python environments, simply run `tox`. ```sh tox ``` Note that
+this randomizes the order of tests but skips "large" tests. To modify this
+behavior, `tox` has to skip the optional *posargs*. ```sh tox -- test ``` ##
+Examples The following example shows how to calculate the DFT-D4 dispersion
+energy for a single structure. ```python import torch import tad_dftd4 as d4
+import tad_mctc as mctc numbers = mctc.convert.symbol_to_number(symbols="C C C
+C N C S H H H H H".split()) # coordinates in Bohr positions = torch.tensor( [
+[-2.56745685564671, -0.02509985979910, 0.00000000000000], [-1.39177582455797,
++2.27696188880014, 0.00000000000000], [+1.27784995624894, +2.45107479759386,
+0.00000000000000], [+2.62801937615793, +0.25927727028120, 0.00000000000000],
+[+1.41097033661123, -1.99890996077412, 0.00000000000000], [-1.17186102298849, -
+2.34220576284180, 0.00000000000000], [-2.39505990368378, -5.22635838332362,
+0.00000000000000], [+2.41961980455457, -3.62158019253045, 0.00000000000000], [-
+2.51744374846065, +3.98181713686746, 0.00000000000000], [+2.24269048384775,
++4.24389473203647, 0.00000000000000], [+4.66488984573956, +0.17907568006409,
+0.00000000000000], [-4.60044244782237, -0.17794734637413, 0.00000000000000], ]
+) # total charge of the system charge = torch.tensor(0.0) # TPSSh-D4-ATM
+parameters param = { "s6": positions.new_tensor(1.0), "s8":
+positions.new_tensor(1.85897750), "s9": positions.new_tensor(1.0), "a1":
+positions.new_tensor(0.44286966), "a2": positions.new_tensor(4.60230534), }
+energy = d4.dftd4(numbers, positions, charge, param) torch.set_printoptions
+(precision=10) print(energy) # tensor([-0.0020841344, -0.0018971195, -
+0.0018107513, -0.0018305695, # -0.0021737693, -0.0019484236, -0.0022788253, -
+0.0004080658, # -0.0004261866, -0.0004199839, -0.0004280768, -0.0005108935])
+``` The next example shows the calculation of dispersion energies for a batch
+of structures. ```python import torch import tad_dftd4 as d4 import tad_mctc as
+mctc # S22 system 4: formamide dimer numbers = mctc.batch.pack(
+( mctc.convert.symbol_to_number("C C N N H H H H H H O O".split()),
+mctc.convert.symbol_to_number("C O N H H H".split()), )) # coordinates in Bohr
+positions = mctc.batch.pack(( torch.tensor([ [-3.81469488143921,
++0.09993441402912, 0.00000000000000], [+3.81469488143921, -0.09993441402912,
+0.00000000000000], [-2.66030049324036, -2.15898251533508, 0.00000000000000],
+[+2.66030049324036, +2.15898251533508, 0.00000000000000], [-0.73178529739380, -
+2.28237795829773, 0.00000000000000], [-5.89039325714111, -0.02589114569128,
+0.00000000000000], [-3.71254944801331, -3.73605775833130, 0.00000000000000],
+[+3.71254944801331, +3.73605775833130, 0.00000000000000], [+0.73178529739380,
++2.28237795829773, 0.00000000000000], [+5.89039325714111, +0.02589114569128,
+0.00000000000000], [-2.74426102638245, +2.16115570068359, 0.00000000000000],
+[+2.74426102638245, -2.16115570068359, 0.00000000000000], ]), torch.tensor([ [-
+0.55569743203406, +1.09030425468557, 0.00000000000000], [+0.51473634678469,
++3.15152550263611, 0.00000000000000], [+0.59869690244446, -1.16861263789477,
+0.00000000000000], [-0.45355203669134, -2.74568780438064, 0.00000000000000],
+[+2.52721209544999, -1.29200800956867, 0.00000000000000], [-2.63139587595376,
++0.96447869452240, 0.00000000000000], ]), )) # total charge of both system
+charge = torch.tensor([0.0, 0.0]) # TPSSh-D4-ATM parameters param = { "s6":
 positions.new_tensor(1.0), "s8": positions.new_tensor(1.85897750), "s9":
 positions.new_tensor(1.0), "a1": positions.new_tensor(0.44286966), "a2":
-positions.new_tensor(4.60230534), } energy = d4.dftd4(numbers, positions,
-charge, param) torch.set_printoptions(precision=10) print(energy) # tensor([-
-0.0020841344, -0.0018971195, -0.0018107513, -0.0018305695, # -0.0021737693, -
-0.0019484236, -0.0022788253, -0.0004080658, # -0.0004261866, -0.0004199839, -
-0.0004280768, -0.0005108935]) ``` The next example shows the calculation of
-dispersion energies for a batch of structures. ```python import torch import
-tad_dftd4 as d4 import tad_mctc as mctc # S22 system 4: formamide dimer numbers
-= mctc.batch.pack(( mctc.convert.symbol_to_number("C C N N H H H H H H O
-O".split()), mctc.convert.symbol_to_number("C O N H H H".split()), )) #
-coordinates in Bohr positions = mctc.batch.pack(( torch.tensor([ [-
-3.81469488143921, +0.09993441402912, 0.00000000000000], [+3.81469488143921, -
-0.09993441402912, 0.00000000000000], [-2.66030049324036, -2.15898251533508,
-0.00000000000000], [+2.66030049324036, +2.15898251533508, 0.00000000000000], [-
-0.73178529739380, -2.28237795829773, 0.00000000000000], [-5.89039325714111, -
-0.02589114569128, 0.00000000000000], [-3.71254944801331, -3.73605775833130,
-0.00000000000000], [+3.71254944801331, +3.73605775833130, 0.00000000000000],
-[+0.73178529739380, +2.28237795829773, 0.00000000000000], [+5.89039325714111,
-+0.02589114569128, 0.00000000000000], [-2.74426102638245, +2.16115570068359,
-0.00000000000000], [+2.74426102638245, -2.16115570068359, 0.00000000000000],
-]), torch.tensor([ [-0.55569743203406, +1.09030425468557, 0.00000000000000],
-[+0.51473634678469, +3.15152550263611, 0.00000000000000], [+0.59869690244446, -
-1.16861263789477, 0.00000000000000], [-0.45355203669134, -2.74568780438064,
-0.00000000000000], [+2.52721209544999, -1.29200800956867, 0.00000000000000], [-
-2.63139587595376, +0.96447869452240, 0.00000000000000], ]), )) # total charge
-of both system charge = torch.tensor([0.0, 0.0]) # TPSSh-D4-ATM parameters
-param = { "s6": positions.new_tensor(1.0), "s8": positions.new_tensor
-(1.85897750), "s9": positions.new_tensor(1.0), "a1": positions.new_tensor
-(0.44286966), "a2": positions.new_tensor(4.60230534), } # calculate dispersion
-energy in Hartree energy = torch.sum(d4.dftd4(numbers, positions, charge,
-param), -1) torch.set_printoptions(precision=10) print(energy) # tensor([-
-0.0088341432, -0.0027013607]) print(energy[0] - 2*energy[1]) # tensor(-
-0.0034314217) ``` ## Contributing This is a volunteer open source projects and
-contributions are always welcome. Please, take a moment to read the
-[contributing guidelines](CONTRIBUTING.md). ## License This project is licensed
-under the Apache License, Version 2.0 (the "License"); you may not use this
-project's files except in compliance with the License. You may obtain a copy of
-the License at http://www.apache.org/licenses/LICENSE-2.0 Unless required by
-applicable law or agreed to in writing, software distributed under the License
-is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-KIND, either express or implied. See the License for the specific language
-governing permissions and limitations under the License.
+positions.new_tensor(4.60230534), } # calculate dispersion energy in Hartree
+energy = torch.sum(d4.dftd4(numbers, positions, charge, param), -1)
+torch.set_printoptions(precision=10) print(energy) # tensor([-0.0088341432, -
+0.0027013607]) print(energy[0] - 2*energy[1]) # tensor(-0.0034314217) ``` ##
+Contributing This is a volunteer open source projects and contributions are
+always welcome. Please, take a moment to read the [contributing guidelines]
+(CONTRIBUTING.md). ## License This project is licensed under the Apache
+License, Version 2.0 (the "License"); you may not use this project's files
+except in compliance with the License. You may obtain a copy of the License at
+http://www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or
+agreed to in writing, software distributed under the License is distributed on
+an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
+or implied. See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `tad_dftd4-0.1.0/pyproject.toml` & `tad_dftd4-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/setup.cfg` & `tad_dftd4-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/setup.py` & `tad_dftd4-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/__init__.py` & `tad_dftd4-0.1.1/src/tad_dftd4/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/__version__.py` & `tad_dftd4-0.1.1/src/tad_dftd4/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Module containing the version string.
 """
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/cutoff.py` & `tad_dftd4-0.1.1/src/tad_dftd4/cutoff.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/damping/__init__.py` & `tad_dftd4-0.1.1/src/tad_dftd4/damping/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/damping/atm.py` & `tad_dftd4-0.1.1/src/tad_dftd4/damping/atm.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/damping/rational.py` & `tad_dftd4-0.1.1/src/tad_dftd4/damping/rational.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/data/__init__.py` & `tad_dftd4-0.1.1/src/tad_dftd4/data/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/data/hardness.py` & `tad_dftd4-0.1.1/src/tad_dftd4/data/hardness.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/data/r4r2.py` & `tad_dftd4-0.1.1/src/tad_dftd4/data/r4r2.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/data/radii.py` & `tad_dftd4-0.1.1/src/tad_dftd4/data/radii.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/data/zeff.py` & `tad_dftd4-0.1.1/src/tad_dftd4/data/zeff.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/defaults.py` & `tad_dftd4-0.1.1/src/tad_dftd4/defaults.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/disp.py` & `tad_dftd4-0.1.1/src/tad_dftd4/disp.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/model.py` & `tad_dftd4-0.1.1/src/tad_dftd4/model.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/ncoord/__init__.py` & `tad_dftd4-0.1.1/src/tad_dftd4/ncoord/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/params.py` & `tad_dftd4-0.1.1/src/tad_dftd4/params.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/typing/__init__.py` & `tad_dftd4-0.1.1/src/tad_dftd4/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/typing/builtin.py` & `tad_dftd4-0.1.1/src/tad_dftd4/typing/builtin.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4/typing/pytorch.py` & `tad_dftd4-0.1.1/src/tad_dftd4/typing/pytorch.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4.egg-info/PKG-INFO` & `tad_dftd4-0.1.1/src/tad_dftd4.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tad_dftd4
-Version: 0.1.0
+Version: 0.1.1
 Summary: Torch autodiff DFT-D4 implementation
 Author: "Marvin Friede"
 License: Apache-2.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -56,24 +56,33 @@
     <td>
       <a href="https://github.com/dftd4/tad-dftd4/releases/latest">
         <img src="https://img.shields.io/github/v/release/dftd4/tad-dftd4?color=orange" alt="Release"/>
       </a>
       <a href="https://pypi.org/project/tad-dftd4/">
         <img src="https://img.shields.io/pypi/v/tad-dftd4?color=orange" alt="PyPI"/>
       </a>
+      <a href="https://anaconda.org/conda-forge/tad-dftd4">
+        <img src="https://img.shields.io/conda/vn/conda-forge/tad-dftd4.svg" alt="Conda Version"/>
+      </a>
       <a href="http://www.apache.org/licenses/LICENSE-2.0">
         <img src="https://img.shields.io/badge/License-Apache%202.0-orange.svg" alt="Apache-2.0"/>
       </a>
     </td>
   </tr>
   <tr>
     <td>Status:</td>
     <td>
-      <a href="https://github.com/dftd4/tad-dftd4/actions/workflows/python.yaml">
-        <img src="https://github.com/dftd4/tad-dftd4/actions/workflows/python.yaml/badge.svg" alt="Test Status"/>
+      <a href="https://github.com/dftd4/tad-dftd4/actions/workflows/ubuntu.yaml">
+        <img src="https://github.com/dftd4/tad-dftd4/actions/workflows/ubuntu.yaml/badge.svg" alt="Test Status Ubuntu"/>
+      </a>
+      <a href="https://github.com/dftd4/tad-dftd4/actions/workflows/macos.yaml">
+        <img src="https://github.com/dftd4/tad-dftd4/actions/workflows/macos.yaml/badge.svg" alt="Test Status macOS"/>
+      </a>
+      <a href="https://github.com/dftd4/tad-dftd4/actions/workflows/windows.yaml">
+        <img src="https://github.com/dftd4/tad-dftd4/actions/workflows/windows.yaml/badge.svg" alt="Test Status Windows"/>
       </a>
       <a href="https://github.com/dftd4/tad-dftd4/actions/workflows/release.yaml">
         <img src="https://github.com/dftd4/tad-dftd4/actions/workflows/release.yaml/badge.svg" alt="Build Status"/>
       </a>
       <a href="https://tad-dftd4.readthedocs.io">
         <img src="https://readthedocs.org/projects/tad-dftd4/badge/?version=latest" alt="Documentation Status"/>
       </a>
@@ -108,14 +117,22 @@
 
 *tad-dftd4* can easily be installed with ``pip``.
 
 ```sh
 pip install tad-dftd4
 ```
 
+### conda
+
+*tad-dftd4* is also available from ``conda``.
+
+```sh
+conda install tad-dftd4
+```
+
 ### From source
 
 This project is hosted on GitHub at [dftd4/tad-dftd4](https://github.com/dftd4/tad-dftd4).
 Obtain the source by cloning the repository with
 
 ```sh
 git clone https://github.com/dftd4/tad-dftd4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tad_dftd4 Version: 0.1.0 Summary: Torch autodiff
+Metadata-Version: 2.1 Name: tad_dftd4 Version: 0.1.1 Summary: Torch autodiff
 DFT-D4 implementation Author: "Marvin Friede" License: Apache-2.0 Classifier:
 Framework :: Pytest Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
@@ -17,17 +17,18 @@
 Requires-Dist: pytest-random-order; extra == "dev" Requires-Dist: pytest-xdist;
 extra == "dev" Requires-Dist: tox; extra == "dev" Provides-Extra: tox Requires-
 Dist: covdefaults; extra == "tox" Requires-Dist: pytest; extra == "tox"
 Requires-Dist: pytest-cov; extra == "tox" Requires-Dist: pytest-random-order;
 extra == "tox" Requires-Dist: pytest-xdist; extra == "tox" # Torch Autodiff for
 DFT-D4
 Compatibility: [Python Versions][PyTorch Versions]
-Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_A_p_a_c_h_e_-_2_._0_]
-Status:        _[_T_e_s_t_ _S_t_a_t_u_s_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i
-               _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_]
+Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_C_o_n_d_a_ _V_e_r_s_i_o_n_]_[_A_p_a_c_h_e_-_2_._0_]
+               _[_T_e_s_t_ _S_t_a_t_u_s_ _U_b_u_n_t_u_]_[_T_e_s_t_ _S_t_a_t_u_s_ _m_a_c_O_S_]_[_T_e_s_t_ _S_t_a_t_u_s_ _W_i_n_d_o_w_s_]
+Status:        _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _S_t_a_t_u_s_]
+               _[_C_o_v_e_r_a_g_e_]
 
 Implementation of the DFT-D4 dispersion model in PyTorch. This module allows to
 process a single structure or a batch of structures for the calculation of
 atom-resolved dispersion energies. For details on the D4 dispersion model, see:
 - E. Caldeweyher, C. Bannwarth and S. Grimme, *J. Chem. Phys.*, 2017, 147,
 034112. [DOI: 10.1063/1.4993215](https://dx.doi.org/10.1063/1.4993215) - E.
 Caldeweyher, S. Ehlert, A. Hansen, H. Neugebauer, S. Spicher, C. Bannwarth and
@@ -35,87 +36,89 @@
 //dx.doi.org/10.1063/1.5090222) - E. Caldeweyher, J.-M. Mewes, S. Ehlert and S.
 Grimme, *Phys. Chem. Chem. Phys.*, 2020, 22, 8499-8512. [DOI: 10.1039/
 D0CP00502A](https://doi.org/10.1039/D0CP00502A) For alternative
 implementations, also check out: - [dftd4](https://dftd4.readthedocs.io):
 Implementation of the DFT-D4 dispersion model in Fortran with Python bindings.
 - [cpp-d4](https://github.com/dftd4/cpp-d4): Implementation of the DFT-D4
 dispersion model in C++. ## Installation ### pip *tad-dftd4* can easily be
-installed with ``pip``. ```sh pip install tad-dftd4 ``` ### From source This
-project is hosted on GitHub at [dftd4/tad-dftd4](https://github.com/dftd4/tad-
-dftd4). Obtain the source by cloning the repository with ```sh git clone https:
-//github.com/dftd4/tad-dftd4 cd tad-dftd4 ``` We recommend using a [conda]
-(https://conda.io/) environment to install the package. You can setup the
-environment manager using a [mambaforge](https://github.com/conda-forge/
-miniforge) installer. Install the required dependencies from the conda-forge
-channel. ```sh mamba env create -n torch -f environment.yaml mamba activate
-torch ``` Install this project with ``pip`` in the environment ```sh pip
-install . ``` The following dependencies are required - [numpy](https://
-numpy.org/) - [tad-mctc](https://github.com/tad-mctc/tad-mctc/) - [tad-
-multicharge](https://github.com/tad-mctc/tad-multicharge/) - [torch](https://
-pytorch.org/) - [pytest](https://docs.pytest.org/) (tests only) ## Development
-For development, additionally install the following tools in your environment.
-```sh mamba install black covdefaults mypy pre-commit pylint pytest pytest-cov
-pytest-xdist tox pip install pytest-random-order ``` With pip, add the option
-``-e`` for installing in development mode, and add ``[dev]`` for the
-development dependencies ```sh pip install -e .[dev] ``` The pre-commit hooks
-are initialized by running the following command in the root of the repository.
-```sh pre-commit install ``` For testing all Python environments, simply run
-`tox`. ```sh tox ``` Note that this randomizes the order of tests but skips
-"large" tests. To modify this behavior, `tox` has to skip the optional
-*posargs*. ```sh tox -- test ``` ## Examples The following example shows how to
-calculate the DFT-D4 dispersion energy for a single structure. ```python import
-torch import tad_dftd4 as d4 import tad_mctc as mctc numbers =
-mctc.convert.symbol_to_number(symbols="C C C C N C S H H H H H".split()) #
-coordinates in Bohr positions = torch.tensor( [ [-2.56745685564671, -
-0.02509985979910, 0.00000000000000], [-1.39177582455797, +2.27696188880014,
-0.00000000000000], [+1.27784995624894, +2.45107479759386, 0.00000000000000],
-[+2.62801937615793, +0.25927727028120, 0.00000000000000], [+1.41097033661123, -
-1.99890996077412, 0.00000000000000], [-1.17186102298849, -2.34220576284180,
-0.00000000000000], [-2.39505990368378, -5.22635838332362, 0.00000000000000],
-[+2.41961980455457, -3.62158019253045, 0.00000000000000], [-2.51744374846065,
-+3.98181713686746, 0.00000000000000], [+2.24269048384775, +4.24389473203647,
-0.00000000000000], [+4.66488984573956, +0.17907568006409, 0.00000000000000], [-
-4.60044244782237, -0.17794734637413, 0.00000000000000], ] ) # total charge of
-the system charge = torch.tensor(0.0) # TPSSh-D4-ATM parameters param = { "s6":
+installed with ``pip``. ```sh pip install tad-dftd4 ``` ### conda *tad-dftd4*
+is also available from ``conda``. ```sh conda install tad-dftd4 ``` ### From
+source This project is hosted on GitHub at [dftd4/tad-dftd4](https://
+github.com/dftd4/tad-dftd4). Obtain the source by cloning the repository with
+```sh git clone https://github.com/dftd4/tad-dftd4 cd tad-dftd4 ``` We
+recommend using a [conda](https://conda.io/) environment to install the
+package. You can setup the environment manager using a [mambaforge](https://
+github.com/conda-forge/miniforge) installer. Install the required dependencies
+from the conda-forge channel. ```sh mamba env create -n torch -
+f environment.yaml mamba activate torch ``` Install this project with ``pip``
+in the environment ```sh pip install . ``` The following dependencies are
+required - [numpy](https://numpy.org/) - [tad-mctc](https://github.com/tad-
+mctc/tad-mctc/) - [tad-multicharge](https://github.com/tad-mctc/tad-
+multicharge/) - [torch](https://pytorch.org/) - [pytest](https://
+docs.pytest.org/) (tests only) ## Development For development, additionally
+install the following tools in your environment. ```sh mamba install black
+covdefaults mypy pre-commit pylint pytest pytest-cov pytest-xdist tox pip
+install pytest-random-order ``` With pip, add the option ``-e`` for installing
+in development mode, and add ``[dev]`` for the development dependencies ```sh
+pip install -e .[dev] ``` The pre-commit hooks are initialized by running the
+following command in the root of the repository. ```sh pre-commit install ```
+For testing all Python environments, simply run `tox`. ```sh tox ``` Note that
+this randomizes the order of tests but skips "large" tests. To modify this
+behavior, `tox` has to skip the optional *posargs*. ```sh tox -- test ``` ##
+Examples The following example shows how to calculate the DFT-D4 dispersion
+energy for a single structure. ```python import torch import tad_dftd4 as d4
+import tad_mctc as mctc numbers = mctc.convert.symbol_to_number(symbols="C C C
+C N C S H H H H H".split()) # coordinates in Bohr positions = torch.tensor( [
+[-2.56745685564671, -0.02509985979910, 0.00000000000000], [-1.39177582455797,
++2.27696188880014, 0.00000000000000], [+1.27784995624894, +2.45107479759386,
+0.00000000000000], [+2.62801937615793, +0.25927727028120, 0.00000000000000],
+[+1.41097033661123, -1.99890996077412, 0.00000000000000], [-1.17186102298849, -
+2.34220576284180, 0.00000000000000], [-2.39505990368378, -5.22635838332362,
+0.00000000000000], [+2.41961980455457, -3.62158019253045, 0.00000000000000], [-
+2.51744374846065, +3.98181713686746, 0.00000000000000], [+2.24269048384775,
++4.24389473203647, 0.00000000000000], [+4.66488984573956, +0.17907568006409,
+0.00000000000000], [-4.60044244782237, -0.17794734637413, 0.00000000000000], ]
+) # total charge of the system charge = torch.tensor(0.0) # TPSSh-D4-ATM
+parameters param = { "s6": positions.new_tensor(1.0), "s8":
+positions.new_tensor(1.85897750), "s9": positions.new_tensor(1.0), "a1":
+positions.new_tensor(0.44286966), "a2": positions.new_tensor(4.60230534), }
+energy = d4.dftd4(numbers, positions, charge, param) torch.set_printoptions
+(precision=10) print(energy) # tensor([-0.0020841344, -0.0018971195, -
+0.0018107513, -0.0018305695, # -0.0021737693, -0.0019484236, -0.0022788253, -
+0.0004080658, # -0.0004261866, -0.0004199839, -0.0004280768, -0.0005108935])
+``` The next example shows the calculation of dispersion energies for a batch
+of structures. ```python import torch import tad_dftd4 as d4 import tad_mctc as
+mctc # S22 system 4: formamide dimer numbers = mctc.batch.pack(
+( mctc.convert.symbol_to_number("C C N N H H H H H H O O".split()),
+mctc.convert.symbol_to_number("C O N H H H".split()), )) # coordinates in Bohr
+positions = mctc.batch.pack(( torch.tensor([ [-3.81469488143921,
++0.09993441402912, 0.00000000000000], [+3.81469488143921, -0.09993441402912,
+0.00000000000000], [-2.66030049324036, -2.15898251533508, 0.00000000000000],
+[+2.66030049324036, +2.15898251533508, 0.00000000000000], [-0.73178529739380, -
+2.28237795829773, 0.00000000000000], [-5.89039325714111, -0.02589114569128,
+0.00000000000000], [-3.71254944801331, -3.73605775833130, 0.00000000000000],
+[+3.71254944801331, +3.73605775833130, 0.00000000000000], [+0.73178529739380,
++2.28237795829773, 0.00000000000000], [+5.89039325714111, +0.02589114569128,
+0.00000000000000], [-2.74426102638245, +2.16115570068359, 0.00000000000000],
+[+2.74426102638245, -2.16115570068359, 0.00000000000000], ]), torch.tensor([ [-
+0.55569743203406, +1.09030425468557, 0.00000000000000], [+0.51473634678469,
++3.15152550263611, 0.00000000000000], [+0.59869690244446, -1.16861263789477,
+0.00000000000000], [-0.45355203669134, -2.74568780438064, 0.00000000000000],
+[+2.52721209544999, -1.29200800956867, 0.00000000000000], [-2.63139587595376,
++0.96447869452240, 0.00000000000000], ]), )) # total charge of both system
+charge = torch.tensor([0.0, 0.0]) # TPSSh-D4-ATM parameters param = { "s6":
 positions.new_tensor(1.0), "s8": positions.new_tensor(1.85897750), "s9":
 positions.new_tensor(1.0), "a1": positions.new_tensor(0.44286966), "a2":
-positions.new_tensor(4.60230534), } energy = d4.dftd4(numbers, positions,
-charge, param) torch.set_printoptions(precision=10) print(energy) # tensor([-
-0.0020841344, -0.0018971195, -0.0018107513, -0.0018305695, # -0.0021737693, -
-0.0019484236, -0.0022788253, -0.0004080658, # -0.0004261866, -0.0004199839, -
-0.0004280768, -0.0005108935]) ``` The next example shows the calculation of
-dispersion energies for a batch of structures. ```python import torch import
-tad_dftd4 as d4 import tad_mctc as mctc # S22 system 4: formamide dimer numbers
-= mctc.batch.pack(( mctc.convert.symbol_to_number("C C N N H H H H H H O
-O".split()), mctc.convert.symbol_to_number("C O N H H H".split()), )) #
-coordinates in Bohr positions = mctc.batch.pack(( torch.tensor([ [-
-3.81469488143921, +0.09993441402912, 0.00000000000000], [+3.81469488143921, -
-0.09993441402912, 0.00000000000000], [-2.66030049324036, -2.15898251533508,
-0.00000000000000], [+2.66030049324036, +2.15898251533508, 0.00000000000000], [-
-0.73178529739380, -2.28237795829773, 0.00000000000000], [-5.89039325714111, -
-0.02589114569128, 0.00000000000000], [-3.71254944801331, -3.73605775833130,
-0.00000000000000], [+3.71254944801331, +3.73605775833130, 0.00000000000000],
-[+0.73178529739380, +2.28237795829773, 0.00000000000000], [+5.89039325714111,
-+0.02589114569128, 0.00000000000000], [-2.74426102638245, +2.16115570068359,
-0.00000000000000], [+2.74426102638245, -2.16115570068359, 0.00000000000000],
-]), torch.tensor([ [-0.55569743203406, +1.09030425468557, 0.00000000000000],
-[+0.51473634678469, +3.15152550263611, 0.00000000000000], [+0.59869690244446, -
-1.16861263789477, 0.00000000000000], [-0.45355203669134, -2.74568780438064,
-0.00000000000000], [+2.52721209544999, -1.29200800956867, 0.00000000000000], [-
-2.63139587595376, +0.96447869452240, 0.00000000000000], ]), )) # total charge
-of both system charge = torch.tensor([0.0, 0.0]) # TPSSh-D4-ATM parameters
-param = { "s6": positions.new_tensor(1.0), "s8": positions.new_tensor
-(1.85897750), "s9": positions.new_tensor(1.0), "a1": positions.new_tensor
-(0.44286966), "a2": positions.new_tensor(4.60230534), } # calculate dispersion
-energy in Hartree energy = torch.sum(d4.dftd4(numbers, positions, charge,
-param), -1) torch.set_printoptions(precision=10) print(energy) # tensor([-
-0.0088341432, -0.0027013607]) print(energy[0] - 2*energy[1]) # tensor(-
-0.0034314217) ``` ## Contributing This is a volunteer open source projects and
-contributions are always welcome. Please, take a moment to read the
-[contributing guidelines](CONTRIBUTING.md). ## License This project is licensed
-under the Apache License, Version 2.0 (the "License"); you may not use this
-project's files except in compliance with the License. You may obtain a copy of
-the License at http://www.apache.org/licenses/LICENSE-2.0 Unless required by
-applicable law or agreed to in writing, software distributed under the License
-is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-KIND, either express or implied. See the License for the specific language
-governing permissions and limitations under the License.
+positions.new_tensor(4.60230534), } # calculate dispersion energy in Hartree
+energy = torch.sum(d4.dftd4(numbers, positions, charge, param), -1)
+torch.set_printoptions(precision=10) print(energy) # tensor([-0.0088341432, -
+0.0027013607]) print(energy[0] - 2*energy[1]) # tensor(-0.0034314217) ``` ##
+Contributing This is a volunteer open source projects and contributions are
+always welcome. Please, take a moment to read the [contributing guidelines]
+(CONTRIBUTING.md). ## License This project is licensed under the Apache
+License, Version 2.0 (the "License"); you may not use this project's files
+except in compliance with the License. You may obtain a copy of the License at
+http://www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or
+agreed to in writing, software distributed under the License is distributed on
+an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
+or implied. See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `tad_dftd4-0.1.0/src/tad_dftd4.egg-info/SOURCES.txt` & `tad_dftd4-0.1.1/src/tad_dftd4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

