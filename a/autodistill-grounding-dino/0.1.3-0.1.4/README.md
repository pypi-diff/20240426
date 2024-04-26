# Comparing `tmp/autodistill-grounding-dino-0.1.3.tar.gz` & `tmp/autodistill-grounding-dino-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-grounding-dino-0.1.3.tar", last modified: Tue Dec  5 09:07:51 2023, max compression
+gzip compressed data, was "autodistill-grounding-dino-0.1.4.tar", last modified: Fri Apr 26 15:36:15 2024, max compression
```

## Comparing `autodistill-grounding-dino-0.1.3.tar` & `autodistill-grounding-dino-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,16 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-12-05 09:07:51.621418 autodistill-grounding-dino-0.1.3/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-12-05 09:07:51.616871 autodistill-grounding-dino-0.1.3/.github/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-12-05 09:07:51.618920 autodistill-grounding-dino-0.1.3/.github/workflows/
--rw-r--r--   0 james      (501) staff       (20)      954 2023-12-01 17:06:14.000000 autodistill-grounding-dino-0.1.3/.github/workflows/publish.yml
--rw-r--r--   0 james      (501) staff       (20)      749 2023-12-01 17:06:14.000000 autodistill-grounding-dino-0.1.3/.github/workflows/test.yml
--rw-r--r--   0 james      (501) staff       (20)      539 2023-12-01 17:06:14.000000 autodistill-grounding-dino-0.1.3/.github/workflows/welcome.yml
--rw-r--r--   0 james      (501) staff       (20)     1799 2023-12-01 17:06:14.000000 autodistill-grounding-dino-0.1.3/.gitignore
--rw-r--r--   0 james      (501) staff       (20)    11356 2023-12-01 17:06:14.000000 autodistill-grounding-dino-0.1.3/LICENSE
--rw-r--r--   0 james      (501) staff       (20)      865 2023-12-01 17:06:14.000000 autodistill-grounding-dino-0.1.3/Makefile
--rw-r--r--   0 james      (501) staff       (20)     2784 2023-12-05 09:07:51.621187 autodistill-grounding-dino-0.1.3/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1847 2023-12-01 17:06:14.000000 autodistill-grounding-dino-0.1.3/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-12-05 09:07:51.619501 autodistill-grounding-dino-0.1.3/autodistill_grounding_dino/
--rw-r--r--   0 james      (501) staff       (20)       97 2023-12-05 09:07:46.000000 autodistill-grounding-dino-0.1.3/autodistill_grounding_dino/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1742 2023-12-05 09:06:07.000000 autodistill-grounding-dino-0.1.3/autodistill_grounding_dino/grounding_dino_model.py
--rw-r--r--   0 james      (501) staff       (20)     3529 2023-12-05 09:06:07.000000 autodistill-grounding-dino-0.1.3/autodistill_grounding_dino/helpers.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-12-05 09:07:51.620534 autodistill-grounding-dino-0.1.3/autodistill_grounding_dino.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     2784 2023-12-05 09:07:51.000000 autodistill-grounding-dino-0.1.3/autodistill_grounding_dino.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      510 2023-12-05 09:07:51.000000 autodistill-grounding-dino-0.1.3/autodistill_grounding_dino.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-12-05 09:07:51.000000 autodistill-grounding-dino-0.1.3/autodistill_grounding_dino.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      155 2023-12-05 09:07:51.000000 autodistill-grounding-dino-0.1.3/autodistill_grounding_dino.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       27 2023-12-05 09:07:51.000000 autodistill-grounding-dino-0.1.3/autodistill_grounding_dino.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-12-05 09:07:51.621464 autodistill-grounding-dino-0.1.3/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1289 2023-12-01 17:06:14.000000 autodistill-grounding-dino-0.1.3/setup.py
+drwxr-xr-x   0 lake       (502) staff       (20)        0 2024-04-26 15:36:15.895975 autodistill-grounding-dino-0.1.4/
+-rw-r--r--   0 lake       (502) staff       (20)    11356 2024-03-19 16:15:31.000000 autodistill-grounding-dino-0.1.4/LICENSE
+-rw-r--r--   0 lake       (502) staff       (20)     2992 2024-04-26 15:36:15.895734 autodistill-grounding-dino-0.1.4/PKG-INFO
+-rw-r--r--   0 lake       (502) staff       (20)     2048 2024-03-21 17:53:56.000000 autodistill-grounding-dino-0.1.4/README.md
+drwxr-xr-x   0 lake       (502) staff       (20)        0 2024-04-26 15:36:15.894218 autodistill-grounding-dino-0.1.4/autodistill_grounding_dino/
+-rw-r--r--   0 lake       (502) staff       (20)       97 2024-04-26 15:32:56.000000 autodistill-grounding-dino-0.1.4/autodistill_grounding_dino/__init__.py
+-rw-r--r--   0 lake       (502) staff       (20)     1742 2024-03-19 16:15:31.000000 autodistill-grounding-dino-0.1.4/autodistill_grounding_dino/grounding_dino_model.py
+-rw-r--r--   0 lake       (502) staff       (20)     3529 2024-03-19 16:15:31.000000 autodistill-grounding-dino-0.1.4/autodistill_grounding_dino/helpers.py
+drwxr-xr-x   0 lake       (502) staff       (20)        0 2024-04-26 15:36:15.895050 autodistill-grounding-dino-0.1.4/autodistill_grounding_dino.egg-info/
+-rw-r--r--   0 lake       (502) staff       (20)     2992 2024-04-26 15:36:15.000000 autodistill-grounding-dino-0.1.4/autodistill_grounding_dino.egg-info/PKG-INFO
+-rw-r--r--   0 lake       (502) staff       (20)      403 2024-04-26 15:36:15.000000 autodistill-grounding-dino-0.1.4/autodistill_grounding_dino.egg-info/SOURCES.txt
+-rw-r--r--   0 lake       (502) staff       (20)        1 2024-04-26 15:36:15.000000 autodistill-grounding-dino-0.1.4/autodistill_grounding_dino.egg-info/dependency_links.txt
+-rw-r--r--   0 lake       (502) staff       (20)      162 2024-04-26 15:36:15.000000 autodistill-grounding-dino-0.1.4/autodistill_grounding_dino.egg-info/requires.txt
+-rw-r--r--   0 lake       (502) staff       (20)       27 2024-04-26 15:36:15.000000 autodistill-grounding-dino-0.1.4/autodistill_grounding_dino.egg-info/top_level.txt
+-rw-r--r--   0 lake       (502) staff       (20)       38 2024-04-26 15:36:15.896029 autodistill-grounding-dino-0.1.4/setup.cfg
+-rw-r--r--   0 lake       (502) staff       (20)     1296 2024-04-26 15:31:48.000000 autodistill-grounding-dino-0.1.4/setup.py
```

### Comparing `autodistill-grounding-dino-0.1.3/LICENSE` & `autodistill-grounding-dino-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autodistill-grounding-dino-0.1.3/PKG-INFO` & `autodistill-grounding-dino-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: autodistill-grounding-dino
-Version: 0.1.3
+Version: 0.1.4
 Summary: GroundingDINO module for use with Autodistill
 Home-page: https://github.com/autodistill/autodistill-grounding-dino
 Author: Roboflow
 Author-email: support@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: autodistill
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: opencv-python>=4.6.0
-Requires-Dist: rf_groundingdino
+Requires-Dist: rf_groundingdino==0.1.2
 Requires-Dist: rf_segment_anything
 Requires-Dist: supervision
 Provides-Extra: dev
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: black==22.3.0; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: twine; extra == "dev"
@@ -41,14 +41,17 @@
 
 This repository contains the code supporting the Grounding DINO base model for use with [Autodistill](https://github.com/autodistill/autodistill).
 
 [Grounding DINO](https://github.com/IDEA-Research/GroundingDINO) is a zero-shot object detection model developed by IDEA Research. You can distill knowledge from Grounding DINO into a smaller model using Autodistill.
 
 Read the [Grounding DINO Autodistill documentation](https://autodistill.github.io/autodistill/base_models/grounding-dino/).
 
+> [!TIP]
+> You can use Autodistill Grounding DINO on your own hardware, or use the [Roboflow hosted version of Autodistill](https://blog.roboflow.com/launch-auto-label/) to label images in the cloud.
+
 ## Installation
 
 To use the Grounding DINO base model, you will need to install the following dependency:
 
 ```bash
 pip3 install autodistill-grounding-dino
 ```
```

### Comparing `autodistill-grounding-dino-0.1.3/README.md` & `autodistill-grounding-dino-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
 This repository contains the code supporting the Grounding DINO base model for use with [Autodistill](https://github.com/autodistill/autodistill).
 
 [Grounding DINO](https://github.com/IDEA-Research/GroundingDINO) is a zero-shot object detection model developed by IDEA Research. You can distill knowledge from Grounding DINO into a smaller model using Autodistill.
 
 Read the [Grounding DINO Autodistill documentation](https://autodistill.github.io/autodistill/base_models/grounding-dino/).
 
+> [!TIP]
+> You can use Autodistill Grounding DINO on your own hardware, or use the [Roboflow hosted version of Autodistill](https://blog.roboflow.com/launch-auto-label/) to label images in the cloud.
+
 ## Installation
 
 To use the Grounding DINO base model, you will need to install the following dependency:
 
 ```bash
 pip3 install autodistill-grounding-dino
 ```
```

### Comparing `autodistill-grounding-dino-0.1.3/autodistill_grounding_dino/grounding_dino_model.py` & `autodistill-grounding-dino-0.1.4/autodistill_grounding_dino/grounding_dino_model.py`

 * *Files identical despite different names*

### Comparing `autodistill-grounding-dino-0.1.3/autodistill_grounding_dino/helpers.py` & `autodistill-grounding-dino-0.1.4/autodistill_grounding_dino/helpers.py`

 * *Files identical despite different names*

### Comparing `autodistill-grounding-dino-0.1.3/autodistill_grounding_dino.egg-info/PKG-INFO` & `autodistill-grounding-dino-0.1.4/autodistill_grounding_dino.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: autodistill-grounding-dino
-Version: 0.1.3
+Version: 0.1.4
 Summary: GroundingDINO module for use with Autodistill
 Home-page: https://github.com/autodistill/autodistill-grounding-dino
 Author: Roboflow
 Author-email: support@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: autodistill
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: opencv-python>=4.6.0
-Requires-Dist: rf_groundingdino
+Requires-Dist: rf_groundingdino==0.1.2
 Requires-Dist: rf_segment_anything
 Requires-Dist: supervision
 Provides-Extra: dev
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: black==22.3.0; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: twine; extra == "dev"
@@ -41,14 +41,17 @@
 
 This repository contains the code supporting the Grounding DINO base model for use with [Autodistill](https://github.com/autodistill/autodistill).
 
 [Grounding DINO](https://github.com/IDEA-Research/GroundingDINO) is a zero-shot object detection model developed by IDEA Research. You can distill knowledge from Grounding DINO into a smaller model using Autodistill.
 
 Read the [Grounding DINO Autodistill documentation](https://autodistill.github.io/autodistill/base_models/grounding-dino/).
 
+> [!TIP]
+> You can use Autodistill Grounding DINO on your own hardware, or use the [Roboflow hosted version of Autodistill](https://blog.roboflow.com/launch-auto-label/) to label images in the cloud.
+
 ## Installation
 
 To use the Grounding DINO base model, you will need to install the following dependency:
 
 ```bash
 pip3 install autodistill-grounding-dino
 ```
```

### Comparing `autodistill-grounding-dino-0.1.3/setup.py` & `autodistill-grounding-dino-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     long_description_content_type="text/markdown",
     url="https://github.com/autodistill/autodistill-grounding-dino",
     install_requires=[
         "torch",
         "autodistill",
         "numpy>=1.20.0",
         "opencv-python>=4.6.0",
-        "rf_groundingdino",
+        "rf_groundingdino==0.1.2",
         "rf_segment_anything",
         "supervision"
     ],
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel"],
     },
```

