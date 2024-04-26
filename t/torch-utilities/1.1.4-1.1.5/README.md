# Comparing `tmp/torch_utilities-1.1.4.tar.gz` & `tmp/torch_utilities-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_utilities-1.1.4.tar", last modified: Mon Mar 11 22:26:12 2024, max compression
+gzip compressed data, was "torch_utilities-1.1.5.tar", last modified: Fri Apr 26 13:36:02 2024, max compression
```

## Comparing `torch_utilities-1.1.4.tar` & `torch_utilities-1.1.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2024-03-11 22:26:12.721178 torch_utilities-1.1.4/
--rw-rw-r--   0 deema     (1000) deema     (1000)     1074 2024-03-11 22:02:35.000000 torch_utilities-1.1.4/LICENSE
--rw-rw-r--   0 deema     (1000) deema     (1000)       71 2024-03-11 22:02:35.000000 torch_utilities-1.1.4/MANIFEST.in
--rw-r--r--   0 deema     (1000) deema     (1000)     5386 2024-03-11 22:26:12.721178 torch_utilities-1.1.4/PKG-INFO
--rw-rw-r--   0 deema     (1000) deema     (1000)     4726 2024-03-11 22:02:35.000000 torch_utilities-1.1.4/README.md
--rw-rw-r--   0 deema     (1000) deema     (1000)       90 2024-03-11 22:02:35.000000 torch_utilities-1.1.4/pyproject.toml
--rw-rw-r--   0 deema     (1000) deema     (1000)      844 2024-03-11 22:26:12.721178 torch_utilities-1.1.4/setup.cfg
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2024-03-11 22:26:12.721178 torch_utilities-1.1.4/tests/
--rw-rw-r--   0 deema     (1000) deema     (1000)        1 2024-03-11 22:02:35.000000 torch_utilities-1.1.4/tests/__init__.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     3196 2024-03-11 22:24:43.000000 torch_utilities-1.1.4/tests/generate_test_data.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    11589 2024-03-11 22:24:43.000000 torch_utilities-1.1.4/tests/test_audio.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     2101 2024-03-11 22:24:43.000000 torch_utilities-1.1.4/tests/test_augmentation.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     4765 2024-03-11 22:24:43.000000 torch_utilities-1.1.4/tests/test_common.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     5896 2024-03-11 22:24:43.000000 torch_utilities-1.1.4/tests/test_data_loading.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     1990 2024-03-11 22:24:43.000000 torch_utilities-1.1.4/tests/test_features.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     4081 2024-03-11 22:24:43.000000 torch_utilities-1.1.4/tests/test_io.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     1151 2024-03-11 22:24:43.000000 torch_utilities-1.1.4/tests/test_metrics.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    37965 2024-03-11 22:24:43.000000 torch_utilities-1.1.4/tests/test_modules.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     3873 2024-03-11 22:24:43.000000 torch_utilities-1.1.4/tests/test_pytorch.py
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2024-03-11 22:26:12.717178 torch_utilities-1.1.4/torch_utilities/
--rw-rw-r--   0 deema     (1000) deema     (1000)      144 2024-03-11 22:02:35.000000 torch_utilities-1.1.4/torch_utilities/__init__.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    17774 2024-03-11 22:24:43.000000 torch_utilities-1.1.4/torch_utilities/audio.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     6251 2024-03-11 22:02:35.000000 torch_utilities-1.1.4/torch_utilities/augmentation.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     7488 2024-03-11 22:24:43.000000 torch_utilities-1.1.4/torch_utilities/common.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    13626 2024-03-11 22:02:35.000000 torch_utilities-1.1.4/torch_utilities/data_loading.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     4020 2024-03-11 22:02:35.000000 torch_utilities-1.1.4/torch_utilities/features.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     7067 2024-03-11 22:02:35.000000 torch_utilities-1.1.4/torch_utilities/io.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     1733 2024-03-11 22:02:35.000000 torch_utilities-1.1.4/torch_utilities/losses.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     3829 2024-03-11 22:24:43.000000 torch_utilities-1.1.4/torch_utilities/metrics.py
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2024-03-11 22:26:12.721178 torch_utilities-1.1.4/torch_utilities/models/
--rw-rw-r--   0 deema     (1000) deema     (1000)  1157965 2024-03-11 22:02:35.000000 torch_utilities-1.1.4/torch_utilities/models/sig_bak_ovr.onnx
--rw-rw-r--   0 deema     (1000) deema     (1000)    45881 2024-03-11 22:24:43.000000 torch_utilities-1.1.4/torch_utilities/modules.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    10435 2024-03-11 22:02:35.000000 torch_utilities-1.1.4/torch_utilities/pytorch.py
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2024-03-11 22:26:12.721178 torch_utilities-1.1.4/torch_utilities.egg-info/
--rw-r--r--   0 deema     (1000) deema     (1000)     5386 2024-03-11 22:26:12.000000 torch_utilities-1.1.4/torch_utilities.egg-info/PKG-INFO
--rw-rw-r--   0 deema     (1000) deema     (1000)     1164 2024-03-11 22:26:12.000000 torch_utilities-1.1.4/torch_utilities.egg-info/SOURCES.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)        1 2024-03-11 22:26:12.000000 torch_utilities-1.1.4/torch_utilities.egg-info/dependency_links.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)      147 2024-03-11 22:26:12.000000 torch_utilities-1.1.4/torch_utilities.egg-info/entry_points.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)      113 2024-03-11 22:26:12.000000 torch_utilities-1.1.4/torch_utilities.egg-info/requires.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)       22 2024-03-11 22:26:12.000000 torch_utilities-1.1.4/torch_utilities.egg-info/top_level.txt
+drwxrwxr-x   0 fdimarzo  (1000) fdimarzo  (1000)        0 2024-04-26 13:36:02.138551 torch_utilities-1.1.5/
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)     1074 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/LICENSE
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)       71 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/MANIFEST.in
+-rw-r--r--   0 fdimarzo  (1000) fdimarzo  (1000)     5386 2024-04-26 13:36:02.138551 torch_utilities-1.1.5/PKG-INFO
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)     4726 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/README.md
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)       90 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/pyproject.toml
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)      844 2024-04-26 13:36:02.138551 torch_utilities-1.1.5/setup.cfg
+drwxrwxr-x   0 fdimarzo  (1000) fdimarzo  (1000)        0 2024-04-26 13:36:02.138551 torch_utilities-1.1.5/tests/
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)        1 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/tests/__init__.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)     3196 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/tests/generate_test_data.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)    11589 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/tests/test_audio.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)     2101 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/tests/test_augmentation.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)     4765 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/tests/test_common.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)     5896 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/tests/test_data_loading.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)     1990 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/tests/test_features.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)     4081 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/tests/test_io.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)     1151 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/tests/test_metrics.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)    37964 2024-04-26 13:34:33.000000 torch_utilities-1.1.5/tests/test_modules.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)     3873 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/tests/test_pytorch.py
+drwxrwxr-x   0 fdimarzo  (1000) fdimarzo  (1000)        0 2024-04-26 13:36:02.138551 torch_utilities-1.1.5/torch_utilities/
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)      144 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/torch_utilities/__init__.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)    17874 2024-04-26 13:34:33.000000 torch_utilities-1.1.5/torch_utilities/audio.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)     6251 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/torch_utilities/augmentation.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)     7488 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/torch_utilities/common.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)    13626 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/torch_utilities/data_loading.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)     4020 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/torch_utilities/features.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)     7067 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/torch_utilities/io.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)     1733 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/torch_utilities/losses.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)     3829 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/torch_utilities/metrics.py
+drwxrwxr-x   0 fdimarzo  (1000) fdimarzo  (1000)        0 2024-04-26 13:36:02.138551 torch_utilities-1.1.5/torch_utilities/models/
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)  1157965 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/torch_utilities/models/sig_bak_ovr.onnx
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)    45881 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/torch_utilities/modules.py
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)    10435 2024-04-26 13:26:15.000000 torch_utilities-1.1.5/torch_utilities/pytorch.py
+drwxrwxr-x   0 fdimarzo  (1000) fdimarzo  (1000)        0 2024-04-26 13:36:02.138551 torch_utilities-1.1.5/torch_utilities.egg-info/
+-rw-r--r--   0 fdimarzo  (1000) fdimarzo  (1000)     5386 2024-04-26 13:36:02.000000 torch_utilities-1.1.5/torch_utilities.egg-info/PKG-INFO
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)     1164 2024-04-26 13:36:02.000000 torch_utilities-1.1.5/torch_utilities.egg-info/SOURCES.txt
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)        1 2024-04-26 13:36:02.000000 torch_utilities-1.1.5/torch_utilities.egg-info/dependency_links.txt
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)      147 2024-04-26 13:36:02.000000 torch_utilities-1.1.5/torch_utilities.egg-info/entry_points.txt
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)      113 2024-04-26 13:36:02.000000 torch_utilities-1.1.5/torch_utilities.egg-info/requires.txt
+-rw-rw-r--   0 fdimarzo  (1000) fdimarzo  (1000)       22 2024-04-26 13:36:02.000000 torch_utilities-1.1.5/torch_utilities.egg-info/top_level.txt
```

### Comparing `torch_utilities-1.1.4/LICENSE` & `torch_utilities-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/PKG-INFO` & `torch_utilities-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_utilities
-Version: 1.1.4
+Version: 1.1.5
 Summary: Simplifying audio and deep learning with PyTorch.
 Home-page: https://github.com/FedericoDiMarzo/torch_utilities
 Author: Federico Di Marzo
 Author-email: federicodimarzo@protonmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `torch_utilities-1.1.4/README.md` & `torch_utilities-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/setup.cfg` & `torch_utilities-1.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = torch_utilities
-version = 1.1.4
+version = 1.1.5
 author = Federico Di Marzo
 author_email = federicodimarzo@protonmail.com
 description = Simplifying audio and deep learning with PyTorch.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/FedericoDiMarzo/torch_utilities
```

