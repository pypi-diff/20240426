# Comparing `tmp/track2p-0.5.1.tar.gz` & `tmp/track2p-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "track2p-0.5.1.tar", last modified: Tue Apr 16 15:14:01 2024, max compression
+gzip compressed data, was "track2p-0.5.2.tar", last modified: Fri Apr 26 14:38:32 2024, max compression
```

## Comparing `track2p-0.5.1.tar` & `track2p-0.5.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.009960 track2p-0.5.1/
--rw-r--r--   0 manonmantez   (501) staff       (20)    35149 2024-02-12 15:58:33.000000 track2p-0.5.1/LICENSE
--rw-r--r--   0 manonmantez   (501) staff       (20)     5073 2024-04-16 15:14:01.009626 track2p-0.5.1/PKG-INFO
--rw-r--r--   0 manonmantez   (501) staff       (20)     4646 2024-04-16 14:56:02.000000 track2p-0.5.1/README.md
--rw-r--r--   0 manonmantez   (501) staff       (20)       38 2024-04-16 15:14:01.010021 track2p-0.5.1/setup.cfg
--rw-r--r--   0 manonmantez   (501) staff       (20)      591 2024-04-16 15:13:05.000000 track2p-0.5.1/setup.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.000571 track2p-0.5.1/track2p/
--rw-r--r--   0 manonmantez   (501) staff       (20)       48 2024-02-22 09:56:18.000000 track2p-0.5.1/track2p/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      417 2024-02-21 12:46:39.000000 track2p-0.5.1/track2p/__main__.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.004501 track2p-0.5.1/track2p/gui/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1/track2p/gui/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     8413 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/cell_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     6456 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/fluo_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     2622 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/import_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    22751 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/main_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    15418 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/raster_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     8677 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/roi_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    10427 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/t2p_wd.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.005757 track2p-0.5.1/track2p/io/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1/track2p/io/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1726 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/io/loaders.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4238 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/io/s2p_loaders.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      773 2024-02-12 11:04:52.000000 track2p-0.5.1/track2p/io/savers.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      252 2024-01-09 12:56:24.000000 track2p-0.5.1/track2p/io/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.006576 track2p-0.5.1/track2p/match/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1/track2p/match/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4471 2024-01-09 12:56:24.000000 track2p-0.5.1/track2p/match/loop.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     5807 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/match/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.006976 track2p-0.5.1/track2p/ops/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1/track2p/ops/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     3348 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/ops/default.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.007909 track2p-0.5.1/track2p/plot/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1/track2p/plot/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    15443 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/plot/output.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      926 2024-02-12 11:04:52.000000 track2p-0.5.1/track2p/plot/progress.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1859 2024-02-12 11:04:52.000000 track2p-0.5.1/track2p/plot/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.009057 track2p-0.5.1/track2p/register/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1/track2p/register/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1348 2024-01-10 11:16:47.000000 track2p-0.5.1/track2p/register/elastix.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4054 2024-01-09 12:56:24.000000 track2p-0.5.1/track2p/register/loop.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     2345 2024-01-09 12:56:24.000000 track2p-0.5.1/track2p/register/utils.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     9791 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/t2p.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.001743 track2p-0.5.1/track2p.egg-info/
--rw-r--r--   0 manonmantez   (501) staff       (20)     5073 2024-04-16 15:14:00.000000 track2p-0.5.1/track2p.egg-info/PKG-INFO
--rw-r--r--   0 manonmantez   (501) staff       (20)      861 2024-04-16 15:14:00.000000 track2p-0.5.1/track2p.egg-info/SOURCES.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)        1 2024-04-16 15:14:00.000000 track2p-0.5.1/track2p.egg-info/dependency_links.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)      163 2024-04-16 15:14:00.000000 track2p-0.5.1/track2p.egg-info/requires.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)        8 2024-04-16 15:14:00.000000 track2p-0.5.1/track2p.egg-info/top_level.txt
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-26 14:38:32.100858 track2p-0.5.2/
+-rw-r--r--   0 manonmantez   (501) staff       (20)    35149 2024-02-12 15:58:33.000000 track2p-0.5.2/LICENSE
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5065 2024-04-26 14:38:32.100623 track2p-0.5.2/PKG-INFO
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4646 2024-04-16 14:56:02.000000 track2p-0.5.2/README.md
+-rw-r--r--   0 manonmantez   (501) staff       (20)       38 2024-04-26 14:38:32.100897 track2p-0.5.2/setup.cfg
+-rw-r--r--   0 manonmantez   (501) staff       (20)      583 2024-04-26 14:36:00.000000 track2p-0.5.2/setup.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-26 14:38:32.094027 track2p-0.5.2/track2p/
+-rw-r--r--   0 manonmantez   (501) staff       (20)       48 2024-02-22 09:56:18.000000 track2p-0.5.2/track2p/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      417 2024-02-21 12:46:39.000000 track2p-0.5.2/track2p/__main__.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-26 14:38:32.096680 track2p-0.5.2/track2p/gui/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.2/track2p/gui/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     8309 2024-04-26 11:45:50.000000 track2p-0.5.2/track2p/gui/cell_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     6456 2024-04-16 14:56:02.000000 track2p-0.5.2/track2p/gui/fluo_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     2063 2024-04-26 11:45:53.000000 track2p-0.5.2/track2p/gui/import_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    24060 2024-04-26 14:35:38.000000 track2p-0.5.2/track2p/gui/main_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    15418 2024-04-16 14:56:02.000000 track2p-0.5.2/track2p/gui/raster_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     8677 2024-04-16 14:56:02.000000 track2p-0.5.2/track2p/gui/roi_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    10642 2024-04-26 11:45:43.000000 track2p-0.5.2/track2p/gui/t2p_wd.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-26 14:38:32.097801 track2p-0.5.2/track2p/io/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.2/track2p/io/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1726 2024-04-26 14:30:23.000000 track2p-0.5.2/track2p/io/loaders.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4238 2024-04-16 14:56:02.000000 track2p-0.5.2/track2p/io/s2p_loaders.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      773 2024-02-12 11:04:52.000000 track2p-0.5.2/track2p/io/savers.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      252 2024-01-09 12:56:24.000000 track2p-0.5.2/track2p/io/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-26 14:38:32.098398 track2p-0.5.2/track2p/match/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.2/track2p/match/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4471 2024-01-09 12:56:24.000000 track2p-0.5.2/track2p/match/loop.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5807 2024-04-16 14:56:02.000000 track2p-0.5.2/track2p/match/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-26 14:38:32.098724 track2p-0.5.2/track2p/ops/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.2/track2p/ops/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     3385 2024-04-24 13:38:09.000000 track2p-0.5.2/track2p/ops/default.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-26 14:38:32.099492 track2p-0.5.2/track2p/plot/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.2/track2p/plot/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    15443 2024-04-16 14:56:02.000000 track2p-0.5.2/track2p/plot/output.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1008 2024-04-17 14:31:55.000000 track2p-0.5.2/track2p/plot/progress.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1905 2024-04-17 14:32:00.000000 track2p-0.5.2/track2p/plot/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-26 14:38:32.100242 track2p-0.5.2/track2p/register/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.2/track2p/register/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1348 2024-01-10 11:16:47.000000 track2p-0.5.2/track2p/register/elastix.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4054 2024-01-09 12:56:24.000000 track2p-0.5.2/track2p/register/loop.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     2391 2024-04-17 14:32:03.000000 track2p-0.5.2/track2p/register/utils.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     9781 2024-04-26 11:45:47.000000 track2p-0.5.2/track2p/t2p.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-26 14:38:32.094675 track2p-0.5.2/track2p.egg-info/
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5065 2024-04-26 14:38:32.000000 track2p-0.5.2/track2p.egg-info/PKG-INFO
+-rw-r--r--   0 manonmantez   (501) staff       (20)      861 2024-04-26 14:38:32.000000 track2p-0.5.2/track2p.egg-info/SOURCES.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)        1 2024-04-26 14:38:32.000000 track2p-0.5.2/track2p.egg-info/dependency_links.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)      155 2024-04-26 14:38:32.000000 track2p-0.5.2/track2p.egg-info/requires.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)        8 2024-04-26 14:38:32.000000 track2p-0.5.2/track2p.egg-info/top_level.txt
```

### Comparing `track2p-0.5.1/LICENSE` & `track2p-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/PKG-INFO` & `track2p-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: track2p
-Version: 0.5.1
+Version: 0.5.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.23.5
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: scikit-image==0.20.0
-Requires-Dist: itk-elastix==0.19.1
+Requires-Dist: itk==5.4rc2
 Requires-Dist: PyQt5==5.15.10
 Requires-Dist: qtpy==2.4.1
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: scikit-learn==1.4.0
 Requires-Dist: openTSNE==1.0.1
 Requires-Dist: pandas==1.5.3
