# Comparing `tmp/plotly3d-0.4.5.tar.gz` & `tmp/plotly3d-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly3d-0.4.5.tar", last modified: Thu Apr 25 23:10:02 2024, max compression
+gzip compressed data, was "plotly3d-0.4.6.tar", last modified: Thu Apr 25 23:12:28 2024, max compression
```

## Comparing `plotly3d-0.4.5.tar` & `plotly3d-0.4.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 23:10:02.131185 plotly3d-0.4.5/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.4.5/LICENSE
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      328 2024-04-25 23:10:02.130102 plotly3d-0.4.5/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      118 2024-04-25 22:33:15.000000 plotly3d-0.4.5/README.md
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 23:10:02.127119 plotly3d-0.4.5/plotly3d/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.4.5/plotly3d/__init__.py
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)     9165 2024-04-25 23:09:15.000000 plotly3d-0.4.5/plotly3d/plot.py
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 23:10:02.129275 plotly3d-0.4.5/plotly3d.egg-info/
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      328 2024-04-25 23:10:02.127594 plotly3d-0.4.5/plotly3d.egg-info/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-25 23:10:02.127978 plotly3d-0.4.5/plotly3d.egg-info/SOURCES.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-25 23:10:02.128443 plotly3d-0.4.5/plotly3d.egg-info/dependency_links.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-25 23:10:02.128963 plotly3d-0.4.5/plotly3d.egg-info/requires.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-25 23:10:02.129513 plotly3d-0.4.5/plotly3d.egg-info/top_level.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-25 23:10:02.131251 plotly3d-0.4.5/setup.cfg
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      422 2024-04-25 23:09:46.000000 plotly3d-0.4.5/setup.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 23:12:28.849503 plotly3d-0.4.6/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.4.6/LICENSE
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      328 2024-04-25 23:12:28.848376 plotly3d-0.4.6/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      118 2024-04-25 22:33:15.000000 plotly3d-0.4.6/README.md
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 23:12:28.845030 plotly3d-0.4.6/plotly3d/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.4.6/plotly3d/__init__.py
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)     9166 2024-04-25 23:12:03.000000 plotly3d-0.4.6/plotly3d/plot.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 23:12:28.847643 plotly3d-0.4.6/plotly3d.egg-info/
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      328 2024-04-25 23:12:28.845554 plotly3d-0.4.6/plotly3d.egg-info/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-25 23:12:28.845939 plotly3d-0.4.6/plotly3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-25 23:12:28.846280 plotly3d-0.4.6/plotly3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-25 23:12:28.847239 plotly3d-0.4.6/plotly3d.egg-info/requires.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-25 23:12:28.847784 plotly3d-0.4.6/plotly3d.egg-info/top_level.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-25 23:12:28.849569 plotly3d-0.4.6/setup.cfg
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      422 2024-04-25 23:12:10.000000 plotly3d-0.4.6/setup.py
```

### Comparing `plotly3d-0.4.5/LICENSE` & `plotly3d-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `plotly3d-0.4.5/plotly3d/plot.py` & `plotly3d-0.4.6/plotly3d/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     legend = kwargs.get('legend', True)
     colorscale = kwargs.get('colorscale', 'Viridis')
     fig = kwargs.get('fig', go.Figure())
     points = np.asarray(points)
     colors = np.asarray(colors) if colors is not None else None
     ticks = kwargs.get('ticks', True)
     figsize = kwargs.get('figsize', None)
-    white_bkgrnd = kwargs.get('white_bkgrd', False)
+    white_bkgrnd = kwargs.get('white_bkgrnd', False)
 
     if rescale:
         if scaler is None:
             scaler = MinMaxScaler()
             scaler.fit(points)
         points_s = scaler.transform(points)
     else:
```

