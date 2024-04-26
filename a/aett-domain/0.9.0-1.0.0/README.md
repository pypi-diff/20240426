# Comparing `tmp/aett_domain-0.9.0.tar.gz` & `tmp/aett_domain-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett_domain-0.9.0.tar", last modified: Mon Apr 22 13:59:23 2024, max compression
+gzip compressed data, was "aett_domain-1.0.0.tar", last modified: Fri Apr 26 16:18:52 2024, max compression
```

## Comparing `aett_domain-0.9.0.tar` & `aett_domain-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:23.959690 aett_domain-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-22 13:59:18.000000 aett_domain-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 13:59:18.000000 aett_domain-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-22 13:59:23.959690 aett_domain-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-22 13:59:18.000000 aett_domain-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-22 13:59:18.000000 aett_domain-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 13:59:23.959690 aett_domain-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:23.955690 aett_domain-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:23.955690 aett_domain-0.9.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:23.955690 aett_domain-0.9.0/src/aett/domain/
--rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-04-22 13:59:18.000000 aett_domain-0.9.0/src/aett/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:23.955690 aett_domain-0.9.0/src/aett_domain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-22 13:59:23.000000 aett_domain-0.9.0/src/aett_domain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-22 13:59:23.000000 aett_domain-0.9.0/src/aett_domain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:59:23.000000 aett_domain-0.9.0/src/aett_domain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 13:59:23.000000 aett_domain-0.9.0/src/aett_domain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 13:59:23.000000 aett_domain-0.9.0/src/aett_domain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:52.621385 aett_domain-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 16:18:47.000000 aett_domain-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 16:18:47.000000 aett_domain-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-26 16:18:52.621385 aett_domain-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-26 16:18:47.000000 aett_domain-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-26 16:18:47.000000 aett_domain-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:18:52.621385 aett_domain-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:52.617385 aett_domain-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:52.617385 aett_domain-1.0.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:52.617385 aett_domain-1.0.0/src/aett/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)    16637 2024-04-26 16:18:47.000000 aett_domain-1.0.0/src/aett/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:52.621385 aett_domain-1.0.0/src/aett_domain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-26 16:18:52.000000 aett_domain-1.0.0/src/aett_domain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-26 16:18:52.000000 aett_domain-1.0.0/src/aett_domain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:18:52.000000 aett_domain-1.0.0/src/aett_domain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 16:18:52.000000 aett_domain-1.0.0/src/aett_domain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 16:18:52.000000 aett_domain-1.0.0/src/aett_domain.egg-info/top_level.txt
```

### Comparing `aett_domain-0.9.0/LICENSE` & `aett_domain-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett_domain-0.9.0/PKG-INFO` & `aett_domain-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-domain
-Version: 0.9.0
+Version: 1.0.0
 Summary: Domain modeling types aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: multipledispatch>=1.0.0
-Requires-Dist: aett-eventstore>=0.9.0
+Requires-Dist: aett-eventstore>=1.0.0
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

### Comparing `aett_domain-0.9.0/README.md` & `aett_domain-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `aett_domain-0.9.0/pyproject.toml` & `aett_domain-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-# pyproject.toml
-
 [build-system]
-requires = ["setuptools>=69.1.1", "wheel"]
+requires = ["setuptools>=69.5.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.domain"]
 
 [project]
 name = "aett-domain"
-version = "0.9.0"
+version = "1.0.0"
 description = "Domain modeling types aett event store"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["events", "event store", "ddd", "domain"]
 dependencies = [
     'multipledispatch >= 1.0.0',
-    'aett-eventstore>=0.9.0'
+    'aett-eventstore>=1.0.0'
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "behave"]
 
 [project.urls]
```

### Comparing `aett_domain-0.9.0/src/aett_domain.egg-info/PKG-INFO` & `aett_domain-1.0.0/src/aett_domain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-domain
-Version: 0.9.0
+Version: 1.0.0
 Summary: Domain modeling types aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: multipledispatch>=1.0.0
-Requires-Dist: aett-eventstore>=0.9.0
+Requires-Dist: aett-eventstore>=1.0.0
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

