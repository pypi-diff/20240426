# Comparing `tmp/hatch_pyinstaller-1.0.tar.gz` & `tmp/hatch_pyinstaller-1.0.1.tar.gz`

## Comparing `hatch_pyinstaller-1.0.tar` & `hatch_pyinstaller-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 hatch_pyinstaller-1.0/README.md
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 hatch_pyinstaller-1.0/hatch_pyinstaller/__init__.py
--rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 hatch_pyinstaller-1.0/hatch_pyinstaller/builder.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hatch_pyinstaller-1.0/hatch_pyinstaller/hooks.py
--rw-r--r--   0        0        0    18431 2020-02-02 00:00:00.000000 hatch_pyinstaller-1.0/LICENCE.txt
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 hatch_pyinstaller-1.0/pyproject.toml
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 hatch_pyinstaller-1.0/PKG-INFO
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 hatch_pyinstaller-1.0.1/README.md
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 hatch_pyinstaller-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_pyinstaller-1.0.1/hatch_pyinstaller/__init__.py
+-rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 hatch_pyinstaller-1.0.1/hatch_pyinstaller/builder.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hatch_pyinstaller-1.0.1/hatch_pyinstaller/hooks.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hatch_pyinstaller-1.0.1/.gitignore
+-rw-r--r--   0        0        0    18431 2020-02-02 00:00:00.000000 hatch_pyinstaller-1.0.1/LICENCE.txt
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 hatch_pyinstaller-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 hatch_pyinstaller-1.0.1/PKG-INFO
```

### Comparing `hatch_pyinstaller-1.0/README.md` & `hatch_pyinstaller-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hatch_pyinstaller-1.0/hatch_pyinstaller/builder.py` & `hatch_pyinstaller-1.0.1/hatch_pyinstaller/builder.py`

 * *Files identical despite different names*

### Comparing `hatch_pyinstaller-1.0/LICENCE.txt` & `hatch_pyinstaller-1.0.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `hatch_pyinstaller-1.0/pyproject.toml` & `hatch_pyinstaller-1.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [project]
 name = "hatch-pyinstaller"
 dependencies = ["hatchling", "PyInstaller"]
 requires-python = ">= 3.7"
 licence = "GPL 2.0"
 keywords = ["hatch", "packaging"]
 authors = [{ name = "William Smith", email = "williams@citisyn.net" }]
-description = "Time tracking application that can submit timecards to AiM"
+description = "Hatch plugin for building binaries using PyInstaller"
 dynamic = ["version"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Plugins",
     "Framework :: Hatch",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
```

### Comparing `hatch_pyinstaller-1.0/PKG-INFO` & `hatch_pyinstaller-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: hatch-pyinstaller
-Version: 1.0
-Summary: Time tracking application that can submit timecards to AiM
+Version: 1.0.1
+Summary: Hatch plugin for building binaries using PyInstaller
 Project-URL: Homepage, https://github.com/mxysptlk/hatch-pyinstaller
 Author-email: William Smith <williams@citisyn.net>
 License-File: LICENCE.txt
 Keywords: hatch,packaging
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Framework :: Hatch
```

