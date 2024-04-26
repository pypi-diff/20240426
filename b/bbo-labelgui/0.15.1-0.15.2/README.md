# Comparing `tmp/bbo-labelgui-0.15.1.tar.gz` & `tmp/bbo-labelgui-0.15.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbo-labelgui-0.15.1.tar", last modified: Thu Nov 23 11:57:24 2023, max compression
+gzip compressed data, was "bbo-labelgui-0.15.2.tar", last modified: Fri Apr 26 05:44:34 2024, max compression
```

## Comparing `bbo-labelgui-0.15.1.tar` & `bbo-labelgui-0.15.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-11-23 11:57:24.786353 bbo-labelgui-0.15.1/
--rw-rw-r--   0 voit     (86501) voit     (86501)    25313 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.1/LICENSE
--rw-rw-r--   0 voit     (86501) voit     (86501)     3569 2023-11-23 11:57:24.786353 bbo-labelgui-0.15.1/PKG-INFO
--rw-rw-r--   0 voit     (86501) voit     (86501)     2982 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.1/README.md
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-11-23 11:57:24.782353 bbo-labelgui-0.15.1/bbo_labelgui.egg-info/
--rw-rw-r--   0 voit     (86501) voit     (86501)     3569 2023-11-23 11:57:24.000000 bbo-labelgui-0.15.1/bbo_labelgui.egg-info/PKG-INFO
--rw-rw-r--   0 voit     (86501) voit     (86501)      410 2023-11-23 11:57:24.000000 bbo-labelgui-0.15.1/bbo_labelgui.egg-info/SOURCES.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)        1 2023-11-23 11:57:24.000000 bbo-labelgui-0.15.1/bbo_labelgui.egg-info/dependency_links.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)       73 2023-11-23 11:57:24.000000 bbo-labelgui-0.15.1/bbo_labelgui.egg-info/requires.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)        9 2023-11-23 11:57:24.000000 bbo-labelgui-0.15.1/bbo_labelgui.egg-info/top_level.txt
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-11-23 11:57:24.786353 bbo-labelgui-0.15.1/labelgui/
--rw-rw-r--   0 voit     (86501) voit     (86501)        0 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.1/labelgui/__init__.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     3135 2023-11-23 08:02:58.000000 bbo-labelgui-0.15.1/labelgui/__main__.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     2036 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.1/labelgui/check.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     1100 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.1/labelgui/config.py
--rw-rw-r--   0 voit     (86501) voit     (86501)      652 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.1/labelgui/helper_gui.py
--rw-rw-r--   0 voit     (86501) voit     (86501)      622 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.1/labelgui/helper_video.py
--rwxrwxr-x   0 voit     (86501) voit     (86501)    66155 2023-11-23 08:36:41.000000 bbo-labelgui-0.15.1/labelgui/labeling_gui.py
--rwxrwxr-x   0 voit     (86501) voit     (86501)     2147 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.1/labelgui/labeling_gui_cfg.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     4527 2023-11-23 11:12:37.000000 bbo-labelgui-0.15.1/labelgui/select_user.py
--rw-rw-r--   0 voit     (86501) voit     (86501)       38 2023-11-23 11:57:24.786353 bbo-labelgui-0.15.1/setup.cfg
--rw-rw-r--   0 voit     (86501) voit     (86501)     1073 2023-11-23 11:38:59.000000 bbo-labelgui-0.15.1/setup.py
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-04-26 05:44:34.437568 bbo-labelgui-0.15.2/
+-rw-rw-r--   0 voit     (86501) voit     (86501)    25313 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.2/LICENSE
+-rw-rw-r--   0 voit     (86501) voit     (86501)     3569 2024-04-26 05:44:34.437568 bbo-labelgui-0.15.2/PKG-INFO
+-rw-rw-r--   0 voit     (86501) voit     (86501)     2982 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.2/README.md
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-04-26 05:44:34.433568 bbo-labelgui-0.15.2/bbo_labelgui.egg-info/
+-rw-rw-r--   0 voit     (86501) voit     (86501)     3569 2024-04-26 05:44:34.000000 bbo-labelgui-0.15.2/bbo_labelgui.egg-info/PKG-INFO
+-rw-rw-r--   0 voit     (86501) voit     (86501)      410 2024-04-26 05:44:34.000000 bbo-labelgui-0.15.2/bbo_labelgui.egg-info/SOURCES.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)        1 2024-04-26 05:44:34.000000 bbo-labelgui-0.15.2/bbo_labelgui.egg-info/dependency_links.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)       73 2024-04-26 05:44:34.000000 bbo-labelgui-0.15.2/bbo_labelgui.egg-info/requires.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)        9 2024-04-26 05:44:34.000000 bbo-labelgui-0.15.2/bbo_labelgui.egg-info/top_level.txt
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-04-26 05:44:34.437568 bbo-labelgui-0.15.2/labelgui/
+-rw-rw-r--   0 voit     (86501) voit     (86501)        0 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.2/labelgui/__init__.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     3135 2023-11-23 08:02:58.000000 bbo-labelgui-0.15.2/labelgui/__main__.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     2036 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.2/labelgui/check.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     1100 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.2/labelgui/config.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)      652 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.2/labelgui/helper_gui.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)      622 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.2/labelgui/helper_video.py
+-rwxrwxr-x   0 voit     (86501) voit     (86501)    67604 2024-04-26 05:44:22.000000 bbo-labelgui-0.15.2/labelgui/labeling_gui.py
+-rwxrwxr-x   0 voit     (86501) voit     (86501)     2147 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.2/labelgui/labeling_gui_cfg.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     4527 2023-11-23 11:12:37.000000 bbo-labelgui-0.15.2/labelgui/select_user.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)       38 2024-04-26 05:44:34.437568 bbo-labelgui-0.15.2/setup.cfg
+-rw-rw-r--   0 voit     (86501) voit     (86501)     1073 2024-04-26 05:44:31.000000 bbo-labelgui-0.15.2/setup.py
```

### Comparing `bbo-labelgui-0.15.1/LICENSE` & `bbo-labelgui-0.15.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bbo-labelgui-0.15.1/PKG-INFO` & `bbo-labelgui-0.15.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbo-labelgui
-Version: 0.15.1
+Version: 0.15.2
 Summary: GUI for guided data labeling
 Home-page: https://github.com/bbo-lab/acm-traingui
 Author: BBO-lab @ caesar
 Author-email: kay-michael.voit@caesar.de
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bbo-labelgui-0.15.1/README.md` & `bbo-labelgui-0.15.2/README.md`

 * *Files identical despite different names*

### Comparing `bbo-labelgui-0.15.1/bbo_labelgui.egg-info/PKG-INFO` & `bbo-labelgui-0.15.2/bbo_labelgui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbo-labelgui
-Version: 0.15.1
+Version: 0.15.2
 Summary: GUI for guided data labeling
 Home-page: https://github.com/bbo-lab/acm-traingui
 Author: BBO-lab @ caesar
 Author-email: kay-michael.voit@caesar.de
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bbo-labelgui-0.15.1/labelgui/__main__.py` & `bbo-labelgui-0.15.2/labelgui/__main__.py`

 * *Files identical despite different names*

### Comparing `bbo-labelgui-0.15.1/labelgui/check.py` & `bbo-labelgui-0.15.2/labelgui/check.py`

 * *Files identical despite different names*

### Comparing `bbo-labelgui-0.15.1/labelgui/config.py` & `bbo-labelgui-0.15.2/labelgui/config.py`

 * *Files identical despite different names*

### Comparing `bbo-labelgui-0.15.1/labelgui/helper_gui.py` & `bbo-labelgui-0.15.2/labelgui/helper_gui.py`

 * *Files identical despite different names*

### Comparing `bbo-labelgui-0.15.1/labelgui/helper_video.py` & `bbo-labelgui-0.15.2/labelgui/helper_video.py`

 * *Files identical despite different names*

### Comparing `bbo-labelgui-0.15.1/labelgui/labeling_gui.py` & `bbo-labelgui-0.15.2/labelgui/labeling_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         if not self.master:
             self.init_assistant_folders(standard_recording_folder)
             self.init_autosave()
             archive_cfg(self.file_config, self.standardLabelsFolder )
             self.restore_last_pose_idx()
 
         if self.cfg['autoLoad']:
