# Comparing `tmp/prefect_email-0.3.3.tar.gz` & `tmp/prefect_email-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_email-0.3.3.tar", last modified: Thu Apr 25 19:20:27 2024, max compression
+gzip compressed data, was "prefect_email-0.3.4.tar", last modified: Fri Apr 26 15:04:06 2024, max compression
```

## Comparing `prefect_email-0.3.3.tar` & `prefect_email-0.3.4.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:27.354595 prefect_email-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-25 19:20:27.354595 prefect_email-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-25 19:20:13.000000 prefect_email-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:27.350595 prefect_email-0.3.3/prefect_email/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-25 19:20:13.000000 prefect_email-0.3.3/prefect_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:26.000000 prefect_email-0.3.3/prefect_email/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-04-25 19:20:13.000000 prefect_email-0.3.3/prefect_email/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-25 19:20:13.000000 prefect_email-0.3.3/prefect_email/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:27.354595 prefect_email-0.3.3/prefect_email.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-25 19:20:27.000000 prefect_email-0.3.3/prefect_email.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-25 19:20:27.000000 prefect_email-0.3.3/prefect_email.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:27.000000 prefect_email-0.3.3/prefect_email.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 19:20:27.000000 prefect_email-0.3.3/prefect_email.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-25 19:20:27.000000 prefect_email-0.3.3/prefect_email.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 19:20:27.000000 prefect_email-0.3.3/prefect_email.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-25 19:20:13.000000 prefect_email-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:27.354595 prefect_email-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:27.354595 prefect_email-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 19:20:13.000000 prefect_email-0.3.3/tests/attachment.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-25 19:20:13.000000 prefect_email-0.3.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-25 19:20:13.000000 prefect_email-0.3.3/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-25 19:20:13.000000 prefect_email-0.3.3/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-25 19:20:13.000000 prefect_email-0.3.3/tests/test_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-25 19:20:13.000000 prefect_email-0.3.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:06.194027 prefect_email-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:50.000000 prefect_email-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:50.000000 prefect_email-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-04-26 15:04:06.194027 prefect_email-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-26 15:03:50.000000 prefect_email-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:06.190027 prefect_email-0.3.4/prefect_email/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-26 15:03:50.000000 prefect_email-0.3.4/prefect_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:04:05.000000 prefect_email-0.3.4/prefect_email/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-04-26 15:03:50.000000 prefect_email-0.3.4/prefect_email/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-26 15:03:50.000000 prefect_email-0.3.4/prefect_email/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:06.190027 prefect_email-0.3.4/prefect_email.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-04-26 15:04:05.000000 prefect_email-0.3.4/prefect_email.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-26 15:04:06.000000 prefect_email-0.3.4/prefect_email.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:04:05.000000 prefect_email-0.3.4/prefect_email.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 15:04:05.000000 prefect_email-0.3.4/prefect_email.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-26 15:04:05.000000 prefect_email-0.3.4/prefect_email.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 15:04:05.000000 prefect_email-0.3.4/prefect_email.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-26 15:03:50.000000 prefect_email-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:04:06.194027 prefect_email-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:06.190027 prefect_email-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 15:03:50.000000 prefect_email-0.3.4/tests/attachment.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-26 15:03:50.000000 prefect_email-0.3.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-26 15:03:50.000000 prefect_email-0.3.4/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-26 15:03:50.000000 prefect_email-0.3.4/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-26 15:03:50.000000 prefect_email-0.3.4/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-26 15:03:50.000000 prefect_email-0.3.4/tests/test_version.py
```

### Comparing `prefect_email-0.3.3/PKG-INFO` & `prefect_email-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-email
-Version: 0.3.3
+Version: 0.3.4
 Summary: Prefect integrations for interacting with email.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-email
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
 Requires-Dist: prefect>=2.14.10
 Provides-Extra: dev
 Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
```

### Comparing `prefect_email-0.3.3/README.md` & `prefect_email-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `prefect_email-0.3.3/prefect_email/credentials.py` & `prefect_email-0.3.4/prefect_email/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_email-0.3.3/prefect_email/message.py` & `prefect_email-0.3.4/prefect_email/message.py`

 * *Files identical despite different names*

### Comparing `prefect_email-0.3.3/prefect_email.egg-info/PKG-INFO` & `prefect_email-0.3.4/prefect_email.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-email
-Version: 0.3.3
+Version: 0.3.4
 Summary: Prefect integrations for interacting with email.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-email
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
 Requires-Dist: prefect>=2.14.10
 Provides-Extra: dev
 Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
```

### Comparing `prefect_email-0.3.3/pyproject.toml` & `prefect_email-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefect_email-0.3.3/tests/conftest.py` & `prefect_email-0.3.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prefect_email-0.3.3/tests/test_block_standards.py` & `prefect_email-0.3.4/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_email-0.3.3/tests/test_credentials.py` & `prefect_email-0.3.4/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_email-0.3.3/tests/test_message.py` & `prefect_email-0.3.4/tests/test_message.py`

 * *Files identical despite different names*

