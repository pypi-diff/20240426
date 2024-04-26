# Comparing `tmp/thornpy-0.8.3.tar.gz` & `tmp/thornpy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\thornpy-0.8.3.tar", last modified: Mon Dec  7 22:47:11 2020, max compression
+gzip compressed data, was "dist\thornpy-0.9.0.tar", last modified: Thu Jan  7 15:25:43 2021, max compression
```

## Comparing `thornpy-0.8.3.tar` & `thornpy-0.9.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2020-12-07 22:47:11.000000 thornpy-0.8.3/
--rw-rw-rw-   0        0        0     1091 2019-07-01 12:36:33.000000 thornpy-0.8.3/LICENSE
--rw-rw-rw-   0        0        0       34 2019-07-01 12:36:33.000000 thornpy-0.8.3/MANIFEST.in
--rw-rw-rw-   0        0        0      545 2020-12-07 22:47:11.000000 thornpy-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0       72 2019-07-01 12:36:33.000000 thornpy-0.8.3/README.md
--rw-rw-rw-   0        0        0       42 2020-12-07 22:47:11.000000 thornpy-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0      766 2020-12-07 22:46:39.000000 thornpy-0.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2020-12-07 22:47:10.000000 thornpy-0.8.3/test/
--rw-rw-rw-   0        0        0      340 2020-01-31 22:02:46.000000 thornpy-0.8.3/test/test_contact.py
--rw-rw-rw-   0        0        0     1019 2020-12-07 15:25:41.000000 thornpy-0.8.3/test/test_geometry.py
--rw-rw-rw-   0        0        0     1762 2020-10-20 18:08:35.000000 thornpy-0.8.3/test/test_manually_clean_sig.py
--rw-rw-rw-   0        0        0     3174 2019-07-01 12:36:33.000000 thornpy-0.8.3/test/test_numtype.py
--rw-rw-rw-   0        0        0      427 2019-07-01 12:36:33.000000 thornpy-0.8.3/test/test_plotting.py
--rw-rw-rw-   0        0        0     1232 2019-07-01 12:36:33.000000 thornpy-0.8.3/test/test_utilities.py
--rw-rw-rw-   0        0        0     1583 2020-06-05 12:59:10.000000 thornpy-0.8.3/test/test_waterfall.py
-drwxrwxrwx   0        0        0        0 2020-12-07 22:47:11.000000 thornpy-0.8.3/thornpy/
--rw-rw-rw-   0        0        0      188 2020-01-31 21:41:15.000000 thornpy-0.8.3/thornpy/__init__.py
--rw-rw-rw-   0        0        0    20376 2020-12-07 22:46:22.000000 thornpy-0.8.3/thornpy/geometry.py
-drwxrwxrwx   0        0        0        0 2020-12-07 22:47:11.000000 thornpy-0.8.3/thornpy/mechanics/
--rw-rw-rw-   0        0        0       21 2020-01-31 21:42:09.000000 thornpy-0.8.3/thornpy/mechanics/__init__.py
--rw-rw-rw-   0        0        0     1765 2020-01-31 21:58:05.000000 thornpy-0.8.3/thornpy/mechanics/contact.py
--rw-rw-rw-   0        0        0     3127 2019-07-01 12:36:33.000000 thornpy-0.8.3/thornpy/numtype.py
--rw-rw-rw-   0        0        0     6470 2020-01-22 16:06:10.000000 thornpy-0.8.3/thornpy/plotting.py
--rw-rw-rw-   0        0        0    19427 2020-10-20 18:02:56.000000 thornpy-0.8.3/thornpy/signal.py
--rw-rw-rw-   0        0        0      875 2020-06-01 19:42:35.000000 thornpy-0.8.3/thornpy/slideshow.py
--rw-rw-rw-   0        0        0     4813 2020-04-19 16:11:26.000000 thornpy-0.8.3/thornpy/utilities.py
-drwxrwxrwx   0        0        0        0 2020-12-07 22:47:11.000000 thornpy-0.8.3/thornpy.egg-info/
--rw-rw-rw-   0        0        0      545 2020-12-07 22:47:10.000000 thornpy-0.8.3/thornpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      554 2020-12-07 22:47:10.000000 thornpy-0.8.3/thornpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-12-07 22:47:10.000000 thornpy-0.8.3/thornpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2020-12-07 22:47:10.000000 thornpy-0.8.3/thornpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2020-12-07 22:47:10.000000 thornpy-0.8.3/thornpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-01-07 15:25:43.000000 thornpy-0.9.0/
+-rw-rw-rw-   0        0        0     1091 2019-07-01 12:36:33.000000 thornpy-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0       34 2019-07-01 12:36:33.000000 thornpy-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      545 2021-01-07 15:25:43.000000 thornpy-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0       72 2019-07-01 12:36:33.000000 thornpy-0.9.0/README.md
+-rw-rw-rw-   0        0        0       42 2021-01-07 15:25:43.000000 thornpy-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      766 2021-01-07 15:25:38.000000 thornpy-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2021-01-07 15:25:42.000000 thornpy-0.9.0/test/
+-rw-rw-rw-   0        0        0      340 2020-01-31 22:02:46.000000 thornpy-0.9.0/test/test_contact.py
+-rw-rw-rw-   0        0        0     1019 2020-12-07 15:25:41.000000 thornpy-0.9.0/test/test_geometry.py
+-rw-rw-rw-   0        0        0     1762 2020-10-20 18:08:35.000000 thornpy-0.9.0/test/test_manually_clean_sig.py
+-rw-rw-rw-   0        0        0     3174 2019-07-01 12:36:33.000000 thornpy-0.9.0/test/test_numtype.py
+-rw-rw-rw-   0        0        0      427 2019-07-01 12:36:33.000000 thornpy-0.9.0/test/test_plotting.py
+-rw-rw-rw-   0        0        0     1232 2019-07-01 12:36:33.000000 thornpy-0.9.0/test/test_utilities.py
+-rw-rw-rw-   0        0        0     1583 2020-06-05 12:59:10.000000 thornpy-0.9.0/test/test_waterfall.py
+drwxrwxrwx   0        0        0        0 2021-01-07 15:25:42.000000 thornpy-0.9.0/thornpy/
+-rw-rw-rw-   0        0        0      188 2020-01-31 21:41:15.000000 thornpy-0.9.0/thornpy/__init__.py
+-rw-rw-rw-   0        0        0    21326 2020-12-09 21:31:50.000000 thornpy-0.9.0/thornpy/geometry.py
+drwxrwxrwx   0        0        0        0 2021-01-07 15:25:43.000000 thornpy-0.9.0/thornpy/mechanics/
+-rw-rw-rw-   0        0        0       21 2020-01-31 21:42:09.000000 thornpy-0.9.0/thornpy/mechanics/__init__.py
+-rw-rw-rw-   0        0        0     1765 2020-01-31 21:58:05.000000 thornpy-0.9.0/thornpy/mechanics/contact.py
+-rw-rw-rw-   0        0        0     3127 2019-07-01 12:36:33.000000 thornpy-0.9.0/thornpy/numtype.py
+-rw-rw-rw-   0        0        0     6470 2020-01-22 16:06:10.000000 thornpy-0.9.0/thornpy/plotting.py
+-rw-rw-rw-   0        0        0    22337 2021-01-07 15:24:04.000000 thornpy-0.9.0/thornpy/signal.py
+-rw-rw-rw-   0        0        0      875 2020-06-01 19:42:35.000000 thornpy-0.9.0/thornpy/slideshow.py
+-rw-rw-rw-   0        0        0     4813 2020-04-19 16:11:26.000000 thornpy-0.9.0/thornpy/utilities.py
+drwxrwxrwx   0        0        0        0 2021-01-07 15:25:43.000000 thornpy-0.9.0/thornpy.egg-info/
+-rw-rw-rw-   0        0        0      545 2021-01-07 15:25:42.000000 thornpy-0.9.0/thornpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2021-01-07 15:25:42.000000 thornpy-0.9.0/thornpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-01-07 15:25:42.000000 thornpy-0.9.0/thornpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2021-01-07 15:25:42.000000 thornpy-0.9.0/thornpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2021-01-07 15:25:42.000000 thornpy-0.9.0/thornpy.egg-info/top_level.txt
```

### Comparing `thornpy-0.8.3/LICENSE` & `thornpy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thornpy-0.8.3/PKG-INFO` & `thornpy-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thornpy
-Version: 0.8.3
+Version: 0.9.0
 Summary: Miscellaneous Python Tools
 Home-page: https://github.com/bthornton191/thornpy
 Author: Ben Thornton
 Author-email: ben.thornton@mscsoftware.com
 License: UNKNOWN
 Description: # thornpy
