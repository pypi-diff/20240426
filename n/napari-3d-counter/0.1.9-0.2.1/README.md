# Comparing `tmp/napari-3d-counter-0.1.9.tar.gz` & `tmp/napari_3d_counter-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-3d-counter-0.1.9.tar", last modified: Fri Feb 16 01:05:17 2024, max compression
+gzip compressed data, was "napari_3d_counter-0.2.1.tar", last modified: Fri Apr 26 21:10:17 2024, max compression
```

## Comparing `napari-3d-counter-0.1.9.tar` & `napari_3d_counter-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 01:05:17.090857 napari-3d-counter-0.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 01:05:17.082857 napari-3d-counter-0.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 01:05:17.086857 napari-3d-counter-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 01:05:17.086857 napari-3d-counter-0.1.9/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-02-16 01:05:17.090857 napari-3d-counter-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/gui_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/launch_napari.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-16 01:05:17.090857 napari-3d-counter-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 01:05:17.082857 napari-3d-counter-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 01:05:17.086857 napari-3d-counter-0.1.9/src/napari_3d_counter/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/src/napari_3d_counter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 01:05:17.090857 napari-3d-counter-0.1.9/src/napari_3d_counter/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/src/napari_3d_counter/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/src/napari_3d_counter/_tests/test_celltype_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/src/napari_3d_counter/_tests/test_python_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/src/napari_3d_counter/_tests/test_reconstruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     9565 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/src/napari_3d_counter/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-16 01:05:17.000000 napari-3d-counter-0.1.9/src/napari_3d_counter/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    18093 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/src/napari_3d_counter/_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/src/napari_3d_counter/celltype_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/src/napari_3d_counter/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 01:05:17.090857 napari-3d-counter-0.1.9/src/napari_3d_counter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-02-16 01:05:17.000000 napari-3d-counter-0.1.9/src/napari_3d_counter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-16 01:05:17.000000 napari-3d-counter-0.1.9/src/napari_3d_counter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 01:05:17.000000 napari-3d-counter-0.1.9/src/napari_3d_counter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-16 01:05:17.000000 napari-3d-counter-0.1.9/src/napari_3d_counter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-16 01:05:17.000000 napari-3d-counter-0.1.9/src/napari_3d_counter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-16 01:05:17.000000 napari-3d-counter-0.1.9/src/napari_3d_counter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-16 01:04:59.000000 napari-3d-counter-0.1.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:10:17.536796 napari_3d_counter-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:10:17.528796 napari_3d_counter-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:10:17.532796 napari_3d_counter-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:10:17.532796 napari_3d_counter-0.2.1/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-04-26 21:10:17.536796 napari_3d_counter-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/gui_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/launch_napari.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-26 21:10:17.536796 napari_3d_counter-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:10:17.528796 napari_3d_counter-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:10:17.532796 napari_3d_counter-0.2.1/src/napari_3d_counter/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/src/napari_3d_counter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:10:17.532796 napari_3d_counter-0.2.1/src/napari_3d_counter/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/src/napari_3d_counter/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/src/napari_3d_counter/_tests/test_celltype_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/src/napari_3d_counter/_tests/test_python_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/src/napari_3d_counter/_tests/test_reconstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13981 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/src/napari_3d_counter/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 21:10:17.000000 napari_3d_counter-0.2.1/src/napari_3d_counter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19144 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/src/napari_3d_counter/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/src/napari_3d_counter/celltype_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/src/napari_3d_counter/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:10:17.532796 napari_3d_counter-0.2.1/src/napari_3d_counter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-04-26 21:10:17.000000 napari_3d_counter-0.2.1/src/napari_3d_counter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-26 21:10:17.000000 napari_3d_counter-0.2.1/src/napari_3d_counter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 21:10:17.000000 napari_3d_counter-0.2.1/src/napari_3d_counter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-26 21:10:17.000000 napari_3d_counter-0.2.1/src/napari_3d_counter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-26 21:10:17.000000 napari_3d_counter-0.2.1/src/napari_3d_counter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 21:10:17.000000 napari_3d_counter-0.2.1/src/napari_3d_counter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-26 21:10:00.000000 napari_3d_counter-0.2.1/tox.ini
```

### Comparing `napari-3d-counter-0.1.9/.github/workflows/test_and_deploy.yml` & `napari_3d_counter-0.2.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-3d-counter-0.1.9/.gitignore` & `napari_3d_counter-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-3d-counter-0.1.9/.napari-hub/config.yml` & `napari_3d_counter-0.2.1/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-3d-counter-0.1.9/.pre-commit-config.yaml` & `napari_3d_counter-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-3d-counter-0.1.9/LICENSE` & `napari_3d_counter-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-3d-counter-0.1.9/PKG-INFO` & `napari_3d_counter-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-3d-counter
-Version: 0.1.9
+Version: 0.2.1
 Summary: A simple plugin for counting objects in 3D images
 Home-page: https://github.com/pnewstein/napari-3d-counter
 Author: Peter Newstein
 Author-email: peternewstein@gmail.com
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://github.com/pnewstein/napari-3d-counter/issues
 Project-URL: Documentation, https://github.com/pnewstein/napari-3d-counter#README.md
