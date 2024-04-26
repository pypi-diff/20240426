# Comparing `tmp/repoqa-0.1.0rc1.tar.gz` & `tmp/repoqa-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repoqa-0.1.0rc1.tar", last modified: Wed Apr 24 00:46:35 2024, max compression
+gzip compressed data, was "repoqa-0.1.0rc2.tar", last modified: Wed Apr 24 19:42:48 2024, max compression
```

## Comparing `repoqa-0.1.0rc1.tar` & `repoqa-0.1.0rc2.tar`

### file list

```diff
@@ -1,82 +1,84 @@
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.969976 repoqa-0.1.0rc1/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     3194 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/.gitignore
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      913 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/.pre-commit-config.yaml
--rw-rw-r--   0 ganler    (1000) ganler    (1000)    11558 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/LICENSE
--rw-r--r--   0 ganler    (1000) ganler    (1000)     3743 2024-04-24 00:46:35.969976 repoqa-0.1.0rc1/PKG-INFO
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     3058 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/README.md
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.965976 repoqa-0.1.0rc1/docs/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2575 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/docs/curate_dataset.md
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      825 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/docs/dev_note.md
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      244 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/pyproject.toml
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.965976 repoqa-0.1.0rc1/repoqa/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      208 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/repoqa/__init__.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      414 2024-04-24 00:46:35.000000 repoqa-0.1.0rc1/repoqa/_version.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)    10634 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/repoqa/compute_score.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1659 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/repoqa/data.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      600 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/repoqa/metric.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.965976 repoqa-0.1.0rc1/repoqa/provider/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      274 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/repoqa/provider/__init__.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      330 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/repoqa/provider/base.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1470 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/repoqa/provider/hf.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1018 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/repoqa/provider/openai.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.965976 repoqa-0.1.0rc1/repoqa/provider/request/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      317 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/repoqa/provider/request/__init__.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1703 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/repoqa/provider/request/openai.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1376 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/repoqa/provider/vllm.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)    12703 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/repoqa/search_needle_function.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1918 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/repoqa/utility.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.969976 repoqa-0.1.0rc1/repoqa.egg-info/
--rw-r--r--   0 ganler    (1000) ganler    (1000)     3743 2024-04-24 00:46:35.000000 repoqa-0.1.0rc1/repoqa.egg-info/PKG-INFO
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1749 2024-04-24 00:46:35.000000 repoqa-0.1.0rc1/repoqa.egg-info/SOURCES.txt
--rw-rw-r--   0 ganler    (1000) ganler    (1000)        1 2024-04-24 00:46:35.000000 repoqa-0.1.0rc1/repoqa.egg-info/dependency_links.txt
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      134 2024-04-24 00:46:35.000000 repoqa-0.1.0rc1/repoqa.egg-info/entry_points.txt
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      123 2024-04-24 00:46:35.000000 repoqa-0.1.0rc1/repoqa.egg-info/requires.txt
--rw-rw-r--   0 ganler    (1000) ganler    (1000)        7 2024-04-24 00:46:35.000000 repoqa-0.1.0rc1/repoqa.egg-info/top_level.txt
--rw-rw-r--   0 ganler    (1000) ganler    (1000)       63 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/requirements.txt
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.965976 repoqa-0.1.0rc1/results/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)       13 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/results/.gitignore
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      675 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/results/README.md
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.965976 repoqa-0.1.0rc1/scripts/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.965976 repoqa-0.1.0rc1/scripts/cherrypick/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      720 2024-04-06 02:26:24.000000 repoqa-0.1.0rc1/scripts/cherrypick/README.md
--rw-rw-r--   0 ganler    (1000) ganler    (1000)    10742 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/scripts/cherrypick/lists.json
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.965976 repoqa-0.1.0rc1/scripts/curate/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1987 2024-04-16 20:28:57.000000 repoqa-0.1.0rc1/scripts/curate/dataset_ensemble_clone.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2480 2024-04-06 02:26:24.000000 repoqa-0.1.0rc1/scripts/curate/dataset_ensemble_gh_api.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.965976 repoqa-0.1.0rc1/scripts/curate/dep_analysis/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     4086 2024-04-19 09:21:06.000000 repoqa-0.1.0rc1/scripts/curate/dep_analysis/cpp.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.965976 repoqa-0.1.0rc1/scripts/curate/dep_analysis/data/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)        7 2024-04-16 20:28:57.000000 repoqa-0.1.0rc1/scripts/curate/dep_analysis/data/.gitignore
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.969976 repoqa-0.1.0rc1/scripts/curate/dep_analysis/java-analysis/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1652 2024-04-06 02:26:24.000000 repoqa-0.1.0rc1/scripts/curate/dep_analysis/java-analysis/dependency-reduced-pom.xml
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.969976 repoqa-0.1.0rc1/scripts/curate/dep_analysis/java-analysis/java-lib/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)  6013426 2024-04-06 02:26:24.000000 repoqa-0.1.0rc1/scripts/curate/dep_analysis/java-analysis/java-lib/java-analysis-1.0-SNAPSHOT.jar
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2984 2024-04-16 20:28:57.000000 repoqa-0.1.0rc1/scripts/curate/dep_analysis/java-analysis/pom.xml
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.965976 repoqa-0.1.0rc1/scripts/curate/dep_analysis/java-analysis/src/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.965976 repoqa-0.1.0rc1/scripts/curate/dep_analysis/java-analysis/src/main/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.965976 repoqa-0.1.0rc1/scripts/curate/dep_analysis/java-analysis/src/main/java/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.965976 repoqa-0.1.0rc1/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.965976 repoqa-0.1.0rc1/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.965976 repoqa-0.1.0rc1/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.969976 repoqa-0.1.0rc1/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     5415 2024-04-06 02:26:24.000000 repoqa-0.1.0rc1/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/DepAnalyze.java
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2199 2024-04-16 20:28:57.000000 repoqa-0.1.0rc1/scripts/curate/dep_analysis/java.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2610 2024-04-16 20:28:57.000000 repoqa-0.1.0rc1/scripts/curate/dep_analysis/python.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     5579 2024-04-16 20:28:57.000000 repoqa-0.1.0rc1/scripts/curate/dep_analysis/rust.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     4294 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/scripts/curate/dep_analysis/typescript.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     4163 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/scripts/curate/function_analysis.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     3980 2024-04-06 02:26:24.000000 repoqa-0.1.0rc1/scripts/curate/github_fetch.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1589 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/scripts/curate/merge_annotation.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1173 2024-04-16 20:28:57.000000 repoqa-0.1.0rc1/scripts/curate/merge_dep.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     4756 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/scripts/curate/needle_annotation.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     3223 2024-04-19 09:21:06.000000 repoqa-0.1.0rc1/scripts/curate/needle_selection.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      129 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/scripts/curate/requirements.txt
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      320 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/scripts/curate/utility.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.969976 repoqa-0.1.0rc1/scripts/demos/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      751 2024-04-06 02:26:24.000000 repoqa-0.1.0rc1/scripts/demos/model_request_oai.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.969976 repoqa-0.1.0rc1/scripts/dev/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)       84 2024-02-25 13:11:01.000000 repoqa-0.1.0rc1/scripts/dev/license-hdr.txt
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 00:46:35.969976 repoqa-0.1.0rc1/scripts/misc/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      877 2024-04-06 02:26:24.000000 repoqa-0.1.0rc1/scripts/misc/estimate_max_char.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2432 2024-04-24 00:46:21.000000 repoqa-0.1.0rc1/scripts/misc/repo_token_size.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      840 2024-04-24 00:46:35.973976 repoqa-0.1.0rc1/setup.cfg
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.248574 repoqa-0.1.0rc2/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     3194 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/.gitignore
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      913 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/.pre-commit-config.yaml
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)    11558 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/LICENSE
+-rw-r--r--   0 ganler    (1000) ganler    (1000)     4439 2024-04-24 19:42:48.248574 repoqa-0.1.0rc2/PKG-INFO
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     3683 2024-04-24 19:42:11.000000 repoqa-0.1.0rc2/README.md
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.244574 repoqa-0.1.0rc2/docs/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2575 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/docs/curate_dataset.md
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      825 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/docs/dev_note.md
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      244 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/pyproject.toml
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.244574 repoqa-0.1.0rc2/repoqa/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      208 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/__init__.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      414 2024-04-24 19:42:48.000000 repoqa-0.1.0rc2/repoqa/_version.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)    10634 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/compute_score.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1659 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/data.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      600 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/metric.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.244574 repoqa-0.1.0rc2/repoqa/provider/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      136 2024-04-24 19:42:11.000000 repoqa-0.1.0rc2/repoqa/provider/__init__.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1021 2024-04-24 19:42:11.000000 repoqa-0.1.0rc2/repoqa/provider/anthropic.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      330 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/provider/base.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1470 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/provider/hf.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1018 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/provider/openai.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.244574 repoqa-0.1.0rc2/repoqa/provider/request/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      317 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/provider/request/__init__.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2037 2024-04-24 19:42:11.000000 repoqa-0.1.0rc2/repoqa/provider/request/anthropic.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1703 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/provider/request/openai.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1376 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/provider/vllm.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)    12885 2024-04-24 19:42:11.000000 repoqa-0.1.0rc2/repoqa/search_needle_function.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1918 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/utility.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.248574 repoqa-0.1.0rc2/repoqa.egg-info/
+-rw-r--r--   0 ganler    (1000) ganler    (1000)     4439 2024-04-24 19:42:48.000000 repoqa-0.1.0rc2/repoqa.egg-info/PKG-INFO
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1815 2024-04-24 19:42:48.000000 repoqa-0.1.0rc2/repoqa.egg-info/SOURCES.txt
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)        1 2024-04-24 19:42:48.000000 repoqa-0.1.0rc2/repoqa.egg-info/dependency_links.txt
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      134 2024-04-24 19:42:48.000000 repoqa-0.1.0rc2/repoqa.egg-info/entry_points.txt
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      149 2024-04-24 19:42:48.000000 repoqa-0.1.0rc2/repoqa.egg-info/requires.txt
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)        7 2024-04-24 19:42:48.000000 repoqa-0.1.0rc2/repoqa.egg-info/top_level.txt
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)       73 2024-04-24 19:42:11.000000 repoqa-0.1.0rc2/requirements.txt
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.244574 repoqa-0.1.0rc2/results/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)       13 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/results/.gitignore
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      675 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/results/README.md
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.240574 repoqa-0.1.0rc2/scripts/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.244574 repoqa-0.1.0rc2/scripts/cherrypick/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      720 2024-04-06 02:26:24.000000 repoqa-0.1.0rc2/scripts/cherrypick/README.md
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)    10742 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/scripts/cherrypick/lists.json
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.244574 repoqa-0.1.0rc2/scripts/curate/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1987 2024-04-16 20:28:57.000000 repoqa-0.1.0rc2/scripts/curate/dataset_ensemble_clone.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2480 2024-04-06 02:26:24.000000 repoqa-0.1.0rc2/scripts/curate/dataset_ensemble_gh_api.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.244574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     4086 2024-04-19 09:21:06.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/cpp.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.244574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/data/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)        7 2024-04-16 20:28:57.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/data/.gitignore
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.248574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1652 2024-04-06 02:26:24.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/dependency-reduced-pom.xml
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.248574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/java-lib/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)  6013426 2024-04-06 02:26:24.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/java-lib/java-analysis-1.0-SNAPSHOT.jar
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2984 2024-04-16 20:28:57.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/pom.xml
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.240574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/src/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.240574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/src/main/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.240574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/src/main/java/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.240574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.240574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.240574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.248574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     5415 2024-04-06 02:26:24.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/DepAnalyze.java
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2199 2024-04-16 20:28:57.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2610 2024-04-16 20:28:57.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/python.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     5579 2024-04-16 20:28:57.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/rust.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     4294 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/typescript.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     4163 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/scripts/curate/function_analysis.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     3980 2024-04-06 02:26:24.000000 repoqa-0.1.0rc2/scripts/curate/github_fetch.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1589 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/scripts/curate/merge_annotation.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1173 2024-04-16 20:28:57.000000 repoqa-0.1.0rc2/scripts/curate/merge_dep.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     4756 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/scripts/curate/needle_annotation.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     3223 2024-04-19 09:21:06.000000 repoqa-0.1.0rc2/scripts/curate/needle_selection.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      129 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/scripts/curate/requirements.txt
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      320 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/scripts/curate/utility.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.248574 repoqa-0.1.0rc2/scripts/demos/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      751 2024-04-06 02:26:24.000000 repoqa-0.1.0rc2/scripts/demos/model_request_oai.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.248574 repoqa-0.1.0rc2/scripts/dev/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)       84 2024-02-25 13:11:01.000000 repoqa-0.1.0rc2/scripts/dev/license-hdr.txt
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.248574 repoqa-0.1.0rc2/scripts/misc/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      877 2024-04-06 02:26:24.000000 repoqa-0.1.0rc2/scripts/misc/estimate_max_char.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2432 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/scripts/misc/repo_token_size.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      891 2024-04-24 19:42:48.252574 repoqa-0.1.0rc2/setup.cfg
```

### Comparing `repoqa-0.1.0rc1/.gitignore` & `repoqa-0.1.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/.pre-commit-config.yaml` & `repoqa-0.1.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/LICENSE` & `repoqa-0.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/PKG-INFO` & `repoqa-0.1.0rc2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,30 @@
-Metadata-Version: 2.1
-Name: repoqa
-Version: 0.1.0rc1
-Summary: "RepoQA for Evaluating Long-Context Code Understanding"
-Home-page: https://github.com/evalplus/repoqa
-License: Apache-2.0
-Platform: any
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: appdirs>=1.4.4
-Requires-Dist: fire>=0.6.0
-Requires-Dist: openai>=1.23.2
-Requires-Dist: nltk>=3.8.1
-Requires-Dist: rich>=13.5.2
-Requires-Dist: vllm>=0.3.3
-Requires-Dist: tree_sitter_languages>=1.10.2
-Requires-Dist: numpy>=1.25.2
-
 # RepoQA: Evaluating Long-Context Code Understanding
 
 <p align="center">
     <a href="#-installation">🚀 Installation</a> •
     <a href="#-search-needle-function">🏁 Search Needle Function</a> •
     <a href="#-read-more">📚 Read More</a>
 </p>
 
 ## 🚀 Installation
 
 ```bash
-pip install repoqa
+# without vLLM (can run openai, anthropic, and huggingface backends)
+pip install --upgrade repoqa
+# with vLLM
+pip install --upgrade "repoqa[vllm]"
 ```
 
 <details><summary>⏬ Install nightly version <i>:: click to expand ::</i></summary>
 <div>
 
 ```bash
-pip install "git+https://github.com/evalplus/repoqa.git" --upgrade
+pip install --upgrade "git+https://github.com/evalplus/repoqa.git"                 # without vLLM
+pip install --upgrade "repoqa[vllm] @ git+https://github.com/evalplus/repoqa@main" # with vLLM
 ```
 
 </div>
 </details>
 
 <details><summary>⏬ Using RepoQA as a local repo? <i>:: click to expand ::</i></summary>
 <div>
