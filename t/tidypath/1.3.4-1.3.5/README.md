# Comparing `tmp/tidypath-1.3.4.tar.gz` & `tmp/tidypath-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidypath-1.3.4.tar", last modified: Fri Apr 26 08:30:12 2024, max compression
+gzip compressed data, was "tidypath-1.3.5.tar", last modified: Fri Apr 26 08:34:06 2024, max compression
```

## Comparing `tidypath-1.3.4.tar` & `tidypath-1.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-26 08:30:12.323393 tidypath-1.3.4/
--rwxr-xr-x   0 userx     (1000) wheel      (998)    35149 2023-06-08 21:46:44.000000 tidypath-1.3.4/LICENSE.md
--rw-r--r--   0 userx     (1000) wheel      (998)     3682 2024-04-26 08:30:12.323393 tidypath-1.3.4/PKG-INFO
--rwxr-xr-x   0 userx     (1000) wheel      (998)     2804 2023-06-08 21:46:44.000000 tidypath-1.3.4/README.md
--rwxr-xr-x   0 userx     (1000) wheel      (998)      106 2024-04-26 08:30:12.323393 tidypath-1.3.4/setup.cfg
--rwxr-xr-x   0 userx     (1000) wheel      (998)     1161 2024-04-26 08:29:52.000000 tidypath-1.3.4/setup.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-26 08:30:12.323393 tidypath-1.3.4/tidypath/
--rwxr-xr-x   0 userx     (1000) wheel      (998)      371 2023-09-01 13:40:54.000000 tidypath-1.3.4/tidypath/__init__.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     1629 2023-06-08 21:46:44.000000 tidypath-1.3.4/tidypath/_helper.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     4998 2024-02-21 23:01:12.000000 tidypath-1.3.4/tidypath/config.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)    14366 2024-04-26 08:29:43.000000 tidypath-1.3.4/tidypath/decorators.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     6165 2023-07-01 08:06:57.000000 tidypath-1.3.4/tidypath/fmt.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     5197 2023-06-08 21:46:44.000000 tidypath-1.3.4/tidypath/inspection.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)    14158 2024-02-14 00:36:13.000000 tidypath-1.3.4/tidypath/paths.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     9844 2023-06-08 21:46:44.000000 tidypath-1.3.4/tidypath/storage.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-26 08:30:12.323393 tidypath-1.3.4/tidypath.egg-info/
--rwxr-xr-x   0 userx     (1000) wheel      (998)     3682 2024-04-26 08:30:12.000000 tidypath-1.3.4/tidypath.egg-info/PKG-INFO
--rwxr-xr-x   0 userx     (1000) wheel      (998)      358 2024-04-26 08:30:12.000000 tidypath-1.3.4/tidypath.egg-info/SOURCES.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)        1 2024-04-26 08:30:12.000000 tidypath-1.3.4/tidypath.egg-info/dependency_links.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)       63 2024-04-26 08:30:12.000000 tidypath-1.3.4/tidypath.egg-info/requires.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)        9 2024-04-26 08:30:12.000000 tidypath-1.3.4/tidypath.egg-info/top_level.txt
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-26 08:34:06.993405 tidypath-1.3.5/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)    35149 2023-06-08 21:46:44.000000 tidypath-1.3.5/LICENSE.md
+-rw-r--r--   0 userx     (1000) wheel      (998)     3682 2024-04-26 08:34:06.993405 tidypath-1.3.5/PKG-INFO
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     2804 2023-06-08 21:46:44.000000 tidypath-1.3.5/README.md
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      106 2024-04-26 08:34:06.993405 tidypath-1.3.5/setup.cfg
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     1161 2024-04-26 08:33:47.000000 tidypath-1.3.5/setup.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-26 08:34:06.993405 tidypath-1.3.5/tidypath/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      371 2023-09-01 13:40:54.000000 tidypath-1.3.5/tidypath/__init__.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     1629 2023-06-08 21:46:44.000000 tidypath-1.3.5/tidypath/_helper.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     4998 2024-02-21 23:01:12.000000 tidypath-1.3.5/tidypath/config.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)    14368 2024-04-26 08:33:12.000000 tidypath-1.3.5/tidypath/decorators.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     6165 2023-07-01 08:06:57.000000 tidypath-1.3.5/tidypath/fmt.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     5197 2023-06-08 21:46:44.000000 tidypath-1.3.5/tidypath/inspection.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)    14158 2024-02-14 00:36:13.000000 tidypath-1.3.5/tidypath/paths.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     9844 2023-06-08 21:46:44.000000 tidypath-1.3.5/tidypath/storage.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-26 08:34:06.993405 tidypath-1.3.5/tidypath.egg-info/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     3682 2024-04-26 08:34:06.000000 tidypath-1.3.5/tidypath.egg-info/PKG-INFO
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      358 2024-04-26 08:34:06.000000 tidypath-1.3.5/tidypath.egg-info/SOURCES.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)        1 2024-04-26 08:34:06.000000 tidypath-1.3.5/tidypath.egg-info/dependency_links.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)       63 2024-04-26 08:34:06.000000 tidypath-1.3.5/tidypath.egg-info/requires.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)        9 2024-04-26 08:34:06.000000 tidypath-1.3.5/tidypath.egg-info/top_level.txt
```

### Comparing `tidypath-1.3.4/LICENSE.md` & `tidypath-1.3.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.4/PKG-INFO` & `tidypath-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.3.4
+Version: 1.3.5
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tidypath-1.3.4/README.md` & `tidypath-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.4/setup.py` & `tidypath-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tidypath',
-    version='1.3.4',
+    version='1.3.5',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=['tidypath'],
     url='https://github.com/medinajorge/tidypath',
     download_url='https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz',
     description="Automatically store/load data in a tidy, efficient way.",
     long_description=open('README.md').read(),
```

### Comparing `tidypath-1.3.4/tidypath/_helper.py` & `tidypath-1.3.5/tidypath/_helper.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.4/tidypath/config.py` & `tidypath-1.3.5/tidypath/config.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.4/tidypath/decorators.py` & `tidypath-1.3.5/tidypath/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
             for ext_i in ext:
                 saving_path = get_saving_path(ext_i)
                 if skip_computation and not Path(saving_path).exists():
                     warnings.warn("Skipping computation. Data not stored.", RuntimeWarning)
                     return SavedataSkippedComputation()
                 elif Path(saving_path).exists() and not overwrite:
                     try:
-                        result = getattr(storage, f"load_{ext}")(saving_path, **load_opts)
+                        result = getattr(storage, f"load_{ext_i}")(saving_path, **load_opts)
                     except EOFError or LZMAError or _lzma.LZMAError:
                         if skip_computation:
                             warnings.warn("Corrupted file. Skipping computation ...", RuntimeWarning)
                             return SavedataSkippedComputation()
                         else:
                             warnings.warn("Corrupted file. Recomputing and storing ...", RuntimeWarning)
                             result = compute_and_save(result, ext_i, saving_path)
```

### Comparing `tidypath-1.3.4/tidypath/fmt.py` & `tidypath-1.3.5/tidypath/fmt.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.4/tidypath/inspection.py` & `tidypath-1.3.5/tidypath/inspection.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.4/tidypath/paths.py` & `tidypath-1.3.5/tidypath/paths.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.4/tidypath/storage.py` & `tidypath-1.3.5/tidypath/storage.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.4/tidypath.egg-info/PKG-INFO` & `tidypath-1.3.5/tidypath.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.3.4
+Version: 1.3.5
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

