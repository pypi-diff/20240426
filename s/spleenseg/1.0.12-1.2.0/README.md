# Comparing `tmp/spleenseg-1.0.12.tar.gz` & `tmp/spleenseg-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spleenseg-1.0.12.tar", last modified: Mon Apr 22 21:53:49 2024, max compression
+gzip compressed data, was "spleenseg-1.2.0.tar", last modified: Thu Apr 25 23:02:46 2024, max compression
```

## Comparing `spleenseg-1.0.12.tar` & `spleenseg-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-22 21:53:49.930040 spleenseg-1.0.12/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1069 2024-04-17 00:36:10.000000 spleenseg-1.0.12/LICENSE
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     7390 2024-04-22 21:53:49.930040 spleenseg-1.0.12/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     6405 2024-04-17 00:36:10.000000 spleenseg-1.0.12/README.md
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     6841 2024-04-22 21:53:48.000000 spleenseg-1.0.12/README.rst
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      223 2024-04-22 15:37:24.000000 spleenseg-1.0.12/requirements.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2024-04-22 21:53:49.930040 spleenseg-1.0.12/setup.cfg
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1848 2024-04-22 21:52:34.000000 spleenseg-1.0.12/setup.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-22 21:53:49.930040 spleenseg-1.0.12/spleenseg/
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-22 21:53:49.930040 spleenseg-1.0.12/spleenseg/core/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    16445 2024-04-22 15:45:59.000000 spleenseg-1.0.12/spleenseg/core/neuralnet.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-22 21:53:49.930040 spleenseg-1.0.12/spleenseg/plotting/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     2038 2024-04-22 00:20:53.000000 spleenseg-1.0.12/spleenseg/plotting/plotting.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     8543 2024-04-22 21:53:21.000000 spleenseg-1.0.12/spleenseg/spleenseg.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-22 21:53:49.930040 spleenseg-1.0.12/spleenseg/transforms/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     7626 2024-04-22 00:04:43.000000 spleenseg-1.0.12/spleenseg/transforms/transforms.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-22 21:53:49.930040 spleenseg-1.0.12/spleenseg.egg-info/
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     7390 2024-04-22 21:53:49.000000 spleenseg-1.0.12/spleenseg.egg-info/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      393 2024-04-22 21:53:49.000000 spleenseg-1.0.12/spleenseg.egg-info/SOURCES.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2024-04-22 21:53:49.000000 spleenseg-1.0.12/spleenseg.egg-info/dependency_links.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       55 2024-04-22 21:53:49.000000 spleenseg-1.0.12/spleenseg.egg-info/entry_points.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      247 2024-04-22 21:53:49.000000 spleenseg-1.0.12/spleenseg.egg-info/requires.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       65 2024-04-22 21:53:49.000000 spleenseg-1.0.12/spleenseg.egg-info/top_level.txt
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-22 21:53:49.930040 spleenseg-1.0.12/tests/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      662 2024-04-17 00:36:10.000000 spleenseg-1.0.12/tests/test_example.py
+drwxrwxr-x   0 rudolphpienaar (2090878) domain_users (2000513)        0 2024-04-25 23:02:46.936343 spleenseg-1.2.0/
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)     1069 2024-04-23 22:06:23.000000 spleenseg-1.2.0/LICENSE
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)     7410 2024-04-25 23:02:46.932847 spleenseg-1.2.0/PKG-INFO
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)     6842 2024-04-25 23:02:44.000000 spleenseg-1.2.0/README.rst
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)      223 2024-04-23 22:06:23.000000 spleenseg-1.2.0/requirements.txt
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)       38 2024-04-25 23:02:46.938648 spleenseg-1.2.0/setup.cfg
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)     1848 2024-04-23 22:06:23.000000 spleenseg-1.2.0/setup.py
+drwxrwxr-x   0 rudolphpienaar (2090878) domain_users (2000513)        0 2024-04-25 23:02:46.810794 spleenseg-1.2.0/spleenseg/
+drwxrwxr-x   0 rudolphpienaar (2090878) domain_users (2000513)        0 2024-04-25 23:02:46.895553 spleenseg-1.2.0/spleenseg/core/
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)    24199 2024-04-25 22:58:32.000000 spleenseg-1.2.0/spleenseg/core/neuralnet.py
+drwxrwxr-x   0 rudolphpienaar (2090878) domain_users (2000513)        0 2024-04-25 23:02:46.908997 spleenseg-1.2.0/spleenseg/plotting/
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)     2113 2024-04-25 22:48:33.000000 spleenseg-1.2.0/spleenseg/plotting/plotting.py
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)     9173 2024-04-25 22:59:17.000000 spleenseg-1.2.0/spleenseg/spleenseg.py
+drwxrwxr-x   0 rudolphpienaar (2090878) domain_users (2000513)        0 2024-04-25 23:02:46.921353 spleenseg-1.2.0/spleenseg/transforms/
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)     7650 2024-04-25 16:11:14.000000 spleenseg-1.2.0/spleenseg/transforms/transforms.py
+drwxrwxr-x   0 rudolphpienaar (2090878) domain_users (2000513)        0 2024-04-25 23:02:46.882063 spleenseg-1.2.0/spleenseg.egg-info/
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)     7410 2024-04-25 23:02:46.000000 spleenseg-1.2.0/spleenseg.egg-info/PKG-INFO
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)      361 2024-04-25 23:02:46.000000 spleenseg-1.2.0/spleenseg.egg-info/SOURCES.txt
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)        1 2024-04-25 23:02:46.000000 spleenseg-1.2.0/spleenseg.egg-info/dependency_links.txt
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)       56 2024-04-25 23:02:46.000000 spleenseg-1.2.0/spleenseg.egg-info/entry_points.txt
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)      247 2024-04-25 23:02:46.000000 spleenseg-1.2.0/spleenseg.egg-info/requires.txt
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)       65 2024-04-25 23:02:46.000000 spleenseg-1.2.0/spleenseg.egg-info/top_level.txt
```

### Comparing `spleenseg-1.0.12/LICENSE` & `spleenseg-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spleenseg-1.0.12/PKG-INFO` & `spleenseg-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: spleenseg
-Version: 1.0.12
+Version: 1.2.0
 Summary: A ChRIS DS plugin heavily hacked off project MONAI's spleen segmenation notebook
 Home-page: https://github.com/FNNDSC/pl-monai_spleenseg
 Author: FNNDSC
 Author-email: dev@babyMRI.org
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Provides-Extra: none
 Provides-Extra: dev
