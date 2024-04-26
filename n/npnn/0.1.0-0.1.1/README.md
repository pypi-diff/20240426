# Comparing `tmp/npnn-0.1.0.tar.gz` & `tmp/npnn-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npnn-0.1.0.tar", last modified: Sat Apr 20 13:38:03 2024, max compression
+gzip compressed data, was "npnn-0.1.1.tar", last modified: Fri Apr 26 12:16:33 2024, max compression
```

## Comparing `npnn-0.1.0.tar` & `npnn-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:38:03.873239 npnn-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-20 13:37:53.000000 npnn-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-20 13:38:03.873239 npnn-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-20 13:37:53.000000 npnn-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-20 13:37:53.000000 npnn-0.1.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 13:38:03.873239 npnn-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:38:03.873239 npnn-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:38:03.873239 npnn-0.1.0/src/npnn/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-20 13:37:53.000000 npnn-0.1.0/src/npnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-04-20 13:37:53.000000 npnn-0.1.0/src/npnn/autograd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-20 13:37:53.000000 npnn-0.1.0/src/npnn/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-20 13:37:53.000000 npnn-0.1.0/src/npnn/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-20 13:37:53.000000 npnn-0.1.0/src/npnn/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-20 13:37:53.000000 npnn-0.1.0/src/npnn/optim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:38:03.873239 npnn-0.1.0/src/npnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-20 13:38:03.000000 npnn-0.1.0/src/npnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-20 13:38:03.000000 npnn-0.1.0/src/npnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 13:38:03.000000 npnn-0.1.0/src/npnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-20 13:38:03.000000 npnn-0.1.0/src/npnn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-20 13:38:03.000000 npnn-0.1.0/src/npnn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:38:03.873239 npnn-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8749 2024-04-20 13:37:53.000000 npnn-0.1.0/tests/test_autograd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:16:33.444130 npnn-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-26 12:16:23.000000 npnn-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-04-26 12:16:33.444130 npnn-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-26 12:16:23.000000 npnn-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-26 12:16:23.000000 npnn-0.1.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 12:16:33.444130 npnn-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:16:33.440130 npnn-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:16:33.444130 npnn-0.1.1/src/npnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-26 12:16:23.000000 npnn-0.1.1/src/npnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-04-26 12:16:23.000000 npnn-0.1.1/src/npnn/autograd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-26 12:16:23.000000 npnn-0.1.1/src/npnn/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-26 12:16:23.000000 npnn-0.1.1/src/npnn/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-26 12:16:23.000000 npnn-0.1.1/src/npnn/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-26 12:16:23.000000 npnn-0.1.1/src/npnn/optim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:16:33.444130 npnn-0.1.1/src/npnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-04-26 12:16:33.000000 npnn-0.1.1/src/npnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-26 12:16:33.000000 npnn-0.1.1/src/npnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 12:16:33.000000 npnn-0.1.1/src/npnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 12:16:33.000000 npnn-0.1.1/src/npnn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 12:16:33.000000 npnn-0.1.1/src/npnn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:16:33.444130 npnn-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8749 2024-04-26 12:16:23.000000 npnn-0.1.1/tests/test_autograd.py
```

### Comparing `npnn-0.1.0/LICENSE` & `npnn-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `npnn-0.1.0/PKG-INFO` & `npnn-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npnn
-Version: 0.1.0
+Version: 0.1.1
 Summary: NumPy Neural Network
 Author-email: Yang Zhang <mail@yangzhang.site>
 License: MIT License
         
         Copyright (c) 2024 Yang Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,14 +26,17 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/AIboy996/npnn
 Keywords: numpy,neural network,machine learning,autograd
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Provides-Extra: cuda11x
@@ -70,14 +73,18 @@
 check [cupy documentation](https://docs.cupy.dev/en/stable/install.html#installing-cupy) for more information.
 
 
 ### API references
 
 See [npnn WIKI](https://github.com/AIboy996/npnn/wiki).
 
+### Known issues
+
+See [npnn known-issues](https://github.com/AIboy996/npnn/wiki#known-issues).
+
 ## Work with npnn!
 > Here we will construct a image classification neural network with npnn.
 
 BTW, this is a course assignment of *DATA620004, School of Data Science, Fudan University*.
 
 ### Task
 Construct and Train a neural network on [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist) to do image classification.
@@ -91,7 +98,19 @@
 - `dataset.py`: provide Fashion MNIST dataset
 - `model.py`: model definition
 - `train.py`: model training
 - `search.py`: parameters searching
 - `test.py`: model testing
 - `viz.py`: visualization
 - `utils.py`: some misc function, such as `save_model`
+
+run `search.py`, you can get a table like:
+
+no|train_id|accuracy|hidden_size|batch_size|learning_rate|regularization|regular_strength
+--|--|--|--|--|--|--|--
+0|2024_0423(1713841292)|0.8306|[384]|3|0.002|None|0.0
+1|2024_0423(1713845802)|0.8145|[384]|3|0.002|l2|0.1
+2|2024_0423(1713849349)|0.8269|[384]|3|0.002|l2|0.01
+3|2024_0423(1713853939)|0.8255|[384]|3|0.002|l2|0.005
+4|2024_0423(1713857657)|0.8373|[384]|3|0.002|l2|0.001
+
+train log file and saved model weights can be found in `./logs` and `./checkpoints` folder.
```

