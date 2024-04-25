# Comparing `tmp/gingerai-0.1.6.tar.gz` & `tmp/gingerai-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gingerai-0.1.6.tar", last modified: Thu Apr 25 13:54:14 2024, max compression
+gzip compressed data, was "gingerai-0.1.7.tar", last modified: Thu Apr 25 13:56:14 2024, max compression
```

## Comparing `gingerai-0.1.6.tar` & `gingerai-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:54:14.976819 gingerai-0.1.6/
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      340 2024-04-25 13:54:14.976819 gingerai-0.1.6/PKG-INFO
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:54:14.000000 gingerai-0.1.6/README.md
-drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:54:14.976819 gingerai-0.1.6/gingerai/
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)     1291 2024-04-25 13:54:14.000000 gingerai-0.1.6/gingerai/TorchNetWrapper.py
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)       82 2024-04-25 13:54:14.000000 gingerai-0.1.6/gingerai/__init__.py
-drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:54:14.976819 gingerai-0.1.6/gingerai.egg-info/
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      340 2024-04-25 13:54:14.000000 gingerai-0.1.6/gingerai.egg-info/PKG-INFO
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      226 2024-04-25 13:54:14.000000 gingerai-0.1.6/gingerai.egg-info/SOURCES.txt
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        1 2024-04-25 13:54:14.000000 gingerai-0.1.6/gingerai.egg-info/dependency_links.txt
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        6 2024-04-25 13:54:14.000000 gingerai-0.1.6/gingerai.egg-info/requires.txt
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        9 2024-04-25 13:54:14.000000 gingerai-0.1.6/gingerai.egg-info/top_level.txt
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)       38 2024-04-25 13:54:14.976819 gingerai-0.1.6/setup.cfg
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      439 2024-04-25 13:54:14.000000 gingerai-0.1.6/setup.py
+drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:56:14.516857 gingerai-0.1.7/
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      340 2024-04-25 13:56:14.516857 gingerai-0.1.7/PKG-INFO
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:56:14.000000 gingerai-0.1.7/README.md
+drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:56:14.516857 gingerai-0.1.7/gingerai/
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)     1790 2024-04-25 13:56:14.000000 gingerai-0.1.7/gingerai/TorchNetWrapper.py
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)       82 2024-04-25 13:56:14.000000 gingerai-0.1.7/gingerai/__init__.py
+drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:56:14.516857 gingerai-0.1.7/gingerai.egg-info/
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      340 2024-04-25 13:56:14.000000 gingerai-0.1.7/gingerai.egg-info/PKG-INFO
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      226 2024-04-25 13:56:14.000000 gingerai-0.1.7/gingerai.egg-info/SOURCES.txt
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        1 2024-04-25 13:56:14.000000 gingerai-0.1.7/gingerai.egg-info/dependency_links.txt
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        6 2024-04-25 13:56:14.000000 gingerai-0.1.7/gingerai.egg-info/requires.txt
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        9 2024-04-25 13:56:14.000000 gingerai-0.1.7/gingerai.egg-info/top_level.txt
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)       38 2024-04-25 13:56:14.516857 gingerai-0.1.7/setup.cfg
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      439 2024-04-25 13:56:14.000000 gingerai-0.1.7/setup.py
```

### Comparing `gingerai-0.1.6/gingerai/TorchNetWrapper.py` & `gingerai-0.1.7/gingerai/TorchNetWrapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,21 +26,31 @@
 
     @staticmethod
     def load_torch_model(ginger_path):
         try:
             with open(ginger_path, "rb") as f:
                 loaded_data = pickle.load(f)
 
-            new_instance = TorchNetWrapper()
-
-            for key, value in loaded_data.__dict__.items():
-                setattr(new_instance, key, value)
+            model = getattr(loaded_data, "model", None)
+            optimizer = getattr(loaded_data, "optimizer", None)
+            loss = getattr(loaded_data, "loss", None)
+            dataset = getattr(loaded_data, "dataset", None)
+
+            if model is None or optimizer is None or loss is None or dataset is None:
+                raise ValueError("One or more required attributes are missing.")
+
+            new_instance = TorchNetWrapper(
+                model=model, optimizer=optimizer, loss_fn=loss, dataset=dataset
+            )
 
             return new_instance
 
         except (pickle.UnpicklingError, AttributeError, KeyError) as e:
+            # Handle specific errors, provide useful feedback
             print(f"Error loading model from {ginger_path}: {e}")
             raise
 
         except Exception as e:
+            # Catch all other exceptions and raise
             print(f"An unexpected error occurred: {e}")
             raise
+
```

