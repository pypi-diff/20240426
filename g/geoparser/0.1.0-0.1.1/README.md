# Comparing `tmp/geoparser-0.1.0.tar.gz` & `tmp/geoparser-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoparser-0.1.0.tar", last modified: Fri Apr 26 17:12:37 2024, max compression
+gzip compressed data, was "geoparser-0.1.1.tar", last modified: Fri Apr 26 18:31:39 2024, max compression
```

## Comparing `geoparser-0.1.0.tar` & `geoparser-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 17:12:37.387110 geoparser-0.1.0/
--rw-rw-rw-   0        0        0     1083 2024-04-26 12:16:15.000000 geoparser-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      455 2024-04-26 17:12:37.387110 geoparser-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       53 2024-04-26 12:16:15.000000 geoparser-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 17:12:37.371111 geoparser-0.1.0/geoparser/
--rw-rw-rw-   0        0        0       34 2024-04-26 14:04:45.000000 geoparser-0.1.0/geoparser/__init__.py
--rw-rw-rw-   0        0        0     1515 2024-04-25 16:46:41.000000 geoparser-0.1.0/geoparser/entities.py
--rw-rw-rw-   0        0        0     5647 2024-04-26 15:46:58.000000 geoparser-0.1.0/geoparser/gazetteer.py
--rw-rw-rw-   0        0        0     9241 2024-04-26 15:47:38.000000 geoparser-0.1.0/geoparser/geoparser.py
-drwxrwxrwx   0        0        0        0 2024-04-26 17:12:37.386111 geoparser-0.1.0/geoparser.egg-info/
--rw-rw-rw-   0        0        0      455 2024-04-26 17:12:37.000000 geoparser-0.1.0/geoparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-04-26 17:12:37.000000 geoparser-0.1.0/geoparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 17:12:37.000000 geoparser-0.1.0/geoparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-04-26 17:12:37.000000 geoparser-0.1.0/geoparser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-26 17:12:37.000000 geoparser-0.1.0/geoparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 17:12:37.387110 geoparser-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2413 2024-04-26 16:50:57.000000 geoparser-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:31:39.755777 geoparser-0.1.1/
+-rw-rw-rw-   0        0        0     1083 2024-04-26 18:30:53.000000 geoparser-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      455 2024-04-26 18:31:39.755777 geoparser-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2024-04-26 18:30:53.000000 geoparser-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 18:31:39.742775 geoparser-0.1.1/geoparser/
+-rw-rw-rw-   0        0        0       34 2024-04-26 18:30:53.000000 geoparser-0.1.1/geoparser/__init__.py
+-rw-rw-rw-   0        0        0     1515 2024-04-26 18:30:53.000000 geoparser-0.1.1/geoparser/entities.py
+-rw-rw-rw-   0        0        0     5647 2024-04-26 18:30:53.000000 geoparser-0.1.1/geoparser/gazetteer.py
+-rw-rw-rw-   0        0        0     9241 2024-04-26 18:30:53.000000 geoparser-0.1.1/geoparser/geoparser.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:31:39.754777 geoparser-0.1.1/geoparser.egg-info/
+-rw-rw-rw-   0        0        0      455 2024-04-26 18:31:39.000000 geoparser-0.1.1/geoparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-04-26 18:31:39.000000 geoparser-0.1.1/geoparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 18:31:39.000000 geoparser-0.1.1/geoparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-26 18:31:39.000000 geoparser-0.1.1/geoparser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-26 18:31:39.000000 geoparser-0.1.1/geoparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 18:31:39.755777 geoparser-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2413 2024-04-26 18:31:15.000000 geoparser-0.1.1/setup.py
```

### Comparing `geoparser-0.1.0/LICENSE` & `geoparser-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geoparser-0.1.0/geoparser/entities.py` & `geoparser-0.1.1/geoparser/entities.py`

 * *Files identical despite different names*

### Comparing `geoparser-0.1.0/geoparser/gazetteer.py` & `geoparser-0.1.1/geoparser/gazetteer.py`

 * *Files identical despite different names*

### Comparing `geoparser-0.1.0/geoparser/geoparser.py` & `geoparser-0.1.1/geoparser/geoparser.py`

 * *Files identical despite different names*

### Comparing `geoparser-0.1.0/setup.py` & `geoparser-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             if filename.endswith('.zip'):
                 with zipfile.ZipFile(file_path, 'r') as zip_ref:
                     zip_ref.extractall(data_dir)
                 os.remove(file_path)
 
 setup(
     name='geoparser',
-    version='0.1.0',
+    version='0.1.1',
     author='Diego Gomes',
     author_email='diego.gomes@uzh.ch',
     packages=find_packages(),
     description='A geoparsing library for English texts',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
```