+Provides-Extra: none
 License-File: LICENSE
 
 Spleen 3D image segmentation (MONAI)
 ====================================
 
 |Version| |MIT License| |ci|
 
@@ -59,17 +60,17 @@
 is assumed to already have been downloaded *a priori* and is provided to
 this plugin by its *parent*. Outputs of the training are model weight
 filesTh.
 
 Installation
 ------------
 
-``pl-monai_spleenseg`` is a `ChRIS <https://chrisproject.org/>`__
-*plugin*, meaning it can run from either within *ChRIS* or the
-command-line.
+``pl-monai_spleenseg`` is a
+`ChRIS <https://chrisproject.org/>`__\ *plugin*, meaning it can run from
+either within *ChRIS* or the command-line.
 
 Local Usage
 -----------
 
 To get started with local command-line usage, use
 `Apptainer <https://apptainer.org/>`__ (a.k.a. Singularity) to run
 ``pl-monai_spleenseg`` as a container:
@@ -218,7 +219,9 @@
 
 .. |Version| image:: https://img.shields.io/docker/v/fnndsc/pl-monai_spleenseg?sort=semver
    :target: https://hub.docker.com/r/fnndsc/pl-monai_spleenseg
 .. |MIT License| image:: https://img.shields.io/github/license/fnndsc/pl-monai_spleenseg
    :target: https://github.com/FNNDSC/pl-monai_spleenseg/blob/main/LICENSE
 .. |ci| image:: https://github.com/FNNDSC/pl-monai_spleenseg/actions/workflows/ci.yml/badge.svg
    :target: https://github.com/FNNDSC/pl-monai_spleenseg/actions/workflows/ci.yml
