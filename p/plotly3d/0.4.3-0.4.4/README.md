# Comparing `tmp/plotly3d-0.4.3.tar.gz` & `tmp/plotly3d-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly3d-0.4.3.tar", last modified: Thu Apr 25 22:27:51 2024, max compression
+gzip compressed data, was "plotly3d-0.4.4.tar", last modified: Thu Apr 25 22:56:46 2024, max compression
```

## Comparing `plotly3d-0.4.3.tar` & `plotly3d-0.4.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 22:27:51.419286 plotly3d-0.4.3/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.4.3/LICENSE
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-25 22:27:51.412100 plotly3d-0.4.3/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      100 2024-04-01 03:31:03.000000 plotly3d-0.4.3/README.md
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 22:27:51.408754 plotly3d-0.4.3/plotly3d/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.4.3/plotly3d/__init__.py
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)     8288 2024-04-25 20:23:51.000000 plotly3d-0.4.3/plotly3d/plot.py
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 22:27:51.411455 plotly3d-0.4.3/plotly3d.egg-info/
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-25 22:27:50.000000 plotly3d-0.4.3/plotly3d.egg-info/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-25 22:27:50.000000 plotly3d-0.4.3/plotly3d.egg-info/SOURCES.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-25 22:27:50.000000 plotly3d-0.4.3/plotly3d.egg-info/dependency_links.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-25 22:27:50.000000 plotly3d-0.4.3/plotly3d.egg-info/requires.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-25 22:27:50.000000 plotly3d-0.4.3/plotly3d.egg-info/top_level.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-25 22:27:51.419505 plotly3d-0.4.3/setup.cfg
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      404 2024-04-25 22:27:10.000000 plotly3d-0.4.3/setup.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 22:56:46.763297 plotly3d-0.4.4/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.4.4/LICENSE
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      328 2024-04-25 22:56:46.762846 plotly3d-0.4.4/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      118 2024-04-25 22:33:15.000000 plotly3d-0.4.4/README.md
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 22:56:46.760567 plotly3d-0.4.4/plotly3d/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.4.4/plotly3d/__init__.py
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)     8670 2024-04-25 22:54:47.000000 plotly3d-0.4.4/plotly3d/plot.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 22:56:46.762361 plotly3d-0.4.4/plotly3d.egg-info/
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      328 2024-04-25 22:56:46.761035 plotly3d-0.4.4/plotly3d.egg-info/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-25 22:56:46.761484 plotly3d-0.4.4/plotly3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-25 22:56:46.761819 plotly3d-0.4.4/plotly3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-25 22:56:46.762176 plotly3d-0.4.4/plotly3d.egg-info/requires.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-25 22:56:46.762503 plotly3d-0.4.4/plotly3d.egg-info/top_level.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-25 22:56:46.764096 plotly3d-0.4.4/setup.cfg
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      422 2024-04-25 22:44:59.000000 plotly3d-0.4.4/setup.py
```

### Comparing `plotly3d-0.4.3/LICENSE` & `plotly3d-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `plotly3d-0.4.3/plotly3d/plot.py` & `plotly3d-0.4.4/plotly3d/plot.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         - title (str): Title of the plot.
         - filename (str): If provided, saves the plot to this file.
         - rescale (bool): If True, rescales points using the provided or default scaler.
         - fig (go.Figure): Plotly figure object to which the scatter plot will be added. If None, a new figure is created.
         - xtitle (str), ytitle (str), ztitle (str): Titles for the X, Y, and Z axes.
     """
     is_3d = points.shape[1] == 3
-    plot_func = go.Scatter3d if is_3d else go.Scatter
+    plot_func = go.Scatter3d if is_3d else lambda z, **kwargs: go.Scatter(**kwargs)
     scaler = kwargs.get('scaler', None)
     s = kwargs.get('s', 1)
     alpha = kwargs.get('alpha', 1)
     title = kwargs.get('title', 'Plot')
     filename = kwargs.get('filename', None)
     xtitle = kwargs.get('xtitle', 'X')
     ytitle = kwargs.get('ytitle', 'Y')
@@ -38,14 +38,17 @@
     force_continuous = kwargs.get('force_continuous', False)
     rescale = kwargs.get('rescale', False)
     legend = kwargs.get('legend', True)
     colorscale = kwargs.get('colorscale', 'Viridis')
     fig = kwargs.get('fig', go.Figure())
     points = np.asarray(points)
     colors = np.asarray(colors) if colors is not None else None
+    ticks = kwargs.get('ticks', True)
+    figsize = kwargs.get('figsize', None)
+
     if rescale:
         if scaler is None:
             scaler = MinMaxScaler()
             scaler.fit(points)
         points_s = scaler.transform(points)
     else:
         points_s = points
@@ -61,62 +64,53 @@
     if is_categorical:
         # Step 3: Categorical Colors Plotting Strategy
         # Map categorical color labels to integers
         color_map, categories = pd.factorize(colors, sort=True)
         # Create a trace for each unique color/category
         for i, color in enumerate(categories):
             idx = color_map == i
-            if is_3d:
-                fig.add_trace(plot_func(
-                    x=points_s[idx, 0],
-                    y=points_s[idx, 1],
-                    z=points_s[idx, 2],
-                    mode='markers',
-                    marker=dict(size=s, opacity=alpha, color=i), # Use integer mapping for color
-                    name=str(color)  # Use actual category name for legend
-                ))
-            else:
-                fig.add_trace(plot_func(
-                    x=points_s[idx, 0],
-                    y=points_s[idx, 1],
-                    mode='markers',
-                    marker=dict(size=s, opacity=alpha, color=i), # Use integer mapping for color
-                    name=str(color)  # Use actual category name for legend
-                ))
-    else:
-        # Step 3: Continuous Colors Plotting Strategy
-        if is_3d:
-            fig.add_trace(plot_func(
-                x=points_s[:, 0],
-                y=points_s[:, 1],
-                z=points_s[:, 2],
-                mode='markers',
-                marker=dict(size=s, color=colors, colorscale='Viridis', opacity=alpha, colorbar=dict(title='Color Scale')),
-            ))
-        else:
             fig.add_trace(plot_func(
-                x=points_s[:, 0],
-                y=points_s[:, 1],
+                x=points_s[idx, 0],
+                y=points_s[idx, 1],
+                z=points_s[idx, 2] if is_3d else None,
                 mode='markers',
-                marker=dict(size=s, color=colors, colorscale='Viridis', opacity=alpha, colorbar=dict(title='Color Scale')),
+                marker=dict(size=s, opacity=alpha, color=i), # Use integer mapping for color
+                name=str(color)  # Use actual category name for legend
             ))
+
+    else:
+        # Step 3: Continuous Colors Plotting Strategy
+        fig.add_trace(plot_func(
+            x=points_s[:, 0],
+            y=points_s[:, 1],
+            z=points_s[:, 2] if is_3d else None,
+            mode='markers',
+            marker=dict(size=s, color=colors, colorscale='Viridis', opacity=alpha, colorbar=dict(title='Color Scale')),
+        ))
     
     fig.data[0].marker.colorscale = colorscale
+    scene=dict(xaxis_title=xtitle, yaxis_title=ytitle)
     if is_3d:
-        fig.update_layout(
-            title=title,
-            scene=dict(xaxis_title=xtitle, yaxis_title=ytitle, zaxis_title=ztitle),
-            showlegend=legend
-        )
-    else:
-        fig.update_layout(
-            title=title,
-            xaxis_title=xtitle, yaxis_title=ytitle,
-            showlegend=legend
-        )
+        scene['zaxis_title'] = ztitle
+    fig.update_layout(
+        title=title,
+        scene=scene,
+        showlegend=legend
+    )
+
+    if not ticks:
+        fig.update_xaxes(showgrid=False, zeroline=False, showline=False, showticklabels=False, ticks="")
+        fig.update_yaxes(showgrid=False, zeroline=False, showline=False, showticklabels=False, ticks="")
+        if is_3d:
+            fig.update_zaxes(showgrid=False, zeroline=False, showline=False, showticklabels=False, ticks="")
+
+    if figsize is not None:
+        assert len(figsize) == 2
+        fig.update_layout(width=figsize[0] * 100, height=figsize[1] * 100)  # width and height in pixels
+
     if filename is not None:
         fig.write_html(filename)
 
     return fig
 
 # for compatability with previous versions
 plot_3d = scatter
@@ -143,14 +137,16 @@
     fig = kwargs.get('fig', go.Figure())
     xtitle = kwargs.get('xtitle', 'X')
     ytitle = kwargs.get('ytitle', 'Y')
     ztitle = kwargs.get('ztitle', 'Z')
     scaler = kwargs.get('scaler', None)
     # colors = kwargs.get('colors', None)
     cmap = kwargs.get('cmap', 'tab20')
+    ticks = kwargs.get('ticks', True)
+    figsize = kwargs.get('figsize', None)
 
     if colors is None:
         colors = np.zeros(trajs.shape[1])
     # color_palette = kwargs.get('color_palette', px.colors.qualitative.Plotly)  # Define a color palette
 
     trajs = np.asarray(trajs)
     if rescale and scaler is None:
@@ -197,11 +193,22 @@
 
     fig.update_layout(
         title=title,
         scene=dict(xaxis_title=xtitle, yaxis_title=ytitle, zaxis_title=ztitle) if is_3d else dict(),
         margin=dict(l=0, r=0, b=0, t=30)
     )
 
+    if not ticks:
+        fig.update_xaxes(showgrid=False, zeroline=False, showline=False, showticklabels=False, ticks="")
+        fig.update_yaxes(showgrid=False, zeroline=False, showline=False, showticklabels=False, ticks="")
+        if is_3d:
+            fig.update_zaxes(showgrid=False, zeroline=False, showline=False, showticklabels=False, ticks="")
+
+    if figsize is not None:
+        assert len(figsize) == 2
+        fig.update_layout(width=figsize[0] * 100, height=figsize[1] * 100)  # width and height in pixels
+
+
     if filename is not None:
         fig.write_html(filename)
 
     return fig
```

