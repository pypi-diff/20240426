# Comparing `tmp/tad_dftd3-0.2.0.tar.gz` & `tmp/tad_dftd3-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tad_dftd3-0.2.0.tar", last modified: Fri Apr 12 09:28:01 2024, max compression
+gzip compressed data, was "tad_dftd3-0.2.1.tar", last modified: Fri Apr 26 18:44:39 2024, max compression
```

## Comparing `tad_dftd3-0.2.0.tar` & `tad_dftd3-0.2.1.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 09:28:01.055168 tad_dftd3-0.2.0/
--rw-rw-r--   0 friede    (1000) friede    (1000)    11358 2023-05-19 08:14:21.000000 tad_dftd3-0.2.0/LICENSE
--rw-rw-r--   0 friede    (1000) friede    (1000)    11047 2024-04-12 09:28:01.055168 tad_dftd3-0.2.0/PKG-INFO
--rw-rw-r--   0 friede    (1000) friede    (1000)    10167 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/README.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)     1306 2024-01-17 12:28:41.000000 tad_dftd3-0.2.0/pyproject.toml
--rw-rw-r--   0 friede    (1000) friede    (1000)     1324 2024-04-12 09:28:01.059168 tad_dftd3-0.2.0/setup.cfg
--rw-rw-r--   0 friede    (1000) friede    (1000)      679 2023-07-25 07:00:47.000000 tad_dftd3-0.2.0/setup.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 09:28:01.051168 tad_dftd3-0.2.0/src/
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 09:28:01.055168 tad_dftd3-0.2.0/src/tad_dftd3/
--rw-rw-r--   0 friede    (1000) friede    (1000)     3485 2024-03-28 15:55:01.000000 tad_dftd3-0.2.0/src/tad_dftd3/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)      672 2024-04-12 09:27:58.000000 tad_dftd3-0.2.0/src/tad_dftd3/__version__.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 09:28:01.055168 tad_dftd3-0.2.0/src/tad_dftd3/damping/
--rw-rw-r--   0 friede    (1000) friede    (1000)      762 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/damping/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4772 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/damping/atm.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1990 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/damping/rational.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 09:28:01.055168 tad_dftd3-0.2.0/src/tad_dftd3/data/
--rw-rw-r--   0 friede    (1000) friede    (1000)      761 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/data/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2464 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/data/r4r2.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1761 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/data/radii.py
--rw-rw-r--   0 friede    (1000) friede    (1000)    87275 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/data/vdw-d3.pt
--rw-rw-r--   0 friede    (1000) friede    (1000)     1671 2024-03-28 15:55:01.000000 tad_dftd3-0.2.0/src/tad_dftd3/defaults.py
--rw-rw-r--   0 friede    (1000) friede    (1000)    10612 2024-03-28 15:55:01.000000 tad_dftd3-0.2.0/src/tad_dftd3/disp.py
--rw-rw-r--   0 friede    (1000) friede    (1000)      832 2024-03-28 12:03:56.000000 tad_dftd3-0.2.0/src/tad_dftd3/exception.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     7059 2024-03-28 15:55:01.000000 tad_dftd3-0.2.0/src/tad_dftd3/model.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 09:28:01.055168 tad_dftd3-0.2.0/src/tad_dftd3/ncoord/
--rw-rw-r--   0 friede    (1000) friede    (1000)      861 2024-03-28 15:55:01.000000 tad_dftd3-0.2.0/src/tad_dftd3/ncoord/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)        0 2023-07-25 07:00:43.000000 tad_dftd3-0.2.0/src/tad_dftd3/py.typed
--rw-rw-r--   0 friede    (1000) friede    (1000)  4240619 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/reference-c6.pt
--rw-rw-r--   0 friede    (1000) friede    (1000)    15344 2024-03-28 15:55:01.000000 tad_dftd3-0.2.0/src/tad_dftd3/reference.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 09:28:01.055168 tad_dftd3-0.2.0/src/tad_dftd3/typing/
--rw-rw-r--   0 friede    (1000) friede    (1000)      756 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/typing/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)      899 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/typing/builtin.py
--rw-rw-r--   0 friede    (1000) friede    (1000)      822 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/typing/d3.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1075 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/typing/pytorch.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 09:28:01.055168 tad_dftd3-0.2.0/src/tad_dftd3.egg-info/
--rw-r--r--   0 friede    (1000) friede    (1000)    11047 2024-04-12 09:28:00.000000 tad_dftd3-0.2.0/src/tad_dftd3.egg-info/PKG-INFO
--rw-rw-r--   0 friede    (1000) friede    (1000)      838 2024-04-12 09:28:01.000000 tad_dftd3-0.2.0/src/tad_dftd3.egg-info/SOURCES.txt
--rw-rw-r--   0 friede    (1000) friede    (1000)        1 2024-04-12 09:28:00.000000 tad_dftd3-0.2.0/src/tad_dftd3.egg-info/dependency_links.txt
--rw-rw-r--   0 friede    (1000) friede    (1000)      205 2024-04-12 09:28:00.000000 tad_dftd3-0.2.0/src/tad_dftd3.egg-info/requires.txt
--rw-rw-r--   0 friede    (1000) friede    (1000)       10 2024-04-12 09:28:00.000000 tad_dftd3-0.2.0/src/tad_dftd3.egg-info/top_level.txt
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-26 18:44:39.796524 tad_dftd3-0.2.1/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)    11358 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/LICENSE
+-rw-r--r--   0 marvin    (1000) marvin    (1000)    12580 2024-04-26 18:44:39.796524 tad_dftd3-0.2.1/PKG-INFO
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)    11010 2024-04-26 18:44:27.000000 tad_dftd3-0.2.1/README.rst
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1306 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/pyproject.toml
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1312 2024-04-26 18:44:39.796524 tad_dftd3-0.2.1/setup.cfg
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      679 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/setup.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-26 18:44:39.772524 tad_dftd3-0.2.1/src/
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-26 18:44:39.788524 tad_dftd3-0.2.1/src/tad_dftd3/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     3485 2024-04-09 21:13:38.000000 tad_dftd3-0.2.1/src/tad_dftd3/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      672 2024-04-26 18:44:27.000000 tad_dftd3-0.2.1/src/tad_dftd3/__version__.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-26 18:44:39.792524 tad_dftd3-0.2.1/src/tad_dftd3/damping/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      762 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/damping/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     4772 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/damping/atm.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1990 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/damping/rational.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-26 18:44:39.792524 tad_dftd3-0.2.1/src/tad_dftd3/data/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      761 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/data/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2464 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/data/r4r2.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1761 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/data/radii.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)    87275 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/data/vdw-d3.pt
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1671 2024-04-09 21:13:38.000000 tad_dftd3-0.2.1/src/tad_dftd3/defaults.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)    10789 2024-04-26 18:44:27.000000 tad_dftd3-0.2.1/src/tad_dftd3/disp.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      832 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/exception.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-26 18:44:39.796524 tad_dftd3-0.2.1/src/tad_dftd3/model/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1707 2024-04-26 18:44:27.000000 tad_dftd3-0.2.1/src/tad_dftd3/model/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)    12518 2024-04-26 18:44:27.000000 tad_dftd3-0.2.1/src/tad_dftd3/model/c6.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     6070 2024-04-26 18:44:27.000000 tad_dftd3-0.2.1/src/tad_dftd3/model/weights.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-26 18:44:39.796524 tad_dftd3-0.2.1/src/tad_dftd3/ncoord/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      861 2024-04-09 21:13:38.000000 tad_dftd3-0.2.1/src/tad_dftd3/ncoord/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)        0 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/py.typed
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)  4240619 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/reference-c6.pt
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)    15344 2024-04-09 21:13:38.000000 tad_dftd3-0.2.1/src/tad_dftd3/reference.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-26 18:44:39.796524 tad_dftd3-0.2.1/src/tad_dftd3/typing/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      756 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/typing/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      921 2024-04-26 18:44:27.000000 tad_dftd3-0.2.1/src/tad_dftd3/typing/builtin.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      822 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/typing/d3.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1097 2024-04-26 18:44:27.000000 tad_dftd3-0.2.1/src/tad_dftd3/typing/pytorch.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-26 18:44:39.796524 tad_dftd3-0.2.1/src/tad_dftd3.egg-info/
+-rw-r--r--   0 marvin    (1000) marvin    (1000)    12580 2024-04-26 18:44:39.000000 tad_dftd3-0.2.1/src/tad_dftd3.egg-info/PKG-INFO
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      904 2024-04-26 18:44:39.000000 tad_dftd3-0.2.1/src/tad_dftd3.egg-info/SOURCES.txt
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)        1 2024-04-26 18:44:39.000000 tad_dftd3-0.2.1/src/tad_dftd3.egg-info/dependency_links.txt
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      194 2024-04-26 18:44:39.000000 tad_dftd3-0.2.1/src/tad_dftd3.egg-info/requires.txt
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)       10 2024-04-26 18:44:39.000000 tad_dftd3-0.2.1/src/tad_dftd3.egg-info/top_level.txt
```

### Comparing `tad_dftd3-0.2.0/LICENSE` & `tad_dftd3-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.0/PKG-INFO` & `tad_dftd3-0.2.1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,18 @@
-Metadata-Version: 2.1
-Name: tad_dftd3
-Version: 0.2.0
-Summary: Torch autodiff DFT-D3 implementation
-License: Apache-2.0
-Project-URL: Documentation, https://tad-dftd3.readthedocs.io/en/latest/
-Project-URL: Source Code, https://github.com/dftd3/tad-dftd3
-Project-URL: Tracker, https://github.com/dftd3/tad-dftd3/issues
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-Provides-Extra: tox
-License-File: LICENSE
-
 Torch autodiff for DFT-D3
 =========================
 