+
+
```

### Comparing `spleenseg-1.0.12/README.md` & `spleenseg-1.2.0/spleenseg.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,143 +1,227 @@
-# Spleen 3D image segmentation (MONAI)
+Metadata-Version: 2.1
+Name: spleenseg
+Version: 1.2.0
+Summary: A ChRIS DS plugin heavily hacked off project MONAI's spleen segmenation notebook
+Home-page: https://github.com/FNNDSC/pl-monai_spleenseg
+Author: FNNDSC
+Author-email: dev@babyMRI.org
+License: MIT
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Provides-Extra: dev
+Provides-Extra: none
+License-File: LICENSE
+
+Spleen 3D image segmentation (MONAI)
+====================================
+
+|Version| |MIT License| |ci|
+
+``pl-monai_spleenseg`` is a `ChRIS <https://chrisproject.org/>`__ *DS*
+plugin based off Project MONAI’s spleen segmentation exemplar. This
+plugin implements the training and inference phases as two distinct
+modes of operation. For training, input files are a set of training
+examples (images and segmented images) and output files are training
+plots and weight (model) files in ``pth`` and ``ONNX`` format. For
+inference, input files are a model file and an image to segment.
+
+Abstract
+--------
+
+Based off Project MONAI’s `spleen segmentation
+notebook <https://github.com/Project-MONAI/tutorials/blob/main/3d_segmentation/spleen_segmentation_3d.ipynb>`__,
+this plugin implements both the *training* and *inference* phases of the
+notebook, using data supplied in the *parent* plugin (see
+Implementation). For the most part, the python notebook code can be used
+*verbatim* in the plugin; however, in this example some deeper
+refactoring (adding typing, and some refactoring) to improve its use as
+a stand-alone application.
+
+In general, notebooks are not ideal for batch usage, and often cells
+repeat code used elsewhere in the notebook. This plugin code
+consolidated and generalized many of these cells into functions,
+reducing the overall code footprint considerably.
+
+For the *training* phase, the parent plugin provides input images
+(training and labeled) and the output is a model (``pth`` and ``ONNX``
+format). For the *inference* phase, the input is a model file, and an
+image with the output being a segmented result.
+
+Implementation
+--------------
+
+The original notebook is a largely self-contained *monolithic*
+application. Exemplar input data is pulled from the web, and the
+notebook proceeds from there. In the case of this ChRIS plugin, some
+straightforward organizational changes are necessary. The training data
+is assumed to already have been downloaded *a priori* and is provided to
+this plugin by its *parent*. Outputs of the training are model weight
+filesTh.
+
+Installation
+------------
+
+``pl-monai_spleenseg`` is a
+`ChRIS <https://chrisproject.org/>`__\ *plugin*, meaning it can run from
+either within *ChRIS* or the command-line.
+
+Local Usage
+-----------
+
+To get started with local command-line usage, use
+`Apptainer <https://apptainer.org/>`__ (a.k.a. Singularity) to run
+``pl-monai_spleenseg`` as a container:
 
