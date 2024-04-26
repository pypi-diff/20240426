# Comparing `tmp/lmn_cx_y22_operating_systems-2.1.tar.gz` & `tmp/lmn_cx_y22_operating_systems-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmn_cx_y22_operating_systems-2.1.tar", last modified: Sat Apr 20 19:09:25 2024, max compression
+gzip compressed data, was "lmn_cx_y22_operating_systems-3.0.tar", last modified: Fri Apr 26 16:44:44 2024, max compression
```

## Comparing `lmn_cx_y22_operating_systems-2.1.tar` & `lmn_cx_y22_operating_systems-3.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 19:09:25.254099 lmn_cx_y22_operating_systems-2.1/
--rw-rw-rw-   0        0        0     3383 2024-04-17 15:36:16.000000 lmn_cx_y22_operating_systems-2.1/.gitignore
--rw-rw-rw-   0        0        0     1754 2024-04-20 18:00:48.000000 lmn_cx_y22_operating_systems-2.1/COPYING
--rw-rw-rw-   0        0        0      681 2024-04-20 17:26:29.000000 lmn_cx_y22_operating_systems-2.1/LICENSE-0BSD
-drwxrwxrwx   0        0        0        0 2024-04-20 19:09:25.213978 lmn_cx_y22_operating_systems-2.1/LICENSES/
--rw-rw-rw-   0        0        0      656 2024-04-17 23:47:39.000000 lmn_cx_y22_operating_systems-2.1/LICENSES/0BSD.txt
--rw-rw-rw-   0        0        0    11558 2024-04-17 14:21:46.000000 lmn_cx_y22_operating_systems-2.1/LICENSES/Apache-2.0.txt
--rw-rw-rw-   0        0        0     7169 2024-04-17 15:09:19.000000 lmn_cx_y22_operating_systems-2.1/LICENSES/CC0-1.0.txt
--rw-rw-rw-   0        0        0     1099 2024-04-17 20:35:00.000000 lmn_cx_y22_operating_systems-2.1/LICENSES/MIT.txt
--rw-rw-rw-   0        0        0     1162 2024-04-20 19:09:25.250826 lmn_cx_y22_operating_systems-2.1/PKG-INFO
--rw-rw-rw-   0        0        0      123 2024-04-17 15:35:59.000000 lmn_cx_y22_operating_systems-2.1/README.md
--rw-rw-rw-   0        0        0     1504 2024-04-20 18:03:19.000000 lmn_cx_y22_operating_systems-2.1/REUSE
--rw-rw-rw-   0        0        0     1973 2024-04-20 18:44:09.000000 lmn_cx_y22_operating_systems-2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-20 19:09:25.254099 lmn_cx_y22_operating_systems-2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-20 19:09:25.198555 lmn_cx_y22_operating_systems-2.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-20 19:09:25.198555 lmn_cx_y22_operating_systems-2.1/src/lmn/
-drwxrwxrwx   0        0        0        0 2024-04-20 19:09:25.198555 lmn_cx_y22_operating_systems-2.1/src/lmn/cx/
-drwxrwxrwx   0        0        0        0 2024-04-20 19:09:25.198555 lmn_cx_y22_operating_systems-2.1/src/lmn/cx/y22/
-drwxrwxrwx   0        0        0        0 2024-04-20 19:09:25.247809 lmn_cx_y22_operating_systems-2.1/src/lmn/cx/y22/operating_systems/
--rw-rw-rw-   0        0        0      313 2024-04-20 17:19:34.000000 lmn_cx_y22_operating_systems-2.1/src/lmn/cx/y22/operating_systems/__init__.py
--rw-rw-rw-   0        0        0     3493 2024-04-20 19:09:04.000000 lmn_cx_y22_operating_systems-2.1/src/lmn/cx/y22/operating_systems/_operating_systems.py
-drwxrwxrwx   0        0        0        0 2024-04-20 19:09:25.250826 lmn_cx_y22_operating_systems-2.1/src/lmn.cx.y22.operating_systems.egg-info/
--rw-rw-rw-   0        0        0     1162 2024-04-20 19:09:24.000000 lmn_cx_y22_operating_systems-2.1/src/lmn.cx.y22.operating_systems.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      521 2024-04-20 19:09:25.000000 lmn_cx_y22_operating_systems-2.1/src/lmn.cx.y22.operating_systems.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 19:09:25.000000 lmn_cx_y22_operating_systems-2.1/src/lmn.cx.y22.operating_systems.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2024-04-20 19:09:25.000000 lmn_cx_y22_operating_systems-2.1/src/lmn.cx.y22.operating_systems.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-20 19:09:25.000000 lmn_cx_y22_operating_systems-2.1/src/lmn.cx.y22.operating_systems.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 16:44:44.062942 lmn_cx_y22_operating_systems-3.0/
+-rw-rw-rw-   0        0        0     3383 2024-04-17 15:36:16.000000 lmn_cx_y22_operating_systems-3.0/.gitignore
+-rw-rw-rw-   0        0        0     1754 2024-04-25 21:35:01.000000 lmn_cx_y22_operating_systems-3.0/COPYING
+-rw-rw-rw-   0        0        0      681 2024-04-25 21:35:01.000000 lmn_cx_y22_operating_systems-3.0/LICENSE-0BSD
+drwxrwxrwx   0        0        0        0 2024-04-26 16:44:44.050433 lmn_cx_y22_operating_systems-3.0/LICENSES/
+-rw-rw-rw-   0        0        0      656 2024-04-17 23:47:39.000000 lmn_cx_y22_operating_systems-3.0/LICENSES/0BSD.txt
+-rw-rw-rw-   0        0        0    11558 2024-04-17 14:21:46.000000 lmn_cx_y22_operating_systems-3.0/LICENSES/Apache-2.0.txt
+-rw-rw-rw-   0        0        0     7169 2024-04-17 15:09:19.000000 lmn_cx_y22_operating_systems-3.0/LICENSES/CC0-1.0.txt
+-rw-rw-rw-   0        0        0     1099 2024-04-17 20:35:00.000000 lmn_cx_y22_operating_systems-3.0/LICENSES/MIT.txt
+-rw-rw-rw-   0        0        0     1162 2024-04-26 16:44:44.062942 lmn_cx_y22_operating_systems-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      123 2024-04-17 15:35:59.000000 lmn_cx_y22_operating_systems-3.0/README.md
+-rw-rw-rw-   0        0        0     1504 2024-04-25 21:35:01.000000 lmn_cx_y22_operating_systems-3.0/REUSE
+-rw-rw-rw-   0        0        0     1973 2024-04-25 21:35:01.000000 lmn_cx_y22_operating_systems-3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 16:44:44.062942 lmn_cx_y22_operating_systems-3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 16:44:44.015591 lmn_cx_y22_operating_systems-3.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 16:44:44.015591 lmn_cx_y22_operating_systems-3.0/src/lmn/
+drwxrwxrwx   0        0        0        0 2024-04-26 16:44:44.015591 lmn_cx_y22_operating_systems-3.0/src/lmn/cx/
+drwxrwxrwx   0        0        0        0 2024-04-26 16:44:44.015591 lmn_cx_y22_operating_systems-3.0/src/lmn/cx/y22/
+drwxrwxrwx   0        0        0        0 2024-04-26 16:44:44.050433 lmn_cx_y22_operating_systems-3.0/src/lmn/cx/y22/operating_systems/
+-rw-rw-rw-   0        0        0      313 2024-04-20 17:19:34.000000 lmn_cx_y22_operating_systems-3.0/src/lmn/cx/y22/operating_systems/__init__.py
+-rw-rw-rw-   0        0        0     5970 2024-04-26 16:42:23.000000 lmn_cx_y22_operating_systems-3.0/src/lmn/cx/y22/operating_systems/_operating_systems.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:44:44.050433 lmn_cx_y22_operating_systems-3.0/src/lmn.cx.y22.operating_systems.egg-info/
+-rw-rw-rw-   0        0        0     1162 2024-04-26 16:44:43.000000 lmn_cx_y22_operating_systems-3.0/src/lmn.cx.y22.operating_systems.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2024-04-26 16:44:44.000000 lmn_cx_y22_operating_systems-3.0/src/lmn.cx.y22.operating_systems.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 16:44:43.000000 lmn_cx_y22_operating_systems-3.0/src/lmn.cx.y22.operating_systems.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2024-04-26 16:44:43.000000 lmn_cx_y22_operating_systems-3.0/src/lmn.cx.y22.operating_systems.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-26 16:44:43.000000 lmn_cx_y22_operating_systems-3.0/src/lmn.cx.y22.operating_systems.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 16:44:44.050433 lmn_cx_y22_operating_systems-3.0/tests/
+-rw-rw-rw-   0        0        0     1175 2024-04-25 21:44:06.000000 lmn_cx_y22_operating_systems-3.0/tests/test_main.py
```

### Comparing `lmn_cx_y22_operating_systems-2.1/.gitignore` & `lmn_cx_y22_operating_systems-3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-2.1/COPYING` & `lmn_cx_y22_operating_systems-3.0/COPYING`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-2.1/LICENSE-0BSD` & `lmn_cx_y22_operating_systems-3.0/LICENSE-0BSD`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-2.1/LICENSES/0BSD.txt` & `lmn_cx_y22_operating_systems-3.0/LICENSES/0BSD.txt`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-2.1/LICENSES/Apache-2.0.txt` & `lmn_cx_y22_operating_systems-3.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-2.1/LICENSES/CC0-1.0.txt` & `lmn_cx_y22_operating_systems-3.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-2.1/LICENSES/MIT.txt` & `lmn_cx_y22_operating_systems-3.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-2.1/PKG-INFO` & `lmn_cx_y22_operating_systems-3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmn.cx.y22.operating_systems
-Version: 2.1
+Version: 3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Zero-Clause BSD (0BSD)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `lmn_cx_y22_operating_systems-2.1/REUSE` & `lmn_cx_y22_operating_systems-3.0/REUSE`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-2.1/pyproject.toml` & `lmn_cx_y22_operating_systems-3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-2.1/src/lmn.cx.y22.operating_systems.egg-info/PKG-INFO` & `lmn_cx_y22_operating_systems-3.0/src/lmn.cx.y22.operating_systems.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmn.cx.y22.operating_systems
-Version: 2.1
+Version: 3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Zero-Clause BSD (0BSD)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `lmn_cx_y22_operating_systems-2.1/src/lmn.cx.y22.operating_systems.egg-info/SOURCES.txt` & `lmn_cx_y22_operating_systems-3.0/src/lmn.cx.y22.operating_systems.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 LICENSES/MIT.txt
 src/lmn.cx.y22.operating_systems.egg-info/PKG-INFO
 src/lmn.cx.y22.operating_systems.egg-info/SOURCES.txt
 src/lmn.cx.y22.operating_systems.egg-info/dependency_links.txt
 src/lmn.cx.y22.operating_systems.egg-info/requires.txt
 src/lmn.cx.y22.operating_systems.egg-info/top_level.txt
 src/lmn/cx/y22/operating_systems/__init__.py
-src/lmn/cx/y22/operating_systems/_operating_systems.py
+src/lmn/cx/y22/operating_systems/_operating_systems.py
+tests/test_main.py
```

