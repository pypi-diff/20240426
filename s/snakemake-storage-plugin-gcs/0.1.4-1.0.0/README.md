# Comparing `tmp/snakemake_storage_plugin_gcs-0.1.4.tar.gz` & `tmp/snakemake_storage_plugin_gcs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_storage_plugin_gcs-0.1.4.tar", max compression
+gzip compressed data, was "snakemake_storage_plugin_gcs-1.0.0.tar", max compression
```

## Comparing `snakemake_storage_plugin_gcs-0.1.4.tar` & `snakemake_storage_plugin_gcs-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1066 2024-03-10 07:07:13.836042 snakemake_storage_plugin_gcs-0.1.4/LICENSE
--rw-r--r--   0        0        0     1167 2024-03-10 07:07:13.836042 snakemake_storage_plugin_gcs-0.1.4/NOTICE
--rw-r--r--   0        0        0      697 2024-03-10 07:07:13.836042 snakemake_storage_plugin_gcs-0.1.4/README.md
--rw-r--r--   0        0        0      979 2024-03-10 07:07:13.840042 snakemake_storage_plugin_gcs-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    17084 2024-03-10 07:07:13.840042 snakemake_storage_plugin_gcs-0.1.4/snakemake_storage_plugin_gcs/__init__.py
--rw-r--r--   0        0        0     1711 1970-01-01 00:00:00.000000 snakemake_storage_plugin_gcs-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-26 10:36:12.983548 snakemake_storage_plugin_gcs-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1167 2024-04-26 10:36:12.983548 snakemake_storage_plugin_gcs-1.0.0/NOTICE
+-rw-r--r--   0        0        0      698 2024-04-26 10:36:12.983548 snakemake_storage_plugin_gcs-1.0.0/README.md
+-rw-r--r--   0        0        0      979 2024-04-26 10:36:12.983548 snakemake_storage_plugin_gcs-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    17263 2024-04-26 10:36:12.983548 snakemake_storage_plugin_gcs-1.0.0/snakemake_storage_plugin_gcs/__init__.py
+-rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 snakemake_storage_plugin_gcs-1.0.0/PKG-INFO
```

### Comparing `snakemake_storage_plugin_gcs-0.1.4/LICENSE` & `snakemake_storage_plugin_gcs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_storage_plugin_gcs-0.1.4/NOTICE` & `snakemake_storage_plugin_gcs-1.0.0/NOTICE`

 * *Files identical despite different names*

### Comparing `snakemake_storage_plugin_gcs-0.1.4/README.md` & `snakemake_storage_plugin_gcs-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Snakemake storage plugin: gcs
 
 A snakemake storage plugin for Google Cloud Storage.
-For documentation and usage instructions, see the [Snakemake plugin catalog](https://snakemake.github.io/snakemake-plugin-catalog/plugins/storage/s3.html).
+For documentation and usage instructions, see the [Snakemake plugin catalog](https://snakemake.github.io/snakemake-plugin-catalog/plugins/storage/gcs.html).
 
 
 ## License
 
 HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license.
```

### Comparing `snakemake_storage_plugin_gcs-0.1.4/pyproject.toml` & `snakemake_storage_plugin_gcs-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-storage-plugin-gcs"
-version = "0.1.4"
+version = "1.0.0"
 description = "A Snakemake storage plugin for Google Cloud Storage"
 authors = [
     "Vanessa Sochat <sochat1@llnl.gov>",
     "Johannes Koester <johannes.koester@uni-due.de>"
 ]
 readme = "README.md"
 repository = "https://github.com/snakemake/snakemake-storage-plugin-gcs"
```

### Comparing `snakemake_storage_plugin_gcs-0.1.4/snakemake_storage_plugin_gcs/__init__.py` & `snakemake_storage_plugin_gcs-1.0.0/snakemake_storage_plugin_gcs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,33 +185,33 @@
             parsed = urlparse(query)
         except Exception as e:
             return StorageQueryValidationResult(
                 query=query,
                 valid=False,
                 reason=f"cannot be parsed as URL ({e})",
             )
-        if parsed.scheme != "gs":
+        if parsed.scheme != "gcs":
             return StorageQueryValidationResult(
                 query=query,
                 valid=False,
-                reason="must start with gs (gs://...)",
+                reason="must start with gcs scheme (gcs://...)",
             )
         return StorageQueryValidationResult(
             query=query,
             valid=True,
         )
 
     @classmethod
     def example_queries(cls) -> List[ExampleQuery]:
         """
         Return an example query with description for this storage provider.
         """
         return [
             ExampleQuery(
-                query="gs://mybucket/myfile.txt",
+                query="gcs://mybucket/myfile.txt",
                 type=QueryType.ANY,
                 description="A file in an google storage (GCS) bucket",
             )
         ]
 
     def use_rate_limiter(self) -> bool:
         """Return False if no rate limiting is needed for this provider."""
@@ -334,15 +334,19 @@
 
         def get_mtime(blob):
             if blob.updated is None:
                 blob.reload()
             return blob.updated.timestamp()
 
         if self.is_directory():
-            return max(get_mtime(blob) for blob in self.directory_entries())
+            entries = list(self.directory_entries())
+            assert (
+                entries
+            ), f"bug: mtime called but directory does not seem to exist: {self.query}"
+            return max(get_mtime(blob) for blob in entries)
         else:
             return get_mtime(self.blob)
 
     @retry.Retry(predicate=google_cloud_retry_predicate)
     def size(self) -> int:
         """
         Return the size in bytes
```

### Comparing `snakemake_storage_plugin_gcs-0.1.4/PKG-INFO` & `snakemake_storage_plugin_gcs-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-storage-plugin-gcs
-Version: 0.1.4
+Version: 1.0.0
 Summary: A Snakemake storage plugin for Google Cloud Storage
 Home-page: https://github.com/snakemake/snakemake-storage-plugin-gcs
 License: MIT
 Keywords: snakemake,storage,plugin,google cloud storage
 Author: Vanessa Sochat
 Author-email: sochat1@llnl.gov
 Requires-Python: >=3.11,<4.0
@@ -19,15 +19,15 @@
 Project-URL: Documentation, https://snakemake.github.io/snakemake-plugin-catalog/plugins/storage/gcs.html
 Project-URL: Repository, https://github.com/snakemake/snakemake-storage-plugin-gcs
 Description-Content-Type: text/markdown
 
 # Snakemake storage plugin: gcs
 
 A snakemake storage plugin for Google Cloud Storage.
-For documentation and usage instructions, see the [Snakemake plugin catalog](https://snakemake.github.io/snakemake-plugin-catalog/plugins/storage/s3.html).
+For documentation and usage instructions, see the [Snakemake plugin catalog](https://snakemake.github.io/snakemake-plugin-catalog/plugins/storage/gcs.html).
 
 
 ## License
 
 HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license.
```

