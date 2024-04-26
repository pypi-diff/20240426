# Comparing `tmp/prefect_slack-0.2.3.tar.gz` & `tmp/prefect_slack-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_slack-0.2.3.tar", last modified: Thu Apr 25 19:20:18 2024, max compression
+gzip compressed data, was "prefect_slack-0.2.4.tar", last modified: Fri Apr 26 15:04:08 2024, max compression
```

## Comparing `prefect_slack-0.2.3.tar` & `prefect_slack-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:18.037281 prefect_slack-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-25 19:20:18.037281 prefect_slack-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-25 19:20:04.000000 prefect_slack-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:18.033281 prefect_slack-0.2.3/prefect_slack/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 19:20:04.000000 prefect_slack-0.2.3/prefect_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:17.000000 prefect_slack-0.2.3/prefect_slack/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-25 19:20:04.000000 prefect_slack-0.2.3/prefect_slack/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-25 19:20:04.000000 prefect_slack-0.2.3/prefect_slack/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:18.037281 prefect_slack-0.2.3/prefect_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-25 19:20:17.000000 prefect_slack-0.2.3/prefect_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-25 19:20:18.000000 prefect_slack-0.2.3/prefect_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:17.000000 prefect_slack-0.2.3/prefect_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 19:20:17.000000 prefect_slack-0.2.3/prefect_slack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-25 19:20:17.000000 prefect_slack-0.2.3/prefect_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 19:20:17.000000 prefect_slack-0.2.3/prefect_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-25 19:20:04.000000 prefect_slack-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:18.037281 prefect_slack-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:18.037281 prefect_slack-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-25 19:20:04.000000 prefect_slack-0.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-25 19:20:04.000000 prefect_slack-0.2.3/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-25 19:20:04.000000 prefect_slack-0.2.3/tests/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-25 19:20:04.000000 prefect_slack-0.2.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:08.386895 prefect_slack-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-26 15:04:08.386895 prefect_slack-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:08.382895 prefect_slack-0.2.4/prefect_slack/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/prefect_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:04:08.000000 prefect_slack-0.2.4/prefect_slack/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/prefect_slack/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/prefect_slack/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:08.386895 prefect_slack-0.2.4/prefect_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-26 15:04:08.000000 prefect_slack-0.2.4/prefect_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-26 15:04:08.000000 prefect_slack-0.2.4/prefect_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:04:08.000000 prefect_slack-0.2.4/prefect_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 15:04:08.000000 prefect_slack-0.2.4/prefect_slack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-26 15:04:08.000000 prefect_slack-0.2.4/prefect_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 15:04:08.000000 prefect_slack-0.2.4/prefect_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:04:08.386895 prefect_slack-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:08.386895 prefect_slack-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/tests/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/tests/test_version.py
```

### Comparing `prefect_slack-0.2.3/PKG-INFO` & `prefect_slack-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-slack
-Version: 0.2.3
+Version: 0.2.4
 Summary: Prefect integrations with Slack
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-slack
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: slack_sdk>=3.15.1
 Requires-Dist: prefect>=2.14.10
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
```

### Comparing `prefect_slack-0.2.3/README.md` & `prefect_slack-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `prefect_slack-0.2.3/prefect_slack/credentials.py` & `prefect_slack-0.2.4/prefect_slack/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_slack-0.2.3/prefect_slack/messages.py` & `prefect_slack-0.2.4/prefect_slack/messages.py`

 * *Files identical despite different names*

### Comparing `prefect_slack-0.2.3/prefect_slack.egg-info/PKG-INFO` & `prefect_slack-0.2.4/prefect_slack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-slack
-Version: 0.2.3
+Version: 0.2.4
 Summary: Prefect integrations with Slack
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-slack
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: slack_sdk>=3.15.1
 Requires-Dist: prefect>=2.14.10
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
```

### Comparing `prefect_slack-0.2.3/pyproject.toml` & `prefect_slack-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefect_slack-0.2.3/tests/conftest.py` & `prefect_slack-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prefect_slack-0.2.3/tests/test_messages.py` & `prefect_slack-0.2.4/tests/test_messages.py`

 * *Files identical despite different names*

