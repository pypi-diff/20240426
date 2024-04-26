# Comparing `tmp/openmindat-0.0.4.tar.gz` & `tmp/openmindat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmindat-0.0.4.tar", last modified: Sun Apr 14 17:33:07 2024, max compression
+gzip compressed data, was "openmindat-0.0.5.tar", last modified: Fri Apr 26 17:48:24 2024, max compression
```

## Comparing `openmindat-0.0.4.tar` & `openmindat-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-14 17:33:07.599038 openmindat-0.0.4/
--rw-r--r--   0 blc        (501) staff       (20)    11357 2023-09-28 23:58:40.000000 openmindat-0.0.4/LICENSE
--rw-r--r--   0 blc        (501) staff       (20)      136 2024-04-09 06:30:41.000000 openmindat-0.0.4/MANIFEST.in
--rw-r--r--   0 blc        (501) staff       (20)     5833 2024-04-14 17:33:07.598785 openmindat-0.0.4/PKG-INFO
--rw-r--r--   0 blc        (501) staff       (20)     5319 2024-04-14 17:31:34.000000 openmindat-0.0.4/README.md
-drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-14 17:33:07.597243 openmindat-0.0.4/openmindat/
--rw-r--r--   0 blc        (501) staff       (20)     6064 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/__init__.py
--rw-r--r--   0 blc        (501) staff       (20)     8140 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/countries.py
--rw-r--r--   0 blc        (501) staff       (20)     5358 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/dana8.py
--rw-r--r--   0 blc        (501) staff       (20)    46900 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/geomaterials.py
--rw-r--r--   0 blc        (501) staff       (20)     3785 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/geomaterials_search.py
--rw-r--r--   0 blc        (501) staff       (20)    20215 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/localities.py
--rw-r--r--   0 blc        (501) staff       (20)     8285 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/localities_age.py
--rw-r--r--   0 blc        (501) staff       (20)     8335 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/localities_status.py
--rw-r--r--   0 blc        (501) staff       (20)     8296 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/localities_type.py
--rw-r--r--   0 blc        (501) staff       (20)     4447 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/locgeoregion2.py
--rw-r--r--   0 blc        (501) staff       (20)     3848 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/locobject.py
--rw-r--r--   0 blc        (501) staff       (20)    11800 2024-04-12 00:35:16.000000 openmindat-0.0.4/openmindat/mindat_api.py
--rw-r--r--   0 blc        (501) staff       (20)    13369 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/minerals_ima.py
--rw-r--r--   0 blc        (501) staff       (20)     5839 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/nickel_strunz.py
--rw-r--r--   0 blc        (501) staff       (20)     3101 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/photo_count.py
-drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-14 17:33:07.598486 openmindat-0.0.4/openmindat.egg-info/
--rw-r--r--   0 blc        (501) staff       (20)     5833 2024-04-14 17:33:07.000000 openmindat-0.0.4/openmindat.egg-info/PKG-INFO
--rw-r--r--   0 blc        (501) staff       (20)      642 2024-04-14 17:33:07.000000 openmindat-0.0.4/openmindat.egg-info/SOURCES.txt
--rw-r--r--   0 blc        (501) staff       (20)        1 2024-04-14 17:33:07.000000 openmindat-0.0.4/openmindat.egg-info/dependency_links.txt
--rw-r--r--   0 blc        (501) staff       (20)        1 2024-03-09 23:51:57.000000 openmindat-0.0.4/openmindat.egg-info/not-zip-safe
--rw-r--r--   0 blc        (501) staff       (20)       16 2024-04-14 17:33:07.000000 openmindat-0.0.4/openmindat.egg-info/requires.txt
--rw-r--r--   0 blc        (501) staff       (20)       11 2024-04-14 17:33:07.000000 openmindat-0.0.4/openmindat.egg-info/top_level.txt
--rw-r--r--   0 blc        (501) staff       (20)       38 2024-04-14 17:33:07.599099 openmindat-0.0.4/setup.cfg
--rw-r--r--   0 blc        (501) staff       (20)     1058 2024-04-14 17:12:58.000000 openmindat-0.0.4/setup.py
+drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-26 17:48:24.532507 openmindat-0.0.5/
+-rw-r--r--   0 blc        (501) staff       (20)    11357 2023-09-28 23:58:40.000000 openmindat-0.0.5/LICENSE
+-rw-r--r--   0 blc        (501) staff       (20)      136 2024-04-09 06:30:41.000000 openmindat-0.0.5/MANIFEST.in
+-rw-r--r--   0 blc        (501) staff       (20)     6247 2024-04-26 17:48:24.532266 openmindat-0.0.5/PKG-INFO
+-rw-r--r--   0 blc        (501) staff       (20)     5741 2024-04-26 17:47:50.000000 openmindat-0.0.5/README.md
+drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-26 17:48:24.530653 openmindat-0.0.5/openmindat/
+-rw-r--r--   0 blc        (501) staff       (20)     6087 2024-04-25 18:17:20.000000 openmindat-0.0.5/openmindat/__init__.py
+-rw-r--r--   0 blc        (501) staff       (20)     8320 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/countries.py
+-rw-r--r--   0 blc        (501) staff       (20)     5656 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/dana8.py
+-rw-r--r--   0 blc        (501) staff       (20)    47522 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/geomaterials.py
+-rw-r--r--   0 blc        (501) staff       (20)     4207 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/geomaterials_search.py
+-rw-r--r--   0 blc        (501) staff       (20)    20573 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/localities.py
+-rw-r--r--   0 blc        (501) staff       (20)     8378 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/localities_age.py
+-rw-r--r--   0 blc        (501) staff       (20)     8578 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/localities_status.py
+-rw-r--r--   0 blc        (501) staff       (20)     8535 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/localities_type.py
+-rw-r--r--   0 blc        (501) staff       (20)     4215 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/locgeoregion2.py
+-rw-r--r--   0 blc        (501) staff       (20)     3775 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/locobject.py
+-rw-r--r--   0 blc        (501) staff       (20)     9166 2024-04-25 17:55:43.000000 openmindat-0.0.5/openmindat/mindat_api.py
+-rw-r--r--   0 blc        (501) staff       (20)    13796 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/minerals_ima.py
+-rw-r--r--   0 blc        (501) staff       (20)     6120 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/nickel_strunz.py
+-rw-r--r--   0 blc        (501) staff       (20)     3496 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/photo_count.py
+drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-26 17:48:24.531961 openmindat-0.0.5/openmindat.egg-info/
+-rw-r--r--   0 blc        (501) staff       (20)     6247 2024-04-26 17:48:24.000000 openmindat-0.0.5/openmindat.egg-info/PKG-INFO
+-rw-r--r--   0 blc        (501) staff       (20)      642 2024-04-26 17:48:24.000000 openmindat-0.0.5/openmindat.egg-info/SOURCES.txt
+-rw-r--r--   0 blc        (501) staff       (20)        1 2024-04-26 17:48:24.000000 openmindat-0.0.5/openmindat.egg-info/dependency_links.txt
+-rw-r--r--   0 blc        (501) staff       (20)        1 2024-03-09 23:51:57.000000 openmindat-0.0.5/openmindat.egg-info/not-zip-safe
+-rw-r--r--   0 blc        (501) staff       (20)       21 2024-04-26 17:48:24.000000 openmindat-0.0.5/openmindat.egg-info/requires.txt
+-rw-r--r--   0 blc        (501) staff       (20)       11 2024-04-26 17:48:24.000000 openmindat-0.0.5/openmindat.egg-info/top_level.txt
+-rw-r--r--   0 blc        (501) staff       (20)       38 2024-04-26 17:48:24.532572 openmindat-0.0.5/setup.cfg
+-rw-r--r--   0 blc        (501) staff       (20)     1076 2024-04-26 17:38:02.000000 openmindat-0.0.5/setup.py
```

### Comparing `openmindat-0.0.4/LICENSE` & `openmindat-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.4/PKG-INFO` & `openmindat-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmindat
-Version: 0.0.4
+Version: 0.0.5
 Summary: An alpha version for OpenMindat package
 Home-page: https://github.com/ChuBL/OpenMindat
 Author: Jiyin Zhang
 Author-email: jiyinz@uidaho.edu
 License: Apache Software License
 Keywords: mindat openmindat mineral data python api
 Classifier: Development Status :: 3 - Alpha
