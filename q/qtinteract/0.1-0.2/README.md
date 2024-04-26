# Comparing `tmp/qtinteract-0.1.tar.gz` & `tmp/qtinteract-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtinteract-0.1.tar", last modified: Tue Jan 30 13:23:40 2024, max compression
+gzip compressed data, was "qtinteract-0.2.tar", last modified: Fri Apr 26 09:27:45 2024, max compression
```

## Comparing `qtinteract-0.1.tar` & `qtinteract-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-01-30 13:23:39.988884 qtinteract-0.1/
--rw-rw-rw-   0        0        0     1136 2024-01-30 13:23:39.985876 qtinteract-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      339 2024-01-30 12:43:23.000000 qtinteract-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-01-30 13:23:39.979868 qtinteract-0.1/qtinteract.egg-info/
--rw-rw-rw-   0        0        0     1136 2024-01-30 13:23:38.000000 qtinteract-0.1/qtinteract.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-01-30 13:23:39.000000 qtinteract-0.1/qtinteract.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-30 13:23:38.000000 qtinteract-0.1/qtinteract.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-01-30 12:44:54.000000 qtinteract-0.1/qtinteract.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2024-01-30 13:23:38.000000 qtinteract-0.1/qtinteract.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-01-30 13:23:38.000000 qtinteract-0.1/qtinteract.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8425 2024-01-29 10:40:46.000000 qtinteract-0.1/qtinteract.py
--rw-rw-rw-   0        0        0       42 2024-01-30 13:23:39.989873 qtinteract-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1128 2024-01-30 12:47:15.000000 qtinteract-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:27:45.753246 qtinteract-0.2/
+-rw-rw-rw-   0        0        0     1440 2024-04-26 09:27:45.752249 qtinteract-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      634 2024-02-14 03:31:44.000000 qtinteract-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 09:27:45.750276 qtinteract-0.2/qtinteract.egg-info/
+-rw-rw-rw-   0        0        0     1440 2024-04-26 09:27:45.000000 qtinteract-0.2/qtinteract.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-26 09:27:45.000000 qtinteract-0.2/qtinteract.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 09:27:45.000000 qtinteract-0.2/qtinteract.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-01-30 12:44:54.000000 qtinteract-0.2/qtinteract.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2024-04-26 09:27:45.000000 qtinteract-0.2/qtinteract.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-26 09:27:45.000000 qtinteract-0.2/qtinteract.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    21980 2024-04-26 09:27:15.000000 qtinteract-0.2/qtinteract.py
+-rw-rw-rw-   0        0        0       42 2024-04-26 09:27:45.754250 qtinteract-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1128 2024-04-26 09:26:56.000000 qtinteract-0.2/setup.py
```

### Comparing `qtinteract-0.1/PKG-INFO` & `qtinteract-0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtinteract
-Version: 0.1
+Version: 0.2
 Summary: Fast interactive plots in Jupyter Notebooks using Qt Widgets
 Home-page: https://github.com/axil/qtinteract
 Author: Lev Maximov
 Author-email: lev.maximov@gmail.com
 License: MIT License
 Keywords: interactive,visualization,qt,widgets,slider
 Classifier: Development Status :: 4 - Beta
@@ -24,18 +24,27 @@
 
 ## Installation
 
     pip install qtinteract
 
 ## Usage
 
+```python
     %gui qt5    
 
     from math import pi
     from qtinteract import iplot
 
     def f(x, a):
         return np.sin(a*x)
 
     x = np.linspace(0, 2*pi, 101)
 
     iplot(x, f, a=(1., 5.))
+```
+![image](https://github.com/axil/qtinteract/assets/170910/c36fe65e-f0bd-49f5-a6f5-44abdb09a037)
+
+## Troubleshooting
+
+* "Kernel died": you forgot to run `%gui qt5`.
+
+* The window with the plot and the slider does not appear. Look at the taskbar, it might appear behind the browser.
```

### Comparing `qtinteract-0.1/qtinteract.egg-info/PKG-INFO` & `qtinteract-0.2/qtinteract.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtinteract
-Version: 0.1
+Version: 0.2
 Summary: Fast interactive plots in Jupyter Notebooks using Qt Widgets
 Home-page: https://github.com/axil/qtinteract
 Author: Lev Maximov
 Author-email: lev.maximov@gmail.com
 License: MIT License
 Keywords: interactive,visualization,qt,widgets,slider
 Classifier: Development Status :: 4 - Beta
@@ -24,18 +24,27 @@
 
 ## Installation
 
     pip install qtinteract
 
 ## Usage
 
+```python
     %gui qt5    
 
     from math import pi
     from qtinteract import iplot
 
     def f(x, a):
         return np.sin(a*x)
 
     x = np.linspace(0, 2*pi, 101)
 
     iplot(x, f, a=(1., 5.))
+```
+![image](https://github.com/axil/qtinteract/assets/170910/c36fe65e-f0bd-49f5-a6f5-44abdb09a037)
+
+## Troubleshooting
+
+* "Kernel died": you forgot to run `%gui qt5`.
+
+* The window with the plot and the slider does not appear. Look at the taskbar, it might appear behind the browser.
```

### Comparing `qtinteract-0.1/setup.py` & `qtinteract-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='qtinteract',
-    version='0.1',
+    version='0.2',
     author='Lev Maximov',
     author_email='lev.maximov@gmail.com',
     url='https://github.com/axil/qtinteract',
     description='Fast interactive plots in Jupyter Notebooks using Qt Widgets',
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires=">=3.7",
```

