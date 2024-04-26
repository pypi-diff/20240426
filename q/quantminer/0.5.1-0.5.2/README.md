# Comparing `tmp/quantminer-0.5.1.tar.gz` & `tmp/quantminer-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantminer-0.5.1.tar", last modified: Wed Apr 24 08:50:33 2024, max compression
+gzip compressed data, was "quantminer-0.5.2.tar", last modified: Fri Apr 26 16:34:48 2024, max compression
```

## Comparing `quantminer-0.5.1.tar` & `quantminer-0.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-24 08:50:33.984829 quantminer-0.5.1/
--rw-r--r--   0 jerryinyang   (501) staff       (20)     3835 2024-04-24 08:50:33.984612 quantminer-0.5.1/PKG-INFO
--rw-r--r--   0 jerryinyang   (501) staff       (20)      258 2024-04-10 10:17:30.000000 quantminer-0.5.1/pyproject.toml
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-24 08:50:33.982423 quantminer-0.5.1/quantminer/
--rw-r--r--   0 jerryinyang   (501) staff       (20)       34 2024-04-10 11:41:22.000000 quantminer-0.5.1/quantminer/__init__.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)     6014 2024-04-24 01:58:38.000000 quantminer-0.5.1/quantminer/_test_transform.py
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-24 08:50:33.983822 quantminer-0.5.1/quantminer/classes/
--rw-r--r--   0 jerryinyang   (501) staff       (20)      126 2024-04-24 01:07:11.000000 quantminer-0.5.1/quantminer/classes/__init__.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)    11263 2024-04-24 02:32:15.000000 quantminer-0.5.1/quantminer/classes/reducers.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)    13017 2024-04-10 04:48:20.000000 quantminer-0.5.1/quantminer/classes/seqkmeans.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)    24480 2024-04-24 02:36:57.000000 quantminer-0.5.1/quantminer/pipminer.py
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-24 08:50:33.984159 quantminer-0.5.1/quantminer.egg-info/
--rw-r--r--   0 jerryinyang   (501) staff       (20)     3835 2024-04-24 08:50:33.000000 quantminer-0.5.1/quantminer.egg-info/PKG-INFO
--rw-r--r--   0 jerryinyang   (501) staff       (20)      362 2024-04-24 08:50:33.000000 quantminer-0.5.1/quantminer.egg-info/SOURCES.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)        1 2024-04-24 08:50:33.000000 quantminer-0.5.1/quantminer.egg-info/dependency_links.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)     1958 2024-04-24 08:50:33.000000 quantminer-0.5.1/quantminer.egg-info/requires.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       11 2024-04-24 08:50:33.000000 quantminer-0.5.1/quantminer.egg-info/top_level.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       38 2024-04-24 08:50:33.984870 quantminer-0.5.1/setup.cfg
--rw-r--r--   0 jerryinyang   (501) staff       (20)      594 2024-04-24 08:49:54.000000 quantminer-0.5.1/setup.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-26 16:34:48.903538 quantminer-0.5.2/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      410 2024-04-26 16:34:48.903311 quantminer-0.5.2/PKG-INFO
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      258 2024-04-10 10:17:30.000000 quantminer-0.5.2/pyproject.toml
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-26 16:34:48.901792 quantminer-0.5.2/quantminer/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       34 2024-04-10 11:41:22.000000 quantminer-0.5.2/quantminer/__init__.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)     6014 2024-04-24 01:58:38.000000 quantminer-0.5.2/quantminer/_test_transform.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-26 16:34:48.902904 quantminer-0.5.2/quantminer/classes/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      126 2024-04-26 16:33:55.000000 quantminer-0.5.2/quantminer/classes/__init__.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)    11263 2024-04-24 02:32:15.000000 quantminer-0.5.2/quantminer/classes/reducers.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)    13017 2024-04-10 04:48:20.000000 quantminer-0.5.2/quantminer/classes/seqkmeans.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)    26534 2024-04-26 16:34:38.000000 quantminer-0.5.2/quantminer/pipminer.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-26 16:34:48.903095 quantminer-0.5.2/quantminer.egg-info/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      410 2024-04-26 16:34:48.000000 quantminer-0.5.2/quantminer.egg-info/PKG-INFO
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      362 2024-04-26 16:34:48.000000 quantminer-0.5.2/quantminer.egg-info/SOURCES.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)        1 2024-04-26 16:34:48.000000 quantminer-0.5.2/quantminer.egg-info/dependency_links.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       93 2024-04-26 16:34:48.000000 quantminer-0.5.2/quantminer.egg-info/requires.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       11 2024-04-26 16:34:48.000000 quantminer-0.5.2/quantminer.egg-info/top_level.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       38 2024-04-26 16:34:48.903583 quantminer-0.5.2/setup.cfg
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      594 2024-04-26 16:33:51.000000 quantminer-0.5.2/setup.py
```

### Comparing `quantminer-0.5.1/quantminer/_test_transform.py` & `quantminer-0.5.2/quantminer/_test_transform.py`

 * *Files identical despite different names*

### Comparing `quantminer-0.5.1/quantminer/classes/reducers.py` & `quantminer-0.5.2/quantminer/classes/reducers.py`

 * *Files identical despite different names*

### Comparing `quantminer-0.5.1/quantminer/classes/seqkmeans.py` & `quantminer-0.5.2/quantminer/classes/seqkmeans.py`

 * *Files identical despite different names*

### Comparing `quantminer-0.5.1/quantminer/pipminer.py` & `quantminer-0.5.2/quantminer/pipminer.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,22 +25,24 @@
                  n_pivots: int, 
                  n_clusters: int = 8,
                  hold_period: int = 6,
                  model_type:Literal['standard', 'ts', 'sequential']='standard',
                  reducer:Literal['FFT', 'PIP', 'Wavelet', 'FFTWavelet']='PIP',
                  verbose = False,
                  wavelet:Literal['db1', 'db2', 'db3', 'db4', 'coif1', 'haar', 'sym5', 'bior3.5']='coif2',
