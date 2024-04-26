# Comparing `tmp/metrics_as_scores-2.8.1.tar.gz` & `tmp/metrics_as_scores-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metrics_as_scores-2.8.1.tar", max compression
+gzip compressed data, was "metrics_as_scores-2.8.2.tar", max compression
```

## Comparing `metrics_as_scores-2.8.1.tar` & `metrics_as_scores-2.8.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      287 2023-02-20 16:35:52.783754 metrics_as_scores-2.8.1/build.py
--rw-r--r--   0        0        0    36442 2022-09-30 12:51:35.511324 metrics_as_scores-2.8.1/LICENSE
--rw-r--r--   0        0        0     2709 2024-01-03 11:09:45.714577 metrics_as_scores-2.8.1/pyproject.toml
--rw-r--r--   0        0        0    23642 2024-01-03 11:10:31.061611 metrics_as_scores-2.8.1/README.md
--rw-r--r--   0        0        0     1063 2023-04-13 06:55:30.716391 metrics_as_scores-2.8.1/src/metrics_as_scores/__init__.py
--rw-r--r--   0        0        0     1157 2023-02-20 16:35:52.798739 metrics_as_scores-2.8.1/src/metrics_as_scores/__version__.py
--rw-r--r--   0        0        0      284 2023-04-13 06:55:30.745365 metrics_as_scores-2.8.1/src/metrics_as_scores/cli/__init__.py
--rw-r--r--   0        0        0     4247 2023-04-13 06:55:30.717395 metrics_as_scores-2.8.1/src/metrics_as_scores/cli/BundleOwn.py
--rw-r--r--   0        0        0      895 2023-02-20 16:35:52.800735 metrics_as_scores-2.8.1/src/metrics_as_scores/cli/Cli.py
--rw-r--r--   0        0        0    20437 2023-07-16 08:13:42.684832 metrics_as_scores-2.8.1/src/metrics_as_scores/cli/CreateDataset.py
--rw-r--r--   0        0        0     2716 2023-04-13 06:55:30.722386 metrics_as_scores-2.8.1/src/metrics_as_scores/cli/Download.py
--rw-r--r--   0        0        0    11653 2023-04-21 13:19:41.659645 metrics_as_scores-2.8.1/src/metrics_as_scores/cli/FitParametric.py
--rw-r--r--   0        0        0     5096 2023-04-13 06:55:30.728381 metrics_as_scores-2.8.1/src/metrics_as_scores/cli/GenerateDensities.py
--rw-r--r--   0        0        0     8397 2023-07-16 08:13:42.685838 metrics_as_scores-2.8.1/src/metrics_as_scores/cli/helpers.py
--rw-r--r--   0        0        0     2203 2023-04-13 06:55:30.735370 metrics_as_scores-2.8.1/src/metrics_as_scores/cli/KnownDatasets.py
--rw-r--r--   0        0        0     1805 2023-04-13 06:55:30.736372 metrics_as_scores-2.8.1/src/metrics_as_scores/cli/LocalDatasets.py
--rw-r--r--   0        0        0     9257 2023-04-13 06:55:30.738364 metrics_as_scores-2.8.1/src/metrics_as_scores/cli/LocalWebserver.py
--rw-r--r--   0        0        0     3199 2023-04-13 06:55:30.742360 metrics_as_scores-2.8.1/src/metrics_as_scores/cli/MainWorkflow.py
--rw-r--r--   0        0        0     3800 2023-04-13 06:55:30.743360 metrics_as_scores-2.8.1/src/metrics_as_scores/cli/Workflow.py
--rw-r--r--   0        0        0      265 2023-04-13 06:55:30.747364 metrics_as_scores-2.8.1/src/metrics_as_scores/data/__init__.py
--rw-r--r--   0        0        0    13093 2023-04-21 13:19:41.661631 metrics_as_scores-2.8.1/src/metrics_as_scores/data/pregenerate.py
--rw-r--r--   0        0        0     5576 2023-04-13 06:55:30.749364 metrics_as_scores-2.8.1/src/metrics_as_scores/data/pregenerate_distns.py
--rw-r--r--   0        0        0     7256 2023-04-21 13:19:41.661631 metrics_as_scores-2.8.1/src/metrics_as_scores/data/pregenerate_fit.py
--rw-r--r--   0        0        0      342 2023-04-13 06:55:30.752350 metrics_as_scores-2.8.1/src/metrics_as_scores/datasets/_default/_quarto.yml
--rw-r--r--   0        0        0    14513 2023-02-20 16:35:52.810722 metrics_as_scores-2.8.1/src/metrics_as_scores/datasets/_default/About.qmd
--rw-r--r--   0        0        0      507 2023-02-20 16:35:52.811720 metrics_as_scores-2.8.1/src/metrics_as_scores/datasets/_default/readme.md
--rw-r--r--   0        0        0     1876 2023-02-20 16:35:52.812720 metrics_as_scores-2.8.1/src/metrics_as_scores/datasets/_default/refs.bib
--rw-r--r--   0        0        0      435 2023-02-20 16:35:52.813718 metrics_as_scores-2.8.1/src/metrics_as_scores/datasets/_default/web/about.html
--rw-r--r--   0        0        0      467 2023-02-20 16:35:52.813718 metrics_as_scores-2.8.1/src/metrics_as_scores/datasets/_default/web/references.html
--rw-r--r--   0        0        0     1488 2023-04-13 06:55:30.752350 metrics_as_scores-2.8.1/src/metrics_as_scores/datasets/known-datasets.bib
--rw-r--r--   0        0        0     1277 2023-04-13 06:55:30.753348 metrics_as_scores-2.8.1/src/metrics_as_scores/datasets/known-datasets.json
--rw-r--r--   0        0        0      226 2023-04-13 06:55:30.754353 metrics_as_scores-2.8.1/src/metrics_as_scores/distribution/__init__.py
--rw-r--r--   0        0        0    48503 2023-07-16 08:13:42.686830 metrics_as_scores-2.8.1/src/metrics_as_scores/distribution/distribution.py
--rw-r--r--   0        0        0    22219 2023-04-13 06:55:30.757346 metrics_as_scores-2.8.1/src/metrics_as_scores/distribution/fitting.py
--rw-r--r--   0        0        0    22308 2023-02-20 16:35:52.817713 metrics_as_scores-2.8.1/src/metrics_as_scores/distribution/fitting_problems.py
--rw-r--r--   0        0        0     2709 2024-01-03 11:10:19.527576 metrics_as_scores-2.8.1/src/metrics_as_scores/pyproject.toml
--rw-r--r--   0        0        0       82 2023-04-13 06:55:30.758350 metrics_as_scores-2.8.1/src/metrics_as_scores/tools/__init__.py
--rw-r--r--   0        0        0     5389 2023-04-13 06:55:30.760341 metrics_as_scores-2.8.1/src/metrics_as_scores/tools/funcs.py
--rw-r--r--   0        0        0     5440 2023-04-13 06:55:30.761351 metrics_as_scores-2.8.1/src/metrics_as_scores/tools/lazy.py
--rw-r--r--   0        0        0      229 2023-04-13 06:55:30.762348 metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/__init__.py
--rw-r--r--   0        0        0     3414 2023-04-13 06:55:30.764342 metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/app_hooks.py
--rw-r--r--   0        0        0      931 2023-02-20 16:35:52.820709 metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/data.py
--rw-r--r--   0        0        0      408 2023-02-20 16:35:52.821708 metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/exception.py
--rw-r--r--   0        0        0    10664 2023-07-16 08:13:42.689826 metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/footer.html
--rw-r--r--   0        0        0      746 2023-07-16 08:13:42.690824 metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/header.html
--rw-r--r--   0        0        0    22823 2023-08-01 07:47:02.103125 metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/main.py
--rw-r--r--   0        0        0     1774 2023-04-13 06:55:30.766341 metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/metrics-as-scores.nginx.conf
--rw-r--r--   0        0        0      556 2023-04-13 06:55:30.788315 metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/metrics-as-scores.service
--rw-r--r--   0        0        0      180 2022-09-05 06:40:38.188152 metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/readme.md
--rw-r--r--   0        0        0   113561 2022-09-05 06:40:56.466003 metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/static/curve.ico
--rw-r--r--   0        0        0    29350 2022-09-05 06:40:22.832754 metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/static/curve.png
--rw-r--r--   0        0        0    11170 2022-09-20 15:00:30.424180 metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/static/loading.png
--rw-r--r--   0        0        0      121 2023-02-20 16:35:52.824708 metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/static/main.js
--rw-r--r--   0        0        0      981 2023-02-20 16:35:52.825704 metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/static/styles.css
--rw-r--r--   0        0        0     1643 2023-02-20 16:35:52.827702 metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/templates/index.html
--rw-r--r--   0        0        0    25293 1970-01-01 00:00:00.000000 metrics_as_scores-2.8.1/PKG-INFO
+-rw-r--r--   0        0        0      287 2023-04-14 08:48:51.676031 metrics_as_scores-2.8.2/build.py
+-rw-r--r--   0        0        0    36442 2022-09-29 14:35:27.510381 metrics_as_scores-2.8.2/LICENSE
+-rw-r--r--   0        0        0     2710 2024-04-26 08:24:50.054330 metrics_as_scores-2.8.2/pyproject.toml
+-rw-r--r--   0        0        0    23640 2024-04-26 08:24:50.053338 metrics_as_scores-2.8.2/README.md
+-rw-r--r--   0        0        0     1063 2023-04-14 08:48:51.697972 metrics_as_scores-2.8.2/src/metrics_as_scores/__init__.py
+-rw-r--r--   0        0        0     1157 2023-04-14 08:48:51.697972 metrics_as_scores-2.8.2/src/metrics_as_scores/__version__.py
+-rw-r--r--   0        0        0      284 2023-04-14 08:48:51.704956 metrics_as_scores-2.8.2/src/metrics_as_scores/cli/__init__.py
+-rw-r--r--   0        0        0     4247 2023-04-14 08:48:51.699968 metrics_as_scores-2.8.2/src/metrics_as_scores/cli/BundleOwn.py
+-rw-r--r--   0        0        0      895 2023-04-19 14:16:25.878901 metrics_as_scores-2.8.2/src/metrics_as_scores/cli/Cli.py
+-rw-r--r--   0        0        0    20437 2024-03-21 08:46:09.750741 metrics_as_scores-2.8.2/src/metrics_as_scores/cli/CreateDataset.py
+-rw-r--r--   0        0        0     2716 2023-04-14 08:48:51.700965 metrics_as_scores-2.8.2/src/metrics_as_scores/cli/Download.py
+-rw-r--r--   0        0        0    11653 2023-04-21 12:55:47.481386 metrics_as_scores-2.8.2/src/metrics_as_scores/cli/FitParametric.py
+-rw-r--r--   0        0        0     5096 2023-04-14 08:48:51.702959 metrics_as_scores-2.8.2/src/metrics_as_scores/cli/GenerateDensities.py
+-rw-r--r--   0        0        0     8397 2024-03-21 08:46:09.751738 metrics_as_scores-2.8.2/src/metrics_as_scores/cli/helpers.py
+-rw-r--r--   0        0        0     2203 2023-04-14 08:48:51.702959 metrics_as_scores-2.8.2/src/metrics_as_scores/cli/KnownDatasets.py
+-rw-r--r--   0        0        0     1805 2023-04-14 08:48:51.702959 metrics_as_scores-2.8.2/src/metrics_as_scores/cli/LocalDatasets.py
+-rw-r--r--   0        0        0     9257 2023-04-14 08:48:51.703956 metrics_as_scores-2.8.2/src/metrics_as_scores/cli/LocalWebserver.py
+-rw-r--r--   0        0        0     3199 2023-04-14 08:48:51.703956 metrics_as_scores-2.8.2/src/metrics_as_scores/cli/MainWorkflow.py
+-rw-r--r--   0        0        0     3800 2023-04-14 08:48:51.703956 metrics_as_scores-2.8.2/src/metrics_as_scores/cli/Workflow.py
+-rw-r--r--   0        0        0      265 2023-04-14 08:48:51.704956 metrics_as_scores-2.8.2/src/metrics_as_scores/data/__init__.py
+-rw-r--r--   0        0        0    13093 2023-04-21 12:55:47.483320 metrics_as_scores-2.8.2/src/metrics_as_scores/data/pregenerate.py
+-rw-r--r--   0        0        0     5576 2023-04-14 08:48:51.705951 metrics_as_scores-2.8.2/src/metrics_as_scores/data/pregenerate_distns.py
+-rw-r--r--   0        0        0     7256 2023-04-21 12:55:47.484491 metrics_as_scores-2.8.2/src/metrics_as_scores/data/pregenerate_fit.py
+-rw-r--r--   0        0        0      342 2023-04-14 08:48:51.707945 metrics_as_scores-2.8.2/src/metrics_as_scores/datasets/_default/_quarto.yml
+-rw-r--r--   0        0        0    14513 2023-04-14 08:48:51.706948 metrics_as_scores-2.8.2/src/metrics_as_scores/datasets/_default/About.qmd
+-rw-r--r--   0        0        0      507 2023-04-14 08:48:51.707945 metrics_as_scores-2.8.2/src/metrics_as_scores/datasets/_default/readme.md
+-rw-r--r--   0        0        0     1876 2023-04-14 08:48:51.707945 metrics_as_scores-2.8.2/src/metrics_as_scores/datasets/_default/refs.bib
+-rw-r--r--   0        0        0      435 2023-04-14 08:48:51.707945 metrics_as_scores-2.8.2/src/metrics_as_scores/datasets/_default/web/about.html
+-rw-r--r--   0        0        0      467 2023-04-14 08:48:51.708943 metrics_as_scores-2.8.2/src/metrics_as_scores/datasets/_default/web/references.html
+-rw-r--r--   0        0        0     1488 2023-04-14 08:48:51.708943 metrics_as_scores-2.8.2/src/metrics_as_scores/datasets/known-datasets.bib
+-rw-r--r--   0        0        0     1277 2023-04-14 08:48:51.708943 metrics_as_scores-2.8.2/src/metrics_as_scores/datasets/known-datasets.json
+-rw-r--r--   0        0        0      226 2023-04-14 08:48:51.708943 metrics_as_scores-2.8.2/src/metrics_as_scores/distribution/__init__.py
+-rw-r--r--   0        0        0    48503 2024-03-21 08:46:09.752736 metrics_as_scores-2.8.2/src/metrics_as_scores/distribution/distribution.py
+-rw-r--r--   0        0        0    22219 2023-04-14 08:48:51.710937 metrics_as_scores-2.8.2/src/metrics_as_scores/distribution/fitting.py
+-rw-r--r--   0        0        0    22308 2023-04-14 08:48:51.710937 metrics_as_scores-2.8.2/src/metrics_as_scores/distribution/fitting_problems.py
+-rw-r--r--   0        0        0     2710 2024-04-26 08:25:14.302317 metrics_as_scores-2.8.2/src/metrics_as_scores/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-04-14 08:48:51.710937 metrics_as_scores-2.8.2/src/metrics_as_scores/tools/__init__.py
+-rw-r--r--   0        0        0     5389 2023-04-14 08:48:51.711935 metrics_as_scores-2.8.2/src/metrics_as_scores/tools/funcs.py
+-rw-r--r--   0        0        0     5440 2023-04-14 08:48:51.711935 metrics_as_scores-2.8.2/src/metrics_as_scores/tools/lazy.py
+-rw-r--r--   0        0        0      229 2023-04-14 08:48:51.712932 metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/__init__.py
+-rw-r--r--   0        0        0     3414 2023-04-14 08:48:51.712932 metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/app_hooks.py
+-rw-r--r--   0        0        0      931 2023-04-14 08:48:51.712932 metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/data.py
+-rw-r--r--   0        0        0      408 2023-04-14 08:48:51.713929 metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/exception.py
+-rw-r--r--   0        0        0    10664 2023-07-12 09:58:48.916612 metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/footer.html
+-rw-r--r--   0        0        0      746 2023-07-12 09:58:48.917609 metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/header.html
+-rw-r--r--   0        0        0    22823 2024-03-21 08:46:09.752736 metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/main.py
+-rw-r--r--   0        0        0     1774 2023-04-14 08:48:51.716924 metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/metrics-as-scores.nginx.conf
+-rw-r--r--   0        0        0      556 2023-04-14 08:48:51.717920 metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/metrics-as-scores.service
+-rw-r--r--   0        0        0      180 2022-10-05 11:00:55.171856 metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/readme.md
+-rw-r--r--   0        0        0   113561 2022-10-05 11:00:55.179698 metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/static/curve.ico
+-rw-r--r--   0        0        0    29350 2022-10-05 11:00:55.182690 metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/static/curve.png
+-rw-r--r--   0        0        0    11170 2022-10-05 11:00:55.183687 metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/static/loading.png
+-rw-r--r--   0        0        0      121 2023-04-14 08:48:51.718917 metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/static/main.js
+-rw-r--r--   0        0        0      981 2023-04-14 08:48:51.718917 metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/static/styles.css
+-rw-r--r--   0        0        0     1643 2023-04-14 08:48:51.719914 metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/templates/index.html
+-rw-r--r--   0        0        0    25300 1970-01-01 00:00:00.000000 metrics_as_scores-2.8.2/PKG-INFO
```

### Comparing `metrics_as_scores-2.8.1/LICENSE` & `metrics_as_scores-2.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/pyproject.toml` & `metrics_as_scores-2.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metrics-as-scores"
-version = "2.8.1"
+version = "2.8.2"
 description = "Interactive web application, tool- and analysis suite for approximating, exploring, understanding, and sampling from conditional distributions."
 authors = ["Sebastian Hönel <development@hoenel.net>"]
 license = "Dual-licensed under GNU General Public License v3 (GPLv3) and closed-source"
 readme = "README.md"
 homepage = "https://github.com/mrshoenel/metrics-as-scores"
 repository = "https://github.com/mrshoenel/metrics-as-scores/issues"
 packages = [{include = "metrics_as_scores", from = "src"}]
