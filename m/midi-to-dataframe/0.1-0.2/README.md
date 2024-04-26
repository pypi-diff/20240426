# Comparing `tmp/midi_to_dataframe-0.1.tar.gz` & `tmp/midi_to_dataframe-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midi_to_dataframe-0.1.tar", last modified: Fri Apr 26 16:05:00 2024, max compression
+gzip compressed data, was "midi_to_dataframe-0.2.tar", last modified: Fri Apr 26 16:23:35 2024, max compression
```

## Comparing `midi_to_dataframe-0.1.tar` & `midi_to_dataframe-0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 taylor     (501) staff       (20)        0 2024-04-26 16:05:00.127084 midi_to_dataframe-0.1/
--rw-r--r--   0 taylor     (501) staff       (20)     4119 2024-04-26 16:03:04.000000 midi_to_dataframe-0.1/LICENSE
--rw-r--r--   0 taylor     (501) staff       (20)       68 2024-04-26 16:03:54.000000 midi_to_dataframe-0.1/MANIFEST.in
--rw-r--r--   0 taylor     (501) staff       (20)     1327 2024-04-26 16:05:00.126388 midi_to_dataframe-0.1/PKG-INFO
--rw-r--r--   0 taylor     (501) staff       (20)     1038 2024-04-26 15:58:56.000000 midi_to_dataframe-0.1/README.md
-drwxr-xr-x   0 taylor     (501) staff       (20)        0 2024-04-26 16:05:00.122275 midi_to_dataframe-0.1/midi_to_dataframe/
--rw-r--r--   0 taylor     (501) staff       (20)      108 2024-04-26 15:58:56.000000 midi_to_dataframe-0.1/midi_to_dataframe/__init__.py
--rw-r--r--   0 taylor     (501) staff       (20)    16656 2024-04-26 15:58:56.000000 midi_to_dataframe-0.1/midi_to_dataframe/midi_reader.py
--rw-r--r--   0 taylor     (501) staff       (20)     8228 2024-04-26 15:58:56.000000 midi_to_dataframe-0.1/midi_to_dataframe/midi_writer.py
--rw-r--r--   0 taylor     (501) staff       (20)     5450 2024-04-26 15:58:56.000000 midi_to_dataframe-0.1/midi_to_dataframe/note_mapper.py
-drwxr-xr-x   0 taylor     (501) staff       (20)        0 2024-04-26 16:05:00.125898 midi_to_dataframe-0.1/midi_to_dataframe.egg-info/
--rw-r--r--   0 taylor     (501) staff       (20)     1327 2024-04-26 16:05:00.000000 midi_to_dataframe-0.1/midi_to_dataframe.egg-info/PKG-INFO
--rw-r--r--   0 taylor     (501) staff       (20)      364 2024-04-26 16:05:00.000000 midi_to_dataframe-0.1/midi_to_dataframe.egg-info/SOURCES.txt
--rw-r--r--   0 taylor     (501) staff       (20)        1 2024-04-26 16:05:00.000000 midi_to_dataframe-0.1/midi_to_dataframe.egg-info/dependency_links.txt
--rw-r--r--   0 taylor     (501) staff       (20)       24 2024-04-26 16:05:00.000000 midi_to_dataframe-0.1/midi_to_dataframe.egg-info/top_level.txt
--rw-r--r--   0 taylor     (501) staff       (20)       38 2024-04-26 16:05:00.127265 midi_to_dataframe-0.1/setup.cfg
--rw-r--r--   0 taylor     (501) staff       (20)      600 2024-04-26 16:00:37.000000 midi_to_dataframe-0.1/setup.py
-drwxr-xr-x   0 taylor     (501) staff       (20)        0 2024-04-26 16:05:00.125052 midi_to_dataframe-0.1/tests/
--rw-r--r--   0 taylor     (501) staff       (20)        0 2024-04-26 15:58:56.000000 midi_to_dataframe-0.1/tests/__init__.py
--rw-r--r--   0 taylor     (501) staff       (20)      885 2024-04-26 15:58:56.000000 midi_to_dataframe-0.1/tests/tests.py
+drwxr-xr-x   0 taylor     (501) staff       (20)        0 2024-04-26 16:23:35.389544 midi_to_dataframe-0.2/
+-rw-r--r--   0 taylor     (501) staff       (20)     4119 2024-04-26 16:03:04.000000 midi_to_dataframe-0.2/LICENSE
+-rw-r--r--   0 taylor     (501) staff       (20)       68 2024-04-26 16:03:54.000000 midi_to_dataframe-0.2/MANIFEST.in
+-rw-r--r--   0 taylor     (501) staff       (20)     1327 2024-04-26 16:23:35.388793 midi_to_dataframe-0.2/PKG-INFO
+-rw-r--r--   0 taylor     (501) staff       (20)     1038 2024-04-26 15:58:56.000000 midi_to_dataframe-0.2/README.md
+drwxr-xr-x   0 taylor     (501) staff       (20)        0 2024-04-26 16:23:35.384535 midi_to_dataframe-0.2/midi_to_dataframe/
+-rw-r--r--   0 taylor     (501) staff       (20)      108 2024-04-26 15:58:56.000000 midi_to_dataframe-0.2/midi_to_dataframe/__init__.py
+-rw-r--r--   0 taylor     (501) staff       (20)    16656 2024-04-26 15:58:56.000000 midi_to_dataframe-0.2/midi_to_dataframe/midi_reader.py
+-rw-r--r--   0 taylor     (501) staff       (20)     8228 2024-04-26 15:58:56.000000 midi_to_dataframe-0.2/midi_to_dataframe/midi_writer.py
+-rw-r--r--   0 taylor     (501) staff       (20)     5450 2024-04-26 15:58:56.000000 midi_to_dataframe-0.2/midi_to_dataframe/note_mapper.py
+drwxr-xr-x   0 taylor     (501) staff       (20)        0 2024-04-26 16:23:35.388193 midi_to_dataframe-0.2/midi_to_dataframe.egg-info/
+-rw-r--r--   0 taylor     (501) staff       (20)     1327 2024-04-26 16:23:35.000000 midi_to_dataframe-0.2/midi_to_dataframe.egg-info/PKG-INFO
+-rw-r--r--   0 taylor     (501) staff       (20)      364 2024-04-26 16:23:35.000000 midi_to_dataframe-0.2/midi_to_dataframe.egg-info/SOURCES.txt
+-rw-r--r--   0 taylor     (501) staff       (20)        1 2024-04-26 16:23:35.000000 midi_to_dataframe-0.2/midi_to_dataframe.egg-info/dependency_links.txt
+-rw-r--r--   0 taylor     (501) staff       (20)       24 2024-04-26 16:23:35.000000 midi_to_dataframe-0.2/midi_to_dataframe.egg-info/top_level.txt
+-rw-r--r--   0 taylor     (501) staff       (20)       38 2024-04-26 16:23:35.389690 midi_to_dataframe-0.2/setup.cfg
+-rw-r--r--   0 taylor     (501) staff       (20)      600 2024-04-26 16:23:17.000000 midi_to_dataframe-0.2/setup.py
+drwxr-xr-x   0 taylor     (501) staff       (20)        0 2024-04-26 16:23:35.387232 midi_to_dataframe-0.2/tests/
+-rw-r--r--   0 taylor     (501) staff       (20)        0 2024-04-26 15:58:56.000000 midi_to_dataframe-0.2/tests/__init__.py
+-rw-r--r--   0 taylor     (501) staff       (20)      885 2024-04-26 15:58:56.000000 midi_to_dataframe-0.2/tests/tests.py
```

### Comparing `midi_to_dataframe-0.1/LICENSE` & `midi_to_dataframe-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `midi_to_dataframe-0.1/PKG-INFO` & `midi_to_dataframe-0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midi_to_dataframe
-Version: 0.1
+Version: 0.2
 Summary: Python library for converting between MIDI files and Pandas DataFrame objects.
 Home-page: https://github.com/TaylorPeer/midi-to-dataframe
 Author: Taylor Peer
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MIDI-to-DataFrame
```