-.. image:: https://img.shields.io/github/v/release/dftd3/tad-dftd3
-   :target: https://github.com/dftd3/tad-dftd3/releases/latest
-   :alt: Release
-
-.. image:: https://img.shields.io/pypi/v/tad-dftd3
-   :target: https://pypi.org/project/tad-dftd3/
-   :alt: PyPI
-
-.. image:: https://img.shields.io/github/license/dftd3/tad-dftd3
-   :target: LICENSE
-   :alt: Apache-2.0
-
-.. image:: https://github.com/dftd3/tad-dftd3/actions/workflows/python.yaml/badge.svg
-   :target: https://github.com/dftd3/tad-dftd3/actions/workflows/python.yaml
-   :alt: CI
-
-.. image:: https://readthedocs.org/projects/tad-dftd3/badge/?version=latest
-   :target: https://tad-dftd3.readthedocs.io
-   :alt: Documentation Status
-
-.. image:: https://codecov.io/gh/dftd3/tad-dftd3/branch/main/graph/badge.svg?token=D3rMNnl26t
-   :target: https://codecov.io/gh/dftd3/tad-dftd3
-   :alt: Coverage
-
-.. image:: https://results.pre-commit.ci/badge/github/dftd3/tad-dftd3/main.svg
-   :target: https://results.pre-commit.ci/latest/github/dftd3/tad-dftd3/main
-   :alt: pre-commit.ci status
-
+|release|
+|license|
+|testubuntu|
+|testmacos|
+|testwindows|
+|docs|
+|coverage|
+|precommit|
 
 Implementation of the DFT-D3 dispersion model in PyTorch.
 This module allows to process a single structure or a batch of structures for the calculation of atom-resolved dispersion energies.
 
 For details on the D3 dispersion model see
 
 - *J. Chem. Phys.*, **2010**, *132*, 154104 (`DOI <https://dx.doi.org/10.1063/1.3382344>`__)