-[![Version](https://img.shields.io/docker/v/fnndsc/pl-monai_spleenseg?sort=semver)](https://hub.docker.com/r/fnndsc/pl-monai_spleenseg)
-[![MIT License](https://img.shields.io/github/license/fnndsc/pl-monai_spleenseg)](https://github.com/FNNDSC/pl-monai_spleenseg/blob/main/LICENSE)
-[![ci](https://github.com/FNNDSC/pl-monai_spleenseg/actions/workflows/ci.yml/badge.svg)](https://github.com/FNNDSC/pl-monai_spleenseg/actions/workflows/ci.yml)
+.. code:: shell
 
-`pl-monai_spleenseg` is a [_ChRIS_](https://chrisproject.org/) _DS_ plugin based off Project MONAI's spleen segmentation exemplar. This plugin implements the training and inference phases as two distinct modes of operation. For training, input files are a set of training examples (images and segmented images) and output files are training plots and weight (model) files in `pth` and `ONNX` format. For inference, input files are a model file and an image to segment.
+   apptainer exec docker://fnndsc/pl-monai_spleenseg spleenseg_train \
+               [--args values...] input/ output/
 
-## Abstract
+To print its available options, run:
 
-Based off Project MONAI's [spleen segmentation notebook](https://github.com/Project-MONAI/tutorials/blob/main/3d_segmentation/spleen_segmentation_3d.ipynb), this plugin implements both the _training_ and _inference_ phases of the notebook, using data supplied in the _parent_ plugin (see Implementation). For the most part, the python notebook code can be used _verbatim_ in the plugin; however, in this example some deeper refactoring (adding typing, and some refactoring) to improve its use as a stand-alone application.
+.. code:: shell
 
-In general, notebooks are not ideal for batch usage, and often cells repeat code used elsewhere in the notebook. This plugin code consolidated and generalized many of these cells into functions, reducing the overall code footprint considerably.
+   apptainer exec docker://fnndsc/pl-monai_spleenseg spleenseg_train --help
 
-For the _training_ phase, the parent plugin provides input images (training and labeled) and the output is a model (`pth` and `ONNX` format). For the _inference_ phase, the input is a model file, and an image with the output being a segmented result.
+Examples
+--------
 
-## Implementation
+``spleenseg_train`` requires two positional arguments: a directory
+containing input data, and a directory containing output data (graphs
+and “model” files). In this plugin, data is downloaded from
+`medicaldecathelon <http://medicaldecathelon.com>`__. To get this data,
+first set an environment variable pointing at the directory to contain
+the pulled and unpacked data:
 
-The original notebook is a largely self-contained _monolithic_ application. Exemplar input data is pulled from the web, and the notebook proceeds from there. In the case of this ChRIS plugin, some straightforward organizational changes are necessary. The training data is assumed to already have been downloaded _a priori_ and is provided to this plugin by its _parent_. Outputs of the training are model weight filesTh.
+.. code:: bash
 
-## Installation
+   export MONAI_DATA_DIR=/some/dir
 
-`pl-monai_spleenseg` is a _[ChRIS](https://chrisproject.org/) plugin_, meaning it can
-run from either within _ChRIS_ or the command-line.
+now, you can pull the data with this python snippet:
 
-## Local Usage
+.. code:: python
 
-To get started with local command-line usage, use [Apptainer](https://apptainer.org/) (a.k.a. Singularity) to run `pl-monai_spleenseg` as a container:
+   # You probably will need to
+   #   pip install -q "monai-weekly[gdown, nibabel, tqdm, ignite]"
+   from monai.apps import download_and_extract
 
-```shell
-apptainer exec docker://fnndsc/pl-monai_spleenseg spleenseg_train \
-            [--args values...] input/ output/
-```
+   directory = os.environ.get("MONAI_DATA_DIRECTORY")
+   root_dir = tempfile.mkdtemp() if directory is None else directory
+   print(root_dir)
 
-To print its available options, run:
 
-```shell
-apptainer exec docker://fnndsc/pl-monai_spleenseg spleenseg_train --help
-```
+   resource = "https://msd-for-monai.s3-us-west-2.amazonaws.com/Task09_Spleen.tar"
+   md5 = "410d4a301da4e5b2f6f86ec3ddba524e"
+   compressed_file = os.path.join(root_dir, "Task09_Spleen.tar")
+   data_dir = os.path.join(root_dir, "Task09_Spleen")
+   if not os.path.exists(data_dir):
+       download_and_extract(resource, compressed_file, root_dir, md5)
 
-## Examples
+Or simply run the supplied ``trainingDataPull.py`` script (which is
+essentially the above code):
 
-`spleenseg_train` requires two positional arguments: a directory containing input data, and a directory containing output data (graphs and "model" files). In this plugin, data is downloaded from [medicaldecathelon](http://medicaldecathelon.com). To get this data, first set an environment variable pointing at the directory to contain the pulled and unpacked data:
+.. code:: bash
 
-```bash 
-export MONAI_DATA_DIR=/some/dir
-```
+   python trainingDataPull.py
 
-now, you can pull the data with this python snippet:
+Create some ``output`` directory, and using our ``$MONAI_DATA_DIR``, we
+can run the plugin:
 
-```python
-# You probably will need to
-#   pip install -q "monai-weekly[gdown, nibabel, tqdm, ignite]"
-from monai.apps import download_and_extract
-
-directory = os.environ.get("MONAI_DATA_DIRECTORY")
-root_dir = tempfile.mkdtemp() if directory is None else directory
-print(root_dir)
-
-
-resource = "https://msd-for-monai.s3-us-west-2.amazonaws.com/Task09_Spleen.tar"
-md5 = "410d4a301da4e5b2f6f86ec3ddba524e"
-compressed_file = os.path.join(root_dir, "Task09_Spleen.tar")
-data_dir = os.path.join(root_dir, "Task09_Spleen")
-if not os.path.exists(data_dir):
-    download_and_extract(resource, compressed_file, root_dir, md5)
-```
-
-Or simply run the supplied `trainingDataPull.py` script (which is essentially the above code):
-
-```bash 
-python trainingDataPull.py
-```
-
-Create some `output` directory, and using our `$MONAI_DATA_DIR`, we can run the plugin:
-
-```shell
-mkdir outgoing/
-apptainer exec docker://fnndsc/pl-monai_spleenseg:latest spleenseg_train \
-        [--args] $MONAI_DATA_DIR outgoing/
-```
+.. code:: shell
 
-## Development
+   mkdir outgoing/
+   apptainer exec docker://fnndsc/pl-monai_spleenseg:latest spleenseg_train \
+           [--args] $MONAI_DATA_DIR outgoing/
+
+Development
+-----------
 
 Instructions for developers.
 
-### Building
+Building
+~~~~~~~~
 
 Build a local container image:
 
-```shell
-docker build -t localhost/fnndsc/pl-monai_spleenseg .
-```
+.. code:: shell
+
+   docker build -t localhost/fnndsc/pl-monai_spleenseg .
+
+Running
+~~~~~~~
+
+Mount the source code ``spleenseg_train.py`` into a container to try out
+changes without rebuild.
+
+.. code:: shell
+
+   docker run --rm -it --userns=host -u $(id -u):$(id -g) \
+       -v $PWD/spleenseg_train.py:/usr/local/lib/python3.11/site-packages/spleenseg_train.py:ro \
+       -v $PWD/in:/incoming:ro -v $PWD/out:/outgoing:rw -w /outgoing \
+       localhost/fnndsc/pl-monai_spleenseg spleenseg_train /incoming /outgoing
+
+Testing
+~~~~~~~
+
+Run unit tests using ``pytest``. It’s recommended to rebuild the image
+to ensure that sources are up-to-date. Use the option
+``--build-arg extras_require=dev`` to install extra dependencies for
+testing.
+
+.. code:: shell
 
-### Running
+   docker build -t localhost/fnndsc/pl-monai_spleenseg:dev --build-arg extras_require=dev .
+   docker run --rm -it localhost/fnndsc/pl-monai_spleenseg:dev pytest
 
-Mount the source code `spleenseg_train.py` into a container to try out changes without rebuild.
+Release
+-------
 
-```shell
-docker run --rm -it --userns=host -u $(id -u):$(id -g) \
-    -v $PWD/spleenseg_train.py:/usr/local/lib/python3.11/site-packages/spleenseg_train.py:ro \
-    -v $PWD/in:/incoming:ro -v $PWD/out:/outgoing:rw -w /outgoing \
-    localhost/fnndsc/pl-monai_spleenseg spleenseg_train /incoming /outgoing
-```
+Steps for release can be automated by `Github
+Actions <.github/workflows/ci.yml>`__. This section is about how to do
+those steps manually.
 
-### Testing
+Increase Version Number
+~~~~~~~~~~~~~~~~~~~~~~~
 
-Run unit tests using `pytest`. It's recommended to rebuild the image to ensure that sources are up-to-date. Use the option `--build-arg extras_require=dev` to install extra dependencies for testing.
+Increase the version number in ``setup.py`` and commit this file.
 
-```shell
-docker build -t localhost/fnndsc/pl-monai_spleenseg:dev --build-arg extras_require=dev .
-docker run --rm -it localhost/fnndsc/pl-monai_spleenseg:dev pytest
-```
+Push Container Image
+~~~~~~~~~~~~~~~~~~~~
 
-## Release
+Build and push an image tagged by the version. For example, for version
+``1.2.3``:
 
-Steps for release can be automated by [Github Actions](.github/workflows/ci.yml). This section is about how to do those steps manually.
+::
 
-### Increase Version Number
+   docker build -t docker.io/fnndsc/pl-monai_spleenseg:1.2.3 .
+   docker push docker.io/fnndsc/pl-monai_spleenseg:1.2.3
 
-Increase the version number in `setup.py` and commit this file.
+Get JSON Representation
+~~~~~~~~~~~~~~~~~~~~~~~
 
-### Push Container Image
+Run
+```chris_plugin_info`` <https://github.com/FNNDSC/chris_plugin#usage>`__
+to produce a JSON description of this plugin, which can be uploaded to
+*ChRIS*.
 
-Build and push an image tagged by the version. For example, for version `1.2.3`:
+.. code:: shell
 
-```
-docker build -t docker.io/fnndsc/pl-monai_spleenseg:1.2.3 .
-docker push docker.io/fnndsc/pl-monai_spleenseg:1.2.3
-```
+   docker run --rm docker.io/fnndsc/pl-monai_spleenseg:1.2.3 chris_plugin_info \
+               -d docker.io/fnndsc/pl-monai_spleenseg:1.2.3 > chris_plugin_info.json
 
-### Get JSON Representation
+Intructions on how to upload the plugin to *ChRIS* can be found here:
+https://chrisproject.org/docs/tutorials/upload_plugin
 
-Run [`chris_plugin_info`](https://github.com/FNNDSC/chris_plugin#usage) to produce a JSON description of this plugin, which can be uploaded to _ChRIS_.
+*-30-*
 
-```shell
-docker run --rm docker.io/fnndsc/pl-monai_spleenseg:1.2.3 chris_plugin_info \
-            -d docker.io/fnndsc/pl-monai_spleenseg:1.2.3 > chris_plugin_info.json
-```
+.. |Version| image:: https://img.shields.io/docker/v/fnndsc/pl-monai_spleenseg?sort=semver
+   :target: https://hub.docker.com/r/fnndsc/pl-monai_spleenseg
+.. |MIT License| image:: https://img.shields.io/github/license/fnndsc/pl-monai_spleenseg
+   :target: https://github.com/FNNDSC/pl-monai_spleenseg/blob/main/LICENSE
+.. |ci| image:: https://github.com/FNNDSC/pl-monai_spleenseg/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/FNNDSC/pl-monai_spleenseg/actions/workflows/ci.yml
 
-Intructions on how to upload the plugin to _ChRIS_ can be found here: https://chrisproject.org/docs/tutorials/upload_plugin
 
-_-30-_
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `spleenseg-1.0.12/README.rst` & `spleenseg-1.2.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 is assumed to already have been downloaded *a priori* and is provided to
 this plugin by its *parent*. Outputs of the training are model weight
 filesTh.
 
 Installation
 ------------
 
-``pl-monai_spleenseg`` is a `ChRIS <https://chrisproject.org/>`__
-*plugin*, meaning it can run from either within *ChRIS* or the
-command-line.
+``pl-monai_spleenseg`` is a
+`ChRIS <https://chrisproject.org/>`__\ *plugin*, meaning it can run from
+either within *ChRIS* or the command-line.
 
 Local Usage
 -----------
 
 To get started with local command-line usage, use
 `Apptainer <https://apptainer.org/>`__ (a.k.a. Singularity) to run
 ``pl-monai_spleenseg`` as a container:
```

### Comparing `spleenseg-1.0.12/setup.py` & `spleenseg-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `spleenseg-1.0.12/spleenseg/plotting/plotting.py` & `spleenseg-1.2.0/spleenseg/plotting/plotting.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 
 from pathlib import Path
+from monai.data.meta_tensor import MetaTensor
 import torch
 import matplotlib.pyplot as plt
 import pudb
 from spleenseg.models import data
 
 
 def plot_imageAndLabel(
@@ -38,15 +39,18 @@
     plt.xlabel("epoch")
     plt.plot(x, y)
     plt.savefig(str(savefile))
     plt.clf()
 
 
 def plot_bestModelOnValidate(
-    input: dict[str, torch.Tensor], output: torch.Tensor, title: str, savefile: Path
+    input: dict[str, torch.Tensor | MetaTensor | int],
+    output: torch.Tensor,
+    title: str,
+    savefile: Path,
 ) -> None:
     plt.figure("check", (18, 6))
     plt.subplot(1, 3, 1)
     plt.title(f"image {title}")
     plt.imshow(input["image"][0, 0, :, :, 80], cmap="gray")
     plt.subplot(1, 3, 2)
     plt.title(f"label {title}")
@@ -63,10 +67,10 @@
 ) -> None:
     plt.figure("Infer", (18, 6))
     plt.subplot(1, 2, 1)
     plt.title(f"input: {title}")
     plt.imshow(input[:, :, 20], cmap="gray")
     plt.subplot(1, 2, 2)
     plt.title(f"result: {title}")
-    plt.imshow(result[0].detach().cpu()[1, :, :, 20])
+    plt.imshow(result.detach().cpu()[1, :, :, 20])
     plt.savefig(str(savefile))
     plt.clf()
```

### Comparing `spleenseg-1.0.12/spleenseg/spleenseg.py` & `spleenseg-1.2.0/spleenseg/spleenseg.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,27 +13,28 @@
 # import os
 import sys
 import re
 import pudb
 from typing import Any, Optional, Callable
 
 from spleenseg.core import neuralnet
+from spleenseg.models.data import TrainingParams
 from spleenseg.transforms import transforms
 from spleenseg.plotting import plotting
 import warnings
 from pyfiglet import Figlet
 
 warnings.filterwarnings(
     "ignore",
     message="For details about installing the optional dependencies, please visit:",
 )
 
 from chris_plugin import chris_plugin, PathMapper
 
-__version__ = "1.0.12"
+__version__ = "1.2.0"
 
 DISPLAY_TITLE = r"""
 
 ███████╗██████╗ ██╗     ███████╗███████╗███╗   ██╗███████╗███████╗ ██████╗
 ██╔════╝██╔══██╗██║     ██╔════╝██╔════╝████╗  ██║██╔════╝██╔════╝██╔════╝
 ███████╗██████╔╝██║     █████╗  █████╗  ██╔██╗ ██║███████╗█████╗  ██║  ███╗
 ╚════██║██╔═══╝ ██║     ██╔══╝  ██╔══╝  ██║╚██╗██║╚════██║██╔══╝  ██║   ██║
@@ -53,14 +54,20 @@
 parser.add_argument(
     "--mode",
     type=str,
     default="training",
     help="mode of behaviour: training or inference",
 )
 parser.add_argument(
+    "--logTransformVols",
+    default=False,
+    action="store_true",
+    help="If specified, save intermediary and inference data as NIfTI volumes",
+)
+parser.add_argument(
     "--useModel",
     type=str,
     default="model.pth",
     help="model to use for inference processing",
 )
 parser.add_argument(
     "--trainImageDir",
@@ -166,33 +173,46 @@
     f = Figlet(font="doom")
     print(f.renderText(f"{options.mode}"))
     print(f"Device = {options.device}")
     print_config()
 
 
 def env_outputDirsMake(options: Namespace) -> None:
+    params: TrainingParams = TrainingParams(options)
     if "training" in options.mode:
-        Path(Path(options.outputdir) / "training").mkdir(parents=True, exist_ok=True)
-        Path(Path(options.outputdir) / "validation").mkdir(parents=True, exist_ok=True)
+        params.preTrainingIO.mkdir(parents=True, exist_ok=True)
+        params.whileTrainingIO.mkdir(parents=True, exist_ok=True)
+        params.whileTrainingValidation.mkdir(parents=True, exist_ok=True)
+        params.postTrainingValidation.mkdir(parents=True, exist_ok=True)
+        params.postTrainingImageSpacings.mkdir(parents=True, exist_ok=True)
     if "inference" in options.mode:
-        Path(Path(options.outputdir) / "inference").mkdir(parents=True, exist_ok=True)
+        params.novelInference.mkdir(parents=True, exist_ok=True)
+
+
+def modelFile_inputdirGet(options: Namespace) -> Path:
+    modelFile: Path = Path(Path(options.inputdir) / options.useModel)
+    if not modelFile.exists():
+        raise FileNotFoundError(f"The model '{modelFile}' does not exist.")
+    return modelFile
 
 
 def training_do(neuralNet: neuralnet.NeuralNet, options: Namespace) -> bool:
     trainingOK: bool = True
 
     neuralNet.trainingFileSet, neuralNet.validationFileSet = (
         inputFilesSets_trainValidateFind(options)
     )
 
     if not neuralNet.trainingTransformsAndSpace_setup():
         return False
 
     if options.mode == "training":
         neuralNet.train()
+    if options.mode == "trainingContinue":
+        neuralNet.train(modelFile_inputdirGet(options))
 
     plotting.plot_trainingMetrics(
         neuralNet.trainingLog,
         neuralNet.trainingParams,
         neuralNet.trainingParams.outputDir / "training" / "trainingLog.png",
     )
 
@@ -202,19 +222,15 @@
     return trainingOK
 
 
 def inference_do(neuralNet: neuralnet.NeuralNet, options: Namespace) -> bool:
     inferenceOK: bool = True
     neuralNet.testingFileSet = testingData_prep(options)
 
-    modelFile: Path = Path(Path(options.inputdir) / options.useModel)
-    if not modelFile.exists():
-        raise FileNotFoundError(f"The model '{modelFile}' does not exist.")
-
-    neuralNet.infer_usingModel(modelFile)
+    neuralNet.infer_usingModel(modelFile_inputdirGet(options))
 
     return inferenceOK
 
 
 @chris_plugin(
     parser=parser,
     title="Spleen 3D image segmentation (MONAI)",
@@ -230,15 +246,15 @@
     are passed to this main method implicitly when ``main()`` is called below without parameters.
 
     :param options: non-positional arguments parsed by the parser given to @chris_plugin
     :param inputdir: directory containing (read-only) input files
     :param outputdir: directory where to write output files
     """
 
-    pudb.set_trace()
+    # pudb.set_trace()
 
     envDetail_print(options)
     env_outputDirsMake(options)
     neuralNet: neuralnet.NeuralNet = neuralnet.NeuralNet(options)
     if "training" in options.mode:
         training_do(neuralNet, options)
```

### Comparing `spleenseg-1.0.12/spleenseg/transforms/transforms.py` & `spleenseg-1.2.0/spleenseg/transforms/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,11 +232,11 @@
     check_loader: DataLoader = DataLoader(check_ds, batch_size=1)
     check_data: Any | None = first(check_loader)
     if not check_data:
         return False
     image, label = (check_data["image"][0][0], check_data["label"][0][0])
     print("")
     print("Checking transforms... :")
-    print(f"sample image shape: {image.shape}")
-    print(f"sample label shape: {label.shape}")
+    print(f"sample 'image' transform shape: {image.shape}")
+    print(f"sample 'label' transform shape: {label.shape}")
     plotting.plot_imageAndLabel(image, label, outputdir / "exemplar_image_label.jpg")
     return True
```

