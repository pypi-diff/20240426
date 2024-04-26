# Comparing `tmp/cloudpy_org-1.4.9.tar.gz` & `tmp/cloudpy_org-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpy_org-1.4.9.tar", last modified: Sat Apr 20 07:41:39 2024, max compression
+gzip compressed data, was "dist\cloudpy_org-1.5.0.tar", last modified: Fri Apr 26 20:39:48 2024, max compression
```

## Comparing `cloudpy_org-1.4.9.tar` & `cloudpy_org-1.5.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 07:41:39.584452 cloudpy_org-1.4.9/
--rw-rw-rw-   0        0        0      935 2024-04-20 07:41:39.583853 cloudpy_org-1.4.9/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.4.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 07:41:39.461035 cloudpy_org-1.4.9/cloudpy_org/
--rw-rw-rw-   0        0        0     1794 2024-04-20 07:41:03.000000 cloudpy_org-1.4.9/cloudpy_org/__init__.py
--rw-rw-rw-   0        0        0    31386 2024-04-20 07:40:37.000000 cloudpy_org-1.4.9/cloudpy_org/aws.py
--rw-rw-rw-   0        0        0    12311 2024-04-20 07:40:33.000000 cloudpy_org-1.4.9/cloudpy_org/docs.py
--rw-rw-rw-   0        0        0     2618 2024-04-20 07:40:27.000000 cloudpy_org-1.4.9/cloudpy_org/imgedit.py
--rw-rw-rw-   0        0        0    49186 2024-04-20 07:40:22.000000 cloudpy_org-1.4.9/cloudpy_org/tools.py
--rw-rw-rw-   0        0        0     3696 2024-04-20 07:40:17.000000 cloudpy_org-1.4.9/cloudpy_org/web.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:41:39.559937 cloudpy_org-1.4.9/cloudpy_org.egg-info/
--rw-rw-rw-   0        0        0      935 2024-04-20 07:41:39.000000 cloudpy_org-1.4.9/cloudpy_org.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-04-20 07:41:39.000000 cloudpy_org-1.4.9/cloudpy_org.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 07:41:39.000000 cloudpy_org-1.4.9/cloudpy_org.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-20 07:41:39.000000 cloudpy_org-1.4.9/cloudpy_org.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-20 07:41:39.000000 cloudpy_org-1.4.9/cloudpy_org.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 07:41:39.584956 cloudpy_org-1.4.9/setup.cfg
--rw-rw-rw-   0        0        0     1324 2024-04-20 07:41:10.000000 cloudpy_org-1.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:39:48.583645 cloudpy_org-1.5.0/
+-rw-rw-rw-   0        0        0      935 2024-04-26 20:39:48.582644 cloudpy_org-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 20:39:48.438570 cloudpy_org-1.5.0/cloudpy_org/
+-rw-rw-rw-   0        0        0     1864 2024-04-26 20:38:32.000000 cloudpy_org-1.5.0/cloudpy_org/__init__.py
+-rw-rw-rw-   0        0        0    31386 2024-04-26 04:25:00.000000 cloudpy_org-1.5.0/cloudpy_org/aws.py
+-rw-rw-rw-   0        0        0     4309 2024-04-26 20:34:35.000000 cloudpy_org-1.5.0/cloudpy_org/client_usage.py
+-rw-rw-rw-   0        0        0    12311 2024-04-20 07:40:33.000000 cloudpy_org-1.5.0/cloudpy_org/docs.py
+-rw-rw-rw-   0        0        0     2618 2024-04-20 07:40:27.000000 cloudpy_org-1.5.0/cloudpy_org/imgedit.py
+-rw-rw-rw-   0        0        0    49186 2024-04-20 07:40:22.000000 cloudpy_org-1.5.0/cloudpy_org/tools.py
+-rw-rw-rw-   0        0        0     3696 2024-04-20 07:40:17.000000 cloudpy_org-1.5.0/cloudpy_org/web.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:39:48.559633 cloudpy_org-1.5.0/cloudpy_org.egg-info/
+-rw-rw-rw-   0        0        0      935 2024-04-26 20:39:46.000000 cloudpy_org-1.5.0/cloudpy_org.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-04-26 20:39:47.000000 cloudpy_org-1.5.0/cloudpy_org.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 20:39:46.000000 cloudpy_org-1.5.0/cloudpy_org.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-26 20:39:46.000000 cloudpy_org-1.5.0/cloudpy_org.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-26 20:39:46.000000 cloudpy_org-1.5.0/cloudpy_org.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 20:39:48.583645 cloudpy_org-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1324 2024-04-26 20:35:53.000000 cloudpy_org-1.5.0/setup.py
```

### Comparing `cloudpy_org-1.4.9/PKG-INFO` & `cloudpy_org-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy_org
-Version: 1.4.9
+Version: 1.5.0
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.4.9/cloudpy_org/__init__.py` & `cloudpy_org-1.5.0/cloudpy_org/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,15 @@
  'eu-west-1': {'long_name': 'Europe (Ireland)', 'code': 'euw1'},
  'eu-west-2': {'long_name': 'Europe (London)', 'code': 'euw2'},
  'eu-west-3': {'long_name': 'Europe (Paris)', 'code': 'euw3'},
  'eu-north-1': {'long_name': 'Europe (Stockholm)', 'code': 'eun1'},
  'sa-east-1': {'long_name': 'South America (São Paulo)', 'code': 'sae1'}}
 subscription_url = 'https://www.cloudpy.org'
 msh = 'secure'
-cloudpy_org_version='1.4.9'
+cloudpy_org_version='1.5.0'
 gsep = {'user_email_sep': '-0-', '@': '-1-', '.': '-2-'}
 from cloudpy_org.tools import processing_tools
 from cloudpy_org.docs import auto_document,convert_jupiter_notebook_to_html,documentation_from_folder
 from cloudpy_org.aws import aws_framework_manager,aws_framework_manager_client,gen_aws_auth_token,gen_new_service_token,configure_aws,get_my_aws_service_token,authenticate_with_token,delete_biscuit,co_token_auth
 from cloudpy_org.web import flask_website
-from cloudpy_org.imgedit import colors
+from cloudpy_org.imgedit import colors
+from cloudpy_org.client_usage import cloudpy_org_aws_framework_client
```

### Comparing `cloudpy_org-1.4.9/cloudpy_org/aws.py` & `cloudpy_org-1.5.0/cloudpy_org/aws.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.4.9/cloudpy_org/docs.py` & `cloudpy_org-1.5.0/cloudpy_org/docs.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.4.9/cloudpy_org/imgedit.py` & `cloudpy_org-1.5.0/cloudpy_org/imgedit.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.4.9/cloudpy_org/tools.py` & `cloudpy_org-1.5.0/cloudpy_org/tools.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.4.9/cloudpy_org/web.py` & `cloudpy_org-1.5.0/cloudpy_org/web.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.4.9/cloudpy_org.egg-info/PKG-INFO` & `cloudpy_org-1.5.0/cloudpy_org.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy-org
-Version: 1.4.9
+Version: 1.5.0
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.4.9/setup.py` & `cloudpy_org-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import path
 
 
 long_description = 'A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.'
 
 setup(
     name="cloudpy_org",
-    version="1.4.9",
+    version="1.5.0",
     description="Cloud data pipeline organization and automation library. Includes AWS framework manager API.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://www.cloudpy.org/",
     author="cloudpy.org",
     author_email="admin@cloudpy.org",
     license="MIT",
```

