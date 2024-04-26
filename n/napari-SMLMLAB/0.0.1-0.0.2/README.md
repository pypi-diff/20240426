# Comparing `tmp/napari_smlmlab-0.0.1.tar.gz` & `tmp/napari_smlmlab-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\turnerp\PycharmProjects\napari-SMLMLAB\dist\.tmp-d8su2o74\napari_smlmlab-0.0.1.tar", last modified: Thu Apr 25 14:23:16 2024, max compression
+gzip compressed data, was "C:\Users\turnerp\PycharmProjects\napari-SMLMLAB\dist\.tmp-e_pi3v7d\napari_smlmlab-0.0.2.tar", last modified: Fri Apr 26 10:43:35 2024, max compression
```

## Comparing `napari_smlmlab-0.0.1.tar` & `napari_smlmlab-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 14:23:16.466172 napari_smlmlab-0.0.1/
--rw-rw-rw-   0        0        0     1515 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      101 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4645 2024-04-25 14:23:16.465175 napari_smlmlab-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2854 2024-04-25 14:22:00.000000 napari_smlmlab-0.0.1/README.md
--rw-rw-rw-   0        0        0     1243 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1819 2024-04-25 14:23:16.471159 napari_smlmlab-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-25 14:23:16.313579 napari_smlmlab-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-25 14:23:16.461185 napari_smlmlab-0.0.1/src/napari_SMLMLAB.egg-info/
--rw-rw-rw-   0        0        0     4645 2024-04-25 14:23:16.000000 napari_smlmlab-0.0.1/src/napari_SMLMLAB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      696 2024-04-25 14:23:16.000000 napari_smlmlab-0.0.1/src/napari_SMLMLAB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 14:23:16.000000 napari_smlmlab-0.0.1/src/napari_SMLMLAB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-25 14:23:16.000000 napari_smlmlab-0.0.1/src/napari_SMLMLAB.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      148 2024-04-25 14:23:16.000000 napari_smlmlab-0.0.1/src/napari_SMLMLAB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 14:23:16.000000 napari_smlmlab-0.0.1/src/napari_SMLMLAB.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-25 14:23:16.400348 napari_smlmlab-0.0.1/src/smlmlab/
--rw-rw-rw-   0        0        0      102 2024-04-25 13:50:35.000000 napari_smlmlab-0.0.1/src/smlmlab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:23:16.410322 napari_smlmlab-0.0.1/src/smlmlab/_tests/
--rw-rw-rw-   0        0        0        0 2024-04-24 10:36:50.000000 napari_smlmlab-0.0.1/src/smlmlab/_tests/__init__.py
--rw-rw-rw-   0        0        0     2176 2024-04-25 13:50:35.000000 napari_smlmlab-0.0.1/src/smlmlab/_tests/test_widget.py
--rw-rw-rw-   0        0        0     9272 2024-04-25 13:50:35.000000 napari_smlmlab-0.0.1/src/smlmlab/_widget.py
--rw-rw-rw-   0        0        0    33707 2024-04-25 13:35:12.000000 napari_smlmlab-0.0.1/src/smlmlab/gui.py
--rw-rw-rw-   0        0        0      502 2024-04-25 13:52:37.000000 napari_smlmlab-0.0.1/src/smlmlab/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-04-25 14:23:16.457196 napari_smlmlab-0.0.1/src/smlmlab/utils/
--rw-rw-rw-   0        0        0        0 2024-04-24 11:59:46.000000 napari_smlmlab-0.0.1/src/smlmlab/utils/__init__.py
--rw-rw-rw-   0        0        0     9793 2024-04-25 12:48:07.000000 napari_smlmlab-0.0.1/src/smlmlab/utils/compute_utils.py
--rw-rw-rw-   0        0        0    27464 2024-04-25 11:05:34.000000 napari_smlmlab-0.0.1/src/smlmlab/utils/events_utils.py
--rw-rw-rw-   0        0        0    24199 2024-04-25 13:38:40.000000 napari_smlmlab-0.0.1/src/smlmlab/utils/import_utils.py
--rw-rw-rw-   0        0        0    37319 2024-04-25 13:38:40.000000 napari_smlmlab-0.0.1/src/smlmlab/utils/loc_utils.py
--rw-rw-rw-   0        0        0    23979 2024-04-25 13:38:40.000000 napari_smlmlab-0.0.1/src/smlmlab/utils/picasso_utils.py
--rw-rw-rw-   0        0        0    10740 2024-04-24 17:38:37.000000 napari_smlmlab-0.0.1/src/smlmlab/utils/viewer_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-26 10:43:35.739201 napari_smlmlab-0.0.2/
+-rw-rw-rw-   0        0        0     1515 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4645 2024-04-26 10:43:35.739201 napari_smlmlab-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2854 2024-04-25 14:22:00.000000 napari_smlmlab-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1243 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1819 2024-04-26 10:43:35.739201 napari_smlmlab-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 10:43:35.654586 napari_smlmlab-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 10:43:35.739201 napari_smlmlab-0.0.2/src/napari_SMLMLAB.egg-info/
+-rw-rw-rw-   0        0        0     4645 2024-04-26 10:43:35.000000 napari_smlmlab-0.0.2/src/napari_SMLMLAB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      696 2024-04-26 10:43:35.000000 napari_smlmlab-0.0.2/src/napari_SMLMLAB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 10:43:35.000000 napari_smlmlab-0.0.2/src/napari_SMLMLAB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-26 10:43:35.000000 napari_smlmlab-0.0.2/src/napari_SMLMLAB.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      148 2024-04-26 10:43:35.000000 napari_smlmlab-0.0.2/src/napari_SMLMLAB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-26 10:43:35.000000 napari_smlmlab-0.0.2/src/napari_SMLMLAB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 10:43:35.707927 napari_smlmlab-0.0.2/src/smlmlab/
+-rw-rw-rw-   0        0        0      102 2024-04-26 10:43:06.000000 napari_smlmlab-0.0.2/src/smlmlab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 10:43:35.707927 napari_smlmlab-0.0.2/src/smlmlab/_tests/
+-rw-rw-rw-   0        0        0        0 2024-04-24 10:36:50.000000 napari_smlmlab-0.0.2/src/smlmlab/_tests/__init__.py
+-rw-rw-rw-   0        0        0     2176 2024-04-25 13:50:35.000000 napari_smlmlab-0.0.2/src/smlmlab/_tests/test_widget.py
+-rw-rw-rw-   0        0        0     9530 2024-04-26 10:41:37.000000 napari_smlmlab-0.0.2/src/smlmlab/_widget.py
+-rw-rw-rw-   0        0        0    33707 2024-04-25 13:35:12.000000 napari_smlmlab-0.0.2/src/smlmlab/gui.py
+-rw-rw-rw-   0        0        0      502 2024-04-25 13:52:37.000000 napari_smlmlab-0.0.2/src/smlmlab/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-04-26 10:43:35.739201 napari_smlmlab-0.0.2/src/smlmlab/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-24 11:59:46.000000 napari_smlmlab-0.0.2/src/smlmlab/utils/__init__.py
+-rw-rw-rw-   0        0        0     9793 2024-04-25 12:48:07.000000 napari_smlmlab-0.0.2/src/smlmlab/utils/compute_utils.py
+-rw-rw-rw-   0        0        0    27464 2024-04-25 11:05:34.000000 napari_smlmlab-0.0.2/src/smlmlab/utils/events_utils.py
+-rw-rw-rw-   0        0        0    24199 2024-04-25 13:38:40.000000 napari_smlmlab-0.0.2/src/smlmlab/utils/import_utils.py
+-rw-rw-rw-   0        0        0    37319 2024-04-25 13:38:40.000000 napari_smlmlab-0.0.2/src/smlmlab/utils/loc_utils.py
+-rw-rw-rw-   0        0        0    23979 2024-04-25 13:38:40.000000 napari_smlmlab-0.0.2/src/smlmlab/utils/picasso_utils.py
+-rw-rw-rw-   0        0        0    10740 2024-04-24 17:38:37.000000 napari_smlmlab-0.0.2/src/smlmlab/utils/viewer_utils.py
```

### Comparing `napari_smlmlab-0.0.1/LICENSE` & `napari_smlmlab-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.1/PKG-INFO` & `napari_smlmlab-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SMLMLAB
-Version: 0.0.1
+Version: 0.0.2
 Summary: Napari widget for BP04 Practical
 Home-page: https://github.com/piedrro/napari-SMLMLAB
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-SMLMLAB/issues
 Project-URL: Documentation, https://github.com/piedrro/napari-SMLMLAB#README.md
