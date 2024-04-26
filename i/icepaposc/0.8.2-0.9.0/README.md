# Comparing `tmp/icepaposc-0.8.2.tar.gz` & `tmp/icepaposc-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/icepaposc-0.8.2.tar", last modified: Fri Dec  3 05:59:20 2021, max compression
+gzip compressed data, was "dist/icepaposc-0.9.0.tar", last modified: Thu Jul  7 07:01:12 2022, max compression
```

## Comparing `icepaposc-0.8.2.tar` & `icepaposc-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2021-12-03 05:59:20.000000 icepaposc-0.8.2/
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     2790 2021-12-03 05:55:33.000000 icepaposc-0.8.2/CHANGELOG.md
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     5493 2018-11-16 13:05:46.000000 icepaposc-0.8.2/CONTRIBUTING.md
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    35149 2018-11-16 13:05:46.000000 icepaposc-0.8.2/LICENSE
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       29 2021-08-23 13:33:01.000000 icepaposc-0.8.2/MANIFEST.in
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      874 2021-12-03 05:59:20.000000 icepaposc-0.8.2/PKG-INFO
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      442 2018-11-19 09:03:29.000000 icepaposc-0.8.2/README.md
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2021-12-03 05:59:20.000000 icepaposc-0.8.2/icepaposc/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      825 2021-12-03 05:57:31.000000 icepaposc-0.8.2/icepaposc/__init__.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2624 2021-06-03 13:32:57.000000 icepaposc-0.8.2/icepaposc/__main__.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1756 2021-05-06 09:51:01.000000 icepaposc-0.8.2/icepaposc/axis_time.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2474 2020-10-07 09:01:01.000000 icepaposc-0.8.2/icepaposc/channel.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    13176 2021-05-06 09:51:01.000000 icepaposc-0.8.2/icepaposc/collector.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     5710 2021-05-06 09:51:01.000000 icepaposc-0.8.2/icepaposc/curve_item.py
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2021-12-03 05:59:20.000000 icepaposc-0.8.2/icepaposc/custom_widgets/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      771 2021-05-06 09:51:01.000000 icepaposc-0.8.2/icepaposc/custom_widgets/__init__.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1798 2021-12-02 06:16:07.000000 icepaposc-0.8.2/icepaposc/custom_widgets/square_radiobtn.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     8145 2021-05-06 09:51:01.000000 icepaposc-0.8.2/icepaposc/dialog_settings.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     4334 2021-05-06 09:51:01.000000 icepaposc-0.8.2/icepaposc/settings.py
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2021-12-03 05:59:20.000000 icepaposc-0.8.2/icepaposc/ui/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      754 2021-06-03 13:28:30.000000 icepaposc-0.8.2/icepaposc/ui/__init__.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    12137 2021-05-06 09:51:01.000000 icepaposc-0.8.2/icepaposc/ui/dialog_settings.ui
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2021-12-03 05:59:20.000000 icepaposc-0.8.2/icepaposc/ui/icons/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      726 2021-06-03 13:32:39.000000 icepaposc-0.8.2/icepaposc/ui/icons/__init__.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)   117527 2021-06-03 13:28:41.000000 icepaposc-0.8.2/icepaposc/ui/resources_rc.py
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    65974 2021-08-23 13:29:35.000000 icepaposc-0.8.2/icepaposc/ui/window_main.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    34854 2021-08-23 13:29:35.000000 icepaposc-0.8.2/icepaposc/window_main.py
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2021-12-03 05:59:20.000000 icepaposc-0.8.2/icepaposc.egg-info/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      874 2021-12-03 05:59:20.000000 icepaposc-0.8.2/icepaposc.egg-info/PKG-INFO
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      704 2021-12-03 05:59:20.000000 icepaposc-0.8.2/icepaposc.egg-info/SOURCES.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)        1 2021-12-03 05:59:20.000000 icepaposc-0.8.2/icepaposc.egg-info/dependency_links.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       55 2021-12-03 05:59:20.000000 icepaposc-0.8.2/icepaposc.egg-info/entry_points.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       36 2021-12-03 05:59:20.000000 icepaposc-0.8.2/icepaposc.egg-info/requires.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       10 2021-12-03 05:59:20.000000 icepaposc-0.8.2/icepaposc.egg-info/top_level.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       38 2021-12-03 05:59:20.000000 icepaposc-0.8.2/setup.cfg
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1504 2021-12-03 05:57:31.000000 icepaposc-0.8.2/setup.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2022-07-07 07:01:12.000000 icepaposc-0.9.0/
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     4625 2022-07-07 06:59:16.000000 icepaposc-0.9.0/CHANGELOG.md
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     5493 2018-11-16 13:05:46.000000 icepaposc-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    35149 2018-11-16 13:05:46.000000 icepaposc-0.9.0/LICENSE
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       29 2021-08-23 13:33:01.000000 icepaposc-0.9.0/MANIFEST.in
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      874 2022-07-07 07:01:12.000000 icepaposc-0.9.0/PKG-INFO
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      442 2018-11-19 09:03:29.000000 icepaposc-0.9.0/README.md
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2022-07-07 07:01:12.000000 icepaposc-0.9.0/icepaposc/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      825 2022-07-07 06:59:43.000000 icepaposc-0.9.0/icepaposc/__init__.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2931 2022-07-07 06:52:54.000000 icepaposc-0.9.0/icepaposc/__main__.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1756 2021-05-06 09:51:01.000000 icepaposc-0.9.0/icepaposc/axis_time.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2474 2020-10-07 09:01:01.000000 icepaposc-0.9.0/icepaposc/channel.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    13176 2021-05-06 09:51:01.000000 icepaposc-0.9.0/icepaposc/collector.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     8020 2022-07-07 06:52:54.000000 icepaposc-0.9.0/icepaposc/curve_item.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2022-07-07 07:01:12.000000 icepaposc-0.9.0/icepaposc/custom_widgets/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      771 2021-05-06 09:51:01.000000 icepaposc-0.9.0/icepaposc/custom_widgets/__init__.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1798 2021-12-02 06:16:07.000000 icepaposc-0.9.0/icepaposc/custom_widgets/square_radiobtn.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     8145 2021-05-06 09:51:01.000000 icepaposc-0.9.0/icepaposc/dialog_settings.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     4334 2021-05-06 09:51:01.000000 icepaposc-0.9.0/icepaposc/settings.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2022-07-07 07:01:12.000000 icepaposc-0.9.0/icepaposc/ui/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      754 2021-06-03 13:28:30.000000 icepaposc-0.9.0/icepaposc/ui/__init__.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    12137 2021-05-06 09:51:01.000000 icepaposc-0.9.0/icepaposc/ui/dialog_settings.ui
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2022-07-07 07:01:12.000000 icepaposc-0.9.0/icepaposc/ui/icons/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      726 2021-06-03 13:32:39.000000 icepaposc-0.9.0/icepaposc/ui/icons/__init__.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)   117527 2021-06-03 13:28:41.000000 icepaposc-0.9.0/icepaposc/ui/resources_rc.py
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    66222 2022-07-07 06:52:54.000000 icepaposc-0.9.0/icepaposc/ui/window_main.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    57181 2022-07-07 06:52:54.000000 icepaposc-0.9.0/icepaposc/window_main.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2022-07-07 07:01:12.000000 icepaposc-0.9.0/icepaposc.egg-info/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      874 2022-07-07 07:01:12.000000 icepaposc-0.9.0/icepaposc.egg-info/PKG-INFO
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      704 2022-07-07 07:01:12.000000 icepaposc-0.9.0/icepaposc.egg-info/SOURCES.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)        1 2022-07-07 07:01:12.000000 icepaposc-0.9.0/icepaposc.egg-info/dependency_links.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       55 2022-07-07 07:01:12.000000 icepaposc-0.9.0/icepaposc.egg-info/entry_points.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       36 2022-07-07 07:01:12.000000 icepaposc-0.9.0/icepaposc.egg-info/requires.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       10 2022-07-07 07:01:12.000000 icepaposc-0.9.0/icepaposc.egg-info/top_level.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       38 2022-07-07 07:01:12.000000 icepaposc-0.9.0/setup.cfg
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1504 2022-07-07 06:59:43.000000 icepaposc-0.9.0/setup.py
```

### Comparing `icepaposc-0.8.2/CONTRIBUTING.md` & `icepaposc-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `icepaposc-0.8.2/LICENSE` & `icepaposc-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `icepaposc-0.8.2/PKG-INFO` & `icepaposc-0.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: icepaposc
-Version: 0.8.2
+Version: 0.9.0
 Summary: Python IcePAP Extension
 Home-page: https://github.com/ALBA-Synchrotron/IcepapOCS
 Author: Jarkko Inki and Roberto Homs-Puron
 Author-email: ctbeamlines@cells.es
 License: GPL
 Description:  Python application to monitor and tune IcePAP based 
         systems.
```

### Comparing `icepaposc-0.8.2/icepaposc/__init__.py` & `icepaposc-0.9.0/icepaposc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with IcepapOCS. If not, see <http://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # The version is updated automatically with bumpversion
 # Do not update manually