@@ -26,15 +26,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: qtpy
 Requires-Dist: pandas
 Requires-Dist: scikit-image
 Requires-Dist: matplotlib
-Requires-Dist: napari==0.4.18
+Requires-Dist: napari<=0.4.19
 Provides-Extra: testing
 Requires-Dist: tox; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-qt; extra == "testing"
 Requires-Dist: napari; extra == "testing"
 Requires-Dist: pyqt5; extra == "testing"
```

### Comparing `napari-3d-counter-0.1.9/README.md` & `napari_3d_counter-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `napari-3d-counter-0.1.9/gui_demo.py` & `napari_3d_counter-0.2.1/gui_demo.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 if len(sys.argv) == 2:
     from napari_3d_counter import Count3D, CellTypeConfig
 
     viewer.window.add_dock_widget(
         Count3D(viewer, [CellTypeConfig("Counter 1")])
     )
 
+napari.run()
 # start wiget
 # add green cells
 # add magenta cells
 # add extra cell
 # undo
 # add extra cell
 # remove it
```

### Comparing `napari-3d-counter-0.1.9/pyproject.toml` & `napari_3d_counter-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -51,8 +51,7 @@
     "node_modules",
     "venv",
     "*vendored*",
     "*_vendor*",
 ]
 
 target-version = "py38"
-fix = true
```

### Comparing `napari-3d-counter-0.1.9/setup.cfg` & `napari_3d_counter-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 packages = find:
 install_requires = 
 	numpy
 	qtpy
 	pandas
 	scikit-image
 	matplotlib
-	napari==0.4.18
+	napari<=0.4.19
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = setuptools_scm
 
 [options.packages.find]
```

### Comparing `napari-3d-counter-0.1.9/src/napari_3d_counter/_tests/test_celltype_config.py` & `napari_3d_counter-0.2.1/src/napari_3d_counter/_tests/test_celltype_config.py`

 * *Files identical despite different names*

### Comparing `napari-3d-counter-0.1.9/src/napari_3d_counter/_tests/test_python_gen.py` & `napari_3d_counter-0.2.1/src/napari_3d_counter/_tests/test_python_gen.py`

 * *Files identical despite different names*

### Comparing `napari-3d-counter-0.1.9/src/napari_3d_counter/_tests/test_reconstruct.py` & `napari_3d_counter-0.2.1/src/napari_3d_counter/_tests/test_reconstruct.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from napari_3d_counter import reconstruct_selected
 
 
 def place_ball(
     image: np.ndarray, position: Tuple[int, int, int], number: int, radius=5
 ) -> np.ndarray:
     ball_z, ball_x, ball_y = np.where(ball(radius))
