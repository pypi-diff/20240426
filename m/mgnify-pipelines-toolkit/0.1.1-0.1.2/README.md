# Comparing `tmp/mgnify_pipelines_toolkit-0.1.1.tar.gz` & `tmp/mgnify_pipelines_toolkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgnify_pipelines_toolkit-0.1.1.tar", last modified: Thu Feb 22 09:03:32 2024, max compression
+gzip compressed data, was "mgnify_pipelines_toolkit-0.1.2.tar", last modified: Fri Apr 26 11:43:50 2024, max compression
```

## Comparing `mgnify_pipelines_toolkit-0.1.1.tar` & `mgnify_pipelines_toolkit-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 09:03:32.456849 mgnify_pipelines_toolkit-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-02-22 09:03:32.456849 mgnify_pipelines_toolkit-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 09:03:32.452848 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 09:03:32.452848 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 09:03:32.456849 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/
--rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/amplicon_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/are_there_primers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/assess_inflection_point_mcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/assess_mcp_proportions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18392 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/classify_var_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/find_mcp_inflection_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/make_asv_count_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/remove_ambiguous_reads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/rev_comp_se_primers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/standard_primer_matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 09:03:32.456849 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/shared/get_subunits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/shared/get_subunits_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/shared/mapseq2biom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 09:03:32.456849 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/constants/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/constants/regex_ambiguous_bases.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/constants/tax_ranks.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/constants/thresholds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/constants/var_region_coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 09:03:32.456849 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-02-22 09:03:32.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-02-22 09:03:32.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 09:03:32.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-22 09:03:32.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-22 09:03:32.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-22 09:03:32.000000 mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-02-22 09:03:24.000000 mgnify_pipelines_toolkit-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 09:03:32.456849 mgnify_pipelines_toolkit-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:50.835709 mgnify_pipelines_toolkit-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-26 11:43:50.835709 mgnify_pipelines_toolkit-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:50.827709 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:50.827709 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:50.831709 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/amplicon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/are_there_primers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/assess_inflection_point_mcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/assess_mcp_proportions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18392 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/classify_var_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/find_mcp_inflection_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/make_asv_count_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/mapseq_to_asv_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/remove_ambiguous_reads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/rev_comp_se_primers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/standard_primer_matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:50.831709 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/shared/get_subunits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/shared/get_subunits_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/shared/mapseq2biom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:50.831709 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/constants/regex_ambiguous_bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/constants/tax_ranks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/constants/thresholds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/constants/var_region_coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:50.831709 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-26 11:43:50.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-26 11:43:50.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:43:50.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-26 11:43:50.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-26 11:43:50.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-26 11:43:50.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 11:43:50.835709 mgnify_pipelines_toolkit-0.1.2/setup.cfg
```

### Comparing `mgnify_pipelines_toolkit-0.1.1/LICENSE` & `mgnify_pipelines_toolkit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.1/PKG-INFO` & `mgnify_pipelines_toolkit-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgnify_pipelines_toolkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Collection of scripts and tools for MGnify pipelines
 Author-email: MGnify team <metagenomics-help@ebi.ac.uk>
 License: Apache Software License 2.0
 Keywords: bioinformatics,pipelines,metagenomics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -51,39 +51,41 @@
 `get_subunits -i ${easel_coords} -n ${meta.id}`
 
 ## Adding a new script to the package
 
 ### New script requirements
 
 There are a few requirements for your script:
+
 - It needs to have a named main function of some kind. See `mgnify_pipelines_toolkit/analysis/shared/get_subunits.py` and the `main()` function for an example
 - Because this package is meant to be run from the command-line, make sure your script can easily pass arguments using tools like `argparse` or `click`
 - A small amount of dependencies. This requirement is subjective, but for example if your script only requires a handful of basic packages like `Biopython`, `numpy`, `pandas`, etc., then it's fine. However if the script has a more extensive list of dependencies, a container is probably a better fit.
 
 ### How to add a new script
 