@@ -33,15 +33,15 @@
 python = ">=3.10, <3.12"
 bokeh = "^2.4.3"
 joblib = "^1.2.0"
 jupyterlab = "^3.4.7"
 matplotlib = "^3.6.0"
 ptvsd = "^4.3.2"
 pymoo = "^0.6.0"
-scipy = "1.10.1"
+scipy = "^1.10.1"
 statsmodels = "^0.13.2"
 StrEnum = "^0.4.8"
 tqdm = "^4.64.1"
 Sphinx = "^5.3.0"
 sphinx-rtd-theme = "^1.1.1"
 toml = "^0.10.2"
 rich = "^13.3.1"
```

### Comparing `metrics_as_scores-2.8.1/README.md` & `metrics_as_scores-2.8.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 ------------------------------------------------------------------------
 
 **Please Note**: ***Metrics As Scores*** (`MAS`) changed considerably
 between versions
 [**`v1.0.8`**](https://github.com/MrShoenel/metrics-as-scores/tree/v1.0.8)
 and **`v2.x.x`**.
 
-The current version is `v2.8.1`.
+The current version is `v2.8.2`.
 
 From version **`v2.x.x`** it has the following new features:
 
 - [Textual User Interface (TUI)](#text-based-user-interface-tui)
 - Proper documentation and testing
 - New version on PyPI. Install the package and run the command line
   interface by typing **`mas`**!
@@ -126,15 +126,15 @@
 - Fit Parametric Distributions for Own Dataset
 - Pre-generate distributions for usage in the
   [**Web-Application**](#web-application)
 - Bundle Own dataset so it can be published
 - Run local, interactive Web-Application using a selected dataset
 
 ![Metrics As Scores Text-based User Interface
-(TUI).](../TUI.png "Metrics As Scores Text-based User Interface (TUI).")
+(TUI).](./TUI.png "Metrics As Scores Text-based User Interface (TUI).")
 
 ## Web Application
 
 Metrics As Scores’ main feature is perhaps the Web Application. It can
 be run directly and locally from the TUI using a selected dataset (you
 may download a known dataset or use your own). The Web Application
 allows to visually inspect each *feature* across all the defined
@@ -142,15 +142,15 @@
 each feature in each group. It offers five different principal types of
 densities: Parametric, Parametric (discrete), Empirical, Empirical
 (discrete), and (approximate) Kernel Density Estimation. The Web
 Application includes a detailed [Help section](#) that should answer
 most of your questions.
 
 ![Metrics As Scores Interactive Web
-.](../WebApp.png "Metrics As Scores Interactive Web Application.")
+.](./WebApp.png "Metrics As Scores Interactive Web Application.")
 
 ## Development Setup
 
 This project was developed using and requires Python `>=3.10`. The
 development documentation can be found at
 <https://mrshoenel.github.io/metrics-as-scores/>. Steps:
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 _P_a_c_k_a_g_e_s - _1_._3_._3_ _R_u_n_n_i_n_g_ _T_e_s_t_s - _2_ _E_x_a_m_p_l_e_ _U_s_a_g_e - _2_._1_ _C_o_n_c_r_e_t_e_ _E_x_a_m_p_l_e_ _U_s_i_n_g
 _t_h_e_ _Q_u_a_l_i_t_a_s_._c_l_a_s_s_ _C_o_r_p_u_s_ _D_a_t_a_s_e_t - _2_._2_ _C_o_n_c_r_e_t_e_ _E_x_a_m_p_l_e_ _U_s_i_n_g_ _t_h_e_ _I_r_i_s_ _D_a_t_a_s_e_t
 - _2_._3_ _D_i_a_m_o_n_d_s_ _E_x_a_m_p_l_e - _3_ _D_a_t_a_s_e_t_s - _3_._1_ _U_s_e_ _Y_o_u_r_ _O_w_n - _3_._2_ _K_n_o_w_n_ _D_a_t_a_s_e_t_s - _4
 _P_e_r_s_o_n_a_l_i_z_i_n_g_ _t_h_e_ _W_e_b_ _A_p_p_l_i_c_a_t_i_o_n - _R_e_f_e_r_e_n_c_e_s --------------------------------
 ---------------------------------------- **Please Note**: ***Metrics As
 Scores*** (`MAS`) changed considerably between versions [**`v1.0.8`**](https://
 github.com/MrShoenel/metrics-as-scores/tree/v1.0.8) and **`v2.x.x`**. The
-current version is `v2.8.1`. From version **`v2.x.x`** it has the following new
+current version is `v2.8.2`. From version **`v2.x.x`** it has the following new
 features: - [Textual User Interface (TUI)](#text-based-user-interface-tui) -
 Proper documentation and testing - New version on PyPI. Install the package and
 run the command line interface by typing **`mas`**! [Metrics As Scores Demo.]
 (https://user-images.githubusercontent.com/5049151/219892077-58854478-b761-
 4a3d-9faf-2fe46c122cf5.webm) --------------------------------------------------
 ---------------------- Contains the data and scripts needed for the application
 **`Metrics as Scores`**, check out _h_t_t_p_s_:_/_/_m_a_s_._r_e_s_e_a_r_c_h_._h_Ã_¶_n_e_l_._n_e_t_/. This
@@ -50,25 +50,25 @@
 if you want to do one of the following: - Show Installed Datasets - Show List
 of Known Datasets Available Online That Can Be Downloaded - Download and
 install a known or existing dataset - Create Own Dataset to be used with
 Metrics-As-Scores - Fit Parametric Distributions for Own Dataset - Pre-generate
 distributions for usage in the [**Web-Application**](#web-application) - Bundle
 Own dataset so it can be published - Run local, interactive Web-Application
 using a selected dataset ![Metrics As Scores Text-based User Interface (TUI).]
-(../TUI.png "Metrics As Scores Text-based User Interface (TUI).") ## Web
+(./TUI.png "Metrics As Scores Text-based User Interface (TUI).") ## Web
 Application Metrics As Scoresâ main feature is perhaps the Web Application.
 It can be run directly and locally from the TUI using a selected dataset (you
 may download a known dataset or use your own). The Web Application allows to
 visually inspect each *feature* across all the defined *groups*. It features
 the PDF/PMF, CDF and CCDF, as well as the PPF for each feature in each group.
 It offers five different principal types of densities: Parametric, Parametric
 (discrete), Empirical, Empirical (discrete), and (approximate) Kernel Density
 Estimation. The Web Application includes a detailed [Help section](#) that
-should answer most of your questions. ![Metrics As Scores Interactive Web .]
-(../WebApp.png "Metrics As Scores Interactive Web Application.") ## Development
+should answer most of your questions. ![Metrics As Scores Interactive Web .](./
+WebApp.png "Metrics As Scores Interactive Web Application.") ## Development
 Setup This project was developed using and requires Python `>=3.10`. The
 development documentation can be found at
 mrshoenel.github.io/metrics-as-scores/>. Steps: 1. Clone the Repository, 2. Set
 up a virtual environment, 3. Install packages. ### Setting Up a Virtual
 Environment It is recommended to use a virtual environment. To use a virtual
 environment, follow these steps (Windows specific; activation of the
 environment might differ). ``` shell virtualenv --python=C:/Python310/
```

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/__init__.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/__init__.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/__version__.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/__version__.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/cli/BundleOwn.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/cli/BundleOwn.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/cli/Cli.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/cli/Cli.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/cli/CreateDataset.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/cli/CreateDataset.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/cli/Download.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/cli/Download.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/cli/FitParametric.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/cli/FitParametric.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/cli/GenerateDensities.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/cli/GenerateDensities.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/cli/helpers.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/cli/KnownDatasets.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/cli/KnownDatasets.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/cli/LocalDatasets.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/cli/LocalDatasets.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/cli/LocalWebserver.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/cli/LocalWebserver.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/cli/MainWorkflow.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/cli/MainWorkflow.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/cli/Workflow.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/cli/Workflow.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/data/pregenerate.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/data/pregenerate.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/data/pregenerate_distns.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/data/pregenerate_distns.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/data/pregenerate_fit.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/data/pregenerate_fit.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/datasets/_default/About.qmd` & `metrics_as_scores-2.8.2/src/metrics_as_scores/datasets/_default/About.qmd`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/datasets/_default/refs.bib` & `metrics_as_scores-2.8.2/src/metrics_as_scores/datasets/_default/refs.bib`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/datasets/known-datasets.bib` & `metrics_as_scores-2.8.2/src/metrics_as_scores/datasets/known-datasets.bib`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/datasets/known-datasets.json` & `metrics_as_scores-2.8.2/src/metrics_as_scores/datasets/known-datasets.json`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/distribution/distribution.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/distribution/distribution.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/distribution/fitting.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/distribution/fitting.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/distribution/fitting_problems.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/distribution/fitting_problems.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/pyproject.toml` & `metrics_as_scores-2.8.2/src/metrics_as_scores/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metrics-as-scores"
-version = "2.8.1"
+version = "2.8.2"
 description = "Interactive web application, tool- and analysis suite for approximating, exploring, understanding, and sampling from conditional distributions."
 authors = ["Sebastian Hönel <development@hoenel.net>"]
 license = "Dual-licensed under GNU General Public License v3 (GPLv3) and closed-source"
 readme = "README.md"
 homepage = "https://github.com/mrshoenel/metrics-as-scores"
 repository = "https://github.com/mrshoenel/metrics-as-scores/issues"
 packages = [{include = "metrics_as_scores", from = "src"}]
@@ -33,15 +33,15 @@
 python = ">=3.10, <3.12"
 bokeh = "^2.4.3"
 joblib = "^1.2.0"
 jupyterlab = "^3.4.7"
 matplotlib = "^3.6.0"
 ptvsd = "^4.3.2"
 pymoo = "^0.6.0"
-scipy = "1.10.1"
+scipy = "^1.10.1"
 statsmodels = "^0.13.2"
 StrEnum = "^0.4.8"
 tqdm = "^4.64.1"
 Sphinx = "^5.3.0"
 sphinx-rtd-theme = "^1.1.1"
 toml = "^0.10.2"
 rich = "^13.3.1"
```

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/tools/funcs.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/tools/funcs.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/tools/lazy.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/tools/lazy.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/app_hooks.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/app_hooks.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/data.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/data.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/footer.html` & `metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/footer.html`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/header.html` & `metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/header.html`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/main.py` & `metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/main.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/metrics-as-scores.nginx.conf` & `metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/metrics-as-scores.nginx.conf`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/metrics-as-scores.service` & `metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/metrics-as-scores.service`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/static/curve.ico` & `metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/static/curve.ico`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/static/curve.png` & `metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/static/curve.png`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/static/loading.png` & `metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/static/loading.png`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/static/styles.css` & `metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/static/styles.css`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/src/metrics_as_scores/webapp/templates/index.html` & `metrics_as_scores-2.8.2/src/metrics_as_scores/webapp/templates/index.html`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.8.1/PKG-INFO` & `metrics_as_scores-2.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metrics-as-scores
-Version: 2.8.1
+Version: 2.8.2
 Summary: Interactive web application, tool- and analysis suite for approximating, exploring, understanding, and sampling from conditional distributions.
 Home-page: https://github.com/mrshoenel/metrics-as-scores
 License: Dual-licensed under GNU General Public License v3 (GPLv3) and closed-source
 Keywords: distribution fitting,statistical tests,context-dependent,metrics,quality,score
 Author: Sebastian Hönel
 Author-email: development@hoenel.net
 Requires-Python: >=3.10,<3.12
@@ -32,15 +32,15 @@
 Requires-Dist: poethepoet (>=0.18.1,<0.19.0)
 Requires-Dist: ptvsd (>=4.3.2,<5.0.0)
 Requires-Dist: pymoo (>=0.6.0,<0.7.0)
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: rich (>=13.3.1,<14.0.0)
 Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
-Requires-Dist: scipy (==1.10.1)
+Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: sphinx-rtd-theme (>=1.1.1,<2.0.0)
 Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: wget (>=3.2,<4.0)
 Project-URL: Repository, https://github.com/mrshoenel/metrics-as-scores/issues
@@ -97,15 +97,15 @@
 ------------------------------------------------------------------------
 
 **Please Note**: ***Metrics As Scores*** (`MAS`) changed considerably
 between versions
 [**`v1.0.8`**](https://github.com/MrShoenel/metrics-as-scores/tree/v1.0.8)
 and **`v2.x.x`**.
 
-The current version is `v2.8.1`.
+The current version is `v2.8.2`.
 
 From version **`v2.x.x`** it has the following new features:
 
 - [Textual User Interface (TUI)](#text-based-user-interface-tui)
 - Proper documentation and testing
 - New version on PyPI. Install the package and run the command line
   interface by typing **`mas`**!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metrics-as-scores Version: 2.8.1 Summary:
+Metadata-Version: 2.1 Name: metrics-as-scores Version: 2.8.2 Summary:
 Interactive web application, tool- and analysis suite for approximating,
 exploring, understanding, and sampling from conditional distributions. Home-
 page: https://github.com/mrshoenel/metrics-as-scores License: Dual-licensed
 under GNU General Public License v3 (GPLv3) and closed-source Keywords:
 distribution fitting,statistical tests,context-dependent,metrics,quality,score
 Author: Sebastian HÃ¶nel Author-email: development@hoenel.net Requires-Python:
 >=3.10,<3.12 Classifier: Development Status :: 5 - Production/Stable
@@ -18,42 +18,42 @@
 (>=2.4.3,<3.0.0) Requires-Dist: joblib (>=1.2.0,<2.0.0) Requires-Dist:
 jupyterlab (>=3.4.7,<4.0.0) Requires-Dist: matplotlib (>=3.6.0,<4.0.0)
 Requires-Dist: myst-parser (>=1.0.0,<2.0.0) Requires-Dist: nptyping
 (>=2.4.1,<3.0.0) Requires-Dist: poethepoet (>=0.18.1,<0.19.0) Requires-Dist:
 ptvsd (>=4.3.2,<5.0.0) Requires-Dist: pymoo (>=0.6.0,<0.7.0) Requires-Dist:
 pytest-cov (>=4.0.0,<5.0.0) Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: rich (>=13.3.1,<14.0.0) Requires-Dist: scikit-learn
-(>=1.2.1,<2.0.0) Requires-Dist: scipy (==1.10.1) Requires-Dist: sphinx-rtd-
-theme (>=1.1.1,<2.0.0) Requires-Dist: statsmodels (>=0.13.2,<0.14.0) Requires-
-Dist: tabulate (>=0.9.0,<0.10.0) Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: tqdm (>=4.64.1,<5.0.0) Requires-Dist: wget (>=3.2,<4.0) Project-
-URL: Repository, https://github.com/mrshoenel/metrics-as-scores/issues
-Description-Content-Type: text/markdown Metrics As Scores [![DOI](https://
-zenodo.org/badge/524333119.svg)](https://zenodo.org/badge/latestdoi/524333119)
-[![status](https://joss.theoj.org/papers/eb549efe6c0111490395496c68717579/
-status.svg)](https://joss.theoj.org/papers/eb549efe6c0111490395496c68717579) [!
-[codecov](https://codecov.io/github/MrShoenel/metrics-as-scores/branch/master/
-graph/badge.svg?token=HO1GYXVEUQ)](https://codecov.io/github/MrShoenel/metrics-
-as-scores) ================ - _1_ _U_s_a_g_e - _1_._1_ _T_e_x_t_-_b_a_s_e_d_ _U_s_e_r_ _I_n_t_e_r_f_a_c_e_ _(_T_U_I_) -
-_1_._2_ _W_e_b_ _A_p_p_l_i_c_a_t_i_o_n - _1_._3_ _D_e_v_e_l_o_p_m_e_n_t_ _S_e_t_u_p - _1_._3_._1_ _S_e_t_t_i_n_g_ _U_p_ _a_ _V_i_r_t_u_a_l
-_E_n_v_i_r_o_n_m_e_n_t - _1_._3_._2_ _I_n_s_t_a_l_l_i_n_g_ _P_a_c_k_a_g_e_s - _1_._3_._3_ _R_u_n_n_i_n_g_ _T_e_s_t_s - _2_ _E_x_a_m_p_l_e_ _U_s_a_g_e
-- _2_._1_ _C_o_n_c_r_e_t_e_ _E_x_a_m_p_l_e_ _U_s_i_n_g_ _t_h_e_ _Q_u_a_l_i_t_a_s_._c_l_a_s_s_ _C_o_r_p_u_s_ _D_a_t_a_s_e_t - _2_._2_ _C_o_n_c_r_e_t_e
-_E_x_a_m_p_l_e_ _U_s_i_n_g_ _t_h_e_ _I_r_i_s_ _D_a_t_a_s_e_t - _2_._3_ _D_i_a_m_o_n_d_s_ _E_x_a_m_p_l_e - _3_ _D_a_t_a_s_e_t_s - _3_._1_ _U_s_e
-_Y_o_u_r_ _O_w_n - _3_._2_ _K_n_o_w_n_ _D_a_t_a_s_e_t_s - _4_ _P_e_r_s_o_n_a_l_i_z_i_n_g_ _t_h_e_ _W_e_b_ _A_p_p_l_i_c_a_t_i_o_n -
-_R_e_f_e_r_e_n_c_e_s --------------------------------------------------------------------
----- **Please Note**: ***Metrics As Scores*** (`MAS`) changed considerably
-between versions [**`v1.0.8`**](https://github.com/MrShoenel/metrics-as-scores/
-tree/v1.0.8) and **`v2.x.x`**. The current version is `v2.8.1`. From version
-**`v2.x.x`** it has the following new features: - [Textual User Interface
-(TUI)](#text-based-user-interface-tui) - Proper documentation and testing - New
-version on PyPI. Install the package and run the command line interface by
-typing **`mas`**! [Metrics As Scores Demo.](https://user-
-images.githubusercontent.com/5049151/219892077-58854478-b761-4a3d-9faf-
-2fe46c122cf5.webm) ------------------------------------------------------------
------------- Contains the data and scripts needed for the application
+(>=1.2.1,<2.0.0) Requires-Dist: scipy (>=1.10.1,<2.0.0) Requires-Dist: sphinx-
+rtd-theme (>=1.1.1,<2.0.0) Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-Dist: toml
+(>=0.10.2,<0.11.0) Requires-Dist: tqdm (>=4.64.1,<5.0.0) Requires-Dist: wget
+(>=3.2,<4.0) Project-URL: Repository, https://github.com/mrshoenel/metrics-as-
+scores/issues Description-Content-Type: text/markdown Metrics As Scores [![DOI]
+(https://zenodo.org/badge/524333119.svg)](https://zenodo.org/badge/latestdoi/
+524333119) [![status](https://joss.theoj.org/papers/
+eb549efe6c0111490395496c68717579/status.svg)](https://joss.theoj.org/papers/
+eb549efe6c0111490395496c68717579) [![codecov](https://codecov.io/github/
+MrShoenel/metrics-as-scores/branch/master/graph/badge.svg?token=HO1GYXVEUQ)]
+(https://codecov.io/github/MrShoenel/metrics-as-scores) ================ - _1
+_U_s_a_g_e - _1_._1_ _T_e_x_t_-_b_a_s_e_d_ _U_s_e_r_ _I_n_t_e_r_f_a_c_e_ _(_T_U_I_) - _1_._2_ _W_e_b_ _A_p_p_l_i_c_a_t_i_o_n - _1_._3
+_D_e_v_e_l_o_p_m_e_n_t_ _S_e_t_u_p - _1_._3_._1_ _S_e_t_t_i_n_g_ _U_p_ _a_ _V_i_r_t_u_a_l_ _E_n_v_i_r_o_n_m_e_n_t - _1_._3_._2_ _I_n_s_t_a_l_l_i_n_g
+_P_a_c_k_a_g_e_s - _1_._3_._3_ _R_u_n_n_i_n_g_ _T_e_s_t_s - _2_ _E_x_a_m_p_l_e_ _U_s_a_g_e - _2_._1_ _C_o_n_c_r_e_t_e_ _E_x_a_m_p_l_e_ _U_s_i_n_g
+_t_h_e_ _Q_u_a_l_i_t_a_s_._c_l_a_s_s_ _C_o_r_p_u_s_ _D_a_t_a_s_e_t - _2_._2_ _C_o_n_c_r_e_t_e_ _E_x_a_m_p_l_e_ _U_s_i_n_g_ _t_h_e_ _I_r_i_s_ _D_a_t_a_s_e_t
+- _2_._3_ _D_i_a_m_o_n_d_s_ _E_x_a_m_p_l_e - _3_ _D_a_t_a_s_e_t_s - _3_._1_ _U_s_e_ _Y_o_u_r_ _O_w_n - _3_._2_ _K_n_o_w_n_ _D_a_t_a_s_e_t_s - _4
+_P_e_r_s_o_n_a_l_i_z_i_n_g_ _t_h_e_ _W_e_b_ _A_p_p_l_i_c_a_t_i_o_n - _R_e_f_e_r_e_n_c_e_s --------------------------------
+---------------------------------------- **Please Note**: ***Metrics As
+Scores*** (`MAS`) changed considerably between versions [**`v1.0.8`**](https://
+github.com/MrShoenel/metrics-as-scores/tree/v1.0.8) and **`v2.x.x`**. The
+current version is `v2.8.2`. From version **`v2.x.x`** it has the following new
+features: - [Textual User Interface (TUI)](#text-based-user-interface-tui) -
+Proper documentation and testing - New version on PyPI. Install the package and
+run the command line interface by typing **`mas`**! [Metrics As Scores Demo.]
+(https://user-images.githubusercontent.com/5049151/219892077-58854478-b761-
+4a3d-9faf-2fe46c122cf5.webm) --------------------------------------------------
+---------------------- Contains the data and scripts needed for the application
 **`Metrics as Scores`**, check out _h_t_t_p_s_:_/_/_m_a_s_._r_e_s_e_a_r_c_h_._h_Ã_¶_n_e_l_._n_e_t_/. This
 package accompanies the paper entitled â*Contextual Operationalization of
 Metrics As Scores: Is My Metric Value Good?*â (HÃ¶nel et al. 2022). It seeks
 to answer the question whether or not the domain a software metric was captured
 in, matters. It enables the user to compare domains and to understand their
 differences. In order to answer the question of whether a metric value is
 actually good, we need to transform it into a **score**. Scores are normalized
```