-    image[
-        ball_z + position[0], ball_x + position[1], ball_y + position[2]
-    ] = number
+    image[ball_z + position[0], ball_x + position[1], ball_y + position[2]] = (
+        number
+    )
     return image
 
 
 def make_sample_data(points: List[Tuple[int, int, int]]) -> np.ndarray:
     labels = np.zeros(shape=(30, 200, 200)).astype(int)
     for i, point in enumerate(points, start=1):
         labels = place_ball(labels, tuple(p - 5 for p in point), i)
```

### Comparing `napari-3d-counter-0.1.9/src/napari_3d_counter/_tests/test_widget.py` & `napari_3d_counter-0.2.1/src/napari_3d_counter/_tests/test_widget.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,34 @@
+from __future__ import annotations
 from dataclasses import dataclass
 from typing import List, Optional
 
 import numpy as np
 import pandas as pd
 from matplotlib.colors import to_hex, to_rgba_array
+import pytest
 
 from napari_3d_counter import CellTypeConfig, Count3D
 from napari_3d_counter.celltype_config import DEFAULT_COLOR_SEQUENCE
+from napari_3d_counter._widget import CellTypeGuiAndData
 
 import napari
 
 
 @dataclass
 class Event:
     value: Optional[List[np.ndarray]] = None
+    action: Optional[str] = "added"
+
+
+def total_n_points(cell_type_gui_and_data: list[CellTypeGuiAndData]):
+    sum = 0
+    for cell_type in cell_type_gui_and_data:
+        sum = sum + cell_type.layer.data.shape[0]
+    return sum
 
 
 # make_napari_viewer is a pytest fixture that returns a napari viewer object
 # capsys is a pytest fixture that captures stdout and stderr output streams
 def test_change_state(make_napari_viewer):
     # make viewer and add an image layer using our fixture
     viewer = make_napari_viewer()
@@ -48,19 +59,21 @@
     # make viewer and add an image layer using our fixture
     viewer = make_napari_viewer()
     viewer.add_image(np.random.random((100, 100, 100)))
 
     # create our widget, passing in the viewer
     my_widget = Count3D(viewer)
     event = Event()
+    default_celltype = my_widget.cell_type_gui_and_data[0]
     event.value = [np.array([1, 1, 1])]
     my_widget.new_pointer_point(event)
+    print(default_celltype.layer.data.shape)
+    assert default_celltype.layer.data.shape == (1, 3)
     event.value = [np.array([2, 2, 2])]
     my_widget.new_pointer_point(event)
-    default_celltype = my_widget.cell_type_gui_and_data[0]
     assert default_celltype.layer.data.shape == (2, 3)
 
 
 def test_keybind_conflict(make_napari_viewer):
     viewer = make_napari_viewer()
     config = [CellTypeConfig(keybind="q"), CellTypeConfig(keybind="q")]
     # create our widget, passing in the viewer
@@ -79,49 +92,160 @@
     event.value = [np.array([1, 1, 1])]
     my_widget.new_pointer_point(event)
     my_widget.undo()
     default_celltype = my_widget.cell_type_gui_and_data[0]
     assert len(default_celltype.layer.data) == 0
 
 
+def test_manual_add(make_napari_viewer):
+    viewer = make_napari_viewer()
+    # create our widget, passing in the viewer
+    my_widget = Count3D(viewer, cell_type_config=[CellTypeConfig("name")])
+    viewer.layers["name"].add([1, 2, 3])
+    assert viewer.layers["name"].data.shape == (1, 3)
+    assert len(my_widget.undo_stack) == 1
+
+
 def test_undo_from_manual_add(make_napari_viewer):
     # make viewer and add an image layer using our fixture
     viewer = make_napari_viewer()
     # create our widget, passing in the viewer
     my_widget = Count3D(viewer, cell_type_config=[CellTypeConfig("name")])
     assert len(my_widget.undo_stack) == 0
     viewer.layers["name"].add([1, 2, 3])