-            rec_file_names = sorted(
+            rec_file_names = (
                 [(standard_recording_folder / i).expanduser().resolve() for i in self.cfg['standardRecordingFileNames']]
             )
             self.load_recordings_from_names(rec_file_names)
 
             self.load_calibrations()
             self.load_origin()
             # self.load_model()
@@ -475,18 +475,14 @@
 
     def plot2d_plot(self, ax, i_cam):
         self.plot2d_update_image(ax, i_cam)
         self.plot2d_draw_labels(ax)
 
     def plot2d_update_image(self, ax, i_cam):
         reader = self.cameras[i_cam]["reader"]
-        # Only subsequent frames seem to come up correctly
-        # TODO: Implement only loading the previous frame if it wasnt loaded directly before?
-        if self.pose_idx > 0:
-            img = reader.get_data(self.pose_idx - 1)
         img = reader.get_data(self.pose_idx)
         if self.controls['plots']['image2d'] is None:
             self.controls['plots']['image2d'] = ax.imshow(img,
                                                           aspect=1,
                                                           cmap='gray',
                                                           vmin=self.vmin,
                                                           vmax=self.vmax)
@@ -609,15 +605,14 @@
 
     def plot2d_click(self, event):
         if not (get_button_status(self.controls['buttons']['zoom']) or
                 get_button_status(self.controls['buttons']['pan'])):
             ax = event.inaxes
 
             # Initialize array
-            cam_idx = self.camera_idx
             fr_idx = self.get_pose_idx()
             label_name = self.get_current_label()
             cam_idx = self.camera_idx
 
             modifiers = QApplication.keyboardModifiers()
 
             if ax is not None:
@@ -661,26 +656,20 @@
                     self.list_labels_select()
 
                 # Left mouse - create
                 elif event.button == 1:
                     x = event.xdata
                     y = event.ydata
                     if (x is not None) and (y is not None):
-                        data_shape = (len(self.cameras), 2)
-                        self.initialize_field(label_name, fr_idx, data_shape)
-
-                        if self.user not in self.labels["labeler_list"]:
-                            self.labels["labeler_list"].append(self.user)
-                        self.labels['labeler'][label_name][fr_idx][cam_idx] = self.labels["labeler_list"].index(
-                            self.user)
-
-                        self.labels['point_times'][label_name][fr_idx][cam_idx] = time.time()
-
-                        coords = np.array([x, y], dtype=np.float64)
-                        self.labels['labels'][label_name][fr_idx][cam_idx] = coords
+                        modifiers = QApplication.keyboardModifiers()
+                        nextframe = self.get_pose_idx() + self.dFrame
+                        if modifiers == QtCore.Qt.AltModifier:
+                            self.autolabel(fr_idx, coords=[x,y], radius=5)
+                        else:
+                            self.add_label([x,y], label_name, cam_idx, fr_idx)
 
                         self.plot2d_update()
                         self.sketch_update()
 
                 # Right mouse - delete
                 elif event.button == 3:
                     if self.user not in self.labels["labeler_list"]:
@@ -690,14 +679,26 @@
                     # For synchronisation, deletion time and user must be recorded
                     self.labels['point_times'][label_name][fr_idx][cam_idx] = time.time()
                     self.labels['labeler'][label_name][fr_idx][cam_idx] = self.labels["labeler_list"].index(self.user)
 
                     self.plot2d_update()
                     self.sketch_update()
 
+    def add_label(self, coords, label_name, cam_idx, fr_idx):
+        data_shape = (len(self.cameras), 2)
+        self.initialize_field(label_name, fr_idx, data_shape)
+        if self.user not in self.labels["labeler_list"]:
+            self.labels["labeler_list"].append(self.user)
+        self.labels['labeler'][label_name][fr_idx][cam_idx] = self.labels["labeler_list"].index(
+            self.user)
+        self.labels['point_times'][label_name][fr_idx][cam_idx] = time.time()
+        coords = np.array(coords, dtype=np.float64)
+        self.labels['labels'][label_name][fr_idx][cam_idx] = coords
+
+
     def initialize_field(self, label_name, frame_idx, data_shape):
         if label_name not in self.labels['labels']:
             self.labels['labels'][label_name] = {}
         if label_name not in self.labels['point_times']:
             self.labels['point_times'][label_name] = {}
         if label_name not in self.labels['labeler']:
             self.labels['labeler'][label_name] = {}
@@ -1392,18 +1393,47 @@
         elif next_label_index < 0:
             next_label_index = np.size(label_keys) - 1
         self.controls['lists']['labels'].setCurrentRow(next_label_index)
         self.list_labels_select()
         self.controls['buttons']['next_label'].clearFocus()
 
     def button_next_press(self):
-        self.set_pose_idx(self.get_pose_idx() + self.dFrame)
+        modifiers = QApplication.keyboardModifiers()
+        nextframe = self.get_pose_idx() + self.dFrame
+        if modifiers == QtCore.Qt.AltModifier:
+            self.autolabel(nextframe)
+        self.set_pose_idx(nextframe)
 
     def button_previous_press(self):
-        self.set_pose_idx(self.get_pose_idx() - self.dFrame)
+        modifiers = QApplication.keyboardModifiers()
+        nextframe = self.get_pose_idx() - self.dFrame
+        if modifiers == QtCore.Qt.AltModifier:
+            self.autolabel(nextframe)
+        self.set_pose_idx(nextframe)
+
+    def autolabel(self, nextframe, radius=10, coords = None):
+        fr_idx = self.get_pose_idx()
+        label_name = self.get_current_label()
+        cam_idx = self.camera_idx
+        reader = self.cameras[cam_idx]["reader"]
+        img = np.linalg.norm(reader.get_data(nextframe), axis=2)
+        if coords is None:
+            coords = self.labels['labels'][label_name][fr_idx][cam_idx]
+            other = self.labels['labels'][label_name][2 * fr_idx - nextframe][cam_idx]
+            if other is not None:
+                coords = 2 * coords - other
+        import scipy
+        img = img.astype(np.uint16)
+        img = scipy.ndimage.convolve1d(img, [1, 2, 3, 4, 3, 2, 1], axis=0)
+        img = scipy.ndimage.convolve1d(img, [1, 2, 3, 4, 3, 2, 1], axis=1)
+        xx, yy = np.meshgrid(np.arange(img.shape[1]), np.arange(img.shape[0]))
+        mask = (xx - coords[0]) ** 2 + (yy - coords[1]) ** 2 < radius ** 2
+        mindex = np.argmax(img * mask)
+        mindex = np.unravel_index(mindex, img.shape)
+        self.add_label((mindex[1], mindex[0]), label_name, cam_idx, nextframe)
 
     def field_current_pose_change(self):
         try:
             current_pose_idx = int(self.controls['fields']['current_pose'].text())
         except ValueError:
             print(f"Invalid pose {self.controls['fields']['current_pose'].text()}")
             return
```

### Comparing `bbo-labelgui-0.15.1/labelgui/labeling_gui_cfg.py` & `bbo-labelgui-0.15.2/labelgui/labeling_gui_cfg.py`

 * *Files identical despite different names*

### Comparing `bbo-labelgui-0.15.1/labelgui/select_user.py` & `bbo-labelgui-0.15.2/labelgui/select_user.py`

 * *Files identical despite different names*

### Comparing `bbo-labelgui-0.15.1/setup.py` & `bbo-labelgui-0.15.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="bbo-labelgui",
-    version="0.15.1",
+    version="0.15.2",
     description="GUI for guided data labeling",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bbo-lab/acm-traingui",
     author="BBO-lab @ caesar",
     author_email="kay-michael.voit@caesar.de",
     license="BSD",
```

