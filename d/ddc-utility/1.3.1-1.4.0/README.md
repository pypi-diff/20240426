# Comparing `tmp/ddc-utility-1.3.1.tar.gz` & `tmp/ddc_utility-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/marton/Dev/ddc-utility/dist/.tmp-r8qm7sob/ddc-utility-1.3.1.tar", last modified: Mon Dec  4 16:03:54 2023, max compression
+gzip compressed data, was "ddc_utility-1.4.0.tar", last modified: Fri Apr 26 13:39:21 2024, max compression
```

## Comparing `ddc-utility-1.3.1.tar` & `ddc_utility-1.4.0.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxrwxr-x   0 marton    (1000) marton    (1000)        0 2023-12-04 16:03:54.882750 ddc-utility-1.3.1/
--rw-rw-r--   0 marton    (1000) marton    (1000)     1086 2023-09-13 06:12:48.000000 ddc-utility-1.3.1/LICENSE
--rw-r--r--   0 marton    (1000) marton    (1000)     1740 2023-12-04 16:03:54.882750 ddc-utility-1.3.1/PKG-INFO
--rw-rw-r--   0 marton    (1000) marton    (1000)     1020 2023-09-13 06:09:23.000000 ddc-utility-1.3.1/README.md
-drwxrwxr-x   0 marton    (1000) marton    (1000)        0 2023-12-04 16:03:54.882750 ddc-utility-1.3.1/ddc_utility/
--rw-rw-r--   0 marton    (1000) marton    (1000)        1 2023-09-13 06:09:23.000000 ddc-utility-1.3.1/ddc_utility/__init__.py
--rw-rw-r--   0 marton    (1000) marton    (1000)       18 2023-12-04 16:01:41.000000 ddc-utility-1.3.1/ddc_utility/__version__.py
--rw-rw-r--   0 marton    (1000) marton    (1000)      412 2023-09-13 06:09:23.000000 ddc-utility-1.3.1/ddc_utility/auth.py
--rw-rw-r--   0 marton    (1000) marton    (1000)    33170 2023-12-04 16:01:41.000000 ddc-utility-1.3.1/ddc_utility/client.py
--rw-rw-r--   0 marton    (1000) marton    (1000)      141 2023-09-13 06:09:23.000000 ddc-utility-1.3.1/ddc_utility/constants.py
--rw-rw-r--   0 marton    (1000) marton    (1000)      412 2023-12-04 16:01:41.000000 ddc-utility-1.3.1/ddc_utility/cube.py
--rw-rw-r--   0 marton    (1000) marton    (1000)     2379 2023-09-13 06:09:23.000000 ddc-utility-1.3.1/ddc_utility/data_collections.py
--rw-rw-r--   0 marton    (1000) marton    (1000)     3187 2023-09-13 06:09:23.000000 ddc-utility-1.3.1/ddc_utility/errors.py
--rw-rw-r--   0 marton    (1000) marton    (1000)     6283 2023-12-04 16:01:41.000000 ddc-utility-1.3.1/ddc_utility/fs.py
--rw-rw-r--   0 marton    (1000) marton    (1000)    10441 2023-09-13 06:09:23.000000 ddc-utility-1.3.1/ddc_utility/metadata.py
--rw-rw-r--   0 marton    (1000) marton    (1000)     2925 2023-12-04 16:01:41.000000 ddc-utility-1.3.1/ddc_utility/store.py
--rw-rw-r--   0 marton    (1000) marton    (1000)    10799 2023-09-13 06:09:23.000000 ddc-utility-1.3.1/ddc_utility/utils.py
-drwxrwxr-x   0 marton    (1000) marton    (1000)        0 2023-12-04 16:03:54.882750 ddc-utility-1.3.1/ddc_utility.egg-info/
--rw-r--r--   0 marton    (1000) marton    (1000)     1740 2023-12-04 16:03:54.000000 ddc-utility-1.3.1/ddc_utility.egg-info/PKG-INFO
--rw-rw-r--   0 marton    (1000) marton    (1000)      504 2023-12-04 16:03:54.000000 ddc-utility-1.3.1/ddc_utility.egg-info/SOURCES.txt
--rw-rw-r--   0 marton    (1000) marton    (1000)        1 2023-12-04 16:03:54.000000 ddc-utility-1.3.1/ddc_utility.egg-info/dependency_links.txt
--rw-rw-r--   0 marton    (1000) marton    (1000)      150 2023-12-04 16:03:54.000000 ddc-utility-1.3.1/ddc_utility.egg-info/requires.txt
--rw-rw-r--   0 marton    (1000) marton    (1000)       12 2023-12-04 16:03:54.000000 ddc-utility-1.3.1/ddc_utility.egg-info/top_level.txt
--rw-rw-r--   0 marton    (1000) marton    (1000)      838 2023-12-04 16:01:41.000000 ddc-utility-1.3.1/pyproject.toml
--rw-rw-r--   0 marton    (1000) marton    (1000)       38 2023-12-04 16:03:54.882750 ddc-utility-1.3.1/setup.cfg
-drwxrwxr-x   0 marton    (1000) marton    (1000)        0 2023-12-04 16:03:54.882750 ddc-utility-1.3.1/test/
--rw-rw-r--   0 marton    (1000) marton    (1000)     2502 2023-09-13 06:09:23.000000 ddc-utility-1.3.1/test/test_metadata.py
+drwxr-xr-x   0 martontolnai   (501) staff       (20)        0 2024-04-26 13:39:21.037793 ddc_utility-1.4.0/
+-rw-r--r--   0 martontolnai   (501) staff       (20)     1086 2024-01-30 13:13:49.000000 ddc_utility-1.4.0/LICENSE
+-rw-r--r--   0 martontolnai   (501) staff       (20)     1783 2024-04-26 13:39:21.037613 ddc_utility-1.4.0/PKG-INFO
+-rw-r--r--   0 martontolnai   (501) staff       (20)     1020 2024-01-30 13:13:49.000000 ddc_utility-1.4.0/README.md
+drwxr-xr-x   0 martontolnai   (501) staff       (20)        0 2024-04-26 13:39:21.033424 ddc_utility-1.4.0/ddc_utility/
+-rw-r--r--   0 martontolnai   (501) staff       (20)        1 2024-01-30 13:13:49.000000 ddc_utility-1.4.0/ddc_utility/__init__.py
+-rw-r--r--   0 martontolnai   (501) staff       (20)       18 2024-04-23 13:40:08.000000 ddc_utility-1.4.0/ddc_utility/__version__.py
+-rw-r--r--   0 martontolnai   (501) staff       (20)      412 2024-01-30 13:13:49.000000 ddc_utility-1.4.0/ddc_utility/auth.py
+-rw-r--r--   0 martontolnai   (501) staff       (20)    34570 2024-04-26 09:50:35.000000 ddc_utility-1.4.0/ddc_utility/client.py
+-rw-r--r--   0 martontolnai   (501) staff       (20)      141 2024-01-30 13:13:49.000000 ddc_utility-1.4.0/ddc_utility/constants.py
+-rw-r--r--   0 martontolnai   (501) staff       (20)      387 2024-04-23 13:40:08.000000 ddc_utility-1.4.0/ddc_utility/cube.py
+-rw-r--r--   0 martontolnai   (501) staff       (20)     2379 2024-01-30 13:13:49.000000 ddc_utility-1.4.0/ddc_utility/data_collections.py
+-rw-r--r--   0 martontolnai   (501) staff       (20)     3188 2024-04-23 13:40:08.000000 ddc_utility-1.4.0/ddc_utility/errors.py
+-rw-r--r--   0 martontolnai   (501) staff       (20)    10441 2024-01-30 13:13:49.000000 ddc_utility-1.4.0/ddc_utility/metadata.py
+-rw-r--r--   0 martontolnai   (501) staff       (20)    10799 2024-01-30 13:13:49.000000 ddc_utility-1.4.0/ddc_utility/utils.py
+drwxr-xr-x   0 martontolnai   (501) staff       (20)        0 2024-04-26 13:39:21.037124 ddc_utility-1.4.0/ddc_utility.egg-info/
+-rw-r--r--   0 martontolnai   (501) staff       (20)     1783 2024-04-26 13:39:21.000000 ddc_utility-1.4.0/ddc_utility.egg-info/PKG-INFO
+-rw-r--r--   0 martontolnai   (501) staff       (20)      465 2024-04-26 13:39:21.000000 ddc_utility-1.4.0/ddc_utility.egg-info/SOURCES.txt
+-rw-r--r--   0 martontolnai   (501) staff       (20)        1 2024-04-26 13:39:21.000000 ddc_utility-1.4.0/ddc_utility.egg-info/dependency_links.txt
+-rw-r--r--   0 martontolnai   (501) staff       (20)      163 2024-04-26 13:39:21.000000 ddc_utility-1.4.0/ddc_utility.egg-info/requires.txt
+-rw-r--r--   0 martontolnai   (501) staff       (20)       12 2024-04-26 13:39:21.000000 ddc_utility-1.4.0/ddc_utility.egg-info/top_level.txt
+-rw-r--r--   0 martontolnai   (501) staff       (20)      866 2024-04-26 13:38:59.000000 ddc_utility-1.4.0/pyproject.toml
+-rw-r--r--   0 martontolnai   (501) staff       (20)       38 2024-04-26 13:39:21.037952 ddc_utility-1.4.0/setup.cfg
+drwxr-xr-x   0 martontolnai   (501) staff       (20)        0 2024-04-26 13:39:21.035560 ddc_utility-1.4.0/test/
+-rw-r--r--   0 martontolnai   (501) staff       (20)     2502 2024-01-30 13:13:49.000000 ddc_utility-1.4.0/test/test_metadata.py
```

### Comparing `ddc-utility-1.3.1/LICENSE` & `ddc_utility-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ddc-utility-1.3.1/PKG-INFO` & `ddc_utility-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddc-utility
-Version: 1.3.1
+Version: 1.4.0
 Summary: Package for retrieving DDC datasests
 Author-email: Balint Alfoldy <alfibalint@gmail.com>, CropOM <marton.tolnai@cropom.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -15,14 +15,16 @@
 Requires-Dist: numcodecs>=0.11.0
 Requires-Dist: pydantic>=1.10.0
 Requires-Dist: pyproj>=3.4.1
 Requires-Dist: requests>=2.28.2
 Requires-Dist: xarray>=2023.1.0
 Requires-Dist: zarr>=2.13.6
 Requires-Dist: fsspec