-    # assert len(my_widget.undo_stack) == 1
+    assert len(my_widget.undo_stack) == 1
+    print("undoing")
     my_widget.undo()
     assert len(my_widget.undo_stack) == 0
 
 
+def test_undo_across_states_again(make_napari_viewer):
+    # make viewer and add an image layer using our fixture
+    viewer = make_napari_viewer()
+    viewer.add_image(np.random.random((100, 100, 100)))
+    # create our widget, passing in the viewer
+    my_widget = Count3D(
+        viewer,
+        cell_type_config=[CellTypeConfig("name"), CellTypeConfig("two")],
+    )
+    event = Event()
+    my_widget.change_state_to(my_widget.cell_type_gui_and_data[0])
+    assert (
+        total_n_points(my_widget.cell_type_gui_and_data)
+        == 0
+        == len(my_widget.undo_stack)
+    )
+    event.value = [np.array([1, 1, 1])]
+    my_widget.new_pointer_point(event)
+    assert (
+        total_n_points(my_widget.cell_type_gui_and_data)
+        == 1
+        == len(my_widget.undo_stack)
+    )
+    my_widget.change_state_to(my_widget.cell_type_gui_and_data[1])
+    event.value = [np.array([2, 2, 2])]
+    my_widget.new_pointer_point(event)
+    assert (
+        total_n_points(my_widget.cell_type_gui_and_data)
+        == 2
+        == len(my_widget.undo_stack)
+    )
+    my_widget.change_state_to(my_widget.cell_type_gui_and_data[1])
+    event.value = [np.array([1, 1, 1])]
+    my_widget.new_pointer_point(event)
+    assert (
+        total_n_points(my_widget.cell_type_gui_and_data)
+        == 3
+        == len(my_widget.undo_stack)
+    )
+    my_widget.change_state_to(my_widget.cell_type_gui_and_data[1])
+    event.value = [np.array([2, 2, 2])]
+    my_widget.new_pointer_point(event)
+    assert (
+        total_n_points(my_widget.cell_type_gui_and_data)
+        == 4
+        == len(my_widget.undo_stack)
+    )
+    my_widget.undo()
+    assert (
+        total_n_points(my_widget.cell_type_gui_and_data)
+        == 3
+        == len(my_widget.undo_stack)
+    )
+    my_widget.undo()
+    assert (
+        total_n_points(my_widget.cell_type_gui_and_data)
+        == 2
+        == len(my_widget.undo_stack)
+    )
+    my_widget.undo()
+    assert (
+        total_n_points(my_widget.cell_type_gui_and_data)
+        == 1
+        == len(my_widget.undo_stack)
+    )
+    my_widget.undo()
+    assert (
+        total_n_points(my_widget.cell_type_gui_and_data)
+        == 0
+        == len(my_widget.undo_stack)
+    )
+
+
 def test_undo_across_states(make_napari_viewer):
     # make viewer and add an image layer using our fixture
     viewer = make_napari_viewer()
     viewer.add_image(np.random.random((100, 100, 100)))
 
     # create our widget, passing in the viewer
-    my_widget = Count3D(viewer)
+
+    my_widget = Count3D(
+        viewer,
+        cell_type_config=[CellTypeConfig("name"), CellTypeConfig("two")],
+    )
     event = Event()
+    my_widget.change_state_to(my_widget.cell_type_gui_and_data[0])
+    assert total_n_points(my_widget.cell_type_gui_and_data) == 0
     event.value = [np.array([1, 1, 1])]
     my_widget.new_pointer_point(event)
+    assert total_n_points(my_widget.cell_type_gui_and_data) == 1
+    my_widget.change_state_to(my_widget.cell_type_gui_and_data[1])
     event.value = [np.array([2, 2, 2])]
     my_widget.new_pointer_point(event)
