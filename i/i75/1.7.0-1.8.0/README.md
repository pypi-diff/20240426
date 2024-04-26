# Comparing `tmp/i75-1.7.0.tar.gz` & `tmp/i75-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i75-1.7.0.tar", last modified: Wed Mar 20 21:55:10 2024, max compression
+gzip compressed data, was "i75-1.8.0.tar", last modified: Fri Apr 26 20:30:05 2024, max compression
```

## Comparing `i75-1.7.0.tar` & `i75-1.8.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:55:10.636125 i75-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-20 21:54:48.000000 i75-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-20 21:54:48.000000 i75-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-03-20 21:55:10.636125 i75-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-03-20 21:54:48.000000 i75-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:55:10.628125 i75-1.7.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1300 2024-03-20 21:54:48.000000 i75-1.7.0/bin/i75
--rwxr-xr-x   0 runner    (1001) docker     (127)     2132 2024-03-20 21:54:48.000000 i75-1.7.0/bin/i75-convert-image
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:55:10.628125 i75-1.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 21:54:48.000000 i75-1.7.0/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:55:10.632125 i75-1.7.0/i75/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-20 21:55:09.000000 i75-1.7.0/i75/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-03-20 21:54:48.000000 i75-1.7.0/i75/basei75.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-20 21:54:48.000000 i75-1.7.0/i75/colour.py
--rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-03-20 21:54:48.000000 i75-1.7.0/i75/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:55:10.632125 i75-1.7.0/i75/emulated/
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-03-20 21:54:48.000000 i75-1.7.0/i75/emulated/hub75.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-03-20 21:54:48.000000 i75-1.7.0/i75/emulated/machine.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-20 21:54:48.000000 i75-1.7.0/i75/emulated/micropython.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-20 21:54:48.000000 i75-1.7.0/i75/emulated/mp_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-03-20 21:54:48.000000 i75-1.7.0/i75/emulated/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-20 21:54:48.000000 i75-1.7.0/i75/emulated/ntptime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-20 21:54:48.000000 i75-1.7.0/i75/emulated/pen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-03-20 21:54:48.000000 i75-1.7.0/i75/emulated/picographics.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-20 21:54:48.000000 i75-1.7.0/i75/emulated/pimoroni.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-20 21:54:48.000000 i75-1.7.0/i75/emulated/pimoroni_i2c.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 21:54:48.000000 i75-1.7.0/i75/emulated/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-03-20 21:54:48.000000 i75-1.7.0/i75/emulated/urequests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-03-20 21:54:48.000000 i75-1.7.0/i75/emulatedi75.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:55:10.632125 i75-1.7.0/i75/fontdata/
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-03-20 21:55:04.000000 i75-1.7.0/i75/fontdata/cg_pixel_3x5_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-03-20 21:54:48.000000 i75-1.7.0/i75/graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-03-20 21:54:48.000000 i75-1.7.0/i75/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-03-20 21:54:48.000000 i75-1.7.0/i75/nativei75.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 21:54:48.000000 i75-1.7.0/i75/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-03-20 21:54:48.000000 i75-1.7.0/i75/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:55:10.632125 i75-1.7.0/i75/tz/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-20 21:54:48.000000 i75-1.7.0/i75/tz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-03-20 21:54:48.000000 i75-1.7.0/i75/tz/europe_london.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:55:10.632125 i75-1.7.0/i75.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-03-20 21:55:10.000000 i75-1.7.0/i75.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-20 21:55:10.000000 i75-1.7.0/i75.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 21:55:10.000000 i75-1.7.0/i75.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-20 21:55:10.000000 i75-1.7.0/i75.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-20 21:55:10.000000 i75-1.7.0/i75.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-20 21:54:48.000000 i75-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 21:55:10.636125 i75-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-03-20 21:54:48.000000 i75-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:55:10.632125 i75-1.7.0/stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-20 21:54:48.000000 i75-1.7.0/stubs/gc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-20 21:54:48.000000 i75-1.7.0/stubs/machine.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-20 21:54:48.000000 i75-1.7.0/stubs/time.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:55:10.636125 i75-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-20 21:54:48.000000 i75-1.7.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:55:10.636125 i75-1.7.0/tests/emulated/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-20 21:54:48.000000 i75-1.7.0/tests/emulated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-20 21:54:48.000000 i75-1.7.0/tests/emulated/test_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-20 21:54:48.000000 i75-1.7.0/tests/emulated/test_pen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-20 21:54:48.000000 i75-1.7.0/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-20 21:54:48.000000 i75-1.7.0/tests/test_emulatedi75.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-20 21:54:48.000000 i75-1.7.0/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-03-20 21:54:48.000000 i75-1.7.0/tests/test_linedrawing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-20 21:54:48.000000 i75-1.7.0/tests/test_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:55:10.636125 i75-1.7.0/tests/tz/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-20 21:54:48.000000 i75-1.7.0/tests/tz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-03-20 21:54:48.000000 i75-1.7.0/tests/tz/test_europe_london.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:30:05.202952 i75-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-26 20:29:45.000000 i75-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 20:29:45.000000 i75-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-04-26 20:30:05.202952 i75-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-26 20:29:45.000000 i75-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:30:05.194952 i75-1.8.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1300 2024-04-26 20:29:45.000000 i75-1.8.0/bin/i75
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2233 2024-04-26 20:29:45.000000 i75-1.8.0/bin/i75-convert-image
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:30:05.194952 i75-1.8.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:29:45.000000 i75-1.8.0/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:30:05.198952 i75-1.8.0/i75/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-26 20:30:04.000000 i75-1.8.0/i75/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-04-26 20:29:45.000000 i75-1.8.0/i75/basei75.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-26 20:29:45.000000 i75-1.8.0/i75/colour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-04-26 20:29:45.000000 i75-1.8.0/i75/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:30:05.198952 i75-1.8.0/i75/emulated/
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-26 20:29:45.000000 i75-1.8.0/i75/emulated/hub75.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-26 20:29:45.000000 i75-1.8.0/i75/emulated/machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-26 20:29:45.000000 i75-1.8.0/i75/emulated/micropython.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-26 20:29:45.000000 i75-1.8.0/i75/emulated/mp_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-26 20:29:45.000000 i75-1.8.0/i75/emulated/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-26 20:29:45.000000 i75-1.8.0/i75/emulated/ntptime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-26 20:29:45.000000 i75-1.8.0/i75/emulated/pen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-26 20:29:45.000000 i75-1.8.0/i75/emulated/picographics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-26 20:29:45.000000 i75-1.8.0/i75/emulated/pimoroni.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-26 20:29:45.000000 i75-1.8.0/i75/emulated/pimoroni_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:29:45.000000 i75-1.8.0/i75/emulated/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-26 20:29:45.000000 i75-1.8.0/i75/emulated/urequests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-26 20:29:45.000000 i75-1.8.0/i75/emulatedi75.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:30:05.198952 i75-1.8.0/i75/fontdata/
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-26 20:29:59.000000 i75-1.8.0/i75/fontdata/cg_pixel_3x5_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-26 20:29:45.000000 i75-1.8.0/i75/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-26 20:29:45.000000 i75-1.8.0/i75/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-26 20:29:45.000000 i75-1.8.0/i75/nativei75.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:29:45.000000 i75-1.8.0/i75/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:30:05.198952 i75-1.8.0/i75/stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-26 20:29:45.000000 i75-1.8.0/i75/stubs/gc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-26 20:29:45.000000 i75-1.8.0/i75/stubs/machine.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-26 20:29:45.000000 i75-1.8.0/i75/stubs/time.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-26 20:29:45.000000 i75-1.8.0/i75/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:30:05.198952 i75-1.8.0/i75/tz/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-26 20:29:45.000000 i75-1.8.0/i75/tz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-26 20:29:45.000000 i75-1.8.0/i75/tz/europe_london.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:30:05.198952 i75-1.8.0/i75.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-04-26 20:30:05.000000 i75-1.8.0/i75.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-26 20:30:05.000000 i75-1.8.0/i75.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:30:05.000000 i75-1.8.0/i75.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-26 20:30:05.000000 i75-1.8.0/i75.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 20:30:05.000000 i75-1.8.0/i75.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-26 20:29:45.000000 i75-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 20:30:05.202952 i75-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-26 20:29:45.000000 i75-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:30:05.202952 i75-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-26 20:29:45.000000 i75-1.8.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:30:05.202952 i75-1.8.0/tests/emulated/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-26 20:29:45.000000 i75-1.8.0/tests/emulated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-26 20:29:45.000000 i75-1.8.0/tests/emulated/test_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-26 20:29:45.000000 i75-1.8.0/tests/emulated/test_pen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-26 20:29:45.000000 i75-1.8.0/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-26 20:29:45.000000 i75-1.8.0/tests/test_emulatedi75.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-26 20:29:45.000000 i75-1.8.0/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-26 20:29:45.000000 i75-1.8.0/tests/test_linedrawing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-26 20:29:45.000000 i75-1.8.0/tests/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:30:05.202952 i75-1.8.0/tests/tz/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-26 20:29:45.000000 i75-1.8.0/tests/tz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-26 20:29:45.000000 i75-1.8.0/tests/tz/test_europe_london.py
```

### Comparing `i75-1.7.0/LICENSE` & `i75-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/PKG-INFO` & `i75-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i75
-Version: 1.7.0
+Version: 1.8.0
 Summary: A wrapper around Pimoroni's `interstate75` library which allows for running locally and easier testing.
 Home-page: https://github.com/andrewjw/i75
 Author: Andrew Wilkinson
 Author-email: andrewjwilkinson@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `i75-1.7.0/README.md` & `i75-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/bin/i75` & `i75-1.8.0/bin/i75`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/bin/i75-convert-image` & `i75-1.8.0/bin/i75-convert-image`

 * *Files 10% similar despite different names*

```diff
@@ -35,15 +35,18 @@
             r += byte.to_bytes(1, byteorder='big')
     return r
 
 def three_colour(im: Image.Image) -> bytes:
     val: bytes = b""
     for y in range(im.height):
         for x in range(im.width):
