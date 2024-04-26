# Comparing `tmp/aviewpy-1.3.5.tar.gz` & `tmp/aviewpy-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aviewpy-1.3.5.tar", last modified: Fri Sep  1 14:14:22 2023, max compression
+gzip compressed data, was "aviewpy-1.3.6.tar", last modified: Fri Apr 26 20:28:56 2024, max compression
```

## Comparing `aviewpy-1.3.5.tar` & `aviewpy-1.3.6.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-09-01 14:14:22.224496 aviewpy-1.3.5/
--rw-rw-rw-   0        0        0     1091 2022-12-20 23:52:04.000000 aviewpy-1.3.5/LICENSE
--rw-rw-rw-   0        0        0       34 2022-12-20 23:52:04.000000 aviewpy-1.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0      664 2023-09-01 14:14:22.219494 aviewpy-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-03-03 21:26:40.000000 aviewpy-1.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-09-01 14:14:22.124496 aviewpy-1.3.5/aviewpy/
--rw-rw-rw-   0        0        0       66 2022-12-20 23:55:30.000000 aviewpy-1.3.5/aviewpy/__init__.py
--rw-rw-rw-   0        0        0    11000 2023-04-12 16:38:53.000000 aviewpy-1.3.5/aviewpy/contact.py
--rw-rw-rw-   0        0        0     3770 2022-12-21 00:15:59.000000 aviewpy-1.3.5/aviewpy/cs.py
-drwxrwxrwx   0        0        0        0 2023-09-01 14:14:22.198495 aviewpy-1.3.5/aviewpy/files/
--rw-rw-rw-   0        0        0        0 2022-12-21 00:31:35.000000 aviewpy-1.3.5/aviewpy/files/__init__.py
--rw-rw-rw-   0        0        0      331 2023-04-28 18:01:01.000000 aviewpy-1.3.5/aviewpy/files/acf.py
--rw-rw-rw-   0        0        0      309 2023-04-28 18:01:16.000000 aviewpy-1.3.5/aviewpy/files/adm.py
--rw-rw-rw-   0        0        0     2336 2023-08-31 19:45:31.000000 aviewpy-1.3.5/aviewpy/files/bin.py
--rw-rw-rw-   0        0        0     1412 2023-07-26 14:08:21.000000 aviewpy-1.3.5/aviewpy/files/cmd.py
--rw-rw-rw-   0        0        0     7470 2023-05-12 18:33:02.000000 aviewpy-1.3.5/aviewpy/files/shell.py
--rw-rw-rw-   0        0        0     7063 2023-05-03 15:18:21.000000 aviewpy-1.3.5/aviewpy/files/to.py
--rw-rw-rw-   0        0        0     3035 2023-04-26 14:59:26.000000 aviewpy-1.3.5/aviewpy/model.py
--rw-rw-rw-   0        0        0     1102 2023-02-01 01:25:09.000000 aviewpy-1.3.5/aviewpy/move.py
--rw-rw-rw-   0        0        0     5232 2023-03-03 21:02:08.000000 aviewpy-1.3.5/aviewpy/objects.py
--rw-rw-rw-   0        0        0     2557 2023-07-07 22:57:12.000000 aviewpy-1.3.5/aviewpy/results.py
--rw-rw-rw-   0        0        0     8469 2023-08-08 18:36:03.000000 aviewpy-1.3.5/aviewpy/sim.py
-drwxrwxrwx   0        0        0        0 2023-09-01 14:14:22.206496 aviewpy-1.3.5/aviewpy/ui/
--rw-rw-rw-   0        0        0        0 2022-12-21 14:52:37.000000 aviewpy-1.3.5/aviewpy/ui/__init__.py
--rw-rw-rw-   0        0        0      941 2023-06-06 21:51:39.000000 aviewpy-1.3.5/aviewpy/ui/alerts.py
--rw-rw-rw-   0        0        0     1372 2023-08-07 13:05:37.000000 aviewpy-1.3.5/aviewpy/ui/messages.py
--rw-rw-rw-   0        0        0     2807 2023-05-12 17:01:09.000000 aviewpy-1.3.5/aviewpy/ui/progressbar.py
--rw-rw-rw-   0        0        0      416 2023-02-14 13:55:42.000000 aviewpy-1.3.5/aviewpy/ui/windows.py
-drwxrwxrwx   0        0        0        0 2023-09-01 14:14:22.215494 aviewpy-1.3.5/aviewpy/utils/
--rw-rw-rw-   0        0        0       20 2022-12-21 00:01:02.000000 aviewpy-1.3.5/aviewpy/utils/__init__.py
--rw-rw-rw-   0        0        0     6041 2023-03-03 21:05:07.000000 aviewpy-1.3.5/aviewpy/utils/dereferencer.py
--rw-rw-rw-   0        0        0     1682 2023-03-18 19:28:15.000000 aviewpy-1.3.5/aviewpy/utils/excepthook.py
--rw-rw-rw-   0        0        0     5173 2022-12-20 23:52:04.000000 aviewpy-1.3.5/aviewpy/utils/res_to_csv.py
--rw-rw-rw-   0        0        0     3885 2023-06-06 14:31:27.000000 aviewpy-1.3.5/aviewpy/utils/utils.py
--rw-rw-rw-   0        0        0     6372 2023-08-28 13:25:45.000000 aviewpy-1.3.5/aviewpy/variables.py
-drwxrwxrwx   0        0        0        0 2023-09-01 14:14:22.178496 aviewpy-1.3.5/aviewpy.egg-info/
--rw-rw-rw-   0        0        0      664 2023-09-01 14:14:21.000000 aviewpy-1.3.5/aviewpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      774 2023-09-01 14:14:21.000000 aviewpy-1.3.5/aviewpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-01 14:14:21.000000 aviewpy-1.3.5/aviewpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-09-01 14:14:21.000000 aviewpy-1.3.5/aviewpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-09-01 14:14:21.000000 aviewpy-1.3.5/aviewpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-09-01 14:14:22.225496 aviewpy-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1094 2022-12-21 15:27:19.000000 aviewpy-1.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-01 14:14:22.217497 aviewpy-1.3.5/test/
--rw-rw-rw-   0        0        0     5501 2023-01-06 20:15:20.000000 aviewpy-1.3.5/test/test_shell.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:28:56.860620 aviewpy-1.3.6/
+-rw-rw-rw-   0        0        0     1091 2022-12-20 23:52:04.000000 aviewpy-1.3.6/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-12-20 23:52:04.000000 aviewpy-1.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      664 2024-04-26 20:28:56.859623 aviewpy-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-03-03 21:26:40.000000 aviewpy-1.3.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 20:28:56.789369 aviewpy-1.3.6/aviewpy/
+-rw-rw-rw-   0        0        0       66 2022-12-20 23:55:30.000000 aviewpy-1.3.6/aviewpy/__init__.py
+-rw-rw-rw-   0        0        0    10737 2023-10-27 17:38:38.000000 aviewpy-1.3.6/aviewpy/contact.py
+-rw-rw-rw-   0        0        0     3770 2022-12-21 00:15:59.000000 aviewpy-1.3.6/aviewpy/cs.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:28:56.842498 aviewpy-1.3.6/aviewpy/files/
+-rw-rw-rw-   0        0        0        0 2022-12-21 00:31:35.000000 aviewpy-1.3.6/aviewpy/files/__init__.py
+-rw-rw-rw-   0        0        0      331 2023-04-28 18:01:01.000000 aviewpy-1.3.6/aviewpy/files/acf.py
+-rw-rw-rw-   0        0        0      309 2023-04-28 18:01:16.000000 aviewpy-1.3.6/aviewpy/files/adm.py
+-rw-rw-rw-   0        0        0     2336 2023-08-31 19:45:31.000000 aviewpy-1.3.6/aviewpy/files/bin.py
+-rw-rw-rw-   0        0        0     1412 2023-07-26 14:08:21.000000 aviewpy-1.3.6/aviewpy/files/cmd.py
+-rw-rw-rw-   0        0        0     1610 2023-11-17 13:38:14.000000 aviewpy-1.3.6/aviewpy/files/mac.py
+-rw-rw-rw-   0        0        0      580 2023-10-10 16:15:01.000000 aviewpy-1.3.6/aviewpy/files/msg.py
+-rw-rw-rw-   0        0        0     7319 2023-09-29 18:30:32.000000 aviewpy-1.3.6/aviewpy/files/shell.py
+-rw-rw-rw-   0        0        0     7063 2023-11-17 13:34:49.000000 aviewpy-1.3.6/aviewpy/files/to.py
+-rw-rw-rw-   0        0        0     3035 2023-04-26 14:59:26.000000 aviewpy-1.3.6/aviewpy/model.py
+-rw-rw-rw-   0        0        0     1102 2023-02-01 01:25:09.000000 aviewpy-1.3.6/aviewpy/move.py
+-rw-rw-rw-   0        0        0     5232 2023-03-03 21:02:08.000000 aviewpy-1.3.6/aviewpy/objects.py
+-rw-rw-rw-   0        0        0     3214 2024-03-19 12:42:37.000000 aviewpy-1.3.6/aviewpy/results.py
+-rw-rw-rw-   0        0        0     8720 2024-03-20 14:04:02.000000 aviewpy-1.3.6/aviewpy/sim.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:28:56.849870 aviewpy-1.3.6/aviewpy/ui/
+-rw-rw-rw-   0        0        0        0 2022-12-21 14:52:37.000000 aviewpy-1.3.6/aviewpy/ui/__init__.py
+-rw-rw-rw-   0        0        0     1241 2024-03-28 12:05:14.000000 aviewpy-1.3.6/aviewpy/ui/alerts.py
+-rw-rw-rw-   0        0        0     1372 2023-10-25 13:46:23.000000 aviewpy-1.3.6/aviewpy/ui/messages.py
+-rw-rw-rw-   0        0        0     7226 2023-11-01 12:02:19.000000 aviewpy-1.3.6/aviewpy/ui/progressbar.py
+-rw-rw-rw-   0        0        0     1953 2024-03-13 20:53:21.000000 aviewpy-1.3.6/aviewpy/ui/turn_on_all_force_graphics.py
+-rw-rw-rw-   0        0        0      694 2023-10-31 19:17:26.000000 aviewpy-1.3.6/aviewpy/ui/windows.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:28:56.856620 aviewpy-1.3.6/aviewpy/utils/
+-rw-rw-rw-   0        0        0       20 2022-12-21 00:01:02.000000 aviewpy-1.3.6/aviewpy/utils/__init__.py
+-rw-rw-rw-   0        0        0     6041 2023-03-03 21:05:07.000000 aviewpy-1.3.6/aviewpy/utils/dereferencer.py
+-rw-rw-rw-   0        0        0     1682 2023-03-18 19:28:15.000000 aviewpy-1.3.6/aviewpy/utils/excepthook.py
+-rw-rw-rw-   0        0        0     7343 2024-03-26 18:21:09.000000 aviewpy-1.3.6/aviewpy/utils/fbd.py
+-rw-rw-rw-   0        0        0     5065 2024-03-20 14:06:29.000000 aviewpy-1.3.6/aviewpy/utils/res_to_csv.py
+-rw-rw-rw-   0        0        0     2888 2023-11-17 13:41:38.000000 aviewpy-1.3.6/aviewpy/utils/utils.py
+-rw-rw-rw-   0        0        0     7746 2024-04-02 14:49:41.000000 aviewpy-1.3.6/aviewpy/variables.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:28:56.829884 aviewpy-1.3.6/aviewpy.egg-info/
+-rw-rw-rw-   0        0        0      664 2024-04-26 20:28:56.000000 aviewpy-1.3.6/aviewpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      878 2024-04-26 20:28:56.000000 aviewpy-1.3.6/aviewpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 20:28:56.000000 aviewpy-1.3.6/aviewpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-26 20:28:56.000000 aviewpy-1.3.6/aviewpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-26 20:28:56.000000 aviewpy-1.3.6/aviewpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 20:28:56.860620 aviewpy-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1094 2022-12-21 15:27:19.000000 aviewpy-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:28:56.858620 aviewpy-1.3.6/test/
+-rw-rw-rw-   0        0        0     5501 2023-01-06 20:15:20.000000 aviewpy-1.3.6/test/test_shell.py
```

### Comparing `aviewpy-1.3.5/LICENSE` & `aviewpy-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.5/PKG-INFO` & `aviewpy-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aviewpy
-Version: 1.3.5
+Version: 1.3.6
 Summary: Python tools for working with in the Adams View python environment
 Home-page: https://github.com/bthornton191/aviewpy
 Author: Ben Thornton
 Author-email: ben.thornton@hexagon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `aviewpy-1.3.5/aviewpy/contact.py` & `aviewpy-1.3.6/aviewpy/contact.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         slip_gcs = CS(np.array([Adams.evaluate_exp(f'{self.name}.Slip_Velocity.{d}.values')
                                 for d in ('X', 'Y', 'Z')]).T)
         penetration = Adams.evaluate_exp(f'{self.name}.Penetration.Depth.values')
         normal_lcs: NDArray = mkr_gcs.rot.apply(normal_gcs.loc, inverse=True)
         normal_unit_lcs: NDArray = mkr_gcs.rot.apply(normal_unit_gcs.loc, inverse=True)
         friction_lcs: NDArray = mkr_gcs.rot.apply(friction_gcs.loc, inverse=True)
         slip_lcs: NDArray = mkr_gcs.rot.apply(slip_gcs.loc, inverse=True)
-        track_pos_lcs: NDArray = mkr_gcs.rot.apply((track_gcs-mkr_gcs).loc, inverse=True)
+        track_pos_lcs: NDArray = mkr_gcs.rot.apply((track_gcs - mkr_gcs).loc, inverse=True)
 
         if False:
             mod = get_parent_model(part)
             for (idx, loc_gcs), loc_lcs in zip(enumerate(track_gcs.loc), track_pos_lcs):
                 mkr_g = mod.ground_part.Markers.create(
                     location=list(loc_gcs),
                     relative_to=mod.ground_part,
@@ -186,15 +186,15 @@
     slip_gcs = CS(np.array([Adams.evaluate_exp(f'{track_name}.Slip_Velocity.{d}.values')
                             for d in ('X', 'Y', 'Z')]).T)
     penetration = Adams.evaluate_exp(f'{track_name}.Penetration.Depth.values')
     normal_lcs: NDArray = mkr_gcs.rot.apply(normal_gcs.loc, inverse=True)
     normal_unit_lcs: NDArray = mkr_gcs.rot.apply(normal_unit_gcs.loc, inverse=True)
     friction_lcs: NDArray = mkr_gcs.rot.apply(friction_gcs.loc, inverse=True)
     slip_lcs: NDArray = mkr_gcs.rot.apply(slip_gcs.loc, inverse=True)
-    track_pos_lcs: NDArray = mkr_gcs.rot.apply((track_gcs-mkr_gcs).loc, inverse=True)
+    track_pos_lcs: NDArray = mkr_gcs.rot.apply((track_gcs - mkr_gcs).loc, inverse=True)
 
     if TESTING:
         mod = get_parent_model(part)
         for (idx, loc_gcs), loc_lcs in zip(enumerate(track_gcs.loc), track_pos_lcs):
             mkr_g = mod.ground_part.Markers.create(
                 location=list(loc_gcs),
                 relative_to=mod.ground_part,
@@ -242,43 +242,39 @@
         **{k: [] for k in Track.COLS},
         **{f'{k}_{d}': [] for d, k in product(['x', 'y', 'z'], Track.COLS_WITH_COMPS)},
         'step': [],
         'contact': [],
         'track': []
     }).set_index('time', drop=True)]
 
-    inc = 100 / len(tracks) if len(tracks) > 0 else 0
-    with progress_bar(f'Processing {geom.parent.name}.{geom.name} contacts...') as pbar:
-        for track in tracks:
-
-            track_data = track.get_data(mkr=ref_mkr,
-                                        i_part=geom in track.cont.i_geometry)
-
-            # Organize the data into a dictionary
-            data = {}
-            for key, values in track_data._asdict().items():
-
-                # Check if `values` has multiple components
-                if isinstance(values, np.ndarray) and len(values.shape) > 1:
-
-                    # If `values` has multiple components,
-                    # split the components (x,y,z) and get magnitudes
-                    data = {
-                        **data,
-                        **{f'{key}_{d}': values[:, i] for i, d in enumerate(['x', 'y', 'z'])},
-                        key: np.sqrt(np.apply_along_axis(np.sum, 1, values**2))
-                    }
-
-                else:
-                    data[key] = values
-
-            # Create DataFrame and append to list
-            dfs.append(pd.DataFrame({**data,
-                                    'step': pd.Series(track_data.time).diff(-1).fillna(0)*-1,
-                                    'contact': track.cont.name,
-                                    'track': track.name})
-                    .set_index('time', drop=True)
-                    .sort_index())
+    for track in tracks:
 
-            pbar.progress += inc
+        track_data = track.get_data(mkr=ref_mkr,
+                                    i_part=geom in track.cont.i_geometry)
+
+        # Organize the data into a dictionary
+        data = {}
+        for key, values in track_data._asdict().items():
+
+            # Check if `values` has multiple components
+            if isinstance(values, np.ndarray) and len(values.shape) > 1:
+
+                # If `values` has multiple components,
+                # split the components (x,y,z) and get magnitudes
+                data = {
+                    **data,
+                    **{f'{key}_{d}': values[:, i] for i, d in enumerate(['x', 'y', 'z'])},
+                    key: np.sqrt(np.apply_along_axis(np.sum, 1, values**2))
+                }
+
+            else:
+                data[key] = values
+
+        # Create DataFrame and append to list
+        dfs.append(pd.DataFrame({**data,
+                                'step': pd.Series(track_data.time).diff(-1).fillna(0) * -1,
+                                 'contact': track.cont.name,
+                                 'track': track.name})
+                   .set_index('time', drop=True)
+                   .sort_index())
 
     return pd.concat(dfs)
```

