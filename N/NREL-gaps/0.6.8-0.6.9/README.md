# Comparing `tmp/NREL-gaps-0.6.8.tar.gz` & `tmp/NREL-gaps-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NREL-gaps-0.6.8.tar", last modified: Tue Jan  2 23:53:46 2024, max compression
+gzip compressed data, was "NREL-gaps-0.6.9.tar", last modified: Mon Jan  8 17:18:17 2024, max compression
```

## Comparing `NREL-gaps-0.6.8.tar` & `NREL-gaps-0.6.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 23:53:46.666624 NREL-gaps-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 23:53:46.662624 NREL-gaps-0.6.8/NREL_gaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-01-02 23:53:46.000000 NREL-gaps-0.6.8/NREL_gaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-02 23:53:46.000000 NREL-gaps-0.6.8/NREL_gaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 23:53:46.000000 NREL-gaps-0.6.8/NREL_gaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-02 23:53:46.000000 NREL-gaps-0.6.8/NREL_gaps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 23:53:46.000000 NREL-gaps-0.6.8/NREL_gaps.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-02 23:53:46.000000 NREL-gaps-0.6.8/NREL_gaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-02 23:53:46.000000 NREL-gaps-0.6.8/NREL_gaps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-01-02 23:53:46.666624 NREL-gaps-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 23:53:46.662624 NREL-gaps-0.6.8/gaps/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 23:53:46.666624 NREL-gaps-0.6.8/gaps/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/cli/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/cli/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)    37725 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (127)    22153 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27080 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/cli/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/cli/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/cli/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/cli/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/cli/reset.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/cli/script.py
--rw-r--r--   0 runner    (1001) docker     (127)    13860 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/cli/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/cli/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    32639 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    24253 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/hpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    14183 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    10433 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/project_points.py
--rw-r--r--   0 runner    (1001) docker     (127)    31936 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/gaps/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-02 23:53:46.666624 NREL-gaps-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-01-02 23:53:38.000000 NREL-gaps-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 17:18:17.069505 NREL-gaps-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 17:18:17.065505 NREL-gaps-0.6.9/NREL_gaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-01-08 17:18:16.000000 NREL-gaps-0.6.9/NREL_gaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-08 17:18:17.000000 NREL-gaps-0.6.9/NREL_gaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 17:18:16.000000 NREL-gaps-0.6.9/NREL_gaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-08 17:18:16.000000 NREL-gaps-0.6.9/NREL_gaps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 17:18:16.000000 NREL-gaps-0.6.9/NREL_gaps.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-08 17:18:16.000000 NREL-gaps-0.6.9/NREL_gaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-08 17:18:16.000000 NREL-gaps-0.6.9/NREL_gaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-01-08 17:18:17.069505 NREL-gaps-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 17:18:17.065505 NREL-gaps-0.6.9/gaps/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16135 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 17:18:17.069505 NREL-gaps-0.6.9/gaps/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/cli/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/cli/collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37725 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22153 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27080 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/cli/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/cli/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/cli/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/cli/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/cli/reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/cli/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13860 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/cli/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/cli/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32639 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24253 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/hpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14183 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10433 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/project_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31936 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/gaps/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 17:18:17.069505 NREL-gaps-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-01-08 17:18:05.000000 NREL-gaps-0.6.9/setup.py
```

### Comparing `NREL-gaps-0.6.8/LICENSE` & `NREL-gaps-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/NREL_gaps.egg-info/PKG-INFO` & `NREL-gaps-0.6.9/NREL_gaps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-gaps
-Version: 0.6.8
+Version: 0.6.9
 Summary: National Renewable Energy Laboratory's (NREL's) Geospatial Analysis Pipelines (GAPs) framework
 Home-page: https://nrel.github.io/gaps/
 Author: Paul Pinchuk
 Maintainer-email: ppinchuk@nrel.gov
 License: BSD 3-Clause
 Keywords: gaps
 Classifier: Development Status :: 4 - Beta
```

### Comparing `NREL-gaps-0.6.8/NREL_gaps.egg-info/SOURCES.txt` & `NREL-gaps-0.6.9/NREL_gaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/PKG-INFO` & `NREL-gaps-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-gaps
-Version: 0.6.8
+Version: 0.6.9
 Summary: National Renewable Energy Laboratory's (NREL's) Geospatial Analysis Pipelines (GAPs) framework
 Home-page: https://nrel.github.io/gaps/
 Author: Paul Pinchuk
 Maintainer-email: ppinchuk@nrel.gov
 License: BSD 3-Clause
 Keywords: gaps
 Classifier: Development Status :: 4 - Beta
```

### Comparing `NREL-gaps-0.6.8/README.rst` & `NREL-gaps-0.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/batch.py` & `NREL-gaps-0.6.9/gaps/batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,61 +91,54 @@
         logger.debug(
             "Batch jobs list: %s", sorted(table.index.values.tolist())
         )
         logger.info("Preparing batch job directories...")
 
         # walk through current directory getting everything to copy
         for source_dir, _, filenames in os.walk(self._base_dir):
+            logger.debug("Processing files in : %s", source_dir)
+
             # don't make additional copies of job sub directories.
             if any(job_tag in source_dir for job_tag in self._sets):
                 continue
 
             # For each dir level, iterate through the batch arg combos
             for tag, (arg_comb, mod_files, __) in self._sets.items():