@@ -48,33 +48,30 @@
 
 > If you do not have a Mindat API key, please refer to [How to Get My Mindat API Key or Token?](https://www.mindat.org/a/how_to_get_my_mindat_api_key)
 
 You can also set the API key by following the general queries.
 
 ### 1. Perform Detailed Queries on Geomaterials
 
-:exclamation: Temporarily Outage, see https://github.com/ChuBL/OpenMindat/issues/12
-
 ```python
-# Temporarily Outage, see https://github.com/ChuBL/OpenMindat/issues/12
 from openmindat import GeomaterialRetriever
 
 gr = GeomaterialRetriever()
 gr.density_min(2.0).density_max(5.0).crystal_system("Hexagonal")
 gr.elements_exc("Au,Ag")
-gr.saveto("./mindat_data")
+gr.save()
 ```
 
 ### 2. Retrieve IMA-Approved Minerals
 
 ```python
 from openmindat import MineralsIMARetriever
 
 mir = MineralsIMARetriever()
-mir.ima(1).fields("id,name,ima_formula,ima_year")
+mir.fields("id,name,ima_formula,ima_year")
 mir.saveto("./mindat_data", 'my_filename')
 ```
 
 ### 3. Search Geomaterials Using Keywords
 
 ```python
 from openmindat import GeomaterialSearchRetriever
@@ -82,15 +79,15 @@
 gsr = GeomaterialSearchRetriever()
 gsr.geomaterials_search("quartz, green, hexagonal")
 gsr.save("filename")
 
 # Alternatively, you can get the list object directly:
 gsr = GeomaterialSearchRetriever()
 gsr.geomaterials_search("ruby, red, hexagonal")
-print(gsr.get_list())
+print(gsr.get_dict())
 ```
 
 ### 4. Retrieve Localities
 
 :exclamation: Some country names, e.g., United States and United Kingdom, are not working due to server-side problems, which will be fixed in the future.
 
 ```python
@@ -99,15 +96,15 @@
 lr = LocalitiesRetriever()
 lr.country("France").txt("mine")
 lr.save()
 
 # Alternatively, you can get the list object directly:
 lr = LocalitiesRetriever()
 lr.country("Canada").description("mine")
-print(lr.get_list())
+print(lr.get_dict())
 ```
 
 ### 5. Retrieve Type Localities for IMA-Approved Mineral Species
 
 ```python
 from openmindat import GeomaterialRetriever
 
@@ -163,28 +160,39 @@
 
 ## License
 
 **Project Licence:** [Apache](LICENSE)
 
 **Mindat Data License:** [CC BY-NC-SA 4.0 DEED](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.en)
 
+The Mindat API is currently in beta test, and while access is free for all, please note that the data provided are not yet licensed for redistribution and are for private, non-commercial use only. Once launched, data will be available under an open-access license, but please always check the terms of use of the license before reusing these data.
+
 ## Author
 
 Jiyin Zhang, Clairmont Cory
 
 ## Acknowledgments
 
 <p float="left">
         <img src="https://github.com/ChuBL/OpenMindat/blob/main/Logo/mindat2017.png?raw=true"  width="25%">
         <img src="https://github.com/ChuBL/OpenMindat/blob/main/Logo/NSF_Official_logo_Low_Res.png?raw=true"  width="10%">
 </p>
 
 - This work is supported by NSF, Award #2126315.
 
-## Updating Logs
+## Upgrading Logs
+
+### 0.0.5
+**Released:** Apr 26, 2024
+
+- The `Internal Server Error` issue in v0.0.4 is fixed from the server side.
+- The get functions are now changed to `get_dict`.
+- Added progress bars for multiple-page queries.
+- Some other minor updates.
+
 
 ### 0.0.4
 **Released:** Apr 14, 2024
 
 - Tentative issue: Data queries involving multiple pages might return an `Internal Server Error` due to server-end issues. [Related GitHub issue](https://github.com/ChuBL/OpenMindat/issues/12)
 - Added support to getting list objects of obtained data in addition to saving it to local directories.
```

### Comparing `openmindat-0.0.4/README.md` & `openmindat-0.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -30,33 +30,30 @@
 
 > If you do not have a Mindat API key, please refer to [How to Get My Mindat API Key or Token?](https://www.mindat.org/a/how_to_get_my_mindat_api_key)
 
 You can also set the API key by following the general queries.
 
 ### 1. Perform Detailed Queries on Geomaterials
 
-:exclamation: Temporarily Outage, see https://github.com/ChuBL/OpenMindat/issues/12
-
 ```python
-# Temporarily Outage, see https://github.com/ChuBL/OpenMindat/issues/12
 from openmindat import GeomaterialRetriever
 
 gr = GeomaterialRetriever()
 gr.density_min(2.0).density_max(5.0).crystal_system("Hexagonal")
 gr.elements_exc("Au,Ag")
-gr.saveto("./mindat_data")
+gr.save()
 ```
 
 ### 2. Retrieve IMA-Approved Minerals
 
 ```python
 from openmindat import MineralsIMARetriever
 
 mir = MineralsIMARetriever()
-mir.ima(1).fields("id,name,ima_formula,ima_year")
+mir.fields("id,name,ima_formula,ima_year")
 mir.saveto("./mindat_data", 'my_filename')
 ```
 
 ### 3. Search Geomaterials Using Keywords
 
 ```python
 from openmindat import GeomaterialSearchRetriever
@@ -64,15 +61,15 @@
 gsr = GeomaterialSearchRetriever()
 gsr.geomaterials_search("quartz, green, hexagonal")
 gsr.save("filename")
 
 # Alternatively, you can get the list object directly:
 gsr = GeomaterialSearchRetriever()
 gsr.geomaterials_search("ruby, red, hexagonal")
-print(gsr.get_list())
+print(gsr.get_dict())
 ```
 
 ### 4. Retrieve Localities
 
 :exclamation: Some country names, e.g., United States and United Kingdom, are not working due to server-side problems, which will be fixed in the future.
 
 ```python
@@ -81,15 +78,15 @@
 lr = LocalitiesRetriever()
 lr.country("France").txt("mine")
 lr.save()
 
 # Alternatively, you can get the list object directly:
 lr = LocalitiesRetriever()
 lr.country("Canada").description("mine")
-print(lr.get_list())
+print(lr.get_dict())
 ```
 
 ### 5. Retrieve Type Localities for IMA-Approved Mineral Species
 
 ```python
 from openmindat import GeomaterialRetriever
 
@@ -145,28 +142,39 @@
 
 ## License
 
 **Project Licence:** [Apache](LICENSE)
 
 **Mindat Data License:** [CC BY-NC-SA 4.0 DEED](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.en)
 
+The Mindat API is currently in beta test, and while access is free for all, please note that the data provided are not yet licensed for redistribution and are for private, non-commercial use only. Once launched, data will be available under an open-access license, but please always check the terms of use of the license before reusing these data.
+
 ## Author
 
 Jiyin Zhang, Clairmont Cory
 
 ## Acknowledgments
 
 <p float="left">
         <img src="https://github.com/ChuBL/OpenMindat/blob/main/Logo/mindat2017.png?raw=true"  width="25%">
         <img src="https://github.com/ChuBL/OpenMindat/blob/main/Logo/NSF_Official_logo_Low_Res.png?raw=true"  width="10%">
 </p>
 
 - This work is supported by NSF, Award #2126315.
 
-## Updating Logs
+## Upgrading Logs
+
+### 0.0.5
+**Released:** Apr 26, 2024
+
+- The `Internal Server Error` issue in v0.0.4 is fixed from the server side.
+- The get functions are now changed to `get_dict`.
+- Added progress bars for multiple-page queries.
+- Some other minor updates.
+
 
 ### 0.0.4
 **Released:** Apr 14, 2024
 
 - Tentative issue: Data queries involving multiple pages might return an `Internal Server Error` due to server-end issues. [Related GitHub issue](https://github.com/ChuBL/OpenMindat/issues/12)
 - Added support to getting list objects of obtained data in addition to saving it to local directories.
```

### Comparing `openmindat-0.0.4/openmindat/__init__.py` & `openmindat-0.0.5/openmindat/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 Examples:
     Using the help function to view the docstring for classes, such as GeomaterialRetriever:
         >>> help(GeomaterialRetriever)
 
     Using the MineralsIMARetriever class to retrieve IMA-approved minerals:
         >>> mir = MineralsIMARetriever()
-        >>> mir.ima(1).fields("id,name,ima_formula,ima_year")
+        >>> mir.fields("id,name,ima_formula,ima_year")
         >>> mir.saveto("/path/to/minerals_data")
 
     Searching geomaterials with specific keywords using GeomaterialSearchRetriever:
         >>> gsr = GeomaterialSearchRetriever()
         >>> gsr.geomaterials_search("quartz, green, hexagonal")
         >>> gsr.save()
 
@@ -51,15 +51,15 @@
         >>> gr = GeomaterialRetriever()
         >>> gr.density_min(2.0).density_max(5.0).crystal_system("Hexagonal")
         >>> gr.elements_exc("Au,Ag")
         >>> gr.saveto("/path/to/geomaterials_data")
         
 Press q to quit.
 """
-from . import mindat_api
+from .mindat_api import MindatApi, MindatApiKeyManeger
 from .minerals_ima import MineralsIMARetriever
 from .minerals_ima import MineralsIdRetriever
 from .geomaterials_search import GeomaterialSearchRetriever
 from .geomaterials import GeomaterialRetriever
 from .geomaterials import GeomaterialIdRetriever
 from .geomaterials import GeomaterialDictRetriever
 from .localities import LocalitiesRetriever
```

### Comparing `openmindat-0.0.4/openmindat/countries.py` & `openmindat-0.0.5/openmindat/countries.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,20 +15,21 @@
         >>> cr = CountriesListRetriever()
         >>> cr.page(2).save()
 
     Press q to quit.
     """
     
     def __init__(self):
-       self.end_point = 'countries' 
+        self.end_point = 'countries' 
         
-       self._params = {}
-       self._init_params()
+        self._params = {}
+        self._init_params()
     
     def _init_params(self):
+        self.end_point = 'countries' 
         self._params.clear()
         self._params = {'format': 'json'}
         self.page_size(1500)
     
     def page(self, PAGE):
         '''
         Returns a page of country data.
@@ -86,28 +87,22 @@
             Returns:
                 None
 
             Example:
                 >>> cr = CountriesListRetriever()
                 >>> cr.page(2).saveto("/path/to/directory")
         '''
-        
-        print("Retrieving Countries. This may take a while... ")
 
         params = self._params
         outdir = OUTDIR
         end_point = self.end_point
         file_name = FILE_NAME
         
         ma = mindat_api.MindatApi()
-        
-        if "page" in params:
-            ma.get_mindat_item(params, end_point, outdir, file_name)
-        else:
-            ma.get_mindat_list(params, end_point, outdir, file_name)
+        ma.download_mindat_json(params, end_point, outdir, file_name)
 
         # Reset the query parameters in case the user wants to make another query.
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
             Executes the query to retrieve the country data and saves the results to the current directory.
@@ -134,27 +129,25 @@
             list of dictionaries.
 
         Example:
             >>> cr = CountriesListRetriever()
             >>> france = cr.page(2).get_list()
 
         '''
-        
-        print("Retrieving countries. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
         ma = mindat_api.MindatApi()        
         #clears params for next get statement     
 
         if "page" in params:
-            results = [ma.get_mindat_dict(params, end_point)]
+            results = [ma.get_mindat_json(params, end_point)]
         else:
-            results = ma.get_mindat_list_object(params, end_point)
+            results = ma.get_mindat_json(params, end_point)
         
         
         self._init_params()
         return results
             
             
         
@@ -173,22 +166,46 @@
         >>> cidr = CountriesIdRetriever()
         >>> cidr.id(5).save()
 
     Press q to quit.
     """
     
     def __init__(self):
-       self.end_point = 'countries' 
+        self.end_point = 'countries' 
         
-       self._params = {}
-       self._init_params()
+        self._params = {}
+        self._init_params()
     
     def _init_params(self):
+        self.end_point = 'countries' 
         self._params.clear()
         self._params = {'format': 'json'}
+        self.page_size(1500)
+        
+    def page_size(self, PAGE_SIZE):
+        '''
+        Sets the number of results per page.
+
+        Args:
+            PAGE_SIZE (int): The number of results per page.
+
+        Returns:
+            self: The CountriesIdRetriever object.
+
+        Example:
+            >>> cidr = CountriesListIdRetriever()
+            >>> cidr.page_size(2)
+            >>> cidr.save()
+
+        '''
+        self._params.update({
+            'page_size': PAGE_SIZE
+        })
+
+        return self
     
     def id(self, ID):
         '''
         Returns a country with the matching ID
 
         Args:
             id (INT): The country id.
@@ -224,24 +241,22 @@
             Returns:
                 None
 
             Example:
                 >>> cidr = CountriesIdRetriever()
                 >>> cidr.id(2).saveto("/path/to/directory")
         '''
-        
-        print("Retrieving Countries. This may take a while... ")
 
         params = self._params
         outdir = OUTDIR
         end_point = self.end_point
         file_name = FILE_NAME
         
         ma = mindat_api.MindatApi()
-        ma.get_mindat_item(params, end_point, outdir, file_name)
+        ma.download_mindat_json(params, end_point, outdir, file_name)
 
         # Reset the query parameters in case the user wants to make another query.
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
             Executes the query to retrieve the list of country data and saves the results to the current directory.
@@ -268,22 +283,20 @@
             list of dictionaries.
 
         Example:
             >>> cidr = countriesIdRetriever()
             >>> france = cidr.id(2).get_liat()
 
         '''
-        
-        print("Retrieving countries. This may take a while... ")
        
         params = self._params
         end_point = self.end_point    
         
         ma = mindat_api.MindatApi()
-        results = [ma.get_mindat_dict(params, end_point)]
+        results = [ma.get_mindat_json(params, end_point)]
         
         self._init_params()
         return results
 
 if __name__ == '__main__':
     cidr = CountriesIdRetriever()
     cidr.id(2).save()
```

### Comparing `openmindat-0.0.4/openmindat/dana8.py` & `openmindat-0.0.5/openmindat/dana8.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,23 +19,48 @@
         >>> dr = DanaRetriever()
         >>> dr.groups().save()
 
     Press q to quit.
     """
     
     def __init__(self):
-       self.sub_endpoint = '' 
-       self.end_point = 'dana-8'
+        self.sub_endpoint = ''
+        self.end_point = 'dana-8'
         
-       self._params = {}
-       self._init_params()
+        self._params = {}
+        self._init_params()
     
     def _init_params(self):
+        self.end_point = 'dana-8'
+        self.sub_endpoint = ''
         self._params.clear()
         self._params = {'format': 'json'}
+        self.page_size(1500)
+
+    def page_size(self, PAGE_SIZE):
+        '''
+        Sets the number of results per page.
+
+        Args:
+            PAGE_SIZE (int): The number of results per page.
+
+        Returns:
+            self: The DanaRetriever object.
+
+        Example:
+            >>> dr = DanaRetriever()
+            >>> dr.page_size(1500)
+            >>> dr.save()
+
+        '''
+        self._params.update({
+            'page_size': PAGE_SIZE
+        })
+
+        return self
         
     def retrieve(self):
         '''
         Returns dana-8 classification
         Not yet working
 
         Returns:
@@ -124,30 +149,28 @@
                 None
 
             Example:
                 >>> dr = DanaRetriever()
                 >>> dr.saveto("/path/to/directory")
         '''
         
-        print("Retrieving Dana8 Data. This may take a while... ")
-
         params = self._params
         outdir = OUTDIR
         file_name = FILE_NAME
         end_point = self.end_point
         
         if self.sub_endpoint != '':
             end_point = '/'.join(['dana-8', self.sub_endpoint])
         
         ma = mindat_api.MindatApi()
         
         if self.sub_endpoint.isnumeric():
-            ma.get_mindat_item(params, end_point, outdir, file_name)
+            ma.download_mindat_json(params, end_point, outdir, file_name)
         else:
-            ma.get_mindat_list(params, end_point, outdir, file_name)
+            ma.download_mindat_json(params, end_point, outdir, file_name)
 
         # Reset the query parameters in case the user wants to make another query.
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
             Executes the query to retrieve the list of dana-8 data and saves the results to the current directory.
@@ -162,39 +185,34 @@
                 >>> dr = DanaRetriever()
                 >>> dr.save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve the dana-8 data as a dictionary.
 
         Returns:
             list of dictionaries.
 
         Example:
             >>> dr = danaRetriever()
-            >>> danaGroups = cr.group().get_list()
+            >>> danaGroups = cr.group().get_dict()
 
         '''
-        
-        print("Retrieving dana-8. This may take a while... ")
        
         params = self._params        
         
         if self.sub_endpoint != '':
             end_point = '/'.join(['dana-8', self.sub_endpoint])
         
         ma = mindat_api.MindatApi()
-        if self.sub_endpoint.isnumeric():
-            results = [ma.get_mindat_dict(params, end_point)]
-        else:
-            results = ma.get_mindat_list_object(params, end_point)
+        results = ma.get_mindat_json(params, end_point)
         
         self._init_params()
         return results
 
 
 if __name__ == '__main__':
     dr = DanaRetriever()
```

### Comparing `openmindat-0.0.4/openmindat/geomaterials.py` & `openmindat-0.0.5/openmindat/geomaterials.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     def __init__(self) -> None:
         self.end_point = 'geomaterials'
         self._params = {}
         self._init_params()
          # Flag to indicate if the geomaterials have been retrieved
 
     def _init_params(self):
+        self.end_point = 'geomaterials'
         self._params.clear()
         self._params.update({'format': 'json'})
         self.page_size(1500)
 
     def bi_min(self, MIN):
         '''
         Sets the minimum value of birifrigence for filtering minerals.
@@ -1258,24 +1259,22 @@
             None
 
         Example:
             >>> gr = GeomaterialRetriever()
             >>> gr.density_min(3.25).saveto("/path/to/directory")
 
         '''
-
-        print("Retrieving geomaterials. This may take a while... ")
        
         params = self._params
         end_point = 'geomaterials'
         outdir = OUTDIR
         file_name = FILE_NAME
 
         ma = mindat_api.MindatApi()
-        ma.get_mindat_list(params, end_point, outdir, file_name)
+        ma.download_mindat_json(params, end_point, outdir, file_name)
 
         # reset the query parameters in case the user wants to make another query
         self._init_params()
 
     def save(self, FILE_NAME = ''):
         '''
         Executes the query to retrieve the list of geomaterials and saves the results to the current directory.
@@ -1292,34 +1291,32 @@
 
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
 
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve the list of geomaterials and returns the json object.
 
         Returns:
             list of dictionaries.
 
         Example:
             >>> gr = GeomaterialRetriever()
-            >>> geoObject = gr.density_min(3.25).get_list()
+            >>> geoObject = gr.density_min(3.25).get_dict()
 
         '''
-        
-        print("Retrieving geomaterials. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
         ma = mindat_api.MindatApi()
-        results = ma.get_mindat_list_object(params, end_point)
+        results = ma.get_mindat_json(params, end_point)
         
         self._init_params()
         return results
 
 
 class GeomaterialIdRetriever:
     """
@@ -1332,24 +1329,48 @@
 
     Attributes:
         id (int): An int to store id parameter.
     """
     
     def __init__(self):
         self.end_point = "geomaterials"
-        self.sub_endpoint = '0'
+        self.sub_endpoint = ''
         
         self._params = {}
         self._init_params()
 
     def _init_params(self):
         self._params.clear()
         self._params = {'format': 'json'}
+        self.end_point = "geomaterials"
+        self.sub_endpoint = ''
+        self.page_size(1500)
+        
+    def page_size(self, PAGE_SIZE):
+        '''
+        Sets the number of results per page.
+
+        Args:
+            PAGE_SIZE (int): The number of results per page.
+
+        Returns:
+            self: The GeomaterialRetriever object.
+
+        Example:
+            >>> gr = GeomaterialRetriever()
+            >>> gr.page_size(50)
+            >>> gr.save()
+
+        '''
+        self._params.update({
+            'page_size': PAGE_SIZE
+        })
+
+        return self
 
-    #ask about if this option of addint variety to this endpoint is a good idea
     def id(self, ID, VARIETIES = None):
         '''
         Returns locality with matching id
 
         Args:
             id (INT): The locality id.
             variety: optional toggle returning varieties with 'y', leave empty if varieties aren't wanted
@@ -1392,23 +1413,21 @@
                 None
 
             Example:
                 >>> gir = GeomaterialIdRetriever()
                 >>> gir.id(5).saveto("/path/to/directory", "geo5")
         '''
 
-        print("Retrieving Geomaterials. This may take a while... ")
-
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         outdir = OUTDIR
         file_name = FILE_NAME
 
         ma = mindat_api.MindatApi()
-        ma.get_mindat_item(params, end_point, outdir, file_name)
+        ma.download_mindat_json(params, end_point, outdir, file_name)
 
         # reset the query parameters in case the user wants to make another query
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
             Executes the query to retrieve the list of geomaterials and saves the results to the current directory.
@@ -1423,34 +1442,32 @@
                 >>> gir = GeomaterialIdRetriever()
                 >>> gir.id(5).save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve geomaterial with a corresponding id and returns a dictionary.
 
         Returns:
             List of Dictionaries.
 
         Example:
             >>> gir = GeomaterialIdRetriever()
-            >>> geo5 = gir.id(5).get_list()
+            >>> geo5 = gir.id(5).get_dict()
 
         '''
-        
-        print("Retrieving geomaterials. This may take a while... ")
        
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         
         ma = mindat_api.MindatApi()
-        results = [ma.get_mindat_dict(params, end_point)]
+        results = ma.get_mindat_json(params, end_point)
         
         self._init_params()
         return results
         
         
         
         #NOT YET WORKING, check in to see if it returns list vs item
@@ -1465,22 +1482,47 @@
 
     Attributes:
         id (int): An int to store id parameter.
     """ 
     
     def __init__(self):
         self.end_point = 'geomaterials/dict'
-        self.sub_endpoint = '0'
+        self.sub_endpoint = ''
         
         self._params = {}
         self._init_params()
 
     def _init_params(self):
+        self.end_point = 'geomaterials/dict'
+        self.sub_endpoint = ''
         self._params.clear()
         self._params = {'format': 'json'}
+        self.page_size(1500)
+        
+    def page_size(self, PAGE_SIZE):
+        '''
+        Sets the number of results per page.
+
+        Args:
+            PAGE_SIZE (int): The number of results per page.
+
+        Returns:
+            self: The GeomaterialDictRetriever object.
+
+        Example:
+            >>> gdr = GeomaterialDictRetriever()
+            >>> gdr.page_size(50)
+            >>> gdr.save()
+
+        '''
+        self._params.update({
+            'page_size': PAGE_SIZE
+        })
+
+        return self
     
     def saveto(self, OUTDIR = '', FILE_NAME = ''):
         '''
             Executes the query to retrieve the Geomaterials with keywords and saves the results to a specified directory.
 
             Args:
                 OUTDIR (str): The directory path where the retrieved Geomaterials will be saved. If not provided, the current directory will be used.
@@ -1490,23 +1532,21 @@
                 None
 
             Example:
                 >>> gdr = GeomaterialDictRetriever()
                 >>> gdr.saveto("/path/to/directory", "geoDict")
         '''
 
-        print("Retrieving Geomaterials. This may take a while... ")
-
         params = self._params
         end_point = self.end_point
         outdir = OUTDIR
         file_name = FILE_NAME
 
         ma = mindat_api.MindatApi()
-        ma.get_mindat_item(params, end_point, outdir, file_name)
+        ma.download_mindat_json(params, end_point, outdir, file_name)
 
         # reset the query parameters in case the user wants to make another query
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
             Executes the query to retrieve the list of geomaterials and saves the results to the current directory.
@@ -1521,37 +1561,34 @@
                 >>> gdr = GeomaterialDictRetriever()
                 >>> gdr.save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)   
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve the dictionary of geomaterials.
 
         Returns:
             dictionary.
 
         Example:
             >>> gdr = GeomaterialDictRetriever()
-            >>> geoDict = gdr.get_list()
+            >>> geoDict = gdr.get_dict()
 
         '''
-        
-        print("Retrieving geomaterials. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
 
         ma = mindat_api.MindatApi()
-        results = [ma.get_mindat_dict(params, end_point)]
+        results = ma.get_mindat_json(params, end_point)
         
         self._init_params()
         return results
         
 
 if __name__ == '__main__':
     gr = GeomaterialRetriever()
     # gr.cleavagetype('Distinct/Good').colour('blue').crystal_system(["Amorphous", "Hexagonal"]).save()
-    gr.id__in("3337, 114").save()
-    # print(gr.density_max('9').density_min(8).ordering('-name')._params)
+    gr.id__in("3337, 114").save()
```

### Comparing `openmindat-0.0.4/openmindat/geomaterials_search.py` & `openmindat-0.0.5/openmindat/geomaterials_search.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,20 +13,44 @@
     Usage:
         >>> gsr = GeomaterialSearchRetriever()
         >>> gsr.geomaterials_search("quartz, green, hexagonal").save()
 
     Press q to quit.
     """
     def __init__(self):
-       self._params = {}
-       self.end_point = 'geomaterials_search'
+        self._params = {}
+        self.end_point = 'geomaterials_search'
     
     def _init_params(self):
+        self.end_point = 'geomaterials_search'
         self._params.clear()
         self._params = {'format': 'json'}
+        self.page_size(1500)
+        
+    def page_size(self, PAGE_SIZE):
+        '''
+        Sets the number of results per page.
+
+        Args:
+            PAGE_SIZE (int): The number of results per page.
+
+        Returns:
+            self: The GeomaterialSearchRetriever object.
+
+        Example:
+            >>> gsr = GeomaterialSearchRetriever()
+            >>> gsr.page_size(500)
+            >>> gsr.save()
+
+        '''
+        self._params.update({
+            'page_size': PAGE_SIZE
+        })
+
+        return self
 
     def geomaterials_search(self, KEYWORDS):
         '''
         Updates the query parameters to search for geomaterials based on specified keywords.
 
         Args:
             KEYWORDS (str): A string containing the keywords to search for. 
@@ -50,23 +74,22 @@
             Args:
                 OUTDIR (str): The directory path where the retrieved geomaterials will be saved. If not provided, the current directory will be used.
                 FILE_NAME (str): An optional file name, if no input is given it uses the end point as a name
 
             Returns:
                 None
         '''
-        print("Retrieving geomaterials. This may take a while... ")
         
         params = self._params
         end_point = self.end_point
         outdir = OUTDIR
         file_name = FILE_NAME
 
         ma = mindat_api.MindatApi()
-        ma.get_mindat_search(params, end_point, outdir, file_name)
+        ma.download_mindat_json(params, end_point, outdir, file_name)
 
         # reset the query parameters in case the user wants to make another query
         self._init_params()
 
     def save(self, FILE_NAME = ''):
         '''
             Executes the query to retrieve the list of geomaterials and saves the results to the current directory.
@@ -77,34 +100,32 @@
             Returns:
                 None
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve the geomaterial search data as a dictionary.
 
         Returns:
             List of dictionaries.
 
         Example:
             >>> gsr = geomaterialSeachRetriever()
-            >>> greenQuarts = gsr.geomaterial_search("quartz, green").get_list()
+            >>> greenQuarts = gsr.geomaterial_search("quartz, green").get_dict()
 
         '''
-        
-        print("Retrieving geomaterial search. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
         ma = mindat_api.MindatApi()
-        results = [ma.get_mindat_dict(params, end_point)]
+        results = ma.get_mindat_json(params, end_point)
         
         self._init_params()
         return results
 
 
 if __name__ == '__main__':
     gsr = GeomaterialSearchRetriever()
```

### Comparing `openmindat-0.0.4/openmindat/localities.py` & `openmindat-0.0.5/openmindat/localities.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
     def __init__(self):
         self._params = {}
         self.end_point = 'localities'
         self._init_params()
 
     def _init_params(self):
+        self.end_point = 'localities'
         self._params.clear()
         self._params = {'format': 'json'}
         self.page_size(1500)
 
     def country(self, COUNTRY_STR):
         '''
         Sets the country or region for the query.
@@ -385,23 +386,21 @@
                 None
 
             Example:
                 >>> lr = LocalitiesRetriever()
                 >>> lr.saveto("/path/to/directory", "france")
         '''
 
-        print("Retrieving localities. This may take a while... ")
-
         params = self._params
         end_point = self.end_point
         outdir = OUTDIR
         file_name = FILE_NAME
 
         ma = mindat_api.MindatApi()
-        ma.get_mindat_list(params, end_point, outdir, file_name)
+        ma.download_mindat_json(params, end_point, outdir, file_name)
 
         # reset the query parameters in case the user wants to make another query
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
             Executes the query to retrieve the list of localities and saves the results to the current directory.
@@ -416,34 +415,32 @@
                 >>> lr = LocalitiesRetriever()
                 >>> lr.save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve the list of localities and returns the json object.
 
         Returns:
             list of dictionaries.
 
         Example:
             >>> lr = LocalitiesRetriever()
-            >>> france = lr.country('France').get_list()
+            >>> france = lr.country('France').get_dict()
 
         '''
-        
-        print("Retrieving localities. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
         ma = mindat_api.MindatApi()
-        results = ma.get_mindat_list_object(params, end_point)
+        results = ma.get_mindat_json(params, end_point)
         
         self._init_params()
         return results
         
         
 class LocalitiesIdRetriever:
     """
@@ -456,22 +453,46 @@
 
     Attributes:
         id (int): An int to store id parameter.
     """
     
     def __init__(self):
         self.end_point = 'localities'
-        self.sub_endpoint = '0'
+        self.sub_endpoint = ''
         
         self._params = {}
         self._init_params()
 
     def _init_params(self):
         self._params.clear()
         self._params = {'format': 'json'}
+        self.end_point = 'localities'
+        self.sub_endpoint = ''
+        self.page_size(1500)
+        
+    def page_size(self, PAGE_SIZE):
+        '''
+        Sets the number of results per page.
+
+        Args:
+            PAGE_SIZE (int): The number of results per page.
+
+        Returns:
+            self: The LocalitiesIdRetriever object.
+            
+        Example:
+            >>> lidr = LocalitiesRetriever()
+            >>> lidr.page_size(50)
+            >>> lidr.saveto()
+        '''
+        self._params.update({
+            'page_size': PAGE_SIZE
+        })
+
+        return self
 
     def id(self, ID):
         '''
         Returns locality with matching id
 
         Args:
             id (INT): The locality id.
@@ -506,25 +527,23 @@
 
             Returns:
                 None
 
             Example:
                 >>> lir = LocalitiesIdRetriever()
                 >>> lir.saveto("/path/to/directory", "france")
-        '''
-
-        print("Retrieving localities. This may take a while... ")
-
+        ''' 
+        
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         outdir = OUTDIR
         file_name = FILE_NAME
 
         ma = mindat_api.MindatApi()
-        ma.get_mindat_item(params, end_point, outdir, file_name)
+        ma.download_mindat_json(params, end_point, outdir, file_name)
 
         # reset the query parameters in case the user wants to make another query
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
             Executes the query to retrieve the list of localities and saves the results to the current directory.
@@ -539,34 +558,32 @@
                 >>> lir = LocalitiesIdRetriever()
                 >>> lir.save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve locality with a corresponding id and returns a dictionary.
 
         Returns:
             List of Dictionaries.
 
         Example:
                 >>> lir = localitiesIdRetriever()
-                >>> locality5 = lir.id(5).get_list()
+                >>> locality5 = lir.id(5).get_dict()
 
         '''
-        
-        print("Retrieving localities. This may take a while... ")
        
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         
         ma = mindat_api.MindatApi()
-        results = [ma.get_mindat_dict(params, end_point)]
+        results = ma.get_mindat_json(params, end_point)
         
         self._init_params()
         return results
 
 if __name__ == '__main__':
     lr = LocalitiesRetriever()
     lr.country("UK").save()
```

### Comparing `openmindat-0.0.4/openmindat/localities_age.py` & `openmindat-0.0.5/openmindat/localities_age.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,20 +15,21 @@
         >>> lar = LocalitiesAgeRetriever()
         >>> lar.page(2).save()
 
     Press q to quit.
     """
     
     def __init__(self):
-       self.end_point = 'locality_age' 
+        self.end_point = 'locality_age' 
         
-       self._params = {}
-       self._init_params()
+        self._params = {}
+        self._init_params()
     
     def _init_params(self):
+        self.end_point = 'locality_age' 
         self._params.clear()
         self._params = {'format': 'json'}
         self.page_size(1500)
         
     def page_size(self, PAGE_SIZE):
         '''
         Sets the number of results per page.
@@ -85,28 +86,22 @@
             Returns:
                 None
 
             Example:
                 >>> lar = LocalityAgeRetriever()
                 >>> lar.saveto("/path/to/directory")
         '''
-        
-        print("Retrieving localities. This may take a while... ")
 
         params = self._params
         outdir = OUTDIR
         end_point = self.end_point
         file_name = FILE_NAME
         
         ma = mindat_api.MindatApi()
-        
-        if "page" in params:
-            ma.get_mindat_item(params, end_point, outdir, file_name)
-        else:
-            ma.get_mindat_list(params, end_point, outdir, file_name)
+        ma.download_mindat_json(params, end_point, outdir, file_name)
             
 
         # Reset the query parameters in case the user wants to make another query.
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
@@ -122,38 +117,32 @@
                 >>> lar = LocalitiesAgeRetriever()
                 >>> lar.page(2).save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve the locality age data as a list of dictionaries.
 
         Returns:
             list of dictionaries.
 
         Example:
                 >>> lar = LocalitiesAgeRetriever()
-                >>> secondAgePage = lar.page(2).get_list()
+                >>> secondAgePage = lar.page(2).get_dict()
 
         '''
-        
-        print("Retrieving localities search. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
         ma = mindat_api.MindatApi()
-        
-        if "page" in params:
-            results = [ma.get_mindat_dict(params, end_point)]
-        else:
-            results = ma.get_mindat_list_object(params, end_point)
+        results = ma.get_mindat_json(params, end_point)
             
         self._init_params()
         return results
         
         
 class LocalitiesAgeIdRetriever:
     """
@@ -169,23 +158,48 @@
         >>> lair = LocalitiesAgeIdRetriever()
         >>> lair.id(5).save()
 
     Press q to quit.
     """
     
     def __init__(self):
-       self.end_point = 'locality_age'
-       self.sub_endpoint = ''
+        self.end_point = 'locality_age'
+        self.sub_endpoint = ''
         
-       self._params = {}
-       self._init_params()
+        self._params = {}
+        self._init_params()
     
     def _init_params(self):
+        self.end_point = 'locality_age'
+        self.sub_endpoint = ''
         self._params.clear()
+        self.page_size(1500)
         self._params = {'format': 'json'}
+        
+    def page_size(self, PAGE_SIZE):
+        '''
+        Sets the number of results per page.
+
+        Args:
+            PAGE_SIZE (int): The number of results per page.
+
+        Returns:
+            self: The LocalitiesAgeIdRetriever object.
+
+        Example:
+            >>> laidr = LocalitiesAgeIdRetriever()
+            >>> laidr.page_size(2)
+            >>> laidr.save()
+
+        '''
+        self._params.update({
+            'page_size': PAGE_SIZE
+        })
+
+        return self
     
     def id(self, ID):
         '''
         Returns a country with the matching ID
 
         Args:
             id (INT): The country id.
@@ -222,24 +236,22 @@
             Returns:
                 None
 
             Example:
                 >>> lair = LocalitiesAgeIdRetriever()
                 >>> lair.id(4).saveto("/path/to/directory")
         '''
-        
-        print("Retrieving localities. This may take a while... ")
 
         params = self._params
         outdir = OUTDIR
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         file_name = FILE_NAME
         
         ma = mindat_api.MindatApi()
-        ma.get_mindat_item(params, end_point, outdir, file_name)
+        ma.download_mindat_json(params, end_point, outdir, file_name)
 
         # Reset the query parameters in case the user wants to make another query.
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
             Executes the query to retrieve the list of locality data and saves the results to the current directory.
@@ -254,34 +266,32 @@
                 >>> lair = localitiesAgeIdRetriever()
                 >>> lair.id(2).save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve locality with a corresponding id and returns a dictionary.
 
         Returns:
             List of Dictionaries.
 
         Example:
                 >>> lair = localitiesAgeIdRetriever()
-                >>> localityAge2 = lair.id(2).get_list()
+                >>> localityAge2 = lair.id(2).get_dict()
 
         '''
-        
-        print("Retrieving localities. This may take a while... ")
        
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         
         ma = mindat_api.MindatApi()
-        results = [ma.get_mindat_dict(params, end_point)]
+        results = ma.get_mindat_json(params, end_point)
         
         self._init_params()
         return results
 
 if __name__ == '__main__':
     lair = LocalitiesAgeIdRetriever()
     lair.id(2).save()
```

### Comparing `openmindat-0.0.4/openmindat/localities_status.py` & `openmindat-0.0.5/openmindat/localities_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,20 +15,21 @@
         >>> lsr = LocalitiesStatusRetriever()
         >>> lsr.page(2).save()
 
     Press q to quit.
     """
     
     def __init__(self):
-       self.end_point = 'locality_status' 
+        self.end_point = 'locality_status' 
         
-       self._params = {}
-       self._init_params()
+        self._params = {}
+        self._init_params()
     
     def _init_params(self):
+        self.end_point = 'locality_status' 
         self._params.clear()
         self._params = {'format': 'json'}
         self.page_size(1500)
         
     def page_size(self, PAGE_SIZE):
         '''
         Sets the number of results per page.
@@ -86,27 +87,25 @@
                 None
 
             Example:
                 >>> lsr = LocalityStatusRetriever()
                 >>> lsr.saveto("/path/to/directory")
         '''
         
-        print("Retrieving localities. This may take a while... ")
-
         params = self._params
         outdir = OUTDIR
         end_point = self.end_point
         file_name = FILE_NAME
         
         ma = mindat_api.MindatApi()
         
         if "page" in params:
-            ma.get_mindat_item(params, end_point, outdir, file_name)
+            ma.download_mindat_json(params, end_point, outdir, file_name)
         else:
-            ma.get_mindat_list(params, end_point, outdir, file_name)
+            ma.download_mindat_json(params, end_point, outdir, file_name)
             
 
         # Reset the query parameters in case the user wants to make another query.
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
@@ -122,38 +121,32 @@
                 >>> lsr = LocalitiesStatusRetriever()
                 >>> lsr.save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve the locality status data as a list of dictionaries.
 
         Returns:
             list of dictionaries.
 
         Example:
                 >>> lsr = LocalitiesStatusRetriever()
-                >>> secondAgePage = lsr.page(2).get_list()
+                >>> secondAgePage = lsr.page(2).get_dict()
 
         '''
-        
-        print("Retrieving localities search. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
         ma = mindat_api.MindatApi()
-        
-        if "page" in params:
-            results = [ma.get_mindat_dict(params, end_point)]
-        else:
-            results = ma.get_mindat_list_object(params, end_point)
+        results = ma.get_mindat_json(params, end_point)
             
         self._init_params()
         return results
         
         
 class LocalitiesStatusIdRetriever:
     """
@@ -169,24 +162,49 @@
         >>> lsir = LocalitiesStatusIdRetriever()
         >>> lsir.id(5).save()
 
     Press q to quit.
     """
     
     def __init__(self):
-       self.end_point = 'locality_status' 
-       self.sub_endpoint = ''
+        self.end_point = 'locality_status' 
+        self.sub_endpoint = ''
         
-       self._params = {}
-       self._init_params()
+        self._params = {}
+        self._init_params()
     
     def _init_params(self):
+        self.end_point = 'locality_status' 
+        self.sub_endpoint = ''
         self._params.clear()
+        self.page_size(1500)
         self._params = {'format': 'json'}
     
+    def page_size(self, PAGE_SIZE):
+        '''
+        Sets the number of results per page.
+
+        Args:
+            PAGE_SIZE (int): The number of results per page.
+
+        Returns:
+            self: The LocalitiesStatusIdRetriever object.
+
+        Example:
+            >>> lsidr = LocalitiesStatusIdRetriever()
+            >>> lsidr.page_size(1500)
+            >>> lsidr.save()
+
+        '''
+        self._params.update({
+            'page_size': PAGE_SIZE
+        })
+
+        return self
+    
     def id(self, ID):
         '''
         Returns a country with the matching ID
 
         Args:
             id (INT): The country id.
 
@@ -221,24 +239,22 @@
             Returns:
                 None
 
             Example:
                 >>> lsir = LocalitiesStatusIdRetriever()
                 >>> lsir.saveto("/path/to/directory")
         '''
-        
-        print("Retrieving localities. This may take a while... ")
 
         params = self._params
         outdir = OUTDIR
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         file_name = FILE_NAME
         
         ma = mindat_api.MindatApi()
-        ma.get_mindat_item(params, end_point, outdir, file_name)
+        ma.download_mindat_json(params, end_point, outdir, file_name)
 
         # Reset the query parameters in case the user wants to make another query.
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
             Executes the query to retrieve the list of locality data and saves the results to the current directory.
@@ -253,34 +269,32 @@
                 >>> lsir = localitiesStatusIdRetriever()
                 >>> lsir.save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve locality status with a corresponding id and returns a dictionary.
 
         Returns:
             List of Dictionaries.
 
         Example:
                 >>> lsir = localitiesStatusIdRetriever()
-                >>> localitystatus2 = lsir.id(2).get_list()
+                >>> localitystatus2 = lsir.id(2).get_dict()
 
         '''
-        
-        print("Retrieving localities. This may take a while... ")
        
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         
         ma = mindat_api.MindatApi()
-        results = [ma.get_mindat_dict(params, end_point)]
+        results = ma.get_mindat_json(params, end_point)
         
         self._init_params()
         return results
 
 if __name__ == '__main__':
     lsir = LocalitiesStatusIdRetriever()
     lsir.id(2).save()
```

### Comparing `openmindat-0.0.4/openmindat/localities_type.py` & `openmindat-0.0.5/openmindat/localities_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,33 +15,34 @@
         >>> ltr = LocalitiesTypeRetriever()
         >>> ltr.page(2).save()
 
     Press q to quit.
     """
     
     def __init__(self):
-       self.end_point = 'locality_type' 
+        self.end_point = 'locality_type' 
         
-       self._params = {}
-       self._init_params()
+        self._params = {}
+        self._init_params()
     
     def _init_params(self):
+        self.end_point = 'locality_type' 
         self._params.clear()
         self._params = {'format': 'json'}
         self.page_size(1500)
         
     def page_size(self, PAGE_SIZE):
         '''
         Sets the number of results per page.
 
         Args:
             PAGE_SIZE (int): The number of results per page.
 
         Returns:
-            self: The LocalitiesRetriever object.
+            self: The LocalitiesTypeRetriever object.
             
         Example:
             >>> ltr = LocalitiesTypeRetriever()
             >>> ltr.page_size(50)
             >>> ltr.saveto()
         '''
         self._params.update({
@@ -85,28 +86,26 @@
             Returns:
                 None
 
             Example:
                 >>> ltr = LocalityTypeRetriever()
                 >>> ltr.page(19).saveto("/path/to/directory")
         '''
-        
-        print("Retrieving localities. This may take a while... ")
 
         params = self._params
         outdir = OUTDIR
         end_point = self.end_point
         file_name = FILE_NAME
         
         ma = mindat_api.MindatApi()
         
         if "page" in params:
-            ma.get_mindat_item(params, end_point, outdir, file_name)
+            ma.download_mindat_json(params, end_point, outdir, file_name)
         else:
-            ma.get_mindat_list(params, end_point, outdir, file_name)
+            ma.download_mindat_json(params, end_point, outdir, file_name)
             
 
         # Reset the query parameters in case the user wants to make another query.
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
@@ -122,37 +121,31 @@
                 >>> ltr = LocalitiesTypeRetriever()
                 >>> ltr.save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve the locality type data as a list of dictionaries.
 
         Returns:
             list of dictionaries.
 
         Example:
                 >>> ltr = LocalitiesTypeRetriever()
-                >>> secondTypePage = ltr.page(2).get_list()
+                >>> secondTypePage = ltr.page(2).get_dict()
         '''
-        
-        print("Retrieving localities search. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
         ma = mindat_api.MindatApi()
-        
-        if "page" in params:
-            results = [ma.get_mindat_dict(params, end_point)]
-        else:
-            results = ma.get_mindat_list_object(params, end_point)
+        results = ma.get_mindat_json(params, end_point)
             
         self._init_params()
         return results
         
         
 class LocalitiesTypeIdRetriever:
     """
@@ -168,23 +161,47 @@
         >>> ltir = LocalitiesTypeIdRetriever()
         >>> ltir.id(5).save()
 
     Press q to quit.
     """
     
     def __init__(self):
-       self.end_point = 'locality_type' 
-       self.sub_endpoint = ''
+        self.end_point = 'locality_type' 
+        self.sub_endpoint = ''
         
-       self._params = {}
-       self._init_params()
+        self._params = {}
+        self._init_params()
     
     def _init_params(self):
+        self.end_point = 'locality_type' 
+        self.sub_endpoint = ''
         self._params.clear()
         self._params = {'format': 'json'}
+        self.page_size(1500)
+        
+    def page_size(self, PAGE_SIZE):
+        '''
+        Sets the number of results per page.
+
+        Args:
+            PAGE_SIZE (int): The number of results per page.
+
+        Returns:
+            self: The LocalitiesTypeIdRetriever object.
+            
+        Example:
+            >>> ltidr = LocalitiesTypeIdRetriever()
+            >>> ltidr.id(50)
+            >>> ltidr.saveto()
+        '''
+        self._params.update({
+            'page_size': PAGE_SIZE
+        })
+
+        return self
     
     def id(self, ID):
         '''
         Returns a country with the matching ID
 
         Args:
             id (INT): The country id.
@@ -220,24 +237,22 @@
             Returns:
                 None
 
             Example:
                 >>> ltir = LocalitiesTypeIdRetriever()
                 >>> ltir.id(2).saveto("/path/to/directory")
         '''
-        
-        print("Retrieving localities. This may take a while... ")
 
         params = self._params
         outdir = OUTDIR
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         file_name = FILE_NAME
         
         ma = mindat_api.MindatApi()
-        ma.get_mindat_item(params, end_point, outdir, file_name)
+        ma.download_mindat_json(params, end_point, outdir, file_name)
 
         # Reset the query parameters in case the user wants to make another query.
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
             Executes the query to retrieve the list of locality data and saves the results to the current directory.
@@ -252,34 +267,32 @@
                 >>> ltir = localitiesTypeIdRetriever()
                 >>> ltir.save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve locality type with a corresponding id and returns a dictionary.
 
         Returns:
             List of Dictionaries.
 
         Example:
                 >>> ltir = localitiesTypeIdRetriever()
-                >>> localityType2 = ltir.id(2).get_list()
+                >>> localityType2 = ltir.id(2).get_dict()
 
         '''
-        
-        print("Retrieving localities. This may take a while... ")
        
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         
         ma = mindat_api.MindatApi()
-        results = [ma.get_mindat_dict(params, end_point)]
+        results = ma.get_mindat_json(params, end_point)
         
         self._init_params()
         return results
 
 if __name__ == '__main__':
     ltir = LocalitiesTypeIdRetriever()
     ltir.id(2).save()
```

### Comparing `openmindat-0.0.4/openmindat/locgeoregion2.py` & `openmindat-0.0.5/openmindat/locgeoregion2.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,20 +15,21 @@
         >>> grr = GeoRegionRetriever()
         >>> grr.page(2).save()
 
     Press q to quit.
     """
     
     def __init__(self):
-       self.end_point = 'locgeoregion2' 
+        self.end_point = 'locgeoregion2' 
         
-       self._params = {}
-       self._init_params()
+        self._params = {}
+        self._init_params()
     
     def _init_params(self):
+        self.end_point = 'locgeoregion2' 
         self._params.clear()
         self._params = {'format': 'json'}
         self.page_size(1500)
         
     def page_size(self, PAGE_SIZE):
         '''
         Sets the number of results per page.
@@ -85,28 +86,26 @@
             Returns:
                 None
 
             Example:
                 >>> grr = GeoRegionRetriever()
                 >>> grr.saveto("/path/to/directory")
         '''
-        
-        print("Retrieving localities. This may take a while... ")
 
         params = self._params
         outdir = OUTDIR
         end_point = self.end_point
         file_name = FILE_NAME
         
         ma = mindat_api.MindatApi()
         
         if "page" in params:
-            ma.get_mindat_item(params, end_point, outdir, file_name)
+            ma.download_mindat_json(params, end_point, outdir, file_name)
         else:
-            ma.get_mindat_list(params, end_point, outdir, file_name)
+            ma.download_mindat_json(params, end_point, outdir, file_name)
             
 
         # Reset the query parameters in case the user wants to make another query.
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
@@ -122,37 +121,31 @@
                 >>> grr = GeoRegionRetriever()
                 >>> grr.page(3).save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve the geoRegion data as a list of dictionaries.
 
         Returns:
             list of dictionaries.
 
         Example:
                 >>> grr = GeoRegionRetriever()
-                >>> georegion3 = grr.page(3).get_list()
+                >>> georegion3 = grr.page(3).get_dict()
         '''
-        
-        print("Retrieving local geoRegion search. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
         ma = mindat_api.MindatApi()
-        
-        if "page" in params:
-            results = [ma.get_mindat_dict(params, end_point)]
-        else:
-            results = ma.get_mindat_list_object(params, end_point)
+        results = ma.get_mindat_json(params, end_point)
             
         self._init_params()
         return results
             
             
 if __name__ == '__main__':
     grr = GeoRegionRetriever()
```

### Comparing `openmindat-0.0.4/openmindat/locobject.py` & `openmindat-0.0.5/openmindat/locobject.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,23 @@
         >>> lor = LocobjectRetriever()
         >>> lor.id(5).save()
 
     Press q to quit.
     """
     
     def __init__(self):
-       self.end_point = 'locobject' 
-       self.sub_endpoint = ''
+        self.end_point = 'locobject' 
+        self.sub_endpoint = ''
         
-       self._params = {}
-       self._init_params()
+        self._params = {}
+        self._init_params()
     
     def _init_params(self):
+        self.end_point = 'locobject' 
+        self.sub_endpoint = ''
         self._params.clear()
         self._params = {'format': 'json'}
     
     def id(self, ID):
         '''
         Returns a loc object with the matching ID
 
@@ -67,24 +69,22 @@
             Returns:
                 None
 
             Example:
                 >>> lor = LocobjectRetriever()
                 >>> lor.saveto("/path/to/directory")
         '''
-        
-        print("Retrieving loc object. This may take a while... ")
 
         params = self._params
         outdir = OUTDIR
         end_point =  '/'.join([self.end_point, self.sub_endpoint])
         file_name = FILE_NAME
         
         ma = mindat_api.MindatApi()
-        ma.get_mindat_item(params, end_point, outdir, file_name)
+        ma.download_mindat_json(params, end_point, outdir, file_name)
 
         # Reset the query parameters in case the user wants to make another query.
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
             Executes the query to retrieve the list of loc object data and saves the results to the current directory.
@@ -99,35 +99,33 @@
                 >>> lor = LocobjectRetriever()
                 >>> lor.id(3).save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve locobject with a corresponding id and returns a dictionary.
 
         Returns:
             List of Dictionaries.
 
         Example:
             >>> lor = LocobjectRetriever()
             >>> lor.id(2)
-            >>> loco2 = lor.get_list()
+            >>> loco2 = lor.get_dict()
 
         '''
-        
-        print("Retrieving locObject. This may take a while... ")
        
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         
         ma = mindat_api.MindatApi()
-        results = [ma.get_mindat_dict(params, end_point)]
+        results = ma.get_mindat_json(params, end_point)
         
         self._init_params()
         return results
 
 if __name__ == '__main__':
     lor = LocobjectRetriever()
     lor.id(2).save()
```

### Comparing `openmindat-0.0.4/openmindat/mindat_api.py` & `openmindat-0.0.5/openmindat/mindat_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,36 @@
+import os
 import re
-import requests
-from pathlib import Path
 import sys
 import json
+import yaml
+import requests
+from pathlib import Path
 from datetime import datetime
 import getpass
-import yaml
-import os
 
 
+def in_notebook():
+    '''
+        Check if the package is running in notebook, e.g., Jupyter or Colab
+        return type: Bool
+    '''
+    try:
+        from IPython import get_ipython
+        if 'IPKernelApp' not in get_ipython().config:  # Check if not within an IPython kernel
+            return False
+    except (ImportError, AttributeError):
+        return False
+    return True
+
+if in_notebook():
+    from tqdm.notebook import tqdm
+else:
+    from tqdm import tqdm
+
 class MindatApiKeyManeger:
     def __init__(self):
         pass
 
     def inspect_stored_api_key(self):
         try:
             env_api_key = os.environ["MINDAT_API_KEY"]
@@ -112,17 +130,15 @@
     def __init__(self):
         self._api_key = None
         self._prepare_api_key()
 
         self.MINDAT_API_URL = "https://api.mindat.org"
         self._headers = {'Authorization': 'Token '+ self._api_key}
         self.params = {'format': 'json'}
-        # self.endpoint = "/items/"
         self.data_dir = './mindat_data/'
-        Path(self.data_dir).mkdir(parents=True, exist_ok=True)
 
     def _prepare_api_key(self):
         mam = MindatApiKeyManeger()
 
         if False == mam.inspect_stored_api_key():
             mam.get_api_key_input()
 
@@ -149,201 +165,116 @@
         
         #input sanitization
         if invalid_symbols:
             raise ValueError(f"Invalid characters in file name: {invalid_symbols}")  
         
         #creating filepath
         if '' == OUTDIR:
-            return Path(self.data_dir, file_name.replace('/', '_') + '.json')
+            out_dir = Path(self.data_dir)
         else:
-            return Path(OUTDIR, file_name.replace('/', '_') + '.json')
-    
-    def get_mindat_search(self, QUERY_DICT, END_POINT, OUTDIR = '', FILE_NAME = ''):
-        params = QUERY_DICT
-    
-        end_point = END_POINT
-        file_name = FILE_NAME if FILE_NAME else END_POINT        
+            out_dir = Path(OUTDIR)
         
-        file_path = self.get_file_path(OUTDIR, file_name)
-
-        with open(file_path, 'w') as f:
-
-            params = QUERY_DICT
-
-            response = requests.get(self.MINDAT_API_URL+ "/" + end_point + "/",
-                            params=params,
-                            headers=self._headers)
-            
-            try:
-                result_data = response.json()
-            except:
-                print("Error: " + str(response.json()))
-                return
-
-            json_data = {"results": result_data}
-
-            json.dump(json_data, f, indent=4)
-
-        print("Successfully saved " + str(len(json_data['results'])) + " entries to " + str(file_path.resolve()))
-
-
-    def print_the_result(self, JSONFILE, FILENAME):
-        print("Successfully retrieved", len(JSONFILE['results']), "items in", FILENAME, '. ')
+        out_dir.mkdir(parents=True, exist_ok=True)
+        return Path(out_dir, file_name.replace('/', '_') + '.json')
 
 
     def get_datetime(self):
         # use datetime to get current date and time
         now = datetime.now()
         dt_string = now.strftime("%m%d%Y%H%M%S")
         return dt_string        
-
-    def get_mindat_list(self, QUERY_DICT, END_POINT, OUTDIR = '', FILE_NAME = ''):
+    
+        
+    def get_mindat_json(self, PARAM_DICT, END_POINT):
         '''
             get all items in a list
             Since this API has a limit of 1500 items per page,
             we need to loop through all pages and save them to a single json file
         '''
-
+        params = PARAM_DICT
         end_point = END_POINT
-        file_name = FILE_NAME if FILE_NAME else END_POINT        
-        
-        file_path = self.get_file_path(OUTDIR, file_name)
-
-        with open(file_path, 'w') as f:
 
-            params = QUERY_DICT
+        # Retrieve the first page of data
+        response = requests.get(self.MINDAT_API_URL+ "/" + end_point + "/",
+                        params=params,
+                        headers=self._headers)
+        try:
+            response_json = response.json()
+            result_data = response_json["results"]
+        except KeyError:
+            # This error indicates the result only has one page
+            # We will convert the result data into a list for consistency
+            result_data = [response_json]
+        except TypeError:
+            # This error indicates the result data is a list instead of a dict
+            # We will pass the response result directly
+            result_data = response_json
+        except:
+            raise ValueError(str(response.reason))
+        
+        # Format the obtained data in a JSON dict
+        json_data = {"results": result_data}
 
-            if len(params) <= 2 and 'format' in params and 'page_size' in params:
-                confirm = input("The query dict only has 'format' and 'page_size' keys. Do you confirm this query? (y/n): ")
-                if confirm.lower() != 'y':
-                    sys.exit("Query not confirmed. Exiting...")
-
-            response = requests.get(self.MINDAT_API_URL+ "/" + end_point + "/",
-                            params=params,
-                            headers=self._headers)
-            
+        # Check if the query involves multiple pages
+        multipage_flag = self._is_multipage_query(params, response.json())
         
-            try:
-                result_data = response.json()["results"]
-            except:
-                print("Error: " + str(response.reason))
-                return
-            
-            json_data = {"results": result_data}
+        if True == multipage_flag:
+            # Create the progress bar
+            total_item = response.json().get("count", None)
+            item_per_request = len(response.json()["results"])
+            pbar = tqdm(total=total_item, desc="Fetching data") if total_item is not None else tqdm(desc="Fetching data")
+            pbar.update(item_per_request)
 
+            # Try if multipage download is needed
             while True:
                 try:
                     next_url = response.json()["next"]
                     response = requests.get(next_url, headers=self._headers)
-                    json_data["results"] += response.json()['results']
-                except requests.exceptions.MissingSchema as e:
+                    new_results = response.json()['results']
+                    json_data["results"] += new_results
+                    pbar.update(len(new_results))
+                except requests.exceptions.MissingSchema:
                     # This error indicates the `next_url` is none
-                    # i.e., we've reached the end of the results
+                    # i.e., No more pages to fetch
                     break
 
-            json.dump(json_data, f, indent=4)            
-        print("Successfully saved " + str(len(json_data['results'])) + " entries to " + str(file_path.resolve()))
-        
-    def get_mindat_item(self, QUERY_DICT, END_POINT, OUTDIR = '', FILE_NAME = ''):
-        '''
-            return one item.
-        '''
-        
-        end_point = END_POINT
-        file_name = FILE_NAME if FILE_NAME else END_POINT  
-        
-        file_path = self.get_file_path(OUTDIR, file_name)
+            # Close the progress bar
+            pbar.close()
+            
+        return json_data
+    
+    def _is_multipage_query(self, PARAM, RAW_JSON):
+        if 'page' in PARAM:
+            return False
         
-        with open(file_path, 'w') as f:
-
-            params = QUERY_DICT
+        raw_json = RAW_JSON
+        try:
+            result_data = raw_json["results"]
+        except:
+            return False
 
-            if len(params) <= 2 and 'format' in params and 'page_size' in params:
-                confirm = input("The query dict only has 'format' and 'page_size' keys. Do you confirm this query? (y/n): ")
-                if confirm.lower() != 'y':
-                    sys.exit("Query not confirmed. Exiting...")
-
-            response = requests.get(self.MINDAT_API_URL+ "/" + end_point + "/",
-                            params=params,
-                            headers=self._headers)
-            
-            try:
-                result_data = response.json()
-            except:
-                print("Error: " + str(response.json()))
-                return
-            
-            json_data = {"results": result_data}
+        return True
 
-            json.dump(json_data, f, indent=4)
-        print("Successfully saved item to " + str(file_path.resolve()))
-        
-    def get_mindat_list_object(self, QUERY_DICT, END_POINT):
+    def download_mindat_json(self, QUERY_DICT, END_POINT, OUTDIR = '', FILE_NAME = ''):
         '''
-            get all items in a list and returns it to a list of dictionaries
-            Since this API has a limit of 1500 items per page,
+            get all items in a list
+            Since this API has a limit of 1000 items per page,
             we need to loop through all pages and save them to a single json file
         '''
+        # get the json data
+        json_data = self.get_mindat_json(QUERY_DICT, END_POINT)
 
-        end_point = END_POINT
-
-        params = QUERY_DICT
-
-        if len(params) <= 2 and 'format' in params and 'page_size' in params:
-            confirm = input("The query dict only has 'format' and 'page_size' keys. Do you confirm this query? (y/n): ")
-            if confirm.lower() != 'y':
-                sys.exit("Query not confirmed. Exiting...")
-
-        response = requests.get(self.MINDAT_API_URL+ "/" + end_point + "/",
-                        params=params,
-                        headers=self._headers)
-            
-        try:
-            result_data = response.json()["results"]
-        except:
-            print("Error: " + str(response.json()))
-            return
-            
-        json_data = result_data
+        # The default output name is same as the endpoint
+        file_name = FILE_NAME if FILE_NAME else END_POINT   
 
-        while True:
-            try:
-                next_url = response.json()["next"]
-                response = requests.get(next_url, headers=self._headers)
-                json_data += response.json()['results']
-
-            except requests.exceptions.MissingSchema as e:
-                # This error indicates the `next_url` is none
-                # i.e., we've reached the end of the results
-                break
-        
-        return json_data
-    
-    def get_mindat_dict(self, QUERY_DICT, END_POINT):
-        '''
-            return one item to an object as a dictionary.
-        '''
-        end_point = END_POINT
-        params = QUERY_DICT
+        # Getting the directory for the output file
+        file_path = self.get_file_path(OUTDIR, file_name)
 
-        if len(params) <= 2 and 'format' in params and 'page_size' in params:
-            confirm = input("The query dict only has 'format' and 'page_size' keys. Do you confirm this query? (y/n): ")
-            if confirm.lower() != 'y':
-                sys.exit("Query not confirmed. Exiting...")
+        # Create and write the json data to the file
+        with open(file_path, 'w') as f:
+            json.dump(json_data, f, indent=4)   
 
-        response = requests.get(self.MINDAT_API_URL+ "/" + end_point + "/",
-                        params=params,
-                        headers=self._headers)
-        
-        try:
-            result_data = response.json()
-        except:
-            print("Error: " + str(response.json()))
-            return
-            
-        json_data = result_data
-        
-        return json_data
+        print("Successfully saved " + str(len(json_data['results'])) + " entries to " + str(file_path.resolve()))
         
 if __name__ == '__main__':
     # test if api key is valid
     ma = MindatApi()
```

### Comparing `openmindat-0.0.4/openmindat/minerals_ima.py` & `openmindat-0.0.5/openmindat/minerals_ima.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     '''
     def __init__(self):
         self.end_point = 'minerals_ima'
         self._params = {}
         self._init_params()
 
     def _init_params(self):
+        self.end_point = 'minerals_ima'
         self._params.clear()
         self._params = {'format': 'json'}
         self.page_size(1500)
 
     def expand(self, EXPAND_FIELDS):
         '''
         Expand the query to include related minerals and select specific fields to expand.
@@ -109,14 +110,15 @@
             'id__in': ids
         })
 
         return self
 
     def ima(self, IS_IMA):
         '''
+            This filter is probably not working as intended. Just ignore it for now.
             Include IMA-approved names only (1) / to be determined(0)
 
             Args:
                 IS_IMA (int): The IMA status to filter the query. 1 for IMA-approved names only, 0 is not clear.
 
             Returns:
                 self: The MineralsIMARetriever object.
@@ -265,23 +267,21 @@
                 None
 
             Example:
                 >>> mir = MineralsIMARetriever()
                 >>> mir.saveto("/path/to/directory")
         '''
 