### Comparing `aviewpy-1.3.5/aviewpy/cs.py` & `aviewpy-1.3.6/aviewpy/cs.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.5/aviewpy/files/bin.py` & `aviewpy-1.3.6/aviewpy/files/bin.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.5/aviewpy/files/cmd.py` & `aviewpy-1.3.6/aviewpy/files/cmd.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.5/aviewpy/files/shell.py` & `aviewpy-1.3.6/aviewpy/files/shell.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from functools import lru_cache
 from itertools import product
 from pathlib import Path
-from time import perf_counter
 from typing import List, Tuple
 import pickle as pkl
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import stl
 from mpl_toolkits import mplot3d
 from scipy.spatial import KDTree
 
-from aviewpy import files
 
 CACH_SUFFIX = '.bshl'
 
+
 def write_shell_file(points: List[Tuple[float, float, float]],
                      facets: List[Tuple[int, int, int]],
                      file_name: Path,
                      scale: float):
     """Writes a shell (.shl) file
 
     Parameters
@@ -36,38 +34,38 @@
     points, facets = drop_duplicates(points, facets)
     n_points = len(points)
     n_facets = len(facets)
 
     lines = [f'{n_points} {n_facets} {scale:.6f}']
     for point in points:
         lines.append(' '.join([f'{v:.8f}' for v in point]))
-    
+
     for facet in facets:
         lines.append(' '.join([str(len(facet))] + [f'{p+1:d}' for p in facet]))
 
     Path(file_name).write_text('\n'.join(lines))
 
 
 def drop_duplicates(points: List[Tuple[float, float, float]],
                     facets: List[Tuple[int, int, int]]):
-    
+
     df_points = pd.DataFrame(points, columns=['x', 'y', 'z'])
     df_points['duplicated'] = df_points.duplicated()
-    
+
     if df_points['duplicated'].any():
-        df_facets = pd.DataFrame(facets)        
+        df_facets = pd.DataFrame(facets)
         df_facets_new = df_facets.copy(deep=True)
         for idx, facet in df_facets.iterrows():
             for jdx, i_pt in enumerate(facet):
                 if df_points['duplicated'].loc[i_pt]:
 
                     new_i_pt = df_points[(df_points['x'] == df_points['x'].loc[i_pt])
-                                            & (df_points['y'] == df_points['y'].loc[i_pt])
-                                            & (df_points['z'] == df_points['z'].loc[i_pt])].iloc[0].name
-                    
+                                         & (df_points['y'] == df_points['y'].loc[i_pt])
+                                         & (df_points['z'] == df_points['z'].loc[i_pt])].iloc[0].name
+
                     df_facets_new.at[idx, jdx] = new_i_pt
 
         df_points_new = df_points.copy(deep=True).drop_duplicates()
         df_points_new['new_index'] = np.arange(len(df_points_new))
         df_facets_new = df_facets_new.applymap(lambda ipt: df_points_new.loc[ipt]['new_index'].astype(int))
 
         new_points = df_points_new[['x', 'y', 'z']].to_numpy()
@@ -75,14 +73,16 @@
 
     else:
         new_points, new_facets = points, facets
 
     return new_points, new_facets
 
 # @lru_cache(maxsize=1)
+
+
 def read_shell_file(file_name: Path, use_cache=True):
     """Reads a shell (.shl) file
 
     Parameters
     ----------
     file_name : Path
         Full path of shell file