-version = '0.8.2'
+version = '0.9.0'
```

### Comparing `icepaposc-0.8.2/icepaposc/__main__.py` & `icepaposc-0.9.0/icepaposc/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,18 @@
 
     parse.add_argument('host', help='IcePAP Host')
     parse.add_argument('--axis', help='Selected axis', default=1, type=int)
     parse.add_argument('-p', '--port', type=int, default=5000,
                        help='IcePAP port')
     parse.add_argument('-t', '--timeout', type=int, default=3,
                        help='Socket timeout')
+    parse.add_argument('--sigset', default='',
+                       help='.lst filename to import signals from')
+    parse.add_argument('--corr', default='', help='Default curves correction factors'
+                                        '--corr=\'pa,pb,ea,eb\'')
     parse.add_argument('-s', '--sig', nargs='*', default=[],
                        help='Preselected signals '
                             '<driver>:<signal name>:<Y-axis>')
 
     # TODO: Allow to pass the axes preselected and type of graph
     # parse.add_argument('-a', nargs='*', help='Axes to save, default all',
     #                    type=int, default=[])
@@ -56,16 +60,17 @@
     #                       help='Activate log level DEBUG')
 
     return parse
 
 
 def main():
     args = get_parser().parse_args()
+    print(args)
 
     app = QApplication(sys.argv)
-    win = WindowMain(args.host, args.port, args.timeout, args.sig, args.axis)
+    win = WindowMain(args.host, args.port, args.timeout, args.sig, args.axis, args.sigset, args.corr)
     win.show()
     sys.exit(app.exec_())
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `icepaposc-0.8.2/icepaposc/axis_time.py` & `icepaposc-0.9.0/icepaposc/axis_time.py`

 * *Files identical despite different names*

### Comparing `icepaposc-0.8.2/icepaposc/channel.py` & `icepaposc-0.9.0/icepaposc/channel.py`

 * *Files identical despite different names*

### Comparing `icepaposc-0.8.2/icepaposc/collector.py` & `icepaposc-0.9.0/icepaposc/collector.py`

 * *Files identical despite different names*

### Comparing `icepaposc-0.8.2/icepaposc/curve_item.py` & `icepaposc-0.9.0/icepaposc/curve_item.py`

 * *Files 22% similar despite different names*

```diff
@@ -37,56 +37,104 @@
         """
         self.subscription_id = subscription_id
         self.driver_addr = driver_addr
         self.signal_name = sig_name
         self.y_axis = y_axis
         self.array_time = []
         self.array_val = []
+        self.array_val_corr = []
         self.val_min = 0
         self.val_max = 0
+        self.val_cross = 0
+        self.val_local_min = 0
+        self.val_local_max = 0
         self.color = linecolor
         self.pen = {'color': linecolor,
                     'width': 1,
                     'style': linestyle}
         self.symbol = linemarker
         self.curve = None
         self.lock = RLock()
         self.signature = ''
         self.update_signature()
+        if sig_name.upper().startswith("POS"): 
+            self.signal_type = 1
+        elif sig_name.upper().startswith("DIF"):
+            self.signal_type = 3
+        elif sig_name.upper().startswith("ENC"):
+            self.signal_type = 2
+        elif sig_name.upper().startswith("VEL"):
+            self.signal_type = 3
+        else:
+            self.signal_type = 0
+        self.corr_factors = [1,0,1,0]
 
     def update_signature(self):
         """Sets the new value of the signature string."""
         self.signature = '{}:{}:{}'.format(self.driver_addr,
                                            self.signal_name,
                                            self.y_axis)
 
     def create_curve(self):
         """Creates a new plot item."""
         with self.lock:
             if self.symbol != '':
                 self.curve = PlotDataItem(x=self.array_time,
-                                          y=self.array_val,
+                                          y=self.array_val_corr,
                                           pen=self.pen,
                                           symbol=self.symbol,
                                           symbolBrush=QtGui.QBrush(self.color),
                                           symbolPen=self.color)
             else:
                 self.curve = PlotDataItem(x=self.array_time,
-                                          y=self.array_val,
+                                          y=self.array_val_corr,
                                           pen=self.pen)
 
         return self.curve
 
-    def update_curve(self, time_min, time_max):
+    def update_curve(self, time_min, time_max, corr_factors=[]):
         """Updates the curve with recent collected data."""
         with self.lock:
+            if corr_factors != None and corr_factors != [] :
+                self.corr_factors = corr_factors
+                self.update_array_val_corr()
             idx_min = self.get_time_index(time_min)
             idx_max = self.get_time_index(time_max)
             self.curve.setData(x=self.array_time[idx_min:idx_max],
-                               y=self.array_val[idx_min:idx_max])
+                               y=self.array_val_corr[idx_min:idx_max])
+                               
+    def update_array_val_corr(self):
+        if self.signal_type == 1:
+            self.array_val_corr = [self.corr_factors[0]*x + self.corr_factors[1] for x in self.array_val]
+        elif self.signal_type == 2:
+            self.array_val_corr = [self.corr_factors[2]*x + self.corr_factors[3] for x in self.array_val]
+        elif self.signal_type == 3:
+            self.array_val_corr = [self.corr_factors[0]*x for x in self.array_val]
+        self.val_min = min(self.array_val_corr)
+        self.val_max = max(self.array_val_corr)
+    
+    def calculate_val_corr(self, val):
+        if self.signal_type == 1:
+            return val * self.corr_factors[0] + self.corr_factors[1]
+        elif self.signal_type == 2:
+            return val * self.corr_factors[2] + self.corr_factors[3]
+        elif self.signal_type == 3:
+            return val * self.corr_factors[0]
+        else:
+            return val
+    
+    def calculate_local_min(self, t1, t2):
+        idx_min = self.get_time_index(t1)
+        idx_max = self.get_time_index(t2)
+        return min(self.array_val_corr[idx_min:idx_max])
+                               
+    def calculate_local_max(self, t1, t2):
+        idx_min = self.get_time_index(t1)
+        idx_max = self.get_time_index(t2)
+        return max(self.array_val_corr[idx_min:idx_max])
 
     def in_range(self, t):
         """
         Check to see if time is within range of collected data.
 
         t - Time value.
         Return: True if time is within range of collected data.
@@ -113,33 +161,38 @@
         """Store new collected data."""
         with self.lock:
             if not self.array_val:
                 self.val_min = self.val_max = new_data[0][1]
             for t, v in new_data:
                 self.array_time.append(t)
                 self.array_val.append(v)
-                if v > self.val_max:
+                vcorr = self.calculate_val_corr(v)
+                self.array_val_corr.append(vcorr)
+                #print(self.array_val_corr[-1])
+                #print(len(self.array_val_corr))
+                if vcorr > self.val_max:
                     self.val_max = v
-                elif v < self.val_min:
+                elif vcorr < self.val_min:
                     self.val_min = v
 
     def get_y(self, time_val):
         """
         Retrieve the signal value corresponding to the provided time value.
 
         t_val - Time value.
         Return: Signal value corresponding to an adjacent sample in time.
         """
         with self.lock:
             idx = self.get_time_index(time_val)
-            return self.array_val[idx]
+            return self.array_val_corr[idx]
 
     def clear(self):
         self.array_time[:] = []
         self.array_val[:] = []
+        self.array_val_corr[:] = []
 
     def get_time_index(self, time_val):
         """
         Retrieve the sample index corresponding to the provided time value.
 
         t_val - Time value.
         Return: Index of a sample adjacent to the provided time value.
```

### Comparing `icepaposc-0.8.2/icepaposc/custom_widgets/__init__.py` & `icepaposc-0.9.0/icepaposc/custom_widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `icepaposc-0.8.2/icepaposc/custom_widgets/square_radiobtn.py` & `icepaposc-0.9.0/icepaposc/custom_widgets/square_radiobtn.py`

 * *Files identical despite different names*

### Comparing `icepaposc-0.8.2/icepaposc/dialog_settings.py` & `icepaposc-0.9.0/icepaposc/dialog_settings.py`

 * *Files identical despite different names*

### Comparing `icepaposc-0.8.2/icepaposc/settings.py` & `icepaposc-0.9.0/icepaposc/settings.py`

 * *Files identical despite different names*

### Comparing `icepaposc-0.8.2/icepaposc/ui/__init__.py` & `icepaposc-0.9.0/icepaposc/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `icepaposc-0.8.2/icepaposc/ui/dialog_settings.ui` & `icepaposc-0.9.0/icepaposc/ui/dialog_settings.ui`

 * *Files identical despite different names*

### Comparing `icepaposc-0.8.2/icepaposc/ui/icons/__init__.py` & `icepaposc-0.9.0/icepaposc/ui/icons/__init__.py`

 * *Files identical despite different names*

### Comparing `icepaposc-0.8.2/icepaposc/ui/resources_rc.py` & `icepaposc-0.9.0/icepaposc/ui/resources_rc.py`

 * *Files identical despite different names*

### Comparing `icepaposc-0.8.2/icepaposc/ui/window_main.ui` & `icepaposc-0.9.0/icepaposc/ui/window_main.ui`

 * *Files 0% similar despite different names*

#### Comparing `icepaposc-0.8.2/icepaposc/ui/window_main.ui` & `icepaposc-0.9.0/icepaposc/ui/window_main.ui`

