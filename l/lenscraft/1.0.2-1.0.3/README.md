# Comparing `tmp/lenscraft-1.0.2.tar.gz` & `tmp/lenscraft-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lenscraft-1.0.2.tar", last modified: Wed Apr 24 19:09:38 2024, max compression
+gzip compressed data, was "lenscraft-1.0.3.tar", last modified: Fri Apr 26 14:09:31 2024, max compression
```

## Comparing `lenscraft-1.0.2.tar` & `lenscraft-1.0.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:09:38.389312 lenscraft-1.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     3947 2024-04-23 18:41:25.000000 lenscraft-1.0.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      503 2024-04-23 19:08:22.000000 lenscraft-1.0.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1672 2024-04-23 18:41:25.000000 lenscraft-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1300 2024-04-24 19:09:38.389312 lenscraft-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      584 2024-04-23 19:24:28.000000 lenscraft-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:09:38.377311 lenscraft-1.0.2/images/
--rw-rw-rw-   0 root         (0) root         (0)   776666 2024-04-23 18:41:25.000000 lenscraft-1.0.2/images/0.9858_1.1766.png
--rw-rw-rw-   0 root         (0) root         (0)   192094 2024-04-23 18:41:25.000000 lenscraft-1.0.2/images/334.png
--rw-rw-rw-   0 root         (0) root         (0)  4916278 2024-04-23 18:41:25.000000 lenscraft-1.0.2/images/Ring_9_9.png
--rw-rw-rw-   0 root         (0) root         (0)    15666 2024-04-23 18:41:25.000000 lenscraft-1.0.2/images/mask.png
--rw-rw-rw-   0 root         (0) root         (0)   755205 2024-04-23 18:41:25.000000 lenscraft-1.0.2/images/spacer_top__13.png
--rw-rw-rw-   0 root         (0) root         (0)   609893 2024-04-23 18:41:25.000000 lenscraft-1.0.2/images/spacer_top__14.png
--rw-rw-rw-   0 root         (0) root         (0)   750759 2024-04-23 18:41:25.000000 lenscraft-1.0.2/images/spacer_top__3.png
--rw-rw-rw-   0 root         (0) root         (0)   916168 2024-04-23 18:41:25.000000 lenscraft-1.0.2/images/spacer_top__9.png
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-23 19:08:22.000000 lenscraft-1.0.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-23 18:41:25.000000 lenscraft-1.0.2/requirments.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 19:09:38.389312 lenscraft-1.0.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:09:38.333308 lenscraft-1.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:09:38.381311 lenscraft-1.0.2/src/lenscraft/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-24 19:00:28.000000 lenscraft-1.0.2/src/lenscraft/__main__.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-04-24 19:09:38.000000 lenscraft-1.0.2/src/lenscraft/_version.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:09:38.385311 lenscraft-1.0.2/src/lenscraft/assets/
--rw-rw-rw-   0 root         (0) root         (0)      923 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/assets/CornerTemplate.png
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:09:38.385311 lenscraft-1.0.2/src/lenscraft/editor/
--rw-rw-rw-   0 root         (0) root         (0)     5370 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/editor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7721 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/gabor.py
--rw-rw-rw-   0 root         (0) root         (0)     5774 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/image.py
--rw-rw-rw-   0 root         (0) root         (0)    17849 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/nodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:09:38.389312 lenscraft-1.0.2/src/lenscraft/texture/
--rw-rw-rw-   0 root         (0) root         (0)      637 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/texture/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2682 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/texture/classify.py
--rw-rw-rw-   0 root         (0) root         (0)    13972 2024-04-24 19:00:28.000000 lenscraft-1.0.2/src/lenscraft/texture/tool.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:09:38.389312 lenscraft-1.0.2/src/lenscraft.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1300 2024-04-24 19:09:38.000000 lenscraft-1.0.2/src/lenscraft.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      877 2024-04-24 19:09:38.000000 lenscraft-1.0.2/src/lenscraft.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 19:09:38.000000 lenscraft-1.0.2/src/lenscraft.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-04-24 19:09:38.000000 lenscraft-1.0.2/src/lenscraft.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      126 2024-04-24 19:09:38.000000 lenscraft-1.0.2/src/lenscraft.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-24 19:09:38.000000 lenscraft-1.0.2/src/lenscraft.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:09:38.389312 lenscraft-1.0.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:41:25.000000 lenscraft-1.0.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:09:31.311537 lenscraft-1.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2024-04-23 18:41:25.000000 lenscraft-1.0.3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      503 2024-04-23 19:08:22.000000 lenscraft-1.0.3/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2024-04-23 18:41:25.000000 lenscraft-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1300 2024-04-26 14:09:31.311537 lenscraft-1.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      584 2024-04-23 19:24:28.000000 lenscraft-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:09:31.299537 lenscraft-1.0.3/images/
+-rw-rw-rw-   0 root         (0) root         (0)   776666 2024-04-23 18:41:25.000000 lenscraft-1.0.3/images/0.9858_1.1766.png
+-rw-rw-rw-   0 root         (0) root         (0)   192094 2024-04-23 18:41:25.000000 lenscraft-1.0.3/images/334.png
+-rw-rw-rw-   0 root         (0) root         (0)  4916278 2024-04-23 18:41:25.000000 lenscraft-1.0.3/images/Ring_9_9.png
+-rw-rw-rw-   0 root         (0) root         (0)    15666 2024-04-23 18:41:25.000000 lenscraft-1.0.3/images/mask.png
+-rw-rw-rw-   0 root         (0) root         (0)   755205 2024-04-23 18:41:25.000000 lenscraft-1.0.3/images/spacer_top__13.png
+-rw-rw-rw-   0 root         (0) root         (0)   609893 2024-04-23 18:41:25.000000 lenscraft-1.0.3/images/spacer_top__14.png
+-rw-rw-rw-   0 root         (0) root         (0)   750759 2024-04-23 18:41:25.000000 lenscraft-1.0.3/images/spacer_top__3.png
+-rw-rw-rw-   0 root         (0) root         (0)   916168 2024-04-23 18:41:25.000000 lenscraft-1.0.3/images/spacer_top__9.png
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-23 19:08:22.000000 lenscraft-1.0.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-23 18:41:25.000000 lenscraft-1.0.3/requirments.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 14:09:31.311537 lenscraft-1.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:09:31.263534 lenscraft-1.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:09:31.307537 lenscraft-1.0.3/src/lenscraft/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-24 19:00:28.000000 lenscraft-1.0.3/src/lenscraft/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-04-26 14:09:31.000000 lenscraft-1.0.3/src/lenscraft/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:09:31.311537 lenscraft-1.0.3/src/lenscraft/assets/
+-rw-rw-rw-   0 root         (0) root         (0)      923 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/assets/CornerTemplate.png
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:09:31.311537 lenscraft-1.0.3/src/lenscraft/editor/
+-rw-rw-rw-   0 root         (0) root         (0)     5370 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/editor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7721 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/gabor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5774 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/image.py
+-rw-rw-rw-   0 root         (0) root         (0)    17849 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/nodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:09:31.311537 lenscraft-1.0.3/src/lenscraft/texture/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/texture/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2682 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/texture/classify.py
+-rw-rw-rw-   0 root         (0) root         (0)    14340 2024-04-26 14:03:03.000000 lenscraft-1.0.3/src/lenscraft/texture/tool.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:09:31.311537 lenscraft-1.0.3/src/lenscraft.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1300 2024-04-26 14:09:31.000000 lenscraft-1.0.3/src/lenscraft.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      877 2024-04-26 14:09:31.000000 lenscraft-1.0.3/src/lenscraft.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 14:09:31.000000 lenscraft-1.0.3/src/lenscraft.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-26 14:09:31.000000 lenscraft-1.0.3/src/lenscraft.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2024-04-26 14:09:31.000000 lenscraft-1.0.3/src/lenscraft.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-26 14:09:31.000000 lenscraft-1.0.3/src/lenscraft.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:09:31.311537 lenscraft-1.0.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:41:25.000000 lenscraft-1.0.3/tests/__init__.py
```

### Comparing `lenscraft-1.0.2/.gitignore` & `lenscraft-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/LICENSE` & `lenscraft-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/PKG-INFO` & `lenscraft-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lenscraft
-Version: 1.0.2
+Version: 1.0.3
 Summary: Application to quickly build machine vision pipelines with little or no code
 Author-email: Gudjon Einar Magnusson <gmagnusson@fraunhofer.org>
 Project-URL: Homepage, https://cma.fraunhofer.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `lenscraft-1.0.2/README.md` & `lenscraft-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/images/0.9858_1.1766.png` & `lenscraft-1.0.3/images/0.9858_1.1766.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/images/334.png` & `lenscraft-1.0.3/images/334.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/images/Ring_9_9.png` & `lenscraft-1.0.3/images/Ring_9_9.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/images/mask.png` & `lenscraft-1.0.3/images/mask.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/images/spacer_top__13.png` & `lenscraft-1.0.3/images/spacer_top__13.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/images/spacer_top__14.png` & `lenscraft-1.0.3/images/spacer_top__14.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/images/spacer_top__3.png` & `lenscraft-1.0.3/images/spacer_top__3.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/images/spacer_top__9.png` & `lenscraft-1.0.3/images/spacer_top__9.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/pyproject.toml` & `lenscraft-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/src/lenscraft/assets/CornerTemplate.png` & `lenscraft-1.0.3/src/lenscraft/assets/CornerTemplate.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/src/lenscraft/editor/__init__.py` & `lenscraft-1.0.3/src/lenscraft/editor/__init__.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/src/lenscraft/gabor.py` & `lenscraft-1.0.3/src/lenscraft/gabor.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/src/lenscraft/image.py` & `lenscraft-1.0.3/src/lenscraft/image.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/src/lenscraft/nodes.py` & `lenscraft-1.0.3/src/lenscraft/nodes.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/src/lenscraft/texture/__init__.py` & `lenscraft-1.0.3/src/lenscraft/texture/__init__.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/src/lenscraft/texture/classify.py` & `lenscraft-1.0.3/src/lenscraft/texture/classify.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/src/lenscraft/texture/tool.py` & `lenscraft-1.0.3/src/lenscraft/texture/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 from typing import List, Optional
 import dearpygui.dearpygui as dpg
 import numpy as np
 import shapely
 from shapely.affinity import scale, translate
 import cv2
 