```

### Comparing `track2p-0.5.1/README.md` & `track2p-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/setup.py` & `track2p-0.5.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='track2p',
-    version='0.5.1',
+    version='0.5.2',
     packages=find_packages(),
     install_requires=[
         'numpy==1.23.5',
         'matplotlib==3.5.3',
         'scikit-image==0.20.0',
-        'itk-elastix==0.19.1',
+        'itk==5.4rc2',
         'PyQt5==5.15.10',
         'qtpy==2.4.1',
         'tqdm==4.66.2',
         'scikit-learn==1.4.0',
         'openTSNE==1.0.1',
         'pandas==1.5.3',
         ],
```

### Comparing `track2p-0.5.1/track2p/gui/cell_plot.py` & `track2p-0.5.2/track2p/gui/cell_plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,52 +35,57 @@
         """It plots the mean image of the recording and the contours of the cells. It also sets the axis to be invisible and the title of the plot. It uses the colors attribute to color the contours of the cells. 
         the match_histograms function of the skimage library is used to match the histograms of the mean image of the recording and the last mean image of the recordings. . This is done to make the mean images of the recordings more comparable."""
         self.ax_image.clear()
         start = time.time()
         l_mean_img=self.all_ops[-1]['meanImg']
         match_mean_img=skimage.exposure.match_histograms(self.ops['meanImg'], l_mean_img, channel_axis=None)
         self.ax_image.imshow(match_mean_img, cmap='gray')
+        cell_count = 0
+        for cell in range(self.nb_cells):
+            bin_mask = np.zeros_like(self.ops['meanImg']) #create a binary mask with the same shape as the mean image of the recording
+            bin_mask[self.stat_t2p[cell]['ypix'], self.stat_t2p[cell]['xpix']] = 1
+            color_cell=self.colors[cell]
+            self.ax_image.contour(bin_mask, levels=[0.5], colors=[color_cell], linewidths=1) 
+            cell_count += 1
+        self.ax_image.axis('off')
+        print(f'time for plotting cells on mean image for recording : {time.time()-start}')
+        print(f'Total cells plotted: {cell_count}')
+        self.draw()
         
+    def plot_cells_remix(self,keys):
+        self.ax_image.clear()
+        start = time.time()
+        l_mean_img=self.all_ops[-1]['meanImg']
+        match_mean_img=skimage.exposure.match_histograms(self.ops['meanImg'], l_mean_img, channel_axis=None)
+        self.ax_image.imshow(match_mean_img, cmap='gray')
+        cell_count = 0
         for cell in range(self.nb_cells):
+            if cell in keys:
+                continue
             bin_mask = np.zeros_like(self.ops['meanImg']) #create a binary mask with the same shape as the mean image of the recording
             bin_mask[self.stat_t2p[cell]['ypix'], self.stat_t2p[cell]['xpix']] = 1
             color_cell=self.colors[cell]
-           
             self.ax_image.contour(bin_mask, levels=[0.5], colors=[color_cell], linewidths=1) 
+            cell_count += 1
         self.ax_image.axis('off')
         print(f'time for plotting cells on mean image for recording : {time.time()-start}')
+        print(f'Total cells plotted: {cell_count}')
         self.draw()
         
+        
            
-    def underline_cell_remix(self,selected_cell_index,vector_curation):
+    def underline_cell_remix(self,colors):
         
         for cell in range(self.nb_cells):