+Requires-Dist: s3fs
+Requires-Dist: shapely
 
 # DDC Utility
 
 This is the Danube Data Cube Utility library, for retrieving data from the Danube Data Cube portal.
 
 ### Installation
```

### Comparing `ddc-utility-1.3.1/README.md` & `ddc_utility-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ddc-utility-1.3.1/ddc_utility/client.py` & `ddc_utility-1.4.0/ddc_utility/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -193,26 +193,26 @@
         self.auth = None
         self.aws_s3 = None
         self.aws_session_exp = 0
         
         super().__init__(client_id, client_secret, host, False)
 
     @authorize_request
-    def get_all_aoi(self, with_geometry: bool = True, desired_type: int = 1) -> Union[pd.DataFrame, List[Dict]]:
+    def get_all_aoi(self, with_geometry: bool = True, output_data_type: int = 1) -> Union[pd.DataFrame, List[Dict]]:
         """
         Get user's all area of interests (AOI).
 
         Args:
             with_geometry (bool, optional): Whether to retrive geometry values.
                 Defaults to True.
-            desired_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as list of dictionaries (2).
+            output_data_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as list of dictionaries (2).
                 Defaults to 1.
 
         Returns:
-            Union[pd.DataFrame, List[Dict]]: Depending on the `desired_type` parameter,
+            Union[pd.DataFrame, List[Dict]]: Depending on the `output_data_type` parameter,
             this function returns either a pandas DataFrame or a list of dictionary containing AOI information.
 
         Raises:
             DdcRequestError: If an error occurs during the process of requesting AOIs.
         """
 
         params = {'user_id': self.client_id,
@@ -226,28 +226,28 @@
                 "GET", route, params=params, auth=self.auth, accept=accept)
 
         except HTTPException as error:
             raise DdcRequestError(
                 f"Error during getting all aoi with params {params} from {route}"
             ) from error
 
