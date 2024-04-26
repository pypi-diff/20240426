# Comparing `tmp/pyvisigraph-2.0.3.tar.gz` & `tmp/pyvisigraph-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvisigraph-2.0.3.tar", last modified: Wed Apr 24 15:19:20 2024, max compression
+gzip compressed data, was "pyvisigraph-2.0.4.tar", last modified: Fri Apr 26 05:43:47 2024, max compression
```

## Comparing `pyvisigraph-2.0.3.tar` & `pyvisigraph-2.0.4.tar`

### file list

```diff
@@ -1,27 +1,24 @@
-drwxr-xr-x   0 pingou    (1000) pingou    (1000)        0 2024-04-24 15:19:20.009105 pyvisigraph-2.0.3/
--rw-r--r--   0 pingou    (1000) pingou    (1000)     1157 2024-04-23 04:11:42.000000 pyvisigraph-2.0.3/LICENSE.txt
--rw-r--r--   0 pingou    (1000) pingou    (1000)      535 2024-04-24 08:35:23.000000 pyvisigraph-2.0.3/MANIFEST.in
--rw-r--r--   0 pingou    (1000) pingou    (1000)     9100 2024-04-24 15:19:20.009105 pyvisigraph-2.0.3/PKG-INFO
--rw-r--r--   0 pingou    (1000) pingou    (1000)     8629 2024-04-24 15:14:40.000000 pyvisigraph-2.0.3/README.md
-drwxr-xr-x   0 pingou    (1000) pingou    (1000)        0 2024-04-24 15:19:20.005105 pyvisigraph-2.0.3/examples/
--rwxr-xr-x   0 pingou    (1000) pingou    (1000)     1553 2024-04-24 10:51:09.000000 pyvisigraph-2.0.3/examples/1_Build_visigraph_without_opti_and_plot_it.py
--rwxr-xr-x   0 pingou    (1000) pingou    (1000)     1608 2024-04-24 10:51:45.000000 pyvisigraph-2.0.3/examples/2_Build_visigraph_with_opti_and_plot_it.py
--rwxr-xr-x   0 pingou    (1000) pingou    (1000)     1330 2024-04-24 06:38:48.000000 pyvisigraph-2.0.3/examples/3_build_graph_from_full_resolution_shapefiles.py
--rwxr-xr-x   0 pingou    (1000) pingou    (1000)     1404 2024-04-24 06:39:00.000000 pyvisigraph-2.0.3/examples/4_calculate_shortest_distance_on_saved_visigraph_and_plot_it.py
--rwxr-xr-x   0 pingou    (1000) pingou    (1000)     1263 2024-04-24 06:39:07.000000 pyvisigraph-2.0.3/examples/5_build_graph_from_poor_resolution_shapefiles.py
--rwxr-xr-x   0 pingou    (1000) pingou    (1000)     1382 2024-04-24 06:39:15.000000 pyvisigraph-2.0.3/examples/6_calculate_shortest_distance_on_saved_visigraph_and_plot_it.py
-drwxr-xr-x   0 pingou    (1000) pingou    (1000)        0 2024-04-24 15:19:20.005105 pyvisigraph-2.0.3/pyvisigraph/
--rw-r--r--   0 pingou    (1000) pingou    (1000)      143 2024-04-17 09:55:47.000000 pyvisigraph-2.0.3/pyvisigraph/__init__.py
--rw-r--r--   0 pingou    (1000) pingou    (1000)     8140 2024-04-23 14:15:34.000000 pyvisigraph-2.0.3/pyvisigraph/graph.py
--rw-r--r--   0 pingou    (1000) pingou    (1000)    12291 2024-04-24 15:10:34.000000 pyvisigraph-2.0.3/pyvisigraph/shape_work.py
--rw-r--r--   0 pingou    (1000) pingou    (1000)     7368 2024-04-23 14:16:17.000000 pyvisigraph-2.0.3/pyvisigraph/visi_graph.py
--rw-r--r--   0 pingou    (1000) pingou    (1000)    12956 2024-04-23 14:16:09.000000 pyvisigraph-2.0.3/pyvisigraph/visible_vertices.py
-drwxr-xr-x   0 pingou    (1000) pingou    (1000)        0 2024-04-24 15:19:20.009105 pyvisigraph-2.0.3/pyvisigraph.egg-info/
--rw-r--r--   0 pingou    (1000) pingou    (1000)     9100 2024-04-24 15:19:19.000000 pyvisigraph-2.0.3/pyvisigraph.egg-info/PKG-INFO
--rw-r--r--   0 pingou    (1000) pingou    (1000)      741 2024-04-24 15:19:19.000000 pyvisigraph-2.0.3/pyvisigraph.egg-info/SOURCES.txt
--rw-r--r--   0 pingou    (1000) pingou    (1000)        1 2024-04-24 15:19:19.000000 pyvisigraph-2.0.3/pyvisigraph.egg-info/dependency_links.txt
--rw-r--r--   0 pingou    (1000) pingou    (1000)       76 2024-04-24 15:19:19.000000 pyvisigraph-2.0.3/pyvisigraph.egg-info/requires.txt
--rw-r--r--   0 pingou    (1000) pingou    (1000)       12 2024-04-24 15:19:19.000000 pyvisigraph-2.0.3/pyvisigraph.egg-info/top_level.txt
--rw-r--r--   0 pingou    (1000) pingou    (1000)       86 2024-04-24 07:41:00.000000 pyvisigraph-2.0.3/requirements.txt
--rw-r--r--   0 pingou    (1000) pingou    (1000)       79 2024-04-24 15:19:20.009105 pyvisigraph-2.0.3/setup.cfg
--rw-r--r--   0 pingou    (1000) pingou    (1000)      751 2024-04-24 15:16:47.000000 pyvisigraph-2.0.3/setup.py
+drwxr-xr-x   0 pingou    (1000) pingou    (1000)        0 2024-04-26 05:43:47.206962 pyvisigraph-2.0.4/
+-rw-r--r--   0 pingou    (1000) pingou    (1000)     1157 2024-04-23 04:11:42.000000 pyvisigraph-2.0.4/LICENSE.txt
+-rw-r--r--   0 pingou    (1000) pingou    (1000)      535 2024-04-24 08:35:23.000000 pyvisigraph-2.0.4/MANIFEST.in
+-rw-r--r--   0 pingou    (1000) pingou    (1000)    11167 2024-04-26 05:43:47.206962 pyvisigraph-2.0.4/PKG-INFO
+-rw-r--r--   0 pingou    (1000) pingou    (1000)    10696 2024-04-26 05:33:33.000000 pyvisigraph-2.0.4/README.md
+drwxr-xr-x   0 pingou    (1000) pingou    (1000)        0 2024-04-26 05:43:47.206962 pyvisigraph-2.0.4/examples/
+-rwxr-xr-x   0 pingou    (1000) pingou    (1000)     1587 2024-04-26 05:22:05.000000 pyvisigraph-2.0.4/examples/1_Build_visigraph_without_opti_and_plot_it.py
+-rwxr-xr-x   0 pingou    (1000) pingou    (1000)     1642 2024-04-26 05:22:32.000000 pyvisigraph-2.0.4/examples/2_Build_visigraph_with_opti_and_plot_it.py
+-rwxr-xr-x   0 pingou    (1000) pingou    (1000)     1404 2024-04-24 06:39:00.000000 pyvisigraph-2.0.4/examples/6_calculate_shortest_distance_on_saved_visigraph_and_plot_it.py
+drwxr-xr-x   0 pingou    (1000) pingou    (1000)        0 2024-04-26 05:43:47.206962 pyvisigraph-2.0.4/pyvisigraph/
+-rw-r--r--   0 pingou    (1000) pingou    (1000)      143 2024-04-17 09:55:47.000000 pyvisigraph-2.0.4/pyvisigraph/__init__.py
+-rw-r--r--   0 pingou    (1000) pingou    (1000)     8140 2024-04-23 14:15:34.000000 pyvisigraph-2.0.4/pyvisigraph/graph.py
+-rw-r--r--   0 pingou    (1000) pingou    (1000)    12291 2024-04-24 15:10:34.000000 pyvisigraph-2.0.4/pyvisigraph/shape_work.py
+-rw-r--r--   0 pingou    (1000) pingou    (1000)     7583 2024-04-26 05:20:33.000000 pyvisigraph-2.0.4/pyvisigraph/visi_graph.py
+-rw-r--r--   0 pingou    (1000) pingou    (1000)    12956 2024-04-23 14:16:09.000000 pyvisigraph-2.0.4/pyvisigraph/visible_vertices.py
+drwxr-xr-x   0 pingou    (1000) pingou    (1000)        0 2024-04-26 05:43:47.206962 pyvisigraph-2.0.4/pyvisigraph.egg-info/
+-rw-r--r--   0 pingou    (1000) pingou    (1000)    11167 2024-04-26 05:43:47.000000 pyvisigraph-2.0.4/pyvisigraph.egg-info/PKG-INFO
+-rw-r--r--   0 pingou    (1000) pingou    (1000)      552 2024-04-26 05:43:47.000000 pyvisigraph-2.0.4/pyvisigraph.egg-info/SOURCES.txt
+-rw-r--r--   0 pingou    (1000) pingou    (1000)        1 2024-04-26 05:43:47.000000 pyvisigraph-2.0.4/pyvisigraph.egg-info/dependency_links.txt
+-rw-r--r--   0 pingou    (1000) pingou    (1000)       76 2024-04-26 05:43:47.000000 pyvisigraph-2.0.4/pyvisigraph.egg-info/requires.txt
+-rw-r--r--   0 pingou    (1000) pingou    (1000)       12 2024-04-26 05:43:47.000000 pyvisigraph-2.0.4/pyvisigraph.egg-info/top_level.txt
+-rw-r--r--   0 pingou    (1000) pingou    (1000)       86 2024-04-24 07:41:00.000000 pyvisigraph-2.0.4/requirements.txt
+-rw-r--r--   0 pingou    (1000) pingou    (1000)       79 2024-04-26 05:43:47.206962 pyvisigraph-2.0.4/setup.cfg
+-rw-r--r--   0 pingou    (1000) pingou    (1000)      751 2024-04-26 05:36:20.000000 pyvisigraph-2.0.4/setup.py
```

### Comparing `pyvisigraph-2.0.3/LICENSE.txt` & `pyvisigraph-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyvisigraph-2.0.3/MANIFEST.in` & `pyvisigraph-2.0.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyvisigraph-2.0.3/PKG-INFO` & `pyvisigraph-2.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: pyvisigraph
-Version: 2.0.3
-Summary: Given a set of simple obstacle polygons, build a visibility graph and find the shortest path between two points.
-Home-page: https://github.com/pingou2712/pyvisigraph
-Download-URL: https://github.com/pingou2712/pyvisigraph/tarball/2.0.3
-Author: Vincent Laffargue
-Author-email: vincent.laffargue@gmail.com
-Keywords: visibility,graph,shortest
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Pyvisigraph - Python Visibility Graph
 
 ![MIT License](https://img.shields.io/github/license/pingou2712/pyvisigraph.svg?style=flat)
 ![PyPI](https://img.shields.io/pypi/v/pyvisigraph.svg?style=flat)
 
 Given a set of simple obstacle polygons, build a visibility graph and find
 the shortest path between two points.
@@ -25,15 +13,15 @@
 runs in O(n^2 log n) time. The shortest path is found using Djikstra's
 algorithm.
 
 # Why a New Project?
 
 First and foremost, this project is structurally based on Christian Reksten-Monsen's Pyvisgraph project (https://github.com/TaipanRex/pyvisgraph). Special thanks to him.
 
-Furthermore, in reviewing projects such as pivisgraph and extremitypathfinder, the main issue I encountered was that these programs operate with approximate values, whether it involves calculations like acos, atan, or even divisions. Besides potentially causing bugs, this also takes more time! The vision for this project is different: it allows for choosing the desired precision (number of decimal place), and all efforts to determine the visibility graph are made using exact values. D.T. Lee's algorithm does not require calculating angles but only comparing them! A simple calculation of the orientation of points is necessary.
+Furthermore, in reviewing projects such as pivisgraph and extremitypathfinder, the main issue I encountered was that these programs operate with approximate values, whether it involves calculations like acos, atan, or even divisions. Besides potentially causing bugs, this also takes more time! The vision for this project is different: it allows for choosing the desired precision (number of decimal place), and all efforts to determine the visibility graph are made using exact values. D.T. Lee's algorithm does not require calculating angles but only comparing them! A simple calculation of the orientation of points is necessary. In the same way, we don't really need to know the coordinates of the intersection points but only need to understand their relative positions to each other!
 
 Result: no bugs related to approximate values, and the work is even done much more quickly!!!
 
 Significant modifications have been made compared to Christian Reksten-Monsen's project, which prevents me from proposing commits...
 
 Moreover, this pivisgraph considers Property 1 from this thesis: https://cs.au.dk/~gerth/advising/thesis/anders-strand-holm-vinther_magnus-strand-holm-vinther.pdf, which significantly reduces the time taken and the number of visibility edges. Simply use the 'opti' mode (see example).
 
@@ -68,19 +56,19 @@
 
 Once the visibility graph is built, it can be saved and subsequently loaded.
 This is useful for large graphs where build time is long. `pickle` is used
 for saving and loading.
 
 ```
 g.save('graph.pk1')
-g2 = VisGraph()
+g2 = VisiGraph()
 g2.load('graph.pk1')
 ```
 
-For obstacles with a large number of points, Pyvisgraph can take advantage of
+For obstacles with a large number of points, Pyvisigraph can take advantage of
 processors with multiple cores using the `multiprocessing` module. Simply
 add the number of workers (processes) to the `build` method:
 
 ```
 >>> g.build(polys, precision=7, workers=4)
 ```
 
@@ -114,31 +102,89 @@
 
 Once the visibility graph is built, it can be saved and subsequently loaded.
 This is useful for large graphs where build time is long. `pickle` is used
 for saving and loading.
 
 ```
 g.save('graph.pk1')
-g2 = VisGraph()
+g2 = VisiGraph()
 g2.load('graph.pk1')
 ```
 
-For obstacles with a large number of points, Pyvisgraph can take advantage of
+For obstacles with a large number of points, Pyvisigraph can take advantage of
 processors with multiple cores using the `multiprocessing` module. Simply
 add the number of workers (processes) to the `build` method:
 
 ```
 >>> g.build(polys, precision=7, workers=4, opti=True, cadre=cadre)
 ```
 
 With the 'opti' mode enabled, the visibility graph then contains only 18 edges!
 
+## Use shortest_path of networkx (Dijkstra's algorithm)
+
+![Figure 4](docs/images/ShortestPath.png)
+
+Here is an example of using VisiGraph and networkx to find the shortest path using Euclidean distance and Dijkstra's algorithm:
+
+```
+import pyvisigraph as vg
+import networkx as nx
+import math
+
+#define used distance
+distance = lambda x, y: math.sqrt((x[0] - y[0])**2 + (x[1] - y[1])**2)
+
+polys = [[(1.0, 0.0),(0.0, 1.0),(-1, 0.0),(0, -1.0)],[(2.0, 2.0),(-2,2),(-0.51, 1.9),(-0.4,1.8),(0, 1.2),(0.5, 1.7),(1.5, 0),(0.5,-1.7),(0, -1.2),(-0.5,-1.8),(-0.51,-1.9),(-2,-2),(2, -2.0)]]
+cadre = (-2.0, -2.0,2.0, 2.0)
+g = vg.VisiGraph()
+g.build(polys, precision=7, opti=True, cadre=cadre, weight=distance)
+
+#Update with new point if needed
+g.update([(0.7,-0.5),(-1.5,0)], weight=distance)
+g.update([(-1,1.35)], weight=distance)
+
+#Shortest path
+path = nx.shortest_path(g.visigraph, source=(-1,1.35), target=(0.7,-0.5), weight='weight')
+
+#Plot it!
+g.plotGraphAndOrSave(polys,path)
+```
+
+## Use astar_path of networkx (A* algorithm)
+
+Here is an example of using VisiGraph and networkx to find the shortest path using Euclidean distance and A* algorithm:
+
+```
+import pyvisigraph as vg
+import networkx as nx
+import math
+
+#define used distance
+distance = lambda x, y: math.sqrt((x[0] - y[0])**2 + (x[1] - y[1])**2)
+
+polys = [[(1.0, 0.0),(0.0, 1.0),(-1, 0.0),(0, -1.0)],[(2.0, 2.0),(-2,2),(-0.51, 1.9),(-0.4,1.8),(0, 1.2),(0.5, 1.7),(1.5, 0),(0.5,-1.7),(0, -1.2),(-0.5,-1.8),(-0.51,-1.9),(-2,-2),(2, -2.0)]]
+cadre = (-2.0, -2.0,2.0, 2.0)
+g = vg.VisiGraph()
+g.build(polys, precision=7, opti=True, cadre=cadre, weight=distance)
+
+#Update with new points if needed
+g.update([(0.7,-0.5),(-1.5,0)], weight=distance)
+g.update([(-1,1.35)], weight=distance)
+
+#Shortest path
+path = nx.astar_path(g.visigraph, source=(-1,1.35), target=(0.7,-0.5), heuristic=distance, weight='weight')
+
+#Plot it!
+g.plotGraphAndOrSave(polys,path)
+```
+
 ## Simple usage with shape - shortest path 
 
-![Figure 4](docs/images/shortestPathWorld.png)
+![Figure 5](docs/images/shortestPathWorld.png)
 
 Here is an example of constructing the visibility graph on the world map in crude quality:
 
 ```
 import pyvisigraph as vg
 
 shape = vg.ShapeWork()
@@ -158,27 +204,27 @@
 start_point = (12.568337, 55.676098) # Copenhagen
 end_point = (103.851959, 1.290270) # Singapore
 shape.calculer_shortest_path(start_point,end_point)
 
 shape.plotPathAndOrSave(show=True, filename='shortestPath.png')
 ```
 
-For obstacles with a large number of points, Pyvisgraph can take advantage of
+For obstacles with a large number of points, Pyvisigraph can take advantage of
 processors with multiple cores using the `multiprocessing` module. Simply
 add the number of workers (processes) to the `buildGraph` method:
 
 ```
 shape.buildGraph('gshhg-shp-2.3.7/GSHHS_shp/c/GSHHS_c_L1.shp', precision=7, workers=4)
 ```
 
 
 
 ## Usage with shape, zone and buffer - shortest path
 
-![Figure 5](docs/images/shortestPathOptiAndCadre.png)
+![Figure 6](docs/images/shortestPathOptiAndCadre.png)
 
 Here is an example of constructing the visibility graph on a part of Sardinia in the Mediterranean at full resolution (we use GSHHS_f_L1.shp). To specify the area of interest, we use the zone option in the buildGraph method, which frames a specific geographic area with coordinates (9.35, 40.98, 9.68, 41.22).
 
 Moreover, since a boat rarely passes exactly along the coast, we apply a buffer of approximately 40 meters to the coastal data. This buffer is implemented using the shpBuffer parameter, which effectively expands the coastline outward to ensure safer navigation routes are calculated.
 
 The default projection used by many global applications is EPSG:4326, which covers almost the entire globe. However, for this specific application focusing on Sardinia, we switch to the EPSG:32632 projection. This local UTM projection is better suited for the region as it minimizes distortions and improves accuracy in local scale studies.
 
@@ -202,15 +248,15 @@
 shape.load('graphshape')
 coord_de_depart = (9.522130177978363, 41.0280536333291)
 coord_darrivee = (9.46699448572067, 41.185838636726395)
 shape.calculer_shortest_path(coord_de_depart,coord_darrivee)
 shape.plotPathAndOrSave(show=True, filename='shortestPath.png')
 ```
 
-For obstacles with a large number of points, Pyvisgraph can take advantage of
+For obstacles with a large number of points, Pyvisigraph can take advantage of
 processors with multiple cores using the `multiprocessing` module. Simply
 add the number of workers (processes) to the `buildGraph` method:
 
 ```
 shape.buildGraph('gshhg-shp-2.3.7/GSHHS_shp/f/GSHHS_f_L1.shp', zone=(9.35, 40.98, 9.68, 41.22),shpBuffer=40,crsProj="EPSG:32632", precision=7, workers=4)
 ```
```

### Comparing `pyvisigraph-2.0.3/README.md` & `pyvisigraph-2.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: pyvisigraph
+Version: 2.0.4
+Summary: Given a set of simple obstacle polygons, build a visibility graph and find the shortest path between two points.
+Home-page: https://github.com/pingou2712/pyvisigraph
+Download-URL: https://github.com/pingou2712/pyvisigraph/tarball/2.0.4
+Author: Vincent Laffargue
+Author-email: vincent.laffargue@gmail.com
+Keywords: visibility,graph,shortest
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Pyvisigraph - Python Visibility Graph
 
 ![MIT License](https://img.shields.io/github/license/pingou2712/pyvisigraph.svg?style=flat)
 ![PyPI](https://img.shields.io/pypi/v/pyvisigraph.svg?style=flat)
 
 Given a set of simple obstacle polygons, build a visibility graph and find
 the shortest path between two points.
@@ -13,15 +25,15 @@
 runs in O(n^2 log n) time. The shortest path is found using Djikstra's
 algorithm.
 
 # Why a New Project?
 
 First and foremost, this project is structurally based on Christian Reksten-Monsen's Pyvisgraph project (https://github.com/TaipanRex/pyvisgraph). Special thanks to him.
 
-Furthermore, in reviewing projects such as pivisgraph and extremitypathfinder, the main issue I encountered was that these programs operate with approximate values, whether it involves calculations like acos, atan, or even divisions. Besides potentially causing bugs, this also takes more time! The vision for this project is different: it allows for choosing the desired precision (number of decimal place), and all efforts to determine the visibility graph are made using exact values. D.T. Lee's algorithm does not require calculating angles but only comparing them! A simple calculation of the orientation of points is necessary.
+Furthermore, in reviewing projects such as pivisgraph and extremitypathfinder, the main issue I encountered was that these programs operate with approximate values, whether it involves calculations like acos, atan, or even divisions. Besides potentially causing bugs, this also takes more time! The vision for this project is different: it allows for choosing the desired precision (number of decimal place), and all efforts to determine the visibility graph are made using exact values. D.T. Lee's algorithm does not require calculating angles but only comparing them! A simple calculation of the orientation of points is necessary. In the same way, we don't really need to know the coordinates of the intersection points but only need to understand their relative positions to each other!
 
 Result: no bugs related to approximate values, and the work is even done much more quickly!!!
 
 Significant modifications have been made compared to Christian Reksten-Monsen's project, which prevents me from proposing commits...
 
 Moreover, this pivisgraph considers Property 1 from this thesis: https://cs.au.dk/~gerth/advising/thesis/anders-strand-holm-vinther_magnus-strand-holm-vinther.pdf, which significantly reduces the time taken and the number of visibility edges. Simply use the 'opti' mode (see example).
 
@@ -56,19 +68,19 @@
 
 Once the visibility graph is built, it can be saved and subsequently loaded.
 This is useful for large graphs where build time is long. `pickle` is used
 for saving and loading.
 
 ```
 g.save('graph.pk1')
-g2 = VisGraph()
+g2 = VisiGraph()
 g2.load('graph.pk1')
 ```
 
-For obstacles with a large number of points, Pyvisgraph can take advantage of
+For obstacles with a large number of points, Pyvisigraph can take advantage of
 processors with multiple cores using the `multiprocessing` module. Simply
 add the number of workers (processes) to the `build` method:
 
 ```
 >>> g.build(polys, precision=7, workers=4)
 ```
 
@@ -102,31 +114,89 @@
 
 Once the visibility graph is built, it can be saved and subsequently loaded.
 This is useful for large graphs where build time is long. `pickle` is used
 for saving and loading.
 
 ```
 g.save('graph.pk1')
-g2 = VisGraph()
+g2 = VisiGraph()
 g2.load('graph.pk1')
 ```
 
-For obstacles with a large number of points, Pyvisgraph can take advantage of
+For obstacles with a large number of points, Pyvisigraph can take advantage of
 processors with multiple cores using the `multiprocessing` module. Simply
 add the number of workers (processes) to the `build` method:
 
 ```
 >>> g.build(polys, precision=7, workers=4, opti=True, cadre=cadre)
 ```
 
 With the 'opti' mode enabled, the visibility graph then contains only 18 edges!
 
+## Use shortest_path of networkx (Dijkstra's algorithm)
+
+![Figure 4](docs/images/ShortestPath.png)
+
+Here is an example of using VisiGraph and networkx to find the shortest path using Euclidean distance and Dijkstra's algorithm:
+
+```
+import pyvisigraph as vg
+import networkx as nx
+import math
+
+#define used distance
+distance = lambda x, y: math.sqrt((x[0] - y[0])**2 + (x[1] - y[1])**2)
+
+polys = [[(1.0, 0.0),(0.0, 1.0),(-1, 0.0),(0, -1.0)],[(2.0, 2.0),(-2,2),(-0.51, 1.9),(-0.4,1.8),(0, 1.2),(0.5, 1.7),(1.5, 0),(0.5,-1.7),(0, -1.2),(-0.5,-1.8),(-0.51,-1.9),(-2,-2),(2, -2.0)]]
+cadre = (-2.0, -2.0,2.0, 2.0)
+g = vg.VisiGraph()
+g.build(polys, precision=7, opti=True, cadre=cadre, weight=distance)
+
+#Update with new point if needed
+g.update([(0.7,-0.5),(-1.5,0)], weight=distance)
+g.update([(-1,1.35)], weight=distance)
+
+#Shortest path
+path = nx.shortest_path(g.visigraph, source=(-1,1.35), target=(0.7,-0.5), weight='weight')
+
+#Plot it!
+g.plotGraphAndOrSave(polys,path)
+```
+
+## Use astar_path of networkx (A* algorithm)
+
+Here is an example of using VisiGraph and networkx to find the shortest path using Euclidean distance and A* algorithm:
+
+```
+import pyvisigraph as vg
+import networkx as nx
+import math
+
+#define used distance
+distance = lambda x, y: math.sqrt((x[0] - y[0])**2 + (x[1] - y[1])**2)
+
+polys = [[(1.0, 0.0),(0.0, 1.0),(-1, 0.0),(0, -1.0)],[(2.0, 2.0),(-2,2),(-0.51, 1.9),(-0.4,1.8),(0, 1.2),(0.5, 1.7),(1.5, 0),(0.5,-1.7),(0, -1.2),(-0.5,-1.8),(-0.51,-1.9),(-2,-2),(2, -2.0)]]
+cadre = (-2.0, -2.0,2.0, 2.0)
+g = vg.VisiGraph()
+g.build(polys, precision=7, opti=True, cadre=cadre, weight=distance)
+
+#Update with new points if needed
+g.update([(0.7,-0.5),(-1.5,0)], weight=distance)
+g.update([(-1,1.35)], weight=distance)
+
+#Shortest path
+path = nx.astar_path(g.visigraph, source=(-1,1.35), target=(0.7,-0.5), heuristic=distance, weight='weight')
+
+#Plot it!
+g.plotGraphAndOrSave(polys,path)
+```
+
 ## Simple usage with shape - shortest path 
 
-![Figure 4](docs/images/shortestPathWorld.png)
+![Figure 5](docs/images/shortestPathWorld.png)
 
 Here is an example of constructing the visibility graph on the world map in crude quality:
 
 ```
 import pyvisigraph as vg
 
 shape = vg.ShapeWork()
@@ -146,27 +216,27 @@
 start_point = (12.568337, 55.676098) # Copenhagen
 end_point = (103.851959, 1.290270) # Singapore
 shape.calculer_shortest_path(start_point,end_point)
 
 shape.plotPathAndOrSave(show=True, filename='shortestPath.png')
 ```
 
-For obstacles with a large number of points, Pyvisgraph can take advantage of
+For obstacles with a large number of points, Pyvisigraph can take advantage of
 processors with multiple cores using the `multiprocessing` module. Simply
 add the number of workers (processes) to the `buildGraph` method:
 
 ```
 shape.buildGraph('gshhg-shp-2.3.7/GSHHS_shp/c/GSHHS_c_L1.shp', precision=7, workers=4)
 ```
 
 
 
 ## Usage with shape, zone and buffer - shortest path
 
-![Figure 5](docs/images/shortestPathOptiAndCadre.png)
+![Figure 6](docs/images/shortestPathOptiAndCadre.png)
 
 Here is an example of constructing the visibility graph on a part of Sardinia in the Mediterranean at full resolution (we use GSHHS_f_L1.shp). To specify the area of interest, we use the zone option in the buildGraph method, which frames a specific geographic area with coordinates (9.35, 40.98, 9.68, 41.22).
 
 Moreover, since a boat rarely passes exactly along the coast, we apply a buffer of approximately 40 meters to the coastal data. This buffer is implemented using the shpBuffer parameter, which effectively expands the coastline outward to ensure safer navigation routes are calculated.
 
 The default projection used by many global applications is EPSG:4326, which covers almost the entire globe. However, for this specific application focusing on Sardinia, we switch to the EPSG:32632 projection. This local UTM projection is better suited for the region as it minimizes distortions and improves accuracy in local scale studies.
 
@@ -190,15 +260,15 @@
 shape.load('graphshape')
 coord_de_depart = (9.522130177978363, 41.0280536333291)
 coord_darrivee = (9.46699448572067, 41.185838636726395)
 shape.calculer_shortest_path(coord_de_depart,coord_darrivee)
 shape.plotPathAndOrSave(show=True, filename='shortestPath.png')
 ```
 
-For obstacles with a large number of points, Pyvisgraph can take advantage of
+For obstacles with a large number of points, Pyvisigraph can take advantage of
 processors with multiple cores using the `multiprocessing` module. Simply
 add the number of workers (processes) to the `buildGraph` method:
 
 ```
 shape.buildGraph('gshhg-shp-2.3.7/GSHHS_shp/f/GSHHS_f_L1.shp', zone=(9.35, 40.98, 9.68, 41.22),shpBuffer=40,crsProj="EPSG:32632", precision=7, workers=4)
 ```
```

### Comparing `pyvisigraph-2.0.3/examples/1_Build_visigraph_without_opti_and_plot_it.py` & `pyvisigraph-2.0.4/examples/1_Build_visigraph_without_opti_and_plot_it.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,13 +23,14 @@
 """
 import pyvisigraph as vg
 
 # Votre polygone et construction de graphe
 polys = [[(1.0, 0.0),(0.0, 1.0),(-1, 0.0),(0, -1.0)],[(2.0, 2.0),(-2,2),(-0.51, 1.9),(-0.4,1.8),(0, 1.2),(0.5, 1.7),(1.5, 0),(0.5,-1.7),(0, -1.2),(-0.5,-1.8),(-0.51,-1.9),(-2,-2),(2, -2.0)]]
 g = vg.VisiGraph()
 g.build(polys, precision=7)
+#Update with new points if needed
 g.update([(0.7,-0.5),(-1.5,0)])
 g.update([(-1,1.35)])
 
 print('Number of visibility edge : ' + str(len(g.visigraph.edges())))
 
 g.plotGraphAndOrSave(polys)
```

### Comparing `pyvisigraph-2.0.3/examples/2_Build_visigraph_with_opti_and_plot_it.py` & `pyvisigraph-2.0.4/examples/2_Build_visigraph_with_opti_and_plot_it.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,13 +25,14 @@
 
 # Votre polygone et construction de graphe
 polys = [[(1.0, 0.0),(0.0, 1.0),(-1, 0.0),(0, -1.0)],[(2.0, 2.0),(-2,2),(-0.51, 1.9),(-0.4,1.8),(0, 1.2),(0.5, 1.7),(1.5, 0),(0.5,-1.7),(0, -1.2),(-0.5,-1.8),(-0.51,-1.9),(-2,-2),(2, -2.0)]]
 cadre = (-2.0, -2.0,2.0, 2.0)
 g = vg.VisiGraph()
 g.build(polys, precision=7, opti=True, cadre=cadre)
 
+#Update with new points if needed
 g.update([(0.7,-0.5),(-1.5,0)])
 g.update([(-1,1.35)])
 
 print('Number of visibility edge : ' + str(len(g.visigraph.edges())))
 
 g.plotGraphAndOrSave(polys)
```

### Comparing `pyvisigraph-2.0.3/examples/3_build_graph_from_full_resolution_shapefiles.py` & `pyvisigraph-2.0.4/examples/6_calculate_shortest_distance_on_saved_visigraph_and_plot_it.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,11 +20,13 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 import pyvisigraph as vg
 
 shape = vg.ShapeWork()
-shape.buildGraph('gshhg-shp-2.3.7/GSHHS_shp/f/GSHHS_f_L1.shp', zone=(9.35, 40.98, 9.68, 41.22),shpBuffer=40,crsProj="EPSG:32632", precision = 7)
-shape.plotGraph()
-shape.save('graphshape')
+shape.load('graphshape')
+coord_de_depart = (9.522130177978363, 41.0280536333291)
+coord_darrivee = (9.46699448572067, 41.185838636726395)
+shape.calculer_shortest_path(coord_de_depart,coord_darrivee)
+shape.plotPathAndOrSave(show=True, filename='shortestPath.png')
```

### Comparing `pyvisigraph-2.0.3/pyvisigraph/graph.py` & `pyvisigraph-2.0.4/pyvisigraph/graph.py`

 * *Files identical despite different names*

### Comparing `pyvisigraph-2.0.3/pyvisigraph/shape_work.py` & `pyvisigraph-2.0.4/pyvisigraph/shape_work.py`

 * *Files identical despite different names*

### Comparing `pyvisigraph-2.0.3/pyvisigraph/visi_graph.py` & `pyvisigraph-2.0.4/pyvisigraph/visi_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,31 +128,34 @@
                 self.graph.maxX = max(self.graph.maxX,point_.x)
         for p in Newpoint:
             for v in visible_vertices(p, self.graph, scan='full', opti = self.opti):
                 point1=(p.x/(2*10**self.precision), p.y/(2*10**self.precision))
                 point2=(v.x/(2*10**self.precision), v.y/(2*10**self.precision))
                 addGraph(point1,point2)
     
-    def plotGraphAndOrSave(self,polys=None, filename=None, show=True):
+    def plotGraphAndOrSave(self,polys=None, path=None, filename=None, show=True):
         fig, ax = plt.subplots()
         if polys:
             ## Visualiser les polygones
             for poly in polys:
                 polygon = patches.Polygon(poly, closed=True, fill=None, edgecolor='black')
                 ax.add_patch(polygon)
         ## Visualiser le graph de visibilite
         pos = {node: node for node in self.visigraph.nodes()}
         nx.draw_networkx_edges(self.visigraph, pos, edge_color='red', style='dashed', alpha=1, ax=ax)
+        if path:
+            path_edges = list(zip(path, path[1:]))
+            nx.draw_networkx_edges(self.visigraph, pos, edgelist=path_edges, edge_color='blue', width=2, ax=ax)
         # Enregistrer l'image
         if filename:
             fig.savefig(filename, dpi=300, bbox_inches='tight', pad_inches=0)
         # Montrer la figure
         if show:
             plt.show()
-
+        return fig,ax
 
 def _visi_graph_wrapper(args):
     try:
         return _visi_graph(*args)
     except KeyboardInterrupt:
         pass
```

### Comparing `pyvisigraph-2.0.3/pyvisigraph/visible_vertices.py` & `pyvisigraph-2.0.4/pyvisigraph/visible_vertices.py`

 * *Files identical despite different names*

### Comparing `pyvisigraph-2.0.3/pyvisigraph.egg-info/PKG-INFO` & `pyvisigraph-2.0.4/pyvisigraph.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyvisigraph
-Version: 2.0.3
+Version: 2.0.4
 Summary: Given a set of simple obstacle polygons, build a visibility graph and find the shortest path between two points.
 Home-page: https://github.com/pingou2712/pyvisigraph
-Download-URL: https://github.com/pingou2712/pyvisigraph/tarball/2.0.3
+Download-URL: https://github.com/pingou2712/pyvisigraph/tarball/2.0.4
 Author: Vincent Laffargue
 Author-email: vincent.laffargue@gmail.com
 Keywords: visibility,graph,shortest
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Pyvisigraph - Python Visibility Graph
@@ -25,15 +25,15 @@
 runs in O(n^2 log n) time. The shortest path is found using Djikstra's
 algorithm.
 
 # Why a New Project?
 
 First and foremost, this project is structurally based on Christian Reksten-Monsen's Pyvisgraph project (https://github.com/TaipanRex/pyvisgraph). Special thanks to him.
 
-Furthermore, in reviewing projects such as pivisgraph and extremitypathfinder, the main issue I encountered was that these programs operate with approximate values, whether it involves calculations like acos, atan, or even divisions. Besides potentially causing bugs, this also takes more time! The vision for this project is different: it allows for choosing the desired precision (number of decimal place), and all efforts to determine the visibility graph are made using exact values. D.T. Lee's algorithm does not require calculating angles but only comparing them! A simple calculation of the orientation of points is necessary.
+Furthermore, in reviewing projects such as pivisgraph and extremitypathfinder, the main issue I encountered was that these programs operate with approximate values, whether it involves calculations like acos, atan, or even divisions. Besides potentially causing bugs, this also takes more time! The vision for this project is different: it allows for choosing the desired precision (number of decimal place), and all efforts to determine the visibility graph are made using exact values. D.T. Lee's algorithm does not require calculating angles but only comparing them! A simple calculation of the orientation of points is necessary. In the same way, we don't really need to know the coordinates of the intersection points but only need to understand their relative positions to each other!
 
 Result: no bugs related to approximate values, and the work is even done much more quickly!!!
 
 Significant modifications have been made compared to Christian Reksten-Monsen's project, which prevents me from proposing commits...
 
 Moreover, this pivisgraph considers Property 1 from this thesis: https://cs.au.dk/~gerth/advising/thesis/anders-strand-holm-vinther_magnus-strand-holm-vinther.pdf, which significantly reduces the time taken and the number of visibility edges. Simply use the 'opti' mode (see example).
 
@@ -68,19 +68,19 @@
 
 Once the visibility graph is built, it can be saved and subsequently loaded.
 This is useful for large graphs where build time is long. `pickle` is used
 for saving and loading.
 
 ```
 g.save('graph.pk1')
-g2 = VisGraph()
+g2 = VisiGraph()
 g2.load('graph.pk1')
 ```
 
-For obstacles with a large number of points, Pyvisgraph can take advantage of
+For obstacles with a large number of points, Pyvisigraph can take advantage of
 processors with multiple cores using the `multiprocessing` module. Simply
 add the number of workers (processes) to the `build` method:
 
 ```
 >>> g.build(polys, precision=7, workers=4)
 ```
 
@@ -114,31 +114,89 @@
 
 Once the visibility graph is built, it can be saved and subsequently loaded.
 This is useful for large graphs where build time is long. `pickle` is used
 for saving and loading.
 
 ```
 g.save('graph.pk1')
-g2 = VisGraph()
+g2 = VisiGraph()
 g2.load('graph.pk1')
 ```
 
-For obstacles with a large number of points, Pyvisgraph can take advantage of
+For obstacles with a large number of points, Pyvisigraph can take advantage of
 processors with multiple cores using the `multiprocessing` module. Simply
 add the number of workers (processes) to the `build` method:
 
 ```
 >>> g.build(polys, precision=7, workers=4, opti=True, cadre=cadre)
 ```
 
 With the 'opti' mode enabled, the visibility graph then contains only 18 edges!
 
+## Use shortest_path of networkx (Dijkstra's algorithm)
+
+![Figure 4](docs/images/ShortestPath.png)
+
+Here is an example of using VisiGraph and networkx to find the shortest path using Euclidean distance and Dijkstra's algorithm:
+
+```
+import pyvisigraph as vg
+import networkx as nx
+import math
+
+#define used distance
+distance = lambda x, y: math.sqrt((x[0] - y[0])**2 + (x[1] - y[1])**2)
+
+polys = [[(1.0, 0.0),(0.0, 1.0),(-1, 0.0),(0, -1.0)],[(2.0, 2.0),(-2,2),(-0.51, 1.9),(-0.4,1.8),(0, 1.2),(0.5, 1.7),(1.5, 0),(0.5,-1.7),(0, -1.2),(-0.5,-1.8),(-0.51,-1.9),(-2,-2),(2, -2.0)]]
+cadre = (-2.0, -2.0,2.0, 2.0)
+g = vg.VisiGraph()
+g.build(polys, precision=7, opti=True, cadre=cadre, weight=distance)
+
+#Update with new point if needed
+g.update([(0.7,-0.5),(-1.5,0)], weight=distance)
+g.update([(-1,1.35)], weight=distance)
+
+#Shortest path
+path = nx.shortest_path(g.visigraph, source=(-1,1.35), target=(0.7,-0.5), weight='weight')
+
+#Plot it!
+g.plotGraphAndOrSave(polys,path)
+```
+
+## Use astar_path of networkx (A* algorithm)
+
+Here is an example of using VisiGraph and networkx to find the shortest path using Euclidean distance and A* algorithm:
+
+```
+import pyvisigraph as vg
+import networkx as nx
+import math
+
+#define used distance
+distance = lambda x, y: math.sqrt((x[0] - y[0])**2 + (x[1] - y[1])**2)
+
+polys = [[(1.0, 0.0),(0.0, 1.0),(-1, 0.0),(0, -1.0)],[(2.0, 2.0),(-2,2),(-0.51, 1.9),(-0.4,1.8),(0, 1.2),(0.5, 1.7),(1.5, 0),(0.5,-1.7),(0, -1.2),(-0.5,-1.8),(-0.51,-1.9),(-2,-2),(2, -2.0)]]
+cadre = (-2.0, -2.0,2.0, 2.0)
+g = vg.VisiGraph()
+g.build(polys, precision=7, opti=True, cadre=cadre, weight=distance)
+
+#Update with new points if needed
+g.update([(0.7,-0.5),(-1.5,0)], weight=distance)
+g.update([(-1,1.35)], weight=distance)
+
+#Shortest path
+path = nx.astar_path(g.visigraph, source=(-1,1.35), target=(0.7,-0.5), heuristic=distance, weight='weight')
+
+#Plot it!
+g.plotGraphAndOrSave(polys,path)
+```
+
 ## Simple usage with shape - shortest path 
 
-![Figure 4](docs/images/shortestPathWorld.png)
+![Figure 5](docs/images/shortestPathWorld.png)
 
 Here is an example of constructing the visibility graph on the world map in crude quality:
 
 ```
 import pyvisigraph as vg
 
 shape = vg.ShapeWork()
@@ -158,27 +216,27 @@
 start_point = (12.568337, 55.676098) # Copenhagen
 end_point = (103.851959, 1.290270) # Singapore
 shape.calculer_shortest_path(start_point,end_point)
 
 shape.plotPathAndOrSave(show=True, filename='shortestPath.png')
 ```
 
-For obstacles with a large number of points, Pyvisgraph can take advantage of
+For obstacles with a large number of points, Pyvisigraph can take advantage of
 processors with multiple cores using the `multiprocessing` module. Simply
 add the number of workers (processes) to the `buildGraph` method:
 
 ```
 shape.buildGraph('gshhg-shp-2.3.7/GSHHS_shp/c/GSHHS_c_L1.shp', precision=7, workers=4)
 ```
 
 
 
 ## Usage with shape, zone and buffer - shortest path
 
-![Figure 5](docs/images/shortestPathOptiAndCadre.png)
+![Figure 6](docs/images/shortestPathOptiAndCadre.png)
 
 Here is an example of constructing the visibility graph on a part of Sardinia in the Mediterranean at full resolution (we use GSHHS_f_L1.shp). To specify the area of interest, we use the zone option in the buildGraph method, which frames a specific geographic area with coordinates (9.35, 40.98, 9.68, 41.22).
 
 Moreover, since a boat rarely passes exactly along the coast, we apply a buffer of approximately 40 meters to the coastal data. This buffer is implemented using the shpBuffer parameter, which effectively expands the coastline outward to ensure safer navigation routes are calculated.
 
 The default projection used by many global applications is EPSG:4326, which covers almost the entire globe. However, for this specific application focusing on Sardinia, we switch to the EPSG:32632 projection. This local UTM projection is better suited for the region as it minimizes distortions and improves accuracy in local scale studies.
 
@@ -202,15 +260,15 @@
 shape.load('graphshape')
 coord_de_depart = (9.522130177978363, 41.0280536333291)
 coord_darrivee = (9.46699448572067, 41.185838636726395)
 shape.calculer_shortest_path(coord_de_depart,coord_darrivee)
 shape.plotPathAndOrSave(show=True, filename='shortestPath.png')
 ```
 
-For obstacles with a large number of points, Pyvisgraph can take advantage of
+For obstacles with a large number of points, Pyvisigraph can take advantage of
 processors with multiple cores using the `multiprocessing` module. Simply
 add the number of workers (processes) to the `buildGraph` method:
 
 ```
 shape.buildGraph('gshhg-shp-2.3.7/GSHHS_shp/f/GSHHS_f_L1.shp', zone=(9.35, 40.98, 9.68, 41.22),shpBuffer=40,crsProj="EPSG:32632", precision=7, workers=4)
 ```
```

### Comparing `pyvisigraph-2.0.3/setup.py` & `pyvisigraph-2.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 with open('requirements.txt', 'r') as fr:
   required = fr.read().splitlines()
   
 setup(
   name = 'pyvisigraph',
   packages = ['pyvisigraph'],
-  version = '2.0.3',
+  version = '2.0.4',
   description = 'Given a set of simple obstacle polygons, build a visibility graph and find the shortest path between two points.',
   long_description=open("README.md").read(),
   long_description_content_type="text/markdown",
   author = 'Vincent Laffargue',
   author_email = 'vincent.laffargue@gmail.com',
   url = 'https://github.com/pingou2712/pyvisigraph',
-  download_url = 'https://github.com/pingou2712/pyvisigraph/tarball/2.0.3',
+  download_url = 'https://github.com/pingou2712/pyvisigraph/tarball/2.0.4',
   install_requires = required,
   keywords = ['visibility', 'graph', 'shortest'],
   classifiers = [],
 )
```

