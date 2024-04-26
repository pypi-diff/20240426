# Comparing `tmp/schubertpy-0.3.14.tar.gz` & `tmp/schubertpy-0.3.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schubertpy-0.3.14.tar", last modified: Fri Apr 26 15:42:07 2024, max compression
+gzip compressed data, was "schubertpy-0.3.15.tar", last modified: Fri Apr 26 15:42:23 2024, max compression
```

## Comparing `schubertpy-0.3.14.tar` & `schubertpy-0.3.15.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-04-26 15:42:07.910905 schubertpy-0.3.14/
--rw-r--r--   0 tranduythanh   (501) staff       (20)     1073 2023-09-25 07:57:01.000000 schubertpy-0.3.14/LICENSE
--rw-r--r--   0 tranduythanh   (501) staff       (20)     6086 2024-04-26 15:42:07.910791 schubertpy-0.3.14/PKG-INFO
--rw-r--r--   0 tranduythanh   (501) staff       (20)     5511 2024-02-14 05:48:03.000000 schubertpy-0.3.14/README.md
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-04-26 15:42:07.907814 schubertpy-0.3.14/schubertpy/
--rw-r--r--   0 tranduythanh   (501) staff       (20)      377 2024-02-13 13:37:36.000000 schubertpy-0.3.14/schubertpy/__init__.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     6220 2024-04-26 02:35:10.000000 schubertpy-0.3.14/schubertpy/abstract_grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      175 2024-02-10 16:43:47.000000 schubertpy-0.3.14/schubertpy/const.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      942 2024-02-13 13:40:38.000000 schubertpy-0.3.14/schubertpy/csv_bijection.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     4806 2024-02-13 13:40:53.000000 schubertpy-0.3.14/schubertpy/grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     4714 2024-02-13 13:40:49.000000 schubertpy-0.3.14/schubertpy/isotropic_grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     5378 2024-02-13 13:41:03.000000 schubertpy-0.3.14/schubertpy/lc.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)    12445 2024-02-13 13:41:11.000000 schubertpy-0.3.14/schubertpy/orthogonal_grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     3059 2024-02-13 13:42:18.000000 schubertpy-0.3.14/schubertpy/partition.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)    40455 2024-02-13 13:42:24.000000 schubertpy-0.3.14/schubertpy/qcalc.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     3049 2024-02-13 13:41:35.000000 schubertpy-0.3.14/schubertpy/schur.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      203 2024-02-13 13:41:38.000000 schubertpy-0.3.14/schubertpy/util.py
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-04-26 15:42:07.910306 schubertpy-0.3.14/schubertpy.egg-info/
--rw-r--r--   0 tranduythanh   (501) staff       (20)     6086 2024-04-26 15:42:07.000000 schubertpy-0.3.14/schubertpy.egg-info/PKG-INFO
--rw-r--r--   0 tranduythanh   (501) staff       (20)      566 2024-04-26 15:42:07.000000 schubertpy-0.3.14/schubertpy.egg-info/SOURCES.txt
--rw-r--r--   0 tranduythanh   (501) staff       (20)        1 2024-04-26 15:42:07.000000 schubertpy-0.3.14/schubertpy.egg-info/dependency_links.txt
--rw-r--r--   0 tranduythanh   (501) staff       (20)       47 2024-04-26 15:42:07.000000 schubertpy-0.3.14/schubertpy.egg-info/requires.txt
--rw-r--r--   0 tranduythanh   (501) staff       (20)       24 2024-04-26 15:42:07.000000 schubertpy-0.3.14/schubertpy.egg-info/top_level.txt
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-04-26 15:42:07.909852 schubertpy-0.3.14/schubertsage/
--rw-r--r--   0 tranduythanh   (501) staff       (20)      304 2024-02-14 06:03:50.000000 schubertpy-0.3.14/schubertsage/__init__.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      793 2024-02-14 06:36:52.000000 schubertpy-0.3.14/schubertsage/conversion.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      132 2024-04-26 15:42:07.911472 schubertpy-0.3.14/setup.cfg
--rw-r--r--   0 tranduythanh   (501) staff       (20)      966 2024-04-26 15:42:07.000000 schubertpy-0.3.14/setup.py
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-04-26 15:42:23.023036 schubertpy-0.3.15/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     1073 2023-09-25 07:57:01.000000 schubertpy-0.3.15/LICENSE
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     6086 2024-04-26 15:42:23.022943 schubertpy-0.3.15/PKG-INFO
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     5511 2024-02-14 05:48:03.000000 schubertpy-0.3.15/README.md
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-04-26 15:42:23.020393 schubertpy-0.3.15/schubertpy/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      377 2024-02-13 13:37:36.000000 schubertpy-0.3.15/schubertpy/__init__.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     6220 2024-04-26 02:35:10.000000 schubertpy-0.3.15/schubertpy/abstract_grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      175 2024-02-10 16:43:47.000000 schubertpy-0.3.15/schubertpy/const.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      942 2024-02-13 13:40:38.000000 schubertpy-0.3.15/schubertpy/csv_bijection.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     4806 2024-02-13 13:40:53.000000 schubertpy-0.3.15/schubertpy/grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     4714 2024-02-13 13:40:49.000000 schubertpy-0.3.15/schubertpy/isotropic_grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     5378 2024-02-13 13:41:03.000000 schubertpy-0.3.15/schubertpy/lc.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)    12445 2024-02-13 13:41:11.000000 schubertpy-0.3.15/schubertpy/orthogonal_grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     3059 2024-02-13 13:42:18.000000 schubertpy-0.3.15/schubertpy/partition.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)    40455 2024-02-13 13:42:24.000000 schubertpy-0.3.15/schubertpy/qcalc.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     3049 2024-02-13 13:41:35.000000 schubertpy-0.3.15/schubertpy/schur.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      203 2024-02-13 13:41:38.000000 schubertpy-0.3.15/schubertpy/util.py
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-04-26 15:42:23.022435 schubertpy-0.3.15/schubertpy.egg-info/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     6086 2024-04-26 15:42:22.000000 schubertpy-0.3.15/schubertpy.egg-info/PKG-INFO
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      566 2024-04-26 15:42:22.000000 schubertpy-0.3.15/schubertpy.egg-info/SOURCES.txt
+-rw-r--r--   0 tranduythanh   (501) staff       (20)        1 2024-04-26 15:42:22.000000 schubertpy-0.3.15/schubertpy.egg-info/dependency_links.txt
+-rw-r--r--   0 tranduythanh   (501) staff       (20)       47 2024-04-26 15:42:22.000000 schubertpy-0.3.15/schubertpy.egg-info/requires.txt
+-rw-r--r--   0 tranduythanh   (501) staff       (20)       24 2024-04-26 15:42:22.000000 schubertpy-0.3.15/schubertpy.egg-info/top_level.txt
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-04-26 15:42:23.022063 schubertpy-0.3.15/schubertsage/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      304 2024-02-14 06:03:50.000000 schubertpy-0.3.15/schubertsage/__init__.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      793 2024-02-14 06:36:52.000000 schubertpy-0.3.15/schubertsage/conversion.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      132 2024-04-26 15:42:23.023433 schubertpy-0.3.15/setup.cfg
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      966 2024-04-26 15:42:22.000000 schubertpy-0.3.15/setup.py
```

### Comparing `schubertpy-0.3.14/LICENSE` & `schubertpy-0.3.15/LICENSE`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.14/PKG-INFO` & `schubertpy-0.3.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubertpy
-Version: 0.3.14
+Version: 0.3.15
 Summary: This Python module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, action and multiplication of Schubert classes, and conversion between different representations of Schubert classes
 Home-page: https://github.com/tranduythanh/schubertpy
 Author: Trần Duy Thanh
 Author-email: fbtranduythanh@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `schubertpy-0.3.14/README.md` & `schubertpy-0.3.15/README.md`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.14/schubertpy/abstract_grassmannian.py` & `schubertpy-0.3.15/schubertpy/abstract_grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.14/schubertpy/csv_bijection.py` & `schubertpy-0.3.15/schubertpy/csv_bijection.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.14/schubertpy/grassmannian.py` & `schubertpy-0.3.15/schubertpy/grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.14/schubertpy/isotropic_grassmannian.py` & `schubertpy-0.3.15/schubertpy/isotropic_grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.14/schubertpy/lc.py` & `schubertpy-0.3.15/schubertpy/lc.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.14/schubertpy/orthogonal_grassmannian.py` & `schubertpy-0.3.15/schubertpy/orthogonal_grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.14/schubertpy/partition.py` & `schubertpy-0.3.15/schubertpy/partition.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.14/schubertpy/qcalc.py` & `schubertpy-0.3.15/schubertpy/qcalc.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.14/schubertpy/schur.py` & `schubertpy-0.3.15/schubertpy/schur.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.14/schubertpy.egg-info/PKG-INFO` & `schubertpy-0.3.15/schubertpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubertpy
-Version: 0.3.14
+Version: 0.3.15
 Summary: This Python module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, action and multiplication of Schubert classes, and conversion between different representations of Schubert classes
 Home-page: https://github.com/tranduythanh/schubertpy
 Author: Trần Duy Thanh
 Author-email: fbtranduythanh@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `schubertpy-0.3.14/schubertpy.egg-info/SOURCES.txt` & `schubertpy-0.3.15/schubertpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.14/schubertsage/conversion.py` & `schubertpy-0.3.15/schubertsage/conversion.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.14/setup.py` & `schubertpy-0.3.15/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Read the contents of your README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='schubertpy',
-    version='0.3.14',
+    version='0.3.15',
     packages=find_packages(),
     description='This Python module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, action and multiplication of Schubert classes, and conversion between different representations of Schubert classes',
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.6',
     author='Trần Duy Thanh',
     author_email='fbtranduythanh@gmail.com',
```

