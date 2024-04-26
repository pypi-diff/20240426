# Comparing `tmp/malariagen_data-8.8.0.tar.gz` & `tmp/malariagen_data-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malariagen_data-8.8.0.tar", max compression
+gzip compressed data, was "malariagen_data-9.0.0.tar", max compression
```

## Comparing `malariagen_data-8.8.0.tar` & `malariagen_data-9.0.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1067 2024-03-20 18:56:24.620680 malariagen_data-8.8.0/LICENSE
--rw-r--r--   0        0        0     2530 2024-03-20 18:56:24.620680 malariagen_data-8.8.0/README.md
--rw-r--r--   0        0        0      987 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/__init__.py
--rw-r--r--   0        0        0     7657 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/af1.py
--rw-r--r--   0        0        0    11991 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/ag3.py
--rw-r--r--   0        0        0     9451 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/amin1.py
--rw-r--r--   0        0        0        0 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/__init__.py
--rw-r--r--   0        0        0    10685 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/aim_data.py
--rw-r--r--   0        0        0      724 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/aim_params.py
--rw-r--r--   0        0        0    17482 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/base.py
--rw-r--r--   0        0        0     7078 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/base_params.py
--rw-r--r--   0        0        0    33322 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/cnv_data.py
--rw-r--r--   0        0        0      537 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/cnv_params.py
--rw-r--r--   0        0        0      903 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/dash_params.py
--rw-r--r--   0        0        0    10036 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/dipclust.py
--rw-r--r--   0        0        0      692 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/dipclust_params.py
--rw-r--r--   0        0        0      270 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/diplotype_distance_params.py
--rw-r--r--   0        0        0     2024 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/frq_params.py
--rw-r--r--   0        0        0    18115 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/fst.py
--rw-r--r--   0        0        0      690 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/fst_params.py
--rw-r--r--   0        0        0    21540 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/g123.py
--rw-r--r--   0        0        0     1083 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/g123_params.py
--rw-r--r--   0        0        0    15770 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/genome_features.py
--rw-r--r--   0        0        0     4300 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/genome_sequence.py
--rw-r--r--   0        0        0     2556 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/gplt_params.py
--rw-r--r--   0        0        0    16647 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/h12.py
--rw-r--r--   0        0        0      739 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/h12_params.py
--rw-r--r--   0        0        0    12730 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/h1x.py
--rw-r--r--   0        0        0    15233 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/hap_data.py
--rw-r--r--   0        0        0      288 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/hap_params.py
--rw-r--r--   0        0        0     9863 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/hapclust.py
--rw-r--r--   0        0        0      468 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/hapclust_params.py
--rw-r--r--   0        0        0      667 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/hapnet_params.py
--rw-r--r--   0        0        0     1323 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/het_params.py
--rw-r--r--   0        0        0     5883 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/igv.py
--rw-r--r--   0        0        0     2758 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/ihs_params.py
--rw-r--r--   0        0        0     1521 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/map_params.py
--rw-r--r--   0        0        0    15204 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/pca.py
--rw-r--r--   0        0        0      524 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/pca_params.py
--rw-r--r--   0        0        0     4533 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/plotly_params.py
--rw-r--r--   0        0        0    40182 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/sample_metadata.py
--rw-r--r--   0        0        0    64953 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/snp_data.py
--rw-r--r--   0        0        0    48792 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/snp_frq.py
--rw-r--r--   0        0        0      554 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/tree_params.py
--rw-r--r--   0        0        0     2046 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anoph/xpehh_params.py
--rw-r--r--   0        0        0   126711 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/anopheles.py
--rw-r--r--   0        0        0    10514 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/mjn.py
--rw-r--r--   0        0        0     1253 2024-03-20 18:56:24.624680 malariagen_data-8.8.0/malariagen_data/pf7.py
--rw-r--r--   0        0        0     4442 2024-03-20 18:56:24.628680 malariagen_data-8.8.0/malariagen_data/pf7_config.json
--rw-r--r--   0        0        0    11756 2024-03-20 18:56:24.628680 malariagen_data-8.8.0/malariagen_data/plasmodium.py
--rw-r--r--   0        0        0     3353 2024-03-20 18:56:24.628680 malariagen_data-8.8.0/malariagen_data/plotly_dendrogram.py
--rw-r--r--   0        0        0     1253 2024-03-20 18:56:24.628680 malariagen_data-8.8.0/malariagen_data/pv4.py
--rw-r--r--   0        0        0     2060 2024-03-20 18:56:24.628680 malariagen_data-8.8.0/malariagen_data/pv4_config.json
--rw-r--r--   0        0        0    38562 2024-03-20 18:56:24.628680 malariagen_data-8.8.0/malariagen_data/util.py
--rw-r--r--   0        0        0    18170 2024-03-20 18:56:24.628680 malariagen_data-8.8.0/malariagen_data/veff.py
--rw-r--r--   0        0        0     2457 2024-03-20 18:56:37.896743 malariagen_data-8.8.0/pyproject.toml
--rw-r--r--   0        0        0     4123 1970-01-01 00:00:00.000000 malariagen_data-8.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/LICENSE
+-rw-r--r--   0        0        0     2954 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/README.md
+-rw-r--r--   0        0        0      987 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/__init__.py
+-rw-r--r--   0        0        0     7663 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/af1.py
+-rw-r--r--   0        0        0    11997 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/ag3.py
+-rw-r--r--   0        0        0     9451 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/amin1.py
+-rw-r--r--   0        0        0        0 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/__init__.py
+-rw-r--r--   0        0        0    10685 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/aim_data.py
+-rw-r--r--   0        0        0      724 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/aim_params.py
+-rw-r--r--   0        0        0    18834 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/base.py
+-rw-r--r--   0        0        0     7078 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/base_params.py
+-rw-r--r--   0        0        0    33307 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/cnv_data.py
+-rw-r--r--   0        0        0      537 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/cnv_params.py
+-rw-r--r--   0        0        0      903 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/dash_params.py
+-rw-r--r--   0        0        0    10036 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/dipclust.py
+-rw-r--r--   0        0        0      692 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/dipclust_params.py
+-rw-r--r--   0        0        0      270 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/diplotype_distance_params.py
+-rw-r--r--   0        0        0     2024 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/frq_params.py
+-rw-r--r--   0        0        0    18115 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/fst.py
+-rw-r--r--   0        0        0      690 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/fst_params.py
+-rw-r--r--   0        0        0    21540 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/g123.py
+-rw-r--r--   0        0        0     1083 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/g123_params.py
+-rw-r--r--   0        0        0    15770 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/genome_features.py
+-rw-r--r--   0        0        0     4300 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/genome_sequence.py
+-rw-r--r--   0        0        0     2556 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/gplt_params.py
+-rw-r--r--   0        0        0    16647 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/h12.py
+-rw-r--r--   0        0        0      739 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/h12_params.py
+-rw-r--r--   0        0        0    12730 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/h1x.py
+-rw-r--r--   0        0        0    15233 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/hap_data.py
+-rw-r--r--   0        0        0      288 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/hap_params.py
+-rw-r--r--   0        0        0     9863 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/hapclust.py
+-rw-r--r--   0        0        0      468 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/hapclust_params.py
+-rw-r--r--   0        0        0      667 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/hapnet_params.py
+-rw-r--r--   0        0        0     1323 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/het_params.py
+-rw-r--r--   0        0        0     5883 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/igv.py
+-rw-r--r--   0        0        0     2758 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/ihs_params.py
+-rw-r--r--   0        0        0     1521 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/map_params.py
+-rw-r--r--   0        0        0    15204 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/pca.py
+-rw-r--r--   0        0        0      524 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/pca_params.py
+-rw-r--r--   0        0        0     4533 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/plotly_params.py
+-rw-r--r--   0        0        0    40182 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/sample_metadata.py
+-rw-r--r--   0        0        0    64953 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/snp_data.py
+-rw-r--r--   0        0        0    48792 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/snp_frq.py
+-rw-r--r--   0        0        0      554 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/tree_params.py
+-rw-r--r--   0        0        0     2046 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/xpehh_params.py
+-rw-r--r--   0        0        0   126711 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anopheles.py
+-rw-r--r--   0        0        0    10514 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/mjn.py
+-rw-r--r--   0        0        0     1253 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/pf7.py
+-rw-r--r--   0        0        0     4442 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/pf7_config.json
+-rw-r--r--   0        0        0    11756 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/plasmodium.py
+-rw-r--r--   0        0        0     3353 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/plotly_dendrogram.py
+-rw-r--r--   0        0        0     1253 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/pv4.py
+-rw-r--r--   0        0        0     2060 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/pv4_config.json
+-rw-r--r--   0        0        0    39556 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/util.py
+-rw-r--r--   0        0        0    18170 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/veff.py
+-rw-r--r--   0        0        0     2486 2024-04-26 06:46:49.708326 malariagen_data-9.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4594 1970-01-01 00:00:00.000000 malariagen_data-9.0.0/PKG-INFO
```

### Comparing `malariagen_data-8.8.0/LICENSE` & `malariagen_data-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/README.md` & `malariagen_data-9.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -40,65 +40,83 @@
 
 Fork and clone this repo:
 
 ```bash
 git clone git@github.com:[username]/malariagen-data-python.git
 ```
 