@@ -103,45 +103,46 @@
             and file_name.stat().st_mtime < cache_file_name.stat().st_mtime):
         with open(file_name.with_suffix(CACH_SUFFIX), 'rb') as fid:
             points, facets = pkl.load(fid)
     else:
         def _parse_lines(lines):
             n_points, n_facets, *_ = [float(v) for v in lines[0].split()]
             points = [tuple(float(v) for v in line.split())
-                    for line in lines[1:int(n_points)+1]]
-            facets = [tuple(int(v)-1 for v in line.split()[1:])
-                    for line in lines[int(n_points)+1:int(n_points+n_facets)+1]
-                    if len(line.split()[1:]) > 2]
-                    
-            return points,facets
+                      for line in lines[1:int(n_points) + 1]]
+            facets = [tuple(int(v) - 1 for v in line.split()[1:])
+                      for line in lines[int(n_points) + 1:int(n_points + n_facets) + 1]
+                      if len(line.split()[1:]) > 2]
+
+            return points, facets
         lines = Path(file_name).read_text().splitlines()
-        
+
         try:
             points, facets = _parse_lines(lines)
         except Exception:                                                                               # pylint: disable=broad-except
             lines = [l for l in lines if all(is_number(v) for v in l.split())]
             points, facets = _parse_lines(lines)
 
         # Remove duplicate points
         points, facets = drop_duplicates(points, facets)
