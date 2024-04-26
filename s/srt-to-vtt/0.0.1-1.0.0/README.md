# Comparing `tmp/srt_to_vtt-0.0.1.tar.gz` & `tmp/srt_to_vtt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srt_to_vtt-0.0.1.tar", last modified: Wed Apr 24 21:31:20 2024, max compression
+gzip compressed data, was "srt_to_vtt-1.0.0.tar", last modified: Thu Apr 25 20:32:41 2024, max compression
```

## Comparing `srt_to_vtt-0.0.1.tar` & `srt_to_vtt-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-24 21:31:20.409665 srt_to_vtt-0.0.1/
--rw-r--r--   0 joshuahamilton   (501) staff       (20)     1071 2024-04-24 19:42:32.000000 srt_to_vtt-0.0.1/LICENSE
--rw-r--r--   0 joshuahamilton   (501) staff       (20)      451 2024-04-24 21:31:20.409485 srt_to_vtt-0.0.1/PKG-INFO
--rw-r--r--   0 joshuahamilton   (501) staff       (20)       69 2024-04-24 19:31:44.000000 srt_to_vtt-0.0.1/README.md
--rw-r--r--   0 joshuahamilton   (501) staff       (20)       38 2024-04-24 21:31:20.409699 srt_to_vtt-0.0.1/setup.cfg
--rw-r--r--   0 joshuahamilton   (501) staff       (20)      625 2024-04-24 21:31:03.000000 srt_to_vtt-0.0.1/setup.py
-drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-24 21:31:20.408682 srt_to_vtt-0.0.1/srt_to_vtt/
--rw-r--r--   0 joshuahamilton   (501) staff       (20)       44 2024-04-24 21:07:49.000000 srt_to_vtt-0.0.1/srt_to_vtt/__init__.py
--rw-r--r--   0 joshuahamilton   (501) staff       (20)       29 2024-04-24 21:19:08.000000 srt_to_vtt-0.0.1/srt_to_vtt/srt_to_vtt.py
-drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-24 21:31:20.409326 srt_to_vtt-0.0.1/srt_to_vtt.egg-info/
--rw-r--r--   0 joshuahamilton   (501) staff       (20)      451 2024-04-24 21:31:20.000000 srt_to_vtt-0.0.1/srt_to_vtt.egg-info/PKG-INFO
--rw-r--r--   0 joshuahamilton   (501) staff       (20)      210 2024-04-24 21:31:20.000000 srt_to_vtt-0.0.1/srt_to_vtt.egg-info/SOURCES.txt
--rw-r--r--   0 joshuahamilton   (501) staff       (20)        1 2024-04-24 21:31:20.000000 srt_to_vtt-0.0.1/srt_to_vtt.egg-info/dependency_links.txt
--rw-r--r--   0 joshuahamilton   (501) staff       (20)       11 2024-04-24 21:31:20.000000 srt_to_vtt-0.0.1/srt_to_vtt.egg-info/top_level.txt
+drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-25 20:32:41.531621 srt_to_vtt-1.0.0/
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)     1071 2024-04-24 19:42:32.000000 srt_to_vtt-1.0.0/LICENSE
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)      451 2024-04-25 20:32:41.531418 srt_to_vtt-1.0.0/PKG-INFO
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)       69 2024-04-24 19:31:44.000000 srt_to_vtt-1.0.0/README.md
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)       38 2024-04-25 20:32:41.531665 srt_to_vtt-1.0.0/setup.cfg
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)      625 2024-04-25 20:31:21.000000 srt_to_vtt-1.0.0/setup.py
+drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-25 20:32:41.530310 srt_to_vtt-1.0.0/srt_to_vtt/
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)       34 2024-04-25 19:50:08.000000 srt_to_vtt-1.0.0/srt_to_vtt/__init__.py
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)      673 2024-04-25 20:19:22.000000 srt_to_vtt-1.0.0/srt_to_vtt/srt_to_vtt.py
+drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-25 20:32:41.531212 srt_to_vtt-1.0.0/srt_to_vtt.egg-info/
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)      451 2024-04-25 20:32:41.000000 srt_to_vtt-1.0.0/srt_to_vtt.egg-info/PKG-INFO
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)      235 2024-04-25 20:32:41.000000 srt_to_vtt-1.0.0/srt_to_vtt.egg-info/SOURCES.txt
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)        1 2024-04-25 20:32:41.000000 srt_to_vtt-1.0.0/srt_to_vtt.egg-info/dependency_links.txt
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)       11 2024-04-25 20:32:41.000000 srt_to_vtt-1.0.0/srt_to_vtt.egg-info/top_level.txt
+drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-25 20:32:41.530957 srt_to_vtt-1.0.0/tests/
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)      113 2024-04-25 20:15:33.000000 srt_to_vtt-1.0.0/tests/test_srt_to_vtt.py
```

### Comparing `srt_to_vtt-0.0.1/LICENSE` & `srt_to_vtt-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `srt_to_vtt-0.0.1/setup.py` & `srt_to_vtt-1.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='srt-to-vtt',
-    version='0.0.1',
+    version='1.0.0',
     packages=find_packages(),
     install_requires=[],
     author='Joshua Hamilton',
     author_email='hamiltonjoshuadavid@gmail.com',
     description='Python package to enable easy conversion of .srt files to .vtt files.',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

