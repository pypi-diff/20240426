# Comparing `tmp/acdc_py-1.0.1.tar.gz` & `tmp/acdc_py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acdc_py-1.0.1.tar", last modified: Wed Apr 17 04:46:06 2024, max compression
+gzip compressed data, was "acdc_py-1.0.2.tar", last modified: Fri Apr 26 14:27:44 2024, max compression
```

## Comparing `acdc_py-1.0.1.tar` & `acdc_py-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 lucazanella7   (501) staff       (20)        0 2024-04-17 04:46:06.223822 acdc_py-1.0.1/
--rw-r--r--   0 lucazanella7   (501) staff       (20)     1069 2024-04-17 03:06:13.000000 acdc_py-1.0.1/LICENSE
--rw-r--r--   0 lucazanella7   (501) staff       (20)      885 2024-04-17 04:46:06.223668 acdc_py-1.0.1/PKG-INFO
--rw-r--r--   0 lucazanella7   (501) staff       (20)     3175 2024-04-17 03:47:32.000000 acdc_py-1.0.1/README.md
-drwxr-xr-x   0 lucazanella7   (501) staff       (20)        0 2024-04-17 04:46:06.222575 acdc_py-1.0.1/acdc_py/
--rw-r--r--   0 lucazanella7   (501) staff       (20)    15324 2024-04-17 03:06:13.000000 acdc_py-1.0.1/acdc_py/GS.py
--rw-r--r--   0 lucazanella7   (501) staff       (20)    15660 2024-04-17 03:06:13.000000 acdc_py-1.0.1/acdc_py/SA.py
--rw-r--r--   0 lucazanella7   (501) staff       (20)     9021 2024-04-17 03:06:13.000000 acdc_py-1.0.1/acdc_py/_SA_GS_subfunctions.py
--rw-r--r--   0 lucazanella7   (501) staff       (20)      251 2024-04-17 03:06:13.000000 acdc_py-1.0.1/acdc_py/__init__.py
--rw-r--r--   0 lucazanella7   (501) staff       (20)    14854 2024-04-17 03:06:13.000000 acdc_py-1.0.1/acdc_py/_condense_diffuse_funcs.py
--rw-r--r--   0 lucazanella7   (501) staff       (20)     8528 2024-04-17 03:06:13.000000 acdc_py-1.0.1/acdc_py/_diffuse_correction_funcs.py
--rw-r--r--   0 lucazanella7   (501) staff       (20)    14444 2024-04-17 03:06:13.000000 acdc_py-1.0.1/acdc_py/_dual_annealing_with_progress_bar.py
--rw-r--r--   0 lucazanella7   (501) staff       (20)     7374 2024-04-17 03:06:13.000000 acdc_py-1.0.1/acdc_py/_get_opt.py
--rw-r--r--   0 lucazanella7   (501) staff       (20)     5890 2024-04-17 03:06:13.000000 acdc_py-1.0.1/acdc_py/_pl.py
--rw-r--r--   0 lucazanella7   (501) staff       (20)     6919 2024-04-17 03:06:13.000000 acdc_py-1.0.1/acdc_py/_pp.py
--rw-r--r--   0 lucazanella7   (501) staff       (20)     3555 2024-04-17 03:06:13.000000 acdc_py-1.0.1/acdc_py/_tl.py
--rw-r--r--   0 lucazanella7   (501) staff       (20)    15107 2024-04-17 03:06:13.000000 acdc_py-1.0.1/acdc_py/get_opt.py
--rw-r--r--   0 lucazanella7   (501) staff       (20)     1711 2024-04-17 03:06:13.000000 acdc_py-1.0.1/acdc_py/pl.py
--rw-r--r--   0 lucazanella7   (501) staff       (20)     4831 2024-04-17 03:06:13.000000 acdc_py-1.0.1/acdc_py/pp.py
--rw-r--r--   0 lucazanella7   (501) staff       (20)     3293 2024-04-17 03:06:13.000000 acdc_py-1.0.1/acdc_py/tl.py
-drwxr-xr-x   0 lucazanella7   (501) staff       (20)        0 2024-04-17 04:46:06.223480 acdc_py-1.0.1/acdc_py.egg-info/
--rw-r--r--   0 lucazanella7   (501) staff       (20)      885 2024-04-17 04:46:06.000000 acdc_py-1.0.1/acdc_py.egg-info/PKG-INFO
--rw-r--r--   0 lucazanella7   (501) staff       (20)      502 2024-04-17 04:46:06.000000 acdc_py-1.0.1/acdc_py.egg-info/SOURCES.txt
--rw-r--r--   0 lucazanella7   (501) staff       (20)        1 2024-04-17 04:46:06.000000 acdc_py-1.0.1/acdc_py.egg-info/dependency_links.txt
--rw-r--r--   0 lucazanella7   (501) staff       (20)       97 2024-04-17 04:46:06.000000 acdc_py-1.0.1/acdc_py.egg-info/requires.txt
--rw-r--r--   0 lucazanella7   (501) staff       (20)        8 2024-04-17 04:46:06.000000 acdc_py-1.0.1/acdc_py.egg-info/top_level.txt
--rw-r--r--   0 lucazanella7   (501) staff       (20)       38 2024-04-17 04:46:06.223869 acdc_py-1.0.1/setup.cfg
--rw-r--r--   0 lucazanella7   (501) staff       (20)     1307 2024-04-17 04:38:54.000000 acdc_py-1.0.1/setup.py
+drwxr-xr-x   0 lucazanella7   (501) staff       (20)        0 2024-04-26 14:27:44.984808 acdc_py-1.0.2/
+-rw-r--r--   0 lucazanella7   (501) staff       (20)     1069 2024-04-17 03:06:13.000000 acdc_py-1.0.2/LICENSE
+-rw-r--r--   0 lucazanella7   (501) staff       (20)     4117 2024-04-26 14:27:44.984668 acdc_py-1.0.2/PKG-INFO
+-rw-r--r--   0 lucazanella7   (501) staff       (20)     3574 2024-04-26 14:27:12.000000 acdc_py-1.0.2/README.md
+drwxr-xr-x   0 lucazanella7   (501) staff       (20)        0 2024-04-26 14:27:44.983584 acdc_py-1.0.2/acdc_py/
+-rw-r--r--   0 lucazanella7   (501) staff       (20)    15324 2024-04-17 03:06:13.000000 acdc_py-1.0.2/acdc_py/GS.py
+-rw-r--r--   0 lucazanella7   (501) staff       (20)    15660 2024-04-17 03:06:13.000000 acdc_py-1.0.2/acdc_py/SA.py
+-rw-r--r--   0 lucazanella7   (501) staff       (20)     9021 2024-04-17 03:06:13.000000 acdc_py-1.0.2/acdc_py/_SA_GS_subfunctions.py
+-rw-r--r--   0 lucazanella7   (501) staff       (20)      251 2024-04-17 03:06:13.000000 acdc_py-1.0.2/acdc_py/__init__.py
+-rw-r--r--   0 lucazanella7   (501) staff       (20)    14854 2024-04-17 03:06:13.000000 acdc_py-1.0.2/acdc_py/_condense_diffuse_funcs.py
+-rw-r--r--   0 lucazanella7   (501) staff       (20)     8528 2024-04-17 03:06:13.000000 acdc_py-1.0.2/acdc_py/_diffuse_correction_funcs.py
+-rw-r--r--   0 lucazanella7   (501) staff       (20)    14444 2024-04-17 03:06:13.000000 acdc_py-1.0.2/acdc_py/_dual_annealing_with_progress_bar.py
+-rw-r--r--   0 lucazanella7   (501) staff       (20)     7374 2024-04-17 03:06:13.000000 acdc_py-1.0.2/acdc_py/_get_opt.py
+-rw-r--r--   0 lucazanella7   (501) staff       (20)     5890 2024-04-17 03:06:13.000000 acdc_py-1.0.2/acdc_py/_pl.py
+-rw-r--r--   0 lucazanella7   (501) staff       (20)     6919 2024-04-17 03:06:13.000000 acdc_py-1.0.2/acdc_py/_pp.py
+-rw-r--r--   0 lucazanella7   (501) staff       (20)     3555 2024-04-17 03:06:13.000000 acdc_py-1.0.2/acdc_py/_tl.py
+-rw-r--r--   0 lucazanella7   (501) staff       (20)    15107 2024-04-17 03:06:13.000000 acdc_py-1.0.2/acdc_py/get_opt.py
+-rw-r--r--   0 lucazanella7   (501) staff       (20)     1711 2024-04-17 03:06:13.000000 acdc_py-1.0.2/acdc_py/pl.py
+-rw-r--r--   0 lucazanella7   (501) staff       (20)     4831 2024-04-17 03:06:13.000000 acdc_py-1.0.2/acdc_py/pp.py
+-rw-r--r--   0 lucazanella7   (501) staff       (20)     3293 2024-04-17 03:06:13.000000 acdc_py-1.0.2/acdc_py/tl.py
+drwxr-xr-x   0 lucazanella7   (501) staff       (20)        0 2024-04-26 14:27:44.984407 acdc_py-1.0.2/acdc_py.egg-info/
+-rw-r--r--   0 lucazanella7   (501) staff       (20)     4117 2024-04-26 14:27:44.000000 acdc_py-1.0.2/acdc_py.egg-info/PKG-INFO
+-rw-r--r--   0 lucazanella7   (501) staff       (20)      502 2024-04-26 14:27:44.000000 acdc_py-1.0.2/acdc_py.egg-info/SOURCES.txt
+-rw-r--r--   0 lucazanella7   (501) staff       (20)        1 2024-04-26 14:27:44.000000 acdc_py-1.0.2/acdc_py.egg-info/dependency_links.txt
+-rw-r--r--   0 lucazanella7   (501) staff       (20)       97 2024-04-26 14:27:44.000000 acdc_py-1.0.2/acdc_py.egg-info/requires.txt
+-rw-r--r--   0 lucazanella7   (501) staff       (20)        8 2024-04-26 14:27:44.000000 acdc_py-1.0.2/acdc_py.egg-info/top_level.txt
+-rw-r--r--   0 lucazanella7   (501) staff       (20)       38 2024-04-26 14:27:44.984854 acdc_py-1.0.2/setup.cfg
+-rw-r--r--   0 lucazanella7   (501) staff       (20)     1705 2024-04-26 14:23:27.000000 acdc_py-1.0.2/setup.py
```

### Comparing `acdc_py-1.0.1/LICENSE` & `acdc_py-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `acdc_py-1.0.1/README.md` & `acdc_py-1.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # acdc_py 🤘
+[![pipy](https://img.shields.io/pypi/v/acdc-py?color=informational)](https://pypi.org/project/acdc-py/1.0.2/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Downloads](https://static.pepy.tech/badge/acdc-py)](https://pepy.tech/project/acdc-py)
+[![Documentation Status](https://readthedocs.org/projects/acdc-py/badge/?version=latest)](https://readthedocs.org/projects/acdc-py/badge/?version=latest)
+
+
+
 
 **A**utomated **C**ommunity **D**etection of **C**ell Populations in Python  
 
 This repo contains the current Python implementation of ACDC, an optimization-based framework to automatize clustering of cell populations from scRNA-seq data using community detection algorithms. 
 ```acdc_py``` is currently **under development** and new functionalities will be released, following completion and benchmarking. 
 ```acdc_py``` is deployed as a Python package and fully compatible with ```Scanpy```.
 
@@ -27,14 +33,18 @@
 STAY TUNED FOR UPDATES AND NOVEL DEVELOPMENTS!🤘🏾
 ```
 
 **Please, be aware that while this project is "work in progress" and outcomes are continuously benchmarked, cross-platform compability might not yet be guaranteed. 
 
 
 # Installation 