### Comparing `torch_utilities-1.1.4/tests/generate_test_data.py` & `torch_utilities-1.1.5/tests/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/tests/test_audio.py` & `torch_utilities-1.1.5/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/tests/test_augmentation.py` & `torch_utilities-1.1.5/tests/test_augmentation.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/tests/test_common.py` & `torch_utilities-1.1.5/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/tests/test_data_loading.py` & `torch_utilities-1.1.5/tests/test_data_loading.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/tests/test_features.py` & `torch_utilities-1.1.5/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/tests/test_io.py` & `torch_utilities-1.1.5/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/tests/test_metrics.py` & `torch_utilities-1.1.5/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/tests/test_modules.py` & `torch_utilities-1.1.5/tests/test_modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,15 +465,14 @@
             with self.subTest(p=p):
                 conv = self.get_instance(p)
                 causal_conv_2d = conv.conv
                 self.assertEqual(type(causal_conv_2d), CausalConv2d)
                 if activation is None:
                     self.assertEqual(type(conv.activation), nn.Identity)
 
-
     def test_forward(self):
         for p in self.params:
             (
                 in_channels,
                 out_channels,
                 kernel_size,
                 stride_f,
```

### Comparing `torch_utilities-1.1.4/tests/test_pytorch.py` & `torch_utilities-1.1.5/tests/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/torch_utilities/audio.py` & `torch_utilities-1.1.5/torch_utilities/audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -692,21 +692,24 @@
     Returns
     -------
     Tensor
         Interleaved signal, the shape is the same of the inputs except
         for the interleaved dimension of lenght D that will be len(xs)*D
     """
     mod = get_np_or_torch(xs[0])
-    stride = len(xs)
-    new_shape = list(xs[0].shape)
-    new_shape[-1] *= stride
-    y = mod.zeros(new_shape)
+    if mod == np:
+        stride = len(xs)
+        new_shape = list(xs[0].shape)
+        new_shape[-1] *= stride
+        y = mod.zeros(new_shape)
 
-    for i, x in enumerate(xs):
-        y[..., i::stride] = x
+        for i, x in enumerate(xs):
+            y[..., i::stride] = x
+    else:
+        y = torch.stack(xs, -1).flatten(-2, -1)
 
     return y
 
 
 def trim_as_shortest(*xs: List[TensorOrArray], dim: int = -1) -> List[TensorOrArray]:
     """
     Trims all the inputs to the same length of the shortest one.
```

### Comparing `torch_utilities-1.1.4/torch_utilities/augmentation.py` & `torch_utilities-1.1.5/torch_utilities/augmentation.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/torch_utilities/common.py` & `torch_utilities-1.1.5/torch_utilities/common.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/torch_utilities/data_loading.py` & `torch_utilities-1.1.5/torch_utilities/data_loading.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/torch_utilities/features.py` & `torch_utilities-1.1.5/torch_utilities/features.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/torch_utilities/io.py` & `torch_utilities-1.1.5/torch_utilities/io.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/torch_utilities/losses.py` & `torch_utilities-1.1.5/torch_utilities/losses.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/torch_utilities/metrics.py` & `torch_utilities-1.1.5/torch_utilities/metrics.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/torch_utilities/models/sig_bak_ovr.onnx` & `torch_utilities-1.1.5/torch_utilities/models/sig_bak_ovr.onnx`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/torch_utilities/modules.py` & `torch_utilities-1.1.5/torch_utilities/modules.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/torch_utilities/pytorch.py` & `torch_utilities-1.1.5/torch_utilities/pytorch.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.1.4/torch_utilities.egg-info/PKG-INFO` & `torch_utilities-1.1.5/torch_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_utilities
-Version: 1.1.4
+Version: 1.1.5
 Summary: Simplifying audio and deep learning with PyTorch.
 Home-page: https://github.com/FedericoDiMarzo/torch_utilities
 Author: Federico Di Marzo
 Author-email: federicodimarzo@protonmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `torch_utilities-1.1.4/torch_utilities.egg-info/SOURCES.txt` & `torch_utilities-1.1.5/torch_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

