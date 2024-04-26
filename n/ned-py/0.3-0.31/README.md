# Comparing `tmp/ned-py-0.3.tar.gz` & `tmp/ned-py-0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ned-py-0.3.tar", last modified: Wed Apr 24 11:42:10 2024, max compression
+gzip compressed data, was "ned-py-0.31.tar", last modified: Fri Apr 26 05:38:07 2024, max compression
```

## Comparing `ned-py-0.3.tar` & `ned-py-0.31.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 meh       (1000) meh       (1000)        0 2024-04-24 11:42:10.007026 ned-py-0.3/
--rw-rw-r--   0 meh       (1000) meh       (1000)     1077 2024-04-03 08:32:56.000000 ned-py-0.3/LICENSE
--rw-r--r--   0 meh       (1000) meh       (1000)     1160 2024-04-24 11:42:10.007026 ned-py-0.3/PKG-INFO
--rw-rw-r--   0 meh       (1000) meh       (1000)     1540 2024-04-24 11:40:59.000000 ned-py-0.3/README.md
-drwxrwxr-x   0 meh       (1000) meh       (1000)        0 2024-04-24 11:42:10.007026 ned-py-0.3/ned/
--rw-rw-r--   0 meh       (1000) meh       (1000)       24 2024-04-03 09:12:28.000000 ned-py-0.3/ned/__init__.py
--rw-rw-r--   0 meh       (1000) meh       (1000)     5031 2024-04-24 11:40:59.000000 ned-py-0.3/ned/helper.py
--rw-rw-r--   0 meh       (1000) meh       (1000)     2151 2024-04-24 11:40:59.000000 ned-py-0.3/ned/metadata.py
--rw-rw-r--   0 meh       (1000) meh       (1000)    18445 2024-04-24 11:40:59.000000 ned-py-0.3/ned/ned.py
-drwxrwxr-x   0 meh       (1000) meh       (1000)        0 2024-04-24 11:42:10.007026 ned-py-0.3/ned_py.egg-info/
--rw-r--r--   0 meh       (1000) meh       (1000)     1160 2024-04-24 11:42:09.000000 ned-py-0.3/ned_py.egg-info/PKG-INFO
--rw-rw-r--   0 meh       (1000) meh       (1000)      268 2024-04-24 11:42:09.000000 ned-py-0.3/ned_py.egg-info/SOURCES.txt
--rw-rw-r--   0 meh       (1000) meh       (1000)        1 2024-04-24 11:42:09.000000 ned-py-0.3/ned_py.egg-info/dependency_links.txt
--rw-rw-r--   0 meh       (1000) meh       (1000)       54 2024-04-24 11:42:09.000000 ned-py-0.3/ned_py.egg-info/requires.txt
--rw-rw-r--   0 meh       (1000) meh       (1000)       10 2024-04-24 11:42:09.000000 ned-py-0.3/ned_py.egg-info/top_level.txt
--rw-rw-r--   0 meh       (1000) meh       (1000)       38 2024-04-24 11:42:10.007026 ned-py-0.3/setup.cfg
--rw-rw-r--   0 meh       (1000) meh       (1000)     1323 2024-04-24 11:40:59.000000 ned-py-0.3/setup.py
-drwxrwxr-x   0 meh       (1000) meh       (1000)        0 2024-04-24 11:42:10.007026 ned-py-0.3/tests/
--rw-rw-r--   0 meh       (1000) meh       (1000)       20 2024-04-06 08:58:23.000000 ned-py-0.3/tests/__init__.py
--rw-rw-r--   0 meh       (1000) meh       (1000)     4200 2024-04-24 11:40:59.000000 ned-py-0.3/tests/test_ned.py
+drwxrwxr-x   0 meh       (1000) meh       (1000)        0 2024-04-26 05:38:07.039226 ned-py-0.31/
+-rw-rw-r--   0 meh       (1000) meh       (1000)     1077 2024-04-03 08:32:56.000000 ned-py-0.31/LICENSE
+-rw-r--r--   0 meh       (1000) meh       (1000)     1161 2024-04-26 05:38:07.039226 ned-py-0.31/PKG-INFO
+-rw-rw-r--   0 meh       (1000) meh       (1000)     1557 2024-04-26 05:35:21.000000 ned-py-0.31/README.md
+drwxrwxr-x   0 meh       (1000) meh       (1000)        0 2024-04-26 05:38:07.039226 ned-py-0.31/ned/
+-rw-rw-r--   0 meh       (1000) meh       (1000)       24 2024-04-03 09:12:28.000000 ned-py-0.31/ned/__init__.py
+-rw-rw-r--   0 meh       (1000) meh       (1000)     5031 2024-04-24 11:40:59.000000 ned-py-0.31/ned/helper.py
+-rw-rw-r--   0 meh       (1000) meh       (1000)     2151 2024-04-24 11:40:59.000000 ned-py-0.31/ned/metadata.py
+-rw-rw-r--   0 meh       (1000) meh       (1000)    19198 2024-04-26 05:35:21.000000 ned-py-0.31/ned/ned.py
+drwxrwxr-x   0 meh       (1000) meh       (1000)        0 2024-04-26 05:38:07.039226 ned-py-0.31/ned_py.egg-info/
+-rw-r--r--   0 meh       (1000) meh       (1000)     1161 2024-04-26 05:38:06.000000 ned-py-0.31/ned_py.egg-info/PKG-INFO
+-rw-rw-r--   0 meh       (1000) meh       (1000)      268 2024-04-26 05:38:07.000000 ned-py-0.31/ned_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 meh       (1000) meh       (1000)        1 2024-04-26 05:38:06.000000 ned-py-0.31/ned_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 meh       (1000) meh       (1000)       54 2024-04-26 05:38:06.000000 ned-py-0.31/ned_py.egg-info/requires.txt
+-rw-rw-r--   0 meh       (1000) meh       (1000)       10 2024-04-26 05:38:06.000000 ned-py-0.31/ned_py.egg-info/top_level.txt
+-rw-rw-r--   0 meh       (1000) meh       (1000)       38 2024-04-26 05:38:07.039226 ned-py-0.31/setup.cfg
+-rw-rw-r--   0 meh       (1000) meh       (1000)     1324 2024-04-26 05:35:21.000000 ned-py-0.31/setup.py
+drwxrwxr-x   0 meh       (1000) meh       (1000)        0 2024-04-26 05:38:07.039226 ned-py-0.31/tests/
+-rw-rw-r--   0 meh       (1000) meh       (1000)       20 2024-04-06 08:58:23.000000 ned-py-0.31/tests/__init__.py
+-rw-rw-r--   0 meh       (1000) meh       (1000)     4661 2024-04-26 05:35:21.000000 ned-py-0.31/tests/test_ned.py
```

### Comparing `ned-py-0.3/LICENSE` & `ned-py-0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `ned-py-0.3/PKG-INFO` & `ned-py-0.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ned-py
-Version: 0.3
+Version: 0.31
 Summary: Python wrapper for Nationaal Energie Dashboard API.
 Home-page: https://github.com/profiteia/ned-py
 Author: Profiteia
 Author-email: victor@profiteia.io
 License: MIT
 Project-URL: Source, https://github.com/profiteia/ned-py
 Project-URL: Documentation, https://github.com/profiteia/ned-py
```