-    
+
         # Cache file
         with open(file_name.with_suffix(CACH_SUFFIX), 'wb') as fid:
             pkl.dump((points, facets), fid)
 
     return points, facets
 
 
 def is_number(s):
     try:
         float(s)
         return True
     except ValueError:
         return False
 
+
 def get_shell_diff_vectors(file_1: Path, file_2: Path):
     """Get a vector of the differences between two (.shl) files
 
     Parameters
     ----------
     file_1 : Path
         Full path of shell file 1
@@ -154,52 +155,53 @@
         True if the two files are the same
     """
     points_1, _ = read_shell_file(file_1)
     points_2, _ = read_shell_file(file_2)
 
     # Match each point in points_1 to the closest point in points_2 and create a dataframe of the distance components
     df = pd.DataFrame(points_1, columns=['x_1', 'y_1', 'z_1'])
-    
+
     df['idx_pt_2'] = KDTree(points_2).query(points_1)[1]
     df[['x_2', 'y_2', 'z_2']] = df['idx_pt_2'].apply(lambda idx: points_2[idx]).tolist()
 
     df[['d_x', 'd_y', 'd_z']] = df[['x_1', 'y_1', 'z_1']].to_numpy() - df[['x_2', 'y_2', 'z_2']].to_numpy()
 
     return df
 
 
 def get_shell_volume(points: List[Tuple[float, float, float]], facets: List[Tuple[int, int, int]]):
     """Get the volume of a shell
-    
+
     Parameters
     ----------
     points : List[Tuple[float, float, float]]
-        Shell points
+        xyz coordinates of shell points
     facets : List[Tuple[int, int, int]]
         Shell facets
-        
+
     Returns
     -------
     float
         Shell volume
     """
     mesh = to_stl_mesh(points, facets)
     volume, *_ = mesh.get_mass_properties()
     return abs(volume)
 
+
 def to_stl_mesh(points, facets):
     """Converts a shell to an stl mesh
 
     Parameters
     ----------
     points : List[Tuple[float, float, float]]
         Shell points
     facets : List[Tuple[int, int, int]]
         Shell facets (index 0)
-    
+
     Returns
     -------
     stl.mesh.Mesh
         Mesh
     """
     points = np.array(points)
     facets = np.array(facets)
@@ -218,20 +220,20 @@
     return mesh
 
 
 def plot_shell(points, facets):
 
     fig = plt.figure()
     ax = fig.add_subplot(projection='3d')
-    
+
     mesh = to_stl_mesh(points=points, facets=facets)
     mesh.update_normals()
     mesh.update_centroids()
-    
+
     ax.add_collection3d(mplot3d.art3d.Poly3DCollection(mesh.vectors, alpha=.75, edgecolor='k'))
     scale = mesh.points.flatten()
     ax.auto_scale_xyz(scale, scale, scale)
-    
+
     for centroid, normal in zip(mesh.centroids, mesh.normals):
-        ax.plot(*np.array([centroid, (centroid+normal*2)]).T, c='r')
+        ax.plot(*np.array([centroid, (centroid + normal * 2)]).T, c='r')
 
     return ax
```

### Comparing `aviewpy-1.3.5/aviewpy/files/to.py` & `aviewpy-1.3.6/aviewpy/files/to.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.5/aviewpy/model.py` & `aviewpy-1.3.6/aviewpy/model.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.5/aviewpy/move.py` & `aviewpy-1.3.6/aviewpy/move.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.5/aviewpy/objects.py` & `aviewpy-1.3.6/aviewpy/objects.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.5/aviewpy/results.py` & `aviewpy-1.3.6/aviewpy/results.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,96 @@
 from pathlib import Path
 from typing import List
+
+import Adams  # type: ignore
 from adamspy.postprocess.msg import get_errors
