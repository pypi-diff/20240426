# Comparing `tmp/eral-0.0.5.tar.gz` & `tmp/eral-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eral-0.0.5.tar", last modified: Fri Apr 26 11:36:11 2024, max compression
+gzip compressed data, was "eral-0.0.6.tar", last modified: Fri Apr 26 11:38:24 2024, max compression
```

## Comparing `eral-0.0.5.tar` & `eral-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 11:36:11.824462 eral-0.0.5/
--rw-rw-rw-   0        0        0     3590 2024-04-26 11:36:11.821462 eral-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2794 2024-04-26 11:21:23.000000 eral-0.0.5/README package.md
--rw-rw-rw-   0        0        0     2972 2024-04-26 11:21:39.000000 eral-0.0.5/README.md
--rw-rw-rw-   0        0        0      801 2024-04-26 11:35:46.000000 eral-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-26 11:36:11.824462 eral-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-26 11:36:11.755462 eral-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 11:36:11.785495 eral-0.0.5/src/eral/
--rw-rw-rw-   0        0        0        0 2023-10-25 13:21:15.000000 eral-0.0.5/src/eral/__init__.py
--rw-rw-rw-   0        0        0     9222 2024-04-12 09:13:29.000000 eral-0.0.5/src/eral/alignment_prototyping_functions.py
--rw-rw-rw-   0        0        0     8236 2024-04-10 12:02:33.000000 eral-0.0.5/src/eral/eral.py
--rw-rw-rw-   0        0        0     4313 2024-04-10 11:36:54.000000 eral-0.0.5/src/eral/eral_score.py
--rw-rw-rw-   0        0        0     7492 2024-04-10 12:12:14.000000 eral-0.0.5/src/eral/time_series_alignment.py
--rw-rw-rw-   0        0        0     1957 2024-02-18 16:15:48.000000 eral-0.0.5/src/eral/time_series_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-26 11:36:11.817461 eral-0.0.5/src/eral.egg-info/
--rw-rw-rw-   0        0        0     3590 2024-04-26 11:36:11.000000 eral-0.0.5/src/eral.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2024-04-26 11:36:11.000000 eral-0.0.5/src/eral.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 11:36:11.000000 eral-0.0.5/src/eral.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      177 2024-04-26 11:36:11.000000 eral-0.0.5/src/eral.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-26 11:36:11.000000 eral-0.0.5/src/eral.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 11:38:24.473481 eral-0.0.6/
+-rw-rw-rw-   0        0        0     3664 2024-04-26 11:38:24.471481 eral-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2868 2024-04-26 11:38:02.000000 eral-0.0.6/README package.md
+-rw-rw-rw-   0        0        0     2972 2024-04-26 11:21:39.000000 eral-0.0.6/README.md
+-rw-rw-rw-   0        0        0      801 2024-04-26 11:38:14.000000 eral-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 11:38:24.474481 eral-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 11:38:24.405484 eral-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 11:38:24.432484 eral-0.0.6/src/eral/
+-rw-rw-rw-   0        0        0        0 2023-10-25 13:21:15.000000 eral-0.0.6/src/eral/__init__.py
+-rw-rw-rw-   0        0        0     9222 2024-04-12 09:13:29.000000 eral-0.0.6/src/eral/alignment_prototyping_functions.py
+-rw-rw-rw-   0        0        0     8236 2024-04-10 12:02:33.000000 eral-0.0.6/src/eral/eral.py
+-rw-rw-rw-   0        0        0     4313 2024-04-10 11:36:54.000000 eral-0.0.6/src/eral/eral_score.py
+-rw-rw-rw-   0        0        0     7492 2024-04-10 12:12:14.000000 eral-0.0.6/src/eral/time_series_alignment.py
+-rw-rw-rw-   0        0        0     1957 2024-02-18 16:15:48.000000 eral-0.0.6/src/eral/time_series_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-26 11:38:24.468482 eral-0.0.6/src/eral.egg-info/
+-rw-rw-rw-   0        0        0     3664 2024-04-26 11:38:24.000000 eral-0.0.6/src/eral.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-04-26 11:38:24.000000 eral-0.0.6/src/eral.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 11:38:24.000000 eral-0.0.6/src/eral.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      177 2024-04-26 11:38:24.000000 eral-0.0.6/src/eral.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-26 11:38:24.000000 eral-0.0.6/src/eral.egg-info/top_level.txt
```

### Comparing `eral-0.0.5/PKG-INFO` & `eral-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eral
-Version: 0.0.5
+Version: 0.0.6
 Summary: Implementation of ERAL algorithm (Stržinar et al., 2024)
 Author-email: Žiga Stržinar <ziga.strzinar@ijs.si>
 Project-URL: Homepage, https://repo.ijs.si/zstrzinar/eral
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -61,15 +61,15 @@
                                    exclusion_zone=0.2)
 ```
 
 For full examples, please refer to the `examples/` directory at [our repository](https://repo.ijs.si/zstrzinar/eral).
 
 ## Demonstration
 The following figure demonstrates ERAL algorithm on a set of time series from the Trace dataset from UCR Archive. The dataset contains 100 time series, each with 275 samples. The time series are aligned and averaged using ERAL, and the resulting prototype is shown in the figure.
-![ERAL demonstration](docs/assets/trace-prototypes.png)
+![ERAL demonstration](https://repo.ijs.si/zstrzinar/eral/-/raw/main/docs/assets/trace-comparison.png?ref_type=heads&inline=false)
 
 
 ## Examples
 
 The `examples/` directory at [our repository](https://repo.ijs.si/zstrzinar/eral) contains Jupyter notebooks that illustrate different uses and capabilities of the ERAL algorithm. 
 To run an example, navigate to the `examples/` directory and execute the desired notebook.
```