```

### Comparing `thornpy-0.8.3/setup.py` & `thornpy-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="thornpy",
-    version="0.8.3",
+    version="0.9.0",
     author="Ben Thornton",
     author_email="ben.thornton@mscsoftware.com",
     description="Miscellaneous Python Tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bthornton191/thornpy",
     packages=setuptools.find_packages(exclude=['test']),
```

### Comparing `thornpy-0.8.3/test/test_geometry.py` & `thornpy-0.9.0/test/test_geometry.py`

 * *Files identical despite different names*

### Comparing `thornpy-0.8.3/test/test_manually_clean_sig.py` & `thornpy-0.9.0/test/test_manually_clean_sig.py`

 * *Files identical despite different names*

### Comparing `thornpy-0.8.3/test/test_numtype.py` & `thornpy-0.9.0/test/test_numtype.py`

 * *Files identical despite different names*

### Comparing `thornpy-0.8.3/test/test_utilities.py` & `thornpy-0.9.0/test/test_utilities.py`

 * *Files identical despite different names*

### Comparing `thornpy-0.8.3/test/test_waterfall.py` & `thornpy-0.9.0/test/test_waterfall.py`

 * *Files identical despite different names*

### Comparing `thornpy-0.8.3/thornpy/geometry.py` & `thornpy-0.9.0/thornpy/geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,14 +156,19 @@
 
 def get_0_to_180(ang):
     if abs(ang) > np.pi:
         ang = 2*np.pi-abs(ang)
     
     return ang
 
