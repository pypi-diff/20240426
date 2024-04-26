# Comparing `tmp/hitips-1.0.4.tar.gz` & `tmp/hitips-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hitips-1.0.4.tar", last modified: Fri Mar 15 19:43:25 2024, max compression
+gzip compressed data, was "hitips-1.0.5.tar", last modified: Fri Apr 26 13:33:54 2024, max compression
```

## Comparing `hitips-1.0.4.tar` & `hitips-1.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 nciadmin  (1001) nciadmin  (1001)        0 2024-03-15 19:43:25.392267 hitips-1.0.4/
--rw-------   0 nciadmin  (1001) nciadmin  (1001)     1068 2023-11-24 15:47:05.000000 hitips-1.0.4/LICENSE.txt
--rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)     3843 2024-03-15 19:43:25.392267 hitips-1.0.4/PKG-INFO
--rw-------   0 nciadmin  (1001) nciadmin  (1001)     3138 2024-01-17 17:21:47.000000 hitips-1.0.4/README.md
-drwxrwxr-x   0 nciadmin  (1001) nciadmin  (1001)        0 2024-03-15 19:43:25.388267 hitips-1.0.4/hitips/
--rw-------   0 nciadmin  (1001) nciadmin  (1001)    50780 2024-03-15 19:28:27.000000 hitips-1.0.4/hitips/Analysis.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)    53624 2024-03-15 19:00:28.000000 hitips-1.0.4/hitips/AnalysisGUI.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)   105209 2024-03-11 19:01:37.000000 hitips-1.0.4/hitips/BatchAnalyzer.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)    21745 2024-03-11 02:56:27.000000 hitips-1.0.4/hitips/Cell_Spot_Tracker.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)    21332 2024-03-15 19:28:11.000000 hitips-1.0.4/hitips/Display.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)    19739 2023-10-27 02:34:12.000000 hitips-1.0.4/hitips/DisplayGUI.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)    27989 2024-03-11 02:56:27.000000 hitips-1.0.4/hitips/GUI_parameters.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)    12590 2023-10-30 16:18:43.000000 hitips-1.0.4/hitips/GridLayout.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)     7077 2024-03-11 02:56:27.000000 hitips-1.0.4/hitips/HiTIPS.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)    10429 2023-11-28 19:29:52.000000 hitips-1.0.4/hitips/IO_ResourceGUI.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)     2053 2023-11-24 18:39:45.000000 hitips-1.0.4/hitips/InputOutput.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)    21275 2024-03-11 02:16:59.000000 hitips-1.0.4/hitips/MetaData_Reader.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)   167336 2022-09-22 05:27:10.000000 hitips-1.0.4/hitips/Roboto-Bold.ttf
--rw-------   0 nciadmin  (1001) nciadmin  (1001)   167000 2022-09-22 05:27:10.000000 hitips-1.0.4/hitips/Roboto-Light.ttf
--rw-------   0 nciadmin  (1001) nciadmin  (1001)        0 2023-11-24 18:59:44.000000 hitips-1.0.4/hitips/__init__.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)     1773 2021-07-19 16:28:45.000000 hitips-1.0.4/hitips/cell_config.json
--rw-------   0 nciadmin  (1001) nciadmin  (1001)      451 2024-01-09 19:58:56.000000 hitips-1.0.4/hitips/logging_decorator.py
-drwxrwxr-x   0 nciadmin  (1001) nciadmin  (1001)        0 2024-03-15 19:43:25.392267 hitips-1.0.4/hitips.egg-info/
--rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)     3843 2024-03-15 19:43:25.000000 hitips-1.0.4/hitips.egg-info/PKG-INFO
--rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)      598 2024-03-15 19:43:25.000000 hitips-1.0.4/hitips.egg-info/SOURCES.txt
--rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)        1 2024-03-15 19:43:25.000000 hitips-1.0.4/hitips.egg-info/dependency_links.txt
--rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)       46 2024-03-15 19:43:25.000000 hitips-1.0.4/hitips.egg-info/entry_points.txt
--rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)      290 2024-03-15 19:43:25.000000 hitips-1.0.4/hitips.egg-info/requires.txt
--rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)        7 2024-03-15 19:43:25.000000 hitips-1.0.4/hitips.egg-info/top_level.txt
--rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)       38 2024-03-15 19:43:25.392267 hitips-1.0.4/setup.cfg
--rw-------   0 nciadmin  (1001) nciadmin  (1001)     1728 2024-03-15 19:42:50.000000 hitips-1.0.4/setup.py
+drwxrwxr-x   0 nciadmin  (1001) nciadmin  (1001)        0 2024-04-26 13:33:54.197115 hitips-1.0.5/
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)     1068 2023-11-24 15:47:05.000000 hitips-1.0.5/LICENSE.txt
+-rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)     3843 2024-04-26 13:33:54.197115 hitips-1.0.5/PKG-INFO
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)     3138 2024-01-17 17:21:47.000000 hitips-1.0.5/README.md
+drwxrwxr-x   0 nciadmin  (1001) nciadmin  (1001)        0 2024-04-26 13:33:54.197115 hitips-1.0.5/hitips/
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)    50780 2024-03-15 19:28:27.000000 hitips-1.0.5/hitips/Analysis.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)    53624 2024-03-15 19:00:28.000000 hitips-1.0.5/hitips/AnalysisGUI.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)   107390 2024-04-22 14:42:35.000000 hitips-1.0.5/hitips/BatchAnalyzer.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)    21745 2024-03-11 02:56:27.000000 hitips-1.0.5/hitips/Cell_Spot_Tracker.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)    21332 2024-03-15 19:28:11.000000 hitips-1.0.5/hitips/Display.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)    19739 2023-10-27 02:34:12.000000 hitips-1.0.5/hitips/DisplayGUI.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)    27989 2024-03-11 02:56:27.000000 hitips-1.0.5/hitips/GUI_parameters.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)    12590 2023-10-30 16:18:43.000000 hitips-1.0.5/hitips/GridLayout.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)     7077 2024-03-11 02:56:27.000000 hitips-1.0.5/hitips/HiTIPS.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)    10429 2023-11-28 19:29:52.000000 hitips-1.0.5/hitips/IO_ResourceGUI.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)     2053 2023-11-24 18:39:45.000000 hitips-1.0.5/hitips/InputOutput.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)    21275 2024-03-11 02:16:59.000000 hitips-1.0.5/hitips/MetaData_Reader.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)   167336 2022-09-22 05:27:10.000000 hitips-1.0.5/hitips/Roboto-Bold.ttf
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)   167000 2022-09-22 05:27:10.000000 hitips-1.0.5/hitips/Roboto-Light.ttf
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)        0 2023-11-24 18:59:44.000000 hitips-1.0.5/hitips/__init__.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)     1773 2021-07-19 16:28:45.000000 hitips-1.0.5/hitips/cell_config.json
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)      451 2024-01-09 19:58:56.000000 hitips-1.0.5/hitips/logging_decorator.py
+drwxrwxr-x   0 nciadmin  (1001) nciadmin  (1001)        0 2024-04-26 13:33:54.197115 hitips-1.0.5/hitips.egg-info/
+-rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)     3843 2024-04-26 13:33:53.000000 hitips-1.0.5/hitips.egg-info/PKG-INFO
+-rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)      598 2024-04-26 13:33:54.000000 hitips-1.0.5/hitips.egg-info/SOURCES.txt
+-rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)        1 2024-04-26 13:33:53.000000 hitips-1.0.5/hitips.egg-info/dependency_links.txt
+-rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)       46 2024-04-26 13:33:54.000000 hitips-1.0.5/hitips.egg-info/entry_points.txt
+-rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)      290 2024-04-26 13:33:54.000000 hitips-1.0.5/hitips.egg-info/requires.txt
+-rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)        7 2024-04-26 13:33:54.000000 hitips-1.0.5/hitips.egg-info/top_level.txt
+-rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)       38 2024-04-26 13:33:54.197115 hitips-1.0.5/setup.cfg
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)     1728 2024-04-26 13:33:42.000000 hitips-1.0.5/setup.py
```

### Comparing `hitips-1.0.4/LICENSE.txt` & `hitips-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hitips-1.0.4/PKG-INFO` & `hitips-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hitips
-Version: 1.0.4
+Version: 1.0.5
 Summary: HiTIPS: High-Throughput Image Processing Software for FISH data analysis
 Home-page: https://github.com/CBIIT/HiTIPS
 Author: keikhosravi
 Author-email: adib.keikhosravi@nih.gov
 License: MIT
 Keywords: high-throughput imaging FISH analysis cell segmentation signal quantification
 Platform: UNKNOWN