@@ -53,68 +35,76 @@
 export PYTHONPATH=$PYTHONPATH:$(pwd)
 pip install -r requirements.txt
 ```
 
 </div>
 </details>
 
-
 ## 🏁 Search Needle Function
 
-### Inference with vLLM
+### Inference with OpenAI Compatible Servers
 
 ```bash
-repoqa.search_needle_function --model "Qwen/CodeQwen1.5-7B-Chat" --caching --backend vllm
+repoqa.search_needle_function --model "gpt4-turbo" --caching --backend openai
+# 💡 If you use customized server such vLLM:
+# repoqa.search_needle_function --base-url "http://url.to.vllm.server/v1" \
+#                               --model "gpt4-turbo" --caching --backend openai
 ```
 
-### Inference with OpenAI Compatible Servers
+### Inference with Anthropic Compatible Servers
 
 ```bash
-repoqa.search_needle_function --base-url "http://api.openai.com/v1" \
-                              --model "gpt4-turbo" --caching --backend openai
+repoqa.search_needle_function --model "claude-3-haiku-20240307" --caching --backend anthropic
+```
+
+### Inference with vLLM
+
+```bash
+repoqa.search_needle_function --model "Qwen/CodeQwen1.5-7B-Chat" \
+                              --caching --backend vllm
 ```
 
 ### Inference with HuggingFace transformers
 
 ```bash
