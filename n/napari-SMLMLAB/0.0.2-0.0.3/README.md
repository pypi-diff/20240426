# Comparing `tmp/napari_smlmlab-0.0.2.tar.gz` & `tmp/napari_smlmlab-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\turnerp\PycharmProjects\napari-SMLMLAB\dist\.tmp-e_pi3v7d\napari_smlmlab-0.0.2.tar", last modified: Fri Apr 26 10:43:35 2024, max compression
+gzip compressed data, was "C:\Users\turnerp\PycharmProjects\napari-SMLMLAB\dist\.tmp-6_6qgu21\napari_smlmlab-0.0.3.tar", last modified: Fri Apr 26 21:32:01 2024, max compression
```

## Comparing `napari_smlmlab-0.0.2.tar` & `napari_smlmlab-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 10:43:35.739201 napari_smlmlab-0.0.2/
--rw-rw-rw-   0        0        0     1515 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      101 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4645 2024-04-26 10:43:35.739201 napari_smlmlab-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2854 2024-04-25 14:22:00.000000 napari_smlmlab-0.0.2/README.md
--rw-rw-rw-   0        0        0     1243 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1819 2024-04-26 10:43:35.739201 napari_smlmlab-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-26 10:43:35.654586 napari_smlmlab-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 10:43:35.739201 napari_smlmlab-0.0.2/src/napari_SMLMLAB.egg-info/
--rw-rw-rw-   0        0        0     4645 2024-04-26 10:43:35.000000 napari_smlmlab-0.0.2/src/napari_SMLMLAB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      696 2024-04-26 10:43:35.000000 napari_smlmlab-0.0.2/src/napari_SMLMLAB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 10:43:35.000000 napari_smlmlab-0.0.2/src/napari_SMLMLAB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-26 10:43:35.000000 napari_smlmlab-0.0.2/src/napari_SMLMLAB.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      148 2024-04-26 10:43:35.000000 napari_smlmlab-0.0.2/src/napari_SMLMLAB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-26 10:43:35.000000 napari_smlmlab-0.0.2/src/napari_SMLMLAB.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-26 10:43:35.707927 napari_smlmlab-0.0.2/src/smlmlab/
--rw-rw-rw-   0        0        0      102 2024-04-26 10:43:06.000000 napari_smlmlab-0.0.2/src/smlmlab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:43:35.707927 napari_smlmlab-0.0.2/src/smlmlab/_tests/
--rw-rw-rw-   0        0        0        0 2024-04-24 10:36:50.000000 napari_smlmlab-0.0.2/src/smlmlab/_tests/__init__.py
--rw-rw-rw-   0        0        0     2176 2024-04-25 13:50:35.000000 napari_smlmlab-0.0.2/src/smlmlab/_tests/test_widget.py
--rw-rw-rw-   0        0        0     9530 2024-04-26 10:41:37.000000 napari_smlmlab-0.0.2/src/smlmlab/_widget.py
--rw-rw-rw-   0        0        0    33707 2024-04-25 13:35:12.000000 napari_smlmlab-0.0.2/src/smlmlab/gui.py
--rw-rw-rw-   0        0        0      502 2024-04-25 13:52:37.000000 napari_smlmlab-0.0.2/src/smlmlab/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-04-26 10:43:35.739201 napari_smlmlab-0.0.2/src/smlmlab/utils/
--rw-rw-rw-   0        0        0        0 2024-04-24 11:59:46.000000 napari_smlmlab-0.0.2/src/smlmlab/utils/__init__.py
--rw-rw-rw-   0        0        0     9793 2024-04-25 12:48:07.000000 napari_smlmlab-0.0.2/src/smlmlab/utils/compute_utils.py
--rw-rw-rw-   0        0        0    27464 2024-04-25 11:05:34.000000 napari_smlmlab-0.0.2/src/smlmlab/utils/events_utils.py
--rw-rw-rw-   0        0        0    24199 2024-04-25 13:38:40.000000 napari_smlmlab-0.0.2/src/smlmlab/utils/import_utils.py
--rw-rw-rw-   0        0        0    37319 2024-04-25 13:38:40.000000 napari_smlmlab-0.0.2/src/smlmlab/utils/loc_utils.py
--rw-rw-rw-   0        0        0    23979 2024-04-25 13:38:40.000000 napari_smlmlab-0.0.2/src/smlmlab/utils/picasso_utils.py
--rw-rw-rw-   0        0        0    10740 2024-04-24 17:38:37.000000 napari_smlmlab-0.0.2/src/smlmlab/utils/viewer_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-26 21:32:01.648079 napari_smlmlab-0.0.3/
+-rw-rw-rw-   0        0        0     1515 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4645 2024-04-26 21:32:01.648079 napari_smlmlab-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2854 2024-04-25 14:22:00.000000 napari_smlmlab-0.0.3/README.md
+-rw-rw-rw-   0        0        0     1243 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1819 2024-04-26 21:32:01.651043 napari_smlmlab-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 21:32:01.587755 napari_smlmlab-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 21:32:01.645172 napari_smlmlab-0.0.3/src/napari_SMLMLAB.egg-info/
+-rw-rw-rw-   0        0        0     4645 2024-04-26 21:32:01.000000 napari_smlmlab-0.0.3/src/napari_SMLMLAB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      696 2024-04-26 21:32:01.000000 napari_smlmlab-0.0.3/src/napari_SMLMLAB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 21:32:01.000000 napari_smlmlab-0.0.3/src/napari_SMLMLAB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-26 21:32:01.000000 napari_smlmlab-0.0.3/src/napari_SMLMLAB.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      148 2024-04-26 21:32:01.000000 napari_smlmlab-0.0.3/src/napari_SMLMLAB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-26 21:32:01.000000 napari_smlmlab-0.0.3/src/napari_SMLMLAB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 21:32:01.625266 napari_smlmlab-0.0.3/src/smlmlab/
+-rw-rw-rw-   0        0        0      102 2024-04-26 21:31:13.000000 napari_smlmlab-0.0.3/src/smlmlab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 21:32:01.629257 napari_smlmlab-0.0.3/src/smlmlab/_tests/
+-rw-rw-rw-   0        0        0        0 2024-04-24 10:36:50.000000 napari_smlmlab-0.0.3/src/smlmlab/_tests/__init__.py
+-rw-rw-rw-   0        0        0     2176 2024-04-25 13:50:35.000000 napari_smlmlab-0.0.3/src/smlmlab/_tests/test_widget.py
+-rw-rw-rw-   0        0        0     9749 2024-04-26 21:31:44.000000 napari_smlmlab-0.0.3/src/smlmlab/_widget.py
+-rw-rw-rw-   0        0        0    33082 2024-04-26 16:20:20.000000 napari_smlmlab-0.0.3/src/smlmlab/gui.py
+-rw-rw-rw-   0        0        0      502 2024-04-25 13:52:37.000000 napari_smlmlab-0.0.3/src/smlmlab/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-04-26 21:32:01.642179 napari_smlmlab-0.0.3/src/smlmlab/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-24 11:59:46.000000 napari_smlmlab-0.0.3/src/smlmlab/utils/__init__.py
+-rw-rw-rw-   0        0        0     9793 2024-04-25 12:48:07.000000 napari_smlmlab-0.0.3/src/smlmlab/utils/compute_utils.py
+-rw-rw-rw-   0        0        0    27432 2024-04-26 16:20:15.000000 napari_smlmlab-0.0.3/src/smlmlab/utils/events_utils.py
+-rw-rw-rw-   0        0        0    20955 2024-04-26 15:44:32.000000 napari_smlmlab-0.0.3/src/smlmlab/utils/import_utils.py
+-rw-rw-rw-   0        0        0    31463 2024-04-26 16:23:10.000000 napari_smlmlab-0.0.3/src/smlmlab/utils/loc_utils.py
+-rw-rw-rw-   0        0        0    24786 2024-04-26 20:50:24.000000 napari_smlmlab-0.0.3/src/smlmlab/utils/picasso_utils.py
+-rw-rw-rw-   0        0        0     8197 2024-04-26 20:55:11.000000 napari_smlmlab-0.0.3/src/smlmlab/utils/viewer_utils.py
```

### Comparing `napari_smlmlab-0.0.2/LICENSE` & `napari_smlmlab-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.2/PKG-INFO` & `napari_smlmlab-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SMLMLAB
-Version: 0.0.2
+Version: 0.0.3
 Summary: Napari widget for BP04 Practical
 Home-page: https://github.com/piedrro/napari-SMLMLAB
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-SMLMLAB/issues
 Project-URL: Documentation, https://github.com/piedrro/napari-SMLMLAB#README.md
```

### Comparing `napari_smlmlab-0.0.2/README.md` & `napari_smlmlab-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.2/pyproject.toml` & `napari_smlmlab-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.2/setup.cfg` & `napari_smlmlab-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.2/src/napari_SMLMLAB.egg-info/PKG-INFO` & `napari_smlmlab-0.0.3/src/napari_SMLMLAB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SMLMLAB
-Version: 0.0.2
+Version: 0.0.3
 Summary: Napari widget for BP04 Practical
 Home-page: https://github.com/piedrro/napari-SMLMLAB
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-SMLMLAB/issues
 Project-URL: Documentation, https://github.com/piedrro/napari-SMLMLAB#README.md
```

### Comparing `napari_smlmlab-0.0.2/src/napari_SMLMLAB.egg-info/SOURCES.txt` & `napari_smlmlab-0.0.3/src/napari_SMLMLAB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.2/src/smlmlab/_tests/test_widget.py` & `napari_smlmlab-0.0.3/src/smlmlab/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.2/src/smlmlab/_widget.py` & `napari_smlmlab-0.0.3/src/smlmlab/_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,29 +43,30 @@
 
         self.viewer.dims.events.current_step.connect(partial(self.draw_molecules, update_vis=False))
 
         self.gui.picasso_detect.clicked.connect(partial(self.pixseq_picasso, detect=True, fit=False))
         self.gui.picasso_fit.clicked.connect(partial(self.pixseq_picasso, detect=False, fit=True))
         self.gui.picasso_detectfit.clicked.connect(partial(self.pixseq_picasso, detect=True, fit=True))
         self.gui.picasso_render.clicked.connect(self.picasso_render)
+        self.gui.export_locs.clicked.connect(self.initialise_export_locs)
 
         self.gui.picasso_vis_mode.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
         self.gui.picasso_vis_mode.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
         self.gui.picasso_vis_size.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
         self.gui.picasso_vis_size.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
         self.gui.picasso_vis_opacity.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
         self.gui.picasso_vis_opacity.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
         self.gui.picasso_vis_edge_width.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
         self.gui.picasso_vis_edge_width.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
 
         self.gui.plot_mode.currentIndexChanged.connect(self.draw_line_plot)
         self.gui.plot_dataset.currentIndexChanged.connect(self.draw_line_plot)
         self.gui.plot_channel.currentIndexChanged.connect(self.draw_line_plot)
 
-        self.verbose = True
+        self.verbose = False
 
         self.dataset_dict = {}
         self.localisation_dict = {"bounding_boxes": {}, "molecules": {}}
         self.traces_dict = {}
         self.plot_dict = {}
         self.contrast_dict = {}
 
@@ -80,46 +81,44 @@
         self.worker = None
         self.multiprocessing_active = False
 
         self.viewer.layers.events.inserted.connect(self.on_add_layer)
 
     def on_add_layer(self, event):
         if event.value.name == "Shapes":
-
             self.shapes_layer = self.viewer.layers["Shapes"]
 
             self.shapes_layer.events.data.connect(self.shapes_layer_updated)
 
             self.shapes_layer.current_edge_color = list(mcolors.to_rgb("green"))
             self.shapes_layer.current_face_color = [0, 0, 0, 0]
             self.shapes_layer.current_edge_width = 1
 
-
     def shapes_layer_updated(self, event):
         try:
-
             if event.action in ["added", "changed", "removed"]:
-
                 shapes_layer = self.viewer.layers["Shapes"]
                 shapes = shapes_layer.data
 
                 if len(shapes) > 0:
-
                     shape_type = shapes_layer.shape_type[-1]
 
                     if shapes_layer.ndim == 3:
-
                         if self.verbose:
                             print("reformatting shapes to ndim=2")
 
                         shapes = shapes_layer.data.copy()
-                        shapes = [shape[:,-2:] for shape in shapes]
+                        shapes = [shape[:, -2:] for shape in shapes]
                         shapes_layer.data = []
                         shapes_layer.add(shapes, shape_type=shape_type)
 
+                    # if event.action == "added":
+                    #     shapes = shapes[-1]
+                    #     shapes_layer.data = shapes
+
                     if shape_type == "line":
                         self.gui.plot_mode.setCurrentIndex(0)
 
                     if shape_type == "rectangle":
                         self.gui.plot_mode.setCurrentIndex(1)
 
                 self.draw_line_plot()
```

### Comparing `napari_smlmlab-0.0.2/src/smlmlab/gui.py` & `napari_smlmlab-0.0.3/src/smlmlab/gui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+# -*- coding: utf-8 -*-
+
 # Form implementation generated from reading ui file 'gui.ui'
 #
 # Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_Frame:
+class Ui_Frame(object):
     def setupUi(self, Frame):
         Frame.setObjectName("Frame")
         Frame.resize(482, 556)
         self.verticalLayout = QtWidgets.QVBoxLayout(Frame)
         self.verticalLayout.setObjectName("verticalLayout")
         self.tabWidget = QtWidgets.QTabWidget(Frame)
         self.tabWidget.setObjectName("tabWidget")
@@ -21,103 +23,70 @@
         self.tab.setObjectName("tab")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.tab)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
         self.formLayout = QtWidgets.QFormLayout()
         self.formLayout.setObjectName("formLayout")
         self.label = QtWidgets.QLabel(self.tab)
         self.label.setObjectName("label")
-        self.formLayout.setWidget(
-            0, QtWidgets.QFormLayout.LabelRole, self.label
-        )
+        self.formLayout.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label)
         self.import_mode = QtWidgets.QComboBox(self.tab)
         self.import_mode.setObjectName("import_mode")
         self.import_mode.addItem("")
         self.import_mode.addItem("")
         self.import_mode.addItem("")
         self.import_mode.addItem("")
-        self.formLayout.setWidget(
-            0, QtWidgets.QFormLayout.FieldRole, self.import_mode
-        )
+        self.formLayout.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.import_mode)
         self.pixseq_channel_layout_label = QtWidgets.QLabel(self.tab)
-        self.pixseq_channel_layout_label.setObjectName(
-            "pixseq_channel_layout_label"
-        )
-        self.formLayout.setWidget(
-            1,
-            QtWidgets.QFormLayout.LabelRole,
-            self.pixseq_channel_layout_label,
-        )
+        self.pixseq_channel_layout_label.setObjectName("pixseq_channel_layout_label")
+        self.formLayout.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.pixseq_channel_layout_label)
         self.channel_layout = QtWidgets.QComboBox(self.tab)
         self.channel_layout.setObjectName("channel_layout")
         self.channel_layout.addItem("")
         self.channel_layout.addItem("")
-        self.formLayout.setWidget(
-            1, QtWidgets.QFormLayout.FieldRole, self.channel_layout
-        )
+        self.formLayout.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.channel_layout)
         self.pixseq_alex_first_frame_label = QtWidgets.QLabel(self.tab)
-        self.pixseq_alex_first_frame_label.setObjectName(
-            "pixseq_alex_first_frame_label"
-        )
-        self.formLayout.setWidget(
-            2,
-            QtWidgets.QFormLayout.LabelRole,
-            self.pixseq_alex_first_frame_label,
-        )
+        self.pixseq_alex_first_frame_label.setObjectName("pixseq_alex_first_frame_label")
+        self.formLayout.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.pixseq_alex_first_frame_label)
         self.alex_first_frame = QtWidgets.QComboBox(self.tab)
         self.alex_first_frame.setObjectName("alex_first_frame")
         self.alex_first_frame.addItem("")
         self.alex_first_frame.addItem("")
-        self.formLayout.setWidget(
-            2, QtWidgets.QFormLayout.FieldRole, self.alex_first_frame
-        )
+        self.formLayout.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.alex_first_frame)
         self.label_32 = QtWidgets.QLabel(self.tab)
         self.label_32.setObjectName("label_32")