-import Adams # type: ignore # noqa # isort:skip
-from Analysis import Analysis # type: ignore # noqa # isort:skip
+from Analysis import Analysis  # type: ignore
+
+from aviewpy.objects import get_parent_model  # type: ignore
 
 SIM_STAT_ERROR_MSG = 'static equilibrium analysis has not been successful'
+PARSE_ERROR_MSG = 'errors found parsing command. command ignored.'
+
 
 def create_result(ans: Analysis, res_name: str, comp_name: str, values: List[float], units: str):
     """Convenience function to create a result component.
-    
+
     Parameters
     ----------
     ans : Analysis
         The analysis to create the result component in.
     res_name : str
         The name of the result set to create.
     comp_name : str
         The name of the result component to create.
     values : List[float]
         The values to set for the result component.
     units : str
         The units of the result component.
+
+    Returns
+    -------
+    Analysis
+        The analysis that the result component was created in. This is returned because the `ans` 
+        argument is not updated in place.
     """
     if len(values) == 0:
         raise ValueError('No values to create result component with.')
-    
+
+    if res_name in ans.results and comp_name in ans.results[res_name]:
+        raise ValueError(f'Result component {ans.name}.{res_name}.{comp_name} already exists!')
+
     value_str = ','.join([str(val) for val in values])
-    cmd = f'numeric_results create values values = {value_str} units = {units} new_result_set_component_name = {ans.full_name}.{res_name}.{comp_name}'
+    Adams.execute_cmd(f'numeric_results create values '
+                      f'units = {units} '
+                      f'new_result_set_component_name = {ans.full_name}.{res_name}.{comp_name} '
+                      f'values = {value_str}')
 
-    Adams.execute_cmd(cmd)
+    return get_parent_model(ans).Analyses[ans.name]
 
 
-def get_sim_errors(msg_file: Path, ignore_static: bool = False):
+def get_sim_errors(msg_file: Path, ignore_static: bool = False, ignore_parse: bool = False):
     """Get the simulation errors from a .msg file.
-    
+
     Parameters
     ----------
     msg_file : Path
         The .msg file to get the errors from.
-    
+
     Returns
     -------
     List[str]
         The list of errors.
     """
     errors: List[str] = get_errors(msg_file)
-    
+
     if ignore_static:
         errors = [e for e in errors if SIM_STAT_ERROR_MSG.lower() not in e.lower()]
-    
+
+    if ignore_parse:
+        errors = [e for e in errors if PARSE_ERROR_MSG.lower() not in e.lower()]
+
     return errors
 
+
 def write_results(ans: Analysis, file_name: Path, binary=False):
     """Write the results of an analysis.
-    
+
     Parameters
     ----------
     ans : Analysis
         The analysis to write the results of.
     binary : bool, optional
         Whether to write the results in binary format, by default False
     """
-    
+
     if binary and ans.parent is not None:
         xrf = Adams.evaluate_exp(f'user_string("{ans.parent.full_name}.analysis_flags.results_xrf")')
         Adams.evaluate_exp(f'output set results model = {ans.parent.full_name} xrf = off')
-    
+
     try:
-        
+
         Adams.execute_cmd(f'file analysis write analysis={ans.full_name} file="{file_name}"')
-        
+
     finally:
         if binary and ans.parent is not None:
             Adams.evaluate_exp(f'output set results model = {ans.parent.full_name} xrf = {xrf}')
```

### Comparing `aviewpy-1.3.5/aviewpy/sim.py` & `aviewpy-1.3.6/aviewpy/sim.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,61 @@
-from contextlib import contextmanager
-from numbers import Number
+import logging
 import os
-from pathlib import Path
 import platform
 import shutil
 import subprocess
-from typing import List, Tuple, Union
+from contextlib import contextmanager
 from math import log10
+from numbers import Number
+from pathlib import Path
+from typing import List, Tuple, Union
 
-import Adams # type: ignore
+import Adams  # type: ignore
 from Simulation import Simulation  # type: ignore
+
 from .files.bin import write_bin_file
+from .files.msg import get_process_id
 
 SIM_PREFERNCES = ['internal', 'external', 'write_files_only']
-
 SIM_EXTS = ['.acf', '.adm', '.xmt_txt', '.req', '.res', '.msg', '.out', '.gra']
 
-def static_funnel(steps: int, **kwargs: Union[float, Tuple[float, float]])->List[str]:
+
+LOG = logging.getLogger(__name__)
+
+
+def static_funnel(steps: int, **kwargs: Union[float, Tuple[float, float]]) -> List[str]:
     """Generate a list of acf commands to simulate a static equilibrium funnel.
-    
+
     Parameters
     ----------
     steps : int
         The number of steps in the funnel
     **kwargs : float or Tuple[float, float]]
         The parameters to vary in the funnel. The value can be a single number, in which case
         the parameter is held constant, or a tuple of two numbers, in which case the parameter
         is varied linearly between the two values.
     """
     lines = []
-    for step in range(1, steps+1):
+    for step in range(1, steps + 1):
         params = []
         for key, value in kwargs.items():
             if isinstance(value, Number):
                 val = value
             else:
                 start_value, end_value = value
 
                 if start_value > 0 and end_value > 0:
 
                     # If both values are positive (most likely), interpolate logarithmically
                     start_value = log10(start_value)
                     end_value = log10(end_value)
                     val = 10 ** (start_value + (end_value - start_value) * step / steps)
-                
+
                 else:
-                    
+
                     # If either value is negative, interpolate linearly
                     val = start_value + (end_value - start_value) * step / steps
 
             params.append(f'{key}={val:d}' if isinstance(val, int) else f'{key}={val:.2e}')
 
         lines.append('equilibrium/' + ', '.join(params))
         lines.append('simulate/static')
@@ -69,31 +75,31 @@
             shutil.copy(aux_file, working_dir)
 
         current_files = {f: os.stat(f).st_mtime for f in Path().iterdir()}
 
     if write_cmd:
         # Write the .cmd file. (NOTE: This file is for reference only)
         Adams.write_command_file(file_name=f'{file_prefix}_.cmd', model=sim.parent)
-    
+
     if write_bin:
         write_bin_file(filename=f'{file_prefix}.bin', entity=sim.parent)
-    
+
     # Write the analysis files
     with temp_sim_prefs(solver_preference='write_files_only', file_prefix=file_prefix):
         sim.simulate()
 
     if working_dir is not None:
 
         # Move all new files
         files = [f for f in Path().iterdir() if f not in current_files]
 
         # Move all files that have been modified
         files += [f for f, st_mtime in current_files.items()
                   if os.stat(f).st_mtime != st_mtime]
-        
+
         for file in (f for f in files if f.suffix not in ['.log', '.tmp']):
             if (working_dir / file.name).is_file():
                 (working_dir / file.name).unlink()
             shutil.move(file.name, working_dir)
 
 
 def solve(acf_file: Path, wait=False, use_adams_car=False) -> subprocess.Popen:
@@ -143,41 +149,45 @@
 
 
 def submit(sim: Simulation,
            file_prefix: str,
            use_adams_car=False,
            wait=False,
            write_cmd=False,
-           write_bin=False):
+           write_bin=False,
+           just_write_files=False):
     """Run a simulation externally and import results on completion.
-    
+
     Parameters
     ----------
     sim : Simulation
         The simulation to submit
     file_prefix : str
         The prefix for the simulation files
     use_adams_car : bool, optional
         Whether to use Adams/Car to solve the simulation, by default False
     wait : bool, optional
         Whether to wait for the simulation to complete, by default False
     write_cmd : bool, optional
         Whether to write a .cmd file of the current model (for reference only), by default False
     write_bin : bool, optional
         Whether to write a .bin file of the current model (for reference only), by default False
-        
+
     Returns
     -------
     subprocess.Popen
         The process running the Adams Solver
     """
     acf_file = Path.cwd() / f'{file_prefix}.acf'
 
     write_simulation_files(sim, file_prefix, write_cmd=write_cmd, write_bin=write_bin)
-    proc = solve(acf_file, wait=wait, use_adams_car=use_adams_car)
+    if not just_write_files:
+        proc = solve(acf_file, wait=wait, use_adams_car=use_adams_car)
+    else:
+        proc = None
 
     return proc
 
 
 @contextmanager
 def temp_sim_prefs(**kwargs):
     """Context manager to temporarily change simulation preferences.
@@ -192,15 +202,15 @@
     Examples
     --------
     To temporarily change the solver preference to external:
     ```python
     with temporary_sim_preferences(solver_preference='external'):
         sim.simulate()
     ```
-    
+
     To temporarily write files and set the file prefix
     ```python
     with temporary_sim_preferences(file_prefix='my_sim', save_files=True):
         sim.simulate()
     ```
     """
     current_settings = {}
@@ -214,30 +224,33 @@
         else:
             current_settings[key] = Adams.evaluate_exp(f'.sim_preferences.{key}')
 
         # Convert bools to yes/no
         if isinstance(value, bool):
             value = 'yes' if value else 'no'
 
-        Adams.execute_cmd(f'simulation set {key} = {value}')
+        cmd = f'simulation set {key} = {value}'
+        LOG.debug(f'Running command: {cmd}')
+        Adams.execute_cmd(cmd)
 
     yield
-    
+
     for key, value in current_settings.items():
-        Adams.execute_cmd(f'simulation set {key} = {value}')
+        cmd = f'simulation set {key} = {value}'
+        LOG.debug(f'Running command: {cmd}')
+        Adams.execute_cmd(cmd)
+
 
 def solve_internal(sim: Simulation, reset=False):
     """Solve a simulation internally.
-    
+
     Parameters
     ----------
     sim : Simulation
         The simulation to solve
     reset : bool, optional
         Whether to reset the simulation before solving, by default False
     """
     Adams.execute_cmd('simulation single_run scripted '
                       f'model_name={sim.parent.full_name} '
                       f'sim_script_name={sim.full_name} '
                       f'reset={"yes" if reset else "no"}')
-
-
```

### Comparing `aviewpy-1.3.5/aviewpy/ui/alerts.py` & `aviewpy-1.3.6/aviewpy/ui/alerts.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,25 @@
     Adams.execute_cmd('interface message graphic_window_level=quiet')
     try:
         yield
     finally:
         Adams.execute_cmd(f'interface message graphic_window_level={level}')
 
 
+@contextmanager
+def adams_warnings_suppressed():
+
+    level = Adams.evaluate_exp('user_string(".system_defaults.threshold")')
+    Adams.execute_cmd('interface message threshold=error')
+    try:
+        yield
+    finally:
+        Adams.execute_cmd(f'interface message threshold={level}')
+
+
 def alert_box(msg: str, alert_type: str = 'info', exc_type: Exception = None):
     """Adams View alert box
 
     Parameters
     ----------
     msg : str
         Text to display
```

### Comparing `aviewpy-1.3.5/aviewpy/ui/messages.py` & `aviewpy-1.3.6/aviewpy/ui/messages.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.5/aviewpy/utils/dereferencer.py` & `aviewpy-1.3.6/aviewpy/utils/dereferencer.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.5/aviewpy/utils/excepthook.py` & `aviewpy-1.3.6/aviewpy/utils/excepthook.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.5/aviewpy/utils/res_to_csv.py` & `aviewpy-1.3.6/aviewpy/utils/res_to_csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,120 +11,123 @@
 3. Change File Type to 'Adams View Python File (*.py)"
 4. Select res_to_csv.py
 """
 
 import os
 import csv
 from collections import OrderedDict
-import Adams #pylint: disable=import-error
-import PyQt4.QtGui #pylint: disable=import-error
+import Adams  # type: ignore
+import PyQt4.QtGui  # type: ignore
 
 TIME_STRING = 'TIME'
 
+
 def res_to_csv(results_filename=None, output_filename=None):
     """Writes data in a results file selected by the user to a csv file.
-    
+
     Arguments:
         results_filename {str} -- Path to an adams results file
     """
-    
+
     if results_filename is None:
         results_filename = _get_filename_from_dialog('res')
         if not results_filename:
             print('You must select a .res file!')
-    
+
     if output_filename is None:
         output_filename = _get_filename_from_dialog('csv')
         if not output_filename:
             print('You must select a .csv file for output!')
 
     # Run an aview cmd command to load the results file.
     aview_cmd = 'file results read file_name = "{}"'.format(os.path.normpath(results_filename).replace(os.sep, '/'))
     Adams.execute_cmd(aview_cmd)
-    
+
     # Get the name of the analysis loaded by the results file
-    selected_analysis_name = os.path.split(results_filename)[-1].replace('.res','')
+    selected_analysis_name = os.path.split(results_filename)[-1].replace('.res', '')
 
-    # Loop through all analyses in the model    
+    # Loop through all analyses in the model
     data = OrderedDict()
     for mod_name in Adams.Models:
         mod = Adams.Models.get(mod_name)
         for ans_name in mod.Analyses:
             if ans_name not in selected_analysis_name:
                 # If this analysis name doesn't match, break
                 break
-            
+
             # Initialize a flag indicating that the TIME array has not been set
             time_found = False
-                
+
             # For each analysis in the model, get the analysis handle
             ans = mod.Analyses.get(ans_name)
 
             # Filtering out XFORM result sets
             filt_res_names = [res_name for res_name in ans.results if 'XFORM' not in res_name and TIME_STRING not in res_name]
