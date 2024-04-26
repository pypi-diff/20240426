# Comparing `tmp/dlordinal-1.0.1.tar.gz` & `tmp/dlordinal-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlordinal-1.0.1.tar", last modified: Thu Jan 18 12:21:13 2024, max compression
+gzip compressed data, was "dlordinal-2.0.0.tar", last modified: Fri Apr 26 07:35:07 2024, max compression
```

## Comparing `dlordinal-1.0.1.tar` & `dlordinal-2.0.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-01-18 12:21:13.062132 dlordinal-1.0.1/
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     1511 2024-01-17 10:55:28.000000 dlordinal-1.0.1/LICENSE
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     3996 2024-01-18 12:21:13.043576 dlordinal-1.0.1/PKG-INFO
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     2743 2024-01-18 12:20:53.000000 dlordinal-1.0.1/README.md
-drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-01-18 12:21:12.324107 dlordinal-1.0.1/dlordinal/
--rw-r--r--   0 fberchez (10051) ayrna     (1001)       35 2024-01-18 12:20:53.000000 dlordinal-1.0.1/dlordinal/__init__.py
-drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-01-18 12:21:12.414309 dlordinal-1.0.1/dlordinal/datasets/
--rw-r--r--   0 fberchez (10051) ayrna     (1001)      147 2024-01-17 10:55:28.000000 dlordinal-1.0.1/dlordinal/datasets/__init__.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     8901 2024-01-17 10:55:28.000000 dlordinal-1.0.1/dlordinal/datasets/adience.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     4812 2024-01-17 10:55:28.000000 dlordinal-1.0.1/dlordinal/datasets/featuredataset.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)    10320 2024-01-17 10:55:28.000000 dlordinal-1.0.1/dlordinal/datasets/fgnet.py
-drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-01-18 12:21:12.524043 dlordinal-1.0.1/dlordinal/distributions/
--rw-r--r--   0 fberchez (10051) ayrna     (1001)      621 2023-09-26 10:54:41.000000 dlordinal-1.0.1/dlordinal/distributions/__init__.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     2052 2024-01-17 10:55:28.000000 dlordinal-1.0.1/dlordinal/distributions/beta_distribution.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     1362 2024-01-17 10:55:28.000000 dlordinal-1.0.1/dlordinal/distributions/binomial_distribution.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     1139 2024-01-17 10:55:28.000000 dlordinal-1.0.1/dlordinal/distributions/exponential_distribution.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     4696 2024-01-17 10:55:28.000000 dlordinal-1.0.1/dlordinal/distributions/general_triangular_distribution.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)      606 2024-01-17 10:55:28.000000 dlordinal-1.0.1/dlordinal/distributions/poisson_distribution.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     3322 2024-01-17 10:55:28.000000 dlordinal-1.0.1/dlordinal/distributions/triangular_distribution.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)      917 2024-01-17 10:55:28.000000 dlordinal-1.0.1/dlordinal/distributions/utils.py
-drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-01-18 12:21:12.576193 dlordinal-1.0.1/dlordinal/estimator/
--rw-r--r--   0 fberchez (10051) ayrna     (1001)       87 2023-10-04 10:38:08.000000 dlordinal-1.0.1/dlordinal/estimator/__init__.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     5468 2024-01-17 10:55:28.000000 dlordinal-1.0.1/dlordinal/estimator/pytorch_estimator.py
-drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-01-18 12:21:12.713915 dlordinal-1.0.1/dlordinal/layers/
--rw-r--r--   0 fberchez (10051) ayrna     (1001)      393 2024-01-17 10:55:28.000000 dlordinal-1.0.1/dlordinal/layers/__init__.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)      249 2024-01-17 10:55:28.000000 dlordinal-1.0.1/dlordinal/layers/activation_function.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     3255 2024-01-17 10:55:28.000000 dlordinal-1.0.1/dlordinal/layers/clm.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     2322 2024-01-17 10:55:28.000000 dlordinal-1.0.1/dlordinal/layers/ordinal_fully_connected.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     1576 2024-01-17 10:55:28.000000 dlordinal-1.0.1/dlordinal/layers/stick_breaking_layer.py
-drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-01-18 12:21:12.934645 dlordinal-1.0.1/dlordinal/losses/
--rw-r--r--   0 fberchez (10051) ayrna     (1001)      905 2024-01-17 10:55:29.000000 dlordinal-1.0.1/dlordinal/losses/__init__.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     6316 2024-01-17 10:55:29.000000 dlordinal-1.0.1/dlordinal/losses/beta_loss.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     3173 2024-01-17 10:55:29.000000 dlordinal-1.0.1/dlordinal/losses/binomial_loss.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     3728 2024-01-17 10:55:29.000000 dlordinal-1.0.1/dlordinal/losses/custom_targets_loss.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     3376 2024-01-17 10:55:29.000000 dlordinal-1.0.1/dlordinal/losses/exponential_loss.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     3360 2024-01-18 11:46:28.000000 dlordinal-1.0.1/dlordinal/losses/general_triangular_loss.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     3820 2024-01-17 10:55:29.000000 dlordinal-1.0.1/dlordinal/losses/mceloss.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     2987 2024-01-17 10:55:29.000000 dlordinal-1.0.1/dlordinal/losses/mcewkloss.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     1840 2024-01-17 10:55:29.000000 dlordinal-1.0.1/dlordinal/losses/ordinal_ecoc_distance_loss.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     3169 2024-01-17 10:55:29.000000 dlordinal-1.0.1/dlordinal/losses/poisson_loss.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     3320 2024-01-17 10:55:29.000000 dlordinal-1.0.1/dlordinal/losses/triangular_loss.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     2647 2024-01-17 10:55:29.000000 dlordinal-1.0.1/dlordinal/losses/wkloss.py
-drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-01-18 12:21:12.962673 dlordinal-1.0.1/dlordinal/metrics/
--rw-r--r--   0 fberchez (10051) ayrna     (1001)      274 2024-01-17 10:55:29.000000 dlordinal-1.0.1/dlordinal/metrics/__init__.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     6033 2024-01-17 10:55:29.000000 dlordinal-1.0.1/dlordinal/metrics/metrics.py
-drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-01-18 12:21:12.991321 dlordinal-1.0.1/dlordinal/models/
--rw-r--r--   0 fberchez (10051) ayrna     (1001)       63 2024-01-17 10:55:29.000000 dlordinal-1.0.1/dlordinal/models/__init__.py
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     4363 2024-01-17 10:55:29.000000 dlordinal-1.0.1/dlordinal/models/obd_ecoc.py
-drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-01-18 12:21:13.016991 dlordinal-1.0.1/dlordinal.egg-info/
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     3996 2024-01-18 12:21:12.000000 dlordinal-1.0.1/dlordinal.egg-info/PKG-INFO
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     1509 2024-01-18 12:21:12.000000 dlordinal-1.0.1/dlordinal.egg-info/SOURCES.txt
--rw-r--r--   0 fberchez (10051) ayrna     (1001)        1 2024-01-18 12:21:12.000000 dlordinal-1.0.1/dlordinal.egg-info/dependency_links.txt
--rw-r--r--   0 fberchez (10051) ayrna     (1001)      231 2024-01-18 12:21:12.000000 dlordinal-1.0.1/dlordinal.egg-info/requires.txt
--rw-r--r--   0 fberchez (10051) ayrna     (1001)       10 2024-01-18 12:21:12.000000 dlordinal-1.0.1/dlordinal.egg-info/top_level.txt
--rw-r--r--   0 fberchez (10051) ayrna     (1001)     1423 2024-01-18 12:20:53.000000 dlordinal-1.0.1/pyproject.toml
--rw-r--r--   0 fberchez (10051) ayrna     (1001)       38 2024-01-18 12:21:13.062589 dlordinal-1.0.1/setup.cfg
--rw-r--r--   0 fberchez (10051) ayrna     (1001)       38 2024-01-17 10:55:29.000000 dlordinal-1.0.1/setup.py
+drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-04-26 07:35:06.991243 dlordinal-2.0.0/
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     1511 2024-04-10 10:59:19.000000 dlordinal-2.0.0/LICENSE
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     5854 2024-04-26 07:35:06.980126 dlordinal-2.0.0/PKG-INFO
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     4601 2024-04-26 07:33:16.000000 dlordinal-2.0.0/README.md
+drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-04-26 07:35:05.912445 dlordinal-2.0.0/dlordinal/
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)       35 2024-04-26 07:33:16.000000 dlordinal-2.0.0/dlordinal/__init__.py
+drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-04-26 07:35:06.326635 dlordinal-2.0.0/dlordinal/datasets/
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)      147 2024-01-17 10:55:28.000000 dlordinal-2.0.0/dlordinal/datasets/__init__.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     8781 2024-04-26 07:33:16.000000 dlordinal-2.0.0/dlordinal/datasets/adience.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     4938 2024-04-26 07:33:16.000000 dlordinal-2.0.0/dlordinal/datasets/featuredataset.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)    10200 2024-04-26 07:33:16.000000 dlordinal-2.0.0/dlordinal/datasets/fgnet.py
+drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-04-26 07:35:06.382497 dlordinal-2.0.0/dlordinal/dropout/
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)      121 2024-04-26 07:33:16.000000 dlordinal-2.0.0/dlordinal/dropout/__init__.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     5361 2024-04-26 07:33:16.000000 dlordinal-2.0.0/dlordinal/dropout/hybrid_dropout.py
+drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-04-26 07:35:06.438709 dlordinal-2.0.0/dlordinal/layers/
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)      393 2024-01-17 10:55:28.000000 dlordinal-2.0.0/dlordinal/layers/__init__.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)      249 2024-01-17 10:55:28.000000 dlordinal-2.0.0/dlordinal/layers/activation_function.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     3926 2024-04-26 07:33:16.000000 dlordinal-2.0.0/dlordinal/layers/clm.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     2322 2024-01-17 10:55:28.000000 dlordinal-2.0.0/dlordinal/layers/ordinal_fully_connected.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     1576 2024-01-17 10:55:28.000000 dlordinal-2.0.0/dlordinal/layers/stick_breaking_layer.py
+drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-04-26 07:35:06.708410 dlordinal-2.0.0/dlordinal/losses/
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)      905 2024-04-10 10:59:19.000000 dlordinal-2.0.0/dlordinal/losses/__init__.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     3149 2024-04-26 07:33:16.000000 dlordinal-2.0.0/dlordinal/losses/beta_loss.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     2953 2024-04-26 07:33:16.000000 dlordinal-2.0.0/dlordinal/losses/binomial_loss.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     3728 2024-04-10 10:59:19.000000 dlordinal-2.0.0/dlordinal/losses/custom_targets_loss.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     3156 2024-04-26 07:33:16.000000 dlordinal-2.0.0/dlordinal/losses/exponential_loss.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     3155 2024-04-26 07:33:16.000000 dlordinal-2.0.0/dlordinal/losses/general_triangular_loss.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     3820 2024-04-10 10:59:19.000000 dlordinal-2.0.0/dlordinal/losses/mceloss.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     2987 2024-04-10 10:59:19.000000 dlordinal-2.0.0/dlordinal/losses/mcewkloss.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     1840 2024-04-10 10:59:19.000000 dlordinal-2.0.0/dlordinal/losses/ordinal_ecoc_distance_loss.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     2949 2024-04-26 07:33:16.000000 dlordinal-2.0.0/dlordinal/losses/poisson_loss.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     3110 2024-04-26 07:33:17.000000 dlordinal-2.0.0/dlordinal/losses/triangular_loss.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     2647 2024-01-17 10:55:29.000000 dlordinal-2.0.0/dlordinal/losses/wkloss.py
+drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-04-26 07:35:06.741420 dlordinal-2.0.0/dlordinal/metrics/
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)      274 2024-01-17 10:55:29.000000 dlordinal-2.0.0/dlordinal/metrics/__init__.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     6033 2024-01-17 10:55:29.000000 dlordinal-2.0.0/dlordinal/metrics/metrics.py
+drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-04-26 07:35:06.773481 dlordinal-2.0.0/dlordinal/models/
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)       63 2024-04-10 10:59:19.000000 dlordinal-2.0.0/dlordinal/models/__init__.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     4363 2024-04-10 10:59:19.000000 dlordinal-2.0.0/dlordinal/models/obd_ecoc.py
+drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-04-26 07:35:06.961114 dlordinal-2.0.0/dlordinal/soft_labelling/
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)      678 2024-04-26 07:33:17.000000 dlordinal-2.0.0/dlordinal/soft_labelling/__init__.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     8441 2024-04-26 07:33:17.000000 dlordinal-2.0.0/dlordinal/soft_labelling/beta_distribution.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     2420 2024-04-26 07:33:17.000000 dlordinal-2.0.0/dlordinal/soft_labelling/binomial_distribution.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     2329 2024-04-26 07:33:17.000000 dlordinal-2.0.0/dlordinal/soft_labelling/exponential_distribution.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     8419 2024-04-26 07:33:17.000000 dlordinal-2.0.0/dlordinal/soft_labelling/general_triangular_distribution.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     2157 2024-04-26 07:33:17.000000 dlordinal-2.0.0/dlordinal/soft_labelling/poisson_distribution.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     6642 2024-04-26 07:33:17.000000 dlordinal-2.0.0/dlordinal/soft_labelling/triangular_distribution.py
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)      917 2024-04-26 07:33:17.000000 dlordinal-2.0.0/dlordinal/soft_labelling/utils.py
+drwxr-xr-x   0 fberchez (10051) ayrna     (1001)        0 2024-04-26 07:35:06.969749 dlordinal-2.0.0/dlordinal.egg-info/
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     5854 2024-04-26 07:35:05.000000 dlordinal-2.0.0/dlordinal.egg-info/PKG-INFO
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     1510 2024-04-26 07:35:05.000000 dlordinal-2.0.0/dlordinal.egg-info/SOURCES.txt
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)        1 2024-04-26 07:35:05.000000 dlordinal-2.0.0/dlordinal.egg-info/dependency_links.txt
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)      231 2024-04-26 07:35:05.000000 dlordinal-2.0.0/dlordinal.egg-info/requires.txt
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)       10 2024-04-26 07:35:05.000000 dlordinal-2.0.0/dlordinal.egg-info/top_level.txt
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)     1423 2024-04-26 07:33:17.000000 dlordinal-2.0.0/pyproject.toml
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)       38 2024-04-26 07:35:06.991641 dlordinal-2.0.0/setup.cfg
+-rw-r--r--   0 fberchez (10051) ayrna     (1001)       38 2024-01-17 10:55:29.000000 dlordinal-2.0.0/setup.py
```

### Comparing `dlordinal-1.0.1/LICENSE` & `dlordinal-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dlordinal-1.0.1/PKG-INFO` & `dlordinal-2.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,119 @@
-Metadata-Version: 2.1
-Name: dlordinal
-Version: 1.0.1
-Summary: Deep learning for ordinal classification
-Author-email: Francisco Bérchez-Moreno <i72bemof@uco.es>, Víctor Manuel Vargas <vvargas@uco.es>, Javier Barbero-Gómez <jbarbero@uco.es>
-Project-URL: Source, https://github.com/ayrna/dlordinal
-Project-URL: Documentation, https://dlordinal.readthedocs.io/en/latest/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: scikit-learn==1.*
-Requires-Dist: numpy==1.*,>=1.21
-Requires-Dist: torch==2.*
-Requires-Dist: torchvision>=0.13
-Requires-Dist: pandas>=1
-Requires-Dist: scipy>=1.7
-Requires-Dist: matplotlib>=3.1
-Requires-Dist: seaborn>=0.12
-Requires-Dist: scikit-image>=0.18
-Requires-Dist: tqdm>=4
-Requires-Dist: Pillow>=8
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
-Requires-Dist: sphinx-rtd-theme; extra == "docs"
-
 # Deep learning utilities library
 
