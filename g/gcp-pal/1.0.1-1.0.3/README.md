# Comparing `tmp/gcp_pal-1.0.1.tar.gz` & `tmp/gcp_pal-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp_pal-1.0.1.tar", max compression
+gzip compressed data, was "gcp_pal-1.0.3.tar", max compression
```

## Comparing `gcp_pal-1.0.1.tar` & `gcp_pal-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0    23782 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/README.md
--rw-r--r--   0        0        0      760 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/__init__.py
--rw-r--r--   0        0        0    31402 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/bigquery.py
--rw-r--r--   0        0        0    13156 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/cloudfunctions.py
--rw-r--r--   0        0        0    13855 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/cloudrun.py
--rw-r--r--   0        0        0     7754 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/cloudscheduler.py
--rw-r--r--   0        0        0       42 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/config/__init__.py
--rw-r--r--   0        0        0      895 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/config/vars.py
--rw-r--r--   0        0        0    12490 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/firestore.py
--rw-r--r--   0        0        0     1674 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/pubsub.py
--rw-r--r--   0        0        0     3873 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/pydocker.py
--rw-r--r--   0        0        0     6860 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/pylogging.py
--rw-r--r--   0        0        0     4737 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/request.py
--rw-r--r--   0        0        0    23631 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/schema.py
--rw-r--r--   0        0        0     6332 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/secretmanager.py
--rw-r--r--   0        0        0       88 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/storage/__init__.py
--rw-r--r--   0        0        0     8735 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/storage/parquet.py
--rw-r--r--   0        0        0    17133 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/storage/storage.py
--rw-r--r--   0        0        0       82 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/utils/__init__.py
--rw-r--r--   0        0        0      935 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/utils/lazy_loader.py
--rw-r--r--   0        0        0    10898 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/utils/utils.py
--rw-r--r--   0        0        0      916 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    24172 1970-01-01 00:00:00.000000 gcp_pal-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    23782 2024-04-25 23:01:53.623017 gcp_pal-1.0.3/README.md
+-rw-r--r--   0        0        0      810 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/__init__.py
+-rw-r--r--   0        0        0    31402 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/bigquery.py
+-rw-r--r--   0        0        0    13156 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/cloudfunctions.py
+-rw-r--r--   0        0        0    13855 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/cloudrun.py
+-rw-r--r--   0        0        0     7754 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/cloudscheduler.py
+-rw-r--r--   0        0        0       42 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/config/__init__.py
+-rw-r--r--   0        0        0      965 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/config/vars.py
+-rw-r--r--   0        0        0    12490 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/firestore.py
+-rw-r--r--   0        0        0     2248 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/project.py
+-rw-r--r--   0        0        0     1674 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/pubsub.py
+-rw-r--r--   0        0        0     3873 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/pydocker.py
+-rw-r--r--   0        0        0     6860 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/pylogging.py
+-rw-r--r--   0        0        0     4737 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/request.py
+-rw-r--r--   0        0        0    23631 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/schema.py
+-rw-r--r--   0        0        0     6332 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/secretmanager.py
+-rw-r--r--   0        0        0       88 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/storage/__init__.py
+-rw-r--r--   0        0        0     8735 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/storage/parquet.py
+-rw-r--r--   0        0        0    17133 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/storage/storage.py
+-rw-r--r--   0        0        0       82 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/utils/__init__.py
+-rw-r--r--   0        0        0      935 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/utils/lazy_loader.py
+-rw-r--r--   0        0        0    11329 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/utils/utils.py
+-rw-r--r--   0        0        0      958 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    24172 1970-01-01 00:00:00.000000 gcp_pal-1.0.3/PKG-INFO
```

### Comparing `gcp_pal-1.0.1/README.md` & `gcp_pal-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.1/gcp_pal/__init__.py` & `gcp_pal-1.0.3/gcp_pal/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,7 +10,8 @@
 PubSub = LazyLoader("gcp_pal.pubsub", "PubSub")
 Logging = LazyLoader("gcp_pal.pylogging", "Logging")
 Request = LazyLoader("gcp_pal.request", "Request")
 Schema = LazyLoader("gcp_pal.schema", "Schema")
 Storage = LazyLoader("gcp_pal.storage", "Storage")
 Parquet = LazyLoader("gcp_pal.storage", "Parquet")
 SecretManager = LazyLoader("gcp_pal.secretmanager", "SecretManager")
+Project = LazyLoader("gcp_pal.project", "Project")
```

### Comparing `gcp_pal-1.0.1/gcp_pal/bigquery.py` & `gcp_pal-1.0.3/gcp_pal/bigquery.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.1/gcp_pal/cloudfunctions.py` & `gcp_pal-1.0.3/gcp_pal/cloudfunctions.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.1/gcp_pal/cloudrun.py` & `gcp_pal-1.0.3/gcp_pal/cloudrun.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.1/gcp_pal/cloudscheduler.py` & `gcp_pal-1.0.3/gcp_pal/cloudscheduler.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.1/gcp_pal/config/vars.py` & `gcp_pal-1.0.3/gcp_pal/config/vars.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     "google.cloud.pubsub_v1": "google-cloud-pubsub",
     "google.cloud.bigquery": "google-cloud-bigquery",
     "google.cloud.firestore": "google-cloud-firestore",
     "google.cloud.functions_v1": "google-cloud-functions",
     "google.cloud.functions_v2": "google-cloud-functions",
     "google.cloud.scheduler_v1": "google-cloud-scheduler",
     "google.cloud.secretmanager": "google-cloud-secret-manager",