-            if cell == selected_cell_index:
-                bin_mask = np.zeros_like(self.ops['meanImg'])
-                if vector_curation[selected_cell_index] in [3,4]:
-                    bin_mask[self.stat_t2p[cell]['ypix'], self.stat_t2p[cell]['xpix']] = 1 
-                    color_cell = (0.4, 0.4, 0.4)
-                    self.colors[cell]=(0.4, 0.4, 0.4)
-                   # color_cell = (0.0, 0.0, 0.0)
-                   # self.colors[cell]=(0.0, 0.0, 0.0) #update colors of plor and fluo  
-                    
-                if vector_curation[selected_cell_index]==2:
-                    bin_mask[self.stat_t2p[cell]['ypix'], self.stat_t2p[cell]['xpix']] = 1 
-                    color_cell =(0.78, 0.78, 0.78)
-                    self.colors[cell]=(0.78, 0.78, 0.78)
-                   # color_cell = (0.4, 0.4, 0.4)
-                   # self.colors[cell]=(0.4, 0.4, 0.4) #update colors of plor and fluo 
-                if vector_curation[selected_cell_index]==1: 
-                    bin_mask[self.stat_t2p[cell]['ypix'], self.stat_t2p[cell]['xpix']] = 1 
-                    color_cell=self.initial_colors[cell]
-                    self.colors[cell]=self.initial_colors[cell] #update colors of plor and fluo  
-                self.ax_image.contour(bin_mask, levels=[0.5], colors=[color_cell], linewidths=1)
-                self.ax_image.contour(bin_mask, levels=[0.5], colors=[color_cell], linewidths=3) #update mean image 
-        self.draw() 
-    
+            bin_mask = np.zeros_like(self.ops['meanImg'])
+            bin_mask[self.stat_t2p[cell]['ypix'], self.stat_t2p[cell]['xpix']] = 1
+            color_cell=colors[cell]
+            self.ax_image.contour(bin_mask, levels=[0.5], colors=[color_cell], linewidths=1)
+        self.draw()
+
    
         
     def underline_cell(self,selected_cell_index):
         """It underlines the selected cell by increasing the linewidth of the contour of the cell"""
         for cell in range(self.nb_cells):
             if cell == selected_cell_index:
                 bin_mask = np.zeros_like(self.ops['meanImg'])
```

### Comparing `track2p-0.5.1/track2p/gui/fluo_plot.py` & `track2p-0.5.2/track2p/gui/fluo_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/gui/import_wd.py` & `track2p-0.5.2/track2p/gui/import_wd.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,33 +28,26 @@
             
             plane_label= QLabel("Choose the plane to analyze:")
             self.textbox = QLineEdit(self)
             self.textbox.setFixedWidth(50) 
             self.textbox.setText('0')
             layout.addRow(plane_label,self.textbox)
             
-            label_combobox= QLabel("not_cell_count_over_days :")
-            self.comboBox = QComboBox(self)
-            layout.addRow(label_combobox,self.comboBox)
-            
             label_run= QLabel("Run the analysis:")
             self.runButton = QPushButton("Run", self)
             self.runButton.clicked.connect(self.run)
             layout.addRow(label_run,self.runButton)
             
                 
         def saveDirectory(self):
             savedirectory= QFileDialog.getExistingDirectory(self, "Select Directory")
             if savedirectory:
                 self.savedirectory=savedirectory
                 self.savedirectoryLabel.setText(f'{self.savedirectory}')
-                track_ops_dict = np.load(os.path.join(self.savedirectory, "track2p", "track_ops.npy"), allow_pickle=True).item()
-                track_ops = SimpleNamespace(**track_ops_dict)
-                for i in range(len(track_ops.all_ds_path)):
-                    self.comboBox.addItem(str(i + 1))
+               
+
                 
                 
         def run(self):
             self.storedPlane = int(self.textbox.text())
-            comboBoxResult = int(self.comboBox.currentText())
-            self.main_window.loadFiles(self.savedirectory, plane=self.storedPlane, combobox_value=comboBoxResult)
+            self.main_window.loadFiles(self.savedirectory, plane=self.storedPlane)
```

### Comparing `track2p-0.5.1/track2p/gui/main_wd.py` & `track2p-0.5.2/track2p/gui/main_wd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from PyQt5.QtCore import Qt
 import os
 import numpy as np
-from PyQt5.QtWidgets import QApplication, QTabWidget, QVBoxLayout, QWidget, QSplitter, QHBoxLayout, QFrame, QFrame,  QMenuBar,QToolBar,QMainWindow,QMenu,QAction,QToolButton,QSpinBox,QPushButton,QLabel
+from PyQt5.QtWidgets import QApplication, QTabWidget, QVBoxLayout, QWidget, QSplitter, QHBoxLayout, QFrame, QFrame,  QMenuBar,QToolBar,QMainWindow,QMenu,QAction,QToolButton,QSpinBox,QPushButton,QLabel,QLineEdit,QSizePolicy,QSpacerItem
 from PyQt5.QtCore import Qt
 import matplotlib.colors as mcolors
 import random
 from types import SimpleNamespace
 from track2p.gui.cell_plot import CellPlotWidget
 from track2p.gui.fluo_plot import FluorescencePlotWidget
 from track2p.gui.roi_plot import ZoomPlotWidget
@@ -138,108 +138,127 @@
         layout = QHBoxLayout()
         
         self.spin_box=QSpinBox()
         self.spin_box.setFixedWidth(100)
         self.spin_box.valueChanged.connect(self.spin_box_changed)
         
         self.status=QLabel("status: ")
+        self.status.setFixedWidth(50)
         self.status_value=QLabel()
+        self.status_value.setFixedWidth(30)
       
         cross_button =QPushButton('✖️')
+        cross_button.setFixedSize(20,20)
         cross_button.clicked.connect(self.cross_button_clicked)
         #cross_button.clicked.connect(self.cross_button_clicked)
         
         validate_button = QPushButton('✓')
+        validate_button.setFixedSize(20,20)
         validate_button.clicked.connect(self.validate_button_clicked)
         
-        save_t2p_color=QPushButton('Save curation')
-        save_t2p_color.clicked.connect(self.save_t2p_color)
-        
+        self.grey_cells_label=QLabel("Select the minimum number of days the cell must be present :")
+        self.grey_cells_value=QLineEdit()
+        self.grey_cells_value.setFixedWidth(50)
+        self.grey_cells_value.returnPressed.connect(self.underline_cell_according_manually_curation)
+        
+        reset=QPushButton('Reset')
+        reset.setFixedSize(50,20)
+        reset.clicked.connect(self.init_plot_cell)
+        
+        #save_t2p_parameter=QPushButton('Save curation')
+        #save_t2p_parameter.clicked.connect(self.save_t2p_parameter)
+        spacer = QSpacerItem(1200, 20, QSizePolicy.Expanding, QSizePolicy.Fixed)
+
+
         layout.addWidget(self.spin_box)
         layout.addWidget(self.status)
         layout.addWidget(self.status_value)
         layout.addWidget(cross_button)
         layout.addWidget(validate_button)
