# Comparing `tmp/pokerkit-0.5.0a0.tar.gz` & `tmp/pokerkit-0.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerkit-0.5.0a0.tar", last modified: Tue Apr 23 17:56:31 2024, max compression
+gzip compressed data, was "pokerkit-0.5.0a1.tar", last modified: Wed Apr 24 16:36:22 2024, max compression
```

## Comparing `pokerkit-0.5.0a0.tar` & `pokerkit-0.5.0a1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-23 17:56:31.690392 pokerkit-0.5.0a0/
--rw-rw-r--   0 juho      (1000) juho      (1000)     1116 2024-04-11 09:02:36.000000 pokerkit-0.5.0a0/LICENSE
--rw-r--r--   0 juho      (1000) juho      (1000)    17204 2024-04-23 17:56:31.690392 pokerkit-0.5.0a0/PKG-INFO
--rw-rw-r--   0 juho      (1000) juho      (1000)    15530 2024-04-23 17:49:32.000000 pokerkit-0.5.0a0/README.rst
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-23 17:56:31.686392 pokerkit-0.5.0a0/pokerkit/
--rw-rw-r--   0 juho      (1000) juho      (1000)     4460 2024-04-20 15:21:12.000000 pokerkit-0.5.0a0/pokerkit/__init__.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    15073 2024-04-09 08:26:29.000000 pokerkit-0.5.0a0/pokerkit/analysis.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    74102 2024-04-23 17:26:14.000000 pokerkit-0.5.0a0/pokerkit/games.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    21443 2024-04-09 09:11:40.000000 pokerkit-0.5.0a0/pokerkit/hands.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    15305 2024-04-09 09:11:43.000000 pokerkit-0.5.0a0/pokerkit/lookups.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    28717 2024-04-09 08:58:34.000000 pokerkit-0.5.0a0/pokerkit/notation.py
--rw-rw-r--   0 juho      (1000) juho      (1000)        0 2024-03-03 02:45:25.000000 pokerkit-0.5.0a0/pokerkit/py.typed
--rw-rw-r--   0 juho      (1000) juho      (1000)   194299 2024-04-23 17:00:45.000000 pokerkit-0.5.0a0/pokerkit/state.py
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-23 17:56:31.690392 pokerkit-0.5.0a0/pokerkit/tests/
--rw-rw-r--   0 juho      (1000) juho      (1000)       88 2024-03-03 02:45:25.000000 pokerkit-0.5.0a0/pokerkit/tests/__init__.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    17128 2024-03-25 16:57:08.000000 pokerkit-0.5.0a0/pokerkit/tests/test_analysis.py
--rw-rw-r--   0 juho      (1000) juho      (1000)     6485 2024-04-23 17:51:34.000000 pokerkit-0.5.0a0/pokerkit/tests/test_games.py
--rw-rw-r--   0 juho      (1000) juho      (1000)     5331 2024-03-15 11:23:34.000000 pokerkit-0.5.0a0/pokerkit/tests/test_lookups.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    28167 2024-03-29 06:34:10.000000 pokerkit-0.5.0a0/pokerkit/tests/test_notation.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    35725 2024-04-23 17:51:05.000000 pokerkit-0.5.0a0/pokerkit/tests/test_papers.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    37676 2024-04-23 14:37:55.000000 pokerkit-0.5.0a0/pokerkit/tests/test_state.py
--rw-rw-r--   0 juho      (1000) juho      (1000)     2062 2024-04-23 17:51:13.000000 pokerkit-0.5.0a0/pokerkit/tests/test_utilities.py
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-23 17:56:31.690392 pokerkit-0.5.0a0/pokerkit/tests/test_wsop/
--rw-rw-r--   0 juho      (1000) juho      (1000)      141 2024-03-03 02:45:25.000000 pokerkit-0.5.0a0/pokerkit/tests/test_wsop/__init__.py
--rw-rw-r--   0 juho      (1000) juho      (1000)   193298 2024-04-16 23:01:37.000000 pokerkit-0.5.0a0/pokerkit/tests/test_wsop/test_2023_43_5.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    32968 2024-04-23 17:38:59.000000 pokerkit-0.5.0a0/pokerkit/tests/test_wsop/test_2023_54_4.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    18574 2024-04-10 07:51:29.000000 pokerkit-0.5.0a0/pokerkit/utilities.py
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-23 17:56:31.690392 pokerkit-0.5.0a0/pokerkit.egg-info/
--rw-r--r--   0 juho      (1000) juho      (1000)    17204 2024-04-23 17:56:31.000000 pokerkit-0.5.0a0/pokerkit.egg-info/PKG-INFO
--rw-rw-r--   0 juho      (1000) juho      (1000)      698 2024-04-23 17:56:31.000000 pokerkit-0.5.0a0/pokerkit.egg-info/SOURCES.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)        1 2024-04-23 17:56:31.000000 pokerkit-0.5.0a0/pokerkit.egg-info/dependency_links.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)        9 2024-04-23 17:56:31.000000 pokerkit-0.5.0a0/pokerkit.egg-info/top_level.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)       38 2024-04-23 17:56:31.690392 pokerkit-0.5.0a0/setup.cfg
--rw-rw-r--   0 juho      (1000) juho      (1000)     2143 2024-04-23 17:55:18.000000 pokerkit-0.5.0a0/setup.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-24 16:36:22.334641 pokerkit-0.5.0a1/
+-rw-rw-r--   0 juho      (1000) juho      (1000)     1116 2024-04-11 09:02:36.000000 pokerkit-0.5.0a1/LICENSE
+-rw-r--r--   0 juho      (1000) juho      (1000)    17204 2024-04-24 16:36:22.334641 pokerkit-0.5.0a1/PKG-INFO
+-rw-rw-r--   0 juho      (1000) juho      (1000)    15530 2024-04-23 17:49:32.000000 pokerkit-0.5.0a1/README.rst
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-24 16:36:22.334641 pokerkit-0.5.0a1/pokerkit/
+-rw-rw-r--   0 juho      (1000) juho      (1000)     4460 2024-04-20 15:21:12.000000 pokerkit-0.5.0a1/pokerkit/__init__.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    15073 2024-04-09 08:26:29.000000 pokerkit-0.5.0a1/pokerkit/analysis.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    73909 2024-04-24 16:25:13.000000 pokerkit-0.5.0a1/pokerkit/games.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    21443 2024-04-09 09:11:40.000000 pokerkit-0.5.0a1/pokerkit/hands.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    15305 2024-04-09 09:11:43.000000 pokerkit-0.5.0a1/pokerkit/lookups.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    28717 2024-04-09 08:58:34.000000 pokerkit-0.5.0a1/pokerkit/notation.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)        0 2024-03-03 02:45:25.000000 pokerkit-0.5.0a1/pokerkit/py.typed
+-rw-rw-r--   0 juho      (1000) juho      (1000)   195732 2024-04-24 16:33:47.000000 pokerkit-0.5.0a1/pokerkit/state.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-24 16:36:22.334641 pokerkit-0.5.0a1/pokerkit/tests/
+-rw-rw-r--   0 juho      (1000) juho      (1000)       88 2024-03-03 02:45:25.000000 pokerkit-0.5.0a1/pokerkit/tests/__init__.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    17128 2024-03-25 16:57:08.000000 pokerkit-0.5.0a1/pokerkit/tests/test_analysis.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)     6485 2024-04-23 17:51:34.000000 pokerkit-0.5.0a1/pokerkit/tests/test_games.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)     5331 2024-03-15 11:23:34.000000 pokerkit-0.5.0a1/pokerkit/tests/test_lookups.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    28167 2024-03-29 06:34:10.000000 pokerkit-0.5.0a1/pokerkit/tests/test_notation.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    35725 2024-04-23 17:51:05.000000 pokerkit-0.5.0a1/pokerkit/tests/test_papers.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    39414 2024-04-24 16:31:51.000000 pokerkit-0.5.0a1/pokerkit/tests/test_state.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)     2062 2024-04-23 17:51:13.000000 pokerkit-0.5.0a1/pokerkit/tests/test_utilities.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-24 16:36:22.334641 pokerkit-0.5.0a1/pokerkit/tests/test_wsop/
+-rw-rw-r--   0 juho      (1000) juho      (1000)      141 2024-03-03 02:45:25.000000 pokerkit-0.5.0a1/pokerkit/tests/test_wsop/__init__.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)   193298 2024-04-16 23:01:37.000000 pokerkit-0.5.0a1/pokerkit/tests/test_wsop/test_2023_43_5.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    32968 2024-04-23 17:38:59.000000 pokerkit-0.5.0a1/pokerkit/tests/test_wsop/test_2023_54_4.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    20720 2024-04-24 16:31:35.000000 pokerkit-0.5.0a1/pokerkit/utilities.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-24 16:36:22.334641 pokerkit-0.5.0a1/pokerkit.egg-info/
+-rw-r--r--   0 juho      (1000) juho      (1000)    17204 2024-04-24 16:36:22.000000 pokerkit-0.5.0a1/pokerkit.egg-info/PKG-INFO
+-rw-rw-r--   0 juho      (1000) juho      (1000)      698 2024-04-24 16:36:22.000000 pokerkit-0.5.0a1/pokerkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)        1 2024-04-24 16:36:22.000000 pokerkit-0.5.0a1/pokerkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)        9 2024-04-24 16:36:22.000000 pokerkit-0.5.0a1/pokerkit.egg-info/top_level.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)       38 2024-04-24 16:36:22.334641 pokerkit-0.5.0a1/setup.cfg
+-rw-rw-r--   0 juho      (1000) juho      (1000)     2143 2024-04-24 16:33:25.000000 pokerkit-0.5.0a1/setup.py
```

### Comparing `pokerkit-0.5.0a0/LICENSE` & `pokerkit-0.5.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a0/PKG-INFO` & `pokerkit-0.5.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerkit
-Version: 0.5.0a0
+Version: 0.5.0a1
 Summary: An open-source Python library for poker game simulations, hand evaluations, and statistical analysis
 Home-page: https://github.com/uoftcprg/pokerkit
 Author: University of Toronto Computer Poker Student Research Group
 Author-email: uoftcprg@studentorg.utoronto.ca
 License: MIT
 Project-URL: Documentation, https://pokerkit.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/uoftcprg/pokerkit