-repoqa.search_needle_function --model "gpt2" "Qwen/CodeQwen1.5-7B-Chat" --caching --backend hf
+repoqa.search_needle_function --model "gpt2" "Qwen/CodeQwen1.5-7B-Chat" \
+                              --caching --backend hf --trust-remote-code
 ```
 
 ### Usage
 
 > [!Tip]
 >
-> * **Input**:
->   * `--model`: Hugging-Face model ID, such as `ise-uiuc/Magicoder-S-DS-6.7B`
->   * `--backend`: `vllm` (default) or `openai`
->   * `--base-url`: OpenAI API base URL
->   * `--code-context-size` (default: 16384): Number of tokens (using DeepSeekCoder tokenizer) of code in the long context
->   * `--caching` (default: False): if enabled, the tokenization and chuncking results will be cached to accelerate subsequent runs
->   * `--max-new-tokens` (default: 1024): Maximum number of new tokens to generate
->   * `--system-message` (default: None): if given, the model use a system message (but note some models don't support system message)
->   * `--tensor-parallel-size`: Number of tensor parallelism (only for vLLM)
->   * `--languages` (default: None): List of languages to evaluate (None means all)
->   * `--result-dir` (default: "results"): Directory to save the model outputs and evaluation results
-> * **Output**:
->   * `results/ntoken_{code-context-size}/{model}.jsonl`: Model generated outputs
->   * `results/ntoken_{code-context-size}/{model}-SCORE.json`: Evaluation scores (also see [Compute Scores](#compute-scores))
+> - **Input**:
+>   - `--model`: Hugging-Face model ID, such as `ise-uiuc/Magicoder-S-DS-6.7B`
+>   - `--backend`: `vllm` (default) or `openai`
+>   - `--base-url`: OpenAI API base URL
+>   - `--code-context-size` (default: 16384): Number of tokens (using DeepSeekCoder tokenizer) of code in the long context
+>   - `--caching` (default: False): if enabled, the tokenization and chuncking results will be cached to accelerate subsequent runs
+>   - `--max-new-tokens` (default: 1024): Maximum number of new tokens to generate
+>   - `--system-message` (default: None): if given, the model use a system message (but note some models don't support system message)
+>   - `--tensor-parallel-size`: Number of tensor parallelism (only for vLLM)
+>   - `--languages` (default: None): List of languages to evaluate (None means all)
+>   - `--result-dir` (default: "results"): Directory to save the model outputs and evaluation results
+> - **Output**:
+>   - `results/ntoken_{code-context-size}/{model}.jsonl`: Model generated outputs
+>   - `results/ntoken_{code-context-size}/{model}-SCORE.json`: Evaluation scores (also see [Compute Scores](#compute-scores))
 
 ### Compute Scores
 
 By default, the `repoqa.search_needle_function` command will also compute scores after producing model outputs.
 However, you can also compute scores separately using the following command:
 
 ```shell
 repoqa.compute_score --model-output-path={model-output}.jsonl
 ```
 
 > [!Tip]
 >
-> * **Input**: Path to the model generated outputs.
-> * **Output**: The evaluation scores would be stored in `{model-output}-SCORES.json`
-
+> - **Input**: Path to the model generated outputs.
+> - **Output**: The evaluation scores would be stored in `{model-output}-SCORES.json`
 
 ## 📚 Read More
 
-* [RepoQA Homepage](https://evalplus.github.io/repoqa.html)
-* [RepoQA Dataset Curation](docs/curate_dataset.md)
-* [RepoQA Development Notes](docs/dev_note.md)
+- [RepoQA Homepage](https://evalplus.github.io/repoqa.html)
+- [RepoQA Dataset Curation](docs/curate_dataset.md)
+- [RepoQA Development Notes](docs/dev_note.md)
```

