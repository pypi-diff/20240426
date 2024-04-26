# Comparing `tmp/setga-1.4.2.tar.gz` & `tmp/setga-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setga-1.4.2.tar", last modified: Fri Apr 26 12:50:33 2024, max compression
+gzip compressed data, was "setga-1.4.3.tar", last modified: Fri Apr 26 12:57:37 2024, max compression
```

## Comparing `setga-1.4.2.tar` & `setga-1.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:50:33.691693 setga-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 12:50:30.000000 setga-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-26 12:50:33.691693 setga-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-26 12:50:30.000000 setga-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:50:33.691693 setga-1.4.2/setga/
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-04-26 12:50:30.000000 setga-1.4.2/setga/select_subset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-04-26 12:50:30.000000 setga-1.4.2/setga/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:50:33.691693 setga-1.4.2/setga.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-26 12:50:33.000000 setga-1.4.2/setga.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-26 12:50:33.000000 setga-1.4.2/setga.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 12:50:33.000000 setga-1.4.2/setga.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 12:50:33.000000 setga-1.4.2/setga.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 12:50:33.000000 setga-1.4.2/setga.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-26 12:50:33.691693 setga-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-26 12:50:32.000000 setga-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:57:37.002044 setga-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 12:57:30.000000 setga-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-26 12:57:37.002044 setga-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-26 12:57:30.000000 setga-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:57:36.998044 setga-1.4.3/setga/
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-04-26 12:57:30.000000 setga-1.4.3/setga/select_subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-04-26 12:57:30.000000 setga-1.4.3/setga/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:57:37.002044 setga-1.4.3/setga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-26 12:57:36.000000 setga-1.4.3/setga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-26 12:57:36.000000 setga-1.4.3/setga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 12:57:36.000000 setga-1.4.3/setga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 12:57:36.000000 setga-1.4.3/setga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 12:57:36.000000 setga-1.4.3/setga.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-26 12:57:37.002044 setga-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-26 12:57:34.000000 setga-1.4.3/setup.py
```

### Comparing `setga-1.4.2/LICENSE` & `setga-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `setga-1.4.2/PKG-INFO` & `setga-1.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setga
-Version: 1.4.2
+Version: 1.4.3
 Summary: library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.
 Home-page: https://github.com/lavakin/setga
 Author: Nikola Kalábová
 Author-email: nikola@kalabova.eu
 License: MIT
 Project-URL: Documentation, https://setga.readthedocs.io/en/latest/genindex.html
 Keywords: Genetic algorithms,minimal subset,multi-objective,optimization
```

### Comparing `setga-1.4.2/README.md` & `setga-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `setga-1.4.2/setga/select_subset.py` & `setga-1.4.3/setga/select_subset.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         raise WrongType("Unknown type of crossover")
 
     if selection == "SPEA2":
         toolbox.register("select", tools.selSPEA2)
     if selection == "NSGA2":
         toolbox.register("select", tools.selNSGA2)
     if selection == "NSGA3":
-        if ref_points == None:
+        if ref_points is None:
             raise WrongType("Ref_points cannot be None")
         toolbox.register("select", tools.selNSGA2,ref_points = ref_points)
     if selection not in ["SPEA2","NSGA2"]:
         raise WrongType("Unknown type of mating")
     
     toolbox.register("migrate",tools.migRing,k=10,selection = toolbox.select)
```

### Comparing `setga-1.4.2/setga/utils.py` & `setga-1.4.3/setga/utils.py`

 * *Files identical despite different names*

### Comparing `setga-1.4.2/setga.egg-info/PKG-INFO` & `setga-1.4.3/setga.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setga
-Version: 1.4.2
+Version: 1.4.3
 Summary: library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.
 Home-page: https://github.com/lavakin/setga
 Author: Nikola Kalábová
 Author-email: nikola@kalabova.eu
 License: MIT
 Project-URL: Documentation, https://setga.readthedocs.io/en/latest/genindex.html
 Keywords: Genetic algorithms,minimal subset,multi-objective,optimization
```

### Comparing `setga-1.4.2/setup.py` & `setga-1.4.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   name = 'setga',         
   packages = ['setga'], 
   license='MIT',       
   description = 'library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.',   # Give a short description about your library
   author = 'Nikola Kalábová',              
   author_email = 'nikola@kalabova.eu',     
   url = 'https://github.com/lavakin/setga',  
-  version = "1.4.2",    
+  version = "1.4.3",    
   keywords = ['Genetic algorithms', 'minimal subset', 'multi-objective', "optimization"],   
   long_description = "library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.",
   project_urls = {"Documentation" :"https://setga.readthedocs.io/en/latest/genindex.html"},
   install_requires=[          
           'numpy',
           'deap',
           "matplotlib",
```