-        print("Retrieving geomaterials. This may take a while... ")
-
         params = self._params
         end_point = self.end_point
         outdir = OUTDIR
         file_name = FILE_NAME
 
         ma = mindat_api.MindatApi()
-        ma.get_mindat_list(params, end_point, outdir, file_name)
+        ma.download_mindat_json(params, end_point, outdir, file_name)
 
         # reset the query parameters in case the user wants to make another query
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
             Executes the query to retrieve the list of geomaterials and saves the results to the current directory.
@@ -296,34 +296,32 @@
                 >>> mir = MineralsIMARetriever()
                 >>> mir.save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve the list of mineral data and returns the json object.
 
         Returns:
             list of dictionaries.
 
         Example:
                 >>> mir = MineralsIMARetriever()
-                >>> quartsIMA = mir.q('quartz').get_list()
+                >>> quartsIMA = mir.q('quartz').get_dict()
 
         '''
-        
-        print("Retrieving minerals. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
         ma = mindat_api.MindatApi()
-        results = ma.get_mindat_list_object(params, end_point)
+        results = ma.get_mindat_json(params, end_point)
         
         self._init_params()
         return results
         
         
 class MineralsIdRetriever:
     """
@@ -336,22 +334,47 @@
 
     Attributes:
         id (int): An int to store id parameter.
     """
     
     def __init__(self):
         self.end_point = 'minerals_ima'
-        self.sub_endpoint = '0'
+        self.sub_endpoint = ''
         
         self._params = {}
         self._init_params()
 
     def _init_params(self):
+        self.end_point = 'minerals_ima'
+        self.sub_endpoint = ''
         self._params.clear()
         self._params = {'format': 'json'}
+        self.page_size(1500)
+        
+    def page_size(self, PAGE_SIZE):
+        '''
+        Sets the number of results per page.
+
+        Args:
+            PAGE_SIZE (int): The number of results per page.
+
+        Returns:
+            self: The MineralsIdRetriever object.
+
+        Example:
+            >>> Midr = MineralsIdRetriever()
+            >>> Midr.page_size(50)
+            >>> Midr.save()
+
+        '''
+        self._params.update({
+            'page_size': PAGE_SIZE
+        })
+
+        return self
 
     def id(self, ID):
         '''
         Returns locality with matching id
 
         Args:
             id (INT): The locality id.