### Comparing `midi_to_dataframe-0.1/README.md` & `midi_to_dataframe-0.2/README.md`

 * *Files identical despite different names*

### Comparing `midi_to_dataframe-0.1/midi_to_dataframe/midi_reader.py` & `midi_to_dataframe-0.2/midi_to_dataframe/midi_reader.py`

 * *Files identical despite different names*

### Comparing `midi_to_dataframe-0.1/midi_to_dataframe/midi_writer.py` & `midi_to_dataframe-0.2/midi_to_dataframe/midi_writer.py`

 * *Files identical despite different names*

### Comparing `midi_to_dataframe-0.1/midi_to_dataframe/note_mapper.py` & `midi_to_dataframe-0.2/midi_to_dataframe/note_mapper.py`

 * *Files identical despite different names*

### Comparing `midi_to_dataframe-0.1/midi_to_dataframe.egg-info/PKG-INFO` & `midi_to_dataframe-0.2/midi_to_dataframe.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midi_to_dataframe
-Version: 0.1
+Version: 0.2
 Summary: Python library for converting between MIDI files and Pandas DataFrame objects.
 Home-page: https://github.com/TaylorPeer/midi-to-dataframe
 Author: Taylor Peer
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MIDI-to-DataFrame
```

### Comparing `midi_to_dataframe-0.1/setup.py` & `midi_to_dataframe-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 # Define version information
-VERSION = '0.1'
+VERSION = '0.2'
 FULLVERSION = VERSION
 
 requirements = [
 ]
 
 setup(name='midi_to_dataframe',
       version=VERSION,
```

### Comparing `midi_to_dataframe-0.1/tests/tests.py` & `midi_to_dataframe-0.2/tests/tests.py`

 * *Files identical despite different names*

