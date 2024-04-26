# Comparing `tmp/brom_drake-0.1.0.tar.gz` & `tmp/brom_drake-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brom_drake-0.1.0.tar", last modified: Tue Apr 16 17:25:27 2024, max compression
+gzip compressed data, was "brom_drake-0.1.1.tar", last modified: Fri Apr 26 21:09:58 2024, max compression
```

## Comparing `brom_drake-0.1.0.tar` & `brom_drake-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:25:27.569141 brom_drake-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 17:25:25.000000 brom_drake-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-16 17:25:27.569141 brom_drake-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-16 17:25:25.000000 brom_drake-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:25:27.569141 brom_drake-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-16 17:25:26.000000 brom_drake-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:25:27.565142 brom_drake-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:25:27.565142 brom_drake-0.1.0/src/brom_drake/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:25:27.565142 brom_drake-0.1.0/src/brom_drake/DiagramTarget/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/DiagramTarget/DiagramTarget.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/DiagramTarget/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:25:27.569141 brom_drake-0.1.0/src/brom_drake/DiagramWatcher/
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/DiagramWatcher/DiagramWatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/DiagramWatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/DiagramWatcher/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/DiagramWatcher/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:25:27.569141 brom_drake-0.1.0/src/brom_drake/PortWatcher/
--rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/PortWatcher/PortWatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/PortWatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:25:27.569141 brom_drake-0.1.0/src/brom_drake/all/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/all/add_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:25:27.565142 brom_drake-0.1.0/src/brom_drake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-16 17:25:27.000000 brom_drake-0.1.0/src/brom_drake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-16 17:25:27.000000 brom_drake-0.1.0/src/brom_drake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:25:27.000000 brom_drake-0.1.0/src/brom_drake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 17:25:27.000000 brom_drake-0.1.0/src/brom_drake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 17:25:27.000000 brom_drake-0.1.0/src/brom_drake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:09:58.323344 brom_drake-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-26 21:09:55.000000 brom_drake-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-26 21:09:58.323344 brom_drake-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-26 21:09:55.000000 brom_drake-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 21:09:58.323344 brom_drake-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-26 21:09:57.000000 brom_drake-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:09:58.319344 brom_drake-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:09:58.319344 brom_drake-0.1.1/src/brom_drake/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:09:58.319344 brom_drake-0.1.1/src/brom_drake/DiagramTarget/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-26 21:09:55.000000 brom_drake-0.1.1/src/brom_drake/DiagramTarget/DiagramTarget.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-26 21:09:55.000000 brom_drake-0.1.1/src/brom_drake/DiagramTarget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:09:58.319344 brom_drake-0.1.1/src/brom_drake/DiagramWatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-04-26 21:09:55.000000 brom_drake-0.1.1/src/brom_drake/DiagramWatcher/DiagramWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-26 21:09:55.000000 brom_drake-0.1.1/src/brom_drake/DiagramWatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-26 21:09:55.000000 brom_drake-0.1.1/src/brom_drake/DiagramWatcher/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-26 21:09:55.000000 brom_drake-0.1.1/src/brom_drake/DiagramWatcher/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:09:58.319344 brom_drake-0.1.1/src/brom_drake/PortWatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-26 21:09:55.000000 brom_drake-0.1.1/src/brom_drake/PortWatcher/PortWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 21:09:55.000000 brom_drake-0.1.1/src/brom_drake/PortWatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 21:09:55.000000 brom_drake-0.1.1/src/brom_drake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:09:58.319344 brom_drake-0.1.1/src/brom_drake/all/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-26 21:09:55.000000 brom_drake-0.1.1/src/brom_drake/all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-26 21:09:55.000000 brom_drake-0.1.1/src/brom_drake/all/add_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:09:58.319344 brom_drake-0.1.1/src/brom_drake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-26 21:09:58.000000 brom_drake-0.1.1/src/brom_drake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-26 21:09:58.000000 brom_drake-0.1.1/src/brom_drake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 21:09:58.000000 brom_drake-0.1.1/src/brom_drake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-26 21:09:58.000000 brom_drake-0.1.1/src/brom_drake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 21:09:58.000000 brom_drake-0.1.1/src/brom_drake.egg-info/top_level.txt
```

### Comparing `brom_drake-0.1.0/LICENSE` & `brom_drake-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brom_drake-0.1.0/PKG-INFO` & `brom_drake-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brom_drake
-Version: 0.1.0
+Version: 0.1.1
 Summary: A set of convenient logging and testing tools for the Drake robotics toolbox.
 Author: Kwesi Rutledge
 Author-email: thesolitaryecrivain@gmail.com
 Keywords: drake,robotics,testing,logging
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `brom_drake-0.1.0/README.md` & `brom_drake-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `brom_drake-0.1.0/setup.py` & `brom_drake-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with codecs.open(
         os.path.join(here, "README.md"), encoding="utf-8"
     ) as f:
         long_description = "\n" + f.read()
 
     setup(
         name="brom_drake",
-        version='0.1.0',
+        version='0.1.1',
         author="Kwesi Rutledge",
         author_email="thesolitaryecrivain@gmail.com",
         description="A set of convenient logging and testing tools for the Drake robotics toolbox.",
         long_description_content_type="text/markdown",
         long_description=long_description,
         # packages=find_packages(where='src/brom_drake'),
         install_requires=['drake', 'meshcat', 'manipulation', 'loguru', 'matplotlib'],
```

### Comparing `brom_drake-0.1.0/src/brom_drake/DiagramWatcher/DiagramWatcher.py` & `brom_drake-0.1.1/src/brom_drake/DiagramWatcher/DiagramWatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 class DiagramWatcher:
     def __init__(
         self,
         subject: DiagramBuilder,
         targets: List[DiagramTarget] = None,
-        plot_dir: str = "./.brom",
+        plot_dir: str = "./brom",
         dpi: int = 300,
     ):
         # Setup
         self.diagram = None
         self.dpi = dpi
 
         # Check subject
```

### Comparing `brom_drake-0.1.0/src/brom_drake/DiagramWatcher/errors.py` & `brom_drake-0.1.1/src/brom_drake/DiagramWatcher/errors.py`

 * *Files identical despite different names*

### Comparing `brom_drake-0.1.0/src/brom_drake/PortWatcher/PortWatcher.py` & `brom_drake-0.1.1/src/brom_drake/PortWatcher/PortWatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def __init__(
         self,
         system: LeafSystem,
         output_port: OutputPort,
         builder: DiagramBuilder,
         logger_name: str = None,
         options: PortWatcherOptions = PortWatcherOptions(),
-        plot_dir: str = "./.brom",
+        plot_dir: str = "./brom",
     ):
         # Setup
         self.options = options
         self.system = system
         self.port = output_port
         self.data = {}
         self.plot_handles = {}
```

### Comparing `brom_drake-0.1.0/src/brom_drake/all/add_watcher.py` & `brom_drake-0.1.1/src/brom_drake/all/add_watcher.py`

 * *Files identical despite different names*

### Comparing `brom_drake-0.1.0/src/brom_drake.egg-info/PKG-INFO` & `brom_drake-0.1.1/src/brom_drake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brom-drake
-Version: 0.1.0
+Version: 0.1.1
 Summary: A set of convenient logging and testing tools for the Drake robotics toolbox.
 Author: Kwesi Rutledge
 Author-email: thesolitaryecrivain@gmail.com
 Keywords: drake,robotics,testing,logging
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `brom_drake-0.1.0/src/brom_drake.egg-info/SOURCES.txt` & `brom_drake-0.1.1/src/brom_drake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