-To add a new Python script, first copy it over to the `mgnify_pipelines_toolkit` directory in this repository, specifically to the subdirectory that makes the most sense. If none of the subdirectories make sense for your script, create a new one. If your script doesn't have a `main()` type function yet, write one. 
+To add a new Python script, first copy it over to the `mgnify_pipelines_toolkit` directory in this repository, specifically to the subdirectory that makes the most sense. If none of the subdirectories make sense for your script, create a new one. If your script doesn't have a `main()` type function yet, write one.
 
 Then, open `pyproject.toml` as you will need to add some bits. First, add any missing dependencies (include the version) to the `dependencies` field.
 
 Then, if you created a new subdirectory to add your script in, go to the `packages` line under `[tool.setuptools]` and add the new subdirectory following the same syntax.
 
 Then, scroll down to the `[project.scripts]` line. Here, you will create an alias command for running your script from the command-line. In the example line:
 
 `get_subunits = "mgnify_pipelines_toolkit.analysis.shared.get_subunits:main"`
 
 - `get_subunits` is the alias
 - `mgnify_pipelines_toolkit.analysis.shared.get_subunits` will link the alias to the script with the path `mgnify_pipelines_toolkit/analysis/shared/get_subunits.py`
-- `:main` will specifically call the function named `main()` when the alias is run. 
+- `:main` will specifically call the function named `main()` when the alias is run.
 
 When you have setup this command, executing `get_subunits` on the command-line will be the equivalent of doing:
 
 `from mgnify_pipelines_toolkit.analysis.shared.get_subunits import main; main()`
 
 You should then write at least one unit test for your addition. This package uses `pytest` at the moment for this purpose. A GitHub Action workflow will run all of the unit tests whenever a commit is pushed to any branch.
 
 Finally, you will need to bump up the version in the `version` line.
 
 At the moment, these should be the only steps required to setup your script in this package (which is subject to change).
 
 ### Building and uploading to PyPi
+
 The building and pushing of the package is automated by GitHub Actions, which will activate only on a new release. Bioconda should then automatically pick up the new PyPi release and push it to their recipes, though it's worth keeping an eye on their automated pull requests just in case [here](https://github.com/bioconda/bioconda-recipes/pulls).
```

### Comparing `mgnify_pipelines_toolkit-0.1.1/README.md` & `mgnify_pipelines_toolkit-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,39 +26,41 @@
 `get_subunits -i ${easel_coords} -n ${meta.id}`
 
 ## Adding a new script to the package
 
 ### New script requirements
 
 There are a few requirements for your script:
+
 - It needs to have a named main function of some kind. See `mgnify_pipelines_toolkit/analysis/shared/get_subunits.py` and the `main()` function for an example
 - Because this package is meant to be run from the command-line, make sure your script can easily pass arguments using tools like `argparse` or `click`
 - A small amount of dependencies. This requirement is subjective, but for example if your script only requires a handful of basic packages like `Biopython`, `numpy`, `pandas`, etc., then it's fine. However if the script has a more extensive list of dependencies, a container is probably a better fit.
 
 ### How to add a new script
 
-To add a new Python script, first copy it over to the `mgnify_pipelines_toolkit` directory in this repository, specifically to the subdirectory that makes the most sense. If none of the subdirectories make sense for your script, create a new one. If your script doesn't have a `main()` type function yet, write one. 
+To add a new Python script, first copy it over to the `mgnify_pipelines_toolkit` directory in this repository, specifically to the subdirectory that makes the most sense. If none of the subdirectories make sense for your script, create a new one. If your script doesn't have a `main()` type function yet, write one.
 
 Then, open `pyproject.toml` as you will need to add some bits. First, add any missing dependencies (include the version) to the `dependencies` field.
 
 Then, if you created a new subdirectory to add your script in, go to the `packages` line under `[tool.setuptools]` and add the new subdirectory following the same syntax.
 
 Then, scroll down to the `[project.scripts]` line. Here, you will create an alias command for running your script from the command-line. In the example line:
 
 `get_subunits = "mgnify_pipelines_toolkit.analysis.shared.get_subunits:main"`
 
 - `get_subunits` is the alias
 - `mgnify_pipelines_toolkit.analysis.shared.get_subunits` will link the alias to the script with the path `mgnify_pipelines_toolkit/analysis/shared/get_subunits.py`
