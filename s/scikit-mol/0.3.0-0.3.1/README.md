# Comparing `tmp/scikit_mol-0.3.0.tar.gz` & `tmp/scikit_mol-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit_mol-0.3.0.tar", last modified: Fri Apr 12 12:40:56 2024, max compression
+gzip compressed data, was "scikit_mol-0.3.1.tar", last modified: Fri Apr 26 09:54:38 2024, max compression
```

## Comparing `scikit_mol-0.3.0.tar` & `scikit_mol-0.3.1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.475579 scikit_mol-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/CITATION.bib
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/CONTRIBUTION.md
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-12 12:40:56.475579 scikit_mol-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.459579 scikit_mol-0.3.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    16093 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/01_basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/01_basic_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    41470 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/02_descriptor_transformer.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/02_descriptor_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.459579 scikit_mol-0.3.0/notebooks/02_descriptor_transformer_files/
--rw-r--r--   0 runner    (1001) docker     (127)    14040 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/02_descriptor_transformer_files/02_descriptor_transformer_5_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/03_example_pipeline.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/03_example_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/04_standardizer.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/04_standardizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.459579 scikit_mol-0.3.0/notebooks/04_standardizer_files/
--rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/04_standardizer_files/04_standardizer_3_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/04_standardizer_files/04_standardizer_3_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/05_smiles_sanitaztion.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/05_smiles_sanitaztion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/06_hyperparameter_tuning.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/06_hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    11673 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/07_parallel_transforms.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/07_parallel_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    54904 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/08_external_library_skopt.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/08_external_library_skopt.py
--rw-r--r--   0 runner    (1001) docker     (127)   266596 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/09_Combinatorial_Method_Usage_with_FingerPrint_Transformers.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18018 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/09_Combinatorial_Method_Usage_with_FingerPrint_Transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)   166074 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/10_pipeline_pandas_output.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11847 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/10_pipeline_pandas_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.463579 scikit_mol-0.3.0/notebooks/images/
--rw-r--r--   0 runner    (1001) docker     (127)    66320 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/AtomPairFingerprintTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (127)    60999 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/AtomPairFingerprintTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (127)    64259 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/Desc2DTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (127)    58977 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/Desc2DTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (127)    66054 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/MACCSTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (127)    60534 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/MACCSTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (127)    65268 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/MorganTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (127)    59856 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/MorganTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (127)    65110 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/RDKitFPTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (127)    60176 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/RDKitFPTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (127)    64025 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/SECFingerprintTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (127)    60783 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/SECFingerprintTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (127)    68278 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/TopologicalTorsionFingerprintTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (127)    60915 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/TopologicalTorsionFingerprintTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/Transformer_Widget.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    52959 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/max_speedup_vs_throughput.png
--rw-r--r--   0 runner    (1001) docker     (127)    46854 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/max_speedup_vs_throughput.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/pair_notebook.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      337 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/run_notebooks.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       25 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/sync_notebooks.sh
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.451579 scikit_mol-0.3.0/ressources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.467579 scikit_mol-0.3.0/ressources/logo/
--rw-r--r--   0 runner    (1001) docker     (127)  1389097 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo.ai
--rw-r--r--   0 runner    (1001) docker     (127)    70075 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_DarkBG.png
--rw-r--r--   0 runner    (1001) docker     (127)    33144 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_DarkBG_300px.png
--rw-r--r--   0 runner    (1001) docker     (127)   150544 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_DarkBG_600dpi.png
--rw-r--r--   0 runner    (1001) docker     (127)    66674 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_LightBG.png
--rw-r--r--   0 runner    (1001) docker     (127)    30449 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_LightBG_300px.png
--rw-r--r--   0 runner    (1001) docker     (127)   143920 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_LightBG_600dpi.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.471579 scikit_mol-0.3.0/scikit_mol/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/scikit_mol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 12:40:56.000000 scikit_mol-0.3.0/scikit_mol/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/scikit_mol/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/scikit_mol/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/scikit_mol/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)    25344 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/scikit_mol/fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/scikit_mol/standardizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/scikit_mol/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.471579 scikit_mol-0.3.0/scikit_mol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-12 12:40:56.000000 scikit_mol-0.3.0/scikit_mol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-12 12:40:56.000000 scikit_mol-0.3.0/scikit_mol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:40:56.000000 scikit_mol-0.3.0/scikit_mol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 12:40:56.000000 scikit_mol-0.3.0/scikit_mol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 12:40:56.000000 scikit_mol-0.3.0/scikit_mol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 12:40:56.475579 scikit_mol-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.471579 scikit_mol-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.471579 scikit_mol-0.3.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   469987 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/data/CDDD_SLC6A4_active_excapedb_subset.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)    18060 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/data/SLC6A4_active_excapedb_subset.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/test_desctransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11081 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/test_fptransformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/test_parameter_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/test_sanitizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/test_scikit_mol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/test_smilestomol.py
--rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:54:38.465525 scikit_mol-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/CITATION.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/CONTRIBUTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-26 09:54:38.465525 scikit_mol-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:54:38.449524 scikit_mol-0.3.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    16093 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/01_basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/01_basic_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41470 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/02_descriptor_transformer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/02_descriptor_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:54:38.449524 scikit_mol-0.3.1/notebooks/02_descriptor_transformer_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    14040 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/02_descriptor_transformer_files/02_descriptor_transformer_5_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/03_example_pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/03_example_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/04_standardizer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/04_standardizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:54:38.449524 scikit_mol-0.3.1/notebooks/04_standardizer_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/04_standardizer_files/04_standardizer_3_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/04_standardizer_files/04_standardizer_3_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/05_smiles_sanitaztion.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/05_smiles_sanitaztion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/06_hyperparameter_tuning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/06_hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11673 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/07_parallel_transforms.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/07_parallel_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54904 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/08_external_library_skopt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/08_external_library_skopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)   266596 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/09_Combinatorial_Method_Usage_with_FingerPrint_Transformers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18018 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/09_Combinatorial_Method_Usage_with_FingerPrint_Transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   166074 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/10_pipeline_pandas_output.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11847 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/10_pipeline_pandas_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:54:38.453524 scikit_mol-0.3.1/notebooks/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    66320 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/images/AtomPairFingerprintTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60999 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/images/AtomPairFingerprintTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    64259 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/images/Desc2DTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (127)    58977 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/images/Desc2DTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    66054 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/images/MACCSTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60534 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/images/MACCSTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    65268 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/images/MorganTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (127)    59856 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/images/MorganTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    65110 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/images/RDKitFPTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60176 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/images/RDKitFPTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    64025 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/images/SECFingerprintTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60783 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/images/SECFingerprintTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    68278 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/images/TopologicalTorsionFingerprintTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60915 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/images/TopologicalTorsionFingerprintTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/images/Transformer_Widget.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    52959 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/images/max_speedup_vs_throughput.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46854 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/images/max_speedup_vs_throughput.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/pair_notebook.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      337 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/run_notebooks.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       25 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/notebooks/sync_notebooks.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:54:38.445525 scikit_mol-0.3.1/ressources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:54:38.457524 scikit_mol-0.3.1/ressources/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)  1389097 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/ressources/logo/ScikitMol_Logo.ai
+-rw-r--r--   0 runner    (1001) docker     (127)    70075 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/ressources/logo/ScikitMol_Logo_DarkBG.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33144 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/ressources/logo/ScikitMol_Logo_DarkBG_300px.png
+-rw-r--r--   0 runner    (1001) docker     (127)   150544 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/ressources/logo/ScikitMol_Logo_DarkBG_600dpi.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66674 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/ressources/logo/ScikitMol_Logo_LightBG.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30449 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/ressources/logo/ScikitMol_Logo_LightBG_300px.png
+-rw-r--r--   0 runner    (1001) docker     (127)   143920 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/ressources/logo/ScikitMol_Logo_LightBG_600dpi.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:54:38.457524 scikit_mol-0.3.1/scikit_mol/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/scikit_mol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 09:54:38.000000 scikit_mol-0.3.1/scikit_mol/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/scikit_mol/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/scikit_mol/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/scikit_mol/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25344 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/scikit_mol/fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/scikit_mol/standardizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/scikit_mol/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:54:38.461525 scikit_mol-0.3.1/scikit_mol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-26 09:54:38.000000 scikit_mol-0.3.1/scikit_mol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-26 09:54:38.000000 scikit_mol-0.3.1/scikit_mol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:54:38.000000 scikit_mol-0.3.1/scikit_mol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-26 09:54:38.000000 scikit_mol-0.3.1/scikit_mol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 09:54:38.000000 scikit_mol-0.3.1/scikit_mol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-26 09:54:38.465525 scikit_mol-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:54:38.461525 scikit_mol-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:54:38.461525 scikit_mol-0.3.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   469987 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/tests/data/CDDD_SLC6A4_active_excapedb_subset.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    18060 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/tests/data/SLC6A4_active_excapedb_subset.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/tests/test_desctransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11081 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/tests/test_fptransformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/tests/test_parameter_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/tests/test_sanitizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/tests/test_scikit_mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/tests/test_smilestomol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-04-26 09:54:32.000000 scikit_mol-0.3.1/tests/test_transformers.py
```

### Comparing `scikit_mol-0.3.0/CITATION.bib` & `scikit_mol-0.3.1/CITATION.bib`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/CONTRIBUTION.md` & `scikit_mol-0.3.1/CONTRIBUTION.md`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/LICENSE` & `scikit_mol-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/PKG-INFO` & `scikit_mol-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scikit_mol
-Version: 0.3.0
+Version: 0.3.1
 Summary: scikit-learn classes for molecule transformation
 Home-page: https://github.com/EBjerrum/scikit-mol
 Download-URL: https://github.com/EBjerrum/scikit-mol
 Author: Esben Jannik Bjerrum
 Author-email: esben@cheminformania.com
