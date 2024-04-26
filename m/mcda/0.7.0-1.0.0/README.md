# Comparing `tmp/mcda-0.7.0.tar.gz` & `tmp/mcda-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcda-0.7.0.tar", last modified: Mon Apr  8 16:22:12 2024, max compression
+gzip compressed data, was "mcda-1.0.0.tar", last modified: Fri Apr 26 16:07:41 2024, max compression
```

## Comparing `mcda-0.7.0.tar` & `mcda-1.0.0.tar`

### file list

```diff
@@ -1,67 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.167923 mcda-0.7.0/
--rw-rw-rw-   0 root         (0) root         (0)      568 2024-04-08 16:22:01.000000 mcda-0.7.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       45 2024-04-08 16:22:01.000000 mcda-0.7.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4365 2024-04-08 16:22:12.167923 mcda-0.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2402 2024-04-08 16:22:01.000000 mcda-0.7.0/README.PYPI.md
--rw-rw-rw-   0 root         (0) root         (0)     2786 2024-04-08 16:22:01.000000 mcda-0.7.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1390 2024-04-08 16:22:01.000000 mcda-0.7.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 16:22:12.167923 mcda-0.7.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.154923 mcda-0.7.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.158923 mcda-0.7.0/src/mcda/
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/categories.py
--rw-rw-rw-   0 root         (0) root         (0)      713 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.159923 mcda-0.7.0/src/mcda/internal/
--rw-rw-rw-   0 root         (0) root         (0)      218 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.162923 mcda-0.7.0/src/mcda/internal/core/
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24045 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/aggregators.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/aliases.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/categories.py
--rw-rw-rw-   0 root         (0) root         (0)    13489 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/criteria_functions.py
--rw-rw-rw-   0 root         (0) root         (0)    15171 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/functions.py
--rw-rw-rw-   0 root         (0) root         (0)     1801 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)    46938 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/matrices.py
--rw-rw-rw-   0 root         (0) root         (0)    21757 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/relations.py
--rw-rw-rw-   0 root         (0) root         (0)    23860 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/scales.py
--rw-rw-rw-   0 root         (0) root         (0)    19032 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/set_functions.py
--rw-rw-rw-   0 root         (0) root         (0)    21526 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/transformers.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    15038 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.163923 mcda-0.7.0/src/mcda/internal/dea/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/dea/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.163923 mcda-0.7.0/src/mcda/internal/mavt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/mavt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26220 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/mavt/uta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.164923 mcda-0.7.0/src/mcda/internal/outranking/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/outranking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    39391 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/outranking/electre.py
--rw-rw-rw-   0 root         (0) root         (0)    32686 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/outranking/promethee.py
--rw-rw-rw-   0 root         (0) root         (0)    38234 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/outranking/srmp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.164923 mcda-0.7.0/src/mcda/internal/plot/
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    44068 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/plot/plot.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/matrices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.165923 mcda-0.7.0/src/mcda/mavt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/mavt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/mavt/aggregators.py
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/mavt/uta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.166923 mcda-0.7.0/src/mcda/outranking/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/outranking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/outranking/electre.py
--rw-rw-rw-   0 root         (0) root         (0)      351 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/outranking/promethee.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/outranking/srmp.py
--rw-rw-rw-   0 root         (0) root         (0)      801 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/plot.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      620 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/relations.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/scales.py
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/set_functions.py
--rw-rw-rw-   0 root         (0) root         (0)      190 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/transformers.py
--rw-rw-rw-   0 root         (0) root         (0)      796 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/types.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.166923 mcda-0.7.0/src/mcda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4365 2024-04-08 16:22:12.000000 mcda-0.7.0/src/mcda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1534 2024-04-08 16:22:12.000000 mcda-0.7.0/src/mcda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 16:22:12.000000 mcda-0.7.0/src/mcda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      134 2024-04-08 16:22:12.000000 mcda-0.7.0/src/mcda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-08 16:22:12.000000 mcda-0.7.0/src/mcda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:07:41.030108 mcda-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-04-26 16:07:30.000000 mcda-1.0.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       45 2024-04-26 16:07:30.000000 mcda-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4367 2024-04-26 16:07:41.030108 mcda-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2391 2024-04-26 16:07:30.000000 mcda-1.0.0/README.PYPI.md
+-rw-rw-rw-   0 root         (0) root         (0)     2775 2024-04-26 16:07:30.000000 mcda-1.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1403 2024-04-26 16:07:30.000000 mcda-1.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 16:07:41.030108 mcda-1.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:07:41.011108 mcda-1.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:07:41.017108 mcda-1.0.0/src/mcda/
+-rw-rw-rw-   0 root         (0) root         (0)      409 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/categories.py
+-rw-rw-rw-   0 root         (0) root         (0)      778 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:07:41.019108 mcda-1.0.0/src/mcda/internal/
+-rw-rw-rw-   0 root         (0) root         (0)      218 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:07:41.023108 mcda-1.0.0/src/mcda/internal/core/
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24037 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/core/aggregators.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/core/aliases.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/core/categories.py
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/core/compatibility.py
+-rw-rw-rw-   0 root         (0) root         (0)    13536 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/core/criteria_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15171 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/core/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/core/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    47210 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/core/matrices.py
+-rw-rw-rw-   0 root         (0) root         (0)    21757 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/core/relations.py
+-rw-rw-rw-   0 root         (0) root         (0)    23860 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/core/scales.py
+-rw-rw-rw-   0 root         (0) root         (0)    19032 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/core/set_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    21613 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/core/transformers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1188 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/core/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    15038 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/core/values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:07:41.024108 mcda-1.0.0/src/mcda/internal/dea/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/dea/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:07:41.024108 mcda-1.0.0/src/mcda/internal/mavt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/mavt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26123 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/mavt/uta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:07:41.025108 mcda-1.0.0/src/mcda/internal/outranking/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/outranking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    39413 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/outranking/electre.py
+-rw-rw-rw-   0 root         (0) root         (0)    32735 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/outranking/promethee.py
+-rw-rw-rw-   0 root         (0) root         (0)    38287 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/outranking/srmp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:07:41.026108 mcda-1.0.0/src/mcda/internal/plot/
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/plot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    44068 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/internal/plot/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      450 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/matrices.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:07:41.026108 mcda-1.0.0/src/mcda/mavt/
+-rw-rw-rw-   0 root         (0) root         (0)       83 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/mavt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/mavt/aggregators.py
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/mavt/uta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:07:41.027108 mcda-1.0.0/src/mcda/outranking/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/outranking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      322 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/outranking/electre.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/outranking/promethee.py
+-rw-rw-rw-   0 root         (0) root         (0)      345 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/outranking/srmp.py
+-rw-rw-rw-   0 root         (0) root         (0)      956 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      770 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/relations.py
+-rw-rw-rw-   0 root         (0) root         (0)      659 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/scales.py
+-rw-rw-rw-   0 root         (0) root         (0)      200 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/set_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/transformers.py
+-rw-rw-rw-   0 root         (0) root         (0)      796 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2024-04-26 16:07:30.000000 mcda-1.0.0/src/mcda/values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:07:41.029108 mcda-1.0.0/src/mcda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4367 2024-04-26 16:07:41.000000 mcda-1.0.0/src/mcda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1786 2024-04-26 16:07:41.000000 mcda-1.0.0/src/mcda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 16:07:41.000000 mcda-1.0.0/src/mcda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2024-04-26 16:07:41.000000 mcda-1.0.0/src/mcda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-26 16:07:41.000000 mcda-1.0.0/src/mcda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:07:41.029108 mcda-1.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2024-04-26 16:07:30.000000 mcda-1.0.0/tests/test_categories.py
+-rw-rw-rw-   0 root         (0) root         (0)    19608 2024-04-26 16:07:30.000000 mcda-1.0.0/tests/test_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-04-26 16:07:30.000000 mcda-1.0.0/tests/test_init.py
+-rw-rw-rw-   0 root         (0) root         (0)    53100 2024-04-26 16:07:30.000000 mcda-1.0.0/tests/test_matrices.py
+-rw-rw-rw-   0 root         (0) root         (0)    12689 2024-04-26 16:07:30.000000 mcda-1.0.0/tests/test_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)    17651 2024-04-26 16:07:30.000000 mcda-1.0.0/tests/test_scales.py
+-rw-rw-rw-   0 root         (0) root         (0)    14901 2024-04-26 16:07:30.000000 mcda-1.0.0/tests/test_set_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    18163 2024-04-26 16:07:30.000000 mcda-1.0.0/tests/test_transformers.py
+-rw-rw-rw-   0 root         (0) root         (0)    15890 2024-04-26 16:07:30.000000 mcda-1.0.0/tests/test_values.py
```

### Comparing `mcda-0.7.0/LICENSE` & `mcda-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcda-0.7.0/PKG-INFO` & `mcda-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcda
-Version: 0.7.0
+Version: 1.0.0
 Summary: Package for Multi Criteria Decision Analysis
 Author-email: Nicolas Duminy <nicolas.duminy@imt-atlantique.fr>, Patrick Meyer <patrick.meyer@imt-atlantique.fr>
 License: Copyright IMT Atlantique, 2021
         
         Project leaders:
           Patrick Meyer <patrick.meyer@imt-atlantique.fr>
           Nicolas Duminy <nicolas.duminy@imt-atlantique.fr>
