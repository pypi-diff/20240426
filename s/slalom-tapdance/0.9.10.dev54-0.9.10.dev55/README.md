# Comparing `tmp/slalom_tapdance-0.9.10.dev54.tar.gz` & `tmp/slalom_tapdance-0.9.10.dev55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slalom_tapdance-0.9.10.dev54.tar", max compression
+gzip compressed data, was "slalom_tapdance-0.9.10.dev55.tar", max compression
```

## Comparing `slalom_tapdance-0.9.10.dev54.tar` & `slalom_tapdance-0.9.10.dev55.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-04-23 21:40:58.321982 slalom_tapdance-0.9.10.dev54/LICENSE
--rw-r--r--   0        0        0     1162 2024-04-23 21:41:18.385856 slalom_tapdance-0.9.10.dev54/pyproject.toml
--rw-r--r--   0        0        0      288 2024-04-23 21:40:58.321982 slalom_tapdance-0.9.10.dev54/tapdance/__init__.py
--rw-r--r--   0        0        0      696 2024-04-23 21:40:58.321982 slalom_tapdance-0.9.10.dev54/tapdance/cli.py
--rw-r--r--   0        0        0    15304 2024-04-23 21:40:58.321982 slalom_tapdance-0.9.10.dev54/tapdance/config.py
--rw-r--r--   0        0        0    14357 2024-04-23 21:40:58.321982 slalom_tapdance-0.9.10.dev54/tapdance/docker.py
--rw-r--r--   0        0        0     1606 2024-04-23 21:40:58.321982 slalom_tapdance-0.9.10.dev54/tapdance/install_helper.py
--rw-r--r--   0        0        0    37111 2024-04-23 21:40:58.321982 slalom_tapdance-0.9.10.dev54/tapdance/plans.py
--rw-r--r--   0        0        0     3180 2024-04-23 21:40:58.321982 slalom_tapdance-0.9.10.dev54/tapdance/states.py
--rw-r--r--   0        0        0    11787 2024-04-23 21:40:58.321982 slalom_tapdance-0.9.10.dev54/tapdance/syncs.py
--rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 slalom_tapdance-0.9.10.dev54/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-26 16:32:12.984948 slalom_tapdance-0.9.10.dev55/LICENSE
+-rw-r--r--   0        0        0     1162 2024-04-26 16:32:28.896973 slalom_tapdance-0.9.10.dev55/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-04-26 16:32:12.988948 slalom_tapdance-0.9.10.dev55/tapdance/__init__.py
+-rw-r--r--   0        0        0      714 2024-04-26 16:32:12.988948 slalom_tapdance-0.9.10.dev55/tapdance/cli.py
+-rw-r--r--   0        0        0    15604 2024-04-26 16:32:12.988948 slalom_tapdance-0.9.10.dev55/tapdance/config.py
+-rw-r--r--   0        0        0    14381 2024-04-26 16:32:12.988948 slalom_tapdance-0.9.10.dev55/tapdance/docker.py
+-rw-r--r--   0        0        0     1606 2024-04-26 16:32:12.988948 slalom_tapdance-0.9.10.dev55/tapdance/install_helper.py
+-rw-r--r--   0        0        0    37120 2024-04-26 16:32:12.988948 slalom_tapdance-0.9.10.dev55/tapdance/plans.py
+-rw-r--r--   0        0        0     3180 2024-04-26 16:32:12.988948 slalom_tapdance-0.9.10.dev55/tapdance/states.py
+-rw-r--r--   0        0        0    11850 2024-04-26 16:32:12.988948 slalom_tapdance-0.9.10.dev55/tapdance/syncs.py
+-rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 slalom_tapdance-0.9.10.dev55/PKG-INFO
```

### Comparing `slalom_tapdance-0.9.10.dev54/LICENSE` & `slalom_tapdance-0.9.10.dev55/LICENSE`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev54/pyproject.toml` & `slalom_tapdance-0.9.10.dev55/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slalom-tapdance"
-version = "0.9.10-dev.54"
+version = "0.9.10-dev.55"
 description = "Tapdance is an orchestration layer for the open source Singer tap platform."
 authors = ["AJ Steers <aj.steers@slalom.com>"]
 license = "MIT"
 packages = [
     {include = "tapdance"}
 ]
```

### Comparing `slalom_tapdance-0.9.10.dev54/tapdance/cli.py` & `slalom_tapdance-0.9.10.dev55/tapdance/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """tapdance.cli - Defines the command-line interface (CLI) for tapdance."""
 
 import fire
 from logless import logged
 
-from tapdance.config import print_version
+from tapdance.config import print_tapdance_version
 from tapdance.docker import build_all_images, build_image
 from tapdance.install_helper import install
 from tapdance.plans import plan
 from tapdance.syncs import sync
 
 
 @logged("tapdance execution")
