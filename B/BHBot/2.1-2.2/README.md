# Comparing `tmp/bhbot-2.1.tar.gz` & `tmp/bhbot-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhbot-2.1.tar", last modified: Thu Apr 18 20:34:05 2024, max compression
+gzip compressed data, was "bhbot-2.2.tar", last modified: Fri Apr 26 19:39:00 2024, max compression
```

## Comparing `bhbot-2.1.tar` & `bhbot-2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:34:05.735477 bhbot-2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:34:05.731477 bhbot-2.1/BHBot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-18 20:34:05.000000 bhbot-2.1/BHBot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 20:34:05.000000 bhbot-2.1/BHBot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:34:05.000000 bhbot-2.1/BHBot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:34:05.000000 bhbot-2.1/BHBot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-18 20:34:01.000000 bhbot-2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-18 20:34:05.735477 bhbot-2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-18 20:34:01.000000 bhbot-2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-18 20:34:01.000000 bhbot-2.1/abstract_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    20821 2024-04-18 20:34:01.000000 bhbot-2.1/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-18 20:34:01.000000 bhbot-2.1/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-18 20:34:01.000000 bhbot-2.1/client_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-04-18 20:34:01.000000 bhbot-2.1/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-18 20:34:01.000000 bhbot-2.1/direct_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-18 20:34:01.000000 bhbot-2.1/font_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9706 2024-04-18 20:34:01.000000 bhbot-2.1/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-18 20:34:01.000000 bhbot-2.1/levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-18 20:34:01.000000 bhbot-2.1/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 20:34:01.000000 bhbot-2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:34:05.735477 bhbot-2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-18 20:34:01.000000 bhbot-2.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 20:34:01.000000 bhbot-2.1/test_pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-04-18 20:34:01.000000 bhbot-2.1/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-18 20:34:01.000000 bhbot-2.1/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:39:00.511493 bhbot-2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:39:00.511493 bhbot-2.2/BHBot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-26 19:39:00.000000 bhbot-2.2/BHBot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-26 19:39:00.000000 bhbot-2.2/BHBot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:39:00.000000 bhbot-2.2/BHBot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:39:00.000000 bhbot-2.2/BHBot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-26 19:38:56.000000 bhbot-2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-26 19:39:00.511493 bhbot-2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-26 19:38:56.000000 bhbot-2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-26 19:38:56.000000 bhbot-2.2/abstract_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20821 2024-04-26 19:38:56.000000 bhbot-2.2/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-26 19:38:56.000000 bhbot-2.2/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-26 19:38:56.000000 bhbot-2.2/client_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-04-26 19:38:56.000000 bhbot-2.2/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-26 19:38:56.000000 bhbot-2.2/direct_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-26 19:38:56.000000 bhbot-2.2/font_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9706 2024-04-26 19:38:56.000000 bhbot-2.2/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-26 19:38:56.000000 bhbot-2.2/levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-26 19:38:56.000000 bhbot-2.2/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-26 19:38:56.000000 bhbot-2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:39:00.511493 bhbot-2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-26 19:38:56.000000 bhbot-2.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-26 19:38:56.000000 bhbot-2.2/test_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-04-26 19:38:56.000000 bhbot-2.2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-26 19:38:56.000000 bhbot-2.2/windows.py
```

### Comparing `bhbot-2.1/BHBot.egg-info/PKG-INFO` & `bhbot-2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: BHBot
-Version: 2.1
-Home-page: https://github.com/Nick2bad4u/BHBot
-Author: Nick
-Author-email: 
-License: Unlicense
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # BHBot
 
 [Этот файл доступен на Русском языке](README_RU.md)
 
 Gold/XP farming bot for Brawlhalla
 
 Heavily inspired by [BrawlhallaEZ](https://github.com/jamunano/BrawlhallaEZ)
@@ -54,8 +44,8 @@
 - Bot requires "Collapse crossovers" to be set to Yes. If you think it should automatically set it to be so, please [open an issue](https://github.com/nick2bad4u/bhbot/issues)
 - Bot requires ingame language to be set to English. If you think it should automatically set it to be so, please [open an issue](https://github.com/nick2bad4u/bhbot/issues)
 
 # Technical Overview
 - The underlying code is always available for review by anyone.
 - Essentially, the bot employs the Windows SendMessage API to transmit inputs directly to the Brawlhalla window. It utilizes pixel detection to discern states and determine the appropriate action at any given moment.
 
-- The BrawlhallaBot class can be utilized directly or you may develop a custom wrapper for it. It is designed to operate independently, with gui.py serving merely as a graphical wrapper using PySimpleGUI.
+- The BrawlhallaBot class can be utilized directly or you may develop a custom wrapper for it. It is designed to operate independently, with gui.py serving merely as a graphical wrapper using PySimpleGUI<img src="https://www.google-analytics.com/collect?v=2&tid=G-6RR5ZF4BJV&cid=555&t=event&en=eventName">
```

### Comparing `bhbot-2.1/LICENSE` & `bhbot-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bhbot-2.1/PKG-INFO` & `bhbot-2.2/BHBot.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BHBot
-Version: 2.1
+Version: 2.2
 Home-page: https://github.com/Nick2bad4u/BHBot
 Author: Nick
 Author-email: 
 License: Unlicense
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -54,8 +54,8 @@
 - Bot requires "Collapse crossovers" to be set to Yes. If you think it should automatically set it to be so, please [open an issue](https://github.com/nick2bad4u/bhbot/issues)
 - Bot requires ingame language to be set to English. If you think it should automatically set it to be so, please [open an issue](https://github.com/nick2bad4u/bhbot/issues)
 
 # Technical Overview
 - The underlying code is always available for review by anyone.
 - Essentially, the bot employs the Windows SendMessage API to transmit inputs directly to the Brawlhalla window. It utilizes pixel detection to discern states and determine the appropriate action at any given moment.
 
-- The BrawlhallaBot class can be utilized directly or you may develop a custom wrapper for it. It is designed to operate independently, with gui.py serving merely as a graphical wrapper using PySimpleGUI.
+- The BrawlhallaBot class can be utilized directly or you may develop a custom wrapper for it. It is designed to operate independently, with gui.py serving merely as a graphical wrapper using PySimpleGUI<img src="https://www.google-analytics.com/collect?v=2&tid=G-6RR5ZF4BJV&cid=555&t=event&en=eventName">
```

### Comparing `bhbot-2.1/README.md` & `bhbot-2.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: BHBot
+Version: 2.2
+Home-page: https://github.com/Nick2bad4u/BHBot
+Author: Nick
+Author-email: 
+License: Unlicense
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # BHBot
 
 [Этот файл доступен на Русском языке](README_RU.md)
 
 Gold/XP farming bot for Brawlhalla
 
 Heavily inspired by [BrawlhallaEZ](https://github.com/jamunano/BrawlhallaEZ)
@@ -44,8 +54,8 @@
 - Bot requires "Collapse crossovers" to be set to Yes. If you think it should automatically set it to be so, please [open an issue](https://github.com/nick2bad4u/bhbot/issues)
 - Bot requires ingame language to be set to English. If you think it should automatically set it to be so, please [open an issue](https://github.com/nick2bad4u/bhbot/issues)
 
 # Technical Overview
 - The underlying code is always available for review by anyone.
 - Essentially, the bot employs the Windows SendMessage API to transmit inputs directly to the Brawlhalla window. It utilizes pixel detection to discern states and determine the appropriate action at any given moment.
 
-- The BrawlhallaBot class can be utilized directly or you may develop a custom wrapper for it. It is designed to operate independently, with gui.py serving merely as a graphical wrapper using PySimpleGUI.
+- The BrawlhallaBot class can be utilized directly or you may develop a custom wrapper for it. It is designed to operate independently, with gui.py serving merely as a graphical wrapper using PySimpleGUI<img src="https://www.google-analytics.com/collect?v=2&tid=G-6RR5ZF4BJV&cid=555&t=event&en=eventName">
```

### Comparing `bhbot-2.1/abstract_mode.py` & `bhbot-2.2/abstract_mode.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.1/bot.py` & `bhbot-2.2/bot.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.1/characters.py` & `bhbot-2.2/characters.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.1/config.py` & `bhbot-2.2/config.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.1/direct_input.py` & `bhbot-2.2/direct_input.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.1/font_loader.py` & `bhbot-2.2/font_loader.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.1/gui.py` & `bhbot-2.2/gui.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.1/levels.py` & `bhbot-2.2/levels.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.1/menu.py` & `bhbot-2.2/menu.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.1/utils.py` & `bhbot-2.2/utils.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.1/windows.py` & `bhbot-2.2/windows.py`

 * *Files identical despite different names*

