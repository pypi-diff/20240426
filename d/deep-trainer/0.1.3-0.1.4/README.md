# Comparing `tmp/deep-trainer-0.1.3.tar.gz` & `tmp/deep_trainer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep-trainer-0.1.3.tar", last modified: Thu Feb 15 21:22:49 2024, max compression
+gzip compressed data, was "deep_trainer-0.1.4.tar", last modified: Fri Apr 26 10:04:05 2024, max compression
```

## Comparing `deep-trainer-0.1.3.tar` & `deep_trainer-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 21:22:49.043204 deep-trainer-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-15 21:22:39.000000 deep-trainer-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-02-15 21:22:49.043204 deep-trainer-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-02-15 21:22:39.000000 deep-trainer-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 21:22:49.039204 deep-trainer-0.1.3/deep_trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-15 21:22:39.000000 deep-trainer-0.1.3/deep_trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 21:22:39.000000 deep-trainer-0.1.3/deep_trainer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 21:22:49.043204 deep-trainer-0.1.3/deep_trainer/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 21:22:39.000000 deep-trainer-0.1.3/deep_trainer/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-02-15 21:22:39.000000 deep-trainer-0.1.3/deep_trainer/pytorch/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    19733 2024-02-15 21:22:39.000000 deep-trainer-0.1.3/deep_trainer/pytorch/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    22516 2024-02-15 21:22:39.000000 deep-trainer-0.1.3/deep_trainer/pytorch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 21:22:49.043204 deep-trainer-0.1.3/deep_trainer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-02-15 21:22:49.000000 deep-trainer-0.1.3/deep_trainer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-02-15 21:22:49.000000 deep-trainer-0.1.3/deep_trainer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 21:22:49.000000 deep-trainer-0.1.3/deep_trainer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-15 21:22:49.000000 deep-trainer-0.1.3/deep_trainer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-15 21:22:49.000000 deep-trainer-0.1.3/deep_trainer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-15 21:22:39.000000 deep-trainer-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-02-15 21:22:49.043204 deep-trainer-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-15 21:22:39.000000 deep-trainer-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:04:05.092712 deep_trainer-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 10:03:59.000000 deep_trainer-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-26 10:04:05.092712 deep_trainer-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-26 10:03:59.000000 deep_trainer-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:04:05.088713 deep_trainer-0.1.4/deep_trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-26 10:03:59.000000 deep_trainer-0.1.4/deep_trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:03:59.000000 deep_trainer-0.1.4/deep_trainer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:04:05.092712 deep_trainer-0.1.4/deep_trainer/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:03:59.000000 deep_trainer-0.1.4/deep_trainer/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-26 10:03:59.000000 deep_trainer-0.1.4/deep_trainer/pytorch/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19733 2024-04-26 10:03:59.000000 deep_trainer-0.1.4/deep_trainer/pytorch/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22516 2024-04-26 10:03:59.000000 deep_trainer-0.1.4/deep_trainer/pytorch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:04:05.092712 deep_trainer-0.1.4/deep_trainer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-26 10:04:05.000000 deep_trainer-0.1.4/deep_trainer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-26 10:04:05.000000 deep_trainer-0.1.4/deep_trainer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:04:05.000000 deep_trainer-0.1.4/deep_trainer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-26 10:04:05.000000 deep_trainer-0.1.4/deep_trainer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-26 10:04:05.000000 deep_trainer-0.1.4/deep_trainer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-26 10:03:59.000000 deep_trainer-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-26 10:04:05.092712 deep_trainer-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 10:03:59.000000 deep_trainer-0.1.4/setup.py
```

### Comparing `deep-trainer-0.1.3/LICENSE` & `deep_trainer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deep-trainer-0.1.3/PKG-INFO` & `deep_trainer-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: deep-trainer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Helper to train deep neural networks
 Home-page: https://github.com/raphaelreme/deep-trainer
 Author: Raphael Reme
 Author-email: raphaelreme-dev@protonmail.com
 License: MIT
 Keywords: deep learning,pytorch
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tensorboard
 Requires-Dist: torch
 Requires-Dist: tqdm
```

### Comparing `deep-trainer-0.1.3/README.md` & `deep_trainer-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `deep-trainer-0.1.3/deep_trainer/pytorch/logging.py` & `deep_trainer-0.1.4/deep_trainer/pytorch/logging.py`

 * *Files identical despite different names*

### Comparing `deep-trainer-0.1.3/deep_trainer/pytorch/metric.py` & `deep_trainer-0.1.4/deep_trainer/pytorch/metric.py`

 * *Files identical despite different names*

### Comparing `deep-trainer-0.1.3/deep_trainer/pytorch/trainer.py` & `deep_trainer-0.1.4/deep_trainer/pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `deep-trainer-0.1.3/deep_trainer.egg-info/PKG-INFO` & `deep_trainer-0.1.4/deep_trainer.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: deep-trainer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Helper to train deep neural networks
 Home-page: https://github.com/raphaelreme/deep-trainer
 Author: Raphael Reme
 Author-email: raphaelreme-dev@protonmail.com
 License: MIT
 Keywords: deep learning,pytorch
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tensorboard
 Requires-Dist: torch
 Requires-Dist: tqdm
```

### Comparing `deep-trainer-0.1.3/setup.cfg` & `deep_trainer-0.1.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 keywords = deep learning, pytorch
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/raphaelreme/deep-trainer
 project_urls = 
 classifiers = 
-	Development Status :: 2 - Pre-Alpha
+	Development Status :: 4 - Beta
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 
 [options]
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	tensorboard
 	torch
```