```

### Comparing `pokerkit-0.5.0a0/README.rst` & `pokerkit-0.5.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a0/pokerkit/__init__.py` & `pokerkit-0.5.0a1/pokerkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a0/pokerkit/analysis.py` & `pokerkit-0.5.0a1/pokerkit/analysis.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a0/pokerkit/games.py` & `pokerkit-0.5.0a1/pokerkit/games.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 tons of parameters to be specified.
 """
 
 from __future__ import annotations
 
 from abc import ABC
 from collections.abc import Callable
-from functools import partial
 from typing import ClassVar
 
 from pokerkit.hands import (
     BadugiHand,
     EightOrBetterLowHand,
     Hand,
     OmahaEightOrBetterLowHand,
@@ -85,15 +84,15 @@
             raw_antes: ValuesLike,
             raw_blinds_or_straddles: ValuesLike,
             bring_in: int,
             *,
             mode: Mode = Mode.TOURNAMENT,
             starting_board_count: int = 1,
             divmod: Callable[[int, int], tuple[int, int]] = divmod,
-            rake: Callable[[int], tuple[int, int]] = partial(rake, rake=0),
+            rake: Callable[[int, State], tuple[int, int]] = rake,
     ) -> None:
         self.automations: tuple[Automation, ...] = automations
         """The automations.
 
         Allows the user to specify what steps they do not care about and
         therefore should be automatically handled by PokerKit.
         """
@@ -156,15 +155,15 @@
         """
         self.divmod: Callable[[int, int], tuple[int, int]] = divmod
         """The divmod function.
 
         This is used to denote how pots are divided up (for multiple
         boards, multiple winners, multiple hand types, etc.).
         """
