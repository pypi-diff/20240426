# Comparing `tmp/synthemol-1.0.2.tar.gz` & `tmp/synthemol-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthemol-1.0.2.tar", last modified: Fri Mar 22 07:03:30 2024, max compression
+gzip compressed data, was "synthemol-1.0.3.tar", last modified: Fri Apr 26 06:20:10 2024, max compression
```

## Comparing `synthemol-1.0.2.tar` & `synthemol-1.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-03-22 07:03:30.818123 synthemol-1.0.2/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1069 2024-03-22 07:03:16.000000 synthemol-1.0.2/LICENSE
--rw-r--r--   0 kyleswanson   (501) staff       (20)     9957 2024-03-22 07:03:30.818393 synthemol-1.0.2/PKG-INFO
--rw-r--r--   0 kyleswanson   (501) staff       (20)     9182 2024-03-22 07:03:16.000000 synthemol-1.0.2/README.md
--rw-r--r--   0 kyleswanson   (501) staff       (20)       79 2024-03-22 07:03:30.818919 synthemol-1.0.2/setup.cfg
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1776 2024-03-22 07:03:16.000000 synthemol-1.0.2/setup.py
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-03-22 07:03:30.670771 synthemol-1.0.2/synthemol/
--rw-r--r--   0 kyleswanson   (501) staff       (20)      169 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/__init__.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      177 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/_version.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1563 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/constants.py
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-03-22 07:03:30.678389 synthemol-1.0.2/synthemol/generate/
--rw-r--r--   0 kyleswanson   (501) staff       (20)      273 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/generate/__init__.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     8554 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/generate/generate.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)    19287 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/generate/generator.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     4194 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/generate/node.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     6343 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/generate/utils.py
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-03-22 07:03:30.680530 synthemol-1.0.2/synthemol/models/
--rw-r--r--   0 kyleswanson   (501) staff       (20)      362 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/models/__init__.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2562 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/models/chemprop_models.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2394 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/models/sklearn_models.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)       27 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/py.typed
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-03-22 07:03:30.684944 synthemol-1.0.2/synthemol/reactions/
--rw-r--r--   0 kyleswanson   (501) staff       (20)      499 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/reactions/__init__.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      396 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/reactions/custom.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     4214 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/reactions/query_mol.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2340 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/reactions/reaction.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     3371 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/reactions/real.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1754 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/reactions/utils.py
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-03-22 07:03:30.666850 synthemol-1.0.2/synthemol/resources/
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-03-22 07:03:30.740339 synthemol-1.0.2/synthemol/resources/real/
--rw-r--r--   0 kyleswanson   (501) staff       (20)  4476164 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/resources/real/building_blocks.csv
--rw-r--r--   0 kyleswanson   (501) staff       (20)  4274772 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/resources/real/reaction_to_building_blocks.pkl
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1662 2024-03-22 07:03:16.000000 synthemol-1.0.2/synthemol/utils.py
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-03-22 07:03:30.674183 synthemol-1.0.2/synthemol.egg-info/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     9957 2024-03-22 07:03:30.000000 synthemol-1.0.2/synthemol.egg-info/PKG-INFO
--rw-r--r--   0 kyleswanson   (501) staff       (20)      876 2024-03-22 07:03:30.000000 synthemol-1.0.2/synthemol.egg-info/SOURCES.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)        1 2024-03-22 07:03:30.000000 synthemol-1.0.2/synthemol.egg-info/dependency_links.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       80 2024-03-22 07:03:30.000000 synthemol-1.0.2/synthemol.egg-info/entry_points.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)      123 2024-03-22 07:03:30.000000 synthemol-1.0.2/synthemol.egg-info/requires.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       10 2024-03-22 07:03:30.000000 synthemol-1.0.2/synthemol.egg-info/top_level.txt
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-04-26 06:20:10.937811 synthemol-1.0.3/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1069 2023-12-05 08:22:12.000000 synthemol-1.0.3/LICENSE
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     9957 2024-04-26 06:20:10.938025 synthemol-1.0.3/PKG-INFO
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     9182 2024-04-26 06:19:57.000000 synthemol-1.0.3/README.md
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       79 2024-04-26 06:20:10.938618 synthemol-1.0.3/setup.cfg
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1783 2024-04-26 06:19:57.000000 synthemol-1.0.3/setup.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-04-26 06:20:10.885696 synthemol-1.0.3/synthemol/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      169 2023-12-05 08:22:12.000000 synthemol-1.0.3/synthemol/__init__.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      177 2024-04-26 06:19:57.000000 synthemol-1.0.3/synthemol/_version.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1563 2024-04-26 06:19:57.000000 synthemol-1.0.3/synthemol/constants.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-04-26 06:20:10.891173 synthemol-1.0.3/synthemol/generate/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      273 2024-04-26 06:19:57.000000 synthemol-1.0.3/synthemol/generate/__init__.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     8554 2024-04-26 06:19:57.000000 synthemol-1.0.3/synthemol/generate/generate.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)    19287 2024-04-26 06:19:57.000000 synthemol-1.0.3/synthemol/generate/generator.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4194 2024-04-26 06:19:57.000000 synthemol-1.0.3/synthemol/generate/node.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     6343 2024-04-26 06:19:57.000000 synthemol-1.0.3/synthemol/generate/utils.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-04-26 06:20:10.892890 synthemol-1.0.3/synthemol/models/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      362 2024-04-26 06:19:57.000000 synthemol-1.0.3/synthemol/models/__init__.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2562 2024-04-26 06:19:57.000000 synthemol-1.0.3/synthemol/models/chemprop_models.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2394 2024-04-26 06:19:57.000000 synthemol-1.0.3/synthemol/models/sklearn_models.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       27 2023-12-05 08:22:12.000000 synthemol-1.0.3/synthemol/py.typed
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-04-26 06:20:10.895761 synthemol-1.0.3/synthemol/reactions/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      499 2024-04-26 06:19:57.000000 synthemol-1.0.3/synthemol/reactions/__init__.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      396 2024-04-26 06:19:57.000000 synthemol-1.0.3/synthemol/reactions/custom.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4214 2024-04-26 06:19:57.000000 synthemol-1.0.3/synthemol/reactions/query_mol.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2340 2024-04-26 06:19:57.000000 synthemol-1.0.3/synthemol/reactions/reaction.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     3371 2024-04-26 06:19:57.000000 synthemol-1.0.3/synthemol/reactions/real.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1754 2024-04-26 06:19:57.000000 synthemol-1.0.3/synthemol/reactions/utils.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-04-26 06:20:10.881472 synthemol-1.0.3/synthemol/resources/
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-04-26 06:20:10.909505 synthemol-1.0.3/synthemol/resources/real/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)  4476164 2024-04-11 04:19:03.000000 synthemol-1.0.3/synthemol/resources/real/building_blocks.csv
+-rw-r--r--   0 kyleswanson   (501) staff       (20)  4274772 2023-12-05 08:22:27.000000 synthemol-1.0.3/synthemol/resources/real/reaction_to_building_blocks.pkl
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1662 2024-04-26 06:19:57.000000 synthemol-1.0.3/synthemol/utils.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-04-26 06:20:10.888366 synthemol-1.0.3/synthemol.egg-info/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     9957 2024-04-26 06:20:10.000000 synthemol-1.0.3/synthemol.egg-info/PKG-INFO
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      876 2024-04-26 06:20:10.000000 synthemol-1.0.3/synthemol.egg-info/SOURCES.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)        1 2024-04-26 06:20:10.000000 synthemol-1.0.3/synthemol.egg-info/dependency_links.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       80 2024-04-26 06:20:10.000000 synthemol-1.0.3/synthemol.egg-info/entry_points.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      130 2024-04-26 06:20:10.000000 synthemol-1.0.3/synthemol.egg-info/requires.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       10 2024-04-26 06:20:10.000000 synthemol-1.0.3/synthemol.egg-info/top_level.txt
```

### Comparing `synthemol-1.0.2/LICENSE` & `synthemol-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `synthemol-1.0.2/PKG-INFO` & `synthemol-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: synthemol
-Version: 1.0.2
+Version: 1.0.3
 Summary: synthemol
 Home-page: https://github.com/swansonk14/SyntheMol
-Download-URL: https://github.com/swansonk14/SyntheMol/archive/refs/tags/v_1.0.2.tar.gz
+Download-URL: https://github.com/swansonk14/SyntheMol/archive/refs/tags/v_1.0.3.tar.gz
 Author: Kyle Swanson
 Author-email: swansonk.14@gmail.com
 License: MIT
 Keywords: machine learning,drug design,generative models,synthesizable molecules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `synthemol-1.0.2/README.md` & `synthemol-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `synthemol-1.0.2/setup.py` & `synthemol-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     entry_points={
         'console_scripts': [
             'synthemol=synthemol.generate.generate:generate_command_line'
         ]
     },
     install_requires=[
         'chemfunc',
-        'chemprop',
+        'chemprop==1.6.1',
         'descriptastorus',
         'matplotlib',
         'numpy',
         'pandas',
         'torch',
         'rdkit',
         'scikit-learn',
```

