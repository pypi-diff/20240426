# Comparing `tmp/stylegan2_pytorch-1.8.8.tar.gz` & `tmp/stylegan2_pytorch-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stylegan2_pytorch-1.8.8.tar", last modified: Thu Jan 27 02:21:57 2022, max compression
+gzip compressed data, was "stylegan2_pytorch-1.8.9.tar", last modified: Tue Jul 19 23:21:16 2022, max compression
```

## Comparing `stylegan2_pytorch-1.8.8.tar` & `stylegan2_pytorch-1.8.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 02:21:57.465989 stylegan2_pytorch-1.8.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-01-27 02:21:47.000000 stylegan2_pytorch-1.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-01-27 02:21:57.465989 stylegan2_pytorch-1.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18507 2022-01-27 02:21:47.000000 stylegan2_pytorch-1.8.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-01-27 02:21:57.465989 stylegan2_pytorch-1.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-01-27 02:21:47.000000 stylegan2_pytorch-1.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 02:21:57.461989 stylegan2_pytorch-1.8.8/stylegan2_pytorch/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-01-27 02:21:47.000000 stylegan2_pytorch-1.8.8/stylegan2_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5594 2022-01-27 02:21:47.000000 stylegan2_pytorch-1.8.8/stylegan2_pytorch/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4289 2022-01-27 02:21:47.000000 stylegan2_pytorch-1.8.8/stylegan2_pytorch/diff_augment.py
--rw-r--r--   0 runner    (1001) docker     (121)    51444 2022-01-27 02:21:47.000000 stylegan2_pytorch-1.8.8/stylegan2_pytorch/stylegan2_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-27 02:21:47.000000 stylegan2_pytorch-1.8.8/stylegan2_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 02:21:57.465989 stylegan2_pytorch-1.8.8/stylegan2_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-01-27 02:21:57.000000 stylegan2_pytorch-1.8.8/stylegan2_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-01-27 02:21:57.000000 stylegan2_pytorch-1.8.8/stylegan2_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-27 02:21:57.000000 stylegan2_pytorch-1.8.8/stylegan2_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-01-27 02:21:57.000000 stylegan2_pytorch-1.8.8/stylegan2_pytorch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-01-27 02:21:57.000000 stylegan2_pytorch-1.8.8/stylegan2_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-27 02:21:57.000000 stylegan2_pytorch-1.8.8/stylegan2_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 23:21:16.277946 stylegan2_pytorch-1.8.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-07-19 23:21:08.000000 stylegan2_pytorch-1.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2022-07-19 23:21:16.277946 stylegan2_pytorch-1.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    18507 2022-07-19 23:21:08.000000 stylegan2_pytorch-1.8.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-07-19 23:21:16.277946 stylegan2_pytorch-1.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-07-19 23:21:08.000000 stylegan2_pytorch-1.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 23:21:16.273946 stylegan2_pytorch-1.8.9/stylegan2_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-19 23:21:08.000000 stylegan2_pytorch-1.8.9/stylegan2_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5594 2022-07-19 23:21:08.000000 stylegan2_pytorch-1.8.9/stylegan2_pytorch/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4289 2022-07-19 23:21:08.000000 stylegan2_pytorch-1.8.9/stylegan2_pytorch/diff_augment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51444 2022-07-19 23:21:08.000000 stylegan2_pytorch-1.8.9/stylegan2_pytorch/stylegan2_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-19 23:21:08.000000 stylegan2_pytorch-1.8.9/stylegan2_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 23:21:16.277946 stylegan2_pytorch-1.8.9/stylegan2_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2022-07-19 23:21:16.000000 stylegan2_pytorch-1.8.9/stylegan2_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2022-07-19 23:21:16.000000 stylegan2_pytorch-1.8.9/stylegan2_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-19 23:21:16.000000 stylegan2_pytorch-1.8.9/stylegan2_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-07-19 23:21:16.000000 stylegan2_pytorch-1.8.9/stylegan2_pytorch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-07-19 23:21:16.000000 stylegan2_pytorch-1.8.9/stylegan2_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-19 23:21:16.000000 stylegan2_pytorch-1.8.9/stylegan2_pytorch.egg-info/top_level.txt
```

### Comparing `stylegan2_pytorch-1.8.8/LICENSE` & `stylegan2_pytorch-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stylegan2_pytorch-1.8.8/PKG-INFO` & `stylegan2_pytorch-1.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stylegan2_pytorch
-Version: 1.8.8
+Version: 1.8.9
 Summary: StyleGan2 in Pytorch
 Home-page: https://github.com/lucidrains/stylegan2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: GPLv3+
 Download-URL: https://github.com/lucidrains/stylegan2-pytorch/archive/v_036.tar.gz
 Keywords: generative adversarial networks,artificial intelligence
```

### Comparing `stylegan2_pytorch-1.8.8/README.md` & `stylegan2_pytorch-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `stylegan2_pytorch-1.8.8/setup.py` & `stylegan2_pytorch-1.8.9/setup.py`

 * *Files identical despite different names*

### Comparing `stylegan2_pytorch-1.8.8/stylegan2_pytorch/cli.py` & `stylegan2_pytorch-1.8.9/stylegan2_pytorch/cli.py`

 * *Files identical despite different names*

### Comparing `stylegan2_pytorch-1.8.8/stylegan2_pytorch/diff_augment.py` & `stylegan2_pytorch-1.8.9/stylegan2_pytorch/diff_augment.py`

 * *Files identical despite different names*

### Comparing `stylegan2_pytorch-1.8.8/stylegan2_pytorch/stylegan2_pytorch.py` & `stylegan2_pytorch-1.8.9/stylegan2_pytorch/stylegan2_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,15 +383,15 @@
         path = self.paths[index]
         img = Image.open(path)
         return self.transform(img)
 
 # augmentations
 
 def random_hflip(tensor, prob):
-    if prob > random():
+    if prob < random():
         return tensor
     return torch.flip(tensor, dims=(3,))
 
 class AugWrapper(nn.Module):
     def __init__(self, D, image_size):
         super().__init__()
         self.D = D
```

### Comparing `stylegan2_pytorch-1.8.8/stylegan2_pytorch.egg-info/PKG-INFO` & `stylegan2_pytorch-1.8.9/stylegan2_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stylegan2-pytorch
-Version: 1.8.8
+Version: 1.8.9
 Summary: StyleGan2 in Pytorch
 Home-page: https://github.com/lucidrains/stylegan2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: GPLv3+
 Download-URL: https://github.com/lucidrains/stylegan2-pytorch/archive/v_036.tar.gz
 Keywords: generative adversarial networks,artificial intelligence
```