```diff
@@ -195,15 +195,15 @@
                                   <height>22</height>
                                 </size>
                               </property>
                               <property name="minimum">
                                 <number>1</number>
                               </property>
                               <property name="maximum">
-                                <number>3</number>
+                                <number>4</number>
                               </property>
                             </widget>
                           </item>
                         </layout>
                       </item>
                       <item>
                         <layout class="QGridLayout" name="gridLayout_7">
@@ -1508,14 +1508,24 @@
                     <item>
                       <property name="text">
                         <string>Y3</string>
                       </property>
                     </item>
                     <item>
                       <property name="text">
+                        <string>Y4</string>
+                      </property>
+                    </item>
+                    <item>
+                      <property name="text">
+                        <string>Y5</string>
+                      </property>
+                    </item>
+                    <item>
+                      <property name="text">
                         <string>X</string>
                       </property>
                     </item>
                   </widget>
                 </item>
                 <item row="0" column="0">
                   <widget class="QLabel" name="label_10">
```

### Comparing `icepaposc-0.8.2/icepaposc/window_main.py` & `icepaposc-0.9.0/icepaposc/window_main.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,33 +20,36 @@
 
 import pyqtgraph as pg
 import numpy as np
 import collections
 import time
 import datetime
 from PyQt5 import QtWidgets, Qt, QtCore, uic, QtGui
-from PyQt5.QtWidgets import QFileDialog
+from PyQt5.QtWidgets import QFileDialog, QShortcut, QApplication
+from PyQt5.QtGui import QKeySequence
+from PyQt5.Qt import QClipboard
 from pkg_resources import resource_filename
 from .collector import Collector
 from .dialog_settings import DialogSettings
 from .settings import Settings
 from .axis_time import AxisTime
 from .curve_item import CurveItem
 
 
 class WindowMain(QtWidgets.QMainWindow):
     """A dialog for plotting IcePAP signals."""
 
-    def __init__(self, host, port, timeout, siglist, selected_driver=None):
+    def __init__(self, host, port, timeout, siglist, selected_driver=None, sigset=None, corr=None):
         """
         Initializes an instance of class WindowMain.
 
         host            - IcePAP system address.
         port            - IcePAP system port number.
         timeout         - Socket timeout.
+        sigset          - .lst file with signal set to import
         siglist         - List of predefined signals.
                             Element Syntax: <driver>:<signal name>:<Y-axis>
                             Example: ["1:PosAxis:1", "1:MeasI:2", "1:MeasVm:3"]
         selected_driver - The driver to display in combobox at startup.
         """
         QtWidgets.QMainWindow.__init__(self, None)
 
@@ -54,14 +57,30 @@
         self.ui = self
         uic.loadUi(ui_filename, baseinstance=self.ui,
                    package="icepaposc.custom_widgets")
 
         self.setAttribute(QtCore.Qt.WA_DeleteOnClose, True)
         self.setWindowTitle('Oscilloscope | {}'.format(host))
         self.settings = Settings()
+        #Corrector factors for POS and ENC
+        if corr != None and corr !='' and corr.count(',')==3:
+             corr1 = corr.split(',')
+             print(corr1)
+             self.ui.txt_poscorr_a.setText(str(float(corr1[0])))
+             self.ui.txt_poscorr_b.setText(str(float(corr1[1])))
+             self.ui.txt_enccorr_a.setText(str(float(corr1[2])))
+             self.ui.txt_enccorr_b.setText(str(float(corr1[3])))
+             self._txt_poscorr_a_focus_lost()
+             self._txt_poscorr_b_focus_lost()
+             self._txt_enccorr_a_focus_lost()
+             self._txt_enccorr_b_focus_lost()
+        self.corr_factors = [1, 0, 1, 0]
+        self.cross_hair2_time = None
+        self.local_t1 = None
+        self.local_t2 = None
 
         try:
             self.collector = Collector(host,
                                        port,
                                        timeout,
                                        self.settings,
                                        self.callback_collect)
@@ -75,93 +94,153 @@
         self.curve_items = []
         self._paused = False
 
         # Switch to using white background and black foreground
         pg.setConfigOption('background', 'w')
         pg.setConfigOption('foreground', 'k')
         self.fgcolor = QtGui.QColor(0, 0, 0)
+        self.color_axes = self.fgcolor
 
         # Set up the plot area.
         self.plot_widget = pg.PlotWidget()
         self._plot_item = self.plot_widget.getPlotItem()
         self.view_boxes = [self.plot_widget.getViewBox(),
                            pg.ViewBox(),
+                           pg.ViewBox(), ##
+                           pg.ViewBox(), ##
                            pg.ViewBox()]
         self.ui.vloCurves.setDirection(QtWidgets.QBoxLayout.BottomToTop)
         self.ui.vloCurves.addWidget(self.plot_widget)
-
+        
+        
         # Set up the X-axis.
         self._plot_item.getAxis('bottom').hide()  # Hide the original X-axis.
         self._axisTime = AxisTime(orientation='bottom')  # Create new X-axis.
         self._axisTime.linkToView(self.view_boxes[0])
         self._plot_item.layout.removeItem(self._plot_item.getAxis('bottom'))
-        self._plot_item.layout.addItem(self._axisTime, 3, 1)
+        self._plot_item.layout.addItem(self._axisTime, 4, 1)
+        #self._plot_item.layout.addItem(self._axisTime, len(self.view_boxes), 1)
         self.now = self.collector.get_current_time()
         self.view_boxes[0].disableAutoRange(axis=self.view_boxes[0].XAxis)
         self.view_boxes[1].disableAutoRange(axis=self.view_boxes[1].XAxis)
         self.view_boxes[2].disableAutoRange(axis=self.view_boxes[2].XAxis)
+        self.view_boxes[3].disableAutoRange(axis=self.view_boxes[3].XAxis) ##
+        self.view_boxes[4].disableAutoRange(axis=self.view_boxes[4].XAxis) ##
         self._reset_x()
 
         # Set up the three Y-axes.
         self._plot_item.showAxis('right')
         self._plot_item.scene().addItem(self.view_boxes[1])
         self._plot_item.scene().addItem(self.view_boxes[2])
+        self._plot_item.scene().addItem(self.view_boxes[3]) ##
         ax3 = pg.AxisItem(orientation='right', linkView=self.view_boxes[2])
+        ax4 = pg.AxisItem(orientation='right', linkView=self.view_boxes[3]) ##
+        ax5 = pg.AxisItem(orientation='right', linkView=self.view_boxes[4]) ##
         self.axes = [self._plot_item.getAxis('left'),
-                     self._plot_item.getAxis('right'), ax3]
+                     self._plot_item.getAxis('right'), ax3, ax4, ax5] ##
         self.axes[1].linkToView(self.view_boxes[1])
         self.view_boxes[1].setXLink(self.view_boxes[0])
         self.view_boxes[2].setXLink(self.view_boxes[0])
+        self.view_boxes[3].setXLink(self.view_boxes[0]) ##
+        self.view_boxes[4].setXLink(self.view_boxes[0]) ##
         self._plot_item.layout.addItem(self.axes[2], 2, 3)
+        self._plot_item.layout.addItem(self.axes[3], 2, 4) ##
+        self._plot_item.layout.addItem(self.axes[4], 2, 5) ##
         self._plot_item.hideButtons()
         self._enable_auto_range_y()
 
         # Set up the crosshair vertical line.
         self.vertical_line = pg.InfiniteLine(angle=90, movable=False)
         self.view_boxes[0].addItem(self.vertical_line, ignoreBounds=True)
-
+        # Set up the fixed crosshair vertical for time measurements.
+        self.vertical_line2 = pg.InfiniteLine(angle=90, movable=False)
         # Initialize comboboxes and buttons.
         self._fill_combo_box_driver_ids(selected_driver)
         self._fill_combo_box_signals()
         self._update_button_status()
         self.ui.red_radio.setChecked(True)
         self.ui.solidline_radio.setChecked(True)
         self.ui.nomarker_radio.setChecked(True)
 
         # Set up signalling connections.
         self._connect_signals()
         self.proxy = pg.SignalProxy(self.plot_widget.scene().sigMouseMoved,
                                     rateLimit=60,
                                     slot=self._mouse_moved)
+        self.proxy1 = pg.SignalProxy(self.plot_widget.scene().sigMouseClicked,
+                                    rateLimit=60,
+                                    slot=self._mouse_clicked)
 
-        # Add any predefined signals.
+        # Add any predefined signals. 7, 9, 11 low contrast on black bgd
+        self.palette_colours = [
+                QtGui.QColor(255, 0, 0),
+                QtGui.QColor(0, 255, 0),
+                QtGui.QColor(0, 127, 255),
+                QtGui.QColor(0, 255, 255),
+                QtGui.QColor(255, 192, 203),
+                QtGui.QColor(255, 255, 0),
+                QtGui.QColor(0, 128, 0),
+                QtGui.QColor(0, 127, 127),
+                QtGui.QColor(127, 127, 0),
+                QtGui.QColor(128, 0, 0), #7
+                QtGui.QColor(0, 0, 255), #9
+                QtGui.QColor(127, 0, 127) #11
+            ]
+
+        button_id = 0
         for sig in siglist:
+            if button_id > 11:
+                button_id = 0
             lst = sig.split(':')
             if len(lst) != 3:
                 msg = 'Bad format of predefined signal "{}".\n' \
                       'It should be: ' \
                       '<driver>:<signal name>:<Y-axis>'.format(sig)
                 print(msg)
                 QtWidgets.QMessageBox.critical(self, 'Bad Signal Syntax', msg)
                 return
-
+            self._add_signal(int(lst[0]), lst[1], int(lst[2]),
+                self.palette_colours[button_id], 
+                QtCore.Qt.SolidLine, self.ui.marker_radio_group.checkedButton().text())
+            button_id = button_id + 1
+            
         # encoder count to motor step conversion factor measurement
         self.ecpmt_just_enabled = False
         self.step_ini = 0
         self.enc_ini = 0
 
         # Set up auto save of collected signal data.
         self._save_ticker = QtCore.QTimer()
         self._save_ticker.timeout.connect(self._auto_save)
         self._save_time = None
         self._idx = 0
         self._settings_updated = False
         self._file_path = None
         self._old_use_append = self.settings.use_append
         self._prepare_next_auto_save()
+        
+        #Import command line signal set
+        #print(sigset)
+        if sigset != '' and sigset != None:
+            self._import_signal_set(sigset)
+        
+        self.hotkey_filename = "default"
+        
+        #Cleanup the layout
+        self._remove_empty_y_axis(3) ##
+        self._remove_empty_y_axis(4) ##
+        self._remove_empty_y_axis(5) ##This is causing an issue
+        
+        #Corrector factors for POS and ENC. Offer possibility to switch between default (steps) or ui (units)
+        self.corr_factors_default = [1, 0, 1, 0]
+        self.corr_factors = [1, 0, 1, 0]
+        self.use_default_corr_factors = True
+        self.corr_factors_ui = [1, 0, 1, 0]
+        self.last_time_value = 0
+
 
     def _fill_combo_box_driver_ids(self, selected_driver):
         driver_ids = self.collector.get_available_drivers()
         for driver_id in driver_ids:
             self.ui.cbDrivers.addItem(str(driver_id))
         if selected_driver is not None:
             start_index = self.ui.cbDrivers.findText(str(selected_driver))
@@ -210,37 +289,80 @@
         self.ui.btnAxisOffsIncrease.clicked.connect(self._axis_offs_pp)
         self.ui.btnAxisOffsDecrease.clicked.connect(self._axis_offs_mm)
         self.ui.btnAxisScaleIncrease.clicked.connect(self._axis_scale_pp)
         self.ui.btnAxisScaleDecrease.clicked.connect(self._axis_scale_mm)
         self.ui.btnWhitebg.clicked.connect(self._do_white_background)
         self.ui.btnGreybg.clicked.connect(self._do_grey_background)
         self.ui.btnBlackbg.clicked.connect(self._do_black_background)
+        
+        self.shortcut = QShortcut(QKeySequence("Ctrl+O"), self)
+        self.shortcut.activated.connect(self._save_window_content_to_file)
+        self.shortcut = QShortcut(QKeySequence("Ctrl+Z"), self)
+        self.shortcut.activated.connect(self._signals_closed_loop_dynamic)
+        self.shortcut = QShortcut(QKeySequence("Ctrl+A"), self)
+        self.shortcut.activated.connect(self._signals_closed_loop_static)
+        self.shortcut = QShortcut(QKeySequence("Ctrl+E"), self)
+        self.shortcut.activated.connect(self._signals_open_loop)
+        self.shortcut = QShortcut(QKeySequence("Ctrl+U"), self)
+        self.shortcut.activated.connect(self._toggle_corr_factors)
+        self.shortcut = QShortcut(QKeySequence("Ctrl+I"), self)
+        self.shortcut.activated.connect(self._get_filename_string)
+        
+        self.ui.txt_poscorr_a.editingFinished.connect(self._txt_poscorr_a_focus_lost)
+        self.ui.txt_poscorr_b.editingFinished.connect(self._txt_poscorr_b_focus_lost)
+        self.ui.txt_enccorr_a.editingFinished.connect(self._txt_enccorr_a_focus_lost)
+        self.ui.txt_enccorr_b.editingFinished.connect(self._txt_enccorr_b_focus_lost)
+        
+    def _txt_poscorr_a_focus_lost(self):
+        self.ui.txt_poscorr_a.setCursorPosition(0)
+
+    def _txt_poscorr_b_focus_lost(self):
+        self.ui.txt_poscorr_b.setCursorPosition(0)
+
+    def _txt_enccorr_a_focus_lost(self):
+        self.ui.txt_enccorr_a.setCursorPosition(0)
+
+    def _txt_enccorr_b_focus_lost(self):
+        self.ui.txt_enccorr_b.setCursorPosition(0)
 
     def closeEvent(self, event):
         """Overloads (QMainWindow) QWidget.closeEvent()."""
         self._remove_all_signals()
         event.accept()
 
     def _update_views(self):
         """Updates the geometry of the view boxes."""
         self.view_boxes[1].setGeometry(self.view_boxes[0].sceneBoundingRect())
         self.view_boxes[2].setGeometry(self.view_boxes[0].sceneBoundingRect())
+        self.view_boxes[3].setGeometry(self.view_boxes[0].sceneBoundingRect()) ##
+        self.view_boxes[4].setGeometry(self.view_boxes[0].sceneBoundingRect()) ##
         self.view_boxes[1].linkedViewChanged(self.view_boxes[0],
                                              self.view_boxes[1].XAxis)
         self.view_boxes[2].linkedViewChanged(self.view_boxes[0],
                                              self.view_boxes[2].XAxis)
+        self.view_boxes[3].linkedViewChanged(self.view_boxes[0],
+                                             self.view_boxes[3].XAxis)  ##
+        self.view_boxes[4].linkedViewChanged(self.view_boxes[0],
+                                             self.view_boxes[4].XAxis)  ##
 
     def _update_button_status(self):
         val = self.ui.lvActiveSig.count() == 0
         self.ui.btnShift.setDisabled(val)
         self.ui.btnRemoveSel.setDisabled(val)
         self.ui.btnRemoveAll.setDisabled(val)
+        
+    def _get_filename_string(self):
+        name, done1 = QtWidgets.QInputDialog.getText(
+             self, 'Filename string', 'Input a file name string for the .csv files (20220131_1500_filename_string_*.csv:', text=self.hotkey_filename )
+        print(name)
+        self.hotkey_filename = name
 
     def _update_plot_axes_labels(self):
-        txt = ['', '', '']
+        #txt = ['', '', '']
+        txt = ['', '', '', '', '']
         for ci in self.curve_items:
             t = "<span style='font-size: 8pt; " \
                 "color: {};'>{}</span>".format(ci.color.name(), ci.signature)
             txt[ci.y_axis - 1] += t
         for i in range(0, len(self.axes)):
             self.axes[i].setLabel(txt[i])
 
@@ -250,17 +372,18 @@
     def _add_button_clicked(self):
         addr = int(self.ui.cbDrivers.currentText())
         my_signal_name = str(self.ui.cbSignals.currentText())
         my_axis = self.ui.sbAxis.value()
         my_linecolor = self._get_line_color()
         my_linestyle = self._get_line_style()
         my_linemarker = self._get_line_marker()
