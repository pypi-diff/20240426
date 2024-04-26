# Comparing `tmp/centurypy-1.0.2.tar.gz` & `tmp/centurypy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "centurypy-1.0.2.tar", last modified: Thu Apr 25 04:37:07 2024, max compression
+gzip compressed data, was "centurypy-1.0.3.tar", last modified: Fri Apr 26 17:21:16 2024, max compression
```

## Comparing `centurypy-1.0.2.tar` & `centurypy-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gerardovivas   (501) staff       (20)        0 2024-04-25 04:37:07.031980 centurypy-1.0.2/
--rw-r--r--   0 gerardovivas   (501) staff       (20)     1070 2023-12-18 17:56:28.000000 centurypy-1.0.2/LICENSE
--rw-r--r--   0 gerardovivas   (501) staff       (20)     2925 2024-04-25 04:37:07.031350 centurypy-1.0.2/PKG-INFO
--rw-r--r--   0 gerardovivas   (501) staff       (20)     2612 2023-12-29 04:38:18.000000 centurypy-1.0.2/README.md
-drwxr-xr-x   0 gerardovivas   (501) staff       (20)        0 2024-04-25 04:37:07.027035 centurypy-1.0.2/centurypy/
--rw-r--r--   0 gerardovivas   (501) staff       (20)       27 2023-10-13 17:46:30.000000 centurypy-1.0.2/centurypy/__init__.py
--rw-r--r--   0 gerardovivas   (501) staff       (20)     2334 2023-12-12 02:06:35.000000 centurypy-1.0.2/centurypy/century.py
--rw-r--r--   0 gerardovivas   (501) staff       (20)     5220 2024-04-25 04:01:06.000000 centurypy-1.0.2/centurypy/genetic.py
--rw-r--r--   0 gerardovivas   (501) staff       (20)     4977 2023-12-16 16:23:00.000000 centurypy-1.0.2/centurypy/main.py
-drwxr-xr-x   0 gerardovivas   (501) staff       (20)        0 2024-04-25 04:37:07.030559 centurypy-1.0.2/centurypy.egg-info/
--rw-r--r--   0 gerardovivas   (501) staff       (20)     2925 2024-04-25 04:37:06.000000 centurypy-1.0.2/centurypy.egg-info/PKG-INFO
--rw-r--r--   0 gerardovivas   (501) staff       (20)      272 2024-04-25 04:37:06.000000 centurypy-1.0.2/centurypy.egg-info/SOURCES.txt
--rw-r--r--   0 gerardovivas   (501) staff       (20)        1 2024-04-25 04:37:06.000000 centurypy-1.0.2/centurypy.egg-info/dependency_links.txt
--rw-r--r--   0 gerardovivas   (501) staff       (20)       19 2024-04-25 04:37:06.000000 centurypy-1.0.2/centurypy.egg-info/requires.txt
--rw-r--r--   0 gerardovivas   (501) staff       (20)       10 2024-04-25 04:37:06.000000 centurypy-1.0.2/centurypy.egg-info/top_level.txt
--rw-r--r--   0 gerardovivas   (501) staff       (20)       38 2024-04-25 04:37:07.032132 centurypy-1.0.2/setup.cfg
--rw-r--r--   0 gerardovivas   (501) staff       (20)      873 2024-04-25 04:00:39.000000 centurypy-1.0.2/setup.py
+drwxr-xr-x   0 gerardovivas   (501) staff       (20)        0 2024-04-26 17:21:16.429916 centurypy-1.0.3/
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     1070 2023-12-18 17:56:28.000000 centurypy-1.0.3/LICENSE
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     2925 2024-04-26 17:21:16.429610 centurypy-1.0.3/PKG-INFO
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     2612 2023-12-29 04:38:18.000000 centurypy-1.0.3/README.md
+drwxr-xr-x   0 gerardovivas   (501) staff       (20)        0 2024-04-26 17:21:16.425866 centurypy-1.0.3/centurypy/
+-rw-r--r--   0 gerardovivas   (501) staff       (20)       27 2023-10-13 17:46:30.000000 centurypy-1.0.3/centurypy/__init__.py
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     2582 2024-04-26 16:08:47.000000 centurypy-1.0.3/centurypy/century.py
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     4398 2024-04-26 14:55:07.000000 centurypy-1.0.3/centurypy/genetic.py
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     4885 2024-04-26 16:54:52.000000 centurypy-1.0.3/centurypy/main.py
+drwxr-xr-x   0 gerardovivas   (501) staff       (20)        0 2024-04-26 17:21:16.428982 centurypy-1.0.3/centurypy.egg-info/
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     2925 2024-04-26 17:21:16.000000 centurypy-1.0.3/centurypy.egg-info/PKG-INFO
+-rw-r--r--   0 gerardovivas   (501) staff       (20)      272 2024-04-26 17:21:16.000000 centurypy-1.0.3/centurypy.egg-info/SOURCES.txt
+-rw-r--r--   0 gerardovivas   (501) staff       (20)        1 2024-04-26 17:21:16.000000 centurypy-1.0.3/centurypy.egg-info/dependency_links.txt
+-rw-r--r--   0 gerardovivas   (501) staff       (20)       19 2024-04-26 17:21:16.000000 centurypy-1.0.3/centurypy.egg-info/requires.txt
+-rw-r--r--   0 gerardovivas   (501) staff       (20)       10 2024-04-26 17:21:16.000000 centurypy-1.0.3/centurypy.egg-info/top_level.txt
+-rw-r--r--   0 gerardovivas   (501) staff       (20)       38 2024-04-26 17:21:16.430003 centurypy-1.0.3/setup.cfg
+-rw-r--r--   0 gerardovivas   (501) staff       (20)      873 2024-04-26 17:20:04.000000 centurypy-1.0.3/setup.py
```

### Comparing `centurypy-1.0.2/LICENSE` & `centurypy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `centurypy-1.0.2/PKG-INFO` & `centurypy-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: centurypy
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library to train and run the CENTURY (Soil Organic Matter) model
 Home-page: https://github.com/vivas24/centurypy
 Author: Gerardo Vivas
 Author-email: vivas.fermin24@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `centurypy-1.0.2/README.md` & `centurypy-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `centurypy-1.0.2/centurypy/century.py` & `centurypy-1.0.3/centurypy/century.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,28 @@
         self.METo = self.Necromasa * self.fs
         self.LENo = LENo
         self.PASo = PASo
         self.ACTo = ACTo
         self.RESPo = RESPo
 
 
-    def resolve(self, time, Kmet, Kest , Kminl, Khumac , Kminp , ResEL , ResEA , ResMet , ResLA , ResPA , PartEst , PartLen , PartAct ):
+    def resolve(self, time, params):
+        Kmet = params[0] 
+        Kest = params[1]
+        Kminl = params[2]
+        Khumac = params[3]
+        Kminp = params[4]
+        ResEL = params[5]
+        ResEA = params[6]
+        ResMet = params[7]
+        ResLA = params[8]
+        ResPA = params[9]
+        PartEst = params[10]
+        PartLen = params[11]
+        PartAct = params[12]
 
         y0 = self.ESTo, self.METo, self.LENo, self.ACTo, self.PASo, self.RESPo
         
         args = (self.Ftex, Kmet, Kest, Kminl, Khumac, Kminp, ResEL, ResEA, ResMet, ResLA, ResPA, PartEst, PartLen, PartAct)
         
         y = odeint(Century.ode, y0, time, args)
```