@@ -17,15 +17,15 @@
         directory LICENCE.  The EUPL is available in 22 official languages of the
         European Union; for more informations, please check its website:
         https://joinup.ec.europa.eu/page/eupl-text-11-12
         
 Project-URL: Homepage, https://py-mcda.readthedocs.io
 Project-URL: Source, https://gitlab.com/decide.imt-atlantique/pymcda
 Project-URL: Issues, https://gitlab.com/decide.imt-atlantique/pymcda/issues
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -40,15 +40,15 @@
 Requires-Dist: typing_extensions; python_version < "3.11"
 Provides-Extra: plot
 Requires-Dist: graphviz; extra == "plot"
 Requires-Dist: matplotlib; extra == "plot"
 Provides-Extra: all
 Requires-Dist: mcda[plot]; extra == "all"
 
-Package for Multi-Criteria Decision Analysis named `mcda` (**Beta**).
+Package for Multi-Criteria Decision Analysis named `mcda`.
 
 
 # Package description
 
 This package is used as a basis to represent Multi-Criteria Decision Aiding (MCDA) problems as well as solve them.
 It also contains relatively low-level plotting functions to visualize a MCDA problem and its solution.
```

### Comparing `mcda-0.7.0/README.PYPI.md` & `mcda-1.0.0/README.PYPI.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Package for Multi-Criteria Decision Analysis named `mcda` (**Beta**).
+Package for Multi-Criteria Decision Analysis named `mcda`.
 
 
 # Package description
 
 This package is used as a basis to represent Multi-Criteria Decision Aiding (MCDA) problems as well as solve them.
 It also contains relatively low-level plotting functions to visualize a MCDA problem and its solution.