@@ -388,23 +411,21 @@
                 None
 
             Example:
                 >>> midr = MineralsIdRetriever()
                 >>> midr.id(3).saveto("/path/to/directory", "Mineral_ima_id")
         '''
 
-        print("Retrieving Minerals. This may take a while... ")
-
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         outdir = OUTDIR
         file_name = FILE_NAME
 
         ma = mindat_api.MindatApi()
-        ma.get_mindat_item(params, end_point, outdir, file_name)
+        ma.download_mindat_json(params, end_point, outdir, file_name)
 
         # reset the query parameters in case the user wants to make another query
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
             Executes the query to retrieve the list of minerals and saves the results to the current directory.
@@ -419,34 +440,32 @@
                 >>> midr = MineralsIdRetriever()
                 >>> midr.id(3).save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve mineral IMA status with a corresponding id and returns a dictionary.
 
         Returns:
             List of Dictionaries.
 
         Example:
                 >>> midr = MineralsIdRetriever()
-                >>> ima9 = midr.id(9).get_list()
+                >>> ima9 = midr.id(9).get_dict()
 
         '''
-        
-        print("Retrieving minerals. This may take a while... ")
        
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         
         ma = mindat_api.MindatApi()
-        results = [ma.get_mindat_dict(params, end_point)]
+        results = ma.get_mindat_json(params, end_point)
         
         self._init_params()
         return results
 
 
 if __name__ == '__main__':
     mir = MineralsIMARetriever()