### Comparing `npnn-0.1.0/readme.md` & `npnn-0.1.1/readme.md`

 * *Files 25% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 check [cupy documentation](https://docs.cupy.dev/en/stable/install.html#installing-cupy) for more information.
 
 
 ### API references
 
 See [npnn WIKI](https://github.com/AIboy996/npnn/wiki).
 
+### Known issues
+
+See [npnn known-issues](https://github.com/AIboy996/npnn/wiki#known-issues).
+
 ## Work with npnn!
 > Here we will construct a image classification neural network with npnn.
 
 BTW, this is a course assignment of *DATA620004, School of Data Science, Fudan University*.
 
 ### Task
 Construct and Train a neural network on [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist) to do image classification.
@@ -47,8 +51,20 @@
 
 - `dataset.py`: provide Fashion MNIST dataset
 - `model.py`: model definition
 - `train.py`: model training
 - `search.py`: parameters searching
 - `test.py`: model testing
 - `viz.py`: visualization
-- `utils.py`: some misc function, such as `save_model`
+- `utils.py`: some misc function, such as `save_model`
+
+run `search.py`, you can get a table like:
+
+no|train_id|accuracy|hidden_size|batch_size|learning_rate|regularization|regular_strength
+--|--|--|--|--|--|--|--
+0|2024_0423(1713841292)|0.8306|[384]|3|0.002|None|0.0
+1|2024_0423(1713845802)|0.8145|[384]|3|0.002|l2|0.1
+2|2024_0423(1713849349)|0.8269|[384]|3|0.002|l2|0.01
+3|2024_0423(1713853939)|0.8255|[384]|3|0.002|l2|0.005
+4|2024_0423(1713857657)|0.8373|[384]|3|0.002|l2|0.001
+
+train log file and saved model weights can be found in `./logs` and `./checkpoints` folder.
```

### Comparing `npnn-0.1.0/src/npnn/autograd.py` & `npnn-0.1.1/src/npnn/autograd.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,10 +152,10 @@
         t.back_childs = self.back_childs
         return t
 
 
 if __name__ == "__main__":
     from .functional import Inner
     x = Tensor(np.random.random((1, 3, 1)), requires_grad=True)
-    loss = Inner()(x.T, x)  # this condition is not included
+    loss = Inner()(x.T, x)  # this case is not considered
     loss.backward()
     print(x.grad)  # we will get a wrong grad.
```

### Comparing `npnn-0.1.0/src/npnn/base.py` & `npnn-0.1.1/src/npnn/base.py`

 * *Files identical despite different names*

### Comparing `npnn-0.1.0/src/npnn/functional.py` & `npnn-0.1.1/src/npnn/functional.py`

 * *Files identical despite different names*

### Comparing `npnn-0.1.0/src/npnn/nn.py` & `npnn-0.1.1/src/npnn/nn.py`

 * *Files identical despite different names*

### Comparing `npnn-0.1.0/src/npnn/optim.py` & `npnn-0.1.1/src/npnn/optim.py`

 * *Files identical despite different names*

### Comparing `npnn-0.1.0/src/npnn.egg-info/PKG-INFO` & `npnn-0.1.1/src/npnn.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npnn
-Version: 0.1.0
+Version: 0.1.1
 Summary: NumPy Neural Network
 Author-email: Yang Zhang <mail@yangzhang.site>
 License: MIT License
         
         Copyright (c) 2024 Yang Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,14 +26,17 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/AIboy996/npnn
 Keywords: numpy,neural network,machine learning,autograd
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Provides-Extra: cuda11x
@@ -70,14 +73,18 @@
 check [cupy documentation](https://docs.cupy.dev/en/stable/install.html#installing-cupy) for more information.
 
 
 ### API references
 
 See [npnn WIKI](https://github.com/AIboy996/npnn/wiki).
 
+### Known issues
+
+See [npnn known-issues](https://github.com/AIboy996/npnn/wiki#known-issues).
+
 ## Work with npnn!
 > Here we will construct a image classification neural network with npnn.
 
 BTW, this is a course assignment of *DATA620004, School of Data Science, Fudan University*.
 
 ### Task
 Construct and Train a neural network on [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist) to do image classification.
@@ -91,7 +98,19 @@
 - `dataset.py`: provide Fashion MNIST dataset
 - `model.py`: model definition
 - `train.py`: model training
 - `search.py`: parameters searching
 - `test.py`: model testing
 - `viz.py`: visualization
 - `utils.py`: some misc function, such as `save_model`
+
+run `search.py`, you can get a table like:
+
+no|train_id|accuracy|hidden_size|batch_size|learning_rate|regularization|regular_strength
+--|--|--|--|--|--|--|--
+0|2024_0423(1713841292)|0.8306|[384]|3|0.002|None|0.0
+1|2024_0423(1713845802)|0.8145|[384]|3|0.002|l2|0.1
+2|2024_0423(1713849349)|0.8269|[384]|3|0.002|l2|0.01
+3|2024_0423(1713853939)|0.8255|[384]|3|0.002|l2|0.005
+4|2024_0423(1713857657)|0.8373|[384]|3|0.002|l2|0.001
+
+train log file and saved model weights can be found in `./logs` and `./checkpoints` folder.
```

### Comparing `npnn-0.1.0/tests/test_autograd.py` & `npnn-0.1.1/tests/test_autograd.py`

 * *Files identical despite different names*

