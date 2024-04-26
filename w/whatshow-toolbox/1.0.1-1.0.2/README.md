# Comparing `tmp/whatshow_toolbox-1.0.1.tar.gz` & `tmp/whatshow_toolbox-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatshow_toolbox-1.0.1.tar", last modified: Wed Apr 24 08:23:00 2024, max compression
+gzip compressed data, was "whatshow_toolbox-1.0.2.tar", last modified: Fri Apr 26 03:23:59 2024, max compression
```

## Comparing `whatshow_toolbox-1.0.1.tar` & `whatshow_toolbox-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 08:23:00.304654 whatshow_toolbox-1.0.1/
--rw-rw-rw-   0        0        0     1780 2024-04-24 08:23:00.302654 whatshow_toolbox-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1672 2024-04-24 08:22:59.000000 whatshow_toolbox-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 08:23:00.305662 whatshow_toolbox-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      403 2024-04-24 08:22:59.000000 whatshow_toolbox-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 08:23:00.280625 whatshow_toolbox-1.0.1/whatshow_toolbox/
--rw-rw-rw-   0        0        0    12823 2024-04-24 08:22:59.000000 whatshow_toolbox-1.0.1/whatshow_toolbox/MatlabFuncHelper.py
--rw-rw-rw-   0        0        0       46 2024-04-24 08:22:59.000000 whatshow_toolbox-1.0.1/whatshow_toolbox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 08:23:00.301655 whatshow_toolbox-1.0.1/whatshow_toolbox.egg-info/
--rw-rw-rw-   0        0        0     1780 2024-04-24 08:23:00.000000 whatshow_toolbox-1.0.1/whatshow_toolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-04-24 08:23:00.000000 whatshow_toolbox-1.0.1/whatshow_toolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 08:23:00.000000 whatshow_toolbox-1.0.1/whatshow_toolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-24 08:23:00.000000 whatshow_toolbox-1.0.1/whatshow_toolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-24 08:23:00.000000 whatshow_toolbox-1.0.1/whatshow_toolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 03:23:59.102356 whatshow_toolbox-1.0.2/
+-rw-rw-rw-   0        0        0     2112 2024-04-26 03:23:59.099135 whatshow_toolbox-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2004 2024-04-26 03:23:58.000000 whatshow_toolbox-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 03:23:59.102356 whatshow_toolbox-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      403 2024-04-26 03:23:58.000000 whatshow_toolbox-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:23:59.084538 whatshow_toolbox-1.0.2/whatshow_toolbox/
+-rw-rw-rw-   0        0        0    13054 2024-04-26 03:23:58.000000 whatshow_toolbox-1.0.2/whatshow_toolbox/MatlabFuncHelper.py
+-rw-rw-rw-   0        0        0       46 2024-04-26 03:23:58.000000 whatshow_toolbox-1.0.2/whatshow_toolbox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:23:59.098136 whatshow_toolbox-1.0.2/whatshow_toolbox.egg-info/
+-rw-rw-rw-   0        0        0     2112 2024-04-26 03:23:58.000000 whatshow_toolbox-1.0.2/whatshow_toolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-04-26 03:23:59.000000 whatshow_toolbox-1.0.2/whatshow_toolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 03:23:58.000000 whatshow_toolbox-1.0.2/whatshow_toolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-26 03:23:58.000000 whatshow_toolbox-1.0.2/whatshow_toolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-26 03:23:58.000000 whatshow_toolbox-1.0.2/whatshow_toolbox.egg-info/top_level.txt
```

### Comparing `whatshow_toolbox-1.0.1/whatshow_toolbox/MatlabFuncHelper.py` & `whatshow_toolbox-1.0.2/whatshow_toolbox/MatlabFuncHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import numpy as np
 class MatlabFuncHelper(object):
     BATCH_SIZE_NO = None;
     
     batch_size = BATCH_SIZE_NO;
     
     ###########################################################################
+    # Batch
+    def setBatchSize(self, batch_size):
+        self.batch_size = batch_size;
+    def getBatchSize(self):
+        return self.batch_size;
+    
+    ###########################################################################
     # checkers
     '''
     check input is a vector like [(batch_size), n],  [(batch_size), ..., n, 1] or [(batch_size), ..., 1, n] 
     '''
     def isvector(self, mat):
         mat = np.asarray(mat);
         if self.batch_size == self.BATCH_SIZE_NO:
@@ -254,15 +261,15 @@
                 else:
                     out[batch_id, ...] = np.roll(mat[batch_id, ...], step[batch_id], axis=0);
         return out;
 
     ###########################################################################
     # Maths
     '''
-    return the maximum value of a matrix or the maximu value of two matrices (for complex value, we compare the magnitude)
+    return the maximum of a matrix or the maximum of two matrices (for complex value, we compare the magnitude)
     @in1:   the matrix to find the maximal value
     @in2:   a scalar or a matrix to be compared with in1. If not given, it means return the maximal value of in1
     @axis:  the axis to compare or find the maximal value
     '''
     def max(self, in1, *args, axis=-1):
         out = None;
         in1 = np.asarray(in1);
```

