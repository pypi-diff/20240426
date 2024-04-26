# Comparing `tmp/eral-0.0.2.tar.gz` & `tmp/eral-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eral-0.0.2.tar", last modified: Fri Apr 26 10:41:06 2024, max compression
+gzip compressed data, was "eral-0.0.3.tar", last modified: Fri Apr 26 11:02:01 2024, max compression
```

## Comparing `eral-0.0.2.tar` & `eral-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 10:41:06.184097 eral-0.0.2/
--rw-rw-rw-   0        0        0     3321 2024-04-26 10:41:06.181096 eral-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2556 2024-04-26 10:09:06.000000 eral-0.0.2/README.md
--rw-rw-rw-   0        0        0      767 2024-04-26 10:40:53.000000 eral-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-26 10:41:06.184097 eral-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-26 10:41:06.121096 eral-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 10:41:06.147094 eral-0.0.2/src/eral/
--rw-rw-rw-   0        0        0        0 2023-10-25 13:21:15.000000 eral-0.0.2/src/eral/__init__.py
--rw-rw-rw-   0        0        0     9222 2024-04-12 09:13:29.000000 eral-0.0.2/src/eral/alignment_prototyping_functions.py
--rw-rw-rw-   0        0        0     8236 2024-04-10 12:02:33.000000 eral-0.0.2/src/eral/eral.py
--rw-rw-rw-   0        0        0     4313 2024-04-10 11:36:54.000000 eral-0.0.2/src/eral/eral_score.py
--rw-rw-rw-   0        0        0     7492 2024-04-10 12:12:14.000000 eral-0.0.2/src/eral/time_series_alignment.py
--rw-rw-rw-   0        0        0     1957 2024-02-18 16:15:48.000000 eral-0.0.2/src/eral/time_series_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:41:06.178096 eral-0.0.2/src/eral.egg-info/
--rw-rw-rw-   0        0        0     3321 2024-04-26 10:41:06.000000 eral-0.0.2/src/eral.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-04-26 10:41:06.000000 eral-0.0.2/src/eral.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 10:41:06.000000 eral-0.0.2/src/eral.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      159 2024-04-26 10:41:06.000000 eral-0.0.2/src/eral.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-26 10:41:06.000000 eral-0.0.2/src/eral.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 11:02:01.449059 eral-0.0.3/
+-rw-rw-rw-   0        0        0     3355 2024-04-26 11:02:01.446059 eral-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2556 2024-04-26 10:09:06.000000 eral-0.0.3/README.md
+-rw-rw-rw-   0        0        0      793 2024-04-26 11:01:13.000000 eral-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 11:02:01.450059 eral-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 11:02:01.358059 eral-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 11:02:01.403058 eral-0.0.3/src/eral/
+-rw-rw-rw-   0        0        0        0 2023-10-25 13:21:15.000000 eral-0.0.3/src/eral/__init__.py
+-rw-rw-rw-   0        0        0     9222 2024-04-12 09:13:29.000000 eral-0.0.3/src/eral/alignment_prototyping_functions.py
+-rw-rw-rw-   0        0        0     8236 2024-04-10 12:02:33.000000 eral-0.0.3/src/eral/eral.py
+-rw-rw-rw-   0        0        0     4313 2024-04-10 11:36:54.000000 eral-0.0.3/src/eral/eral_score.py
+-rw-rw-rw-   0        0        0     7492 2024-04-10 12:12:14.000000 eral-0.0.3/src/eral/time_series_alignment.py
+-rw-rw-rw-   0        0        0     1957 2024-02-18 16:15:48.000000 eral-0.0.3/src/eral/time_series_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-26 11:02:01.443059 eral-0.0.3/src/eral.egg-info/
+-rw-rw-rw-   0        0        0     3355 2024-04-26 11:02:01.000000 eral-0.0.3/src/eral.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-04-26 11:02:01.000000 eral-0.0.3/src/eral.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 11:02:01.000000 eral-0.0.3/src/eral.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      177 2024-04-26 11:02:01.000000 eral-0.0.3/src/eral.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-26 11:02:01.000000 eral-0.0.3/src/eral.egg-info/top_level.txt
```

### Comparing `eral-0.0.2/PKG-INFO` & `eral-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: eral
-Version: 0.0.2
+Version: 0.0.3
 Summary: Implementation of ERAL algorithm (Stržinar et al., 2024)
 Author-email: Žiga Stržinar <ziga.strzinar@ijs.si>
 Project-URL: Homepage, https://repo.ijs.si/zstrzinar/eral
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: dtw-python>=1.3.0
+Requires-Dist: matplotlib>=3.6.2
 Requires-Dist: numpy>=1.23.4
 Requires-Dist: pandas<2.0.0,>=1.4.3
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: scikit-learn>=1.2.1
 Requires-Dist: scipy>=1.9.0
 Requires-Dist: tslearn>=0.6.3
 Requires-Dist: line-profiler>=4.1.2
```

### Comparing `eral-0.0.2/README.md` & `eral-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `eral-0.0.2/pyproject.toml` & `eral-0.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [project]
 name = "eral"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Žiga Stržinar", email="ziga.strzinar@ijs.si" },
 ]
 description = "Implementation of ERAL algorithm (Stržinar et al., 2024)"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "dtw-python>=1.3.0",
+    "matplotlib>=3.6.2",
     "numpy>=1.23.4",
     "pandas>=1.4.3, <2.0.0",
     "python-dateutil>=2.8.2",
     "scikit-learn>=1.2.1",
     "scipy>=1.9.0",
     "tslearn>=0.6.3",
     "line-profiler>=4.1.2",
```

### Comparing `eral-0.0.2/src/eral/alignment_prototyping_functions.py` & `eral-0.0.3/src/eral/alignment_prototyping_functions.py`

 * *Files identical despite different names*

### Comparing `eral-0.0.2/src/eral/eral.py` & `eral-0.0.3/src/eral/eral.py`

 * *Files identical despite different names*

### Comparing `eral-0.0.2/src/eral/eral_score.py` & `eral-0.0.3/src/eral/eral_score.py`

 * *Files identical despite different names*

### Comparing `eral-0.0.2/src/eral/time_series_alignment.py` & `eral-0.0.3/src/eral/time_series_alignment.py`

 * *Files identical despite different names*

### Comparing `eral-0.0.2/src/eral/time_series_helpers.py` & `eral-0.0.3/src/eral/time_series_helpers.py`

 * *Files identical despite different names*

### Comparing `eral-0.0.2/src/eral.egg-info/PKG-INFO` & `eral-0.0.3/src/eral.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: eral
-Version: 0.0.2
+Version: 0.0.3
 Summary: Implementation of ERAL algorithm (Stržinar et al., 2024)
 Author-email: Žiga Stržinar <ziga.strzinar@ijs.si>
 Project-URL: Homepage, https://repo.ijs.si/zstrzinar/eral
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: dtw-python>=1.3.0
+Requires-Dist: matplotlib>=3.6.2
 Requires-Dist: numpy>=1.23.4
 Requires-Dist: pandas<2.0.0,>=1.4.3
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: scikit-learn>=1.2.1
 Requires-Dist: scipy>=1.9.0
 Requires-Dist: tslearn>=0.6.3
 Requires-Dist: line-profiler>=4.1.2
```