-        self.formLayout.setWidget(
-            3, QtWidgets.QFormLayout.LabelRole, self.label_32
-        )
+        self.formLayout.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_32)
         self.import_limt = QtWidgets.QComboBox(self.tab)
         self.import_limt.setObjectName("import_limt")
         self.import_limt.addItem("")
         self.import_limt.addItem("")
         self.import_limt.addItem("")
         self.import_limt.addItem("")
         self.import_limt.addItem("")
         self.import_limt.addItem("")
         self.import_limt.addItem("")
         self.import_limt.addItem("")
-        self.formLayout.setWidget(
-            3, QtWidgets.QFormLayout.FieldRole, self.import_limt
-        )
+        self.formLayout.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.import_limt)
         self.label_15 = QtWidgets.QLabel(self.tab)
         self.label_15.setObjectName("label_15")
-        self.formLayout.setWidget(
-            4, QtWidgets.QFormLayout.LabelRole, self.label_15
-        )
+        self.formLayout.setWidget(4, QtWidgets.QFormLayout.LabelRole, self.label_15)
         self.pixel_size = QtWidgets.QDoubleSpinBox(self.tab)
         self.pixel_size.setDecimals(3)
         self.pixel_size.setProperty("value", 0.116)
         self.pixel_size.setObjectName("pixel_size")
-        self.formLayout.setWidget(
-            4, QtWidgets.QFormLayout.FieldRole, self.pixel_size
-        )
+        self.formLayout.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.pixel_size)
         self.verticalLayout_2.addLayout(self.formLayout)
         self.import_data = QtWidgets.QPushButton(self.tab)
         self.import_data.setObjectName("import_data")
         self.verticalLayout_2.addWidget(self.import_data)
         self.import_progressbar = QtWidgets.QProgressBar(self.tab)
         self.import_progressbar.setMaximumSize(QtCore.QSize(16777215, 10))
         self.import_progressbar.setProperty("value", 0)
         self.import_progressbar.setObjectName("import_progressbar")
         self.verticalLayout_2.addWidget(self.import_progressbar)
-        spacerItem = QtWidgets.QSpacerItem(
-            20,
-            40,
-            QtWidgets.QSizePolicy.Minimum,
-            QtWidgets.QSizePolicy.Expanding,
-        )
+        spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_2.addItem(spacerItem)
         self.tabWidget.addTab(self.tab, "")
         self.tab_2 = QtWidgets.QWidget()
         self.tab_2.setObjectName("tab_2")
         self.verticalLayout_3 = QtWidgets.QVBoxLayout(self.tab_2)
         self.verticalLayout_3.setObjectName("verticalLayout_3")
         self.tabWidget_2 = QtWidgets.QTabWidget(self.tab_2)
@@ -131,98 +100,60 @@
         font.setBold(True)
         font.setWeight(75)
         self.label_3.setFont(font)
         self.label_3.setObjectName("label_3")
         self.verticalLayout_4.addWidget(self.label_3)
         self.formLayout_3 = QtWidgets.QFormLayout()
         self.formLayout_3.setObjectName("formLayout_3")
-        self.label_7 = QtWidgets.QLabel(self.tab_3)
-        self.label_7.setObjectName("label_7")
-        self.formLayout_3.setWidget(
-            0, QtWidgets.QFormLayout.LabelRole, self.label_7
-        )
-        self.picasso_detect_mode = QtWidgets.QComboBox(self.tab_3)
-        self.picasso_detect_mode.setObjectName("picasso_detect_mode")
-        self.picasso_detect_mode.addItem("")
-        self.picasso_detect_mode.addItem("")
-        self.formLayout_3.setWidget(
-            0, QtWidgets.QFormLayout.FieldRole, self.picasso_detect_mode
-        )
         self.label_11 = QtWidgets.QLabel(self.tab_3)
         self.label_11.setObjectName("label_11")
-        self.formLayout_3.setWidget(
-            1, QtWidgets.QFormLayout.LabelRole, self.label_11
-        )
+        self.formLayout_3.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_11)
         self.picasso_dataset = QtWidgets.QComboBox(self.tab_3)
         self.picasso_dataset.setObjectName("picasso_dataset")
-        self.formLayout_3.setWidget(
-            1, QtWidgets.QFormLayout.FieldRole, self.picasso_dataset
-        )
+        self.formLayout_3.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.picasso_dataset)
         self.label_6 = QtWidgets.QLabel(self.tab_3)
         self.label_6.setObjectName("label_6")
-        self.formLayout_3.setWidget(
-            2, QtWidgets.QFormLayout.LabelRole, self.label_6
-        )
+        self.formLayout_3.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_6)
         self.picasso_channel = QtWidgets.QComboBox(self.tab_3)
         self.picasso_channel.setObjectName("picasso_channel")
-        self.formLayout_3.setWidget(
-            2, QtWidgets.QFormLayout.FieldRole, self.picasso_channel
-        )
+        self.formLayout_3.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.picasso_channel)
         self.label_8 = QtWidgets.QLabel(self.tab_3)
         self.label_8.setObjectName("label_8")
-        self.formLayout_3.setWidget(
-            3, QtWidgets.QFormLayout.LabelRole, self.label_8
-        )
+        self.formLayout_3.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_8)
         self.picasso_frame_mode = QtWidgets.QComboBox(self.tab_3)
         self.picasso_frame_mode.setObjectName("picasso_frame_mode")
         self.picasso_frame_mode.addItem("")
         self.picasso_frame_mode.addItem("")
-        self.formLayout_3.setWidget(
-            3, QtWidgets.QFormLayout.FieldRole, self.picasso_frame_mode
-        )
-        self.label_5 = QtWidgets.QLabel(self.tab_3)
-        self.label_5.setObjectName("label_5")
-        self.formLayout_3.setWidget(
-            5, QtWidgets.QFormLayout.LabelRole, self.label_5
-        )
-        self.picasso_min_net_gradient = QtWidgets.QLineEdit(self.tab_3)
-        self.picasso_min_net_gradient.setObjectName("picasso_min_net_gradient")
-        self.formLayout_3.setWidget(
-            5, QtWidgets.QFormLayout.FieldRole, self.picasso_min_net_gradient
-        )
+        self.formLayout_3.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.picasso_frame_mode)
         self.label_28 = QtWidgets.QLabel(self.tab_3)
         self.label_28.setObjectName("label_28")
-        self.formLayout_3.setWidget(
-            4, QtWidgets.QFormLayout.LabelRole, self.label_28
-        )
+        self.formLayout_3.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_28)
         self.picasso_box_size = QtWidgets.QComboBox(self.tab_3)
         self.picasso_box_size.setObjectName("picasso_box_size")
         self.picasso_box_size.addItem("")
         self.picasso_box_size.addItem("")
         self.picasso_box_size.addItem("")
         self.picasso_box_size.addItem("")
-        self.formLayout_3.setWidget(
-            4, QtWidgets.QFormLayout.FieldRole, self.picasso_box_size
-        )
+        self.formLayout_3.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.picasso_box_size)
+        self.label_5 = QtWidgets.QLabel(self.tab_3)
+        self.label_5.setObjectName("label_5")
+        self.formLayout_3.setWidget(4, QtWidgets.QFormLayout.LabelRole, self.label_5)
+        self.picasso_min_net_gradient = QtWidgets.QLineEdit(self.tab_3)
+        self.picasso_min_net_gradient.setObjectName("picasso_min_net_gradient")
+        self.formLayout_3.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.picasso_min_net_gradient)
         self.label_35 = QtWidgets.QLabel(self.tab_3)
         self.label_35.setObjectName("label_35")
-        self.formLayout_3.setWidget(
-            6, QtWidgets.QFormLayout.LabelRole, self.label_35
-        )
+        self.formLayout_3.setWidget(5, QtWidgets.QFormLayout.LabelRole, self.label_35)
         self.picasso_roi_border_width = QtWidgets.QLineEdit(self.tab_3)
         self.picasso_roi_border_width.setObjectName("picasso_roi_border_width")
-        self.formLayout_3.setWidget(
-            6, QtWidgets.QFormLayout.FieldRole, self.picasso_roi_border_width
-        )
+        self.formLayout_3.setWidget(5, QtWidgets.QFormLayout.FieldRole, self.picasso_roi_border_width)
         self.verticalLayout_4.addLayout(self.formLayout_3)
         self.picasso_remove_overlapping = QtWidgets.QCheckBox(self.tab_3)
         self.picasso_remove_overlapping.setChecked(True)
-        self.picasso_remove_overlapping.setObjectName(
-            "picasso_remove_overlapping"
-        )
+        self.picasso_remove_overlapping.setObjectName("picasso_remove_overlapping")
         self.verticalLayout_4.addWidget(self.picasso_remove_overlapping)
         self.picasso_window_cropping = QtWidgets.QCheckBox(self.tab_3)
         self.picasso_window_cropping.setObjectName("picasso_window_cropping")
         self.verticalLayout_4.addWidget(self.picasso_window_cropping)
         self.picasso_minimise_ram = QtWidgets.QCheckBox(self.tab_3)
         self.picasso_minimise_ram.setObjectName("picasso_minimise_ram")
         self.verticalLayout_4.addWidget(self.picasso_minimise_ram)
@@ -239,20 +170,15 @@
         self.gridLayout_6.addWidget(self.picasso_detectfit, 0, 2, 1, 1)
         self.verticalLayout_4.addLayout(self.gridLayout_6)
         self.picasso_progressbar = QtWidgets.QProgressBar(self.tab_3)
         self.picasso_progressbar.setMaximumSize(QtCore.QSize(16777215, 10))
         self.picasso_progressbar.setProperty("value", 0)
         self.picasso_progressbar.setObjectName("picasso_progressbar")
         self.verticalLayout_4.addWidget(self.picasso_progressbar)
-        spacerItem1 = QtWidgets.QSpacerItem(
-            20,
-            40,
-            QtWidgets.QSizePolicy.Minimum,
-            QtWidgets.QSizePolicy.Expanding,
-        )
+        spacerItem1 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_4.addItem(spacerItem1)
         self.tabWidget_2.addTab(self.tab_3, "")
         self.tab_5 = QtWidgets.QWidget()
         self.tab_5.setObjectName("tab_5")
         self.verticalLayout_6 = QtWidgets.QVBoxLayout(self.tab_5)
         self.verticalLayout_6.setObjectName("verticalLayout_6")
         self.label_2 = QtWidgets.QLabel(self.tab_5)
@@ -262,72 +188,77 @@
         self.label_2.setFont(font)
         self.label_2.setObjectName("label_2")
         self.verticalLayout_6.addWidget(self.label_2)
         self.formLayout_4 = QtWidgets.QFormLayout()
         self.formLayout_4.setObjectName("formLayout_4")
         self.label_4 = QtWidgets.QLabel(self.tab_5)
         self.label_4.setObjectName("label_4")
-        self.formLayout_4.setWidget(
-            0, QtWidgets.QFormLayout.LabelRole, self.label_4
-        )
+        self.formLayout_4.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_4)
         self.picasso_render_dataset = QtWidgets.QComboBox(self.tab_5)
         self.picasso_render_dataset.setObjectName("picasso_render_dataset")
-        self.formLayout_4.setWidget(
-            0, QtWidgets.QFormLayout.FieldRole, self.picasso_render_dataset
-        )
+        self.formLayout_4.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.picasso_render_dataset)
         self.label_9 = QtWidgets.QLabel(self.tab_5)
         self.label_9.setObjectName("label_9")
-        self.formLayout_4.setWidget(
-            1, QtWidgets.QFormLayout.LabelRole, self.label_9
-        )
+        self.formLayout_4.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_9)
         self.picasso_render_channel = QtWidgets.QComboBox(self.tab_5)
         self.picasso_render_channel.setObjectName("picasso_render_channel")
-        self.formLayout_4.setWidget(
-            1, QtWidgets.QFormLayout.FieldRole, self.picasso_render_channel
-        )
+        self.formLayout_4.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.picasso_render_channel)
         self.label_10 = QtWidgets.QLabel(self.tab_5)
         self.label_10.setObjectName("label_10")
-        self.formLayout_4.setWidget(
-            2, QtWidgets.QFormLayout.LabelRole, self.label_10
-        )
+        self.formLayout_4.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_10)
         self.picasso_render_blur_method = QtWidgets.QComboBox(self.tab_5)
-        self.picasso_render_blur_method.setObjectName(
-            "picasso_render_blur_method"
-        )
+        self.picasso_render_blur_method.setObjectName("picasso_render_blur_method")
         self.picasso_render_blur_method.addItem("")
         self.picasso_render_blur_method.addItem("")
         self.picasso_render_blur_method.addItem("")
         self.picasso_render_blur_method.addItem("")
         self.picasso_render_blur_method.addItem("")
-        self.formLayout_4.setWidget(
-            2, QtWidgets.QFormLayout.FieldRole, self.picasso_render_blur_method
-        )
+        self.formLayout_4.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.picasso_render_blur_method)
         self.label_13 = QtWidgets.QLabel(self.tab_5)
         self.label_13.setObjectName("label_13")
-        self.formLayout_4.setWidget(
-            3, QtWidgets.QFormLayout.LabelRole, self.label_13
-        )
+        self.formLayout_4.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_13)
         self.picasso_render_min_blur = QtWidgets.QDoubleSpinBox(self.tab_5)
         self.picasso_render_min_blur.setSingleStep(0.1)
         self.picasso_render_min_blur.setObjectName("picasso_render_min_blur")
-        self.formLayout_4.setWidget(
-            3, QtWidgets.QFormLayout.FieldRole, self.picasso_render_min_blur
-        )
+        self.formLayout_4.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.picasso_render_min_blur)
         self.verticalLayout_6.addLayout(self.formLayout_4)
         self.picasso_render = QtWidgets.QPushButton(self.tab_5)
         self.picasso_render.setObjectName("picasso_render")
         self.verticalLayout_6.addWidget(self.picasso_render)
-        spacerItem2 = QtWidgets.QSpacerItem(
-            20,
-            40,
-            QtWidgets.QSizePolicy.Minimum,
-            QtWidgets.QSizePolicy.Expanding,
-        )
+        spacerItem2 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_6.addItem(spacerItem2)
         self.tabWidget_2.addTab(self.tab_5, "")
+        self.tab_7 = QtWidgets.QWidget()
+        self.tab_7.setObjectName("tab_7")
+        self.verticalLayout_8 = QtWidgets.QVBoxLayout(self.tab_7)
+        self.verticalLayout_8.setObjectName("verticalLayout_8")
+        self.label_74 = QtWidgets.QLabel(self.tab_7)
+        self.label_74.setObjectName("label_74")
+        self.verticalLayout_8.addWidget(self.label_74)
+        self.formLayout_19 = QtWidgets.QFormLayout()
+        self.formLayout_19.setObjectName("formLayout_19")
+        self.label_72 = QtWidgets.QLabel(self.tab_7)
+        self.label_72.setObjectName("label_72")
+        self.formLayout_19.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_72)
+        self.locs_export_dataset = QtWidgets.QComboBox(self.tab_7)
+        self.locs_export_dataset.setObjectName("locs_export_dataset")
+        self.formLayout_19.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.locs_export_dataset)
+        self.label_71 = QtWidgets.QLabel(self.tab_7)
+        self.label_71.setObjectName("label_71")
+        self.formLayout_19.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_71)
+        self.locs_export_channel = QtWidgets.QComboBox(self.tab_7)
+        self.locs_export_channel.setObjectName("locs_export_channel")
+        self.formLayout_19.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.locs_export_channel)
+        self.verticalLayout_8.addLayout(self.formLayout_19)
+        self.export_locs = QtWidgets.QPushButton(self.tab_7)
+        self.export_locs.setObjectName("export_locs")
+        self.verticalLayout_8.addWidget(self.export_locs)
+        spacerItem3 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_8.addItem(spacerItem3)
+        self.tabWidget_2.addTab(self.tab_7, "")
         self.tab_4 = QtWidgets.QWidget()
         self.tab_4.setObjectName("tab_4")
         self.verticalLayout_5 = QtWidgets.QVBoxLayout(self.tab_4)
         self.verticalLayout_5.setObjectName("verticalLayout_5")
         self.label_27 = QtWidgets.QLabel(self.tab_4)
         font = QtGui.QFont()
         font.setBold(True)
