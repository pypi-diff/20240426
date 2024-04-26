# Comparing `tmp/dxrt-1.0.2.tar.gz` & `tmp/dxrt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxrt-1.0.2.tar", last modified: Thu Apr 25 19:20:01 2024, max compression
+gzip compressed data, was "dxrt-1.0.3.tar", last modified: Fri Apr 26 05:06:41 2024, max compression
```

## Comparing `dxrt-1.0.2.tar` & `dxrt-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 19:20:01.090793 dxrt-1.0.2/
--rw-rw-rw-   0        0        0      182 2024-04-25 19:20:01.089334 dxrt-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      121 2024-04-19 15:57:17.000000 dxrt-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 19:20:01.074210 dxrt-1.0.2/dxrt/
--rw-rw-rw-   0        0        0       42 2024-04-19 15:57:12.000000 dxrt-1.0.2/dxrt/__init__.py
--rw-rw-rw-   0        0        0     1999 2024-04-25 19:09:22.000000 dxrt-1.0.2/dxrt/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-04-25 19:20:01.087081 dxrt-1.0.2/dxrt.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-25 19:20:00.000000 dxrt-1.0.2/dxrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-25 19:20:00.000000 dxrt-1.0.2/dxrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 19:20:00.000000 dxrt-1.0.2/dxrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-25 19:20:00.000000 dxrt-1.0.2/dxrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-25 19:20:00.000000 dxrt-1.0.2/dxrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 19:20:01.090793 dxrt-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      332 2024-04-25 19:15:12.000000 dxrt-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:06:41.567393 dxrt-1.0.3/
+-rw-rw-rw-   0        0        0      182 2024-04-26 05:06:41.566351 dxrt-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2024-04-26 05:03:57.000000 dxrt-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 05:06:41.552882 dxrt-1.0.3/dxrt/
+-rw-rw-rw-   0        0        0       41 2024-04-26 05:02:31.000000 dxrt-1.0.3/dxrt/__init__.py
+-rw-rw-rw-   0        0        0    44028 2024-04-16 17:45:56.000000 dxrt-1.0.3/dxrt/pokemon.csv
+-rw-rw-rw-   0        0        0     2312 2024-04-26 05:01:30.000000 dxrt-1.0.3/dxrt/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:06:41.560769 dxrt-1.0.3/dxrt.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-26 05:06:41.000000 dxrt-1.0.3/dxrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-04-26 05:06:41.000000 dxrt-1.0.3/dxrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 05:06:41.000000 dxrt-1.0.3/dxrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-26 05:06:41.000000 dxrt-1.0.3/dxrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-26 05:06:41.000000 dxrt-1.0.3/dxrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 05:06:41.567393 dxrt-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      354 2024-04-26 05:03:20.000000 dxrt-1.0.3/setup.py
```