-        layout.addWidget(save_t2p_color)
+        layout.addItem(spacer)
+        layout.addWidget(self.grey_cells_label)
+        layout.addWidget(self.grey_cells_value)
+        layout.addWidget(reset)
+        
+        #layout.addWidget(save_t2p_parameter)
         
         status_widget.setLayout(layout)
         statusBar.addWidget(status_widget)
       
 
         QApplication.setStyle('Cleanlooks')
         self.setWindowTitle("track2p GUI")
         self.show()
         
-    def save_t2p_color(self):
+    def save_t2p_parameter(self):
         track_ops_dict = np.load(os.path.join(self.t2p_folder_path, "track2p", "track_ops.npy"), allow_pickle=True).item() #load track2p dict
-        track_ops_dict['colors'] = self.new_colors #update and save track2p.colors for cells that were curated manually 
         track_ops_dict['vector_curation']=self.vector_curation_t2p #update and save track2p.vector_curation for cells that were curated manually 
         track_ops_dict['curated_cells']=self.curated_cells #update and save track2p.curated_cells for cells that were curated manually
         np.save(os.path.join(self.t2p_folder_path, "track2p", "track_ops.npy"), track_ops_dict) #save track2p dict 
         
-            # Create a table with cell number and status
-        data = {'Cell Number': list(self.vector_curation_t2p.keys()), 'Status': list(self.vector_curation_t2p.values())}
-        df = pd.DataFrame(data)
-        print(df)
-        
-        df.to_csv(os.path.join(self.t2p_folder_path, "track2p",'cell_status.csv'), index=False, sep=';')
+        status_suite2p = [f'{value} / {len(self.t2p_match_mat_allday[1])}' for value in self.num_ones.values()]
+        data = {'cell_number': list(self.vector_curation_t2p.keys()), 'status_t2p': list(self.vector_curation_t2p.values()), 'status_s2p': status_suite2p}
+        self.df = pd.DataFrame(data)
+
+        nb_cells= f'number of cells present on all days : {len(self.t2p_match_mat_allday)}'  
+        is_cell_prob=f'probability used in track2p algorithm : {self.iscell_thr}'
+        num_zeros_t2p = f'number of cells deleted in track2p : {len([value for value in self.vector_curation_t2p.values() if value == 0])}'
+        
+        info_string = ""
+        for day in range(len(self.all_iscell_t2p) + 1):
+            num_values_equal_to_day = len([value for value in self.num_ones.values() if value == day])
+            info_string += f"Number of cells present {day} day out of {len(self.all_iscell_t2p)}: {num_values_equal_to_day}\n"
+            keys_for_day = [key for key, value in self.num_ones.items() if value == day]
+            info_string += f'Indexes: {keys_for_day}\n\n'
+    
+
+        with open(os.path.join(self.t2p_folder_path, "track2p",'info.txt'), 'w') as f:
+            f.write(nb_cells + "\n" + is_cell_prob + "\n\n" +info_string +"\n\n" + num_zeros_t2p +"\n\n" + self.df.to_string(index=False) + "\n")
         
+
     def spin_box_changed(self):
         current_value = self.spin_box.value() #selected ROI 
         value=self.vector_curation_t2p[current_value] #status of ROI 
         self.status_value.setText(f"{value}") # display the status 
         self.update_selection(current_value) #update 
     
     def cross_button_clicked(self):
-        if self.vector_curation_t2p[self.spin_box.value()] in [1, 2, 3]:
-            self.vector_curation_t2p[self.spin_box.value()]= 4
+        if self.vector_curation_t2p[self.spin_box.value()] ==1:
+            self.vector_curation_t2p[self.spin_box.value()]= 0
+            self.colors[self.spin_box.value()] =(0.78, 0.78, 0.78)
         self.curated_cells.append(self.spin_box.value()) #add the cells to curated cells list
-           
-            
-        #if self.vector_curation_t2p[self.spin_box.value()]==0:
-          #  self.vector_curation_t2p[self.spin_box.value()]= 4
-            #self.status_value.setText(f"Status: {self.vector_curation_t2p[self.spin_box.value()]}") 
-       # if self.vector_curation_t2p[self.spin_box.value()]==1:
-        #    self.vector_curation_t2p[self.spin_box.value()]= 4
-            #self.status_value.setText(f"Status: {self.vector_curation_t2p[self.spin_box.value()]}")
-        self.update_remix(self.spin_box.value())
+        for i in range(self.tabs.count()): 
+            tab_widget = self.tabs.widget(i)
+            cell_object = tab_widget.findChild(CellPlotWidget)
+            cell_object.colors= self.colors
+            cell_object.plot_cells()
+        self.save_t2p_parameter()
+        self.update_selection(self.spin_box.value())
     
     def validate_button_clicked(self):
-        if self.vector_curation_t2p[self.spin_box.value()] in [2, 3, 4]:
+        if self.vector_curation_t2p[self.spin_box.value()] ==0:
             self.vector_curation_t2p[self.spin_box.value()]= 1
+            self.colors[self.spin_box.value()] =self.colors_copy[self.spin_box.value()]
         self.curated_cells.append(self.spin_box.value())
-            #self.status_value.setText(f"Status: {self.vector_curation_t2p[self.spin_box.value()]}")
-            
-        #if self.vector_curation_t2p[self.spin_box.value()]==0:
-            #self.new_vector_curation[self.spin_box.value()]=1 !!!!!!!!!!!!!!!!!!!!!!
-           # self.vector_curation_t2p[self.spin_box.value()]= 1 
-            #self.status_value.setText(f"Status: {self.vector_curation_t2p[self.spin_box.value()]}")
-        #if self.vector_curation_t2p[self.spin_box.value()]== 2:
-         #   self.vector_curation_t2p[self.spin_box.value()]= 1 
-            #self.status_value.setText(f"Status: {self.vector_curation_t2p[self.spin_box.value()]}")
-        self.update_remix(self.spin_box.value())
+        for i in range(self.tabs.count()): 
+            tab_widget = self.tabs.widget(i)
+            cell_object = tab_widget.findChild(CellPlotWidget)
+            cell_object.colors= self.colors
+            cell_object.plot_cells()
+        self.save_t2p_parameter()
+        self.update_selection(self.spin_box.value())
         
     def update_remix(self,index):