-        self.rake: Callable[[int], tuple[int, int]] = rake
+        self.rake: Callable[[int, State], tuple[int, int]] = rake
         """The rake function.
 
         Rake functions are used in PokerKit to denote how the rakes are
         collected from the pot. Multiple pots may exist (side-pots) in
         which case the method is called for each pot.
         """
 
@@ -419,15 +418,15 @@
             raw_blinds_or_straddles: ValuesLike,
             small_bet: int,
             big_bet: int,
             *,
             mode: Mode = Mode.TOURNAMENT,
             starting_board_count: int = 1,
             divmod: Callable[[int, int], tuple[int, int]] = divmod,
-            rake: Callable[[int], tuple[int, int]] = partial(rake, rake=0),
+            rake: Callable[[int, State], tuple[int, int]] = rake,
     ) -> None:
         super().__init__(
             automations,
             (
                 Street(
                     False,
                     (False,) * self.hole_dealing_count,
@@ -499,15 +498,15 @@
             raw_antes: ValuesLike,
             raw_blinds_or_straddles: ValuesLike,
             min_bet: int,
             *,
             mode: Mode = Mode.TOURNAMENT,
             starting_board_count: int = 1,
             divmod: Callable[[int, int], tuple[int, int]] = divmod,
-            rake: Callable[[int], tuple[int, int]] = partial(rake, rake=0),
+            rake: Callable[[int, State], tuple[int, int]] = rake,
     ) -> None:
         super().__init__(
             automations,
             ante_trimming_status,
             raw_antes,
             raw_blinds_or_straddles,
             min_bet,
@@ -541,15 +540,15 @@
             big_bet: int,
             raw_starting_stacks: ValuesLike,
             player_count: int,
             *,
             mode: Mode = Mode.TOURNAMENT,
             starting_board_count: int = 1,
             divmod: Callable[[int, int], tuple[int, int]] = divmod,
-            rake: Callable[[int], tuple[int, int]] = partial(rake, rake=0),
+            rake: Callable[[int, State], tuple[int, int]] = rake,
     ) -> State:
         """Create a fixed-limit Texas hold'em game.
 
         Below is an example hand in fixed-limit Texas hold'em.
 
         >>> state = FixedLimitTexasHoldem.create_state(
         ...     (
@@ -635,15 +634,15 @@
             min_bet: int,
             raw_starting_stacks: ValuesLike,
             player_count: int,
             *,
             mode: Mode = Mode.TOURNAMENT,
             starting_board_count: int = 1,
             divmod: Callable[[int, int], tuple[int, int]] = divmod,
-            rake: Callable[[int], tuple[int, int]] = partial(rake, rake=0),
+            rake: Callable[[int, State], tuple[int, int]] = rake,
     ) -> State:
         """Create a no-limit Texas hold'em game.
 
         Below shows the 4-runout hand between Phil Hellmuth and the
         Loose Cannon Ernest Wiggins.
 
         Link: https://youtu.be/cnjJv7x0HMY?si=4l05Ez7lQVczt8DI&t=638
@@ -914,15 +913,15 @@
             min_bet: int,
             raw_starting_stacks: ValuesLike,
             player_count: int,
             *,
             mode: Mode = Mode.TOURNAMENT,
             starting_board_count: int = 1,
             divmod: Callable[[int, int], tuple[int, int]] = divmod,
-            rake: Callable[[int], tuple[int, int]] = partial(rake, rake=0),
+            rake: Callable[[int, State], tuple[int, int]] = rake,
     ) -> State:
         """Create a no-limit short-deck hold'em game.
 
         Below shows an all-in hand between Xuan and Phua.
 
         Link: https://youtu.be/QlgCcphLjaQ
 
@@ -1058,15 +1057,15 @@
             min_bet: int,
             raw_starting_stacks: ValuesLike,
             player_count: int,
             *,
             mode: Mode = Mode.TOURNAMENT,
             starting_board_count: int = 1,
             divmod: Callable[[int, int], tuple[int, int]] = divmod,
-            rake: Callable[[int], tuple[int, int]] = partial(rake, rake=0),
+            rake: Callable[[int, State], tuple[int, int]] = rake,
     ) -> State:
         """Create a pot-limit Omaha hold'em game.
 
         Below shows the largest online poker pot every played between
         Patrik Antonius and Viktor Blom.
 
         Link: https://youtu.be/UMBm66Id2AA
@@ -1203,15 +1202,15 @@
             big_bet: int,
             raw_starting_stacks: ValuesLike,
             player_count: int,
             *,
             mode: Mode = Mode.TOURNAMENT,
             starting_board_count: int = 1,
             divmod: Callable[[int, int], tuple[int, int]] = divmod,
-            rake: Callable[[int], tuple[int, int]] = partial(rake, rake=0),
+            rake: Callable[[int, State], tuple[int, int]] = rake,
     ) -> State:
         """Create a fixed-limit Omaha hold'em high/low-split eight or better
         low game.
 
         :param automations: The automations.
         :param ante_trimming_status: The ante trimming status.
         :param raw_antes: The "raw" antes.
@@ -1268,15 +1267,15 @@
             bring_in: int,
             small_bet: int,
             big_bet: int,
             *,
             mode: Mode = Mode.TOURNAMENT,
             starting_board_count: int = 1,
             divmod: Callable[[int, int], tuple[int, int]] = divmod,
-            rake: Callable[[int], tuple[int, int]] = partial(rake, rake=0),
+            rake: Callable[[int, State], tuple[int, int]] = rake,
     ) -> None:
         super().__init__(
             automations,
             (
                 Street(
                     False,
                     (False, False, True),
@@ -1352,15 +1351,15 @@
             big_bet: int,
             raw_starting_stacks: ValuesLike,
             player_count: int,
             *,
             mode: Mode = Mode.TOURNAMENT,
             starting_board_count: int = 1,
             divmod: Callable[[int, int], tuple[int, int]] = divmod,
-            rake: Callable[[int], tuple[int, int]] = partial(rake, rake=0),
+            rake: Callable[[int, State], tuple[int, int]] = rake,
     ) -> State:
         """Create a fixed-limit seven card stud game.
 
         :param automations: The automations.
         :param ante_trimming_status: The ante trimming status.
         :param raw_antes: The "raw" antes.
         :param bring_in: The bring-in.
