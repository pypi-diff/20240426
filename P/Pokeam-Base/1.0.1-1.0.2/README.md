# Comparing `tmp/pokeam_base-1.0.1.tar.gz` & `tmp/pokeam_base-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokeam_base-1.0.1.tar", last modified: Wed Apr 24 18:35:56 2024, max compression
+gzip compressed data, was "pokeam_base-1.0.2.tar", last modified: Thu Apr 25 19:37:02 2024, max compression
```

## Comparing `pokeam_base-1.0.1.tar` & `pokeam_base-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 18:35:56.199097 pokeam_base-1.0.1/
--rw-rw-rw-   0        0        0      195 2024-04-24 18:35:56.198050 pokeam_base-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 18:35:56.186428 pokeam_base-1.0.1/Pokeam_Base/
--rw-rw-rw-   0        0        0       43 2024-04-19 15:35:58.000000 pokeam_base-1.0.1/Pokeam_Base/__init__.py
--rw-rw-rw-   0        0        0    44028 2024-04-16 17:22:33.000000 pokeam_base-1.0.1/Pokeam_Base/pokemon.csv
--rw-rw-rw-   0        0        0     2491 2024-04-23 17:29:36.000000 pokeam_base-1.0.1/Pokeam_Base/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-04-24 18:35:56.197052 pokeam_base-1.0.1/Pokeam_Base.egg-info/
--rw-rw-rw-   0        0        0      195 2024-04-24 18:35:56.000000 pokeam_base-1.0.1/Pokeam_Base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-04-24 18:35:56.000000 pokeam_base-1.0.1/Pokeam_Base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 18:35:56.000000 pokeam_base-1.0.1/Pokeam_Base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 18:35:56.000000 pokeam_base-1.0.1/Pokeam_Base.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-24 18:35:56.000000 pokeam_base-1.0.1/Pokeam_Base.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      145 2024-04-19 15:57:04.000000 pokeam_base-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 18:35:56.199097 pokeam_base-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      372 2024-04-24 18:35:49.000000 pokeam_base-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:37:02.666680 pokeam_base-1.0.2/
+-rw-rw-rw-   0        0        0      195 2024-04-25 19:37:02.665681 pokeam_base-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 19:37:02.657271 pokeam_base-1.0.2/Pokeam_Base/
+-rw-rw-rw-   0        0        0       43 2024-04-19 15:35:58.000000 pokeam_base-1.0.2/Pokeam_Base/__init__.py
+-rw-rw-rw-   0        0        0    44028 2024-04-16 17:22:33.000000 pokeam_base-1.0.2/Pokeam_Base/pokemon.csv
+-rw-rw-rw-   0        0        0     2057 2024-04-25 19:30:22.000000 pokeam_base-1.0.2/Pokeam_Base/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:37:02.664713 pokeam_base-1.0.2/Pokeam_Base.egg-info/
+-rw-rw-rw-   0        0        0      195 2024-04-25 19:37:02.000000 pokeam_base-1.0.2/Pokeam_Base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2024-04-25 19:37:02.000000 pokeam_base-1.0.2/Pokeam_Base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 19:37:02.000000 pokeam_base-1.0.2/Pokeam_Base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-25 19:37:02.000000 pokeam_base-1.0.2/Pokeam_Base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-25 19:37:02.000000 pokeam_base-1.0.2/Pokeam_Base.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      145 2024-04-19 15:57:04.000000 pokeam_base-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-25 19:37:02.666680 pokeam_base-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      372 2024-04-25 19:30:22.000000 pokeam_base-1.0.2/setup.py
```

### Comparing `pokeam_base-1.0.1/Pokeam_Base/pokemon.csv` & `pokeam_base-1.0.2/Pokeam_Base/pokemon.csv`

 * *Files identical despite different names*

