# Comparing `tmp/mycloudlab1-0.0.2.tar.gz` & `tmp/mycloudlab1-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mycloudlab1-0.0.2.tar", last modified: Tue Apr 16 13:39:47 2024, max compression
+gzip compressed data, was "mycloudlab1-0.0.3.tar", last modified: Fri Apr 26 14:16:00 2024, max compression
```

## Comparing `mycloudlab1-0.0.2.tar` & `mycloudlab1-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:39:47.260863 mycloudlab1-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-16 13:39:47.260863 mycloudlab1-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-16 13:39:39.000000 mycloudlab1-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:39:47.260863 mycloudlab1-0.0.2/mycloudlab1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-16 13:39:47.000000 mycloudlab1-0.0.2/mycloudlab1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-16 13:39:47.000000 mycloudlab1-0.0.2/mycloudlab1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:39:47.000000 mycloudlab1-0.0.2/mycloudlab1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 13:39:47.000000 mycloudlab1-0.0.2/mycloudlab1.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 13:39:47.000000 mycloudlab1-0.0.2/mycloudlab1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:39:47.000000 mycloudlab1-0.0.2/mycloudlab1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:39:47.260863 mycloudlab1-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-16 13:39:39.000000 mycloudlab1-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:16:00.499455 mycloudlab1-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-26 14:16:00.499455 mycloudlab1-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-26 14:15:55.000000 mycloudlab1-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:16:00.499455 mycloudlab1-0.0.3/mycloudlab1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-26 14:16:00.000000 mycloudlab1-0.0.3/mycloudlab1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-26 14:16:00.000000 mycloudlab1-0.0.3/mycloudlab1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:16:00.000000 mycloudlab1-0.0.3/mycloudlab1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-26 14:16:00.000000 mycloudlab1-0.0.3/mycloudlab1.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 14:16:00.000000 mycloudlab1-0.0.3/mycloudlab1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:16:00.000000 mycloudlab1-0.0.3/mycloudlab1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 14:16:00.499455 mycloudlab1-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-26 14:15:55.000000 mycloudlab1-0.0.3/setup.py
```