@@ -16,14 +16,14 @@
     fire.Fire(
         {
             "plan": plan,
             "sync": sync,
             "install": install,
             "build_all_images": build_all_images,
             "build_image": build_image,
-            "--version": print_version,
+            "--version": print_tapdance_version,
         }
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `slalom_tapdance-0.9.10.dev54/tapdance/config.py` & `slalom_tapdance-0.9.10.dev55/tapdance/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,27 +72,31 @@
                 elif str(v) == "0":
                     conf_dict[setting_name] = 0
                 else:
                     conf_dict[setting_name] = v
     return conf_dict
 
 
-def print_version():
+def print_tapdance_version():
     """Print the tapdance version number."""
     try:
-        from importlib import metadata
+        from importlib.metadata import version
+        tapdance_version = version('slalom-tapdance')
+        logging.info(f"slalom-tapdance version {tapdance_version}")
     except ImportError:
-        # Running on pre-3.8 Python; use importlib-metadata package
-        import importlib_metadata as metadata
-    try:
-        version = metadata.version("tapdance")
-    except metadata.PackageNotFoundError:
-        version = "[could not be detected]"
-    print(f"tapdance version {version}")
+        logging.info(f"slalom-tapdance version could not be detected")
 
+def print_plugin_version(tap_exe = None, target_exe = None):
+    """
+    Print the tap and target version numbers if they're available.
+    Unable to get version information for the tap and target inside of tapdance
+    Could add the version command to the config so that we could call it with runnow
+    """
+    logging.info(f'Tap: {tap_exe}')
+    logging.info(f'Target: {target_exe}')
 
 @logged(
     "getting '{plugin_name}' config file using: config_dir={config_dir}, "
     "config_file={config_file}",
     log_fn=logging.debug,
 )
 def get_or_create_config(
```

### Comparing `slalom_tapdance-0.9.10.dev54/tapdance/docker.py` & `slalom_tapdance-0.9.10.dev55/tapdance/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     source_image: Optional[str] = None,
     plugins_index: Optional[str] = None,
     push: bool = False,
     pre: bool = False,
     ignore_cache: bool = False,
 ) -> List[str]:
     """
-    Create the docker images for the tap and target combinations.
+    Create the docker images for the tap and target combinations in the singer_index.yml.
 
     """
     plugins = _get_plugins_list(plugins_index)
     created_images = []
     #For every tap in the singer_index.yml, loop through all the targets and create a docker image. 
     for tap_name, tap_source, tap_alias in plugins:
         tap_alias = tap_alias or tap_name
```

### Comparing `slalom_tapdance-0.9.10.dev54/tapdance/install_helper.py` & `slalom_tapdance-0.9.10.dev55/tapdance/install_helper.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev54/tapdance/plans.py` & `slalom_tapdance-0.9.10.dev55/tapdance/plans.py`

 * *Files 0% similar despite different names*

```diff
@@ -556,15 +556,15 @@
     ------
     ValueError
         Raised if an argument value is not within expected domain.
     FileExistsError
         Raised if files do not exist in default locations, or if paths provided do not
         point to valid files.
     """
-    config.print_version()
+    config.print_tapdance_version()
 
     taps_dir = config.get_taps_dir(taps_dir)
     config_file, tap_settings = config.get_or_create_config(
         f"tap-{tap_name}",
         taps_dir=taps_dir,
         config_dir=config_dir,
         config_file=config_file,
```

### Comparing `slalom_tapdance-0.9.10.dev54/tapdance/states.py` & `slalom_tapdance-0.9.10.dev55/tapdance/states.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev54/tapdance/syncs.py` & `slalom_tapdance-0.9.10.dev55/tapdance/syncs.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     exclude_tables: {List(str)}
         A list of tables to exclude. Ignored
         if table_name arg is not "*".
     replication_strategy : {str}
         One of "FULL_TABLE", "INCREMENTAL", or "LOG_BASED"; by default "INCREMENTAL" or
         a value is set in the TAP_{TAPNAME}_REPLICATION_STRATEGY environment variable.
     """
-    config.print_version()
+    config.print_tapdance_version()
 
     taps_dir = config.get_taps_dir(taps_dir)
     config_file, tap_settings = config.get_or_create_config(
         f"tap-{tap_name}",
         taps_dir=taps_dir,
         config_dir=config_dir,
         config_file=config_file,
@@ -101,14 +101,17 @@
         f"target-{target_name}",
         taps_dir=taps_dir,
         config_dir=config_dir,
         config_file=target_config_file,
     )
     tap_exe = tap_exe or tap_settings.get("EXE", f"tap-{tap_name}")
     target_exe = target_exe or target_settings.get("EXE", f"target-{target_name}")
+
+    config.print_plugin_version(tap_exe,target_exe)
+
     replication_strategy = replication_strategy or tap_settings.get(
         "REPLICATION_STRATEGY", "INCREMENTAL"
     )
     config.validate_replication_strategy(replication_strategy)
 
     table_name = table_name or tap_settings.get("TABLE_NAME", None)
     exclude_tables = exclude_tables or tap_settings.get("EXCLUDE_TABLES", None)
```

### Comparing `slalom_tapdance-0.9.10.dev54/PKG-INFO` & `slalom_tapdance-0.9.10.dev55/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slalom-tapdance
-Version: 0.9.10.dev54
+Version: 0.9.10.dev55
 Summary: Tapdance is an orchestration layer for the open source Singer tap platform.
 License: MIT
 Author: AJ Steers
 Author-email: aj.steers@slalom.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

