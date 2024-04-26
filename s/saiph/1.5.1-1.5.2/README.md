# Comparing `tmp/saiph-1.5.1.tar.gz` & `tmp/saiph-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saiph-1.5.1.tar", max compression
+gzip compressed data, was "saiph-1.5.2.tar", max compression
```

## Comparing `saiph-1.5.1.tar` & `saiph-1.5.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     9861 2024-01-18 16:07:29.213794 saiph-1.5.1/LICENSE
--rw-r--r--   0        0        0     2214 2024-01-18 16:07:29.217794 saiph-1.5.1/pyproject.toml
--rw-r--r--   0        0        0      286 2024-01-18 16:07:29.217794 saiph-1.5.1/saiph/__init__.py
--rw-r--r--   0        0        0     4439 2024-01-18 16:07:29.217794 saiph-1.5.1/saiph/conftest.py
--rw-r--r--   0        0        0     1195 2024-01-18 16:07:29.217794 saiph-1.5.1/saiph/contribution.py
--rw-r--r--   0        0        0     1384 2024-01-18 16:07:29.217794 saiph-1.5.1/saiph/contribution_test.py
--rw-r--r--   0        0        0      119 2024-01-18 16:07:29.217794 saiph-1.5.1/saiph/exception.py
--rw-r--r--   0        0        0     7031 2024-01-18 16:07:29.217794 saiph-1.5.1/saiph/inverse_transform.py
--rw-r--r--   0        0        0     9868 2024-01-18 16:07:29.217794 saiph-1.5.1/saiph/inverse_transform_test.py
--rw-r--r--   0        0        0      410 2024-01-18 16:07:29.217794 saiph-1.5.1/saiph/lib/size.py
--rw-r--r--   0        0        0     2511 2024-01-18 16:07:29.217794 saiph-1.5.1/saiph/models.py
--rw-r--r--   0        0        0     8738 2024-01-18 16:07:29.217794 saiph-1.5.1/saiph/projection.py
--rw-r--r--   0        0        0    13496 2024-01-18 16:07:29.217794 saiph-1.5.1/saiph/projection_test.py
--rw-r--r--   0        0        0       26 2024-01-18 16:07:29.217794 saiph-1.5.1/saiph/reduction/__init__.py
--rw-r--r--   0        0        0    15986 2024-01-18 16:07:29.217794 saiph-1.5.1/saiph/reduction/famd.py
--rw-r--r--   0        0        0     4911 2024-01-18 16:07:29.217794 saiph-1.5.1/saiph/reduction/famd_sparse.py
--rw-r--r--   0        0        0     4879 2024-01-18 16:07:29.217794 saiph-1.5.1/saiph/reduction/famd_sparse_test.py
--rw-r--r--   0        0        0     8509 2024-01-18 16:07:29.217794 saiph-1.5.1/saiph/reduction/famd_test.py
--rw-r--r--   0        0        0     9690 2024-01-18 16:07:29.217794 saiph-1.5.1/saiph/reduction/mca.py
--rw-r--r--   0        0        0     6868 2024-01-18 16:07:29.217794 saiph-1.5.1/saiph/reduction/mca_test.py
--rw-r--r--   0        0        0     4558 2024-01-18 16:07:29.221794 saiph-1.5.1/saiph/reduction/pca.py
--rw-r--r--   0        0        0     3829 2024-01-18 16:07:29.221794 saiph-1.5.1/saiph/reduction/pca_test.py
--rw-r--r--   0        0        0        0 2024-01-18 16:07:29.221794 saiph-1.5.1/saiph/reduction/utils/__init__.py
--rw-r--r--   0        0        0     3823 2024-01-18 16:07:29.221794 saiph-1.5.1/saiph/reduction/utils/common.py
--rw-r--r--   0        0        0     2455 2024-01-18 16:07:29.221794 saiph-1.5.1/saiph/reduction/utils/common_test.py
--rw-r--r--   0        0        0     4709 2024-01-18 16:07:29.221794 saiph-1.5.1/saiph/reduction/utils/svd.py
--rw-r--r--   0        0        0     5288 2024-01-18 16:07:29.221794 saiph-1.5.1/saiph/reduction/utils/svd_test.py
--rw-r--r--   0        0        0     5178 2024-01-18 16:07:29.221794 saiph-1.5.1/saiph/serializer.py
--rw-r--r--   0        0        0     2002 2024-01-18 16:07:29.221794 saiph-1.5.1/saiph/serializer_test.py
--rw-r--r--   0        0        0        0 2024-01-18 16:07:29.221794 saiph-1.5.1/saiph/tests/__init_.py
--rw-r--r--   0        0        0     1402 2024-01-18 16:07:29.221794 saiph-1.5.1/saiph/tests/benchmark_test.py
--rw-r--r--   0        0        0      521 2024-01-18 16:07:29.221794 saiph-1.5.1/saiph/tests/profile_cpu.py
--rw-r--r--   0        0        0      983 2024-01-18 16:07:29.221794 saiph-1.5.1/saiph/tests/profile_memory.py
--rw-r--r--   0        0        0     5405 2024-01-18 16:07:29.221794 saiph-1.5.1/saiph/visualization.py
--rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 saiph-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     9861 2024-04-26 09:34:44.539190 saiph-1.5.2/LICENSE
+-rw-r--r--   0        0        0     2210 2024-04-26 09:34:44.543191 saiph-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0      286 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/__init__.py
+-rw-r--r--   0        0        0     4439 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/conftest.py
+-rw-r--r--   0        0        0     1195 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/contribution.py
+-rw-r--r--   0        0        0     1384 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/contribution_test.py
+-rw-r--r--   0        0        0      119 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/exception.py
+-rw-r--r--   0        0        0     7031 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/inverse_transform.py
+-rw-r--r--   0        0        0     9868 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/inverse_transform_test.py
+-rw-r--r--   0        0        0      410 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/lib/size.py
+-rw-r--r--   0        0        0     2511 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/models.py
+-rw-r--r--   0        0        0     8738 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/projection.py
+-rw-r--r--   0        0        0    13496 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/projection_test.py
+-rw-r--r--   0        0        0       26 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/__init__.py
+-rw-r--r--   0        0        0    15986 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/famd.py
+-rw-r--r--   0        0        0     4911 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/famd_sparse.py
+-rw-r--r--   0        0        0     4879 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/famd_sparse_test.py
+-rw-r--r--   0        0        0     8509 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/famd_test.py
+-rw-r--r--   0        0        0     9690 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/mca.py
+-rw-r--r--   0        0        0     6868 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/mca_test.py
+-rw-r--r--   0        0        0     4558 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/pca.py
+-rw-r--r--   0        0        0     3829 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/pca_test.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/utils/__init__.py
+-rw-r--r--   0        0        0     3823 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/utils/common.py
+-rw-r--r--   0        0        0     2455 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/utils/common_test.py
+-rw-r--r--   0        0        0     4709 2024-04-26 09:34:44.547191 saiph-1.5.2/saiph/reduction/utils/svd.py
+-rw-r--r--   0        0        0     5288 2024-04-26 09:34:44.547191 saiph-1.5.2/saiph/reduction/utils/svd_test.py
+-rw-r--r--   0        0        0     5178 2024-04-26 09:34:44.547191 saiph-1.5.2/saiph/serializer.py
+-rw-r--r--   0        0        0     2002 2024-04-26 09:34:44.547191 saiph-1.5.2/saiph/serializer_test.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:34:44.547191 saiph-1.5.2/saiph/tests/__init_.py
+-rw-r--r--   0        0        0     1402 2024-04-26 09:34:44.547191 saiph-1.5.2/saiph/tests/benchmark_test.py
+-rw-r--r--   0        0        0      521 2024-04-26 09:34:44.547191 saiph-1.5.2/saiph/tests/profile_cpu.py
+-rw-r--r--   0        0        0      983 2024-04-26 09:34:44.547191 saiph-1.5.2/saiph/tests/profile_memory.py
+-rw-r--r--   0        0        0     5405 2024-04-26 09:34:44.547191 saiph-1.5.2/saiph/visualization.py
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 saiph-1.5.2/PKG-INFO
```

### Comparing `saiph-1.5.1/LICENSE` & `saiph-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/pyproject.toml` & `saiph-1.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "saiph"
 # Also modify in saiph/__init__.py