### Comparing `synthemol-1.0.2/synthemol/constants.py` & `synthemol-1.0.3/synthemol/constants.py`

 * *Files identical despite different names*

### Comparing `synthemol-1.0.2/synthemol/generate/generate.py` & `synthemol-1.0.3/synthemol/generate/generate.py`

 * *Files identical despite different names*

### Comparing `synthemol-1.0.2/synthemol/generate/generator.py` & `synthemol-1.0.3/synthemol/generate/generator.py`

 * *Files identical despite different names*

### Comparing `synthemol-1.0.2/synthemol/generate/node.py` & `synthemol-1.0.3/synthemol/generate/node.py`

 * *Files identical despite different names*

### Comparing `synthemol-1.0.2/synthemol/generate/utils.py` & `synthemol-1.0.3/synthemol/generate/utils.py`

 * *Files identical despite different names*

### Comparing `synthemol-1.0.2/synthemol/models/chemprop_models.py` & `synthemol-1.0.3/synthemol/models/chemprop_models.py`

 * *Files identical despite different names*

### Comparing `synthemol-1.0.2/synthemol/models/sklearn_models.py` & `synthemol-1.0.3/synthemol/models/sklearn_models.py`

 * *Files identical despite different names*

### Comparing `synthemol-1.0.2/synthemol/reactions/query_mol.py` & `synthemol-1.0.3/synthemol/reactions/query_mol.py`

 * *Files identical despite different names*

