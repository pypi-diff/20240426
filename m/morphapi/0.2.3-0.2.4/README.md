# Comparing `tmp/morphapi-0.2.3.tar.gz` & `tmp/morphapi-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphapi-0.2.3.tar", last modified: Tue Mar 19 12:23:40 2024, max compression
+gzip compressed data, was "morphapi-0.2.4.tar", last modified: Fri Apr 26 13:57:18 2024, max compression
```

## Comparing `morphapi-0.2.3.tar` & `morphapi-0.2.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:23:40.917168 morphapi-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:23:40.909169 morphapi-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:23:40.913169 morphapi-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-19 12:23:35.000000 morphapi-0.2.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-19 12:23:35.000000 morphapi-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-19 12:23:35.000000 morphapi-0.2.3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-19 12:23:35.000000 morphapi-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-19 12:23:35.000000 morphapi-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-03-19 12:23:40.917168 morphapi-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-19 12:23:35.000000 morphapi-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:23:40.913169 morphapi-0.2.3/morphapi/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-19 12:23:35.000000 morphapi-0.2.3/morphapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:23:40.913169 morphapi-0.2.3/morphapi/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 12:23:35.000000 morphapi-0.2.3/morphapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-03-19 12:23:35.000000 morphapi-0.2.3/morphapi/api/allenmorphology.py
--rw-r--r--   0 runner    (1001) docker     (127)    16887 2024-03-19 12:23:35.000000 morphapi-0.2.3/morphapi/api/mouselight.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-19 12:23:35.000000 morphapi-0.2.3/morphapi/api/mpin_celldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-03-19 12:23:35.000000 morphapi-0.2.3/morphapi/api/neuromorphorg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:23:40.917168 morphapi-0.2.3/morphapi/morphology/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 12:23:35.000000 morphapi-0.2.3/morphapi/morphology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-03-19 12:23:35.000000 morphapi-0.2.3/morphapi/morphology/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     9791 2024-03-19 12:23:35.000000 morphapi-0.2.3/morphapi/morphology/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-03-19 12:23:35.000000 morphapi-0.2.3/morphapi/paths_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:23:40.917168 morphapi-0.2.3/morphapi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 12:23:35.000000 morphapi-0.2.3/morphapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-03-19 12:23:35.000000 morphapi-0.2.3/morphapi/utils/data_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-03-19 12:23:35.000000 morphapi-0.2.3/morphapi/utils/webqueries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:23:40.917168 morphapi-0.2.3/morphapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-03-19 12:23:40.000000 morphapi-0.2.3/morphapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-19 12:23:40.000000 morphapi-0.2.3/morphapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 12:23:40.000000 morphapi-0.2.3/morphapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-19 12:23:40.000000 morphapi-0.2.3/morphapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-19 12:23:40.000000 morphapi-0.2.3/morphapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-03-19 12:23:35.000000 morphapi-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 12:23:40.917168 morphapi-0.2.3/setup.cfg
+drwxr-xr-x   0 adamtyson   (501) staff       (20)        0 2024-04-26 13:57:18.499450 morphapi-0.2.4/
+drwxr-xr-x   0 adamtyson   (501) staff       (20)        0 2024-04-26 13:57:18.460327 morphapi-0.2.4/.github/
+drwxr-xr-x   0 adamtyson   (501) staff       (20)        0 2024-04-26 13:57:18.462115 morphapi-0.2.4/.github/workflows/
+-rw-r--r--   0 adamtyson   (501) staff       (20)     1444 2024-02-09 14:31:34.000000 morphapi-0.2.4/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 adamtyson   (501) staff       (20)      978 2024-02-09 14:31:34.000000 morphapi-0.2.4/.gitignore
+-rw-r--r--   0 adamtyson   (501) staff       (20)      624 2024-04-26 10:23:07.000000 morphapi-0.2.4/CITATION.cff
+-rw-r--r--   0 adamtyson   (501) staff       (20)     1082 2024-02-09 14:31:34.000000 morphapi-0.2.4/LICENSE
+-rw-r--r--   0 adamtyson   (501) staff       (20)      229 2024-04-26 10:23:07.000000 morphapi-0.2.4/MANIFEST.in
+-rw-r--r--   0 adamtyson   (501) staff       (20)     2277 2024-04-26 13:57:18.499110 morphapi-0.2.4/PKG-INFO
+-rw-r--r--   0 adamtyson   (501) staff       (20)      402 2024-02-09 14:31:34.000000 morphapi-0.2.4/README.md
+drwxr-xr-x   0 adamtyson   (501) staff       (20)        0 2024-04-26 13:57:18.473334 morphapi-0.2.4/morphapi/
+-rw-r--r--   0 adamtyson   (501) staff       (20)      174 2024-02-09 14:31:34.000000 morphapi-0.2.4/morphapi/__init__.py
+drwxr-xr-x   0 adamtyson   (501) staff       (20)        0 2024-04-26 13:57:18.475788 morphapi-0.2.4/morphapi/api/
+-rw-r--r--   0 adamtyson   (501) staff       (20)        0 2024-02-09 14:31:34.000000 morphapi-0.2.4/morphapi/api/__init__.py
+-rw-r--r--   0 adamtyson   (501) staff       (20)     3651 2024-02-09 14:31:34.000000 morphapi-0.2.4/morphapi/api/allenmorphology.py
+-rw-r--r--   0 adamtyson   (501) staff       (20)    16887 2024-04-26 10:23:07.000000 morphapi-0.2.4/morphapi/api/mouselight.py
+-rw-r--r--   0 adamtyson   (501) staff       (20)     5706 2024-04-26 10:23:07.000000 morphapi-0.2.4/morphapi/api/mpin_celldb.py
+-rw-r--r--   0 adamtyson   (501) staff       (20)     8449 2024-02-09 14:31:34.000000 morphapi-0.2.4/morphapi/api/neuromorphorg.py
+drwxr-xr-x   0 adamtyson   (501) staff       (20)        0 2024-04-26 13:57:18.495376 morphapi-0.2.4/morphapi/morphology/
+-rw-r--r--   0 adamtyson   (501) staff       (20)        0 2024-02-09 14:31:34.000000 morphapi-0.2.4/morphapi/morphology/__init__.py
+-rw-r--r--   0 adamtyson   (501) staff       (20)     4531 2024-02-09 14:31:34.000000 morphapi-0.2.4/morphapi/morphology/cache.py
+-rw-r--r--   0 adamtyson   (501) staff       (20)     8850 2024-04-26 13:56:19.000000 morphapi-0.2.4/morphapi/morphology/morphology.py
+-rw-r--r--   0 adamtyson   (501) staff       (20)     1627 2024-02-09 14:31:34.000000 morphapi-0.2.4/morphapi/paths_manager.py
+drwxr-xr-x   0 adamtyson   (501) staff       (20)        0 2024-04-26 13:57:18.496680 morphapi-0.2.4/morphapi/utils/
+-rw-r--r--   0 adamtyson   (501) staff       (20)        0 2024-02-09 14:31:34.000000 morphapi-0.2.4/morphapi/utils/__init__.py
+-rw-r--r--   0 adamtyson   (501) staff       (20)     3086 2024-02-09 14:31:34.000000 morphapi-0.2.4/morphapi/utils/data_io.py
+-rw-r--r--   0 adamtyson   (501) staff       (20)     4072 2024-04-26 10:23:07.000000 morphapi-0.2.4/morphapi/utils/webqueries.py
+drwxr-xr-x   0 adamtyson   (501) staff       (20)        0 2024-04-26 13:57:18.497116 morphapi-0.2.4/morphapi.egg-info/
+-rw-r--r--   0 adamtyson   (501) staff       (20)     2277 2024-04-26 13:57:18.000000 morphapi-0.2.4/morphapi.egg-info/PKG-INFO
+-rw-r--r--   0 adamtyson   (501) staff       (20)      631 2024-04-26 13:57:18.000000 morphapi-0.2.4/morphapi.egg-info/SOURCES.txt
+-rw-r--r--   0 adamtyson   (501) staff       (20)        1 2024-04-26 13:57:18.000000 morphapi-0.2.4/morphapi.egg-info/dependency_links.txt
+-rw-r--r--   0 adamtyson   (501) staff       (20)      279 2024-04-26 13:57:18.000000 morphapi-0.2.4/morphapi.egg-info/requires.txt
+-rw-r--r--   0 adamtyson   (501) staff       (20)        9 2024-04-26 13:57:18.000000 morphapi-0.2.4/morphapi.egg-info/top_level.txt
+-rw-r--r--   0 adamtyson   (501) staff       (20)     2421 2024-04-26 10:23:07.000000 morphapi-0.2.4/pyproject.toml
+-rw-r--r--   0 adamtyson   (501) staff       (20)       38 2024-04-26 13:57:18.499523 morphapi-0.2.4/setup.cfg
```

### Comparing `morphapi-0.2.3/.github/workflows/test_and_deploy.yml` & `morphapi-0.2.4/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.3/.gitignore` & `morphapi-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.3/CITATION.cff` & `morphapi-0.2.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.3/LICENSE` & `morphapi-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.3/PKG-INFO` & `morphapi-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphapi
-Version: 0.2.3
+Version: 0.2.4
 Summary: A lightweight python package to download neuronal morphologies
 Author-email: Federico Claudi <hello@brainglobe.info>
 License: MIT
 Project-URL: Homepage, https://github.com/brainglobe/morphapi
 Project-URL: Bug Tracker, https://github.com/brainglobe/morphapi/issues
 Project-URL: Documentation, https://github.com/brainglobe/morphapi
 Project-URL: Source Code, https://github.com/brainglobe/morphapi