-version = "1.5.1"
+version = "1.5.2"
 description = "A projection package"
 authors = ["Octopize <help@octopize.io>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.9,<3.12"
 pandas = "^1.3"
 numpy = "^1.21"
 scipy = "^1.7"
 scikit-learn = "^1.0"
-toolz = "^0.11.2"
+toolz = "0.*"
 matplotlib = {version = "^3.5.2", optional = true}
 pydantic = "^2"
 msgspec = "^0.18.5"
 
 [tool.poetry.extras]
 matplotlib = ["matplotlib"]
```

### Comparing `saiph-1.5.1/saiph/conftest.py` & `saiph-1.5.2/saiph/conftest.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/contribution.py` & `saiph-1.5.2/saiph/contribution.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/contribution_test.py` & `saiph-1.5.2/saiph/contribution_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/inverse_transform.py` & `saiph-1.5.2/saiph/inverse_transform.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/inverse_transform_test.py` & `saiph-1.5.2/saiph/inverse_transform_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/models.py` & `saiph-1.5.2/saiph/models.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/projection.py` & `saiph-1.5.2/saiph/projection.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/projection_test.py` & `saiph-1.5.2/saiph/projection_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/reduction/famd.py` & `saiph-1.5.2/saiph/reduction/famd.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/reduction/famd_sparse.py` & `saiph-1.5.2/saiph/reduction/famd_sparse.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/reduction/famd_sparse_test.py` & `saiph-1.5.2/saiph/reduction/famd_sparse_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/reduction/famd_test.py` & `saiph-1.5.2/saiph/reduction/famd_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/reduction/mca.py` & `saiph-1.5.2/saiph/reduction/mca.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/reduction/mca_test.py` & `saiph-1.5.2/saiph/reduction/mca_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/reduction/pca.py` & `saiph-1.5.2/saiph/reduction/pca.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/reduction/pca_test.py` & `saiph-1.5.2/saiph/reduction/pca_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/reduction/utils/common.py` & `saiph-1.5.2/saiph/reduction/utils/common.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/reduction/utils/common_test.py` & `saiph-1.5.2/saiph/reduction/utils/common_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/reduction/utils/svd.py` & `saiph-1.5.2/saiph/reduction/utils/svd.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/reduction/utils/svd_test.py` & `saiph-1.5.2/saiph/reduction/utils/svd_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/serializer.py` & `saiph-1.5.2/saiph/serializer.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/serializer_test.py` & `saiph-1.5.2/saiph/serializer_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/tests/benchmark_test.py` & `saiph-1.5.2/saiph/tests/benchmark_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/tests/profile_cpu.py` & `saiph-1.5.2/saiph/tests/profile_cpu.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/tests/profile_memory.py` & `saiph-1.5.2/saiph/tests/profile_memory.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/saiph/visualization.py` & `saiph-1.5.2/saiph/visualization.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.1/PKG-INFO` & `saiph-1.5.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: saiph
-Version: 1.5.1
+Version: 1.5.2
 Summary: A projection package
 License: Apache-2.0
 Author: Octopize
 Author-email: help@octopize.io
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: matplotlib
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0) ; extra == "matplotlib"
 Requires-Dist: msgspec (>=0.18.5,<0.19.0)
 Requires-Dist: numpy (>=1.21,<2.0)
 Requires-Dist: pandas (>=1.3,<2.0)
 Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: scikit-learn (>=1.0,<2.0)
 Requires-Dist: scipy (>=1.7,<2.0)
-Requires-Dist: toolz (>=0.11.2,<0.12.0)
+Requires-Dist: toolz (<1.0.0)
```