-Install Python 3.8 (current recommended version for local development), e.g.:
+Install Python, e.g.:
 
 ```bash
 sudo add-apt-repository ppa:deadsnakes/ppa
-sudo apt install python3.8 python3.8-venv
+sudo apt install python3.9 python3.9-venv
 ```
 
 Install pipx, e.g.:
 
 ```bash
-python3.8 -m pip install --user pipx
-python3.8 -m pipx ensurepath
+python3.9 -m pip install --user pipx
+python3.9 -m pipx ensurepath
 ```
 
 Install [poetry](https://python-poetry.org/docs/#installation), e.g.:
 
 ```bash
-pipx install poetry==1.4.1 --python=/usr/bin/python3.8
+pipx install poetry==1.8.2 --python=/usr/bin/python3.9
 ```
 
 Create development environment:
 
 ```bash
 cd malariagen-data-python
-poetry use 3.8
+poetry use 3.9
 poetry install
 ```
 
 Activate development environment:
 
 ```bash
 poetry shell
 ```
 
 Install pre-commit and pre-commit hooks:
 
 ```bash
-pipx install pre-commit --python=/usr/bin/python3.8
+pipx install pre-commit --python=/usr/bin/python3.9
 pre-commit install
 ```
 
 Run pre-commit checks (isort, black, blackdoc, flake8, ...) manually:
 
 ```bash
 pre-commit run --all-files
 ```
 
-Run tests:
+Run fast unit tests using simulated data:
 
 ```bash
-poetry run pytest -v
+poetry run pytest -v tests/anoph
+```
+
+To run legacy tests which read data from GCS, you'll need to [install the Google Cloud CLI](https://cloud.google.com/sdk/docs/install). E.g., if on Linux:
+
+```bash
+./install_gcloud.sh
+```
+
+You'll then need to obtain application-default credentials, e.g.:
+
+```bash
+./google-cloud-sdk/bin/gcloud auth application-default login
+```
+
+Once this is done, you can run legacy tests:
+
+```bash
+poetry run pytest --ignore=tests/anoph -v tests
 ```
 
 Tests will run slowly the first time, as data required for testing
 will be read from GCS. Subsequent runs will be faster as data will be
 cached locally in the "gcs_cache" folder.
 
 ## Release process
```

### Comparing `malariagen_data-8.8.0/malariagen_data/__init__.py` & `malariagen_data-9.0.0/malariagen_data/__init__.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/af1.py` & `malariagen_data-9.0.0/malariagen_data/af1.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,30 +131,30 @@
             f"Cohorts analysis        : {self._cohorts_analysis}\n"
             f"Site filters analysis   : {self._site_filters_analysis}\n"
             f"Software version        : malariagen_data {malariagen_data.__version__}\n"
             f"Client location         : {self.client_location}\n"
             f"---\n"
             f"Please note that data are subject to terms of use,\n"
             f"for more information see https://www.malariagen.net/data\n"
-            f"or contact data@malariagen.net. For API documentation see \n"
+            f"or contact support@malariagen.net. For API documentation see \n"
             f"https://malariagen.github.io/malariagen-data-python/v{malariagen_data.__version__}/Af1.html"
         )
         return text
 
     def _repr_html_(self):
         html = f"""
             <table class="malariagen-af1">
                 <thead>
                     <tr>
                         <th style="text-align: left" colspan="2">MalariaGEN Af1 API client</th>
                     </tr>
                     <tr><td colspan="2" style="text-align: left">
                         Please note that data are subject to terms of use,
                         for more information see <a href="https://www.malariagen.net/data">
-                        the MalariaGEN website</a> or contact data@malariagen.net.
+                        the MalariaGEN website</a> or contact support@malariagen.net.
                         See also the <a href="https://malariagen.github.io/malariagen-data-python/v{malariagen_data.__version__}/Af1.html">Af1 API docs</a>.
                     </td></tr>
                 </thead>
                 <tbody>
                     <tr>
                         <th style="text-align: left">
                             Storage URL
```

### Comparing `malariagen_data-8.8.0/malariagen_data/ag3.py` & `malariagen_data-9.0.0/malariagen_data/ag3.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,30 +211,30 @@
             f"AIM analysis            : {self._aim_analysis}\n"
             f"Site filters analysis   : {self._site_filters_analysis}\n"
             f"Software version        : malariagen_data {malariagen_data.__version__}\n"
             f"Client location         : {self.client_location}\n"
             f"---\n"
             f"Please note that data are subject to terms of use,\n"
             f"for more information see https://www.malariagen.net/data\n"
-            f"or contact data@malariagen.net. For API documentation see \n"
+            f"or contact support@malariagen.net. For API documentation see \n"
             f"https://malariagen.github.io/malariagen-data-python/v{malariagen_data.__version__}/Ag3.html"
         )
         return text
 
     def _repr_html_(self):
         html = f"""
             <table class="malariagen-ag3">
                 <thead>
                     <tr>
                         <th style="text-align: left" colspan="2">MalariaGEN Ag3 API client</th>
                     </tr>
                     <tr><td colspan="2" style="text-align: left">
                         Please note that data are subject to terms of use,
                         for more information see <a href="https://www.malariagen.net/data">
