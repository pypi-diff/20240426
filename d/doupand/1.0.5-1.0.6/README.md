# Comparing `tmp/doupand-1.0.5.tar.gz` & `tmp/doupand-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doupand-1.0.5.tar", last modified: Thu Mar 28 11:58:21 2024, max compression
+gzip compressed data, was "doupand-1.0.6.tar", last modified: Fri Apr 26 14:38:16 2024, max compression
```

## Comparing `doupand-1.0.5.tar` & `doupand-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-03-28 11:58:21.029268 doupand-1.0.5/
--rw-r--r--   0 tongjun    (501) staff       (20)     1469 2023-04-07 19:08:40.000000 doupand-1.0.5/LICENSE
--rw-r--r--   0 tongjun    (501) staff       (20)     2039 2024-03-28 11:58:21.029121 doupand-1.0.5/PKG-INFO
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-03-28 11:58:21.025648 doupand-1.0.5/doupand/
--rw-r--r--   0 tongjun    (501) staff       (20)      133 2023-04-08 17:33:37.000000 doupand-1.0.5/doupand/__init__.py
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-03-28 11:58:21.027120 doupand-1.0.5/doupand/api/
--rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-06 17:31:40.000000 doupand-1.0.5/doupand/api/__init__.py
--rw-r--r--   0 tongjun    (501) staff       (20)     3291 2024-03-27 17:35:36.000000 doupand-1.0.5/doupand/api/client.py
--rw-r--r--   0 tongjun    (501) staff       (20)       54 2024-03-27 17:31:05.000000 doupand-1.0.5/doupand/api/dp_url.csv
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-03-28 11:58:21.028782 doupand-1.0.5/doupand/utils/
--rw-r--r--   0 tongjun    (501) staff       (20)        0 2023-04-06 17:18:45.000000 doupand-1.0.5/doupand/utils/__init__.py
--rw-r--r--   0 tongjun    (501) staff       (20)      277 2023-04-08 17:11:54.000000 doupand-1.0.5/doupand/utils/cons.py
--rw-r--r--   0 tongjun    (501) staff       (20)       71 2024-03-27 17:35:19.000000 doupand-1.0.5/doupand/utils/dp_tk.csv
--rw-r--r--   0 tongjun    (501) staff       (20)      701 2023-04-07 14:51:56.000000 doupand-1.0.5/doupand/utils/userauth.py
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-03-28 11:58:21.026445 doupand-1.0.5/doupand.egg-info/
--rw-r--r--   0 tongjun    (501) staff       (20)     2039 2024-03-28 11:58:20.000000 doupand-1.0.5/doupand.egg-info/PKG-INFO
--rw-r--r--   0 tongjun    (501) staff       (20)      357 2024-03-28 11:58:20.000000 doupand-1.0.5/doupand.egg-info/SOURCES.txt
--rw-r--r--   0 tongjun    (501) staff       (20)        1 2024-03-28 11:58:20.000000 doupand-1.0.5/doupand.egg-info/dependency_links.txt
--rw-r--r--   0 tongjun    (501) staff       (20)       16 2024-03-28 11:58:20.000000 doupand-1.0.5/doupand.egg-info/requires.txt
--rw-r--r--   0 tongjun    (501) staff       (20)        8 2024-03-28 11:58:20.000000 doupand-1.0.5/doupand.egg-info/top_level.txt
--rw-r--r--   0 tongjun    (501) staff       (20)       38 2024-03-28 11:58:21.029315 doupand-1.0.5/setup.cfg
--rw-r--r--   0 tongjun    (501) staff       (20)     2400 2024-03-28 11:56:59.000000 doupand-1.0.5/setup.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-04-26 14:38:16.392271 doupand-1.0.6/
+-rw-r--r--   0 tongjun    (501) staff       (20)     1469 2023-04-07 19:08:40.000000 doupand-1.0.6/LICENSE
+-rw-r--r--   0 tongjun    (501) staff       (20)     2039 2024-04-26 14:38:16.391994 doupand-1.0.6/PKG-INFO
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-04-26 14:38:16.389386 doupand-1.0.6/doupand/
+-rw-r--r--   0 tongjun    (501) staff       (20)      133 2024-04-26 14:38:05.000000 doupand-1.0.6/doupand/__init__.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-04-26 14:38:16.390626 doupand-1.0.6/doupand/api/
+-rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-06 17:31:40.000000 doupand-1.0.6/doupand/api/__init__.py
+-rw-r--r--   0 tongjun    (501) staff       (20)     3291 2024-03-27 17:35:36.000000 doupand-1.0.6/doupand/api/client.py
+-rw-r--r--   0 tongjun    (501) staff       (20)       54 2024-03-27 17:31:05.000000 doupand-1.0.6/doupand/api/dp_url.csv
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-04-26 14:38:16.391675 doupand-1.0.6/doupand/utils/
+-rw-r--r--   0 tongjun    (501) staff       (20)        0 2023-04-06 17:18:45.000000 doupand-1.0.6/doupand/utils/__init__.py
+-rw-r--r--   0 tongjun    (501) staff       (20)      277 2023-04-08 17:11:54.000000 doupand-1.0.6/doupand/utils/cons.py
+-rw-r--r--   0 tongjun    (501) staff       (20)       71 2024-03-27 17:35:19.000000 doupand-1.0.6/doupand/utils/dp_tk.csv
+-rw-r--r--   0 tongjun    (501) staff       (20)      701 2023-04-07 14:51:56.000000 doupand-1.0.6/doupand/utils/userauth.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-04-26 14:38:16.389991 doupand-1.0.6/doupand.egg-info/
+-rw-r--r--   0 tongjun    (501) staff       (20)     2039 2024-04-26 14:38:16.000000 doupand-1.0.6/doupand.egg-info/PKG-INFO
+-rw-r--r--   0 tongjun    (501) staff       (20)      357 2024-04-26 14:38:16.000000 doupand-1.0.6/doupand.egg-info/SOURCES.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)        1 2024-04-26 14:38:16.000000 doupand-1.0.6/doupand.egg-info/dependency_links.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)       16 2024-04-26 14:38:16.000000 doupand-1.0.6/doupand.egg-info/requires.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)        8 2024-04-26 14:38:16.000000 doupand-1.0.6/doupand.egg-info/top_level.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)       38 2024-04-26 14:38:16.392316 doupand-1.0.6/setup.cfg
+-rw-r--r--   0 tongjun    (501) staff       (20)     2400 2024-04-26 14:38:05.000000 doupand-1.0.6/setup.py
```

### Comparing `doupand-1.0.5/LICENSE` & `doupand-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `doupand-1.0.5/PKG-INFO` & `doupand-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doupand
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple and easy-to-use financial data interface library built for normal investors!
 Home-page: https://doupand.com
 Author: DouBro
 Author-email: doupand@163.com
 License: BSD
 Keywords: Financial Data Interface
 Platform: all
```