-        #update and save the changes for track2p (new_colors is used for track2p.colors in save_t2p_color)
-        self.status_value.setText(f"Status: {self.vector_curation_t2p[index]}") 
-        if self.vector_curation_t2p[index]==2:
-            #self.new_colors[index]=(0.4, 0.4, 0.4)#grey
-            self.new_colors[index]=(0.78, 0.78, 0.78) #white
-        if self.vector_curation_t2p[index] in [3,4]:
-            self.new_colors[index]=(0.4, 0.4, 0.4)
-            #self.new_colors[index]=(0,0,0)
-        if self.vector_curation_t2p[index]==1: 
-            self.new_colors[index]=self.init_colors[index]
+        #update and save the changes for track2p (new_colors is used for track2p.colors in save_t2p_parameter)
+        self.status_value.setText(f"{self.vector_curation_t2p[index]}") 
         current_tab_index = self.tabs.currentIndex()
         current_tab_widget = self.tabs.widget(current_tab_index)
-        cell_plot = current_tab_widget.findChild(CellPlotWidget)
-        
-             
+        cell_plot = current_tab_widget.findChild(CellPlotWidget)         
         if cell_plot:
-            cell_plot.underline_cell_remix(index,vector_curation=self.vector_curation_t2p)
+            cell_plot.underline_cell(index)
             
                
     def init_cell(self,index):
         """it displays the first cell of the t2p_match_mat_allday and its fluorescence and zooms across days. It is called when the application is opened.
         An instance of FluorescencePlotWidget and an instance of ZoomPlotWidget are created and added to attributes of the MainWindow class. """
         tab_widget = self.tabs.widget(0)
         cell_object = tab_widget.findChild(CellPlotWidget) #It finds the instance of the CellPlotWidget class in the first tab of the QTabWidget
@@ -255,27 +274,31 @@
                                             all_stat_t2p=self.all_stat_t2p,
                                             colors=self.colors,
                                             all_iscell_t2p=self.all_iscell_t2p,
                                             t2p_match_mat_allday=self.t2p_match_mat_allday,track_ops=self.track_ops)
             self.bottom_layout.addWidget(self.roi_plot)
         self.fluorescence_plot.display_all_f_t2p(index)
         self.roi_plot.display_zooms(index)
-        self.status_value.setText(f"Status: {self.vector_curation_t2p[self.spin_box.value()]}") #once files are loaded 
+        self.status_value.setText(f"{self.vector_curation_t2p[self.spin_box.value()]}") #once files are loaded 
 
     
-    def loadFiles(self, t2p_folder_path, plane, combobox_value):
+    def loadFiles(self, t2p_folder_path, plane):
         self.t2p_folder_path = t2p_folder_path
         if self.fluorescence_plot is not None:
             self.clearData()
         # load track2p outputs           
         t2p_match_mat = np.load(os.path.join(self.t2p_folder_path,"track2p" ,f"plane{plane}_match_mat.npy"), allow_pickle=True)
         self.t2p_match_mat_allday = t2p_match_mat[~np.any(t2p_match_mat == None, axis=1), :]
         track_ops_dict = np.load(os.path.join(self.t2p_folder_path, "track2p", "track_ops.npy"), allow_pickle=True).item()
         track_ops = SimpleNamespace(**track_ops_dict)
         self.track_ops = track_ops
+        self.iscell_thr=track_ops.iscell_thr
+        
+        
+        
         # process suite2p files 
         for (i, ds_path) in enumerate(track_ops.all_ds_path):
             ops = np.load(os.path.join(ds_path, 'suite2p', f'plane{plane}', 'ops.npy'), allow_pickle=True).item()
             stat = np.load(os.path.join(ds_path, 'suite2p', f'plane{plane}', 'stat.npy'), allow_pickle=True)
             f = np.load(os.path.join(ds_path, 'suite2p', f'plane{plane}', 'F.npy'), allow_pickle=True)
             iscell = np.load(os.path.join(ds_path, 'suite2p', f'plane{plane}', 'iscell.npy'), allow_pickle=True)
             
@@ -287,91 +310,110 @@
                     f_iscell = f[iscell[:, 1] > track_ops.iscell_thr, :] 
 
             stat_t2p = stat_iscell[self.t2p_match_mat_allday[:, i].astype(int)]
             f_t2p = f_iscell[self.t2p_match_mat_allday[:, i].astype(int), :]
             self.all_stat_t2p.append(stat_t2p)
             self.all_f_t2p.append(f_t2p)
             self.all_ops.append(ops)
-            self.all_iscell_t2p.append(iscell)            
+            self.all_iscell_t2p.append(iscell)
+                        
         # initializes or retrieve track2p dictionary parameters
         
         if track_ops.curated_cells is None:
-            self.curated_cells=[]
+            self.curated_cells=[] #initialize the list of curated cells
         else:
-            self.curated_cells=track_ops.curated_cells
+            self.curated_cells=track_ops.curated_cells 
             
         if track_ops.vector_curation is None:
             self.vector_curation_keys=np.arange(self.t2p_match_mat_allday.shape[0]) #number of cells (rows in matrix)
             self.vector_curation_values = np.ones_like(self.vector_curation_keys)
             self.vector_curation_t2p = dict(zip(self.vector_curation_keys, self.vector_curation_values))
 
-            #self.new_vector_curation=self.vector_curation_t2p.copy()
         else:
-            print('vector_curation is not None')
             self.vector_curation_t2p=track_ops.vector_curation
-            #self.new_vector_curation=track_ops.vector_curation.copy()
+
                     
         if track_ops.colors is None:
-            self.colors=self.generate_vibrant_colors(len(self.all_stat_t2p[0])) 
-            self.new_colors=self.colors.copy()
+            self.colors=self.generate_vibrant_colors(len(self.all_stat_t2p[0]))
+            track_ops_dict['colors'] = self.colors
+            np.save(os.path.join(self.t2p_folder_path, "track2p", "track_ops.npy"), track_ops_dict) 
+            self.track_ops = track_ops
+            
         else:
