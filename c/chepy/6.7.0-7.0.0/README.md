# Comparing `tmp/chepy-6.7.0.tar.gz` & `tmp/chepy-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chepy-6.7.0.tar", last modified: Tue Mar 19 04:10:33 2024, max compression
+gzip compressed data, was "dist/chepy-7.0.0.tar", last modified: Fri Apr 26 02:27:45 2024, max compression
```

## Comparing `chepy-6.7.0.tar` & `chepy-7.0.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:10:33.000000 chepy-6.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-19 04:10:31.000000 chepy-6.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-03-19 04:10:33.000000 chepy-6.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-03-19 04:10:31.000000 chepy-6.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:10:33.000000 chepy-6.7.0/chepy/
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13262 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    52291 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:10:33.000000 chepy-6.7.0/chepy/extras/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/extras/bruteforce.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/extras/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/extras/combinatons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/extras/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/extras/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:10:33.000000 chepy-6.7.0/chepy/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/aritmeticlogic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/codetidy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14496 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)    65398 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/dataformat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/datetimemodule.py
--rw-r--r--   0 runner    (1001) docker     (127)    61373 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/encryptionencoding.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    22637 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)    17679 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:10:33.000000 chepy-6.7.0/chepy/modules/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8250 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/internal/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/internal/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    59599 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/internal/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/internal/ls47.py
--rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/internal/rison.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/networking.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/other.py
--rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/publickey.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    23366 2024-03-19 04:10:31.000000 chepy-6.7.0/chepy/modules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:10:33.000000 chepy-6.7.0/chepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-03-19 04:10:33.000000 chepy-6.7.0/chepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-19 04:10:33.000000 chepy-6.7.0/chepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 04:10:33.000000 chepy-6.7.0/chepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-19 04:10:33.000000 chepy-6.7.0/chepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-19 04:10:33.000000 chepy-6.7.0/chepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-19 04:10:33.000000 chepy-6.7.0/chepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-19 04:10:31.000000 chepy-6.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-19 04:10:33.000000 chepy-6.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-19 04:10:31.000000 chepy-6.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:10:33.000000 chepy-6.7.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:10:33.000000 chepy-6.7.0/tests/test_extras/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 04:10:32.000000 chepy-6.7.0/tests/test_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-19 04:10:32.000000 chepy-6.7.0/tests/test_extras/test_bruteforce.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-19 04:10:32.000000 chepy-6.7.0/tests/test_extras/test_characters.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-19 04:10:32.000000 chepy-6.7.0/tests/test_extras/test_combinations.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-19 04:10:32.000000 chepy-6.7.0/tests/test_extras/test_crypto_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-19 04:10:32.000000 chepy-6.7.0/tests/test_extras/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:27:45.000000 chepy-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 02:27:43.000000 chepy-7.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-26 02:27:45.000000 chepy-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-26 02:27:43.000000 chepy-7.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:27:45.000000 chepy-7.0.0/chepy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13262 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52341 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:27:45.000000 chepy-7.0.0/chepy/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/extras/bruteforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/extras/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/extras/combinatons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/extras/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/extras/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:27:45.000000 chepy-7.0.0/chepy/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8296 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/aritmeticlogic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/codetidy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14496 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66858 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/dataformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/datetimemodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64483 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/encryptionencoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22637 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17679 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:27:45.000000 chepy-7.0.0/chepy/modules/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/internal/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/internal/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59599 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/internal/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/internal/ls47.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/internal/rison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/publickey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23366 2024-04-26 02:27:43.000000 chepy-7.0.0/chepy/modules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:27:45.000000 chepy-7.0.0/chepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-26 02:27:45.000000 chepy-7.0.0/chepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-26 02:27:45.000000 chepy-7.0.0/chepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 02:27:45.000000 chepy-7.0.0/chepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 02:27:45.000000 chepy-7.0.0/chepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-26 02:27:45.000000 chepy-7.0.0/chepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 02:27:45.000000 chepy-7.0.0/chepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-26 02:27:43.000000 chepy-7.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-26 02:27:45.000000 chepy-7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-26 02:27:43.000000 chepy-7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:27:45.000000 chepy-7.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:27:45.000000 chepy-7.0.0/tests/test_extras/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 02:27:43.000000 chepy-7.0.0/tests/test_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-26 02:27:43.000000 chepy-7.0.0/tests/test_extras/test_bruteforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-26 02:27:43.000000 chepy-7.0.0/tests/test_extras/test_characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-26 02:27:43.000000 chepy-7.0.0/tests/test_extras/test_combinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-26 02:27:43.000000 chepy-7.0.0/tests/test_extras/test_crypto_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-26 02:27:43.000000 chepy-7.0.0/tests/test_extras/test_misc.py
```

### Comparing `chepy-6.7.0/PKG-INFO` & `chepy-7.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chepy
-Version: 6.7.0
+Version: 7.0.0
 Summary: UNKNOWN
 Home-page: https://github.com/securisec/chepy
 Author: @securisec
 License: GPL
 Project-URL: Documentation, https://chepy.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/securisec/chepy
 Description: <p align="center">