-                        the MalariaGEN website</a> or contact data@malariagen.net.
+                        the MalariaGEN website</a> or contact support@malariagen.net.
                         See also the <a href="https://malariagen.github.io/malariagen-data-python/v{malariagen_data.__version__}/Ag3.html">Ag3 API docs</a>.
                     </td></tr>
                 </thead>
                 <tbody>
                     <tr>
                         <th style="text-align: left">
                             Storage URL
```

### Comparing `malariagen_data-8.8.0/malariagen_data/amin1.py` & `malariagen_data-9.0.0/malariagen_data/amin1.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/aim_data.py` & `malariagen_data-9.0.0/malariagen_data/anoph/aim_data.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/aim_params.py` & `malariagen_data-9.0.0/malariagen_data/anoph/aim_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/base.py` & `malariagen_data-9.0.0/malariagen_data/anoph/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Literal,
     Mapping,
     Optional,
     Sequence,
     Tuple,
     Union,
 )
-
+from textwrap import dedent
 import bokeh.io
 import numpy as np
 import pandas as pd
 import zarr  # type: ignore
 from numpydoc_decorator import doc  # type: ignore
 from tqdm.auto import tqdm as tqdm_auto
 from tqdm.dask import TqdmCallback
@@ -72,18 +72,45 @@
         # Set up fsspec filesystem. N.B., we use fsspec here to allow for
         # accessing different types of storage - fsspec will automatically
         # detect which type of storage to use based on the URL provided.
         # E.g., if the URL begins with "gs://" then a GCSFileSystem will
         # be used to read from Google Cloud Storage.
         if storage_options is None:
             storage_options = dict()