+                 cluster_selection_mode:Literal['best', 'baseline']='best',
                  ) -> None:
             
         self.n_lookback = n_lookback
         self.n_pivots = n_pivots
         self.hold_period = hold_period
         self.n_cluster = n_clusters
 
         self._model_type = model_type
+        self._cluster_selection_mode = cluster_selection_mode
 
         # Store Training Data
         self._data: List = []
         self._price_data = []
         self._data_train_X: Union[List, np.ndarray] = []
         self._data_train_y: Union[List, np.ndarray] = []
 
@@ -489,18 +491,27 @@
         Assess each cluster's performance, and selected the best performing clusters
         """
         self._cluster_labels_long.clear()
         self._cluster_labels_short.clear()
 
         # Store the cluster scores from each data
         cluster_scores = []
+        baseline_long = []
+        baseline_short = []
 
         # Compute the returns
         _returns = np.diff(self._price_data, prepend=self._price_data[0])
 
+        # Baseline Metrics
+        baseline_returns = pd.Series(_returns)
+        baseline_profit_factor = max(qt.stats.profit_factor(baseline_returns), 0)
+        baseline_sharpe_ratio = max(qt.stats.sharpe(baseline_returns), 0)
+        baseline_upi = max(qt.stats.ulcer_performance_index(baseline_returns), 1)
+        baseline_max_dd = qt.stats.max_drawdown(baseline_returns) 
+
         # Get the cluster labels
         _labels = self._cluster_labels
 
         # Iterate through each cluster label
         for _label in range(self.n_cluster):
 
             # Create a mask for the label in the labels; everything else should be zero
@@ -509,20 +520,54 @@
             # Filter the labels
             _signals = mask_label.astype(int)
 
             # Implement Holding Period
             _signals = self.__apply_holding_period(_signals)
 
             # Get the returns, compute martin score
-            _ret = _signals * _returns
-            cluster_scores.append(self.__compute_martin(_ret))
+            _returns = _signals * _returns
+            _martin = self.__compute_martin(_returns)
+
+            if (_martin is np.inf) or np.isnan(_martin):
+                cluster_scores.append(0)
+            else:
+                cluster_scores.append(_martin)
+                
+            if self._cluster_selection_mode == 'baseline':
+                for direction in [1, -1]:                
+                    # Compute the returns
+                    _ret = pd.Series(_returns * direction)
+
+                    # Compute the kpis
+                    _pf = qt.stats.profit_factor(_ret)
+                    _sharpe = qt.stats.rolling_sharpe(_ret).mean()
+                    _upi = qt.stats.ulcer_performance_index(_ret)
+                    _max_dd = qt.stats.to_drawdown_series(_ret).mean()
+
+                    if (_upi is np.inf) or np.isnan(_upi):
+                        continue
+
+                    if ((_pf > baseline_profit_factor) and
+                        (_sharpe > baseline_sharpe_ratio) and
+                        (_upi > baseline_upi) and 
+                        (_max_dd > baseline_max_dd)):
+                
+                        if direction > 0:
+                            baseline_long.append(_label)
+                        else:
+                            baseline_short.append(_label)
 
         # Append the selected cluster labels
-        self._cluster_labels_long.append(np.argmax(cluster_scores))
-        self._cluster_labels_short.append(np.argmin(cluster_scores))
+        if self._cluster_selection_mode == 'baseline':
+            self._cluster_labels_long = baseline_long
+            self._cluster_labels_short = baseline_short
+
+        else:
+            self._cluster_labels_long.append(np.argmax(cluster_scores))
+            self._cluster_labels_short.append(np.argmin(cluster_scores))
 
 
     def _compute_performance(self):
         """
         Test the performance of the selected clusters
         """
 
@@ -744,24 +789,24 @@
     train_data = train_data["close"].dropna(axis=0)
     train_data = train_data.to_numpy()
 
     test_data = test_data["close"].dropna(axis=0)
     test_data = test_data.to_numpy()
 
 
-    miner = Miner(25, 10, reducer="Wavelet", wavelet='haar')
+    miner = Miner(25, 4, 16, 3, cluster_selection_mode='')
 
     # print('Successful')
     # miner.fit(np.diff(train_data, prepend=train_data[0]-1), train_data)
     # print(miner.test(np.diff(test_data, prepend=test_data[0]-1), test_data))
 
-    # miner.fit(train_data)
-    miner.fit(np.diff(train_data, prepend=train_data[0]-1), train_data)
+    miner.fit(train_data)
+    # miner.fit(np.diff(train_data, prepend=train_data[0]-1), train_data)
+    print(miner._cluster_labels_long)
+    print(miner._cluster_labels_short)
 
     # miner.save_model(parent_path / 'pipminer.pkl')
-
     # miner : Miner = Miner.load_model(parent_path / 'pipminer.pkl')
-
     # print(miner.transform(test_data))
 
-    # print(miner.test(test_data))
-    print(miner.test(np.diff(test_data, prepend=test_data[0]-1), test_data))
+    # print(miner.test(train_data))
+    # print(miner.test(np.diff(test_data, prepend=test_data[0]-1), test_data))
```

### Comparing `quantminer-0.5.1/setup.py` & `quantminer-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 # Function to read the requirements from the requirements.txt file
 def read_requirements():
     with open('requirements.txt', 'r') as f:
         return [line.strip() for line in f if line.strip()]
 
 setup(
     name='quantminer',
-    version='0.5.1',
+    version='0.5.2',
     description='Data/Pattern Mining Algorithms for Financial Data',
     author='Jerry Inyang',
     author_email='jerprog0@gmail.com',
     packages=find_packages(),  # Automatically finds your package
     install_requires=read_requirements()  # Reads requirements dynamically from requirements.txt
 )
```

