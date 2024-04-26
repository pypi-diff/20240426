# Comparing `tmp/odhpy-0.0.9.tar.gz` & `tmp/odhpy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odhpy-0.0.9.tar", last modified: Wed Dec 14 05:40:54 2022, max compression
+gzip compressed data, was "odhpy-0.1.0.tar", last modified: Fri Apr 26 05:33:50 2024, max compression
```

## Comparing `odhpy-0.0.9.tar` & `odhpy-0.1.0.tar`

### file list

```diff
@@ -1,33 +1,55 @@
-drwxrwxrwx   0        0        0        0 2022-12-14 05:40:54.007897 odhpy-0.0.9/
--rw-rw-rw-   0        0        0     1448 2022-12-14 05:40:54.007897 odhpy-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      961 2022-12-11 06:47:55.000000 odhpy-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2022-12-14 05:40:54.007897 odhpy-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      740 2022-12-04 07:28:14.000000 odhpy-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-14 05:40:53.977632 odhpy-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2022-12-14 05:40:53.983612 odhpy-0.0.9/src/odhpy/
--rw-rw-rw-   0        0        0       73 2022-12-11 07:33:10.000000 odhpy-0.0.9/src/odhpy/__init__.py
--rw-rw-rw-   0        0        0      123 2022-12-11 07:25:35.000000 odhpy-0.0.9/src/odhpy/demo.py
-drwxrwxrwx   0        0        0        0 2022-12-14 05:40:53.995936 odhpy-0.0.9/src/odhpy/io/
--rw-rw-rw-   0        0        0       17 2022-12-13 06:20:10.000000 odhpy-0.0.9/src/odhpy/io/__init__.py
--rw-rw-rw-   0        0        0      983 2022-12-14 05:40:31.000000 odhpy-0.0.9/src/odhpy/io/io.py
-drwxrwxrwx   0        0        0        0 2022-12-14 05:40:53.998927 odhpy-0.0.9/src/odhpy/plots/
--rw-rw-rw-   0        0        0       30 2022-12-11 12:34:43.000000 odhpy-0.0.9/src/odhpy/plots/__init__.py
--rw-rw-rw-   0        0        0     1988 2022-12-12 12:31:36.000000 odhpy-0.0.9/src/odhpy/plots/plot_functions.py
--rw-rw-rw-   0        0        0        0 2022-12-12 22:38:32.000000 odhpy-0.0.9/src/odhpy/plots/plotly_helpers.py
-drwxrwxrwx   0        0        0        0 2022-12-14 05:40:54.001917 odhpy-0.0.9/src/odhpy/stoch/
--rw-rw-rw-   0        0        0       23 2022-12-14 04:17:45.000000 odhpy-0.0.9/src/odhpy/stoch/__init__.py
--rw-rw-rw-   0        0        0        0 2022-12-11 07:35:57.000000 odhpy-0.0.9/src/odhpy/stoch/analyse.py
--rw-rw-rw-   0        0        0     2867 2022-12-14 04:11:12.000000 odhpy-0.0.9/src/odhpy/stoch/generate.py
-drwxrwxrwx   0        0        0        0 2022-12-14 05:40:54.003910 odhpy-0.0.9/src/odhpy/trans/
--rw-rw-rw-   0        0        0       27 2022-12-08 21:34:03.000000 odhpy-0.0.9/src/odhpy/trans/__init__.py
--rw-rw-rw-   0        0        0     3237 2022-12-11 07:57:56.000000 odhpy-0.0.9/src/odhpy/trans/transformers.py
-drwxrwxrwx   0        0        0        0 2022-12-14 05:40:54.006900 odhpy-0.0.9/src/odhpy/utils/
--rw-rw-rw-   0        0        0       69 2022-12-13 04:10:17.000000 odhpy-0.0.9/src/odhpy/utils/__init__.py
--rw-rw-rw-   0        0        0     1475 2022-12-14 01:01:28.000000 odhpy-0.0.9/src/odhpy/utils/dataframe_functions.py
--rw-rw-rw-   0        0        0     1885 2022-12-11 07:43:28.000000 odhpy-0.0.9/src/odhpy/utils/datetime_functions.py
--rw-rw-rw-   0        0        0      205 2022-12-14 05:40:45.000000 odhpy-0.0.9/src/odhpy/version.py
-drwxrwxrwx   0        0        0        0 2022-12-14 05:40:53.993943 odhpy-0.0.9/src/odhpy.egg-info/
--rw-rw-rw-   0        0        0     1448 2022-12-14 05:40:53.000000 odhpy-0.0.9/src/odhpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      599 2022-12-14 05:40:53.000000 odhpy-0.0.9/src/odhpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-14 05:40:53.000000 odhpy-0.0.9/src/odhpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-12-14 05:40:53.000000 odhpy-0.0.9/src/odhpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.543233 odhpy-0.1.0/
+-rw-rw-rw-   0        0        0     2793 2024-04-26 05:33:50.542233 odhpy-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2175 2024-04-03 03:37:24.000000 odhpy-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 05:33:50.544233 odhpy-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      960 2024-03-19 03:03:09.000000 odhpy-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.502233 odhpy-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.511232 odhpy-0.1.0/src/odhpy/
+-rw-rw-rw-   0        0        0       76 2024-03-14 03:25:23.000000 odhpy-0.1.0/src/odhpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.517233 odhpy-0.1.0/src/odhpy/clim/
+-rw-rw-rw-   0        0        0       21 2024-03-14 03:25:23.000000 odhpy-0.1.0/src/odhpy/clim/__init__.py
+-rw-rw-rw-   0        0        0     6756 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/clim/clim.py
+-rw-rw-rw-   0        0        0      128 2024-03-14 03:25:23.000000 odhpy-0.1.0/src/odhpy/demo.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.523245 odhpy-0.1.0/src/odhpy/io/
+-rw-rw-rw-   0        0        0      128 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/io/__init__.py
+-rw-rw-rw-   0        0        0     4256 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/io/csv_io.py
+-rw-rw-rw-   0        0        0     2868 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/io/idx_io.py
+-rw-rw-rw-   0        0        0     6065 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/io/iqqm_out_reader.py
+-rw-rw-rw-   0        0        0     1705 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/io/lqn_io.py
+-rw-rw-rw-   0        0        0     3059 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/io/res_csv_io.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.525233 odhpy-0.1.0/src/odhpy/maps/
+-rw-rw-rw-   0        0        0       29 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/maps/__init__.py
+-rw-rw-rw-   0        0        0     5090 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/maps/station_maps.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.529233 odhpy-0.1.0/src/odhpy/plots/
+-rw-rw-rw-   0        0        0      121 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/plots/__init__.py
+-rw-rw-rw-   0        0        0    23149 2024-04-26 05:19:03.000000 odhpy-0.1.0/src/odhpy/plots/altair_plots.py
+-rw-rw-rw-   0        0        0      274 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/plots/node_diagrams.py
+-rw-rw-rw-   0        0        0     1988 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/plots/plot_functions.py
+-rw-rw-rw-   0        0        0        0 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/plots/plotly_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.532233 odhpy-0.1.0/src/odhpy/stats/
+-rw-rw-rw-   0        0        0      111 2024-03-18 23:58:54.000000 odhpy-0.1.0/src/odhpy/stats/__init__.py
+-rw-rw-rw-   0        0        0     2498 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/stats/aggregate_stats.py
+-rw-rw-rw-   0        0        0    12092 2024-04-03 03:37:24.000000 odhpy-0.1.0/src/odhpy/stats/reliability_stats_class.py
+-rw-rw-rw-   0        0        0     9163 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/stats/storage_level_assessment.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.534233 odhpy-0.1.0/src/odhpy/stats/swflo2s/
+-rw-rw-rw-   0        0        0       22 2024-04-03 03:37:24.000000 odhpy-0.1.0/src/odhpy/stats/swflo2s/__init__.py
+-rw-rw-rw-   0        0        0     6755 2024-04-03 03:37:24.000000 odhpy-0.1.0/src/odhpy/stats/swflo2s/swflo2s.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.536233 odhpy-0.1.0/src/odhpy/stoch/
+-rw-rw-rw-   0        0        0       23 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/stoch/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/stoch/analyse.py
+-rw-rw-rw-   0        0        0     2867 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/stoch/generate.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.538233 odhpy-0.1.0/src/odhpy/trans/
+-rw-rw-rw-   0        0        0       27 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/trans/__init__.py
+-rw-rw-rw-   0        0        0     2953 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/trans/transformers.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.542233 odhpy-0.1.0/src/odhpy/utils/
+-rw-rw-rw-   0        0        0       99 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/utils/__init__.py
+-rw-rw-rw-   0        0        0    11382 2024-04-03 03:37:24.000000 odhpy-0.1.0/src/odhpy/utils/dataframe_functions.py
+-rw-rw-rw-   0        0        0    10157 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/utils/datetime_functions.py
+-rw-rw-rw-   0        0        0      753 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/utils/interpolation.py
+-rw-rw-rw-   0        0        0      210 2024-04-26 05:24:30.000000 odhpy-0.1.0/src/odhpy/version.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.516232 odhpy-0.1.0/src/odhpy.egg-info/
+-rw-rw-rw-   0        0        0     2793 2024-04-26 05:33:50.000000 odhpy-0.1.0/src/odhpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2024-04-26 05:33:50.000000 odhpy-0.1.0/src/odhpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 05:33:50.000000 odhpy-0.1.0/src/odhpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-26 05:33:50.000000 odhpy-0.1.0/src/odhpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-26 05:33:50.000000 odhpy-0.1.0/src/odhpy.egg-info/top_level.txt
```

### Comparing `odhpy-0.0.9/PKG-INFO` & `odhpy-0.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,82 @@
-Metadata-Version: 2.1
-Name: odhpy
-Version: 0.0.9
-Summary: A collection of splashings to master that which has no form and count that which is uncountable.
-Home-page: https://bitbucket.org/odhydrology/odhpy.git
-Author: Chas Egan
-Author-email: chas@odhydrology.com
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # odhpy
 
 ## Installation
 