#### html2text {}

```diff
@@ -1,47 +1,45 @@
-Metadata-Version: 2.1 Name: repoqa Version: 0.1.0rc1 Summary: "RepoQA for
-Evaluating Long-Context Code Understanding" Home-page: https://github.com/
-evalplus/repoqa License: Apache-2.0 Platform: any Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: Apache Software License Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-appdirs>=1.4.4 Requires-Dist: fire>=0.6.0 Requires-Dist: openai>=1.23.2
-Requires-Dist: nltk>=3.8.1 Requires-Dist: rich>=13.5.2 Requires-Dist:
-vllm>=0.3.3 Requires-Dist: tree_sitter_languages>=1.10.2 Requires-Dist:
-numpy>=1.25.2 # RepoQA: Evaluating Long-Context Code Understanding
+# RepoQA: Evaluating Long-Context Code Understanding
      _ð____ _I_n_s_t_a_l_l_a_t_i_o_n â¢ _ð____ _S_e_a_r_c_h_ _N_e_e_d_l_e_ _F_u_n_c_t_i_o_n â¢ _ð____ _R_e_a_d_ _M_o_r_e
-## ð Installation ```bash pip install repoqa ``` â¬ Install nightly version
-:: click to expand ::
-```bash pip install "git+https://github.com/evalplus/repoqa.git" --upgrade ```
+## ð Installation ```bash # without vLLM (can run openai, anthropic, and
+huggingface backends) pip install --upgrade repoqa # with vLLM pip install --
+upgrade "repoqa[vllm]" ``` â¬ Install nightly version :: click to expand ::
+```bash pip install --upgrade "git+https://github.com/evalplus/repoqa.git" #
+without vLLM pip install --upgrade "repoqa[vllm] @ git+https://github.com/
+evalplus/repoqa@main" # with vLLM ```
 â¬ Using RepoQA as a local repo? :: click to expand ::
 ```bash git clone https://github.com/evalplus/repoqa.git cd repoqa export
 PYTHONPATH=$PYTHONPATH:$(pwd) pip install -r requirements.txt ```