-            r, g, b = im.getpixel((x, y))
+            try:
+                r, g, b = im.getpixel((x, y))
+            except ValueError:
+                r, g, b, a = im.getpixel((x, y))
             val += r.to_bytes(1, byteorder='big')
             val += g.to_bytes(1, byteorder='big')
             val += b.to_bytes(1, byteorder='big')
     return val
 
 def main() -> None:
     im = Image.open(sys.argv[1])
```

### Comparing `i75-1.7.0/i75/__init__.py` & `i75-1.8.0/i75/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "1.7.0"
+__version__ = "1.8.0"
 
 import picographics
 if hasattr(picographics, "DisplayType"):
     from .emulatedi75 import EmulatedI75
     I75 = EmulatedI75  # type: ignore
 else:
     from .nativei75 import NativeI75
```

### Comparing `i75-1.7.0/i75/basei75.py` & `i75-1.8.0/i75/basei75.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/colour.py` & `i75-1.8.0/i75/colour.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/datetime.py` & `i75-1.8.0/i75/datetime.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/emulated/hub75.py` & `i75-1.8.0/i75/emulated/hub75.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/emulated/machine.py` & `i75-1.8.0/i75/emulated/machine.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/emulated/micropython.py` & `i75-1.8.0/i75/emulated/micropython.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/emulated/mp_time.py` & `i75-1.8.0/i75/emulated/mp_time.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/emulated/network.py` & `i75-1.8.0/i75/emulated/network.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/emulated/ntptime.py` & `i75-1.8.0/i75/emulated/ntptime.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/emulated/pen.py` & `i75-1.8.0/i75/emulated/pen.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/emulated/picographics.py` & `i75-1.8.0/i75/emulated/picographics.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/emulated/pimoroni.py` & `i75-1.8.0/i75/emulated/pimoroni.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/emulated/pimoroni_i2c.py` & `i75-1.8.0/i75/emulated/pimoroni_i2c.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/emulated/urequests.py` & `i75-1.8.0/i75/emulated/urequests.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/emulatedi75.py` & `i75-1.8.0/i75/emulatedi75.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/fontdata/cg_pixel_3x5_5.py` & `i75-1.8.0/i75/fontdata/cg_pixel_3x5_5.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 # This font data was generated from
 # data/cg-pixel-3x5/cg-pixel-3x5.ttf with size 5.
 HEIGHT = 6
 SPACE_WIDTH = 3
 DATA = {
-    '$': (3, b'\x06\x03\x02\x06\x03\x00'),
-    'N': (3, b'\x03\x05\x05\x05\x05\x00'),
-    '|': (1, b'\x01\x01\x00\x01\x01\x00'),
-    '-': (3, b'\x00\x00\x07\x00\x00\x00'),
-    '"': (3, b'\x05\x05\x00\x00\x00\x00'),
-    'Z': (3, b'\x07\x04\x02\x01\x07\x00'),
-    '0': (3, b'\x07\x05\x05\x05\x07\x00'),
-    '#': (3, b'\x05\x07\x05\x07\x05\x00'),
-    'O': (3, b'\x02\x05\x05\x05\x02\x00'),
-    "'": (1, b'\x01\x01\x00\x00\x00\x00'),
+    '@': (3, b'\x02\x05\x07\x01\x06\x00'),
+    '1': (2, b'\x02\x03\x02\x02\x02\x00'),
     '*': (3, b'\x05\x02\x07\x02\x05\x00'),
-    ']': (2, b'\x03\x02\x02\x02\x03\x00'),
-    '&': (3, b'\x06\x01\x06\x05\x06\x00'),
     'I': (1, b'\x01\x01\x01\x01\x01\x00'),
-    '4': (3, b'\x05\x05\x07\x04\x04\x00'),
-    '6': (3, b'\x06\x01\x03\x05\x02\x00'),
-    'R': (3, b'\x03\x05\x03\x05\x05\x00'),
-    ';': (2, b'\x00\x02\x00\x02\x01\x00'),
+    '#': (3, b'\x05\x07\x05\x07\x05\x00'),
+    'X': (3, b'\x05\x05\x02\x05\x05\x00'),
     '2': (3, b'\x03\x04\x02\x01\x07\x00'),
-    '`': (2, b'\x01\x02\x00\x00\x00\x00'),
-    'K': (3, b'\x05\x05\x03\x05\x05\x00'),
-    '{': (3, b'\x06\x02\x03\x02\x06\x00'),
-    '.': (1, b'\x00\x00\x00\x00\x01\x00'),
-    ':': (1, b'\x00\x01\x00\x01\x00\x00'),
-    '=': (3, b'\x00\x07\x00\x07\x00\x00'),
+    'P': (3, b'\x03\x05\x03\x01\x01\x00'),
     'U': (3, b'\x05\x05\x05\x05\x07\x00'),
-    'M': (3, b'\x05\x07\x05\x05\x05\x00'),
-    'W': (3, b'\x05\x05\x05\x07\x05\x00'),
-    '9': (3, b'\x02\x05\x06\x04\x03\x00'),
-    '?': (3, b'\x03\x04\x02\x00\x02\x00'),
-    '@': (3, b'\x02\x05\x07\x01\x06\x00'),
-    '[': (2, b'\x03\x01\x01\x01\x03\x00'),
-    'G': (3, b'\x06\x01\x01\x05\x06\x00'),
-    '}': (3, b'\x03\x02\x06\x02\x03\x00'),
-    '\\': (3, b'\x01\x01\x02\x04\x04\x00'),
-    'Q': (3, b'\x02\x05\x05\x07\x06\x00'),
-    '<': (3, b'\x04\x02\x01\x02\x04\x00'),
-    'V': (3, b'\x05\x05\x05\x07\x02\x00'),
     'C': (3, b'\x02\x05\x01\x05\x02\x00'),
-    'A': (3, b'\x02\x05\x07\x05\x05\x00'),
-    'E': (3, b'\x07\x01\x07\x01\x07\x00'),
-    'J': (3, b'\x04\x04\x04\x05\x02\x00'),
-    '>': (3, b'\x01\x02\x04\x02\x01\x00'),
-    '1': (2, b'\x02\x03\x02\x02\x02\x00'),
-    '_': (3, b'\x00\x00\x00\x00\x07\x00'),
+    ']': (2, b'\x03\x02\x02\x02\x03\x00'),
+    ':': (1, b'\x00\x01\x00\x01\x00\x00'),
+    'N': (3, b'\x03\x05\x05\x05\x05\x00'),
     '%': (3, b'\x01\x04\x02\x01\x04\x00'),
-    '8': (3, b'\x02\x05\x02\x05\x02\x00'),
-    '~': (3, b'\x00\x06\x03\x00\x00\x00'),
+    '4': (3, b'\x05\x05\x07\x04\x04\x00'),
+    '-': (3, b'\x00\x00\x07\x00\x00\x00'),
+    '7': (3, b'\x07\x04\x02\x02\x02\x00'),
+    'H': (3, b'\x05\x05\x07\x05\x05\x00'),
+    'S': (3, b'\x06\x01\x02\x04\x03\x00'),
+    '$': (3, b'\x06\x03\x02\x06\x03\x00'),
+    ';': (2, b'\x00\x02\x00\x02\x01\x00'),
+    ')': (2, b'\x01\x02\x02\x02\x01\x00'),
     '+': (3, b'\x00\x02\x07\x02\x00\x00'),
+    '>': (3, b'\x01\x02\x04\x02\x01\x00'),
+    'Y': (3, b'\x05\x05\x07\x02\x02\x00'),
+    'A': (3, b'\x02\x05\x07\x05\x05\x00'),
+    '6': (3, b'\x06\x01\x03\x05\x02\x00'),
+    'T': (3, b'\x07\x02\x02\x02\x02\x00'),
+    '[': (2, b'\x03\x01\x01\x01\x03\x00'),
+    'D': (3, b'\x03\x05\x05\x05\x03\x00'),
     '!': (1, b'\x01\x01\x01\x00\x01\x00'),
-    'P': (3, b'\x03\x05\x03\x01\x01\x00'),
+    'F': (3, b'\x07\x01\x07\x01\x01\x00'),
+    '?': (3, b'\x03\x04\x02\x00\x02\x00'),
+    '<': (3, b'\x04\x02\x01\x02\x04\x00'),
     ',': (2, b'\x00\x00\x00\x02\x01\x00'),
+    '`': (2, b'\x01\x02\x00\x00\x00\x00'),
     'B': (3, b'\x03\x05\x03\x05\x03\x00'),
+    '_': (3, b'\x00\x00\x00\x00\x07\x00'),
+    "'": (1, b'\x01\x01\x00\x00\x00\x00'),
+    '.': (1, b'\x00\x00\x00\x00\x01\x00'),
+    'R': (3, b'\x03\x05\x03\x05\x05\x00'),
     '5': (3, b'\x07\x01\x03\x04\x03\x00'),
-    '3': (3, b'\x03\x04\x02\x04\x03\x00'),
-    'L': (3, b'\x01\x01\x01\x01\x07\x00'),
-    'T': (3, b'\x07\x02\x02\x02\x02\x00'),
-    'S': (3, b'\x06\x01\x02\x04\x03\x00'),
-    '(': (2, b'\x02\x01\x01\x01\x02\x00'),
     '/': (3, b'\x04\x04\x02\x01\x01\x00'),
-    '7': (3, b'\x07\x04\x02\x02\x02\x00'),
-    'F': (3, b'\x07\x01\x07\x01\x01\x00'),
-    'Y': (3, b'\x05\x05\x07\x02\x02\x00'),
-    ')': (2, b'\x01\x02\x02\x02\x01\x00'),
-    'D': (3, b'\x03\x05\x05\x05\x03\x00'),
+    '(': (2, b'\x02\x01\x01\x01\x02\x00'),
+    '=': (3, b'\x00\x07\x00\x07\x00\x00'),
+    'Q': (3, b'\x02\x05\x05\x07\x06\x00'),
+    '|': (1, b'\x01\x01\x00\x01\x01\x00'),
+    'E': (3, b'\x07\x01\x07\x01\x07\x00'),
+    'W': (3, b'\x05\x05\x05\x07\x05\x00'),
+    '"': (3, b'\x05\x05\x00\x00\x00\x00'),
+    'O': (3, b'\x02\x05\x05\x05\x02\x00'),
+    '}': (3, b'\x03\x02\x06\x02\x03\x00'),
+    '0': (3, b'\x07\x05\x05\x05\x07\x00'),
+    'V': (3, b'\x05\x05\x05\x07\x02\x00'),
+    '~': (3, b'\x00\x06\x03\x00\x00\x00'),
+    '\\': (3, b'\x01\x01\x02\x04\x04\x00'),
+    'K': (3, b'\x05\x05\x03\x05\x05\x00'),
+    '3': (3, b'\x03\x04\x02\x04\x03\x00'),
+    'M': (3, b'\x05\x07\x05\x05\x05\x00'),
+    '&': (3, b'\x06\x01\x06\x05\x06\x00'),
     '^': (3, b'\x02\x05\x00\x00\x00\x00'),
-    'X': (3, b'\x05\x05\x02\x05\x05\x00'),
-    'H': (3, b'\x05\x05\x07\x05\x05\x00'),
+    'G': (3, b'\x06\x01\x01\x05\x06\x00'),
+    '{': (3, b'\x06\x02\x03\x02\x06\x00'),
+    'J': (3, b'\x04\x04\x04\x05\x02\x00'),
+    'Z': (3, b'\x07\x04\x02\x01\x07\x00'),
+    '9': (3, b'\x02\x05\x06\x04\x03\x00'),
+    'L': (3, b'\x01\x01\x01\x01\x07\x00'),
+    '8': (3, b'\x02\x05\x02\x05\x02\x00'),
 }
