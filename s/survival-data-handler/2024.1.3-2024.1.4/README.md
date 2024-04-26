# Comparing `tmp/survival_data_handler-2024.1.3.tar.gz` & `tmp/survival_data_handler-2024.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survival_data_handler-2024.1.3.tar", last modified: Wed Apr 24 08:54:36 2024, max compression
+gzip compressed data, was "survival_data_handler-2024.1.4.tar", last modified: Fri Apr 26 17:54:29 2024, max compression
```

## Comparing `survival_data_handler-2024.1.3.tar` & `survival_data_handler-2024.1.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:54:36.751077 survival_data_handler-2024.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-24 08:54:24.000000 survival_data_handler-2024.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-24 08:54:36.751077 survival_data_handler-2024.1.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2108 2024-04-24 08:54:24.000000 survival_data_handler-2024.1.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-24 08:54:24.000000 survival_data_handler-2024.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 08:54:24.000000 survival_data_handler-2024.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 08:54:36.751077 survival_data_handler-2024.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:54:36.747077 survival_data_handler-2024.1.3/survival_data_handler/
--rwxr-xr-x   0 runner    (1001) docker     (127)      762 2024-04-24 08:54:24.000000 survival_data_handler-2024.1.3/survival_data_handler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20382 2024-04-24 08:54:24.000000 survival_data_handler-2024.1.3/survival_data_handler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-24 08:54:24.000000 survival_data_handler-2024.1.3/survival_data_handler/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-24 08:54:24.000000 survival_data_handler-2024.1.3/survival_data_handler/plotting.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5573 2024-04-24 08:54:24.000000 survival_data_handler-2024.1.3/survival_data_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:54:36.751077 survival_data_handler-2024.1.3/survival_data_handler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-24 08:54:36.000000 survival_data_handler-2024.1.3/survival_data_handler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-24 08:54:36.000000 survival_data_handler-2024.1.3/survival_data_handler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:54:36.000000 survival_data_handler-2024.1.3/survival_data_handler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 08:54:36.000000 survival_data_handler-2024.1.3/survival_data_handler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 08:54:36.000000 survival_data_handler-2024.1.3/survival_data_handler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:54:36.747077 survival_data_handler-2024.1.3/test/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3872 2024-04-24 08:54:24.000000 survival_data_handler-2024.1.3/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:54:29.381084 survival_data_handler-2024.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-26 17:54:29.381084 survival_data_handler-2024.1.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2108 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 17:54:29.381084 survival_data_handler-2024.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:54:29.377084 survival_data_handler-2024.1.4/survival_data_handler/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      762 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/survival_data_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/survival_data_handler/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16777 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/survival_data_handler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/survival_data_handler/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/survival_data_handler/plotting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5863 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/survival_data_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:54:29.381084 survival_data_handler-2024.1.4/survival_data_handler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-26 17:54:29.000000 survival_data_handler-2024.1.4/survival_data_handler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-26 17:54:29.000000 survival_data_handler-2024.1.4/survival_data_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 17:54:29.000000 survival_data_handler-2024.1.4/survival_data_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-26 17:54:29.000000 survival_data_handler-2024.1.4/survival_data_handler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 17:54:29.000000 survival_data_handler-2024.1.4/survival_data_handler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:54:29.381084 survival_data_handler-2024.1.4/test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5496 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/test/test_main.py
```

### Comparing `survival_data_handler-2024.1.3/LICENSE` & `survival_data_handler-2024.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.1.3/PKG-INFO` & `survival_data_handler-2024.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: survival_data_handler
-Version: 2024.1.3
+Version: 2024.1.4
 Author-email: Vincent Laurent <vlaurent@eurobios.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3
 Requires-Dist: seaborn
 Requires-Dist: numba
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
 Requires-Dist: pandas>2
 Requires-Dist: lifelines
