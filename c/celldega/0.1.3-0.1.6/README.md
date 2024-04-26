# Comparing `tmp/celldega-0.1.3.tar.gz` & `tmp/celldega-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "celldega-0.1.6.tar", last modified: Fri Apr 26 17:26:24 2024, max compression
```

## Comparing `celldega-0.1.3.tar` & `celldega-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,19 @@
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 celldega-0.1.3/src/celldega/__init__.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 celldega-0.1.3/src/celldega/static/widget.css
--rw-r--r--   0        0        0  6841087 2020-02-02 00:00:00.000000 celldega-0.1.3/src/celldega/static/widget.js
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 celldega-0.1.3/.gitignore
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 celldega-0.1.3/README.md
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 celldega-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 celldega-0.1.3/PKG-INFO
+drwxr-xr-x   0 feni       (503) staff       (20)        0 2024-04-26 17:26:24.239168 celldega-0.1.6/
+-rw-r--r--   0 feni       (503) staff       (20)     1526 2024-04-26 17:26:24.238843 celldega-0.1.6/PKG-INFO
+-rw-r--r--   0 feni       (503) staff       (20)     1009 2024-04-23 17:00:35.000000 celldega-0.1.6/README.md
+-rw-r--r--   0 feni       (503) staff       (20)      930 2024-04-26 17:23:39.000000 celldega-0.1.6/pyproject.toml
+-rw-r--r--   0 feni       (503) staff       (20)       38 2024-04-26 17:26:24.239230 celldega-0.1.6/setup.cfg
+drwxr-xr-x   0 feni       (503) staff       (20)        0 2024-04-26 17:26:24.234991 celldega-0.1.6/src/
+drwxr-xr-x   0 feni       (503) staff       (20)        0 2024-04-26 17:26:24.235781 celldega-0.1.6/src/celldega/
+-rw-r--r--   0 feni       (503) staff       (20)      285 2024-04-23 17:00:35.000000 celldega-0.1.6/src/celldega/__init__.py
+drwxr-xr-x   0 feni       (503) staff       (20)        0 2024-04-26 17:26:24.237309 celldega-0.1.6/src/celldega/pre/
+-rw-r--r--   0 feni       (503) staff       (20)    16313 2024-04-26 17:21:20.000000 celldega-0.1.6/src/celldega/pre/__init__.py
+drwxr-xr-x   0 feni       (503) staff       (20)        0 2024-04-26 17:26:24.237976 celldega-0.1.6/src/celldega/viz/
+-rw-r--r--   0 feni       (503) staff       (20)       66 2024-04-23 17:00:35.000000 celldega-0.1.6/src/celldega/viz/__init__.py
+-rw-r--r--   0 feni       (503) staff       (20)     1702 2024-04-25 18:31:07.000000 celldega-0.1.6/src/celldega/viz/widget.py
+drwxr-xr-x   0 feni       (503) staff       (20)        0 2024-04-26 17:26:24.238339 celldega-0.1.6/src/celldega.egg-info/
+-rw-r--r--   0 feni       (503) staff       (20)     1526 2024-04-26 17:26:24.000000 celldega-0.1.6/src/celldega.egg-info/PKG-INFO
+-rw-r--r--   0 feni       (503) staff       (20)      313 2024-04-26 17:26:24.000000 celldega-0.1.6/src/celldega.egg-info/SOURCES.txt
+-rw-r--r--   0 feni       (503) staff       (20)        1 2024-04-26 17:26:24.000000 celldega-0.1.6/src/celldega.egg-info/dependency_links.txt
+-rw-r--r--   0 feni       (503) staff       (20)      199 2024-04-26 17:26:24.000000 celldega-0.1.6/src/celldega.egg-info/requires.txt
+-rw-r--r--   0 feni       (503) staff       (20)        9 2024-04-26 17:26:24.000000 celldega-0.1.6/src/celldega.egg-info/top_level.txt
```