-        return self._process_response(response, desired_type)
+        return self._process_response(response, output_data_type)
 
     @authorize_request
-    def get_aoi_by_id(self, aoi_id: int, desired_type: int = 1) -> Union[pd.DataFrame, Dict]:
+    def get_aoi_by_id(self, aoi_id: int, output_data_type: int = 1) -> Union[pd.DataFrame, Dict]:
         """
         Get user's area of interests (AOI) by ID.
 
         Args:
             aoi_id (int): ID of the AOI.
-            desired_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as a dictionary(2).
+            output_data_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as a dictionary(2).
                 Defaults to 1.
 
         Returns:
-            Union[pd.DataFrame, Dict]: Depending on the `desired_type` parameter,
+            Union[pd.DataFrame, Dict]: Depending on the `output_data_type` parameter,
             this function returns either a pandas DataFrame or a dictionary containing AOI information.
 
         Raises:
             DdcRequestError: If an error occurs during the process of requesting the AOI.
         """
 
         params = {'user_id': self.client_id,
@@ -261,24 +261,26 @@
                 "GET", route, params=params, auth=self.auth, accept=accept)
 
         except HTTPException as error:
             raise DdcRequestError(
                 f"Error during getting all aoi with params {params} from {route}"
             ) from error
 
-        return self._process_response(response, desired_type)
+        return self._process_response(response, output_data_type)
 
     @authorize_request
     def create_aoi(self,
                    name: str,
                    geometry: Union[Geometry, Polygon, MultiPolygon, str],
                    time_range: Union[TimeRange, Tuple[pd.Timestamp, pd.Timestamp], Tuple[str, str]],
                    data_layers: Union[List[DataCollection], List[Dict]] = None,
+                   layer_selection_id:  int = None,
+                   layer_ids: List[int] = [],
                    is_dynamic: bool = False,
-                   desired_type: int = 1
+                   output_data_type: int = 1
                    ) -> Union[pd.DataFrame, Dict]:
         """
         Create an area of interests (AOI).
 
         Args:
             name (str): The name of the area of interest.
             geometry (Union[Geometry, Polygon, MultiPolygon, str]): The geometry of the area of interest.
@@ -292,21 +294,23 @@
                 Example:
                     [
                         {'name': 'S2L2A', 'bands': ['B04', 'B08']},
                         {'name': 'Meteorology', 'bands': ['Temp Avg', 'Prec']}
                     ]
                 If None, the AOI cube will be created with an empty polygon.
                 Defaults to None.
+            layer_selection_id (int): Layer selection ID. 
+            layer_ids (List[int]): List of layer IDs.
             is_dynamic (bool, optional): Whether the AOI is dynamic (True) or static (False).
                 Defaults to False.
-            desired_type (int, optional): Whether to return the result as a `pandas.DataFrame` (1) or as a dictionary (2).
+            output_data_type (int, optional): Whether to return the result as a `pandas.DataFrame` (1) or as a dictionary (2).
                 Defaults to 1.
 
         Returns:
-            Union[pd.DataFrame, Dict]: Depending on the `desired_type` parameter,
+            Union[pd.DataFrame, Dict]: Depending on the `output_data_type` parameter,
             this function returns either a pandas DataFrame or a dictionary containing AOI information.
 
         Raises:
             DdcRequestError: If an error occurs during the process of creating the AOI.
 
         """
         if not isinstance(time_range, TimeRange):