```

### Comparing `hitips-1.0.4/README.md` & `hitips-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `hitips-1.0.4/hitips/Analysis.py` & `hitips-1.0.5/hitips/Analysis.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.4/hitips/AnalysisGUI.py` & `hitips-1.0.5/hitips/AnalysisGUI.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.4/hitips/BatchAnalyzer.py` & `hitips-1.0.5/hitips/BatchAnalyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,14 +171,44 @@
                 process.start()
             for process in processes:
                 process.join()
 
     def update_params_dict(self, params_dict):
         self.params_dict=params_dict
         
+    def check_and_append_args(self, col, row, fov, t, func_args):
+        # Initialize a flag to indicate whether to append arguments
+        append_args = False
+
+        # Check for the nucleus information file if the corresponding checkbox is checked
+        if self.params_dict['NucInfoChkBox_check_status']:
+            cell_file_name = f"temp_cell_df_column_{col}_row_{row}_time_point_{t}_field_index_{fov}.pickle"
+            cell_file_path = os.path.join(self.temp_dir, cell_file_name)
+            # If the cell file is missing, set the flag to append arguments
+            if not os.path.isfile(cell_file_path):
+                append_args = True
+
+        # Check for spot files if their corresponding checkboxes are checked
+        for channel in range(1, 6):
+            channel_key = f'SpotCh{channel}CheckBox_status_check'
+            if self.params_dict[channel_key]:
+                spot_file_name = f"temp_spot_df_column_{col}_row_{row}_time_point_{t}_field_index_{fov}_channel_{channel}.pickle"
+                spot_file_path = os.path.join(self.temp_dir, spot_file_name)
+                # If any spot file is missing, set the flag to append arguments
+                if not os.path.isfile(spot_file_path):
+                    append_args = True
+                    # If one file is missing, no need to check further
+                    break
+
+        # Append the func_args if any file is missing and the corresponding checkbox is checked
+        if append_args:
+            func_args = np.append(func_args, np.array([col, row, fov, t]).reshape(1, 4), axis=0)
+
+        return func_args
+    
     @log_errors(logging.getLogger(__name__))            
     def ON_APPLYBUTTON(self, Meta_Data_df):
         """
         Begins the batch analysis process, including setting paths, reading metadata, and initiating analyses.
 
         Parameters:
 
@@ -247,15 +277,15 @@
                     for col in columns:
                         df_parallel = self.Meta_Data_df.loc[(self.Meta_Data_df['column'] == str(col)) & 
                                                               (self.Meta_Data_df['row'] == str(row)) & 
                                                               (self.Meta_Data_df['field_index'] == str(fov)) & 
                                                               (self.Meta_Data_df['time_point'] == str(t))]
                         if df_parallel.empty == False:
 
-                            func_args=np.append(func_args,np.array([col,row,fov,t]).reshape(1,4),axis=0)
+                            func_args = self.check_and_append_args( col, row, fov, t, func_args)
         if (os.name == 'nt'):
             # Windows does not fork, so it's safe to use the multiprocessing directly.
             self._process_jobs_posix(func_args, jobs_number)
         else:
             # For POSIX systems, ensure safe multiprocessing context
             self._process_jobs_posix(func_args, jobs_number)
 
@@ -323,14 +353,19 @@
                     if spots_loc.empty:
                         spot_channels=np.array([])
                     else:
                         spot_channels = spots_loc['channel'].unique()
         
                     for fov in fovs:
                         
+                        track_file_name = os.path.join(self.temp_dir , "tracks_df_column_"+str(col)+"_row_" + str(row) + "_field_index_" +str(fov)+'.pickle')
+                        if os.path.exists(track_file_name):
+                            continue
+                        
+                        
                         spot_images,spot_dict_stack = {}, {}
                         for chnl in spot_channels:
                             spot_images[str(int(chnl))] = []
                             
                         masks, lbl_imgs, nuc_imgs=[], [], []
                         for t in time_points:
                             self.df_checker = self.Meta_Data_df.loc[(self.Meta_Data_df['column'] == str(col)) & 
@@ -378,14 +413,15 @@
                             tracks_pd = Tracking.RUN_BTRACK(label_stack, self.params_dict)
                         
                         if self.params_dict['NucTrackingMethod_currentText'] == "DeepCell":
                         
                             tracks_pd = Tracking.deepcell_tracking(t_stack_nuc,label_stack,self.params_dict)
                         ###
                         tracks_pd_copy = tracks_pd.copy()
+                        
                         tracks_pd_copy=tracks_pd_copy.rename(columns={"t": "time_point", "x": "centroid-1", "y": "centroid-0", "ID": "cell_index"})
                         tracks_pd_copy["time_point"] = tracks_pd_copy["time_point"] + 1
                         tracks_pd_copy = tracks_pd_copy.astype({'centroid-0':'int', 'centroid-1':'int'})
                         self.cell_df =  self.cell_df.astype({'centroid-0':'int', 'centroid-1':'int', 'time_point':'int', 'cell_index':'int'})
                         field_cell_df = self.cell_df.loc[(self.cell_df['field_index'] == fov)&(self.cell_df['column'] == col)&(self.cell_df['row'] == row)]
                         for trck_ind, trck_row in tracks_pd_copy.iterrows():
 
@@ -480,15 +516,15 @@
                                 bin_img = Tracking.zero_pad_patch(masks_stack[int(pd_row['t']), min_row:max_row, min_col:max_col], desired_size=patch_size)
                                 mask_patches.append(bin_img)
                                 lbl_img, n_feat = label(bin_img)
                                 label_center = int(self.params_dict['patchsize_currentText']/2)
                                 lbl_img[lbl_img!=lbl_img[label_center,label_center]]=0
                                 bin_img = lbl_img>0
 
-                                bin_img = ndimage.binary_dilation(bin_img, structure=np.ones((12,12))>0).astype(bin_img.dtype)
+                                bin_img = ndimage.binary_dilation(bin_img, structure=np.ones((5,5))>0).astype(bin_img.dtype)
 
 
                                 img_patch[bin_img==0]=0
                                 row_shift, col_shift = ndimage.center_of_mass(bin_img)
                                 if (math.isnan(row_shift) or math.isnan(col_shift)):
                                     final_translation = np.array([0, 0])
                                 else:
@@ -784,14 +820,17 @@
                             large_rotcell_stack = self.normalize_stack(large_rotcell_stack)
                             imwrite(self.cell_level_file_name(cell_tracking_folder, 'single_track_images', 'aligned_nuclei_image', '.tif', col, row, fov, id_),
                                     np.rollaxis(large_rotcell_stack, 2, 0), imagej=True, metadata={'axes': 'TYX'})
                             
                             single_track_copy.to_csv(self.cell_level_file_name(cell_tracking_folder, 'single_track_tables', 'track_table', '.csv', col, row, fov, id_))  
                             print("saved track: "+ 'col' + str(col) + r'_row' + str(row) + r'_field' + str(fov) + r'_cell' + str(id_))
                             
+                        track_file_name = os.path.join(self.temp_dir , "tracks_df_column_"+str(col)+"_row_" + str(row) + "_field_index_" +str(fov)+'.pickle')
+                        tracks_pd_copy.to_pickle(track_file_name)
+                            
         self.SAVE_NUCLEI_INFORMATION(self.cell_df, columns, rows)
         self.spot_cell_index = True
         self.PROCESS_ALL_SPOT_CHANNELS()
         try:
             shutil.rmtree(self.temp_dir, onerror=self.remove_readonly)
         except Exception as e:
             print(f"Error removing {self.temp_dir}: {e}")
```