-            
+
             for res_name in filt_res_names:
                 # For each result set, get the result set handle
-                res = ans.results.get(res_name)                    
+                res = ans.results.get(res_name)
                 for comp_name in res.keys():
                     # for each result component in the result set, get the result component handle
                     comp = res.get(comp_name)
 
                     if TIME_STRING in comp_name and not time_found:
                         # If this is the first time component encountered, add TIME to the data dictionary
                         data[TIME_STRING] = comp.values
                         time_found = True
 
                     elif TIME_STRING not in comp_name:
                         # If this is not a TIME component, add item to the data dictionary
                         # Key = (result set name), (result component name)
                         # Value = list of numeric data
                         data['{}.{}'.format(res_name, comp_name)] = comp.values
-        
+
     if TIME_STRING in data:
         # If the data dictionary has a time key, move it to the front
-        data.move_to_end(TIME_STRING, last=False) 
+        data.move_to_end(TIME_STRING, last=False)
 
     if output_filename is None:
         # If the output file is not given, set equal to the results file
         output_filename = results_filename.replace('.res', '.csv')
 
     # Write the data dictionary to a csv
     try:
-        with open(output_filename, "w",newline = '') as outfile:
+        with open(output_filename, "w", newline='') as outfile:
             writer = csv.writer(outfile)
             writer.writerow(data.keys())
             writer.writerows(zip(*data.values()))
     except PermissionError:
         message_box = PyQt4.QtGui.QMessageBox()
         message_box.setTitle('Permission Denied!')
         message_box.setText(f'Permission to access {output_filename} was denied!  Please close any programs that are using it and rerun this script.')
         message_box.setIcon(PyQt4.QtGui.QMessageBox.Warning)
         message_box.setStandardButtons(PyQt4.QtGui.QMessageBox.Ok)
         message_box.exec_()
 
+
 def _get_filename_from_dialog(file_type):
     """Opens a dialog for user to select a file
-    
+
     Arguments:
         file_type {str} -- Type of file ('res' or 'csv')
-    
+
     Returns:
         str -- Filename of file selected by user.
     """
 
-    if file_type is 'res':
+    if file_type == 'res':
         caption = 'Select a results file.'
         filter = 'Adams Results Files (*.res)'
         # Bring up a dialog for the user to select a results file
         filename = PyQt4.QtGui.QFileDialog.getOpenFileName(caption=caption, filter=filter)
 
-    elif file_type is 'csv':
-        caption='Select location to save the csv results file.'
-        filter='CSV Files (*.csv)'
+    elif file_type == 'csv':
+        caption = 'Select location to save the csv results file.'
+        filter = 'CSV Files (*.csv)'
         # Bring up a dialog for the user to select a results file
-        filename = PyQt4.QtGui.QFileDialog.getSaveFileName(caption=caption, filter=filter)       
+        filename = PyQt4.QtGui.QFileDialog.getSaveFileName(caption=caption, filter=filter)
 
     return filename
 
-if __name__ == 'aview_main':
+
+if __name__ in ['aview_main', '__main__']:
     res_to_csv()
```

### Comparing `aviewpy-1.3.5/aviewpy/variables.py` & `aviewpy-1.3.6/aviewpy/variables.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,42 @@
 
-from functools import singledispatch
 from numbers import Number
-from typing import Iterable, List, Union
+from typing import List, Tuple, TypeVar, Union, overload
 
 import Adams  # type: ignore
 from Object import ObjectBase  # type: ignore
-from Object import Object  # type: ignore
-from Analysis import Analysis  # type: ignore
+from Object import ObjectComment  # type: ignore
 from DesignVariable import DesignVariable  # type: ignore
 
-def set_dv(parent, name: str, value, append=False, **kwargs)->Union[DesignVariable, None]:
+
+@overload
+def set_dv(parent: str,
+           name: str,
+           value: Union[Number, str, ObjectBase],
+           append=False,
+           **kwargs) -> None:
+    ...
+
+
+@overload
+def set_dv(parent:  Union[ObjectComment, ObjectBase],
+           name: str,
+           value: Union[Number, str, ObjectBase],
+           append=False,
+           **kwargs) -> DesignVariable:
+    ...
+
+
+def set_dv(parent: Union[str, ObjectComment, ObjectBase],
+           name: str,
+           value,
+           append=False,
+           **kwargs) -> Union[DesignVariable, None]:
     """Sets the value of a design variable. If the design variable does not exist, it is created.
-    
+
     Note
     ----
     Return value is `None` if `parent' is a string.
 
     Parameters
     ----------
     parent : ObjectBase or str
@@ -26,70 +47,76 @@
         Value(s) to set the design variable to
     append : bool, optional
         If True, appends the given value to the existing value of the design variable, by default False
     **kwargs
         Additional keyword arguments to pass to the DesignVariable.create* methods.
     """
     # Make sure the value is a list
-    value = [value] if not isinstance(value, Iterable) or isinstance(value, str) else value
+    value = make_list(value)
+
+    if len(value) == 0:
+        raise ValueError('Value cannot be an empty list!')
 
     if isinstance(parent, str):
         _set_dv_str(parent, name, value, append)
         dv = None
 
-    elif isinstance(parent, Object):
+    elif isinstance(parent, ObjectComment):
         dv = _set_dv_obj(parent, name, value, append, **kwargs)
-    
+
     elif isinstance(parent, ObjectBase):
-        # Must treat `ObjectBase`s that aren't `Object`s (e.g. `Analysis`) different because the 
+        # Must treat `ObjectBase`s that aren't `ObjectComment`s (e.g. `Analysis`) different because the
         # python API doesn't support setting desisgn variables for analyses, but the cmd API does...
         _set_dv_str(parent.full_name, name, value, append)
         dv = None
-        
+
     else:
-        raise TypeError(f'Invalid type for value: {type(value)}')
+        raise TypeError(f'The parent must be an ObjectComment or str, not {type(parent)}')
 
     return dv
 
 
-def _set_dv_obj(parent: Object, name: str, value: List[Union[Number, str, ObjectBase]], append=False, **kwargs):
+def _set_dv_obj(parent: ObjectComment, name: str, value: List[Union[Number, str, ObjectBase]], append=False, **kwargs):
     """Function to handle setting a design variable when the parent is an ObjectBase"""
     if name in parent.DesignVariables:
         # If the design variable already exists
         dv = parent.DesignVariables[name]
 
         if append:
-            value = dv.value + value
+            try:
+                orig_val = dv.value
+            except OSError:
+                orig_val = make_list(Adams.evaluate_exp(f'{dv.full_name}'))
+
+            value = orig_val + value
 
         dv.update(value=value, **kwargs)
 
     else:
         dv = _create_dv(value, parent, name, **kwargs)
 
     return dv
 
 