@@ -390,80 +321,53 @@
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.gridLayout_14.addWidget(self.picasso_vis_edge_width, 1, 3, 1, 1)
         self.verticalLayout_5.addLayout(self.gridLayout_14)
-        spacerItem3 = QtWidgets.QSpacerItem(
-            20,
-            215,
-            QtWidgets.QSizePolicy.Minimum,
-            QtWidgets.QSizePolicy.Expanding,
-        )
-        self.verticalLayout_5.addItem(spacerItem3)
+        spacerItem4 = QtWidgets.QSpacerItem(20, 215, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_5.addItem(spacerItem4)
         self.tabWidget_2.addTab(self.tab_4, "")
         self.verticalLayout_3.addWidget(self.tabWidget_2)
-        spacerItem4 = QtWidgets.QSpacerItem(
-            20,
-            40,
-            QtWidgets.QSizePolicy.Minimum,
-            QtWidgets.QSizePolicy.Expanding,
-        )
-        self.verticalLayout_3.addItem(spacerItem4)
+        spacerItem5 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_3.addItem(spacerItem5)
         self.tabWidget.addTab(self.tab_2, "")
         self.tab_6 = QtWidgets.QWidget()
         self.tab_6.setObjectName("tab_6")
         self.verticalLayout_7 = QtWidgets.QVBoxLayout(self.tab_6)
         self.verticalLayout_7.setObjectName("verticalLayout_7")
         self.formLayout_5 = QtWidgets.QFormLayout()
         self.formLayout_5.setObjectName("formLayout_5")
         self.label_16 = QtWidgets.QLabel(self.tab_6)
         self.label_16.setObjectName("label_16")
-        self.formLayout_5.setWidget(
-            0, QtWidgets.QFormLayout.LabelRole, self.label_16
-        )
+        self.formLayout_5.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_16)
         self.plot_mode = QtWidgets.QComboBox(self.tab_6)
         self.plot_mode.setObjectName("plot_mode")
         self.plot_mode.addItem("")
         self.plot_mode.addItem("")
-        self.formLayout_5.setWidget(
-            0, QtWidgets.QFormLayout.FieldRole, self.plot_mode
-        )
+        self.formLayout_5.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.plot_mode)
         self.label_17 = QtWidgets.QLabel(self.tab_6)
         self.label_17.setObjectName("label_17")
-        self.formLayout_5.setWidget(
-            1, QtWidgets.QFormLayout.LabelRole, self.label_17
-        )
+        self.formLayout_5.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_17)
         self.plot_dataset = QtWidgets.QComboBox(self.tab_6)
         self.plot_dataset.setObjectName("plot_dataset")
-        self.formLayout_5.setWidget(
-            1, QtWidgets.QFormLayout.FieldRole, self.plot_dataset
-        )
+        self.formLayout_5.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.plot_dataset)
         self.label_18 = QtWidgets.QLabel(self.tab_6)
         self.label_18.setObjectName("label_18")
-        self.formLayout_5.setWidget(
-            2, QtWidgets.QFormLayout.LabelRole, self.label_18
-        )
+        self.formLayout_5.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_18)
         self.plot_channel = QtWidgets.QComboBox(self.tab_6)
         self.plot_channel.setObjectName("plot_channel")
-        self.formLayout_5.setWidget(
-            2, QtWidgets.QFormLayout.FieldRole, self.plot_channel
-        )
+        self.formLayout_5.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.plot_channel)
         self.verticalLayout_7.addLayout(self.formLayout_5)
         self.graph_container = QtWidgets.QWidget(self.tab_6)
-        sizePolicy = QtWidgets.QSizePolicy(
-            QtWidgets.QSizePolicy.MinimumExpanding,
-            QtWidgets.QSizePolicy.MinimumExpanding,
-        )
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.MinimumExpanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(
-            self.graph_container.sizePolicy().hasHeightForWidth()
-        )
+        sizePolicy.setHeightForWidth(self.graph_container.sizePolicy().hasHeightForWidth())
         self.graph_container.setSizePolicy(sizePolicy)
         self.graph_container.setMinimumSize(QtCore.QSize(50, 0))
         self.graph_container.setToolTipDuration(0)
         self.graph_container.setObjectName("graph_container")
         self.verticalLayout_7.addWidget(self.graph_container)
         self.tabWidget.addTab(self.tab_6, "")
         self.verticalLayout.addWidget(self.tabWidget)
@@ -474,22 +378,18 @@
         self.label_12.setFont(font)
         self.label_12.setObjectName("label_12")
         self.verticalLayout.addWidget(self.label_12)
         self.formLayout_2 = QtWidgets.QFormLayout()
         self.formLayout_2.setObjectName("formLayout_2")
         self.label_14 = QtWidgets.QLabel(Frame)
         self.label_14.setObjectName("label_14")
-        self.formLayout_2.setWidget(
-            0, QtWidgets.QFormLayout.LabelRole, self.label_14
-        )
+        self.formLayout_2.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_14)
         self.dataset_selector = QtWidgets.QComboBox(Frame)
         self.dataset_selector.setObjectName("dataset_selector")
-        self.formLayout_2.setWidget(
-            0, QtWidgets.QFormLayout.FieldRole, self.dataset_selector
-        )
+        self.formLayout_2.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.dataset_selector)
         self.verticalLayout.addLayout(self.formLayout_2)
         self.gridLayout = QtWidgets.QGridLayout()
         self.gridLayout.setObjectName("gridLayout")
         self.show_dd = QtWidgets.QPushButton(Frame)
         self.show_dd.setText("")
         self.show_dd.setObjectName("show_dd")
         self.gridLayout.addWidget(self.show_dd, 0, 0, 1, 1)
@@ -520,115 +420,72 @@
         _translate = QtCore.QCoreApplication.translate
         Frame.setWindowTitle(_translate("Frame", "Frame"))
         self.label.setText(_translate("Frame", "Import Mode"))
         self.import_mode.setItemText(0, _translate("Frame", "FRET"))
         self.import_mode.setItemText(1, _translate("Frame", "Donor"))
         self.import_mode.setItemText(2, _translate("Frame", "Acceptor"))
         self.import_mode.setItemText(3, _translate("Frame", "ALEX"))
-        self.pixseq_channel_layout_label.setText(
-            _translate("Frame", "Channel Layout")
-        )
-        self.channel_layout.setItemText(
-            0, _translate("Frame", "Donor-Acceptor")
-        )
-        self.channel_layout.setItemText(
-            1, _translate("Frame", "Acceptor-Donor")
-        )
-        self.pixseq_alex_first_frame_label.setText(
-            _translate("Frame", "ALEX First Frame Excitation")
-        )
+        self.pixseq_channel_layout_label.setText(_translate("Frame", "Channel Layout"))
+        self.channel_layout.setItemText(0, _translate("Frame", "Donor-Acceptor"))
+        self.channel_layout.setItemText(1, _translate("Frame", "Acceptor-Donor"))
+        self.pixseq_alex_first_frame_label.setText(_translate("Frame", "ALEX First Frame Excitation"))
         self.alex_first_frame.setItemText(0, _translate("Frame", "Donor"))
         self.alex_first_frame.setItemText(1, _translate("Frame", "Acceptor"))
         self.label_32.setText(_translate("Frame", "Import Limit"))
         self.import_limt.setItemText(0, _translate("Frame", "None"))
         self.import_limt.setItemText(1, _translate("Frame", "10"))
         self.import_limt.setItemText(2, _translate("Frame", "50"))
         self.import_limt.setItemText(3, _translate("Frame", "100"))
         self.import_limt.setItemText(4, _translate("Frame", "200"))
         self.import_limt.setItemText(5, _translate("Frame", "300"))
         self.import_limt.setItemText(6, _translate("Frame", "400"))
         self.import_limt.setItemText(7, _translate("Frame", "500"))
         self.label_15.setText(_translate("Frame", "Pixel Size (um)"))
         self.import_data.setText(_translate("Frame", "Import"))
-        self.tabWidget.setTabText(
-            self.tabWidget.indexOf(self.tab), _translate("Frame", "Import")
-        )
-        self.label_3.setText(
-            _translate("Frame", "Detect Localisations (Picasso)")
-        )
-        self.label_7.setText(_translate("Frame", "Detect/Fit Mode"))
-        self.picasso_detect_mode.setItemText(
-            0, _translate("Frame", "Molecules")
-        )
-        self.picasso_detect_mode.setItemText(
-            1, _translate("Frame", "Bounding Boxes")
-        )
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab), _translate("Frame", "Import"))
+        self.label_3.setText(_translate("Frame", "Detect Localisations (Picasso)"))
         self.label_11.setText(_translate("Frame", "Dataset"))
         self.label_6.setText(_translate("Frame", "Channel"))
         self.label_8.setText(_translate("Frame", "Frame Mode"))
         self.picasso_frame_mode.setItemText(0, _translate("Frame", "Active"))
         self.picasso_frame_mode.setItemText(1, _translate("Frame", "All"))
-        self.label_5.setText(_translate("Frame", "Min Net Gradient"))
-        self.picasso_min_net_gradient.setText(_translate("Frame", "1000"))
         self.label_28.setText(_translate("Frame", "Box Size"))
         self.picasso_box_size.setItemText(0, _translate("Frame", "3"))
         self.picasso_box_size.setItemText(1, _translate("Frame", "5"))
         self.picasso_box_size.setItemText(2, _translate("Frame", "7"))
         self.picasso_box_size.setItemText(3, _translate("Frame", "9"))
+        self.label_5.setText(_translate("Frame", "Min Net Gradient"))
+        self.picasso_min_net_gradient.setText(_translate("Frame", "1000"))
         self.label_35.setText(_translate("Frame", "ROI Border Width (Pixels)"))
         self.picasso_roi_border_width.setText(_translate("Frame", "5"))
-        self.picasso_remove_overlapping.setText(
-            _translate(
-                "Frame",
-                "Remove Overlapping Fiducials/Bounding Boxes (determined by Picaso Box Size)",
-            )
-        )
-        self.picasso_window_cropping.setText(
-            _translate(
-                "Frame", "Remove Localisations Outside Field Of View (FOV)"
-            )
-        )
-        self.picasso_minimise_ram.setText(
-            _translate("Frame", "Minimise RAM usage")
-        )
+        self.picasso_remove_overlapping.setText(_translate("Frame", "Remove Overlapping Fiducials/Bounding Boxes (determined by Picaso Box Size)"))
+        self.picasso_window_cropping.setText(_translate("Frame", "Remove Localisations Outside Field Of View (FOV)"))
+        self.picasso_minimise_ram.setText(_translate("Frame", "Minimise RAM usage"))
         self.picasso_fit.setText(_translate("Frame", "Fit"))
         self.picasso_detect.setText(_translate("Frame", "Detect"))
         self.picasso_detectfit.setText(_translate("Frame", "Detect and Fit"))
-        self.tabWidget_2.setTabText(
-            self.tabWidget_2.indexOf(self.tab_3), _translate("Frame", "Detect")
-        )
+        self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_3), _translate("Frame", "Detect"))
         self.label_2.setText(_translate("Frame", "Render Fiducials (Picasso)"))
         self.label_4.setText(_translate("Frame", "Dataset"))
         self.label_9.setText(_translate("Frame", "Channel"))
         self.label_10.setText(_translate("Frame", "Blur Method"))
-        self.picasso_render_blur_method.setItemText(
-            0, _translate("Frame", "None")
-        )
-        self.picasso_render_blur_method.setItemText(
-            1, _translate("Frame", "One-Pixel-Blur")
-        )
-        self.picasso_render_blur_method.setItemText(
-            2, _translate("Frame", "Global Localisation Precision")
-        )
-        self.picasso_render_blur_method.setItemText(
-            3, _translate("Frame", "Individual Localisation Precision")
-        )
-        self.picasso_render_blur_method.setItemText(
-            4, _translate("Frame", "Individual Localisation Precision, iso")
-        )
+        self.picasso_render_blur_method.setItemText(0, _translate("Frame", "None"))
+        self.picasso_render_blur_method.setItemText(1, _translate("Frame", "One-Pixel-Blur"))
+        self.picasso_render_blur_method.setItemText(2, _translate("Frame", "Global Localisation Precision"))
+        self.picasso_render_blur_method.setItemText(3, _translate("Frame", "Individual Localisation Precision"))
+        self.picasso_render_blur_method.setItemText(4, _translate("Frame", "Individual Localisation Precision, iso"))
         self.label_13.setText(_translate("Frame", "Min. Blur (cam. pixel)"))
-        self.picasso_render.setText(
-            _translate("Frame", "Render Localisations")
-        )
-        self.tabWidget_2.setTabText(
-            self.tabWidget_2.indexOf(self.tab_5), _translate("Frame", "Render")
-        )
-        self.label_27.setText(
-            _translate("Frame", "Localisation Visualisation Settings")
-        )
+        self.picasso_render.setText(_translate("Frame", "Render Localisations"))
+        self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_5), _translate("Frame", "Render"))
+        self.label_74.setText(_translate("Frame", "Picasso HDF5 Localisations will be exported at the Dataset import directory"))
+        self.label_72.setText(_translate("Frame", "Dataset"))
+        self.label_71.setText(_translate("Frame", "Channel"))
+        self.export_locs.setText(_translate("Frame", "Export Localisations"))
+        self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_7), _translate("Frame", "Export Localisations"))
+        self.label_27.setText(_translate("Frame", "Localisation Visualisation Settings"))
         self.picasso_vis_size.setItemText(0, _translate("Frame", "1"))
         self.picasso_vis_size.setItemText(1, _translate("Frame", "2"))
         self.picasso_vis_size.setItemText(2, _translate("Frame", "3"))
         self.picasso_vis_size.setItemText(3, _translate("Frame", "4"))
         self.picasso_vis_size.setItemText(4, _translate("Frame", "5"))
         self.picasso_vis_size.setItemText(5, _translate("Frame", "6"))
         self.picasso_vis_size.setItemText(6, _translate("Frame", "7"))
@@ -658,26 +515,17 @@
         self.picasso_vis_edge_width.setItemText(3, _translate("Frame", "0.4"))
         self.picasso_vis_edge_width.setItemText(4, _translate("Frame", "0.5"))
         self.picasso_vis_edge_width.setItemText(5, _translate("Frame", "0.6"))
         self.picasso_vis_edge_width.setItemText(6, _translate("Frame", "0.7"))
         self.picasso_vis_edge_width.setItemText(7, _translate("Frame", "0.8"))
         self.picasso_vis_edge_width.setItemText(8, _translate("Frame", "0.9"))
         self.picasso_vis_edge_width.setItemText(9, _translate("Frame", "1.0"))
-        self.tabWidget_2.setTabText(
-            self.tabWidget_2.indexOf(self.tab_4),
-            _translate("Frame", "Visualisation Settings"),
-        )
-        self.tabWidget.setTabText(
-            self.tabWidget.indexOf(self.tab_2), _translate("Frame", "SMLM")
-        )
+        self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_4), _translate("Frame", "Visualisation Settings"))
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_2), _translate("Frame", "SMLM"))
         self.label_16.setText(_translate("Frame", "Plot Mode"))
         self.plot_mode.setItemText(0, _translate("Frame", "Line Profiles"))
-        self.plot_mode.setItemText(
-            1, _translate("Frame", "Single Molecule Time Series")
-        )
+        self.plot_mode.setItemText(1, _translate("Frame", "Single Molecule Time Series"))
         self.label_17.setText(_translate("Frame", "Plot Dataset"))
         self.label_18.setText(_translate("Frame", "Plot Channel"))
-        self.tabWidget.setTabText(
-            self.tabWidget.indexOf(self.tab_6), _translate("Frame", "Plots")
-        )
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_6), _translate("Frame", "Plots"))
         self.label_12.setText(_translate("Frame", "Display Mode"))
         self.label_14.setText(_translate("Frame", "Dataset [PageUp/PageDown]"))
