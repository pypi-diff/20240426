# Comparing `tmp/plotly3d-0.4.2.tar.gz` & `tmp/plotly3d-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly3d-0.4.2.tar", last modified: Wed Apr 17 04:03:44 2024, max compression
+gzip compressed data, was "plotly3d-0.4.3.tar", last modified: Thu Apr 25 22:27:51 2024, max compression
```

## Comparing `plotly3d-0.4.2.tar` & `plotly3d-0.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-17 04:03:44.798858 plotly3d-0.4.2/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.4.2/LICENSE
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-17 04:03:44.787278 plotly3d-0.4.2/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      100 2024-04-01 03:31:03.000000 plotly3d-0.4.2/README.md
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-17 04:03:44.733870 plotly3d-0.4.2/plotly3d/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.4.2/plotly3d/__init__.py
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)     8258 2024-04-17 04:00:07.000000 plotly3d-0.4.2/plotly3d/plot.py
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-17 04:03:44.773243 plotly3d-0.4.2/plotly3d.egg-info/
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-17 04:03:42.000000 plotly3d-0.4.2/plotly3d.egg-info/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-17 04:03:42.000000 plotly3d-0.4.2/plotly3d.egg-info/SOURCES.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-17 04:03:42.000000 plotly3d-0.4.2/plotly3d.egg-info/dependency_links.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-17 04:03:42.000000 plotly3d-0.4.2/plotly3d.egg-info/requires.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-17 04:03:42.000000 plotly3d-0.4.2/plotly3d.egg-info/top_level.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-17 04:03:44.804060 plotly3d-0.4.2/setup.cfg
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      404 2024-04-17 04:00:11.000000 plotly3d-0.4.2/setup.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 22:27:51.419286 plotly3d-0.4.3/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.4.3/LICENSE
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-25 22:27:51.412100 plotly3d-0.4.3/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      100 2024-04-01 03:31:03.000000 plotly3d-0.4.3/README.md
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 22:27:51.408754 plotly3d-0.4.3/plotly3d/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.4.3/plotly3d/__init__.py
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)     8288 2024-04-25 20:23:51.000000 plotly3d-0.4.3/plotly3d/plot.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 22:27:51.411455 plotly3d-0.4.3/plotly3d.egg-info/
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-25 22:27:50.000000 plotly3d-0.4.3/plotly3d.egg-info/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-25 22:27:50.000000 plotly3d-0.4.3/plotly3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-25 22:27:50.000000 plotly3d-0.4.3/plotly3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-25 22:27:50.000000 plotly3d-0.4.3/plotly3d.egg-info/requires.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-25 22:27:50.000000 plotly3d-0.4.3/plotly3d.egg-info/top_level.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-25 22:27:51.419505 plotly3d-0.4.3/setup.cfg
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      404 2024-04-25 22:27:10.000000 plotly3d-0.4.3/setup.py
```

### Comparing `plotly3d-0.4.2/LICENSE` & `plotly3d-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plotly3d-0.4.2/plotly3d/plot.py` & `plotly3d-0.4.3/plotly3d/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     - trajs: numpy array of shape (a, b, c), where
       a: time bins, b: trajectory index, c: space dimension (c=3 for 3D).
 
     Returns:
     - Plotly figure containing the trajectories plotted in 3D space.
     """
     is_3d = trajs.shape[2] == 3
-    plot_func = go.Scatter3d if is_3d else go.Scatter
+    plot_func = go.Scatter3d if is_3d else lambda z, **kwargs: go.Scatter(**kwargs)
     s = kwargs.get('s', 1)
     s_end = kwargs.get('s_end', 1)
     title = kwargs.get('title', 'Plot')
     filename = kwargs.get('filename', None)
     rescale = kwargs.get('rescale', False)
     fig = kwargs.get('fig', go.Figure())
     xtitle = kwargs.get('xtitle', 'X')
```