@@ -74,20 +32,33 @@
 
 Installation
 ------------
 
 pip
 ~~~
 
+|pypi|
+
 The project can easily be installed with ``pip``.
 
 .. code::
 
     pip install tad-dftd3
 
+conda
+~~~~~
+
+|conda|
+
+*tad-dftd3* is also available from ``conda``.
+
+.. code::
+
+    conda install tad-dftd3
+
 From source
 ~~~~~~~~~~~
 
 This project is hosted on GitHub at `dftd3/tad-dftd3 <https://github.com/dftd3/tad-dftd3>`__.
 Obtain the source by cloning the repository with
 
 .. code::
@@ -310,7 +281,48 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 
 Unless you explicitly state otherwise, any contribution intentionally
 submitted for inclusion in this project by you, as defined in the
 Apache-2.0 license, shall be licensed as above, without any additional
 terms or conditions.
+
+
+.. |release| image:: https://img.shields.io/github/v/release/dftd3/tad-dftd3
+   :target: https://github.com/dftd3/tad-dftd3/releases/latest
+   :alt: Release
+
+.. |pypi| image:: https://img.shields.io/pypi/v/tad-dftd3
+   :target: https://pypi.org/project/tad-dftd3/
+   :alt: PyPI
+
+.. |conda| image:: https://img.shields.io/conda/vn/conda-forge/tad-dftd3.svg
+    :target: https://anaconda.org/conda-forge/tad-dftd3
+    :alt: Conda Version
+
+.. |license| image:: https://img.shields.io/github/license/dftd3/tad-dftd3
+   :target: LICENSE
+   :alt: Apache-2.0
+
+.. |testubuntu| image:: https://github.com/dftd3/tad-dftd3/actions/workflows/ubuntu.yaml/badge.svg
+   :target: https://github.com/dftd3/tad-dftd3/actions/workflows/ubuntu.yaml
+   :alt: Tests Ubuntu
+
+.. |testmacos| image:: https://github.com/dftd3/tad-dftd3/actions/workflows/macos.yaml/badge.svg
+   :target: https://github.com/dftd3/tad-dftd3/actions/workflows/macos.yaml
+   :alt: Tests macOS
+
+.. |testwindows| image:: https://github.com/dftd3/tad-dftd3/actions/workflows/windows.yaml/badge.svg
+   :target: https://github.com/dftd3/tad-dftd3/actions/workflows/windows.yaml
+   :alt: Tests Windows
+
+.. |docs| image:: https://readthedocs.org/projects/tad-dftd3/badge/?version=latest
+   :target: https://tad-dftd3.readthedocs.io
+   :alt: Documentation Status
+
+.. |coverage| image:: https://codecov.io/gh/dftd3/tad-dftd3/branch/main/graph/badge.svg?token=D3rMNnl26t
+   :target: https://codecov.io/gh/dftd3/tad-dftd3
+   :alt: Coverage
+
+.. |precommit| image:: https://results.pre-commit.ci/badge/github/dftd3/tad-dftd3/main.svg
+   :target: https://results.pre-commit.ci/latest/github/dftd3/tad-dftd3/main
+   :alt: pre-commit.ci status
```

### Comparing `tad_dftd3-0.2.0/README.rst` & `tad_dftd3-0.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,58 @@
+Metadata-Version: 2.1
+Name: tad_dftd3
+Version: 0.2.1
+Summary: Torch autodiff DFT-D3 implementation
+License: Apache-2.0
+Project-URL: Documentation, https://tad-dftd3.readthedocs.io/en/latest/
+Project-URL: Source Code, https://github.com/dftd3/tad-dftd3
+Project-URL: Tracker, https://github.com/dftd3/tad-dftd3/issues
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: tad-mctc
+Requires-Dist: torch
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: covdefaults; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-random-order; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: tox; extra == "dev"
+Provides-Extra: tox
+Requires-Dist: covdefaults; extra == "tox"
+Requires-Dist: pytest; extra == "tox"
+Requires-Dist: pytest-cov; extra == "tox"
+Requires-Dist: pytest-random-order; extra == "tox"
+Requires-Dist: pytest-xdist; extra == "tox"
+
 Torch autodiff for DFT-D3
 =========================
 
