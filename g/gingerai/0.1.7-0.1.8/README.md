# Comparing `tmp/gingerai-0.1.7.tar.gz` & `tmp/gingerai-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gingerai-0.1.7.tar", last modified: Thu Apr 25 13:56:14 2024, max compression
+gzip compressed data, was "gingerai-0.1.8.tar", last modified: Thu Apr 25 23:27:45 2024, max compression
```

## Comparing `gingerai-0.1.7.tar` & `gingerai-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:56:14.516857 gingerai-0.1.7/
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      340 2024-04-25 13:56:14.516857 gingerai-0.1.7/PKG-INFO
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:56:14.000000 gingerai-0.1.7/README.md
-drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:56:14.516857 gingerai-0.1.7/gingerai/
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)     1790 2024-04-25 13:56:14.000000 gingerai-0.1.7/gingerai/TorchNetWrapper.py
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)       82 2024-04-25 13:56:14.000000 gingerai-0.1.7/gingerai/__init__.py
-drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:56:14.516857 gingerai-0.1.7/gingerai.egg-info/
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      340 2024-04-25 13:56:14.000000 gingerai-0.1.7/gingerai.egg-info/PKG-INFO
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      226 2024-04-25 13:56:14.000000 gingerai-0.1.7/gingerai.egg-info/SOURCES.txt
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        1 2024-04-25 13:56:14.000000 gingerai-0.1.7/gingerai.egg-info/dependency_links.txt
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        6 2024-04-25 13:56:14.000000 gingerai-0.1.7/gingerai.egg-info/requires.txt
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        9 2024-04-25 13:56:14.000000 gingerai-0.1.7/gingerai.egg-info/top_level.txt
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)       38 2024-04-25 13:56:14.516857 gingerai-0.1.7/setup.cfg
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      439 2024-04-25 13:56:14.000000 gingerai-0.1.7/setup.py
+drwxr-xr-x   0 tranie     (501) staff       (20)        0 2024-04-25 23:27:45.887085 gingerai-0.1.8/
+-rw-r--r--   0 tranie     (501) staff       (20)      389 2024-04-25 23:27:45.886749 gingerai-0.1.8/PKG-INFO
+-rw-r--r--   0 tranie     (501) staff       (20)        0 2024-04-25 23:27:45.000000 gingerai-0.1.8/README.md
+drwxr-xr-x   0 tranie     (501) staff       (20)        0 2024-04-25 23:27:45.883194 gingerai-0.1.8/gingerai/
+-rw-r--r--   0 tranie     (501) staff       (20)     3077 2024-04-25 23:27:45.000000 gingerai-0.1.8/gingerai/ModelUploader.py
+-rw-r--r--   0 tranie     (501) staff       (20)       90 2024-04-25 23:27:45.000000 gingerai-0.1.8/gingerai/__init__.py
+drwxr-xr-x   0 tranie     (501) staff       (20)        0 2024-04-25 23:27:45.886150 gingerai-0.1.8/gingerai.egg-info/
+-rw-r--r--   0 tranie     (501) staff       (20)      389 2024-04-25 23:27:45.000000 gingerai-0.1.8/gingerai.egg-info/PKG-INFO
+-rw-r--r--   0 tranie     (501) staff       (20)      224 2024-04-25 23:27:45.000000 gingerai-0.1.8/gingerai.egg-info/SOURCES.txt
+-rw-r--r--   0 tranie     (501) staff       (20)        1 2024-04-25 23:27:45.000000 gingerai-0.1.8/gingerai.egg-info/dependency_links.txt
+-rw-r--r--   0 tranie     (501) staff       (20)       34 2024-04-25 23:27:45.000000 gingerai-0.1.8/gingerai.egg-info/requires.txt
+-rw-r--r--   0 tranie     (501) staff       (20)        9 2024-04-25 23:27:45.000000 gingerai-0.1.8/gingerai.egg-info/top_level.txt
+-rw-r--r--   0 tranie     (501) staff       (20)       38 2024-04-25 23:27:45.887160 gingerai-0.1.8/setup.cfg
+-rw-r--r--   0 tranie     (501) staff       (20)      476 2024-04-25 23:27:45.000000 gingerai-0.1.8/setup.py
```