-    my_widget.change_state_to(my_widget.cell_type_gui_and_data[1])
+    assert total_n_points(my_widget.cell_type_gui_and_data) == 2
+    my_widget.change_state_to(my_widget.cell_type_gui_and_data[0])
     my_widget.new_pointer_point(event)
+    assert total_n_points(my_widget.cell_type_gui_and_data) == 3
     event.value = [np.array([2, 2, 2])]
     my_widget.undo()  # other state
+    assert total_n_points(my_widget.cell_type_gui_and_data) == 2
     my_widget.undo()  # current state state
+    assert total_n_points(my_widget.cell_type_gui_and_data) == 1
     default_celltype = my_widget.cell_type_gui_and_data[0]
-    assert len(default_celltype.layer.data) == 1
-    # saturate undos without errors
     my_widget.undo()
+    assert total_n_points(my_widget.cell_type_gui_and_data) == 0
+
+
+def test_undo_from_manual_add_across_states(make_napari_viewer):
+    # make viewer and add an image layer using our fixture
+    viewer = make_napari_viewer()
+    # create our widget, passing in the viewer
+    my_widget = Count3D(
+        viewer, cell_type_config=[CellTypeConfig("one"), CellTypeConfig("two")]
+    )
+    assert len(my_widget.undo_stack) == 0
+    viewer.layers["one"].add([1, 2, 3])
+    viewer.layers["two"].add([1, 2, 3])
+    assert len(my_widget.undo_stack) == 2
     my_widget.undo()
+    assert len(my_widget.undo_stack) == 1
+    assert total_n_points(my_widget.cell_type_gui_and_data) == 1
     my_widget.undo()
+    assert len(my_widget.undo_stack) == 0
+    assert total_n_points(my_widget.cell_type_gui_and_data) == 0
 
 
 def test_name_counter(make_napari_viewer):
     viewer = make_napari_viewer()
     my_widget = Count3D(viewer)
     event = Event()
     event.value = [np.array([1, 1, 1])]
@@ -227,14 +351,16 @@
     my_widget.read_points_from_df(df)
     cell_type = my_widget.cell_type_gui_and_data[-1]
     assert cell_type.layer.name == "test_name"
     assert cell_type.layer.data.shape[0] == 1
 
 
 def test_change_symbol(make_napari_viewer):
+    if napari.__version__.split(".")[:3] == ["0", "4", "19"]:
+        pytest.skip("changing symbol not supported in napari 0.4.19")
     viewer = make_napari_viewer()
     my_widget = Count3D(viewer, [CellTypeConfig(name="test_name")])
     my_widget.new_pointer_point(Event([np.array([1, 2, 1])]))
     cell_type = my_widget.cell_type_gui_and_data[0]
     star = napari.layers.points._points_constants.Symbol.STAR
     cell_type.layer.current_symbol = star
     assert cell_type.layer.symbol[0] == star
@@ -280,8 +406,8 @@
 # my_widget(viewer.layers[0])
 
 # # read captured output and check that it's as we expected
 # captured = capsys.readouterr()
 # assert captured.out == f"you have selected {layer}\n"
 
 if __name__ == "__main__":
