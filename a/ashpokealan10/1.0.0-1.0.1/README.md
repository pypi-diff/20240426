# Comparing `tmp/ashpokealan10-1.0.0.tar.gz` & `tmp/ashpokealan10-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ashpokealan10-1.0.0.tar", last modified: Tue Apr 23 18:27:04 2024, max compression
+gzip compressed data, was "dist\ashpokealan10-1.0.1.tar", last modified: Fri Apr 26 03:09:44 2024, max compression
```

## Comparing `ashpokealan10-1.0.0.tar` & `ashpokealan10-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 18:27:04.000000 ashpokealan10-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:27:04.000000 ashpokealan10-1.0.0/ashpokealan10/
--rw-rw-rw-   0        0        0    44829 2024-04-18 06:24:35.000000 ashpokealan10-1.0.0/ashpokealan10/pokemon.csv
--rw-rw-rw-   0        0        0     2041 2024-04-23 15:15:52.000000 ashpokealan10-1.0.0/ashpokealan10/random_pokemon.py
--rw-rw-rw-   0        0        0       41 2024-04-19 15:35:37.000000 ashpokealan10-1.0.0/ashpokealan10/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:27:04.000000 ashpokealan10-1.0.0/ashpokealan10.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-23 18:27:03.000000 ashpokealan10-1.0.0/ashpokealan10.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      242 2024-04-23 18:27:03.000000 ashpokealan10-1.0.0/ashpokealan10.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        7 2024-04-23 18:27:03.000000 ashpokealan10-1.0.0/ashpokealan10.egg-info/requires.txt
--rw-rw-rw-   0        0        0      286 2024-04-23 18:27:03.000000 ashpokealan10-1.0.0/ashpokealan10.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       14 2024-04-23 18:27:03.000000 ashpokealan10-1.0.0/ashpokealan10.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      242 2024-04-23 18:27:04.000000 ashpokealan10-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      107 2024-04-23 15:17:10.000000 ashpokealan10-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 18:27:04.000000 ashpokealan10-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      375 2024-04-19 15:49:08.000000 ashpokealan10-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:09:44.000000 ashpokealan10-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-04-26 03:09:44.000000 ashpokealan10-1.0.1/ashpokealan10/
+-rw-rw-rw-   0        0        0      643 2024-04-26 02:56:06.000000 ashpokealan10-1.0.1/ashpokealan10/alan.py
+-rw-rw-rw-   0        0        0    44829 2024-04-18 06:24:35.000000 ashpokealan10-1.0.1/ashpokealan10/pokemon.csv
+-rw-rw-rw-   0        0        0     2043 2024-04-26 03:02:18.000000 ashpokealan10-1.0.1/ashpokealan10/random_pokemon.py
+-rw-rw-rw-   0        0        0       41 2024-04-19 15:35:37.000000 ashpokealan10-1.0.1/ashpokealan10/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:09:44.000000 ashpokealan10-1.0.1/ashpokealan10.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-26 03:09:44.000000 ashpokealan10-1.0.1/ashpokealan10.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      251 2024-04-26 03:09:44.000000 ashpokealan10-1.0.1/ashpokealan10.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2024-04-26 03:09:44.000000 ashpokealan10-1.0.1/ashpokealan10.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      308 2024-04-26 03:09:44.000000 ashpokealan10-1.0.1/ashpokealan10.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       14 2024-04-26 03:09:44.000000 ashpokealan10-1.0.1/ashpokealan10.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      251 2024-04-26 03:09:44.000000 ashpokealan10-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2024-04-23 15:17:10.000000 ashpokealan10-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 03:09:44.000000 ashpokealan10-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      386 2024-04-26 03:09:07.000000 ashpokealan10-1.0.1/setup.py
```

### Comparing `ashpokealan10-1.0.0/ashpokealan10/pokemon.csv` & `ashpokealan10-1.0.1/ashpokealan10/pokemon.csv`

 * *Files identical despite different names*

### Comparing `ashpokealan10-1.0.0/ashpokealan10/random_pokemon.py` & `ashpokealan10-1.0.1/ashpokealan10/random_pokemon.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pkg_resources
 
 
 class RandomPokemon:
     FILE_PATH = pkg_resources.resource_filename(__name__, "pokemon.csv")
 
     # Constructor
-    def _init_(self):
+    def __init__(self):
         self._file = pd.read_csv(self.FILE_PATH)  # se lee el archivo pandas
         self._number = None
         self._name = None
         self._type1 = None
         self._pokemon = None
 
     def generate_random(self):
```