```

### Comparing `openmindat-0.0.4/openmindat/nickel_strunz.py` & `openmindat-0.0.5/openmindat/nickel_strunz.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,23 +20,48 @@
         >>> sr = StrunzRetriever()
         >>> sr.classes().save()
 
     Press q to quit.
     """
     
     def __init__(self):
-       self.end_point = 'nickel-strunz-10'
-       self.sub_endpoint = '' 
+        self.end_point = 'nickel-strunz-10'
+        self.sub_endpoint = '' 
         
-       self._params = {}
-       self._init_params()
+        self._params = {}
+        self._init_params()
     
     def _init_params(self):
+        self.end_point = 'nickel-strunz-10'
+        self.sub_endpoint = '' 
         self._params.clear()
         self._params = {'format': 'json'}
+        self.page_size(1500)
+
+    def page_size(self, PAGE_SIZE):
+        '''
+        Sets the number of results per page.
+
+        Args:
+            PAGE_SIZE (int): The number of results per page.
+
+        Returns:
+            self: The StrunzRetriever object.
+
+        Example:
+            >>> sr = StrunzRetriever()
+            >>> sr.page_size(1500)
+            >>> sr.save()
+
+        '''
+        self._params.update({
+            'page_size': PAGE_SIZE
+        })
+
+        return self
         
     def retrieve(self):
         '''
         Returns Nickel Strunz classification
         Not yet working
 
         Returns:
@@ -142,28 +167,26 @@
             Returns:
                 None
 
             Example:
                 >>> sr = strunzRetriever()
                 >>> sr.families.saveto("/path/to/directory")
         '''
-        
-        print("Retrieving nickel strunz Data. This may take a while... ")
 
         params = self._params
         outdir = OUTDIR
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         file_name = FILE_NAME
         
         ma = mindat_api.MindatApi()
         
         if 'classes' in self.sub_endpoint:
-            ma.get_mindat_item(params, end_point, outdir, file_name)
+            ma.download_mindat_json(params, end_point, outdir, file_name)
         else:
-            ma.get_mindat_list(params, end_point, outdir, file_name)
+            ma.download_mindat_json(params, end_point, outdir, file_name)
 
         # Reset the query parameters in case the user wants to make another query.
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
             Executes the query to retrieve the list of nickel strunz data and saves the results to the current directory.
@@ -178,37 +201,31 @@
                 >>> sr = StrunzRetriever()
                 >>> sr.save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve the nickel_strunz data as a list of dictionaries.
 
         Returns:
             list of dictionaries.
 
         Example:
                 >>> sr = StrunzRetriever()
-                >>> nickelStrunzClasses = sr.classes().get_list()
+                >>> nickelStrunzClasses = sr.classes().get_dict()
         '''
-        
-        print("Retrieving nickel-strunz. This may take a while... ")
        
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         
         ma = mindat_api.MindatApi()
-        
-        if "classes" in self.sub_endpoint:
-            results = [ma.get_mindat_dict(params, end_point)]
-        else:
-            results = ma.get_mindat_list_object(params, end_point)
+        results = ma.get_mindat_json(params, end_point)
             
         self._init_params()
         return results
 
 
 if __name__ == '__main__':
     sr = StrunzRetriever()
```

### Comparing `openmindat-0.0.4/openmindat/photo_count.py` & `openmindat-0.0.5/openmindat/photo_count.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,22 +13,46 @@
         >>> pcr = PhotoCountRetriever()
         >>> pcr.save()
 
     Press q to quit.
     """
     
     def __init__(self):