-    test_change_face_color(napari.viewer.Viewer)
+    test_undo_across_states_again(napari.viewer.Viewer)
```

### Comparing `napari-3d-counter-0.1.9/src/napari_3d_counter/_widget.py` & `napari_3d_counter-0.2.1/src/napari_3d_counter/_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 implements the counting interface and the reconstruction plugin
 """
 
 from dataclasses import dataclass
 from functools import partial
 from pathlib import Path
 from typing import List, Optional, Literal
+from threading import Lock
 
 import napari
 import numpy as np
 import pandas as pd
 from matplotlib.colors import to_hex, to_rgba_array
 from napari.utils.events import Event
 from qtpy.QtCore import Qt  # type: ignore
@@ -78,19 +79,23 @@
     """
     Represents the cell type GUI and data
     """
 
     keybind: str
     button: QPushButton
     layer: napari.layers.Points
+    gui_lock: Lock
 
     def update_button_gui(self):
         """
         Updates the button with current name, and number of cells
         """
+        # do nothing if gui_lock is locked
+        if self.gui_lock.locked():
+            return
         # update the button
         keybind_str = f" ({self.keybind})" if self.keybind else ""
         button_text = (
             f"[{self.layer.data.shape[0]}] {self.layer.name}" + keybind_str
         )
         self.button.setText(button_text)
         color = to_hex(self.layer.current_edge_color)
@@ -152,15 +157,15 @@
             cell_type_config = DEFUALT_CONFIG
         self.initial_config = process_cell_type_config(cell_type_config)
         # viewer is needed to add layers
         self.viewer = napari_viewer
         # a stack containing points with added layers
         self.undo_stack: List[CellTypeGuiAndData] = []
         # prevents unwanted animations
-        self.currently_adding_point = False
+        self.gui_lock = Lock()
         # add out of slice markers
         self.out_of_slice_points = self.viewer.add_points(
             ndim=2,
             size=self.initial_config[0].out_of_slice_point_size,
             name="out of slice",
         )
         # set up cell type points layers
@@ -226,15 +231,22 @@
         assert ndims == 2
         self.out_of_slice_points.data = data
 
     def handle_data_changed(self, event: Event):
         """
         Handle adding point specific to the layer
         """
-        if self.currently_adding_point:
+        # try:
+        # event.value[0]
+        # except IndexError:
+        # # received an empty event
+        # return
+        if self.gui_lock.locked():
+            return
+        if event.action == "added":
             return
         # add to out_of_slice_points
         self.update_out_of_slice()
         # figure out current cell type
         current_points = event.source
         current_cell_type = next(
             cell_type
@@ -247,28 +259,36 @@
         current_cell_type.update_button_gui()
 
     def new_pointer_point(self, event: Event):
         """
         Handle a new point being added to the pointer
         by adding to the correct sub-layer
         """
+        if event.action == "adding":
+            return
+        if self.gui_lock.locked():
+            return
         pointer_coords = event.value
+        assert self.gui_lock.acquire(blocking=False)
         self.pointer.data = []
+        self.gui_lock.release()
         current_cell_type = self.pointer_type_state
         # dispatch point to appropriate layer
         # implicitly calls self.handle_data_changed
         current_point_layer = current_cell_type.layer
+        # import pudb; pudb.set_trace()
         current_point_layer.add(coords=pointer_coords)
         # hack to unselect last added point
         # prevent layer specific handlers from updating
-        self.currently_adding_point = True
         # add and remove point
+        assert self.gui_lock.acquire(blocking=False)
         current_point_layer.add(coords=pointer_coords)
         current_point_layer.remove_selected()
-        self.currently_adding_point = False
+        self.gui_lock.release()
+        self.update_out_of_slice()
 
     def update_gui(self):
         """
         Updates button color and button text
         """
         for cell_type in self.cell_type_gui_and_data:
             cell_type.update_button_gui()
@@ -293,15 +313,18 @@
             symbol=config.symbol,
             face_color=config.face_color,
             edge_width=config.edge_width,
         )
         point_layer.events.data.connect(self.handle_data_changed)
         btn = QPushButton()
         out = CellTypeGuiAndData(
-            keybind=config.keybind, button=btn, layer=point_layer
+            keybind=config.keybind,
+            button=btn,
+            layer=point_layer,
+            gui_lock=self.gui_lock,
         )
         # set up event handler that changes state to this
         change_state_fun = NamedPartial(
             partial(self.change_state_to, out), config.name
         )
         if config.keybind:
             try:
@@ -317,20 +340,25 @@
         # Update rest of the points when face_color, size, symbol, edge_width changes
         point_layer.events.current_face_color.connect(
             partial(out.update_attr, "face_color")
         )
         point_layer.events.current_size.connect(
             partial(out.update_attr, "size")
         )
-        point_layer.events.current_symbol.connect(
-            partial(out.update_attr, "symbol")
-        )
         point_layer.events.current_edge_width.connect(
             partial(out.update_attr, "edge_width")
         )
+        def update_symbol():
+            if napari.__version__.split(".")[:3] == ["0", "4", "19"]:
+                # see https://github.com/napari/napari/issues/6865
+                print("Updating exising symbols is not supported in napari 0.4.19\n"
+                      "This feature is availible in napari 0.4.18")
+            else:
+                out.update_attr("symbol")
+        point_layer.events.current_symbol.connect(update_symbol)
         return out
 
     def change_state_to(self, state: CellTypeGuiAndData, *args, **kwargs):
         """
         Changes the state
         """
         # handler for qt events
@@ -362,15 +390,17 @@
         _ = args
         _ = kwargs
         if not self.undo_stack:
             print("No previous changes")
             return
         cell_type = self.undo_stack.pop()
         point_layer = cell_type.layer
+        assert self.gui_lock.acquire(blocking=True)
         point_layer.data = point_layer.data[:-1]
+        self.gui_lock.release()
         self.update_out_of_slice()
         # update button
         cell_type.update_button_gui()
 
     def config_in_python(self) -> str:
         """
         Creates a python string that when run,
