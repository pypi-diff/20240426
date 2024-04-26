# Comparing `tmp/TheBeans-0.0.7.tar.gz` & `tmp/thebeans-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TheBeans-0.0.7.tar", last modified: Thu Apr  4 01:12:38 2024, max compression
+gzip compressed data, was "thebeans-0.0.8.tar", last modified: Fri Apr 26 15:55:38 2024, max compression
```

## Comparing `TheBeans-0.0.7.tar` & `thebeans-0.0.8.tar`

### file list

```diff
@@ -1,75 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.357570 TheBeans-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.345569 TheBeans-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.349570 TheBeans-0.0.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.349570 TheBeans-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:12:20.000000 TheBeans-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-04 01:12:20.000000 TheBeans-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-04 01:12:38.357570 TheBeans-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-04 01:12:20.000000 TheBeans-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.357570 TheBeans-0.0.7/TheBeans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-04 01:12:38.000000 TheBeans-0.0.7/TheBeans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-04 01:12:38.000000 TheBeans-0.0.7/TheBeans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:12:38.000000 TheBeans-0.0.7/TheBeans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 01:12:38.000000 TheBeans-0.0.7/TheBeans.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 01:12:38.000000 TheBeans-0.0.7/TheBeans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 01:12:38.000000 TheBeans-0.0.7/TheBeans.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.353570 TheBeans-0.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/CSVtoDF.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.353570 TheBeans-0.0.7/docs/Labs/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/Labs/_cats_.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/Labs/_dogs_.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/Labs/broken_dogs_.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/Labs/guestbook.txt
--rw-r--r--   0 runner    (1001) docker     (127)    33576 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/Labs/lab4.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    42912 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/Labs/lab5.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/Labs/learning_python.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/Labs/name.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/Labs/reasons.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.357570 TheBeans-0.0.7/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    15852 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/CedarCubMuck.dbf
--rw-r--r--   0 runner    (1001) docker     (127)   309152 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/CedarCubMuck.shp
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/ExampleBeansLab7.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/StudyArea.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/classnotes.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/csv.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   117900 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/europe_110.geo.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/ipyleaflet.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/raster.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   207731 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/us_regions.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.357570 TheBeans-0.0.7/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/thebeans.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-04 01:12:20.000000 TheBeans-0.0.7/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-04 01:12:20.000000 TheBeans-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 01:12:20.000000 TheBeans-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-04 01:12:20.000000 TheBeans-0.0.7/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 01:12:38.357570 TheBeans-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.357570 TheBeans-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 01:12:20.000000 TheBeans-0.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-04 01:12:20.000000 TheBeans-0.0.7/tests/test_thebeans.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.357570 TheBeans-0.0.7/thebeans/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-04 01:12:20.000000 TheBeans-0.0.7/thebeans/CSVtoDF.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-04 01:12:20.000000 TheBeans-0.0.7/thebeans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-04 01:12:20.000000 TheBeans-0.0.7/thebeans/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-04-04 01:12:20.000000 TheBeans-0.0.7/thebeans/thebeans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.950176 thebeans-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-26 15:55:28.000000 thebeans-0.0.8/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.938176 thebeans-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.938176 thebeans-0.0.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.942176 thebeans-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-26 15:55:28.000000 thebeans-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:55:28.000000 thebeans-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-26 15:55:28.000000 thebeans-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-26 15:55:38.950176 thebeans-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-26 15:55:28.000000 thebeans-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.950176 thebeans-0.0.8/TheBeans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-26 15:55:38.000000 thebeans-0.0.8/TheBeans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-26 15:55:38.000000 thebeans-0.0.8/TheBeans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:55:38.000000 thebeans-0.0.8/TheBeans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 15:55:38.000000 thebeans-0.0.8/TheBeans.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-26 15:55:38.000000 thebeans-0.0.8/TheBeans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 15:55:38.000000 thebeans-0.0.8/TheBeans.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.942176 thebeans-0.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/CSVtoDF.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.942176 thebeans-0.0.8/docs/Labs/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/Labs/_cats_.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/Labs/_dogs_.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/Labs/broken_dogs_.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/Labs/guestbook.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    33576 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/Labs/lab4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    42912 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/Labs/lab5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/Labs/learning_python.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/Labs/name.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/Labs/reasons.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.946176 thebeans-0.0.8/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/ExampleBeans.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/Lab9_Toolbar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/StudyArea.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/csv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   117900 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/europe_110.geo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/folium.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/raster.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   207731 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/us_regions.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.946176 thebeans-0.0.8/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/thebeans.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-26 15:55:28.000000 thebeans-0.0.8/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-26 15:55:28.000000 thebeans-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 15:55:28.000000 thebeans-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-26 15:55:28.000000 thebeans-0.0.8/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:55:38.950176 thebeans-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.946176 thebeans-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:55:28.000000 thebeans-0.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-26 15:55:28.000000 thebeans-0.0.8/tests/test_thebeans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.946176 thebeans-0.0.8/thebeans/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-26 15:55:28.000000 thebeans-0.0.8/thebeans/CSVtoDF.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-26 15:55:28.000000 thebeans-0.0.8/thebeans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-26 15:55:28.000000 thebeans-0.0.8/thebeans/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-26 15:55:28.000000 thebeans-0.0.8/thebeans/foliummap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14476 2024-04-26 15:55:28.000000 thebeans-0.0.8/thebeans/thebeans.py
```

### Comparing `TheBeans-0.0.7/.github/workflows/docs-build.yml` & `thebeans-0.0.8/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.7/.github/workflows/docs.yml` & `thebeans-0.0.8/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.7/.github/workflows/installation.yml` & `thebeans-0.0.8/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.7/.github/workflows/macos.yml` & `thebeans-0.0.8/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.7/.github/workflows/pypi.yml` & `thebeans-0.0.8/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.7/.github/workflows/ubuntu.yml` & `thebeans-0.0.8/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.7/.github/workflows/windows.yml` & `thebeans-0.0.8/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.7/.gitignore` & `thebeans-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.7/PKG-INFO` & `thebeans-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TheBeans
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python package with the beans.
 Author-email: Lucas Phillips <lphill57@vols.utk.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/phillipslucas/TheBeans
 Keywords: TheBeans
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `TheBeans-0.0.7/TheBeans.egg-info/PKG-INFO` & `thebeans-0.0.8/TheBeans.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TheBeans
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python package with the beans.
 Author-email: Lucas Phillips <lphill57@vols.utk.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/phillipslucas/TheBeans
 Keywords: TheBeans
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `TheBeans-0.0.7/TheBeans.egg-info/SOURCES.txt` & `thebeans-0.0.8/TheBeans.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -37,26 +37,25 @@
 docs/Labs/broken_dogs_.txt
 docs/Labs/guestbook.txt
 docs/Labs/lab4.ipynb
 docs/Labs/lab5.ipynb
 docs/Labs/learning_python.txt
 docs/Labs/name.txt
 docs/Labs/reasons.txt
