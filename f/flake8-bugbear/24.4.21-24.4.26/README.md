# Comparing `tmp/flake8_bugbear-24.4.21.tar.gz` & `tmp/flake8_bugbear-24.4.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_bugbear-24.4.21.tar", last modified: Sun Apr 21 15:52:31 2024, max compression
+gzip compressed data, was "flake8_bugbear-24.4.26.tar", last modified: Fri Apr 26 14:51:08 2024, max compression
```

## Comparing `flake8_bugbear-24.4.21.tar` & `flake8_bugbear-24.4.26.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:52:31.004003 flake8_bugbear-24.4.21/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    31212 2024-04-21 15:52:31.004003 flake8_bugbear-24.4.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    29537 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    78687 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/bugbear.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:52:31.004003 flake8_bugbear-24.4.21/flake8_bugbear.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    31212 2024-04-21 15:52:30.000000 flake8_bugbear-24.4.21/flake8_bugbear.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-21 15:52:30.000000 flake8_bugbear-24.4.21/flake8_bugbear.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 15:52:30.000000 flake8_bugbear-24.4.21/flake8_bugbear.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-21 15:52:30.000000 flake8_bugbear-24.4.21/flake8_bugbear.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 15:52:30.000000 flake8_bugbear-24.4.21/flake8_bugbear.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-21 15:52:30.000000 flake8_bugbear-24.4.21/flake8_bugbear.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 15:52:30.000000 flake8_bugbear-24.4.21/flake8_bugbear.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-21 15:52:31.004003 flake8_bugbear-24.4.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:52:31.004003 flake8_bugbear-24.4.21/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b001.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b002.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b003.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b004.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b005.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b006_b008.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b007.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b008_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b009_b010.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b011.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b012.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b013.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b014.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b015.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b016.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b017.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b018_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b018_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b018_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b018_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b019.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b020.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b021.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b022.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b023.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b024.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b025.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b026.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b027.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b028.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b029.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b030.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b031.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b032.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b033.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b034.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b035.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b036.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b037.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b901.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b902.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b902_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b902_py38.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b903.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b904.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b905_py310.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b906.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b907.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b908.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b909.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/b950.py
--rw-r--r--   0 runner    (1001) docker     (127)    37452 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tests/test_bugbear.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-21 15:52:20.000000 flake8_bugbear-24.4.21/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:51:08.371871 flake8_bugbear-24.4.26/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    31297 2024-04-26 14:51:08.371871 flake8_bugbear-24.4.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    29622 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    80067 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/bugbear.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:51:08.367871 flake8_bugbear-24.4.26/flake8_bugbear.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    31297 2024-04-26 14:51:08.000000 flake8_bugbear-24.4.26/flake8_bugbear.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-26 14:51:08.000000 flake8_bugbear-24.4.26/flake8_bugbear.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:51:08.000000 flake8_bugbear-24.4.26/flake8_bugbear.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-26 14:51:08.000000 flake8_bugbear-24.4.26/flake8_bugbear.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:51:08.000000 flake8_bugbear-24.4.26/flake8_bugbear.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-26 14:51:08.000000 flake8_bugbear-24.4.26/flake8_bugbear.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 14:51:08.000000 flake8_bugbear-24.4.26/flake8_bugbear.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-26 14:51:08.371871 flake8_bugbear-24.4.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:51:08.367871 flake8_bugbear-24.4.26/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b001.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b002.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b003.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b004.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b005.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b006_b008.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b007.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b008_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b009_b010.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b011.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b012.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b013.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b014.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b015.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b016.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b017.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b018_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b018_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b018_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b018_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b019.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b020.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b021.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b022.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b023.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b024.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b025.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b026.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b027.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b028.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b029.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b030.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b031.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b032.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b033.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b034.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b035.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b036.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b037.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b901.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b902.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b902_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b902_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b903.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b904.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b905_py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b906.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b907.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b908.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b909.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/b950.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37452 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tests/test_bugbear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-26 14:50:54.000000 flake8_bugbear-24.4.26/tox.ini
```

### Comparing `flake8_bugbear-24.4.21/LICENSE` & `flake8_bugbear-24.4.26/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/PKG-INFO` & `flake8_bugbear-24.4.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-bugbear
-Version: 24.4.21
+Version: 24.4.26
 Summary: A plugin for flake8 finding likely bugs and design problems in your program. Contains warnings that don't belong in pyflakes and pycodestyle.
 Author-email: Łukasz Langa <lukasz@langa.pl>
 License: MIT
 Project-URL: Homepage, https://github.com/PyCQA/flake8-bugbear
 Project-URL: Change Log, https://github.com/PyCQA/flake8-bugbear#change-log
 Keywords: flake8,bugbear,bugs,pyflakes,pylint,linter,qa
 Classifier: Development Status :: 5 - Production/Stable
@@ -385,14 +385,19 @@
 
 MIT
 
 
 Change Log
 ----------
 
