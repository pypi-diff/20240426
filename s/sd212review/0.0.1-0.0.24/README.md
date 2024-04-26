# Comparing `tmp/sd212review-0.0.1.tar.gz` & `tmp/sd212review-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd212review-0.0.1.tar", last modified: Fri Apr 28 08:58:29 2023, max compression
+gzip compressed data, was "sd212review-0.0.24.tar", last modified: Fri Apr 26 13:27:05 2024, max compression
```

## Comparing `sd212review-0.0.1.tar` & `sd212review-0.0.24.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 roche    (32893) scs      (10120)        0 2023-04-28 08:58:29.760342 sd212review-0.0.1/
--rw-------   0 roche    (32893) scs      (10120)     1066 2023-04-28 08:21:49.000000 sd212review-0.0.1/LICENSE
--rw-------   0 roche    (32893) scs      (10120)     1137 2023-04-28 08:58:29.760342 sd212review-0.0.1/PKG-INFO
--rw-------   0 roche    (32893) scs      (10120)      801 2023-04-28 08:58:12.000000 sd212review-0.0.1/README.md
--rw-------   0 roche    (32893) scs      (10120)      431 2023-04-28 08:51:20.000000 sd212review-0.0.1/pyproject.toml
-drwx------   0 roche    (32893) scs      (10120)        0 2023-04-28 08:58:29.760342 sd212review-0.0.1/sd212review/
--rw-------   0 roche    (32893) scs      (10120)       33 2023-04-28 08:32:48.000000 sd212review-0.0.1/sd212review/__init__.py
--rw-------   0 roche    (32893) scs      (10120)      247 2023-04-28 08:35:33.000000 sd212review-0.0.1/sd212review/whichunit.py
-drwx------   0 roche    (32893) scs      (10120)        0 2023-04-28 08:58:29.760342 sd212review-0.0.1/sd212review.egg-info/
--rw-------   0 roche    (32893) scs      (10120)     1137 2023-04-28 08:58:29.000000 sd212review-0.0.1/sd212review.egg-info/PKG-INFO
--rw-------   0 roche    (32893) scs      (10120)      221 2023-04-28 08:58:29.000000 sd212review-0.0.1/sd212review.egg-info/SOURCES.txt
--rw-------   0 roche    (32893) scs      (10120)        1 2023-04-28 08:58:29.000000 sd212review-0.0.1/sd212review.egg-info/dependency_links.txt
--rw-------   0 roche    (32893) scs      (10120)       12 2023-04-28 08:58:29.000000 sd212review-0.0.1/sd212review.egg-info/top_level.txt
--rw-------   0 roche    (32893) scs      (10120)       38 2023-04-28 08:58:29.760342 sd212review-0.0.1/setup.cfg
+drwx------   0 roche    (32893) scs      (10120)        0 2024-04-26 13:27:05.411184 sd212review-0.0.24/
+-rw-------   0 roche    (32893) scs      (10120)     1066 2024-04-26 13:16:54.000000 sd212review-0.0.24/LICENSE
+-rw-r--r--   0 roche    (32893) scs      (10120)     1139 2024-04-26 13:27:05.411184 sd212review-0.0.24/PKG-INFO
+-rw-------   0 roche    (32893) scs      (10120)      802 2024-04-26 13:25:33.000000 sd212review-0.0.24/README.md
+-rw-------   0 roche    (32893) scs      (10120)      432 2024-04-26 13:25:33.000000 sd212review-0.0.24/pyproject.toml
+drwx------   0 roche    (32893) scs      (10120)        0 2024-04-26 13:27:05.411184 sd212review-0.0.24/sd212review/
+-rw-------   0 roche    (32893) scs      (10120)       33 2024-04-26 13:16:54.000000 sd212review-0.0.24/sd212review/__init__.py
+-rw-------   0 roche    (32893) scs      (10120)      316 2024-04-26 13:25:33.000000 sd212review-0.0.24/sd212review/whichunit.py
+drwx------   0 roche    (32893) scs      (10120)        0 2024-04-26 13:27:05.411184 sd212review-0.0.24/sd212review.egg-info/
+-rw-r--r--   0 roche    (32893) scs      (10120)     1139 2024-04-26 13:27:05.000000 sd212review-0.0.24/sd212review.egg-info/PKG-INFO
+-rw-------   0 roche    (32893) scs      (10120)      221 2024-04-26 13:27:05.000000 sd212review-0.0.24/sd212review.egg-info/SOURCES.txt
+-rw-------   0 roche    (32893) scs      (10120)        1 2024-04-26 13:27:05.000000 sd212review-0.0.24/sd212review.egg-info/dependency_links.txt
+-rw-------   0 roche    (32893) scs      (10120)       12 2024-04-26 13:27:05.000000 sd212review-0.0.24/sd212review.egg-info/top_level.txt
+-rw-------   0 roche    (32893) scs      (10120)       38 2024-04-26 13:27:05.411184 sd212review-0.0.24/setup.cfg
```

### Comparing `sd212review-0.0.1/LICENSE` & `sd212review-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `sd212review-0.0.1/PKG-INFO` & `sd212review-0.0.24/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd212review
-Version: 0.0.1
+Version: 0.0.24
 Summary: Simple Python module to tell you which unit to write review questions for SD212
 Author-email: Dan Roche <roche@usna.edu>
 Project-URL: Homepage, https://github.com/sd212usna/sd212review
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -12,18 +12,18 @@
 Simple Python module to tell you which unit to write review questions for SD212
 
 # Usage
 
     from sd212review import whichunit
 
     # you can call it with a number
-    whichunit(257863) # returns 2
+    whichunit(261234) # returns 11
 
     # or you can call it with a string
-    whichunit('m264351') # returns 3
+    whichunit('m264321') # returns 2
 
 # Build instructions
 
 Follow [this tutorial on packaging](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 and [this quickstart for setuptools](https://setuptools.pypa.io/en/latest/userguide/quickstart.html).
 
 Pip/conda/mamba packages needed:
```

### Comparing `sd212review-0.0.1/README.md` & `sd212review-0.0.24/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Simple Python module to tell you which unit to write review questions for SD212
 
 # Usage
 
     from sd212review import whichunit
 
     # you can call it with a number
-    whichunit(257863) # returns 2
+    whichunit(261234) # returns 11
 
     # or you can call it with a string
-    whichunit('m264351') # returns 3
+    whichunit('m264321') # returns 2
 
 # Build instructions
 
 Follow [this tutorial on packaging](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 and [this quickstart for setuptools](https://setuptools.pypa.io/en/latest/userguide/quickstart.html).
 
 Pip/conda/mamba packages needed:
```

### Comparing `sd212review-0.0.1/sd212review.egg-info/PKG-INFO` & `sd212review-0.0.24/sd212review.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd212review
-Version: 0.0.1
+Version: 0.0.24
 Summary: Simple Python module to tell you which unit to write review questions for SD212
 Author-email: Dan Roche <roche@usna.edu>
 Project-URL: Homepage, https://github.com/sd212usna/sd212review
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -12,18 +12,18 @@
 Simple Python module to tell you which unit to write review questions for SD212
 
 # Usage
 
     from sd212review import whichunit
 
     # you can call it with a number
-    whichunit(257863) # returns 2
+    whichunit(261234) # returns 11
 
     # or you can call it with a string
-    whichunit('m264351') # returns 3
+    whichunit('m264321') # returns 2
 
 # Build instructions
 
 Follow [this tutorial on packaging](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 and [this quickstart for setuptools](https://setuptools.pypa.io/en/latest/userguide/quickstart.html).
 
 Pip/conda/mamba packages needed:
```

