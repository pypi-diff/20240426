# Comparing `tmp/athenademo-0.1.0.tar.gz` & `tmp/athenademo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athenademo-0.1.0.tar", max compression
+gzip compressed data, was "athenademo-0.2.0.tar", max compression
```

## Comparing `athenademo-0.1.0.tar` & `athenademo-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-04-25 23:35:43.916722 athenademo-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-25 23:35:43.916722 athenademo-0.1.0/athenademo/__init__.py
--rw-r--r--   0        0        0       51 2024-04-25 23:36:53.302469 athenademo-0.1.0/athenademo/main.py
--rw-r--r--   0        0        0      315 2024-04-25 23:39:54.626852 athenademo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 athenademo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-25 23:35:43.916722 athenademo-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 23:35:43.916722 athenademo-0.2.0/athenademo/__init__.py
+-rw-r--r--   0        0        0       51 2024-04-25 23:36:53.302469 athenademo-0.2.0/athenademo/main.py
+-rw-r--r--   0        0        0      325 2024-04-25 23:46:43.572099 athenademo-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 athenademo-0.2.0/PKG-INFO
```