-## ð Search Needle Function ### Inference with vLLM ```bash
-repoqa.search_needle_function --model "Qwen/CodeQwen1.5-7B-Chat" --caching --
-backend vllm ``` ### Inference with OpenAI Compatible Servers ```bash
-repoqa.search_needle_function --base-url "http://api.openai.com/v1" \ --model
-"gpt4-turbo" --caching --backend openai ``` ### Inference with HuggingFace
-transformers ```bash repoqa.search_needle_function --model "gpt2" "Qwen/
-CodeQwen1.5-7B-Chat" --caching --backend hf ``` ### Usage > [!Tip] > > *
-**Input**: > * `--model`: Hugging-Face model ID, such as `ise-uiuc/Magicoder-S-
-DS-6.7B` > * `--backend`: `vllm` (default) or `openai` > * `--base-url`: OpenAI
-API base URL > * `--code-context-size` (default: 16384): Number of tokens
-(using DeepSeekCoder tokenizer) of code in the long context > * `--caching`
+## ð Search Needle Function ### Inference with OpenAI Compatible Servers
+```bash repoqa.search_needle_function --model "gpt4-turbo" --caching --backend
+openai # ð¡ If you use customized server such vLLM: #
+repoqa.search_needle_function --base-url "http://url.to.vllm.server/v1" \ # --
+model "gpt4-turbo" --caching --backend openai ``` ### Inference with Anthropic
+Compatible Servers ```bash repoqa.search_needle_function --model "claude-3-
+haiku-20240307" --caching --backend anthropic ``` ### Inference with vLLM
+```bash repoqa.search_needle_function --model "Qwen/CodeQwen1.5-7B-Chat" \ --
+caching --backend vllm ``` ### Inference with HuggingFace transformers ```bash
+repoqa.search_needle_function --model "gpt2" "Qwen/CodeQwen1.5-7B-Chat" \ --
+caching --backend hf --trust-remote-code ``` ### Usage > [!Tip] > > -
+**Input**: > - `--model`: Hugging-Face model ID, such as `ise-uiuc/Magicoder-S-
+DS-6.7B` > - `--backend`: `vllm` (default) or `openai` > - `--base-url`: OpenAI
+API base URL > - `--code-context-size` (default: 16384): Number of tokens
+(using DeepSeekCoder tokenizer) of code in the long context > - `--caching`
 (default: False): if enabled, the tokenization and chuncking results will be
-cached to accelerate subsequent runs > * `--max-new-tokens` (default: 1024):
-Maximum number of new tokens to generate > * `--system-message` (default:
+cached to accelerate subsequent runs > - `--max-new-tokens` (default: 1024):
+Maximum number of new tokens to generate > - `--system-message` (default:
 None): if given, the model use a system message (but note some models don't
-support system message) > * `--tensor-parallel-size`: Number of tensor
-parallelism (only for vLLM) > * `--languages` (default: None): List of
-languages to evaluate (None means all) > * `--result-dir` (default: "results"):
-Directory to save the model outputs and evaluation results > * **Output**: > *
-`results/ntoken_{code-context-size}/{model}.jsonl`: Model generated outputs > *
+support system message) > - `--tensor-parallel-size`: Number of tensor
+parallelism (only for vLLM) > - `--languages` (default: None): List of
+languages to evaluate (None means all) > - `--result-dir` (default: "results"):
+Directory to save the model outputs and evaluation results > - **Output**: > -
+`results/ntoken_{code-context-size}/{model}.jsonl`: Model generated outputs > -
 `results/ntoken_{code-context-size}/{model}-SCORE.json`: Evaluation scores
 (also see [Compute Scores](#compute-scores)) ### Compute Scores By default, the
 `repoqa.search_needle_function` command will also compute scores after
 producing model outputs. However, you can also compute scores separately using
 the following command: ```shell repoqa.compute_score --model-output-path=
-{model-output}.jsonl ``` > [!Tip] > > * **Input**: Path to the model generated
-outputs. > * **Output**: The evaluation scores would be stored in `{model-
-output}-SCORES.json` ## ð Read More * [RepoQA Homepage](https://
-evalplus.github.io/repoqa.html) * [RepoQA Dataset Curation](docs/
-curate_dataset.md) * [RepoQA Development Notes](docs/dev_note.md)
+{model-output}.jsonl ``` > [!Tip] > > - **Input**: Path to the model generated
+outputs. > - **Output**: The evaluation scores would be stored in `{model-
+output}-SCORES.json` ## ð Read More - [RepoQA Homepage](https://
+evalplus.github.io/repoqa.html) - [RepoQA Dataset Curation](docs/
+curate_dataset.md) - [RepoQA Development Notes](docs/dev_note.md)
```

### Comparing `repoqa-0.1.0rc1/docs/curate_dataset.md` & `repoqa-0.1.0rc2/docs/curate_dataset.md`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/docs/dev_note.md` & `repoqa-0.1.0rc2/docs/dev_note.md`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/repoqa/compute_score.py` & `repoqa-0.1.0rc2/repoqa/compute_score.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/repoqa/data.py` & `repoqa-0.1.0rc2/repoqa/data.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/repoqa/metric.py` & `repoqa-0.1.0rc2/repoqa/metric.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/repoqa/provider/hf.py` & `repoqa-0.1.0rc2/repoqa/provider/hf.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/repoqa/provider/openai.py` & `repoqa-0.1.0rc2/repoqa/provider/openai.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/repoqa/provider/request/openai.py` & `repoqa-0.1.0rc2/repoqa/provider/request/openai.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/repoqa/provider/vllm.py` & `repoqa-0.1.0rc2/repoqa/provider/vllm.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/repoqa/search_needle_function.py` & `repoqa-0.1.0rc2/repoqa/search_needle_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 }
 
 
 # Model context below:
 TEMPLATE = "instruction\ncode_context\ndescription\ninstruction"
 
 INSTRUCTION = (
-    "Based on the function discription and code context,"
-    " please reproduce the described function from the code context in a markdown block:"
+    "Based on the function description and code context,"
+    " please retrieve and repeat the exact described function from the code context in a code block wrapped by ```:"
 )
 
 
 def _backward_tokenizable_lines(lines, tokenizer, max_tokens):
     """Return the text and tokens from bottom to top"""
     text = ""
     ntokens = 0
@@ -298,28 +298,32 @@
     ]
 
     if len(tasks) == 0:
         print("No tasks to evaluate! Exiting...")
         return
 
     if backend == "openai":
-        from repoqa.provider import OpenAIProvider
+        from repoqa.provider.openai import OpenAIProvider
 
         engine = OpenAIProvider(model, base_url=base_url)
     elif backend == "vllm":
-        from repoqa.provider import VllmProvider
+        from repoqa.provider.vllm import VllmProvider
 
         engine = VllmProvider(
             model,
             tensor_parallel_size=tensor_parallel_size,
             max_model_len=int(code_context_size * 1.25),  # Magic number
             trust_remote_code=trust_remote_code,
         )
+    elif backend == "anthropic":
+        from repoqa.provider.anthropic import AnthropicProvider
+
+        engine = AnthropicProvider(model)
     elif backend == "hf":
-        from repoqa.provider import HfProvider
+        from repoqa.provider.hf import HfProvider
 
         engine = HfProvider(model, trust_remote_code=trust_remote_code)
 
     if not system_message:
         print("🔥 System message is disabled")
         system_message = None
```

### Comparing `repoqa-0.1.0rc1/repoqa/utility.py` & `repoqa-0.1.0rc2/repoqa/utility.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/repoqa.egg-info/PKG-INFO` & `repoqa-0.1.0rc2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repoqa
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: "RepoQA for Evaluating Long-Context Code Understanding"
 Home-page: https://github.com/evalplus/repoqa
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,37 +12,43 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: fire>=0.6.0
 Requires-Dist: openai>=1.23.2
 Requires-Dist: nltk>=3.8.1
 Requires-Dist: rich>=13.5.2