-docs/examples/CedarCubMuck.dbf
-docs/examples/CedarCubMuck.shp
-docs/examples/ExampleBeansLab7.ipynb
+docs/examples/ExampleBeans.ipynb
+docs/examples/Lab9_Toolbar.ipynb
 docs/examples/StudyArea.geojson
-docs/examples/classnotes.ipynb
 docs/examples/csv.ipynb
 docs/examples/europe_110.geo.json
-docs/examples/intro.ipynb
-docs/examples/ipyleaflet.ipynb
+docs/examples/folium.ipynb
+docs/examples/quickstart.ipynb
 docs/examples/raster.ipynb
 docs/examples/us_regions.geojson
 docs/examples/vector.ipynb
 docs/overrides/main.html
 tests/__init__.py
 tests/test_thebeans.py
 thebeans/CSVtoDF.py
 thebeans/__init__.py
 thebeans/common.py
+thebeans/foliummap.py
 thebeans/thebeans.py
```

### Comparing `TheBeans-0.0.7/docs/Labs/lab4.ipynb` & `thebeans-0.0.8/docs/Labs/lab4.ipynb`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.7/docs/Labs/lab5.ipynb` & `thebeans-0.0.8/docs/Labs/lab5.ipynb`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.7/docs/contributing.md` & `thebeans-0.0.8/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.7/docs/examples/StudyArea.geojson` & `thebeans-0.0.8/docs/examples/StudyArea.geojson`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.7/docs/examples/classnotes.ipynb` & `thebeans-0.0.8/docs/examples/Lab9_Toolbar.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7010745614035088%*

 * *Differences: {"'cells'": "{0: {'cell_type': 'markdown', 'source': "*

 * *            "['[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/phillipslucas/TheBeans/blob/main/docs/examples/Lab9_Toolbar.ipynb)'], "*

 * *            "delete: ['execution_count', 'outputs']}, 1: {'execution_count': 1, 'outputs': "*

 * *            "[OrderedDict([('data', OrderedDict([('application/vnd.jupyter.widget-view+json', "*

 * *            "OrderedDict([('model_id', '71971bf05184423fab700901e1eeb9f […]*

```diff
@@ -1,116 +1,111 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "#create slider outside of map, \n",
-                "zoom_slider = IntSlider(description='Zoom level:', min=0, max=15, value=7) #integer slyder, zoome level label\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "# passes zoom slider value, which can be read, IF LINKED, by other widgets.\n",
-                "zoom_slider.value"
+                "[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/phillipslucas/TheBeans/blob/main/docs/examples/Lab9_Toolbar.ipynb)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 1,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "71971bf05184423fab700901e1eeb9f1",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "Map(center=[0, 0], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title', 'zoom_out_text'\u2026"
+                        ]
+                    },
+                    "execution_count": 1,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
-                "#ipyleaflet build off ipywidgets\n",
-                "\n",
-                "#\n",
-                "\n",
-                "from ipyleaflet import  basemaps, WidgetControl\n",
-                "from ipywidgets import IntSlider, ColorPicker, jslink, Output #output super powerful upload of files\n",
-                "\n",
-                "m = thebeans.Map(center=(46.01, 6.16), zoom=12, basemap=basemaps.OpenTopoMap)\n",
-                "zoom_slider = IntSlider(description='Zoom level:', min=0, max=17, value=7) #integer slyder, zoome level label, max value is 15 but bug allows you to zoom in to 17. change to 24 to avoid confusion.\n",
-                "jslink((zoom_slider, 'value'), (m, 'zoom')) #VERY IMPORTANT LINE, links control to the widget. change value of this slider changes value of zoom on map\n",
-                "widget_control1 = WidgetControl(widget=zoom_slider, position='topright') #widget control places the widget\n",
-                "m.add(widget_control1)\n",
-                "\n",
-                "out_widget = Output(layout={'border': '1px solid black'})\n",
-                "output_control = WidgetControl(widget=out_widget, position='bottomright')\n",
-                "m.add(output_control) #adds nothing because haven't put anything in it yet?\n",
-                "\n",
-                "with out_widget:\n",
-                "    print('Hello world!') #Adds something to the out_widget\n",
-                "    #can pass datasets and plots to it\n",
-                "    #sample data\n",
-                "    x = [4, 23, 4, 5, 6, 9,8, 1]\n",
-                "    y = [5, 6, 7, 8, 9, 10, 11, 12]\n",
+                "import thebeans\n",
                 "\n",