+def get_0_to_360(ang):
+    if ang < 0:
+        ang = 2*np.pi + ang
+    return ang
+
 def get_3point_ang(a, b, c):
     ang = math.atan2(c[1]-b[1], c[0]-b[0]) - math.atan2(a[1]-b[1], a[0]-b[0])
 
     if ang < 0:
         ang += 2*np.pi
     
     if ang > np.pi:
@@ -214,23 +219,23 @@
         sols = [tuple([eq.subs([(x_c_sym, x_c), (y_c_sym, y_c), (x_1_sym, x_1), (y_1_sym, y_1), (r_curve_sym, r_curve)]) for eq in sym_sol]) for sym_sol in sym_sols]
 
     else:
         
         eq_circle = sp.Eq((x - x_c)**2 + (y - y_c)**2, r_curve**2)
         eq_perp = sp.Eq((y - y_c)/(x - x_c), -(x - x_1)/(y - y_1))
 
-        init = (float(np.mean([x_0, x_1])), float(np.mean([y_0, y_1])))
+        init = (50, 150)
         sols = sp.nsolve((eq_circle, eq_perp), (x, y), init, verify=False)
         sols = [[sols[row, col] for row in range(sols.rows)] for col in range(sols.cols)]
 
     # Get the best solution  
-    best_sol = _get_best_sol(x_0, y_0, x_1, y_1, x_c, y_c, x_prev, y_prev, r_curve, sols)
+    best_sol = _get_best_sol4(x_0, y_0, x_1, y_1, x_c, y_c, x_prev, y_prev, r_curve, sols)
 
-    x_tan = float(best_sol[0])
-    y_tan = float(best_sol[1])
+    x_tan = float(sp.re(best_sol[0]))
+    y_tan = float(sp.re(best_sol[1]))
     
     # Figure out how many points in the arc and line (scale by length)
     arc_length = r_curve * get_3point_ang((x_0, y_0), (x_c, y_c), (x_tan, y_tan))
     line_length = norm([x_1 - x_tan, y_1 - y_tan])
     line_pts = round(pts/(arc_length/line_length + 1))
     arc_pts = pts - line_pts if line_pts < pts else 1
 