@@ -330,44 +334,79 @@
 
         json_data = {
             "user_id": self.client_id,
             "name": name,
             "geometry": geometry_str,
             "start_date": time_range_str[0],
             "end_date": time_range_str[1],
-            "is_dynamic": is_dynamic,
-            "data_layers": {"data_sources": data_layers_lst}
+            "is_dynamic": is_dynamic
         }
 
+        if layer_selection_id:
+            json_data["layer_selection_id"] = layer_selection_id
+        elif len(layer_ids) > 0:
+            layer_ids_str = ','.join(str(x) for x in layer_ids)
+            json_data["layer_ids"] = layer_ids_str
+        else:
+            json_data["data_layers"] = {"data_sources": data_layers_lst}
+
         route = "/aoi_manager/create_aoi"
         accept = "application/json"
         content_type = "application/json"
 
         try:
             response = self._make_request(
                 "POST", route, json_data=json_data, auth=self.auth, content_type=content_type, accept=accept)
 
         except HTTPException as error:
             raise DdcRequestError(
                 f"Error during creating aoi with body {json_data} from {route}"
             ) from error
 
-        return self._process_response(response, desired_type)
+        return self._process_response(response, output_data_type)
 
     @authorize_request
-    def get_crop_types(self, desired_type: int = 1) -> Union[pd.DataFrame, List[Dict]]:
+    def get_data_layers(self, output_data_type: int = 1) -> Union[pd.DataFrame, List[Dict]]:
+        """
+        Get available data layers
+
+        Args:
+
+        Returns:
+            Union[pd.DataFrame, Dict]: Depending on the `output_data_type` parameter,
+            this function returns either a pandas DataFrame or a dictionary containing crop type information.
+        """
+
+        params = {'user_id': self.client_id}
+
+        route = "/aoi_manager/data_layers"
+        accept = "application/json"
+
+        try:
+            response = self._make_request(
+                "GET", route, params=params, auth=self.auth, accept=accept)
+
+        except HTTPException as error:
+            raise DdcRequestError(
+                f"Error during getting crop types with params {params} from {route}"
+            ) from error
+
+        return self._process_response(response, output_data_type)
+
+    @authorize_request
+    def get_crop_types(self, output_data_type: int = 1) -> Union[pd.DataFrame, List[Dict]]:
         """
         Get available crop types.
 
         Args:
-            desired_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as a dictionary(2).
+            output_data_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as a dictionary(2).
                 Defaults to 1.
 
         Returns:
-            Union[pd.DataFrame, List[Dict]]: Depending on the `desired_type` parameter,
+            Union[pd.DataFrame, List[Dict]]: Depending on the `output_data_type` parameter,
             this function returns either a pandas DataFrame or a list of dictionary containing crop type information.
 
         Raises:
             DdcRequestError: If an error occurs during the process of requesting crop types.
         """
 
         params = {'user_id': self.client_id}