### Comparing `eral-0.0.5/README package.md` & `eral-0.0.6/README package.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                                    exclusion_zone=0.2)
 ```
 
 For full examples, please refer to the `examples/` directory at [our repository](https://repo.ijs.si/zstrzinar/eral).
 
 ## Demonstration
 The following figure demonstrates ERAL algorithm on a set of time series from the Trace dataset from UCR Archive. The dataset contains 100 time series, each with 275 samples. The time series are aligned and averaged using ERAL, and the resulting prototype is shown in the figure.
-![ERAL demonstration](docs/assets/trace-prototypes.png)
+![ERAL demonstration](https://repo.ijs.si/zstrzinar/eral/-/raw/main/docs/assets/trace-comparison.png?ref_type=heads&inline=false)
 
 
 ## Examples
 
 The `examples/` directory at [our repository](https://repo.ijs.si/zstrzinar/eral) contains Jupyter notebooks that illustrate different uses and capabilities of the ERAL algorithm. 
 To run an example, navigate to the `examples/` directory and execute the desired notebook.
```

### Comparing `eral-0.0.5/README.md` & `eral-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `eral-0.0.5/pyproject.toml` & `eral-0.0.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "eral"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name="Žiga Stržinar", email="ziga.strzinar@ijs.si" },
 ]
 description = "Implementation of ERAL algorithm (Stržinar et al., 2024)"
 readme = "README package.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `eral-0.0.5/src/eral/alignment_prototyping_functions.py` & `eral-0.0.6/src/eral/alignment_prototyping_functions.py`

 * *Files identical despite different names*

### Comparing `eral-0.0.5/src/eral/eral.py` & `eral-0.0.6/src/eral/eral.py`

 * *Files identical despite different names*

### Comparing `eral-0.0.5/src/eral/eral_score.py` & `eral-0.0.6/src/eral/eral_score.py`

 * *Files identical despite different names*

### Comparing `eral-0.0.5/src/eral/time_series_alignment.py` & `eral-0.0.6/src/eral/time_series_alignment.py`

 * *Files identical despite different names*

### Comparing `eral-0.0.5/src/eral/time_series_helpers.py` & `eral-0.0.6/src/eral/time_series_helpers.py`

 * *Files identical despite different names*

### Comparing `eral-0.0.5/src/eral.egg-info/PKG-INFO` & `eral-0.0.6/src/eral.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eral
-Version: 0.0.5
+Version: 0.0.6
 Summary: Implementation of ERAL algorithm (Stržinar et al., 2024)
 Author-email: Žiga Stržinar <ziga.strzinar@ijs.si>
 Project-URL: Homepage, https://repo.ijs.si/zstrzinar/eral
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -61,15 +61,15 @@
                                    exclusion_zone=0.2)
 ```
 
 For full examples, please refer to the `examples/` directory at [our repository](https://repo.ijs.si/zstrzinar/eral).
 
 ## Demonstration
 The following figure demonstrates ERAL algorithm on a set of time series from the Trace dataset from UCR Archive. The dataset contains 100 time series, each with 275 samples. The time series are aligned and averaged using ERAL, and the resulting prototype is shown in the figure.
-![ERAL demonstration](docs/assets/trace-prototypes.png)
+![ERAL demonstration](https://repo.ijs.si/zstrzinar/eral/-/raw/main/docs/assets/trace-comparison.png?ref_type=heads&inline=false)
 
 
 ## Examples
 
 The `examples/` directory at [our repository](https://repo.ijs.si/zstrzinar/eral) contains Jupyter notebooks that illustrate different uses and capabilities of the ERAL algorithm. 
 To run an example, navigate to the `examples/` directory and execute the desired notebook.
```