-            print('colors is not None')
             self.colors= track_ops.colors #affected by the choice of the user (grey cells) 
-            self.new_colors=track_ops.colors.copy() #will be use only to save the change of cells curated manually in the UI 
+            self.colors_copy=track_ops.colors.copy()#not affected by the choice of the user (grey cells)
+            
 
-        if track_ops.init_colors is None: # the first time that the colors are generated (track2p opens with UI)
-            self.init_colors=self.colors.copy()
-            track_ops_dict['init_colors'] = self.init_colors
-            np.save(os.path.join(self.t2p_folder_path, "track2p", "track_ops.npy"), track_ops_dict) 
-        else:   
-            self.init_colors=track_ops.init_colors
                 
         self.spin_box.setSuffix(f'/{len(self.t2p_match_mat_allday)-1}')
         self.spin_box.setMinimum(0)
         self.spin_box.setMaximum(len(self.t2p_match_mat_allday)-1) 
-            
+        
+        self.num_ones = {}  # Initialize as dictionary
+        
         for i, line in enumerate(self.t2p_match_mat_allday): #i= number of cells 
         
                 all_iscell_value=[]
+                
                 for j,index_match in enumerate(line): #j=number of days 
     
                     if track_ops.iscell_thr is None: #Manually curated 
                         iscell=self.all_iscell_t2p[j] # retrieve the iscell of day j 
                         indices_lignes_1 = np.where(iscell[:,0]==1)[0] # take the indices where the ROIs were considered as cells in suite2p
                         true_index=indices_lignes_1[index_match] # take the "true index" 
                         iscell_value=iscell[true_index,0] 
                         all_iscell_value.append(iscell_value)
-                    else: 
+                    else: #CHECK THIS PART
                         iscell=self.all_iscell_t2p[j]
                         indices_lignes_1= np.where(iscell[:,1]>track_ops.iscell_thr)[0] # take the indices where the ROIs have a probability greater than trackops.is_cell_thr
                         true_index=indices_lignes_1[index_match] # take the "true index" 
                         iscell_value=iscell[true_index,0] 
                         all_iscell_value.append(iscell_value)
-                if i not in self.curated_cells:      
-                    if all(value == 1.0 for value in all_iscell_value):
-                        self.colors[i]=self.colors[i] #colors
-                        self.vector_curation_t2p[i]=1      
-                    if all_iscell_value.count(0.0) != 0 and all_iscell_value.count(0.0) <= int(combobox_value):
-                        #self.colors[i]=(0.4, 0.4, 0.4) #grey
-                        self.colors[i]=(0.78, 0.78, 0.78) #white
-                        self.vector_curation_t2p[i]=2 
-                    if all_iscell_value.count(0.0) > int(combobox_value):
-                        self.colors[i]=(0.4, 0.4, 0.4)
-                        #self.colors[i]=(0.0, 0.0, 0.0) #noir
-                        self.vector_curation_t2p[i]= 3 
-                            
-        self.save_t2p_color()
+                        
+                self.num_ones[i] = all_iscell_value.count(1)
+   
+        self.save_t2p_parameter()
+        for i, line in enumerate(self.t2p_match_mat_allday): #i= number of cells 
+            if self.df.iloc[i, 1]==0:
+                self.colors[i] =(0.78, 0.78, 0.78)
         self.meanimage()
         self.init_cell(0)
-
- 
         
+  
         
-    
-    
+    def init_plot_cell(self):
+        self.colors= self.colors_copy.copy()
+        for i, line in enumerate(self.t2p_match_mat_allday): #i= number of cells 
+            if self.df.iloc[i, 1]==0:
+                self.colors[i] =(0.78, 0.78, 0.78)
+        for i in range(self.tabs.count()): 
+            tab_widget = self.tabs.widget(i)
+            cell_object = tab_widget.findChild(CellPlotWidget)
+            cell_object.colors= self.colors
+            cell_object.plot_cells()
+            
+        
+    def underline_cell_according_manually_curation(self):
+        match_mal_all_day_copie=self.t2p_match_mat_allday.copy()
+        all_keys=[]
+        for key,value in self.num_ones.items():
+            if value < int(self.grey_cells_value.text()):
+                match_mal_all_day_copie[key, :]=np.nan
+                all_keys.append(key)
+        match_mal_all_day_copie = match_mal_all_day_copie.astype(float)
+        # Now you can count the number of rows with at least one np.nan
+        num_rows_with_nan = np.any(np.isnan(match_mal_all_day_copie), axis=1).sum()
+        for i in range(self.tabs.count()): 
+            tab_widget = self.tabs.widget(i)
+            cell_object = tab_widget.findChild(CellPlotWidget)
+            cell_object.colors= self.colors
+            cell_object.plot_cells_remix(keys=all_keys)
+            
+            
+
     def clearData(self):
         self.all_f_t2p= []
         self.all_ops = []
         self.all_stat_t2p = []
         self.all_iscell_t2p = []
         self.colors = None
         self.t2p_match_mat_allday = None
@@ -410,15 +452,15 @@
             tab.setLayout(layout)
             self.tabs.addTab(tab, f"Day {i + 1}")
             cell_plot.cell_selected.connect(self.update_selection)
         
     def update_selection(self, selected_cell_index):
         self.selected_cell_index = selected_cell_index
         self.spin_box.setValue(selected_cell_index) 
-        self.status_value.setText(f"Status: {self.vector_curation_t2p[selected_cell_index]}")        
+        self.status_value.setText(f"{self.vector_curation_t2p[selected_cell_index]}")        
         #it removes the underline of the previsouly selected cell even if the tab is not visible (not the current tab)
         for i in range(self.tabs.count()): 
             tab_widget = self.tabs.widget(i)
             cell_object = tab_widget.findChild(CellPlotWidget)
             cell_object.remove_previous_underline()
         current_tab_index = self.tabs.currentIndex()
         current_tab_widget = self.tabs.widget(current_tab_index)
```

### Comparing `track2p-0.5.1/track2p/gui/raster_wd.py` & `track2p-0.5.2/track2p/gui/raster_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/gui/roi_plot.py` & `track2p-0.5.2/track2p/gui/roi_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/gui/t2p_wd.py` & `track2p-0.5.2/track2p/gui/t2p_wd.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,20 +119,27 @@
         def run(self):
             # Store the text in a variable
             self.is_cell= self.is_cell_thr.text()
             self.reg_channel= self.reg_chan.text()
             self.save_track2p_path= self.savedirectory
             self.stored_all_ds_path = []
             for i in range(self.paths_list.count()):
