# Comparing `tmp/setga-1.4.1.tar.gz` & `tmp/setga-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setga-1.4.1.tar", last modified: Thu Apr 25 13:32:25 2024, max compression
+gzip compressed data, was "setga-1.4.2.tar", last modified: Fri Apr 26 12:50:33 2024, max compression
```

## Comparing `setga-1.4.1.tar` & `setga-1.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:32:25.050269 setga-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-25 13:32:22.000000 setga-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-25 13:32:25.050269 setga-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-25 13:32:22.000000 setga-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:32:25.050269 setga-1.4.1/setga/
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-04-25 13:32:22.000000 setga-1.4.1/setga/select_subset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-04-25 13:32:22.000000 setga-1.4.1/setga/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:32:25.050269 setga-1.4.1/setga.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-25 13:32:25.000000 setga-1.4.1/setga.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-25 13:32:25.000000 setga-1.4.1/setga.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:32:25.000000 setga-1.4.1/setga.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 13:32:25.000000 setga-1.4.1/setga.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 13:32:25.000000 setga-1.4.1/setga.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-25 13:32:25.050269 setga-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-25 13:32:23.000000 setga-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:50:33.691693 setga-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 12:50:30.000000 setga-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-26 12:50:33.691693 setga-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-26 12:50:30.000000 setga-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:50:33.691693 setga-1.4.2/setga/
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-04-26 12:50:30.000000 setga-1.4.2/setga/select_subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-04-26 12:50:30.000000 setga-1.4.2/setga/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:50:33.691693 setga-1.4.2/setga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-26 12:50:33.000000 setga-1.4.2/setga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-26 12:50:33.000000 setga-1.4.2/setga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 12:50:33.000000 setga-1.4.2/setga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 12:50:33.000000 setga-1.4.2/setga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 12:50:33.000000 setga-1.4.2/setga.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-26 12:50:33.691693 setga-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-26 12:50:32.000000 setga-1.4.2/setup.py
```

### Comparing `setga-1.4.1/LICENSE` & `setga-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `setga-1.4.1/PKG-INFO` & `setga-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setga
-Version: 1.4.1
+Version: 1.4.2
 Summary: library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.
 Home-page: https://github.com/lavakin/setga
 Author: Nikola Kalábová
 Author-email: nikola@kalabova.eu
 License: MIT
 Project-URL: Documentation, https://setga.readthedocs.io/en/latest/genindex.html
 Keywords: Genetic algorithms,minimal subset,multi-objective,optimization
```

### Comparing `setga-1.4.1/README.md` & `setga-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `setga-1.4.1/setga/select_subset.py` & `setga-1.4.2/setga/select_subset.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # mutation: ["bit_flip","inversion"]
 # crossover: ["uniform", "onepoint","twopoint","partialy_matched","ordered","uniform_partialy_matched"],
 # selection: ["SPEA2","NGSA2"]
 def run_minimizer(set_size,eval_ind, stats_by,stats_names,eval_func_kwargs={},mutation_rate = 0.001,crossover_rate = 0.02, 
                   pop_size = 150, num_gen = 8000, num_islands = 6, mutation = "bit_flip" , 
                   crossover =  "uniform_partialy_matched", selection = "SPEA2",frac_init_not_removed = 0.01,
-                  create_individual_funct = None, create_individual_func_kwargs={}):
+                  create_individual_funct = None, create_individual_func_kwargs={}, ref_points = None):
     """Run minimizer algorithm to optimize individual solutions.
 
     :param set_size: int
         Size of the set to be optimized.
     :param evaluate_individual: function
         Function to evaluate a single individual.
     :param eval_func_kwargs: dict
@@ -119,14 +119,18 @@
     if crossover not in ["uniform", "onepoint","twopoint","partialy_matched","ordered","uniform_partialy_matched"] and not callable(crossover):
         raise WrongType("Unknown type of crossover")
 
     if selection == "SPEA2":
         toolbox.register("select", tools.selSPEA2)
     if selection == "NSGA2":
         toolbox.register("select", tools.selNSGA2)
+    if selection == "NSGA3":
+        if ref_points == None:
+            raise WrongType("Ref_points cannot be None")
+        toolbox.register("select", tools.selNSGA2,ref_points = ref_points)
     if selection not in ["SPEA2","NSGA2"]:
         raise WrongType("Unknown type of mating")
     
     toolbox.register("migrate",tools.migRing,k=10,selection = toolbox.select)
 
     stats = tools.Statistics()
```

### Comparing `setga-1.4.1/setga/utils.py` & `setga-1.4.2/setga/utils.py`

 * *Files identical despite different names*

### Comparing `setga-1.4.1/setga.egg-info/PKG-INFO` & `setga-1.4.2/setga.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setga
-Version: 1.4.1
+Version: 1.4.2
 Summary: library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.
 Home-page: https://github.com/lavakin/setga
 Author: Nikola Kalábová
 Author-email: nikola@kalabova.eu
 License: MIT
 Project-URL: Documentation, https://setga.readthedocs.io/en/latest/genindex.html
 Keywords: Genetic algorithms,minimal subset,multi-objective,optimization
```

### Comparing `setga-1.4.1/setup.py` & `setga-1.4.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   name = 'setga',         
   packages = ['setga'], 
   license='MIT',       
   description = 'library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.',   # Give a short description about your library
   author = 'Nikola Kalábová',              
   author_email = 'nikola@kalabova.eu',     
   url = 'https://github.com/lavakin/setga',  
-  version = "1.4.1",    
+  version = "1.4.2",    
   keywords = ['Genetic algorithms', 'minimal subset', 'multi-objective', "optimization"],   
   long_description = "library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.",
   project_urls = {"Documentation" :"https://setga.readthedocs.io/en/latest/genindex.html"},
   install_requires=[          
           'numpy',
           'deap',
           "matplotlib",
```