### Comparing `ned-py-0.3/README.md` & `ned-py-0.31/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 ```
 users()
 authorisations()
 
 get_forecast()
 get_consumption()
+get_production()
 get_production_provinces()
 get_production_offshore()
 get_production_netherlands()
 ```
 
 The API lacks clear documentation. Not all datapoints are available and backcast is not yet implemented. Checkout ned/helper.py for `is_valid_request` to see which requests are valid. 
 This package will be updated when more information becomes available.
```

### Comparing `ned-py-0.3/ned/helper.py` & `ned-py-0.31/ned/helper.py`

 * *Files identical despite different names*

### Comparing `ned-py-0.3/ned/metadata.py` & `ned-py-0.31/ned/metadata.py`

 * *Files identical despite different names*

### Comparing `ned-py-0.3/ned/ned.py` & `ned-py-0.31/ned/ned.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,15 @@
         try:
             if "hydra:member" in response.json():
                 response = response.json()["hydra:member"]
             else:
                 response = response.json()
         except JSONDecodeError:
             self.logger.error(f"Error decoding JSON response: {response.text}")
+            self.logger.info(f"For request: ", json.dumps(params, indent=4))
             return []
 
         # if response is not a list, check for errors
         if not isinstance(response, list) and "hydra:description" in response:
             self.logger.info(
                 f"{response['hydra:title']}: {response['hydra:description']}"
             )