-                "    fig, ax = plt.subplots()\n",
                 "\n",
-                "    ax.plot(x, y)\n",
+                "#Create a map\n",
+                "m = thebeans.Map()\n",
                 "\n",
-                "#out_widget.clear_output() #clears output\n",
+                "#add toolbar using the add_toolbar function\n",
+                "#explore the buttons at your leisure\n",
+                "m.add_toolbar()\n",
                 "\n",
                 "\n",
-                "m\n",
-                "# color_picker = ColorPicker(description='Pick a color:')\n",
-                "# widget_control2 = WidgetControl(widget=color_picker, position='bottomright')\n",
-                "# m.add(widget_control2)\n",
-                "# m"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import geopandas as gpd\n",
-                "\n",
-                "\n",
-                "\n",
-                "df = gpd.read_file('StudyArea.geojson')\n",
-                "\n",
-                "#re-project to local stateplane 2285 - North WA, 4326 WGS 84\n",
-                "df = df.to_crs(epsg=4326)\n",
-                "\n",
-                "df[\"lon\"] = df[\"geometry\"].centroid.x\n",
-                "df[\"lat\"] = df[\"geometry\"].centroid.y\n",
-                "df\n"
+                "m"
             ]
         }
     ],
     "metadata": {
+        "hide_input": false,
         "kernelspec": {
-            "display_name": "base",
+            "display_name": "Python 3",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.11.8"
+        },
+        "toc": {
+            "base_numbering": 1,
+            "nav_menu": {},
+            "number_sections": true,
+            "sideBar": true,
+            "skip_h1_title": false,
+            "title_cell": "Table of Contents",
+            "title_sidebar": "Contents",
+            "toc_cell": false,
+            "toc_position": {},
+            "toc_section_display": true,
+            "toc_window_display": false
+        },
+        "varInspector": {
+            "cols": {
+                "lenName": 16,
+                "lenType": 16,
+                "lenVar": 40
+            },
+            "kernels_config": {
+                "python": {
+                    "delete_cmd_postfix": "",
+                    "delete_cmd_prefix": "del ",
+                    "library": "var_list.py",
+                    "varRefreshCmd": "print(var_dic_list())"
+                },
+                "r": {
+                    "delete_cmd_postfix": ") ",
+                    "delete_cmd_prefix": "rm(",
+                    "library": "var_list.r",
+                    "varRefreshCmd": "cat(var_dic_list()) "
+                }
+            },
+            "types_to_exclude": [
+                "module",
+                "function",
+                "builtin_function_or_method",
+                "instance",
+                "_Feature"
+            ],
+            "window_display": false
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `TheBeans-0.0.7/docs/examples/csv.ipynb` & `thebeans-0.0.8/docs/examples/csv.ipynb`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.7/docs/examples/europe_110.geo.json` & `thebeans-0.0.8/docs/examples/europe_110.geo.json`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.7/docs/examples/us_regions.geojson` & `thebeans-0.0.8/docs/examples/us_regions.geojson`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.7/docs/examples/vector.ipynb` & `thebeans-0.0.8/docs/examples/vector.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947916666666667%*

 * *Differences: {"'cells'": "{0: {'source': "*

 * *            "['[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/phillipslucas/TheBeans/blob/main/docs/examples/vector.ipynb)']}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "[![image](https://colab.research.google.com/assets/colab-badge.svg)]()"
+                "[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/phillipslucas/TheBeans/blob/main/docs/examples/vector.ipynb)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
```

### Comparing `TheBeans-0.0.7/docs/installation.md` & `thebeans-0.0.8/docs/installation.md`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.7/mkdocs.yml` & `thebeans-0.0.8/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -72,17 +72,19 @@
     - Installation: installation.md
     - Usage: usage.md
     - Contributing: contributing.md
     - FAQ: faq.md
     - Changelog: changelog.md
     - Report Issues: https://github.com/phillipslucas/TheBeans/issues
     - Examples:
-        - examples/ExampleBeansLab7.ipynb
+        - examples/ExampleBeans.ipynb
         - examples/csv.ipynb
         - examples/vector.ipynb
+        - examples/raster.ipynb
+        - examples/Lab9_Toolbar.ipynb
     - API Reference:
           - thebeans module: thebeans.md
           - common module: common.md
           - CSVtoDF module: CSVtoDF.md
     - Labs:
         - Labs/lab4.ipynb
         - Labs/lab5.ipynb
```

### Comparing `TheBeans-0.0.7/pyproject.toml` & `thebeans-0.0.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "TheBeans"
-version = "0.0.7"
+version = "0.0.8"
 dynamic = [
     "dependencies",
 ]
 description = "Python package with the beans."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.7"
+current_version = "0.0.8"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