-- `:main` will specifically call the function named `main()` when the alias is run. 
+- `:main` will specifically call the function named `main()` when the alias is run.
 
 When you have setup this command, executing `get_subunits` on the command-line will be the equivalent of doing:
 
 `from mgnify_pipelines_toolkit.analysis.shared.get_subunits import main; main()`
 
 You should then write at least one unit test for your addition. This package uses `pytest` at the moment for this purpose. A GitHub Action workflow will run all of the unit tests whenever a commit is pushed to any branch.
 
 Finally, you will need to bump up the version in the `version` line.
 
 At the moment, these should be the only steps required to setup your script in this package (which is subject to change).
 
 ### Building and uploading to PyPi
-The building and pushing of the package is automated by GitHub Actions, which will activate only on a new release. Bioconda should then automatically pick up the new PyPi release and push it to their recipes, though it's worth keeping an eye on their automated pull requests just in case [here](https://github.com/bioconda/bioconda-recipes/pulls).
+
+The building and pushing of the package is automated by GitHub Actions, which will activate only on a new release. Bioconda should then automatically pick up the new PyPi release and push it to their recipes, though it's worth keeping an eye on their automated pull requests just in case [here](https://github.com/bioconda/bioconda-recipes/pulls).
```

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/amplicon_utils.py` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/amplicon_utils.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/are_there_primers.py` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/are_there_primers.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/assess_inflection_point_mcp.py` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/assess_inflection_point_mcp.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/assess_mcp_proportions.py` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/assess_mcp_proportions.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/classify_var_regions.py` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/classify_var_regions.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/find_mcp_inflection_points.py` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/find_mcp_inflection_points.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/make_asv_count_table.py` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/make_asv_count_table.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 logging.basicConfig(level=logging.DEBUG)
 
 def parse_args():
 
     parser = argparse.ArgumentParser()
 
-    parser.add_argument("-t", "--taxa", required=True, type=str, help="Path to DADA2 taxa file")
+    parser.add_argument("-t", "--taxa", required=True, type=str, help="Path to taxa file")
     parser.add_argument("-f", "--fwd", required=True, type=str, help="Path to DADA2 forward map file")
     parser.add_argument("-r", "--rev", required=False, type=str, help="Path to DADA2 reverse map file")
     parser.add_argument("-a", "--amp", required=True, type=str, help="Path to extracted amp_region reads from inference subworkflow")
     parser.add_argument("-hd", "--headers", required=True, type=str, help="Path to fastq headers")
     parser.add_argument("-s", "--sample", required=True, type=str, help="Sample ID")
 
     args = parser.parse_args()
@@ -45,15 +45,15 @@
     _SAMPLE = args.sample
 
     return _TAXA, _FWD, _REV, _AMP, _HEADERS, _SAMPLE
 
 
 def order_df(taxa_df):
 
-    if len(taxa_df.columns) == 8:
+    if len(taxa_df.columns) == 9:
         taxa_df = taxa_df.sort_values(_SILVA_TAX_RANKS, ascending=True)
     elif len(taxa_df.columns) == 10:
         taxa_df = taxa_df.sort_values(_PR2_TAX_RANKS, ascending=True)
     else:
         logging.error("Data frame not the right size, something wrong.")
         exit(1)
 
