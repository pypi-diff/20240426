# Comparing `tmp/fixinventory_plugin_digitalocean-4.0.4.tar.gz` & `tmp/fixinventory_plugin_digitalocean-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory_plugin_digitalocean-4.0.4.tar", last modified: Wed Apr 24 19:31:17 2024, max compression
+gzip compressed data, was "fixinventory_plugin_digitalocean-4.0.5.tar", last modified: Fri Apr 26 20:24:10 2024, max compression
```

## Comparing `fixinventory_plugin_digitalocean-4.0.4.tar` & `fixinventory_plugin_digitalocean-4.0.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:17.819436 fixinventory_plugin_digitalocean-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-24 19:31:17.819436 fixinventory_plugin_digitalocean-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:17.811436 fixinventory_plugin_digitalocean-4.0.4/fix_plugin_digitalocean/
--rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/fix_plugin_digitalocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16224 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/fix_plugin_digitalocean/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    48601 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/fix_plugin_digitalocean/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/fix_plugin_digitalocean/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    26362 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/fix_plugin_digitalocean/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/fix_plugin_digitalocean/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:17.819436 fixinventory_plugin_digitalocean-4.0.4/fixinventory_plugin_digitalocean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-24 19:31:17.000000 fixinventory_plugin_digitalocean-4.0.4/fixinventory_plugin_digitalocean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-24 19:31:17.000000 fixinventory_plugin_digitalocean-4.0.4/fixinventory_plugin_digitalocean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:31:17.000000 fixinventory_plugin_digitalocean-4.0.4/fixinventory_plugin_digitalocean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 19:31:17.000000 fixinventory_plugin_digitalocean-4.0.4/fixinventory_plugin_digitalocean.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:28:24.000000 fixinventory_plugin_digitalocean-4.0.4/fixinventory_plugin_digitalocean.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 19:31:17.000000 fixinventory_plugin_digitalocean-4.0.4/fixinventory_plugin_digitalocean.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-24 19:31:17.000000 fixinventory_plugin_digitalocean-4.0.4/fixinventory_plugin_digitalocean.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 19:31:17.819436 fixinventory_plugin_digitalocean-4.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:17.811436 fixinventory_plugin_digitalocean-4.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:17.819436 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/cdns.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/cpu_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/domain_records.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/domains.py
--rw-r--r--   0 runner    (1001) docker     (127)    10579 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/droplets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/firewalls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8942 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/floatingip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/loadbalancers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/memory_available.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/neighbor_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/projectresources.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/registry_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/registry_repository_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/spaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/volumes.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/fixtures/vpcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25838 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-24 19:27:16.000000 fixinventory_plugin_digitalocean-4.0.4/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:24:10.069504 fixinventory_plugin_digitalocean-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-26 20:24:10.069504 fixinventory_plugin_digitalocean-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:24:10.061504 fixinventory_plugin_digitalocean-4.0.5/fix_plugin_digitalocean/
+-rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/fix_plugin_digitalocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16224 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/fix_plugin_digitalocean/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48601 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/fix_plugin_digitalocean/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/fix_plugin_digitalocean/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26362 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/fix_plugin_digitalocean/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/fix_plugin_digitalocean/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:24:10.069504 fixinventory_plugin_digitalocean-4.0.5/fixinventory_plugin_digitalocean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-26 20:24:10.000000 fixinventory_plugin_digitalocean-4.0.5/fixinventory_plugin_digitalocean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-26 20:24:10.000000 fixinventory_plugin_digitalocean-4.0.5/fixinventory_plugin_digitalocean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:24:10.000000 fixinventory_plugin_digitalocean-4.0.5/fixinventory_plugin_digitalocean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-26 20:24:10.000000 fixinventory_plugin_digitalocean-4.0.5/fixinventory_plugin_digitalocean.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:21:25.000000 fixinventory_plugin_digitalocean-4.0.5/fixinventory_plugin_digitalocean.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-26 20:24:10.000000 fixinventory_plugin_digitalocean-4.0.5/fixinventory_plugin_digitalocean.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-26 20:24:10.000000 fixinventory_plugin_digitalocean-4.0.5/fixinventory_plugin_digitalocean.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-26 20:24:10.069504 fixinventory_plugin_digitalocean-4.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:24:10.061504 fixinventory_plugin_digitalocean-4.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:24:10.069504 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/cdns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/cpu_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/domain_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10579 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/droplets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/firewalls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8942 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/floatingip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/loadbalancers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/memory_available.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/neighbor_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/projectresources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/registry_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/registry_repository_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/spaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/fixtures/vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25838 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-26 20:20:17.000000 fixinventory_plugin_digitalocean-4.0.5/test/test_config.py
```

### Comparing `fixinventory_plugin_digitalocean-4.0.4/PKG-INFO` & `fixinventory_plugin_digitalocean-4.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-digitalocean
-Version: 4.0.4
+Version: 4.0.5
 Summary: Fix DigitalOcean Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/digitalocean
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.4
+Requires-Dist: fixinventorylib==4.0.5
 Requires-Dist: boto3
 Requires-Dist: requests
 Requires-Dist: botocore
 Requires-Dist: retrying
 Provides-Extra: test
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: tzlocal; extra == "test"
```

### Comparing `fixinventory_plugin_digitalocean-4.0.4/fix_plugin_digitalocean/__init__.py` & `fixinventory_plugin_digitalocean-4.0.5/fix_plugin_digitalocean/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/fix_plugin_digitalocean/client.py` & `fixinventory_plugin_digitalocean-4.0.5/fix_plugin_digitalocean/client.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/fix_plugin_digitalocean/collector.py` & `fixinventory_plugin_digitalocean-4.0.5/fix_plugin_digitalocean/collector.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/fix_plugin_digitalocean/config.py` & `fixinventory_plugin_digitalocean-4.0.5/fix_plugin_digitalocean/config.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/fix_plugin_digitalocean/resources.py` & `fixinventory_plugin_digitalocean-4.0.5/fix_plugin_digitalocean/resources.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/fix_plugin_digitalocean/utils.py` & `fixinventory_plugin_digitalocean-4.0.5/fix_plugin_digitalocean/utils.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/fixinventory_plugin_digitalocean.egg-info/PKG-INFO` & `fixinventory_plugin_digitalocean-4.0.5/fixinventory_plugin_digitalocean.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-digitalocean
-Version: 4.0.4
+Version: 4.0.5
 Summary: Fix DigitalOcean Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/digitalocean
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.4
+Requires-Dist: fixinventorylib==4.0.5
 Requires-Dist: boto3
 Requires-Dist: requests
 Requires-Dist: botocore
 Requires-Dist: retrying
 Provides-Extra: test
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: tzlocal; extra == "test"
```

### Comparing `fixinventory_plugin_digitalocean-4.0.4/fixinventory_plugin_digitalocean.egg-info/SOURCES.txt` & `fixinventory_plugin_digitalocean-4.0.5/fixinventory_plugin_digitalocean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/pyproject.toml` & `fixinventory_plugin_digitalocean-4.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fixinventory-plugin-digitalocean"
 description = "Fix DigitalOcean Collector Plugin"
