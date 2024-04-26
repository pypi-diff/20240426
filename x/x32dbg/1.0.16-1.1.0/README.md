# Comparing `tmp/x32dbg-1.0.16.tar.gz` & `tmp/x32dbg-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x32dbg-1.0.16.tar", last modified: Wed Apr 17 09:16:12 2024, max compression
+gzip compressed data, was "x32dbg-1.1.0.tar", last modified: Fri Apr 26 03:09:27 2024, max compression
```

## Comparing `x32dbg-1.0.16.tar` & `x32dbg-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 09:16:11.994025 x32dbg-1.0.16/
--r--r--r--   0        0        0    35613 2022-10-01 07:57:15.000000 x32dbg-1.0.16/LICENSE
--rw-rw-rw-   0        0        0      245 2024-04-17 09:16:11.962836 x32dbg-1.0.16/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-17 09:16:11.994025 x32dbg-1.0.16/setup.cfg
--rw-rw-rw-   0        0        0      392 2024-04-17 09:10:20.000000 x32dbg-1.0.16/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 09:16:11.658833 x32dbg-1.0.16/x32dbg/
--rw-rw-rw-   0        0        0    69916 2024-04-17 09:13:03.000000 x32dbg-1.0.16/x32dbg/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 09:16:11.916021 x32dbg-1.0.16/x32dbg.egg-info/
--rw-rw-rw-   0        0        0      245 2024-04-17 09:16:11.000000 x32dbg-1.0.16/x32dbg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      155 2024-04-17 09:16:11.000000 x32dbg-1.0.16/x32dbg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 09:16:11.000000 x32dbg-1.0.16/x32dbg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-17 09:16:11.000000 x32dbg-1.0.16/x32dbg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 03:09:27.633299 x32dbg-1.1.0/
+-rw-rw-rw-   0        0        0    35613 2022-10-01 07:57:15.000000 x32dbg-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1035 2024-04-26 03:09:27.631313 x32dbg-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2024-04-23 11:37:43.000000 x32dbg-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 03:09:27.633299 x32dbg-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      991 2024-04-24 08:43:35.000000 x32dbg-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:09:27.359393 x32dbg-1.1.0/x32dbg/
+-rw-rw-rw-   0        0        0   150749 2024-04-25 13:28:41.000000 x32dbg-1.1.0/x32dbg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:09:27.571322 x32dbg-1.1.0/x32dbg.egg-info/
+-rw-rw-rw-   0        0        0     1035 2024-04-26 03:09:27.000000 x32dbg-1.1.0/x32dbg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      165 2024-04-26 03:09:27.000000 x32dbg-1.1.0/x32dbg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 03:09:27.000000 x32dbg-1.1.0/x32dbg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-26 03:09:27.000000 x32dbg-1.1.0/x32dbg.egg-info/top_level.txt
```

### Comparing `x32dbg-1.0.16/LICENSE` & `x32dbg-1.1.0/LICENSE`

 * *Files identical despite different names*

