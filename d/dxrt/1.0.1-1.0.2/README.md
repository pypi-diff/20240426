# Comparing `tmp/dxrt-1.0.1.tar.gz` & `tmp/dxrt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxrt-1.0.1.tar", last modified: Thu Apr 25 16:24:22 2024, max compression
+gzip compressed data, was "dxrt-1.0.2.tar", last modified: Thu Apr 25 19:20:01 2024, max compression
```

## Comparing `dxrt-1.0.1.tar` & `dxrt-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 16:24:22.532333 dxrt-1.0.1/
--rw-rw-rw-   0        0        0      182 2024-04-25 16:24:22.530918 dxrt-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      121 2024-04-19 15:57:17.000000 dxrt-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 16:24:22.516220 dxrt-1.0.1/dxrt/
--rw-rw-rw-   0        0        0       42 2024-04-19 15:57:12.000000 dxrt-1.0.1/dxrt/__init__.py
--rw-rw-rw-   0        0        0    44028 2024-04-16 17:45:56.000000 dxrt-1.0.1/dxrt/pokemon.csv
--rw-rw-rw-   0        0        0     2127 2024-04-19 15:57:10.000000 dxrt-1.0.1/dxrt/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-04-25 16:24:22.528901 dxrt-1.0.1/dxrt.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-25 16:24:22.000000 dxrt-1.0.1/dxrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-04-25 16:24:22.000000 dxrt-1.0.1/dxrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 16:24:22.000000 dxrt-1.0.1/dxrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-25 16:24:22.000000 dxrt-1.0.1/dxrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-25 16:24:22.000000 dxrt-1.0.1/dxrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 16:24:22.533347 dxrt-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      332 2024-04-25 16:24:16.000000 dxrt-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:20:01.090793 dxrt-1.0.2/
+-rw-rw-rw-   0        0        0      182 2024-04-25 19:20:01.089334 dxrt-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      121 2024-04-19 15:57:17.000000 dxrt-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 19:20:01.074210 dxrt-1.0.2/dxrt/
+-rw-rw-rw-   0        0        0       42 2024-04-19 15:57:12.000000 dxrt-1.0.2/dxrt/__init__.py
+-rw-rw-rw-   0        0        0     1999 2024-04-25 19:09:22.000000 dxrt-1.0.2/dxrt/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:20:01.087081 dxrt-1.0.2/dxrt.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-25 19:20:00.000000 dxrt-1.0.2/dxrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-25 19:20:00.000000 dxrt-1.0.2/dxrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 19:20:00.000000 dxrt-1.0.2/dxrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-25 19:20:00.000000 dxrt-1.0.2/dxrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-25 19:20:00.000000 dxrt-1.0.2/dxrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 19:20:01.090793 dxrt-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      332 2024-04-25 19:15:12.000000 dxrt-1.0.2/setup.py
```

### Comparing `dxrt-1.0.1/dxrt/random_pokemon.py` & `dxrt-1.0.2/dxrt/random_pokemon.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,13 +78,7 @@
   	
   def getGeneration(self):
   	return self._generation
   	
   def getLegendary(self):
   	return self._legendary
   	
-#Probando la clase 
-pokemon = RandomPokemon()
-pokemon.generate_random()
-
-print(pokemon.getPokemon())
-print( pokemon.getName())
```