-This package may be installed using pip from Bitbucket (requires authentication), or directly from PyPi (public). These are both shown below.
+This package may be installed using pip from Bitbucket (requires authentication), or directly from PyPi (public), or from a .tar.gz. Examples are shown below.
 
 ```bash
 pip install git+https://bitbucket.org/odhydrology/odhpy.git
 ```
 
 ```bash
 pip install odhpy
 ```
 
+```bash
+pip install .\dist\odhpy-0.0.32.tar.gz
+```
+
 ## Usage
 
 ```python
 import odhpy
 
 # returns the package version
 odhpy.__version__
 
 # prints 'Hello world!' to the console
 odhpy.hello_world()
 ```
 
-## Uploading to PyPi
+## Build and Upload to PyPi
 
-First build a distribution from an anaconda prompt in the root of your project, and then upload the dist to PyPi using Twine. Twine will prompt you for your PyPi username and password.
+First build a distribution from an anaconda prompt in the root of your project, and then upload the dist to PyPi using Twine.
 
 ```bash
 python setup.py sdist
 ```
 
 ```bash
-twine upload dist/*
+twine upload dist\odhpy-0.0.32.tar.gz
 ```
 
+As of Nov 2023, PyPi uses an API token instead of a conventional password. You can still use Twine, but the username is "__token__", and password is the API token which is very long string starting with "pypi-". 
+
+``` bash
+username = __token__
+password = pypi-#####################################################################################
+```
+
+Where can I find the API token password? Chas has it in his emails. It is also here on the network at *.\ODH working files\Professional development, reading, etc\Software\ODHSoftware\ODHPy\PyPi_password_and_instructions.txt*.
+
+How do I make a new API token? Go to your PyPi account settings, and click on "API tokens". Then click on "Add API token", and give it a name. The token will be displayed on the next screen.
+
 ## Unit Tests
 