@@ -1414,15 +1413,15 @@
             big_bet: int,
             raw_starting_stacks: ValuesLike,
             player_count: int,
             *,
             mode: Mode = Mode.TOURNAMENT,
             starting_board_count: int = 1,
             divmod: Callable[[int, int], tuple[int, int]] = divmod,
-            rake: Callable[[int], tuple[int, int]] = partial(rake, rake=0),
+            rake: Callable[[int, State], tuple[int, int]] = rake,
     ) -> State:
         """Create a fixed-limit seven card stud high/low-split eight or
         better low game.
 
         :param automations: The automations.
         :param ante_trimming_status: The ante trimming status.
         :param raw_antes: The "raw" antes.
@@ -1469,15 +1468,15 @@
             big_bet: int,
             raw_starting_stacks: ValuesLike,
             player_count: int,
             *,
             mode: Mode = Mode.TOURNAMENT,
             starting_board_count: int = 1,
             divmod: Callable[[int, int], tuple[int, int]] = divmod,
-            rake: Callable[[int], tuple[int, int]] = partial(rake, rake=0),
+            rake: Callable[[int, State], tuple[int, int]] = rake,
     ) -> State:
         """Create a fixed-limit razz game.
 
         :param automations: The automations.
         :param ante_trimming_status: The ante trimming status.
         :param raw_antes: The "raw" antes.
         :param bring_in: The bring-in.
@@ -1535,15 +1534,15 @@
             raw_antes: ValuesLike,
             raw_blinds_or_straddles: ValuesLike,
             min_bet: int,
             *,
             mode: Mode = Mode.TOURNAMENT,
             starting_board_count: int = 1,
             divmod: Callable[[int, int], tuple[int, int]] = divmod,