@@ -76,19 +76,18 @@
         - Chepy CLI has full autocompletion.
         - Supports pe, elf, and other various file format specific parsing.  
         - Extendable via [plugins](https://chepy-plugins.readthedocs.io/en/latest/)
         - Infinitely scalable as it can leverage the full Python library.
         - Chepy can interface with the full Cyberchef web app to a certain degree. It is easy to move from Chepy to Cyberchef if need be. 
         - The Chepy python library is significantly faster than the Cyberchef Node library.
         - Works with HTTP/S requests without CORS issues.
+        - `magic` support via the Chepy ML plugin.
         
         #### Disadvantages
-        - Chepy is not a web app (at least for now).
         - Chepy does not offer every single thing that Cyberchef does
-        - Chepy does not have the `magic` method (at the moment)
         
         
         ## Installation
         Chepy can be installed in a few ways.
         
         ### Pypi
         ```bash
@@ -151,10 +150,10 @@
         * :ref:`genindex`
         * :ref:`modindex`
         * :ref:`search`
         ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: ==3.10.*
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: extras
```

### Comparing `chepy-6.7.0/README.md` & `chepy-7.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -67,19 +67,18 @@
 - Chepy CLI has full autocompletion.
 - Supports pe, elf, and other various file format specific parsing.  
 - Extendable via [plugins](https://chepy-plugins.readthedocs.io/en/latest/)
 - Infinitely scalable as it can leverage the full Python library.
 - Chepy can interface with the full Cyberchef web app to a certain degree. It is easy to move from Chepy to Cyberchef if need be. 
 - The Chepy python library is significantly faster than the Cyberchef Node library.
 - Works with HTTP/S requests without CORS issues.
+- `magic` support via the Chepy ML plugin.
 
 #### Disadvantages
-- Chepy is not a web app (at least for now).
 - Chepy does not offer every single thing that Cyberchef does
-- Chepy does not have the `magic` method (at the moment)
 
 
 ## Installation
 Chepy can be installed in a few ways.
 
 ### Pypi
 ```bash
```

### Comparing `chepy-6.7.0/chepy/__init__.py` & `chepy-7.0.0/chepy/__init__.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/__main__.py` & `chepy-7.0.0/chepy/__main__.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/config.py` & `chepy-7.0.0/chepy/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,9 +131,9 @@
 
             for plugin in my_plugins:
                 try:
                     klass, mod = inspect.getmembers(plugin, inspect.isclass)[0]
                     loaded = getattr(plugin, klass)
                     plugins.append(loaded)
                 except:
-                    logging.warning("Error loading {}".format(plugin.__name__))
+                    logging.warning(f"Error loading {plugin.__name__}")
         return plugins
```

### Comparing `chepy-6.7.0/chepy/core.py` & `chepy-7.0.0/chepy/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 class ChepyCore(object):
     """The ChepyCore class for Chepy is primarily used as an interface
     for all the current modules/classes in Chepy, or for plugin development.
     The `ChepyCore` class is what provides the various attributes like **states**,
     **buffers**, etc and is required to use and extend Chepy.
 
     Args:
-        \*data (tuple): The core class takes arbitrary number of arguments as \*args.
+        *data (tuple): The core class takes arbitrary number of arguments as *args.
 
     Attributes:
         states (dict): Contains all the current states. Each arg passed to
             the ChepyCore class will be considered a state.
         buffers (dict): Contains all the current buffers if a buffer is saved.
         state (Any): The data in the current state. The state changes each time a
             Chepy method is called.
@@ -923,15 +923,15 @@
     def load_from_url(
         self,
         method: str = "GET",
         params: dict = {},
         json: dict = None,
         headers: dict = {},
         cookies: dict = {},
-    ):
+    ):  # pragma: no cover
         """Load binary content from a url
 
         Most common http methods are supported; but some methods may not provide a response body.
 
         Args:
             method (str, optional): Request method. Defaults to 'GET'.
             params (dict, optional): Query Args. Defaults to {}.
@@ -1465,14 +1465,15 @@
         # dont run if from cli
         if sys.stdout.isatty():  # pragma: no cover
             logging.warning("callback cannot be used via the cli")
             return self
         self.state = callback_function(self.state)
         return self
 
+    @ChepyDecorators.call_stack
     def register(
         self,
         pattern: Union[str, bytes],
         ignore_case: bool = False,
         multiline: bool = False,
         dotall: bool = False,
         unicode: bool = False,
```

### Comparing `chepy-6.7.0/chepy/extras/bruteforce.py` & `chepy-7.0.0/chepy/extras/bruteforce.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/extras/characters.py` & `chepy-7.0.0/chepy/extras/characters.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/extras/combinatons.py` & `chepy-7.0.0/chepy/extras/combinatons.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/extras/crypto.py` & `chepy-7.0.0/chepy/extras/crypto.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/extras/misc.py` & `chepy-7.0.0/chepy/extras/misc.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/modules/aritmeticlogic.py` & `chepy-7.0.0/chepy/modules/networking.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,251 +1,227 @@
-import binascii
-import statistics
-from typing import TypeVar, Union
-from functools import reduce as functools_reduce
+import collections
+import ipaddress
+import socket
+import ssl
+import urllib.parse as _py_urlparse
+from typing import TypeVar
 
-from ..core import ChepyCore, ChepyDecorators
-from .exceptions import StateNotList
-from .internal.helpers import detect_delimiter
+import regex as re
 
+from ..core import ChepyCore, ChepyDecorators
 
-AritmeticLogicT = TypeVar("AritmeticLogicT", bound="AritmeticLogic")
+NetworkingT = TypeVar("NetworkingT", bound="Networking")
 
 
-class AritmeticLogic(ChepyCore):
+class Networking(ChepyCore):
     def __init__(self, *data):
         super().__init__(*data)
 
-    def __hex_to_int(self, n):  # pragma: no cover
-        if isinstance(n, str):
-            return int(n, 0)
-        if isinstance(n, int):
-            return n
-
     @ChepyDecorators.call_stack
-    def str_bit_shift_right(self, amount: int) -> AritmeticLogicT:
-        """Bit shift string right
+    def defang_url(self) -> NetworkingT:
+        """Make a URL harmless
 
-        Args:
-            amount (int): Amount to shift
+        Takes a Universal Resource Locator (URL) and 'Defangs' it;
+        meaning the URL becomes invalid, neutralising the risk of accidentally
+        clicking on a malicious link. This is often used when dealing with
+        malicious links or IOCs.
 
         Returns:
-            Chepy: The Chepy object
+            Chepy: The Chepy object.
+
+        Examples:
+            >>> Chepy("https://app.google.com/?lol=some data&a=1").defang_url().o
+            "hxxps://app[.]google[.]com/?lol=some data&a=1"
         """
-        self.state = binascii.unhexlify(
-            "".join(list(format(ord(x) >> int(amount), "02x") for x in list("hello")))
-        )
+        self.state = re.sub(r"(^htt)", "hxx", self._convert_to_str())
+        self.state = re.sub(r"\.", "[.]", self._convert_to_str())
         return self
 
     @ChepyDecorators.call_stack
-    def add(self, n: int) -> AritmeticLogicT:
-        """Add a number to the state
-
-        Args:
-            n (int): Number to add with. Can be decimal or hex string without 0x
+    def refang_url(self) -> NetworkingT:
+        """Refangs a URL so that it is clickable
 
         Returns:
             Chepy: The Chepy object.
-        """
-        # Determine the base of the key (hexadecimal or decimal)
-        if isinstance(n, int):
-            # Try converting to decimal
-            key_int = n
-        else:
-            try:
-                # Try converting to hexadecimal
-                key_int = int(n, 16)
-            except ValueError:  # pragma: no cover
-                self._log.error(
-                    "Invalid key format. Must be a decimal or hexadecimal string."
-                )
-                return self
 
-        hold = b""
-        for char_code in self._convert_to_bytes():
-            # Add the key to the integer and take the result modulo 255
-            result_code = (char_code + key_int) % 256
-
-            # Convert the result back to a byte
-            hold += result_code.to_bytes(1, byteorder="big")
-
-        self.state = hold
+        Examples:
+            >>> Chepy("hxxps://app[.]google[.]com/?lol=some data&a=1").refang_url().o
+            "https://app.google.com/?lol=some data&a=1"
+        """
+        self.state = re.sub(r"(^hxx)", "htt", self._convert_to_str())
+        self.state = re.sub(r"\[\.\]", ".", self._convert_to_str())
         return self
 
     @ChepyDecorators.call_stack
-    def addition(self, delimiter=None) -> AritmeticLogicT:
-        """Adds a list of numbers. If an item in the string is not a number it is excluded from the list.
+    def defang_ip(self) -> NetworkingT:
+        """Make an IP address harmless
 
-        Args:
-            delimiter (str, optional): Delimiter. Defaults to None.
+        Takes a IPv4 or IPv6 address and 'Defangs' it, meaning the
+        IP becomes invalid, removing the risk of accidentally utilising
+        it as an IP address.
 
         Returns:
             Chepy: The Chepy object.
-        """
-        data = self._convert_to_str()
-        print('🟢 ', data)
-        if not delimiter:
-            delimiter = detect_delimiter(data)
-        # only work on numbers
-        nums = []
-        for n in data.split(delimiter):
-            try:
-                nums.append(int(n))
-            except:  # noqa: E722
-                continue
-
-        self.state = functools_reduce(lambda x, y: x + y, nums)
-        return self
 
-    @ChepyDecorators.call_stack
-    def sub(self, n: int) -> AritmeticLogicT:
-        """SUB the input with the given key
-
-        Args:
-            n (int): Number to subtract with
+        Examples:
+            >>> Chepy("2001:4860:4860::8844").defang_ip().o
+            "2001[:]4860[:]4860[:][:]8844"
 
-        Returns:
-            Chepy: The Chepy object.
+            >>> Chepy("127.0.0.1").defang_ip().o
+            "127[.]0[.]0[.]1"
         """
-        # Determine the base of the key (hexadecimal or decimal)
-        if isinstance(n, int):
-            # Try converting to decimal
-            key_int = n
+        if ":" in self._convert_to_str():
+            self.state = re.sub(r":", "[:]", self._convert_to_str())
         else:
-            try:
-                # Try converting to hexadecimal
-                key_int = int(n, 16)
-            except ValueError:  # pragma: no cover
-                self._log.error(
-                    "Invalid key format. Must be a decimal or hexadecimal string."
-                )
-                return self
-
-        hold = b""
-        for char_code in self._convert_to_bytes():
-            # Add the key to the integer and take the result modulo 255
-            result_code = (char_code - key_int) % 256
-
-            # Convert the result back to a byte
-            hold += result_code.to_bytes(1, byteorder="big")
-
-        self.state = hold
+            self.state = re.sub(r"\.|:", "[.]", self._convert_to_str())
         return self
 
     @ChepyDecorators.call_stack
-    def subtract(self, delimiter=None) -> AritmeticLogicT:
-        """Subtracts a list of numbers. If an item in the string is not a number it is excluded from the list.
-
-        Args:
-            delimiter (str, optional): Delimiter. Defaults to None.
+    def refang_ip(self) -> NetworkingT:
+        """Refangs an IP address
 
         Returns:
             Chepy: The Chepy object.
-        """
-        data = self._convert_to_str()
-        if not delimiter:
-            delimiter = detect_delimiter(data)
-        # only work on numbers
-        nums = []
-        for n in data.split(delimiter):
-            try:
-                nums.append(int(n))
-            except:  # noqa: E722
-                continue
-
-        self.state = functools_reduce(lambda x, y: x - y, nums)
-        return self
-
-    @ChepyDecorators.call_stack
-    def multiply(self, n: int) -> AritmeticLogicT:
-        """Multiply a number to the state
-
-        Args:
-            n (int): Number to multiply with
 
-        Returns:
-            Chepy: The Chepy object.
+        Examples:
+            >>> Chepy("127[.]0[.]0[.]1").refang_ip().o
+            "127.0.0.1"
         """
-        if not isinstance(self.state, int):
-            self.state = self.__hex_to_int(self.state)
-        self.state = self.state * n
+        self.state = re.sub(r"\[\.\]|\[\:\]", ".", self._convert_to_str())
         return self
 
     @ChepyDecorators.call_stack
-    def divide(self, n: int) -> AritmeticLogicT:
-        """Divide a number to the state. Chepy is not optimized for float math.
-        Subsequent methods may fail.
-
-        Args:
-            n (int): Number to divide with
+    def parse_uri(self) -> NetworkingT:
+        """Parse a URI
 
         Returns:
             Chepy: The Chepy object.
+
+        Examples:
+            >>> Chepy("http://example.com/resource?foo=bar#fragment").parse_uri().o
+            {
+                "scheme": "http",
+                "location": "example.com",
+                "path": "/resource",
+                "params": "",
+                "query": {"foo": ["bar"]},
+                "fragment": "fragment",
+            }
         """
-        if not isinstance(self.state, int):
-            self.state = self.__hex_to_int(self.state)
-        self.state = self.state / n
+        parsed = _py_urlparse.urlparse(self._convert_to_str())
+        self.state = {
+            "scheme": parsed.scheme,
+            "location": parsed.netloc,
+            "path": parsed.path,
+            "params": parsed.params,
+            "query": _py_urlparse.parse_qs(parsed.query),
+            "fragment": parsed.fragment,
+        }
         return self
 
     @ChepyDecorators.call_stack
-    def power(self, n: int) -> AritmeticLogicT:
-        """Convert state to the n power of
-
-        Args:
-            n (int): Exponent
+    def parse_ip_range(self) -> NetworkingT:
+        """Enumerate IP address in a CIDR range
 
         Returns:
             Chepy: The Chepy object.
+
+        Examples:
+            >>> Chepy("10.10.10.1/24").parse_ip_range().o
+            [
+                "10.10.10.1",
+                "10.10.10.2,
+                ...
+                "10.10.10.254"
+            ]
         """
-        if not isinstance(self.state, int):
-            self.state = self.__hex_to_int(self.state)
-        self.state = self.state**n
+        self.state = [
+            str(i)
+            for i in ipaddress.ip_network(self._convert_to_str(), strict=False).hosts()
+        ]
         return self
 
     @ChepyDecorators.call_stack
-    def sum(self) -> AritmeticLogicT:
-        """Calculate the sum of the state
+    def parse_ipv6(self) -> NetworkingT:
+        """Get longhand and shorthand of IPv6
 
         Returns:
             Chepy: The Chepy object.
+
+        Examples:
+            >>> Chepy("2001:4860:4860::8888").parse_ipv6().o
+            {
+                "long": "2001:4860:4860:0000:0000:0000:0000:8888",
+                "short": "2001:4860:4860::8888",
+            }
         """
-        assert isinstance(self.state, list), StateNotList()
-        numbers = list(self.__hex_to_int(x) for x in self.state)
-        self.state = sum(numbers)
+        ip = ipaddress.ip_address(self._convert_to_str())
+        self.state = {"long": ip.exploded, "short": ip.compressed}
         return self
 
     @ChepyDecorators.call_stack
-    def mean(self) -> AritmeticLogicT:
-        """Calculate the mean of the state
+    def get_ssl_cert(self, port: int = 443) -> NetworkingT:
+        """Get the server side SSL certificate for a domain
+
+        Args:
+            port (int, optional): Server port. Defaults to 443.
 
         Returns:
-            Chepy: The Chepy object.
-        """
-        assert isinstance(self.state, list), StateNotList()
-        numbers = list(self.__hex_to_int(x) for x in self.state)
-        self.state = statistics.mean(numbers)
-        return self
+            Chepy: The Chepy object
+
+        Examples:
+            >>> Chepy('google.com').get_ssl_cert().o
+            {
+                'subject': {
+                    'commonName': '*.google.com',
+                    'organizationName': 'Google LLC',
+                ...
+                'caIssuers': ('http://pki.goog/gsr2/GTS1O1.crt',),
+                'crlDistributionPoints': ('http://crl.pki.goog/GTS1O1.crl',)
+            }
+        """
+        domain = re.sub("^\w+://", "", self._convert_to_str())
+        with socket.create_connection((domain, port)) as sock:
+            context = ssl.create_default_context()
+            context.check_hostname = False
+            with context.wrap_socket(sock, server_hostname=domain) as sslsock:
+                cert = sslsock.getpeercert()
+                final = {}
+                for key in cert.keys():
+                    if key == "subject" or key == "issuer":
+                        final[key] = dict(
+                            collections.ChainMap(*list(map(dict, cert[key])))
+                        )
+                    elif key == "subjectAltName":
+                        final[key] = list(
+                            map(lambda x: dict([x]), cert["subjectAltName"])
+                        )
+                    else:
+                        final[key] = cert[key]
+                self.state = final
+                return self
 
     @ChepyDecorators.call_stack
-    def median(self) -> AritmeticLogicT:
-        """Calculate the median of the state
+    def int_to_ip(self) -> NetworkingT:
+        """Convert an integer to an IP address
 
         Returns:
             Chepy: The Chepy object.
+
+        Examples:
+            >>> Chepy(3232235777).int_to_ip().o
         """
-        assert isinstance(self.state, list), StateNotList()
-        numbers = list(self.__hex_to_int(x) for x in self.state)
-        self.state = statistics.median(numbers)
+        self.state = str(ipaddress.ip_address(self._convert_to_int()))
         return self
 
     @ChepyDecorators.call_stack
-    def int_to_base(self, base: Union[int, str]) -> AritmeticLogicT:
-        """Convert the state to a different base
-
-        Args:
-            base (int): Base to convert to
+    def ip_to_int(self) -> NetworkingT:
+        """Convert an integer to an IP address
 
         Returns:
             Chepy: The Chepy object.
+
+        Examples:
+            >>> Chepy(3232235777).int_to_ip().o
         """
-        self.state = int(self.state, base)
-        return self
+        self.state = int(ipaddress.ip_address(self._convert_to_str()))
+        return self
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `chepy-6.7.0/chepy/modules/codetidy.py` & `chepy-7.0.0/chepy/modules/codetidy.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/modules/compression.py` & `chepy-7.0.0/chepy/modules/compression.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/modules/dataformat.py` & `chepy-7.0.0/chepy/modules/dataformat.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from random import randint
 from .internal.constants import Encoding
 from .internal.helpers import (
     detect_delimiter,
     Rotate,
     Uint1Array,
     UUEncoderDecoder,
+    Base92,
+    Base45,
 )
 
 yaml = lazy_import.lazy_module("yaml")
 import regex as re
 import hexdump
 from ast import literal_eval
 from typing import TypeVar, Union, List, Literal
@@ -317,29 +319,74 @@
             >>> Chepy("some data").base32_encode().out.decode()
             "ONXW2ZJAMRQXIYI="
         """
         self.state = base64.b32encode(self._convert_to_bytes())
         return self
 
     @ChepyDecorators.call_stack
-    def from_base32(self) -> DataFormatT:
+    def from_base32(self, remove_whitespace: bool = True) -> DataFormatT:
         """Decode as Base32
 
         Base32 is a notation for encoding arbitrary byte data using a
         restricted set of symbols that can be conveniently used by humans
         and processed by computers. It uses a smaller set of characters than
         Base64, usually the uppercase alphabet and the numbers 2 to 7.
 
+        Args:
+            remove_whitespace(bool, optional): If true, all whitespaces are removed
+
         Returns:
             Chepy: The Chepy object.
         """
+        if remove_whitespace:
+            self.state = self.remove_whitespace().o
         self.state = base64.b32decode(self.state)
         return self
 
     @ChepyDecorators.call_stack
+    def to_base92(self) -> DataFormatT:
+        """Encode to Base92
+
+        Returns:
+            Chepy: The Chepy object.
+        """
+        self.state = Base92.b92encode(self._convert_to_bytes())
+        return self
+
+    @ChepyDecorators.call_stack
+    def from_base92(self) -> DataFormatT:
+        """Decode from Base92
+
+        Returns:
+            Chepy: The Chepy object.
+        """
+        self.state = Base92.b92decode(self._convert_to_str())
+        return self
+
+    @ChepyDecorators.call_stack
+    def to_base45(self) -> DataFormatT:
+        """Encode to Base45
+
+        Returns:
+            Chepy: The Chepy object.
+        """
+        self.state = Base45().b45encode(self._convert_to_bytes())
+        return self
+
+    @ChepyDecorators.call_stack
+    def from_base45(self) -> DataFormatT:
+        """Decode from Base45
+
+        Returns:
+            Chepy: The Chepy object.
+        """
+        self.state = Base45().b45decode(self._convert_to_bytes())
+        return self
+
+    @ChepyDecorators.call_stack
     def to_base91(self) -> DataFormatT:  # pragma: no cover
         """Base91 encode
         Reference: https://github.com/aberaud/base91-python/blob/master/base91.py#L69
 
         Returns:
             Chepy: The Chepy object.
         """
@@ -481,36 +528,41 @@
                 "utf-8",
             )
         else:
             self.state = base64.b64encode(self._convert_to_bytes())
         return self
 
     @ChepyDecorators.call_stack
-    def from_base64(self, custom: str = None, url_safe: bool = False) -> DataFormatT:
+    def from_base64(
+        self, custom: str = None, url_safe: bool = False, remove_whitespace: bool = True
+    ) -> DataFormatT:
         """Decode as Base64
 
         Base64 is a notation for encoding arbitrary byte data using a
         restricted set of symbols that can be conveniently used by humans
         and processed by computers.This property decodes raw data
         into an ASCII Base64 string.
 
         Args:
             custom (str, optional): Provide a custom charset to base64 with
             url_safe (bool, optional): If true, decode url safe. Defaults to False
+            remove_whitespace(bool, optional): If true, all whitespaces are removed
 
         Returns:
             Chepy: The Chepy object.
 
         Examples:
             Base64 decode using a custom string
             >>> c = Chepy("QqxhNG/mMKtYPqoz64FVR42=")
             >>> c.from_base64(custom="./0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz")
             >>> c.out
             b"some random? data"
         """
+        if remove_whitespace:
+            data = self.remove_whitespace().o
         data = self._convert_to_str()
         if custom is not None:
             std_base64chars = (
                 "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/="
             )
             data = data.translate(str.maketrans(custom, std_base64chars))
         data += "=="
@@ -550,15 +602,15 @@
         if delimiter == "":
             self.state = binascii.hexlify(self._convert_to_bytes())
         else:
             self.state = binascii.hexlify(self._convert_to_bytes(), sep=delimiter)
         return self
 
     @ChepyDecorators.call_stack
-    def from_hex(self, delimiter: str = None, join_by: str = " ") -> DataFormatT:
+    def from_hex(self, delimiter: str = None, join_by: str = "") -> DataFormatT:
         """Convert a non delimited hex string to string
 
         Args:
             delimiter (str, optional): Delimiter. Defaults to None.
             join_by (str, optional): Join by. Defaults to ' '.
 
         Returns:
```

### Comparing `chepy-6.7.0/chepy/modules/datetimemodule.py` & `chepy-7.0.0/chepy/modules/datetimemodule.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/modules/encryptionencoding.py` & `chepy-7.0.0/chepy/modules/encryptionencoding.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,17 +80,17 @@
         # modify iv according to mode
         iv = self._str_to_bytes(iv)
         if iv_format == "hex":
             iv = binascii.unhexlify(iv)
         if iv_format == "base64" or iv_format == "b64":
             iv = base64.b64decode(iv)
         if iv_format == "utf-8" or iv_format == "utf8":
-            iv = key.decode().encode("utf-8")
+            iv = iv.decode().encode("utf-8")
         if iv_format == "latin-1":
-            iv = key.decode().encode("latin-1")
+            iv = iv.decode().encode("latin-1")
         if iv_format == "raw":
             iv = iv
         else:
             iv = binascii.unhexlify(binascii.hexlify(iv))
         return key, iv
 
     def _rsa_process_key(self, key: str, is_file: bool, passphrase=None):
@@ -317,15 +317,14 @@
         x = bytearray(b"")
         # check if state is a list and keys are list
         if isinstance(self.state, bytearray) and isinstance(key, bytearray):
             for char, key_val in zip(self.state, itertools.cycle(key)):
                 x.append(char ^ key_val)
 
         else:
-
             if key_type == "utf":
                 key = str(key)
                 key = binascii.hexlify(key.encode())
             elif key_type == "base64":
                 key = binascii.hexlify(base64.b64decode(key.encode()))
             elif key_type == "decimal":
                 key = binascii.hexlify(
@@ -798,34 +797,42 @@
             >>> c = Chepy("f8b27a0d8c837edce87dd13a1ab41f96")
             >>> c.hex_to_str()
             >>> c.triple_des_decrypt("super secret password !!")
             >>> c.o
             b"some data"
         """
 
-        self.__check_mode(mode)
-
         key, iv = self._convert_key(key, iv, key_format, iv_format)
 
         if mode == "CBC":
             cipher = DES3.new(key, mode=DES3.MODE_CBC, iv=iv)
             self.state = Padding.unpad(cipher.decrypt(self._convert_to_bytes()), 8)
             return self
+        elif mode == "CBC/NoPadding":
+            cipher = DES3.new(key, mode=DES3.MODE_CBC, iv=iv)
+            self.state = cipher.decrypt(self._convert_to_bytes())
+            return self
         elif mode == "ECB":
             cipher = DES3.new(key, mode=DES3.MODE_ECB)
             self.state = Padding.unpad(cipher.decrypt(self._convert_to_bytes()), 8)
             return self
+        elif mode == "ECB/NoPadding":
+            cipher = DES3.new(key, mode=DES3.MODE_ECB)
+            self.state = cipher.decrypt(self._convert_to_bytes())
+            return self
         elif mode == "CTR":
             cipher = DES3.new(key, mode=DES3.MODE_CTR, nonce=b"")
             self.state = cipher.decrypt(self._convert_to_bytes())
             return self
         elif mode == "OFB":
             cipher = DES3.new(key, mode=DES3.MODE_OFB, iv=iv)
             self.state = cipher.decrypt(self._convert_to_bytes())
             return self
+        else:  # pragma: no cover
+            raise ValueError("Invalid mode")
 
     @ChepyDecorators.call_stack
     def aes_encrypt(
         self,
         key: str,
         iv: str = "00000000000000000000000000000000",
         mode: str = "CBC",
@@ -890,15 +897,15 @@
         self,
         key: str,
         iv: str = "00000000000000000000000000000000",
         mode: str = "CBC",
         key_format: str = "hex",
         iv_format: str = "hex",
     ) -> EncryptionEncodingT:
-        """Decrypt raw state encrypted with DES.
+        """Decrypt raw state encrypted with AES.
         CFB mode reflects Cyberchef and not native python behaviour.
 
         Args:
             key (str): Required. The secret key
             iv (str, optional): IV for certain modes only.
                 Defaults to '00000000000000000000000000000000'.
             mode (str, optional): Encryption mode. Defaults to 'CBC'.
@@ -912,30 +919,36 @@
             >>> c = Chepy("5fb8c186394fc399849b89d3b6605fa3")
             >>> c.hex_to_str()
             >>> c.aes_decrypt("7365637265742070617373776f726421")
             >>> c.o
             b"some data"
         """
 
-        assert mode in ["CBC", "CFB", "OFB", "CTR", "ECB", "GCM"], "Not a valid mode."
-
         key, iv = self._convert_key(key, iv, key_format, iv_format)
 
         if mode == "CBC":
             cipher = AES.new(key, mode=AES.MODE_CBC, iv=iv)
             self.state = Padding.unpad(cipher.decrypt(self._convert_to_bytes()), 16)
             return self
-        if mode == "CFB":
+        elif mode == "CBC/NoPadding":
+            cipher = AES.new(key, mode=AES.MODE_CBC, iv=iv)
+            self.state = cipher.decrypt(self._convert_to_bytes())
+            return self
+        elif mode == "CFB":
             cipher = AES.new(key, mode=AES.MODE_CFB, iv=iv, segment_size=128)
             self.state = cipher.decrypt(self._convert_to_bytes())
             return self
         elif mode == "ECB":
             cipher = AES.new(key, mode=AES.MODE_ECB)
             self.state = Padding.unpad(cipher.decrypt(self._convert_to_bytes()), 16)
             return self
+        elif mode == "ECB/NoPadding":
+            cipher = AES.new(key, mode=AES.MODE_ECB)
+            self.state = cipher.decrypt(self._convert_to_bytes())
+            return self
         elif mode == "CTR":
             counter = Counter.new(128, initial_value=int.from_bytes(iv, "big"))
             cipher = AES.new(key, mode=AES.MODE_CTR, counter=counter)
             self.state = cipher.decrypt(self._convert_to_bytes())
             return self
         elif mode == "GCM":
             cipher = AES.new(
@@ -945,14 +958,16 @@
             )
             self.state = cipher.decrypt(self._convert_to_bytes())
             return self
         elif mode == "OFB":
             cipher = AES.new(key, mode=AES.MODE_OFB, iv=iv)
             self.state = cipher.decrypt(self._convert_to_bytes())
             return self
+        else:  # pragma: no cover
+            raise ValueError("Invalid AES mode")
 
     @ChepyDecorators.call_stack
     def blowfish_encrypt(
         self,
         key: str,
         iv: str = "0000000000000000",
         mode: str = "CBC",
@@ -1104,14 +1119,15 @@
         Returns:
             Chepy: The Chepy object.
         """
         input_str = self._convert_to_str()
         alphabet = "abcdefghijklmnopqrstuvwxyz"
         output = ""
         fail = 0
+        key = key.lower()
 
         if not key:
             raise ValueError("No key entered")  # pragma: no cover
         if not key.isalpha():
             raise ValueError("The key must consist only of letters")  # pragma: no cover
 
         for i in range(len(input_str)):
@@ -1501,15 +1517,15 @@
             hold.append(f"{d}{i}".encode())
         random.shuffle(hold)
         self.state = join_by.join(hold)
         return self
 
     @ChepyDecorators.call_stack
     def from_letter_number_code(
-        self, delimiter: Union[str, bytes] = ' ', join_by: Union[str, bytes] = ""
+        self, delimiter: Union[str, bytes] = " ", join_by: Union[str, bytes] = ""
     ) -> EncryptionEncodingT:
         """Decode A1Z26
 
         Args:
             delimiter (Union[str, bytes], optional): Split on. Defaults to ' '.
             join_by (Union[str, bytes], optional): Join output by. Defaults to ''.
 
@@ -1572,16 +1588,16 @@
 
         Returns:
             Chepy: The Chepy object.
         """
         key = self._bytes_to_str(key)
         key = "".join(re.findall(r"[A-Z]+", key))
         keyword_str = key.upper().replace("J", "I")
-        keyword_set = set(keyword_str)
-        keyword_list = []
+        # keyword_set = set(keyword_str)
+        # keyword_list = []
         alpha = "ABCDEFGHIKLMNOPQRSTUVWXYZ"
         x_co = []
         y_co = []
         structure = []
 
         output = ""
         count = 0
@@ -1634,15 +1650,15 @@
 
         Returns:
             Chepy: The Chepy object.
         """
         key = self._bytes_to_str(key)
         key = "".join(re.findall(r"[A-Z]+", key))
         keyword_str = key.upper().replace("J", "I")
-        keyword_set = set(keyword_str)
+        # keyword_set = set(keyword_str)
         alpha = "ABCDEFGHIKLMNOPQRSTUVWXYZ"
         structure = []
 
         output = ""
         count = 0
         trans = ""
 
@@ -1815,7 +1831,77 @@
         """
         key = self._str_to_bytes(key)
         if encode_key:
             key = base64.b64encode(key)
         out = Fernet(key).decrypt(self._convert_to_bytes())
         self.state = out
         return self
+
+    @ChepyDecorators.call_stack
+    def railfence_encode(self, key=2, offset=0) -> EncryptionEncodingT:
+        """Encode to railfence
+
+        Args:
+            key (int, optional): Key. Should be equal or larger than data. Defaults to 2.
+            offset (int, optional): Offset. Defaults to 0.
+
+        Returns:
+            Chepy: The Chepy object.
+        """
+        key, offset = int(key), int(offset)
+        data = self._convert_to_str()
+        if key < 2:
+            raise ValueError("Key has to be bigger than 2")  # pragma: no cover
+        elif key > len(data):
+            raise ValueError(
+                "Key should be smaller than the plain text's length"
+            )  # pragma: no cover
+
+        if offset < 0:
+            raise ValueError("Offset has to be a positive integer")  # pragma: no cover
+
+        cycle = (key - 1) * 2
+        rows = [""] * key
+
+        for pos in range(len(data)):
+            row_idx = key - 1 - abs(cycle // 2 - (pos + offset) % cycle)
+            rows[row_idx] += data[pos]
+
+        self.state = "".join(rows).strip()
+        return self
+
+    @ChepyDecorators.call_stack
+    def railfence_decode(self, key=2, offset=0) -> EncryptionEncodingT:
+        """Decode railfence
+
+        Args:
+            key (int, optional): Key. Should be equal or larger than data. Defaults to 2.
+            offset (int, optional): Offset. Defaults to 0.
+
+        Returns:
+            Chepy: The Chepy object.
+        """
+        key, offset = int(key), int(offset)
+        cipher = self._convert_to_str()
+
+        if key < 2:
+            raise ValueError("Key has to be bigger than 2")  # pragma: no cover
+        elif key > len(cipher):
+            raise ValueError(
+                "Key should be smaller than the cipher's length"
+            )  # pragma: no cover
+
+        if offset < 0:
+            raise ValueError("Offset has to be a positive integer")  # pragma: no cover
+
+        cycle = (key - 1) * 2
+        plaintext = [""] * len(cipher)
+
+        j = 0
+        for y in range(key):
+            for x in range(len(cipher)):
+                if (y + x + offset) % cycle == 0 or (y - x - offset) % cycle == 0:
+                    plaintext[x] = cipher[j]
+                    j += 1
+
+        self.state = "".join(plaintext).strip()
+        return self
```

### Comparing `chepy-6.7.0/chepy/modules/extractors.py` & `chepy-7.0.0/chepy/modules/extractors.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/modules/hashing.py` & `chepy-7.0.0/chepy/modules/hashing.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/modules/internal/cli.py` & `chepy-7.0.0/chepy/modules/internal/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import sys
 import inspect
 import regex as re
 import pprint
 
-import editor
 from docstring_parser import parse as _parse_doc
 from prompt_toolkit.completion import Completer, Completion
 from prompt_toolkit import print_formatted_text
 from prompt_toolkit.styles import Style
 from prompt_toolkit.formatted_text import FormattedText
 
 from chepy import Chepy
@@ -76,23 +75,23 @@
     """Get docs for a method"""
     try:
         print(yellow(getattr(Chepy, method).__doc__))
     except:
         print(red(pprint.pformat("Could not find docs...")))
 
 
-def cli_edit_state(fire: object, args: list):
-    """Edit the current state
+# def cli_edit_state(fire: object, args: list):
+#     """Edit the current state
 
-    Args:
-        args (object): Cli args
-    """
-    current_index = fire._current_index
-    hold = editor.edit(contents=str(fire.states[current_index])).decode()
-    args[current_index] = hold
+#     Args:
+#         args (object): Cli args
+#     """
+#     current_index = fire._current_index
+#     hold = editor.edit(contents=str(fire.states[current_index])).decode()
+#     args[current_index] = hold
 
 
 def cli_highlight(fire: object, highlight: str):
     """Highlight regex match for cli
     
     Args:
         fire (object): The fire object.
```

### Comparing `chepy-6.7.0/chepy/modules/internal/colors.py` & `chepy-7.0.0/chepy/modules/internal/colors.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/modules/internal/constants.py` & `chepy-7.0.0/chepy/modules/internal/constants.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/modules/internal/ls47.py` & `chepy-7.0.0/chepy/modules/internal/ls47.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/modules/internal/rison.py` & `chepy-7.0.0/chepy/modules/internal/rison.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/modules/language.py` & `chepy-7.0.0/chepy/modules/language.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/modules/links.py` & `chepy-7.0.0/chepy/modules/links.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/modules/other.py` & `chepy-7.0.0/chepy/modules/other.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/modules/publickey.py` & `chepy-7.0.0/chepy/modules/publickey.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/modules/search.py` & `chepy-7.0.0/chepy/modules/search.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy/modules/utils.py` & `chepy-7.0.0/chepy/modules/utils.py`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/chepy.egg-info/PKG-INFO` & `chepy-7.0.0/chepy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chepy
-Version: 6.7.0
+Version: 7.0.0
 Summary: UNKNOWN
 Home-page: https://github.com/securisec/chepy
 Author: @securisec
 License: GPL
 Project-URL: Documentation, https://chepy.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/securisec/chepy
 Description: <p align="center">
@@ -76,19 +76,18 @@
         - Chepy CLI has full autocompletion.
         - Supports pe, elf, and other various file format specific parsing.  
         - Extendable via [plugins](https://chepy-plugins.readthedocs.io/en/latest/)
         - Infinitely scalable as it can leverage the full Python library.
         - Chepy can interface with the full Cyberchef web app to a certain degree. It is easy to move from Chepy to Cyberchef if need be. 
         - The Chepy python library is significantly faster than the Cyberchef Node library.
         - Works with HTTP/S requests without CORS issues.
+        - `magic` support via the Chepy ML plugin.
         
         #### Disadvantages
-        - Chepy is not a web app (at least for now).
         - Chepy does not offer every single thing that Cyberchef does
-        - Chepy does not have the `magic` method (at the moment)
         
         
         ## Installation
         Chepy can be installed in a few ways.
         
         ### Pypi
         ```bash
@@ -151,10 +150,10 @@
         * :ref:`genindex`
         * :ref:`modindex`
         * :ref:`search`
         ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: ==3.10.*
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: extras
```

### Comparing `chepy-6.7.0/chepy.egg-info/SOURCES.txt` & `chepy-7.0.0/chepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chepy-6.7.0/setup.py` & `chepy-7.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     },
     extras_require={"extras": core_extra_deps + plugin_deps},
     packages=find_packages(exclude=(["tests", "docs"])),
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3.10",
     ],
-    python_requires="==3.10.*",
+    python_requires=">=3.10",
     entry_points={"console_scripts": ["chepy = chepy.__main__:main"]},
 )
```

### Comparing `chepy-6.7.0/tests/test_extras/test_characters.py` & `chepy-7.0.0/tests/test_extras/test_characters.py`

 * *Files identical despite different names*

