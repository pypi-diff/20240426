# Comparing `tmp/autoviz-0.1.901.tar.gz` & `tmp/autoviz-0.1.902.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoviz-0.1.901.tar", last modified: Thu Apr 25 11:03:02 2024, max compression
+gzip compressed data, was "autoviz-0.1.902.tar", last modified: Fri Apr 26 11:46:39 2024, max compression
```

## Comparing `autoviz-0.1.901.tar` & `autoviz-0.1.902.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-04-25 11:03:02.464404 autoviz-0.1.901/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    17919 2024-04-25 11:03:02.460260 autoviz-0.1.901/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)    15585 2024-03-30 12:37:03.000000 autoviz-0.1.901/README.md
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-04-25 11:03:02.332745 autoviz-0.1.901/autoviz/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    34934 2024-04-01 12:36:55.000000 autoviz-0.1.901/autoviz/AutoViz_Class.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    64881 2024-04-15 14:08:34.000000 autoviz-0.1.901/autoviz/AutoViz_Holo.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    24022 2024-04-01 11:59:10.000000 autoviz-0.1.901/autoviz/AutoViz_NLP.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)   117365 2024-04-02 11:29:27.000000 autoviz-0.1.901/autoviz/AutoViz_Utils.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      875 2024-04-01 11:59:10.000000 autoviz-0.1.901/autoviz/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      404 2024-04-25 10:29:14.000000 autoviz-0.1.901/autoviz/__version__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    18388 2024-04-01 11:59:10.000000 autoviz-0.1.901/autoviz/classify_method.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-04-25 11:03:02.440736 autoviz-0.1.901/autoviz.egg-info/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    17919 2024-04-25 11:03:01.000000 autoviz-0.1.901/autoviz.egg-info/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)      339 2024-04-25 11:03:01.000000 autoviz-0.1.901/autoviz.egg-info/SOURCES.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2024-04-25 11:03:01.000000 autoviz-0.1.901/autoviz.egg-info/dependency_links.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)      256 2024-04-25 11:03:01.000000 autoviz-0.1.901/autoviz.egg-info/requires.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2024-04-25 11:03:01.000000 autoviz-0.1.901/autoviz.egg-info/top_level.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2024-04-25 11:03:02.464404 autoviz-0.1.901/setup.cfg
--rwxrwxrwx   0 ram       (1000) ram       (1000)     3013 2024-04-25 10:55:30.000000 autoviz-0.1.901/setup.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-04-26 11:46:39.401417 autoviz-0.1.902/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    17919 2024-04-26 11:46:39.401417 autoviz-0.1.902/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    15585 2024-03-30 12:37:03.000000 autoviz-0.1.902/README.md
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-04-26 11:46:39.263368 autoviz-0.1.902/autoviz/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    34934 2024-04-01 12:36:55.000000 autoviz-0.1.902/autoviz/AutoViz_Class.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    64881 2024-04-15 14:08:34.000000 autoviz-0.1.902/autoviz/AutoViz_Holo.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    24022 2024-04-01 11:59:10.000000 autoviz-0.1.902/autoviz/AutoViz_NLP.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)   117365 2024-04-02 11:29:27.000000 autoviz-0.1.902/autoviz/AutoViz_Utils.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      875 2024-04-01 11:59:10.000000 autoviz-0.1.902/autoviz/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      404 2024-04-25 10:29:14.000000 autoviz-0.1.902/autoviz/__version__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    18388 2024-04-01 11:59:10.000000 autoviz-0.1.902/autoviz/classify_method.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-04-26 11:46:39.385774 autoviz-0.1.902/autoviz.egg-info/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    17919 2024-04-26 11:46:38.000000 autoviz-0.1.902/autoviz.egg-info/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      339 2024-04-26 11:46:38.000000 autoviz-0.1.902/autoviz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2024-04-26 11:46:38.000000 autoviz-0.1.902/autoviz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      256 2024-04-26 11:46:38.000000 autoviz-0.1.902/autoviz.egg-info/requires.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2024-04-26 11:46:38.000000 autoviz-0.1.902/autoviz.egg-info/top_level.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2024-04-26 11:46:39.401417 autoviz-0.1.902/setup.cfg
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     3253 2024-04-25 12:32:02.000000 autoviz-0.1.902/setup.py
```

### Comparing `autoviz-0.1.901/PKG-INFO` & `autoviz-0.1.902/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.901
+Version: 0.1.902
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz.git
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # AutoViz: The One-Line Automatic Data Visualization Library
         
         ![logo](images/logo.png)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autoviz Version: 0.1.901 Summary: Automatically