```

### Comparing `mcda-0.7.0/README.md` & `mcda-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Package for Multi-Criteria Decision Analysis named `mcda` (**Beta**).
+Package for Multi-Criteria Decision Analysis named `mcda`.
 
 
 # Table of contents
 
 [TOC]
```

### Comparing `mcda-0.7.0/pyproject.toml` & `mcda-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 [tool.pytest.ini_options]
 pythonpath = [
   "src"
 ]
 
 [project]
 name = "mcda"
-version = "0.7.0"
+version = "1.0.0"
 authors = [
   { name="Nicolas Duminy", email="nicolas.duminy@imt-atlantique.fr" },
   { name="Patrick Meyer", email="patrick.meyer@imt-atlantique.fr" },
 ]
 description = "Package for Multi Criteria Decision Analysis"
 readme = "README.PYPI.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Mathematics",
```

### Comparing `mcda-0.7.0/src/mcda/functions.py` & `mcda-1.0.0/src/mcda/functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""This module gathers all classes used to define functions.
+"""
 from .internal.core.aggregators import AdditiveValueFunctions
 from .internal.core.criteria_functions import (
     CriteriaFunctions,
     CriterionFunction,
 )
 from .internal.core.functions import (
     AffineFunction,
```

### Comparing `mcda-0.7.0/src/mcda/internal/core/aggregators.py` & `mcda-1.0.0/src/mcda/internal/core/aggregators.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     FuzzyScale,
     QuantitativeScale,
     Scale,
     common_scale_type,
 )
 from ..core.set_functions import ISetFunction, Mobius
 from ..core.values import CommensurableValues, Values
+from .compatibility import dataframe_map
 from .utils import set_module
 
 I_S = TypeVar("I_S", bound=Scale, covariant=True)
 O_S = TypeVar("O_S", bound=Scale, covariant=True)
 
 
 class Aggregator(Generic[I_S, O_S], ABC):
@@ -175,15 +176,15 @@
     ) -> AdjacencyValueMatrix[O_S]:
         """Apply aggregation method to each cell of a partial values matrix.
 
         :param partial_values:
         :return: aggregated partial values for each cell
         """
         return AdjacencyValueMatrix(
-            partial_values.data.applymap(self._aggregate_series),
+            dataframe_map(partial_values.data, self._aggregate_series),
             scale=self.out_scale,
             stype=self.out_stype,
         )
 
     @overload
     def __call__(
         self, data: Series, *args, **kwargs
@@ -605,17 +606,15 @@
                 key=lambda v: self.scale.value(v),
                 reverse=True,
             )
             lmin = min(_labels.index(a), _labels.index(b))
             lmax = max(_labels.index(a), _labels.index(b))
             _labels = _labels[lmin : lmax + 1]
         sims = [
-            self.scale.similarity(
-                self.scale.fuzzy[self.scale.labels.index(v)], ref_fuzzy
-            )
+            self.scale.similarity(self.scale.fuzzy[v], ref_fuzzy)
             for v in _labels
         ]
         return _labels[max(range(len(_labels)), key=lambda i: sims[i])]
 
     def _aggregate_series(
         self, series: Series, *args, weights=None, **kwargs
     ) -> Any:
```

### Comparing `mcda-0.7.0/src/mcda/internal/core/categories.py` & `mcda-1.0.0/src/mcda/internal/core/categories.py`

 * *Files identical despite different names*

### Comparing `mcda-0.7.0/src/mcda/internal/core/criteria_functions.py` & `mcda-1.0.0/src/mcda/internal/core/criteria_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from typing import Any, Generic, Mapping, Type, TypeVar, Union, cast, overload
 
 from pandas import DataFrame, Series
 
 from .aliases import Function
+from .compatibility import dataframe_map
 from .matrices import PartialValueMatrix, PerformanceTable
 from .scales import Scale
 from .utils import set_module
 from .values import CommensurableValues, Values
 
 I_S = TypeVar("I_S", bound=Scale, covariant=True)
 O_S = TypeVar("O_S", bound=Scale, covariant=True)
@@ -330,15 +331,15 @@
         :return: resulting partial values matrix
 
         .. note::
             This method is called when calling object as a function with a
             :class:`PartialValueMatrix` input.
         """
         return PartialValueMatrix(
-            partial_values.data.applymap(self._apply_series),
+            dataframe_map(partial_values.data, self._apply_series),
             scales=self.out_scales,
             stype=self.out_stype,
         )
 
     @overload
     def __call__(self, x: Series) -> Series:  # pragma: nocover
         ...