-Requires-Dist: vllm>=0.3.3
 Requires-Dist: tree_sitter_languages>=1.10.2
 Requires-Dist: numpy>=1.25.2
+Requires-Dist: anthropic>=0.25.6
+Provides-Extra: vllm
+Requires-Dist: vllm>=0.3.3; extra == "vllm"
 
 # RepoQA: Evaluating Long-Context Code Understanding
 
 <p align="center">
     <a href="#-installation">🚀 Installation</a> •
     <a href="#-search-needle-function">🏁 Search Needle Function</a> •
     <a href="#-read-more">📚 Read More</a>
 </p>
 
 ## 🚀 Installation
 
 ```bash
-pip install repoqa
+# without vLLM (can run openai, anthropic, and huggingface backends)
+pip install --upgrade repoqa
+# with vLLM
+pip install --upgrade "repoqa[vllm]"
 ```
 
 <details><summary>⏬ Install nightly version <i>:: click to expand ::</i></summary>
 <div>
 
 ```bash
-pip install "git+https://github.com/evalplus/repoqa.git" --upgrade
+pip install --upgrade "git+https://github.com/evalplus/repoqa.git"                 # without vLLM
+pip install --upgrade "repoqa[vllm] @ git+https://github.com/evalplus/repoqa@main" # with vLLM
 ```
 
 </div>
 </details>
 
 <details><summary>⏬ Using RepoQA as a local repo? <i>:: click to expand ::</i></summary>
 <div>
@@ -53,68 +59,76 @@
 export PYTHONPATH=$PYTHONPATH:$(pwd)
 pip install -r requirements.txt
 ```
 
 </div>
 </details>
 
-
 ## 🏁 Search Needle Function
 
-### Inference with vLLM
+### Inference with OpenAI Compatible Servers
 
 ```bash
-repoqa.search_needle_function --model "Qwen/CodeQwen1.5-7B-Chat" --caching --backend vllm
+repoqa.search_needle_function --model "gpt4-turbo" --caching --backend openai
+# 💡 If you use customized server such vLLM:
+# repoqa.search_needle_function --base-url "http://url.to.vllm.server/v1" \
+#                               --model "gpt4-turbo" --caching --backend openai
 ```
 
-### Inference with OpenAI Compatible Servers
+### Inference with Anthropic Compatible Servers
+
+```bash
+repoqa.search_needle_function --model "claude-3-haiku-20240307" --caching --backend anthropic
+```
+
+### Inference with vLLM
 
 ```bash
-repoqa.search_needle_function --base-url "http://api.openai.com/v1" \
-                              --model "gpt4-turbo" --caching --backend openai
+repoqa.search_needle_function --model "Qwen/CodeQwen1.5-7B-Chat" \
+                              --caching --backend vllm
 ```
 
 ### Inference with HuggingFace transformers
 
 ```bash
-repoqa.search_needle_function --model "gpt2" "Qwen/CodeQwen1.5-7B-Chat" --caching --backend hf
+repoqa.search_needle_function --model "gpt2" "Qwen/CodeQwen1.5-7B-Chat" \
+                              --caching --backend hf --trust-remote-code
 ```
 
 ### Usage
 
 > [!Tip]
 >
-> * **Input**:
->   * `--model`: Hugging-Face model ID, such as `ise-uiuc/Magicoder-S-DS-6.7B`
->   * `--backend`: `vllm` (default) or `openai`
->   * `--base-url`: OpenAI API base URL
->   * `--code-context-size` (default: 16384): Number of tokens (using DeepSeekCoder tokenizer) of code in the long context
->   * `--caching` (default: False): if enabled, the tokenization and chuncking results will be cached to accelerate subsequent runs
->   * `--max-new-tokens` (default: 1024): Maximum number of new tokens to generate
->   * `--system-message` (default: None): if given, the model use a system message (but note some models don't support system message)
->   * `--tensor-parallel-size`: Number of tensor parallelism (only for vLLM)
->   * `--languages` (default: None): List of languages to evaluate (None means all)
->   * `--result-dir` (default: "results"): Directory to save the model outputs and evaluation results
-> * **Output**:
->   * `results/ntoken_{code-context-size}/{model}.jsonl`: Model generated outputs
->   * `results/ntoken_{code-context-size}/{model}-SCORE.json`: Evaluation scores (also see [Compute Scores](#compute-scores))
+> - **Input**:
+>   - `--model`: Hugging-Face model ID, such as `ise-uiuc/Magicoder-S-DS-6.7B`
+>   - `--backend`: `vllm` (default) or `openai`
+>   - `--base-url`: OpenAI API base URL
+>   - `--code-context-size` (default: 16384): Number of tokens (using DeepSeekCoder tokenizer) of code in the long context
+>   - `--caching` (default: False): if enabled, the tokenization and chuncking results will be cached to accelerate subsequent runs
+>   - `--max-new-tokens` (default: 1024): Maximum number of new tokens to generate
+>   - `--system-message` (default: None): if given, the model use a system message (but note some models don't support system message)
+>   - `--tensor-parallel-size`: Number of tensor parallelism (only for vLLM)
+>   - `--languages` (default: None): List of languages to evaluate (None means all)
+>   - `--result-dir` (default: "results"): Directory to save the model outputs and evaluation results
+> - **Output**:
+>   - `results/ntoken_{code-context-size}/{model}.jsonl`: Model generated outputs
+>   - `results/ntoken_{code-context-size}/{model}-SCORE.json`: Evaluation scores (also see [Compute Scores](#compute-scores))
 
 ### Compute Scores
 
 By default, the `repoqa.search_needle_function` command will also compute scores after producing model outputs.
 However, you can also compute scores separately using the following command:
 
 ```shell
 repoqa.compute_score --model-output-path={model-output}.jsonl
 ```
 
 > [!Tip]
 >
-> * **Input**: Path to the model generated outputs.
-> * **Output**: The evaluation scores would be stored in `{model-output}-SCORES.json`
-
+> - **Input**: Path to the model generated outputs.
+> - **Output**: The evaluation scores would be stored in `{model-output}-SCORES.json`
 
 ## 📚 Read More
 
-* [RepoQA Homepage](https://evalplus.github.io/repoqa.html)
-* [RepoQA Dataset Curation](docs/curate_dataset.md)
-* [RepoQA Development Notes](docs/dev_note.md)
+- [RepoQA Homepage](https://evalplus.github.io/repoqa.html)
+- [RepoQA Dataset Curation](docs/curate_dataset.md)
+- [RepoQA Development Notes](docs/dev_note.md)
```