@@ -380,31 +419,31 @@
                 "GET", route, params=params, auth=self.auth, accept=accept)
 
         except HTTPException as error:
             raise DdcRequestError(
                 f"Error during getting crop types with params {params} from {route}"
             ) from error
 
-        return self._process_response(response, desired_type)
+        return self._process_response(response, output_data_type)
 
     @authorize_request
     def create_crop_type(self,
                          crop_type_name: str,
-                         desired_type: int = 1
+                         output_data_type: int = 1
                          ) -> Union[pd.DataFrame, Dict]:
         """
         Create crop type.
 
         Args:
             crop_type_name (str): Name of the crop type.
-            desired_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as a dictionary(2).
+            output_data_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as a dictionary(2).
                 Defaults to 1.
 
         Returns:
-            Union[pd.DataFrame, Dict]: Depending on the `desired_type` parameter,
+            Union[pd.DataFrame, Dict]: Depending on the `output_data_type` parameter,
             this function returns either a pandas DataFrame or a dictionary containing crop type information.
 
         Raises:
             DdcRequestError: If an error occurs during the process of creating the growing season.
 
         """
 
@@ -422,28 +461,28 @@
                 "POST", route, json_data=json_data, auth=self.auth, content_type=content_type, accept=accept)
 
         except HTTPException as error:
             raise DdcRequestError(
                 f"Error during creating crop type with body {json_data} from {route}"
             ) from error
 
-        return self._process_response(response, desired_type)
+        return self._process_response(response, output_data_type)
 
     @authorize_request
-    def get_crop_variety(self, crop_type_id: int, desired_type: int = 1) -> Union[pd.DataFrame, List[Dict]]:
+    def get_crop_variety(self, crop_type_id: int, output_data_type: int = 1) -> Union[pd.DataFrame, List[Dict]]:
         """
         Get available crop types.
 
         Args:
             crop_type_id (int): ID of crop type.
-            desired_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as a dictionary(2).
+            output_data_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as a dictionary(2).
                 Defaults to 1.
 
         Returns:
-            Union[pd.DataFrame, List[Dict]]: Depending on the `desired_type` parameter,
+            Union[pd.DataFrame, List[Dict]]: Depending on the `output_data_type` parameter,
             this function returns either a pandas DataFrame or a list of dictionary containing crop variety information.
 
         Raises:
             DdcRequestError: If an error occurs during the process of requesting crop variety.
         """
 
         params = {'user_id': self.client_id,
@@ -457,33 +496,33 @@
                 "GET", route, params=params, auth=self.auth, accept=accept)
 
         except HTTPException as error:
             raise DdcRequestError(
                 f"Error during getting crop variety with params {params} from {route}"
             ) from error
 
-        return self._process_response(response, desired_type)
+        return self._process_response(response, output_data_type)
 
     @authorize_request
     def create_crop_variety(self,
                             crop_type_id: id,
                             crop_variety_name: str,
-                            desired_type: int = 1
+                            output_data_type: int = 1
                             ) -> Union[pd.DataFrame, Dict]:
         """
         Create crop variety.
 
         Args:
             crop_type_id (id): ID of crop type.
             crop_variety_name (str): Name of the crop variety.
-            desired_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as a dictionary(2).
+            output_data_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as a dictionary(2).
                 Defaults to 1.
 
         Returns:
-            Union[pd.DataFrame, Dict]: Depending on the `desired_type` parameter,
+            Union[pd.DataFrame, Dict]: Depending on the `output_data_type` parameter,
             this function returns either a pandas DataFrame or a dictionary containing crop variety information.
 
         Raises:
             DdcRequestError: If an error occurs during the process of creating the crop variety.
 
         """
 
@@ -502,28 +541,28 @@
                 "POST", route, json_data=json_data, auth=self.auth, content_type=content_type, accept=accept)
 
         except HTTPException as error:
             raise DdcRequestError(
                 f"Error during creating crop variety with body {json_data} from {route}"
             ) from error
 
-        return self._process_response(response, desired_type)
+        return self._process_response(response, output_data_type)
 
     @authorize_request