@@ -62,72 +62,80 @@
 def make_tax_assignment_dict_silva(taxa_df, asv_dict):
 
     tax_assignment_dict = defaultdict(int)
 
     for i in range(len(taxa_df)):
         
         sorted_index = taxa_df.index[i]
-        asv_count = asv_dict[sorted_index]
+        asv_num = taxa_df.iloc[i, 0]
+        asv_count = asv_dict[asv_num]
 
         if asv_count == 0:
             continue
 
+        sk = taxa_df.loc[sorted_index, "Superkingdom"]
         k = taxa_df.loc[sorted_index, "Kingdom"]
         p = taxa_df.loc[sorted_index, "Phylum"]
         c = taxa_df.loc[sorted_index, "Class"]
         o = taxa_df.loc[sorted_index, "Order"]
         f = taxa_df.loc[sorted_index, "Family"]
         g = taxa_df.loc[sorted_index, "Genus"]        
         s = taxa_df.loc[sorted_index, "Species"]
 
         tax_assignment = ""
 
         while True:
 
+            if sk != "0":
+                sk = "_".join(sk.split(" "))
+                tax_assignment += sk
+            else:
+                break
+
             if k != "0":
                 k = "_".join(k.split(" "))
-                if k == "Archaea" or k == "Bacteria":
-                    tax_assignment += f"sk__{k}"
-                elif k == "Eukaryota":
-                    tax_assignment += f"sk__Eukaryota"
-                else:
-                    tax_assignment += f"sk__Eukaryota\tk__{k}"
+                tax_assignment += f"\t{k}"
+            elif sk != "0":
+                tax_assignment += f"\tk__"
             else:
                 break
 
             if p != "0":
-                if k == "Archaea" or k == "Bacteria":
-                    tax_assignment += f"\tk__"
                 p = "_".join(p.split(" "))
-                tax_assignment += f"\tp__{p}"
+                tax_assignment += f"\t{p}"
             else:
                 break
+
             if c != "0":
                 c = "_".join(c.split(" "))
-                tax_assignment += f"\tc__{c}"
+                tax_assignment += f"\t{c}"
             else:
                 break
+
             if o != "0":
                 o = "_".join(o.split(" "))
-                tax_assignment += f"\to__{o}"
+                tax_assignment += f"\t{o}"
             else:
                 break
+
             if f != "0":
                 f = "_".join(f.split(" "))
-                tax_assignment += f"\tf__{f}"
+                tax_assignment += f"\t{f}"
             else:
                 break
+
             if g != "0":
                 g = "_".join(g.split(" "))
-                tax_assignment += f"\tg__{g}"
+                tax_assignment += f"\t{g}"
             else:
                 break
+
             if s != "0":
                 s = "_".join(s.split(" "))
-                tax_assignment += f"\ts__{s}"
+                tax_assignment += f"\t{s}"
             break
 
         if tax_assignment == "":
             continue
 
         tax_assignment_dict[tax_assignment] += asv_count
     
@@ -136,15 +144,16 @@
 def make_tax_assignment_dict_pr2(taxa_df, asv_dict):
 
     tax_assignment_dict = defaultdict(int)
 
     for i in range(len(taxa_df)):
         
         sorted_index = taxa_df.index[i]
-        asv_count = asv_dict[sorted_index]
+        asv_num = taxa_df.iloc[i, 0]
+        asv_count = asv_dict[asv_num]
 
         if asv_count == 0:
             continue
 
         d = taxa_df.loc[sorted_index, "Domain"]
         sg = taxa_df.loc[sorted_index, "Supergroup"]
         dv = taxa_df.loc[sorted_index, "Division"]
@@ -157,53 +166,63 @@
 
         tax_assignment = ""
 
         while True:
 
             if d != "0":
                 d = "_".join(d.split(" "))
-                tax_assignment += f"d__{d}"
+                tax_assignment += d
             else:
                 break
 
             if sg != "0":
                 sg = "_".join(sg.split(" "))
