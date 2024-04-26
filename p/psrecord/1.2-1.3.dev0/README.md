# Comparing `tmp/psrecord-1.2.tar.gz` & `tmp/psrecord-1.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/psrecord-1.2.tar", last modified: Thu May 28 13:08:24 2020, max compression
+gzip compressed data, was "psrecord-1.3.dev0.tar", last modified: Fri Apr 26 10:55:49 2024, max compression
```

## Comparing `psrecord-1.2.tar` & `psrecord-1.3.dev0.tar`

### file list

```diff
@@ -1,23 +1,32 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2020-05-28 13:08:24.018787 psrecord-1.2/
--rw-rw-r--   0 tom       (1000) tom       (1000)      875 2020-05-28 13:07:30.000000 psrecord-1.2/CHANGES.md
--rw-rw-r--   0 tom       (1000) tom       (1000)     1299 2020-05-28 09:33:31.000000 psrecord-1.2/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       77 2020-05-28 09:33:31.000000 psrecord-1.2/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)     3992 2020-05-28 13:08:24.014787 psrecord-1.2/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     2626 2020-05-28 09:33:31.000000 psrecord-1.2/README.rst
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2020-05-28 13:08:24.014787 psrecord-1.2/psrecord/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1396 2020-05-28 13:07:44.000000 psrecord-1.2/psrecord/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     7602 2020-05-28 13:06:04.000000 psrecord-1.2/psrecord/main.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2020-05-28 13:08:24.014787 psrecord-1.2/psrecord/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2020-05-28 09:33:31.000000 psrecord-1.2/psrecord/tests/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1726 2020-05-28 09:33:31.000000 psrecord-1.2/psrecord/tests/test_main.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2020-05-28 13:08:24.014787 psrecord-1.2/psrecord.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)     3992 2020-05-28 13:08:23.000000 psrecord-1.2/psrecord.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      334 2020-05-28 13:08:23.000000 psrecord-1.2/psrecord.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2020-05-28 13:08:23.000000 psrecord-1.2/psrecord.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       10 2020-05-28 13:08:23.000000 psrecord-1.2/psrecord.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        9 2020-05-28 13:08:23.000000 psrecord-1.2/psrecord.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)    51707 2020-05-28 09:33:31.000000 psrecord-1.2/screenshot.png
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2020-05-28 13:08:24.014787 psrecord-1.2/scripts/
--rwxrwxr-x   0 tom       (1000) tom       (1000)      107 2020-05-28 09:33:31.000000 psrecord-1.2/scripts/psrecord
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2020-05-28 13:08:24.018787 psrecord-1.2/setup.cfg
--rwxrwxr-x   0 tom       (1000) tom       (1000)     2302 2020-05-28 13:06:04.000000 psrecord-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:55:49.625949 psrecord-1.3.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:55:49.621949 psrecord-1.3.dev0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:55:49.621949 psrecord-1.3.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/.github/workflows/update-changelog.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-26 10:55:49.625949 psrecord-1.3.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:55:49.625949 psrecord-1.3.dev0/psrecord/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/psrecord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/psrecord/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-26 10:55:49.000000 psrecord-1.3.dev0/psrecord/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/psrecord/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:55:49.625949 psrecord-1.3.dev0/psrecord/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/psrecord/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/psrecord/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:55:49.625949 psrecord-1.3.dev0/psrecord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-26 10:55:49.000000 psrecord-1.3.dev0/psrecord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-26 10:55:49.000000 psrecord-1.3.dev0/psrecord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:55:49.000000 psrecord-1.3.dev0/psrecord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-26 10:55:49.000000 psrecord-1.3.dev0/psrecord.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 10:55:49.000000 psrecord-1.3.dev0/psrecord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 10:55:49.000000 psrecord-1.3.dev0/psrecord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:55:49.000000 psrecord-1.3.dev0/psrecord.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    51707 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 10:55:49.625949 psrecord-1.3.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/tox.ini
```

### Comparing `psrecord-1.2/CHANGES.md` & `psrecord-1.3.dev0/CHANGES.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-1.2 (2020-05-28)
-----------------
+## 1.2 (2020-05-28)
 
 - Fixed compatibility with latest versions of psutil and fixed issue with
   determining CPU usage from child processes. [#56]
 
 - Fixed plotting to work on machines where Agg is not the default
   Matplotlib backend. [#44]
 
-1.1 (2018-06-16)
-----------------
+## 1.1 (2018-06-16)
 
 - Fixed installation via pip if psutil was not installed. [#37]
 
-1.0 (2016-12-05)
-----------------
+## 1.0 (2016-12-05)
 
 - Fix compatibility with recent versions of psutil. [#18, #19]
 
 - psutil is now properly defined as a dependency in install_requires. [#16]
 
-0.2 (2014-10-22)
-----------------
+## 0.2 (2014-10-22)
 
 - Recognize zombie processes. [#7]
 
 - Improve general reliability.
 
 - Allow interval to be a floating-point value.
 
 - Fix compatibility with psutil >= 2.0. [#10]
 
-- Ensure that log file gets closed and plot gets drawn if process is
-  interrupted. [#13]
+- Ensure that log file gets closed and plot gets drawn if process is interrupted. [#13]
 
-0.1 (2013-12-17)
-----------------
+## 0.1 (2013-12-17)
 
 - Initial release
```

### Comparing `psrecord-1.2/LICENSE` & `psrecord-1.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `psrecord-1.2/README.rst` & `psrecord-1.3.dev0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 Installation
 ============
 
 To install, simply do::
 
     pip install psrecord
 
+To install with the optional plotting dependencies, do::
+
+    pip install psrecord[plot]
+
 Usage
 =====
 
 Basics
 ------
 
 To record the CPU and memory activity of an existing process to a file (use sudo for a root process):
```

### Comparing `psrecord-1.2/psrecord/__init__.py` & `psrecord-1.3.dev0/psrecord/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,10 +19,11 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-from .main import main  # noqa
+from .main import main
 
-__version__ = '1.2'
+__version__ = "1.3.dev0"
+main()
```

### Comparing `psrecord-1.2/screenshot.png` & `psrecord-1.3.dev0/screenshot.png`

 * *Files identical despite different names*

### Comparing `psrecord-1.2/setup.py` & `psrecord-1.3.dev0/psrecord/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,30 @@
-#!/usr/bin/env python
-#
 # Copyright (c) 2013, Thomas P. Robitaille
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
-# 1. Redistributions of source code must retain the above copyright notice, this
-# list of conditions and the following disclaimer.
+# 1. Redistributions of source code must retain the above copyright notice,
+# this list of conditions and the following disclaimer.
 #
 # 2. Redistributions in binary form must reproduce the above copyright notice,
 # this list of conditions and the following disclaimer in the documentation
 # and/or other materials provided with the distribution.
 #
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
 # AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-from setuptools import setup, Command
-
-from distutils.command.build_py import build_py
-
-with open('README.rst') as infile:
-    long_description = infile.read()
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+# ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+# LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+# CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+# SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+# INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+# CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+# ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+# POSSIBILITY OF SUCH DAMAGE.
 
-from psrecord import __version__
+from .main import main  # noqa
+from .main import monitor  # noqa
+from ._version import __version__  # noqa
 
-setup(name='psrecord',
-      version=__version__,
-      description='Python package to record activity from processes',
-      long_description=long_description,
-      url='https://github.com/astrofrog/psrecord',
-      license='Simplified BSD License',
-      author='Thomas Robitaille',
-      author_email='thomas.robitaille@gmail.com',
-      packages=['psrecord', 'psrecord.tests'],
-      provides=['psrecord'],
-      scripts=['scripts/psrecord'],
-      install_requires=['psutil>=2'],
-      cmdclass={'build_py': build_py},
-      classifiers=[
-                   "Development Status :: 3 - Alpha",
-                   "Programming Language :: Python",
-                   "License :: OSI Approved :: BSD License",
-                  ],
-     )
+__all__ = ["main", "monitor", "__version__"]
```