-    def get_crop_models(self, crop_type_id: int, desired_type: int = 1) -> Union[pd.DataFrame, List[Dict]]:
+    def get_crop_models(self, crop_type_id: int, output_data_type: int = 1) -> Union[pd.DataFrame, List[Dict]]:
         """
         Get available crop model list.
 
         Args:
             crop_type_id (int): ID of crop type.
-            desired_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as a dictionary(2).
+            output_data_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as a dictionary(2).
                 Defaults to 1.
 
         Returns:
-            Union[pd.DataFrame, List[Dict]]: Depending on the `desired_type` parameter,
+            Union[pd.DataFrame, List[Dict]]: Depending on the `output_data_type` parameter,
             this function returns either a pandas DataFrame or a list of dictionary containing crop model information.
 
         Raises:
             DdcRequestError: If an error occurs during the process of requesting crop models.
         """
 
         params = {'user_id': self.client_id,
@@ -537,42 +576,46 @@
                 "GET", route, params=params, auth=self.auth, accept=accept)
 
         except HTTPException as error:
             raise DdcRequestError(
                 f"Error during getting crop models with params {params} from {route}"
             ) from error
 
-        return self._process_response(response, desired_type)
+        return self._process_response(response, output_data_type)
 
     @authorize_request
     def run_crop_model(self,
                        aoi_id: int,
                        time_range: Union[TimeRange, Tuple[pd.Timestamp, pd.Timestamp], Tuple[str, str]],
                        sowing_date: Union[pd.Timestamp, str],
                        irrigation: List[Union[IrrigationSchedule, Tuple[Union[pd.Timestamp, str], float]]],
                        init_water_content: float,
                        growing_season_id: int,
                        crop_model_name: str,
-                       desired_type: int = 1) -> Union[pd.DataFrame, List[Dict]]:
+                       seasonal_trajectory: bool,
+                       soil_type: str,
+                       output_data_type: int = 1) -> Union[pd.DataFrame, List[Dict]]:
         """
         Run crop model.
 
         Args:
             aoi_id (int): ID of the AOI.
             time_range (Union[TimeRange, Tuple[pd.Timestamp, pd.Timestamp], Tuple[str, str]]): Time range for the simulation.
             sowing_date (Union[pd.Timestamp, str]): Sowing date for the simulation.
             irrigation (List[Union[IrrigationSchedule, Tuple[Union[pd.Timestamp, str], float]]]): Irrigation schedule for the simulation.
             init_water_content (float): Initial water content for the simulation.
             growing_season_id (int): ID of the growing season.
             crop_model_name (str): Name of the crop model.
-            desired_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as a dictionary(2).
+            seasonal_trajectory (bool): Flag for utilization of CLMS PPI ST in the modelling process
+            soil_type (str): USDA soil type definition  
+            output_data_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as a dictionary(2).
                 Defaults to 1.
 
         Returns:
-            Union[pd.DataFrame, List[Dict]]: Depending on the `desired_type` parameter,
+            Union[pd.DataFrame, List[Dict]]: Depending on the `output_data_type` parameter,
             this function returns either a pandas DataFrame or a list of dictionary containing crop model information.
 
         Raises:
             DdcRequestError: If an error occurs during the process of running crop model.
 
         """
 
@@ -595,43 +638,45 @@
             "aoi_id": aoi_id,
             "start_date": time_range_str[0],
             "end_date": time_range_str[1],
             "sowing_date": sowing_date_str,
             "irrigation": irrigation_str,
             "init_water_content": init_water_content,
             "growing_season_id": growing_season_id,
-            "crop_model_name": crop_model_name
+            "crop_model_name": crop_model_name,
+            "seasonal_trajectory": seasonal_trajectory,
+            "soil_type": soil_type
         }
 
         route = "/crop_model/run"
         accept = "application/json"
 
         try:
             response = self._make_request(
                 "GET", route, params=params, auth=self.auth, accept=accept)
 
         except HTTPException as error:
             raise DdcRequestError(
                 f"Error during running crop modle with params {params} from {route}"
             ) from error
 
-        return self._process_response(response, desired_type)
+        return self._process_response(response, output_data_type)
 
     @authorize_request
-    def get_growing_season(self, aoi_id: int, desired_type: int = 1) -> Union[pd.DataFrame, List[Dict]]:
+    def get_growing_season(self, aoi_id: int, output_data_type: int = 1) -> Union[pd.DataFrame, List[Dict]]:
         """
         Get growing seasons for AOI.
 
         Args:
             aoi_id (int): ID of the AOI.
-            desired_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as a dictionary(2).
+            output_data_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as a dictionary(2).
                 Defaults to 1.
 
         Returns:
-            Union[pd.DataFrame, List[Dict]]: Depending on the `desired_type` parameter,
+            Union[pd.DataFrame, List[Dict]]: Depending on the `output_data_type` parameter,
             this function returns either a pandas DataFrame or a list of dictionary containing growing season information.
 
         Raises:
             DdcRequestError: If an error occurs during the process of requesting growing seasons.
         """
 
         params = {'user_id': self.client_id,
@@ -645,44 +690,44 @@
                 "GET", route, params=params, auth=self.auth, accept=accept)
 
         except HTTPException as error:
             raise DdcRequestError(
                 f"Error during getting growing seasons with params {params} from {route}"
             ) from error
 
