# Comparing `tmp/daml-0.45.0.tar.gz` & `tmp/daml-0.51.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daml-0.45.0.tar", max compression
+gzip compressed data, was "daml-0.51.0.tar", max compression
```

## Comparing `daml-0.45.0.tar` & `daml-0.51.0.tar`

### file list

```diff
@@ -1,52 +1,61 @@
--rw-r--r--   0        0        0     1060 2024-04-05 03:05:52.944366 daml-0.45.0/LICENSE.txt
--rw-r--r--   0        0        0     2528 2024-04-05 03:05:52.944366 daml-0.45.0/README.md
--rw-r--r--   0        0        0     5218 2024-04-05 03:05:57.752400 daml-0.45.0/pyproject.toml
--rw-r--r--   0        0        0      230 2024-04-05 03:05:57.756399 daml-0.45.0/src/daml/__init__.py
--rw-r--r--   0        0        0      115 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/__init__.py
--rw-r--r--   0        0        0     8269 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/base.py
--rw-r--r--   0        0        0        0 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/models/tensorflow/__init__.py
--rw-r--r--   0        0        0    14452 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/models/tensorflow/autoencoder.py
--rw-r--r--   0        0        0     3207 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/models/tensorflow/gmm.py
--rw-r--r--   0        0        0     7823 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/models/tensorflow/losses.py
--rw-r--r--   0        0        0    49533 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/models/tensorflow/pixelcnn.py
--rw-r--r--   0        0        0     4332 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/models/tensorflow/trainer.py
--rw-r--r--   0        0        0      348 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/od/__init__.py
--rw-r--r--   0        0        0     9375 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/od/ae.py
--rw-r--r--   0        0        0     7797 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/od/aegmm.py
--rw-r--r--   0        0        0    14179 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/od/llr.py
--rw-r--r--   0        0        0    11453 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/od/vae.py
--rw-r--r--   0        0        0     9801 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/od/vaegmm.py
--rw-r--r--   0        0        0        0 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/utils/__init__.py
--rw-r--r--   0        0        0     1758 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/utils/_types.py
--rw-r--r--   0        0        0     5269 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/utils/frameworks.py
--rw-r--r--   0        0        0     5410 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/utils/missing_optional_dependency.py
--rw-r--r--   0        0        0      647 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/utils/prediction.py
--rw-r--r--   0        0        0        0 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/utils/tensorflow/__init__.py
--rw-r--r--   0        0        0     9525 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/utils/tensorflow/distance.py
--rw-r--r--   0        0        0     1096 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/utils/tensorflow/perturbation.py
--rw-r--r--   0        0        0     3522 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/utils/tensorflow/prediction.py
--rw-r--r--   0        0        0      217 2024-04-05 03:05:52.948366 daml-0.45.0/src/daml/_alibi_detect/version.py
--rw-r--r--   0        0        0        0 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/_internal/metrics/__init__.py
--rw-r--r--   0        0        0     2442 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/_internal/metrics/base.py
--rw-r--r--   0        0        0     2912 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/_internal/metrics/ber.py
--rw-r--r--   0        0        0     2819 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/_internal/metrics/divergence.py
--rw-r--r--   0        0        0    15892 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/_internal/metrics/od.py
--rw-r--r--   0        0        0    13841 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/_internal/metrics/sufficiency.py
--rw-r--r--   0        0        0     1167 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/_internal/metrics/uap.py
--rw-r--r--   0        0        0     2316 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/_internal/metrics/utils.py
--rw-r--r--   0        0        0        0 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/_internal/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/_internal/models/pytorch/__init__.py
--rw-r--r--   0        0        0     6240 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/_internal/models/pytorch/autoencoder.py
--rw-r--r--   0        0        0     1354 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/_internal/models/pytorch/blocks.py
--rw-r--r--   0        0        0     1675 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/_internal/models/pytorch/utils.py
--rw-r--r--   0        0        0        0 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/_internal/models/tensorflow/__init__.py
--rw-r--r--   0        0        0     5107 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/_internal/models/tensorflow/alibi.py
--rw-r--r--   0        0        0      856 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/_prototype/README.md
--rw-r--r--   0        0        0     4544 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/_prototype/linting.py
--rw-r--r--   0        0        0      586 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/metrics/__init__.py
--rw-r--r--   0        0        0      303 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/metrics/outlier_detection/__init__.py
--rw-r--r--   0        0        0      151 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/models/__init__.py
--rw-r--r--   0        0        0      186 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/models/ae/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 03:05:52.952366 daml-0.45.0/src/daml/py.typed
--rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 daml-0.45.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-04-26 03:05:58.911849 daml-0.51.0/LICENSE.txt
+-rw-r--r--   0        0        0     2528 2024-04-26 03:05:58.911849 daml-0.51.0/README.md
+-rw-r--r--   0        0        0     5218 2024-04-26 03:06:03.903852 daml-0.51.0/pyproject.toml
+-rw-r--r--   0        0        0      230 2024-04-26 03:06:03.907852 daml-0.51.0/src/daml/__init__.py
+-rw-r--r--   0        0        0      115 2024-04-26 03:05:58.915849 daml-0.51.0/src/daml/_alibi_detect/__init__.py
+-rw-r--r--   0        0        0     8269 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/base.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/__init__.py
+-rw-r--r--   0        0        0    14452 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/autoencoder.py
+-rw-r--r--   0        0        0     3207 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/gmm.py
+-rw-r--r--   0        0        0     7823 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/losses.py
+-rw-r--r--   0        0        0    49533 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/pixelcnn.py
+-rw-r--r--   0        0        0     4332 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/trainer.py
+-rw-r--r--   0        0        0      348 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/od/__init__.py
+-rw-r--r--   0        0        0     9375 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/od/ae.py
+-rw-r--r--   0        0        0     7797 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/od/aegmm.py
+-rw-r--r--   0        0        0    14179 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/od/llr.py
+-rw-r--r--   0        0        0    11453 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/od/vae.py
+-rw-r--r--   0        0        0     9801 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/od/vaegmm.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/utils/__init__.py
+-rw-r--r--   0        0        0     1758 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/utils/_types.py
+-rw-r--r--   0        0        0     5269 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/utils/frameworks.py
+-rw-r--r--   0        0        0     5410 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/utils/missing_optional_dependency.py
+-rw-r--r--   0        0        0      647 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/utils/prediction.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/utils/tensorflow/__init__.py
+-rw-r--r--   0        0        0     9525 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/utils/tensorflow/distance.py
+-rw-r--r--   0        0        0     1096 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/utils/tensorflow/perturbation.py
+-rw-r--r--   0        0        0     3522 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/utils/tensorflow/prediction.py
+-rw-r--r--   0        0        0      217 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/version.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/__init__.py
+-rw-r--r--   0        0        0     2442 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/base.py
+-rw-r--r--   0        0        0     2912 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/ber.py
+-rw-r--r--   0        0        0     2819 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/divergence.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/drift/__init__.py
+-rw-r--r--   0        0        0     8981 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/drift/base.py
+-rw-r--r--   0        0        0     3897 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/drift/cvm.py
+-rw-r--r--   0        0        0     3954 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/drift/ks.py
+-rw-r--r--   0        0        0     7199 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/drift/mmd.py
+-rw-r--r--   0        0        0    10972 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/drift/torch.py
+-rw-r--r--   0        0        0     5285 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/drift/uncertainty.py
+-rw-r--r--   0        0        0    15892 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/od.py
+-rw-r--r--   0        0        0    13841 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/sufficiency.py
+-rw-r--r--   0        0        0     1167 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/uap.py
+-rw-r--r--   0        0        0     2316 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/utils.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/models/pytorch/__init__.py
+-rw-r--r--   0        0        0     6240 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/models/pytorch/autoencoder.py
+-rw-r--r--   0        0        0     1354 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/models/pytorch/blocks.py
+-rw-r--r--   0        0        0     1675 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/models/pytorch/utils.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/models/tensorflow/__init__.py
+-rw-r--r--   0        0        0     5107 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/models/tensorflow/alibi.py
+-rw-r--r--   0        0        0      856 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_prototype/README.md
+-rw-r--r--   0        0        0     7453 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_prototype/cleaning.py
+-rw-r--r--   0        0        0     4544 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_prototype/linting.py
+-rw-r--r--   0        0        0      626 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/metrics/__init__.py
+-rw-r--r--   0        0        0      678 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/metrics/drift/__init__.py
+-rw-r--r--   0        0        0      303 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/metrics/outlier_detection/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/models/__init__.py
+-rw-r--r--   0        0        0      186 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/models/ae/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/py.typed
+-rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 daml-0.51.0/PKG-INFO
```

### Comparing `daml-0.45.0/LICENSE.txt` & `daml-0.51.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/README.md` & `daml-0.51.0/README.md`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/pyproject.toml` & `daml-0.51.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "daml"
-version = "0.45.0" # dynamic
+version = "0.51.0" # dynamic
 description = "DAML provides a simple interface to characterize image data and its impact on model performance across classification and object-detection tasks"
 license = "MIT"
 readme = "README.md"
 homepage = "https://daml.ai/"
 repository = "https://github.com/aria-ml/daml/"
 documentation = "https://daml.readthedocs.io/"
```