-.. image:: https://img.shields.io/github/v/release/dftd3/tad-dftd3
-   :target: https://github.com/dftd3/tad-dftd3/releases/latest
-   :alt: Release
-
-.. image:: https://img.shields.io/pypi/v/tad-dftd3
-   :target: https://pypi.org/project/tad-dftd3/
-   :alt: PyPI
-
-.. image:: https://img.shields.io/github/license/dftd3/tad-dftd3
-   :target: LICENSE
-   :alt: Apache-2.0
-
-.. image:: https://github.com/dftd3/tad-dftd3/actions/workflows/python.yaml/badge.svg
-   :target: https://github.com/dftd3/tad-dftd3/actions/workflows/python.yaml
-   :alt: CI
-
-.. image:: https://readthedocs.org/projects/tad-dftd3/badge/?version=latest
-   :target: https://tad-dftd3.readthedocs.io
-   :alt: Documentation Status
-
-.. image:: https://codecov.io/gh/dftd3/tad-dftd3/branch/main/graph/badge.svg?token=D3rMNnl26t
-   :target: https://codecov.io/gh/dftd3/tad-dftd3
-   :alt: Coverage
-
-.. image:: https://results.pre-commit.ci/badge/github/dftd3/tad-dftd3/main.svg
-   :target: https://results.pre-commit.ci/latest/github/dftd3/tad-dftd3/main
-   :alt: pre-commit.ci status
-
+|release|
+|license|
+|testubuntu|
+|testmacos|
+|testwindows|
+|docs|
+|coverage|
+|precommit|
 
 Implementation of the DFT-D3 dispersion model in PyTorch.
 This module allows to process a single structure or a batch of structures for the calculation of atom-resolved dispersion energies.
 
 For details on the D3 dispersion model see
 
 - *J. Chem. Phys.*, **2010**, *132*, 154104 (`DOI <https://dx.doi.org/10.1063/1.3382344>`__)
@@ -52,20 +72,33 @@
 
 Installation
 ------------
 
 pip
 ~~~
 
+|pypi|
+
 The project can easily be installed with ``pip``.
 
 .. code::
 
     pip install tad-dftd3
 
+conda
+~~~~~
+
+|conda|
+
+*tad-dftd3* is also available from ``conda``.
+
+.. code::
+
+    conda install tad-dftd3
+
 From source
 ~~~~~~~~~~~
 
 This project is hosted on GitHub at `dftd3/tad-dftd3 <https://github.com/dftd3/tad-dftd3>`__.
 Obtain the source by cloning the repository with
 
 .. code::
@@ -288,7 +321,48 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 
 Unless you explicitly state otherwise, any contribution intentionally
 submitted for inclusion in this project by you, as defined in the
 Apache-2.0 license, shall be licensed as above, without any additional
 terms or conditions.
+
+
+.. |release| image:: https://img.shields.io/github/v/release/dftd3/tad-dftd3
+   :target: https://github.com/dftd3/tad-dftd3/releases/latest
+   :alt: Release
+
+.. |pypi| image:: https://img.shields.io/pypi/v/tad-dftd3
+   :target: https://pypi.org/project/tad-dftd3/
+   :alt: PyPI
+
+.. |conda| image:: https://img.shields.io/conda/vn/conda-forge/tad-dftd3.svg
+    :target: https://anaconda.org/conda-forge/tad-dftd3
+    :alt: Conda Version
+
+.. |license| image:: https://img.shields.io/github/license/dftd3/tad-dftd3
+   :target: LICENSE
+   :alt: Apache-2.0
+
+.. |testubuntu| image:: https://github.com/dftd3/tad-dftd3/actions/workflows/ubuntu.yaml/badge.svg
+   :target: https://github.com/dftd3/tad-dftd3/actions/workflows/ubuntu.yaml
+   :alt: Tests Ubuntu
+
+.. |testmacos| image:: https://github.com/dftd3/tad-dftd3/actions/workflows/macos.yaml/badge.svg
+   :target: https://github.com/dftd3/tad-dftd3/actions/workflows/macos.yaml
+   :alt: Tests macOS
+
+.. |testwindows| image:: https://github.com/dftd3/tad-dftd3/actions/workflows/windows.yaml/badge.svg
+   :target: https://github.com/dftd3/tad-dftd3/actions/workflows/windows.yaml
+   :alt: Tests Windows
+
+.. |docs| image:: https://readthedocs.org/projects/tad-dftd3/badge/?version=latest
+   :target: https://tad-dftd3.readthedocs.io
+   :alt: Documentation Status
+
+.. |coverage| image:: https://codecov.io/gh/dftd3/tad-dftd3/branch/main/graph/badge.svg?token=D3rMNnl26t
+   :target: https://codecov.io/gh/dftd3/tad-dftd3
+   :alt: Coverage
+
+.. |precommit| image:: https://results.pre-commit.ci/badge/github/dftd3/tad-dftd3/main.svg
+   :target: https://results.pre-commit.ci/latest/github/dftd3/tad-dftd3/main
+   :alt: pre-commit.ci status
```

### Comparing `tad_dftd3-0.2.0/pyproject.toml` & `tad_dftd3-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.0/setup.cfg` & `tad_dftd3-0.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 	Source Code = https://github.com/dftd3/tad-dftd3
 	Tracker = https://github.com/dftd3/tad-dftd3/issues
 
 [options]
 packages = find:
 install_requires = 
 	numpy
