# Comparing `tmp/infodesreg-0.0.2.tar.gz` & `tmp/infodesreg-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infodesreg-0.0.2.tar", last modified: Fri Apr 26 18:13:55 2024, max compression
+gzip compressed data, was "infodesreg-0.0.3.tar", last modified: Fri Apr 26 18:22:03 2024, max compression
```

## Comparing `infodesreg-0.0.2.tar` & `infodesreg-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:13:55.871930 infodesreg-0.0.2/
--rw-r--r--   0 firuzjuraev   (501) staff       (20)     1073 2024-04-26 17:42:23.000000 infodesreg-0.0.2/LICENSE
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      713 2024-04-26 18:13:55.871740 infodesreg-0.0.2/PKG-INFO
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      202 2024-04-26 17:42:07.000000 infodesreg-0.0.2/README.md
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      491 2024-04-26 18:13:16.000000 infodesreg-0.0.2/pyproject.toml
--rw-r--r--   0 firuzjuraev   (501) staff       (20)       38 2024-04-26 18:13:55.871967 infodesreg-0.0.2/setup.cfg
-drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:13:55.869922 infodesreg-0.0.2/src/
-drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:13:55.870803 infodesreg-0.0.2/src/dynamic_regressor_fjuraev/
--rw-r--r--   0 firuzjuraev   (501) staff       (20)       20 2024-04-26 18:13:06.000000 infodesreg-0.0.2/src/dynamic_regressor_fjuraev/__init__.py
--rw-r--r--   0 firuzjuraev   (501) staff       (20)     4994 2024-04-26 17:34:16.000000 infodesreg-0.0.2/src/dynamic_regressor_fjuraev/base.py
-drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:13:55.871579 infodesreg-0.0.2/src/infodesreg.egg-info/
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      713 2024-04-26 18:13:55.000000 infodesreg-0.0.2/src/infodesreg.egg-info/PKG-INFO
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      264 2024-04-26 18:13:55.000000 infodesreg-0.0.2/src/infodesreg.egg-info/SOURCES.txt
--rw-r--r--   0 firuzjuraev   (501) staff       (20)        1 2024-04-26 18:13:55.000000 infodesreg-0.0.2/src/infodesreg.egg-info/dependency_links.txt
--rw-r--r--   0 firuzjuraev   (501) staff       (20)       26 2024-04-26 18:13:55.000000 infodesreg-0.0.2/src/infodesreg.egg-info/top_level.txt
+drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:22:03.943185 infodesreg-0.0.3/
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)     1073 2024-04-26 17:42:23.000000 infodesreg-0.0.3/LICENSE
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)      713 2024-04-26 18:22:03.943021 infodesreg-0.0.3/PKG-INFO
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)      202 2024-04-26 17:42:07.000000 infodesreg-0.0.3/README.md
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)      491 2024-04-26 18:21:51.000000 infodesreg-0.0.3/pyproject.toml
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)       38 2024-04-26 18:22:03.943220 infodesreg-0.0.3/setup.cfg
+drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:22:03.941001 infodesreg-0.0.3/src/
+drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:22:03.942084 infodesreg-0.0.3/src/dynamic_regressor_fjuraev/
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)       20 2024-04-26 18:13:06.000000 infodesreg-0.0.3/src/dynamic_regressor_fjuraev/__init__.py
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)     4994 2024-04-26 17:34:16.000000 infodesreg-0.0.3/src/dynamic_regressor_fjuraev/base.py
+drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:22:03.942883 infodesreg-0.0.3/src/infodesreg.egg-info/
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)      713 2024-04-26 18:22:03.000000 infodesreg-0.0.3/src/infodesreg.egg-info/PKG-INFO
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)      264 2024-04-26 18:22:03.000000 infodesreg-0.0.3/src/infodesreg.egg-info/SOURCES.txt
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)        1 2024-04-26 18:22:03.000000 infodesreg-0.0.3/src/infodesreg.egg-info/dependency_links.txt
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)       26 2024-04-26 18:22:03.000000 infodesreg-0.0.3/src/infodesreg.egg-info/top_level.txt
```

### Comparing `infodesreg-0.0.2/LICENSE` & `infodesreg-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `infodesreg-0.0.2/PKG-INFO` & `infodesreg-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infodesreg
-Version: 0.0.2
+Version: 0.0.3
 Summary: Dynamic Ensemble Selectio for Regression tasks
 Author-email: Panda <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `infodesreg-0.0.2/src/dynamic_regressor_fjuraev/base.py` & `infodesreg-0.0.3/src/dynamic_regressor_fjuraev/base.py`

 * *Files identical despite different names*

### Comparing `infodesreg-0.0.2/src/infodesreg.egg-info/PKG-INFO` & `infodesreg-0.0.3/src/infodesreg.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infodesreg
-Version: 0.0.2
+Version: 0.0.3
 Summary: Dynamic Ensemble Selectio for Regression tasks
 Author-email: Panda <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```
