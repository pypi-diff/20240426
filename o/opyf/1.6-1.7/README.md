# Comparing `tmp/opyf-1.6.tar.gz` & `tmp/opyf-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opyf-1.6.tar", last modified: Mon Jan 29 12:46:19 2024, max compression
+gzip compressed data, was "opyf-1.7.tar", last modified: Fri Apr 26 15:25:00 2024, max compression
```

## Comparing `opyf-1.6.tar` & `opyf-1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 12:46:19.726411 opyf-1.6/
--rwxrwxrwx   0 root         (0) root         (0)    35147 2019-12-22 12:21:55.000000 opyf-1.6/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     7580 2024-01-29 12:46:19.725939 opyf-1.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     6677 2024-01-29 09:21:37.000000 opyf-1.6/ReadMe.md
--rwxrwxrwx   0 root         (0) root         (0)     1057 2024-01-29 12:46:04.000000 opyf-1.6/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-01-29 12:46:19.726512 opyf-1.6/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 12:46:19.714456 opyf-1.6/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 12:46:19.722957 opyf-1.6/src/opyf/
--rwxrwxrwx   0 root         (0) root         (0)    62962 2024-01-29 09:35:18.000000 opyf-1.6/src/opyf/Analyzer.py
--rwxrwxrwx   0 root         (0) root         (0)    15512 2020-04-26 10:03:50.000000 opyf-1.6/src/opyf/Files.py
--rwxrwxrwx   0 root         (0) root         (0)    13864 2021-10-28 09:42:29.000000 opyf-1.6/src/opyf/Filters.py
--rwxrwxrwx   0 root         (0) root         (0)     9066 2020-12-31 16:35:22.000000 opyf-1.6/src/opyf/Interpolate.py
--rwxrwxrwx   0 root         (0) root         (0)      964 2021-05-11 20:04:41.000000 opyf-1.6/src/opyf/MeshesAndTime.py
--rwxrwxrwx   0 root         (0) root         (0)    47309 2024-01-29 10:26:34.000000 opyf-1.6/src/opyf/Render.py
--rwxrwxrwx   0 root         (0) root         (0)      489 2020-04-27 10:04:17.000000 opyf-1.6/src/opyf/Tools.py
--rwxrwxrwx   0 root         (0) root         (0)     5243 2024-01-29 10:55:31.000000 opyf-1.6/src/opyf/Track.py
--rwxrwxrwx   0 root         (0) root         (0)      414 2019-12-22 12:21:55.000000 opyf-1.6/src/opyf/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    10754 2021-03-08 14:14:06.000000 opyf-1.6/src/opyf/custom_cmap.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 12:46:19.725430 opyf-1.6/src/opyf.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     7580 2024-01-29 12:46:19.000000 opyf-1.6/src/opyf.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      400 2024-01-29 12:46:19.000000 opyf-1.6/src/opyf.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-01-29 12:46:19.000000 opyf-1.6/src/opyf.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      105 2024-01-29 12:46:19.000000 opyf-1.6/src/opyf.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        5 2024-01-29 12:46:19.000000 opyf-1.6/src/opyf.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-26 15:25:00.815847 opyf-1.7/
+-rwxrwxrwx   0 root         (0) root         (0)    35147 2019-12-22 12:21:55.000000 opyf-1.7/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     7580 2024-04-26 15:25:00.815479 opyf-1.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     6677 2024-01-29 09:21:37.000000 opyf-1.7/ReadMe.md
+-rwxrwxrwx   0 root         (0) root         (0)     1057 2024-04-26 13:30:28.000000 opyf-1.7/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-26 15:25:00.815930 opyf-1.7/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-26 15:25:00.807337 opyf-1.7/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-26 15:25:00.812960 opyf-1.7/src/opyf/
+-rwxrwxrwx   0 root         (0) root         (0)    62968 2024-04-26 13:23:50.000000 opyf-1.7/src/opyf/Analyzer.py
+-rwxrwxrwx   0 root         (0) root         (0)    15512 2020-04-26 10:03:50.000000 opyf-1.7/src/opyf/Files.py
+-rwxrwxrwx   0 root         (0) root         (0)    13864 2021-10-28 09:42:29.000000 opyf-1.7/src/opyf/Filters.py
+-rwxrwxrwx   0 root         (0) root         (0)     9066 2020-12-31 16:35:22.000000 opyf-1.7/src/opyf/Interpolate.py
+-rwxrwxrwx   0 root         (0) root         (0)      964 2021-05-11 20:04:41.000000 opyf-1.7/src/opyf/MeshesAndTime.py
+-rwxrwxrwx   0 root         (0) root         (0)    47309 2024-01-29 10:26:34.000000 opyf-1.7/src/opyf/Render.py
+-rwxrwxrwx   0 root         (0) root         (0)      489 2020-04-27 10:04:17.000000 opyf-1.7/src/opyf/Tools.py
+-rwxrwxrwx   0 root         (0) root         (0)     5243 2024-01-29 10:55:31.000000 opyf-1.7/src/opyf/Track.py
+-rwxrwxrwx   0 root         (0) root         (0)      414 2019-12-22 12:21:55.000000 opyf-1.7/src/opyf/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10754 2021-03-08 14:14:06.000000 opyf-1.7/src/opyf/custom_cmap.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-26 15:25:00.814972 opyf-1.7/src/opyf.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     7580 2024-04-26 15:25:00.000000 opyf-1.7/src/opyf.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      400 2024-04-26 15:25:00.000000 opyf-1.7/src/opyf.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-26 15:25:00.000000 opyf-1.7/src/opyf.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      105 2024-04-26 15:25:00.000000 opyf-1.7/src/opyf.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2024-04-26 15:25:00.000000 opyf-1.7/src/opyf.egg-info/top_level.txt
```

### Comparing `opyf-1.6/LICENSE` & `opyf-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `opyf-1.6/PKG-INFO` & `opyf-1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opyf
-Version: 1.6
+Version: 1.7
 Summary: OpyFlow - Python package for Optical Flow measurements.
 Author-email: Gauthier Rousseau <gauthier.rousseau@gmail.com>
 Project-URL: Homepage, https://github.com/groussea/opyflow
 Project-URL: Bug Tracker, https://github.com/groussea/opyflow/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `opyf-1.6/ReadMe.md` & `opyf-1.7/ReadMe.md`

 * *Files identical despite different names*

### Comparing `opyf-1.6/pyproject.toml` & `opyf-1.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "opyf"
-version = "1.6"
+version = "1.7"
 authors = [
   { name="Gauthier Rousseau", email="gauthier.rousseau@gmail.com" },
 ]
 description = "OpyFlow - Python package for Optical Flow measurements."
 readme = "ReadMe.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `opyf-1.6/src/opyf/Analyzer.py` & `opyf-1.7/src/opyf/Analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1181,15 +1181,15 @@
         if s - self.vec[0] > 0:
             self.stab.set_vecTime(
                 Ntot=1,
                 starting_frame=self.vec[0],
                 step=s - self.vec[0])
             self.stab.extractGoodFeaturesAndDisplacements()
             transformation_rigid_matrix, rigid_mask = cv2.estimateAffine2D(
-                self.stab.X + self.stab.V/2, self.stab.X + self.stab.V/2 ) #because the position of the displacement is half the distance btw GFTs
+                self.stab.X + self.stab.V/2, self.stab.X - self.stab.V/2 ) #because the position of the displacement is half the distance btw GFTs
             dst = cv2.warpAffine(
                 self.stab.vis,
                 transformation_rigid_matrix,
                 (self.stab.Lvis,
                  self.stab.Hvis))
             self.vis = dst
         print('-------------Stabilization End -------------')