-	opt-einsum
 	tad-mctc
 	torch
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
```

### Comparing `tad_dftd3-0.2.0/setup.py` & `tad_dftd3-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/__init__.py` & `tad_dftd3-0.2.1/src/tad_dftd3/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/__version__.py` & `tad_dftd3-0.2.1/src/tad_dftd3/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Version module for *tad-dftd3*.
 """
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/damping/__init__.py` & `tad_dftd3-0.2.1/src/tad_dftd3/damping/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/damping/atm.py` & `tad_dftd3-0.2.1/src/tad_dftd3/damping/atm.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/damping/rational.py` & `tad_dftd3-0.2.1/src/tad_dftd3/damping/rational.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/data/__init__.py` & `tad_dftd3-0.2.1/src/tad_dftd3/data/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/data/r4r2.py` & `tad_dftd3-0.2.1/src/tad_dftd3/data/r4r2.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/data/radii.py` & `tad_dftd3-0.2.1/src/tad_dftd3/data/radii.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/data/vdw-d3.pt` & `tad_dftd3-0.2.1/src/tad_dftd3/data/vdw-d3.pt`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/defaults.py` & `tad_dftd3-0.2.1/src/tad_dftd3/defaults.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/disp.py` & `tad_dftd3-0.2.1/src/tad_dftd3/disp.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 >>> weights = d3.model.weight_references(numbers, cn, ref)
 >>> c6 = d3.model.atomic_c6(numbers, weights, ref)
 >>> energy = d3.disp.dispersion(numbers, positions, param, c6)
 >>> torch.set_printoptions(precision=7)
 >>> print(torch.sum(energy[0] - energy[1] - energy[2]))  # energy in Hartree
 tensor(-0.0003964, dtype=torch.float64)
 """
-from typing import Dict, Optional
+from __future__ import annotations
 
 import torch
 from tad_mctc import storch
 from tad_mctc.batch import real_pairs
 from tad_mctc.data import pse
 
 from . import data, defaults, model, ncoord
@@ -73,24 +73,25 @@
 
 __all__ = ["dftd3", "dispersion", "dispersion2", "dispersion3"]
 
 
 def dftd3(
     numbers: Tensor,
     positions: Tensor,
-    param: Dict[str, Tensor],
+    param: dict[str, Tensor],
     *,
-    ref: Optional[Reference] = None,
-    rcov: Optional[Tensor] = None,
-    rvdw: Optional[Tensor] = None,
-    r4r2: Optional[Tensor] = None,
-    cutoff: Optional[Tensor] = None,
+    ref: Reference | None = None,
+    rcov: Tensor | None = None,
+    rvdw: Tensor | None = None,
+    r4r2: Tensor | None = None,
+    cutoff: Tensor | None = None,
     counting_function: CountingFunction = ncoord.exp_count,
     weighting_function: WeightingFunction = model.gaussian_weight,
     damping_function: DampingFunction = rational_damping,
+    chunk_size: int | None = None,
 ) -> Tensor:
     """
     Evaluate DFT-D3 dispersion energy for a batch of geometries.
 
     Parameters
     ----------
     numbers : torch.Tensor
@@ -109,14 +110,17 @@
         r⁴ over r² expectation values of the atoms in the system.
     damping_function : Callable, optional
         Damping function evaluate distance dependent contributions.
     weighting_function : Callable, optional
         Function to calculate weight of individual reference systems.
     counting_function : Callable, optional
         Calculates counting value in range 0 to 1 for each atom pair.
+    chunk_size : int, optional
+        Chunk size for chunked computation of huge tensors that otherwise
+        create memory bottlenecks.
 
     Returns
     -------
     Tensor
         Atom-resolved DFT-D3 dispersion energy for each geometry.
     """
     dd: DD = {"device": positions.device, "dtype": positions.dtype}
@@ -138,15 +142,15 @@
     if r4r2 is None:
         r4r2 = data.R4R2.to(**dd)[numbers]
 
     cn = ncoord.cn_d3(
         numbers, positions, counting_function=counting_function, rcov=rcov
     )
     weights = model.weight_references(numbers, cn, ref, weighting_function)
-    c6 = model.atomic_c6(numbers, weights, ref)
+    c6 = model.atomic_c6(numbers, weights, ref, chunk_size=chunk_size)
 
     return dispersion(
         numbers,
         positions,
         param,
         c6,
         rvdw,
@@ -155,20 +159,20 @@
         cutoff=cutoff,
     )
 
 
 def dispersion(
     numbers: Tensor,
     positions: Tensor,
-    param: Dict[str, Tensor],
+    param: dict[str, Tensor],
     c6: Tensor,
-    rvdw: Optional[Tensor] = None,
-    r4r2: Optional[Tensor] = None,
+    rvdw: Tensor | None = None,
+    r4r2: Tensor | None = None,
     damping_function: DampingFunction = rational_damping,
-    cutoff: Optional[Tensor] = None,
+    cutoff: Tensor | None = None,
     **kwargs: Any,
 ) -> Tensor:
     """
     Calculate dispersion energy between pairs of atoms.
 
     Parameters
     ----------
@@ -206,15 +210,15 @@
         )
     if numbers.shape != r4r2.shape:
         raise ValueError(
             "Shape of expectation values is not consistent with atomic numbers.",
         )
     if torch.max(numbers) >= defaults.MAX_ELEMENT:
         raise ValueError(
-            f"No D3 parameters available for Z > {defaults.MAX_ELEMENT-1} "
+            f"No D3 parameters available for Z > {defaults.MAX_ELEMENT - 1} "
             f"({pse.Z2S[defaults.MAX_ELEMENT]})."
         )
 
     # two-body dispersion
     energy = dispersion2(
         numbers, positions, param, c6, r4r2, damping_function, cutoff, **kwargs
     )
@@ -228,15 +232,15 @@
 
     return energy
 
 
 def dispersion2(
     numbers: Tensor,
     positions: Tensor,
-    param: Dict[str, Tensor],
+    param: dict[str, Tensor],
     c6: Tensor,
     r4r2: Tensor,
     damping_function: DampingFunction,
     cutoff: Tensor,
     **kwargs: Any,
 ) -> Tensor:
     """