+Metadata-Version: 2.1 Name: autoviz Version: 0.1.902 Summary: Automatically
 Visualize any dataset, any size with a single line of code Home-page: https://
 github.com/AutoViML/AutoViz.git Author: Ram Seshadri License: Apache License
 2.0 Description: # AutoViz: The One-Line Automatic Data Visualization Library !
 [logo](images/logo.png) Unlock the power of **AutoViz** to visualize any
 dataset, any size, with just a single line of code! Plus, now you can get a
 quick assessment of your dataset's quality and fix DQ issues through the FixDQ
 () function. [![Pepy Downloads](https://pepy.tech/badge/autoviz)](https://
```

### Comparing `autoviz-0.1.901/README.md` & `autoviz-0.1.902/README.md`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.901/autoviz/AutoViz_Class.py` & `autoviz-0.1.902/autoviz/AutoViz_Class.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.901/autoviz/AutoViz_Holo.py` & `autoviz-0.1.902/autoviz/AutoViz_Holo.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.901/autoviz/AutoViz_NLP.py` & `autoviz-0.1.902/autoviz/AutoViz_NLP.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.901/autoviz/AutoViz_Utils.py` & `autoviz-0.1.902/autoviz/AutoViz_Utils.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.901/autoviz/__init__.py` & `autoviz-0.1.902/autoviz/__init__.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.901/autoviz/classify_method.py` & `autoviz-0.1.902/autoviz/classify_method.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.901/autoviz.egg-info/PKG-INFO` & `autoviz-0.1.902/autoviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.901
+Version: 0.1.902
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz.git
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # AutoViz: The One-Line Automatic Data Visualization Library
         
         ![logo](images/logo.png)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autoviz Version: 0.1.901 Summary: Automatically
+Metadata-Version: 2.1 Name: autoviz Version: 0.1.902 Summary: Automatically
 Visualize any dataset, any size with a single line of code Home-page: https://
 github.com/AutoViML/AutoViz.git Author: Ram Seshadri License: Apache License
 2.0 Description: # AutoViz: The One-Line Automatic Data Visualization Library !
 [logo](images/logo.png) Unlock the power of **AutoViz** to visualize any
 dataset, any size, with just a single line of code! Plus, now you can get a
 quick assessment of your dataset's quality and fix DQ issues through the FixDQ
 () function. [![Pepy Downloads](https://pepy.tech/badge/autoviz)](https://
```

### Comparing `autoviz-0.1.901/setup.py` & `autoviz-0.1.902/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,66 +9,70 @@
 
 list_req = [
     "xlrd",
     "wordcloud",
     "emoji",
     # Assuming numpy version <1.25.0 is compatible with older Python versions and older HoloViews
     "pyamg",
-    "matplotlib<=3.7.4",  # Specify versions compatible with older Python versions
-    "seaborn>=0.12.2",
     "scikit-learn",
     "statsmodels",
     "nltk",
     "textblob",
     "xgboost>=0.82,<1.7",
     "fsspec>=0.8.3",
     "typing-extensions>=4.1.1",
     "pandas-dq>=1.29"
 ]
 # Define default dependencies (compatible with older Python versions)
 install_requires = list_req
 
-if python_version <= (3, 10):
+if python_version < (3, 10):
     install_requires = list_req + [
     "numpy<1.24",  # older version. otherwise you get numpy bool error
     "hvplot~=0.7.3",      # Older compatible version
     "holoviews<=1.14.9",  # Older compatible version
     "panel~=0.14.4", ## this is an old versjon of panel
     "param==1.13.0", ### something broke in panel without this
     "pandas<2.0", ## pandas must be below 2.0 version
+    "matplotlib<=3.7.4", ## newer version of matplotlib
+    "seaborn<=0.12.2", ## newer version of seaborn ##
     ]
 
 # For Python versions >= 3.10 and < 3.11, update the dependency list
-if (3, 10) < python_version <= (3, 11):
+if (3, 10) <= python_version <= (3, 11):
     install_requires = list_req + [
         # Keep most dependencies as is, adjust only where necessary
         "numpy>=1.24.0",  # Update as needed for compatibility with newer HoloViews
         # Update other dependencies as needed
         "hvplot>=0.9.2", ###newer hvplot
         "holoviews>=1.16.0",  # Update based on the bug fix relevant to Python 3.10
         # Ensure other dependencies are compatible
         "panel>=1.4.0", ## this is a new version of panel
         "pandas>=2.0", ## pandas must be below 2.0 version
+        "matplotlib>3.7.4", ## newer version of matplotlib
+        "seaborn>0.12.2", ## newer version of seaborn ##
     ]
 
 # For Python versions >= 3.11, ensure HoloViews is at least 1.15.3 for the bug fix
 if python_version > (3, 11):
     install_requires = list_req + [
         # Adjust dependencies as needed for Python 3.11
         "numpy>=1.25.0",  # Update as needed for compatibility with newer HoloViews
         "hvplot>=0.9.2", ###newer hvplot
         "holoviews>=1.15.3",  # Ensure version is >= 1.15.3 for Python 3.11 support
         # Update or keep other dependencies as needed
         "panel>=1.4.0", ## this is a new version of panel
         "pandas<2.0", ## pandas must be below 2.0 version
+        "matplotlib>3.7.4", ## newer version of matplotlib
+        "seaborn>0.12.2", ## newer version of seaborn ##
     ]
 
 setuptools.setup(
     name="autoviz",
-    version="0.1.901",
+    version="0.1.902",
     author="Ram Seshadri",
     description="Automatically Visualize any dataset, any size with a single line of code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     url="https://github.com/AutoViML/AutoViz.git",
     packages=setuptools.find_packages(exclude=("tests",)),
```

