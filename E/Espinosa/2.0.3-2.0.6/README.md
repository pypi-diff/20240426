# Comparing `tmp/espinosa-2.0.3.tar.gz` & `tmp/espinosa-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espinosa-2.0.3.tar", last modified: Fri Apr 26 05:11:10 2024, max compression
+gzip compressed data, was "espinosa-2.0.6.tar", last modified: Fri Apr 26 05:20:29 2024, max compression
```

## Comparing `espinosa-2.0.3.tar` & `espinosa-2.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 05:11:10.481686 espinosa-2.0.3/
-drwxrwxrwx   0        0        0        0 2024-04-26 05:11:10.466175 espinosa-2.0.3/Espinosa/
--rw-rw-rw-   0        0        0       41 2024-04-26 05:06:50.000000 espinosa-2.0.3/Espinosa/__init__.py
--rw-rw-rw-   0        0        0     1923 2024-04-26 05:06:18.000000 espinosa-2.0.3/Espinosa/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-04-26 05:11:10.477551 espinosa-2.0.3/Espinosa.egg-info/
--rw-rw-rw-   0        0        0      187 2024-04-26 05:11:10.000000 espinosa-2.0.3/Espinosa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-04-26 05:11:10.000000 espinosa-2.0.3/Espinosa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 05:11:10.000000 espinosa-2.0.3/Espinosa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-26 05:11:10.000000 espinosa-2.0.3/Espinosa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-26 05:11:10.000000 espinosa-2.0.3/Espinosa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      187 2024-04-26 05:11:10.480683 espinosa-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      150 2024-04-26 05:08:12.000000 espinosa-2.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-26 05:11:10.481686 espinosa-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      363 2024-04-26 05:09:27.000000 espinosa-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:20:29.128344 espinosa-2.0.6/
+drwxrwxrwx   0        0        0        0 2024-04-26 05:20:29.106654 espinosa-2.0.6/Espinosa/
+-rw-rw-rw-   0        0        0       41 2024-04-26 05:06:50.000000 espinosa-2.0.6/Espinosa/__init__.py
+-rw-rw-rw-   0        0        0     2218 2024-04-26 05:19:39.000000 espinosa-2.0.6/Espinosa/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:20:29.120279 espinosa-2.0.6/Espinosa.egg-info/
+-rw-rw-rw-   0        0        0      187 2024-04-26 05:20:29.000000 espinosa-2.0.6/Espinosa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-04-26 05:20:29.000000 espinosa-2.0.6/Espinosa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 05:20:29.000000 espinosa-2.0.6/Espinosa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-26 05:20:29.000000 espinosa-2.0.6/Espinosa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-26 05:20:29.000000 espinosa-2.0.6/Espinosa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      187 2024-04-26 05:20:29.124584 espinosa-2.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2024-04-26 05:08:12.000000 espinosa-2.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 05:20:29.128344 espinosa-2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      363 2024-04-26 05:20:22.000000 espinosa-2.0.6/setup.py
```