-                tax_assignment += f"\tsg__{sg}"
+                tax_assignment += f"\t{sg}"
             else:
                 break
+
             if dv != "0":
                 dv = "_".join(dv.split(" "))
-                tax_assignment += f"\tdv__{dv}"
+                tax_assignment += f"\t{dv}"
+            else:
+                break
 
             if sdv != "0":
                 sdv = "_".join(sdv.split(" "))
-                tax_assignment += f"\tsdv__{sdv}"
+                tax_assignment += f"\t{sdv}"
+            else:
+                break
+
             if c != "0":
                 c = "_".join(c.split(" "))
-                tax_assignment += f"\tc__{c}"
+                tax_assignment += f"\t{c}"
             else:
                 break
+
             if o != "0":
                 o = "_".join(o.split(" "))
-                tax_assignment += f"\to__{o}"
+                tax_assignment += f"\t{o}"
             else:
                 break
+
             if f != "0":
                 f = "_".join(f.split(" "))
-                tax_assignment += f"\tf__{f}"
+                tax_assignment += f"\t{f}"
             else:
                 break
+
             if g != "0":
                 g = "_".join(g.split(" "))
-                tax_assignment += f"\tg__{g}"
+                tax_assignment += f"\t{g}"
             else:
                 break
+
             if s != "0":
                 s = "_".join(s.split(" "))
-                tax_assignment += f"\ts__{s}"
+                tax_assignment += f"\t{s}"
             break
 
         if tax_assignment == "":
             continue
 
         tax_assignment_dict[tax_assignment] += asv_count
 
@@ -249,23 +268,23 @@
             
             if len(asv_intersection) == 1 and asv_intersection[0] == "0":
                 continue
         else:
             asv_intersection = fwd_asvs
 
         if headers[counter] in amp_reads:
-            asv_dict[int(asv_intersection[0]) - 1] += 1
+            asv_dict[f"seq_{int(asv_intersection[0]) - 1}"] += 1
     
     fwd_fr.close()
     if paired_end:
         rev_fr.close()
 
     ref_db = ""
 
-    if len(taxa_df.columns) == 8:
+    if len(taxa_df.columns) == 9:
         tax_assignment_dict = make_tax_assignment_dict_silva(taxa_df, asv_dict)
         ref_db = "silva"
     elif len(taxa_df.columns) == 10:
         tax_assignment_dict = make_tax_assignment_dict_pr2(taxa_df, asv_dict)
         ref_db = "pr2"
 
     with open(f"./{_SAMPLE}_{amp_region}_{ref_db}_asv_krona_counts.txt", "w") as fw:
