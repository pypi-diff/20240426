# Comparing `tmp/prefect_shell-0.2.3.tar.gz` & `tmp/prefect_shell-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_shell-0.2.3.tar", last modified: Thu Apr 25 15:15:08 2024, max compression
+gzip compressed data, was "prefect_shell-0.2.4.tar", last modified: Fri Apr 26 15:04:12 2024, max compression
```

## Comparing `prefect_shell-0.2.3.tar` & `prefect_shell-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:08.558530 prefect_shell-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-04-25 15:15:08.558530 prefect_shell-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:08.554530 prefect_shell-0.2.3/prefect_shell/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/prefect_shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 15:15:08.000000 prefect_shell-0.2.3/prefect_shell/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    15327 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/prefect_shell/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:08.558530 prefect_shell-0.2.3/prefect_shell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-04-25 15:15:08.000000 prefect_shell-0.2.3/prefect_shell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-25 15:15:08.000000 prefect_shell-0.2.3/prefect_shell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:15:08.000000 prefect_shell-0.2.3/prefect_shell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 15:15:08.000000 prefect_shell-0.2.3/prefect_shell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-25 15:15:08.000000 prefect_shell-0.2.3/prefect_shell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 15:15:08.000000 prefect_shell-0.2.3/prefect_shell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:15:08.558530 prefect_shell-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:08.554530 prefect_shell-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/tests/test_commands_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:12.089886 prefect_shell-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8579 2024-04-26 15:04:12.089886 prefect_shell-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:12.085886 prefect_shell-0.2.4/prefect_shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/prefect_shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:04:11.000000 prefect_shell-0.2.4/prefect_shell/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15327 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/prefect_shell/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:12.089886 prefect_shell-0.2.4/prefect_shell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8579 2024-04-26 15:04:11.000000 prefect_shell-0.2.4/prefect_shell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 15:04:12.000000 prefect_shell-0.2.4/prefect_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:04:11.000000 prefect_shell-0.2.4/prefect_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 15:04:11.000000 prefect_shell-0.2.4/prefect_shell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-26 15:04:11.000000 prefect_shell-0.2.4/prefect_shell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 15:04:11.000000 prefect_shell-0.2.4/prefect_shell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:04:12.089886 prefect_shell-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:12.089886 prefect_shell-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/tests/test_commands_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/tests/test_version.py
```

### Comparing `prefect_shell-0.2.3/PKG-INFO` & `prefect_shell-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-shell
-Version: 0.2.3
+Version: 0.2.4
 Summary: Prefect integrations for interacting with shell commands.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-shell
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

### Comparing `prefect_shell-0.2.3/README.md` & `prefect_shell-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `prefect_shell-0.2.3/prefect_shell/commands.py` & `prefect_shell-0.2.4/prefect_shell/commands.py`

 * *Files identical despite different names*

### Comparing `prefect_shell-0.2.3/prefect_shell.egg-info/PKG-INFO` & `prefect_shell-0.2.4/prefect_shell.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-shell
-Version: 0.2.3
+Version: 0.2.4
 Summary: Prefect integrations for interacting with shell commands.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-shell
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

### Comparing `prefect_shell-0.2.3/pyproject.toml` & `prefect_shell-0.2.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,35 +3,31 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-shell"
 description = "Prefect integrations for interacting with shell commands."
 readme = "README.md"
 requires-python = ">=3.8"
-license = {text = "Apache License 2.0"}
+license = { text = "Apache License 2.0" }
 keywords = ["prefect"]
-authors = [
-  {name = "Prefect Technologies, Inc.", email = "help@prefect.io"}
-]
+authors = [{ name = "Prefect Technologies, Inc.", email = "help@prefect.io" }]
 classifiers = [
   "Natural Language :: English",
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
 ]
-dependencies = [
-  "prefect>=2.14.10",
-]
+dependencies = ["prefect>=2.14.10"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
   "aiohttp",
   "coverage",
   "interrogate",
@@ -54,15 +50,15 @@
 [project.entry-points."prefect.collections"]
 prefect_shell = "prefect_shell"
 
 [tool.setuptools_scm]
 version_file = "prefect_shell/_version.py"
 root = "../../.."
 tag_regex = "^prefect-shell-(?P<version>\\d+\\.\\d+\\.\\d+)$"
-fallback_version = "0.0.0"
+fallback_version = "0.2.0"
 git_describe_command = 'git describe --dirty --tags --long --match "prefect-shell-*[0-9]*"'
 
 [tool.interrogate]
 ignore-init-module = true
 ignore_init_method = true
 exclude = ["prefect_shell/_version.py", "tests"]
 fail-under = 95
@@ -72,8 +68,8 @@
 omit = ["tests/*", "prefect_shell/_version.py"]
 
 [tool.coverage.report]
 fail_under = 80
 show_missing = true
 
 [tool.pytest.ini_options]
-asyncio_mode = "auto"
+asyncio_mode = "auto"
```

### Comparing `prefect_shell-0.2.3/tests/conftest.py` & `prefect_shell-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prefect_shell-0.2.3/tests/test_block_standards.py` & `prefect_shell-0.2.4/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_shell-0.2.3/tests/test_commands.py` & `prefect_shell-0.2.4/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `prefect_shell-0.2.3/tests/test_commands_windows.py` & `prefect_shell-0.2.4/tests/test_commands_windows.py`

 * *Files identical despite different names*