-Install the nose2 test-runner framework. Then from the root project folder run the nose2 module. This will automatically find and run tests in any modules named "test_*".
+WARNING: Run unit tests from an anaconda environment with compatable dependencies!
+
+Install the nose2 test-runner framework. 
 
 ```bash
 pip install nose2
 ```
 
+Then from the root project folder run the nose2 module. You can do this as a python modules, or just direcly from the anaconda prompt (both examples given below). This will automatically find and run tests in any modules named "test_*".
+
 ```bash
 python -m nose2
 ```
 
+```bash
+nose2
+```
+
+You can run specific tests by specifying the module name. Example below.
+
+```bash
+nose2 src.odhpy.stats.tests
+```
+
 ## License
 
 None.
```

### Comparing `odhpy-0.0.9/src/odhpy/plots/plot_functions.py` & `odhpy-0.1.0/src/odhpy/plots/plot_functions.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.0.9/src/odhpy/stoch/generate.py` & `odhpy-0.1.0/src/odhpy/stoch/generate.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.0.9/src/odhpy/trans/transformers.py` & `odhpy-0.1.0/src/odhpy/trans/transformers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 import pandas as pd
 from datetime import datetime, timedelta
 from odhpy import utils
 
 
-def join_on_dates(df1, df2):
+def join_on_dates(df1, df2, assert_format_standards=True):
     """_summary_
     Assumes df1 and df2 both have datetime indexes with values that are daily,
     and sequentially ascending.
 
     Args:
         df1 (_type_): _description_
         df2 (_type_): _description_
 
     Returns:
         _type_: _description_
     """
