# Comparing `tmp/pokeaditto_base-1.0.0.tar.gz` & `tmp/Pokeaditto_base-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokeaditto_base-1.0.0.tar", last modified: Wed Apr 24 16:18:35 2024, max compression
+gzip compressed data, was "Pokeaditto_base-1.0.1.tar", last modified: Fri Apr 26 00:25:47 2024, max compression
```

## Comparing `pokeaditto_base-1.0.0.tar` & `Pokeaditto_base-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 16:18:35.599915 pokeaditto_base-1.0.0/
--rw-rw-rw-   0        0        0      204 2024-04-24 16:18:35.598879 pokeaditto_base-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 16:18:35.596761 pokeaditto_base-1.0.0/Pokeaditto_base.egg-info/
--rw-rw-rw-   0        0        0      204 2024-04-24 16:18:35.000000 pokeaditto_base-1.0.0/Pokeaditto_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-04-24 16:18:35.000000 pokeaditto_base-1.0.0/Pokeaditto_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 16:18:35.000000 pokeaditto_base-1.0.0/Pokeaditto_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 16:18:35.000000 pokeaditto_base-1.0.0/Pokeaditto_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 16:18:35.000000 pokeaditto_base-1.0.0/Pokeaditto_base.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      121 2024-04-24 16:17:38.000000 pokeaditto_base-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 16:18:35.600918 pokeaditto_base-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      336 2024-04-24 16:17:38.000000 pokeaditto_base-1.0.0/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2024-04-26 00:25:47.347252 Pokeaditto_base-1.0.1/
+-rw-rw----   0 root         (0) everybody  (9997)      197 2024-04-26 00:25:47.335252 Pokeaditto_base-1.0.1/PKG-INFO
+drwxrwx---   0 root         (0) everybody  (9997)        0 2024-04-26 00:25:47.291252 Pokeaditto_base-1.0.1/Pokeaditto_base.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      197 2024-04-26 00:25:47.000000 Pokeaditto_base-1.0.1/Pokeaditto_base.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      262 2024-04-26 00:25:47.000000 Pokeaditto_base-1.0.1/Pokeaditto_base.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2024-04-26 00:25:47.000000 Pokeaditto_base-1.0.1/Pokeaditto_base.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        7 2024-04-26 00:25:47.000000 Pokeaditto_base-1.0.1/Pokeaditto_base.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       10 2024-04-26 00:25:47.000000 Pokeaditto_base-1.0.1/Pokeaditto_base.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)      121 2024-04-24 16:17:38.000000 Pokeaditto_base-1.0.1/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2024-04-26 00:25:47.319252 Pokeaditto_base-1.0.1/pokeditto/
+-rw-rw----   0 root         (0) everybody  (9997)       42 2024-04-25 23:11:45.000000 Pokeaditto_base-1.0.1/pokeditto/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3438 2024-04-24 15:20:01.000000 Pokeaditto_base-1.0.1/pokeditto/random_pokemon.py
+-rw-rw----   0 root         (0) everybody  (9997)       38 2024-04-26 00:25:47.347252 Pokeaditto_base-1.0.1/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      336 2024-04-25 23:10:00.000000 Pokeaditto_base-1.0.1/setup.py
```