```

### Comparing `i75-1.7.0/i75/graphics.py` & `i75-1.8.0/i75/graphics.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/image.py` & `i75-1.8.0/i75/image.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/nativei75.py` & `i75-1.8.0/i75/nativei75.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/text.py` & `i75-1.8.0/i75/text.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/tz/__init__.py` & `i75-1.8.0/i75/tz/__init__.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75/tz/europe_london.py` & `i75-1.8.0/i75/tz/europe_london.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/i75.egg-info/PKG-INFO` & `i75-1.8.0/i75.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i75
-Version: 1.7.0
+Version: 1.8.0
 Summary: A wrapper around Pimoroni's `interstate75` library which allows for running locally and easier testing.
 Home-page: https://github.com/andrewjw/i75
 Author: Andrew Wilkinson
 Author-email: andrewjwilkinson@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `i75-1.7.0/i75.egg-info/SOURCES.txt` & `i75-1.8.0/i75.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 i75/emulated/pen.py
 i75/emulated/picographics.py
 i75/emulated/pimoroni.py
 i75/emulated/pimoroni_i2c.py
 i75/emulated/py.typed
 i75/emulated/urequests.py
 i75/fontdata/cg_pixel_3x5_5.py
+i75/stubs/gc.pyi
+i75/stubs/machine.pyi
+i75/stubs/time.pyi
 i75/tz/__init__.py
 i75/tz/europe_london.py
-stubs/gc.pyi
-stubs/machine.pyi
-stubs/time.pyi
 tests/__init__.py
 tests/test_datetime.py
 tests/test_emulatedi75.py
 tests/test_image.py
 tests/test_linedrawing.py
 tests/test_text.py
 tests/emulated/__init__.py
```