+Requires-Dist: numpy
 
 # Survival data handler
 ![code coverage](https://raw.githubusercontent.com/eurobios-mews-labs/survival-data-handler/coverage-badge/coverage.svg?raw=true)
 [![PyPI version](https://badge.fury.io/py/palma.svg)](https://badge.fury.io/py/palma)
 
 ```python
 import pandas as pd
```

### Comparing `survival_data_handler-2024.1.3/README.md` & `survival_data_handler-2024.1.4/README.md`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.1.3/survival_data_handler/__init__.py` & `survival_data_handler-2024.1.4/survival_data_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.1.3/survival_data_handler/metric.py` & `survival_data_handler-2024.1.4/survival_data_handler/metric.py`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.1.3/survival_data_handler/plotting.py` & `survival_data_handler-2024.1.4/survival_data_handler/plotting.py`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.1.3/survival_data_handler/utils.py` & `survival_data_handler-2024.1.4/survival_data_handler/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,20 +49,22 @@
     data.loc[crit_lines] = data_correct
     return data
 
 
 def compute_derivative(data: pd.DataFrame,
                        unit) -> pd.DataFrame:
     times = data.columns.to_numpy()
-    return data.T.diff().divide(
+    diff = data.T.diff()
+    return diff.divide(
         pd.Series(times, index=times).dt.total_seconds().diff() / unit,
         axis=0
     ).T
 
 
+
 def _cut(x):
     y = x.copy()
     for i in range(0, y.shape[1] - 1):
         y[:, i] = np.nanmin(y[:, :i + 1], axis=1)
     return y
 
 
@@ -102,22 +104,31 @@
     dt = 1.*np.ones((len(survival_estimate), 1), dtype=precision) * deltas.reshape(
         1, -1)
 
     surv_int = survival_estimate.__deepcopy__().astype(float)
 
     s_left = survival_estimate.iloc[:, 1:].values.astype(float)
     s_right = survival_estimate.iloc[:, :-1].values.astype(float)
+    t0 = survival_estimate.columns[0]
+    if "time" in str(dt.dtype):
+        dt = dt / np.timedelta64(1, 's')
+        t0 /= np.timedelta64(1, 's')
 
     surv_int.iloc[:, :-1] = (s_left + s_right) / 2.
     surv_int.iloc[:, :-1] *= dt
+    surv_int = surv_int.drop(surv_int.columns[-1], axis=1)
+
+    surv_int = pd.DataFrame(
+        np.cumsum(surv_int[np.sort(surv_int.columns)[::-1]], axis=1),
+        index=surv_int.index,
+        columns=surv_int.columns)
 
-    surv_int = surv_int[np.sort(surv_int.columns)[::-1]].cumsum(axis=1)
     ret = (surv_int / survival_estimate).astype(precision)
     ret[survival_estimate == 0] = 0
-    return ret - survival_estimate.columns[0]
+    return ret - t0
 
 
 class _PoolShift:
     def __init__(self, dates, starting_dates, data):
         self.dates = dates
         self.starting_dates = starting_dates.values
         self.starting_dates_index = starting_dates.index.to_numpy()
```

### Comparing `survival_data_handler-2024.1.3/survival_data_handler.egg-info/PKG-INFO` & `survival_data_handler-2024.1.4/survival_data_handler.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: survival_data_handler
-Version: 2024.1.3
+Version: 2024.1.4
 Author-email: Vincent Laurent <vlaurent@eurobios.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3
 Requires-Dist: seaborn
 Requires-Dist: numba
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
 Requires-Dist: pandas>2
 Requires-Dist: lifelines
+Requires-Dist: numpy
 
 # Survival data handler
 ![code coverage](https://raw.githubusercontent.com/eurobios-mews-labs/survival-data-handler/coverage-badge/coverage.svg?raw=true)
 [![PyPI version](https://badge.fury.io/py/palma.svg)](https://badge.fury.io/py/palma)
 
 ```python
 import pandas as pd
```

### Comparing `survival_data_handler-2024.1.3/test/test_main.py` & `survival_data_handler-2024.1.4/test/test_main.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 
 
 import pandas as pd
 import pytest
 from lifelines import CoxPHFitter
 from lifelines.datasets import load_rossi
 
-from survival_data_handler.main import SurvivalEstimation, Lifespan
+from survival_data_handler.main import SurvivalEstimation, Lifespan, TimeCurveData
 from survival_data_handler.utils import smooth, process_survival_function, \
     compute_derivative
+from survival_data_handler.base import TimeCurveInterpolation
 
 
 @pytest.fixture()
 def data():
     rossi = load_rossi()
     cph = CoxPHFitter()
     cph.fit(rossi, duration_col='week', event_col='arrest')
@@ -51,26 +52,29 @@
     ret = compute_derivative(curves, unit)
     assert all(pd.DataFrame(ret < 0))
 
 
 def test_survival_estimation(data):
     _, curves = data
     se = SurvivalEstimation(
-        curves.drop_duplicates(), unit='D',
+        curves.drop_duplicates(),
+        unit='D',
         n_unit=365.25)
     se.plot_residual_life()
-    # se.plot_residual_life(mean_behaviour=False)
+    se.plot_residual_life(mean_behaviour=False)
 
 
 def test_survival_estimation_attributes(data):
     rossi, curves = data
 
     rossi["index"] = rossi.index
     se = SurvivalEstimation(survival_curves=curves)
-    assert hasattr(se, "hazard_interp")
+    assert isinstance(se.hazard_function, TimeCurveData)
+    assert isinstance(se.survival_function, TimeCurveData)
+    assert isinstance(se.cumulative_hazard_function, TimeCurveData)
 
 
 def test_lifespan(data):
     rossi, curves = data
 
     age = pd.to_timedelta(rossi["age"] * 365.25, unit="D")
     birth = pd.to_datetime('2000')
@@ -108,10 +112,47 @@
         curves,
         index=rossi["index"],
         birth=birth,
         age=age,
         window=(pd.to_datetime("2000"), pd.to_datetime("2001"))
     )
     lifespan.add_supervision(durations=rossi["duration"] + birth, event=rossi["arrest"])
-    lifespan.plot_tagged_sample(lifespan.survival_function, )
+
     lifespan.compute_confusion_matrix(on="survival_function", threshold=0.2)
-    test_is_survival_curves(lifespan.survival_function)
+    lifespan.plot_average_tagged(on="survival_function")
+    lifespan.plot_average_tagged(on="survival_function", plot_test_window=True, plot_type=None)
+    lifespan.plot_dist_facet_grid(on="survival_function")
+    lifespan.plot_tagged_sample(on="survival_function", n_sample=10)
+    lifespan.plot_tagged_sample(on="survival_function", n_sample_pos=10)
+    lifespan.plot_tagged_sample(on="survival_function")
+    test_is_survival_curves(lifespan.survival_function.round(3))
+
+
+def test_curve_object(data):
+    rossi, curves = data
+    tc = TimeCurveData(curves)
+    tc_prime = tc.derivative()
+    assert isinstance(tc_prime, TimeCurveData)
+    assert isinstance((-tc_prime), TimeCurveData)
+    assert isinstance((tc_prime / tc), TimeCurveData)
+    assert isinstance((tc_prime.exp() / tc), TimeCurveData)
+    assert isinstance((tc_prime.log() - tc), TimeCurveData)
+    assert isinstance((tc_prime.exp() + tc), TimeCurveData)
+
+
+def test_interpolation_curves(data):
+    rossi, curves = data
+    rossi["duration"] = pd.to_timedelta(rossi["week"]*7, unit="D")
+    rossi["birth"] = pd.to_datetime('2000')
+    rossi["index"] = rossi.index
+
+    tc = TimeCurveData(curves)
+    tc_prime = tc.interpolation
+
+    ti = TimeCurveInterpolation(
+        tc_prime,
+        index=rossi["index"],
+        birth=rossi["birth"],
+        period=pd.to_timedelta(30, "D"),
+        window=(pd.to_datetime("2000"), pd.to_datetime("2001")))
+    assert isinstance(ti.unique_curve, TimeCurveData)
+    assert isinstance(ti.curve, TimeCurveData)
```