-        return self._process_response(response, desired_type)
+        return self._process_response(response, output_data_type)
 
     @authorize_request
     def create_growing_season(self,
                               aoi_id: int,
                               time_range: Union[TimeRange, Tuple[pd.Timestamp, pd.Timestamp], Tuple[str, str]],
                               sowing_date: Union[pd.Timestamp, str],
                               crop_type_id: int,
                               crop_variety_id: int,
                               crop_model_id: int,
-                              desired_type: int = 1
+                              output_data_type: int = 1
                               ) -> Union[pd.DataFrame, Dict]:
         """
         Create growing season for AOI.
 
         Args:
             aoi_id (int): ID of the AOI.
             time_range (Union[TimeRange, Tuple[pd.Timestamp, pd.Timestamp], Tuple[str, str]]):
                 The time range for which the growing season is defined.
                 This can be provided as a `ddc_utility.TimeRange` object, a tuple of two `pandas.Timestamp` objects,
                 or a tuple of two strings representing dates.
             sowing_date (Union[pd.Timestamp, str]): The date when the crop is sown.
             crop_type_id (int): ID of crop type.
             crop_variety_id (int): ID of crop variety.
             crop_model_id (int): ID of crop model.
-            desired_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as a dictionary(2).
+            output_data_type (int, optional): Whether to return the result as pandas.DataFrame (1) or as a dictionary(2).
                 Defaults to 1.
 
         Returns:
-            Union[pd.DataFrame, Dict]: Depending on the `desired_type` parameter,
+            Union[pd.DataFrame, Dict]: Depending on the `output_data_type` parameter,
             this function returns either a pandas DataFrame or a dictionary containing growing season information.
 
         Raises:
             DdcRequestError: If an error occurs during the process of creating the growing season.
 
         """
 
@@ -714,15 +759,15 @@
                 "POST", route, json_data=json_data, auth=self.auth, content_type=content_type, accept=accept)
 
         except HTTPException as error:
             raise DdcRequestError(
                 f"Error during creating growing season with body {json_data} from {route}"
             ) from error
 
-        return self._process_response(response, desired_type)
+        return self._process_response(response, output_data_type)
 
     @authorize_s3_access
     def open_aoi_cube(self, aoi_id: int, bucket_name: str = DEFAULT_AOI_BUCKET) -> xr.Dataset:
         """
         Open AOI cube as an xarray.Dataset.
 
         Args:
@@ -752,68 +797,58 @@
         except Exception as error:
             raise DdcRequestError(
                 f"Error during getting AOI cube from {zarr_path}"
             ) from error
         return cube
 
     @authorize_s3_access
-    def open_ddc_cube(self, dataset_name: str, bucket_name: str = DEFAULT_DDC_BUCKET) -> xr.Dataset:
+    def open_ddc_cube(self, zarr_path: str, zarr_group: Optional[str] = None, bucket_name: str = DEFAULT_DDC_BUCKET) -> xr.Dataset:
         """
         Open DDC dataset as an xarray.Dataset.
 
         Args:
-            dataset_name (str): Name of the DDC dataset.
+            zarr_path (str): zarr path to the dataset.
+            zarr_group (str): zarr group of the dataset.
             bucket_name (str, optional): Name of the S3 bucket where the zarr cube is stored.
                 Defaults to `DEFAULT_AOI_BUCKET`.
 
         Returns:
             xr.Dataset: DDC cube.
 
         Raises:
             DdcClientError: If user don't have access to the bucket.
             DdcRequestError: If an error occurs during opening the cube.
 
         """
-        dataset_name_to_zarr_path = {
-            "meteorology": {"zarr_name": "met.zarr", "group": "meteorology"},
-            "nhrl": {"zarr_name": "nhrl.zarr", "group": "nhrl"},
-            "ecosystem": {"zarr_name": "ecosystem.zarr", "group": "ecosystem"},
-            "soil": {"zarr_name": "taki.zarr", "group": "soil"},
-        }
-
-        zarr_path_info = dataset_name_to_zarr_path.get(dataset_name)
-        if not zarr_path_info:
-            raise ValueError(
-                f"Invalid dataset_name: {dataset_name} - must be one of {list(dataset_name_to_zarr_path.keys())}")
 
-        zarr_path = f"s3://{bucket_name}/{zarr_path_info['zarr_name']}"
+        zarr_path = f"s3://{bucket_name}/{zarr_path}"
 
         try:
             cube = open_cube(path=zarr_path,
                              fs=self.aws_s3,
-                             group=zarr_path_info['group'])
+                             group=zarr_group)
         except PermissionError as error:
             raise DdcClientError(
                 "User don't have access for this operation") from error
         except Exception as error:
             raise DdcRequestError(
                 f"Error during getting DDC cube from {zarr_path}"
             ) from error
         return cube
 
     
-    def _process_response(self, data: Any, desired_type: int = None):
-        if desired_type == 1:
+    def _process_response(self, data: Any, output_data_type: int = None):
+        if output_data_type == 1:
             if isinstance(data, list):
                 return pd.DataFrame(data)
             if isinstance(data, dict):
                 return pd.DataFrame([data])
             else:
                 raise ValueError(
-                    f"Can't post-process API response -- {type(data)} is invalid with desired_type of {desired_type}")
+                    f"Can't post-process API response -- {type(data)} is invalid with output_data_type of {output_data_type}")
         else:
             return data
 
     def fetch_token(self) -> Dict:
         """Fetch token from a remote token endpoint."""
 
         route = "/get_token"
```

### Comparing `ddc-utility-1.3.1/ddc_utility/data_collections.py` & `ddc_utility-1.4.0/ddc_utility/data_collections.py`

 * *Files identical despite different names*

### Comparing `ddc-utility-1.3.1/ddc_utility/errors.py` & `ddc_utility-1.4.0/ddc_utility/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 class DdcClientError(DdcException):
     """
     Exception raised for client related errors
     """
     pass
 
 
+
 class HTTPException(DdcException):
     """
     Exception raised when an HTTP request fails
 
     Attributes
     ----------
     response : requests.Response | aiohttp.ClientResponse
```

### Comparing `ddc-utility-1.3.1/ddc_utility/metadata.py` & `ddc_utility-1.4.0/ddc_utility/metadata.py`

 * *Files identical despite different names*

### Comparing `ddc-utility-1.3.1/ddc_utility/utils.py` & `ddc_utility-1.4.0/ddc_utility/utils.py`

 * *Files identical despite different names*

### Comparing `ddc-utility-1.3.1/ddc_utility.egg-info/PKG-INFO` & `ddc_utility-1.4.0/ddc_utility.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddc-utility
-Version: 1.3.1
+Version: 1.4.0
 Summary: Package for retrieving DDC datasests
 Author-email: Balint Alfoldy <alfibalint@gmail.com>, CropOM <marton.tolnai@cropom.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -15,14 +15,16 @@
 Requires-Dist: numcodecs>=0.11.0
 Requires-Dist: pydantic>=1.10.0
 Requires-Dist: pyproj>=3.4.1
 Requires-Dist: requests>=2.28.2
 Requires-Dist: xarray>=2023.1.0
 Requires-Dist: zarr>=2.13.6
 Requires-Dist: fsspec
+Requires-Dist: s3fs
+Requires-Dist: shapely
 
 # DDC Utility
 
 This is the Danube Data Cube Utility library, for retrieving data from the Danube Data Cube portal.
 
 ### Installation
```

### Comparing `ddc-utility-1.3.1/pyproject.toml` & `ddc_utility-1.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ddc-utility"
-version = "1.3.1"
+version = "1.4.0"
 description = "Package for retrieving DDC datasests"
 authors = [
     {name = "Balint Alfoldy", email = "alfibalint@gmail.com"},
     {name = "CropOM", email = "marton.tolnai@cropom.com"},
 ]
 readme = "README.md"
 requires-python = ">=3.8"
@@ -19,15 +19,17 @@
     "matplotlib >= 3.6.2",
     "numcodecs >= 0.11.0",
     "pydantic >= 1.10.0",
     "pyproj >= 3.4.1",
     "requests >= 2.28.2",
     "xarray >= 2023.1.0",
     "zarr >= 2.13.6",
-    "fsspec"
+    "fsspec", 
+    "s3fs",
+    "shapely"
 ]
 
 [tool.setuptools.packages.find]
 include = ["ddc_utility*"]
 
 [build-system]
 requires = ["setuptools>=61.0"]
```

### Comparing `ddc-utility-1.3.1/test/test_metadata.py` & `ddc_utility-1.4.0/test/test_metadata.py`

 * *Files identical despite different names*