### Comparing `i75-1.7.0/pyproject.toml` & `i75-1.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/setup.py` & `i75-1.8.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,19 +35,16 @@
     author="Andrew Wilkinson",
     author_email="andrewjwilkinson@gmail.com",
     description="A wrapper around Pimoroni's `interstate75` library which allows for running locally and easier testing.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andrewjw/i75",
     scripts=["bin/i75", "bin/i75-convert-image"],
-    packages=setuptools.find_packages() + ["i75.emulated", "i75.tz", "i75.fontdata",],
-    include_package_data=True,
-    data_files = [
-        ('stubs', glob('stubs/*.pyi'))
-    ],
+    packages=setuptools.find_packages() + ["i75.emulated", "i75.tz", "i75.fontdata"],
+    package_data={"i75": ["stubs/*.pyi"]},
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `i75-1.7.0/stubs/gc.pyi` & `i75-1.8.0/i75/stubs/gc.pyi`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/stubs/machine.pyi` & `i75-1.8.0/i75/stubs/machine.pyi`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/stubs/time.pyi` & `i75-1.8.0/i75/stubs/time.pyi`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/tests/__init__.py` & `i75-1.8.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/tests/emulated/__init__.py` & `i75-1.8.0/tests/emulated/__init__.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/tests/emulated/test_machine.py` & `i75-1.8.0/tests/emulated/test_machine.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/tests/emulated/test_pen.py` & `i75-1.8.0/tests/emulated/test_pen.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/tests/test_datetime.py` & `i75-1.8.0/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/tests/test_emulatedi75.py` & `i75-1.8.0/tests/test_emulatedi75.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/tests/test_image.py` & `i75-1.8.0/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/tests/test_linedrawing.py` & `i75-1.8.0/tests/test_linedrawing.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/tests/test_text.py` & `i75-1.8.0/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/tests/tz/__init__.py` & `i75-1.8.0/tests/tz/__init__.py`

 * *Files identical despite different names*

### Comparing `i75-1.7.0/tests/tz/test_europe_london.py` & `i75-1.8.0/tests/tz/test_europe_london.py`

 * *Files identical despite different names*