@@ -284,15 +289,15 @@
     """
     angs = []
     for sol in sols:
         
         # Look for NaNs
         if any([math.isnan(v) for v in sol]):
             # If NaNs found, skip this solution
-            angs.append(-np.inf if i_center==1 else np.inf)
+            angs.append(np.inf if i_center==1 else -np.inf)
             continue
 
         # try:
         x_tan = float(sol[0])
         y_tan = float(sol[1])
         # except TypeError:
         #     continue
@@ -300,15 +305,39 @@
         x_arc, y_arc = get_arc_points(x_0, y_0, x_tan, y_tan, x_c, y_c, x_prev, y_prev, 100)
 
         start_ang = abs(get_3point_ang((x_prev, y_prev), (x_0, y_0), (x_arc[1], y_arc[1])))
         end_ang = abs(get_3point_ang((x_arc[-2], y_arc[-2]), (x_tan, y_tan), (x_1, y_1)))
 
         angs.append(min([start_ang, end_ang]))
         
-    return sols[angs.index(max(angs))] if i_center == 1 else sols[angs.index(min(angs))]
+    return sols[angs.index(min(angs))] if i_center == 1 else sols[angs.index(max(angs))]
+
+def _get_best_sol4(x_0, y_0, x_1, y_1, x_c, y_c, x_prev, y_prev, r_curve, sols, i_center=1):
+    """Gets the solution with the the solution with maximum or minimum subtended angle.
+    
+    """
+    arc_lengths = []
+    for sol in sols:
+        
+        # Look for NaNs
+        if any([math.isnan(sp.re(v)) for v in sol]):
+            # If NaNs found, skip this solution
+            arc_lengths.append(np.inf)
+            continue
+
+        x_tan = float(sp.re(sol[0]))
+        y_tan = float(sp.re(sol[1]))
+
+        # arc_length = r_curve * get_3point_ang((x_0, y_0), (x_c, y_c), (x_tan, y_tan))
+        arc_length = r_curve * get_0_to_360(get_angle_two_vecs(x_0-x_c, y_0-y_c, x_tan-x_c, y_tan-y_c))
+        line_length = norm([x_1 - x_tan, y_1 - y_tan])
+
+        arc_lengths.append(arc_length + line_length)
+        
+    return sols[arc_lengths.index(min(arc_lengths))]
 
 def get_line_points(x_0, y_0, x_1, y_1, pts=10):
     return np.linspace(x_0, x_1, pts), np.linspace(y_0, y_1, pts)
 
 def arc_center(x_0, y_0, x_1, y_1, m_0):
     """Returns the x and y coordinates of the center of curvature of an arc given the start and end coordinates, and the slope at the start.
```

### Comparing `thornpy-0.8.3/thornpy/mechanics/contact.py` & `thornpy-0.9.0/thornpy/mechanics/contact.py`

 * *Files identical despite different names*

### Comparing `thornpy-0.8.3/thornpy/numtype.py` & `thornpy-0.9.0/thornpy/numtype.py`

 * *Files identical despite different names*

### Comparing `thornpy-0.8.3/thornpy/plotting.py` & `thornpy-0.9.0/thornpy/plotting.py`

 * *Files identical despite different names*

### Comparing `thornpy-0.8.3/thornpy/signal.py` & `thornpy-0.9.0/thornpy/signal.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from scipy.signal import butter, filtfilt, find_peaks
 from scipy.signal.windows import hann, hamming, blackman, boxcar
 import matplotlib.pyplot as plt
 from matplotlib import cm  
 from matplotlib.colors import Normalize
 from matplotlib.lines import Line2D
 import numpy as np
-
+import pandas as pd
 
 
 def low_pass(sig, time, freq_cutoff, N=5):
     """Applies a Nth order butterworth lowpass filter.
     
     Parameters
     ----------
@@ -28,15 +28,15 @@
     -------
     list
         Filtered signal
     list
         Time signal associated with filtered signal
 
     """
