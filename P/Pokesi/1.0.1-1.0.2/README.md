# Comparing `tmp/pokesi-1.0.1.tar.gz` & `tmp/pokesi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokesi-1.0.1.tar", last modified: Wed Apr 24 18:17:38 2024, max compression
+gzip compressed data, was "pokesi-1.0.2.tar", last modified: Fri Apr 26 13:56:17 2024, max compression
```

## Comparing `pokesi-1.0.1.tar` & `pokesi-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 18:17:38.242618 pokesi-1.0.1/
--rw-rw-rw-   0        0        0      237 2024-04-24 18:17:38.241584 pokesi-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 18:17:38.203304 pokesi-1.0.1/Pokesi/
--rw-rw-rw-   0        0        0       56 2024-04-23 17:51:13.000000 pokesi-1.0.1/Pokesi/_init_.py
--rw-rw-rw-   0        0        0    44028 2024-04-16 17:24:52.000000 pokesi-1.0.1/Pokesi/pokemon.csv
--rw-rw-rw-   0        0        0     1059 2024-04-17 18:57:31.000000 pokesi-1.0.1/Pokesi/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-04-24 18:17:38.239295 pokesi-1.0.1/Pokesi.egg-info/
--rw-rw-rw-   0        0        0      237 2024-04-24 18:17:37.000000 pokesi-1.0.1/Pokesi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2024-04-24 18:17:38.000000 pokesi-1.0.1/Pokesi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 18:17:37.000000 pokesi-1.0.1/Pokesi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 18:17:37.000000 pokesi-1.0.1/Pokesi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 18:17:37.000000 pokesi-1.0.1/Pokesi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      143 2024-04-23 17:52:21.000000 pokesi-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 18:17:38.243766 pokesi-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      517 2024-04-24 18:17:24.000000 pokesi-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 13:56:17.749824 pokesi-1.0.2/
+-rw-rw-rw-   0        0        0      201 2024-04-26 13:56:17.747814 pokesi-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-26 13:56:17.712813 pokesi-1.0.2/Pokesi/
+-rw-rw-rw-   0        0        0       41 2024-04-24 18:56:10.000000 pokesi-1.0.2/Pokesi/_init_.py
+-rw-rw-rw-   0        0        0    44028 2024-04-16 17:24:52.000000 pokesi-1.0.2/Pokesi/pokemon.csv
+-rw-rw-rw-   0        0        0     2235 2024-04-26 13:54:47.000000 pokesi-1.0.2/Pokesi/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-26 13:56:17.745817 pokesi-1.0.2/Pokesi.egg-info/
+-rw-rw-rw-   0        0        0      201 2024-04-26 13:56:17.000000 pokesi-1.0.2/Pokesi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2024-04-26 13:56:17.000000 pokesi-1.0.2/Pokesi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 13:56:17.000000 pokesi-1.0.2/Pokesi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-26 13:56:17.000000 pokesi-1.0.2/Pokesi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-26 13:56:17.000000 pokesi-1.0.2/Pokesi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      148 2024-04-26 11:21:43.000000 pokesi-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 13:56:17.749824 pokesi-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      367 2024-04-26 13:54:47.000000 pokesi-1.0.2/setup.py
```

### Comparing `pokesi-1.0.1/Pokesi/pokemon.csv` & `pokesi-1.0.2/Pokesi/pokemon.csv`

 * *Files identical despite different names*