-        self._fs, self._base_path = init_filesystem(url, **storage_options)
+        try:
+            self._fs, self._base_path = init_filesystem(url, **storage_options)
+        except Exception as exc:  # pragma: no cover
+            raise IOError(
+                "An error occurred establishing a connection to the storage system. Please see the nested exception for more details."
+            ) from exc
 
-        # Lazily load config.
-        self._config: Optional[Dict] = None
+        # Eagerly load config to trigger any access problems early.
+        try:
+            with self.open_file(self._config_path) as f:
+                self._config = json.load(f)
+        except Exception as exc:  # pragma: no cover
+            if isinstance(exc, OSError) and "forbidden" in str(exc):
+                # This seems to be the best way to detect the case where the
+                # current user is trying to access GCS but has not been granted
+                # permissions. Reraise with a helpful message.
+                raise PermissionError(
+                    dedent(
+                        """
+                           Your Google account does not appear to have permission to access the data.
+                           If you have not yet submitted a data access request, please complete the form
+                           at the following link: https://forms.gle/d1NV3aL3EoVQGSHYA
+
+                           If you are still experiencing problems accessing data, please email
+                           data@malariagen.net for support.
+                        """
+                    )
+                ) from exc
+            else:
+                # Some other kind of error, reraise.
+                raise exc
 
         # Get bokeh to output plots to the notebook - this is a common gotcha,
         # users forget to do this and wonder why bokeh plots don't show.
         if bokeh_output_notebook:  # pragma: no cover
             bokeh.io.output_notebook(hide_banner=True)
 
         # Check colab location is in the US.