```

### Comparing `morphapi-0.2.3/morphapi/api/allenmorphology.py` & `morphapi-0.2.4/morphapi/api/allenmorphology.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.3/morphapi/api/mouselight.py` & `morphapi-0.2.4/morphapi/api/mouselight.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.3/morphapi/api/mpin_celldb.py` & `morphapi-0.2.4/morphapi/api/mpin_celldb.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.3/morphapi/api/neuromorphorg.py` & `morphapi-0.2.4/morphapi/api/neuromorphorg.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.3/morphapi/morphology/cache.py` & `morphapi-0.2.4/morphapi/morphology/cache.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.3/morphapi/morphology/morphology.py` & `morphapi-0.2.4/morphapi/morphology/morphology.py`

 * *Files 14% similar despite different names*

```diff
@@ -69,52 +69,18 @@
         if self.data_file_type is None:
             return
         elif self.data_file_type == "json":
             raise NotImplementedError
         else:
             self.load_from_swc()
 
-    def repair_swc_file(self):
-        """
-        Fixes this: https://github.com/BlueBrain/NeuroM/issues/835
-        """
-        with open(self.data_file, "r") as read:
-            content = read.readlines()
-
-        clean = []
-        for line in content:
-            if not len(line):
-                clean.append(line)
-                continue
-
-            line = line.replace("\n", "").replace("\t", " ")
-            vals = line.split(" ")
-            if len(vals) < 2:
-                clean.append(line)
-                continue
-
-            if vals[1] != "1" and vals[-1] == "-1":
-                vals[-1] = "0"
-                clean.append(" ".join(vals))
-            else:
-                clean.append(line)
-
-        if len(clean) != len(content):
-            raise ValueError
-
-        with open(self.data_file, "w") as write:
-            for line in clean:
-                write.write(f"{line}\n")
-
     def load_from_swc(self):
         if self.neuron_name is None:
             self.neuron_name = self.data_file.name
 