#### html2text {}

```diff
@@ -1,47 +1,55 @@
-Metadata-Version: 2.1 Name: repoqa Version: 0.1.0rc1 Summary: "RepoQA for
+Metadata-Version: 2.1 Name: repoqa Version: 0.1.0rc2 Summary: "RepoQA for
 Evaluating Long-Context Code Understanding" Home-page: https://github.com/
 evalplus/repoqa License: Apache-2.0 Platform: any Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: Apache Software License Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 appdirs>=1.4.4 Requires-Dist: fire>=0.6.0 Requires-Dist: openai>=1.23.2
 Requires-Dist: nltk>=3.8.1 Requires-Dist: rich>=13.5.2 Requires-Dist:
-vllm>=0.3.3 Requires-Dist: tree_sitter_languages>=1.10.2 Requires-Dist:
-numpy>=1.25.2 # RepoQA: Evaluating Long-Context Code Understanding
+tree_sitter_languages>=1.10.2 Requires-Dist: numpy>=1.25.2 Requires-Dist:
+anthropic>=0.25.6 Provides-Extra: vllm Requires-Dist: vllm>=0.3.3; extra ==
+"vllm" # RepoQA: Evaluating Long-Context Code Understanding
      _ð____ _I_n_s_t_a_l_l_a_t_i_o_n â¢ _ð____ _S_e_a_r_c_h_ _N_e_e_d_l_e_ _F_u_n_c_t_i_o_n â¢ _ð____ _R_e_a_d_ _M_o_r_e
-## ð Installation ```bash pip install repoqa ``` â¬ Install nightly version
-:: click to expand ::
-```bash pip install "git+https://github.com/evalplus/repoqa.git" --upgrade ```
+## ð Installation ```bash # without vLLM (can run openai, anthropic, and
+huggingface backends) pip install --upgrade repoqa # with vLLM pip install --
+upgrade "repoqa[vllm]" ``` â¬ Install nightly version :: click to expand ::
+```bash pip install --upgrade "git+https://github.com/evalplus/repoqa.git" #
+without vLLM pip install --upgrade "repoqa[vllm] @ git+https://github.com/
+evalplus/repoqa@main" # with vLLM ```
 â¬ Using RepoQA as a local repo? :: click to expand ::
 ```bash git clone https://github.com/evalplus/repoqa.git cd repoqa export
 PYTHONPATH=$PYTHONPATH:$(pwd) pip install -r requirements.txt ```
-## ð Search Needle Function ### Inference with vLLM ```bash
-repoqa.search_needle_function --model "Qwen/CodeQwen1.5-7B-Chat" --caching --
-backend vllm ``` ### Inference with OpenAI Compatible Servers ```bash
-repoqa.search_needle_function --base-url "http://api.openai.com/v1" \ --model
-"gpt4-turbo" --caching --backend openai ``` ### Inference with HuggingFace
-transformers ```bash repoqa.search_needle_function --model "gpt2" "Qwen/
-CodeQwen1.5-7B-Chat" --caching --backend hf ``` ### Usage > [!Tip] > > *
-**Input**: > * `--model`: Hugging-Face model ID, such as `ise-uiuc/Magicoder-S-
-DS-6.7B` > * `--backend`: `vllm` (default) or `openai` > * `--base-url`: OpenAI
-API base URL > * `--code-context-size` (default: 16384): Number of tokens
-(using DeepSeekCoder tokenizer) of code in the long context > * `--caching`
+## ð Search Needle Function ### Inference with OpenAI Compatible Servers
+```bash repoqa.search_needle_function --model "gpt4-turbo" --caching --backend
+openai # ð¡ If you use customized server such vLLM: #
+repoqa.search_needle_function --base-url "http://url.to.vllm.server/v1" \ # --
+model "gpt4-turbo" --caching --backend openai ``` ### Inference with Anthropic
+Compatible Servers ```bash repoqa.search_needle_function --model "claude-3-
+haiku-20240307" --caching --backend anthropic ``` ### Inference with vLLM
+```bash repoqa.search_needle_function --model "Qwen/CodeQwen1.5-7B-Chat" \ --
+caching --backend vllm ``` ### Inference with HuggingFace transformers ```bash
+repoqa.search_needle_function --model "gpt2" "Qwen/CodeQwen1.5-7B-Chat" \ --
+caching --backend hf --trust-remote-code ``` ### Usage > [!Tip] > > -
+**Input**: > - `--model`: Hugging-Face model ID, such as `ise-uiuc/Magicoder-S-
+DS-6.7B` > - `--backend`: `vllm` (default) or `openai` > - `--base-url`: OpenAI
+API base URL > - `--code-context-size` (default: 16384): Number of tokens
+(using DeepSeekCoder tokenizer) of code in the long context > - `--caching`
 (default: False): if enabled, the tokenization and chuncking results will be
-cached to accelerate subsequent runs > * `--max-new-tokens` (default: 1024):
-Maximum number of new tokens to generate > * `--system-message` (default:
+cached to accelerate subsequent runs > - `--max-new-tokens` (default: 1024):
+Maximum number of new tokens to generate > - `--system-message` (default:
 None): if given, the model use a system message (but note some models don't
-support system message) > * `--tensor-parallel-size`: Number of tensor
-parallelism (only for vLLM) > * `--languages` (default: None): List of
-languages to evaluate (None means all) > * `--result-dir` (default: "results"):
-Directory to save the model outputs and evaluation results > * **Output**: > *
-`results/ntoken_{code-context-size}/{model}.jsonl`: Model generated outputs > *
+support system message) > - `--tensor-parallel-size`: Number of tensor
+parallelism (only for vLLM) > - `--languages` (default: None): List of
+languages to evaluate (None means all) > - `--result-dir` (default: "results"):
+Directory to save the model outputs and evaluation results > - **Output**: > -
+`results/ntoken_{code-context-size}/{model}.jsonl`: Model generated outputs > -
 `results/ntoken_{code-context-size}/{model}-SCORE.json`: Evaluation scores
 (also see [Compute Scores](#compute-scores)) ### Compute Scores By default, the
 `repoqa.search_needle_function` command will also compute scores after
 producing model outputs. However, you can also compute scores separately using
 the following command: ```shell repoqa.compute_score --model-output-path=