### Comparing `doupand-1.0.5/doupand/api/client.py` & `doupand-1.0.6/doupand/api/client.py`

 * *Files identical despite different names*

### Comparing `doupand-1.0.5/doupand/utils/userauth.py` & `doupand-1.0.6/doupand/utils/userauth.py`

 * *Files identical despite different names*

### Comparing `doupand-1.0.5/doupand.egg-info/PKG-INFO` & `doupand-1.0.6/doupand.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doupand
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple and easy-to-use financial data interface library built for normal investors!
 Home-page: https://doupand.com
 Author: DouBro
 Author-email: doupand@163.com
 License: BSD
 Keywords: Financial Data Interface
 Platform: all
```

### Comparing `doupand-1.0.5/setup.py` & `doupand-1.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     5331  873305.BJ  873305  ...          BSE         北交所
     5332  873339.BJ  873339  ...          BSE         北交所
     5333  873527.BJ  873527  ...          BSE         北交所
 """
 
 setup(
     name='doupand',
-    version="1.0.5",
+    version="1.0.6",
     description='A simple and easy-to-use financial data interface library built for normal investors!',
     long_description=long_desc,
     author='DouBro',
     author_email='doupand@163.com',
     packages=find_packages(),
     platforms=["all"],
     license='BSD',
```

