# Comparing `tmp/pokerengine-1.5.1.tar.gz` & `tmp/pokerengine-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerengine-1.5.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pokerengine-1.6.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pokerengine-1.5.1.tar` & `pokerengine-1.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     3831 2022-11-09 12:37:21.000000 pokerengine-1.5.1/.clang-format
--rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 pokerengine-1.5.1/.github/dependabot.yaml
--rw-r--r--   0        0        0      648 2022-11-09 12:37:21.000000 pokerengine-1.5.1/.github/workflows/pre-commit-updater.yml
--rw-r--r--   0        0        0      578 2022-11-09 12:37:21.000000 pokerengine-1.5.1/.gitignore
--rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 pokerengine-1.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2032 2022-11-09 12:37:21.000000 pokerengine-1.5.1/CMakeLists.txt
--rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pokerengine-1.5.1/README.md
--rw-r--r--   0        0        0    40775 2022-11-09 12:37:21.000000 pokerengine-1.5.1/cmake/CPM.cmake
--rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 pokerengine-1.5.1/cmake/Packages.cmake
--rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 pokerengine-1.5.1/examples/hand_straight.py
--rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/bits.hpp
--rw-r--r--   0        0        0     7514 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/card/card.hpp
--rw-r--r--   0        0        0     2663 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/card/cards.hpp
--rw-r--r--   0        0        0     3364 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/card/hand.hpp
--rw-r--r--   0        0        0     1585 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/constants.hpp
--rw-r--r--   0        0        0    31732 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/engine.hpp
--rw-r--r--   0        0        0     3119 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/enums.hpp
--rw-r--r--   0        0        0     4460 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/evaluator/evaluation.hpp
--rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/evaluator/evaluation_result.hpp
--rw-r--r--   0        0        0   136152 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/evaluator/lookup_tables.hpp
--rw-r--r--   0        0        0     5387 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/evaluator/result.hpp
--rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/pokerengine.hpp
--rw-r--r--   0        0        0     8217 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/python/pycard.hpp
--rw-r--r--   0        0        0     1925 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/python/pyconstants.hpp
--rw-r--r--   0        0        0    12076 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/python/pyengine.hpp
--rw-r--r--   0        0        0     5720 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/python/pyenums.hpp
--rw-r--r--   0        0        0     2586 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/python/pyevaluation.hpp
--rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/python/python.hpp
--rw-r--r--   0        0        0     1327 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/string.hpp
--rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/types.hpp
--rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pokerengine-1.5.1/include/pokerengine/vector.hpp
--rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 pokerengine-1.5.1/licenses/MIT
--rw-r--r--   0        0        0     1190 2022-11-09 12:37:21.000000 pokerengine-1.5.1/pyproject.toml
--rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/__init__.py
--rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/card.py
--rw-r--r--   0        0        0      814 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/constants.py
--rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/engine.py
--rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/enums.py
--rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/evaluation.py
--rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/pokerengine_core/__init__.pyi
--rw-r--r--   0        0        0     7462 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/pokerengine_core/card.pyi
--rw-r--r--   0        0        0      672 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/pokerengine_core/constants.pyi
--rw-r--r--   0        0        0     7963 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/pokerengine_core/engine.pyi
--rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/pokerengine_core/enums/__init__.pyi
--rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/pokerengine_core/enums/action.pyi
--rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/pokerengine_core/enums/combination.pyi
--rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/pokerengine_core/enums/position.pyi
--rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/pokerengine_core/enums/rank.pyi
--rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/pokerengine_core/enums/round.pyi
--rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/pokerengine_core/enums/state.pyi
--rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/pokerengine_core/enums/suit.pyi
--rw-r--r--   0        0        0     2418 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/pokerengine_core/evaluation.pyi
--rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine/pokerengine_core/utils.pyi
--rw-r--r--   0        0        0      922 2022-11-09 12:37:21.000000 pokerengine-1.5.1/src/pokerengine.cpp
--rw-r--r--   0        0        0      703 2022-11-09 12:37:21.000000 pokerengine-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     3831 2022-11-09 12:37:21.000000 pokerengine-1.6/.clang-format
+-rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 pokerengine-1.6/.github/dependabot.yaml
+-rw-r--r--   0        0        0      648 2022-11-09 12:37:21.000000 pokerengine-1.6/.github/workflows/pre-commit-updater.yml
+-rw-r--r--   0        0        0      578 2022-11-09 12:37:21.000000 pokerengine-1.6/.gitignore
+-rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 pokerengine-1.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2030 2022-11-09 12:37:21.000000 pokerengine-1.6/CMakeLists.txt
+-rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pokerengine-1.6/README.md
+-rw-r--r--   0        0        0    40775 2022-11-09 12:37:21.000000 pokerengine-1.6/cmake/CPM.cmake
+-rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 pokerengine-1.6/cmake/Packages.cmake
+-rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 pokerengine-1.6/examples/hand_straight.py
+-rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/bits.hpp
+-rw-r--r--   0        0        0     7476 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/card/card.hpp
+-rw-r--r--   0        0        0     2663 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/card/cards.hpp
+-rw-r--r--   0        0        0     3364 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/card/hand.hpp
+-rw-r--r--   0        0        0     1544 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/constants.hpp
+-rw-r--r--   0        0        0    31732 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/engine.hpp
+-rw-r--r--   0        0        0     3119 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/enums.hpp
+-rw-r--r--   0        0        0     4460 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/evaluator/evaluation.hpp
+-rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/evaluator/evaluation_result.hpp
+-rw-r--r--   0        0        0   136152 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/evaluator/lookup_tables.hpp
+-rw-r--r--   0        0        0     5387 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/evaluator/result.hpp
+-rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/pokerengine.hpp
+-rw-r--r--   0        0        0     8217 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/python/pycard.hpp
+-rw-r--r--   0        0        0     1856 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/python/pyconstants.hpp
+-rw-r--r--   0        0        0    12076 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/python/pyengine.hpp
+-rw-r--r--   0        0        0     5720 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/python/pyenums.hpp
+-rw-r--r--   0        0        0     2586 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/python/pyevaluation.hpp
+-rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/python/python.hpp
+-rw-r--r--   0        0        0     1327 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/string.hpp
+-rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/types.hpp
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pokerengine-1.6/include/pokerengine/vector.hpp
+-rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 pokerengine-1.6/licenses/MIT
+-rw-r--r--   0        0        0     1188 2022-11-09 12:37:21.000000 pokerengine-1.6/pyproject.toml
+-rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/__init__.py
+-rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/card.py
+-rw-r--r--   0        0        0      814 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/constants.py
+-rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/engine.py
+-rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/enums.py
+-rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/evaluation.py
+-rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/pokerengine_core/__init__.pyi
+-rw-r--r--   0        0        0     7462 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/pokerengine_core/card.pyi
+-rw-r--r--   0        0        0      672 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/pokerengine_core/constants.pyi
+-rw-r--r--   0        0        0     7963 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/pokerengine_core/engine.pyi
+-rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/pokerengine_core/enums/__init__.pyi
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/pokerengine_core/enums/action.pyi
+-rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/pokerengine_core/enums/combination.pyi
+-rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/pokerengine_core/enums/position.pyi
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/pokerengine_core/enums/rank.pyi
+-rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/pokerengine_core/enums/round.pyi
+-rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/pokerengine_core/enums/state.pyi
+-rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/pokerengine_core/enums/suit.pyi
+-rw-r--r--   0        0        0     2418 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/pokerengine_core/evaluation.pyi
+-rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine/pokerengine_core/utils.pyi
+-rw-r--r--   0        0        0      922 2022-11-09 12:37:21.000000 pokerengine-1.6/src/pokerengine.cpp
+-rw-r--r--   0        0        0      701 2022-11-09 12:37:21.000000 pokerengine-1.6/PKG-INFO
```

### Comparing `pokerengine-1.5.1/.clang-format` & `pokerengine-1.6/.clang-format`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/.github/workflows/pre-commit-updater.yml` & `pokerengine-1.6/.github/workflows/pre-commit-updater.yml`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/.gitignore` & `pokerengine-1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/.pre-commit-config.yaml` & `pokerengine-1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/CMakeLists.txt` & `pokerengine-1.6/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cmake_minimum_required(VERSION 3.12)
 