@@ -461,14 +462,36 @@
             "Providing",
             start_date,
             end_date,
             granularitytimezone,
             types,
             points,
         )
+
+    # Generic function to get the production of all types and points
+    def get_production(
+        self,
+        granularity: str,
+        start_date: datetime,
+        end_date: Optional[datetime] = None,
+        granularitytimezone: str = "CET (Central European Time)",
+        types: Optional[List[str]] = list(NED_TYPES.keys()),
+        points: Optional[List[str]] = list(NED_POINTS.keys()),
+    ) -> Union[pd.DataFrame, List[dict]]:
+
+        return self.get_request(
+            granularity,
+            "Current",
+            "Providing",
+            start_date,
+            end_date,
+            granularitytimezone,
+            types,
+            points,
+        )
 
     def get_production_provinces(
         self,
         granularity: str,
         start_date: datetime,
         end_date: Optional[datetime] = None,
         granularitytimezone: str = "CET (Central European Time)",
```

### Comparing `ned-py-0.3/ned_py.egg-info/PKG-INFO` & `ned-py-0.31/ned_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ned-py
-Version: 0.3
+Version: 0.31
 Summary: Python wrapper for Nationaal Energie Dashboard API.
 Home-page: https://github.com/profiteia/ned-py
 Author: Profiteia
 Author-email: victor@profiteia.io
 License: MIT
 Project-URL: Source, https://github.com/profiteia/ned-py
 Project-URL: Documentation, https://github.com/profiteia/ned-py
```

### Comparing `ned-py-0.3/setup.py` & `ned-py-0.31/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ned-py",
-    version="0.3",
+    version="0.31",
     packages=find_packages(),
     description="Python wrapper for Nationaal Energie Dashboard API.",
     long_description="Receive and parse data from the Nationaal Energie Dashboard (ned.nl).",
     author="Profiteia",
     author_email="victor@profiteia.io",
     license="MIT",
     classifiers=[
```

### Comparing `ned-py-0.3/tests/test_ned.py` & `ned-py-0.31/tests/test_ned.py`

 * *Files 13% similar despite different names*

```diff
@@ -90,14 +90,32 @@
 def test_users_df():
     nedapi.as_dataframe = True
 
     result = nedapi.users()
     assert type(result) == pd.DataFrame and not result.empty
 
 
+def test_production():
+    nedapi.as_dataframe = False
+
+    result = nedapi.get_production(
+        "15 minutes", pd.Timestamp(2024, 1, 1), pd.Timestamp(2024, 1, 2)
+    )
+    assert type(result) == list and len(result) > 0
+
+
+def test_production_df():
+    nedapi.as_dataframe = True
+
+    result = nedapi.get_production(
+        "15 minutes", pd.Timestamp(2024, 1, 1), pd.Timestamp(2024, 1, 2)
+    )
+    assert type(result) == pd.DataFrame and not result.empty
+
+
 def test_production_netherlands():
     nedapi.as_dataframe = False
 
     result = nedapi.get_production_netherlands(
         "15 minutes", pd.Timestamp(2024, 1, 1), pd.Timestamp(2024, 1, 2)
     )
     assert type(result) == list and len(result) > 0
```