@@ -275,25 +276,25 @@
         self.start = np.array(start) if start else None
         self.end = np.array(end) if end else None
         self.done = False
         self.line_id = None
         self.outside_polygon_id = None
         self.inside_polygon_id = None
         self.width = width  # Width of the rectangles
+        self._last_draw = 0
 
     def length(self):
         v = self.start - self.end
         return np.linalg.norm(v)
 
     def mouse_move(self, pos):
         # pos = np.array(dpg.get_mouse_pos(local=True))
         if not self.done:
             self.end = pos
             self.draw()
-            self.draw_rectangles()
 
     def mouse_click(self, pos):
         # pos = np.array(dpg.get_mouse_pos(local=True))
         if self.start is None:
             print("Start", pos)
             self.start = pos
         elif not self.done:
@@ -310,30 +311,40 @@
             dpg.delete_item(self.line_id)
         if self.outside_polygon_id is not None:
             dpg.delete_item(self.outside_polygon_id)
         if self.inside_polygon_id is not None:
             dpg.delete_item(self.inside_polygon_id)
 
     def draw(self):
-        if self.line_id:
+        dt = time.time() - self._last_draw
+        if dt < 0.05:
+            # Prevent drawing too fast
+            return
+        
+        self.draw_line()
+        self.draw_rectangles()
+        self._last_draw = time.time()
+
+    def draw_line(self):
+        if self.line_id and dpg.does_item_exist(self.line_id):
             dpg.delete_item(self.line_id)
 
         if self.start is not None and self.end is not None:
             self.line_id = dpg.draw_line(
                 self.start,
                 self.end,
                 color=(255, 0, 0, 255),
                 thickness=3,
                 parent=self.tab.canvas_id,
             )
 
     def draw_rectangles(self):