-                self.stored_all_ds_path.append(self.paths_list.item(i).data(Qt.UserRole))
+                item=self.paths_list.item(i).data(Qt.UserRole)
+                item_universel=item.replace("\\", "/")
+                #self.stored_all_ds_path.append(self.paths_list.item(i).data(Qt.UserRole))
+                self.stored_all_ds_path.append(item_universel)
             print("All parameters have been recorded ! The track2p algorithm is running...")
            # self.track_ops = DefaultTrackOps() #Initializes the self.track_ops object with the default parameters
             self.track_ops.all_ds_path= self.stored_all_ds_path
             #print(f'self.track_ops.all_ds_path : {self.track_ops.all_ds_path}')
-            self.track_ops.save_path = self.save_track2p_path
+            #print(self.save_path)
+            save_path=self.save_track2p_path
+            save_path=save_path.replace("\\", "/")
+            #self.track_ops.save_path = self.save_track2p_path
+            self.track_ops.save_path = save_path
             self.track_ops.reg_chan=int(self.reg_channel)
             if self.checkbox1.isChecked():
                 self.track_ops.iscell_thr=None
             if self.checkbox2.isChecked():
                 self.track_ops.iscell_thr=float(self.is_cell)
             if self.checkbox3.isChecked():
                 self.track_ops.save_in_s2p_format=True
@@ -140,20 +147,18 @@
             self.askQuestion()
 
         # In your askQuestion method:
         def askQuestion(self):
             reply = QMessageBox.question(self, "", "Run completed successfully!\nDo you want to launch the gui?", QMessageBox.Yes | QMessageBox.No, QMessageBox.No)
 
             if reply == QMessageBox.Yes:
-                dialog = ComboBoxDialog(self)
-                if dialog.exec_():
-                    plane, comboBoxResult = dialog.getResults()
-                    self.storedPlane = int(plane)
-                    comboBoxResult = int(comboBoxResult)
-                    self.main_window.loadFiles(self.save_track2p_path, plane=self.storedPlane, combobox_value=comboBoxResult)
+                text, ok = QInputDialog.getText(self, '', 'Enter your plane:')
+                if ok:
+                    self.storedPlane=int(text)
+                    self.main_window.loadFiles(self.save_track2p_path, plane=self.storedPlane)
                     self.close()
             if reply == QMessageBox.No:
                 pass
         
         def saveDirectory(self):
             savedirectory= QFileDialog.getExistingDirectory(self, "Select Directory")
             if savedirectory:
@@ -174,22 +179,22 @@
 
 
         def moveFileToBox(self):
             selectedItems = self.computer_file_list.selectedItems()
             for item in selectedItems:
                 self.computer_file_list.takeItem(self.computer_file_list.row(item))
                 self.paths_list.addItem(item)
-       
+     
 
         def moveFileToComputer(self):
             selectedItems = self.paths_list.selectedItems()
             for item in selectedItems:
                 self.paths_list.takeItem(self.paths_list.row(item))
                 self.computer_file_list.addItem(item)
-                
+    
 
 class ComboBoxDialog(QDialog):
     def __init__(self, parent=None):
         super(ComboBoxDialog, self).__init__(parent)
         self.parent=parent
         self.layout = QFormLayout(self)
```

### Comparing `track2p-0.5.1/track2p/io/loaders.py` & `track2p-0.5.2/track2p/io/loaders.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/io/s2p_loaders.py` & `track2p-0.5.2/track2p/io/s2p_loaders.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/io/savers.py` & `track2p-0.5.2/track2p/io/savers.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/match/loop.py` & `track2p-0.5.2/track2p/match/loop.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/match/utils.py` & `track2p-0.5.2/track2p/match/utils.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/ops/default.py` & `track2p-0.5.2/track2p/ops/default.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,25 +28,26 @@
 
         # plotting parameters
         self.win_size = 48 # window size for visualising matched ROIs across days (crop of mean image)
         self.sat_perc = 99.9 # percentile to saturate image at (only affects visualisation not the registration/matching)
         
         self.colors = None # save color after curation
         self.vector_curation=None #save the status of the ROIs after curation
-        self.init_colors=None #save the initial colors of the ROIs (before curation)
         self.curated_cells=None #save the index of the curated cells
         
         
         self.save_in_s2p_format = False # save the output in suite2p format (this is useful for downstream analysis with suite2p)
 
         # make the output directories when initialising the object
         
     def init_save_paths(self):
         self.save_path = os.path.join(self.save_path, 'track2p/')
+        self.save_path=self.save_path.replace("\\", "/")
         self.save_path_fig = os.path.join(self.save_path, 'fig/')
+        self.save_path_fig=self.save_path_fig.replace("\\", "/")
         make_dir(self.save_path)
         make_dir(self.save_path_fig)
 
 
     def to_dict(self):
         # this is useful for saving the object to avoid needing class definition in downstream analysis
         track_ops_dict = {}
```

### Comparing `track2p-0.5.1/track2p/plot/output.py` & `track2p-0.5.2/track2p/plot/output.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/plot/progress.py` & `track2p-0.5.2/track2p/plot/progress.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 from track2p.plot.utils import match_hist_all
 
 def plot_all_planes(all_ds_avg_ch, track_ops, sat_perc=99):
+    print("starting")
     nplanes = track_ops.nplanes
     fig, axs = plt.subplots(nplanes, len(track_ops.all_ds_path), figsize=(3 * len(track_ops.all_ds_path), 3 * nplanes), dpi=300)
     # add dummy dimension to axs if only one plane
     if nplanes==1:
         axs = np.expand_dims(axs, axis=0)
-    
+    print("starting match hist all")
     all_ds_avg_ch_matched = match_hist_all(all_ds_avg_ch)
 
 
     for i in range(nplanes):
         for j in range(len(track_ops.all_ds_path)):
             img = all_ds_avg_ch_matched[j][i]
             axs[i, j].imshow(img, cmap='gray', vmin=0, vmax=np.percentile(img, sat_perc))
             axs[i, j].set_title('Plane ' + str(i) + ' in dataset ' + str(j))
             axs[i, j].axis('off')