-    freq_samp = 1/(time[1]-time[0])
+    freq_samp = (len(time)-1)/(time[-1]-time[0])
     omega = freq_cutoff/freq_samp*2
     b_coef, a_coef = butter(N, omega)
     return list(filtfilt(b_coef, a_coef, sig)), time
         
 def step_function(index, start, init_val, end, final_val):
     """Approximates the Heaviside step function with a cubic polynomial.
     
@@ -569,7 +569,95 @@
     else:
         plt.draw()
 
     if indices is True:
         return y, i_mod
     else:
         return y
+
+def resample_dataframe(df: pd.DataFrame, resample_time: int, time_column='index', time_unit='s', datetime_column=None) -> pd.DataFrame:
+    """Resamples `df` using sample time `resample_time` in microseconds.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        DataFrame to resample
+    resample_time : int
+        Resample time in microseconds
+    time_column : str, optional
+        Name of time column, by default 'index'
+    time_unit : str, optional
+        Unit of time colujmn, by default 's'
+    datetime_column : str, optional
+        Name of datetime column, by default None
+
+    Returns
+    -------
+    pd.DataFrame
+        Resampled DataFrame
+
+    """
+    def resample(df: pd.DataFrame, datetime_column: str, resample_time:int) -> pd.DataFrame:
+        """Resamples df
+        
+        Parameters
+        ----------
+        df : DataFrame
+            Data Frame to be resampled
+        resample_time : int
+            New sample time in microseconds
+        datetime_column : str
+            Name of DateTime column
+
+        """
+        df.drop_duplicates(subset=datetime_column, inplace=True)
+        
+        # Set the index as the date (preserver current)
+        index_name = df.index.name
+        if index_name is not None:
+            df = df.reset_index()
+        df = df.set_index(datetime_column, drop=True)
+
+        # Resample
+        _df = df.resample(f'{resample_time}U').asfreq()
+
+        # Join with original
+        df = _df.join(df, lsuffix='__', how='outer')
+
+        for column in [c for c in df.columns if c.endswith('__')]:
+            # _tmpdf[column].fillna(_tmpdf[column[:-1]], inplace=True)
+            del df[column]
+
+        # df[datetime_column] = df.index.values
+        
+        df = df.apply(pd.Series.interpolate, args=('time',)).bfill()
+        df = df.resample(f'{resample_time}U').asfreq()        
+
+        df = df.reset_index()
+
+        if index_name is not None:
+            df = df.set_index(index_name, drop=True)
+        
+        return df
+
+    if datetime_column is None and time_column == 'index':
+
+        # If the time column is the index
+        datetime_column = '__datetime'
+        df[datetime_column] = pd.to_datetime(df.index, unit=time_unit) 
+        df = resample(df, datetime_column, resample_time=resample_time)
+        df = df.drop(datetime_column, axis=1)
+
+    elif datetime_column is None:
+
+        # If a time column is passed
+        datetime_column = '__datetime'
+        df[datetime_column] = pd.to_datetime(df[time_column], unit=time_unit)    
+        df = resample(df, datetime_column, resample_time=resample_time)
+        df = df.drop(datetime_column, axis=1)
+
+    else:
+
+        #  If a datetime column is passed
+        df = resample(df, datetime_column, resample_time=resample_time)
+    
+    return df
```

### Comparing `thornpy-0.8.3/thornpy/slideshow.py` & `thornpy-0.9.0/thornpy/slideshow.py`

 * *Files identical despite different names*

### Comparing `thornpy-0.8.3/thornpy/utilities.py` & `thornpy-0.9.0/thornpy/utilities.py`

 * *Files identical despite different names*

### Comparing `thornpy-0.8.3/thornpy.egg-info/PKG-INFO` & `thornpy-0.9.0/thornpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thornpy
-Version: 0.8.3
+Version: 0.9.0
 Summary: Miscellaneous Python Tools
 Home-page: https://github.com/bthornton191/thornpy
 Author: Ben Thornton
 Author-email: ben.thornton@mscsoftware.com
 License: UNKNOWN
 Description: # thornpy
```

### Comparing `thornpy-0.8.3/thornpy.egg-info/SOURCES.txt` & `thornpy-0.9.0/thornpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