### Comparing `daml-0.45.0/src/daml/_alibi_detect/base.py` & `daml-0.51.0/src/daml/_alibi_detect/base.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_alibi_detect/models/tensorflow/autoencoder.py` & `daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/autoencoder.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_alibi_detect/models/tensorflow/gmm.py` & `daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/gmm.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_alibi_detect/models/tensorflow/losses.py` & `daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/losses.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_alibi_detect/models/tensorflow/pixelcnn.py` & `daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/pixelcnn.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_alibi_detect/models/tensorflow/trainer.py` & `daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/trainer.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_alibi_detect/od/ae.py` & `daml-0.51.0/src/daml/_alibi_detect/od/ae.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_alibi_detect/od/aegmm.py` & `daml-0.51.0/src/daml/_alibi_detect/od/aegmm.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_alibi_detect/od/llr.py` & `daml-0.51.0/src/daml/_alibi_detect/od/llr.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_alibi_detect/od/vae.py` & `daml-0.51.0/src/daml/_alibi_detect/od/vae.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_alibi_detect/od/vaegmm.py` & `daml-0.51.0/src/daml/_alibi_detect/od/vaegmm.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_alibi_detect/utils/_types.py` & `daml-0.51.0/src/daml/_alibi_detect/utils/_types.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_alibi_detect/utils/frameworks.py` & `daml-0.51.0/src/daml/_alibi_detect/utils/frameworks.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_alibi_detect/utils/missing_optional_dependency.py` & `daml-0.51.0/src/daml/_alibi_detect/utils/missing_optional_dependency.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_alibi_detect/utils/prediction.py` & `daml-0.51.0/src/daml/_alibi_detect/utils/prediction.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_alibi_detect/utils/tensorflow/distance.py` & `daml-0.51.0/src/daml/_alibi_detect/utils/tensorflow/distance.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_alibi_detect/utils/tensorflow/perturbation.py` & `daml-0.51.0/src/daml/_alibi_detect/utils/tensorflow/perturbation.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_alibi_detect/utils/tensorflow/prediction.py` & `daml-0.51.0/src/daml/_alibi_detect/utils/tensorflow/prediction.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_internal/metrics/base.py` & `daml-0.51.0/src/daml/_internal/metrics/base.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_internal/metrics/ber.py` & `daml-0.51.0/src/daml/_internal/metrics/ber.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_internal/metrics/divergence.py` & `daml-0.51.0/src/daml/_internal/metrics/divergence.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_internal/metrics/od.py` & `daml-0.51.0/src/daml/_internal/metrics/od.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_internal/metrics/sufficiency.py` & `daml-0.51.0/src/daml/_internal/metrics/sufficiency.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_internal/metrics/uap.py` & `daml-0.51.0/src/daml/_internal/metrics/uap.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_internal/metrics/utils.py` & `daml-0.51.0/src/daml/_internal/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_internal/models/pytorch/autoencoder.py` & `daml-0.51.0/src/daml/_internal/models/pytorch/autoencoder.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_internal/models/pytorch/blocks.py` & `daml-0.51.0/src/daml/_internal/models/pytorch/blocks.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_internal/models/pytorch/utils.py` & `daml-0.51.0/src/daml/_internal/models/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_internal/models/tensorflow/alibi.py` & `daml-0.51.0/src/daml/_internal/models/tensorflow/alibi.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_prototype/README.md` & `daml-0.51.0/src/daml/_prototype/README.md`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/_prototype/linting.py` & `daml-0.51.0/src/daml/_prototype/linting.py`

 * *Files identical despite different names*

### Comparing `daml-0.45.0/src/daml/metrics/__init__.py` & `daml-0.51.0/src/daml/metrics/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from importlib.util import find_spec
 
 from daml._internal.metrics.ber import BER
 from daml._internal.metrics.divergence import Divergence
 from daml._internal.metrics.uap import UAP
+from daml.metrics import drift
 
-__all__ = ["BER", "Divergence", "UAP"]
+__all__ = ["BER", "Divergence", "UAP", "drift"]
 
 if (
     find_spec("tensorflow") is not None
     and find_spec("tensorflow_probability") is not None
 ):  # pragma: no cover
     from . import outlier_detection
```

### Comparing `daml-0.45.0/PKG-INFO` & `daml-0.51.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daml
-Version: 0.45.0
+Version: 0.51.0
 Summary: DAML provides a simple interface to characterize image data and its impact on model performance across classification and object-detection tasks
 Home-page: https://daml.ai/
 License: MIT
 Author: Andrew Weng
 Author-email: andrew.weng@ariacoustics.com
 Maintainer: ARiA
 Maintainer-email: daml@ariacoustics.com
```