-`dlordinal` is an open-source Python toolkit focused on deep learning with ordinal methodologies. It is compatible with
-[scikit-learn](https://scikit-learn.org).
-
-The library includes various modules such as loss functions, models, layers, metrics, and an estimator.
+`dlordinal` is an open-source Python toolkit focused on deep learning with ordinal methodologies.
 
 | Overview  |                                                                                                                                          |
 |-----------|------------------------------------------------------------------------------------------------------------------------------------------|
 | **CI/CD** | [![!codecov](https://img.shields.io/codecov/c/github/ayrna/dlordinal?label=codecov&logo=codecov)](https://codecov.io/gh/ayrna/dlordinal) [![!docs](https://readthedocs.org/projects/dlordinal/badge/?version=latest&style=flat)](https://dlordinal.readthedocs.io/en/latest/)  [![!python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/) |
-| **Code**  | [![![binder]](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ayrna/dlordinal/main?filepath=tutorials) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Linter: Ruff](https://img.shields.io/badge/Linter-Ruff-brightgreen?style=flat-square)](https://github.com/charliermarsh/ruff)                     |
+| **Code**  | [![![pypi]](https://img.shields.io/pypi/v/dlordinal)](https://pypi.org/project/dlordinal/2.0.0/) [![![binder]](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ayrna/dlordinal/main?filepath=tutorials) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Linter: Ruff](https://img.shields.io/badge/Linter-Ruff-brightgreen?style=flat-square)](https://github.com/charliermarsh/ruff)                     |
+
+
+## Table of Contents
+- [⚙️ Installation](#%EF%B8%8F-installation)
+- [📖 Documentation](#-documentation)
+- [Collaborating](#collaborating)
+    - [Guidelines for code contributions](#guidelines-for-code-contributions)
 
 ## ⚙️ Installation
 
-You can install **dlordinal** directly from the GitHub repository using the following command in your terminal:
+`dlordinal v2.0.0` is the last version supported by Python 3.8, Python 3.9 and Python 3.10.
+
+The easiest way to install `dlordinal` is via `pip`:
+
+```bash
+pip install dlordinal
+```
+
+## 📖 Documentation
+
+`Sphinx` is a documentation generator tool that is commonly used in the Python ecosystem. It allows developers to write documentation in a markup language called reStructuredText (reST) and generates HTML, PDF, and other formats from it. Sphinx provides a powerful and flexible way to document code, making it easier for developers to create comprehensive and user-friendly documentation for their projects.
+
+To document `dlordinal`, it is necessary to install all documentation dependencies:
+
+```bash
+pip install -e '.[docs]'
+```
+
+Then access the `docs/` directory:
+
+```bash
+docs/
+↳ api.rst
+↳ conf.py
+↳ distributions.rst
+↳ references.bib
+↳ ...
+```
+
+If a new module is created in the software project, the `api.rst` file must be modified to include the name of the new module:
+
+```plaintext
+.. _api:
+
+=============
+API Reference
+=============
+
+This is the API for the **dlordinal** package.
+
+.. toctree::
+   :maxdepth: 2
+   :caption: Contents:
+
+   losses
+   datasets
+   distributions
+   layers
+   metrics
+   sklearn_integration
+   ***NEW_MODULE***
+```
+
+Afterwards, a new file in `.rst` format associated to the new module must be created, specifying the automatic inclusion of documentation from the module files containing a docstring, and the inclusion of the bibliography if it exists within any of them.
+
+```bash
+docs/
+↳ api.rst
+↳ conf.py
+↳ distributions.rst
+↳ new_module.rst
+↳ references.bib
+↳ ...
+```
 
-    pip install git+https://github.com/ayrna/dlordinal.git@main
+```plaintext
+.. _new_module:
 
-Also, you can clone the repository and then install the library from the local repository folder:
+New Module
+==========
 
-    git clone git@github.com:ayrna/dlordinal.git
-    pip install ./dlordinal
+.. automodule:: dlordinal.new_module
+    :members:
+
+.. footbibliography::
+
+```
+
+Finally, if any new bibliographic citations have been added, they should be included in the `references.bib` file.
 
 ## Collaborating
 
 Code contributions to the dlordinal project are welcomed via pull requests.
 Please, contact the maintainers (maybe opening an issue) before doing any work to make sure that your contributions align with the project.
 
 ### Guidelines for code contributions
 
+* You can clone the repository and then install the library from the local repository folder:
+
+```bash
+git clone git@github.com:ayrna/dlordinal.git
+pip install ./dlordinal
+```
+
 * In order to set up the environment for development, install the project in editable mode and include the optional dev requirements:
 ```bash
 pip install -e '.[dev]'
 ```
 * Install the pre-commit hooks before starting to make any modifications:
 ```bash
 pre-commit install
```

### Comparing `dlordinal-1.0.1/dlordinal/datasets/adience.py` & `dlordinal-2.0.0/dlordinal/datasets/adience.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,39 @@
 from sklearn.model_selection import StratifiedShuffleSplit
 from tqdm import tqdm
 
 
 class Adience:
     """
     Base class for the Adience dataset.
+
+    Parameters
+    ----------
+    extract_file_path : Union[str, Path]
+        Path to the tar.gz file containing the dataset.
+    folds_path : Union[str, Path]
+        Path to the folder containing the folds.
+    images_path : Union[str, Path]
+        Path to the folder containing the images.
+    transformed_images_path : Union[str, Path]
+        Path to the folder containing the transformed images.
+    partition_path : Union[str, Path]
+        Path to the folder containing the partitions.
+    number_partitions : int, optional
+        Number of partitions to create, by default 20.
+    ranges : list, optional
+        List of age ranges to use, by default [(0, 2), (4, 6), (8, 13),
+        (15, 20), (25, 32), (38, 43), (48, 53), (60, 100)].
+    test_size : float, optional
+        Test size, by default 0.2.
+    extract : bool, optional
+        Boolean indicating if the tar.gz file should be extracted, by default True.
+    transfrom : bool, optional
+        Boolean indicating if the images should be transformed and the partitions
+        created, by default True.
     """
 
     def __init__(
         self,
         extract_file_path: Union[str, Path],
         folds_path: Union[str, Path],
         images_path: Union[str, Path],
@@ -33,41 +58,14 @@
             (48, 53),
             (60, 100),
         ],
         test_size: float = 0.2,
         extract: bool = True,
         transfrom: bool = True,
     ) -> None:
-        """
-        Parameters
-        ----------
-        extract_file_path : Union[str, Path]
-            Path to the tar.gz file containing the dataset.
-        folds_path : Union[str, Path]
-            Path to the folder containing the folds.
-        images_path : Union[str, Path]
-            Path to the folder containing the images.
-        transformed_images_path : Union[str, Path]
-            Path to the folder containing the transformed images.
-        partition_path : Union[str, Path]
-            Path to the folder containing the partitions.
-        number_partitions : int, optional
-            Number of partitions to create, by default 20.
-        ranges : list, optional
-            List of age ranges to use, by default [(0, 2), (4, 6), (8, 13),
-            (15, 20), (25, 32), (38, 43), (48, 53), (60, 100)].
-        test_size : float, optional
-            Test size, by default 0.2.
-        extract : bool, optional
-            Boolean indicating if the tar.gz file should be extracted, by default True.
-        transfrom : bool, optional
-            Boolean indicating if the images should be transformed and the partitions
-            created, by default True.
-        """
-
         super().__init__()
 
         self.extract_file_path = Path(extract_file_path)
         self.folds_path = Path(folds_path)
         self.images_path = Path(images_path)
         self.transformed_images_path = Path(transformed_images_path)
         self.partition_path = Path(partition_path)
```

### Comparing `dlordinal-1.0.1/dlordinal/datasets/featuredataset.py` & `dlordinal-2.0.0/dlordinal/datasets/featuredataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,20 @@
     def get_valid_shape_array(self, v: ArrayLike):
         """Convert the input ArrayLike object to a 2D numpy array with shape (n, 1)
         if it is a 1D array.
 
         Parameters
         ----------
         v : ArrayLike
+            Input array.
 
+        Returns
+        -------
+        v : np.ndarray
+            2D numpy array with shape (n, 1).
         """
 
         if isinstance(v, pd.Series):
             v = v.values  # type: ignore
         if len(v.shape) == 1:  # type: ignore
             v = np.reshape(v, (-1, 1))
         return v
```

### Comparing `dlordinal-1.0.1/dlordinal/datasets/fgnet.py` & `dlordinal-2.0.0/dlordinal/datasets/fgnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,49 +13,45 @@
 from torchvision.datasets.vision import VisionDataset
 from tqdm import tqdm
 
 
 class FGNet(VisionDataset):
     """
     Base class for FGNet dataset.
+
+    Parameters
+    ----------
+    root : str or Path
+        Root directory of dataset
+    download : bool, optional
+        If True, downloads the dataset from the internet and puts it in root directory.
+        If dataset is already downloaded, it is not downloaded again.
+    process_data : bool, optional
+        If True, processes the dataset and puts it in root directory.
+        If dataset is already processed, it is not processed again.
+    target_size : tuple, optional
+        Size of the images after resizing.
+    categories : list, optional
+        List of categories to be used.
+    test_size : float, optional
+        Size of the test set.
+    validation_size : float, optional
+        Size of the validation set.
     """
 
     def __init__(
         self,
         root: Union[str, Path],
         download: bool = False,
         process_data: bool = True,
         target_size: tuple = (128, 128),
         categories: list = [3, 11, 16, 24, 40],
         test_size: float = 0.2,
         validation_size: float = 0.15,
     ) -> None:
-        """
-        FGNet dataset.
-
-        Parameters
-        ----------
-        root : str or Path
-            Root directory of dataset
-        download : bool, optional
-            If True, downloads the dataset from the internet and puts it in root directory.
-            If dataset is already downloaded, it is not downloaded again.
-        process_data : bool, optional
-            If True, processes the dataset and puts it in root directory.
-            If dataset is already processed, it is not processed again.
-        target_size : tuple, optional
-            Size of the images after resizing.
-        categories : list, optional
-            List of categories to be used.
-        test_size : float, optional
-            Size of the test set.
-        validation_size : float, optional
-            Size of the validation set.
-        """
-
         super(FGNet, self).__init__(root)
 
         self.root = Path(self.root)
         self.root.parent.mkdir(parents=True, exist_ok=True)
         self.target_size = target_size
         self.categories = categories
         self.test_size = test_size
```

### Comparing `dlordinal-1.0.1/dlordinal/distributions/utils.py` & `dlordinal-2.0.0/dlordinal/soft_labelling/utils.py`

 * *Files identical despite different names*

### Comparing `dlordinal-1.0.1/dlordinal/layers/clm.py` & `dlordinal-2.0.0/dlordinal/losses/wkloss.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,79 @@
-from math import sqrt
+from typing import Optional
 
 import torch
-from torch.nn import Module
+import torch.nn as nn
 
 
-class CLM(Module):
+class WKLoss(nn.Module):
     """
-    Implementation of the cumulative link model from :footcite:t:`vargas2020clm` as a torch layer.
-    Different link functions can be used, including logit, probit and cloglog.
+    Implements Weighted Kappa Loss. Weighted Kappa Loss was introduced by :footcite:t:`deLaTorre2018kappa`.
+    Weighted Kappa is widely used in Ordinal Classification Problems. Its
+    value lies in :math:`[-\\infty, \\log 2]`, where :math:`\\log 2` means the random prediction
 
     Parameters
     ----------
     num_classes : int
-        The number of classes.
-    link_function : str
-        The link function to use. Can be ``'logit'``, ``'probit'`` or ``'cloglog'``.
-    min_distance : float, default=0.0
-       The minimum distance between thresholds
+        Number of unique classes in your dataset.
+    penalization_type : str, default='quadratic'
+        Weighting to be considered for calculating kappa
+        statistics. A valid value is one of ``['linear', 'quadratic']``.
+        Defaults to 'quadratic'.
+    epsilon : float, default=1e-10
+        Increment to avoid log zero,
+        so the loss will be :math:`\\log(1 - k + \\epsilon)`, where :math:`k` lies
+        in :math:`[-1, 1]`. Defaults to ``1e-10``.
     """
 
-    def __init__(self, num_classes, link_function, min_distance=0.0, **kwargs):
-        super().__init__()
+    def __init__(
+        self,
+        num_classes: int,
+        penalization_type: str = "quadratic",
+        weight: Optional[torch.Tensor] = None,
+        epsilon: Optional[float] = 1e-10,
+    ):
+        super(WKLoss, self).__init__()
         self.num_classes = num_classes
-        self.link_function = link_function
-        self.min_distance = min_distance
-        self.dist = torch.distributions.Normal(0, 1)
-        self.device = "cpu"
+        if penalization_type == "quadratic":
+            self.y_pow = 2
+        if penalization_type == "linear":
+            self.y_pow = 1
+
+        self.epsilon = epsilon
+        self.weight = weight
+
+    def forward(self, y_pred, y_true):
+        num_classes = self.num_classes
+        y = torch.eye(num_classes)
+        y_true = y[y_true]
 
-        self.thresholds_b = torch.nn.Parameter(data=torch.Tensor(1), requires_grad=True)
-        torch.nn.init.uniform_(self.thresholds_b, 0.0, 0.1)
+        y_true = y_true.float()
 
-        self.thresholds_a = torch.nn.Parameter(
-            data=torch.Tensor(self.num_classes - 2), requires_grad=True
-        )
-        torch.nn.init.uniform_(
-            self.thresholds_a,
-            sqrt((1.0 / (self.num_classes - 2)) / 2),
-            sqrt(1.0 / (self.num_classes - 2)),
+        repeat_op = (
+            torch.Tensor(list(range(num_classes))).unsqueeze(1).repeat((1, num_classes))
         )
+        repeat_op_sq = torch.square((repeat_op - repeat_op.T))
+        weights = repeat_op_sq / ((num_classes - 1) ** 2)
 
-    def _convert_thresholds(self, b, a, min_distance):
-        a = a**2
-        a = a + min_distance
-        thresholds_param = torch.cat((b, a), dim=0)
-        th = torch.sum(
-            torch.tril(
-                torch.ones((self.num_classes - 1, self.num_classes - 1)).to(
-                    self.device
-                ),
-                diagonal=-1,
-            )
-            * torch.reshape(
-                torch.tile(thresholds_param, (self.num_classes - 1,)).to(self.device),
-                shape=(self.num_classes - 1, self.num_classes - 1),
-            ),
-            dim=(1,),
+        # Apply class weight
+        if self.weight is not None:
+            # Repeat weight num_classes times in columns
+            tiled_weight = self.weight.repeat((num_classes, 1))
+            weights *= tiled_weight
+
+        pred_ = y_pred**self.y_pow
+        pred_norm = pred_ / (self.epsilon + torch.reshape(torch.sum(pred_, 1), [-1, 1]))
+
+        hist_rater_a = torch.sum(pred_norm, 0)
+        hist_rater_b = torch.sum(y_true, 0)
+
+        conf_mat = torch.matmul(pred_norm.T, y_true)
+
+        bsize = y_pred.size(0)
+        nom = torch.sum(weights * conf_mat)
+        expected_probs = torch.matmul(
+            torch.reshape(hist_rater_a, [num_classes, 1]),
+            torch.reshape(hist_rater_b, [1, num_classes]),
         )
-        return th
-
-    def _clm(self, projected: torch.Tensor, thresholds: torch.Tensor):
-        projected = torch.reshape(projected, shape=(-1,))
-
-        m = projected.shape[0]
-        a = torch.reshape(torch.tile(thresholds, (m,)), shape=(m, -1))
-        b = torch.transpose(
-            torch.reshape(
-                torch.tile(projected, (self.num_classes - 1,)), shape=(-1, m)
-            ),
-            0,
-            1,
-        )
-        z3 = a - b
-
-        if self.link_function == "probit":
-            a3T = self.dist.cdf(z3)
-        elif self.link_function == "cloglog":
-            a3T = 1 - torch.exp(-torch.exp(z3))
-        else:
-            a3T = 1.0 / (1.0 + torch.exp(-z3))
-
-        ones = torch.ones((m, 1)).to(self.device)
-        a3 = torch.cat((a3T, ones), dim=1)
-        a3[:, 1:] = a3[:, 1:] - a3[:, 0:-1]
-
-        return a3
-
-    def forward(self, x):
-        """
-        Parameters
-        ----------
-        x : torch.Tensor
-            The input tensor.
-
-        Returns
-        -------
-        output: Tensor
-            The output tensor.
-        """
-
-        thresholds = self._convert_thresholds(
-            self.thresholds_b, self.thresholds_a, self.min_distance
-        )
-
-        return self._clm(x, thresholds)
-
-    def to(self, device):
-        self.device = device
+        denom = torch.sum(weights * expected_probs / bsize)
 
-        return self
+        return nom / (denom + self.epsilon)
```

### Comparing `dlordinal-1.0.1/dlordinal/layers/ordinal_fully_connected.py` & `dlordinal-2.0.0/dlordinal/layers/ordinal_fully_connected.py`

 * *Files identical despite different names*

### Comparing `dlordinal-1.0.1/dlordinal/layers/stick_breaking_layer.py` & `dlordinal-2.0.0/dlordinal/layers/stick_breaking_layer.py`

 * *Files identical despite different names*

### Comparing `dlordinal-1.0.1/dlordinal/losses/__init__.py` & `dlordinal-2.0.0/dlordinal/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `dlordinal-1.0.1/dlordinal/losses/binomial_loss.py` & `dlordinal-2.0.0/dlordinal/losses/poisson_loss.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Optional
 
 import torch
 from torch import Tensor
 
-from ..distributions import get_binomial_probabilities
+from ..soft_labelling import get_poisson_soft_labels
 from .custom_targets_loss import CustomTargetsCrossEntropyLoss
 
 
-class BinomialCrossEntropyLoss(CustomTargetsCrossEntropyLoss):
-    """Binomial unimodal regularised cross entropy loss from :footcite:t:`liu2020unimodal`.
+class PoissonCrossEntropyLoss(CustomTargetsCrossEntropyLoss):
+    """Poisson unimodal regularised cross entropy loss from :footcite:t:`liu2020unimodal`.
 
     Parameters
     ----------
-    num_classes : int, default=5
+    num_classes : int
         Number of classes.
     eta : float, default=1.0
         Parameter that controls the influence of the regularisation.
     weight : Optional[Tensor], default=None
         A manual rescaling weight given to each class. If given, has to be a Tensor
         of size `C`. Otherwise, it is treated as if having all ones.
     size_average : Optional[bool], default=None
@@ -38,36 +38,32 @@
         Specifies the reduction to apply to the output: ``'none'`` | ``'mean'`` |
         ``'sum'``. ``'none'``: no reduction will be applied, ``'mean'``: the sum of
         the output will be divided by the number of elements in the output,
         ``'sum'``: the output will be summed. Note: :attr:`size_average` and
         :attr:`reduce` are in the process of being deprecated, and in the meantime,
         specifying either of those two args will override :attr:`reduction`.
         Default: ``'mean'``
-    label_smoothing : float, default=0.0
-        Controls the amount of label smoothing for the loss. Zero means no smoothing.
-        Default: ``0.0``
     """
 
     def __init__(
         self,
-        num_classes: int = 5,
+        num_classes: int,
         eta: float = 1.0,
         weight: Optional[Tensor] = None,
         size_average=None,
         ignore_index: int = -100,
         reduce=None,
         reduction: str = "mean",
-        label_smoothing: float = 0.0,
     ):
         # Precompute class probabilities for each label
-        cls_probs = torch.tensor(get_binomial_probabilities(num_classes)).float()
+        cls_probs = torch.tensor(get_poisson_soft_labels(num_classes)).float()
 
         super().__init__(
             cls_probs=cls_probs,
             eta=eta,
             weight=weight,
             size_average=size_average,
             ignore_index=ignore_index,
             reduce=reduce,
             reduction=reduction,
-            label_smoothing=label_smoothing,
+            label_smoothing=0.0,
         )
```

### Comparing `dlordinal-1.0.1/dlordinal/losses/custom_targets_loss.py` & `dlordinal-2.0.0/dlordinal/losses/custom_targets_loss.py`

 * *Files identical despite different names*

### Comparing `dlordinal-1.0.1/dlordinal/losses/exponential_loss.py` & `dlordinal-2.0.0/dlordinal/losses/binomial_loss.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 from typing import Optional
 
 import torch
 from torch import Tensor
 
-from ..distributions import get_exponential_probabilities
+from ..soft_labelling import get_binomial_soft_labels
 from .custom_targets_loss import CustomTargetsCrossEntropyLoss
 
 
-class ExponentialRegularisedCrossEntropyLoss(CustomTargetsCrossEntropyLoss):
-    """Expontential unimodal regularised cross entropy loss from :footcite:t:`liu2020unimodal`.
+class BinomialCrossEntropyLoss(CustomTargetsCrossEntropyLoss):
+    """Binomial unimodal regularised cross entropy loss from :footcite:t:`liu2020unimodal`.
 
     Parameters
     ----------
-    num_classes : int, default=5
+    num_classes : int
         Number of classes.
     eta : float, default=1.0
         Parameter that controls the influence of the regularisation.
-    p : float, default=1
-        Exponent parameter. Introduced in :footcite:t:`vargas2023exponential` as an
-        application of the :math:`L^p` norm.
     weight : Optional[Tensor], default=None
         A manual rescaling weight given to each class. If given, has to be a Tensor
         of size `C`. Otherwise, it is treated as if having all ones.
     size_average : Optional[bool], default=None
         Deprecated (see :attr:`reduction`). By default, the losses are averaged over
         each loss element in the batch. Note that for some losses, there are
         multiple elements per sample. If the field :attr:`size_average` is set to
@@ -41,37 +38,32 @@
         Specifies the reduction to apply to the output: ``'none'`` | ``'mean'`` |
         ``'sum'``. ``'none'``: no reduction will be applied, ``'mean'``: the sum of
         the output will be divided by the number of elements in the output,
         ``'sum'``: the output will be summed. Note: :attr:`size_average` and
         :attr:`reduce` are in the process of being deprecated, and in the meantime,
         specifying either of those two args will override :attr:`reduction`.
         Default: ``'mean'``
-    label_smoothing : float, default=0.0
-        Controls the amount of label smoothing for the loss. Zero means no smoothing.
-        Default: ``0.0``
     """
 
     def __init__(
         self,
-        num_classes: int = 5,
+        num_classes: int,
         eta: float = 1.0,
-        p: float = 1,
         weight: Optional[Tensor] = None,
         size_average=None,
         ignore_index: int = -100,
         reduce=None,
         reduction: str = "mean",
-        label_smoothing: float = 0.0,
     ):
         # Precompute class probabilities for each label
-        cls_probs = torch.tensor(get_exponential_probabilities(num_classes, p)).float()
+        cls_probs = torch.tensor(get_binomial_soft_labels(num_classes)).float()
 
         super().__init__(
             cls_probs=cls_probs,
             eta=eta,
             weight=weight,
             size_average=size_average,
             ignore_index=ignore_index,
             reduce=reduce,
             reduction=reduction,
-            label_smoothing=label_smoothing,
+            label_smoothing=0.0,
         )
```

### Comparing `dlordinal-1.0.1/dlordinal/losses/general_triangular_loss.py` & `dlordinal-2.0.0/dlordinal/losses/triangular_loss.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from typing import Optional
 
-import numpy as np
 import torch
 from torch import Tensor
 
-from ..distributions import get_general_triangular_probabilities
+from ..soft_labelling import get_triangular_soft_labels
 from .custom_targets_loss import CustomTargetsCrossEntropyLoss
 
 
-class GeneralTriangularCrossEntropyLoss(CustomTargetsCrossEntropyLoss):
-    """Generalised triangular unimodal regularised cross entropy loss from :footcite:t:`vargas2023gentri`.
+class TriangularCrossEntropyLoss(CustomTargetsCrossEntropyLoss):
+    """Triangular unimodal regularised cross entropy loss from :footcite:t:`vargas2023softlabelling`.
 
     Parameters
     ----------
     num_classes : int
         Number of classes.
-    alphas : np.ndarray
-        The alpha parameters for the triangular distribution.
+    alpha2 : float, default=0.05
+        Parameter that controls the probability deposited in adjacent classes.
     eta : float, default=1.0
         Parameter that controls the influence of the regularisation.
     weight : Optional[Tensor], default=None
         A manual rescaling weight given to each class. If given, has to be a Tensor
         of size `C`. Otherwise, it is treated as if having all ones.
     size_average : Optional[bool], default=None
         Deprecated (see :attr:`reduction`). By default, the losses are averaged over
@@ -41,38 +40,32 @@
         Specifies the reduction to apply to the output: ``'none'`` | ``'mean'`` |
         ``'sum'``. ``'none'``: no reduction will be applied, ``'mean'``: the sum of
         the output will be divided by the number of elements in the output,
         ``'sum'``: the output will be summed. Note: :attr:`size_average` and
         :attr:`reduce` are in the process of being deprecated, and in the meantime,
         specifying either of those two args will override :attr:`reduction`.
         Default: ``'mean'``
-    label_smoothing : float, default=0.0
-        Controls the amount of label smoothing for the loss. Zero means no smoothing.
-        Default: ``0.0``
     """
 
     def __init__(
         self,
         num_classes: int,
-        alphas: np.ndarray,
+        alpha2: float = 0.05,
         eta: float = 1.0,
         weight: Optional[Tensor] = None,
         size_average=None,
         ignore_index: int = -100,
         reduce=None,
         reduction: str = "mean",
-        label_smoothing: float = 0.0,
     ):
         # Precompute class probabilities for each label
-        r = get_general_triangular_probabilities(num_classes, alphas, verbose=0)
-        cls_probs = torch.tensor(r)
-
+        cls_probs = torch.tensor(get_triangular_soft_labels(num_classes, alpha2))
         super().__init__(
             cls_probs=cls_probs,
             eta=eta,
             weight=weight,
             size_average=size_average,
             ignore_index=ignore_index,
             reduce=reduce,
             reduction=reduction,
-            label_smoothing=label_smoothing,
+            label_smoothing=0.0,
         )
```

### Comparing `dlordinal-1.0.1/dlordinal/losses/mceloss.py` & `dlordinal-2.0.0/dlordinal/losses/mceloss.py`

 * *Files identical despite different names*

### Comparing `dlordinal-1.0.1/dlordinal/losses/mcewkloss.py` & `dlordinal-2.0.0/dlordinal/losses/mcewkloss.py`

 * *Files identical despite different names*

### Comparing `dlordinal-1.0.1/dlordinal/losses/ordinal_ecoc_distance_loss.py` & `dlordinal-2.0.0/dlordinal/losses/ordinal_ecoc_distance_loss.py`

 * *Files identical despite different names*

### Comparing `dlordinal-1.0.1/dlordinal/losses/poisson_loss.py` & `dlordinal-2.0.0/dlordinal/losses/beta_loss.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from typing import Optional
 
 import torch
 from torch import Tensor
 
-from ..distributions import get_poisson_probabilities
+from ..soft_labelling import get_beta_soft_labels
 from .custom_targets_loss import CustomTargetsCrossEntropyLoss
 
 
-class PoissonCrossEntropyLoss(CustomTargetsCrossEntropyLoss):
-    """Poisson unimodal regularised cross entropy loss from :footcite:t:`liu2020unimodal`.
+class BetaCrossEntropyLoss(CustomTargetsCrossEntropyLoss):
+    """Beta unimodal regularised cross entropy loss from :footcite:t:`vargas2022unimodal`.
 
     Parameters
     ----------
-    num_classes : int, default=5
+    num_classes : int
         Number of classes.
+    params_set : str, default='standard'
+        The set of parameters to use for the beta distribution (chosen from the
+        _beta_params_set dictionary).
     eta : float, default=1.0
         Parameter that controls the influence of the regularisation.
     weight : Optional[Tensor], default=None
         A manual rescaling weight given to each class. If given, has to be a Tensor
         of size `C`. Otherwise, it is treated as if having all ones.
     size_average : Optional[bool], default=None
         Deprecated (see :attr:`reduction`). By default, the losses are averaged over
@@ -38,36 +41,33 @@
         Specifies the reduction to apply to the output: ``'none'`` | ``'mean'`` |
         ``'sum'``. ``'none'``: no reduction will be applied, ``'mean'``: the sum of
         the output will be divided by the number of elements in the output,
         ``'sum'``: the output will be summed. Note: :attr:`size_average` and
         :attr:`reduce` are in the process of being deprecated, and in the meantime,
         specifying either of those two args will override :attr:`reduction`.
         Default: ``'mean'``
-    label_smoothing : float, default=0.0
-        Controls the amount of label smoothing for the loss. Zero means no smoothing.
-        Default: ``0.0``
     """
 
     def __init__(
         self,
-        num_classes: int = 5,
+        num_classes: int,
+        params_set: str = "standard",
         eta: float = 1.0,
         weight: Optional[Tensor] = None,
         size_average=None,
         ignore_index: int = -100,
         reduce=None,
         reduction: str = "mean",
-        label_smoothing: float = 0.0,
     ):
         # Precompute class probabilities for each label
-        cls_probs = torch.tensor(get_poisson_probabilities(num_classes)).float()
+        cls_probs = torch.tensor(get_beta_soft_labels(num_classes, params_set)).float()
 
         super().__init__(
             cls_probs=cls_probs,
             eta=eta,
             weight=weight,
             size_average=size_average,
             ignore_index=ignore_index,
             reduce=reduce,
             reduction=reduction,
-            label_smoothing=label_smoothing,
+            label_smoothing=0.0,
         )
```

### Comparing `dlordinal-1.0.1/dlordinal/losses/triangular_loss.py` & `dlordinal-2.0.0/dlordinal/losses/exponential_loss.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from typing import Optional
 
 import torch
 from torch import Tensor
 
-from ..distributions import get_triangular_probabilities
+from ..soft_labelling import get_exponential_soft_labels
 from .custom_targets_loss import CustomTargetsCrossEntropyLoss
 
 
-class TriangularCrossEntropyLoss(CustomTargetsCrossEntropyLoss):
-    """Triangular unimodal regularised cross entropy loss from :footcite:t:`vargas2023softlabelling`.
+class ExponentialRegularisedCrossEntropyLoss(CustomTargetsCrossEntropyLoss):
+    """Expontential unimodal regularised cross entropy loss from :footcite:t:`liu2020unimodal`.
 
     Parameters
     ----------
-    num_classes : int, default=5
+    num_classes : int
         Number of classes.
-    alpha2 : float, default=0.05
-        Parameter that controls the influence of the regularisation.
     eta : float, default=1.0
         Parameter that controls the influence of the regularisation.
+    p : float, default=1
+        Exponent parameter. Introduced in :footcite:t:`vargas2023exponential` as an
+        application of the :math:`L^p` norm.
     weight : Optional[Tensor], default=None
         A manual rescaling weight given to each class. If given, has to be a Tensor
         of size `C`. Otherwise, it is treated as if having all ones.
     size_average : Optional[bool], default=None
         Deprecated (see :attr:`reduction`). By default, the losses are averaged over
         each loss element in the batch. Note that for some losses, there are
         multiple elements per sample. If the field :attr:`size_average` is set to
@@ -40,36 +41,33 @@
         Specifies the reduction to apply to the output: ``'none'`` | ``'mean'`` |
         ``'sum'``. ``'none'``: no reduction will be applied, ``'mean'``: the sum of
         the output will be divided by the number of elements in the output,
         ``'sum'``: the output will be summed. Note: :attr:`size_average` and
         :attr:`reduce` are in the process of being deprecated, and in the meantime,
         specifying either of those two args will override :attr:`reduction`.
         Default: ``'mean'``
-    label_smoothing : float, default=0.0
-        Controls the amount of label smoothing for the loss. Zero means no smoothing.
-        Default: ``0.0``
     """
 
     def __init__(
         self,
-        num_classes: int = 5,
-        alpha2: float = 0.05,
+        num_classes: int,
         eta: float = 1.0,
+        p: float = 1,
         weight: Optional[Tensor] = None,
         size_average=None,
         ignore_index: int = -100,
         reduce=None,
         reduction: str = "mean",
-        label_smoothing: float = 0.0,
     ):
         # Precompute class probabilities for each label
-        cls_probs = torch.tensor(get_triangular_probabilities(num_classes, alpha2))
+        cls_probs = torch.tensor(get_exponential_soft_labels(num_classes, p)).float()
+
         super().__init__(
             cls_probs=cls_probs,
             eta=eta,
             weight=weight,
             size_average=size_average,
             ignore_index=ignore_index,
             reduce=reduce,
             reduction=reduction,
-            label_smoothing=label_smoothing,
+            label_smoothing=0.0,
         )
```

### Comparing `dlordinal-1.0.1/dlordinal/metrics/metrics.py` & `dlordinal-2.0.0/dlordinal/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `dlordinal-1.0.1/dlordinal/models/obd_ecoc.py` & `dlordinal-2.0.0/dlordinal/models/obd_ecoc.py`

 * *Files identical despite different names*

### Comparing `dlordinal-1.0.1/pyproject.toml` & `dlordinal-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "toml", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dlordinal"
-version = "1.0.1"
+version = "2.0.0"
 authors = [
     {name = "Francisco Bérchez-Moreno", email = "i72bemof@uco.es"},
     {name = "Víctor Manuel Vargas", email = "vvargas@uco.es"},
     {name = "Javier Barbero-Gómez", email = "jbarbero@uco.es"},
 ]
 description = "Deep learning for ordinal classification"
 readme = "README.md"
```