```

### Comparing `napari_smlmlab-0.0.2/src/smlmlab/utils/compute_utils.py` & `napari_smlmlab-0.0.3/src/smlmlab/utils/compute_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.2/src/smlmlab/utils/events_utils.py` & `napari_smlmlab-0.0.3/src/smlmlab/utils/events_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     def update_ui(self, error=None, init=False):
         try:
             if self.verbose:
                 print(f"Updating UI, init = {init}")
 
             controls = ["import_data", "picasso_detect", "picasso_fit",
-                        "picasso_detectfit", "picasso_render"]
+                        "picasso_detectfit", "picasso_render", "export_locs"]
 
             progressbars = ["import_progressbar", "picasso_progressbar", ]
 
             for progressbar in progressbars:
                 if hasattr(self.gui, progressbar):
                     getattr(self.gui, progressbar).setValue(0)
 
@@ -342,14 +342,15 @@
         try:
             if self.verbose:
                 print("Populating channel selectors")
 
             self.update_channel_selector(dataset_selector="picasso_dataset", channel_selector="picasso_channel", )
             self.update_channel_selector(dataset_selector="picasso_render_dataset", channel_selector="picasso_render_channel", )
             self.update_channel_selector(dataset_selector="plot_dataset", channel_selector="plot_channel", efficiency=True, )
+            self.update_channel_selector(dataset_selector="locs_export_dataset", channel_selector="locs_export_channel", efficiency=True, )
 
         except:
             print(traceback.format_exc())
 
     def update_channel_select_buttons(self):
         try:
             datast_name = self.gui.dataset_selector.currentText()
@@ -637,13 +638,10 @@
         self.slider = self.findChild(QSlider, slider_name)
         self.label = self.findChild(QLabel, label_name)
 
         slider_value = self.slider.value()
         self.label.setText(str(slider_value))
 
     def update_picasso_options(self):
-        if self.picasso_detect_mode.currentText() == "Molecules":
-            self.picasso_frame_mode.clear()
-            self.picasso_frame_mode.addItems(["Active", "All"])
-        else:
-            self.picasso_frame_mode.clear()
-            self.picasso_frame_mode.addItem("Active")
+
+        self.picasso_frame_mode.clear()
+        self.picasso_frame_mode.addItems(["Active", "All"])
```

### Comparing `napari_smlmlab-0.0.2/src/smlmlab/utils/import_utils.py` & `napari_smlmlab-0.0.3/src/smlmlab/utils/import_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,36 +21,30 @@
         channel_list = dat["channel_list"]
         channel_frame_list = dat["channel_frame_list"]
         channel_images = dat["channel_images"]
 
         n_frames = len(frame_list)
 
         with Image.open(path) as image:
-            for frame_index, channels, channel_frame in zip(
-                frame_list, channel_list, channel_frame_list
-            ):
+            for frame_index, channels, channel_frame in zip(frame_list, channel_list, channel_frame_list):
                 image_shape = dat["image_shape"]
                 stop_event = dat["stop_event"]
 
                 if not stop_event.is_set():
                     image.seek(frame_index)
                     img_frame = np.array(image)
 
                     if len(channels) == 1:
                         img_frames = [img_frame]
                     else:
                         img_frames = np.array_split(img_frame, 2, axis=-1)
 
                     for channel, channel_img in zip(channels, img_frames):
                         shared_mem = channel_images[channel]
-                        np_array = np.ndarray(
-                            image_shape,
-                            dtype=dat["dtype"],
-                            buffer=shared_mem.buf,
-                        )
+                        np_array = np.ndarray(image_shape, dtype=dat["dtype"], buffer=shared_mem.buf, )
                         np_array[channel_frame] = channel_img
 
                 progress = int(((frame_index + 1) / n_frames) * 100)
                 progress_dict[index] = progress
 
     except:
         print(traceback.format_exc())
@@ -61,25 +55,22 @@
     def create_import_shared_image(self, image_size):
         shared_mem = None
 
         try:
             if self.verbose:
                 print("Creating shared image...")
 
-            shared_mem = shared_memory.SharedMemory(
-                create=True, size=image_size
-            )
+            shared_mem = shared_memory.SharedMemory(create=True, size=image_size)
 
         except:
             print(traceback.format_exc())
 
         return shared_mem
 
     def get_image_info(self, path):
-
         if self.verbose:
             print(f"Getting image info for {path}")
 
         image_size = os.path.getsize(path)  # Get file size directly
 
         with tifffile.TiffFile(path) as tif:
             n_frames = len(tif.pages)  # Number of pages (frames)
@@ -124,85 +115,50 @@
             import_mode = self.gui.import_mode.currentText()
             import_limit_combo = self.gui.import_limt.currentText()
             channel_layout = self.gui.channel_layout.currentText()
             alex_first_frame = self.gui.alex_first_frame.currentText()
             pixel_size = self.gui.pixel_size.text()
 
             for path_index, path in enumerate(paths):
-
                 path = self.format_import_path(path)
                 file_name = os.path.basename(path)
 
                 dataset_name = file_name
 
                 if dataset_name not in shared_images:
                     shared_images[dataset_name] = {}
 
-                n_frames, image_shape, dtype, image_size = self.get_image_info(
-                    path
-                )
-
-                if import_mode.lower() in [
-                    "donor",
-                    "acceptor",
-                    "dd",
-                    "da",
-                    "ad",
-                    "aa",
-                ]:
+                n_frames, image_shape, dtype, image_size = self.get_image_info(path)
+
+                if import_mode.lower() in ["donor", "acceptor", "dd", "da", "ad", "aa", ]:
                     if import_limit_combo != "None":
-                        import_limit = int(
-                            self.pixseq_import_limt.currentText()
-                        )
+                        import_limit = int(self.pixseq_import_limt.currentText())
                     else:
                         import_limit = n_frames
 
-                    image_shape = (
-                        import_limit,
-                        image_shape[1],
-                        image_shape[2],
-                    )
+                    image_shape = (import_limit, image_shape[1], image_shape[2],)
 
                     frame_list = list(range(n_frames))[:import_limit]
 
                     unique_frames = np.unique(frame_list)
                     n_frames = len(unique_frames)
 
                     channel_names = [import_mode.lower()]
                     channel_list = [channel_names] * n_frames
 
                     channel_images = {}
                     for channel in channel_names:
                         if self.verbose:
-                            print(
-                                f"Creating image memory for {dataset_name} {channel}..."
-                            )
-
-                        shared_image = self.create_import_shared_image(
-                            image_size
-                        )
+                            print(f"Creating image memory for {dataset_name} {channel}...")
+
+                        shared_image = self.create_import_shared_image(image_size)
                         channel_images[channel] = shared_image
                         shared_images[dataset_name][channel] = shared_image
 
-                    image_dict = {
-                        "path": path,
-                        "dataset_name": dataset_name,
-                        "n_frames": n_frames,
-                        "pixel_size": pixel_size,
-                        "channel_names": channel_names,
-                        "channel_list": channel_list,
-                        "frame_list": frame_list,
-                        "channel_frame_list": frame_list,
-                        "channel_images": channel_images,
-                        "image_shape": image_shape,
-                        "channel_layout": channel_layout,
-                        "alex_first_frame": alex_first_frame,
-                        "dtype": dtype,
-                        "import_mode": import_mode.lower(),
-                    }
+                    image_dict = {"path": path, "dataset_name": dataset_name, "n_frames": n_frames, "pixel_size": pixel_size, "channel_names": channel_names, "channel_list": channel_list, "frame_list": frame_list, "channel_frame_list": frame_list, "channel_images": channel_images, "image_shape": image_shape, "channel_layout": channel_layout, "alex_first_frame": alex_first_frame, "dtype": dtype, "import_mode": import_mode.lower(), }
 
                     image_list.append(image_dict)
 
                 elif import_mode.lower() == "fret":
                     if import_limit_combo != "None":
                         import_limit = int(self.gui.import_limt.currentText())
                     else:
@@ -211,84 +167,51 @@
                     frame_list = list(range(n_frames))[:import_limit]
 
                     if channel_layout.lower() == "donor-acceptor":
                         channel_names = ["donor", "acceptor"]
                     else:
                         channel_names = ["acceptor", "donor"]
 