-    min_datetime = min(min(df1.index),min(df2.index)) 
-    max_datetime = max(max(df1.index),max(df2.index)) 
+    if assert_format_standards:
+        utils.assert_df_format_standards(df1)
+        utils.assert_df_format_standards(df2)
+    min_datetime = datetime.strptime(min(min(df1.index),min(df2.index)), r"%Y-%m-%d")
+    max_datetime = datetime.strptime(max(max(df1.index),max(df2.index)), r"%Y-%m-%d")
     ans_df = pd.DataFrame()
-    ans_df["Date"] = utils.get_dates(min_datetime, max_datetime)
+    ans_df["Date"] = utils.get_dates(min_datetime, max_datetime, str_format=r"%Y-%m-%d")
     ans_df.set_index("Date", inplace=True)
     ans_df = ans_df.join(df1, how='left')
     ans_df = ans_df.join(df2, how='left', lsuffix='_left', rsuffix='_right')
+    if assert_format_standards:
+        utils.assert_df_format_standards(ans_df)
     return ans_df
 
 
+
 def get_exceedence(obs_df, mod_df, plotting_position="cunnane") -> pd.DataFrame:
     """_summary_
 
     Args:
         obs_df (_type_): _description_
         mod_df (_type_): _description_
         plotting_position (str, optional): _description_. Defaults to "cunnane". Other supported values: "weibull", "gringorten". See https://glossary.ametsoc.org/wiki/Plotting_position
@@ -41,48 +47,37 @@
     """
     df = obs_df.join(mod_df, how='inner')
     df = df.dropna()
     df.columns = ['x', 'y']
     df.x = df.x.sort_values(ascending=False).values
     df.y = df.y.sort_values(ascending=False).values
     n = len(df)
-    index_starting_at_one = [i + 1 for i in range(n)]
-    if plotting_position == "cunnane":
-        df.index = [100 * (r - 0.4)/(n + 0.2) for r in index_starting_at_one]
-    elif plotting_position == "weibull":
-        df.index = [100 * (r/(n + 1)) for r in index_starting_at_one]
-    elif plotting_position == "gringorten":
-        df.index = [100 * (r - 0.44)/(n + 0.12) for r in index_starting_at_one]
-    else:
-        raise Exception(f"Plotting position not supported: {plotting_position}")
+    df.index = get_exceedence_plotting_position(n, plotting_position)
     return df
 
-def get_exceedence(obs_df, mod_df, plotting_position="cunnane") -> pd.DataFrame:
-    """_summary_
+
+
+def get_exceedence_plotting_position(length, plotting_position="cunnane"):
+    """Get plotting position values for a given length.
 
     Args:
-        obs_df (_type_): _description_
-        mod_df (_type_): _description_
         plotting_position (str, optional): _description_. Defaults to "cunnane". Other supported values: "weibull", "gringorten". See https://glossary.ametsoc.org/wiki/Plotting_position
 
     Raises:
-        Exception: _description_
+        Exception: If plotting position is not supported.
 
     Returns:
         _type_: _description_
     """
-    df = obs_df.join(mod_df, how='inner')
-    df = df.dropna()
-    df.columns = ['x', 'y']
-    df.x = df.x.sort_values(ascending=False).values
-    df.y = df.y.sort_values(ascending=False).values
-    n = len(df)
+    
+    n = length
+
     index_starting_at_one = [i + 1 for i in range(n)]
     if plotting_position == "cunnane":
-        df.index = [100 * (r - 0.4)/(n + 0.2) for r in index_starting_at_one]
+        plotting_points = [100 * (r - 0.4)/(n + 0.2) for r in index_starting_at_one]
     elif plotting_position == "weibull":
-        df.index = [100 * (r/(n + 1)) for r in index_starting_at_one]
+        plotting_points = [100 * (r/(n + 1)) for r in index_starting_at_one]
     elif plotting_position == "gringorten":
-        df.index = [100 * (r - 0.44)/(n + 0.12) for r in index_starting_at_one]
+        plotting_points = [100 * (r - 0.44)/(n + 0.12) for r in index_starting_at_one]
     else:
         raise Exception(f"Plotting position not supported: {plotting_position}")
-    return df
+    return plotting_points
```