-            
+    print("done")
     plt.close(fig)
+    print("done")
+
```

### Comparing `track2p-0.5.1/track2p/plot/utils.py` & `track2p-0.5.2/track2p/plot/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 from skimage.exposure import match_histograms
 
 
 def match_hist_all(all_ds_avg_ch):
+    print("starting macth hist all function")
     ref = all_ds_avg_ch[0][0]
     all_ds_avg_ch_matched = []
     for ds_avg_ch in all_ds_avg_ch:
         ds_avg_ch_matched = []
         for i in range(len(ds_avg_ch)):
             ds_avg_ch_matched.append(match_histograms(ds_avg_ch[i], ref))
         all_ds_avg_ch_matched.append(ds_avg_ch_matched)
```

### Comparing `track2p-0.5.1/track2p/register/elastix.py` & `track2p-0.5.2/track2p/register/elastix.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/register/loop.py` & `track2p-0.5.2/track2p/register/loop.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/register/utils.py` & `track2p-0.5.2/track2p/register/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 
 def get_all_ds_img_for_reg(all_ds_avg_ch1, all_ds_avg_ch2, track_ops): # chooses which channel to use for registration and returns all_ref_img and all_mov_img (shifted by one day to always register to previous day)
+    print("starting get_all_ds_img_for_reg ")
     if track_ops.reg_chan==0:
         all_ds_avg = all_ds_avg_ch1
     elif track_ops.reg_chan==1:
         all_ds_avg = all_ds_avg_ch2
         print('WARNING: using anatomical channel for registration (this is not always available)')
 
     all_ds_ref_img = []
```

### Comparing `track2p-0.5.1/track2p/t2p.py` & `track2p-0.5.2/track2p/t2p.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,42 +27,57 @@
     # 3) Plot available planes for registration
     plot_all_planes(all_ds_avg_ch1, track_ops)
     if track_ops.nchannels==2:
         plot_all_planes(all_ds_avg_ch2, track_ops)
 
     # 4) do the actual registration based on chosen channel
     all_ds_ref_img, all_ds_mov_img = get_all_ds_img_for_reg(all_ds_avg_ch1, all_ds_avg_ch2, track_ops)
+
+    
+    #HERE 
+    
     all_ds_mov_img_reg, all_ds_reg_params = run_reg_loop(all_ds_ref_img, all_ds_mov_img, track_ops) # TODO: save basic parameters for each registration as feedback (e. g. ammoung of shift, rotation, etc.) for later plotting
+
     plot_reg_img_output(track_ops)
+    
 
     # 5) apply computed transorm to all ROIs
     all_ds_all_roi_ref, all_ds_all_roi_mov, all_ds_all_roi_reg, all_ds_roi_counter = reg_all_ds_all_roi(all_ds_reg_params, track_ops)
+ 
 
     # 6) optional: generate 'yellow intersection' plot (this is only needed for plotting below)
     all_ds_ref_reg_inters = get_all_ref_nonref_inters(all_ds_all_roi_ref, all_ds_all_roi_reg, track_ops)
+
     all_ds_ref_mov_inters = get_all_ref_nonref_inters(all_ds_all_roi_ref, all_ds_all_roi_mov, track_ops)
 
+
     track_ops.all_ds_ref_mov_inters = all_ds_ref_mov_inters
     track_ops.all_ds_ref_reg_inters = all_ds_ref_reg_inters
 
     # this line is very memory-intensive because of the ROIS (TODO: maybe instead of contours just plot RGB) (or somehow generate RGB image of contours (in the part before))
     if track_ops.show_roi_reg_output:
         plot_roi_reg_output(track_ops)
+      
 
     # 7) get optimal assignments for all pairs of recordings (first to last)
     all_ds_assign, all_ds_assign_thr, all_ds_thr_met, all_ds_thr = get_all_ds_assign(track_ops, all_ds_all_roi_ref, all_ds_all_roi_reg)
     plot_thr_met_hist(all_ds_thr_met, all_ds_thr, track_ops)
 
+
     # 8) get match matrices for all pairs of recordings (first to last)
     all_pl_match_mat = get_all_pl_match_mat(all_ds_all_roi_ref, all_ds_assign_thr, track_ops)
 
+
     # 9) save results
     save_track_ops(track_ops)
+
+    
     save_all_pl_match_mat(all_pl_match_mat, track_ops)
 
+
     # 10) save in suite2p format
     if track_ops.save_in_s2p_format:
         print('Saving in suite2p format...')
         save_in_s2p_format(track_ops)
         
     # 10) plot results
     print('Generating plots (this can take some time)...')
@@ -162,17 +177,15 @@
                     redcell_iscell_t2p.append(redcell_t2p)  
     
 
 
 # Define the output folder path
     #output_folderpath = "/Users/manonmantez/Desktop/el/fake_suite2p"
     output_folderpath=os.path.join(folderpath, "fake_suite2p")
-    print(track_ops.all_ds_path)
     last_elements = [os.path.basename(path) for path in track_ops.all_ds_path]
-    print(last_elements)
 # Save each element of each list to a .npy file
     for i, (stat_t2p, f_t2p, ops, iscell_t2p, fneu_t2p, spks_t2p) in enumerate(zip(all_stat_t2p, all_f_t2p, all_ops, all_iscell_t2p, fneu_iscell_t2p, spks_iscell_t2p)):
         subfolder_path = os.path.join(output_folderpath, last_elements[i])
         if not os.path.exists(subfolder_path):
             os.makedirs(subfolder_path)
     
         np.save(os.path.join(subfolder_path, f"stat.npy"), stat_t2p)
```

### Comparing `track2p-0.5.1/track2p.egg-info/PKG-INFO` & `track2p-0.5.2/track2p.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: track2p
-Version: 0.5.1
+Version: 0.5.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.23.5
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: scikit-image==0.20.0
-Requires-Dist: itk-elastix==0.19.1
+Requires-Dist: itk==5.4rc2
 Requires-Dist: PyQt5==5.15.10
 Requires-Dist: qtpy==2.4.1
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: scikit-learn==1.4.0
 Requires-Dist: openTSNE==1.0.1
 Requires-Dist: pandas==1.5.3
```

### Comparing `track2p-0.5.1/track2p.egg-info/SOURCES.txt` & `track2p-0.5.2/track2p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