```

### Comparing `mcda-0.7.0/src/mcda/internal/core/functions.py` & `mcda-1.0.0/src/mcda/internal/core/functions.py`

 * *Files identical despite different names*

### Comparing `mcda-0.7.0/src/mcda/internal/core/interfaces.py` & `mcda-1.0.0/src/mcda/internal/core/interfaces.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,13 +65,13 @@
         pass
 
 
 class Sorter(ABC):
     """Interface to implement clustering/sorting MCDA algorithms."""
 
     @abstractmethod
-    def clusterize(self, **kwargs) -> CommensurableValues:  # pragma: nocover
-        """Clusterize alternatives.
+    def sort(self, **kwargs) -> CommensurableValues:  # pragma: nocover
+        """Sort alternatives in clusters.
 
         :return: cluster of each alternative
         """
         pass
```

### Comparing `mcda-0.7.0/src/mcda/internal/core/matrices.py` & `mcda-1.0.0/src/mcda/internal/core/matrices.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     overload,
 )
 
 from pandas import DataFrame, Series, concat
 from scipy.sparse import csr_matrix
 from scipy.sparse.csgraph import connected_components, floyd_warshall
 
+from .compatibility import dataframe_map
 from .scales import (
     BinaryScale,
     DiscreteQuantitativeScale,
     OrdinalScale,
     QuantitativeScale,
     Scale,
     common_scale_type,
@@ -731,15 +732,15 @@
         """Return values at criterion.
 
         :param key: criterion
         :raises KeyError: if `key` criterion doesn't exist
         :return:
         """
         return AdjacencyValueMatrix(
-            self._data.applymap(lambda s: s[key]),
+            dataframe_map(self._data, lambda s: s[key]),
             scale=self._scales[key],
             stype=self._stype,
         )
 
     def __iter__(self) -> Iterator[Any]:
         """Iterate on the criteria"""
         return iter(self._matrix.criteria)
@@ -774,27 +775,31 @@
             criteria = (
                 cast(Series, self.data.iloc[0, 0]).index.tolist()
                 if isinstance(self.data.iloc[0, 0], Series)
                 else list(range(len(self.data.iloc[0, 0])))
             )
         if len(set(criteria)) != len(criteria):
             raise KeyError("criteria must be uniques")
-        self.data = self.data.applymap(
-            lambda s: Series(list(s), index=criteria)
+        self.data = dataframe_map(
+            self.data, lambda s: Series(list(s), index=criteria)
         )
         self.scales: Mapping[Any, S] = {}
         _stype = cast(Type[S], Scale if stype is None else stype)
         for c in criteria:
             if isinstance(scales, Mapping) and c in scales:
                 self.scales[c] = scales[c]
             elif isinstance(scales, Scale):
                 self.scales[c] = cast(S, scales)
             else:
                 self.scales[c] = _stype.fit(
-                    Series(self.data.applymap(lambda s: s[c]).values.flatten())
+                    Series(
+                        dataframe_map(
+                            self.data, lambda s: s[c]
+                        ).values.flatten()
+                    )
                 )
             if stype and not isinstance(self.scales.get(c), stype):
                 raise TypeError("'stype' and 'scales' types mismatch")
         self.stype = (
             cast(
                 Type[S],
                 common_scale_type([type(s) for s in self.scales.values()]),
@@ -849,37 +854,37 @@
 
         :return: ``True`` if both are equal
         """
         if not isinstance(other, PartialValueMatrix):
             return False
         _values = cast(PartialValueMatrix, other)
         if self.scales == _values.scales:
-            d1 = self.data.applymap(lambda s: s.to_dict())
-            d2 = _values.data.applymap(lambda s: s.to_dict())
+            d1 = dataframe_map(self.data, lambda s: s.to_dict())
+            d2 = dataframe_map(_values.data, lambda s: s.to_dict())
             return d1.to_dict() == d2.to_dict()
         return False
 
     @property
     def within_scales(self) -> DataFrame:
         """Return a dataframe indicating which values are within their
         respective scale.
 
         :return:
         """
-        return self.data.applymap(
-            lambda s: Values(s, self.scales).within_scales
+        return dataframe_map(
+            self.data, lambda s: Values(s, self.scales).within_scales
         )
 
     @property
     def is_within_scales(self) -> bool:
         """Check whether all values are within their respective scales.
 
         :return:
         """
-        return self.within_scales.applymap(lambda s: s.all()).all(None)
+        return dataframe_map(self.within_scales, lambda s: s.all()).all(None)
 
     @property
     def is_numeric(self) -> bool:
         """Check whether table is numeric.
 
         :return:
         :rtype: bool
@@ -901,16 +906,17 @@
         :raise TypeError: if :attr:`scales` are not ordinal
         """
         if self.is_numeric:
             return cast(PartialValueMatrix[QuantitativeScale], self.copy())
         if not self.is_ordinal:
             raise TypeError("cannot convert to numerics nominal values")
         return PartialValueMatrix(
-            self.data.applymap(
-                lambda s: Values(s, scales=self.scales).to_numeric.data
+            dataframe_map(
+                self.data,
+                lambda s: Values(s, scales=self.scales).to_numeric.data,
             ),
             scales={
                 c: cast(OrdinalScale, s).numeric
                 for c, s in self.scales.items()
             },
         )
 
@@ -930,15 +936,17 @@
         :param rows:
         :param columns:
         :return:
         """
         vertices = self.vertices if vertices is None else vertices
         criteria = self.criteria if criteria is None else criteria
         return self.__class__(
-            self.data.loc[vertices, vertices].applymap(lambda s: s[criteria]),
+            dataframe_map(
+                self.data.loc[vertices, vertices], lambda s: s[criteria]
+            ),
             scales={
                 criterion: self.scales[criterion] for criterion in criteria
             },
             stype=self.stype,
         )
 
 
@@ -1249,15 +1257,15 @@
         # Create new matrix with appropriate names for components
         components = []
         for component_index in range(n_components):
             component = tuple(
                 self.data.index[labels == component_index].tolist()
             )
             components.append(component)
-        new_matrix = DataFrame(0, index=components, columns=components)
+        new_matrix = DataFrame(False, index=components, columns=components)
         for component_a, component_b in product(
             range(n_components), range(n_components)
         ):
             if component_a != component_b:
                 new_matrix.iloc[component_a, component_b] = (
                     self.data.iloc[
                         labels == component_a, labels == component_b
@@ -1279,15 +1287,17 @@
             raise TypeError(
                 "This property is only defined for binary matrices"
             )
         n_components, labels = connected_components(
             self.data.to_numpy(), connection="strong"
         )
         components = range(n_components)
-        new_matrix = DataFrame(0, index=self.vertices, columns=self.vertices)
+        new_matrix = DataFrame(
+            False, index=self.vertices, columns=self.vertices
+        )
         for component_a, component_b in product(components, components):
             if component_a != component_b:
                 new_matrix.loc[
                     labels == component_a, labels == component_b
                 ] = (
                     self.data.loc[labels == component_a, labels == component_b]
                     .to_numpy()
```

### Comparing `mcda-0.7.0/src/mcda/internal/core/relations.py` & `mcda-1.0.0/src/mcda/internal/core/relations.py`

 * *Files identical despite different names*

### Comparing `mcda-0.7.0/src/mcda/internal/core/scales.py` & `mcda-1.0.0/src/mcda/internal/core/scales.py`

 * *Files identical despite different names*

### Comparing `mcda-0.7.0/src/mcda/internal/core/set_functions.py` & `mcda-1.0.0/src/mcda/internal/core/set_functions.py`

 * *Files identical despite different names*

### Comparing `mcda-0.7.0/src/mcda/internal/core/transformers.py` & `mcda-1.0.0/src/mcda/internal/core/transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 scales.
 """
 from abc import ABC, abstractmethod
 from typing import Any, Mapping, TypeVar, Union, cast, overload
 
 from pandas import DataFrame, Series
 
+from .compatibility import dataframe_map
 from .matrices import (
     AdjacencyValueMatrix,
     PartialValueMatrix,
     PerformanceTable,
 )
 from .scales import (
     DiscreteQuantitativeScale,
@@ -345,16 +346,17 @@
 
         :param partial_values:
         :return: normalized partial value matrix (new object)
 
         .. note:: not intended for general usage
         """
         return PartialValueMatrix(
-            partial_values.data.applymap(
-                lambda s: cls._normalize_series(s, partial_values.scales)
+            dataframe_map(
+                partial_values.data,
+                lambda s: cls._normalize_series(s, partial_values.scales),
             ),
             scales=QuantitativeScale.normal(),
         )
 
     @classmethod
     def _transform_partial_values(
         cls,
@@ -366,18 +368,19 @@
         :param partial_values:
         :param out_scales: output scales
         :return: transformed partial value matrix (new object)
 
         .. note:: not intended for general usage
         """
         return PartialValueMatrix(
-            partial_values.data.applymap(
+            dataframe_map(
+                partial_values.data,
                 lambda s: cls._transform_series(
                     s, partial_values.scales, out_scales
-                )
+                ),
             ),
             scales=out_scales,
         )
 
     @overload
     @classmethod
     def normalize(cls, data: Any, in_scales: Scale) -> Any:  # pragma: nocover
```

### Comparing `mcda-0.7.0/src/mcda/internal/core/values.py` & `mcda-1.0.0/src/mcda/internal/core/values.py`

 * *Files identical despite different names*

### Comparing `mcda-0.7.0/src/mcda/internal/mavt/uta.py` & `mcda-1.0.0/src/mcda/internal/mavt/uta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 """This module implements the UTA algorithms.
 
 Implementation and naming conventions are taken from :cite:p:`siskos2005uta`.
-
-.. todo::
-    Rework internal methods/functions to make classes prettier and more
-    efficient
 """
 from typing import Any, Dict, List, Union
 
 import numpy as np
 from pulp import LpMaximize, LpMinimize, LpProblem, LpVariable, lpSum
 from pulp import value as pulp_value
```

### Comparing `mcda-0.7.0/src/mcda/internal/outranking/electre.py` & `mcda-1.0.0/src/mcda/internal/outranking/electre.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,19 @@
 """This module implements the Electre algorithms.
 
 Implementation and naming conventions are taken from
 :cite:p:`vincke1998electre`.
 """
 from abc import ABC, abstractmethod
-from typing import (
-    Any,
-    Dict,
-    Generic,
-    List,
-    Mapping,
-    Set,
-    Tuple,
-    TypeVar,
-    Union,
-    cast,
-)
+from typing import Any, Dict, Generic, List, Set, Tuple, TypeVar, Union, cast
 
 from pandas import DataFrame, Series
 
 from ..core.categories import BoundedCategoryProfile
+from ..core.compatibility import dataframe_map
 from ..core.interfaces import Assignator, Ranker, Selector
 from ..core.matrices import (
     AdjacencyValueMatrix,
     OutrankingMatrix,
     PartialValueMatrix,
     PerformanceTable,
     create_outranking_matrix,
@@ -217,15 +207,15 @@
     """
 
     def __init__(
         self,
         performance_table: PerformanceTable[QuantitativeScale],
         criteria_weights: Dict[Any, float],
         concordance_threshold: float,
-        veto_thresholds: Mapping[Any, float],
+        veto_thresholds: Dict[Any, float],
     ):
         super().__init__(
             performance_table=performance_table,
             criteria_weights=criteria_weights,
         )
         self.concordance_threshold = concordance_threshold
         self.veto_thresholds = veto_thresholds
@@ -243,16 +233,17 @@
         """
         res = DataFrame(
             0,
             index=concordance_matrix.vertices,
             columns=concordance_matrix.vertices,
         )
         d_hat = Series(self.veto_thresholds)
-        non_vetos = discordance_matrix.data.applymap(
-            lambda s: (s[d_hat.index.tolist()] <= d_hat).all()
+        non_vetos = dataframe_map(
+            discordance_matrix.data,
+            lambda s: (s[d_hat.index.tolist()] <= d_hat).all(),
         )
         res[
             (concordance_matrix.data >= self.concordance_threshold) & non_vetos
         ] = 1
         return create_outranking_matrix(res)
 
     def construct(self) -> OutrankingMatrix:
@@ -338,16 +329,16 @@
 
     def __init__(
         self,
         performance_table: PerformanceTable[QuantitativeScale],
         criteria_weights: Dict[Any, float],
         weak_concordance_threshold: float,
         strong_concordance_threshold: float,
-        weak_veto_thresholds: Mapping[Any, float],
-        strong_veto_thresholds: Mapping[Any, float],
+        weak_veto_thresholds: Dict[Any, float],
+        strong_veto_thresholds: Dict[Any, float],
     ):
         super().__init__(
             performance_table=performance_table,
             criteria_weights=criteria_weights,
         )
         self.weak_concordance_threshold = weak_concordance_threshold
         self.strong_concordance_threshold = strong_concordance_threshold
@@ -380,16 +371,17 @@
         )
 
         res = DataFrame(
             0,
             index=concordance_matrix.vertices,
             columns=concordance_matrix.vertices,
         )
-        non_vetos = discordance_matrix.data.applymap(
-            lambda s: (s[d_hat.index.tolist()] <= d_hat).all()
+        non_vetos = dataframe_map(
+            discordance_matrix.data,
+            lambda s: (s[d_hat.index.tolist()] <= d_hat).all(),
         )
         res[
             (concordance_matrix.data >= concordance_matrix.data.T)
             & (concordance_matrix.data >= c_hat)
             & non_vetos
         ] = 1
         return create_outranking_matrix(res)
```

### Comparing `mcda-0.7.0/src/mcda/internal/outranking/promethee.py` & `mcda-1.0.0/src/mcda/internal/outranking/promethee.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import matplotlib.pyplot as plt
 from pandas import DataFrame, Series
 from sklearn.decomposition import PCA
 
 from ..core.aggregators import Aggregator, NormalizedWeightedSum
 from ..core.aliases import NumericFunction
+from ..core.compatibility import dataframe_map
 from ..core.interfaces import Ranker
 from ..core.matrices import (
     AdjacencyValueMatrix,
     PartialValueMatrix,
     PerformanceTable,
 )
 from ..core.relations import (
@@ -565,15 +566,15 @@
 
     def pairwise_discordance(self, partial_preferences: Series) -> float:
         pass
 
     def discordance_from_partial(
         self, partial_preferences: AdjacencyMatrix
     ) -> AdjacencyMatrix:
-        data = partial_preferences.data.applymap(self.pairwise_discordance)
+        data = partial_preferences.data.map(self.pairwise_discordance)
         return partial_preferences.__class__(data)
 
 
 class Veto(GeneralizedCriteriaAggregator):
     def __init__(
         self,
         veto_thresholds: Dict[Any, float],
@@ -587,15 +588,15 @@
 
     def pairwise_veto(self, partial_preferences: Series) -> float:
         pass
 
     def veto_from_partial(
         self, partial_preferences: AdjacencyMatrix
     ) -> AdjacencyMatrix:
-        data = partial_preferences.data.applymap(self.pairwise_veto)
+        data = partial_preferences.data.map(self.pairwise_veto)
         return partial_preferences.__class__(data)
 
 
 class StrongVeto(Veto):
     def pairwise_veto(self, partial_preferences: Series) -> float:
         pass
 
@@ -758,15 +759,15 @@
         index=partial_preferences.vertices,
         columns=cast(
             Series, partial_preferences.data.iloc[0, 0]
         ).index.tolist(),
         dtype=float,
     )
     criteria_preferences = {
-        c: partial_preferences.data.applymap(lambda s, crit=c: s[crit])
+        c: dataframe_map(partial_preferences.data, lambda s, crit=c: s[crit])
         for c in res.columns
     }
     for a in res.index:
         for c, crit_prefs in criteria_preferences.items():
             res.loc[a, c] = (crit_prefs.loc[a] - crit_prefs[a]).mean()
     return res
 
@@ -816,16 +817,16 @@
         """Compute preferences for each alternatives' pair from partial
         preferences.
 
         :param partial_preferences:
         :return: preferences
         """
         return AdjacencyValueMatrix(
-            partial_preferences.data.applymap(
-                self.generalized_criteria_aggregator
+            dataframe_map(
+                partial_preferences.data, self.generalized_criteria_aggregator
             ),
             scale=self.generalized_criteria_aggregator.out_scale,
             stype=self.generalized_criteria_aggregator.out_stype,
         )
 
     @abstractmethod
     def flows(
```

### Comparing `mcda-0.7.0/src/mcda/internal/outranking/srmp.py` & `mcda-1.0.0/src/mcda/internal/outranking/srmp.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     LpMaximize,
     LpProblem,
     LpVariable,
     lpSum,
 )
 from pulp import value as pulp_value
 
+from ..core.compatibility import dataframe_map
 from ..core.interfaces import Learner, Ranker
 from ..core.matrices import PerformanceTable
 from ..core.relations import (
     IndifferenceRelation,
     OutrankingMatrix,
     PreferenceRelation,
     PreferenceStructure,
@@ -594,15 +595,15 @@
         )
         value_to_rank = {
             value: rank
             for value, rank in zip(
                 final_values, range(1, len(final_values) + 1)
             )
         }
-        ranks = rankings.applymap(lambda x: value_to_rank[x])
+        ranks = dataframe_map(rankings, lambda x: value_to_rank[x])
         nb_ranks = len(value_to_rank)
 
         # Create figure and axes
         fig = Figure(figsize=figsize)
         ax = Axis(xlabel="Profiles", ylabel="Rank")
         fig.add_axis(ax)
```

### Comparing `mcda-0.7.0/src/mcda/internal/plot/plot.py` & `mcda-1.0.0/src/mcda/internal/plot/plot.py`

 * *Files identical despite different names*

### Comparing `mcda-0.7.0/src/mcda/scales.py` & `mcda-1.0.0/src/mcda/scales.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""This module gathers all data scales and their features.
+"""
 from .internal.core.scales import (
     DiscreteQuantitativeScale,
     FuzzyScale,
     NominalScale,
     PreferenceDirection,
     QualitativeScale,
     QuantitativeScale,
```

### Comparing `mcda-0.7.0/src/mcda/types.py` & `mcda-1.0.0/src/mcda/types.py`

 * *Files identical despite different names*

### Comparing `mcda-0.7.0/src/mcda.egg-info/PKG-INFO` & `mcda-1.0.0/src/mcda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcda
-Version: 0.7.0
+Version: 1.0.0
 Summary: Package for Multi Criteria Decision Analysis
 Author-email: Nicolas Duminy <nicolas.duminy@imt-atlantique.fr>, Patrick Meyer <patrick.meyer@imt-atlantique.fr>
 License: Copyright IMT Atlantique, 2021
         
         Project leaders:
           Patrick Meyer <patrick.meyer@imt-atlantique.fr>
           Nicolas Duminy <nicolas.duminy@imt-atlantique.fr>
@@ -17,15 +17,15 @@
         directory LICENCE.  The EUPL is available in 22 official languages of the
         European Union; for more informations, please check its website:
         https://joinup.ec.europa.eu/page/eupl-text-11-12
         
 Project-URL: Homepage, https://py-mcda.readthedocs.io
 Project-URL: Source, https://gitlab.com/decide.imt-atlantique/pymcda
 Project-URL: Issues, https://gitlab.com/decide.imt-atlantique/pymcda/issues
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -40,15 +40,15 @@
 Requires-Dist: typing_extensions; python_version < "3.11"
 Provides-Extra: plot
 Requires-Dist: graphviz; extra == "plot"
 Requires-Dist: matplotlib; extra == "plot"
 Provides-Extra: all
 Requires-Dist: mcda[plot]; extra == "all"
 
-Package for Multi-Criteria Decision Analysis named `mcda` (**Beta**).
+Package for Multi-Criteria Decision Analysis named `mcda`.
 
 
 # Package description
 
 This package is used as a basis to represent Multi-Criteria Decision Aiding (MCDA) problems as well as solve them.
 It also contains relatively low-level plotting functions to visualize a MCDA problem and its solution.
```