-version = "4.0.4"
+version = "4.0.5"
 authors = [{name="Some Engineering Inc."}]
 license = { text="AGPLv3" }
 requires-python = ">=3.11"
 classifiers = [
     # Current project status
     "Development Status :: 5 - Production/Stable",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "fixinventorylib==4.0.4",
+    "fixinventorylib==4.0.5",
     "boto3",
     "requests",
     "botocore",
     "retrying"
 ]
 
 [project.optional-dependencies]
```

### Comparing `fixinventory_plugin_digitalocean-4.0.4/test/fixtures/__init__.py` & `fixinventory_plugin_digitalocean-4.0.5/test/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/test/fixtures/apps.py` & `fixinventory_plugin_digitalocean-4.0.5/test/fixtures/apps.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/test/fixtures/cpu_metrics.py` & `fixinventory_plugin_digitalocean-4.0.5/test/fixtures/cpu_metrics.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/test/fixtures/databases.py` & `fixinventory_plugin_digitalocean-4.0.5/test/fixtures/databases.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/test/fixtures/domain_records.py` & `fixinventory_plugin_digitalocean-4.0.5/test/fixtures/domain_records.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/test/fixtures/droplets.py` & `fixinventory_plugin_digitalocean-4.0.5/test/fixtures/droplets.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/test/fixtures/firewalls.py` & `fixinventory_plugin_digitalocean-4.0.5/test/fixtures/firewalls.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/test/fixtures/floatingip.py` & `fixinventory_plugin_digitalocean-4.0.5/test/fixtures/floatingip.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/test/fixtures/k8s.py` & `fixinventory_plugin_digitalocean-4.0.5/test/fixtures/k8s.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/test/fixtures/loadbalancers.py` & `fixinventory_plugin_digitalocean-4.0.5/test/fixtures/loadbalancers.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/test/fixtures/memory_available.py` & `fixinventory_plugin_digitalocean-4.0.5/test/fixtures/memory_available.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/test/fixtures/projectresources.py` & `fixinventory_plugin_digitalocean-4.0.5/test/fixtures/projectresources.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/test/fixtures/projects.py` & `fixinventory_plugin_digitalocean-4.0.5/test/fixtures/projects.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/test/fixtures/regions.py` & `fixinventory_plugin_digitalocean-4.0.5/test/fixtures/regions.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/test/fixtures/registry_repositories.py` & `fixinventory_plugin_digitalocean-4.0.5/test/fixtures/registry_repositories.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/test/fixtures/tags.py` & `fixinventory_plugin_digitalocean-4.0.5/test/fixtures/tags.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/test/fixtures/volumes.py` & `fixinventory_plugin_digitalocean-4.0.5/test/fixtures/volumes.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_digitalocean-4.0.4/test/test_collector.py` & `fixinventory_plugin_digitalocean-4.0.5/test/test_collector.py`

 * *Files identical despite different names*