@@ -1421,7 +1421,9 @@
 #        if filename is None:
 #            filename='Goof_features_positions_from_frame'+ str(self.vec[0]) + 'to' + str(self.vec[-2]) + '_with_shift_'+str(self.paramVecTime['shift'])
 #
 #        for samples in self.samplesMat:
 #           folderFrame=outFolder+'/'+filename+'/'+format(t,'04.0f')+'_to_'+format(t+self.paramVecTime['step']
 #           Files.mkdir2()
 #           cv2.imwrite()
+
+# %%
```

### Comparing `opyf-1.6/src/opyf/Files.py` & `opyf-1.7/src/opyf/Files.py`

 * *Files identical despite different names*

### Comparing `opyf-1.6/src/opyf/Filters.py` & `opyf-1.7/src/opyf/Filters.py`

 * *Files identical despite different names*

### Comparing `opyf-1.6/src/opyf/Interpolate.py` & `opyf-1.7/src/opyf/Interpolate.py`

 * *Files identical despite different names*

### Comparing `opyf-1.6/src/opyf/MeshesAndTime.py` & `opyf-1.7/src/opyf/MeshesAndTime.py`

 * *Files identical despite different names*

### Comparing `opyf-1.6/src/opyf/Render.py` & `opyf-1.7/src/opyf/Render.py`

 * *Files identical despite different names*

### Comparing `opyf-1.6/src/opyf/Track.py` & `opyf-1.7/src/opyf/Track.py`

 * *Files identical despite different names*

### Comparing `opyf-1.6/src/opyf/custom_cmap.py` & `opyf-1.7/src/opyf/custom_cmap.py`

 * *Files identical despite different names*

### Comparing `opyf-1.6/src/opyf.egg-info/PKG-INFO` & `opyf-1.7/src/opyf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opyf
-Version: 1.6
+Version: 1.7
 Summary: OpyFlow - Python package for Optical Flow measurements.
 Author-email: Gauthier Rousseau <gauthier.rousseau@gmail.com>
 Project-URL: Homepage, https://github.com/groussea/opyflow
 Project-URL: Bug Tracker, https://github.com/groussea/opyflow/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