+### pypi
+```shell
+pip install acdc-py
+```
 ### local
 ```shell
 git clone https://github.com/califano-lab/acdc_py/
 cd acdc_py
 pip install -e .
 ```
```

### Comparing `acdc_py-1.0.1/acdc_py/GS.py` & `acdc_py-1.0.2/acdc_py/GS.py`

 * *Files identical despite different names*

### Comparing `acdc_py-1.0.1/acdc_py/SA.py` & `acdc_py-1.0.2/acdc_py/SA.py`

 * *Files identical despite different names*

### Comparing `acdc_py-1.0.1/acdc_py/_SA_GS_subfunctions.py` & `acdc_py-1.0.2/acdc_py/_SA_GS_subfunctions.py`

 * *Files identical despite different names*

### Comparing `acdc_py-1.0.1/acdc_py/_condense_diffuse_funcs.py` & `acdc_py-1.0.2/acdc_py/_condense_diffuse_funcs.py`

 * *Files identical despite different names*

### Comparing `acdc_py-1.0.1/acdc_py/_diffuse_correction_funcs.py` & `acdc_py-1.0.2/acdc_py/_diffuse_correction_funcs.py`

 * *Files identical despite different names*

### Comparing `acdc_py-1.0.1/acdc_py/_dual_annealing_with_progress_bar.py` & `acdc_py-1.0.2/acdc_py/_dual_annealing_with_progress_bar.py`

 * *Files identical despite different names*

### Comparing `acdc_py-1.0.1/acdc_py/_get_opt.py` & `acdc_py-1.0.2/acdc_py/_get_opt.py`

 * *Files identical despite different names*

### Comparing `acdc_py-1.0.1/acdc_py/_pl.py` & `acdc_py-1.0.2/acdc_py/_pl.py`

 * *Files identical despite different names*

### Comparing `acdc_py-1.0.1/acdc_py/_pp.py` & `acdc_py-1.0.2/acdc_py/_pp.py`

 * *Files identical despite different names*

### Comparing `acdc_py-1.0.1/acdc_py/_tl.py` & `acdc_py-1.0.2/acdc_py/_tl.py`

 * *Files identical despite different names*

### Comparing `acdc_py-1.0.1/acdc_py/get_opt.py` & `acdc_py-1.0.2/acdc_py/get_opt.py`

 * *Files identical despite different names*

### Comparing `acdc_py-1.0.1/acdc_py/pl.py` & `acdc_py-1.0.2/acdc_py/pl.py`

 * *Files identical despite different names*

### Comparing `acdc_py-1.0.1/acdc_py/pp.py` & `acdc_py-1.0.2/acdc_py/pp.py`

 * *Files identical despite different names*

### Comparing `acdc_py-1.0.1/acdc_py/tl.py` & `acdc_py-1.0.2/acdc_py/tl.py`

 * *Files identical despite different names*

### Comparing `acdc_py-1.0.1/setup.py` & `acdc_py-1.0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
+# read the contents of your README file
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 setuptools.setup(
     name="acdc_py",
-    version="1.0.1",
+    version="1.0.2",
     author="Alexander L.E. Wang & Luca Zanella & Alessandro Vasciaveo",
     author_email="aw3436@cumc.columbia.edu",
     packages=["acdc_py"],
     description="A package to quickly identify unbiased graph-based clusterings via parameter optimization in Python",
-    long_description="This Scanpy-compatible package provides the ability to iterative compute clusterings using graph-based on combinations of resolution and KNN. At each point in this search space, a metric, such as silhouette score, is computed. The solution from this search space that maximizes the metric results in an optimal unbiased clustering solution. This process is sped up by our subsampling and diffusion feature that provides a near-identical solution in a much shorter time.",
+    long_description=long_description,
+    #long_description="This Scanpy-compatible package provides the ability to iterative compute clusterings using graph-based on combinations of resolution and KNN. At each point in this search space, a metric, such as silhouette score, is computed. The solution from this search space that maximizes the metric results in an optimal unbiased clustering solution. This process is sped up by our subsampling and diffusion feature that provides a near-identical solution in a much shorter time.",
+    #long_description = file: "README.md",
     long_description_content_type="text/markdown",
     url="https://github.com/califano-lab/acdc_py",
+    project_urls = {
+    'Documentation': 'https://acdc.readthedocs.io/en/latest/',
+    'Source': 'https://github.com/califano-lab/acdc_py',
+    },
     license='MIT',
     python_requires='>=3.8',
     install_requires=[
         "scipy",
         "tqdm",
         "scanpy",
         "anndata",
```

