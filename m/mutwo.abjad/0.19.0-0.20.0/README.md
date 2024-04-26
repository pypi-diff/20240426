# Comparing `tmp/mutwo.abjad-0.19.0.tar.gz` & `tmp/mutwo_abjad-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutwo.abjad-0.19.0.tar", last modified: Mon Jan  8 20:02:00 2024, max compression
+gzip compressed data, was "mutwo_abjad-0.20.0.tar", last modified: Fri Apr 26 15:18:26 2024, max compression
```

## Comparing `mutwo.abjad-0.19.0.tar` & `mutwo_abjad-0.20.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-08 20:02:00.561168 mutwo.abjad-0.19.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1541 2024-01-08 20:02:00.561168 mutwo.abjad-0.19.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      795 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-08 20:02:00.553167 mutwo.abjad-0.19.0/mutwo/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-08 20:02:00.557168 mutwo.abjad-0.19.0/mutwo/abjad_converters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1660 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_converters/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      507 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_converters/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      428 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_converters/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-08 20:02:00.557168 mutwo.abjad-0.19.0/mutwo/abjad_converters/events/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_converters/events/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    57247 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_converters/events/building.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    38939 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_converters/events/quantization.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-08 20:02:00.557168 mutwo.abjad-0.19.0/mutwo/abjad_converters/parameters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_converters/parameters/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10043 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_converters/parameters/heji.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      685 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_converters/parameters/lyrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2139 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_converters/parameters/pitches.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10727 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_converters/parameters/tempos.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1403 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_converters/parameters/volumes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6023 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_converters/process_container_routines.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-08 20:02:00.557168 mutwo.abjad-0.19.0/mutwo/abjad_parameters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      170 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_parameters/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7353 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_parameters/abc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30726 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_parameters/attachments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      593 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_parameters/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      458 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_parameters/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-08 20:02:00.557168 mutwo.abjad-0.19.0/mutwo/abjad_utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_utilities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2748 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_utilities/abjad.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      293 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_utilities/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4671 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_utilities/tests.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      548 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_utilities/tools.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-08 20:02:00.557168 mutwo.abjad-0.19.0/mutwo/abjad_version/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      144 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo/abjad_version/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-08 20:02:00.557168 mutwo.abjad-0.19.0/mutwo.abjad.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1541 2024-01-08 20:02:00.000000 mutwo.abjad-0.19.0/mutwo.abjad.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1187 2024-01-08 20:02:00.000000 mutwo.abjad-0.19.0/mutwo.abjad.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-01-08 20:02:00.000000 mutwo.abjad-0.19.0/mutwo.abjad.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      187 2024-01-08 20:02:00.000000 mutwo.abjad-0.19.0/mutwo.abjad.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-01-08 20:02:00.000000 mutwo.abjad-0.19.0/mutwo.abjad.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-08 20:02:00.553167 mutwo.abjad-0.19.0/mutwo_third_party/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-08 20:02:00.557168 mutwo.abjad-0.19.0/mutwo_third_party/abjad/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7734 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/mutwo_third_party/abjad/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-01-08 20:02:00.561168 mutwo.abjad-0.19.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1404 2024-01-08 20:01:49.000000 mutwo.abjad-0.19.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:18:26.403199 mutwo_abjad-0.20.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1541 2024-04-26 15:18:26.403199 mutwo_abjad-0.20.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      795 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:18:26.399199 mutwo_abjad-0.20.0/mutwo/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:18:26.399199 mutwo_abjad-0.20.0/mutwo/abjad_converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1990 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_converters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      503 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_converters/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      428 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_converters/constants.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:18:26.399199 mutwo_abjad-0.20.0/mutwo/abjad_converters/events/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_converters/events/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    55201 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_converters/events/building.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    38187 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_converters/events/quantization.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:18:26.403199 mutwo_abjad-0.20.0/mutwo/abjad_converters/parameters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_converters/parameters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10040 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_converters/parameters/heji.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      685 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_converters/parameters/lyrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2124 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_converters/parameters/pitches.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9925 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_converters/parameters/tempos.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1403 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_converters/parameters/volumes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5896 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_converters/process_container_routines.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:18:26.403199 mutwo_abjad-0.20.0/mutwo/abjad_parameters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      170 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_parameters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7344 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_parameters/abc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30665 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_parameters/attachments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      593 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_parameters/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      458 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_parameters/constants.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:18:26.403199 mutwo_abjad-0.20.0/mutwo/abjad_utilities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_utilities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2748 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_utilities/abjad.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      293 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_utilities/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4645 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_utilities/tests.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      548 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_utilities/tools.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:18:26.403199 mutwo_abjad-0.20.0/mutwo/abjad_version/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      144 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo/abjad_version/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:18:26.403199 mutwo_abjad-0.20.0/mutwo.abjad.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1541 2024-04-26 15:18:26.000000 mutwo_abjad-0.20.0/mutwo.abjad.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1187 2024-04-26 15:18:26.000000 mutwo_abjad-0.20.0/mutwo.abjad.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-26 15:18:26.000000 mutwo_abjad-0.20.0/mutwo.abjad.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      187 2024-04-26 15:18:26.000000 mutwo_abjad-0.20.0/mutwo.abjad.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-26 15:18:26.000000 mutwo_abjad-0.20.0/mutwo.abjad.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:18:26.399199 mutwo_abjad-0.20.0/mutwo_third_party/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:18:26.403199 mutwo_abjad-0.20.0/mutwo_third_party/abjad/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7734 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/mutwo_third_party/abjad/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-26 15:18:26.403199 mutwo_abjad-0.20.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1404 2024-04-26 15:18:16.000000 mutwo_abjad-0.20.0/setup.py
```

### Comparing `mutwo.abjad-0.19.0/LICENSE` & `mutwo_abjad-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mutwo.abjad-0.19.0/PKG-INFO` & `mutwo_abjad-0.20.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: mutwo.abjad
-Version: 0.19.0
+Version: 0.20.0
 Summary: abjad extension for event based framework mutwo
 Home-page: https://github.com/mutwo-org/mutwo.abjad
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo-org.github.io
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mutwo.core<2.0.0,>=1.4.0
-Requires-Dist: mutwo.music<1.0.0,>=0.26.0
+Requires-Dist: mutwo.core<3.0.0,>=2.0.0
+Requires-Dist: mutwo.music<1.0.0,>=0.27.0
 Requires-Dist: abjad<3.12.0,>=3.9.0
 Requires-Dist: abjad-ext-nauert<3.12.0,>=3.9.0
 Requires-Dist: python-ranges<2.0.0,>=1.2.0
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.1; extra == "testing"
-Requires-Dist: mutwo.ekmelily<1.0.0,>=0.8.0; extra == "testing"
+Requires-Dist: mutwo.ekmelily<1.0.0,>=0.9.0; extra == "testing"
 
 # mutwo.abjad
 
 [![Build Status](https://circleci.com/gh/mutwo-org/mutwo.abjad.svg?style=shield)](https://circleci.com/gh/mutwo-org/mutwo.abjad)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![PyPI version](https://badge.fury.io/py/mutwo.abjad.svg)](https://badge.fury.io/py/mutwo.abjad)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `mutwo.abjad-0.19.0/README.md` & `mutwo_abjad-0.20.0/README.md`

 * *Files identical despite different names*

### Comparing `mutwo.abjad-0.19.0/mutwo/abjad_converters/__init__.py` & `mutwo_abjad-0.20.0/mutwo/abjad_converters/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """Build Lilypond scores via `Abjad <https://github.com/Abjad/abjad>`_ from Mutwo data.
 
 The following converter classes help to quantize and translate Mutwo data to
 Western notation. Due to the complex nature of this task, Mutwo tries to offer as
 many optional arguments as possible through which the user can affect the conversion
 routines. The most important class and best starting point for organising a conversion
-setting is :class:`SequentialEventToAbjadVoice`.
+setting is :class:`ConsecutionToAbjadVoice`.
 If one wants to build complete scores from within mutwo, the module offers the
-:class:`NestedComplexEventToAbjadContainer`.
+:class:`NestedCompoundToAbjadContainer`.
 
 **Known bugs and limitations:**
 
 1. Indicators attached to rests which follow another rest won't be translated to
    `abjad`. This behaviour happens because
-   :class:`~mutwo.abjad_converters.SequentialEventToAbjadVoice`
-   ties rests before converting the data to `abjad` objects.
+   :class:`~mutwo.abjad_converters.LeafMakerConsecutionToQuantizedAbjadContainer` and
+   :class:`~mutwo.abjad_converters.NauertConsecutionToQuantizedAbjadContainer`
+   tie rests before converting the data to `abjad` objects. With a different (maybe
+   user-declared) quantizer this limitation can be fixed. For more details see
+   the comment `here <https://github.com/mutwo-org/mutwo.abjad/blob/58b0044/mutwo/abjad_converters/events/quantization.py#L102-L128>_.
 
 2. Quantization can be slow and not precise. Try both quantization classes.
    Change the parameters. Use different settings and classes for different
    parts of your music.
 """
 
 # Apply monkey patch
```

### Comparing `mutwo.abjad-0.19.0/mutwo/abjad_converters/events/quantization.py` & `mutwo_abjad-0.20.0/mutwo/abjad_converters/events/quantization.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Module to quantize free :class:`SequentialEvent` to notation based abjad :class:`Container`"""
+"""Module to quantize free :class:`Consecution` to notation based abjad :class:`Container`"""
 
 import abc
 import typing
 import warnings
 
 try:
     import quicktions as fractions  # type: ignore
@@ -16,98 +16,98 @@
 from mutwo import abjad_utilities
 from mutwo import core_converters
 from mutwo import core_events
 from mutwo import core_parameters
 from mutwo import core_utilities
 
 __all__ = (
-    "SequentialEventToQuantizedAbjadContainer",
-    "NauertSequentialEventToQuantizedAbjadContainer",
-    "NauertSequentialEventToDurationLineBasedQuantizedAbjadContainer",
-    "LeafMakerSequentialEventToQuantizedAbjadContainer",
-    "LeafMakerSequentialEventToDurationLineBasedQuantizedAbjadContainer",
+    "ConsecutionToQuantizedAbjadContainer",
+    "NauertConsecutionToQuantizedAbjadContainer",
+    "NauertConsecutionToDurationLineBasedQuantizedAbjadContainer",
+    "LeafMakerConsecutionToQuantizedAbjadContainer",
+    "LeafMakerConsecutionToDurationLineBasedQuantizedAbjadContainer",
 )
 
 
-IsSimpleEventRestTuple: typing.TypeAlias = tuple[bool, ...]
+IsChrononRestTuple: typing.TypeAlias = tuple[bool, ...]
 QuantizationData: typing.TypeAlias = tuple[
-    abjad.Container, tuple[tuple[tuple[int, ...], ...], ...], IsSimpleEventRestTuple
+    abjad.Container, tuple[tuple[tuple[int, ...], ...], ...], IsChrononRestTuple
 ]
 
 
 # XXX: In the future `default_tempo_envelope` should be set to `None` and
 # `mutwo` should, by default, use `event_to_tempo_envelope`. Then
 # `default_tempo_envelope` should be removed completely.
-class SequentialEventToQuantizedAbjadContainer(core_converters.abc.Converter):
-    """Quantize :class:`~mutwo.core_events.SequentialEvent` objects.
+class ConsecutionToQuantizedAbjadContainer(core_converters.abc.Converter):
+    """Quantize :class:`~mutwo.core_events.Consecution` objects.
 
     :param default_time_signature_sequence: Set time signatures to divide the quantized abjad data
-        in desired bar sizes. If the converted :class:`~mutwo.core_events.SequentialEvent`
+        in desired bar sizes. If the converted :class:`~mutwo.core_events.Consecution`
         is longer than the sum of all passed time signatures, the last time signature
         will be repeated for the remaining bars.
     :type default_time_signature_sequence: typing.Sequence[abjad.TimeSignature]
     :param event_to_time_signature_tuple: Function which extracts a
         `tuple[abjad.TimeSignature, ...]` from a :class:`mutwo.core_events.abc.Event`.
         If set to `None` `mutwo` falls back to `default_time_signature_sequence`.
         Default to `None`.
-    :param is_simple_event_rest: Function to detect if the
-        the inspected :class:`mutwo.core_events.SimpleEvent` is a Rest. By
+    :param is_chronon_rest: Function to detect if the
+        the inspected :class:`mutwo.core_events.Chronon` is a Rest. By
         default Mutwo simply checks if 'pitch_list' contain any objects. If not,
         the Event will be interpreted as a rest.
-    :type is_simple_event_rest: typing.Callable[[core_events.SimpleEvent], bool], optional
+    :type is_chronon_rest: typing.Callable[[core_events.Chronon], bool], optional
     """
 
     def __init__(
         self,
         default_time_signature_sequence: typing.Sequence[abjad.TimeSignature] = (
             abjad.TimeSignature((4, 4)),
         ),
         event_to_time_signature_tuple: typing.Optional[
             typing.Callable[
                 [core_events.abc.Event],
                 typing.Optional[tuple[abjad.TimeSignature, ...]],
             ]
         ] = None,
-        is_simple_event_rest: typing.Optional[
-            typing.Callable[[core_events.SimpleEvent], bool]
+        is_chronon_rest: typing.Optional[
+            typing.Callable[[core_events.Chronon], bool]
         ] = None,
     ):
         default_time_signature_sequence_count = len(default_time_signature_sequence)
         if default_time_signature_sequence_count == 0:
             raise abjad_utilities.NoTimeSignatureError()
 
-        if is_simple_event_rest is None:
+        if is_chronon_rest is None:
 
-            def is_simple_event_rest(simple_event: core_events.SimpleEvent) -> bool:
+            def is_chronon_rest(chronon: core_events.Chronon) -> bool:
                 pitch_list = core_utilities.call_function_except_attribute_error(
-                    lambda e: e.pitch_list, simple_event, []
+                    lambda e: e.pitch_list, chronon, []
                 )
                 return not bool(pitch_list)
 
         default_time_signature_tuple = tuple(default_time_signature_sequence)
         self._default_time_signature_tuple = default_time_signature_tuple
 
         self._event_to_time_signature_tuple = event_to_time_signature_tuple
 
-        self._is_simple_event_rest = is_simple_event_rest
+        self._is_chronon_rest = is_chronon_rest
 
     def _get_time_signature_tuple(
         self, event: core_events.abc.Event
     ) -> tuple[abjad.TimeSignature, ...]:
         if self._event_to_time_signature_tuple:
             if time_signature_tuple := self._event_to_time_signature_tuple(event):
                 return time_signature_tuple
         return self._default_time_signature_tuple
 
-    def _tie_rests(self, sequential_event_to_convert: core_events.SequentialEvent):
+    def _tie_rests(self, consecution_to_convert: core_events.Consecution):
         # Tie rests before further processing the event
         #
         # We need to do this, because otherwise pitches/volumes/indicators
         # don't get attached to the right leaves, since
-        # 'related_abjad_leaf_index_tuple_tuple_per_simple_event' would point
+        # 'related_abjad_leaf_index_tuple_tuple_per_chronon' would point
         # to rests where notes are expected. This is because the quantizer
         # auto-splits and auto-combines rests in the following cases:
         #
         #   - if they are too long and span across two bars
         #   - if they are pointless (e.g. first beat of 4/4 bar 1/16 and a 3/16
         #     rest would be combined to a 1/4 rest) the quantizer
         #     automatically combines them (in 'rewrite_meter').
@@ -122,75 +122,70 @@
         # auto-split, while still persisting indicators on a rest sequence.
         # For this, the quantizer would need to only tie rests, that
         # don't contain any playing or notation indicators. Furthermore
         # it would be disallowed to auto-merge rests in further proceedings
         # (as rewrite_meter or concatenate_adjacent_tuplets) that have
         # indicators applied to them. For this we would need to pin tags to
         # events according to their status.
-        return sequential_event_to_convert.tie_by(
-            lambda event0, event1: self._is_simple_event_rest(event0)
-            and self._is_simple_event_rest(event1),
-            event_type_to_examine=core_events.SimpleEvent,
-            mutate=False,  # type: ignore
+        return consecution_to_convert.copy().tie_by(
+            lambda event0, event1: self._is_chronon_rest(event0)
+            and self._is_chronon_rest(event1),
+            event_type_to_examine=core_events.Chronon,
         )
 
-    def _apply_is_rest(self, sequential_event_to_convert: core_events.SequentialEvent):
-        # Apply 'is_rest' attribute to each event in the 'SequentialEvent'
+    def _apply_is_rest(self, consecution_to_convert: core_events.Consecution):
+        # Apply 'is_rest' attribute to each event in the 'Consecution'
         # (this is needed for further proceedings)
-        is_simple_event_rest_tuple = tuple(
-            self._is_simple_event_rest(simple_event)
-            for simple_event in sequential_event_to_convert
+        is_chronon_rest_tuple = tuple(
+            self._is_chronon_rest(chronon) for chronon in consecution_to_convert
         )
-        is_simple_event_rest_iterator = iter(is_simple_event_rest_tuple)
+        is_chronon_rest_iterator = iter(is_chronon_rest_tuple)
         return (
-            sequential_event_to_convert.set_parameter(  # type: ignore
+            consecution_to_convert.copy().set_parameter(  # type: ignore
                 "is_rest",
-                lambda _: next(is_simple_event_rest_iterator),
+                lambda _: next(is_chronon_rest_iterator),
                 set_unassigned_parameter=True,
-                mutate=False,  # type: ignore
             ),
-            is_simple_event_rest_tuple,
+            is_chronon_rest_tuple,
         )
 
     # ###################################################################### #
     #               public methods for interaction with the user             #
     # ###################################################################### #
 
     @abc.abstractmethod
     def convert(
-        self, sequential_event_to_convert: core_events.SequentialEvent
+        self, consecution_to_convert: core_events.Consecution
     ) -> QuantizationData:
         ...
 
 
-class NauertSequentialEventToQuantizedAbjadContainer(
-    SequentialEventToQuantizedAbjadContainer
-):
-    """Quantize :class:`~mutwo.core_events.SequentialEvent` objects via :mod:`abjadext.nauert`.
+class NauertConsecutionToQuantizedAbjadContainer(ConsecutionToQuantizedAbjadContainer):
+    """Quantize :class:`~mutwo.core_events.Consecution` objects via :mod:`abjadext.nauert`.
 
     :param default_time_signature_sequence: Set time signatures to divide the quantized abjad data
-        in desired bar sizes. If the converted :class:`~mutwo.core_events.SequentialEvent`
+        in desired bar sizes. If the converted :class:`~mutwo.core_events.Consecution`
         is longer than the sum of all passed time signatures, the last time signature
         will be repeated for the remaining bars.
     :type default_time_signature_sequence: typing.Sequence[abjad.TimeSignature]
     :param duration_unit: This defines the `duration_unit` of the passed
-        :class:`~mutwo.core_events.SequentialEvent` (how the
+        :class:`~mutwo.core_events.Consecution` (how the
         :attr:`~mutwo.core_events.abc.Event.duration` attribute will be
         interpreted). Can either be 'beats' (default) or 'miliseconds'.
         WARNING: 'miliseconds' isn't working properly yet!
     :param attack_point_optimizer: Optionally the user can pass a
         :class:`nauert.AttackPointOptimizer` object. Attack point optimizer help to
         split events and tie them for better looking notation. The default attack point
         optimizer is :class:`nauert.MeasurewiseAttackPointOptimizer` which splits events
         to better represent metrical structures within bars. If no optimizer is desired
         this argument can be set to ``None``.
 
-    Unlike :class:`LeafMakerSequentialEventToQuantizedAbjadContainer` this converter
+    Unlike :class:`LeafMakerConsecutionToQuantizedAbjadContainer` this converter
     supports nested tuplets and ties across tuplets. But this converter is much slower
-    than the :class:`LeafMakerSequentialEventToQuantizedAbjadContainer`. Because the
+    than the :class:`LeafMakerConsecutionToQuantizedAbjadContainer`. Because the
     converter depends on the abjad extension `nauert` its quality is dependent on the
     inner mechanism of the used package. Because the quantization made by the `nauert`
     package can be somewhat indeterministic a lot of tweaking may be necessary for
     complex musical structures.
     """
 
     # TODO(add proper miliseconds conversion: you will have to add the tempo_envelope
@@ -248,123 +243,123 @@
         except IndexError:
             return None
 
     @staticmethod
     def _process_abjad_leaf(
         indices: list[int],
         abjad_leaf: abjad.Leaf,
-        related_abjad_leaves_per_simple_event: list[list[tuple[int, ...]]],
+        related_abjad_leaves_per_chronon: list[list[tuple[int, ...]]],
         q_event_sequence: nauert.QEventSequence,
         has_tie: bool,
         index_of_previous_q_event: int,
     ) -> tuple[bool, int]:
-        q_event = NauertSequentialEventToQuantizedAbjadContainer._get_respective_q_event_from_abjad_leaf(
+        q_event = NauertConsecutionToQuantizedAbjadContainer._get_respective_q_event_from_abjad_leaf(
             abjad_leaf
         )
 
         if q_event and type(q_event) != nauert.TerminalQEvent:
             nth_q_event = q_event_sequence.sequence.index(q_event)
-            related_abjad_leaves_per_simple_event[nth_q_event].append(tuple(indices))
+            related_abjad_leaves_per_chronon[nth_q_event].append(tuple(indices))
             index_of_previous_q_event = nth_q_event
         elif has_tie:
-            related_abjad_leaves_per_simple_event[index_of_previous_q_event].append(
+            related_abjad_leaves_per_chronon[index_of_previous_q_event].append(
                 tuple(indices)
             )
         # skip leaves without any links
         # else:
-        #     related_abjad_leaves_per_simple_event.append([tuple(indices)])
+        #     related_abjad_leaves_per_chronon.append([tuple(indices)])
 
         has_tie = abjad.get.has_indicator(abjad_leaf, abjad.Tie)
 
         return has_tie, index_of_previous_q_event
 
     @staticmethod
     def _process_tuplet(
         indices: list[int],
         tuplet: abjad.Tuplet,
-        related_abjad_leaves_per_simple_event: list[list[tuple[int, ...]]],
+        related_abjad_leaves_per_chronon: list[list[tuple[int, ...]]],
         q_event_sequence: nauert.QEventSequence,
         has_tie: bool,
         index_of_previous_q_event: int,
     ) -> tuple[bool, int]:
         for (
             nth_abjad_leaf_or_tuplet,
             abjad_leaf_or_tuplet,
         ) in enumerate(tuplet):
             (
                 has_tie,
                 index_of_previous_q_event,
-            ) = NauertSequentialEventToQuantizedAbjadContainer._process_abjad_leaf_or_tuplet(
+            ) = NauertConsecutionToQuantizedAbjadContainer._process_abjad_leaf_or_tuplet(
                 indices + [nth_abjad_leaf_or_tuplet],
                 abjad_leaf_or_tuplet,
-                related_abjad_leaves_per_simple_event,
+                related_abjad_leaves_per_chronon,
                 q_event_sequence,
                 has_tie,
                 index_of_previous_q_event,
             )
 
         return has_tie, index_of_previous_q_event
 
     @staticmethod
     def _process_abjad_leaf_or_tuplet(
         index_list: list[int],
         abjad_leaf_or_tuplet: typing.Union[abjad.Tuplet, abjad.Leaf],
-        related_abjad_leaves_per_simple_event: list[list[tuple[int, ...]]],
+        related_abjad_leaves_per_chronon: list[list[tuple[int, ...]]],
         q_event_sequence: nauert.QEventSequence,
         has_tie: bool,
         index_of_previous_q_event: int,
     ) -> tuple[bool, int]:
         if isinstance(abjad_leaf_or_tuplet, abjad.Tuplet):
-            return NauertSequentialEventToQuantizedAbjadContainer._process_tuplet(
+            return NauertConsecutionToQuantizedAbjadContainer._process_tuplet(
                 index_list,
                 abjad_leaf_or_tuplet,
-                related_abjad_leaves_per_simple_event,
+                related_abjad_leaves_per_chronon,
                 q_event_sequence,
                 has_tie,
                 index_of_previous_q_event,
             )
 
         else:
-            return NauertSequentialEventToQuantizedAbjadContainer._process_abjad_leaf(
+            return NauertConsecutionToQuantizedAbjadContainer._process_abjad_leaf(
                 index_list,
                 abjad_leaf_or_tuplet,
-                related_abjad_leaves_per_simple_event,
+                related_abjad_leaves_per_chronon,
                 q_event_sequence,
                 has_tie,
                 index_of_previous_q_event,
             )
 
     @staticmethod
-    def _make_related_abjad_leaves_per_simple_event(
-        sequential_event: core_events.SequentialEvent,
+    def _make_related_abjad_leaves_per_chronon(
+        consecution: core_events.Consecution,
         q_event_sequence: nauert.QEventSequence,
         quanitisized_abjad_leaf_voice: abjad.Voice,
     ) -> tuple[tuple[tuple[int, ...], ...], ...,]:
         has_tie = False
         index_of_previous_q_event: int = 0
-        related_abjad_leaves_per_simple_event: list[list[tuple[int, ...]]] = [
-            [] for _ in sequential_event
+        related_abjad_leaves_per_chronon: list[list[tuple[int, ...]]] = [
+            [] for _ in consecution
         ]
         for nth_bar, bar in enumerate(quanitisized_abjad_leaf_voice):
             for nth_abjad_leaf_or_tuplet, abjad_leaf_or_tuplet in enumerate(bar):
                 (
                     has_tie,
                     index_of_previous_q_event,
-                ) = NauertSequentialEventToQuantizedAbjadContainer._process_abjad_leaf_or_tuplet(
+                ) = NauertConsecutionToQuantizedAbjadContainer._process_abjad_leaf_or_tuplet(
                     [nth_bar, nth_abjad_leaf_or_tuplet],
                     abjad_leaf_or_tuplet,
-                    related_abjad_leaves_per_simple_event,
+                    related_abjad_leaves_per_chronon,
                     q_event_sequence,
                     has_tie,
                     index_of_previous_q_event,
                 )
 
         return tuple(
             tuple(tuple(item) for item in pair)
-            for pair in related_abjad_leaves_per_simple_event
+            for pair in related_abjad_leaves_per_chronon
         )
 
     @staticmethod
     def _make_q_schema(
         time_signature_tuple: tuple[abjad.TimeSignature, ...],
         search_tree: typing.Optional[nauert.SearchTree],
     ) -> nauert.QSchema:
@@ -385,27 +380,29 @@
         )
 
     # ###################################################################### #
     #                         private methods                                #
     # ###################################################################### #
 
     def _get_q_schema(self, event: core_events.abc.Event) -> nauert.MeasurewiseQSchema:
-        return NauertSequentialEventToQuantizedAbjadContainer._make_q_schema(
+        return NauertConsecutionToQuantizedAbjadContainer._make_q_schema(
             self._get_time_signature_tuple(event), self._search_tree
         )
 
-    def _sequential_event_to_q_event_sequence(
-        self, sequential_event: core_events.SequentialEvent
+    def _consecution_to_q_event_sequence(
+        self, consecution: core_events.Consecution
     ) -> nauert.QEventSequence:
-        duration_list = list(sequential_event.get_parameter("duration"))
+        duration_list = list(
+            map(to_abjad_compatible_duration, consecution.get_parameter("duration"))
+        )
 
-        for nth_simple_event, simple_event in enumerate(sequential_event):
-            if simple_event.is_rest:
-                duration_list[nth_simple_event] = (
-                    core_parameters.DirectDuration(0) - duration_list[nth_simple_event]
+        for nth_chronon, chronon in enumerate(consecution):
+            if chronon.is_rest:
+                duration_list[nth_chronon] = (
+                    0 - duration_list[nth_chronon]
                 )
 
         if self._duration_unit == "beats":
             return nauert.QEventSequence.from_tempo_scaled_durations(
                 duration_list, tempo=abjad.MetronomeMark((1, 4), 60)
             )
 
@@ -433,71 +430,69 @@
         )
 
     # ###################################################################### #
     #               public methods for interaction with the user             #
     # ###################################################################### #
 
     def convert(
-        self, sequential_event_to_convert: core_events.SequentialEvent
+        self, consecution_to_convert: core_events.Consecution
     ) -> QuantizationData:
-        sequential_event_to_convert, is_simple_event_rest_tuple = self._apply_is_rest(
-            self._tie_rests(sequential_event_to_convert)
-        )
-        q_event_sequence = self._sequential_event_to_q_event_sequence(
-            sequential_event_to_convert
+        consecution_to_convert, is_chronon_rest_tuple = self._apply_is_rest(
+            self._tie_rests(consecution_to_convert)
         )
-        q_schema = self._get_q_schema(sequential_event_to_convert)
+        q_event_sequence = self._consecution_to_q_event_sequence(consecution_to_convert)
+        q_schema = self._get_q_schema(consecution_to_convert)
         quanitisized_abjad_leaf_voice = (
             self._q_event_sequence_to_quanitisized_abjad_leaf_voice(
                 q_event_sequence, q_schema
             )
         )
 
-        related_abjad_leaves_per_simple_event = NauertSequentialEventToQuantizedAbjadContainer._make_related_abjad_leaves_per_simple_event(
-            sequential_event_to_convert, q_event_sequence, quanitisized_abjad_leaf_voice
+        related_abjad_leaves_per_chronon = NauertConsecutionToQuantizedAbjadContainer._make_related_abjad_leaves_per_chronon(
+            consecution_to_convert, q_event_sequence, quanitisized_abjad_leaf_voice
         )
         return (
             quanitisized_abjad_leaf_voice,
-            related_abjad_leaves_per_simple_event,
-            is_simple_event_rest_tuple,
+            related_abjad_leaves_per_chronon,
+            is_chronon_rest_tuple,
         )
 
 
-class LeafMakerSequentialEventToQuantizedAbjadContainer(
-    SequentialEventToQuantizedAbjadContainer
+class LeafMakerConsecutionToQuantizedAbjadContainer(
+    ConsecutionToQuantizedAbjadContainer
 ):
-    """Quantize :class:`~mutwo.core_events.SequentialEvent` object via :mod:`abjad.LeafMaker`.
+    """Quantize :class:`~mutwo.core_events.Consecution` object via :mod:`abjad.LeafMaker`.
 
     :param default_time_signature_sequence: Set time signatures to divide the quantized abjad data
         in desired bar sizes. If the converted
-        :class:`~mutwo.core_events.SequentialEvent` is longer than the sum of
+        :class:`~mutwo.core_events.Consecution` is longer than the sum of
         all passed time signatures, the last time signature
         will be repeated for the remaining bars.
     :type default_time_signature_sequence: typing.Sequence[abjad.TimeSignature]
     :param concatenate_adjacent_tuplets: Set to `True` if quantizer should concatenate
         adjacent tuplets via :func:`mutwo.abjad_utilities.concatenate_adjacent_tuplets`.
         Because this function can make processing slower (and may lead to not-yet-fixed
         bugs) it can be deactivated if not used. Default to `True`.
     :type concatenate_adjacent_tuplets: bool
     :param reduce_multiplier: Set to `True` if quantizer should call
-        :func:`mutwo.abjad_utilities.reduce_multiplier` after sequential event
+        :func:`mutwo.abjad_utilities.reduce_multiplier` after consecution
         has been quantized. Can be useful if working with tuplets. If no tuplets
         are used it can be deactivated for faster conversion. Default to ``True``.
     :type reduce_multiplier: bool
 
     This method is significantly faster than the
-    :class:`NauertSequentialEventToQuantizedAbjadContainer`. But it also
+    :class:`NauertConsecutionToQuantizedAbjadContainer`. But it also
     has several known limitations:
 
-        1. :class:`LeafMakerSequentialEventToQuantizedAbjadContainer` doesn't
+        1. :class:`LeafMakerConsecutionToQuantizedAbjadContainer` doesn't
            support nested tuplets.
-        2. :class:`LeafMakerSequentialEventToQuantizedAbjadContainer` doesn't
+        2. :class:`LeafMakerConsecutionToQuantizedAbjadContainer` doesn't
            support ties across tuplets with different prolation (or across tuplets
            and not-tuplet notation). If ties are desired the user has to build them
-           manually before passing the :class:`~mutwo.core_events.SequentialEvent`
+           manually before passing the :class:`~mutwo.core_events.Consecution`
            to the converter.
     """
 
     _maximum_dot_count = 1
 
     def __init__(
         self,
@@ -535,17 +530,15 @@
         return offset_inventory
 
     @staticmethod
     def _add_explicit_beams(
         bar: abjad.Container, meter: abjad.Meter, global_offset: abjad.Offset
     ) -> None:
         offset_inventory = (
-            LeafMakerSequentialEventToQuantizedAbjadContainer._find_offset_inventory(
-                meter
-            )
+            LeafMakerConsecutionToQuantizedAbjadContainer._find_offset_inventory(meter)
         )
         leaf_offset_list = []
         # don't attach beams on tuplets
         relevant_bar_items = filter(
             lambda leaf_or_tuplet: isinstance(leaf_or_tuplet, abjad.Leaf)
             and leaf_or_tuplet.written_duration < fractions.Fraction(1, 4),
             bar,
@@ -581,24 +574,24 @@
         return global_offset
 
     # ###################################################################### #
     #                       private methods                                  #
     # ###################################################################### #
 
     def _make_note_tuple(
-        self, sequential_event_to_convert: core_events.SequentialEvent
+        self, consecution_to_convert: core_events.Consecution
     ) -> tuple[abjad.Leaf, ...]:
         pitch_list = [
-            None if event.is_rest else "c" for event in sequential_event_to_convert
+            None if event.is_rest else "c" for event in consecution_to_convert
         ]
         # It has to be a list! Otherwise abjad raises an exception.
         duration_list = list(
             map(
-                lambda duration: abjad.Duration(duration),
-                sequential_event_to_convert.get_parameter("duration"),
+                lambda duration: abjad.Duration(to_abjad_compatible_duration(duration)),
+                consecution_to_convert.get_parameter("duration"),
             )
         )
         note_tuple = tuple(self._leaf_maker(pitch_list, duration_list))
         return note_tuple
 
     def _rewrite_meter(self, voice: abjad.Voice):
         time_signature_iter = iter(self._time_signature_tuple)
@@ -627,18 +620,18 @@
         if difference:
             last_bar.extend(self._leaf_maker([None], [difference]))
             abjad.Meter.rewrite_meter(
                 last_bar[:], time_signature, maximum_dot_count=self._maximum_dot_count
             )
 
     def _make_voice(
-        self, sequential_event_to_convert: core_events.SequentialEvent
+        self, consecution_to_convert: core_events.Consecution
     ) -> abjad.Voice:
         # first build notes
-        note_tuple = self._make_note_tuple(sequential_event_to_convert)
+        note_tuple = self._make_note_tuple(consecution_to_convert)
 
         # split notes by time signatures
         notes_split_by_time_signature_sequence = abjad.mutate.split(
             note_tuple,
             [time_signature.duration for time_signature in self._time_signature_tuple],
             cyclic=True,
         )
@@ -681,62 +674,60 @@
                     self._get_data_for_tuplet_or_leaf(
                         index_tuple + (nth_leaf_or_tuplet_of_tuplet,),
                         sub_leaf_or_tuplet,
                     )
                 )
             return tuple(data_per_leaf_or_tuplet_list)
 
-    def _make_related_abjad_leaves_per_simple_event(
+    def _make_related_abjad_leaves_per_chronon(
         self, voice: abjad.Voice
     ) -> tuple[tuple[tuple[int, ...], ...], ...]:
         data_per_tuplet_or_leaf_list = []
         for nth_bar, bar in enumerate(voice):
             for nth_leaf_or_tuplet, leaf_or_tuplet in enumerate(bar):
                 data_per_tuplet_or_leaf_list.extend(
                     self._get_data_for_tuplet_or_leaf(
                         (nth_bar, nth_leaf_or_tuplet), leaf_or_tuplet
                     )
                 )
 
-        related_abjad_leaves_per_simple_event = []
+        related_abjad_leaves_per_chronon = []
         related_abjad_leaves = []
         was_previous_note_rest = None
         has_previous_tie = None
         for index_tuple, has_tie, is_rest in data_per_tuplet_or_leaf_list:
             if has_previous_tie or all((was_previous_note_rest, is_rest)):
                 related_abjad_leaves.append(index_tuple)
             else:
                 if related_abjad_leaves:
-                    related_abjad_leaves_per_simple_event.append(
-                        tuple(related_abjad_leaves)
-                    )
+                    related_abjad_leaves_per_chronon.append(tuple(related_abjad_leaves))
                 related_abjad_leaves = [index_tuple]
 
             has_previous_tie = has_tie
             was_previous_note_rest = is_rest
 
         if related_abjad_leaves:
-            related_abjad_leaves_per_simple_event.append(tuple(related_abjad_leaves))
+            related_abjad_leaves_per_chronon.append(tuple(related_abjad_leaves))
 
-        return tuple(related_abjad_leaves_per_simple_event)
+        return tuple(related_abjad_leaves_per_chronon)
 
     def convert(
-        self, sequential_event_to_convert: core_events.SequentialEvent
+        self, consecution_to_convert: core_events.Consecution
     ) -> QuantizationData:
-        sequential_event_to_convert, is_simple_event_rest_tuple = self._apply_is_rest(
-            self._tie_rests(sequential_event_to_convert)
+        consecution_to_convert, is_chronon_rest_tuple = self._apply_is_rest(
+            self._tie_rests(consecution_to_convert)
         )
         self._time_signature_tuple = self._get_time_signature_tuple(
-            sequential_event_to_convert
+            consecution_to_convert
         )
-        voice = self._make_voice(sequential_event_to_convert)
-        related_abjad_leaves_per_simple_event = (
-            self._make_related_abjad_leaves_per_simple_event(voice)
+        voice = self._make_voice(consecution_to_convert)
+        related_abjad_leaves_per_chronon = self._make_related_abjad_leaves_per_chronon(
+            voice
         )
-        return voice, related_abjad_leaves_per_simple_event, is_simple_event_rest_tuple
+        return voice, related_abjad_leaves_per_chronon, is_chronon_rest_tuple
 
 
 class _DurationLineBasedQuantizedAbjadContainerMixin(object):
     """Mixin for duration-line based quantization.
 
     :param duration_line_minimum_length: The minimum length of a duration line.
     :type duration_line_minimum_length: int
@@ -753,19 +744,19 @@
     abjad Voice, otherwise Lilypond won't be able to render the desired output.
 
     **Example:**
 
     >>> import abjad
     >>> from mutwo import abjad_converters
     >>> from mutwo import core_events, music_events
-    >>> converter = abjad_converters.SequentialEventToAbjadVoice(
-    ...     abjad_converters.LeafMakerSequentialEventToDurationLineBasedQuantizedAbjadContainer(
+    >>> converter = abjad_converters.ConsecutionToAbjadVoice(
+    ...     abjad_converters.LeafMakerConsecutionToDurationLineBasedQuantizedAbjadContainer(
     ...        )
     ...    )
-    >>> seq = core_events.SequentialEvent(
+    >>> seq = core_events.Consecution(
     ...     [
     ...         music_events.NoteLike("c", 0.25),
     ...         music_events.NoteLike("d", 1),
     ...         music_events.NoteLike([], 0.25),
     ...         music_events.NoteLike("e", 1),
     ...         music_events.NoteLike("e", 1)
     ...     ]
@@ -810,19 +801,19 @@
             ),
             first_element,
         )
 
     def _adjust_quantisized_abjad_leaves(
         self,
         quanitisized_abjad_leaf_voice: abjad.Container,
-        related_abjad_leaves_per_simple_event: tuple[tuple[tuple[int, ...], ...], ...],
+        related_abjad_leaves_per_chronon: tuple[tuple[tuple[int, ...], ...], ...],
     ):
         is_first = True
 
-        for abjad_leaves_indices in related_abjad_leaves_per_simple_event:
+        for abjad_leaves_indices in related_abjad_leaves_per_chronon:
             if abjad_leaves_indices:
                 first_element = core_utilities.get_nested_item_from_index_sequence(
                     abjad_leaves_indices[0], quanitisized_abjad_leaf_voice
                 )
                 if is_first:
                     self._prepare_first_element(first_element)
                     is_first = False
@@ -843,16 +834,16 @@
                         core_utilities.set_nested_item_from_index_sequence(
                             indices,
                             quanitisized_abjad_leaf_voice,
                             abjad.Skip(element.written_duration),
                         )
 
 
-class NauertSequentialEventToDurationLineBasedQuantizedAbjadContainer(
-    NauertSequentialEventToQuantizedAbjadContainer,
+class NauertConsecutionToDurationLineBasedQuantizedAbjadContainer(
+    NauertConsecutionToQuantizedAbjadContainer,
     _DurationLineBasedQuantizedAbjadContainerMixin,
 ):
     def __init__(
         self,
         *args,
         duration_line_minimum_length: int = 6,
         duration_line_thickness: int = 3,
@@ -862,35 +853,35 @@
         _DurationLineBasedQuantizedAbjadContainerMixin.__init__(
             self,
             duration_line_minimum_length=duration_line_minimum_length,
             duration_line_thickness=duration_line_thickness,
         )
 
     def convert(
-        self, sequential_event_to_convert: core_events.SequentialEvent
+        self, consecution_to_convert: core_events.Consecution
     ) -> QuantizationData:
         (
             quanitisized_abjad_leaf_voice,
-            related_abjad_leaves_per_simple_event,
-            is_simple_event_rest_tuple,
-        ) = super().convert(sequential_event_to_convert)
+            related_abjad_leaves_per_chronon,
+            is_chronon_rest_tuple,
+        ) = super().convert(consecution_to_convert)
 
         self._adjust_quantisized_abjad_leaves(
-            quanitisized_abjad_leaf_voice, related_abjad_leaves_per_simple_event
+            quanitisized_abjad_leaf_voice, related_abjad_leaves_per_chronon
         )
 
         return (
             quanitisized_abjad_leaf_voice,
-            related_abjad_leaves_per_simple_event,
-            is_simple_event_rest_tuple,
+            related_abjad_leaves_per_chronon,
+            is_chronon_rest_tuple,
         )
 
 
-class LeafMakerSequentialEventToDurationLineBasedQuantizedAbjadContainer(
-    LeafMakerSequentialEventToQuantizedAbjadContainer,
+class LeafMakerConsecutionToDurationLineBasedQuantizedAbjadContainer(
+    LeafMakerConsecutionToQuantizedAbjadContainer,
     _DurationLineBasedQuantizedAbjadContainerMixin,
 ):
     def __init__(
         self,
         *args,
         duration_line_minimum_length: int = 6,
         duration_line_thickness: int = 3,
@@ -900,39 +891,43 @@
         _DurationLineBasedQuantizedAbjadContainerMixin.__init__(
             self,
             duration_line_thickness=duration_line_thickness,
             duration_line_minimum_length=duration_line_minimum_length,
         )
 
     def convert(
-        self, sequential_event_to_convert: core_events.SequentialEvent
+        self, consecution_to_convert: core_events.Consecution
     ) -> QuantizationData:
         (
             quanitisized_abjad_leaf_voice,
-            related_abjad_leaves_per_simple_event,
-            is_simple_event_rest_tuple,
-        ) = super().convert(sequential_event_to_convert)
+            related_abjad_leaves_per_chronon,
+            is_chronon_rest_tuple,
+        ) = super().convert(consecution_to_convert)
 
         self._adjust_quantisized_abjad_leaves(
-            quanitisized_abjad_leaf_voice, related_abjad_leaves_per_simple_event
+            quanitisized_abjad_leaf_voice, related_abjad_leaves_per_chronon
         )
 
         # only assign first item to abjad leaves
-        post_processed_releated_abjad_leaves_per_simple_event = []
-        for related_abjad_leaves in related_abjad_leaves_per_simple_event:
-            post_processed_releated_abjad_leaves_per_simple_event.append(
+        post_processed_releated_abjad_leaves_per_chronon = []
+        for related_abjad_leaves in related_abjad_leaves_per_chronon:
+            post_processed_releated_abjad_leaves_per_chronon.append(
                 (related_abjad_leaves[0],)
             )
 
         return (
             quanitisized_abjad_leaf_voice,
-            post_processed_releated_abjad_leaves_per_simple_event,
-            is_simple_event_rest_tuple,
+            post_processed_releated_abjad_leaves_per_chronon,
+            is_chronon_rest_tuple,
         )
 
 
-NauertSequentialEventToDurationLineBasedQuantizedAbjadContainer._set_docs(
-    NauertSequentialEventToQuantizedAbjadContainer
+NauertConsecutionToDurationLineBasedQuantizedAbjadContainer._set_docs(
+    NauertConsecutionToQuantizedAbjadContainer
 )
-LeafMakerSequentialEventToDurationLineBasedQuantizedAbjadContainer._set_docs(
-    LeafMakerSequentialEventToQuantizedAbjadContainer
+LeafMakerConsecutionToDurationLineBasedQuantizedAbjadContainer._set_docs(
+    LeafMakerConsecutionToQuantizedAbjadContainer
 )
+
+
+def to_abjad_compatible_duration(duration: core_parameters.abc.Duration):
+    return getattr(duration, "ratio", None) or duration.beat_count
```

### Comparing `mutwo.abjad-0.19.0/mutwo/abjad_converters/parameters/__init__.py` & `mutwo_abjad-0.20.0/mutwo/abjad_converters/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `mutwo.abjad-0.19.0/mutwo/abjad_converters/parameters/heji.py` & `mutwo_abjad-0.20.0/mutwo/abjad_converters/parameters/heji.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 
         pitch_as_western_pitch = music_parameters.WesternPitch(
             closest_pythagorean_pitch_name[0], octave
         )
         reference_pitch_as_western_pitch = music_parameters.WesternPitch(
             self._reference_pitch, 4
         )
-        expected_difference_in_cents = pitch_to_convert.interval
+        expected_difference_in_cents = pitch_to_convert.cents
         while (
             expected_difference_in_cents
             - (
                 (
                     pitch_as_western_pitch.midi_pitch_number
                     - reference_pitch_as_western_pitch.midi_pitch_number
                 )
```

### Comparing `mutwo.abjad-0.19.0/mutwo/abjad_converters/parameters/lyrics.py` & `mutwo_abjad-0.20.0/mutwo/abjad_converters/parameters/lyrics.py`

 * *Files identical despite different names*

### Comparing `mutwo.abjad-0.19.0/mutwo/abjad_converters/parameters/pitches.py` & `mutwo_abjad-0.20.0/mutwo/abjad_converters/parameters/pitches.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         :class:`music_parameters.WesternPitch` for further information.
     :type allowed_division_sequence: typing.Sequence[fractions.Fraction]
 
     This default class simply checks if the passed Mutwo object belongs to
     :class:`mutwo.music_parameters.WesternPitch`. If it does, Mutwo
     will initialise the Abjad Pitch from the :attr:`name` attribute.
     Otherwise Mutwo will simply initialise the Abjad Pitch from the
-    objects :attr:`frequency` attribute.
+    objects :attr:`hertz` attribute.
 
     If users desire to make more complex conversions (for instance
     due to ``scordatura`` or transpositions of instruments), one can simply
     inherit from this class to define more complex cases.
     """
 
     def __init__(
@@ -43,13 +43,13 @@
         ),
     ):
         self._allowed_division_sequence = allowed_division_sequence
 
     def convert(self, pitch_to_convert: music_parameters.abc.Pitch) -> abjad.Pitch:
         if isinstance(pitch_to_convert, music_parameters.WesternPitch):
             return abjad.NamedPitch(
-                pitch_to_convert.round_to(
-                    self._allowed_division_sequence, mutate=False
+                pitch_to_convert.copy().round_to(
+                    self._allowed_division_sequence
                 ).name
             )
         else:
-            return abjad.NamedPitch.from_hertz(pitch_to_convert.frequency)
+            return abjad.NamedPitch.from_hertz(pitch_to_convert.hertz)
```

### Comparing `mutwo.abjad-0.19.0/mutwo/abjad_converters/parameters/tempos.py` & `mutwo_abjad-0.20.0/mutwo/abjad_converters/parameters/tempos.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,117 +5,101 @@
     import quicktions as fractions  # type: ignore
 except ImportError:
     import fractions  # type: ignore
 
 from mutwo import abjad_parameters
 from mutwo import core_converters
 from mutwo import core_constants
-from mutwo import core_events
 from mutwo import core_parameters
 from mutwo import core_utilities
 
 __all__ = (
-    "TempoEnvelopeToAbjadAttachmentTempo",
-    "ComplexTempoEnvelopeToAbjadAttachmentTempo",
+    "TempoToAbjadAttachmentTempo",
+    "ComplexTempoToAbjadAttachmentTempo",
 )
 
 
-class TempoEnvelopeToAbjadAttachmentTempo(core_converters.abc.Converter):
+class TempoToAbjadAttachmentTempo(core_converters.abc.Converter):
     """Convert tempo envelope to :class:`~mutwo.abjad_parameters.Tempo`.
 
     Abstract base class for tempo envelope conversion. See
-    :class:`ComplexTempoEnvelopeToAbjadAttachmentTempo` for a concrete
+    :class:`ComplexTempoToAbjadAttachmentTempo` for a concrete
     class.
     """
 
     @abc.abstractmethod
     def convert(
-        self, tempo_envelope_to_convert: core_events.TempoEnvelope
+        self, tempo_to_convert: core_parameters.abc.Tempo
     ) -> tuple[tuple[core_constants.Real, abjad_parameters.Tempo], ...]:
         # return tuple filled with subtuples (leaf_index, abjad_parameters.Tempo)
         raise NotImplementedError()
 
 
-class ComplexTempoEnvelopeToAbjadAttachmentTempo(TempoEnvelopeToAbjadAttachmentTempo):
-    """Convert tempo envelope to :class:`~mutwo.abjad_parameters.Tempo`.
+class ComplexTempoToAbjadAttachmentTempo(TempoToAbjadAttachmentTempo):
+    """Convert tempo to :class:`~mutwo.abjad_parameters.Tempo`.
 
     This object tries to intelligently set correct tempo abjad_parameters to an
     :class:`abjad.Voice` object, appropriate to Western notation standards.
     Therefore it will not repeat tempo indications if they are merely repetitions
     of previous tempo indications and it will write 'a tempo' when returning to the
     same tempo after ritardandi or accelerandi.
     """
 
     # ###################################################################### #
     #                     private static methods                             #
     # ###################################################################### #
 
     @staticmethod
-    def _convert_tempo_point_tuple(
-        tempo_point_tuple: tuple[
-            typing.Union[core_constants.Real, core_parameters.abc.TempoPoint], ...
+    def _convert_tempo_tuple(
+        tempo_tuple: tuple[
+            typing.Union[core_constants.Real, core_parameters.abc.Tempo], ...
         ]
-    ) -> tuple[core_parameters.abc.TempoPoint, ...]:
+    ) -> tuple[core_parameters.abc.Tempo, ...]:
         return tuple(
-            tempo_point
-            if isinstance(tempo_point, core_parameters.abc.TempoPoint)
-            else core_parameters.DirectTempoPoint(float(tempo_point))
-            for tempo_point in tempo_point_tuple
+            tempo
+            if isinstance(tempo, core_parameters.abc.Tempo)
+            else core_parameters.DirectTempo(float(tempo))
+            for tempo in tempo_tuple
         )
 
     @staticmethod
     def _find_dynamic_change_indication(
-        tempo_point: core_parameters.abc.TempoPoint,
-        next_tempo_point: typing.Optional[core_parameters.abc.TempoPoint],
+        tempo: core_parameters.abc.Tempo,
+        next_tempo: typing.Optional[core_parameters.abc.Tempo],
     ) -> typing.Optional[str]:
         dynamic_change_indication = None
-        if next_tempo_point:
-            absolute_tempo_for_current_tempo_point = (
-                tempo_point.absolute_tempo_in_beats_per_minute
-            )
-            absolute_tempo_for_next_tempo_point = (
-                next_tempo_point.absolute_tempo_in_beats_per_minute
-            )
-            if (
-                absolute_tempo_for_current_tempo_point
-                > absolute_tempo_for_next_tempo_point
-            ):
+        if next_tempo:
+            absolute_tempo_for_current_tempo = tempo.bpm
+            absolute_tempo_for_next_tempo = next_tempo.bpm
+            if absolute_tempo_for_current_tempo > absolute_tempo_for_next_tempo:
                 dynamic_change_indication = "rit."
-            elif (
-                absolute_tempo_for_current_tempo_point
-                < absolute_tempo_for_next_tempo_point
-            ):
+            elif absolute_tempo_for_current_tempo < absolute_tempo_for_next_tempo:
                 dynamic_change_indication = "acc."
 
         return dynamic_change_indication
 
     @staticmethod
     def _shall_write_metronome_mark(
-        tempo_envelope_to_convert: core_events.TempoEnvelope,
-        tempo_point_index: int,
-        tempo_point: core_parameters.abc.TempoPoint,
-        tempo_point_tuple: tuple[core_parameters.abc.TempoPoint, ...],
+        tempo_to_convert: core_parameters.FlexTempo,
+        tempo_index: int,
+        tempo: core_parameters.abc.Tempo,
+        tempo_tuple: tuple[core_parameters.abc.Tempo, ...],
     ) -> bool:
         write_metronome_mark = True
-        for previous_tempo_point, previous_tempo_point_duration in zip(
-            reversed(tempo_point_tuple[:tempo_point_index]),
-            reversed(
-                tempo_envelope_to_convert.get_parameter("duration")[:tempo_point_index]
-            ),
+        for previous_tempo, previous_tempo_duration in zip(
+            reversed(tempo_tuple[:tempo_index]),
+            reversed(tempo_to_convert.get_parameter("duration")[:tempo_index]),
         ):
             # make sure the previous tempo point could have been written
             # down (longer duration than minimal duration)
-            if previous_tempo_point_duration > 0:
+            if previous_tempo_duration > 0:
                 # if the previous writeable MetronomeMark has the same
                 # beats per minute than the current event, there is no
                 # need to write it down again
-                if (
-                    previous_tempo_point.absolute_tempo_in_beats_per_minute
-                    == tempo_point.absolute_tempo_in_beats_per_minute
-                ):
+                if previous_tempo.bpm == tempo.bpm:
                     write_metronome_mark = False
                     break
 
                 # but if it differs, we should definitely write it down
                 else:
                     break
 
@@ -136,143 +120,149 @@
             break
 
         return stop_dynamic_change_indicaton
 
     @staticmethod
     def _find_metronome_mark_values(
         write_metronome_mark: bool,
-        tempo_point: core_parameters.abc.TempoPoint,
+        tempo: core_parameters.abc.Tempo,
         stop_dynamic_change_indicaton: bool,
     ) -> tuple[
         typing.Optional[tuple[int, int]],
         typing.Optional[typing.Union[int, tuple[int, int]]],
         typing.Optional[str],
     ]:
         if write_metronome_mark:
-            textual_indication: typing.Optional[str] = tempo_point.textual_indication
-            reference = fractions.Fraction(tempo_point.reference) * fractions.Fraction(
-                1, 4
+            textual_indication: typing.Optional[str] = getattr(
+                tempo, "textual_indication", None
             )
+            reference = fractions.Fraction(getattr(tempo, "reference", 1))
             reference_duration: typing.Optional[tuple[int, int]] = (
                 reference.numerator,
                 reference.denominator,
             )
-            units_per_minute: typing.Optional[typing.Union[int, tuple[int, int]]] = (
-                (
-                    int(tempo_point.tempo_or_tempo_range_in_beats_per_minute[0]),
-                    int(tempo_point.tempo_or_tempo_range_in_beats_per_minute[1]),
-                )
-                if isinstance(
-                    tempo_point.tempo_or_tempo_range_in_beats_per_minute, tuple
-                )
-                else int(tempo_point.tempo_or_tempo_range_in_beats_per_minute)
-            )
+
+            if hasattr(tempo, "bpm_range"):
+                if (b := tempo.bpm_range.start) != tempo.bpm_range.end:
+                    units_per_minute = (
+                        int(tempo.bpm_range.start),
+                        int(tempo.bpm_range.end),
+                    )
+                else:
+                    units_per_minute = int(b)
+            else:
+                units_per_minute = int(tempo.bpm)
 
         else:
             reference_duration = None
             units_per_minute = None
             # check if you can write 'a tempo'
             if stop_dynamic_change_indicaton:
                 textual_indication = "a tempo"
             else:
                 textual_indication = None
 
         return reference_duration, units_per_minute, textual_indication
 
     @staticmethod
-    def _process_tempo_event(
-        tempo_envelope_to_convert: core_events.TempoEnvelope,
-        tempo_point_index: int,
-        tempo_point: core_parameters.abc.TempoPoint,
-        tempo_point_tuple: tuple[core_parameters.abc.TempoPoint, ...],
+    def _process_tempo_chronon(
+        tempo_to_convert: core_parameters.FlexTempo,
+        tempo_index: int,
+        tempo: core_parameters.abc.Tempo,
+        tempo_tuple: tuple[core_parameters.abc.Tempo, ...],
         tempo_attachment_tuple: tuple[
             tuple[core_constants.Real, abjad_parameters.Tempo], ...
         ],
     ) -> abjad_parameters.Tempo:
         try:
-            next_tempo_point: typing.Optional[
-                core_parameters.abc.TempoPoint
-            ] = tempo_point_tuple[tempo_point_index + 1]
+            next_tempo: typing.Optional[core_parameters.abc.Tempo] = tempo_tuple[
+                tempo_index + 1
+            ]
         except IndexError:
-            next_tempo_point = None
+            next_tempo = None
 
         # check for dynamic_change_indication
         dynamic_change_indication = (
-            ComplexTempoEnvelopeToAbjadAttachmentTempo._find_dynamic_change_indication(
-                tempo_point, next_tempo_point
+            ComplexTempoToAbjadAttachmentTempo._find_dynamic_change_indication(
+                tempo, next_tempo
             )
         )
 
         write_metronome_mark = (
-            ComplexTempoEnvelopeToAbjadAttachmentTempo._shall_write_metronome_mark(
-                tempo_envelope_to_convert,
-                tempo_point_index,
-                tempo_point,
-                tempo_point_tuple,
+            ComplexTempoToAbjadAttachmentTempo._shall_write_metronome_mark(
+                tempo_to_convert,
+                tempo_index,
+                tempo,
+                tempo_tuple,
             )
         )
 
-        stop_dynamic_change_indicaton = ComplexTempoEnvelopeToAbjadAttachmentTempo._shall_stop_dynamic_change_indication(
-            tempo_attachment_tuple
+        stop_dynamic_change_indicaton = (
+            ComplexTempoToAbjadAttachmentTempo._shall_stop_dynamic_change_indication(
+                tempo_attachment_tuple
+            )
         )
 
         (
             reference_duration,
             units_per_minute,
             textual_indication,
-        ) = ComplexTempoEnvelopeToAbjadAttachmentTempo._find_metronome_mark_values(
-            write_metronome_mark, tempo_point, stop_dynamic_change_indicaton
+        ) = ComplexTempoToAbjadAttachmentTempo._find_metronome_mark_values(
+            write_metronome_mark, tempo, stop_dynamic_change_indicaton
         )
 
         # for writing 'a tempo'
         if textual_indication == "a tempo":
             write_metronome_mark = True
 
-        converted_tempo_point = abjad_parameters.Tempo(
+        converted_tempo = abjad_parameters.Tempo(
             reference_duration=reference_duration,
             units_per_minute=units_per_minute,
             textual_indication=textual_indication,
             dynamic_change_indication=dynamic_change_indication,
             stop_dynamic_change_indicaton=stop_dynamic_change_indicaton,
             print_metronome_mark=write_metronome_mark,
         )
 
-        return converted_tempo_point
+        return converted_tempo
 
     # ###################################################################### #
     #                           public api                                   #
     # ###################################################################### #
 
     def convert(
-        self, tempo_envelope_to_convert: core_events.TempoEnvelope
+        self, tempo_to_convert: core_parameters.abc.Tempo
     ) -> tuple[tuple[core_constants.Real, abjad_parameters.Tempo], ...]:
-        tempo_point_tuple = (
-            ComplexTempoEnvelopeToAbjadAttachmentTempo._convert_tempo_point_tuple(
-                tuple(tempo_envelope_to_convert.value_tuple)
-            )
+        if isinstance(tempo_to_convert, core_parameters.FlexTempo):
+            flex_tempo_to_convert = tempo_to_convert
+        else:
+            flex_tempo_to_convert = core_parameters.FlexTempo([[0, tempo_to_convert]])
+
+        tempo_tuple = ComplexTempoToAbjadAttachmentTempo._convert_tempo_tuple(
+            tuple(flex_tempo_to_convert.parameter_tuple)
         )
+        print(tempo_tuple)
 
         tempo_attachment_list: list[
             tuple[core_constants.Real, abjad_parameters.Tempo]
         ] = []
-        for tempo_point_index, absolute_time, duration, tempo_point in zip(
-            range(len(tempo_point_tuple)),
+        for tempo_index, absolute_time, duration, tempo in zip(
+            range(len(tempo_tuple)),
             core_utilities.accumulate_from_n(
-                tempo_envelope_to_convert.get_parameter("duration"),
+                flex_tempo_to_convert.get_parameter("duration"),
                 core_parameters.DirectDuration(0),
             ),
-            tuple(tempo_envelope_to_convert.get_parameter("duration")) + (1,),
-            tempo_point_tuple,
+            tuple(flex_tempo_to_convert.get_parameter("duration")) + (1,),
+            tempo_tuple,
         ):
-
             tempo_attachment = (
-                ComplexTempoEnvelopeToAbjadAttachmentTempo._process_tempo_event(
-                    tempo_envelope_to_convert,
-                    tempo_point_index,
-                    tempo_point,
-                    tempo_point_tuple,
+                ComplexTempoToAbjadAttachmentTempo._process_tempo_chronon(
+                    flex_tempo_to_convert,
+                    tempo_index,
+                    tempo,
+                    tempo_tuple,
                     tuple(tempo_attachment_list),
                 )
             )
             tempo_attachment_list.append((absolute_time, tempo_attachment))
 
         return tuple(tempo_attachment_list)
```

### Comparing `mutwo.abjad-0.19.0/mutwo/abjad_converters/parameters/volumes.py` & `mutwo_abjad-0.20.0/mutwo/abjad_converters/parameters/volumes.py`

 * *Files identical despite different names*

### Comparing `mutwo.abjad-0.19.0/mutwo/abjad_converters/process_container_routines.py` & `mutwo_abjad-0.20.0/mutwo/abjad_converters/process_container_routines.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,33 +18,33 @@
 )
 
 
 class ProcessAbjadContainerRoutine(abc.ABC):
     @abc.abstractmethod
     def __call__(
         self,
-        complex_event_to_convert: core_events.abc.ComplexEvent,
+        compound_to_convert: core_events.abc.Compound,
         container_to_process: abjad.Container,
     ):
         raise NotImplementedError
 
 
 class AddDurationLineEngraver(ProcessAbjadContainerRoutine):
     def __call__(
         self,
-        complex_event_to_convert: core_events.abc.ComplexEvent,
+        compound_to_convert: core_events.abc.Compound,
         container_to_process: abjad.Container,
     ):
         container_to_process.consists_commands.append("Duration_line_engraver")
 
 
 class PrepareForDurationLineBasedNotation(ProcessAbjadContainerRoutine):
     def __call__(
         self,
-        _: core_events.abc.ComplexEvent,
+        _: core_events.abc.Compound,
         container_to_process: abjad.Container,
     ):
         first_element = abjad.get.leaf(container_to_process, 0)
         before_grace_container = abjad.get.before_grace_container(first_element)
         if before_grace_container:
             first_element = abjad.get.leaf(before_grace_container, 0)
         # don't write rests (simply write empty space)
@@ -69,47 +69,47 @@
             first_element,
         )
 
 
 class AddInstrumentName(ProcessAbjadContainerRoutine):
     def __init__(
         self,
-        complex_event_to_instrument_name: typing.Callable[
-            [core_events.abc.ComplexEvent], str
-        ] = lambda complex_event: complex_event.instrument_name,
-        complex_event_to_short_instrument_name: typing.Callable[
-            [core_events.abc.ComplexEvent], str
-        ] = lambda complex_event: complex_event.short_instrument_name,
+        compound_to_instrument_name: typing.Callable[
+            [core_events.abc.Compound], str
+        ] = lambda compound: compound.instrument_name,
+        compound_to_short_instrument_name: typing.Callable[
+            [core_events.abc.Compound], str
+        ] = lambda compound: compound.short_instrument_name,
         instrument_name_font_size: str = "teeny",
         short_instrument_name_font_size: str = "teeny",
     ):
-        self._complex_event_to_instrument_name = complex_event_to_instrument_name
-        self._complex_event_to_short_instrument_name = (
-            complex_event_to_short_instrument_name
+        self._compound_to_instrument_name = compound_to_instrument_name
+        self._compound_to_short_instrument_name = (
+            compound_to_short_instrument_name
         )
         self._instrument_name_font_size = instrument_name_font_size
         self._short_instrument_name_font_size = short_instrument_name_font_size
 
     def __call__(
         self,
-        complex_event_to_convert: core_events.abc.ComplexEvent,
+        compound_to_convert: core_events.abc.Compound,
         container_to_process: abjad.Container,
     ):
         first_leaf = abjad.get.leaf(container_to_process[0], 0)
 
         try:
-            instrument_name = self._complex_event_to_instrument_name(
-                complex_event_to_convert
+            instrument_name = self._compound_to_instrument_name(
+                compound_to_convert
             )
         except AttributeError:
             instrument_name = None
 
         try:
-            short_instrument_name = self._complex_event_to_short_instrument_name(
-                complex_event_to_convert
+            short_instrument_name = self._compound_to_short_instrument_name(
+                compound_to_convert
             )
         except AttributeError:
             short_instrument_name = None
 
         lilypond_context = container_to_process.lilypond_context.name
 
         if instrument_name:
@@ -135,15 +135,15 @@
 
 class AddAccidentalStyle(ProcessAbjadContainerRoutine):
     def __init__(self, accidental_style: str):
         self._accidental_style = accidental_style
 
     def __call__(
         self,
-        complex_event_to_convert: core_events.abc.ComplexEvent,
+        compound_to_convert: core_events.abc.Compound,
         container_to_process: abjad.Container,
     ):
         first_leaf = abjad.get.leaf(container_to_process[0], 0)
 
         if self._accidental_style:
             abjad.attach(
                 abjad.LilyPondLiteral(f'\\accidentalStyle "{self._accidental_style}"'),
@@ -153,15 +153,15 @@
 
 class SetStaffSize(ProcessAbjadContainerRoutine):
     def __init__(self, difference_of_size: int):
         self._difference_of_size = difference_of_size
 
     def __call__(
         self,
-        complex_event_to_convert: core_events.abc.ComplexEvent,
+        compound_to_convert: core_events.abc.Compound,
         container_to_process: abjad.Container,
     ):
         first_leaf = abjad.get.leaf(container_to_process[0], 0)
         abjad.attach(
             abjad.LilyPondLiteral(
                 f"\\magnifyStaff #(magstep {self._difference_of_size})",
                 format_slot="before",
```

### Comparing `mutwo.abjad-0.19.0/mutwo/abjad_parameters/abc.py` & `mutwo_abjad-0.20.0/mutwo/abjad_parameters/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 @dataclasses.dataclass()
 class AbjadAttachment(abc.ABC):
     """Abstract base class for all Abjad attachments."""
 
     indicator: typing.Optional[
         music_parameters.abc.PlayingIndicator | music_parameters.abc.NotationIndicator
     ] = None
-    is_simple_event_rest: typing.Optional[
-        typing.Callable[[core_events.SimpleEvent], bool]
+    is_chronon_rest: typing.Optional[
+        typing.Callable[[core_events.Chronon], bool]
     ] = None
     mutwo_pitch_to_abjad_pitch: typing.Optional[
         typing.Callable[[music_parameters.abc.Pitch], abjad.Pitch]
     ] = None
     mutwo_pitch_to_abjad_pitch: typing.Optional[
         typing.Callable[[music_parameters.abc.Pitch], abjad.Pitch]
     ] = None
```

### Comparing `mutwo.abjad-0.19.0/mutwo/abjad_parameters/attachments.py` & `mutwo_abjad-0.20.0/mutwo/abjad_parameters/attachments.py`

 * *Files 2% similar despite different names*

```diff
@@ -825,64 +825,64 @@
         return True
 
     def process_leaf(self, leaf: abjad.Leaf) -> LeafOrLeafSequence:
         abjad.attach(abjad.StopTextSpan(), leaf)
         return leaf
 
 
-class GraceNoteSequentialEvent(abjad_parameters.abc.BangFirstAttachment):
-    def __init__(self, grace_note_sequential_event: abjad.BeforeGraceContainer):
-        self._grace_note_sequential_event = grace_note_sequential_event
+class GraceNoteConsecution(abjad_parameters.abc.BangFirstAttachment):
+    def __init__(self, grace_note_consecution: abjad.BeforeGraceContainer):
+        self._grace_note_consecution = grace_note_consecution
 
     @classmethod
     def from_indicator_collection(
         cls, indicator_collection: music_parameters.abc.IndicatorCollection, **kwargs
     ) -> typing.Optional[abjad_parameters.abc.AbjadAttachment]:
         """Always return None.
 
-        GraceNoteSequentialEvent can't be initialised from IndicatorCollection.
+        GraceNoteConsecution can't be initialised from IndicatorCollection.
         """
         return None
 
     @property
     def is_active(self) -> bool:
         return True
 
     def process_leaf(self, leaf: abjad.Leaf) -> LeafOrLeafSequence:
         for (
             indicator_to_detach
         ) in (
             abjad_parameters.constants.INDICATORS_TO_DETACH_FROM_MAIN_LEAF_AT_GRACE_NOTES_TUPLE
         ):
             detached_indicator = abjad.detach(indicator_to_detach, leaf)
-            abjad.attach(detached_indicator, self._grace_note_sequential_event[0])
-        abjad.attach(self._grace_note_sequential_event, leaf)
+            abjad.attach(detached_indicator, self._grace_note_consecution[0])
+        abjad.attach(self._grace_note_consecution, leaf)
         return leaf
 
 
-class AfterGraceNoteSequentialEvent(abjad_parameters.abc.BangLastAttachment):
-    def __init__(self, after_grace_note_sequential_event: abjad.AfterGraceContainer):
-        self._after_grace_note_sequential_event = after_grace_note_sequential_event
+class AfterGraceNoteConsecution(abjad_parameters.abc.BangLastAttachment):
+    def __init__(self, after_grace_note_consecution: abjad.AfterGraceContainer):
+        self._after_grace_note_consecution = after_grace_note_consecution
 
     @classmethod
     def from_indicator_collection(
         cls, indicator_collection: music_parameters.abc.IndicatorCollection, **kwargs
     ) -> typing.Optional[abjad_parameters.abc.AbjadAttachment]:
         """Always return None.
 
-        AfterGraceNoteSequentialEvent can't be initialised from IndicatorCollection.
+        AfterGraceNoteConsecution can't be initialised from IndicatorCollection.
         """
         return None
 
     @property
     def is_active(self) -> bool:
         return True
 
     def process_leaf(self, leaf: abjad.Leaf) -> LeafOrLeafSequence:
-        abjad.attach(self._after_grace_note_sequential_event, leaf)
+        abjad.attach(self._after_grace_note_consecution, leaf)
         return leaf
 
 
 def set_note_head_style(
     leaf: abjad.Chord, note_head_index: int = 0, style: str = "#'harmonic"
 ):
     abjad.tweak(
```

### Comparing `mutwo.abjad-0.19.0/mutwo/abjad_parameters/configurations.py` & `mutwo_abjad-0.20.0/mutwo/abjad_parameters/configurations.py`

 * *Files identical despite different names*

### Comparing `mutwo.abjad-0.19.0/mutwo/abjad_utilities/abjad.py` & `mutwo_abjad-0.20.0/mutwo/abjad_utilities/abjad.py`

 * *Files identical despite different names*

### Comparing `mutwo.abjad-0.19.0/mutwo/abjad_utilities/tests.py` & `mutwo_abjad-0.20.0/mutwo/abjad_utilities/tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,20 +45,20 @@
 
     def _test(
         self,
         name: str,
         reset_tests: bool = False,
         force_png: bool = False,
         converter=None,
-        ev: core_events.abc.Event = core_events.SequentialEvent(
-            [core_events.SimpleEvent(1)]
+        ev: core_events.abc.Event = core_events.Consecution(
+            [core_events.Chronon(1)]
         ),
     ):
         if converter is None:
-            converter = self._abjad_converters.SequentialEventToAbjadVoice()
+            converter = self._abjad_converters.ConsecutionToAbjadVoice()
 
         converted_event = converter.convert(_parse_event(ev))
 
         p = self.base_path
 
         ly_ok_path = f"{p}{os.sep}{name}_ok.ly"
         ly_test_path = f"{p}{os.sep}{name}_test.ly"
@@ -119,18 +119,18 @@
     def _abjad_converters(self):
         return __import__("mutwo.abjad_converters").abjad_converters
 
 
 def _parse_event(ev):
     match ev:
         case music_events.NoteLike():
-            ev = core_events.SequentialEvent([ev])
-        case core_events.SequentialEvent():
+            ev = core_events.Consecution([ev])
+        case core_events.Consecution():
             ev = ev
-        case core_events.SimultaneousEvent():
+        case core_events.Concurrence():
             ev = ev
         case _:
             raise NotImplementedError(type(ev))
     return ev
 
 
 def run_if_ekmelily_available(method_to_wrap: typing.Callable):
```

### Comparing `mutwo.abjad-0.19.0/mutwo/abjad_utilities/tools.py` & `mutwo_abjad-0.20.0/mutwo/abjad_utilities/tools.py`

 * *Files identical despite different names*

### Comparing `mutwo.abjad-0.19.0/mutwo.abjad.egg-info/PKG-INFO` & `mutwo_abjad-0.20.0/mutwo.abjad.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: mutwo.abjad
-Version: 0.19.0
+Version: 0.20.0
 Summary: abjad extension for event based framework mutwo
 Home-page: https://github.com/mutwo-org/mutwo.abjad
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo-org.github.io
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mutwo.core<2.0.0,>=1.4.0
-Requires-Dist: mutwo.music<1.0.0,>=0.26.0
+Requires-Dist: mutwo.core<3.0.0,>=2.0.0
+Requires-Dist: mutwo.music<1.0.0,>=0.27.0
 Requires-Dist: abjad<3.12.0,>=3.9.0
 Requires-Dist: abjad-ext-nauert<3.12.0,>=3.9.0
 Requires-Dist: python-ranges<2.0.0,>=1.2.0
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.1; extra == "testing"
-Requires-Dist: mutwo.ekmelily<1.0.0,>=0.8.0; extra == "testing"
+Requires-Dist: mutwo.ekmelily<1.0.0,>=0.9.0; extra == "testing"
 
 # mutwo.abjad
 
 [![Build Status](https://circleci.com/gh/mutwo-org/mutwo.abjad.svg?style=shield)](https://circleci.com/gh/mutwo-org/mutwo.abjad)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![PyPI version](https://badge.fury.io/py/mutwo.abjad.svg)](https://badge.fury.io/py/mutwo.abjad)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `mutwo.abjad-0.19.0/mutwo.abjad.egg-info/SOURCES.txt` & `mutwo_abjad-0.20.0/mutwo.abjad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mutwo.abjad-0.19.0/mutwo_third_party/abjad/__init__.py` & `mutwo_abjad-0.20.0/mutwo_third_party/abjad/__init__.py`

 * *Files identical despite different names*

### Comparing `mutwo.abjad-0.19.0/setup.py` & `mutwo_abjad-0.20.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 extras_require = {
     "testing": [
         "pytest>=7.1.1",
-        "mutwo.ekmelily>=0.8.0, <1.0.0",
+        "mutwo.ekmelily>=0.9.0, <1.0.0",
     ]
 }
 
 setuptools.setup(
     name="mutwo.abjad",
     version=VERSION,
     license="GPL",
@@ -33,16 +33,16 @@
             include=["mutwo.*", "mutwo_third_party.*"]
         )
         if package[:5] != "tests"
     ],
     setup_requires=[],
     install_requires=[
         # Mutwo dependencies
-        "mutwo.core>=1.4.0, <2.0.0",
-        "mutwo.music>=0.26.0, <1.0.0",
+        "mutwo.core>=2.0.0, <3.0.0",
+        "mutwo.music>=0.27.0, <1.0.0",
         # Abjad dependencies
         "abjad>=3.9.0, <3.12.0",
         "abjad-ext-nauert>=3.9.0, <3.12.0",
         # Other dependencies
         "python-ranges>=1.2.0, <2.0.0",
     ],
     extras_require=extras_require,
```