+                mod_files = {Path(fp) for fp in mod_files}
                 # Add the job tag to the directory path.
                 # This will copy config subdirs into the job subdirs
                 source_dir = Path(source_dir)
                 destination_dir = (
                     self._base_dir
                     / tag
                     / source_dir.relative_to(self._base_dir)
                 )
                 destination_dir.mkdir(parents=True, exist_ok=True)
 
                 for name in filenames:
                     if BATCH_CSV_FN in name:
                         continue
-                    _copy_batch_file(
-                        source_dir / name,
-                        destination_dir / name,
-                    )
-
-                for fp_source in mod_files:
-                    logger.debug(
-                        "Copying and modifying run file %r to job: %r",
-                        fp_source,
-                        tag,
-                    )
-                    fp_source = Path(fp_source)
-                    fp_target = destination_dir / fp_source.relative_to(
-                        self._base_dir
-                    )
-                    fp_target.parent.mkdir(parents=True, exist_ok=True)
-                    _mod_file(fp_source, fp_target, arg_comb)
-
-                pipeline_file_target = (
-                    destination_dir
-                    / self._pipeline_fp.relative_to(self._base_dir)
-                )
-                pipeline_file_target.parent.mkdir(parents=True, exist_ok=True)
-                _copy_batch_file(
-                    self._pipeline_fp,
-                    destination_dir
-                    / self._pipeline_fp.relative_to(self._base_dir),
-                )
+                    fp_source = source_dir / name
+                    fp_target = destination_dir / name
+                    if fp_source in mod_files:
+                        _mod_file(fp_source, fp_target, arg_comb)
+                    else:
+                        _copy_batch_file(fp_source, destination_dir / name)
+
+        for tag in self._sets:
+            destination_dir = self._base_dir / tag
+            pipeline_file_target = (
+                destination_dir / self._pipeline_fp.relative_to(self._base_dir)
+            )
+            pipeline_file_target.parent.mkdir(parents=True, exist_ok=True)
+            _copy_batch_file(
+                self._pipeline_fp,
+                destination_dir
+                / self._pipeline_fp.relative_to(self._base_dir),
+            )
 
         logger.info("Batch job directories ready for execution.")
 
     def _run_pipelines(self, monitor_background=False):
         """Run the pipeline modules for each batch job."""
 
         for sub_directory in self.sub_dirs:
@@ -441,14 +434,17 @@
         value = f"{value}0"
 
     return value
 
 
 def _mod_file(fpath_in, fpath_out, arg_mods):
     """Import and modify the contents of a json. Dump to new file."""
+    logger.debug(
+        "Copying and modifying run file %r to job: %r", fpath_in, fpath_out
+    )
     config_type = ConfigType(fpath_in.name.split(".")[-1])
     config = config_type.load(fpath_in)
     config_type.write(fpath_out, _mod_dict(config, arg_mods))
 
 
 def _mod_dict(inp, arg_mods):
     """Recursively modify key/value pairs in a dictionary."""
```

### Comparing `NREL-gaps-0.6.8/gaps/cli/batch.py` & `NREL-gaps-0.6.9/gaps/cli/batch.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/cli/cli.py` & `NREL-gaps-0.6.9/gaps/cli/cli.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/cli/collect.py` & `NREL-gaps-0.6.9/gaps/cli/collect.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/cli/command.py` & `NREL-gaps-0.6.9/gaps/cli/command.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/cli/config.py` & `NREL-gaps-0.6.9/gaps/cli/config.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/cli/documentation.py` & `NREL-gaps-0.6.9/gaps/cli/documentation.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/cli/execution.py` & `NREL-gaps-0.6.9/gaps/cli/execution.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/cli/pipeline.py` & `NREL-gaps-0.6.9/gaps/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/cli/preprocessing.py` & `NREL-gaps-0.6.9/gaps/cli/preprocessing.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/cli/reset.py` & `NREL-gaps-0.6.9/gaps/cli/reset.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/cli/script.py` & `NREL-gaps-0.6.9/gaps/cli/script.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/cli/status.py` & `NREL-gaps-0.6.9/gaps/cli/status.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/cli/templates.py` & `NREL-gaps-0.6.9/gaps/cli/templates.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/collection.py` & `NREL-gaps-0.6.9/gaps/collection.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/config.py` & `NREL-gaps-0.6.9/gaps/config.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/exceptions.py` & `NREL-gaps-0.6.9/gaps/exceptions.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/hpc.py` & `NREL-gaps-0.6.9/gaps/hpc.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/legacy.py` & `NREL-gaps-0.6.9/gaps/legacy.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/log.py` & `NREL-gaps-0.6.9/gaps/log.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/pipeline.py` & `NREL-gaps-0.6.9/gaps/pipeline.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/project_points.py` & `NREL-gaps-0.6.9/gaps/project_points.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/status.py` & `NREL-gaps-0.6.9/gaps/status.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/utilities.py` & `NREL-gaps-0.6.9/gaps/utilities.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/gaps/warnings.py` & `NREL-gaps-0.6.9/gaps/warnings.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.6.8/setup.py` & `NREL-gaps-0.6.9/setup.py`

 * *Files identical despite different names*