-        self.repair_swc_file()
-
         nrn = nm.load_morphology(self.data_file)
 
         # Get position and radius of some
         soma_pos = nrn.soma.points[0, :3]
         soma_radius = nrn.soma.points[0, -1]
 
         # Get the rest of the data and store it
```

### Comparing `morphapi-0.2.3/morphapi/paths_manager.py` & `morphapi-0.2.4/morphapi/paths_manager.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.3/morphapi/utils/data_io.py` & `morphapi-0.2.4/morphapi/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.3/morphapi/utils/webqueries.py` & `morphapi-0.2.4/morphapi/utils/webqueries.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.3/morphapi.egg-info/PKG-INFO` & `morphapi-0.2.4/morphapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphapi
-Version: 0.2.3
+Version: 0.2.4
 Summary: A lightweight python package to download neuronal morphologies
 Author-email: Federico Claudi <hello@brainglobe.info>
 License: MIT
 Project-URL: Homepage, https://github.com/brainglobe/morphapi
 Project-URL: Bug Tracker, https://github.com/brainglobe/morphapi/issues
 Project-URL: Documentation, https://github.com/brainglobe/morphapi
 Project-URL: Source Code, https://github.com/brainglobe/morphapi
```

### Comparing `morphapi-0.2.3/morphapi.egg-info/SOURCES.txt` & `morphapi-0.2.4/morphapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.3/pyproject.toml` & `morphapi-0.2.4/pyproject.toml`

 * *Files identical despite different names*