### Comparing `synthemol-1.0.2/synthemol/reactions/reaction.py` & `synthemol-1.0.3/synthemol/reactions/reaction.py`

 * *Files identical despite different names*

### Comparing `synthemol-1.0.2/synthemol/reactions/real.py` & `synthemol-1.0.3/synthemol/reactions/real.py`

 * *Files identical despite different names*

### Comparing `synthemol-1.0.2/synthemol/reactions/utils.py` & `synthemol-1.0.3/synthemol/reactions/utils.py`

 * *Files identical despite different names*

### Comparing `synthemol-1.0.2/synthemol/resources/real/building_blocks.csv` & `synthemol-1.0.3/synthemol/resources/real/building_blocks.csv`

 * *Files identical despite different names*

### Comparing `synthemol-1.0.2/synthemol/resources/real/reaction_to_building_blocks.pkl` & `synthemol-1.0.3/synthemol/resources/real/reaction_to_building_blocks.pkl`

 * *Files identical despite different names*

### Comparing `synthemol-1.0.2/synthemol/utils.py` & `synthemol-1.0.3/synthemol/utils.py`

 * *Files identical despite different names*

### Comparing `synthemol-1.0.2/synthemol.egg-info/PKG-INFO` & `synthemol-1.0.3/synthemol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: synthemol
-Version: 1.0.2
+Version: 1.0.3
 Summary: synthemol
 Home-page: https://github.com/swansonk14/SyntheMol
-Download-URL: https://github.com/swansonk14/SyntheMol/archive/refs/tags/v_1.0.2.tar.gz
+Download-URL: https://github.com/swansonk14/SyntheMol/archive/refs/tags/v_1.0.3.tar.gz
 Author: Kyle Swanson
 Author-email: swansonk.14@gmail.com
 License: MIT
 Keywords: machine learning,drug design,generative models,synthesizable molecules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `synthemol-1.0.2/synthemol.egg-info/SOURCES.txt` & `synthemol-1.0.3/synthemol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

