# Comparing `tmp/shipyard_tableau-0.2.0a2.tar.gz` & `tmp/shipyard_tableau-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_tableau-0.2.0a2.tar", max compression
+gzip compressed data, was "shipyard_tableau-0.2.1.tar", max compression
```

## Comparing `shipyard_tableau-0.2.0a2.tar` & `shipyard_tableau-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-05-12 18:48:21.844008 shipyard_tableau-0.2.0a2/README.md
--rw-r--r--   0        0        0      504 2024-04-22 19:08:25.769943 shipyard_tableau-0.2.0a2/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-12 18:48:21.844300 shipyard_tableau-0.2.0a2/shipyard_tableau/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 03:34:57.766724 shipyard_tableau-0.2.0a2/shipyard_tableau/cli/__init__.py
--rw-r--r--   0        0        0      397 2024-01-11 03:34:57.767260 shipyard_tableau-0.2.0a2/shipyard_tableau/cli/authtest.py
--rw-r--r--   0        0        0     4830 2024-04-22 19:08:25.764216 shipyard_tableau-0.2.0a2/shipyard_tableau/cli/download_view.py
--rw-r--r--   0        0        0     1741 2024-03-26 15:34:44.459652 shipyard_tableau-0.2.0a2/shipyard_tableau/cli/job_status.py
--rw-r--r--   0        0        0     5419 2024-04-01 15:54:40.974367 shipyard_tableau-0.2.0a2/shipyard_tableau/cli/refresh_resource.py
--rw-r--r--   0        0        0     1538 2024-03-26 15:34:44.460446 shipyard_tableau-0.2.0a2/shipyard_tableau/tableau.py
--rw-r--r--   0        0        0     9037 2024-03-26 15:35:00.430548 shipyard_tableau-0.2.0a2/shipyard_tableau/tableau_utils.py
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 shipyard_tableau-0.2.0a2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:21.844008 shipyard_tableau-0.2.1/README.md
+-rw-r--r--   0        0        0      502 2024-04-26 06:21:53.470147 shipyard_tableau-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-05-12 18:48:21.844300 shipyard_tableau-0.2.1/shipyard_tableau/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-11 03:34:57.766724 shipyard_tableau-0.2.1/shipyard_tableau/cli/__init__.py
+-rw-r--r--   0        0        0      477 2024-04-26 06:22:46.433080 shipyard_tableau-0.2.1/shipyard_tableau/cli/authtest.py
+-rw-r--r--   0        0        0     4860 2024-04-23 15:02:35.316668 shipyard_tableau-0.2.1/shipyard_tableau/cli/download_view.py
+-rw-r--r--   0        0        0     1741 2024-03-26 15:34:44.459652 shipyard_tableau-0.2.1/shipyard_tableau/cli/job_status.py
+-rw-r--r--   0        0        0     5419 2024-04-01 15:54:40.974367 shipyard_tableau-0.2.1/shipyard_tableau/cli/refresh_resource.py
+-rw-r--r--   0        0        0     1464 2024-04-26 06:22:46.426600 shipyard_tableau-0.2.1/shipyard_tableau/tableau.py
+-rw-r--r--   0        0        0     9037 2024-03-26 15:35:00.430548 shipyard_tableau-0.2.1/shipyard_tableau/tableau_utils.py
+-rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 shipyard_tableau-0.2.1/PKG-INFO
```

### Comparing `shipyard_tableau-0.2.0a2/shipyard_tableau/cli/download_view.py` & `shipyard_tableau-0.2.1/shipyard_tableau/cli/download_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,17 @@
         args = get_args()
 
         # Set all file parameters
         destination_folder_name = shipyard.clean_folder_name(
             args.destination_folder_name
         )
         if destination_folder_name:
-            shipyard.create_folder_if_dne(destination_folder_name=destination_folder_name)
+            shipyard.create_folder_if_dne(
+                destination_folder_name=destination_folder_name
+            )
 
         destination_full_path = shipyard.combine_folder_and_file_name(
             folder_name=destination_folder_name, file_name=args.destination_file_name
         )
 
         server, connection = tableau_utils.connect_to_tableau(
             args.username,
```

### Comparing `shipyard_tableau-0.2.0a2/shipyard_tableau/cli/job_status.py` & `shipyard_tableau-0.2.1/shipyard_tableau/cli/job_status.py`

 * *Files identical despite different names*

### Comparing `shipyard_tableau-0.2.0a2/shipyard_tableau/cli/refresh_resource.py` & `shipyard_tableau-0.2.1/shipyard_tableau/cli/refresh_resource.py`

 * *Files identical despite different names*

### Comparing `shipyard_tableau-0.2.0a2/shipyard_tableau/tableau.py` & `shipyard_tableau-0.2.1/shipyard_tableau/tableau.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     def __init__(
         self, username: str, password: str, server_url: str, site: str = ""
     ) -> None:
         self.username = username
         self.password = password
         self.server_url = server_url
         self.site = site
-        super().__init__(username=username, password=password, site=site)
 
     def connect(self, sign_in_method, **kwargs):
         try:
             if sign_in_method not in ["username_password", "access_token"]:
                 logger.authtest(f"Invalid sign in method: {sign_in_method}")
                 return 1
             elif sign_in_method == "username_password":
```

### Comparing `shipyard_tableau-0.2.0a2/shipyard_tableau/tableau_utils.py` & `shipyard_tableau-0.2.1/shipyard_tableau/tableau_utils.py`

 * *Files identical despite different names*

### Comparing `shipyard_tableau-0.2.0a2/PKG-INFO` & `shipyard_tableau-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-tableau
-Version: 0.2.0a2
+Version: 0.2.1
 Summary: A local client for connecting and working with Tableau
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