-       self.end_point = 'photocount' 
+        self.end_point = 'photocount' 
         
-       self._params = {}
-       self._init_params()
+        self._params = {}
+        self._init_params()
     
     def _init_params(self):
+        self.end_point = 'photocount' 
         self._params.clear()
         self._params = {'format': 'json'}
+        self.page_size(1500)
+
+    def page_size(self, PAGE_SIZE):
+        '''
+        Sets the number of results per page.
+
+        Args:
+            PAGE_SIZE (int): The number of results per page.
+
+        Returns:
+            self: The PhotoCountRetriever object.
+
+        Example:
+            >>> pcr = PhotoCountRetriever()
+            >>> pcr.page_size(1500)
+            >>> pcr.save()
+
+        '''
+        self._params.update({
+            'page_size': PAGE_SIZE
+        })
+
+        return self
     
     #when fixed check if this needs get item or get list
     def saveto(self, OUTDIR = '', FILE_NAME = ''):
         '''
             Executes the query to retrieve the photo count with keywords and saves the results to a specified directory.
 
             Args:
@@ -38,24 +62,22 @@
             Returns:
                 None
 
             Example:
                 >>> pcr = PhotoCountRetriever()
                 >>> pcr.saveto("/path/to/directory")
         '''
-        
-        print("Retrieving photo count. This may take a while... ")
 
         params = self._params
         outdir = OUTDIR
         end_point = self.end_point
         file_name = FILE_NAME
         
         ma = mindat_api.MindatApi()