### Comparing `hitips-1.0.4/hitips/Cell_Spot_Tracker.py` & `hitips-1.0.5/hitips/Cell_Spot_Tracker.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.4/hitips/Display.py` & `hitips-1.0.5/hitips/Display.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.4/hitips/DisplayGUI.py` & `hitips-1.0.5/hitips/DisplayGUI.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.4/hitips/GUI_parameters.py` & `hitips-1.0.5/hitips/GUI_parameters.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.4/hitips/GridLayout.py` & `hitips-1.0.5/hitips/GridLayout.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.4/hitips/HiTIPS.py` & `hitips-1.0.5/hitips/HiTIPS.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.4/hitips/IO_ResourceGUI.py` & `hitips-1.0.5/hitips/IO_ResourceGUI.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.4/hitips/InputOutput.py` & `hitips-1.0.5/hitips/InputOutput.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.4/hitips/MetaData_Reader.py` & `hitips-1.0.5/hitips/MetaData_Reader.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.4/hitips/Roboto-Bold.ttf` & `hitips-1.0.5/hitips/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `hitips-1.0.4/hitips/Roboto-Light.ttf` & `hitips-1.0.5/hitips/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `hitips-1.0.4/hitips/cell_config.json` & `hitips-1.0.5/hitips/cell_config.json`

 * *Files identical despite different names*

### Comparing `hitips-1.0.4/hitips.egg-info/PKG-INFO` & `hitips-1.0.5/hitips.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hitips
-Version: 1.0.4
+Version: 1.0.5
 Summary: HiTIPS: High-Throughput Image Processing Software for FISH data analysis
 Home-page: https://github.com/CBIIT/HiTIPS
 Author: keikhosravi
 Author-email: adib.keikhosravi@nih.gov
 License: MIT
 Keywords: high-throughput imaging FISH analysis cell segmentation signal quantification
 Platform: UNKNOWN
```

### Comparing `hitips-1.0.4/hitips.egg-info/SOURCES.txt` & `hitips-1.0.5/hitips.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hitips-1.0.4/setup.py` & `hitips-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="hitips",
-    version="1.0.4",
+    version="1.0.5",
     author="keikhosravi",
     author_email="adib.keikhosravi@nih.gov",
     description="HiTIPS: High-Throughput Image Processing Software for FISH data analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CBIIT/HiTIPS",
     packages=find_packages(),
```