-License: Apache-2.0
+License: LGPL-3.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scikit_mol-0.3.0/README.md` & `scikit_mol-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/01_basic_usage.ipynb` & `scikit_mol-0.3.1/notebooks/01_basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/01_basic_usage.py` & `scikit_mol-0.3.1/notebooks/01_basic_usage.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/02_descriptor_transformer.ipynb` & `scikit_mol-0.3.1/notebooks/02_descriptor_transformer.ipynb`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/02_descriptor_transformer.py` & `scikit_mol-0.3.1/notebooks/02_descriptor_transformer.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/02_descriptor_transformer_files/02_descriptor_transformer_5_0.png` & `scikit_mol-0.3.1/notebooks/02_descriptor_transformer_files/02_descriptor_transformer_5_0.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/03_example_pipeline.ipynb` & `scikit_mol-0.3.1/notebooks/03_example_pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/03_example_pipeline.py` & `scikit_mol-0.3.1/notebooks/03_example_pipeline.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/04_standardizer.ipynb` & `scikit_mol-0.3.1/notebooks/04_standardizer.ipynb`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/04_standardizer.py` & `scikit_mol-0.3.1/notebooks/04_standardizer.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/04_standardizer_files/04_standardizer_3_0.png` & `scikit_mol-0.3.1/notebooks/04_standardizer_files/04_standardizer_3_0.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/04_standardizer_files/04_standardizer_3_1.png` & `scikit_mol-0.3.1/notebooks/04_standardizer_files/04_standardizer_3_1.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/05_smiles_sanitaztion.ipynb` & `scikit_mol-0.3.1/notebooks/05_smiles_sanitaztion.ipynb`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/05_smiles_sanitaztion.py` & `scikit_mol-0.3.1/notebooks/05_smiles_sanitaztion.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/06_hyperparameter_tuning.ipynb` & `scikit_mol-0.3.1/notebooks/06_hyperparameter_tuning.ipynb`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/06_hyperparameter_tuning.py` & `scikit_mol-0.3.1/notebooks/06_hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/07_parallel_transforms.ipynb` & `scikit_mol-0.3.1/notebooks/07_parallel_transforms.ipynb`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/07_parallel_transforms.py` & `scikit_mol-0.3.1/notebooks/07_parallel_transforms.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/08_external_library_skopt.ipynb` & `scikit_mol-0.3.1/notebooks/08_external_library_skopt.ipynb`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/08_external_library_skopt.py` & `scikit_mol-0.3.1/notebooks/08_external_library_skopt.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/09_Combinatorial_Method_Usage_with_FingerPrint_Transformers.ipynb` & `scikit_mol-0.3.1/notebooks/09_Combinatorial_Method_Usage_with_FingerPrint_Transformers.ipynb`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/09_Combinatorial_Method_Usage_with_FingerPrint_Transformers.py` & `scikit_mol-0.3.1/notebooks/09_Combinatorial_Method_Usage_with_FingerPrint_Transformers.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/10_pipeline_pandas_output.ipynb` & `scikit_mol-0.3.1/notebooks/10_pipeline_pandas_output.ipynb`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/10_pipeline_pandas_output.py` & `scikit_mol-0.3.1/notebooks/10_pipeline_pandas_output.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/README.md` & `scikit_mol-0.3.1/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/images/AtomPairFingerprintTransformer_par.png` & `scikit_mol-0.3.1/notebooks/images/AtomPairFingerprintTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/images/AtomPairFingerprintTransformer_par.svg` & `scikit_mol-0.3.1/notebooks/images/AtomPairFingerprintTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/images/Desc2DTransformer_par.png` & `scikit_mol-0.3.1/notebooks/images/Desc2DTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/images/Desc2DTransformer_par.svg` & `scikit_mol-0.3.1/notebooks/images/Desc2DTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/images/MACCSTransformer_par.png` & `scikit_mol-0.3.1/notebooks/images/MACCSTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/images/MACCSTransformer_par.svg` & `scikit_mol-0.3.1/notebooks/images/MACCSTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/images/MorganTransformer_par.png` & `scikit_mol-0.3.1/notebooks/images/MorganTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/images/MorganTransformer_par.svg` & `scikit_mol-0.3.1/notebooks/images/MorganTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/images/RDKitFPTransformer_par.png` & `scikit_mol-0.3.1/notebooks/images/RDKitFPTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/images/RDKitFPTransformer_par.svg` & `scikit_mol-0.3.1/notebooks/images/RDKitFPTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/images/SECFingerprintTransformer_par.png` & `scikit_mol-0.3.1/notebooks/images/SECFingerprintTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/images/SECFingerprintTransformer_par.svg` & `scikit_mol-0.3.1/notebooks/images/SECFingerprintTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/images/TopologicalTorsionFingerprintTransformer_par.png` & `scikit_mol-0.3.1/notebooks/images/TopologicalTorsionFingerprintTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/images/TopologicalTorsionFingerprintTransformer_par.svg` & `scikit_mol-0.3.1/notebooks/images/TopologicalTorsionFingerprintTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/images/Transformer_Widget.jpg` & `scikit_mol-0.3.1/notebooks/images/Transformer_Widget.jpg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/images/max_speedup_vs_throughput.png` & `scikit_mol-0.3.1/notebooks/images/max_speedup_vs_throughput.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/notebooks/images/max_speedup_vs_throughput.svg` & `scikit_mol-0.3.1/notebooks/images/max_speedup_vs_throughput.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo.ai` & `scikit_mol-0.3.1/ressources/logo/ScikitMol_Logo.ai`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_DarkBG.png` & `scikit_mol-0.3.1/ressources/logo/ScikitMol_Logo_DarkBG.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_DarkBG_300px.png` & `scikit_mol-0.3.1/ressources/logo/ScikitMol_Logo_DarkBG_300px.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_DarkBG_600dpi.png` & `scikit_mol-0.3.1/ressources/logo/ScikitMol_Logo_DarkBG_600dpi.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_LightBG.png` & `scikit_mol-0.3.1/ressources/logo/ScikitMol_Logo_LightBG.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_LightBG_300px.png` & `scikit_mol-0.3.1/ressources/logo/ScikitMol_Logo_LightBG_300px.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_LightBG_600dpi.png` & `scikit_mol-0.3.1/ressources/logo/ScikitMol_Logo_LightBG_600dpi.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/scikit_mol/conversions.py` & `scikit_mol-0.3.1/scikit_mol/conversions.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/scikit_mol/core.py` & `scikit_mol-0.3.1/scikit_mol/core.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/scikit_mol/descriptors.py` & `scikit_mol-0.3.1/scikit_mol/descriptors.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/scikit_mol/fingerprints.py` & `scikit_mol-0.3.1/scikit_mol/fingerprints.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/scikit_mol/standardizer.py` & `scikit_mol-0.3.1/scikit_mol/standardizer.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/scikit_mol/utilities.py` & `scikit_mol-0.3.1/scikit_mol/utilities.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/scikit_mol.egg-info/PKG-INFO` & `scikit_mol-0.3.1/scikit_mol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scikit_mol
-Version: 0.3.0
+Version: 0.3.1
 Summary: scikit-learn classes for molecule transformation
 Home-page: https://github.com/EBjerrum/scikit-mol
 Download-URL: https://github.com/EBjerrum/scikit-mol
 Author: Esben Jannik Bjerrum
 Author-email: esben@cheminformania.com
-License: Apache-2.0
+License: LGPL-3.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scikit_mol-0.3.0/scikit_mol.egg-info/SOURCES.txt` & `scikit_mol-0.3.1/scikit_mol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/setup.cfg` & `scikit_mol-0.3.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = scikit_mol
 url = https://github.com/EBjerrum/scikit-mol
 download_url = https://github.com/EBjerrum/scikit-mol
-license = Apache-2.0
+license = LGPL-3.0
 license_file = LICENSE
 description = scikit-learn classes for molecule transformation
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Esben Jannik Bjerrum
 author_email = esben@cheminformania.com
 classifiers =
```

### Comparing `scikit_mol-0.3.0/tests/conftest.py` & `scikit_mol-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/tests/data/CDDD_SLC6A4_active_excapedb_subset.csv.gz` & `scikit_mol-0.3.1/tests/data/CDDD_SLC6A4_active_excapedb_subset.csv.gz`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/tests/data/SLC6A4_active_excapedb_subset.csv` & `scikit_mol-0.3.1/tests/data/SLC6A4_active_excapedb_subset.csv`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/tests/fixtures.py` & `scikit_mol-0.3.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/tests/test_desctransformer.py` & `scikit_mol-0.3.1/tests/test_desctransformer.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/tests/test_fptransformers.py` & `scikit_mol-0.3.1/tests/test_fptransformers.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/tests/test_parameter_types.py` & `scikit_mol-0.3.1/tests/test_parameter_types.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/tests/test_sanitizer.py` & `scikit_mol-0.3.1/tests/test_sanitizer.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/tests/test_smilestomol.py` & `scikit_mol-0.3.1/tests/test_smilestomol.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.3.0/tests/test_transformers.py` & `scikit_mol-0.3.1/tests/test_transformers.py`

 * *Files identical despite different names*