-        self._add_signal(addr, my_signal_name, my_axis,
+        self._add_signal(addr, my_signal_name, my_axis,  
                          my_linecolor, my_linestyle, my_linemarker)
-
+                         
+                         
     def _get_line_color(self):
         the_btn = self.ui.color_radio_group.checkedButton()
         if the_btn:
             return the_btn.palette().color(QtGui.QPalette.WindowText)
         else:
             return QtGui.QColor(0, 0, 0)
 
@@ -295,14 +418,15 @@
             msg = 'Failed to subscribe to signal {} ' \
                   'from driver {}.\n{}'.format(signal_name, driver_addr, e)
             print(msg)
             QtWidgets.QMessageBox.critical(self, 'Add Curve', msg)
             return
         ci = CurveItem(subscription_id, driver_addr, signal_name,
                        y_axis, linecolor, linestyle, linemarker)
+        self._add_y_axis(y_axis) ##
         self._add_curve(ci)
         self.curve_items.append(ci)
         self.collector.start(subscription_id)
         self.ui.lvActiveSig.addItem(ci.signature)
         index = len(self.curve_items) - 1
         self.ui.lvActiveSig.setCurrentRow(index)
         self.ui.lvActiveSig.item(index).setForeground(ci.color)
@@ -312,46 +436,96 @@
         if auto_save:
             self._auto_save(True)
 
     def _remove_selected_signal(self):
         self._auto_save(True)
         index = self.ui.lvActiveSig.currentRow()
         ci = self.curve_items[index]
+        y_axis = ci.y_axis
         self.collector.unsubscribe(ci.subscription_id)
         self._remove_curve_plot(ci)
         self.ui.lvActiveSig.takeItem(index)
         self.curve_items.remove(ci)
+        self._remove_empty_y_axis(y_axis) ##
         self._update_plot_axes_labels()
         self._update_button_status()
 
     def _remove_all_signals(self):
         """Removes all signals."""
         self._auto_save(True)
-        for ci in self.curve_items:
+        for index in range(self.ui.lvActiveSig.count()-1, -1, -1):
+            #print(index)
+            ci = self.curve_items[index]
             self.collector.unsubscribe(ci.subscription_id)
             self._remove_curve_plot(ci)
-        self.ui.lvActiveSig.clear()
+            y_axis = ci.y_axis
+            self.ui.lvActiveSig.takeItem(index)
+            self.curve_items.remove(ci)
+            self._remove_empty_y_axis(y_axis) ##
+        #self.ui.lvActiveSig.clear()
         self.curve_items = []
+        ##self._remove_empty_y_axes() ##
         self._update_plot_axes_labels()
         self._update_button_status()
+        self.hotkey_filename = "default"
+        
+    def _add_y_axis(self, y_axis): ##
+        #print(y_axis, "add")
+        i = y_axis - 1
+        if y_axis > 2 and self.y_axis_empty(y_axis):
+            self.view_boxes[i] = pg.ViewBox()
+            self.view_boxes[i].disableAutoRange(axis=self.view_boxes[i].XAxis) ##
+            self._plot_item.scene().addItem(self.view_boxes[i])
+            self.axes[i] = pg.AxisItem(orientation='right', linkView=self.view_boxes[i])
+            self.view_boxes[i].setXLink(self.view_boxes[0])
+            self._plot_item.layout.addItem(self.axes[i], 2, y_axis)
+            self.axes[i].setPen(self.color_axes)
+            self.axes[i].setTextPen(self.color_axes)
+
+            
+    def _remove_empty_y_axis(self, y_axis): ##
+            #print(y_axis, "remove")
+            i = y_axis -1
+            #for i in range(len(self.axes)):
+            if i != None and i > 1:
+                if self.y_axis_empty(y_axis):
+                    try:
+                        self._plot_item.layout.removeItem(self.axes[i]) ##
+                        self._plot_item.scene().removeItem(self.axes[i]) ##
+                        self._plot_item.scene().removeItem(self.view_boxes[i]) ###Why does this fail at the init
+                    except:
+                        return
+
+    def y_axis_empty(self, y_axis):
+        for ci in self.curve_items:
+            if ci.y_axis == y_axis:
+                #print(y_axis, "not empty")
+                return False
+        #print(y_axis, "empty")
+        return True
+                
 
     def _shift_button_clicked(self):
         """Assign a curve to a different y axis."""
         index = self.ui.lvActiveSig.currentRow()
         ci = self.curve_items[index]
         self._remove_curve_plot(ci)
-        ci.y_axis = (ci.y_axis % 3) + 1
+        y_axis = ci.y_axis
+        self._add_y_axis((ci.y_axis % len(self.axes)) + 1) ##
+        ci.y_axis = (ci.y_axis % len(self.axes)) + 1
+        self._remove_empty_y_axis(y_axis) ##
         ci.update_signature()
         self._add_curve(ci)
         self.ui.lvActiveSig.takeItem(index)
         self.ui.lvActiveSig.insertItem(index, ci.signature)
         self.ui.lvActiveSig.item(index).setForeground(ci.color)
         self.ui.lvActiveSig.item(index).setBackground(Qt.QColor(0, 0, 0))
         self.ui.lvActiveSig.setCurrentRow(index)
         self._update_plot_axes_labels()
+        
 
     def _add_curve(self, ci):
         """
         Create a new curve and add it to a viewbox.
 
         ci - Curve item that will be the owner.
         """
@@ -360,40 +534,100 @@
 
     def _mouse_moved(self, evt):
         """
         Acts om mouse move.
 
         evt - Event containing the position of the mouse pointer.
         """
+        #print(evt)
         pos = evt[0]  # The signal proxy turns original arguments into a tuple.
         if self.plot_widget.sceneBoundingRect().contains(pos):
             mouse_point = self.view_boxes[0].mapSceneToView(pos)
             time_value = mouse_point.x()
+            self.last_time_value = time_value
+            self._update_signals_text(time_value)
+
+    def _update_signals_text(self, time_value):
+        try:
+            date = datetime.datetime.fromtimestamp(time_value)
+            pretty_time = date.strftime("%H:%M:%S.%f")[:-3]
+        except ValueError:  # Time out of range.
+            return
+        txtmax = ''
+        txtnow = ''
+        txtmin = ''
+        txtdiff = ''
+        txtlocalmin = ''
+        txtlocalmax = ''
+        text_size = 9
+        for ci in self.curve_items:
+            tmp = "<span style='font-size: {}pt; color: {};'>|"
+            tmp = tmp.format(text_size, ci.color.name())
+            if ci.in_range(time_value):
+                txtmax += "{}{}</span>".format(tmp, ci.val_max)
+                txtnow += "{}{}</span>".format(tmp, ci.get_y(time_value))
+                txtmin += "{}{}</span>".format(tmp, ci.val_min)
+                if self.cross_hair2_time != None:
+                    #print(ci.val_cross, ci.get_y(time_value))
+                    txtdiff += "{}{}</span>".format(tmp, ci.get_y(time_value) - ci.val_cross)
+            #You can enter here because of a click after a double click or after a ctrlo
+            if self.local_t1 != None and self.local_t2 != None and ci.in_range(self.local_t1) and ci.in_range(self.local_t2):
+                txtlocalmin += "{}{}</span>".format(tmp, ci.calculate_local_min(self.local_t1, self.local_t2))
+                txtlocalmax += "{}{}</span>".format(tmp, ci.calculate_local_max(self.local_t1, self.local_t2))
+        if self.cross_hair2_time != None:
+            tmp = "|<span style='font-size: {}pt; color: {};'>{} {}</span>"
+            txtnow += tmp.format(text_size,
+                             str(self.fgcolor.name()), pretty_time, 
+                             datetime.datetime.fromtimestamp(abs(time_value-self.cross_hair2_time)).strftime("%S.%f")[:-3])
+            tmp = "|<span style='font-size: {}pt; color: {};'>{} {}</span>"
+        else:
+            tmp = "|<span style='font-size: {}pt; color: {};'>{}</span>"
+            txtnow += tmp.format(text_size,
+                             str(self.fgcolor.name()), pretty_time)
+
+        if self.cross_hair2_time != None: 
+            title = "<br>{}<br>{}<br>{}<br>{}".format(txtmax, txtnow, txtmin, txtdiff)
+        else:
+            if self.local_t2 != None and self.local_t1 != None: #you can't have crosshair on and display locals
+                title = "<br>{}<br>{}<br>{}".format(txtlocalmax, txtnow, txtlocalmin)
+            else:
+                title = "<br>{}<br>{}<br>{}".format(txtmax, txtnow, txtmin)
+        self.plot_widget.setTitle(title)
+        self.vertical_line.setPos(time_value)
+            
+    def _mouse_clicked(self, evt):
+        pos = evt[0]  # The signal proxy turns original arguments into a tuple.
+        mouse_point = self.view_boxes[0].mapSceneToView(evt[0].scenePos())
+        time_value = mouse_point.x()
+        if evt[0].double():
             try:
                 date = datetime.datetime.fromtimestamp(time_value)
                 pretty_time = date.strftime("%H:%M:%S.%f")[:-3]
             except ValueError:  # Time out of range.
                 return
-            txtmax = ''
-            txtnow = ''
-            txtmin = ''
-            text_size = 10
+            self.cross_hair2_time = time_value
+            self.view_boxes[0].addItem(self.vertical_line2, ignoreBounds=True)
+            self.vertical_line2.setPos(mouse_point.x())
             for ci in self.curve_items:
-                tmp = "<span style='font-size: {}pt; color: {};'>|"
-                tmp = tmp.format(text_size, ci.color.name())
                 if ci.in_range(time_value):
-                    txtmax += "{}{}</span>".format(tmp, ci.val_max)
-                    txtnow += "{}{}</span>".format(tmp, ci.get_y(time_value))
-                    txtmin += "{}{}</span>".format(tmp, ci.val_min)
-            tmp = "|<span style='font-size: {}pt; color: {};'>{}</span>"
-            txtnow += tmp.format(text_size,
-                                 str(self.fgcolor.name()), pretty_time)
-            title = "<br>{}<br>{}<br>{}".format(txtmax, txtnow, txtmin)
-            self.plot_widget.setTitle(title)
-            self.vertical_line.setPos(mouse_point.x())
+                    ci.val_cross = ci.get_y(time_value)
+            self.local_t1 = time_value 
+            self.local_t2 = None
+        else:
+            if self.cross_hair2_time != None:
+                self.cross_hair2_time = None
+                self.view_boxes[0].removeItem(self.vertical_line2)
+            if self.local_t2 == None:
+                self.local_t2 = time_value
+            else:
+                self.local_t1 = None
+                self.local_t2 = None
+        #print(evt)
+            
+            
 
     def _remove_curve_plot(self, ci):
         """
         Remove a curve from the plot area.
 
         ci - Curve item to remove.
         """
@@ -412,90 +646,217 @@
     def _do_black_background(self):
         color_axes = QtGui.QColor(255, 255, 255)
         color_plot = QtGui.QColor(0, 0, 0)
         self._set_plot_colors(color_axes, color_plot)
 
     def _set_plot_colors(self, color_axes, color_plot):
         self.plot_widget.setBackground(color_plot)
-        for i in range(3):
+        self.color_axes = color_axes
+        for i in range(len(self.axes)):   ##
             self.axes[i].setPen(color_axes)
             self.axes[i].setTextPen(color_axes)
         self._axisTime.setPen(color_axes)
         self._axisTime.setTextPen(color_axes)
         self.fgcolor = color_axes
 
     def _signals_closed_loop(self):
         """Display a specific set of curves."""
         self._remove_all_signals()
         drv_addr = int(self.ui.cbDrivers.currentText())
-        self._add_signal(drv_addr, 'PosAxis', 1, QtGui.QColor(
-            255, 0, 0), QtCore.Qt.SolidLine, '')
-        self._add_signal(drv_addr, 'DifAxTgtenc', 2, QtGui.QColor(
-            0, 255, 0), QtCore.Qt.SolidLine, '')
-        self._add_signal(drv_addr, 'DifAxMotor', 2, QtGui.QColor(
-            0, 127, 255), QtCore.Qt.SolidLine, '')
-        self._add_signal(drv_addr, 'StatReady', 3, QtGui.QColor(
-            0, 255, 255), QtCore.Qt.DotLine, '')
-        self._add_signal(drv_addr, 'StatMoving', 3, QtGui.QColor(
-            255, 192, 203), QtCore.Qt.DotLine, '')
-        self._add_signal(drv_addr, 'StatSettling', 3, QtGui.QColor(
-            255, 255, 0), QtCore.Qt.DotLine, '')
-        self._add_signal(drv_addr, 'StatOutofwin', 3,
-                         QtGui.QColor(128, 0, 0), QtCore.Qt.DotLine, '')
-        self._add_signal(drv_addr, 'StatWarning', 3,
-                         QtGui.QColor(0, 128, 0), QtCore.Qt.DotLine, '')
-        self._add_signal(drv_addr, 'StatStopcode', 3,
-                         QtGui.QColor(255, 0, 0), QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'PosAxis', 1, self.palette_colours[0], 
+            QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'DifAxTgtenc', 2, self.palette_colours[1], 
+            QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'DifAxMotor', 4, self.palette_colours[2], 
+            QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'VelCurrent', 5, self.palette_colours[3],
+            QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'VelMotor', 5, self.palette_colours[4], 
+            QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'StatReady', 3, self.palette_colours[4], 
+            QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'StatMoving', 3, self.palette_colours[5], 
+            QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'StatSettling', 3, self.palette_colours[6], 
+            QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'StatOutofwin', 3, self.palette_colours[7], 
+            QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'StatWarning', 3, self.palette_colours[8], 
+            QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'StatStopcode', 3, self.palette_colours[9], 
+            QtCore.Qt.DotLine, '')
         self.view_boxes[0].enableAutoRange(axis=self.view_boxes[0].YAxis)
         self.view_boxes[1].disableAutoRange(axis=self.view_boxes[1].YAxis)
         self.view_boxes[1].setYRange(-30, 70, padding=0)
         self.view_boxes[2].disableAutoRange(axis=self.view_boxes[2].YAxis)
         self.view_boxes[2].setYRange(-1, 20, padding=0)
+        self.hotkey_filename = "Closed_loop_plot"
 
     def _signals_currents(self):
         """Display a specific set of curves."""
         self._remove_all_signals()
         drv_addr = int(self.ui.cbDrivers.currentText())
         self._add_signal(drv_addr, 'PosAxis', 1, QtGui.QColor(
             255, 0, 0), QtCore.Qt.SolidLine, '')
-        self._add_signal(drv_addr, 'MeasI', 2, QtGui.QColor(
+        self._add_signal(drv_addr, 'PosTgtenc', 1, QtGui.QColor(
+            255, 192, 203), QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'MeasI', 3, QtGui.QColor(
             0, 255, 0), QtCore.Qt.SolidLine, '')
-        self._add_signal(drv_addr, 'MeasVm', 3, QtGui.QColor(
+        self._add_signal(drv_addr, 'VelCurrent', 2, QtGui.QColor(
             0, 127, 255), QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'VelMotor', 2, QtGui.QColor(
+            255, 255, 0), QtCore.Qt.SolidLine, '')
         # Ajust plot axis
         self.view_boxes[0].enableAutoRange(axis=self.view_boxes[0].YAxis)
-        self.view_boxes[1].disableAutoRange(axis=self.view_boxes[1].YAxis)
-        self.view_boxes[1].setYRange(-9, 10, padding=0)
-        self.view_boxes[2].enableAutoRange(axis=self.view_boxes[2].YAxis)
+        self.view_boxes[1].enableAutoRange(axis=self.view_boxes[1].YAxis)
+        self.view_boxes[2].disableAutoRange(axis=self.view_boxes[2].YAxis)
+        self.view_boxes[2].setYRange(-0.5, 17.5, padding=0)
+        self.hotkey_filename = "Currents_plot"
+
+    def _signals_closed_loop_dynamic(self):
+        """Display a specific set of curves."""
+        self._remove_all_signals()
+        drv_addr = int(self.ui.cbDrivers.currentText())
+        self._add_signal(drv_addr, 'PosAxis', 1, self.palette_colours[0],
+            QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'DifAxTgtenc', 2, self.palette_colours[1], 
+            QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'DifAxMotor', 2, self.palette_colours[2], 
+            QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'VelCurrent', 4, self.palette_colours[3],
+            QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'VelMotor', 4, self.palette_colours[4], 
+            QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'MeasI', 3, self.palette_colours[5], 
+            QtCore.Qt.SolidLine, '')            
+        self._add_signal(drv_addr, 'EncTgtenc', 5, self.palette_colours[6], 
+            QtCore.Qt.SolidLine, '')            
+        self._add_signal(drv_addr, 'StatReady', 3, self.palette_colours[4], 
+            QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'StatMoving', 3, self.palette_colours[5], 
+            QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'StatSettling', 3, self.palette_colours[6], 
+            QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'StatOutofwin', 3, self.palette_colours[7], 
+            QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'StatWarning', 3, self.palette_colours[8], 
+            QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'StatStopcode', 3, self.palette_colours[9], 
+            QtCore.Qt.DotLine, '')
+        # Ajust plot axis
+        self.view_boxes[0].enableAutoRange(axis=self.view_boxes[0].YAxis)
+        self.view_boxes[1].enableAutoRange(axis=self.view_boxes[1].YAxis)
+        self.view_boxes[3].enableAutoRange(axis=self.view_boxes[3].YAxis)
+        self.view_boxes[4].enableAutoRange(axis=self.view_boxes[4].YAxis)
+        self.view_boxes[2].disableAutoRange(axis=self.view_boxes[2].YAxis)
+        self.view_boxes[2].setYRange(-0.5, 17.5, padding=0)
+        self.hotkey_filename = "Closed_loopd_plot"
+        self._do_black_background()
+
+    def _signals_closed_loop_static(self):
+        """Display a specific set of curves."""
+        self._remove_all_signals()
+        drv_addr = int(self.ui.cbDrivers.currentText())
+        self._add_signal(drv_addr, 'PosAxis', 1, self.palette_colours[0], 
+            QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'DifAxTgtenc', 2, self.palette_colours[1], 
+            QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'DifAxMotor', 4, self.palette_colours[2], 
+            QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'EncTgtenc', 5, self.palette_colours[3], 
+            QtCore.Qt.SolidLine, '')            
+        self._add_signal(drv_addr, 'StatReady', 3, self.palette_colours[4], 
+            QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'StatMoving', 3, self.palette_colours[5], 
+            QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'StatSettling', 3, self.palette_colours[6], 
+            QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'StatOutofwin', 3, self.palette_colours[7], 
+            QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'StatWarning', 3, self.palette_colours[8], 
+            QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'StatStopcode', 3, self.palette_colours[9], 
+            QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'MeasI', 3, self.palette_colours[10], 
+            QtCore.Qt.SolidLine, '')            
+        self.view_boxes[0].enableAutoRange(axis=self.view_boxes[0].YAxis)
+        self.view_boxes[1].enableAutoRange(axis=self.view_boxes[1].YAxis)
+        self.view_boxes[3].enableAutoRange(axis=self.view_boxes[3].YAxis)
+        self.view_boxes[4].enableAutoRange(axis=self.view_boxes[4].YAxis)
+        self.view_boxes[2].disableAutoRange(axis=self.view_boxes[2].YAxis)
+        self.view_boxes[2].setYRange(-0.5, 17.5, padding=0)
+        self.hotkey_filename = "Closed_loops_plot"
+        self._do_black_background()
+        
+    def _signals_open_loop(self):
+        """Display a specific set of curves."""
+        self._remove_all_signals()
+        drv_addr = int(self.ui.cbDrivers.currentText())
+        self._add_signal(drv_addr, 'PosAxis', 1, self.palette_colours[0], 
+            QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'DifAxTgtenc', 2, self.palette_colours[1], 
+            QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'EncTgtenc', 4, self.palette_colours[2], 
+            QtCore.Qt.SolidLine, '')            
+        self._add_signal(drv_addr, 'StatWarning', 3, self.palette_colours[3], 
+            QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'MeasI', 3, self.palette_colours[4], 
+            QtCore.Qt.DotLine, '')
+        self._add_signal(drv_addr, 'VelMotor', 5, self.palette_colours[5], 
+            QtCore.Qt.SolidLine, '')   #Not necessary 
+        self.view_boxes[0].enableAutoRange(axis=self.view_boxes[0].YAxis)
+        self.view_boxes[1].enableAutoRange(axis=self.view_boxes[1].YAxis)
+        self.view_boxes[3].enableAutoRange(axis=self.view_boxes[3].YAxis)
+        self.view_boxes[4].enableAutoRange(axis=self.view_boxes[4].YAxis)
+        self.view_boxes[2].disableAutoRange(axis=self.view_boxes[2].YAxis)
+        self.view_boxes[2].setYRange(-0.5, 17.5, padding=0)
+        self.hotkey_filename = "Open_loop_plot"
+        self._do_black_background()
 
+        
     def _signals_velocities(self):
         """Display a specific set of curves."""
         self._remove_all_signals()
         drv_addr = int(self.ui.cbDrivers.currentText())
         self._add_signal(drv_addr, 'PosAxis', 1, QtGui.QColor(
             255, 0, 0), QtCore.Qt.SolidLine, '')
-        self._add_signal(drv_addr, 'VelCurrent', 2, QtGui.QColor(
+        self._add_signal(drv_addr, 'PosTgtenc', 1, QtGui.QColor(
+            255, 192, 203), QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'DifAxMotor', 2, QtGui.QColor(
+            0, 127, 255), QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'DifAxTgtenc', 2, QtGui.QColor(
             0, 255, 0), QtCore.Qt.SolidLine, '')
-        self._add_signal(drv_addr, 'VelMotor', 2, QtGui.QColor(
+        self._add_signal(drv_addr, 'VelCurrent', 3, QtGui.QColor(
             0, 127, 255), QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'VelMotor', 3, QtGui.QColor(
+            255, 255, 0), QtCore.Qt.SolidLine, '')
         # Ajust plot axis
         self.view_boxes[0].enableAutoRange(axis=self.view_boxes[0].YAxis)
         self.view_boxes[1].enableAutoRange(axis=self.view_boxes[1].YAxis)
-        #self.view_boxes[1].disableAutoRange(axis=self.view_boxes[1].YAxis)
-        #self.view_boxes[1].setYRange(-9, 10, padding=0)
+        #self.view_boxes[2].disableAutoRange(axis=self.view_boxes[2].YAxis)
+        #self.view_boxes[2].setYRange(-0.5, 17.5, padding=0)
         self.view_boxes[2].enableAutoRange(axis=self.view_boxes[2].YAxis)
+        self.hotkey_filename = "Velocities_plot"
+
 
     def _signals_target(self):
         """Display a specific set of curves."""
         self._remove_all_signals()
         drv_addr = int(self.ui.cbDrivers.currentText())
         self._add_signal(drv_addr, 'PosAxis', 1, QtGui.QColor(
             255, 0, 0), QtCore.Qt.SolidLine, '')
-        self._add_signal(drv_addr, 'EncTgtenc', 2, QtGui.QColor(
+        self._add_signal(drv_addr, 'PosTgtenc', 1, QtGui.QColor(
+            255, 192, 203), QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'DifAxTgtenc', 2, QtGui.QColor(
             0, 255, 0), QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'DifAxMotor', 2, QtGui.QColor(
+            0, 127, 255), QtCore.Qt.SolidLine, '')
+        self._add_signal(drv_addr, 'EncTgtenc', 3, QtGui.QColor(
+            255, 255, 0), QtCore.Qt.SolidLine, '')
+        self.hotkey_filename = "Target_plot"
 
     def _clear_all(self):
         """Clear all the displayed curves."""
         self._auto_save()
         for ci in self.curve_items:
             ci.clear()
 
@@ -506,19 +867,22 @@
             t = ci.start_time()
             if 0 < t < time_start:
                 time_start = t
         self.view_boxes[0].setXRange(time_start,
                                      self.collector.get_current_time(),
                                      padding=0)
 
-    def _import_signal_set(self):
-        fname = QFileDialog.getOpenFileName(
-            self, "Import Signal Set",
-            filter="Signal Set Files Files (*.lst);;All Files (*)",
-            directory=self.settings.signals_set_folder)
+    def _import_signal_set(self, filename=None):
+        if filename == None:
+            fname = QFileDialog.getOpenFileName(
+                self, "Import Signal Set",
+                filter="Signal Set Files Files (*.lst);;All Files (*)",
+                directory=self.settings.signals_set_folder)
+        else:
+            fname = [filename]
         if fname:
             self._remove_all_signals()
             drv_addr = int(self.ui.cbDrivers.currentText())
             with open(fname[0], 'r') as f:
                 for ll in f:
                     tokens = ll.split()
                     if len(tokens) < 4:
@@ -556,15 +920,18 @@
         now = self.collector.get_current_time()
         start = now - self.settings.default_x_axis_len
         self.view_boxes[0].setXRange(start, now, padding=0)
 
     def _enable_auto_range_y(self):
         self.view_boxes[0].enableAutoRange(axis=self.view_boxes[0].YAxis)
         self.view_boxes[1].enableAutoRange(axis=self.view_boxes[1].YAxis)
-        self.view_boxes[2].enableAutoRange(axis=self.view_boxes[2].YAxis)
+        #Keep 2 for status/currents that don't need often autoranging
+        #self.view_boxes[2].enableAutoRange(axis=self.view_boxes[2].YAxis) 
+        self.view_boxes[3].enableAutoRange(axis=self.view_boxes[3].YAxis)##
+        self.view_boxes[4].enableAutoRange(axis=self.view_boxes[4].YAxis)##
 
     def _pause_x_axis(self):
         """Freeze the X axis."""
         if self._paused:
             self._paused = False
             self.ui.btnPause.setText('Pause')
         else:
@@ -578,54 +945,87 @@
         x_min = self.view_boxes[0].viewRange()[0][0]
         x_max = self.view_boxes[0].viewRange()[0][1]
         self.view_boxes[0].setXRange(now - (x_max - x_min), now, padding=0)
 
     def enable_action(self, enable=True):
         """Enables or disables menu item File|Settings."""
         self.ui.actionSettings.setEnabled(enable)
+        
+    def _save_window_content_to_file(self):
+        if self.corr_factors == [1, 0, 1, 0]:
+            unitstr = "st"
+        else:
+            unitstr = "u"
+        filename1 = "{:03d}_{}_{}_{}.csv".format(int(self.ui.cbDrivers.currentText()), time.strftime("%y%m%d_%H%M%S", time.localtime()), self.hotkey_filename, unitstr)
+        QApplication.clipboard().setText(filename1)
+        #print(filename1)
+        user_path = os.path.expanduser("~")
+        base_folder = os.path.join(user_path, '.icepaposc')
+        filename2 = os.path.join(base_folder,(filename1))
+        #print(filename2)
+        self._save_to_file(filename2)
 
-    def _save_to_file(self):
+    def _save_to_file(self, filename = None):
         if not self.curve_items:
             return
-        capt = "Save to csv file"
-        fa = QtWidgets.QFileDialog.getSaveFileName(caption=capt,
+        if filename == None or filename == False:
+            capt = "Save to csv file"
+            fa = QtWidgets.QFileDialog.getSaveFileName(caption=capt,
                                                    filter="*.csv")
-        fn = str(fa[0])
+            fn = str(fa[0])
+        else:
+            x_min = self.view_boxes[0].viewRange()[0][0]
+            x_max = self.view_boxes[0].viewRange()[0][1]
+            fn = filename
+            #If set visible window as local window and update legend
+            self.local_t1 = x_min
+            self.local_t2 = x_max
+            self._update_signals_text(self.last_time_value)
         if not fn:
             return
         if fn[-4:] != ".csv":
             fn = fn + ".csv"
         try:
             f = open(fn, "w+")
         except Exception as e:
             msg = 'Failed to open/create file: {}\n{}'.format(fn, e)
             print(msg)
             QtWidgets.QMessageBox.critical(self, 'File Open Failed', msg)
             return
-        self._create_csv_file(f)
+        if filename == None or filename == False:
+            self._create_csv_file(f)
+        else:
+            self._create_csv_file(f, [x_min, x_max])
         f.close()
+        
 
-    def _create_csv_file(self, csv_file):
+    def _create_csv_file(self, csv_file, time_range=None):
         my_dict = collections.OrderedDict()
         for ci in self.curve_items:
             header = "time-{}-{}".format(ci.driver_addr, ci.signal_name)
             my_dict[header] = ci.array_time
             header = "val-{}-{}".format(ci.driver_addr, ci.signal_name)
-            my_dict[header] = ci.array_val
+            my_dict[header] = ci.array_val_corr
         key_longest = list(my_dict.keys())[0]
         for key in my_dict:
             if my_dict[key][0] < my_dict[key_longest][0]:
                 key_longest = key
         for key in my_dict:
             delta = len(my_dict[key_longest]) - len(my_dict[key])
             my_dict[key] = delta * [np.nan] + my_dict[key]
         for key in my_dict:
             csv_file.write(",{}".format(key))
         csv_file.write("\n")
-        for idx in range(0, len(my_dict[key_longest])):
+        if time_range == None:
+            idx_ini = 0
+            idx_end = len(my_dict[key_longest])
+        else:
+            idx_ini = self.curve_items[0].get_time_index(time_range[0])
+            idx_end = self.curve_items[0].get_time_index(time_range[1])
+        for idx in range(idx_ini, idx_end):
             line = str(idx)
             for key in my_dict:
                 line += ",{}".format(my_dict[key][idx])
             csv_file.write(line + '\n')
 
     def _auto_save(self, use_new_file=False):
         if not self.curve_items or not self._file_path:
@@ -637,15 +1037,15 @@
         # Create matrix.
         my_dict = collections.OrderedDict()
         for ci in self.curve_items:
             start_idx = ci.get_time_index(self._save_time)
             header = "time-{}-{}".format(ci.driver_addr, ci.signal_name)
             my_dict[header] = ci.array_time[start_idx:]
             header = "val-{}-{}".format(ci.driver_addr, ci.signal_name)
-            my_dict[header] = ci.array_val[start_idx:]
+            my_dict[header] = ci.array_val_corr[start_idx:]
         key_longest = None
         for key in my_dict:  # Find a non empty list.
             if my_dict[key]:
                 key_longest = key
                 break
         if not key_longest:
             self._prepare_next_auto_save(True)
@@ -726,40 +1126,37 @@
         value_list - List of tuples (time, value).
         """
         for ci in self.curve_items:
             if ci.subscription_id == subscription_id:
                 ci.collect(value_list)
         if not self._paused:
             self._update_view()
+        else:
+            x_min = self.view_boxes[0].viewRange()[0][0]
+            x_max = self.view_boxes[0].viewRange()[0][1]
+            self._update_curves(x_min, x_max)
 
     def _update_view(self):
         x_min = self.view_boxes[0].viewRange()[0][0]
         x_max = self.view_boxes[0].viewRange()[0][1]
 
         # Update the X-axis.
         now_in_range = self.now <= x_max
         self.now = self.collector.get_current_time()
         if now_in_range:
             self.view_boxes[0].setXRange(self.now - (x_max - x_min),
                                          self.now,
                                          padding=0)
         self.ui.btnNow.setDisabled(now_in_range)
 
-        try:
-            # retrieve POS and ENC affine corrections
-            self.collector.poscorr_a = float(self.ui.txt_poscorr_a.text())
-            self.collector.poscorr_b = float(self.ui.txt_poscorr_b.text())
-            self.collector.enccorr_a = float(self.ui.txt_enccorr_a.text())
-            self.collector.enccorr_b = float(self.ui.txt_enccorr_b.text())
-        except ValueError:
-            pass
-
-        # Update the curves.
-        for ci in self.curve_items:
-            ci.update_curve(x_min, x_max)
+        # Update the displayed curves based on corrections
+        self._update_curves(x_min, x_max)
+     
+        # Update the legend 
+        self._update_signals_text(self.last_time_value)
 
         # Update encoder count to motor step conversion factor measurement
         if self.ui.chkEctsTurn.isChecked():
             addr = self.collector.channels[
                 self.collector.current_channel].icepap_address
             step_now = self.collector.icepap_system[addr].get_pos("AXIS")
             cfgANSTEP = int(
@@ -781,22 +1178,73 @@
             if (step_now - self.step_ini) != 0:
                 enc_cts_per_motor_turn = \
                     (enc_now - self.enc_ini) * 1.0 * cfgANSTEP \
                     / ((step_now - self.step_ini) * cfgANTURN)
             else:
                 enc_cts_per_motor_turn = 0
             self.ui.txtEctsTurn.setText(str(enc_cts_per_motor_turn))
+            self.ui.txtEctsTurn.setCursorPosition(0)
+            
+    def _update_curves(self, x_min, x_max):
+        corr_factors_need_update = False
+        try:
+            # retrieve POS and ENC affine corrections
+            pa = float(self.ui.txt_poscorr_a.text())
+            if pa == '': pa = self.corr_factors[0]
+            pb = float(self.ui.txt_poscorr_b.text())
+            if pb == '': pb = self.corr_factors[1]
+            ea = float(self.ui.txt_enccorr_a.text())
+            if ea == '': ea = self.corr_factors[2]
+            eb = float(self.ui.txt_enccorr_b.text())
+            if eb == '': eb = self.corr_factors[3]
+            
+            #print([pa, pb, ea, eb])
+
+            self.collector.poscorr_a = 1 #float(self.ui.txt_poscorr_a.text())
+            self.collector.poscorr_b = 0 #float(self.ui.txt_poscorr_b.text())
+            self.collector.enccorr_a = 1 #float(self.ui.txt_enccorr_a.text())
+            self.collector.enccorr_b = 0 #float(self.ui.txt_enccorr_b.text())
+            
+            #If the ui corr_factors changed, or a switch from ui to def was requested, change.
+            #Ui change takes precedence:
+            if pa != self.corr_factors_ui[0] or pb != self.corr_factors_ui[1] or \
+                ea != self.corr_factors_ui[2] or eb != self.corr_factors_ui[3]: 
+                corr_factors_need_update = True
+                self.corr_factors_ui = [pa, pb, ea, eb]
+                self.corr_factors = self.corr_factors_ui
+                self.use_default_corr_factors = False
+            elif self.use_default_corr_factors and self.corr_factors != self.corr_factors_default:
+                corr_factors_need_update = True
+                self.corr_factors = self.corr_factors_default
+            elif (not self.use_default_corr_factors) and (self.corr_factors == self.corr_factors_default):
+                corr_factors_need_update = True
+                self.corr_factors = self.corr_factors_ui
+                
+        except ValueError:
+            pass
+
+        # Update the curves.
+        for ci in self.curve_items:
+            if corr_factors_need_update: 
+                ci.update_curve(x_min, x_max, corr_factors=self.corr_factors)
+                self._update_signals_text(self.last_time_value)
+            else:
+                ci.update_curve(x_min, x_max)
+    
+            
+    def _toggle_corr_factors(self):
+        self.use_default_corr_factors = not self.use_default_corr_factors
 
     def enable_ects_per_turn_calculation(self):
         if self.ui.chkEctsTurn.isChecked():
             self.ecpmt_just_enabled = True
 
     def _set_axis_autoscale(self):
         axis = self.ui.cbAxisCtrlSelect.currentIndex()
-        if axis < 3:
+        if axis < len(self.axes):   ##
             # Yn axis
             self.view_boxes[axis].enableAutoRange(
                 axis=self.view_boxes[axis].YAxis)
         else:
             # X axis
             self._reset_x()
 
@@ -813,34 +1261,34 @@
         self._chg_axis_scale(1.25)
 
     def _chg_axis_offs(self, offsfact):
         axis, amin, amax = self._get_axis_range()
         c = (amin+amax)/2
         d = (amax-amin)/2
         c += d*2*offsfact
-        if axis < 3:
+        if axis < len(self.axes):
             # Yn axis
             self.view_boxes[axis].setYRange(c-d, c+d, padding=0)
         else:
             # X axis
             self.view_boxes[0].setXRange(c-d, c+d, padding=0)
 
     def _chg_axis_scale(self, scalefact):
         axis, amin, amax = self._get_axis_range()
         c = (amin+amax)/2
         d = (amax-amin)/2*scalefact
-        if axis < 3:
+        if axis < len(self.axes):
             # Yn axis
             self.view_boxes[axis].setYRange(c-d, c+d, padding=0)
         else:
             # X axis
             self.view_boxes[0].setXRange(c-d, c+d, padding=0)
 
     def _get_axis_range(self):
         axis = self.ui.cbAxisCtrlSelect.currentIndex()
-        if axis < 3:
+        if axis < len(self.axes):
             # Yn axis
             [amin, amax] = self.view_boxes[axis].viewRange()[1]
         else:
             # X axis
             [amin, amax] = self.view_boxes[0].viewRange()[0]
         return axis, amin, amax
```

### Comparing `icepaposc-0.8.2/icepaposc.egg-info/PKG-INFO` & `icepaposc-0.9.0/icepaposc.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: icepaposc
-Version: 0.8.2
+Version: 0.9.0
 Summary: Python IcePAP Extension
 Home-page: https://github.com/ALBA-Synchrotron/IcepapOCS
 Author: Jarkko Inki and Roberto Homs-Puron
 Author-email: ctbeamlines@cells.es
 License: GPL
 Description:  Python application to monitor and tune IcePAP based 
         systems.
```

### Comparing `icepaposc-0.8.2/icepaposc.egg-info/SOURCES.txt` & `icepaposc-0.9.0/icepaposc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `icepaposc-0.8.2/setup.py` & `icepaposc-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from setuptools import find_packages
 
 # The version is updated automatically with bumpversion
 # Do not update manually
-__version = '0.8.2'
+__version = '0.9.0'
 
 # windows installer:
 # python setup.py bdist_wininst
 
 
 long_description = """ Python application to monitor and tune IcePAP based 
 systems. """
```