@@ -288,15 +292,15 @@
     s8 = param.get("s8", torch.tensor(defaults.S8, **dd))
     return s6 * e6 + s8 * e8
 
 
 def dispersion3(
     numbers: Tensor,
     positions: Tensor,
-    param: Dict[str, Tensor],
+    param: dict[str, Tensor],
     c6: Tensor,
     rvdw: Tensor,
     cutoff: Tensor,
     rs9: Tensor = torch.tensor(4.0 / 3.0),
 ) -> Tensor:
     """
     Three-body dispersion term. Currently this is only a wrapper for the
```

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/exception.py` & `tad_dftd3-0.2.1/src/tad_dftd3/exception.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/model.py` & `tad_dftd3-0.2.1/src/tad_dftd3/model/weights.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,58 +36,23 @@
 >>> c6 = d3.model.atomic_c6(numbers, weights, ref)
 >>> torch.set_printoptions(precision=7)
 >>> print(c6)
 tensor([[10.4130471,  5.4368822,  5.4368822],
         [ 5.4368822,  3.0930154,  3.0930154],
         [ 5.4368822,  3.0930154,  3.0930154]], dtype=torch.float64)
 """
-import torch
-from tad_mctc.math import einsum
-
-from .reference import Reference
-from .typing import Any, Tensor, WeightingFunction
-
-__all__ = ["atomic_c6", "gaussian_weight", "weight_references"]
-
-
-def atomic_c6(numbers: Tensor, weights: Tensor, reference: Reference) -> Tensor:
-    """
-    Calculate atomic dispersion coefficients.
+from __future__ import annotations
 
-    Parameters
-    ----------
-    numbers : Tensor
-        The atomic numbers of the atoms in the system of shape `(..., nat)`.
-    weights : Tensor
-        Weights of all reference systems of shape `(..., nat, 7)`.
-    reference : Reference
-        Reference systems for D3 model. Contains the reference C6 coefficients
-        of shape `(..., nelements, nelements, 7, 7)`.
-
-    Returns
-    -------
-    Tensor
-        Atomic dispersion coefficients of shape `(..., nat, nat)`.
-    """
-    # (..., nel, nel, 7, 7) -> (..., nat, nat, 7, 7)
-    rc6 = reference.c6[numbers.unsqueeze(-1), numbers.unsqueeze(-2)]
+import torch
+from tad_mctc import storch
 
-    # The default einsum path is fastest if the large tensors comes first.
-    # (..., n1, n2, r1, r2) * (..., n1, r1) * (..., n2, r2) -> (..., n1, n2)
-    return einsum(
-        "...ijab,...ia,...jb->...ij",
-        *(rc6, weights, weights),
-        optimize=[(0, 1), (0, 1)],
-    )
+from ..reference import Reference
+from ..typing import Any, Tensor, WeightingFunction
 