@@ -182,17 +209,14 @@
             # Add retrieved files to the result.
             files.update(retrieved_files)
 
         return files
 
     @property
     def config(self) -> Dict:
-        if self._config is None:
-            with self.open_file(self._config_path) as f:
-                self._config = json.load(f)
         return self._config.copy()
 
     # Note regarding release identifiers and storage paths. Within the
     # data storage, we have used path segments like "v3", "v3.1", "v3.2",
     # etc., to separate data from different releases. There is an inconsistency
     # in this convention, because the "v3" should have been "v3.0". To
     # make the API more consistent, we would like to use consistent release
@@ -246,15 +270,17 @@
         summary="""
             Here we discover which releases are available, by listing the storage
             directory and examining the subdirectories. This may include "pre-releases"
             where data may be incomplete.
         """
     )
     def _discover_releases(self) -> Tuple[str, ...]:
-        sub_dirs = sorted([p.split("/")[-1] for p in self._fs.ls(self._base_path)])
+        sub_dirs = sorted(
+            [p.split("/")[-1] for p in self._fs.ls(self._base_path, detail=False)]
+        )
         discovered_releases = tuple(
             sorted(
                 [
                     self._path_to_release(d)
                     for d in sub_dirs
                     # FIXME: this matches v3 and v3.1, but also v3001.1
                     if d.startswith(f"v{self._major_version_number}")
```

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/base_params.py` & `malariagen_data-9.0.0/malariagen_data/anoph/base_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/cnv_data.py` & `malariagen_data-9.0.0/malariagen_data/anoph/cnv_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Optional, Sequence, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 import dask.array as da
 import numpy as np
 import pandas as pd
 import xarray as xr
 import zarr  # type: ignore
 from numpydoc_decorator import doc  # type: ignore
@@ -780,18 +780,18 @@
         debug("figure out X axis limits from data")
         x_min = start[0]
         x_max = end[-1]
 
         debug("set up plot title")
         title = "CNV HMM"
         if sample_sets is not None:
-            if isinstance(sample_sets, Sequence):
-                sample_sets_text = ", ".join(sample_sets)
-            else:
+            if isinstance(sample_sets, str):
                 sample_sets_text = sample_sets
+            else:
+                sample_sets_text = ", ".join(sample_sets)
             title += f" - {sample_sets_text}"
         if sample_query is not None:
             title += f" ({sample_query})"
 
         debug("figure out plot height")
         if height is None:
             plot_height = 100 + row_height * n_samples
```

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/cnv_params.py` & `malariagen_data-9.0.0/malariagen_data/anoph/cnv_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/dash_params.py` & `malariagen_data-9.0.0/malariagen_data/anoph/dash_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/dipclust.py` & `malariagen_data-9.0.0/malariagen_data/anoph/dipclust.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/dipclust_params.py` & `malariagen_data-9.0.0/malariagen_data/anoph/dipclust_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/frq_params.py` & `malariagen_data-9.0.0/malariagen_data/anoph/frq_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/fst.py` & `malariagen_data-9.0.0/malariagen_data/anoph/fst.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/fst_params.py` & `malariagen_data-9.0.0/malariagen_data/anoph/fst_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/g123.py` & `malariagen_data-9.0.0/malariagen_data/anoph/g123.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/g123_params.py` & `malariagen_data-9.0.0/malariagen_data/anoph/g123_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/genome_features.py` & `malariagen_data-9.0.0/malariagen_data/anoph/genome_features.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/genome_sequence.py` & `malariagen_data-9.0.0/malariagen_data/anoph/genome_sequence.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/gplt_params.py` & `malariagen_data-9.0.0/malariagen_data/anoph/gplt_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/h12.py` & `malariagen_data-9.0.0/malariagen_data/anoph/h12.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/h12_params.py` & `malariagen_data-9.0.0/malariagen_data/anoph/h12_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/h1x.py` & `malariagen_data-9.0.0/malariagen_data/anoph/h1x.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/hap_data.py` & `malariagen_data-9.0.0/malariagen_data/anoph/hap_data.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/hapclust.py` & `malariagen_data-9.0.0/malariagen_data/anoph/hapclust.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/hapnet_params.py` & `malariagen_data-9.0.0/malariagen_data/anoph/hapnet_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/het_params.py` & `malariagen_data-9.0.0/malariagen_data/anoph/het_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/igv.py` & `malariagen_data-9.0.0/malariagen_data/anoph/igv.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/ihs_params.py` & `malariagen_data-9.0.0/malariagen_data/anoph/ihs_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/map_params.py` & `malariagen_data-9.0.0/malariagen_data/anoph/map_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/pca.py` & `malariagen_data-9.0.0/malariagen_data/anoph/pca.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/pca_params.py` & `malariagen_data-9.0.0/malariagen_data/anoph/pca_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/plotly_params.py` & `malariagen_data-9.0.0/malariagen_data/anoph/plotly_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/sample_metadata.py` & `malariagen_data-9.0.0/malariagen_data/anoph/sample_metadata.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/snp_data.py` & `malariagen_data-9.0.0/malariagen_data/anoph/snp_data.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/snp_frq.py` & `malariagen_data-9.0.0/malariagen_data/anoph/snp_frq.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/tree_params.py` & `malariagen_data-9.0.0/malariagen_data/anoph/tree_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anoph/xpehh_params.py` & `malariagen_data-9.0.0/malariagen_data/anoph/xpehh_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/anopheles.py` & `malariagen_data-9.0.0/malariagen_data/anopheles.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/mjn.py` & `malariagen_data-9.0.0/malariagen_data/mjn.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/pf7.py` & `malariagen_data-9.0.0/malariagen_data/pf7.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/pf7_config.json` & `malariagen_data-9.0.0/malariagen_data/pf7_config.json`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/plasmodium.py` & `malariagen_data-9.0.0/malariagen_data/plasmodium.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/plotly_dendrogram.py` & `malariagen_data-9.0.0/malariagen_data/plotly_dendrogram.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/pv4.py` & `malariagen_data-9.0.0/malariagen_data/pv4.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/pv4_config.json` & `malariagen_data-9.0.0/malariagen_data/pv4_config.json`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/malariagen_data/util.py` & `malariagen_data-9.0.0/malariagen_data/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,28 +308,50 @@
 
     return v
 
 
 def init_filesystem(url, **kwargs):
     """Initialise a fsspec filesystem from a given base URL and parameters."""
 
-    # special case Google Cloud Storage, use anonymous access, avoids a delay
-    if url.startswith("gs://") or url.startswith("gcs://"):
-        kwargs["token"] = "anon"
-    elif "gs://" in url:
-        # chained URL
-        kwargs["gs"] = dict(token="anon")
-    elif "gcs://" in url:
-        # chained URL
-        kwargs["gcs"] = dict(token="anon")
+    # Special case Google Cloud Storage, authenticate the user.
+    if "gs://" in url or "gcs://" in url:
+        if colab is not None:  # pragma: no cover
+            # We are in colab, use colab's built-in authentication function.
+            colab.auth.authenticate_user()
+        else:
+            # Assume user has performed gcloud auth application-default login
+            pass
+        import google.auth  # type: ignore
+
+        # Load application-default credentials.
+        with warnings.catch_warnings():
+            # Warnings are generally not that useful here, silence them.
+            warnings.simplefilter("ignore")
+
+            # To make this work with a service account on github actions, the
+            # scopes parameter is needed, see also:
+            # https://stackoverflow.com/a/74562563/761177
+            credentials, _ = google.auth.default(
+                scopes=["https://www.googleapis.com/auth/cloud-platform"]
+            )
+
+        # Ensure credentials are passed through to gcsfs.
+        if url.startswith("gs://") or url.startswith("gcs://"):
+            kwargs["token"] = credentials
+        elif "gs://" in url:
+            # Chained URL.
+            kwargs["gs"] = dict(token=credentials)
+        elif "gcs://" in url:
+            # Chained URL.
+            kwargs["gcs"] = dict(token=credentials)
 
-    # process the url using fsspec
+    # Process the URL using fsspec.
     fs, path = url_to_fs(url, **kwargs)
 
-    # path compatibility, fsspec/gcsfs behaviour varies between version
+    # Path compatibility, fsspec/gcsfs behaviour varies between versions.
     while path.endswith("/"):
         path = path[:-1]
 
     return fs, path
 
 
 def init_zarr_store(fs, path):
```

### Comparing `malariagen_data-8.8.0/malariagen_data/veff.py` & `malariagen_data-9.0.0/malariagen_data/veff.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-8.8.0/pyproject.toml` & `malariagen_data-9.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "malariagen_data"
-version = "8.8.0"
+version = "9.0.0"
 description = "A package for accessing and analysing MalariaGEN data."
 readme = "README.md"
 documentation = "https://malariagen.github.io/malariagen-data-python/latest/"
 repository = "https://github.com/malariagen/malariagen-data-python"
 authors = [
     "Alistair Miles <alistair.miles@sanger.ac.uk>",
     "Chris Clarkson <cc28@sanger.ac.uk>",
@@ -14,28 +14,29 @@
     "Kelly Bennett <kb25@sanger.ac.uk>",
     "Sanjay Nagi <sanjay.nagi@lstmed.ac.uk>",
 ]
 license = "MIT"
 
 [tool.poetry.dependencies]
 # ensure compatibility with numba
-python = ">=3.8,<3.12"
+python = ">=3.9,<3.13"
 # ensure compatibility with numba
-numpy = "<1.27"
+numpy = "*"
 numba = "*"
 # force llvmlite above broken version
 llvmlite = ">0.34"
 scipy = "*"
 pandas = "*"
 zarr = "*"
 dask = {version="*", extras=["array"]}
 fsspec = "*"
 gcsfs = "*"
+google-auth = "*"
 BioPython = "*"
-scikit-allel = "*"
+scikit-allel = "1.3.8"
 xarray = "*"
 plotly = "*"
 # https://github.com/bokeh/bokeh/issues/12614
 # bokeh 3.0 has a problem with stretch sizing modes
 bokeh = ">=3.1.0"
 statsmodels = "*"
 ipyleaflet = ">=0.17.0"
@@ -51,15 +52,15 @@
 # ensure support for dash in jupyter notebooks
 # https://dash.plotly.com/dash-in-jupyter
 dash = ">=2.11.0"
 dash-cytoscape = "*"
 numpydoc_decorator = ">=2.1.0"
 typing_extensions = "*"
 typeguard = ">=4.0.0"
-protopunica = "*"
+protopunica = "0.14.8.post1"
 # accelerate plotly - https://plotly.com/python/renderers/#performance
 orjson = "*"
 # providers spinners
 yaspin = "*"
 # provides efficient neighbour-joining tree implementation
 biotite = "*"
```

### Comparing `malariagen_data-8.8.0/PKG-INFO` & `malariagen_data-9.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: malariagen_data
-Version: 8.8.0
+Version: 9.0.0
 Summary: A package for accessing and analysing MalariaGEN data.
 Home-page: https://github.com/malariagen/malariagen-data-python
 License: MIT
 Author: Alistair Miles
 Author-email: alistair.miles@sanger.ac.uk
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: BioPython
 Requires-Dist: biotite
 Requires-Dist: bokeh (>=3.1.0)
 Requires-Dist: dash (>=2.11.0)
 Requires-Dist: dash-cytoscape
 Requires-Dist: dask[array]
 Requires-Dist: fsspec
 Requires-Dist: gcsfs
+Requires-Dist: google-auth
 Requires-Dist: igv-notebook (>=0.2.3)
 Requires-Dist: ipinfo (!=4.4.1)
 Requires-Dist: ipyleaflet (>=0.17.0)
 Requires-Dist: ipywidgets
 Requires-Dist: llvmlite (>0.34)
 Requires-Dist: numba
-Requires-Dist: numpy (<1.27)
+Requires-Dist: numpy
 Requires-Dist: numpydoc_decorator (>=2.1.0)
 Requires-Dist: orjson
 Requires-Dist: pandas
 Requires-Dist: plotly
-Requires-Dist: protopunica
-Requires-Dist: scikit-allel
+Requires-Dist: protopunica (==0.14.8.post1)
+Requires-Dist: scikit-allel (==1.3.8)
 Requires-Dist: scipy
 Requires-Dist: statsmodels
 Requires-Dist: tqdm
 Requires-Dist: typeguard (>=4.0.0)
 Requires-Dist: typing_extensions
 Requires-Dist: xarray
 Requires-Dist: yaspin
@@ -88,65 +89,83 @@
 
 Fork and clone this repo:
 
 ```bash
 git clone git@github.com:[username]/malariagen-data-python.git
 ```
 
-Install Python 3.8 (current recommended version for local development), e.g.:
+Install Python, e.g.:
 
 ```bash
 sudo add-apt-repository ppa:deadsnakes/ppa
-sudo apt install python3.8 python3.8-venv
+sudo apt install python3.9 python3.9-venv
 ```
 
 Install pipx, e.g.:
 
 ```bash
-python3.8 -m pip install --user pipx
-python3.8 -m pipx ensurepath
+python3.9 -m pip install --user pipx
+python3.9 -m pipx ensurepath
 ```
 
 Install [poetry](https://python-poetry.org/docs/#installation), e.g.:
 
 ```bash
-pipx install poetry==1.4.1 --python=/usr/bin/python3.8
+pipx install poetry==1.8.2 --python=/usr/bin/python3.9
 ```
 
 Create development environment:
 
 ```bash
 cd malariagen-data-python
-poetry use 3.8
+poetry use 3.9
 poetry install
 ```
 
 Activate development environment:
 
 ```bash
 poetry shell
 ```
 
 Install pre-commit and pre-commit hooks:
 
 ```bash
-pipx install pre-commit --python=/usr/bin/python3.8
+pipx install pre-commit --python=/usr/bin/python3.9
 pre-commit install
 ```
 
 Run pre-commit checks (isort, black, blackdoc, flake8, ...) manually:
 
 ```bash
 pre-commit run --all-files
 ```
 
-Run tests:
+Run fast unit tests using simulated data:
 
 ```bash
-poetry run pytest -v
+poetry run pytest -v tests/anoph
+```
+
+To run legacy tests which read data from GCS, you'll need to [install the Google Cloud CLI](https://cloud.google.com/sdk/docs/install). E.g., if on Linux:
+
+```bash
+./install_gcloud.sh
+```
+
+You'll then need to obtain application-default credentials, e.g.:
+
+```bash
+./google-cloud-sdk/bin/gcloud auth application-default login
+```
+
+Once this is done, you can run legacy tests:
+
+```bash
+poetry run pytest --ignore=tests/anoph -v tests
 ```
 
 Tests will run slowly the first time, as data required for testing
 will be read from GCS. Subsequent runs will be faster as data will be
 cached locally in the "gcs_cache" folder.
 
 ## Release process
```