```

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/remove_ambiguous_reads.py` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/remove_ambiguous_reads.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/rev_comp_se_primers.py` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/rev_comp_se_primers.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/amplicon/standard_primer_matching.py` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/standard_primer_matching.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/shared/get_subunits.py` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/shared/get_subunits.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/shared/get_subunits_coords.py` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/shared/get_subunits_coords.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/analysis/shared/mapseq2biom.py` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/shared/mapseq2biom.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/constants/regex_ambiguous_bases.py` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/constants/regex_ambiguous_bases.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/constants/tax_ranks.py` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/constants/tax_ranks.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-_SILVA_TAX_RANKS = ["Kingdom", "Phylum", "Class", "Order", "Family", "Genus", "Species"]
+_SILVA_TAX_RANKS = ["Superkingdom", "Kingdom", "Phylum", "Class", "Order", "Family", "Genus", "Species"]
 _PR2_TAX_RANKS = ["Domain", "Supergroup", "Division", "Subdivision", "Class", "Order", "Family", "Genus", "Species"]
```

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/constants/thresholds.py` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/constants/thresholds.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit/constants/var_region_coordinates.py` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/constants/var_region_coordinates.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit.egg-info/PKG-INFO` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgnify_pipelines_toolkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Collection of scripts and tools for MGnify pipelines
 Author-email: MGnify team <metagenomics-help@ebi.ac.uk>
 License: Apache Software License 2.0
 Keywords: bioinformatics,pipelines,metagenomics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -51,39 +51,41 @@
 `get_subunits -i ${easel_coords} -n ${meta.id}`
 
 ## Adding a new script to the package
 
 ### New script requirements
 
 There are a few requirements for your script:
+
 - It needs to have a named main function of some kind. See `mgnify_pipelines_toolkit/analysis/shared/get_subunits.py` and the `main()` function for an example
 - Because this package is meant to be run from the command-line, make sure your script can easily pass arguments using tools like `argparse` or `click`
 - A small amount of dependencies. This requirement is subjective, but for example if your script only requires a handful of basic packages like `Biopython`, `numpy`, `pandas`, etc., then it's fine. However if the script has a more extensive list of dependencies, a container is probably a better fit.
 
 ### How to add a new script
 
-To add a new Python script, first copy it over to the `mgnify_pipelines_toolkit` directory in this repository, specifically to the subdirectory that makes the most sense. If none of the subdirectories make sense for your script, create a new one. If your script doesn't have a `main()` type function yet, write one. 
+To add a new Python script, first copy it over to the `mgnify_pipelines_toolkit` directory in this repository, specifically to the subdirectory that makes the most sense. If none of the subdirectories make sense for your script, create a new one. If your script doesn't have a `main()` type function yet, write one.
 
 Then, open `pyproject.toml` as you will need to add some bits. First, add any missing dependencies (include the version) to the `dependencies` field.
 
 Then, if you created a new subdirectory to add your script in, go to the `packages` line under `[tool.setuptools]` and add the new subdirectory following the same syntax.
 
 Then, scroll down to the `[project.scripts]` line. Here, you will create an alias command for running your script from the command-line. In the example line:
 
 `get_subunits = "mgnify_pipelines_toolkit.analysis.shared.get_subunits:main"`
 
 - `get_subunits` is the alias
 - `mgnify_pipelines_toolkit.analysis.shared.get_subunits` will link the alias to the script with the path `mgnify_pipelines_toolkit/analysis/shared/get_subunits.py`
-- `:main` will specifically call the function named `main()` when the alias is run. 
+- `:main` will specifically call the function named `main()` when the alias is run.
 
 When you have setup this command, executing `get_subunits` on the command-line will be the equivalent of doing:
 
 `from mgnify_pipelines_toolkit.analysis.shared.get_subunits import main; main()`
 
 You should then write at least one unit test for your addition. This package uses `pytest` at the moment for this purpose. A GitHub Action workflow will run all of the unit tests whenever a commit is pushed to any branch.
 
 Finally, you will need to bump up the version in the `version` line.
 
 At the moment, these should be the only steps required to setup your script in this package (which is subject to change).
 
 ### Building and uploading to PyPi
+
 The building and pushing of the package is automated by GitHub Actions, which will activate only on a new release. Bioconda should then automatically pick up the new PyPi release and push it to their recipes, though it's worth keeping an eye on their automated pull requests just in case [here](https://github.com/bioconda/bioconda-recipes/pulls).
```

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit.egg-info/SOURCES.txt` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 mgnify_pipelines_toolkit/analysis/amplicon/amplicon_utils.py
 mgnify_pipelines_toolkit/analysis/amplicon/are_there_primers.py
 mgnify_pipelines_toolkit/analysis/amplicon/assess_inflection_point_mcp.py
 mgnify_pipelines_toolkit/analysis/amplicon/assess_mcp_proportions.py
 mgnify_pipelines_toolkit/analysis/amplicon/classify_var_regions.py
 mgnify_pipelines_toolkit/analysis/amplicon/find_mcp_inflection_points.py
 mgnify_pipelines_toolkit/analysis/amplicon/make_asv_count_table.py
+mgnify_pipelines_toolkit/analysis/amplicon/mapseq_to_asv_table.py
 mgnify_pipelines_toolkit/analysis/amplicon/remove_ambiguous_reads.py
 mgnify_pipelines_toolkit/analysis/amplicon/rev_comp_se_primers.py
 mgnify_pipelines_toolkit/analysis/amplicon/standard_primer_matching.py
 mgnify_pipelines_toolkit/analysis/shared/__init__.py
 mgnify_pipelines_toolkit/analysis/shared/get_subunits.py
 mgnify_pipelines_toolkit/analysis/shared/get_subunits_coords.py
 mgnify_pipelines_toolkit/analysis/shared/mapseq2biom.py
```

