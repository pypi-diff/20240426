# Comparing `tmp/fixinventory_plugin_slack-4.0.4.tar.gz` & `tmp/fixinventory_plugin_slack-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory_plugin_slack-4.0.4.tar", last modified: Wed Apr 24 19:34:40 2024, max compression
+gzip compressed data, was "fixinventory_plugin_slack-4.0.5.tar", last modified: Fri Apr 26 20:24:23 2024, max compression
```

## Comparing `fixinventory_plugin_slack-4.0.4.tar` & `fixinventory_plugin_slack-4.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:34:40.503594 fixinventory_plugin_slack-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 19:31:48.000000 fixinventory_plugin_slack-4.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-24 19:34:40.503594 fixinventory_plugin_slack-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 19:31:48.000000 fixinventory_plugin_slack-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:34:40.499594 fixinventory_plugin_slack-4.0.4/fix_plugin_slack/
--rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-04-24 19:31:48.000000 fixinventory_plugin_slack-4.0.4/fix_plugin_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-24 19:31:48.000000 fixinventory_plugin_slack-4.0.4/fix_plugin_slack/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-24 19:31:48.000000 fixinventory_plugin_slack-4.0.4/fix_plugin_slack/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:34:40.499594 fixinventory_plugin_slack-4.0.4/fixinventory_plugin_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-24 19:34:40.000000 fixinventory_plugin_slack-4.0.4/fixinventory_plugin_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-24 19:34:40.000000 fixinventory_plugin_slack-4.0.4/fixinventory_plugin_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:34:40.000000 fixinventory_plugin_slack-4.0.4/fixinventory_plugin_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-24 19:34:40.000000 fixinventory_plugin_slack-4.0.4/fixinventory_plugin_slack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:32:53.000000 fixinventory_plugin_slack-4.0.4/fixinventory_plugin_slack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 19:34:40.000000 fixinventory_plugin_slack-4.0.4/fixinventory_plugin_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 19:34:40.000000 fixinventory_plugin_slack-4.0.4/fixinventory_plugin_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-24 19:31:48.000000 fixinventory_plugin_slack-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 19:34:40.503594 fixinventory_plugin_slack-4.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:34:40.499594 fixinventory_plugin_slack-4.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-24 19:31:48.000000 fixinventory_plugin_slack-4.0.4/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:24:23.606320 fixinventory_plugin_slack-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 20:21:16.000000 fixinventory_plugin_slack-4.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-26 20:24:23.606320 fixinventory_plugin_slack-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-26 20:21:16.000000 fixinventory_plugin_slack-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:24:23.606320 fixinventory_plugin_slack-4.0.5/fix_plugin_slack/
+-rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-04-26 20:21:16.000000 fixinventory_plugin_slack-4.0.5/fix_plugin_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-26 20:21:16.000000 fixinventory_plugin_slack-4.0.5/fix_plugin_slack/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-26 20:21:16.000000 fixinventory_plugin_slack-4.0.5/fix_plugin_slack/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:24:23.606320 fixinventory_plugin_slack-4.0.5/fixinventory_plugin_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-26 20:24:23.000000 fixinventory_plugin_slack-4.0.5/fixinventory_plugin_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-26 20:24:23.000000 fixinventory_plugin_slack-4.0.5/fixinventory_plugin_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:24:23.000000 fixinventory_plugin_slack-4.0.5/fixinventory_plugin_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-26 20:24:23.000000 fixinventory_plugin_slack-4.0.5/fixinventory_plugin_slack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:22:29.000000 fixinventory_plugin_slack-4.0.5/fixinventory_plugin_slack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 20:24:23.000000 fixinventory_plugin_slack-4.0.5/fixinventory_plugin_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 20:24:23.000000 fixinventory_plugin_slack-4.0.5/fixinventory_plugin_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-26 20:21:16.000000 fixinventory_plugin_slack-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-26 20:24:23.606320 fixinventory_plugin_slack-4.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:24:23.606320 fixinventory_plugin_slack-4.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-26 20:21:16.000000 fixinventory_plugin_slack-4.0.5/test/test_config.py
```

### Comparing `fixinventory_plugin_slack-4.0.4/PKG-INFO` & `fixinventory_plugin_slack-4.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-slack
-Version: 4.0.4
+Version: 4.0.5
 Summary: Fix Slack Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/slack
 Classifier: Development Status :: 4 - Beta
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
 Requires-Dist: slack-sdk
 Requires-Dist: retrying
 
 # fix-plugin-slack
 Slack collector for Fix
 
 ## License
```

### Comparing `fixinventory_plugin_slack-4.0.4/fix_plugin_slack/__init__.py` & `fixinventory_plugin_slack-4.0.5/fix_plugin_slack/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_slack-4.0.4/fix_plugin_slack/resources.py` & `fixinventory_plugin_slack-4.0.5/fix_plugin_slack/resources.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_slack-4.0.4/fixinventory_plugin_slack.egg-info/PKG-INFO` & `fixinventory_plugin_slack-4.0.5/fixinventory_plugin_slack.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-slack
-Version: 4.0.4
+Version: 4.0.5
 Summary: Fix Slack Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/slack
 Classifier: Development Status :: 4 - Beta
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
 Requires-Dist: slack-sdk
 Requires-Dist: retrying
 
 # fix-plugin-slack
 Slack collector for Fix
 
 ## License
```

### Comparing `fixinventory_plugin_slack-4.0.4/pyproject.toml` & `fixinventory_plugin_slack-4.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fixinventory-plugin-slack"
 description = "Fix Slack Plugin"
-version = "4.0.4"
+version = "4.0.5"
 authors = [{name="Some Engineering Inc."}]
 license = { text="AGPLv3" }
 requires-python = ">=3.11"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
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
     "slack-sdk",
     "retrying",
 ]
 
 [project.entry-points."fix.plugins"]
 slack_bot = "fix_plugin_slack:SlackBotPlugin"
 slack_collector = "fix_plugin_slack:SlackCollectorPlugin"
```