### Comparing `centurypy-1.0.2/centurypy/genetic.py` & `centurypy-1.0.3/centurypy/genetic.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,28 +21,15 @@
         self.population = []
         self.milestones = []
         self.fitness = []
         self.generate_population()
 
 
     def mse(self, parameters):
-        model_data = self.century_model.resolve(self.time_data,
-                                                parameters[0], 
-                                                parameters[1], 
-                                                parameters[2], 
-                                                parameters[3], 
-                                                parameters[4], 
-                                                parameters[5], 
-                                                parameters[6], 
-                                                parameters[7], 
-                                                parameters[8], 
-                                                parameters[9], 
-                                                parameters[10], 
-                                                parameters[11], 
-                                                parameters[12])
+        model_data = self.century_model.resolve(self.time_data, parameters)
         max_value = 0
         for i in [0,1]:
             values_model = model_data[i]
             values_training = self.training_data[i]
             sum = 0
             for j in range(len(values_model)):
                 sum += (values_model[j] - values_training[j]) ** 2
```

### Comparing `centurypy-1.0.2/centurypy.egg-info/PKG-INFO` & `centurypy-1.0.3/centurypy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: centurypy
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library to train and run the CENTURY (Soil Organic Matter) model
 Home-page: https://github.com/vivas24/centurypy
 Author: Gerardo Vivas
 Author-email: vivas.fermin24@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `centurypy-1.0.2/setup.py` & `centurypy-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 PACKAGE_NAME = 'centurypy'
 AUTHOR = 'Gerardo Vivas'
 AUTHOR_EMAIL = 'vivas.fermin24@gmail.com'
 URL = 'https://github.com/vivas24/centurypy'
 LICENSE = 'MIT'
 DESCRIPTION = 'Library to train and run the CENTURY (Soil Organic Matter) model' 
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8')
```

