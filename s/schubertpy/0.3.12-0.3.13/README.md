# Comparing `tmp/schubertpy-0.3.12.tar.gz` & `tmp/schubertpy-0.3.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schubertpy-0.3.12.tar", last modified: Tue Feb 13 16:37:58 2024, max compression
+gzip compressed data, was "schubertpy-0.3.13.tar", last modified: Fri Apr 26 15:40:53 2024, max compression
```

## Comparing `schubertpy-0.3.12.tar` & `schubertpy-0.3.13.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-02-13 16:37:58.751981 schubertpy-0.3.12/
--rw-r--r--   0 tranduythanh   (501) staff       (20)     1073 2023-09-25 07:57:01.000000 schubertpy-0.3.12/LICENSE
--rw-r--r--   0 tranduythanh   (501) staff       (20)     4828 2024-02-13 16:37:58.751920 schubertpy-0.3.12/PKG-INFO
--rw-r--r--   0 tranduythanh   (501) staff       (20)     4253 2024-02-13 16:08:31.000000 schubertpy-0.3.12/README.md
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-02-13 16:37:58.750893 schubertpy-0.3.12/schubertpy/
--rw-r--r--   0 tranduythanh   (501) staff       (20)      377 2024-02-13 13:37:36.000000 schubertpy-0.3.12/schubertpy/__init__.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     6220 2024-02-13 13:40:26.000000 schubertpy-0.3.12/schubertpy/abstract_grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      175 2024-02-10 16:43:47.000000 schubertpy-0.3.12/schubertpy/const.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      942 2024-02-13 13:40:38.000000 schubertpy-0.3.12/schubertpy/csv_bijection.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     4806 2024-02-13 13:40:53.000000 schubertpy-0.3.12/schubertpy/grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     4714 2024-02-13 13:40:49.000000 schubertpy-0.3.12/schubertpy/isotropic_grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     5378 2024-02-13 13:41:03.000000 schubertpy-0.3.12/schubertpy/lc.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)    12445 2024-02-13 13:41:11.000000 schubertpy-0.3.12/schubertpy/orthogonal_grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     3059 2024-02-13 13:42:18.000000 schubertpy-0.3.12/schubertpy/partition.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)    40455 2024-02-13 13:42:24.000000 schubertpy-0.3.12/schubertpy/qcalc.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     3049 2024-02-13 13:41:35.000000 schubertpy-0.3.12/schubertpy/schur.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      203 2024-02-13 13:41:38.000000 schubertpy-0.3.12/schubertpy/util.py
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-02-13 16:37:58.751691 schubertpy-0.3.12/schubertpy.egg-info/
--rw-r--r--   0 tranduythanh   (501) staff       (20)     4828 2024-02-13 16:37:58.000000 schubertpy-0.3.12/schubertpy.egg-info/PKG-INFO
--rw-r--r--   0 tranduythanh   (501) staff       (20)      514 2024-02-13 16:37:58.000000 schubertpy-0.3.12/schubertpy.egg-info/SOURCES.txt
--rw-r--r--   0 tranduythanh   (501) staff       (20)        1 2024-02-13 16:37:58.000000 schubertpy-0.3.12/schubertpy.egg-info/dependency_links.txt
--rw-r--r--   0 tranduythanh   (501) staff       (20)       47 2024-02-13 16:37:58.000000 schubertpy-0.3.12/schubertpy.egg-info/requires.txt
--rw-r--r--   0 tranduythanh   (501) staff       (20)       11 2024-02-13 16:37:58.000000 schubertpy-0.3.12/schubertpy.egg-info/top_level.txt
--rw-r--r--   0 tranduythanh   (501) staff       (20)      132 2024-02-13 16:37:58.752408 schubertpy-0.3.12/setup.cfg
--rw-r--r--   0 tranduythanh   (501) staff       (20)      966 2024-02-13 16:37:57.000000 schubertpy-0.3.12/setup.py
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-04-26 15:40:53.017373 schubertpy-0.3.13/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     1073 2023-09-25 07:57:01.000000 schubertpy-0.3.13/LICENSE
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     6113 2024-04-26 15:40:53.017244 schubertpy-0.3.13/PKG-INFO
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     5511 2024-02-14 05:48:03.000000 schubertpy-0.3.13/README.md
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-04-26 15:40:53.015066 schubertpy-0.3.13/schubertpy/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      377 2024-02-13 13:37:36.000000 schubertpy-0.3.13/schubertpy/__init__.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     6220 2024-04-26 02:35:10.000000 schubertpy-0.3.13/schubertpy/abstract_grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      175 2024-02-10 16:43:47.000000 schubertpy-0.3.13/schubertpy/const.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      942 2024-02-13 13:40:38.000000 schubertpy-0.3.13/schubertpy/csv_bijection.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     4806 2024-02-13 13:40:53.000000 schubertpy-0.3.13/schubertpy/grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     4714 2024-02-13 13:40:49.000000 schubertpy-0.3.13/schubertpy/isotropic_grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     5378 2024-02-13 13:41:03.000000 schubertpy-0.3.13/schubertpy/lc.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)    12445 2024-02-13 13:41:11.000000 schubertpy-0.3.13/schubertpy/orthogonal_grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     3059 2024-02-13 13:42:18.000000 schubertpy-0.3.13/schubertpy/partition.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)    40455 2024-02-13 13:42:24.000000 schubertpy-0.3.13/schubertpy/qcalc.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     3049 2024-02-13 13:41:35.000000 schubertpy-0.3.13/schubertpy/schur.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      203 2024-02-13 13:41:38.000000 schubertpy-0.3.13/schubertpy/util.py
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-04-26 15:40:53.016747 schubertpy-0.3.13/schubertpy.egg-info/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     6113 2024-04-26 15:40:52.000000 schubertpy-0.3.13/schubertpy.egg-info/PKG-INFO
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      566 2024-04-26 15:40:52.000000 schubertpy-0.3.13/schubertpy.egg-info/SOURCES.txt
+-rw-r--r--   0 tranduythanh   (501) staff       (20)        1 2024-04-26 15:40:52.000000 schubertpy-0.3.13/schubertpy.egg-info/dependency_links.txt
+-rw-r--r--   0 tranduythanh   (501) staff       (20)       59 2024-04-26 15:40:52.000000 schubertpy-0.3.13/schubertpy.egg-info/requires.txt
+-rw-r--r--   0 tranduythanh   (501) staff       (20)       24 2024-04-26 15:40:52.000000 schubertpy-0.3.13/schubertpy.egg-info/top_level.txt
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-04-26 15:40:53.016522 schubertpy-0.3.13/schubertsage/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      304 2024-02-14 06:03:50.000000 schubertpy-0.3.13/schubertsage/__init__.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      793 2024-02-14 06:36:52.000000 schubertpy-0.3.13/schubertsage/conversion.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      132 2024-04-26 15:40:53.017824 schubertpy-0.3.13/setup.cfg
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      966 2024-04-26 15:40:50.000000 schubertpy-0.3.13/setup.py
```

### Comparing `schubertpy-0.3.12/LICENSE` & `schubertpy-0.3.13/LICENSE`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.12/schubertpy/abstract_grassmannian.py` & `schubertpy-0.3.13/schubertpy/abstract_grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.12/schubertpy/csv_bijection.py` & `schubertpy-0.3.13/schubertpy/csv_bijection.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.12/schubertpy/grassmannian.py` & `schubertpy-0.3.13/schubertpy/grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.12/schubertpy/isotropic_grassmannian.py` & `schubertpy-0.3.13/schubertpy/isotropic_grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.12/schubertpy/lc.py` & `schubertpy-0.3.13/schubertpy/lc.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.12/schubertpy/orthogonal_grassmannian.py` & `schubertpy-0.3.13/schubertpy/orthogonal_grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.12/schubertpy/partition.py` & `schubertpy-0.3.13/schubertpy/partition.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.12/schubertpy/qcalc.py` & `schubertpy-0.3.13/schubertpy/qcalc.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.12/schubertpy/schur.py` & `schubertpy-0.3.13/schubertpy/schur.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.12/schubertpy.egg-info/SOURCES.txt` & `schubertpy-0.3.13/schubertpy.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -14,8 +14,10 @@
 schubertpy/qcalc.py
 schubertpy/schur.py
 schubertpy/util.py
 schubertpy.egg-info/PKG-INFO
 schubertpy.egg-info/SOURCES.txt
 schubertpy.egg-info/dependency_links.txt
 schubertpy.egg-info/requires.txt
-schubertpy.egg-info/top_level.txt
+schubertpy.egg-info/top_level.txt
+schubertsage/__init__.py
+schubertsage/conversion.py
```

### Comparing `schubertpy-0.3.12/setup.py` & `schubertpy-0.3.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Read the contents of your README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='schubertpy',
-    version='0.3.12',
+    version='0.3.13',
     packages=find_packages(),
     description='This Python module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, action and multiplication of Schubert classes, and conversion between different representations of Schubert classes',
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.6',
     author='Trần Duy Thanh',
     author_email='fbtranduythanh@gmail.com',
```