+24.4.26
+~~~~~~~
+
+* B909: Fix false positive affecting containers of mutables (#469)
+
 24.4.21
 ~~~~~~~
 
 * B950: Add pragma comment to line length ignores (#463)
 * B909: Add more cases to detect + more container mutating functions (#460)
 
 24.2.6
```

### Comparing `flake8_bugbear-24.4.21/README.rst` & `flake8_bugbear-24.4.26/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -347,14 +347,19 @@
 
 MIT
 
 
 Change Log
 ----------
 
+24.4.26
+~~~~~~~
+
+* B909: Fix false positive affecting containers of mutables (#469)
+
 24.4.21
 ~~~~~~~
 
 * B950: Add pragma comment to line length ignores (#463)
 * B909: Add more cases to detect + more container mutating functions (#460)
 
 24.2.6
```

### Comparing `flake8_bugbear-24.4.21/bugbear.py` & `flake8_bugbear-24.4.26/bugbear.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from functools import lru_cache, partial
 from keyword import iskeyword
 from typing import Dict, List, Set, Union
 
 import attr
 import pycodestyle
 
-__version__ = "24.4.21"
+__version__ = "24.4.26"
 
 LOG = logging.getLogger("flake8.bugbear")
 CONTEXTFUL_NODES = (
     ast.Module,
     ast.ClassDef,
     ast.AsyncFunctionDef,
     ast.FunctionDef,
@@ -1577,19 +1577,21 @@
             check(3, "count")
         elif node.func.attr == "split":
             check(2, "maxsplit")
 
     def check_for_b909(self, node: ast.For):
         if isinstance(node.iter, ast.Name):
             name = _to_name_str(node.iter)
+            key = _to_name_str(node.target)
         elif isinstance(node.iter, ast.Attribute):
             name = _to_name_str(node.iter)
+            key = _to_name_str(node.target)
         else:
             return
-        checker = B909Checker(name)
+        checker = B909Checker(name, key)
         checker.visit(node.body)
         for mutation in itertools.chain.from_iterable(
             m for m in checker.mutations.values()
         ):
             self.errors.append(B909(mutation.lineno, mutation.col_offset))
 
 
@@ -1599,14 +1601,54 @@
         yield node.attr
     elif isinstance(node, ast.Call):
         yield from compose_call_path(node.func)
     elif isinstance(node, ast.Name):
         yield node.id
 
 
+def _tansform_slice_to_py39(slice: ast.Slice) -> ast.Slice | ast.Name:
+    """Transform a py38 style slice to a py39 style slice.
+
+    In py39 the slice was changed to have simple names directly assigned:
+    ```py
+    # code:
+    some_dict[key]
+    # py38:
+    slice=Index(
+        value=Name(
+                lineno=152,
+                col_offset=14,
+                end_lineno=152,
+                end_col_offset=17,
+                id='key',
+                ctx=Load()
+            ),
+    )
+    # py39 onwards:
+    slice=Name(
+                lineno=152,
+                col_offset=14,
+                end_lineno=152,
+                end_col_offset=17,
+                id='key',
+                ctx=Load()
+            ),
+    ```
+
+    > Changed in version 3.9: Simple indices are represented by their value,
+    > extended slices are represented as tuples.
+    from https://docs.python.org/3/library/ast.html#module-ast
+    """
+    if sys.version_info >= (3, 9):
+        return slice
+    if isinstance(slice, ast.Index) and isinstance(slice.value, ast.Name):
+        slice = slice.value
+    return slice
+
+
 class B909Checker(ast.NodeVisitor):
     # https://docs.python.org/3/library/stdtypes.html#mutable-sequence-types
     MUTATING_FUNCTIONS = (
         "append",
         "sort",
         "reverse",
         "remove",
@@ -1620,22 +1662,27 @@
         "intersection_update",
         "difference_update",
         "symmetric_difference_update",
         "add",
         "discard",
     )
 
-    def __init__(self, name: str):
+    def __init__(self, name: str, key: str):
         self.name = name
+        self.key = key
         self.mutations = defaultdict(list)
         self._conditional_block = 0
 
     def visit_Assign(self, node: ast.Assign):
         for target in node.targets:
-            if isinstance(target, ast.Subscript) and _to_name_str(target.value):
+            if (
+                isinstance(target, ast.Subscript)
+                and _to_name_str(target.value) == self.name
+                and _to_name_str(_tansform_slice_to_py39(target.slice)) != self.key
+            ):
                 self.mutations[self._conditional_block].append(node)
         self.generic_visit(node)
 
     def visit_AugAssign(self, node: ast.AugAssign):
         if _to_name_str(node.target) == self.name:
             self.mutations[self._conditional_block].append(node)
         self.generic_visit(node)
```

### Comparing `flake8_bugbear-24.4.21/flake8_bugbear.egg-info/PKG-INFO` & `flake8_bugbear-24.4.26/flake8_bugbear.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-bugbear
-Version: 24.4.21
+Version: 24.4.26
 Summary: A plugin for flake8 finding likely bugs and design problems in your program. Contains warnings that don't belong in pyflakes and pycodestyle.
 Author-email: Łukasz Langa <lukasz@langa.pl>
 License: MIT
 Project-URL: Homepage, https://github.com/PyCQA/flake8-bugbear
 Project-URL: Change Log, https://github.com/PyCQA/flake8-bugbear#change-log
 Keywords: flake8,bugbear,bugs,pyflakes,pylint,linter,qa
 Classifier: Development Status :: 5 - Production/Stable
@@ -385,14 +385,19 @@
 
 MIT
 
 
 Change Log
 ----------
 
+24.4.26
+~~~~~~~
+
+* B909: Fix false positive affecting containers of mutables (#469)
+
 24.4.21
 ~~~~~~~
 
 * B950: Add pragma comment to line length ignores (#463)
 * B909: Add more cases to detect + more container mutating functions (#460)
 
 24.2.6
```

### Comparing `flake8_bugbear-24.4.21/flake8_bugbear.egg-info/SOURCES.txt` & `flake8_bugbear-24.4.26/flake8_bugbear.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/pyproject.toml` & `flake8_bugbear-24.4.26/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b001.py` & `flake8_bugbear-24.4.26/tests/b001.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b005.py` & `flake8_bugbear-24.4.26/tests/b005.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b006_b008.py` & `flake8_bugbear-24.4.26/tests/b006_b008.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b007.py` & `flake8_bugbear-24.4.26/tests/b007.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b009_b010.py` & `flake8_bugbear-24.4.26/tests/b009_b010.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b012.py` & `flake8_bugbear-24.4.26/tests/b012.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b013.py` & `flake8_bugbear-24.4.26/tests/b013.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b014.py` & `flake8_bugbear-24.4.26/tests/b014.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b017.py` & `flake8_bugbear-24.4.26/tests/b017.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b018_classes.py` & `flake8_bugbear-24.4.26/tests/b018_classes.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b018_functions.py` & `flake8_bugbear-24.4.26/tests/b018_functions.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b018_nested.py` & `flake8_bugbear-24.4.26/tests/b018_nested.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b019.py` & `flake8_bugbear-24.4.26/tests/b019.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b020.py` & `flake8_bugbear-24.4.26/tests/b020.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b021.py` & `flake8_bugbear-24.4.26/tests/b021.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b023.py` & `flake8_bugbear-24.4.26/tests/b023.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b024.py` & `flake8_bugbear-24.4.26/tests/b024.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b027.py` & `flake8_bugbear-24.4.26/tests/b027.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b030.py` & `flake8_bugbear-24.4.26/tests/b030.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b031.py` & `flake8_bugbear-24.4.26/tests/b031.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b034.py` & `flake8_bugbear-24.4.26/tests/b034.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b035.py` & `flake8_bugbear-24.4.26/tests/b035.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b036.py` & `flake8_bugbear-24.4.26/tests/b036.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b037.py` & `flake8_bugbear-24.4.26/tests/b037.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b901.py` & `flake8_bugbear-24.4.26/tests/b901.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b902.py` & `flake8_bugbear-24.4.26/tests/b902.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b902_extended.py` & `flake8_bugbear-24.4.26/tests/b902_extended.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b902_py38.py` & `flake8_bugbear-24.4.26/tests/b902_py38.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b903.py` & `flake8_bugbear-24.4.26/tests/b903.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b904.py` & `flake8_bugbear-24.4.26/tests/b904.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b905_py310.py` & `flake8_bugbear-24.4.26/tests/b905_py310.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b906.py` & `flake8_bugbear-24.4.26/tests/b906.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b907.py` & `flake8_bugbear-24.4.26/tests/b907.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b908.py` & `flake8_bugbear-24.4.26/tests/b908.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/b909.py` & `flake8_bugbear-24.4.26/tests/b909.py`

 * *Files 17% similar despite different names*

```diff
@@ -123,7 +123,30 @@
 # should error (?)
 for _ in foo:
     foo.remove(1)
     if bar:
         bar.remove(1)
         break
     break
+
+lst: list[dict] = [{}, {}, {}]
+for dic in lst:
+    dic["key"] = False # no error
+
+
+
+for grammar in grammars:
+    errors[grammar.version] = InvalidInput() # no error
+
+
+
+for key in self.hpo_params:
+    if key in nni_config:
+        nni_config[key] = self.hpo_params[key] # no error
+
+
+some_dict = {"foo": "bar"}
+for key in some_dict:
+    some_dict[key] = 3 # no error
+
+for key in some_dict.keys():
+    some_dict[key] = 3 # no error
```

### Comparing `flake8_bugbear-24.4.21/tests/b950.py` & `flake8_bugbear-24.4.26/tests/b950.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tests/test_bugbear.py` & `flake8_bugbear-24.4.26/tests/test_bugbear.py`

 * *Files identical despite different names*

### Comparing `flake8_bugbear-24.4.21/tox.ini` & `flake8_bugbear-24.4.26/tox.ini`

 * *Files identical despite different names*