-        ma.get_mindat_item(params, end_point, outdir, file_name)
+        ma.download_mindat_json(params, end_point, outdir, file_name)
 
         # Reset the query parameters in case the user wants to make another query.
         self._init_params()
     
     def save(self, FILE_NAME = ''):
         '''
             Executes the query to retrieve the list of photo count data and saves the results to the current directory.
@@ -70,34 +92,32 @@
                 >>> pcr = PhotoCountRetriever()
                 >>> pcr.save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve photo counts and returns a dictionary.
 
         Returns:
             List of Dictionaries.
 
         Example:
                 >>> pcr = PhotoCountRetriever()
-                >>> photoCount = pcr.get_list()
+                >>> photoCount = pcr.get_dict()
 
         '''
-        
-        print("Retrieving photo count. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
         ma = mindat_api.MindatApi()
-        results = [ma.get_mindat_dict(params, end_point)]
+        results = ma.get_mindat_json(params, end_point)
         
         self._init_params()
         return results
 
 if __name__ == '__main__':
     pcr = PhotoCountRetriever()
     pcr.save()
```

### Comparing `openmindat-0.0.4/openmindat.egg-info/PKG-INFO` & `openmindat-0.0.5/openmindat.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmindat
-Version: 0.0.4
+Version: 0.0.5
 Summary: An alpha version for OpenMindat package
 Home-page: https://github.com/ChuBL/OpenMindat
 Author: Jiyin Zhang
 Author-email: jiyinz@uidaho.edu
 License: Apache Software License
 Keywords: mindat openmindat mineral data python api
 Classifier: Development Status :: 3 - Alpha
@@ -48,33 +48,30 @@
 
 > If you do not have a Mindat API key, please refer to [How to Get My Mindat API Key or Token?](https://www.mindat.org/a/how_to_get_my_mindat_api_key)
 
 You can also set the API key by following the general queries.
 
 ### 1. Perform Detailed Queries on Geomaterials
 
-:exclamation: Temporarily Outage, see https://github.com/ChuBL/OpenMindat/issues/12
-
 ```python
-# Temporarily Outage, see https://github.com/ChuBL/OpenMindat/issues/12
 from openmindat import GeomaterialRetriever
 
 gr = GeomaterialRetriever()
 gr.density_min(2.0).density_max(5.0).crystal_system("Hexagonal")
 gr.elements_exc("Au,Ag")
-gr.saveto("./mindat_data")
+gr.save()
 ```
 
 ### 2. Retrieve IMA-Approved Minerals
 
 ```python
 from openmindat import MineralsIMARetriever
 
 mir = MineralsIMARetriever()
-mir.ima(1).fields("id,name,ima_formula,ima_year")
+mir.fields("id,name,ima_formula,ima_year")
 mir.saveto("./mindat_data", 'my_filename')
 ```
 
 ### 3. Search Geomaterials Using Keywords
 
 ```python
 from openmindat import GeomaterialSearchRetriever
@@ -82,15 +79,15 @@
 gsr = GeomaterialSearchRetriever()
 gsr.geomaterials_search("quartz, green, hexagonal")
 gsr.save("filename")
 
 # Alternatively, you can get the list object directly:
 gsr = GeomaterialSearchRetriever()
 gsr.geomaterials_search("ruby, red, hexagonal")
-print(gsr.get_list())
+print(gsr.get_dict())
 ```
 
 ### 4. Retrieve Localities
 
 :exclamation: Some country names, e.g., United States and United Kingdom, are not working due to server-side problems, which will be fixed in the future.
 
 ```python
@@ -99,15 +96,15 @@
 lr = LocalitiesRetriever()
 lr.country("France").txt("mine")
 lr.save()
 
 # Alternatively, you can get the list object directly:
 lr = LocalitiesRetriever()
 lr.country("Canada").description("mine")
-print(lr.get_list())
+print(lr.get_dict())
 ```
 
 ### 5. Retrieve Type Localities for IMA-Approved Mineral Species
 
 ```python
 from openmindat import GeomaterialRetriever
 
@@ -163,28 +160,39 @@
 
 ## License
 
 **Project Licence:** [Apache](LICENSE)
 
 **Mindat Data License:** [CC BY-NC-SA 4.0 DEED](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.en)
 
+The Mindat API is currently in beta test, and while access is free for all, please note that the data provided are not yet licensed for redistribution and are for private, non-commercial use only. Once launched, data will be available under an open-access license, but please always check the terms of use of the license before reusing these data.
+
 ## Author
 
 Jiyin Zhang, Clairmont Cory
 
 ## Acknowledgments
 
 <p float="left">
         <img src="https://github.com/ChuBL/OpenMindat/blob/main/Logo/mindat2017.png?raw=true"  width="25%">
         <img src="https://github.com/ChuBL/OpenMindat/blob/main/Logo/NSF_Official_logo_Low_Res.png?raw=true"  width="10%">
 </p>
 
 - This work is supported by NSF, Award #2126315.
 
-## Updating Logs
+## Upgrading Logs
+
+### 0.0.5
+**Released:** Apr 26, 2024
+
+- The `Internal Server Error` issue in v0.0.4 is fixed from the server side.
+- The get functions are now changed to `get_dict`.
+- Added progress bars for multiple-page queries.
+- Some other minor updates.
+
 
 ### 0.0.4
 **Released:** Apr 14, 2024
 
 - Tentative issue: Data queries involving multiple pages might return an `Internal Server Error` due to server-end issues. [Related GitHub issue](https://github.com/ChuBL/OpenMindat/issues/12)
 - Added support to getting list objects of obtained data in addition to saving it to local directories.
```

### Comparing `openmindat-0.0.4/openmindat.egg-info/SOURCES.txt` & `openmindat-0.0.5/openmindat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.4/setup.py` & `openmindat-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(name='openmindat',
-      version='0.0.4',
+      version='0.0.5',
       description='An alpha version for OpenMindat package',
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: Apache Software License',
         "Programming Language :: Python :: 3",
@@ -21,11 +21,12 @@
       url='https://github.com/ChuBL/OpenMindat',
       author='Jiyin Zhang',
       author_email='jiyinz@uidaho.edu',
       license='Apache Software License',
       packages=['openmindat'],
       install_requires=[
           'requests',
-          'PyYAML'
+          'PyYAML',
+          'tqdm'
       ],
       include_package_data=True,
       zip_safe=False)
```