-        if self.outside_polygon_id is not None:
+        if self.outside_polygon_id and dpg.does_item_exist(self.outside_polygon_id):
             dpg.delete_item(self.outside_polygon_id)
-        if self.inside_polygon_id is not None:
+        if self.inside_polygon_id and dpg.does_item_exist(self.inside_polygon_id):
             dpg.delete_item(self.inside_polygon_id)
 
         width = max(self.length() / 3, self.width)
         x, y = self.outside_region(width).exterior.xy
         points_outside = list(zip(x, y))
         self.outside_polygon_id = dpg.draw_polygon(
             points=points_outside,
```

### Comparing `lenscraft-1.0.2/src/lenscraft/utils.py` & `lenscraft-1.0.3/src/lenscraft/utils.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.2/src/lenscraft.egg-info/PKG-INFO` & `lenscraft-1.0.3/src/lenscraft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lenscraft
-Version: 1.0.2
+Version: 1.0.3
 Summary: Application to quickly build machine vision pipelines with little or no code
 Author-email: Gudjon Einar Magnusson <gmagnusson@fraunhofer.org>
 Project-URL: Homepage, https://cma.fraunhofer.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `lenscraft-1.0.2/src/lenscraft.egg-info/SOURCES.txt` & `lenscraft-1.0.3/src/lenscraft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