```

### Comparing `napari-3d-counter-0.1.9/src/napari_3d_counter/celltype_config.py` & `napari_3d_counter-0.2.1/src/napari_3d_counter/celltype_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,17 +140,19 @@
             name_int += 1
         unique_names.append(f"{name} [{name_int}]")
     outline_sizes = [
         DEFAULT_OUTLINE_SIZE if c.outline_size is None else c.outline_size
         for c in cell_type_configs
     ]
     out_of_slice_sizes = [
-        DEFAULT_OUT_OF_SLICE_SIZE
-        if c.out_of_slice_point_size is None
-        else c.out_of_slice_point_size
+        (
+            DEFAULT_OUT_OF_SLICE_SIZE
+            if c.out_of_slice_point_size is None
+            else c.out_of_slice_point_size
+        )
         for c in cell_type_configs
     ]
     symbols = [
         DEFAULT_SYMBOL if c.symbol is None else c.symbol
         for c in cell_type_configs
     ]
     face_colors = [
```

### Comparing `napari-3d-counter-0.1.9/src/napari_3d_counter/napari.yaml` & `napari_3d_counter-0.2.1/src/napari_3d_counter/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-3d-counter-0.1.9/src/napari_3d_counter.egg-info/PKG-INFO` & `napari_3d_counter-0.2.1/src/napari_3d_counter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-3d-counter
-Version: 0.1.9
+Version: 0.2.1
 Summary: A simple plugin for counting objects in 3D images
 Home-page: https://github.com/pnewstein/napari-3d-counter
 Author: Peter Newstein
 Author-email: peternewstein@gmail.com
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://github.com/pnewstein/napari-3d-counter/issues
 Project-URL: Documentation, https://github.com/pnewstein/napari-3d-counter#README.md
@@ -26,15 +26,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: qtpy
 Requires-Dist: pandas
 Requires-Dist: scikit-image
 Requires-Dist: matplotlib
-Requires-Dist: napari==0.4.18
+Requires-Dist: napari<=0.4.19
 Provides-Extra: testing
 Requires-Dist: tox; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-qt; extra == "testing"
 Requires-Dist: napari; extra == "testing"
 Requires-Dist: pyqt5; extra == "testing"
```

### Comparing `napari-3d-counter-0.1.9/src/napari_3d_counter.egg-info/SOURCES.txt` & `napari_3d_counter-0.2.1/src/napari_3d_counter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-3d-counter-0.1.9/tox.ini` & `napari_3d_counter-0.2.1/tox.ini`

 * *Files identical despite different names*

