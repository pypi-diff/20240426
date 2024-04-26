# Comparing `tmp/argusex1-1.0.4.tar.gz` & `tmp/argusex1-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argusex1-1.0.4.tar", last modified: Wed Apr 24 18:51:34 2024, max compression
+gzip compressed data, was "argusex1-2.0.2.tar", last modified: Fri Apr 26 04:19:50 2024, max compression
```

## Comparing `argusex1-1.0.4.tar` & `argusex1-2.0.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 18:51:34.984072 argusex1-1.0.4/
-drwxrwxrwx   0        0        0        0 2024-04-24 18:51:34.967758 argusex1-1.0.4/ArgusEX1/
--rw-rw-rw-   0        0        0    44028 2024-04-16 17:13:40.000000 argusex1-1.0.4/ArgusEX1/Poc.csv
--rw-rw-rw-   0        0        0       43 2024-04-24 18:51:28.000000 argusex1-1.0.4/ArgusEX1/__inti__.py
--rw-rw-rw-   0        0        0     2116 2024-04-24 16:18:34.000000 argusex1-1.0.4/ArgusEX1/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-04-24 18:51:34.980915 argusex1-1.0.4/ArgusEX1.egg-info/
--rw-rw-rw-   0        0        0      187 2024-04-24 18:51:34.000000 argusex1-1.0.4/ArgusEX1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-04-24 18:51:34.000000 argusex1-1.0.4/ArgusEX1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 18:51:34.000000 argusex1-1.0.4/ArgusEX1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 18:51:34.000000 argusex1-1.0.4/ArgusEX1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-24 18:51:34.000000 argusex1-1.0.4/ArgusEX1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      187 2024-04-24 18:51:34.981909 argusex1-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      148 2024-04-23 18:31:59.000000 argusex1-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 18:51:34.984072 argusex1-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      368 2024-04-24 18:50:18.000000 argusex1-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 04:19:50.773756 argusex1-2.0.2/
+drwxrwxrwx   0        0        0        0 2024-04-26 04:19:50.758082 argusex1-2.0.2/ArgusEX1/
+-rw-rw-rw-   0        0        0       41 2024-04-26 04:16:59.000000 argusex1-2.0.2/ArgusEX1/__inti__.py
+-rw-rw-rw-   0        0        0     2055 2024-04-26 04:13:44.000000 argusex1-2.0.2/ArgusEX1/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-26 04:19:50.770683 argusex1-2.0.2/ArgusEX1.egg-info/
+-rw-rw-rw-   0        0        0      187 2024-04-26 04:19:50.000000 argusex1-2.0.2/ArgusEX1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-04-26 04:19:50.000000 argusex1-2.0.2/ArgusEX1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 04:19:50.000000 argusex1-2.0.2/ArgusEX1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-26 04:19:50.000000 argusex1-2.0.2/ArgusEX1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-26 04:19:50.000000 argusex1-2.0.2/ArgusEX1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      187 2024-04-26 04:19:50.772715 argusex1-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2024-04-26 04:16:59.000000 argusex1-2.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 04:19:50.773756 argusex1-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      368 2024-04-26 04:19:39.000000 argusex1-2.0.2/setup.py
```

### Comparing `argusex1-1.0.4/ArgusEX1/random_pokemon.py` & `argusex1-2.0.2/ArgusEX1/random_pokemon.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,56 @@
 import pandas as pd
 import pkg_resources
 
 class RandomPokemon:
-      FILE_PATH = pkg_resources.resource_filename(__name__, 'Poc.csv')
+      FILE_PATH = pkg_resources.resource_filename(__name__, 'Pokem.csv')
       def __init__(self):
             self.file = pd.read_csv(self.FILE_PATH)
             self._pokemon = None
             self._number = None
             self._Name = None
             self._Type1 = None
       def generate_pokemon(self):
             self._pokemon = self.file.sample()
             self._number = self._pokemon["#"].values[0]
             self._name = self._pokemon["Name"].values[0]
             self._Type1 = self._pokemon["Type 1"].values[0]
             self._Type2 = self._pokemon["Type 2"].values[0]
-            self._Total= self._pokemon["Total"].values[0]
-            self._HP = self._pokemon["HP"].values[0]
-            self._Attack = self._pokemon["Attack"].values[0]
-            self._Defense = self._pokemon["Defense"].values[0]
-            self._Sp_Atk = self._pokemon["Sp. Atk"].values[0]
-            self._Sp_Def = self._pokemon["Sp. Def"].values[0]
-            self._Speed = self._pokemon["Speed"].values[0]
-            self._Legendary = self._pokemon["Legendary"].values[0]
-            self._Generation = self._pokemon["Generation"].values[0]
+            self._Total = self._pokemon["Total"].values[0]
+            self._hp = self._pokemon["HP"].values[0]
+            self._attack = self._pokemon["Attack"].values[0]
+            self._defense = self._pokemon["Defense"].values[0]
+            self._atsp = self._pokemon["Sp. Atk"].values[0]
+            self._dfsp = self._pokemon["Sp. Def"].values[0]
+            self._sp = self._pokemon["Speed"].values[0]
+            self._generacion = self._pokemon["Generation"].values[0]
+            self._legend = self._pokemon["Legendary"].values[0]
 
       def get_pokemon(self):
             return self._pokemon
       def get_number(self):
             return self._number
       def get_name(self):
             return self._name
       def get_Type1(self):
             return self._Type1
-
       def get_Type2(self):
-            return self._Type2
+          return self._Type2
       def get_Total(self):
-            return self._Total
-      def get_HP(self):
-            return self._HP
-      def get_Attack(self):
-            return self._Attack
-      def get_Defense(self):
-            return self._Defense
-      def get_Sp_Atk(self):
-            return self._Sp_Atk
-      def get_Sp_Def(self):
-            return self._Sp_Def
-      def get_Speed(self):
-            return self._Speed
-      def get_Legendary(self):
-            return self._Legendary
-      def get_Generation(self):
-            return self._Generation
-
-
-
-
-
-
+          return self._Total
+      def get_hp(self):
+          return self._hp
+      def get_attack(self):
+          return self._attack
+      def get_defense(self):
+          return self._defense
+      def get_atsp(self):
+          return self._atsp
+      def get_dfsp(self):
+          return self._dfsp
+      def get_sp(self):
+          return self._sp
+      def get_generacion(self):
+          return self._generacion
+      def get_legend(self):
+          return self._legend
```