+    "google.cloud.resource_manager": "google-cloud-resource-manager",
     "google.cloud.run_v1": "google-cloud-run",
     "google.cloud.run_v2": "google-cloud-run",
     "gcsfs": "gcsfs",
     "pyarrow": "pyarrow",
     "pandas": "pandas",
     "pandas_gbq": "pandas-gbq",
     "docker": "docker",
```

### Comparing `gcp_pal-1.0.1/gcp_pal/firestore.py` & `gcp_pal-1.0.3/gcp_pal/firestore.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.1/gcp_pal/pubsub.py` & `gcp_pal-1.0.3/gcp_pal/pubsub.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.1/gcp_pal/pydocker.py` & `gcp_pal-1.0.3/gcp_pal/pydocker.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.1/gcp_pal/pylogging.py` & `gcp_pal-1.0.3/gcp_pal/pylogging.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.1/gcp_pal/request.py` & `gcp_pal-1.0.3/gcp_pal/request.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.1/gcp_pal/schema.py` & `gcp_pal-1.0.3/gcp_pal/schema.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.1/gcp_pal/secretmanager.py` & `gcp_pal-1.0.3/gcp_pal/secretmanager.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.1/gcp_pal/storage/parquet.py` & `gcp_pal-1.0.3/gcp_pal/storage/parquet.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.1/gcp_pal/storage/storage.py` & `gcp_pal-1.0.3/gcp_pal/storage/storage.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.1/gcp_pal/utils/lazy_loader.py` & `gcp_pal-1.0.3/gcp_pal/utils/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.1/gcp_pal/utils/utils.py` & `gcp_pal-1.0.3/gcp_pal/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 err = try_import("google.cloud.logging", "logging", errors="ignore")
 try_import("google.cloud.logging.handlers.transports", "logging", errors="ignore")
 if err is not None:
     from google.cloud import logging as gcp_logging
     from google.cloud.logging.handlers.transports import SyncTransport
 
-    if os.getenv("PLATFORM", "GCP") in ["GCP", "local"]:
+    if os.getenv("PLATFORM", "") in ["GCP", "local"]:
         client = gcp_logging.Client()
         handler = gcp_logging.handlers.CloudLoggingHandler(
             client, name="gcp_pal", transport=SyncTransport
         )
         client.setup_logging()
 
 
@@ -288,34 +288,48 @@
         range_n = range(n_values)
         output = {k: [d[i][k] for i in range_n] for k in keys}
     else:
         output = d
     return output
 
 
-def get_auth_default():
+def get_auth_default(errors="raise"):
     """
     Get the default project from google.auth.default() and store it in an environment variable.
 
     Returns:
     - str: The default project.
     """
     try_import("google.auth", "get_default_project")
     import google.auth as google_auth
 
     project = os.getenv("_GOOGLE_AUTH_DEFAULT_PROJECT", None)
     credentials = os.getenv("_GOOGLE_AUTH_DEFAULT_CREDENTIALS", None)
-    if project is None:
-        credentials, project = google_auth.default()
-        os.environ["_GOOGLE_AUTH_DEFAULT_PROJECT"] = project
+    if project is not None:
         try:
-            os.environ["_GOOGLE_AUTH_DEFAULT_CREDENTIALS"] = credentials.to_json()
+            credentials = google_auth.credentials.Credentials.from_json(credentials)
         except AttributeError:
             pass
-        print(f"Obtained default project: {project}")
+        return credentials, project
+
+    credentials, project = google_auth.default()
+    if project is None:
+        err = "No default project found. Please set the PROJECT environment variable."
+        if errors == "raise":
+            raise ValueError(err)
+        else:
+            print("Warning:", err)
+        return credentials, project
+
+    os.environ["_GOOGLE_AUTH_DEFAULT_PROJECT"] = project
+    try:
+        os.environ["_GOOGLE_AUTH_DEFAULT_CREDENTIALS"] = credentials.to_json()
+    except AttributeError:
+        pass
+    print(f"Obtained default project: {project}")
     return credentials, project
 
 
 def zip_directory(directory, output_file=None, omit_root=True):
     """
     Zip a directory.
```

### Comparing `gcp_pal-1.0.1/pyproject.toml` & `gcp_pal-1.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcp-pal"
-version = "1.0.1"
+version = "1.0.3"
 description = ""
 authors = ["VitaminB16 <artemiy.nosov@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
@@ -29,11 +29,12 @@
 google-auth-oauthlib = "^1.2.0"
 docker = "^7.0.0"
 google-cloud-run = "^0.10.5"
 pyyaml = "^6.0.1"
 google-cloud-secret-manager = "^2.19.0"
 google-cloud-scheduler = "^2.13.3"
 google-cloud-logging = "^3.10.0"
+google-cloud-resource-manager = "^1.12.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gcp_pal-1.0.1/PKG-INFO` & `gcp_pal-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-pal
-Version: 1.0.1
+Version: 1.0.3
 Summary: 
 Author: VitaminB16
 Author-email: artemiy.nosov@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