-    # NOTE: This old version creates large intermediate tensors and builds the
-    # full matrix before the sum reduction, which requires a lot of memory.
-    #
-    # gw = w.unsqueeze(-1).unsqueeze(-3) * w.unsqueeze(-2).unsqueeze(-4)
-    # c6 = torch.sum(torch.sum(torch.mul(gw, rc6), dim=-1), dim=-1)
+__all__ = ["gaussian_weight", "weight_references"]
 
 
 def gaussian_weight(dcn: Tensor, factor: float = 4.0) -> Tensor:
     """
     Calculate weight of indivdual reference system.
 
     Parameters
@@ -161,37 +126,43 @@
     # such small values can lead to relatively large deviations because the
     # small value is not added to the weights, and hence, the case where
     # `weights` and `norms` are equal does not yield one anymore. In fact, the
     # test suite fails because some elements deviate up to around 1e-4.
     # We solve this by running in double precision, adding a very small number
     # and using multiple masks.
 
+    small = torch.tensor(1e-300, device=cn.device, dtype=torch.double)
+
     # normalize weights
     norm = torch.where(
         mask,
         torch.sum(weights, dim=-1, keepdim=True),
-        torch.tensor(1e-300, device=cn.device, dtype=torch.double),  # double!
+        small,  # double!
     )
 
     # back to real dtype
-    gw_temp = (weights / norm).type(cn.dtype)
+    gw_temp = storch.divide(weights, norm, eps=small).type(cn.dtype)
+    assert torch.isnan(gw_temp).sum() == 0
 
     # The following section handles cases with large CNs that lead to zeros in
     # after the exponential in the weighting function. If this happens all
     # weights become zero, which is not desired. Instead, we set the weight of
     # the largest reference number to one.
     # This case can occur if the CN of the current (actual) system is too far
     # away from the largest CN of the reference systems. An example would be an
     # atom within a fullerene (La3N@C80).
 
     # maximum reference CN for each atom
     maxcn = torch.max(refcn, dim=-1, keepdim=True)[0]
 
-    # prevent division by 0 and small values
-    exceptional = (torch.isnan(gw_temp)) | (gw_temp > torch.finfo(cn.dtype).max)
+    # Here, we catch the potential NaN's from `gw_temp`. We cannot use `gw_temp`
+    # directly, because we have to use safe divide to not get NaN's in the
+    # backward. But `norm == 0` is equivalent. Additionally, we catch very
+    # large values occuring because of division by small values.
+    exceptional = (norm == 0) | (gw_temp > torch.finfo(cn.dtype).max)
 
     gw = torch.where(
         exceptional,
         torch.where(refcn == maxcn, one, zero),
         gw_temp,
     )
```

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/ncoord/__init__.py` & `tad_dftd3-0.2.1/src/tad_dftd3/ncoord/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/reference-c6.pt` & `tad_dftd3-0.2.1/src/tad_dftd3/reference-c6.pt`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/reference.py` & `tad_dftd3-0.2.1/src/tad_dftd3/reference.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/typing/__init__.py` & `tad_dftd3-0.2.1/src/tad_dftd3/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/typing/builtin.py` & `tad_dftd3-0.2.1/src/tad_dftd3/typing/builtin.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,10 +15,10 @@
 """
 Type annotations: Built-ins
 ===========================
 
 Built-in type annotations are imported from the *tad-mctc* library, which
 handles some version checking.
 """
-from tad_mctc.typing import Any, Callable, NoReturn, TypedDict
+from tad_mctc.typing import Any, Callable, NoReturn, Protocol, TypedDict
 
-__all__ = ["Any", "Callable", "NoReturn", "TypedDict"]
+__all__ = ["Any", "Callable", "NoReturn", "Protocol", "TypedDict"]
```

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/typing/d3.py` & `tad_dftd3-0.2.1/src/tad_dftd3/typing/d3.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3/typing/pytorch.py` & `tad_dftd3-0.2.1/src/tad_dftd3/typing/pytorch.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,23 +19,25 @@
 PyTorch-related type annotations for this project.
 """
 from tad_mctc.typing import (
     DD,
     CountingFunction,
     DampingFunction,
     Molecule,
+    Size,
     Tensor,
     TensorOrTensors,
     get_default_device,
     get_default_dtype,
 )
 
 __all__ = [
     "DD",
     "CountingFunction",
     "DampingFunction",
     "Molecule",
+    "Size",
     "Tensor",
     "TensorOrTensors",
     "get_default_device",
     "get_default_dtype",
 ]
```

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3.egg-info/PKG-INFO` & `tad_dftd3-0.2.1/src/tad_dftd3.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tad-dftd3
-Version: 0.2.0
+Name: tad_dftd3
+Version: 0.2.1
 Summary: Torch autodiff DFT-D3 implementation
 License: Apache-2.0
 Project-URL: Documentation, https://tad-dftd3.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/dftd3/tad-dftd3
 Project-URL: Tracker, https://github.com/dftd3/tad-dftd3/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -12,49 +12,47 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: tad-mctc
+Requires-Dist: torch
 Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: covdefaults; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-random-order; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: tox; extra == "dev"
 Provides-Extra: tox
-License-File: LICENSE
+Requires-Dist: covdefaults; extra == "tox"
+Requires-Dist: pytest; extra == "tox"
+Requires-Dist: pytest-cov; extra == "tox"
+Requires-Dist: pytest-random-order; extra == "tox"
+Requires-Dist: pytest-xdist; extra == "tox"
 
 Torch autodiff for DFT-D3
 =========================
 
-.. image:: https://img.shields.io/github/v/release/dftd3/tad-dftd3
-   :target: https://github.com/dftd3/tad-dftd3/releases/latest
-   :alt: Release
-
-.. image:: https://img.shields.io/pypi/v/tad-dftd3
-   :target: https://pypi.org/project/tad-dftd3/
-   :alt: PyPI
-
-.. image:: https://img.shields.io/github/license/dftd3/tad-dftd3
-   :target: LICENSE
-   :alt: Apache-2.0
-
-.. image:: https://github.com/dftd3/tad-dftd3/actions/workflows/python.yaml/badge.svg
-   :target: https://github.com/dftd3/tad-dftd3/actions/workflows/python.yaml
-   :alt: CI
-
-.. image:: https://readthedocs.org/projects/tad-dftd3/badge/?version=latest
-   :target: https://tad-dftd3.readthedocs.io
-   :alt: Documentation Status
-
-.. image:: https://codecov.io/gh/dftd3/tad-dftd3/branch/main/graph/badge.svg?token=D3rMNnl26t
-   :target: https://codecov.io/gh/dftd3/tad-dftd3
-   :alt: Coverage
-
-.. image:: https://results.pre-commit.ci/badge/github/dftd3/tad-dftd3/main.svg
-   :target: https://results.pre-commit.ci/latest/github/dftd3/tad-dftd3/main
-   :alt: pre-commit.ci status
-
+|release|
+|license|
+|testubuntu|
+|testmacos|
+|testwindows|
+|docs|
+|coverage|
+|precommit|
 
 Implementation of the DFT-D3 dispersion model in PyTorch.
 This module allows to process a single structure or a batch of structures for the calculation of atom-resolved dispersion energies.
 
 For details on the D3 dispersion model see
 
 - *J. Chem. Phys.*, **2010**, *132*, 154104 (`DOI <https://dx.doi.org/10.1063/1.3382344>`__)