-{model-output}.jsonl ``` > [!Tip] > > * **Input**: Path to the model generated
-outputs. > * **Output**: The evaluation scores would be stored in `{model-
-output}-SCORES.json` ## ð Read More * [RepoQA Homepage](https://
-evalplus.github.io/repoqa.html) * [RepoQA Dataset Curation](docs/
-curate_dataset.md) * [RepoQA Development Notes](docs/dev_note.md)
+{model-output}.jsonl ``` > [!Tip] > > - **Input**: Path to the model generated
+outputs. > - **Output**: The evaluation scores would be stored in `{model-
+output}-SCORES.json` ## ð Read More - [RepoQA Homepage](https://
+evalplus.github.io/repoqa.html) - [RepoQA Dataset Curation](docs/
+curate_dataset.md) - [RepoQA Development Notes](docs/dev_note.md)
```

### Comparing `repoqa-0.1.0rc1/repoqa.egg-info/SOURCES.txt` & `repoqa-0.1.0rc2/repoqa.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,21 @@
 repoqa.egg-info/PKG-INFO
 repoqa.egg-info/SOURCES.txt
 repoqa.egg-info/dependency_links.txt
 repoqa.egg-info/entry_points.txt
 repoqa.egg-info/requires.txt
 repoqa.egg-info/top_level.txt
 repoqa/provider/__init__.py
+repoqa/provider/anthropic.py
 repoqa/provider/base.py
 repoqa/provider/hf.py
 repoqa/provider/openai.py
 repoqa/provider/vllm.py
 repoqa/provider/request/__init__.py
+repoqa/provider/request/anthropic.py
 repoqa/provider/request/openai.py
 results/.gitignore
 results/README.md
 scripts/cherrypick/README.md
 scripts/cherrypick/lists.json
 scripts/curate/dataset_ensemble_clone.py
 scripts/curate/dataset_ensemble_gh_api.py
```

### Comparing `repoqa-0.1.0rc1/results/README.md` & `repoqa-0.1.0rc2/results/README.md`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/cherrypick/README.md` & `repoqa-0.1.0rc2/scripts/cherrypick/README.md`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/cherrypick/lists.json` & `repoqa-0.1.0rc2/scripts/cherrypick/lists.json`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/curate/dataset_ensemble_clone.py` & `repoqa-0.1.0rc2/scripts/curate/dataset_ensemble_clone.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/curate/dataset_ensemble_gh_api.py` & `repoqa-0.1.0rc2/scripts/curate/dataset_ensemble_gh_api.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/curate/dep_analysis/cpp.py` & `repoqa-0.1.0rc2/scripts/curate/dep_analysis/cpp.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/curate/dep_analysis/java-analysis/dependency-reduced-pom.xml` & `repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/dependency-reduced-pom.xml`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/curate/dep_analysis/java-analysis/java-lib/java-analysis-1.0-SNAPSHOT.jar` & `repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/java-lib/java-analysis-1.0-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/curate/dep_analysis/java-analysis/pom.xml` & `repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/pom.xml`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/DepAnalyze.java` & `repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/DepAnalyze.java`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/curate/dep_analysis/java.py` & `repoqa-0.1.0rc2/scripts/curate/dep_analysis/java.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/curate/dep_analysis/python.py` & `repoqa-0.1.0rc2/scripts/curate/dep_analysis/python.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/curate/dep_analysis/rust.py` & `repoqa-0.1.0rc2/scripts/curate/dep_analysis/rust.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/curate/dep_analysis/typescript.py` & `repoqa-0.1.0rc2/scripts/curate/dep_analysis/typescript.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/curate/function_analysis.py` & `repoqa-0.1.0rc2/scripts/curate/function_analysis.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/curate/github_fetch.py` & `repoqa-0.1.0rc2/scripts/curate/github_fetch.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/curate/merge_annotation.py` & `repoqa-0.1.0rc2/scripts/curate/merge_annotation.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/curate/merge_dep.py` & `repoqa-0.1.0rc2/scripts/curate/merge_dep.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/curate/needle_annotation.py` & `repoqa-0.1.0rc2/scripts/curate/needle_annotation.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/curate/needle_selection.py` & `repoqa-0.1.0rc2/scripts/curate/needle_selection.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/demos/model_request_oai.py` & `repoqa-0.1.0rc2/scripts/demos/model_request_oai.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/misc/estimate_max_char.py` & `repoqa-0.1.0rc2/scripts/misc/estimate_max_char.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/scripts/misc/repo_token_size.py` & `repoqa-0.1.0rc2/scripts/misc/repo_token_size.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc1/setup.cfg` & `repoqa-0.1.0rc2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -18,20 +18,23 @@
 dependency_links = 
 install_requires = 
 	appdirs>=1.4.4
 	fire>=0.6.0
 	openai>=1.23.2
 	nltk>=3.8.1
 	rich>=13.5.2
-	vllm>=0.3.3
 	tree_sitter_languages>=1.10.2
 	numpy>=1.25.2
+	anthropic>=0.25.6
 
 [options.entry_points]
 console_scripts = 
 	repoqa.search_needle_function = repoqa.search_needle_function:main
 	repoqa.compute_score = repoqa.compute_score:main
 
+[options.extras_require]
+vllm = vllm>=0.3.3
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