```

### Comparing `napari_smlmlab-0.0.1/README.md` & `napari_smlmlab-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.1/pyproject.toml` & `napari_smlmlab-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.1/setup.cfg` & `napari_smlmlab-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.1/src/napari_SMLMLAB.egg-info/PKG-INFO` & `napari_smlmlab-0.0.2/src/napari_SMLMLAB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SMLMLAB
-Version: 0.0.1
+Version: 0.0.2
 Summary: Napari widget for BP04 Practical
 Home-page: https://github.com/piedrro/napari-SMLMLAB
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-SMLMLAB/issues
 Project-URL: Documentation, https://github.com/piedrro/napari-SMLMLAB#README.md
```

### Comparing `napari_smlmlab-0.0.1/src/napari_SMLMLAB.egg-info/SOURCES.txt` & `napari_smlmlab-0.0.2/src/napari_SMLMLAB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.1/src/smlmlab/_tests/test_widget.py` & `napari_smlmlab-0.0.2/src/smlmlab/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.1/src/smlmlab/_widget.py` & `napari_smlmlab-0.0.2/src/smlmlab/_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,39 +80,51 @@
         self.worker = None
         self.multiprocessing_active = False
 
         self.viewer.layers.events.inserted.connect(self.on_add_layer)
 
     def on_add_layer(self, event):
         if event.value.name == "Shapes":