### Comparing `mgnify_pipelines_toolkit-0.1.1/mgnify_pipelines_toolkit.egg-info/entry_points.txt` & `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/entry_points.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,10 +4,11 @@
 assess_mcp_proportions = mgnify_pipelines_toolkit.analysis.amplicon.assess_mcp_proportions:main
 classify_var_regions = mgnify_pipelines_toolkit.analysis.amplicon.classify_var_regions:main
 find_mcp_inflection_points = mgnify_pipelines_toolkit.analysis.amplicon.find_mcp_inflection_points:main
 get_subunits = mgnify_pipelines_toolkit.analysis.shared.get_subunits:main
 get_subunits_coords = mgnify_pipelines_toolkit.analysis.shared.get_subunits_coords:main
 make_asv_count_table = mgnify_pipelines_toolkit.analysis.amplicon.make_asv_count_table:main
 mapseq2biom = mgnify_pipelines_toolkit.analysis.shared.mapseq2biom:main
+mapseq_to_asv_table = mgnify_pipelines_toolkit.analysis.amplicon.mapseq_to_asv_table:main
 remove_ambiguous_reads = mgnify_pipelines_toolkit.analysis.amplicon.remove_ambiguous_reads:main
 rev_comp_se_primers = mgnify_pipelines_toolkit.analysis.amplicon.rev_comp_se_primers:main
 standard_primer_matching = mgnify_pipelines_toolkit.analysis.amplicon.standard_primer_matching:main
```

### Comparing `mgnify_pipelines_toolkit-0.1.1/pyproject.toml` & `mgnify_pipelines_toolkit-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mgnify_pipelines_toolkit"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.md"
 license = {text = "Apache Software License 2.0"}
 authors = [
   { name = "MGnify team", email = "metagenomics-help@ebi.ac.uk" },
 ]
 keywords = ["bioinformatics", "pipelines", "metagenomics"]
 description = "Collection of scripts and tools for MGnify pipelines"
@@ -45,14 +45,15 @@
 assess_mcp_proportions = "mgnify_pipelines_toolkit.analysis.amplicon.assess_mcp_proportions:main"
 classify_var_regions = "mgnify_pipelines_toolkit.analysis.amplicon.classify_var_regions:main"
 find_mcp_inflection_points = "mgnify_pipelines_toolkit.analysis.amplicon.find_mcp_inflection_points:main"
 make_asv_count_table = "mgnify_pipelines_toolkit.analysis.amplicon.make_asv_count_table:main"
 remove_ambiguous_reads = "mgnify_pipelines_toolkit.analysis.amplicon.remove_ambiguous_reads:main"
 rev_comp_se_primers = "mgnify_pipelines_toolkit.analysis.amplicon.rev_comp_se_primers:main"
 standard_primer_matching = "mgnify_pipelines_toolkit.analysis.amplicon.standard_primer_matching:main"
+mapseq_to_asv_table = "mgnify_pipelines_toolkit.analysis.amplicon.mapseq_to_asv_table:main"
 
 [project.optional-dependencies]
 tests = [
     "pytest==7.4.0",
     "pytest-md==0.2.0",
     "pytest-workflow==2.0.1",
     "biopython==1.82",
```