-                    image_shape = (
-                        import_limit,
-                        image_shape[1],
-                        image_shape[2] // 2,
-                    )
+                    image_shape = (import_limit, image_shape[1], image_shape[2] // 2,)
 
                     unique_frames = np.unique(frame_list)
                     n_frames = len(unique_frames)
 
                     channel_list = [channel_names] * n_frames
 
                     channel_images = {}
                     for channel in channel_names:
                         if self.verbose:
-                            print(
-                                f"Creating shared image for {dataset_name} {channel}..."
-                            )
-
-                        shared_image = self.create_import_shared_image(
-                            image_size // 2
-                        )
+                            print(f"Creating shared image for {dataset_name} {channel}...")
+
+                        shared_image = self.create_import_shared_image(image_size // 2)
                         channel_images[channel] = shared_image
                         shared_images[dataset_name][channel] = shared_image
 
-                    image_dict = {
-                        "path": path,
-                        "dataset_name": dataset_name,
-                        "n_frames": n_frames,
-                        "pixel_size": pixel_size,
-                        "channel_names": channel_names,
-                        "channel_list": channel_list,
-                        "frame_list": frame_list,
-                        "channel_frame_list": frame_list,
-                        "channel_images": channel_images,
-                        "image_shape": image_shape,
-                        "channel_layout": channel_layout,
-                        "alex_first_frame": alex_first_frame,
-                        "dtype": dtype,
-                        "import_mode": import_mode.lower(),
-                    }
+                    image_dict = {"path": path, "dataset_name": dataset_name, "n_frames": n_frames, "pixel_size": pixel_size, "channel_names": channel_names, "channel_list": channel_list, "frame_list": frame_list, "channel_frame_list": frame_list, "channel_images": channel_images, "image_shape": image_shape, "channel_layout": channel_layout, "alex_first_frame": alex_first_frame, "dtype": dtype, "import_mode": import_mode.lower(), }
 
                     image_list.append(image_dict)
 
                 elif import_mode.lower() == "alex":
                     if import_limit_combo != "None":
-                        import_limit = int(
-                            self.pixseq_import_limt.currentText()
-                        )
+                        import_limit = int(self.pixseq_import_limt.currentText())
                     else:
                         import_limit = n_frames
 
                     frame_list = list(range(n_frames))
 
                     even_frames = frame_list[::2][:import_limit]
                     odd_frames = frame_list[1::2][:import_limit]
 
-                    frame_list = np.unique(
-                        np.concatenate([even_frames, odd_frames])
-                    )
+                    frame_list = np.unique(np.concatenate([even_frames, odd_frames]))
                     frame_list = np.sort(frame_list).tolist()
-                    channel_frame_list = np.repeat(
-                        np.arange(len(frame_list) // 2), 2
-                    )
+                    channel_frame_list = np.repeat(np.arange(len(frame_list) // 2), 2)
 
                     n_frames = len(frame_list)
-                    image_shape = (
-                        n_frames // 2,
-                        image_shape[1],
-                        image_shape[2] // 2,
-                    )
+                    image_shape = (n_frames // 2, image_shape[1], image_shape[2] // 2,)
 
                     channel_list = []
 
                     for frame in frame_list:
                         if frame % 2 == 0:
                             if alex_first_frame.lower() == "donor":
                                 channel_ex = "d"
@@ -297,74 +220,40 @@
                         else:
                             if alex_first_frame.lower() == "donor":
                                 channel_ex = "a"
                             else:
                                 channel_ex = "d"
 
                         if channel_layout.lower() == "donor-acceptor":
-                            channel_names = [
-                                f"{channel_ex}d",
-                                f"{channel_ex}a",
-                            ]
+                            channel_names = [f"{channel_ex}d", f"{channel_ex}a", ]
                         else:
-                            channel_names = [
-                                f"{channel_ex}a",
-                                f"{channel_ex}d",
-                            ]
+                            channel_names = [f"{channel_ex}a", f"{channel_ex}d", ]
 
                         channel_list.append(channel_names)
 
                     channel_names = np.unique(channel_list)
 
                     channel_images = {}
                     for channel in channel_names:
                         if self.verbose:
-                            print(
-                                f"Creating shared memory for {dataset_name} {channel}..."
-                            )
-
-                        shared_image = self.create_import_shared_image(
-                            image_size // 4
-                        )
+                            print(f"Creating shared memory for {dataset_name} {channel}...")
+
+                        shared_image = self.create_import_shared_image(image_size // 4)
                         channel_images[channel] = shared_image
                         shared_images[dataset_name][channel] = shared_image
 
-                    image_dict = {
-                        "path": path,
-                        "dataset_name": dataset_name,
-                        "n_frames": n_frames,
-                        "pixel_size": pixel_size,
-                        "channel_names": channel_names,
-                        "channel_list": channel_list,
-                        "frame_list": frame_list,
-                        "channel_frame_list": channel_frame_list,
-                        "channel_images": channel_images,
-                        "image_shape": image_shape,
-                        "channel_layout": channel_layout,
-                        "alex_first_frame": alex_first_frame,
-                        "dtype": dtype,
-                        "import_mode": import_mode.lower(),
-                    }
+                    image_dict = {"path": path, "dataset_name": dataset_name, "n_frames": n_frames, "pixel_size": pixel_size, "channel_names": channel_names, "channel_list": channel_list, "frame_list": frame_list, "channel_frame_list": channel_frame_list, "channel_images": channel_images, "image_shape": image_shape, "channel_layout": channel_layout, "alex_first_frame": alex_first_frame, "dtype": dtype, "import_mode": import_mode.lower(), }
 
                     image_list.append(image_dict)
 
                 channel_layout = self.gui.channel_layout.currentText()
                 alex_first_frame = self.gui.alex_first_frame.currentText()
 
                 if dataset_name not in import_dict:
-                    import_dict[dataset_name] = {
-                        "path": path,
-                        "pixel_size": pixel_size,
-                        "import_mode": import_mode.lower(),
-                        "import_limit": import_limit,
-                        "channel_layout": channel_layout,
-                        "alex_first_frame": alex_first_frame,
-                        "image_shape": image_shape,
-                        "dtype": dtype,
-                    }
+                    import_dict[dataset_name] = {"path": path, "pixel_size": pixel_size, "import_mode": import_mode.lower(), "import_limit": import_limit, "channel_layout": channel_layout, "alex_first_frame": alex_first_frame, "image_shape": image_shape, "dtype": dtype, }
         except:
             print(traceback.format_exc())
 
         return image_list, shared_images, import_dict
 
     def populate_import_compute_jobs(self, image_list):
         if self.verbose:
@@ -373,44 +262,31 @@
         compute_jobs = []
 
         for image_dict in image_list:
             frame_list = np.unique(image_dict["frame_list"])
             channel_list = image_dict["channel_list"]
             channel_frame_list = image_dict["channel_frame_list"]
 
-            compute_jobs.append(
-                {
-                    "frame_list": frame_list,
-                    "channel_list": channel_list,
-                    "channel_frame_list": channel_frame_list,
-                    "stop_event": self.stop_event,
-                    **image_dict,
-                }
-            )
+            compute_jobs.append({"frame_list": frame_list, "channel_list": channel_list, "channel_frame_list": channel_frame_list, "stop_event": self.stop_event, **image_dict, })
 
         return compute_jobs
 
     def process_compute_jobs(self, compute_jobs, progress_callback=None):
         if self.verbose:
             print(f"Processing {len(compute_jobs)} compute jobs.")
 
         cpu_count = int(multiprocessing.cpu_count() * 0.75)
         timeout_duration = 10  # Timeout in seconds
 
         with Manager() as manager:
             progress_dict = manager.dict()
 
-            with concurrent.futures.ProcessPoolExecutor(
-                max_workers=cpu_count
-            ) as executor:
+            with concurrent.futures.ProcessPoolExecutor(max_workers=cpu_count) as executor:
                 # Submit all jobs and store the future objects
-                futures = [
-                    executor.submit(import_image_data, job, progress_dict, i)
-                    for i, job in enumerate(compute_jobs)
-                ]
+                futures = [executor.submit(import_image_data, job, progress_dict, i) for i, job in enumerate(compute_jobs)]
 
                 while any(not future.done() for future in futures):
                     # Calculate and emit progress
                     total_progress = sum(progress_dict.values())
                     overall_progress = int(total_progress / len(compute_jobs))
                     if progress_callback is not None:
                         progress_callback.emit(overall_progress)
@@ -442,17 +318,15 @@
                 pixel_size = dataset_dict["pixel_size"]
 
                 dataset_images = self.shared_images[dataset_name]
 
                 channel_names = dataset_images.keys()
 
                 for channel_name, shared_mem in dataset_images.items():
-                    image = np.ndarray(
-                        image_shape, dtype=dtype, buffer=shared_mem.buf
-                    ).copy()
+                    image = np.ndarray(image_shape, dtype=dtype, buffer=shared_mem.buf).copy()
                     image = image.astype(np.uint16)
 
                     shared_mem.close()
                     shared_mem.unlink()
 
                     if channel_name not in image_dict:
                         image_dict[channel_name] = {"data": []}
@@ -481,30 +355,26 @@
 
                     image_dict[channel_name]["data"] = image
                     image_dict[channel_name]["path"] = path
                     image_dict[channel_name]["channel_ref"] = channel_ref
                     image_dict[channel_name]["excitation"] = excitation
                     image_dict[channel_name]["emission"] = emission
                     image_dict[channel_name]["channel_layout"] = channel_layout
-                    image_dict[channel_name][
-                        "alex_first_frame"
-                    ] = alex_first_frame
+                    image_dict[channel_name]["alex_first_frame"] = alex_first_frame
                     image_dict[channel_name]["FRET"] = fret
                     image_dict[channel_name]["import_mode"] = import_mode
                     image_dict[channel_name]["gap_label"] = None
                     image_dict[channel_name]["sequence_label"] = None
                     image_dict[channel_name]["pixel_size"] = pixel_size
 
                 if dataset_name not in self.dataset_dict.keys():
                     self.dataset_dict[dataset_name] = image_dict
                 else:
                     for channel_name, channel_dict in image_dict.items():
-                        self.dataset_dict[dataset_name][
-                            channel_name
-                        ] = channel_dict
+                        self.dataset_dict[dataset_name][channel_name] = channel_dict
 
         except:
             pass
 
     def closed_import_shared_images(self):
         if hasattr(self, "shared_images"):
             if self.verbose:
@@ -513,23 +383,19 @@
             for dataset_name, dataset_dict in self.shared_images.items():
                 for channel_name, shared_mem in dataset_dict.items():
                     shared_mem.close()
                     shared_mem.unlink()
 
     def _pixseq_import_data(self, progress_callback=None, paths=[]):
         try:
-            image_list, self.shared_images, import_dict = (
-                self.populate_import_lists(paths=paths)
-            )
+            image_list, self.shared_images, import_dict = (self.populate_import_lists(paths=paths))
 
             compute_jobs = self.populate_import_compute_jobs(image_list)
 
-            self.process_compute_jobs(
-                compute_jobs, progress_callback=progress_callback
-            )
+            self.process_compute_jobs(compute_jobs, progress_callback=progress_callback)
 
             self.populate_import_dataset_dict(import_dict)
 
             self.closed_import_shared_images()
 
         except:
             print(traceback.format_exc())
@@ -561,14 +427,19 @@
             self.gui.picasso_render_dataset.blockSignals(False)
 
             self.gui.plot_dataset.blockSignals(True)
             self.gui.plot_dataset.clear()
             self.gui.plot_dataset.addItems(dataset_names)
             self.gui.plot_dataset.blockSignals(False)
 
+            self.gui.locs_export_dataset.blockSignals(True)
+            self.gui.locs_export_dataset.clear()
+            self.gui.locs_export_dataset.addItems(dataset_names)
+            self.gui.locs_export_dataset.blockSignals(False)
+
         except:
             print(traceback.format_exc())
 
     def initialise_localisation_dict(self):
         if hasattr(self, "localisation_dict"):
             self.localisation_dict = {"bounding_boxes": {}, "molecules": {}}
 
@@ -576,25 +447,21 @@
             if self.verbose:
                 print("Initialising localisation dict.")
 
             for dataset_name, dataset_dict in self.dataset_dict.items():
                 if dataset_name not in self.localisation_dict.keys():
                     self.localisation_dict["molecules"][dataset_name] = {}
 
-                molecule_dict = self.localisation_dict["molecules"][
-                    dataset_name
-                ]
+                molecule_dict = self.localisation_dict["molecules"][dataset_name]
 
                 for channel_name, channel_dict in dataset_dict.items():
                     if channel_name not in molecule_dict.keys():
                         molecule_dict[channel_name.lower()] = {}
 
-                self.localisation_dict["molecules"][
-                    dataset_name
-                ] = molecule_dict
+                self.localisation_dict["molecules"][dataset_name] = molecule_dict
 
     def _pixseq_import_data_finished(self):
         if self.verbose:
             print("Finished importing data, executing post import functions")
 
         self.initialise_localisation_dict()
         self.populate_dataset_combos()
@@ -604,31 +471,22 @@
         self.update_active_image()
 
         self.update_ui()
 
     def import_image_data(self):
         try:
             desktop = os.path.expanduser("~/Desktop")
-            paths = QFileDialog.getOpenFileNames(
-                self, "Open file", desktop, "Image files (*.tif *.tiff)"
-            )[0]
+            paths = QFileDialog.getOpenFileNames(self, "Open file", desktop, "Image files (*.tif *.tiff)")[0]
 
             paths = [path for path in paths if path != ""]
 
             if paths != []:
                 self.update_ui(init=True)
 
                 self.worker = Worker(self._pixseq_import_data, paths=paths)
-                self.worker.signals.progress.connect(
-                    partial(
-                        self.pixseq_progress,
-                        progress_bar=self.gui.import_progressbar,
-                    )
-                )
-                self.worker.signals.finished.connect(
-                    self._pixseq_import_data_finished
-                )
+                self.worker.signals.progress.connect(partial(self.pixseq_progress, progress_bar=self.gui.import_progressbar, ))
+                self.worker.signals.finished.connect(self._pixseq_import_data_finished)
                 # self.worker.signals.error.connect(self.update_ui)
                 self.threadpool.start(self.worker)
 
         except:
             self.update_ui()
```

### Comparing `napari_smlmlab-0.0.2/src/smlmlab/utils/loc_utils.py` & `napari_smlmlab-0.0.3/src/smlmlab/utils/loc_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import concurrent
 import os
 import shutil
 import tempfile
 import traceback
 from functools import partial
 from pathlib import Path
-
+import pandas as pd
 import h5py
 import numpy as np
 import yaml
 from qtpy.QtWidgets import QFileDialog
 
 from smlmlab.utils.compute_utils import Worker
 
@@ -17,81 +17,58 @@
 class picasso_loc_utils:
 
     def __init__(self, locs: np.recarray = None, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.locs = locs
 
-        self.detected_dtype = [
-            ("frame", "<i4"),
-            ("x", "<i4"),
-            ("y", "<i4"),
-            ("net_gradient", "<f4"),
-        ]
-
-        self.fitted_dtype = [
-            ("frame", "<u4"),
-            ("x", "<f4"),
-            ("y", "<f4"),
-            ("photons", "<f4"),
-            ("sx", "<f4"),
-            ("sy", "<f4"),
-            ("bg", "<f4"),
-            ("lpx", "<f4"),
-            ("lpy", "<f4"),
-            ("ellipticity", "<f4"),
-            ("net_gradient", "<f4"),
-        ]
+        self.detected_dtype = [("frame", "<i4"), ("x", "<i4"), ("y", "<i4"), ("net_gradient", "<f4"), ]
+
+        self.fitted_dtype = [("frame", "<u4"), ("x", "<f4"), ("y", "<f4"), ("photons", "<f4"), ("sx", "<f4"), ("sy", "<f4"), ("bg", "<f4"), ("lpx", "<f4"), ("lpy", "<f4"), ("ellipticity", "<f4"), ("net_gradient", "<f4"), ]
 
         if self.locs is not None:
             self.get_loc_info()
 
     def get_loc_info(self):
-
         self.dtype = self.locs.dtype
         self.columns = self.locs.dtype.names
 
         if self.locs.dtype == self.fitted_dtype:
             self.loc_type = "molecule"
         else:
             self.loc_type = "bbox"
 
     def coerce_new_loc_format(self, new_loc):
-
         if len(new_loc) != len(self.dtype):
             difference = len(self.dtype) - len(new_loc)
             if difference > 0:
                 new_loc = list(new_loc)
                 for i in range(difference):
                     new_loc = new_loc + [0]
                 new_loc = tuple(new_loc)
 
         return new_loc
 
     def remove_duplicate_locs(self, locs=None):
-
         try:
-
             if locs is not None:
                 self.locs = locs
                 self.get_loc_info()
 
             unique_records, indices = np.unique(self.locs, return_index=True)
 
             self.locs = self.locs[indices]
 
         except:
             print(traceback.format_exc())
 
         return locs
 
     def add_loc(self, locs=None, new_loc=None):
-
         try:
-
             if locs is not None:
                 self.locs = locs
                 self.get_loc_info()
 
             if type(new_loc) == list:
                 new_loc = tuple(new_loc)
             if type(new_loc) in [np.ndarray, np.recarray]:
@@ -107,43 +84,35 @@
 
         except:
             print(traceback.format_exc())
 
         return self.locs
 
     def remove_loc(self, locs=None, loc_index=None):
-
         try:
-
             if locs is not None:
                 self.locs = locs
                 self.get_loc_info()
 
             if loc_index is not None:
-
                 if loc_index < len(self.locs):
-
-                    self.locs = self.locs.view(np.float32).reshape(
-                        len(self.locs), -1
-                    )
+                    self.locs = self.locs.view(np.float32).reshape(len(self.locs), -1)
                     self.locs = np.delete(self.locs, loc_index, axis=0)
                     self.locs = self.locs.view(self.dtype)
                     self.locs = np.squeeze(self.locs, axis=1)
 
                 self.remove_duplicate_locs()
 
         except:
             print(traceback.format_exc())
 
         return self.locs
 
     def create_locs(self, new_loc, fitted=False):
-
         try:
-
             if fitted == False:
                 dtype = self.detected_dtype
             else:
                 dtype = self.fitted_dtype
 
             if type(new_loc) == list:
                 new_loc = [tuple(new_loc)]
@@ -157,15 +126,14 @@
         except:
             print(traceback.format_exc())
 
         return self.locs
 
 
 def format_picasso_path(path):
-
     if "%" in str(path):
         path = path.replace("%", "%%")
 
     path = os.path.normpath(path)
 
     if os.name == "nt":
         if path.startswith("\\\\"):
@@ -176,275 +144,208 @@
 
 def export_picasso_localisation(loc_data):
 
     try:
         locs = loc_data["locs"]
         h5py_path = loc_data["hdf5_path"]
         yaml_path = loc_data["info_path"]
+        csv_path = loc_data["csv_path"]
         info = loc_data["picasso_info"]
 
+        locs_df = pd.DataFrame(locs)
+
         h5py_path = format_picasso_path(h5py_path)
         yaml_path = format_picasso_path(yaml_path)
+        csv_path = format_picasso_path(csv_path)
 
         # Create temporary files
         temp_h5py_path = tempfile.NamedTemporaryFile(delete=False).name
         temp_yaml_path = tempfile.NamedTemporaryFile(delete=False).name
+        temp_csv_path = tempfile.NamedTemporaryFile(delete=False).name
 
         h5py_path.parent.mkdir(parents=True, exist_ok=True)
         yaml_path.parent.mkdir(parents=True, exist_ok=True)
+        csv_path.parent.mkdir(parents=True, exist_ok=True)
 
         # Save to temporary HDF5 file
         with h5py.File(temp_h5py_path, "w") as hdf_file:
             hdf_file.create_dataset("locs", data=locs)
 
         # Save to temporary YAML file
         with open(temp_yaml_path, "w") as file:
             yaml.dump_all(info, file, default_flow_style=False)
 
+        # Save to temporary TXT file
+        locs_df.to_csv(temp_csv_path, sep=",", index=False)
+
         try:
             shutil.move(temp_h5py_path, h5py_path)
             shutil.move(temp_yaml_path, yaml_path)
+            shutil.move(temp_csv_path, csv_path)
         except:
+            print("Could not move files to import directory. Saving to desktop instead.")
 
-            print(
-                "Could not move files to import directory. Saving to desktop instead."
-            )
-
-            desktop_dir = os.path.join(
-                os.path.join(os.environ["USERPROFILE"]), "Desktop"
-            )
+            desktop_dir = os.path.join(os.path.join(os.environ["USERPROFILE"]), "Desktop")
 
             desktop_h5py_path = os.path.join(desktop_dir, h5py_path.name)
             desktop_yaml_path = os.path.join(desktop_dir, yaml_path.name)
 
             shutil.move(temp_h5py_path, desktop_h5py_path)
             shutil.move(temp_yaml_path, desktop_yaml_path)
 
     except Exception:
         print(traceback.format_exc())
 
 
 class _loc_utils:
 
     def _import_picasso_localisations_finished(self):
-
         try:
             self.update_ui()
 
             self.draw_molecules(update_vis=True)
             self.draw_bounding_boxes(update_vis=True)
 
         except:
             print(traceback.format_exc())
 
     def _import_picasso_localisations(self, progress_callback=None, path=""):
-
         try:
-
             dataset = self.import_picasso_dataset.currentText()
             channel = self.import_picasso_channel.currentText()
             type = self.import_picasso_type.currentText()
 
             if type == "Molecules":
                 if dataset not in self.localisation_dict["molecules"].keys():
                     self.localisation_dict["molecules"][dataset] = {}
-                if (
-                    channel.lower()
-                    not in self.localisation_dict["molecules"][dataset].keys()
-                ):
-                    self.localisation_dict["molecules"][dataset][
-                        channel.lower()
-                    ] = {}
+                if (channel.lower() not in self.localisation_dict["molecules"][dataset].keys()):
+                    self.localisation_dict["molecules"][dataset][channel.lower()] = {}
 
             yaml_path = path.replace(".hdf5", ".yaml")
 
-            dtype = [
-                ("frame", "<u4"),
-                ("x", "<f4"),
-                ("y", "<f4"),
-                ("photons", "<f4"),
-                ("sx", "<f4"),
-                ("sy", "<f4"),
-                ("bg", "<f4"),
-                ("lpx", "<f4"),
-                ("lpy", "<f4"),
-                ("ellipticity", "<f4"),
-                ("net_gradient", "<f4"),
-            ]
+            dtype = [("frame", "<u4"), ("x", "<f4"), ("y", "<f4"), ("photons", "<f4"), ("sx", "<f4"), ("sy", "<f4"), ("bg", "<f4"), ("lpx", "<f4"), ("lpy", "<f4"), ("ellipticity", "<f4"), ("net_gradient", "<f4"), ]
 
             if self.verbose:
                 print("Loading localisations from hdf5")
 
             with h5py.File(path, "r") as f:
-                locs = np.array(f["locs"], dtype=dtype).view(np.recarray)
-                # print(locs.dtype.descr)
-                # print(len(locs[0]))
+                locs = np.array(f["locs"], dtype=dtype).view(np.recarray)  # print(locs.dtype.descr)  # print(len(locs[0]))
 
             box_size = self.picasso_box_size.currentText()
 
             if self.verbose:
                 print("Loading localisations from yaml")
 
             if os.path.exists(yaml_path):
                 with open(yaml_path) as info_file:
-                    info = list(
-                        yaml.load_all(info_file, Loader=yaml.UnsafeLoader)
-                    )
+                    info = list(yaml.load_all(info_file, Loader=yaml.UnsafeLoader))
 
                 if "Box Size" in info[1].keys():
                     box_size = info[1]["Box Size"]
 
             if type == "Molecules":
-
                 if self.verbose:
                     print("Creating render locs")
 
                 render_locs = {}
                 for frame in np.unique(locs.frame):
                     frame_locs = locs[locs.frame == frame].copy()
-                    render_locs[frame] = np.vstack(
-                        (frame_locs.y, frame_locs.x)
-                    ).T.tolist()
+                    render_locs[frame] = np.vstack((frame_locs.y, frame_locs.x)).T.tolist()
 
                 loc_centres = self.get_localisation_centres(locs)
 
                 if self.verbose:
                     print("Updating localisation dict")
 
-                self.localisation_dict["molecules"][dataset][channel.lower()][
-                    "localisations"
-                ] = locs.copy()
-                self.localisation_dict["molecules"][dataset][channel.lower()][
-                    "localisation_centres"
-                ] = loc_centres.copy()
-                self.localisation_dict["molecules"][dataset][channel.lower()][
-                    "render_locs"
-                ] = render_locs
-                self.localisation_dict["molecules"][dataset][channel.lower()][
-                    "fitted"
-                ] = True
-                self.localisation_dict["molecules"][dataset][channel.lower()][
-                    "box_size"
-                ] = box_size
+                self.localisation_dict["molecules"][dataset][channel.lower()]["localisations"] = locs.copy()
+                self.localisation_dict["molecules"][dataset][channel.lower()]["localisation_centres"] = loc_centres.copy()
+                self.localisation_dict["molecules"][dataset][channel.lower()]["render_locs"] = render_locs
+                self.localisation_dict["molecules"][dataset][channel.lower()]["fitted"] = True
+                self.localisation_dict["molecules"][dataset][channel.lower()]["box_size"] = box_size
 
             else:
                 unique_frames = np.unique(locs.frame)
                 locs = locs[locs.frame == unique_frames[0]]
 
                 loc_centres = self.get_localisation_centres(locs)
 
                 if self.verbose:
                     print("Updating localisation dict")
 
-                self.localisation_dict["bounding_boxes"][
-                    "localisations"
-                ] = locs.copy()
-                self.localisation_dict["bounding_boxes"][
-                    "localisation_centres"
-                ] = loc_centres.copy()
+                self.localisation_dict["bounding_boxes"]["localisations"] = locs.copy()
+                self.localisation_dict["bounding_boxes"]["localisation_centres"] = loc_centres.copy()
                 self.localisation_dict["bounding_boxes"]["render_locs"] = {}
                 self.localisation_dict["bounding_boxes"]["fitted"] = True
                 self.localisation_dict["bounding_boxes"]["box_size"] = box_size
 
         except:
             print(traceback.format_exc())
 
     def import_picaaso_localisations(self):
-
         try:
-
             dataset = self.import_picasso_dataset.currentText()
             channel = self.import_picasso_channel.currentText()
             type = self.import_picasso_type.currentText()
 
             if dataset in self.dataset_dict.keys():
                 if channel.lower() in self.dataset_dict[dataset].keys():
-
-                    dataset_path = self.dataset_dict[dataset][channel.lower()][
-                        "path"
-                    ]
+                    dataset_path = self.dataset_dict[dataset][channel.lower()]["path"]
 
                     dataset_dir = os.path.dirname(dataset_path)
 
                     if os.path.exists(dataset_dir) == False:
                         dataset_dir = os.path.expanduser("~/Desktop")
 
-                    path, _ = QFileDialog.getOpenFileName(
-                        self, "Open Files", dataset_dir, "Files (*.hdf5)"
-                    )
+                    path, _ = QFileDialog.getOpenFileName(self, "Open Files", dataset_dir, "Files (*.hdf5)")
 
                     if path != "":
-
                         path = self.format_import_path(path)
 
                         if os.path.exists(path):
-
                             self.update_ui(init=True)
 
-                            self.worker = Worker(
-                                self._import_picasso_localisations, path=path
-                            )
-                            self.worker.signals.finished.connect(
-                                self._import_picasso_localisations_finished
-                            )
+                            self.worker = Worker(self._import_picasso_localisations, path=path)
+                            self.worker.signals.finished.connect(self._import_picasso_localisations_finished)
                             self.threadpool.start(self.worker)
         except:
             self.update_ui()
             print(traceback.format_exc())
 
     def update_loc_export_options(self):
-
         try:
-
             dataset_name = self.locs_export_dataset.currentText()
 
-            if (
-                dataset_name in self.dataset_dict.keys()
-                or dataset_name == "All Datasets"
-            ):
-
+            if (dataset_name in self.dataset_dict.keys() or dataset_name == "All Datasets"):
                 if dataset_name == "All Datasets":
                     channel_names = ["All Channels"]
                 else:
-                    channel_names = list(
-                        self.dataset_dict[dataset_name].keys()
-                    )
-                    channel_names = [
-                        name
-                        for name in channel_names
-                        if "efficiency" not in name.lower()
-                    ]
-
-                    for channel_index, channel_name in enumerate(
-                        channel_names
-                    ):
+                    channel_names = list(self.dataset_dict[dataset_name].keys())
+                    channel_names = [name for name in channel_names if "efficiency" not in name.lower()]
+
+                    for channel_index, channel_name in enumerate(channel_names):
                         if channel_name in ["donor", "acceptor"]:
-                            channel_names[channel_index] = (
-                                channel_name.capitalize()
-                            )
+                            channel_names[channel_index] = (channel_name.capitalize())
                         else:
                             channel_names[channel_index] = channel_name.upper()
 
                     channel_names.insert(0, "All Channels")
 
                 self.locs_export_channel.blockSignals(True)
                 self.locs_export_channel.clear()
                 self.locs_export_channel.addItems(channel_names)
                 self.locs_export_channel.blockSignals(False)
 
         except:
             print(traceback.format_exc())
 
-    def export_locs(
-        self, progress_callback=None, export_dataset="", export_channel=""
-    ):
+    def export_locs(self, progress_callback=None, export_dataset="", export_channel="",
+            export_loc_mode="Molecules"):
 
         try:
 
-            export_loc_mode = self.locs_export_mode.currentText()
             export_loc_jobs = []
 
             if export_dataset == "All Datasets":
                 dataset_list = list(self.dataset_dict.keys())
             else:
                 dataset_list = [export_dataset]
 
@@ -452,223 +353,136 @@
                 loc_type_list = ["Molecules"]
             elif export_loc_mode == "Bounding Boxes":
                 loc_type_list = ["Bounding Boxes"]
             else:
                 loc_type_list = ["Molecules", "Bounding Boxes"]
 
             for dataset_name in dataset_list:
-
                 if export_channel == "All Channels":
                     channel_list = list(self.dataset_dict[dataset_name].keys())
                 else:
                     channel_list = [export_channel]
 
-                channel_list = [
-                    channel.lower()
-                    for channel in channel_list
-                    if "efficiency" not in channel.lower()
-                ]
+                channel_list = [channel.lower() for channel in channel_list if "efficiency" not in channel.lower()]
 
                 for channel_name in channel_list:
-
                     for loc_type in loc_type_list:
-
                         if loc_type == "Molecules":
-                            loc_dict, n_locs, fitted = self.get_loc_dict(
-                                dataset_name, channel_name, type="molecules"
-                            )
+                            loc_dict, n_locs, fitted = self.get_loc_dict(dataset_name, channel_name, type="molecules")
                         elif loc_type == "Bounding Boxes":
-                            loc_dict, n_locs, fitted = self.get_loc_dict(
-                                dataset_name,
-                                channel_name,
-                                type="bounding_boxes",
-                            )
+                            loc_dict, n_locs, fitted = self.get_loc_dict(dataset_name, channel_name, type="bounding_boxes", )
 
                         if n_locs > 0 and fitted == True:
 
                             locs = loc_dict["localisations"]
                             box_size = loc_dict["box_size"]
 
                             if "min_net_gradient" in loc_dict.keys():
                                 min_net_gradient = loc_dict["min_net_gradient"]
                             else:
-                                min_net_gradient = int(
-                                    self.picasso_min_net_gradient.text()
-                                )
-
-                            if (
-                                channel_name
-                                in self.dataset_dict[dataset_name].keys()
-                            ):
-
-                                import_path = self.dataset_dict[dataset_name][
-                                    channel_name
-                                ]["path"]
-                                image_shape = self.dataset_dict[dataset_name][
-                                    channel_name
-                                ]["data"].shape
+                                min_net_gradient = int(self.gui.picasso_min_net_gradient.text())
+
+                            if (channel_name in self.dataset_dict[dataset_name].keys()):
+                                import_path = self.dataset_dict[dataset_name][channel_name]["path"]
+                                image_shape = self.dataset_dict[dataset_name][channel_name]["data"].shape
 
                                 base, ext = os.path.splitext(import_path)
 
                                 if channel_name in ["donor", "acceptor"]:
-                                    export_channel_name = (
-                                        channel_name.capitalize()
-                                    )
+                                    export_channel_name = (channel_name.capitalize())
                                 else:
                                     export_channel_name = channel_name.upper()
 
                                 if loc_type == "Bounding Boxes":
                                     hdf5_path = base + "_picasso_bboxes.hdf5"
                                     info_path = base + "_picasso_bboxes.yaml"
+                                    csv_path = base + "_picasso_bboxes.csv"
                                 else:
-                                    hdf5_path = (
-                                        base
-                                        + f"_picasso_{export_channel_name}_molecules.hdf5"
-                                    )
-                                    info_path = (
-                                        base
-                                        + f"_picasso_{export_channel_name}_molecules.yaml"
-                                    )
-
-                                picasso_info = [
-                                    {
-                                        "Byte Order": "<",
-                                        "Data Type": "uint16",
-                                        "File": import_path,
-                                        "Frames": image_shape[0],
-                                        "Height": image_shape[1],
-                                        "Micro-Manager Acquisiton Comments": "",
-                                        "Width": image_shape[2],
-                                    },
-                                    {
-                                        "Box Size": box_size,
-                                        "Fit method": "LQ, Gaussian",
-                                        "Generated by": "Picasso Localize",
-                                        "Min. Net Gradient": min_net_gradient,
-                                        "Pixelsize": 130,
-                                        "ROI": None,
-                                    },
-                                ]
-
-                                export_loc_job = {
-                                    "dataset_name": dataset_name,
-                                    "channel_name": channel_name,
-                                    "loc_type": loc_type,
-                                    "locs": locs,
-                                    "fitted": fitted,
-                                    "hdf5_path": hdf5_path,
-                                    "info_path": info_path,
-                                    "picasso_info": picasso_info,
-                                }
+                                    hdf5_path = (base + f"_picasso_{export_channel_name}_molecules.hdf5")
+                                    info_path = (base + f"_picasso_{export_channel_name}_molecules.yaml")
+                                    csv_path = (base + f"_picasso_{export_channel_name}_molecules.csv")
+
+                                picasso_info = [{"Byte Order": "<", "Data Type": "uint16", "File": import_path, "Frames": image_shape[0],
+                                                 "Height": image_shape[1], "Micro-Manager Acquisiton Comments": "", "Width": image_shape[2], },
+                                                {"Box Size": box_size, "Fit method": "LQ, Gaussian", "Generated by": "Picasso Localize",
+                                                 "Min. Net Gradient": min_net_gradient, "Pixelsize": 130, "ROI": None, }, ]
+
+                                export_loc_job = {"dataset_name": dataset_name, "channel_name": channel_name,
+                                                  "loc_type": loc_type, "locs": locs, "fitted": fitted,
+                                                  "hdf5_path": hdf5_path, "info_path": info_path, "csv_path": csv_path,
+                                                  "picasso_info": picasso_info, }
+
                             export_loc_jobs.append(export_loc_job)
 
             if len(export_loc_jobs) > 0:
-
-                with concurrent.futures.ThreadPoolExecutor(
-                    max_workers=1
-                ) as executor:
-                    futures = [
-                        executor.submit(export_picasso_localisation, job)
-                        for job in export_loc_jobs
-                    ]
+                with concurrent.futures.ThreadPoolExecutor(max_workers=1) as executor:
+                    futures = [executor.submit(export_picasso_localisation, job) for job in export_loc_jobs]
 
                     for future in concurrent.futures.as_completed(futures):
                         try:
                             future.result()
                         except:
                             print(traceback.format_exc())
 
-                        progress = int(
-                            100
-                            * (len(export_loc_jobs) - len(futures))
-                            / len(export_loc_jobs)
-                        )
+                        progress = int(100 * (len(export_loc_jobs) - len(futures)) / len(export_loc_jobs))
 
                         if progress_callback is not None:
                             progress_callback.emit(progress)
 
         except:
             self.update_ui()
             print(traceback.format_exc())
 
     def export_locs_finished(self):
-
         try:
-
             print("Exporting locs finished")
             self.update_ui()
 
         except:
             self.update_ui()
             print(traceback.format_exc())
 
-    def initialise_export_locs(
-        self, event=None, export_dataset="", export_channel=""
-    ):
+    def initialise_export_locs(self, event=None, export_dataset="", export_channel=""):
 
         try:
-
-            if (
-                export_dataset == ""
-                or export_dataset not in self.dataset_dict.keys()
-            ):
-                export_dataset = self.locs_export_dataset.currentText()
+            if (export_dataset == "" or export_dataset not in self.dataset_dict.keys()):
+                export_dataset = self.gui.locs_export_dataset.currentText()
             if export_channel == "":
-                export_channel = self.locs_export_channel.currentText()
+                export_channel = self.gui.locs_export_channel.currentText()
 
             self.update_ui(init=True)
 
-            self.worker = Worker(
-                self.export_locs,
-                export_dataset=export_dataset,
-                export_channel=export_channel,
-            )
-            self.worker.signals.progress.connect(
-                partial(
-                    self.pixseq_progress, progress_bar=self.export_progressbar
-                )
-            )
+            if self.verbose:
+                print(f"Exporting localisations for {export_dataset} {export_channel}")
+
+            self.worker = Worker(self.export_locs, export_dataset=export_dataset,
+                export_channel=export_channel, )
             self.worker.signals.finished.connect(self.export_locs_finished)
             self.threadpool.start(self.worker)
 
         except:
+            print(traceback.format_exc())
             self.update_ui()
 
     def get_loc_dict(self, dataset_name="", channel_name="", type="molecules"):
-
         loc_dict = {}
         n_localisations = 0
         fitted = False
 
         try:
-
             if type.lower() == "molecules":
-
-                if (
-                    dataset_name
-                    not in self.localisation_dict["molecules"].keys()
-                ):
+                if (dataset_name not in self.localisation_dict["molecules"].keys()):
                     self.localisation_dict["molecules"][dataset_name] = {}
                 else:
-                    if (
-                        channel_name
-                        not in self.localisation_dict["molecules"][
-                            dataset_name
-                        ].keys()
-                    ):
-                        self.localisation_dict["molecules"][dataset_name][
-                            channel_name
-                        ] = {}
+                    if (channel_name not in self.localisation_dict["molecules"][dataset_name].keys()):
+                        self.localisation_dict["molecules"][dataset_name][channel_name] = {}
                     else:
-                        loc_dict = self.localisation_dict["molecules"][
-                            dataset_name
-                        ][channel_name].copy()
+                        loc_dict = self.localisation_dict["molecules"][dataset_name][channel_name].copy()
 
             else:
-
                 if "bounding_boxes" not in self.localisation_dict.keys():
                     self.localisation_dict["bounding_boxes"] = {}
 
                 loc_dict = self.localisation_dict["bounding_boxes"].copy()
 
             if "localisations" in loc_dict.keys():
                 n_localisations = len(loc_dict["localisations"])
@@ -677,55 +491,44 @@
                 fitted = loc_dict["fitted"]
 
         except:
             print(traceback.format_exc())
 
         return loc_dict, n_localisations, fitted
 
-    def update_loc_dict(
-        self, dataset_name="", channel_name="", type="molecules", loc_dict={}
-    ):
-
+    def update_loc_dict(self, dataset_name="", channel_name="", type="molecules", loc_dict={}):
         try:
-
             if type == "molecules":
-                self.localisation_dict["molecules"][dataset_name][
-                    channel_name
-                ] = loc_dict
+                self.localisation_dict["molecules"][dataset_name][channel_name] = loc_dict
             else:
                 self.localisation_dict["bounding_boxes"] = loc_dict
 
         except:
             print(traceback.format_exc())
 
     def get_bbox_dict(self, dataset_name, channel_name):
-
         bbox_dict = {}
 
         if "bounding_boxes" not in self.localisation_dict.keys():
             self.localisation_dict["bounding_boxes"] = {}
 
         return bbox_dict
 
     def compute_net_gradient(self, position, box_size=None):
-
         net_gradient = 0
 
         try:
-
             dataset = self.gui.dataset_selector.currentText()
             channel = self.active_channel
             frame = self.viewer.dims.current_step[0]
 
             if box_size is None:
                 box_size = self.picasso_box_size.currentText()
 
-            loc_mask, _, loc_bg_mask = self.generate_localisation_mask(
-                box_size, spot_shape="square"
-            )
+            loc_mask, _, loc_bg_mask = self.generate_localisation_mask(box_size, spot_shape="square")
 
             box_size = len(loc_mask[0])
 
             x, y = position[0], position[1]
 
             if box_size % 2 == 0:
                 x += 0.5
@@ -739,45 +542,36 @@
                 # Odd spot width
                 x, y = round(x), round(y)
                 x1 = x - (box_size // 2)
                 x2 = x + (box_size // 2) + 1
                 y1 = y - (box_size // 2)
                 y2 = y + (box_size // 2) + 1
 
-            loc_spot = self.dataset_dict[dataset][channel]["data"][frame][
-                y1:y2, x1:x2
-            ]
+            loc_spot = self.dataset_dict[dataset][channel]["data"][frame][y1:y2, x1:x2]
 
             loc_spot_values = np.sum(loc_spot[loc_mask])
             loc_spot_bg_values = np.mean(loc_spot[loc_bg_mask])
 
             net_gradient = loc_spot_values
 
         except:
             print(traceback.format_exc())
 
         return float(net_gradient)
 
     def add_manual_localisation(self, position, mode):
-
         try:
-
             active_dataset = self.gui.dataset_selector.currentText()
             active_channel = self.active_channel
             box_size = int(self.picasso_box_size.currentText())
             frame = self.viewer.dims.current_step[0]
-            net_gradient = self.compute_net_gradient(
-                position, box_size=box_size
-            )
+            net_gradient = self.compute_net_gradient(position, box_size=box_size)
 
             if mode == "molecules":
-
-                loc_dict, n_locs, _ = self.get_loc_dict(
-                    active_dataset, active_channel, type="molecules"
-                )
+                loc_dict, n_locs, _ = self.get_loc_dict(active_dataset, active_channel, type="molecules")
 
                 if n_locs > 0:
                     locs = loc_dict["localisations"].copy()
                     render_locs = loc_dict["render_locs"].copy()
                     loc_centers = loc_dict["localisation_centres"].copy()
                     box_size = int(loc_dict["box_size"])
                     dtype = locs.dtype
@@ -785,128 +579,80 @@
                     loc_utils = picasso_loc_utils(locs)
 
                     x, y = position
 
                     frame_locs = locs[locs.frame == frame]
 
                     if len(frame_locs) > 0:
-
                         loc_coords = np.vstack((frame_locs.y, frame_locs.x)).T
 
                         # Calculate Euclidean distances
-                        distances = np.sqrt(
-                            np.sum(
-                                (loc_coords - np.array([y, x])) ** 2, axis=1
-                            )
-                        )
+                        distances = np.sqrt(np.sum((loc_coords - np.array([y, x])) ** 2, axis=1))
 
                         # Find the index of the minimum distance
                         min_index = np.argmin(distances)
                         min_distance = distances[min_index]
 
                         if min_distance < box_size:
-
                             locs = loc_utils.remove_loc(loc_index=min_index)
 
-                            loc_centers = np.delete(
-                                loc_centers, min_index, axis=0
-                            )
+                            loc_centers = np.delete(loc_centers, min_index, axis=0)
                             loc_centers = loc_centers.tolist()
 
                             render_frame_locs = render_locs[frame].copy()
-                            render_frame_locs = np.unique(
-                                render_frame_locs, axis=0
-                            ).tolist()
-                            distances = np.sqrt(
-                                np.sum(
-                                    (
-                                        np.array(render_frame_locs)
-                                        - np.array([y, x])
-                                    )
-                                    ** 2,
-                                    axis=1,
-                                )
-                            )
+                            render_frame_locs = np.unique(render_frame_locs, axis=0).tolist()
+                            distances = np.sqrt(np.sum((np.array(render_frame_locs) - np.array([y, x])) ** 2, axis=1, ))
                             min_index = np.argmin(distances)
                             render_frame_locs.pop(min_index)
                             render_locs[frame] = render_frame_locs
 
                             loc_dict["localisations"] = locs
                             loc_dict["localisation_centres"] = loc_centers
                             loc_dict["render_locs"] = render_locs
 
-                            self.update_loc_dict(
-                                active_dataset,
-                                active_channel,
-                                "molecules",
-                                loc_dict,
-                            )
+                            self.update_loc_dict(active_dataset, active_channel, "molecules", loc_dict, )
                             self.draw_molecules(update_vis=True)
 
                         else:
+                            locs = loc_utils.add_loc(new_loc=[frame, x, y, net_gradient])
 
-                            locs = loc_utils.add_loc(
-                                new_loc=[frame, x, y, net_gradient]
-                            )
-
-                            loc_centers = np.append(
-                                loc_centers,
-                                np.array([[frame, y, x]], dtype=int),
-                                axis=0,
-                            )
+                            loc_centers = np.append(loc_centers, np.array([[frame, y, x]], dtype=int), axis=0, )
                             loc_centers = loc_centers.tolist()
 
                             if len(render_locs[frame]) == 0:
                                 render_locs[frame] = [[round(y), round(x)]]
                             else:
                                 render_locs[frame].append([round(y), round(x)])
 
                             loc_dict["localisations"] = locs
                             loc_dict["localisation_centres"] = loc_centers
                             loc_dict["render_locs"] = render_locs
 
-                            self.update_loc_dict(
-                                active_dataset,
-                                active_channel,
-                                "molecules",
-                                loc_dict,
-                            )
+                            self.update_loc_dict(active_dataset, active_channel, "molecules", loc_dict, )
                             self.draw_molecules(update_vis=True)
 
                     else:
+                        locs = loc_utils.add_loc(new_loc=[frame, x, y, net_gradient])
 
-                        locs = loc_utils.add_loc(
-                            new_loc=[frame, x, y, net_gradient]
-                        )
-
-                        loc_centers = np.append(
-                            loc_centers,
-                            np.array([[frame, y, x]], dtype=int),
-                            axis=0,
-                        )
+                        loc_centers = np.append(loc_centers, np.array([[frame, y, x]], dtype=int), axis=0, )
                         loc_centers = loc_centers.tolist()
 
                         if frame in render_locs.keys():
                             if len(render_locs[frame]) == 0:
                                 render_locs[frame] = [[round(y), round(x)]]
                             else:
                                 render_locs[frame].append([round(y), round(x)])
                         else:
                             render_locs[frame] = [[round(y), round(x)]]
 
                         loc_dict["localisations"] = locs
                         loc_dict["localisation_centres"] = loc_centers
                         loc_dict["render_locs"] = render_locs
 
-                        self.update_loc_dict(
-                            active_dataset,
-                            active_channel,
-                            "molecules",
-                            loc_dict,
-                        )
+                        self.update_loc_dict(active_dataset, active_channel, "molecules", loc_dict, )
                         self.draw_molecules(update_vis=True)
 
                 else:
                     x, y = position
 
                     box_size = int(self.picasso_box_size.currentText())
 
@@ -920,27 +666,21 @@
 
                     loc_dict["localisations"] = locs
                     loc_dict["localisation_centres"] = loc_centers
                     loc_dict["render_locs"] = render_locs
                     loc_dict["fitted"] = False
                     loc_dict["box_size"] = box_size
 
-                    self.update_loc_dict(
-                        active_dataset, active_channel, "molecules", loc_dict
-                    )
+                    self.update_loc_dict(active_dataset, active_channel, "molecules", loc_dict)
                     self.draw_molecules(update_vis=True)
 
             elif mode == "bounding_box":
-
-                loc_dict, n_locs, _ = self.get_loc_dict(
-                    active_dataset, active_channel, type="bounding_box"
-                )
+                loc_dict, n_locs, _ = self.get_loc_dict(active_dataset, active_channel, type="bounding_box")
 
                 if n_locs > 0:
-
                     locs = loc_dict["localisations"].copy()
                     loc_centers = loc_dict["localisation_centres"].copy()
                     box_size = int(loc_dict["box_size"])
                     dtype = locs.dtype
 
                     loc_utils = picasso_loc_utils(locs)
 
@@ -950,77 +690,52 @@
 
                     if loc_centers.shape[-1] != 2:
                         loc_coords = loc_centers[:, 1:].copy()
                     else:
                         loc_coords = loc_centers.copy()
 
                     # Calculate Euclidean distances
-                    distances = np.sqrt(
-                        np.sum((loc_coords - np.array([y, x])) ** 2, axis=1)
-                    )
+                    distances = np.sqrt(np.sum((loc_coords - np.array([y, x])) ** 2, axis=1))
 
                     # Find the index of the minimum distance
                     min_index = np.argmin(distances)
                     min_distance = distances[min_index]
 
                     # print(f"min_distance: {min_distance}")
 
                     if min_distance < box_size:
-
                         locs = loc_utils.remove_loc(loc_index=min_index)
 
                         loc_centers = np.delete(loc_centers, min_index, axis=0)
                         loc_centers = loc_centers.tolist()
 
                         # print(f"len locs: {len(locs)}, len loc_centers: {len(loc_centers)}")
 
                         loc_dict["localisations"] = locs
                         loc_dict["localisation_centres"] = loc_centers
-                        self.update_loc_dict(
-                            active_dataset,
-                            active_channel,
-                            "bounding_boxes",
-                            loc_dict,
-                        )
+                        self.update_loc_dict(active_dataset, active_channel, "bounding_boxes", loc_dict, )
                         self.draw_bounding_boxes()
 
                     else:
-
-                        locs = loc_utils.add_loc(
-                            new_loc=[frame, x, y, net_gradient]
-                        )
+                        locs = loc_utils.add_loc(new_loc=[frame, x, y, net_gradient])
 
                         if loc_centers.shape[-1] == 3:
-                            loc_centers = np.append(
-                                loc_centers,
-                                np.array([[frame, y, x]], dtype=int),
-                                axis=0,
-                            )
+                            loc_centers = np.append(loc_centers, np.array([[frame, y, x]], dtype=int), axis=0, )
                         if loc_centers.shape[-1] == 2:
-                            loc_centers = np.append(
-                                loc_centers,
-                                np.array([[y, x]], dtype=int),
-                                axis=0,
-                            )
+                            loc_centers = np.append(loc_centers, np.array([[y, x]], dtype=int), axis=0, )
 
                         loc_centers = loc_centers.tolist()
 
                         loc_dict["localisations"] = locs
                         loc_dict["localisation_centres"] = loc_centers
 
-                        self.update_loc_dict(
-                            active_dataset,
-                            active_channel,
-                            "bounding_boxes",
-                            loc_dict,
-                        )
+                        self.update_loc_dict(active_dataset, active_channel, "bounding_boxes", loc_dict, )
                         self.draw_bounding_boxes()
 
                 else:
-
                     x, y = position
 
                     box_size = int(self.picasso_box_size.currentText())
 
                     new_loc = [frame, position[0], position[1], net_gradient]
 
                     loc_utils = picasso_loc_utils()
@@ -1029,23 +744,17 @@
                     loc_centers = [[y, x]]
 
                     loc_dict["localisations"] = locs
                     loc_dict["localisation_centres"] = loc_centers
                     loc_dict["fitted"] = False
                     loc_dict["box_size"] = box_size
 
-                    self.update_loc_dict(
-                        active_dataset,
-                        active_channel,
-                        "bounding_boxes",
-                        loc_dict,
-                    )
+                    self.update_loc_dict(active_dataset, active_channel, "bounding_boxes", loc_dict, )
                     self.draw_bounding_boxes()
 
             elif mode == "lsp":
-
                 x, y = position
 
                 print(x, y)
 
         except:
             print(traceback.format_exc())
```

### Comparing `napari_smlmlab-0.0.2/src/smlmlab/utils/picasso_utils.py` & `napari_smlmlab-0.0.3/src/smlmlab/utils/picasso_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import concurrent.futures
 import multiprocessing
 import os
 import time
 import traceback
 from functools import partial
 from multiprocessing import shared_memory
-
+import warnings
 import numpy as np
 from picasso import localize
 from picasso.gaussmle import gaussmle
 from picasso.localize import get_spots, identify_frame
 from picasso.render import render
-
 from smlmlab.utils.compute_utils import Worker
-
+from threading import Lock
+import threading
+from multiprocessing import Manager
 
 def remove_overlapping_locs(locs, box_size):
     try:
         coordinates = np.vstack((locs.y, locs.x)).T
 
         # Calculate all pairwise differences
         diff = coordinates[:, np.newaxis, :] - coordinates[np.newaxis, :, :]
@@ -52,16 +53,18 @@
     spots = np.zeros((n_spots, box, box), dtype=movie.dtype)
     for id, (frame, xc, yc) in enumerate(zip(ids_frame, ids_x, ids_y)):
         spots[id] = movie[frame, yc - r: yc + r + 1, xc - r: xc + r + 1]
 
     return spots
 
 
-def picasso_detect(dat):
+def picasso_detect(dat, progress_list):
+
     result = None
+    frame_index = dat["frame_index"]
 
     try:
         frame_index = dat["frame_index"]
         min_net_gradient = dat["min_net_gradient"]
         box_size = dat["box_size"]
         roi = dat["roi"]
         dataset = dat["dataset"]
@@ -89,14 +92,17 @@
                 locs = dat["frame_locs"]
 
             expected_loc_length = 4
 
             if fit:
                 expected_loc_length = 12
                 try:
+
+                    warnings.filterwarnings("ignore", category=RuntimeWarning)
+
                     image = np.expand_dims(frame, axis=0)
                     camera_info = {"baseline": 100.0, "gain": 1, "sensitivity": 1.0, "qe": 0.9, }
                     spot_data = get_spots(image, locs, box_size, camera_info)
 
                     # frame = np.expand_dims(frame, axis=0)
                     # locs.frame = 0
                     # spot_data = cut_spots(frame, locs.frame, locs.x, locs.y, box_size)
@@ -124,14 +130,16 @@
             locs = np.array(locs).view(np.recarray)
 
             result = {"dataset": dataset, "channel": channel, "frame_index": frame_index, "locs": locs, "render_locs": render_locs, }
 
     except:
         print(traceback.format_exc())
 
+    progress_list.append(frame_index)
+
     return result
 
 
 class _picasso_detect_utils:
 
     def populate_localisation_dict(self, loc_dict, render_loc_dict, detect_mode, image_channel, box_size, fitted=False, ):
         if self.verbose:
@@ -180,15 +188,15 @@
     def _picasso_wrapper_result(self, result):
         try:
             if self.verbose:
                 print("Picasso wrapper result received")
 
             fitted, loc_dict, render_loc_dict, total_locs = result
 
-            detect_mode = self.gui.picasso_detect_mode.currentText()
+            detect_mode = "Molecules"
             image_channel = self.gui.picasso_channel.currentText()
             box_size = int(self.gui.picasso_box_size.currentText())
 
             dataset_names = list(loc_dict.keys())
 
             if len(dataset_names) > 0:
                 self.populate_localisation_dict(loc_dict, render_loc_dict, detect_mode, image_channel, box_size, fitted, )
@@ -197,14 +205,15 @@
                     self.pixseq_notification(f"Fitted {total_locs} {detect_mode}")
                 else:
                     self.pixseq_notification(f"Detected {total_locs} {detect_mode}")
 
         except:
             print(traceback.format_exc())
 
+
     def _picasso_wrapper_finished(self, active_frame_index = None):
         try:
             image_channel = self.gui.picasso_channel.currentText()
             dataset_name = self.gui.picasso_dataset.currentText()
 
             if dataset_name == "All Datasets":
                 dataset_name = self.active_dataset
@@ -215,14 +224,15 @@
             self.draw_bounding_boxes()
 
             self.update_ui()
 
         except:
             print(traceback.format_exc())
 
+
     def get_frame_locs(self, dataset_name, image_channel, frame_index):
         try:
             loc_dict, n_locs, _ = self.get_loc_dict(dataset_name, image_channel.lower(), type="molecules")
 
             if "localisations" not in loc_dict.keys():
                 return None
             else:
@@ -325,48 +335,53 @@
                 if frame_mode.lower() == "active":
                     executor_class = concurrent.futures.ThreadPoolExecutor
                     cpu_count = 1
                 else:
                     executor_class = concurrent.futures.ProcessPoolExecutor
                     cpu_count = int(multiprocessing.cpu_count() * 0.9)
 
-                with executor_class(max_workers=cpu_count) as executor:
-                    futures = {executor.submit(picasso_detect, job): job for job in compute_jobs}
+                with Manager() as manager:
+                    progress_list = manager.list()
 
-                iter = 0
-                for future in concurrent.futures.as_completed(futures):
-                    if self.stop_event.is_set():
-                        future.cancel()
-                    else:
-                        job = futures[future]
-                        try:
-                            result = future.result(timeout=timeout_duration)  # Process result here
-
-                            if result is not None:
-                                dataset_name = result["dataset"]
-
-                                if dataset_name not in loc_dict:
-                                    loc_dict[dataset_name] = []
-                                    render_loc_dict[dataset_name] = {}
-
-                                locs = result["locs"]
-                                render_locs = result["render_locs"]
-
-                                loc_dict[dataset_name].extend(locs)
-                                render_loc_dict[dataset_name] = {**render_loc_dict[dataset_name], **render_locs, }
-
-                            iter += 1
-                            progress = int((iter / len(compute_jobs)) * 100)
-                            progress_callback.emit(progress)  # Emit the signal
-
-                        except concurrent.futures.TimeoutError:
-                            # print(f"Task {job} timed out after {timeout_duration} seconds.")
-                            pass
-                        except Exception as e:
-                            print(f"Error occurred in task {job}: {e}")  # Handle other exceptions
+                    with executor_class(max_workers=cpu_count) as executor:
+                        futures = {executor.submit(picasso_detect, job, progress_list): job for job in compute_jobs}
+
+                        # Calculate and emit progress
+                        while any(not future.done() for future in futures):
+                            progress = (len(progress_list)/len(compute_jobs)) * 100
+                            if progress_callback is not None:
+                                progress_callback.emit(progress)
+
+                        for future in concurrent.futures.as_completed(futures):
+
+                            if self.stop_event.is_set():
+                                future.cancel()
+                            else:
+                                job = futures[future]
+                                try:
+                                    result = future.result(timeout=timeout_duration)  # Process result here
+
+                                    if result is not None:
+                                        dataset_name = result["dataset"]
+
+                                        if dataset_name not in loc_dict:
+                                            loc_dict[dataset_name] = []
+                                            render_loc_dict[dataset_name] = {}
+
+                                        locs = result["locs"]
+                                        render_locs = result["render_locs"]
+
+                                        loc_dict[dataset_name].extend(locs)
+                                        render_loc_dict[dataset_name] = {**render_loc_dict[dataset_name], **render_locs, }
+
+                                except concurrent.futures.TimeoutError:
+                                    print(f"Task {job} timed out after {timeout_duration} seconds.")
+                                    pass
+                                except Exception as e:
+                                    print(f"Error occurred in task {job}: {e}")  # Handle other exceptions
 
                 if self.verbose:
                     print("Finished Picasso compute jobs...")
                     print("Compiling Picasso results...")
 
                 total_locs = 0
                 for dataset, locs in loc_dict.items():
@@ -421,15 +436,17 @@
                     self.threadpool.start(self.worker)
 
         except:
             print(traceback.format_exc())
 
             self.update_ui()
 
-    def render_picasso_locs(self, locs, image_shape, blur_method=None, min_blur_width=1, pixel_size=1, progress_callback=None, oversampling=20, ):
+    def render_picasso_locs(self, locs, image_shape, blur_method=None,
+            min_blur_width=1, pixel_size=1, progress_callback=None, oversampling=20, ):
+
         try:
             h, w = image_shape[-2:]
 
             viewport = [(0, 0), (h, w)]
 
             n_rendered_locs, image = render(locs, viewport=viewport,
                 blur_method=blur_method, min_blur_width=min_blur_width, oversampling=oversampling, )
@@ -471,42 +488,44 @@
             image_channel = self.gui.picasso_render_channel.currentText()
             blur_method = self.gui.picasso_render_blur_method.currentText()
             min_blur_width = float(self.gui.picasso_render_min_blur.text())
 
             if (image_channel.lower() in self.localisation_dict["molecules"][dataset_name].keys()):
                 localisation_dict = self.localisation_dict["molecules"][dataset_name][image_channel.lower()].copy()
 
-                if localisation_dict["fitted"] == True:
-                    locs = localisation_dict["localisations"]
+                if "fitted" in localisation_dict:
 
-                    image_shape = list(self.dataset_dict[dataset_name][image_channel.lower()]["data"].shape)
-                    pixel_size = float(self.dataset_dict[dataset_name][image_channel.lower()]["pixel_size"])
+                    if localisation_dict["fitted"] == True:
+                        locs = localisation_dict["localisations"]
 
-                    if blur_method == "One-Pixel-Blur":
-                        blur_method = "smooth"
-                    elif blur_method == "Global Localisation Precision":
-                        blur_method = "convolve"
-                    elif (blur_method == "Individual Localisation Precision, iso"):
-                        blur_method = "gaussian_iso"
-                    elif blur_method == "Individual Localisation Precision":
-                        blur_method = "gaussian"
-                    else:
-                        blur_method = None
-
-                    self.update_ui(init=True)
+                        image_shape = list(self.dataset_dict[dataset_name][image_channel.lower()]["data"].shape)
+                        pixel_size = float(self.dataset_dict[dataset_name][image_channel.lower()]["pixel_size"])
 
-                    worker = Worker(self.render_picasso_locs, locs=locs, image_shape=image_shape,
-                        blur_method=blur_method, min_blur_width=min_blur_width, pixel_size=pixel_size, )
-                    worker.signals.result.connect(self.draw_picasso_render)
-                    worker.signals.finished.connect(self.picasso_render_finished)
-                    self.threadpool.start(worker)
+                        if blur_method == "One-Pixel-Blur":
+                            blur_method = "smooth"
+                        elif blur_method == "Global Localisation Precision":
+                            blur_method = "convolve"
+                        elif (blur_method == "Individual Localisation Precision, iso"):
+                            blur_method = "gaussian_iso"
+                        elif blur_method == "Individual Localisation Precision":
+                            blur_method = "gaussian"
+                        else:
+                            blur_method = None
+
+                        self.update_ui(init=True)
+
+                        worker = Worker(self.render_picasso_locs, locs=locs, image_shape=image_shape,
+                            blur_method=blur_method, min_blur_width=min_blur_width, pixel_size=pixel_size, )
+                        worker.signals.result.connect(self.draw_picasso_render)
+                        worker.signals.finished.connect(self.picasso_render_finished)
+                        self.threadpool.start(worker)
 
         except:
             print(traceback.format_exc())
-            self.update_ui(init=True)
+            self.update_ui(init=False)
 
     def generate_roi(self):
 
         if self.verbose:
             print("Generating ROI")
 
         border_width = self.gui.picasso_roi_border_width.text()
```

### Comparing `napari_smlmlab-0.0.2/src/smlmlab/utils/viewer_utils.py` & `napari_smlmlab-0.0.3/src/smlmlab/utils/viewer_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,162 +1,104 @@
 import traceback
 
 
 class _viewer_utils:
 
     def draw_bounding_boxes(self, update_vis=False):
-
-        if hasattr(self, "localisation_dict") and hasattr(
-            self, "active_channel"
-        ):
+        if hasattr(self, "localisation_dict") and hasattr(self, "active_channel"):
             if hasattr(self, "bbox_layer"):
                 show_bboxes = self.bbox_layer.visible
             else:
                 show_bboxes = True
 
             if show_bboxes:
-
                 layer_names = [layer.name for layer in self.viewer.layers]
 
                 dataset_name = self.gui.dataset_selector.currentText()
                 image_channel = self.active_channel
 
-                if (
-                    "localisation_centres"
-                    in self.localisation_dict["bounding_boxes"].keys()
-                ):
+                if ("localisation_centres" in self.localisation_dict["bounding_boxes"].keys()):
                     if self.verbose:
                         print("Drawing bounding_boxes")
 
-                    loc_dict, n_locs, fitted = self.get_loc_dict(
-                        type="bounding_boxes"
-                    )
+                    loc_dict, n_locs, fitted = self.get_loc_dict(type="bounding_boxes")
 
                     localisations = loc_dict["localisations"].copy()
-                    localisation_centres = self.get_localisation_centres(
-                        localisations, mode="bounding_boxes"
-                    )
+                    localisation_centres = self.get_localisation_centres(localisations, mode="bounding_boxes")
 
                     vis_mode = self.gui.picasso_vis_mode.currentText()
                     vis_size = float(self.gui.picasso_vis_size.currentText())
-                    vis_opacity = float(
-                        self.gui.picasso_vis_opacity.currentText()
-                    )
-                    vis_edge_width = float(
-                        self.gui.picasso_vis_edge_width.currentText()
-                    )
-
-                    pixel_size = float(
-                        self.dataset_dict[dataset_name][image_channel.lower()][
-                            "pixel_size"
-                        ]
-                    )
+                    vis_opacity = float(self.gui.picasso_vis_opacity.currentText())
+                    vis_edge_width = float(self.gui.picasso_vis_edge_width.currentText())
+
+                    pixel_size = float(self.dataset_dict[dataset_name][image_channel.lower()]["pixel_size"])
                     scale = [pixel_size, pixel_size]
 
                     if pixel_size != 1:
                         vis_size = vis_size / pixel_size
 
                     if vis_mode.lower() == "square":
                         symbol = "square"
                     elif vis_mode.lower() == "disk":
                         symbol = "disc"
                     elif vis_mode.lower() == "x":
                         symbol = "cross"
 
                     if "bounding_boxes" not in layer_names:
-                        self.bbox_layer = self.viewer.add_points(
-                            localisation_centres,
-                            edge_color="white",
-                            ndim=2,
-                            face_color=[0, 0, 0, 0],
-                            opacity=vis_opacity,
-                            name="bounding_boxes",
-                            symbol=symbol,
-                            size=vis_size,
-                            visible=True,
-                            edge_width=vis_edge_width,
-                            scale=scale,
-                        )
-
-                        self.bbox_layer.mouse_drag_callbacks.append(
-                            self._mouse_event
-                        )
-                        self.bbox_layer.events.visible.connect(
-                            self.draw_bounding_boxes
-                        )
+                        self.bbox_layer = self.viewer.add_points(localisation_centres, edge_color="white", ndim=2, face_color=[0, 0, 0, 0], opacity=vis_opacity, name="bounding_boxes", symbol=symbol, size=vis_size, visible=True, edge_width=vis_edge_width, scale=scale, )
+
+                        self.bbox_layer.mouse_drag_callbacks.append(self._mouse_event)
+                        self.bbox_layer.events.visible.connect(self.draw_bounding_boxes)
 
                     else:
-                        self.viewer.layers["bounding_boxes"].data = (
-                            localisation_centres
-                        )
+                        self.viewer.layers["bounding_boxes"].data = (localisation_centres)
                         self.viewer.layers["bounding_boxes"].scale = scale
 
-                    self.bbox_layer.selected_data = list(
-                        range(len(self.bbox_layer.data))
-                    )
+                    self.bbox_layer.selected_data = list(range(len(self.bbox_layer.data)))
                     self.bbox_layer.opacity = vis_opacity
                     self.bbox_layer.symbol = symbol
                     self.bbox_layer.size = vis_size
                     self.bbox_layer.edge_width = vis_edge_width
                     self.bbox_layer.edge_color = "white"
                     self.bbox_layer.selected_data = []
                     self.bbox_layer.refresh()
 
                 for layer in layer_names:
                     self.viewer.layers[layer].refresh()
 
     def draw_molecules(self, update_vis=False):
         remove_molecules = True
 
-        if hasattr(self, "localisation_dict") and hasattr(
-            self, "active_channel"
-        ):
+        if hasattr(self, "localisation_dict") and hasattr(self, "active_channel"):
             if hasattr(self, "molecule_layer"):
                 show_molecules = self.molecule_layer.visible
             else:
                 show_molecules = True
 
             if show_molecules:
                 layer_names = [layer.name for layer in self.viewer.layers]
 
                 active_frame = self.viewer.dims.current_step[0]
 
                 dataset_name = self.gui.dataset_selector.currentText()
                 image_channel = self.active_channel
 
                 if image_channel != "" and dataset_name != "":
-                    if (
-                        image_channel.lower()
-                        in self.localisation_dict["molecules"][
-                            dataset_name
-                        ].keys()
-                    ):
-                        localisation_dict = self.localisation_dict[
-                            "molecules"
-                        ][dataset_name][image_channel.lower()].copy()
+                    if (image_channel.lower() in self.localisation_dict["molecules"][dataset_name].keys()):
+                        localisation_dict = self.localisation_dict["molecules"][dataset_name][image_channel.lower()].copy()
 
                         if "render_locs" in localisation_dict.keys():
                             render_locs = localisation_dict["render_locs"]
 
                             vis_mode = self.gui.picasso_vis_mode.currentText()
-                            vis_size = float(
-                                self.gui.picasso_vis_size.currentText()
-                            )
-                            vis_opacity = float(
-                                self.gui.picasso_vis_opacity.currentText()
-                            )
-                            vis_edge_width = float(
-                                self.gui.picasso_vis_edge_width.currentText()
-                            )
-
-                            pixel_size = float(
-                                self.dataset_dict[dataset_name][
-                                    image_channel.lower()
-                                ]["pixel_size"]
-                            )
+                            vis_size = float(self.gui.picasso_vis_size.currentText())
+                            vis_opacity = float(self.gui.picasso_vis_opacity.currentText())
+                            vis_edge_width = float(self.gui.picasso_vis_edge_width.currentText())
+
+                            pixel_size = float(self.dataset_dict[dataset_name][image_channel.lower()]["pixel_size"])
                             scale = [pixel_size, pixel_size]
 
                             if pixel_size != 1:
                                 vis_size = vis_size / pixel_size
 
                             if vis_mode.lower() == "square":
                                 symbol = "square"
@@ -168,63 +110,38 @@
                             if active_frame in render_locs.keys():
                                 remove_molecules = False
 
                                 if "molecules" not in layer_names:
                                     if self.verbose:
                                         print("Drawing molecules")
 
-                                    self.molecule_layer = (
-                                        self.viewer.add_points(
-                                            render_locs[active_frame],
-                                            ndim=2,
-                                            edge_color="red",
-                                            face_color=[0, 0, 0, 0],
-                                            opacity=vis_opacity,
-                                            name="molecules",
-                                            symbol=symbol,
-                                            size=vis_size,
-                                            edge_width=vis_edge_width,
-                                            scale=scale,
-                                        )
-                                    )
-
-                                    self.molecule_layer.mouse_drag_callbacks.append(
-                                        self._mouse_event
-                                    )
-                                    self.molecule_layer.events.visible.connect(
-                                        self.draw_molecules
-                                    )
+                                    self.molecule_layer = (self.viewer.add_points(render_locs[active_frame], ndim=2, edge_color="red", face_color=[0, 0, 0, 0], opacity=vis_opacity, name="molecules", symbol=symbol, size=vis_size, edge_width=vis_edge_width, scale=scale, ))
+
+                                    self.molecule_layer.mouse_drag_callbacks.append(self._mouse_event)
+                                    self.molecule_layer.events.visible.connect(self.draw_molecules)
 
                                     update_vis = True
 
                                 else:
                                     if self.verbose:
                                         print("Updating molecule data")
 
-                                    self.molecule_layer.data = render_locs[
-                                        active_frame
-                                    ]
+                                    self.molecule_layer.data = render_locs[active_frame]
                                     self.molecule_layer.selected_data = []
                                     self.molecule_layer.scale = scale
 
                                 if update_vis:
                                     if self.verbose:
-                                        print(
-                                            "Updating molecule visualisation settings"
-                                        )
-
-                                    self.molecule_layer.selected_data = list(
-                                        range(len(self.molecule_layer.data))
-                                    )
+                                        print("Updating molecule visualisation settings")
+
+                                    self.molecule_layer.selected_data = list(range(len(self.molecule_layer.data)))
                                     self.molecule_layer.opacity = vis_opacity
                                     self.molecule_layer.symbol = symbol
                                     self.molecule_layer.size = vis_size
-                                    self.molecule_layer.edge_width = (
-                                        vis_edge_width
-                                    )
+                                    self.molecule_layer.edge_width = (vis_edge_width)
                                     self.molecule_layer.edge_color = "red"
                                     self.molecule_layer.selected_data = []
                                     self.molecule_layer.refresh()
 
                 if remove_molecules:
                     if "molecules" in layer_names:
                         self.viewer.layers["molecules"].data = []
```

