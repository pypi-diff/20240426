# Comparing `tmp/plotly3d-0.4.4.tar.gz` & `tmp/plotly3d-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly3d-0.4.4.tar", last modified: Thu Apr 25 22:56:46 2024, max compression
+gzip compressed data, was "plotly3d-0.4.5.tar", last modified: Thu Apr 25 23:10:02 2024, max compression
```

## Comparing `plotly3d-0.4.4.tar` & `plotly3d-0.4.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 22:56:46.763297 plotly3d-0.4.4/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.4.4/LICENSE
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      328 2024-04-25 22:56:46.762846 plotly3d-0.4.4/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      118 2024-04-25 22:33:15.000000 plotly3d-0.4.4/README.md
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 22:56:46.760567 plotly3d-0.4.4/plotly3d/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.4.4/plotly3d/__init__.py
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)     8670 2024-04-25 22:54:47.000000 plotly3d-0.4.4/plotly3d/plot.py
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 22:56:46.762361 plotly3d-0.4.4/plotly3d.egg-info/
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      328 2024-04-25 22:56:46.761035 plotly3d-0.4.4/plotly3d.egg-info/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-25 22:56:46.761484 plotly3d-0.4.4/plotly3d.egg-info/SOURCES.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-25 22:56:46.761819 plotly3d-0.4.4/plotly3d.egg-info/dependency_links.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-25 22:56:46.762176 plotly3d-0.4.4/plotly3d.egg-info/requires.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-25 22:56:46.762503 plotly3d-0.4.4/plotly3d.egg-info/top_level.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-25 22:56:46.764096 plotly3d-0.4.4/setup.cfg
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      422 2024-04-25 22:44:59.000000 plotly3d-0.4.4/setup.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 23:10:02.131185 plotly3d-0.4.5/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.4.5/LICENSE
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      328 2024-04-25 23:10:02.130102 plotly3d-0.4.5/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      118 2024-04-25 22:33:15.000000 plotly3d-0.4.5/README.md
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 23:10:02.127119 plotly3d-0.4.5/plotly3d/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.4.5/plotly3d/__init__.py
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)     9165 2024-04-25 23:09:15.000000 plotly3d-0.4.5/plotly3d/plot.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 23:10:02.129275 plotly3d-0.4.5/plotly3d.egg-info/
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      328 2024-04-25 23:10:02.127594 plotly3d-0.4.5/plotly3d.egg-info/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-25 23:10:02.127978 plotly3d-0.4.5/plotly3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-25 23:10:02.128443 plotly3d-0.4.5/plotly3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-25 23:10:02.128963 plotly3d-0.4.5/plotly3d.egg-info/requires.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-25 23:10:02.129513 plotly3d-0.4.5/plotly3d.egg-info/top_level.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-25 23:10:02.131251 plotly3d-0.4.5/setup.cfg
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      422 2024-04-25 23:09:46.000000 plotly3d-0.4.5/setup.py
```

### Comparing `plotly3d-0.4.4/LICENSE` & `plotly3d-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `plotly3d-0.4.4/plotly3d/plot.py` & `plotly3d-0.4.5/plotly3d/plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     legend = kwargs.get('legend', True)
     colorscale = kwargs.get('colorscale', 'Viridis')
     fig = kwargs.get('fig', go.Figure())
     points = np.asarray(points)
     colors = np.asarray(colors) if colors is not None else None
     ticks = kwargs.get('ticks', True)
     figsize = kwargs.get('figsize', None)
+    white_bkgrnd = kwargs.get('white_bkgrd', False)
 
     if rescale:
         if scaler is None:
             scaler = MinMaxScaler()
             scaler.fit(points)
         points_s = scaler.transform(points)
     else:
@@ -103,14 +104,20 @@
         if is_3d:
             fig.update_zaxes(showgrid=False, zeroline=False, showline=False, showticklabels=False, ticks="")
 
     if figsize is not None:
         assert len(figsize) == 2
         fig.update_layout(width=figsize[0] * 100, height=figsize[1] * 100)  # width and height in pixels
 
+    if white_bkgrnd:
+        fig.update_layout(
+            paper_bgcolor='white',  # Color of the whole background
+            plot_bgcolor='white'        # Color of the plotting area
+        )
+
     if filename is not None:
         fig.write_html(filename)
 
     return fig
 
 # for compatability with previous versions
 plot_3d = scatter
@@ -139,14 +146,15 @@
     ytitle = kwargs.get('ytitle', 'Y')
     ztitle = kwargs.get('ztitle', 'Z')
     scaler = kwargs.get('scaler', None)
     # colors = kwargs.get('colors', None)
     cmap = kwargs.get('cmap', 'tab20')
     ticks = kwargs.get('ticks', True)
     figsize = kwargs.get('figsize', None)
+    white_bkgrnd = kwargs.get('white_bkgrd', False)
 
     if colors is None:
         colors = np.zeros(trajs.shape[1])
     # color_palette = kwargs.get('color_palette', px.colors.qualitative.Plotly)  # Define a color palette
 
     trajs = np.asarray(trajs)
     if rescale and scaler is None:
@@ -203,12 +211,17 @@
         if is_3d:
             fig.update_zaxes(showgrid=False, zeroline=False, showline=False, showticklabels=False, ticks="")
 
     if figsize is not None:
         assert len(figsize) == 2
         fig.update_layout(width=figsize[0] * 100, height=figsize[1] * 100)  # width and height in pixels
 
+    if white_bkgrnd:
+        fig.update_layout(
+            paper_bgcolor='white',  # Color of the whole background
+            plot_bgcolor='white'        # Color of the plotting area
+        )
 
     if filename is not None:
         fig.write_html(filename)
 
     return fig
```