-project(pokerengine VERSION 1.5.1)
+project(pokerengine VERSION 1.6)
 
 include(cmake/Packages.cmake)
 
 set(CMAKE_CXX_STANDARD 20)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_EXTENSIONS OFF)
```

### Comparing `pokerengine-1.5.1/cmake/CPM.cmake` & `pokerengine-1.6/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/examples/hand_straight.py` & `pokerengine-1.6/examples/hand_straight.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/include/pokerengine/bits.hpp` & `pokerengine-1.6/include/pokerengine/bits.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/include/pokerengine/card/card.hpp` & `pokerengine-1.6/include/pokerengine/card/card.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     }
 
     auto operator==(const card &other) const noexcept -> bool {
         return get_card() == other.get_card();
     }
 
     explicit operator std::string() const {
-        return std::string{ get_rank() } + std::string{ constants::SEPARATOR } + std::string{ get_suit() };
+        return std::string{ get_rank() } + std::string{ get_suit() };
     }
 
     [[nodiscard]] auto as_bitset() const noexcept -> types::bit_set {
         return types::bit_set{ 1 } << card_;
     }
 
     [[nodiscard]] auto get_card() const noexcept -> uint8_t {
```

### Comparing `pokerengine-1.5.1/include/pokerengine/card/cards.hpp` & `pokerengine-1.6/include/pokerengine/card/cards.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/include/pokerengine/card/hand.hpp` & `pokerengine-1.6/include/pokerengine/card/hand.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/include/pokerengine/constants.hpp` & `pokerengine-1.6/include/pokerengine/constants.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 #include <array>
 #include <cstdint>
 #include <string>
 
 #include "pokerengine.hpp"
 
 namespace pokerengine::constants {
-const std::string_view SEPARATOR = "_";
-
 const uint8_t MASK_RANKS_NUMBER = 0b0000'1111;
 const uint16_t MASK_RANKS = 0b0001'1111'1111'1111;
 
 const uint8_t RANKS = 13;
 const uint8_t SUITS = 4;
 
 const uint8_t DECK_SIZE = RANKS * SUITS;
```

### Comparing `pokerengine-1.5.1/include/pokerengine/engine.hpp` & `pokerengine-1.6/include/pokerengine/engine.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -569,15 +569,15 @@
         auto iterable = this->engine.players.get_players();
         return std::accumulate(iterable.cbegin(), iterable.cend(), 0, [&](int value, auto const &element) -> int {
             return element.state != enums::state::out && element.state != enums::state::allin ? value + 1 :
                                                                                                 value;
         });
     }
 
-    [[nodiscard]] auto in_terminal_state() const -> bool {
+    [[nodiscard]] auto is_showdown() const -> bool {
         return get_number_alive() > 1;
     }
 
     auto set_current(enums::position position) -> void {
         current_ = position;
     }
 
@@ -703,15 +703,15 @@
     using actual::engine_detail< Engine >::engine_detail;
 
     auto reset() noexcept -> void {
         set_round(enums::round::preflop);
         set_flop_dealt(false);
     }
 
-    [[nodiscard]] auto is_showdown() const noexcept -> bool {
+    [[nodiscard]] auto in_terminal_state() const noexcept -> bool {
         return get_round() == enums::round::showdown;
     }
 
     [[nodiscard]] auto get_round() const noexcept -> enums::round {
         return round_;
     }
```

### Comparing `pokerengine-1.5.1/include/pokerengine/enums.hpp` & `pokerengine-1.6/include/pokerengine/enums.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/include/pokerengine/evaluator/evaluation.hpp` & `pokerengine-1.6/include/pokerengine/evaluator/evaluation.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/include/pokerengine/evaluator/evaluation_result.hpp` & `pokerengine-1.6/include/pokerengine/evaluator/evaluation_result.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/include/pokerengine/evaluator/lookup_tables.hpp` & `pokerengine-1.6/include/pokerengine/evaluator/lookup_tables.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/include/pokerengine/evaluator/result.hpp` & `pokerengine-1.6/include/pokerengine/evaluator/result.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/include/pokerengine/python/pycard.hpp` & `pokerengine-1.6/include/pokerengine/python/pycard.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/include/pokerengine/python/pyconstants.hpp` & `pokerengine-1.6/include/pokerengine/python/pyconstants.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 #include "python/python.hpp"
 
 namespace python {
 auto setup_constants_all(py::module_ &module_) -> void {
     auto constants = module_.def_submodule("constants");
 
-    constants.attr("SEPARATOR") = pokerengine::constants::SEPARATOR;
     constants.attr("MASK_RANKS_NUMBER") = pokerengine::constants::MASK_RANKS_NUMBER;
     constants.attr("MASK_RANKS") = pokerengine::constants::MASK_RANKS;
     constants.attr("RANKS") = pokerengine::constants::RANKS;
     constants.attr("SUITS") = pokerengine::constants::SUITS;
     constants.attr("DECK_SIZE") = pokerengine::constants::DECK_SIZE;
     constants.attr("CARD_INDEX_MIN") = pokerengine::constants::CARD_INDEX_MIN;
     constants.attr("CARD_INDEX_MAX") = pokerengine::constants::CARD_INDEX_MAX;
```

### Comparing `pokerengine-1.5.1/include/pokerengine/python/pyengine.hpp` & `pokerengine-1.6/include/pokerengine/python/pyengine.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -71,16 +71,16 @@
                     .def("set_next_current",
                          &pokerengine::positions_manager< pokerengine::engine< A, B > >::set_next_current)
                     .def("set_next_round_player",
                          &pokerengine::positions_manager< pokerengine::engine< A, B > >::set_next_round_player)
                     .def("actionable",
                          &pokerengine::positions_manager< pokerengine::engine< A, B > >::get_actionable)
                     .def_property_readonly(
-                                    "terminal_state",
-                                    &pokerengine::positions_manager< pokerengine::engine< A, B > >::in_terminal_state)
+                                    "showdown",
+                                    &pokerengine::positions_manager< pokerengine::engine< A, B > >::is_showdown)
                     .def_property_readonly(
                                     "number_alive",
                                     &pokerengine::positions_manager< pokerengine::engine< A, B > >::get_number_alive)
                     .def_property_readonly(
                                     "future_actionable",
                                     &pokerengine::positions_manager< pokerengine::engine< A, B > >::get_future_actionable)
                     .def_property_readonly(
@@ -113,16 +113,16 @@
                                     "round_highest_bet",
                                     &pokerengine::pot_manager< pokerengine::engine< A, B >, A, B >::get_round_highest_bet);
     py::class_< pokerengine::round_manager< pokerengine::engine< A, B > > >(
                     module_, ("Round" + pyclass_postfix).c_str(), py::module_local())
                     .def(py::init< pokerengine::engine< A, B > & >(), py::arg("engine"))
                     .def("reset", &pokerengine::round_manager< pokerengine::engine< A, B > >::reset)
                     .def_property_readonly(
-                                    "showdown",
-                                    &pokerengine::round_manager< pokerengine::engine< A, B > >::is_showdown)
+                                    "terminal_state",
+                                    &pokerengine::round_manager< pokerengine::engine< A, B > >::in_terminal_state)
                     .def_property("round",
                                   &pokerengine::round_manager< pokerengine::engine< A, B > >::get_round,
                                   &pokerengine::round_manager< pokerengine::engine< A, B > >::set_round)
                     .def_property("flop_dealt",
                                   &pokerengine::round_manager< pokerengine::engine< A, B > >::get_flop_dealt,
                                   &pokerengine::round_manager< pokerengine::engine< A, B > >::set_flop_dealt);
 }
@@ -164,15 +164,15 @@
                     .def_readwrite("front", &pokerengine::player::front)
                     .def_readwrite("round_bet", &pokerengine::player::round_bet)
                     .def_readwrite("state", &pokerengine::player::state)
                     .def_readwrite("id", &pokerengine::player::id);
     py::class_< pokerengine::player_action >(module_, "PlayerAction", py::module_local())
                     .def(py::init< int32_t, pokerengine::enums::action, pokerengine::enums::position >(),
                          py::arg("amount"),
-                         py::arg("amount"),
+                         py::arg("action"),
                          py::arg("position"))
                     .def(py::self == py::self, py::arg("other")) // NOLINT
                     .def("__str__",
                          [](pokerengine::player_action &self) -> std::string { return std::string{ self }; })
                     .def_readwrite("amount", &pokerengine::player_action::amount)
                     .def_readwrite("action", &pokerengine::player_action::action)
                     .def_readwrite("position", &pokerengine::player_action::position);
```

### Comparing `pokerengine-1.5.1/include/pokerengine/python/pyenums.hpp` & `pokerengine-1.6/include/pokerengine/python/pyenums.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/include/pokerengine/python/pyevaluation.hpp` & `pokerengine-1.6/include/pokerengine/python/pyevaluation.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/include/pokerengine/string.hpp` & `pokerengine-1.6/include/pokerengine/string.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/include/pokerengine/vector.hpp` & `pokerengine-1.6/include/pokerengine/vector.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/licenses/MIT` & `pokerengine-1.6/licenses/MIT`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/pyproject.toml` & `pokerengine-1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["scikit-build-core==0.6.1", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "pokerengine"
-version = "1.5.1"
+version = "1.6"
 description = "Poker Library"
 readme = "README.md"
 authors = [
     {name = "raindinners"}
 ]
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `pokerengine-1.5.1/src/pokerengine/constants.py` & `pokerengine-1.6/src/pokerengine/constants.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/src/pokerengine/enums.py` & `pokerengine-1.6/src/pokerengine/enums.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/src/pokerengine/pokerengine_core/card.pyi` & `pokerengine-1.6/src/pokerengine/pokerengine_core/card.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/src/pokerengine/pokerengine_core/constants.pyi` & `pokerengine-1.6/src/pokerengine/pokerengine_core/constants.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/src/pokerengine/pokerengine_core/engine.pyi` & `pokerengine-1.6/src/pokerengine/pokerengine_core/engine.pyi`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -223,19 +223,19 @@
     def player(self) -> Player:
         """
         Use this method to get current player.
 
         :return: Current player
         """
     @property
-    def terminal_state(self) -> bool:
+    def showdown(self) -> bool:
         """
-        Use this method to get game state.
+        Use this method to get is game is showdown.
 
-        :return: Is number alive is greater than one
+        :return: Is game is showdown
         """
     def actionable(self) -> int:
         """
         Use this method to get number actionable players.
 
         :return: Number actionable
         """
@@ -304,19 +304,19 @@
     """
 
     flop_dealt: bool = False
     round: RoundE = RoundE.NONE
 
     def __init__(self, engine: Engine) -> None: ...
     @property
-    def showdown(self) -> bool:
+    def terminal_state(self) -> bool:
         """
-        Use this method to get is game is showdown.
+        Use this method to get game state.
 
-        :return: Is game is showdown
+        :return: Is number alive is greater than one
         """
     def reset(self) -> None:
         """
         Use this method to reset round.
 
         :return: :class:`None`
         """
```

### Comparing `pokerengine-1.5.1/src/pokerengine/pokerengine_core/evaluation.pyi` & `pokerengine-1.6/src/pokerengine/pokerengine_core/evaluation.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/src/pokerengine.cpp` & `pokerengine-1.6/src/pokerengine.cpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.5.1/PKG-INFO` & `pokerengine-1.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerengine
-Version: 1.5.1
+Version: 1.6
 Summary: Poker Library
 Keywords: raindinners,engine,poker,texas,holdem,texas-holdem,texas_holdem,pybind11,scikit-build-core,fast,c++,magic_enum,stubs,python-stubs,python_stubs,pythonstubs,py-stubs,py_stubs,pystubs
 Author: raindinners
 Requires-Python: >=3.8
 Provides-Extra: dev
 Provides-Extra: build
 Requires-Dist: black~=23.10.0; extra == "dev"
```