-def _set_dv_str(parent: str, name: str, value: List[Union[Number, str, ObjectBase]], append=False)->None:
+def _set_dv_str(parent: str, name: str, value: List[Union[Number, str, ObjectBase]], append=False) -> None:
     """Function to handle setting a design variable when the parent is a string"""
     if Adams.evaluate_exp(f'db_exists("{parent}.{name}")') and append:
-        value_ = Adams.evaluate_exp(f'{parent}.{name}')
-        value_ = [value_] if not isinstance(value_, (tuple, list)) else list(value_)
-        value = value_ + value
+        value = make_list(Adams.evaluate_exp(f'{parent}.{name}')) + value
 
     _cmd_set_dv(value, parent, name)
 
 
-def _create_dv(value: list, parent: Object, name: str, **kwargs):
+def _create_dv(value: list, parent: ObjectComment, name: str, **kwargs):
     """Creates a design variable with the given value.
-    
+
     Parameters
     ----------
     value : List of Number, str, or ObjectBase
         Value(s) to set the design variable to
-    parent : Object
+    parent : ObjectComment
         Parent object of the design variable
     name : str
         Name of the design variable
     **kwargs
         Additional keyword arguments to pass to the DesignVariable.create* methods.
     """
     if isinstance(value, list) and all(isinstance(v, str) for v in value):
@@ -107,64 +134,104 @@
         raise TypeError(f'Invalid type for value: {type(value)}')
 
     return dv
 
 
 def _cmd_set_dv(value: list, parent: str, name: str):
     """Sets the value of a design variable. If the design variable does not exist, it is created.
-    
+
     Parameters
     ----------
     value : Number, str, or ObjectBase (or list of any of these)
         Value(s) to set the design variable to
     parent : str
         Parent object of the design variable
     name : str
         Name of the design variable
     """
-    
+
     if isinstance(value, list) and all(isinstance(v, str) for v in value):
         val_text = ', '.join([f'\'{v}\'' for v in value])
         Adams.execute_cmd(f'var set var={parent}.{name} str={val_text}')
 
     elif isinstance(value, list) and all(isinstance(v, Number) for v in value):
         val_text = ', '.join([f'{v}' for v in value])
         Adams.execute_cmd(f'var set var={parent}.{name} real={val_text}')
 
     elif isinstance(value, list) and all(isinstance(v, int) for v in value):
         val_text = ', '.join([f'{v}' for v in value])
         Adams.execute_cmd(f'var set var={parent}.{name} int={val_text}')
 
     elif isinstance(value, list) and all(isinstance(v, ObjectBase) for v in value):
-        val_text = ', '.join([f'{v}' for v in value])
+        val_text = ', '.join([f'{v.full_name}' for v in value])
         Adams.execute_cmd(f'var set var={parent}.{name} obj={val_text}')
 
     else:
         raise TypeError(f'Invalid type for value: {type(value)}')
 
 
-def get_dv(parent: Union[ObjectBase, str], name: str)->List[Union[Number, str, Object]]:
+class NO_DEFAULT:
+    pass
+
+
+def get_dv(parent: Union[ObjectBase, str],
+           name: str,
+           default: List[Union[Number, str, ObjectComment]] = NO_DEFAULT) -> List[Union[Number, str, ObjectComment]]:
     """Returns the value of the design variable `name` from the object `parent`.
 
     Parameters
     ----------
     parent : ObjectBase or str
         Parent object of the design variable
     name : str
         Name of the design variable
 
     Returns
     -------
-    List[Number, str, or Object]
+    List[Number, str, or ObjectComment]
         Value(s) of the design variable
     """
     if isinstance(parent, ObjectBase):
-        parent=parent.full_name
+        parent = parent.full_name
     elif not isinstance(parent, str):
         raise TypeError(f'Invalid type for parent: {type(parent)}')
 
-    value = Adams.evaluate_exp(f'{parent}.{name}')
+    dvs = make_list(Adams.evaluate_exp(f'db_children({parent}, "variable")'))
+
+    if f'{parent}.{name}'.lower() in [n.lower() for n in dvs]:
+        value = Adams.evaluate_exp(f'{parent}.{name}')
+    elif default is NO_DEFAULT:
+        raise ValueError(f'No design variable named "{name}" exists for object "{parent}"')
+    else:
+        value = default
 
     # Make sure the value is a list
-    value = [value] if not isinstance(value, Iterable) or isinstance(value, str) else value
-    
+    value = make_list(value)
+
     return value
+
+
+Input = TypeVar('Input')
+
+
+@overload
+def make_list(value: str) -> List[str]:
+    ...
+
+
+@overload
+def make_list(value: List[Input]) -> List[Input]:
+    ...
+
+
+@overload
+def make_list(value: Tuple[Input]) -> List[Input]:
+    ...
+
+
+@overload
+def make_list(value: Input) -> List[Input]:
+    ...
+
+
+def make_list(value: str) -> List[str]:
+    return list(value) if isinstance(value, (list, tuple)) else [value]
```

### Comparing `aviewpy-1.3.5/aviewpy.egg-info/PKG-INFO` & `aviewpy-1.3.6/aviewpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aviewpy
-Version: 1.3.5
+Version: 1.3.6
 Summary: Python tools for working with in the Adams View python environment
 Home-page: https://github.com/bthornton191/aviewpy
 Author: Ben Thornton
 Author-email: ben.thornton@hexagon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `aviewpy-1.3.5/aviewpy.egg-info/SOURCES.txt` & `aviewpy-1.3.6/aviewpy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,24 @@
 aviewpy.egg-info/requires.txt
 aviewpy.egg-info/top_level.txt
 aviewpy/files/__init__.py
 aviewpy/files/acf.py
 aviewpy/files/adm.py
 aviewpy/files/bin.py
 aviewpy/files/cmd.py
+aviewpy/files/mac.py
+aviewpy/files/msg.py
 aviewpy/files/shell.py
 aviewpy/files/to.py
 aviewpy/ui/__init__.py
 aviewpy/ui/alerts.py
 aviewpy/ui/messages.py
 aviewpy/ui/progressbar.py
+aviewpy/ui/turn_on_all_force_graphics.py
 aviewpy/ui/windows.py
 aviewpy/utils/__init__.py
 aviewpy/utils/dereferencer.py
 aviewpy/utils/excepthook.py
+aviewpy/utils/fbd.py
 aviewpy/utils/res_to_csv.py
 aviewpy/utils/utils.py
 test/test_shell.py
```

### Comparing `aviewpy-1.3.5/setup.py` & `aviewpy-1.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.5/test/test_shell.py` & `aviewpy-1.3.6/test/test_shell.py`

 * *Files identical despite different names*