-            rake: Callable[[int], tuple[int, int]] = partial(rake, rake=0),
+            rake: Callable[[int, State], tuple[int, int]] = rake,
     ) -> None:
         super().__init__(
             automations,
             (
                 Street(
                     False,
                     (False,) * self.hole_dealing_count,
@@ -1597,15 +1596,15 @@
             raw_blinds_or_straddles: ValuesLike,
             small_bet: int,
             big_bet: int,
             *,
             mode: Mode = Mode.TOURNAMENT,
             starting_board_count: int = 1,
             divmod: Callable[[int, int], tuple[int, int]] = divmod,
-            rake: Callable[[int], tuple[int, int]] = partial(rake, rake=0),
+            rake: Callable[[int, State], tuple[int, int]] = rake,
     ) -> None:
         super().__init__(
             automations,
             (
                 Street(
                     False,
                     (False,) * self.hole_dealing_count,
@@ -1680,15 +1679,15 @@
             min_bet: int,
             raw_starting_stacks: ValuesLike,
             player_count: int,
             *,
             mode: Mode = Mode.TOURNAMENT,
             starting_board_count: int = 1,
             divmod: Callable[[int, int], tuple[int, int]] = divmod,
-            rake: Callable[[int], tuple[int, int]] = partial(rake, rake=0),
+            rake: Callable[[int, State], tuple[int, int]] = rake,
     ) -> State:
         """Create a no-limit deuce-to-seven lowball single draw game.
 
         :param automations: The automations.
         :param ante_trimming_status: The ante trimming status.
         :param raw_antes: The "raw" antes.
         :param raw_blinds_or_straddles: The "raw" blinds or straddles.
@@ -1734,15 +1733,15 @@
             big_bet: int,
             raw_starting_stacks: ValuesLike,
             player_count: int,
             *,
             mode: Mode = Mode.TOURNAMENT,
             starting_board_count: int = 1,
             divmod: Callable[[int, int], tuple[int, int]] = divmod,
-            rake: Callable[[int], tuple[int, int]] = partial(rake, rake=0),
+            rake: Callable[[int, State], tuple[int, int]] = rake,
     ) -> State:
         """Create a fixed-limit deuce-to-seven lowball triple draw game.
 
         Below shows a bad beat between Yockey and Arieh.
 
         Link: https://youtu.be/pChCqb2FNxY
 
@@ -1886,15 +1885,15 @@
             big_bet: int,
             raw_starting_stacks: ValuesLike,
             player_count: int,
             *,
             mode: Mode = Mode.TOURNAMENT,
             starting_board_count: int = 1,
             divmod: Callable[[int, int], tuple[int, int]] = divmod,
-            rake: Callable[[int], tuple[int, int]] = partial(rake, rake=0),
+            rake: Callable[[int, State], tuple[int, int]] = rake,
     ) -> State:
         """Create a fixed-limit badugi game.
 
         Below shows an example badugi hand from Wikipedia.
 
         Link: https://en.wikipedia.org/wiki/Badugi
```

### Comparing `pokerkit-0.5.0a0/pokerkit/hands.py` & `pokerkit-0.5.0a1/pokerkit/hands.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a0/pokerkit/lookups.py` & `pokerkit-0.5.0a1/pokerkit/lookups.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a0/pokerkit/notation.py` & `pokerkit-0.5.0a1/pokerkit/notation.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a0/pokerkit/state.py` & `pokerkit-0.5.0a1/pokerkit/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """:mod:`pokerkit.state` implements classes related to poker states."""
 
+from __future__ import annotations
+
 from abc import ABC
 from collections.abc import Callable, Iterable, Iterator
 from collections import Counter, deque
 from dataclasses import InitVar, dataclass, field, KW_ONLY
 from enum import StrEnum, unique
 from functools import partial
 from itertools import chain, filterfalse, islice, starmap
 from operator import getitem, sub
 from random import shuffle
-from typing import Any
 from warnings import warn
 
 from pokerkit.hands import Hand
 from pokerkit.lookups import Label, Lookup
 from pokerkit.utilities import (
     Card,
     CardsLike,
@@ -369,40 +370,51 @@
     """The tournament poker state type."""
     CASH_GAME = 'Cash-game'
     """The cash-game poker state type."""
 
 
 @dataclass(frozen=True)
 class Pot:
-    """The class for pots.
+    """The class for pots."""
 
-    >>> pot = Pot(100, (1, 3))
-    >>> pot.amount
-    100
-    >>> pot.player_indices
-    (1, 3)
-
-    >>> pot = Pot(-1, (1, 3))
-    Traceback (most recent call last):
-        ...
-    ValueError: The pot amount -1 is negative.
+    raked_amount: int
+    """The raked amount (from the original amount
+    :attr:`pokerkit.state.Pot`).
+    """
+    unraked_amount: int
+    """The unraked amount (remaining from the original amount
+    :attr:`pokerkit.state.Pot`).
     """
-
-    amount: int
-    """The amount (unraked)."""
     player_indices: tuple[int, ...]
     """The player indices of those who are eligible to win.
 
     This means A: they contributed to this pot and B: they are still
     active (in the hand).
     """
 
     def __post_init__(self) -> None:
-        if self.amount < 0:
-            raise ValueError(f'The pot amount {self.amount} is negative.')
+        if self.raked_amount < 0:
+            raise ValueError(
+                f'The raked amount {self.raked_amount} is negative.',
+            )
+        elif self.unraked_amount < 0:
+            raise ValueError(
+                f'The unraked amount {self.unraked_amount} is negative.',
+            )
+
+    @property
+    def amount(self) -> int:
+        """Return the pot amount.
+
+        This is the sum of the portion it is raked and the remaining
+        pot.
+
+        :return: The pot amount.
+        """
+        return self.raked_amount + self.unraked_amount
 
 
 @dataclass(frozen=True)
 class Operation(ABC):
     """The abstract base class for operations."""
 
     _: KW_ONLY
@@ -556,28 +568,39 @@
 
 @dataclass(frozen=True)
 class ChipsPushing(Operation):
     """The class for chips pushings."""
 
     amounts: tuple[int, ...]
     """The amounts."""
-    rake: int
-    """The rake."""
+    raked_amount: int
+    """The raked amount."""
+
+    @property
+    def unraked_amount(self) -> int:
+        """Return the amount that was not raked and therefore pushed.
+
+        This is identical to the sum of values in
+        :attr:`pokerkit.state.ChipsPushing.amounts`.
+
+        :return: The unraked amount.
+        """
+        return sum(self.amounts)
 
     @property
     def total_amount(self) -> int:
         """Return the total amount.
 
         >>> chips_pushing = ChipsPushing((1, 2, 3), 0)
         >>> chips_pushing.total_amount
         6
 
         :return: The total amount.
         """
-        return sum(self.amounts) + self.rake
+        return self.raked_amount + self.unraked_amount
 
 
 @dataclass(frozen=True)
 class ChipsPulling(Operation):
     """The class for chips pullings."""
 
     player_index: int
@@ -732,15 +755,15 @@
     Folding(commentary=None, player_index=0)
 
     The bets are collected and distributed to the winner.
 
     >>> state.collect_bets()
     BetCollection(commentary=None, bets=(0, 0))
     >>> state.push_chips()
-    ChipsPushing(commentary=None, amounts=(0, 2), rake=0)
+    ChipsPushing(commentary=None, amounts=(0, 2), raked_amount=0)
     >>> state.pull_chips(1)
     ChipsPulling(commentary=None, player_index=1, amount=3)
 
     The game has terminated.
 
     >>> state.status
     False
@@ -848,20 +871,25 @@
     divmod: Callable[[int, int], tuple[int, int]] = divmod
     """The divmod function. Defaults to PokerKit's that detects integral
     or real values automatically.
 
     This is used to denote how pots are divided up (for multiple boards,
     multiple winners, multiple hand types, etc.).
     """
-    rake: Callable[[int], tuple[Any, int]] = partial(rake, rake=0)
+    rake: Callable[[int, State], tuple[int, int]] = rake
     """The rake function. Defaults to zero rake.
 
     Rake functions are used in PokerKit to denote how the rakes are
     collected from the pot. Multiple pots may exist (side-pots) in which
     case the method is called for each pot.
+
+    The user may supply a custom rake function. This function must
+    accept two positional arguments: the state and the amount to be
+    raked. Its return value should be a tuple consisting of two values:
+    the raked amount and the remaining, unraked amount.
     """
     antes: tuple[int, ...] = field(init=False)
     """The antes.
 
     This value is "interpreted" version of the "raw" antes.
     """
     blinds_or_straddles: tuple[int, ...] = field(init=False)
@@ -1358,15 +1386,15 @@
         HoleCardsShowingOrMucking(commentary=None, player_index=1, hole_card...
         >>> state.street is None
         True
 
         Teardown.
 
         >>> state.push_chips()
-        ChipsPushing(commentary=None, amounts=(6, 0), rake=0)
+        ChipsPushing(commentary=None, amounts=(6, 0), raked_amount=0)
         >>> state.street is None
         True
         >>> state.pull_chips()
         ChipsPulling(commentary=None, player_index=0, amount=6)
         >>> state.street is None
         True
 
@@ -2503,15 +2531,15 @@
         HoleCardsShowingOrMucking(commentary=None, player_index=0, hole_card...
         >>> state.show_or_muck_hole_cards()  # doctest: +ELLIPSIS
         HoleCardsShowingOrMucking(commentary=None, player_index=1, hole_card...
 
         Teardown.
 
         >>> state.push_chips()
-        ChipsPushing(commentary=None, amounts=(66, 0), rake=0)
+        ChipsPushing(commentary=None, amounts=(66, 0), raked_amount=0)
         >>> state.total_pot_amount
         66
         >>> state.pull_chips()
         ChipsPulling(commentary=None, player_index=0, amount=66)
         >>> state.total_pot_amount
         0
 
@@ -2603,25 +2631,25 @@
         CheckingOrCalling(commentary=None, player_index=5, amount=100)
         >>> state.check_or_call()
         CheckingOrCalling(commentary=None, player_index=0, amount=49)
         >>> tuple(state.pots)
         ()
         >>> state.check_or_call()
         CheckingOrCalling(commentary=None, player_index=1, amount=98)
-        >>> next(state.pots)
-        Pot(amount=300, player_indices=(0, 1, 2, 3, 4, 5))
+        >>> next(state.pots)  # doctest: +ELLIPSIS
+        Pot(raked_amount=0, unraked_amount=300, player_indices=(0, 1, 2, 3, ...
         >>> pots = tuple(state.pots)
         >>> len(pots)
         3
-        >>> pots[0]
-        Pot(amount=300, player_indices=(0, 1, 2, 3, 4, 5))
+        >>> pots[0]  # doctest: +ELLIPSIS
+        Pot(raked_amount=0, unraked_amount=300, player_indices=(0, 1, 2, 3, ...
         >>> pots[1]
-        Pot(amount=250, player_indices=(1, 2, 3, 4, 5))
+        Pot(raked_amount=0, unraked_amount=250, player_indices=(1, 2, 3, 4, 5))
         >>> pots[2]
-        Pot(amount=300, player_indices=(2, 3, 4))
+        Pot(raked_amount=0, unraked_amount=300, player_indices=(2, 3, 4))
 
         Flop.
 
         >>> state.deal_board()  # doctest: +ELLIPSIS
         BoardDealing(commentary=None, cards=(..., ..., ...))
 
         Turn.
@@ -2685,15 +2713,18 @@
                 ):
                     player_indices.append(i)
 
             while pots and pots[-1].player_indices == tuple(player_indices):
                 amount += pots.pop().amount
 
             if amount:
-                pots.append(Pot(amount, tuple(player_indices)))
+                raked_amount, unraked_amount = self.rake(amount, self)
+                pot = Pot(raked_amount, unraked_amount, tuple(player_indices))
+
+                pots.append(pot)
 
             amount = 0
             previous_contribution = contribution
 
         yield from pots
 
     # ante posting
@@ -3013,14 +3044,18 @@
         return True
 
     def collect_bets(self, *, commentary: str | None = None) -> BetCollection:
         """Collect the bets.
 
         In this operation, the outstanding bets are collected into the pot.
 
+        Note that, when the hand is folded, the last aggressor's bet is
+        returned to his/her stack. The rest of the outstanding bets are
+        collected to the pot.
+
         :param commentary: The optional commentary.
         :return: The bet collection.
         :raises ValueError: If the bet collection cannot be done.
         """
         self.verify_bet_collection()
 
         assert self.bet_collection_status
@@ -5683,21 +5718,20 @@
         :raises ValueError: If the chips pushing cannot be done.
         """
         self.verify_chips_pushing()
 
         assert self._pots is not None and self._pots
 
         pot = self._pots.pop()
-        raked_amount, pushed_amount = self.rake(pot.amount)
         bets = self.bets.copy()
 
         if sum(self.statuses) == 1:
             assert len(pot.player_indices) == 1
 
-            self.bets[pot.player_indices[0]] += pushed_amount
+            self.bets[pot.player_indices[0]] += pot.unraked_amount
         else:
 
             def push(player_indices: list[int], amount: int) -> None:
                 player_indices.sort()
 
                 for j, k in enumerate(player_indices):
                     assert self.statuses[k]
@@ -5710,15 +5744,15 @@
 
                     if not j:
                         sub_amount += remainder
 
                     self.bets[k] += sub_amount
 
             pushed_amount_quotient, pushed_amount_remainder = self.divmod(
-                pushed_amount,
+                pot.unraked_amount,
                 self.board_count,
             )
 
             for i in self.board_indices:
                 pushed_amount = pushed_amount_quotient
 
                 if not i:
@@ -5752,15 +5786,15 @@
                     if not j:
                         amount += remainder
 
                     push(player_indices, amount)
 
         operation = ChipsPushing(
             tuple(starmap(sub, zip(self.bets, bets))),
-            raked_amount,
+            pot.raked_amount,
             commentary=commentary,
         )
 
         self._update_chips_pushing(operation)
 
         return operation
```

### Comparing `pokerkit-0.5.0a0/pokerkit/tests/test_analysis.py` & `pokerkit-0.5.0a1/pokerkit/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a0/pokerkit/tests/test_games.py` & `pokerkit-0.5.0a1/pokerkit/tests/test_games.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a0/pokerkit/tests/test_lookups.py` & `pokerkit-0.5.0a1/pokerkit/tests/test_lookups.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a0/pokerkit/tests/test_notation.py` & `pokerkit-0.5.0a1/pokerkit/tests/test_notation.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a0/pokerkit/tests/test_papers.py` & `pokerkit-0.5.0a1/pokerkit/tests/test_papers.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a0/pokerkit/tests/test_state.py` & `pokerkit-0.5.0a1/pokerkit/tests/test_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1047,15 +1047,15 @@
             ),
             True,
             0,
             (1, 2),
             2,
             (100, 10),
             2,
-            rake=partial(rake, rake=0.1),
+            rake=partial(rake, percentage=0.1),
         )
 
         state.deal_hole('2c3c')
         state.deal_hole('2d3d')
         state.complete_bet_or_raise_to(10)
         state.check_or_call()
         state.burn_card('??')
@@ -1079,15 +1079,15 @@
             ),
             True,
             0,
             (1, 2),
             2,
             (100, 10, 1000),
             3,
-            rake=partial(rake, rake=0.1),
+            rake=partial(rake, percentage=0.1),
         )
 
         state.deal_hole('2c3c')
         state.deal_hole('2d3d')
         state.deal_hole('2h3h')
         state.complete_bet_or_raise_to(1000)
         state.check_or_call()
@@ -1114,15 +1114,15 @@
             ),
             True,
             0,
             (1, 2),
             2,
             (100, 10, 10000, 1000),
             4,
-            rake=partial(rake, rake=0.1),
+            rake=partial(rake, percentage=0.1),
         )
 
         state.deal_hole('2c3c')
         state.deal_hole('2d3d')
         state.deal_hole('2h3h')
         state.deal_hole('2s3s')
         state.complete_bet_or_raise_to(10000)
@@ -1152,15 +1152,15 @@
             ),
             True,
             0,
             (1, 2),
             2,
             (100, 10, 100000, 10000, 1000),
             5,
-            rake=partial(rake, rake=0.1),
+            rake=partial(rake, percentage=0.1),
         )
 
         state.deal_hole('2c3c')
         state.deal_hole('2d3d')
         state.deal_hole('2h3h')
         state.deal_hole('2s3s')
         state.deal_hole('4c5c')
@@ -1178,14 +1178,70 @@
         state.push_chips()
         state.push_chips()
         state.push_chips()
         state.push_chips()
         self.assertFalse(state.status)
         self.assertEqual(state.stacks, [90, 9, 99000, 9000, 900])
 
+        state = NoLimitTexasHoldem.create_state(
+            (
+                Automation.ANTE_POSTING,
+                Automation.BET_COLLECTION,
+                Automation.BLIND_OR_STRADDLE_POSTING,
+                Automation.HOLE_CARDS_SHOWING_OR_MUCKING,
+                Automation.HAND_KILLING,
+                Automation.CHIPS_PULLING,
+            ),
+            True,
+            0,
+            (1, 2),
+            2,
+            100,
+            2,
+            rake=partial(rake, percentage=0.1),
+        )
+
+        state.deal_hole('????')
+        state.deal_hole('????')
+        state.complete_bet_or_raise_to(6)
+        state.complete_bet_or_raise_to(18)
+        state.complete_bet_or_raise_to(54)
+        state.fold()
+        state.push_chips()
+        self.assertFalse(state.status)
+        self.assertEqual(state.stacks, [82, 116])
+
+        state = NoLimitTexasHoldem.create_state(
+            (
+                Automation.ANTE_POSTING,
+                Automation.BET_COLLECTION,
+                Automation.BLIND_OR_STRADDLE_POSTING,
+                Automation.HOLE_CARDS_SHOWING_OR_MUCKING,
+                Automation.HAND_KILLING,
+                Automation.CHIPS_PULLING,
+            ),
+            True,
+            0,
+            (1, 2),
+            2,
+            100,
+            2,
+            rake=partial(rake, percentage=0.1, no_flop_no_drop=True),
+        )
+
+        state.deal_hole('????')
+        state.deal_hole('????')
+        state.complete_bet_or_raise_to(6)
+        state.complete_bet_or_raise_to(18)
+        state.complete_bet_or_raise_to(54)
+        state.fold()
+        state.push_chips()
+        self.assertFalse(state.status)
+        self.assertEqual(state.stacks, [82, 118])
+
     def test_unknown_showdown(self) -> None:
         state = NoLimitTexasHoldem.create_state(
             (
                 Automation.ANTE_POSTING,
                 Automation.BET_COLLECTION,
                 Automation.BLIND_OR_STRADDLE_POSTING,
                 Automation.HAND_KILLING,
```

### Comparing `pokerkit-0.5.0a0/pokerkit/tests/test_utilities.py` & `pokerkit-0.5.0a1/pokerkit/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a0/pokerkit/tests/test_wsop/test_2023_43_5.py` & `pokerkit-0.5.0a1/pokerkit/tests/test_wsop/test_2023_43_5.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a0/pokerkit/tests/test_wsop/test_2023_54_4.py` & `pokerkit-0.5.0a1/pokerkit/tests/test_wsop/test_2023_54_4.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a0/pokerkit/utilities.py` & `pokerkit-0.5.0a1/pokerkit/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,24 @@
 from __future__ import annotations
 
 from collections.abc import Iterable, Iterator, Mapping
 from dataclasses import dataclass
 from enum import Enum, StrEnum, unique
 from functools import partial
 from itertools import product, starmap
+from math import inf
 from numbers import Integral
 from operator import is_not
 from random import shuffle
-from typing import Any, cast, TypeVar
+from typing import Any, cast, TYPE_CHECKING, TypeVar
 import builtins
 
+if TYPE_CHECKING:
+    from pokerkit.state import State
+
 _T = TypeVar('_T')
 
 
 @unique
 class Rank(StrEnum):
     """The enum class for ranks.
 
@@ -652,38 +656,89 @@
 
     quotient = dividend / divisor
     remainder = dividend - quotient * divisor
 
     return cast(tuple[int, int], (quotient, remainder))
 
 
-def rake(amount: int, rake: float) -> tuple[int, int]:
+def rake(
+        amount: int,
+        state: State | None = None,
+        *,
+        percentage: float = 0,
+        cap: float = inf,
+        no_flop_no_drop: bool = False,
+) -> tuple[int, int]:
     """Rake the amount.
 
-    >>> rake(100, 0)
+    Note that the percentage value are expected to be within range
+    [``0``, ``1``]. For instance, ``0.1`` represents 10%.
+
+    >>> rake(100)
     (0, 100)
-    >>> rake(1000, 0.1)
+    >>> rake(1000, percentage=0.1)
     (100, 900)
-    >>> rake(10, 0.11)
+    >>> rake(10, percentage=0.11)
     (1, 9)
-    >>> rake(10.0, 0.11)
+    >>> rake(10.0, percentage=0.11)
     (1.1, 8.9)
+    >>> rake(10.0, percentage=0.11, cap=1.0)
+    (1.0, 9.0)
+    >>> rake(100, percentage=0.1, no_flop_no_drop=True)  # doctest: +ELLIPSIS
+    Traceback (most recent call last):
+        ...
+    ValueError: If no-flop-no-drop is enabled, the state must be checked, bu...
+
+    In game contexts, the ``state`` parameter will not be ``None`` as it
+    is by default. This can be used to encode a more complicated raking
+    logic.
+
+    If ``no_flop_no_drop`` is enabled, this means that a rake will only
+    be collected if a flop is dealt. Since PokerKit caters to many
+    variants, we interpret this as being that there exists at least one
+    card on the board. Some variants do not involve board cards, so if
+    this parameter is set to ``True``, no rake will be raked whatsoever.
 
     :param amount: The pot amount.
-    :param rake: The rake.
-    :return: The raked amount and the remaining amount.
-    """
-    raked_amount = amount * rake
+    :param state: The optional poker state whose pot is being raked.
+    :param percentage: The rake percentage, defaults to ``0``. It should
+                       be between ``0`` (0%) and ``1`` (100%).
+    :param cap: The maximum raked amount, defaults to ``math.inf``
+                (unlimited).
+    :param no_flop_no_drop: ``True`` to only rake when there are cards
+                            on the board, ``False`` otherwise. Defaults
+                            to ``False``.
+    :return: The raked amount and the unraked amount.
+    """
+    if not 0 <= percentage <= 1:
+        raise ValueError(
+            'The rake percentage ({percentage}) should be between 0 and 1.',
+        )
+
+    if no_flop_no_drop:
+        if state is None:
+            raise ValueError(
+                (
+                    'If no-flop-no-drop is enabled, the state must be checked,'
+                    ' but it is unavailable.'
+                ),
+            )
+
+        if not any(state.board_cards):
+            return 0, amount
+
+    raked_amount = amount * percentage
 
     if isinstance(amount, Integral):
         raked_amount = round(raked_amount)
 
-    remaining_amount = amount - raked_amount
+    raked_amount = min(raked_amount, cap)
+    unraked_amount = amount - raked_amount
 
-    return cast(tuple[int, int], (raked_amount, remaining_amount))
+    return cast(tuple[int, int], (raked_amount, unraked_amount))
 
 
 def parse_value(raw_value: str) -> int:
     """Convert ``str`` to a number.
 
     >>> parse_value('3')
     3
```

### Comparing `pokerkit-0.5.0a0/pokerkit.egg-info/PKG-INFO` & `pokerkit-0.5.0a1/pokerkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerkit
-Version: 0.5.0a0
+Version: 0.5.0a1
 Summary: An open-source Python library for poker game simulations, hand evaluations, and statistical analysis
 Home-page: https://github.com/uoftcprg/pokerkit
 Author: University of Toronto Computer Poker Student Research Group
 Author-email: uoftcprg@studentorg.utoronto.ca
 License: MIT
 Project-URL: Documentation, https://pokerkit.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/uoftcprg/pokerkit
```

### Comparing `pokerkit-0.5.0a0/pokerkit.egg-info/SOURCES.txt` & `pokerkit-0.5.0a1/pokerkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a0/setup.py` & `pokerkit-0.5.0a1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 from setuptools import find_packages, setup
 
 setup(
     name='pokerkit',
-    version='0.5.0a0',
+    version='0.5.0a1',
     description='An open-source Python library for poker game simulations, hand evaluations, and statistical analysis',
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
     url='https://github.com/uoftcprg/pokerkit',
     author='University of Toronto Computer Poker Student Research Group',
     author_email='uoftcprg@studentorg.utoronto.ca',
     license='MIT',
```