@@ -74,20 +72,33 @@
 
 Installation
 ------------
 
 pip
 ~~~
 
+|pypi|
+
 The project can easily be installed with ``pip``.
 
 .. code::
 
     pip install tad-dftd3
 
+conda
+~~~~~
+
+|conda|
+
+*tad-dftd3* is also available from ``conda``.
+
+.. code::
+
+    conda install tad-dftd3
+
 From source
 ~~~~~~~~~~~
 
 This project is hosted on GitHub at `dftd3/tad-dftd3 <https://github.com/dftd3/tad-dftd3>`__.
 Obtain the source by cloning the repository with
 
 .. code::
@@ -310,7 +321,48 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 
 Unless you explicitly state otherwise, any contribution intentionally
 submitted for inclusion in this project by you, as defined in the
 Apache-2.0 license, shall be licensed as above, without any additional
 terms or conditions.
+
+
+.. |release| image:: https://img.shields.io/github/v/release/dftd3/tad-dftd3
+   :target: https://github.com/dftd3/tad-dftd3/releases/latest
+   :alt: Release
+
+.. |pypi| image:: https://img.shields.io/pypi/v/tad-dftd3
+   :target: https://pypi.org/project/tad-dftd3/
+   :alt: PyPI
+
+.. |conda| image:: https://img.shields.io/conda/vn/conda-forge/tad-dftd3.svg
+    :target: https://anaconda.org/conda-forge/tad-dftd3
+    :alt: Conda Version
+
+.. |license| image:: https://img.shields.io/github/license/dftd3/tad-dftd3
+   :target: LICENSE
+   :alt: Apache-2.0
+
+.. |testubuntu| image:: https://github.com/dftd3/tad-dftd3/actions/workflows/ubuntu.yaml/badge.svg
+   :target: https://github.com/dftd3/tad-dftd3/actions/workflows/ubuntu.yaml
+   :alt: Tests Ubuntu
+
+.. |testmacos| image:: https://github.com/dftd3/tad-dftd3/actions/workflows/macos.yaml/badge.svg
+   :target: https://github.com/dftd3/tad-dftd3/actions/workflows/macos.yaml
+   :alt: Tests macOS
+
+.. |testwindows| image:: https://github.com/dftd3/tad-dftd3/actions/workflows/windows.yaml/badge.svg
+   :target: https://github.com/dftd3/tad-dftd3/actions/workflows/windows.yaml
+   :alt: Tests Windows
+
+.. |docs| image:: https://readthedocs.org/projects/tad-dftd3/badge/?version=latest
+   :target: https://tad-dftd3.readthedocs.io
+   :alt: Documentation Status
+
+.. |coverage| image:: https://codecov.io/gh/dftd3/tad-dftd3/branch/main/graph/badge.svg?token=D3rMNnl26t
+   :target: https://codecov.io/gh/dftd3/tad-dftd3
+   :alt: Coverage
+
+.. |precommit| image:: https://results.pre-commit.ci/badge/github/dftd3/tad-dftd3/main.svg
+   :target: https://results.pre-commit.ci/latest/github/dftd3/tad-dftd3/main
+   :alt: pre-commit.ci status
```

### Comparing `tad_dftd3-0.2.0/src/tad_dftd3.egg-info/SOURCES.txt` & `tad_dftd3-0.2.1/src/tad_dftd3.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 setup.cfg
 setup.py
 src/tad_dftd3/__init__.py
 src/tad_dftd3/__version__.py
 src/tad_dftd3/defaults.py
 src/tad_dftd3/disp.py
 src/tad_dftd3/exception.py
-src/tad_dftd3/model.py
 src/tad_dftd3/py.typed
 src/tad_dftd3/reference-c6.pt
 src/tad_dftd3/reference.py
 src/tad_dftd3.egg-info/PKG-INFO
 src/tad_dftd3.egg-info/SOURCES.txt
 src/tad_dftd3.egg-info/dependency_links.txt
 src/tad_dftd3.egg-info/requires.txt
@@ -20,12 +19,15 @@
 src/tad_dftd3/damping/__init__.py
 src/tad_dftd3/damping/atm.py
 src/tad_dftd3/damping/rational.py
 src/tad_dftd3/data/__init__.py
 src/tad_dftd3/data/r4r2.py
 src/tad_dftd3/data/radii.py
 src/tad_dftd3/data/vdw-d3.pt
+src/tad_dftd3/model/__init__.py
+src/tad_dftd3/model/c6.py
+src/tad_dftd3/model/weights.py
 src/tad_dftd3/ncoord/__init__.py
 src/tad_dftd3/typing/__init__.py
 src/tad_dftd3/typing/builtin.py
 src/tad_dftd3/typing/d3.py
 src/tad_dftd3/typing/pytorch.py
```