-            layer_list = [layer.name for layer in self.viewer.layers if layer.name != "Shapes"]
 
             self.shapes_layer = self.viewer.layers["Shapes"]
 
             self.shapes_layer.events.data.connect(self.shapes_layer_updated)
 
             self.shapes_layer.current_edge_color = list(mcolors.to_rgb("green"))
             self.shapes_layer.current_face_color = [0, 0, 0, 0]
             self.shapes_layer.current_edge_width = 1
 
+
     def shapes_layer_updated(self, event):
         try:
+
             if event.action in ["added", "changed", "removed"]:
+
                 shapes_layer = self.viewer.layers["Shapes"]
-                shape_type = shapes_layer.shape_type[-1]
+                shapes = shapes_layer.data
+
+                if len(shapes) > 0:
+
+                    shape_type = shapes_layer.shape_type[-1]
+
+                    if shapes_layer.ndim == 3:
+
+                        if self.verbose:
+                            print("reformatting shapes to ndim=2")
 
-                if shape_type == "line":
-                    shape = shapes_layer.data[-1].copy()
-                    shape = shape[:, 1:]
-                    self.viewer.layers["Shapes"].data[-1] = shape
+                        shapes = shapes_layer.data.copy()
+                        shapes = [shape[:,-2:] for shape in shapes]
+                        shapes_layer.data = []
+                        shapes_layer.add(shapes, shape_type=shape_type)
 
-                    self.gui.plot_mode.setCurrentIndex(0)
+                    if shape_type == "line":
+                        self.gui.plot_mode.setCurrentIndex(0)
 
-                if shape_type == "rectangle":
-                    self.gui.plot_mode.setCurrentIndex(1)
+                    if shape_type == "rectangle":
+                        self.gui.plot_mode.setCurrentIndex(1)
 
                 self.draw_line_plot()
 
         except:
             print(traceback.format_exc())
 
     def get_plot_data(self):
```

### Comparing `napari_smlmlab-0.0.1/src/smlmlab/gui.py` & `napari_smlmlab-0.0.2/src/smlmlab/gui.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.1/src/smlmlab/utils/compute_utils.py` & `napari_smlmlab-0.0.2/src/smlmlab/utils/compute_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.1/src/smlmlab/utils/events_utils.py` & `napari_smlmlab-0.0.2/src/smlmlab/utils/events_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.1/src/smlmlab/utils/import_utils.py` & `napari_smlmlab-0.0.2/src/smlmlab/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.1/src/smlmlab/utils/loc_utils.py` & `napari_smlmlab-0.0.2/src/smlmlab/utils/loc_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.1/src/smlmlab/utils/picasso_utils.py` & `napari_smlmlab-0.0.2/src/smlmlab/utils/picasso_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.1/src/smlmlab/utils/viewer_utils.py` & `napari_smlmlab-0.0.2/src/smlmlab/utils/viewer_utils.py`

 * *Files identical despite different names*

